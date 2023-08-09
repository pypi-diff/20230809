# Comparing `tmp/problem_bank_helpers-0.2.0.tar.gz` & `tmp/problem_bank_helpers-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "problem_bank_helpers-0.2.0.tar", max compression
+gzip compressed data, was "problem_bank_helpers-0.2.1.tar", max compression
```

## Comparing `problem_bank_helpers-0.2.0.tar` & `problem_bank_helpers-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rwxr-xr-x   0        0        0        1 2021-06-14 01:41:43.016309 problem_bank_helpers-0.2.0/LICENSE
--rw-r--r--   0        0        0     1244 2021-06-14 01:41:43.033405 problem_bank_helpers-0.2.0/README.md
--rw-r--r--   0        0        0       44 2023-06-30 00:13:15.868563 problem_bank_helpers-0.2.0/data/animals.csv
--rw-r--r--   0        0        0        0 2023-07-26 04:00:06.482196 problem_bank_helpers-0.2.0/data/empty.csv
--rw-r--r--   0        0        0       61 2023-06-30 00:13:15.869185 problem_bank_helpers-0.2.0/data/jumpers.csv
--rw-r--r--   0        0        0       84 2023-06-30 00:13:15.869706 problem_bank_helpers-0.2.0/data/manual_vehicles.csv
--rw-r--r--   0        0        0      248 2023-06-30 00:13:15.870015 problem_bank_helpers-0.2.0/data/metals.csv
--rw-r--r--   0        0        0       75 2023-06-30 00:13:15.870268 problem_bank_helpers-0.2.0/data/names.csv
--rw-r--r--   0        0        0       56 2023-06-30 00:13:15.870498 problem_bank_helpers-0.2.0/data/vehicles.csv
--rw-r--r--   0        0        0      716 2023-07-26 03:56:04.969547 problem_bank_helpers-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       59 2023-07-26 03:57:08.453361 problem_bank_helpers-0.2.0/src/problem_bank_helpers/__init__.py
--rw-r--r--   0        0        0       44 2023-06-29 23:59:26.052387 problem_bank_helpers-0.2.0/src/problem_bank_helpers/data/animals.csv
--rw-r--r--   0        0        0       61 2023-06-29 23:59:26.052468 problem_bank_helpers-0.2.0/src/problem_bank_helpers/data/jumpers.csv
--rw-r--r--   0        0        0       84 2023-06-29 23:59:26.052539 problem_bank_helpers-0.2.0/src/problem_bank_helpers/data/manual_vehicles.csv
--rw-r--r--   0        0        0      248 2023-06-29 23:59:26.052616 problem_bank_helpers-0.2.0/src/problem_bank_helpers/data/metals.csv
--rw-r--r--   0        0        0       75 2023-06-29 23:59:26.052689 problem_bank_helpers-0.2.0/src/problem_bank_helpers/data/names.csv
--rw-r--r--   0        0        0       56 2023-06-29 23:59:26.052756 problem_bank_helpers-0.2.0/src/problem_bank_helpers/data/vehicles.csv
--rw-r--r--   0        0        0    17971 2023-07-26 03:50:49.754889 problem_bank_helpers-0.2.0/src/problem_bank_helpers/problem_bank_helpers.py
--rw-r--r--   0        0        0     2130 2023-07-26 04:01:39.772310 problem_bank_helpers-0.2.0/setup.py
--rw-r--r--   0        0        0     1981 2023-07-26 04:01:39.772508 problem_bank_helpers-0.2.0/PKG-INFO
+-rwxr-xr-x   0        0        0        1 2021-06-14 01:41:43.016309 problem_bank_helpers-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1244 2021-06-14 01:41:43.033405 problem_bank_helpers-0.2.1/README.md
+-rw-r--r--   0        0        0       44 2023-06-30 00:13:15.868563 problem_bank_helpers-0.2.1/data/animals.csv
+-rw-r--r--   0        0        0       61 2023-06-30 00:13:15.869185 problem_bank_helpers-0.2.1/data/jumpers.csv
+-rw-r--r--   0        0        0       84 2023-06-30 00:13:15.869706 problem_bank_helpers-0.2.1/data/manual_vehicles.csv
+-rw-r--r--   0        0        0      248 2023-06-30 00:13:15.870015 problem_bank_helpers-0.2.1/data/metals.csv
+-rw-r--r--   0        0        0       75 2023-06-30 00:13:15.870268 problem_bank_helpers-0.2.1/data/names.csv
+-rw-r--r--   0        0        0       56 2023-06-30 00:13:15.870498 problem_bank_helpers-0.2.1/data/vehicles.csv
+-rw-r--r--   0        0        0      716 2023-08-09 01:05:33.956349 problem_bank_helpers-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       59 2023-08-09 01:05:54.663929 problem_bank_helpers-0.2.1/src/problem_bank_helpers/__init__.py
+-rw-r--r--   0        0        0       44 2023-06-29 23:59:26.052387 problem_bank_helpers-0.2.1/src/problem_bank_helpers/data/animals.csv
+-rw-r--r--   0        0        0       61 2023-06-29 23:59:26.052468 problem_bank_helpers-0.2.1/src/problem_bank_helpers/data/jumpers.csv
+-rw-r--r--   0        0        0       84 2023-06-29 23:59:26.052539 problem_bank_helpers-0.2.1/src/problem_bank_helpers/data/manual_vehicles.csv
+-rw-r--r--   0        0        0      248 2023-06-29 23:59:26.052616 problem_bank_helpers-0.2.1/src/problem_bank_helpers/data/metals.csv
+-rw-r--r--   0        0        0       75 2023-06-29 23:59:26.052689 problem_bank_helpers-0.2.1/src/problem_bank_helpers/data/names.csv
+-rw-r--r--   0        0        0       56 2023-06-29 23:59:26.052756 problem_bank_helpers-0.2.1/src/problem_bank_helpers/data/vehicles.csv
+-rw-r--r--   0        0        0    18473 2023-08-09 01:03:08.945324 problem_bank_helpers-0.2.1/src/problem_bank_helpers/problem_bank_helpers.py
+-rw-r--r--   0        0        0     2130 2023-08-09 01:06:26.931043 problem_bank_helpers-0.2.1/setup.py
+-rw-r--r--   0        0        0     1981 2023-08-09 01:06:26.931230 problem_bank_helpers-0.2.1/PKG-INFO
```

### Comparing `problem_bank_helpers-0.2.0/README.md` & `problem_bank_helpers-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `problem_bank_helpers-0.2.0/pyproject.toml` & `problem_bank_helpers-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "problem_bank_helpers"
-version = "0.2.0"
+version = "0.2.1"
 description = "Helpful utilities for the open problem bank."
 authors = ["Firas Moosvi and Jake Bobowski"]
 license = "MIT"
 readme = "README.md"
 documentation = "https://problem_bank_helpers.readthedocs.io/en/latest/"
 homepage = "https://github.com/open-resources/problem_bank_helpers"
 repository = "https://github.com/open-resources/problem_bank_helpers"
```

