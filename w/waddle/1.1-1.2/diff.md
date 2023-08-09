# Comparing `tmp/waddle-1.1.tar.gz` & `tmp/waddle-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waddle-1.1.tar", last modified: Fri Feb 17 01:33:08 2023, max compression
+gzip compressed data, was "waddle-1.2.tar", last modified: Wed Aug  9 04:30:09 2023, max compression
```

## Comparing `waddle-1.1.tar` & `waddle-1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-17 01:33:08.939017 waddle-1.1/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       24 2022-06-26 19:33:58.000000 waddle-1.1/MANIFEST.in
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     4050 2023-02-17 01:33:08.939017 waddle-1.1/PKG-INFO
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     3351 2023-02-13 21:31:35.000000 waddle-1.1/README.md
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)      271 2023-02-17 01:33:08.939017 waddle-1.1/setup.cfg
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     1370 2023-02-17 01:33:04.000000 waddle-1.1/setup.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-17 01:33:08.939017 waddle-1.1/waddle/
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)      265 2023-02-17 01:33:04.000000 waddle-1.1/waddle/__init__.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-17 01:33:08.939017 waddle-1.1/waddle/aws/
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)       61 2022-06-26 19:33:58.000000 waddle-1.1/waddle/aws/__init__.py
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     3196 2023-02-13 21:37:33.000000 waddle-1.1/waddle/aws/pstore.py
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)      486 2023-02-13 21:39:09.000000 waddle-1.1/waddle/aws/session.py
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     7360 2023-02-13 21:41:41.000000 waddle-1.1/waddle/bunch.py
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     3360 2023-02-13 21:33:49.000000 waddle-1.1/waddle/cli.py
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     7752 2023-02-17 01:29:04.000000 waddle-1.1/waddle/param_bunch.py
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)      128 2022-06-26 19:33:58.000000 waddle-1.1/waddle/settings.py
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)      448 2022-06-26 19:33:58.000000 waddle-1.1/waddle/utils.py
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)        3 2022-06-26 19:33:58.000000 waddle-1.1/waddle/version
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-17 01:33:08.939017 waddle-1.1/waddle.egg-info/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     4050 2023-02-17 01:33:08.000000 waddle-1.1/waddle.egg-info/PKG-INFO
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      434 2023-02-17 01:33:08.000000 waddle-1.1/waddle.egg-info/SOURCES.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        1 2023-02-17 01:33:08.000000 waddle-1.1/waddle.egg-info/dependency_links.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       44 2023-02-17 01:33:08.000000 waddle-1.1/waddle.egg-info/entry_points.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       82 2023-02-17 01:33:08.000000 waddle-1.1/waddle.egg-info/requires.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        7 2023-02-17 01:33:08.000000 waddle-1.1/waddle.egg-info/top_level.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        1 2023-02-17 01:31:09.000000 waddle-1.1/waddle.egg-info/zip-safe
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-08-09 04:30:09.192774 waddle-1.2/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       24 2022-07-15 13:30:14.000000 waddle-1.2/MANIFEST.in
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     4030 2023-08-09 04:30:09.192774 waddle-1.2/PKG-INFO
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     3351 2023-08-09 02:56:54.000000 waddle-1.2/README.md
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)      271 2023-08-09 04:30:09.192774 waddle-1.2/setup.cfg
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     1370 2023-08-09 04:30:03.000000 waddle-1.2/setup.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-08-09 04:30:09.192774 waddle-1.2/waddle/
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)      265 2023-08-09 04:30:03.000000 waddle-1.2/waddle/__init__.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-08-09 04:30:09.192774 waddle-1.2/waddle/aws/
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)       61 2022-07-15 13:30:14.000000 waddle-1.2/waddle/aws/__init__.py
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     3955 2023-08-09 03:38:51.000000 waddle-1.2/waddle/aws/pstore.py
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)      353 2023-08-09 03:01:45.000000 waddle-1.2/waddle/aws/session.py
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     7360 2023-08-09 02:56:54.000000 waddle-1.2/waddle/bunch.py
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     3360 2023-08-09 02:56:54.000000 waddle-1.2/waddle/cli.py
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     9298 2023-08-09 04:10:39.000000 waddle-1.2/waddle/param_bunch.py
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)      128 2022-07-15 13:30:14.000000 waddle-1.2/waddle/settings.py
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)      448 2022-07-15 13:30:14.000000 waddle-1.2/waddle/utils.py
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)        3 2022-07-15 13:30:14.000000 waddle-1.2/waddle/version
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-08-09 04:30:09.192774 waddle-1.2/waddle.egg-info/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     4030 2023-08-09 04:30:08.000000 waddle-1.2/waddle.egg-info/PKG-INFO
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      434 2023-08-09 04:30:08.000000 waddle-1.2/waddle.egg-info/SOURCES.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        1 2023-08-09 04:30:08.000000 waddle-1.2/waddle.egg-info/dependency_links.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       43 2023-08-09 04:30:08.000000 waddle-1.2/waddle.egg-info/entry_points.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       82 2023-08-09 04:30:08.000000 waddle-1.2/waddle.egg-info/requires.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        7 2023-08-09 04:30:08.000000 waddle-1.2/waddle.egg-info/top_level.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        1 2023-08-09 03:40:45.000000 waddle-1.2/waddle.egg-info/zip-safe
```

### Comparing `waddle-1.1/PKG-INFO` & `waddle-1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: waddle
-Version: 1.1
+Version: 1.2
 Summary: A pathy wrapper around aws parameter store
 Home-page: https://github.com/angry-penguins/waddle
 Author: Preetam Shingavi
 Author-email: p.shingavi@yahoo.com
 License: BSD
 Keywords: aws python parameter-store kms
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: BSD License
@@ -150,9 +149,7 @@
     }
 }
 config = Bunch(config)
 env = config.env()
 assert env('FTP_PASSWORD') == 'password'
 assert env('FTP_HOST') == '127.0.0.1'
 ```
-
-
```

