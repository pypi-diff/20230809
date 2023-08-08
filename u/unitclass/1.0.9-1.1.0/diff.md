# Comparing `tmp/unitclass-1.0.9.tar.gz` & `tmp/unitclass-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitclass-1.0.9.tar", last modified: Thu Aug  3 20:45:07 2023, max compression
+gzip compressed data, was "unitclass-1.1.0.tar", last modified: Tue Aug  8 23:49:25 2023, max compression
```

## Comparing `unitclass-1.0.9.tar` & `unitclass-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 blake      (501) staff       (20)        0 2023-08-03 20:45:07.965579 unitclass-1.0.9/
--rw-r--r--   0 blake      (501) staff       (20)    35149 2023-01-29 20:27:25.000000 unitclass-1.0.9/LICENSE
--rw-r--r--   0 blake      (501) staff       (20)     7249 2023-08-03 20:45:07.965448 unitclass-1.0.9/PKG-INFO
--rw-r--r--   0 blake      (501) staff       (20)     6480 2023-07-17 21:47:14.000000 unitclass-1.0.9/README.md
--rw-r--r--   0 blake      (501) staff       (20)      852 2023-08-03 20:44:25.000000 unitclass-1.0.9/pyproject.toml
--rw-r--r--   0 blake      (501) staff       (20)       38 2023-08-03 20:45:07.965613 unitclass-1.0.9/setup.cfg
-drwxr-xr-x   0 blake      (501) staff       (20)        0 2023-08-03 20:45:07.965281 unitclass-1.0.9/unitclass.egg-info/
--rw-r--r--   0 blake      (501) staff       (20)     7249 2023-08-03 20:45:07.000000 unitclass-1.0.9/unitclass.egg-info/PKG-INFO
--rw-r--r--   0 blake      (501) staff       (20)      177 2023-08-03 20:45:07.000000 unitclass-1.0.9/unitclass.egg-info/SOURCES.txt
--rw-r--r--   0 blake      (501) staff       (20)        1 2023-08-03 20:45:07.000000 unitclass-1.0.9/unitclass.egg-info/dependency_links.txt
--rw-r--r--   0 blake      (501) staff       (20)       10 2023-08-03 20:45:07.000000 unitclass-1.0.9/unitclass.egg-info/top_level.txt
--rw-r--r--   0 blake      (501) staff       (20)    48315 2023-08-03 20:44:08.000000 unitclass-1.0.9/unitclass.py
+drwxr-xr-x   0 blake      (501) staff       (20)        0 2023-08-08 23:49:25.054448 unitclass-1.1.0/
+-rw-r--r--   0 blake      (501) staff       (20)    35149 2023-01-29 20:27:25.000000 unitclass-1.1.0/LICENSE
+-rw-r--r--   0 blake      (501) staff       (20)     7249 2023-08-08 23:49:25.054308 unitclass-1.1.0/PKG-INFO
+-rw-r--r--   0 blake      (501) staff       (20)     6480 2023-07-17 21:47:14.000000 unitclass-1.1.0/README.md
+-rw-r--r--   0 blake      (501) staff       (20)      852 2023-08-08 23:49:02.000000 unitclass-1.1.0/pyproject.toml
+-rw-r--r--   0 blake      (501) staff       (20)       38 2023-08-08 23:49:25.054485 unitclass-1.1.0/setup.cfg
+drwxr-xr-x   0 blake      (501) staff       (20)        0 2023-08-08 23:49:25.054137 unitclass-1.1.0/unitclass.egg-info/
+-rw-r--r--   0 blake      (501) staff       (20)     7249 2023-08-08 23:49:25.000000 unitclass-1.1.0/unitclass.egg-info/PKG-INFO
+-rw-r--r--   0 blake      (501) staff       (20)      177 2023-08-08 23:49:25.000000 unitclass-1.1.0/unitclass.egg-info/SOURCES.txt
+-rw-r--r--   0 blake      (501) staff       (20)        1 2023-08-08 23:49:25.000000 unitclass-1.1.0/unitclass.egg-info/dependency_links.txt
+-rw-r--r--   0 blake      (501) staff       (20)       10 2023-08-08 23:49:25.000000 unitclass-1.1.0/unitclass.egg-info/top_level.txt
+-rw-r--r--   0 blake      (501) staff       (20)    48475 2023-08-08 21:57:17.000000 unitclass-1.1.0/unitclass.py
```

### Comparing `unitclass-1.0.9/LICENSE` & `unitclass-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unitclass-1.0.9/PKG-INFO` & `unitclass-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitclass
-Version: 1.0.9
+Version: 1.1.0
 Summary: Physical unit class suitable for calculations in the sciences.
 Author-email: Blake Garretson <blake@blakeg.net>
 Project-URL: Homepage, https://github.com/blakegarretson/unitclass
 Project-URL: Bug Tracker, https://github.com/blakegarretson/unitclass/issues
 Keywords: unit,units,SI,conversion
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `unitclass-1.0.9/README.md` & `unitclass-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `unitclass-1.0.9/pyproject.toml` & `unitclass-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "unitclass"
-version = "1.0.9"
+version = "1.1.0"
 authors = [
   { name="Blake Garretson", email="blake@blakeg.net" },
 ]
 description = "Physical unit class suitable for calculations in the sciences."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `unitclass-1.0.9/unitclass.egg-info/PKG-INFO` & `unitclass-1.1.0/unitclass.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitclass
-Version: 1.0.9
+Version: 1.1.0
 Summary: Physical unit class suitable for calculations in the sciences.
 Author-email: Blake Garretson <blake@blakeg.net>
 Project-URL: Homepage, https://github.com/blakegarretson/unitclass
 Project-URL: Bug Tracker, https://github.com/blakegarretson/unitclass/issues
 Keywords: unit,units,SI,conversion
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `unitclass-1.0.9/unitclass.py` & `unitclass-1.1.0/unitclass.py`

 * *Files 0% similar despite different names*

```diff
@@ -293,14 +293,15 @@
     ('data', 'KB', 'kilobyte kilobytes', 1024, 'B'),
     ('data', 'MB', 'megabyte megabytes', 1024, 'KB'),
     ('data', 'GB', 'gigabyte gigabytes', 1024, 'MB'),
     ('data', 'TB', 'terabyte terabytes', 1024, 'GB'),
     ('data', 'PB', 'petabyte petabytes', 1024, 'TB'),
     ('data', 'EB', 'exabyte exabytes', 1024, 'PB'),
     ('currency', 'USD', 'dollars dollar usdollar', 1, ''),