### Comparing `problem_bank_helpers-0.2.0/src/problem_bank_helpers/problem_bank_helpers.py` & `problem_bank_helpers-0.2.1/src/problem_bank_helpers/problem_bank_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 import numpy as np
 import sigfig
 import pandas as pd
 import importlib.resources
 from decimal import Decimal, getcontext, ROUND_HALF_UP
 import re
 
+# Set rounding context
+round_context = getcontext()
+round_context.rounding = ROUND_HALF_UP
+
 ## Load data and dictionaries
 
 ## Better way of loading data and dictionaries
 # Based on this Stack Overflow post: https://stackoverflow.com/questions/65397082/using-resources-module-to-import-data-files
 
 with importlib.resources.open_text("problem_bank_helpers.data", "animals.csv") as file:
     animals = pd.read_csv(file)["Animals"].tolist()
@@ -79,15 +83,15 @@
 def round_sig(x, sig):
     from math import log10, floor
     if x == 0:
         y = 0
     else:
         y = sig - int(floor(log10(abs(x)))) - 1
     # avoid precision loss with floats 
-    x = Decimal(repr(x))
+    x = Decimal(str(x))
     return float(round(x, y))
 
 # def round_sig(x, sig_figs = 3):
 #     """A function that rounds to specific significant digits. Original from SO: https://stackoverflow.com/a/3413529/2217577; adapted by Jake Bobowski
 
 #     Args:
 #         x (float): Number to round to sig figs
