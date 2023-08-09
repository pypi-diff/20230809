# Comparing `tmp/apit212-1.0.4.tar.gz` & `tmp/apit212-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apit212-1.0.4.tar", last modified: Mon Aug  7 03:23:46 2023, max compression
+gzip compressed data, was "apit212-1.0.5.tar", last modified: Wed Aug  9 00:01:24 2023, max compression
```

## Comparing `apit212-1.0.4.tar` & `apit212-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 03:23:46.485903 apit212-1.0.4/
--rw-rw-rw-   0        0        0     1083 2023-07-05 18:54:25.000000 apit212-1.0.4/LICENSE
--rw-rw-rw-   0        0        0    11137 2023-08-07 03:23:46.484454 apit212-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0    10370 2023-08-07 03:22:14.000000 apit212-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-08-07 03:23:46.443155 apit212-1.0.4/apit212/
--rw-rw-rw-   0        0        0    46709 2023-08-07 03:23:06.000000 apit212-1.0.4/apit212/Apit212.py
--rw-rw-rw-   0        0        0       98 2023-07-05 18:54:13.000000 apit212-1.0.4/apit212/__init__.py
--rw-rw-rw-   0        0        0     1254 2023-08-05 10:09:12.000000 apit212-1.0.4/apit212/apitconstant.py
--rw-rw-rw-   0        0        0     4884 2023-07-28 08:42:03.000000 apit212-1.0.4/apit212/cfdScrape.py
-drwxrwxrwx   0        0        0        0 2023-08-07 03:23:46.482462 apit212-1.0.4/apit212.egg-info/
--rw-rw-rw-   0        0        0    11137 2023-08-07 03:23:46.000000 apit212-1.0.4/apit212.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-08-07 03:23:46.000000 apit212-1.0.4/apit212.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 03:23:46.000000 apit212-1.0.4/apit212.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-08-07 03:23:46.000000 apit212-1.0.4/apit212.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-08-07 03:23:46.000000 apit212-1.0.4/apit212.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      839 2023-08-07 02:59:38.000000 apit212-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-07 03:23:46.488590 apit212-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      898 2023-08-07 02:59:34.000000 apit212-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-09 00:01:24.804136 apit212-1.0.5/
+-rw-rw-rw-   0        0        0     1083 2023-07-05 18:54:25.000000 apit212-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0    11137 2023-08-09 00:01:24.803629 apit212-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0    10370 2023-08-07 03:22:14.000000 apit212-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-08-09 00:01:24.756810 apit212-1.0.5/apit212/
+-rw-rw-rw-   0        0        0    47045 2023-08-09 00:00:07.000000 apit212-1.0.5/apit212/Apit212.py
+-rw-rw-rw-   0        0        0       98 2023-07-05 18:54:13.000000 apit212-1.0.5/apit212/__init__.py
+-rw-rw-rw-   0        0        0     1254 2023-08-05 10:09:12.000000 apit212-1.0.5/apit212/apitconstant.py
+-rw-rw-rw-   0        0        0     4884 2023-07-28 08:42:03.000000 apit212-1.0.5/apit212/cfdScrape.py
+drwxrwxrwx   0        0        0        0 2023-08-09 00:01:24.800377 apit212-1.0.5/apit212.egg-info/
+-rw-rw-rw-   0        0        0    11137 2023-08-09 00:01:24.000000 apit212-1.0.5/apit212.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-08-09 00:01:24.000000 apit212-1.0.5/apit212.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-09 00:01:24.000000 apit212-1.0.5/apit212.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-08-09 00:01:24.000000 apit212-1.0.5/apit212.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-09 00:01:24.000000 apit212-1.0.5/apit212.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      839 2023-08-09 00:00:27.000000 apit212-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-09 00:01:24.805146 apit212-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      898 2023-08-09 00:00:31.000000 apit212-1.0.5/setup.py
```

### Comparing `apit212-1.0.4/LICENSE` & `apit212-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `apit212-1.0.4/PKG-INFO` & `apit212-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apit212
-Version: 1.0.4
+Version: 1.0.5
 Summary: Unofficial trading212 API
 Home-page: https://github.com/Flock92/aPit212
 Author: Flock92
 Author-email: Flock92 <stuwe_3000@outlook.com>
 Maintainer-email: Flock92 <stuwe_3000@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Flock92/apit212
```