+    ('currency', 'cents', 'cent', 0.01, 'USD'),
     ('currency', 'pennies', 'penny', 0.01, 'USD'),
     ('currency', 'nickels', 'nickel', 0.05, 'USD'),
     ('currency', 'dimes', 'dime', 0.10, 'USD'),
     ('currency', 'quarters', 'quarter', 0.25, 'USD'),
     ('speed', 'mph', 'mileperhour', 1, 'mi/hr'),
     ('speed', 'kph', 'kmperhour', 1, 'km/hr'),
     ('speed', 'c', 'lightspeed', 299792458, 'm/s'),
@@ -1000,15 +1001,16 @@
 
     def __format__(self, format_spec='g'):
         unit_str = self.unit.translate(self.to_specials)
         prefix = ''
         if 'USD' in unit_str:
             prefix = '$'
             unit_str = unit_str.replace('USD', '')
-            format_spec = '.2f'
+            if 'g' in format_spec: # format money to 2 decimals unless a specific fixed format is requested
+                format_spec = '.2f'
         number = "{r:{f}}".format(r=self.value, f=format_spec)
         if unit_str and (unit_str in no_space_units): 
             space = ''
         else:
             space = ' '
         return "{}{}{}{}".format(prefix, number, space, unit_str).strip()
```