### Comparing `waddle-1.1/README.md` & `waddle-1.2/README.md`

 * *Files identical despite different names*

### Comparing `waddle-1.1/setup.py` & `waddle-1.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = '1.1'
+version = '1.2'
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='waddle',
     version=version,
@@ -28,15 +28,15 @@
     packages=find_packages(exclude=['ez_setup', 'examples', 'tests']),
     include_package_data=True,
     zip_safe=True,
     install_requires=[
         'pyyaml',
         'boto3>=1.9.0',
         'click>=7.0',
-        'murmuration>=0.8',
+        'murmuration>=1.2',
         'ruamel.yaml>=0.15.87',
         'halo>=0.0.26',
     ],
     entry_points={
         'console_scripts': [
             'waddle=waddle.cli:main',
         ]
```

### Comparing `waddle-1.1/waddle/bunch.py` & `waddle-1.2/waddle/bunch.py`

 * *Files identical despite different names*

### Comparing `waddle-1.1/waddle/cli.py` & `waddle-1.2/waddle/cli.py`

 * *Files identical despite different names*

### Comparing `waddle-1.1/waddle/param_bunch.py` & `waddle-1.2/waddle/param_bunch.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,30 +19,40 @@
     'ParamBunch',
 ]
 
 
 dict_class = CommentedMap
 
 
-def ssm_scalar_constructor(loader, node, profile=None, region=None):
+def ssm_scalar_constructor(
+        loader, node, profile=None, region=None,
+        session=None, ssm_client=None):
     key = loader.construct_scalar(node)
-    return get_parameter(key, profile=profile, region=region)
+    return get_parameter(
+        key, profile=profile, region=region, session=session,
+        client=ssm_client)
 
 
 class Yaml(YAML):
-    def __init__(self, profile=None, region=None):
+    def __init__(self, profile=None, region=None, session=None, client=None):
         super().__init__(typ='rt')
         self.explicit_start = True
         self.preserve_quotes = True
         self.indent(sequence=4, mapping=2, offset=2)
-        if profile or region:
+        if profile or region or session or client:
+            from .aws.pstore import create_ssm_client
+            c = create_ssm_client(
+                profile=profile, region=region, session=session,
+                client=client)
             fn = partial(
                 ssm_scalar_constructor,
                 profile=profile,
-                region=region)
+                region=region,
+                session=session,
+                ssm_client=c)
             self.constructor.add_constructor('!ssm', fn)
 
 
 def dump_yaml(x, filename):
     y = Yaml()
     if isinstance(filename, str):
         with open(filename, 'w') as f:
