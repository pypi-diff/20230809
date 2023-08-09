# Comparing `tmp/jaraco.crypto-3.1.0.tar.gz` & `tmp/jaraco.crypto-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.crypto-3.1.0.tar", last modified: Mon Aug  7 00:22:16 2023, max compression
+gzip compressed data, was "jaraco.crypto-3.1.1.tar", last modified: Wed Aug  9 02:49:10 2023, max compression
```

## Comparing `jaraco.crypto-3.1.0.tar` & `jaraco.crypto-3.1.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2023-08-07 00:22:16.053395 jaraco.crypto-3.1.0/
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)      133 2023-08-06 23:47:09.000000 jaraco.crypto-3.1.0/.coveragerc
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)      246 2022-09-11 16:31:36.000000 jaraco.crypto-3.1.0/.editorconfig
-drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2023-08-07 00:22:16.047963 jaraco.crypto-3.1.0/.github/
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)      148 2022-09-11 16:31:36.000000 jaraco.crypto-3.1.0/.github/dependabot.yml
-drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2023-08-07 00:22:16.048155 jaraco.crypto-3.1.0/.github/workflows/
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3146 2023-08-06 23:47:09.000000 jaraco.crypto-3.1.0/.github/workflows/main.yml
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)       81 2022-09-11 16:31:36.000000 jaraco.crypto-3.1.0/.pre-commit-config.yaml
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)      188 2023-08-06 23:47:09.000000 jaraco.crypto-3.1.0/.readthedocs.yaml
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1023 2023-08-06 23:47:09.000000 jaraco.crypto-3.1.0/LICENSE
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)      927 2023-08-07 00:22:03.000000 jaraco.crypto-3.1.0/NEWS.rst
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)     2031 2023-08-07 00:22:16.053497 jaraco.crypto-3.1.0/PKG-INFO
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1481 2023-08-06 23:47:09.000000 jaraco.crypto-3.1.0/README.rst
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1504 2023-08-06 23:57:22.000000 jaraco.crypto-3.1.0/certutil.py
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)      261 2023-08-07 00:13:38.000000 jaraco.crypto-3.1.0/conftest.py
-drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2023-08-07 00:22:16.048797 jaraco.crypto-3.1.0/docs/
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1203 2023-08-07 00:07:21.000000 jaraco.crypto-3.1.0/docs/conf.py
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)       78 2023-08-06 23:47:09.000000 jaraco.crypto-3.1.0/docs/history.rst
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)      910 2023-08-06 23:47:09.000000 jaraco.crypto-3.1.0/docs/index.rst
-drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2023-08-07 00:22:16.043575 jaraco.crypto-3.1.0/jaraco/
-drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2023-08-07 00:22:16.051658 jaraco.crypto-3.1.0/jaraco/crypto/
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)        0 2022-09-11 16:31:36.000000 jaraco.crypto-3.1.0/jaraco/crypto/__init__.py
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)    39889 2023-08-06 23:56:39.000000 jaraco.crypto-3.1.0/jaraco/crypto/blowfish.py
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)     2178 2023-08-07 00:10:08.000000 jaraco.crypto-3.1.0/jaraco/crypto/cert.py
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)     4785 2023-08-06 23:56:39.000000 jaraco.crypto-3.1.0/jaraco/crypto/cipher.py
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1835 2023-08-06 23:56:39.000000 jaraco.crypto-3.1.0/jaraco/crypto/digest.py
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)     3647 2023-08-07 00:12:12.000000 jaraco.crypto-3.1.0/jaraco/crypto/evp.py
-drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2023-08-07 00:22:16.052068 jaraco.crypto-3.1.0/jaraco/crypto/itsdangerous/
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)        0 2022-09-11 16:31:36.000000 jaraco.crypto-3.1.0/jaraco/crypto/itsdangerous/__init__.py
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)     2260 2023-08-06 23:56:39.000000 jaraco.crypto-3.1.0/jaraco/crypto/itsdangerous/compat.py
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1167 2023-08-06 23:56:39.000000 jaraco.crypto-3.1.0/jaraco/crypto/rand.py
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1395 2023-08-07 00:03:36.000000 jaraco.crypto-3.1.0/jaraco/crypto/support.py
-drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2023-08-07 00:22:16.053199 jaraco.crypto-3.1.0/jaraco/crypto/tests/
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)        0 2022-09-11 16:31:36.000000 jaraco.crypto-3.1.0/jaraco/crypto/tests/__init__.py
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1207 2022-09-11 16:31:36.000000 jaraco.crypto-3.1.0/jaraco/crypto/tests/test_cipher.py
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)      804 2023-08-06 23:52:24.000000 jaraco.crypto-3.1.0/jaraco/crypto/tests/test_digest.py
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)      561 2023-08-06 23:52:24.000000 jaraco.crypto-3.1.0/jaraco/crypto/tests/test_rand.py
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)      715 2022-09-11 16:31:36.000000 jaraco.crypto-3.1.0/jaraco/crypto/tests/test_threads.py
-drwxr-xr-x   0 jaraco   (697332) primarygroup (89939)        0 2023-08-07 00:22:16.049704 jaraco.crypto-3.1.0/jaraco.crypto.egg-info/
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)     2031 2023-08-07 00:22:16.000000 jaraco.crypto-3.1.0/jaraco.crypto.egg-info/PKG-INFO
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)      903 2023-08-07 00:22:16.000000 jaraco.crypto-3.1.0/jaraco.crypto.egg-info/SOURCES.txt
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)        1 2023-08-07 00:22:16.000000 jaraco.crypto-3.1.0/jaraco.crypto.egg-info/dependency_links.txt
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)      275 2023-08-07 00:22:16.000000 jaraco.crypto-3.1.0/jaraco.crypto.egg-info/requires.txt
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)        7 2023-08-07 00:22:16.000000 jaraco.crypto-3.1.0/jaraco.crypto.egg-info/top_level.txt
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)      154 2023-08-06 23:47:09.000000 jaraco.crypto-3.1.0/mypy.ini
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)      186 2023-08-06 23:47:09.000000 jaraco.crypto-3.1.0/pyproject.toml
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)      842 2023-08-06 23:47:09.000000 jaraco.crypto-3.1.0/pytest.ini
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)     1023 2023-08-07 00:22:16.053855 jaraco.crypto-3.1.0/setup.cfg
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)       44 2023-08-06 23:47:09.000000 jaraco.crypto-3.1.0/towncrier.toml
--rw-r--r--   0 jaraco   (697332) primarygroup (89939)      771 2023-08-06 23:47:09.000000 jaraco.crypto-3.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 02:49:10.642510 jaraco.crypto-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-09 02:48:46.000000 jaraco.crypto-3.1.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-08-09 02:48:46.000000 jaraco.crypto-3.1.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 02:49:10.634510 jaraco.crypto-3.1.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-09 02:48:46.000000 jaraco.crypto-3.1.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 02:49:10.634510 jaraco.crypto-3.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-08-09 02:48:46.000000 jaraco.crypto-3.1.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-09 02:48:46.000000 jaraco.crypto-3.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-09 02:48:46.000000 jaraco.crypto-3.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-08-09 02:48:46.000000 jaraco.crypto-3.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-08-09 02:48:46.000000 jaraco.crypto-3.1.1/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-08-09 02:49:10.642510 jaraco.crypto-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-08-09 02:48:46.000000 jaraco.crypto-3.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-08-09 02:48:46.000000 jaraco.crypto-3.1.1/certutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-09 02:48:46.000000 jaraco.crypto-3.1.1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 02:49:10.634510 jaraco.crypto-3.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-08-09 02:48:46.000000 jaraco.crypto-3.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-09 02:48:46.000000 jaraco.crypto-3.1.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-08-09 02:48:46.000000 jaraco.crypto-3.1.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 02:49:10.630510 jaraco.crypto-3.1.1/jaraco/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 02:49:10.638510 jaraco.crypto-3.1.1/jaraco/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-09 02:48:46.000000 jaraco.crypto-3.1.1/jaraco/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39889 2023-08-09 02:48:46.000000 jaraco.crypto-3.1.1/jaraco/crypto/blowfish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-08-09 02:48:46.000000 jaraco.crypto-3.1.1/jaraco/crypto/cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-08-09 02:48:46.000000 jaraco.crypto-3.1.1/jaraco/crypto/cipher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-08-09 02:48:46.000000 jaraco.crypto-3.1.1/jaraco/crypto/digest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-08-09 02:48:46.000000 jaraco.crypto-3.1.1/jaraco/crypto/evp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 02:49:10.638510 jaraco.crypto-3.1.1/jaraco/crypto/itsdangerous/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-09 02:48:46.000000 jaraco.crypto-3.1.1/jaraco/crypto/itsdangerous/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-08-09 02:48:46.000000 jaraco.crypto-3.1.1/jaraco/crypto/itsdangerous/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-08-09 02:48:46.000000 jaraco.crypto-3.1.1/jaraco/crypto/rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-08-09 02:48:46.000000 jaraco.crypto-3.1.1/jaraco/crypto/support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 02:49:10.642510 jaraco.crypto-3.1.1/jaraco/crypto/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-09 02:48:46.000000 jaraco.crypto-3.1.1/jaraco/crypto/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-08-09 02:48:46.000000 jaraco.crypto-3.1.1/jaraco/crypto/tests/test_cipher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-08-09 02:48:46.000000 jaraco.crypto-3.1.1/jaraco/crypto/tests/test_digest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-08-09 02:48:46.000000 jaraco.crypto-3.1.1/jaraco/crypto/tests/test_rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-08-09 02:48:46.000000 jaraco.crypto-3.1.1/jaraco/crypto/tests/test_threads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 02:49:10.634510 jaraco.crypto-3.1.1/jaraco.crypto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-08-09 02:49:10.000000 jaraco.crypto-3.1.1/jaraco.crypto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-08-09 02:49:10.000000 jaraco.crypto-3.1.1/jaraco.crypto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 02:49:10.000000 jaraco.crypto-3.1.1/jaraco.crypto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-08-09 02:49:10.000000 jaraco.crypto-3.1.1/jaraco.crypto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-09 02:49:10.000000 jaraco.crypto-3.1.1/jaraco.crypto.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-09 02:48:46.000000 jaraco.crypto-3.1.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-09 02:48:46.000000 jaraco.crypto-3.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-08-09 02:48:46.000000 jaraco.crypto-3.1.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-08-09 02:49:10.642510 jaraco.crypto-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-09 02:48:46.000000 jaraco.crypto-3.1.1/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-09 02:48:46.000000 jaraco.crypto-3.1.1/tox.ini
```

### Comparing `jaraco.crypto-3.1.0/.github/workflows/main.yml` & `jaraco.crypto-3.1.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `jaraco.crypto-3.1.0/LICENSE` & `jaraco.crypto-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jaraco.crypto-3.1.0/NEWS.rst` & `jaraco.crypto-3.1.1/NEWS.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v3.1.1
+======
+
+Bugfixes
+--------
+
+- Restored Windows support. (#4)
+
+
 v3.1.0
 ======
 
 Features
 --------
 
 - Require Python 3.8 or later.
```

