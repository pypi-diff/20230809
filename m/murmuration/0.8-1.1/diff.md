# Comparing `tmp/murmuration-0.8.tar.gz` & `tmp/murmuration-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "murmuration-0.8.tar", last modified: Fri Feb 17 00:57:48 2023, max compression
+gzip compressed data, was "murmuration-1.1.tar", last modified: Wed Aug  9 02:55:55 2023, max compression
```

## Comparing `murmuration-0.8.tar` & `murmuration-1.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-17 00:57:48.205022 murmuration-0.8/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     4362 2023-02-17 00:57:48.205022 murmuration-0.8/PKG-INFO
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     3572 2023-02-17 00:53:57.000000 murmuration-0.8/README.md
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-17 00:57:48.195022 murmuration-0.8/murmuration/
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-16 23:00:02.000000 murmuration-0.8/murmuration/__init__.py
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     1326 2023-02-17 00:03:23.000000 murmuration-0.8/murmuration/aws.py
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     3381 2023-02-17 00:05:09.000000 murmuration-0.8/murmuration/gcm.py
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)      614 2023-02-17 00:45:17.000000 murmuration-0.8/murmuration/helpers.py
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     1369 2023-02-17 00:04:53.000000 murmuration-0.8/murmuration/kms.py
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     1662 2023-02-16 23:00:02.000000 murmuration-0.8/murmuration/kms_wrap.py
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     2090 2023-02-17 00:05:59.000000 murmuration-0.8/murmuration/kms_wrapped.py
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)       22 2023-02-16 23:00:02.000000 murmuration-0.8/murmuration/settings.py
-drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-02-17 00:57:48.205022 murmuration-0.8/murmuration.egg-info/
--rw-r--r--   0 2ps       (1000) 2ps       (1000)     4362 2023-02-17 00:57:48.000000 murmuration-0.8/murmuration.egg-info/PKG-INFO
--rw-r--r--   0 2ps       (1000) 2ps       (1000)      411 2023-02-17 00:57:48.000000 murmuration-0.8/murmuration.egg-info/SOURCES.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        1 2023-02-17 00:57:48.000000 murmuration-0.8/murmuration.egg-info/dependency_links.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       26 2023-02-17 00:57:48.000000 murmuration-0.8/murmuration.egg-info/requires.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)       12 2023-02-17 00:57:48.000000 murmuration-0.8/murmuration.egg-info/top_level.txt
--rw-r--r--   0 2ps       (1000) 2ps       (1000)        1 2023-02-16 23:08:47.000000 murmuration-0.8/murmuration.egg-info/zip-safe
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)      153 2023-02-17 00:57:48.205022 murmuration-0.8/setup.cfg
--rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     1319 2023-02-17 00:57:44.000000 murmuration-0.8/setup.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-08-09 02:55:55.482775 murmuration-1.1/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     4342 2023-08-09 02:55:55.482775 murmuration-1.1/PKG-INFO
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     3572 2023-08-09 02:32:48.000000 murmuration-1.1/README.md
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-08-09 02:55:55.482775 murmuration-1.1/murmuration/
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-08-09 02:32:48.000000 murmuration-1.1/murmuration/__init__.py
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)      396 2023-08-09 02:41:16.000000 murmuration-1.1/murmuration/aws.py
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     3381 2023-08-09 02:32:48.000000 murmuration-1.1/murmuration/gcm.py
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)      614 2023-08-09 02:32:48.000000 murmuration-1.1/murmuration/helpers.py
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     1486 2023-08-09 02:45:29.000000 murmuration-1.1/murmuration/kms.py
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     1662 2023-08-09 02:32:48.000000 murmuration-1.1/murmuration/kms_wrap.py
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     2206 2023-08-09 02:41:16.000000 murmuration-1.1/murmuration/kms_wrapped.py
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)       22 2023-08-09 02:32:48.000000 murmuration-1.1/murmuration/settings.py
+drwxr-xr-x   0 2ps       (1000) 2ps       (1000)        0 2023-08-09 02:55:55.482775 murmuration-1.1/murmuration.egg-info/
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)     4342 2023-08-09 02:55:55.000000 murmuration-1.1/murmuration.egg-info/PKG-INFO
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)      449 2023-08-09 02:55:55.000000 murmuration-1.1/murmuration.egg-info/SOURCES.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        1 2023-08-09 02:55:55.000000 murmuration-1.1/murmuration.egg-info/dependency_links.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       55 2023-08-09 02:55:55.000000 murmuration-1.1/murmuration.egg-info/entry_points.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       26 2023-08-09 02:55:55.000000 murmuration-1.1/murmuration.egg-info/requires.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)       12 2023-08-09 02:55:55.000000 murmuration-1.1/murmuration.egg-info/top_level.txt
+-rw-r--r--   0 2ps       (1000) 2ps       (1000)        1 2023-08-09 02:55:55.000000 murmuration-1.1/murmuration.egg-info/zip-safe
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)      153 2023-08-09 02:55:55.482775 murmuration-1.1/setup.cfg
+-rwxr-xr-x   0 2ps       (1000) 2ps       (1000)     1388 2023-08-09 02:55:50.000000 murmuration-1.1/setup.py
```

### Comparing `murmuration-0.8/PKG-INFO` & `murmuration-1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: murmuration
-Version: 0.8
+Version: 1.1
 Summary: encryption primitives for use with aws
 Home-page: https://github.com/angry-penguins/murmuration
 Author: Preetam Shingavi
 Author-email: p.shingavi@yahoo.com
 License: BSD
 Keywords: aws python encryption cryptography kms
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: BSD License
@@ -110,9 +109,7 @@
 Once you have created that file, you can run tests using `make`:
 
 ```bash
 make test
 ```
 
 
