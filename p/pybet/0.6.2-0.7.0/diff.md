# Comparing `tmp/pybet-0.6.2.tar.gz` & `tmp/pybet-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybet-0.6.2.tar", max compression
+gzip compressed data, was "pybet-0.7.0.tar", max compression
```

## Comparing `pybet-0.6.2.tar` & `pybet-0.7.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35823 2022-12-14 21:43:12.915289 pybet-0.6.2/LICENSE
--rw-r--r--   0        0        0       84 2023-02-18 00:28:56.230892 pybet-0.6.2/pybet/__init__.py
--rw-r--r--   0        0        0     8054 2023-05-04 23:05:01.296759 pybet-0.6.2/pybet/market.py
--rw-r--r--   0        0        0    11717 2023-05-08 20:37:50.564904 pybet-0.6.2/pybet/odds.py
--rw-r--r--   0        0        0       49 2023-02-18 00:28:56.233330 pybet-0.6.2/pybet/staking/__init__.py
--rw-r--r--   0        0        0     1496 2023-04-29 12:08:45.277280 pybet-0.6.2/pybet/staking/kelly.py
--rw-r--r--   0        0        0      989 2023-05-08 20:40:41.727261 pybet-0.6.2/pyproject.toml
--rw-r--r--   0        0        0      539 2023-02-18 00:28:56.218112 pybet-0.6.2/README.md
--rw-r--r--   0        0        0     1389 1970-01-01 00:00:00.000000 pybet-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0    35823 2022-12-14 21:43:12.915289 pybet-0.7.0/LICENSE
+-rw-r--r--   0        0        0       84 2023-02-18 00:28:56.230892 pybet-0.7.0/pybet/__init__.py
+-rw-r--r--   0        0        0    10336 2023-08-08 21:26:36.954848 pybet-0.7.0/pybet/market.py
+-rw-r--r--   0        0        0    11717 2023-06-12 22:15:51.544566 pybet-0.7.0/pybet/odds.py
+-rw-r--r--   0        0        0       49 2023-02-18 00:28:56.233330 pybet-0.7.0/pybet/staking/__init__.py
+-rw-r--r--   0        0        0     1496 2023-04-29 12:08:45.277280 pybet-0.7.0/pybet/staking/kelly.py
+-rw-r--r--   0        0        0     1015 2023-08-08 21:26:36.954848 pybet-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      539 2023-02-18 00:28:56.218112 pybet-0.7.0/README.md
+-rw-r--r--   0        0        0     1389 1970-01-01 00:00:00.000000 pybet-0.7.0/PKG-INFO
```

### Comparing `pybet-0.6.2/LICENSE` & `pybet-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pybet-0.6.2/pybet/market.py` & `pybet-0.7.0/pybet/market.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 from __future__ import annotations
 from decimal import Decimal
+from functools import reduce
+from itertools import permutations
+from operator import mul
 from typing import Any, List
 from .odds import Odds
 
 
 class Market(dict):
     """A betting market represented by a dictionary of runners and odds
 
@@ -114,14 +117,63 @@
         """
 
         adjustment = (100 + margin) / self.percentage
         for runner, odds in self.items():
             self[runner] = Odds(Decimal(odds) / adjustment)
         return self
 
+    def derive(self, places: int, *, discounts: List[float] | None = None) -> Market:
+        """Derives a place market from a win market using the Harville formula (see https://en.wikipedia.org/wiki/Harville_formula)
+        applying a specified discounted version of that formula if required
+
+        :param places: The number of places to derive the market for
+        :type places: int
+        :param discounts: A list of discounts to apply to the probability of each horse in the market, defaults to None
+        :type discounts: List[float], optional
+        :raises ValueError: If the number of places is invalid
+        :raises ValueError: If the market is not a win market
+        :return: A revised market with the specified number of places
+        :rtype: Market
+
+        :Example:
+            >>> market = Market({'Frankel': Odds(3), 'Sea The Stars': Odds(3), 'Nijinsky': Odds(3)})
+            >>> market.derive(2).get('Frankel')
+            Decimal('1.5')
+        """
+
+        if self.places != 1:
+            raise ValueError("Derivation only possible from win market")
+
+        if places >= len(self) or places <= 1:
+            raise ValueError("Invalid number of places")
+
+        fair_market = Market(self)
+        fair_market.apply_margin(0)
+        derived_market = Market.fromkeys(self.keys())
+        prob = lambda x: float(fair_market[x].to_probability())
+        product = lambda x: reduce(mul, x, 1)
+        prob_exponent = lambda x, y: prob(x) ** discounts[y] if discounts else prob(x)
+
+        for perm in list(permutations(self.keys(), places)):
+            denominator = product([prob_exponent(h, i) for i, h in enumerate(perm)])
+            numerator = product(
+                [
+                    sum(prob_exponent(h, i) for h in self.keys() if h not in perm[:i])
+                    for i, _ in enumerate(perm)
+                ]
+            )
+            perm_probability = denominator / numerator
+
+            for horse in perm:
+                derived_market[horse] = (derived_market[horse] or 0) + Odds.probability(
+                    perm_probability
+                )
+
+        return derived_market
+
     def equalise(self) -> Market:
         """Resets a market so that all runners have equal odds with no overround
 
         :return: A revised market with no margin built in
         :rtype: Market
 
         :Example:
```

### Comparing `pybet-0.6.2/pybet/odds.py` & `pybet-0.7.0/pybet/odds.py`

 * *Files identical despite different names*

### Comparing `pybet-0.6.2/pybet/staking/kelly.py` & `pybet-0.7.0/pybet/staking/kelly.py`

 * *Files identical despite different names*

### Comparing `pybet-0.6.2/pyproject.toml` & `pybet-0.7.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybet"
-version = "0.6.2"
+version = "0.7.0"
 description = "A library of betting utilities to assist with calculation of bets, stakes and markets"
 license = "GPL-3.0-only"
 authors = ["Robert Peacock <robertjamespeacock@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/peaky76/pybet"
 documentation = "https://pybet.readthedocs.io/"
 keywords = ["betting", "gambling"]
@@ -20,18 +20,18 @@
 [tool.poetry.group.dev.dependencies]
 auto-changelog = "^0.6.0"
 black = "^23.1.0"
 coverage = "^7.1.0"
 mypy = "^1.0.1"
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
-ruff = "^0.0.265"
-sphinx = "^6.1.3"
+ruff = ">=0.0.265,<0.0.283"
+sphinx = ">=6.1.3,<8.0.0"
 sphinx-rtd-theme = "^1.2.0"
 
 [tool.ruff]
-ignore = ["E501"]
+ignore = ["E501", "F821"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pybet-0.6.2/README.md` & `pybet-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pybet-0.6.2/PKG-INFO` & `pybet-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybet
-Version: 0.6.2
+Version: 0.7.0
 Summary: A library of betting utilities to assist with calculation of bets, stakes and markets
 Home-page: https://github.com/peaky76/pybet
 License: GPL-3.0-only
 Keywords: betting,gambling
 Author: Robert Peacock
 Author-email: robertjamespeacock@gmail.com
 Requires-Python: >=3.9.0,<4.0.0
```