@@ -91,18 +101,24 @@
         for key, value in d.items():
             if isinstance(value, Mapping):
                 yield from ParamBunch._traverse(value, prefix + [ key ])
             else:
                 yield '.'.join(prefix + [ key ]), value
 
     @staticmethod
-    def try_decrypt(value, region=None, profile=None, session=None):
-        if isinstance(value, str):
+    def try_decrypt(
+            value, region=None, profile=None,
+            session=None, client=None):
+        # an artifact of murmuration encryption is that all
+        # encrypted values will start with 'AQI', so fast fail
+        # out of decrypt
+        if isinstance(value, str) and value[:3] == 'AQI':
             try:
-                value = kms_wrapped.decrypt(value, region, profile, session)
+                value = kms_wrapped.decrypt(
+                    value, region, profile, session, client=client)
             except ValueError:
                 pass
         return value
 
     def from_file(self, filename, decrypt=True, handle_tags=True):
         # late load logger in case anyone sets up logging
         # later
@@ -131,22 +147,28 @@
                 raise KeyError(f'`{key}` is not a valid key name')
             if key.startswith('meta.'):
                 self[key] = value
             else:
                 values.append((key, value))
         self.handle_file_values(values, decrypt)
 
-    def handle_file_values(self, values, decrypt):
+    def handle_file_values(self, values, decrypt, session=None, client=None):
+        from murmuration.aws import kms_client
         region = self.get('meta.region')
         profile = self.get('meta.profile')
+        client = kms_client(
+            region=region, profile=profile,
+            session=session, client=client)
         for key, value in values:
             if not decrypt:
                 self[key] = value
                 continue
-            self[key] = ParamBunch.try_decrypt(value, region, profile)
+            self[key] = ParamBunch.try_decrypt(
+                value, region, profile,
+                session=session, client=client)
             if self[key] != value:
                 self.encrypted.append(key)
 
     def load(self, prefix=None, filename=None, decrypt=True):
         if prefix:
             self.from_aws(prefix)
         if filename:
@@ -167,25 +189,40 @@
     def _encrypted_keys(self):
         namespace = self.get('meta.namespace', '')
         ms_encrypted = set()
         for x in self.encrypted:
             ms_encrypted.add(ssm_key(namespace, x))
         return ms_encrypted
 
-    def to_aws(self, force_encryption=False, verbose=True):
+    def to_aws(
+            self, force_encryption=False, verbose=True,
+            profile=None, region=None, session=None, ssm_client=None):
+        from .aws.pstore import create_ssm_client
+        ssm_client = create_ssm_client(
+            profile=profile, region=region, session=session, client=ssm_client)
         ms_encrypted = self._encrypted_keys()
         kms_key = self.get('meta.kms_key')
         for key, value in self.aws_items():
             encrypted = key in ms_encrypted
             encrypted = encrypted or force_encryption
-            put_parameter(key, value, kms_key, encrypted, verbose)
-
-    def delete_from_aws(self, verbose=True):
+            put_parameter(
+                key, value, kms_key, encrypted, verbose,
+                session=session, client=ssm_client)
+
+    def delete_from_aws(
+            self, verbose=True,
+            profile=None, region=None,
+            session=None, ssm_client=None):
+        from .aws.pstore import create_ssm_client
+        ssm_client = create_ssm_client(
+            profile=profile, region=region, session=session, client=ssm_client)
         keys = [ key for key, _ in self.aws_items() ]
-        delete_parameters(*keys, verbose=verbose)
+        delete_parameters(
+            *keys, verbose=verbose,
+            session=session, client=ssm_client)
 
     def original_value(self, key):
         data = self.original_values
         if key in data:
             return data, key, data[key]
         pieces = key.split('.')
         for x in pieces[:-1]:
```

### Comparing `waddle-1.1/waddle.egg-info/PKG-INFO` & `waddle-1.2/waddle.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: waddle
-Version: 1.1
+Version: 1.2
 Summary: A pathy wrapper around aws parameter store
 Home-page: https://github.com/angry-penguins/waddle
 Author: Preetam Shingavi
 Author-email: p.shingavi@yahoo.com
 License: BSD
 Keywords: aws python parameter-store kms
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: BSD License
@@ -150,9 +149,7 @@
     }
 }
 config = Bunch(config)
 env = config.env()
 assert env('FTP_PASSWORD') == 'password'
 assert env('FTP_HOST') == '127.0.0.1'
 ```
-
-
```