-
-
```

### Comparing `murmuration-0.8/README.md` & `murmuration-1.1/README.md`

 * *Files identical despite different names*

### Comparing `murmuration-0.8/murmuration/aws.py` & `murmuration-1.1/murmuration/kms.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-from threading import local
-from boto3 import Session
+from boto3.session import Session
+from .helpers import as_bytes
+from .helpers import b64_str
+from .helpers import from_b64_str
+from .aws import kms_client
+from .helpers import prefix_alias
 
 
-cache = local()
-
-
-__all__ = [
-    'kms_client',
-    'cached_client',
-    'cached_session',
-    'threadlocal_var',
-]
-
-
-def threadlocal_var(varname, factory, *a, **k):
-    v = getattr(cache, varname, None)
-    if v is None:
-        v = factory(*a, **k)
-        setattr(cache, varname, v)
-    return v
+def encrypt_bytes(
+        plain_text: bytes,
+        alias: str,
+        region: str = None,
+        profile: str = None,
+        session: Session = None,
+        client=None) -> bytes:
+    client = kms_client(region, profile, session, client)
+    alias = prefix_alias(alias)
+    data = client.encrypt(KeyId=alias, Plaintext=plain_text)
+    return data['CiphertextBlob']
 
 
-def cached_session(region: str = None, profile: str = None):
-    key = f'{region}-{profile}'
-    sessions = threadlocal_var('session', dict)
-    session = sessions.get(key)
-    if not session:
-        if profile and profile in Session().available_profiles:
-            session = Session(region_name=region, profile_name=profile)
-        else:
-            session = Session(region_name=region)
-        sessions[key] = session
-    return session
+def decrypt_bytes(
+        cipher_text: bytes,
+        region: str = None,
+        profile: str = None,
+        session: Session = None,
+        client=None) -> bytes:
+    client = kms_client(region, profile, session, client)
+    data = client.decrypt(CiphertextBlob=cipher_text)
+    return data['Plaintext']
 
 
-def cached_client(client: str, region: str = None, profile: str = None):
-    key = f'{region}-{profile}-{client}'
-    clients = threadlocal_var('client', dict)
-    x = clients.get(key)
-    if not x:
-        session = cached_session(region, profile)
-        x = clients[key] = session.client(client)
-    return x
+def encrypt(
+        plain_text,
+        alias,
+        region: str = None,
+        profile: str = None,
+        session: Session = None,
+        client=None) -> str:
+    plain_text = as_bytes(plain_text)
+    data = encrypt_bytes(plain_text, alias, region, profile, session, client)
+    return b64_str(data)
 
 
-def kms_client(
+def decrypt(
+        cipher_text: str,
         region: str = None,
         profile: str = None,
-        session: Session = None):
-    if session:
-        return session.client('kms')
-    return cached_client('kms', region, profile)
+        session: Session = None,
+        client=None,):
+    cipher_text = from_b64_str(cipher_text)
+    data = decrypt_bytes(cipher_text, region, profile, session, client)
+    return data.decode('utf-8')
```

### Comparing `murmuration-0.8/murmuration/gcm.py` & `murmuration-1.1/murmuration/gcm.py`

 * *Files identical despite different names*

### Comparing `murmuration-0.8/murmuration/helpers.py` & `murmuration-1.1/murmuration/helpers.py`

 * *Files identical despite different names*

### Comparing `murmuration-0.8/murmuration/kms_wrap.py` & `murmuration-1.1/murmuration/kms_wrap.py`

 * *Files identical despite different names*

### Comparing `murmuration-0.8/murmuration/kms_wrapped.py` & `murmuration-1.1/murmuration/kms_wrapped.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,58 +11,62 @@
 
 
 def encrypt_bytes(
         plain_text: bytes,
         alias: str,
         region: str = None,
         profile: str = None,
-        session: Session = None) -> str:
-    client = kms_client(region, profile, session)
+        session: Session = None,
+        client=None) -> str:
+    client = kms_client(region, profile, session, client)
     alias = prefix_alias(alias)
     response = client.generate_data_key(KeyId=alias, KeySpec='AES_256')
     data_key = response['Plaintext']
     header = response['CiphertextBlob']
     value = gcm_encrypt(plain_text, data_key, auth_header=header)
     return value
 
 
 def decrypt_bytes(
         packed_value: str,
         region: str = None,
         profile: str = None,
-        session: Session = None) -> bytes:
+        session: Session = None,
+        client=None) -> bytes:
     pieces = packed_value.split('|', 1)
     if len(pieces) != 2:
         raise ValueError('Invalid wrapped secret, no data key found')
     wrapped_data_key = pieces[0]
     try:
         wrapped_data_key = from_b64_str(wrapped_data_key)
     except binascii.Error as ex:
         raise ValueError('data key is not properly base64 encoded') from ex
