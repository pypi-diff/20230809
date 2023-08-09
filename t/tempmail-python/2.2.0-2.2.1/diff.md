# Comparing `tmp/tempmail-python-2.2.0.tar.gz` & `tmp/tempmail-python-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tempmail-python-2.2.0.tar", last modified: Mon Aug  7 15:58:13 2023, max compression
+gzip compressed data, was "tempmail-python-2.2.1.tar", last modified: Wed Aug  9 05:42:17 2023, max compression
```

## Comparing `tempmail-python-2.2.0.tar` & `tempmail-python-2.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:58:13.144544 tempmail-python-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-07 15:58:03.000000 tempmail-python-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-08-07 15:58:13.144544 tempmail-python-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-08-07 15:58:03.000000 tempmail-python-2.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 15:58:13.144544 tempmail-python-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-07 15:58:03.000000 tempmail-python-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:58:13.144544 tempmail-python-2.2.0/tempmail/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-07 15:58:03.000000 tempmail-python-2.2.0/tempmail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-08-07 15:58:03.000000 tempmail-python-2.2.0/tempmail/providers.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-07 15:58:03.000000 tempmail-python-2.2.0/tempmail/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:58:13.144544 tempmail-python-2.2.0/tempmail_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-08-07 15:58:13.000000 tempmail-python-2.2.0/tempmail_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-08-07 15:58:13.000000 tempmail-python-2.2.0/tempmail_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 15:58:13.000000 tempmail-python-2.2.0/tempmail_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-07 15:58:13.000000 tempmail-python-2.2.0/tempmail_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-07 15:58:13.000000 tempmail-python-2.2.0/tempmail_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 05:42:17.552390 tempmail-python-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-09 05:42:08.000000 tempmail-python-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-08-09 05:42:17.552390 tempmail-python-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-08-09 05:42:08.000000 tempmail-python-2.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-09 05:42:17.552390 tempmail-python-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-09 05:42:08.000000 tempmail-python-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 05:42:17.552390 tempmail-python-2.2.1/tempmail/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-09 05:42:08.000000 tempmail-python-2.2.1/tempmail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-08-09 05:42:08.000000 tempmail-python-2.2.1/tempmail/providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-09 05:42:08.000000 tempmail-python-2.2.1/tempmail/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 05:42:17.552390 tempmail-python-2.2.1/tempmail_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-08-09 05:42:17.000000 tempmail-python-2.2.1/tempmail_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-08-09 05:42:17.000000 tempmail-python-2.2.1/tempmail_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 05:42:17.000000 tempmail-python-2.2.1/tempmail_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-09 05:42:17.000000 tempmail-python-2.2.1/tempmail_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-09 05:42:17.000000 tempmail-python-2.2.1/tempmail_python.egg-info/top_level.txt
```

### Comparing `tempmail-python-2.2.0/LICENSE` & `tempmail-python-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tempmail-python-2.2.0/PKG-INFO` & `tempmail-python-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tempmail-python
-Version: 2.2.0
+Version: 2.2.1
 Summary: Python library for generating and managing temporary email addresses.
 Home-page: https://github.com/cubicbyte/tempmail-python
 Author: cubicbyte
 Author-email: bmaruhnenko@gmail.com
 License: MIT
 Keywords: disposable-email temporary-email temp-email temp-mail email mail email-generator mail-generator
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `tempmail-python-2.2.0/README.md` & `tempmail-python-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `tempmail-python-2.2.0/setup.py` & `tempmail-python-2.2.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def read(path: str) -> str:
     with open(path, 'r', encoding='utf-8') as f:
         return f.read()
 
 setup(
     name='tempmail-python',
-    version='2.2.0',
+    version='2.2.1',
     description='Python library for generating and managing temporary email addresses.',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     author='cubicbyte',
     author_email='bmaruhnenko@gmail.com',
     url='https://github.com/cubicbyte/tempmail-python',
     packages = find_packages(),
```

### Comparing `tempmail-python-2.2.0/tempmail/providers.py` & `tempmail-python-2.2.1/tempmail/providers.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,17 +66,25 @@
     @utils.cache
     def get_domains() -> tuple[str, ...]:
         """List of allowed email domains"""
         resp = requests.get('https://www.1secmail.com/api/v1/?action=getDomainList')
         resp.raise_for_status()
         return tuple(resp.json())
 
-    def __str__(self) -> str:
+    @property
+    def address(self) -> str:
+        """The full email address"""
         return f'{self.username}@{self.domain}'
 
+    def __repr__(self) -> str:
+        return f'<{self.__class__.__name__} address={self.address!r}>'
+
+    def __str__(self) -> str:
+        return self.address
+
     @dataclass
     class MessageInfo:
         id: int
         from_addr: str
         subject: str
         date_str: str
         _mail: 'OneSecMail'
```

### Comparing `tempmail-python-2.2.0/tempmail_python.egg-info/PKG-INFO` & `tempmail-python-2.2.1/tempmail_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tempmail-python
-Version: 2.2.0
+Version: 2.2.1
 Summary: Python library for generating and managing temporary email addresses.
 Home-page: https://github.com/cubicbyte/tempmail-python
 Author: cubicbyte
 Author-email: bmaruhnenko@gmail.com
 License: MIT
 Keywords: disposable-email temporary-email temp-email temp-mail email mail email-generator mail-generator
 Classifier: Development Status :: 5 - Production/Stable
```