### Comparing `apit212-1.0.4/README.md` & `apit212-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `apit212-1.0.4/apit212/Apit212.py` & `apit212-1.0.5/apit212/Apit212.py`

 * *Files 0% similar despite different names*

```diff
@@ -330,15 +330,20 @@
             return {"code": "requestTimeout", "message": em}
         except requests.exceptions.HTTPError as em:
             return {"code": "HTTPError", "message": em}
         except requests.exceptions.RequestException as em:
             return {"code": "Unknown", "message": em}
         
         price = r.json()
-        result = float(price[0]["response"]["candles"][0][-2])
+        try:
+            result = float(price[0]["response"]["candles"][0][-2])
+        except IndexError as em:
+            return {"code":"indexError","response":f"{r.json}"}
+        except KeyError as em:
+            return {"code":"keyError", "response":f"{r.json}"}
 
         return result
         
     # GET CHART DATA
     def chart_data(self, instrument: str, _useaskprice: str = "false", 
                    period: str = "ONE_MINUTE", size: int = 500) -> list:
         """
@@ -403,16 +408,21 @@
         except requests.exceptions.RequestException as em:
             return {"code": "Unknown", "message": em}
         
         result = []
         data = r.json()
         
         for i in enumerate(data):
-            result.append(dict({"ticker":data[i[0]]["request"]["ticker"], "price": float(data[i[0]]["response"]["candles"][0][-2])}))
-                         
+            try:
+                result.append(dict({"ticker":data[i[0]]["request"]["ticker"], "price": float(data[i[0]]["response"]["candles"][0][-2])}))
+            except IndexError as em:
+                pass
+            except KeyError as em:
+                pass
+
         return result
 
     # GET AUTH VALIDATE
     def auth_validate(self) -> dict:
         """
         :return: {'id': '********-****-****-****-************', 'accountId': ********, 'customerId': ********,
         'tradingType': 'CFD', 'customerUuid': '********-****-****-****-************', 'frontend': 'WC4',
@@ -729,15 +739,15 @@
     # PLACE LIMIT ORDER
     def limit_order(self,
                     instrument: str,
                     quantity: float,
                     target_price: float,
                     take_profit: float,
                     stop_loss: float,
-                    notify: str = "NONE"):
+                    notify: str = "NONE") -> dict:
         """the minimum requirement to submit a limit order is the instrument, quantity and target price.
         You can also set a take_profit and stop_loss limits. I would like to point out that this
         function will only submit your order and will make no attempts to change any of the parameters.
 
         :param instrument:
         :param quantity:
         :param target_price:
```

### Comparing `apit212-1.0.4/apit212/apitconstant.py` & `apit212-1.0.5/apit212/apitconstant.py`

 * *Files identical despite different names*

### Comparing `apit212-1.0.4/apit212/cfdScrape.py` & `apit212-1.0.5/apit212/cfdScrape.py`

 * *Files identical despite different names*

### Comparing `apit212-1.0.4/apit212.egg-info/PKG-INFO` & `apit212-1.0.5/apit212.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apit212
-Version: 1.0.4
+Version: 1.0.5
 Summary: Unofficial trading212 API
 Home-page: https://github.com/Flock92/aPit212
 Author: Flock92
 Author-email: Flock92 <stuwe_3000@outlook.com>
 Maintainer-email: Flock92 <stuwe_3000@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Flock92/apit212
```

### Comparing `apit212-1.0.4/pyproject.toml` & `apit212-1.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "apit212"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
 { name= "Flock92", email= "stuwe_3000@outlook.com" },
 ]
 
 maintainers = [
   {name = "Flock92", email = "stuwe_3000@outlook.com"}
 ]
```

### Comparing `apit212-1.0.4/setup.py` & `apit212-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 long_description = """This is an unofficial API use to interact with the trading212 platform. It is still currently in
                    it's testing stages I created this API to challenge myself and also start creating a portfolio of
                    work that i can showcase to employers"""
 
 setup(
     name="apit212",
-    version="1.0.4",
+    version="1.0.5",
     packages=find_packages(),
     requires=[
         'requests',
         'selenium',
     ],
     author="Flock92",
     author_email="stuwe_3000@outlook.com",
```

