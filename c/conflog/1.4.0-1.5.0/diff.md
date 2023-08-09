# Comparing `tmp/conflog-1.4.0.tar.gz` & `tmp/conflog-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conflog-1.4.0.tar", last modified: Tue Jun 27 12:51:20 2023, max compression
+gzip compressed data, was "conflog-1.5.0.tar", last modified: Wed Aug  9 01:07:35 2023, max compression
```

## Comparing `conflog-1.4.0.tar` & `conflog-1.5.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:51:20.878944 conflog-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-06-27 12:50:25.000000 conflog-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-06-27 12:51:20.878944 conflog-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-06-27 12:50:25.000000 conflog-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:51:20.874943 conflog-1.4.0/conflog/
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-06-27 12:50:25.000000 conflog-1.4.0/conflog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-06-27 12:50:25.000000 conflog-1.4.0/conflog/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:51:20.878944 conflog-1.4.0/conflog/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:50:25.000000 conflog-1.4.0/conflog/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-27 12:50:25.000000 conflog-1.4.0/conflog/handlers/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-27 12:50:25.000000 conflog-1.4.0/conflog/handlers/stream_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:51:20.878944 conflog-1.4.0/conflog/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-27 12:50:25.000000 conflog-1.4.0/conflog/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-27 12:50:25.000000 conflog-1.4.0/conflog/loaders/environ_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-27 12:50:25.000000 conflog-1.4.0/conflog/loaders/ini_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-27 12:50:25.000000 conflog-1.4.0/conflog/loaders/json_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-27 12:50:25.000000 conflog-1.4.0/conflog/loaders/xml_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-27 12:50:25.000000 conflog-1.4.0/conflog/loaders/yaml_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:51:20.874943 conflog-1.4.0/conflog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-06-27 12:51:20.000000 conflog-1.4.0/conflog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-27 12:51:20.000000 conflog-1.4.0/conflog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 12:51:20.000000 conflog-1.4.0/conflog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-27 12:51:20.000000 conflog-1.4.0/conflog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-27 12:51:20.000000 conflog-1.4.0/conflog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 12:51:20.878944 conflog-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-27 12:50:25.000000 conflog-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:51:20.878944 conflog-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:50:25.000000 conflog-1.4.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:51:20.878944 conflog-1.4.0/tests/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:50:25.000000 conflog-1.4.0/tests/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-27 12:50:25.000000 conflog-1.4.0/tests/handlers/test_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-27 12:50:25.000000 conflog-1.4.0/tests/handlers/test_stream_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:51:20.878944 conflog-1.4.0/tests/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:50:25.000000 conflog-1.4.0/tests/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-27 12:50:25.000000 conflog-1.4.0/tests/loaders/test_environ_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-06-27 12:50:25.000000 conflog-1.4.0/tests/loaders/test_ini_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-06-27 12:50:25.000000 conflog-1.4.0/tests/loaders/test_json_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-06-27 12:50:25.000000 conflog-1.4.0/tests/loaders/test_xml_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-27 12:50:25.000000 conflog-1.4.0/tests/loaders/test_yaml_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9574 2023-06-27 12:50:25.000000 conflog-1.4.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-06-27 12:50:25.000000 conflog-1.4.0/tests/test_conflog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:07:35.505716 conflog-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-08-09 01:06:54.000000 conflog-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-08-09 01:07:35.505716 conflog-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-08-09 01:06:54.000000 conflog-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:07:35.501716 conflog-1.5.0/conflog/
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-08-09 01:06:54.000000 conflog-1.5.0/conflog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-08-09 01:06:54.000000 conflog-1.5.0/conflog/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:07:35.501716 conflog-1.5.0/conflog/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-09 01:06:54.000000 conflog-1.5.0/conflog/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-08-09 01:06:54.000000 conflog-1.5.0/conflog/handlers/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-09 01:06:54.000000 conflog-1.5.0/conflog/handlers/stream_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:07:35.501716 conflog-1.5.0/conflog/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-08-09 01:06:54.000000 conflog-1.5.0/conflog/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-08-09 01:06:54.000000 conflog-1.5.0/conflog/loaders/environ_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-08-09 01:06:54.000000 conflog-1.5.0/conflog/loaders/ini_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-08-09 01:06:54.000000 conflog-1.5.0/conflog/loaders/json_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-08-09 01:06:54.000000 conflog-1.5.0/conflog/loaders/xml_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-09 01:06:54.000000 conflog-1.5.0/conflog/loaders/yaml_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:07:35.501716 conflog-1.5.0/conflog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-08-09 01:07:35.000000 conflog-1.5.0/conflog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-08-09 01:07:35.000000 conflog-1.5.0/conflog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 01:07:35.000000 conflog-1.5.0/conflog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-09 01:07:35.000000 conflog-1.5.0/conflog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-09 01:07:35.000000 conflog-1.5.0/conflog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-09 01:07:35.505716 conflog-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-08-09 01:06:54.000000 conflog-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:07:35.501716 conflog-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-09 01:06:54.000000 conflog-1.5.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:07:35.501716 conflog-1.5.0/tests/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-09 01:06:54.000000 conflog-1.5.0/tests/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-08-09 01:06:54.000000 conflog-1.5.0/tests/handlers/test_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-08-09 01:06:54.000000 conflog-1.5.0/tests/handlers/test_stream_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 01:07:35.505716 conflog-1.5.0/tests/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-09 01:06:54.000000 conflog-1.5.0/tests/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-08-09 01:06:54.000000 conflog-1.5.0/tests/loaders/test_environ_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-08-09 01:06:54.000000 conflog-1.5.0/tests/loaders/test_ini_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-08-09 01:06:54.000000 conflog-1.5.0/tests/loaders/test_json_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-08-09 01:06:54.000000 conflog-1.5.0/tests/loaders/test_xml_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-08-09 01:06:54.000000 conflog-1.5.0/tests/loaders/test_yaml_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10991 2023-08-09 01:06:54.000000 conflog-1.5.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-08-09 01:06:54.000000 conflog-1.5.0/tests/test_conflog.py
```

### Comparing `conflog-1.4.0/LICENSE` & `conflog-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `conflog-1.4.0/PKG-INFO` & `conflog-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conflog
-Version: 1.4.0
+Version: 1.5.0
 Summary: Python logging setup via environment variables and configuration files
 Home-page: https://github.com/cliffano/pyconflog
 Author: Cliffano Subagio
 Author-email: cliffano@gmail.com
 Keywords: log,logger,logging,config,configuration,environment,envvar,ini,json,xml,yaml
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,15 +12,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img align="right" src="https://raw.github.com/cliffano/pyconflog/main/avatar.jpg" alt="Avatar"/>
 
 [![Build Status](https://github.com/cliffano/pyconflog/workflows/CI/badge.svg)](https://github.com/cliffano/pyconflog/actions?query=workflow%3ACI)
-[![Vulnerabilities Status](https://snyk.io/test/github/cliffano/pyconflog/badge.svg)](https://snyk.io/test/github/cliffano/pyconflog)
+[![Security Status](https://snyk.io/test/github/cliffano/pyconflog/badge.svg)](https://snyk.io/test/github/cliffano/pyconflog)
 [![Published Version](https://img.shields.io/pypi/v/conflog.svg)](https://pypi.python.org/pypi/conflog)
 <br/>
 
 Pyconflog
 ---------
 
 Pyconflog library provides Python logging setup via environment variables and configuration files.
```