### Comparing `jaraco.crypto-3.1.0/PKG-INFO` & `jaraco.crypto-3.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.crypto
-Version: 3.1.0
+Version: 3.1.1
 Summary: Cryptography support by jaraco
 Home-page: https://github.com/jaraco/jaraco.crypto
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jaraco.crypto-3.1.0/README.rst` & `jaraco.crypto-3.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `jaraco.crypto-3.1.0/certutil.py` & `jaraco.crypto-3.1.1/certutil.py`

 * *Files identical despite different names*

### Comparing `jaraco.crypto-3.1.0/docs/conf.py` & `jaraco.crypto-3.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaraco.crypto-3.1.0/docs/index.rst` & `jaraco.crypto-3.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `jaraco.crypto-3.1.0/jaraco/crypto/blowfish.py` & `jaraco.crypto-3.1.1/jaraco/crypto/blowfish.py`

 * *Files identical despite different names*

### Comparing `jaraco.crypto-3.1.0/jaraco/crypto/cert.py` & `jaraco.crypto-3.1.1/jaraco/crypto/cert.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,22 +39,22 @@
         ('ex_data', CRYPTO_EX_DATA),
     ]
 
 
 FILETYPE_PEM = 1
 FILETYPE_ASN1 = 2
 
-lib = find_library('libeay32') or find_library('libssl')
+lib = find_library('libcrypto') or find_library('libssl')
 assert lib, "Couldn't find OpenSSL"
 
 lib.BN_bn2hex.restype = ctypes.c_char_p
 
 
 class X509(ctypes.Structure):