-    client = kms_client(region, profile, session)
+    client = kms_client(region, profile, session, client)
     try:
         response = client.decrypt(CiphertextBlob=wrapped_data_key)
     except ClientError as ex:
         raise ValueError(*ex.args) from ex
     data_key = response['Plaintext']
     plain_text = gcm_decrypt(packed_value, data_key)
     return plain_text
 
 
 def encrypt(
         plain_text,
         alias,
         region: str = None,
         profile: str = None,
-        session: Session = None) -> str:
+        session: Session = None,
+        client=None) -> str:
     plain_text = as_bytes(plain_text)
-    data = encrypt_bytes(plain_text, alias, region, profile, session)
+    data = encrypt_bytes(plain_text, alias, region, profile, session, client)
     return data
 
 
 def decrypt(
         packed_value: str,
         region: str = None,
         profile: str = None,
-        session: Session = None):
-    data = decrypt_bytes(packed_value, region, profile, session)
+        session: Session = None,
+        client=None):
+    data = decrypt_bytes(packed_value, region, profile, session, client)
     return data.decode('utf-8')
```

### Comparing `murmuration-0.8/murmuration.egg-info/PKG-INFO` & `murmuration-1.1/murmuration.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: murmuration
-Version: 0.8
+Version: 1.1
 Summary: encryption primitives for use with aws
 Home-page: https://github.com/angry-penguins/murmuration
 Author: Preetam Shingavi
 Author-email: p.shingavi@yahoo.com
 License: BSD
 Keywords: aws python encryption cryptography kms
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: BSD License
@@ -110,9 +109,7 @@
 Once you have created that file, you can run tests using `make`:
 
 ```bash
 make test
 ```
 
 
-
-
```

### Comparing `murmuration-0.8/setup.py` & `murmuration-1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 from setuptools import setup, find_packages
 
 
-version = '0.8'
+version = '1.1'
 with open('README.md', 'r') as f:
     long_description = f.read()
 
-setup(name='murmuration',
-      version=version,
-      description="encryption primitives for use with aws",
-      long_description=long_description,
-      long_description_content_type='text/markdown',
-      classifiers=[
-          'Development Status :: 5 - Production/Stable',
-          'Intended Audience :: Developers',
-          'Topic :: Software Development :: Libraries :: Python Modules',
-          'Programming Language :: Python :: 3',
-          'Programming Language :: Python :: 3.6',
-          'Programming Language :: Python :: 3.7',
-          'License :: OSI Approved :: BSD License',
-          'Topic :: Security :: Cryptography',
-          'Topic :: Utilities',
-      ], # Get strings from http://pypi.python.org/pypi?%3Aaction=list_classifiers
-      keywords='aws python encryption cryptography kms',
-      author='Preetam Shingavi',
-      author_email='p.shingavi@yahoo.com',
-      url='https://github.com/angry-penguins/murmuration',
-      license='BSD',
-      packages=find_packages(exclude=['ez_setup', 'examples', 'tests']),
-      include_package_data=True,
-      zip_safe=True,
-      install_requires=[
-          'boto3',
-          'pycryptodome>=3.7.3',
-      ])
+setup(
+    name='murmuration',
+    version=version,
+    description="encryption primitives for use with aws",
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    classifiers=[
+        'Development Status :: 5 - Production/Stable',
+        'Intended Audience :: Developers',
+        'Topic :: Software Development :: Libraries :: Python Modules',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'License :: OSI Approved :: BSD License',
+        'Topic :: Security :: Cryptography',
+        'Topic :: Utilities',
+    ], # Get strings from http://pypi.python.org/pypi?%3Aaction=list_classifiers
+    keywords='aws python encryption cryptography kms',
+    author='Preetam Shingavi',
+    author_email='p.shingavi@yahoo.com',
+    url='https://github.com/angry-penguins/murmuration',
+    license='BSD',
+    packages=find_packages(exclude=['ez_setup', 'examples', 'tests']),
+    include_package_data=True,
+    zip_safe=True,
+    entry_points={
+        'console_scripts': [
+            'kms_wrap = murmuration.kms_wrap:main',
+        ],
+    },
+    install_requires=[
+        'boto3',
+        'pycryptodome>=3.7.3',
+    ])
```