### Comparing `conflog-1.4.0/README.md` & `conflog-1.5.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <img align="right" src="https://raw.github.com/cliffano/pyconflog/main/avatar.jpg" alt="Avatar"/>
 
 [![Build Status](https://github.com/cliffano/pyconflog/workflows/CI/badge.svg)](https://github.com/cliffano/pyconflog/actions?query=workflow%3ACI)
-[![Vulnerabilities Status](https://snyk.io/test/github/cliffano/pyconflog/badge.svg)](https://snyk.io/test/github/cliffano/pyconflog)
+[![Security Status](https://snyk.io/test/github/cliffano/pyconflog/badge.svg)](https://snyk.io/test/github/cliffano/pyconflog)
 [![Published Version](https://img.shields.io/pypi/v/conflog.svg)](https://pypi.python.org/pypi/conflog)
 <br/>
 
 Pyconflog
 ---------
 
 Pyconflog library provides Python logging setup via environment variables and configuration files.
```

### Comparing `conflog-1.4.0/conflog/__init__.py` & `conflog-1.5.0/conflog/__init__.py`

 * *Files identical despite different names*

### Comparing `conflog-1.4.0/conflog/config.py` & `conflog-1.5.0/conflog/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         return self.conf.get('format', DEFAULT_FORMAT)
 
     def get_level(self) -> int:
         """Get log level.
         If log level is not specified, default to 'info'.
         """
         level = self.conf.get('level', DEFAULT_LEVEL)
-        return LEVELS[level]
+        return LEVELS[level.lower()]
 
     def get_extras(self) -> dict:
         """Get extras.
         Extras is a dictionary of extra message parameters
         to be added to the log.
         If extras is not specified, default to an empty dictionary.
         """
```

### Comparing `conflog-1.4.0/conflog/handlers/file_handler.py` & `conflog-1.5.0/conflog/handlers/file_handler.py`

 * *Files identical despite different names*

### Comparing `conflog-1.4.0/conflog/loaders/ini_loader.py` & `conflog-1.5.0/conflog/loaders/ini_loader.py`

 * *Files identical despite different names*

### Comparing `conflog-1.4.0/conflog/loaders/xml_loader.py` & `conflog-1.5.0/conflog/loaders/xml_loader.py`

 * *Files identical despite different names*

### Comparing `conflog-1.4.0/conflog.egg-info/PKG-INFO` & `conflog-1.5.0/conflog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conflog
-Version: 1.4.0
+Version: 1.5.0
 Summary: Python logging setup via environment variables and configuration files
 Home-page: https://github.com/cliffano/pyconflog
 Author: Cliffano Subagio
 Author-email: cliffano@gmail.com
 Keywords: log,logger,logging,config,configuration,environment,envvar,ini,json,xml,yaml
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,15 +12,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img align="right" src="https://raw.github.com/cliffano/pyconflog/main/avatar.jpg" alt="Avatar"/>
 
 [![Build Status](https://github.com/cliffano/pyconflog/workflows/CI/badge.svg)](https://github.com/cliffano/pyconflog/actions?query=workflow%3ACI)
-[![Vulnerabilities Status](https://snyk.io/test/github/cliffano/pyconflog/badge.svg)](https://snyk.io/test/github/cliffano/pyconflog)
+[![Security Status](https://snyk.io/test/github/cliffano/pyconflog/badge.svg)](https://snyk.io/test/github/cliffano/pyconflog)
 [![Published Version](https://img.shields.io/pypi/v/conflog.svg)](https://pypi.python.org/pypi/conflog)
 <br/>
 
 Pyconflog
 ---------
 
 Pyconflog library provides Python logging setup via environment variables and configuration files.
```

### Comparing `conflog-1.4.0/conflog.egg-info/SOURCES.txt` & `conflog-1.5.0/conflog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `conflog-1.4.0/setup.py` & `conflog-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `conflog-1.4.0/tests/handlers/test_file_handler.py` & `conflog-1.5.0/tests/handlers/test_file_handler.py`

 * *Files identical despite different names*

### Comparing `conflog-1.4.0/tests/handlers/test_stream_handler.py` & `conflog-1.5.0/tests/handlers/test_stream_handler.py`

 * *Files identical despite different names*

### Comparing `conflog-1.4.0/tests/loaders/test_environ_loader.py` & `conflog-1.5.0/tests/loaders/test_environ_loader.py`

 * *Files identical despite different names*

### Comparing `conflog-1.4.0/tests/loaders/test_ini_loader.py` & `conflog-1.5.0/tests/loaders/test_ini_loader.py`

 * *Files identical despite different names*

### Comparing `conflog-1.4.0/tests/loaders/test_json_loader.py` & `conflog-1.5.0/tests/loaders/test_json_loader.py`

 * *Files identical despite different names*

### Comparing `conflog-1.4.0/tests/loaders/test_xml_loader.py` & `conflog-1.5.0/tests/loaders/test_xml_loader.py`

 * *Files identical despite different names*

### Comparing `conflog-1.4.0/tests/loaders/test_yaml_loader.py` & `conflog-1.5.0/tests/loaders/test_yaml_loader.py`

 * *Files identical despite different names*

### Comparing `conflog-1.4.0/tests/test_config.py` & `conflog-1.5.0/tests/test_config.py`

 * *Files 15% similar despite different names*

```diff
@@ -184,7 +184,41 @@
         config = Config(conf_files=['somefile.ini'], conf_dict=conf_dict)
         self.assertEqual(config.get_handlers(), ['stream'])
         self.assertEqual(config.get_datefmt(), '%y')
         self.assertEqual(config.get_filename(), 'overwriteconfdictlog.log')
         self.assertEqual(config.get_filemode(), 'w')
         self.assertEqual(config.get_format(), '%(message)s')
         self.assertEqual(config.get_level(), logging.CRITICAL)
+
+    def test_get_config_with_uppercase_level(self):
+        conf_dict = {
+            'handlers': 'stream',
+            'datefmt': '%y',
+            'filename': 'overwriteconfdictlog.log',
+            'filemode': 'w',
+            'format': '%(message)s',
+            'level': 'CRITICAL'
+        }
+        config = Config(conf_dict=conf_dict)
+        self.assertEqual(config.get_handlers(), ['stream'])
+        self.assertEqual(config.get_datefmt(), '%y')
+        self.assertEqual(config.get_filename(), 'overwriteconfdictlog.log')
+        self.assertEqual(config.get_filemode(), 'w')
+        self.assertEqual(config.get_format(), '%(message)s')
+        self.assertEqual(config.get_level(), logging.CRITICAL)
+
+    def test_get_config_with_mixed_case_level(self):
+        conf_dict = {
+            'handlers': 'stream',
+            'datefmt': '%y',
+            'filename': 'overwriteconfdictlog.log',
+            'filemode': 'w',
+            'format': '%(message)s',
+            'level': 'WaRning'
+        }
+        config = Config(conf_dict=conf_dict)
+        self.assertEqual(config.get_handlers(), ['stream'])
+        self.assertEqual(config.get_datefmt(), '%y')
+        self.assertEqual(config.get_filename(), 'overwriteconfdictlog.log')
+        self.assertEqual(config.get_filemode(), 'w')
+        self.assertEqual(config.get_format(), '%(message)s')
+        self.assertEqual(config.get_level(), logging.WARNING)
```

### Comparing `conflog-1.4.0/tests/test_conflog.py` & `conflog-1.5.0/tests/test_conflog.py`

 * *Files identical despite different names*