@@ -165,37 +169,47 @@
         float/str: Rounded number output to correct significant figures.
     """
     a = [item for item in args]
     kw = {item:v for item,v in kwargs.items() if item in ['sigfigs', 'decimals']}
         
     num_str = str(float(a[0]))
         
-    # Add trailing zeroes if needed
-    
+    # Create default sigfigs if necessary
     if kw.get('sigfigs',None):
         z = kw['sigfigs']
     elif kw.get('decimals', None):
         z = kw['decimals']
     else:
         z = 3 # Default sig figs
         kwargs['sigfigs'] = z
 
-    
-
     # Handle big and small numbers carefully
     if abs(float(num_str)) < 1e-4 or abs(float(num_str)) > 1e15:
         power = int(abs(float(num_str))).as_integer_ratio()[1].bit_length() - 1
         if power < 0:
             power = 0
         num_str = format(float(num_str), f".{power}e")
         kwargs['notation'] = 'sci'
     else:
         num_str = num_str + str(0)*z*2
-                
-    result = sigfig.round(num_str,**kwargs)
+    
+    # Add trailing zeroes if necessary
+    if z > sigfigs(num_str):
+        split_string = num_str.split("e")
+        if "." not in split_string[0]:
+            split_string[0] = split_string[0] + "."
+        split_string[0] = split_string[0] + ("0"*(z - sigfigs(num_str)))
+        num_str = "e".join(split_string)
+    
+    # sigfig.round doesn't like zero
+    if abs(float(num_str)) == 0:
+        result = num_str
+        print("num is zero: " + result + "\n")
+    else:            
+        result = sigfig.round(num_str,**kwargs)
         
     # Switch back to the original format if it was a float
     if isinstance(a[0],float):
         return float(result.replace(",", "")) # Note, sig figs will not be carried through if this is a float
     elif isinstance(a[0],str):
         return result
     elif isinstance(a[0],int):
@@ -204,15 +218,15 @@
         return sigfig.round(*args,**kwargs)
 
 def round_str(*args,**kwargs):
     
     if type(args[0]) is str:
         return args[0]
     
-    if 'sigfigs' not in kwargs.keys():
+    if 'sigfigs' not in kwargs.keys() and 'decimals' not in kwargs.keys():
         kwargs['sigfigs'] = 2
     
     if 'format' not in kwargs.keys():
         if np.abs(args[0]) < 1:
             return roundp(*args,**kwargs,format='std')
         elif np.abs(args[0]) < 1E6:
             return roundp(*args,**kwargs,format='English')
@@ -239,20 +253,15 @@
     # Solution attributed to: https://stackoverflow.com/a/53329223
 
     if type(num) == str:
         return num
     elif type(num) == dict:
         return num
     else:
-        
-
-        round_context = getcontext()
-        round_context.rounding = ROUND_HALF_UP
-
-        tmp = Decimal(repr(num)).quantize(Decimal('1.'+'0'*digits_after_decimal))
+        tmp = Decimal(str(num)).quantize(Decimal('1.'+'0'*digits_after_decimal))
         
         return str(tmp)
 
 def sign_str(number):
     """Returns the sign of the input number as a string.
 
     Args:
```

### Comparing `problem_bank_helpers-0.2.0/setup.py` & `problem_bank_helpers-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*'], 'problem_bank_helpers': ['data/*']}
 
 install_requires = \
 ['numpy>=1.20.3,<2.0.0', 'pandas>=2.0.0,<3.0.0', 'sigfig>=1.1.9,<2.0.0']
 
 setup_kwargs = {
     'name': 'problem-bank-helpers',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'Helpful utilities for the open problem bank.',
     'long_description': '# Problem Bank Helpers \n\n[![Python](https://img.shields.io/badge/python-3.9-blue)]()\n[![codecov](https://codecov.io/gh/open-resources/problem_bank_helpers/branch/main/graph/badge.svg)](https://codecov.io/gh/open-resources/problem_bank_helpers)\n[![Documentation Status](https://readthedocs.org/projects/problem_bank_helpers/badge/?version=latest)](https://problem_bank_helpers.readthedocs.io/en/latest/?badge=latest)\n\n\n## Installation\n\n```bash\n$ pip install -i https://test.pypi.org/simple/ problem_bank_helpers\n```\n\n## Features\n\n- TODO\n\n## Dependencies\n\n- TODO\n\n## Usage\n\n- TODO\n\n## Documentation\n\nThe official documentation is hosted on Read the Docs: https://problem_bank_helpers.readthedocs.io/en/latest/\n\n## Contributors\n\nWe welcome and recognize all contributions. You can see a list of current contributors in the [contributors tab](https://github.com/open-resources/problem_bank_helpers/graphs/contributors).\n\n### Credits\n\nThis package was created with Cookiecutter and the UBC-MDS/cookiecutter-ubc-mds project template, modified from the [pyOpenSci/cookiecutter-pyopensci](https://github.com/pyOpenSci/cookiecutter-pyopensci) project template and the [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage).\n',
     'author': 'Firas Moosvi and Jake Bobowski',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/open-resources/problem_bank_helpers',
```

### Comparing `problem_bank_helpers-0.2.0/PKG-INFO` & `problem_bank_helpers-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: problem-bank-helpers
-Version: 0.2.0
+Version: 0.2.1
 Summary: Helpful utilities for the open problem bank.
 Home-page: https://github.com/open-resources/problem_bank_helpers
 License: MIT
 Author: Firas Moosvi and Jake Bobowski
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