-    _fields_ = []
+    _fields_ = []  # type: ignore
 
     def get_serial_number(self):
         asn1_i = lib.X509_get_serialNumber(ctypes.byref(self))
         bignum = lib.ASN1_INTEGER_to_BN(asn1_i, None)
         try:
             hex = lib.BN_bn2hex(bignum)
             result = int(hex, 16)
```

### Comparing `jaraco.crypto-3.1.0/jaraco/crypto/cipher.py` & `jaraco.crypto-3.1.1/jaraco/crypto/cipher.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     def finalize(self, data=None):
         if data is not None:
             self.update(data)
         self.finalized = True
         out = ctypes.create_string_buffer(evp.MAX_BLOCK_LENGTH)
         out_len = ctypes.c_int()
         res = evp.CipherFinal_ex(self, out, out_len)
-        if not res == 1:
+        if res != 1:
             raise CipherError("Error finalizing cipher")
         self.out_data.append(out.raw[: out_len.value])
         self.finalize = lambda: ''.join(self.out_data)
         return b''.join(self.out_data)
 
 
 _init_args = (
```

### Comparing `jaraco.crypto-3.1.0/jaraco/crypto/digest.py` & `jaraco.crypto-3.1.1/jaraco/crypto/digest.py`

 * *Files identical despite different names*

### Comparing `jaraco.crypto-3.1.0/jaraco/crypto/evp.py` & `jaraco.crypto-3.1.1/jaraco/crypto/evp.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     Copy the function by the given name from the EVP library into this
     namespace.
     """
     libname = 'EVP_' + name
     globals()[name] = getattr(lib, libname)
 
 
-lib = find_library('libeay32') or find_library('libssl')
+lib = find_library('libcrypto') or find_library('libssl')
 assert lib, "Couldn't find OpenSSL"
 
 # Define the argtypes and result types for the EVP functions
 list(
     map(
         _reg,
         'get_digestbyname DigestInit DigestInit_ex '
@@ -74,15 +74,20 @@
 def _set_digest_arg_types(DigestType, Digest):
     get_digestbyname.argtypes = (c_char_p,)
     get_digestbyname.restype = POINTER(DigestType)
     DigestInit.argtypes = (
         POINTER(Digest),
         POINTER(DigestType),
     )
-    DigestInit_ex.argtypes = lib.EVP_DigestInit.argtypes + (c_void_p,)
+    DigestInit_ex.argtypes = tuple(
+        itertools.chain(
+            lib.EVP_DigestInit.argtypes,
+            (c_void_p,),
+        )
+    )
     DigestInit_ex.restype = c_int
     DigestUpdate.argtypes = POINTER(Digest), c_char_p, c_int
     DigestUpdate.restype = c_int
     DigestFinal_ex.argtypes = (
         POINTER(Digest),
         c_char_p,
         POINTER(c_uint),
```

### Comparing `jaraco.crypto-3.1.0/jaraco/crypto/itsdangerous/compat.py` & `jaraco.crypto-3.1.1/jaraco/crypto/itsdangerous/compat.py`

 * *Files 13% similar despite different names*

```diff
@@ -54,16 +54,16 @@
     But if you call this compatibility wrapper instead, you get the
     desired result.
 
     >>> res, ts = frozen(unsign)(
     ...     signer, signed, max_age=5, return_timestamp=True)
     >>> res
     b'my string'
-    >>> ts
-    FakeDatetime(2019, 1, 23, 18, 44, 58)
+    >>> ts == datetime.datetime(2019, 1, 23, 18, 44, 58)
+    True
 
     And the signature does show as expired when it's supposed to be.
 
     >>> freeze_time('2019-01-23T18:45:58')(unsign)(signer, signed, max_age=5)
     Traceback (most recent call last):
     ...
     itsdangerous.exc.SignatureExpired: Signature age 60 > 5 seconds
```

### Comparing `jaraco.crypto-3.1.0/jaraco/crypto/rand.py` & `jaraco.crypto-3.1.1/jaraco/crypto/rand.py`

 * *Files identical despite different names*

### Comparing `jaraco.crypto-3.1.0/jaraco/crypto/support.py` & `jaraco.crypto-3.1.1/jaraco/crypto/support.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import ctypes
 import os
 import platform
 import subprocess
+import glob
 
 
 def find_lib_Linux(lib_name):
-    try:
-        lines = subprocess.check_output(['ldconfig', '-p'], text=True)
-    except TypeError:
-        lines = subprocess.check_output(['ldconfig', '-p'], text=True)
+    lines = subprocess.check_output(['ldconfig', '-p'], text=True, encoding='utf-8')
 
     for line in lines.splitlines():
         lib, _, rest = line.strip().partition(' ')
         _, _, path = rest.rpartition(' ')
         found_name, _, _ = lib.partition('.')
         if lib_name == found_name:
             return path
@@ -22,30 +20,43 @@
     func = globals().get(f'find_lib_{platform.system()}', find_lib_default)
     found = func(lib_name)
     return found and ctypes.cdll.LoadLibrary(found)
 
 
 def find_lib_default(lib_name):
     """
-    Given a name like libeay32, find the best match.
+    Given a name like libcrypto, find the best match.
     """
     # todo, allow the target environment to customize this behavior
     roots = [
-        'c:\\Program Files\\OpenSSL\\',
-        '\\OpenSSL-Win64',
         '/usr/local/opt/openssl/lib/',
         '/opt/homebrew/lib/',
     ]
-    ext = (
-        '.dll'
-        if platform.system() == 'Windows'
-        else '.dylib'
-        if platform.system() == 'Darwin'
-        else '.so'
-    )
+    ext = '.dylib' if platform.system() == 'Darwin' else '.so'
     filename = lib_name + ext
     return next(_find_file(filename, roots), None)
 
 
+def find_lib_Windows(lib_name):
+    """
+    Default OpenSSL installs to the Windows system folder and are
+    reachable without a path or extension, but must have the right
+    name.
+    """
+    heuristic_paths = [
+        'C:\\Program Files\\OpenSSL',
+        '\\OpenSSL-Win64',
+        'C:\\Program Files\\OpenSSL-Win64-ARM',
+    ]
+    search_paths = os.environ['PATH'].split(os.pathsep) + heuristic_paths
+    names = [
+        name
+        for path in search_paths
+        for name in glob.glob(path + os.sep + f'{lib_name}*.dll')
+    ]
+
+    return next(iter(names), None)
+
+
 def _find_file(filename, roots):
     candidates = (os.path.join(root, filename) for root in roots)
     return filter(os.path.exists, candidates)
```

### Comparing `jaraco.crypto-3.1.0/jaraco/crypto/tests/test_cipher.py` & `jaraco.crypto-3.1.1/jaraco/crypto/tests/test_cipher.py`

 * *Files identical despite different names*

### Comparing `jaraco.crypto-3.1.0/jaraco/crypto/tests/test_digest.py` & `jaraco.crypto-3.1.1/jaraco/crypto/tests/test_digest.py`

 * *Files identical despite different names*

### Comparing `jaraco.crypto-3.1.0/jaraco/crypto/tests/test_rand.py` & `jaraco.crypto-3.1.1/jaraco/crypto/tests/test_rand.py`

 * *Files identical despite different names*

### Comparing `jaraco.crypto-3.1.0/jaraco/crypto/tests/test_threads.py` & `jaraco.crypto-3.1.1/jaraco/crypto/tests/test_threads.py`

 * *Files identical despite different names*

### Comparing `jaraco.crypto-3.1.0/jaraco.crypto.egg-info/PKG-INFO` & `jaraco.crypto-3.1.1/jaraco.crypto.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.crypto
-Version: 3.1.0
+Version: 3.1.1
 Summary: Cryptography support by jaraco
 Home-page: https://github.com/jaraco/jaraco.crypto
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jaraco.crypto-3.1.0/jaraco.crypto.egg-info/SOURCES.txt` & `jaraco.crypto-3.1.1/jaraco.crypto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaraco.crypto-3.1.0/pytest.ini` & `jaraco.crypto-3.1.1/pytest.ini`

 * *Files identical despite different names*

### Comparing `jaraco.crypto-3.1.0/setup.cfg` & `jaraco.crypto-3.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 	python_implementation != "PyPy"
 	pytest-cov
 	pytest-mypy >= 0.9.1; \
 	python_implementation != "PyPy"
 	pytest-enabler >= 2.2
 	pytest-ruff
 	
-	itsdangerous
+	itsdangerous < 2
 	freezegun
 docs = 
 	sphinx >= 3.5
 	jaraco.packaging >= 9.3
 	rst.linker >= 1.9
 	furo
 	sphinx-lint
```

### Comparing `jaraco.crypto-3.1.0/tox.ini` & `jaraco.crypto-3.1.1/tox.ini`

 * *Files identical despite different names*

