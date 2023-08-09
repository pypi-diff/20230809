# Comparing `tmp/scitokens-1.7.4.tar.gz` & `tmp/scitokens-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scitokens-1.7.4.tar", last modified: Tue Nov 22 14:15:20 2022, max compression
+gzip compressed data, was "scitokens-1.8.0.tar", last modified: Wed Aug  9 01:17:31 2023, max compression
```

## Comparing `scitokens-1.7.4.tar` & `scitokens-1.8.0.tar`

### file list

```diff
@@ -1,46 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 14:15:20.881742 scitokens-1.7.4/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-11-22 14:15:11.000000 scitokens-1.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-11-22 14:15:11.000000 scitokens-1.7.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    10928 2022-11-22 14:15:20.881742 scitokens-1.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9815 2022-11-22 14:15:11.000000 scitokens-1.7.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 14:15:20.877742 scitokens-1.7.4/configs/
--rw-r--r--   0 runner    (1001) docker     (121)     5636 2022-11-22 14:15:11.000000 scitokens-1.7.4/configs/python-scitokens.spec
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-11-22 14:15:11.000000 scitokens-1.7.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-11-22 14:15:20.881742 scitokens-1.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2565 2022-11-22 14:15:11.000000 scitokens-1.7.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 14:15:20.877742 scitokens-1.7.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 14:15:20.881742 scitokens-1.7.4/src/scitokens/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-22 14:15:11.000000 scitokens-1.7.4/src/scitokens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    25971 2022-11-22 14:15:11.000000 scitokens-1.7.4/src/scitokens/scitokens.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 14:15:20.881742 scitokens-1.7.4/src/scitokens/tools/
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-11-22 14:15:11.000000 scitokens-1.7.4/src/scitokens/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7318 2022-11-22 14:15:11.000000 scitokens-1.7.4/src/scitokens/tools/admin_create_key.py
--rw-r--r--   0 runner    (1001) docker     (121)     1777 2022-11-22 14:15:11.000000 scitokens-1.7.4/src/scitokens/tools/admin_create_token.py
--rw-r--r--   0 runner    (1001) docker     (121)     1629 2022-11-22 14:15:11.000000 scitokens-1.7.4/src/scitokens/urltools.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 14:15:20.881742 scitokens-1.7.4/src/scitokens/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     1037 2022-11-22 14:15:11.000000 scitokens-1.7.4/src/scitokens/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2878 2022-11-22 14:15:11.000000 scitokens-1.7.4/src/scitokens/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1162 2022-11-22 14:15:11.000000 scitokens-1.7.4/src/scitokens/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)    14325 2022-11-22 14:15:11.000000 scitokens-1.7.4/src/scitokens/utils/keycache.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 14:15:20.881742 scitokens-1.7.4/src/scitokens.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10928 2022-11-22 14:15:20.000000 scitokens-1.7.4/src/scitokens.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-11-22 14:15:20.000000 scitokens-1.7.4/src/scitokens.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-22 14:15:20.000000 scitokens-1.7.4/src/scitokens.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-11-22 14:15:20.000000 scitokens-1.7.4/src/scitokens.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-11-22 14:15:20.000000 scitokens-1.7.4/src/scitokens.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-11-22 14:15:20.000000 scitokens-1.7.4/src/scitokens.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 14:15:20.881742 scitokens-1.7.4/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     4415 2022-11-22 14:15:11.000000 scitokens-1.7.4/tests/create_sample_token.py
--rw-r--r--   0 runner    (1001) docker     (121)     3978 2022-11-22 14:15:11.000000 scitokens-1.7.4/tests/create_webserver.py
--rw-r--r--   0 runner    (1001) docker     (121)      215 2022-11-22 14:15:11.000000 scitokens-1.7.4/tests/load_token.py
--rw-r--r--   0 runner    (1001) docker     (121)      559 2022-11-22 14:15:11.000000 scitokens-1.7.4/tests/sample_ecdsa_keypair.pem
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-11-22 14:15:11.000000 scitokens-1.7.4/tests/simple_ec_private_key.pem
--rw-r--r--   0 runner    (1001) docker     (121)     1674 2022-11-22 14:15:11.000000 scitokens-1.7.4/tests/simple_private_key.pem
--rw-r--r--   0 runner    (1001) docker     (121)    11647 2022-11-22 14:15:11.000000 scitokens-1.7.4/tests/test_admin_create_key.py
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-11-22 14:15:11.000000 scitokens-1.7.4/tests/test_config.ini
--rw-r--r--   0 runner    (1001) docker     (121)     2573 2022-11-22 14:15:11.000000 scitokens-1.7.4/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (121)    17134 2022-11-22 14:15:11.000000 scitokens-1.7.4/tests/test_create_scitoken.py
--rw-r--r--   0 runner    (1001) docker     (121)     8359 2022-11-22 14:15:11.000000 scitokens-1.7.4/tests/test_keycache.py
--rw-r--r--   0 runner    (1001) docker     (121)    13731 2022-11-22 14:15:11.000000 scitokens-1.7.4/tests/test_scitokens.py
--rw-r--r--   0 runner    (1001) docker     (121)     1369 2022-11-22 14:15:11.000000 scitokens-1.7.4/tests/test_urltools.py
--rw-r--r--   0 runner    (1001) docker     (121)     3868 2022-11-22 14:15:11.000000 scitokens-1.7.4/tests/test_with_http.py
+drwxr-xr-x   0 derekweitzel   (501) staff       (20)        0 2023-08-09 01:17:31.792981 scitokens-1.8.0/
+-rw-r--r--   0 derekweitzel   (501) staff       (20)    11357 2023-08-09 01:15:06.000000 scitokens-1.8.0/LICENSE
+-rw-r--r--   0 derekweitzel   (501) staff       (20)      101 2023-08-09 01:15:06.000000 scitokens-1.8.0/MANIFEST.in
+-rw-r--r--   0 derekweitzel   (501) staff       (20)    12455 2023-08-09 01:17:31.793096 scitokens-1.8.0/PKG-INFO
+-rw-r--r--   0 derekweitzel   (501) staff       (20)    11342 2023-08-09 01:15:06.000000 scitokens-1.8.0/README.rst
+drwxr-xr-x   0 derekweitzel   (501) staff       (20)        0 2023-08-09 01:17:31.779574 scitokens-1.8.0/configs/
+-rw-r--r--   0 derekweitzel   (501) staff       (20)     5948 2023-08-09 01:15:06.000000 scitokens-1.8.0/configs/python-scitokens.spec
+-rw-r--r--   0 derekweitzel   (501) staff       (20)       81 2023-08-09 01:15:06.000000 scitokens-1.8.0/pyproject.toml
+-rw-r--r--   0 derekweitzel   (501) staff       (20)       74 2023-08-09 01:17:31.793497 scitokens-1.8.0/setup.cfg
+-rw-r--r--   0 derekweitzel   (501) staff       (20)     2636 2023-08-09 01:15:06.000000 scitokens-1.8.0/setup.py
+drwxr-xr-x   0 derekweitzel   (501) staff       (20)        0 2023-08-09 01:17:31.776854 scitokens-1.8.0/src/
+drwxr-xr-x   0 derekweitzel   (501) staff       (20)        0 2023-08-09 01:17:31.780784 scitokens-1.8.0/src/scitokens/
+-rw-r--r--   0 derekweitzel   (501) staff       (20)      179 2023-08-09 01:15:06.000000 scitokens-1.8.0/src/scitokens/__init__.py
+-rw-r--r--   0 derekweitzel   (501) staff       (20)    26088 2023-08-09 01:15:06.000000 scitokens-1.8.0/src/scitokens/scitokens.py
+drwxr-xr-x   0 derekweitzel   (501) staff       (20)        0 2023-08-09 01:17:31.784577 scitokens-1.8.0/src/scitokens/tools/
+-rw-r--r--   0 derekweitzel   (501) staff       (20)       42 2023-08-09 01:15:06.000000 scitokens-1.8.0/src/scitokens/tools/__init__.py
+-rw-r--r--   0 derekweitzel   (501) staff       (20)     7318 2023-08-09 01:15:06.000000 scitokens-1.8.0/src/scitokens/tools/admin_create_key.py
+-rw-r--r--   0 derekweitzel   (501) staff       (20)     2204 2023-08-09 01:15:06.000000 scitokens-1.8.0/src/scitokens/tools/admin_create_token.py
+-rw-r--r--   0 derekweitzel   (501) staff       (20)     2129 2023-08-09 01:15:06.000000 scitokens-1.8.0/src/scitokens/tools/verify_token.py
+-rw-r--r--   0 derekweitzel   (501) staff       (20)     1791 2023-08-09 01:15:06.000000 scitokens-1.8.0/src/scitokens/urltools.py
+drwxr-xr-x   0 derekweitzel   (501) staff       (20)        0 2023-08-09 01:17:31.786847 scitokens-1.8.0/src/scitokens/utils/
+-rw-r--r--   0 derekweitzel   (501) staff       (20)     1037 2023-08-09 01:15:06.000000 scitokens-1.8.0/src/scitokens/utils/__init__.py
+-rw-r--r--   0 derekweitzel   (501) staff       (20)     2878 2023-08-09 01:15:06.000000 scitokens-1.8.0/src/scitokens/utils/config.py
+-rw-r--r--   0 derekweitzel   (501) staff       (20)      773 2023-08-09 01:15:06.000000 scitokens-1.8.0/src/scitokens/utils/demo.py
+-rw-r--r--   0 derekweitzel   (501) staff       (20)     1162 2023-08-09 01:15:06.000000 scitokens-1.8.0/src/scitokens/utils/errors.py
+-rw-r--r--   0 derekweitzel   (501) staff       (20)    14306 2023-08-09 01:15:06.000000 scitokens-1.8.0/src/scitokens/utils/keycache.py
+-rw-r--r--   0 derekweitzel   (501) staff       (20)     2933 2023-08-09 01:15:06.000000 scitokens-1.8.0/src/scitokens/utils/scitokens_protect.py
+drwxr-xr-x   0 derekweitzel   (501) staff       (20)        0 2023-08-09 01:17:31.783008 scitokens-1.8.0/src/scitokens.egg-info/
+-rw-r--r--   0 derekweitzel   (501) staff       (20)    12455 2023-08-09 01:17:31.000000 scitokens-1.8.0/src/scitokens.egg-info/PKG-INFO
+-rw-r--r--   0 derekweitzel   (501) staff       (20)     1124 2023-08-09 01:17:31.000000 scitokens-1.8.0/src/scitokens.egg-info/SOURCES.txt
+-rw-r--r--   0 derekweitzel   (501) staff       (20)        1 2023-08-09 01:17:31.000000 scitokens-1.8.0/src/scitokens.egg-info/dependency_links.txt
+-rw-r--r--   0 derekweitzel   (501) staff       (20)      215 2023-08-09 01:17:31.000000 scitokens-1.8.0/src/scitokens.egg-info/entry_points.txt
+-rw-r--r--   0 derekweitzel   (501) staff       (20)       50 2023-08-09 01:17:31.000000 scitokens-1.8.0/src/scitokens.egg-info/requires.txt
+-rw-r--r--   0 derekweitzel   (501) staff       (20)       10 2023-08-09 01:17:31.000000 scitokens-1.8.0/src/scitokens.egg-info/top_level.txt
+drwxr-xr-x   0 derekweitzel   (501) staff       (20)        0 2023-08-09 01:17:31.792679 scitokens-1.8.0/tests/
+-rw-r--r--   0 derekweitzel   (501) staff       (20)     4415 2023-08-09 01:15:06.000000 scitokens-1.8.0/tests/create_sample_token.py
+-rw-r--r--   0 derekweitzel   (501) staff       (20)     3978 2023-08-09 01:15:06.000000 scitokens-1.8.0/tests/create_webserver.py
+-rw-r--r--   0 derekweitzel   (501) staff       (20)      215 2023-08-09 01:15:06.000000 scitokens-1.8.0/tests/load_token.py
+-rw-r--r--   0 derekweitzel   (501) staff       (20)      559 2023-08-09 01:15:06.000000 scitokens-1.8.0/tests/sample_ecdsa_keypair.pem
+-rw-r--r--   0 derekweitzel   (501) staff       (20)      242 2023-08-09 01:15:06.000000 scitokens-1.8.0/tests/simple_ec_private_key.pem
+-rw-r--r--   0 derekweitzel   (501) staff       (20)     1674 2023-08-09 01:15:06.000000 scitokens-1.8.0/tests/simple_private_key.pem
+-rw-r--r--   0 derekweitzel   (501) staff       (20)    11647 2023-08-09 01:15:06.000000 scitokens-1.8.0/tests/test_admin_create_key.py
+-rw-r--r--   0 derekweitzel   (501) staff       (20)       33 2023-08-09 01:15:06.000000 scitokens-1.8.0/tests/test_config.ini
+-rw-r--r--   0 derekweitzel   (501) staff       (20)     2573 2023-08-09 01:15:06.000000 scitokens-1.8.0/tests/test_config.py
+-rw-r--r--   0 derekweitzel   (501) staff       (20)    18089 2023-08-09 01:15:06.000000 scitokens-1.8.0/tests/test_create_scitoken.py
+-rw-r--r--   0 derekweitzel   (501) staff       (20)     2612 2023-08-09 01:15:06.000000 scitokens-1.8.0/tests/test_demo.py
+-rw-r--r--   0 derekweitzel   (501) staff       (20)     9605 2023-08-09 01:15:06.000000 scitokens-1.8.0/tests/test_keycache.py
+-rw-r--r--   0 derekweitzel   (501) staff       (20)    13731 2023-08-09 01:15:06.000000 scitokens-1.8.0/tests/test_scitokens.py
+-rw-r--r--   0 derekweitzel   (501) staff       (20)     1369 2023-08-09 01:15:06.000000 scitokens-1.8.0/tests/test_urltools.py
+-rw-r--r--   0 derekweitzel   (501) staff       (20)     3868 2023-08-09 01:15:06.000000 scitokens-1.8.0/tests/test_with_http.py
```

### Comparing `scitokens-1.7.4/LICENSE` & `scitokens-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scitokens-1.7.4/PKG-INFO` & `scitokens-1.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scitokens
-Version: 1.7.4
+Version: 1.8.0
 Summary: SciToken reference implementation library
 Home-page: https://scitokens.org
 Author: Brian Bockelman
 Author-email: team@scitokens.org
 License: Apache-2.0
 Project-URL: Documentation, https://scitokens.readthedocs.io/
 Project-URL: Issue Tracker, https://github.com/scitokens/scitokens/issues
@@ -219,14 +219,51 @@
     >>> enf.test(stoken, "write", "/store/user/bbockelm/foo")
     True
 
 The ``test`` method uses the SciTokens built-in path parsing to validate the
 authorization.  The ``generate_acls`` method allows the caller to cache
 the ACL information from the token.
 
+Creating Sample Tokens
+----------------------
+
+Typically, an access token is generated during an OAuth2 workflow to facilitate 
+authentication and authorization. However, for testing and experimentation purposes, 
+`the demo token generator <https://demo.scitokens.org/>`__ provides users with the
+ability to create sample tokens with customized payload:
+
+::
+    
+    >>> payload = {"sub": "<email adress>", "scope": "read:/protected"}
+    >>> token = scitokens.utils.demo.token(payload)
+
+The ``token`` method makes a request to the generator to create a serialized token 
+for the specified payload. Users can also retrieve a parsed token by calling the 
+``parsed_token`` method, which returns a SciToken object corresponding to the 
+token. The object contains the decoded token data, including the claims and signature. 
+
+Decorator
+-------------
+
+This protect decorator is designed to be used with a `flask <https://flask.palletsprojects.com/>`_ application. It can be used like:
+
+.. code-block:: python
+
+    @scitokens_protect.protect(audience="https://demo.scitokens.org", scope="read:/secret", issuer="https://demo.scitokens.org")
+    def Secret(token: SciToken):
+        # ... token is now available.
+
+The possible arguments are:
+
+- ``audience`` (str or list): Audience expected in the client token
+- ``scope`` (str): Scope required to access the function
+- ``issuer`` (str): The issuer to require of the client token
+
+The protected function can optionally take an argument ``token``, which is the parsed SciToken object.
+
 Configuration
 -------------
 
 An optional configuration file can be provided that will alter the behavior of 
 the SciTokens library.  Configuration options include:
 
 ================== ========================================================================================
```

### Comparing `scitokens-1.7.4/README.rst` & `scitokens-1.8.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -191,14 +191,51 @@
     >>> enf.test(stoken, "write", "/store/user/bbockelm/foo")
     True
 
 The ``test`` method uses the SciTokens built-in path parsing to validate the
 authorization.  The ``generate_acls`` method allows the caller to cache
 the ACL information from the token.
 
+Creating Sample Tokens
+----------------------
+
+Typically, an access token is generated during an OAuth2 workflow to facilitate 
+authentication and authorization. However, for testing and experimentation purposes, 
+`the demo token generator <https://demo.scitokens.org/>`__ provides users with the
+ability to create sample tokens with customized payload:
+
+::
+    
+    >>> payload = {"sub": "<email adress>", "scope": "read:/protected"}
+    >>> token = scitokens.utils.demo.token(payload)
+
+The ``token`` method makes a request to the generator to create a serialized token 
+for the specified payload. Users can also retrieve a parsed token by calling the 
+``parsed_token`` method, which returns a SciToken object corresponding to the 
+token. The object contains the decoded token data, including the claims and signature. 
+
+Decorator
+-------------
+
+This protect decorator is designed to be used with a `flask <https://flask.palletsprojects.com/>`_ application. It can be used like:
+
+.. code-block:: python
+
+    @scitokens_protect.protect(audience="https://demo.scitokens.org", scope="read:/secret", issuer="https://demo.scitokens.org")
+    def Secret(token: SciToken):
+        # ... token is now available.
+
+The possible arguments are:
+
+- ``audience`` (str or list): Audience expected in the client token
+- ``scope`` (str): Scope required to access the function
+- ``issuer`` (str): The issuer to require of the client token
+
+The protected function can optionally take an argument ``token``, which is the parsed SciToken object.
+
 Configuration
 -------------
 
 An optional configuration file can be provided that will alter the behavior of 
 the SciTokens library.  Configuration options include:
 
 ================== ========================================================================================
```

### Comparing `scitokens-1.7.4/configs/python-scitokens.spec` & `scitokens-1.8.0/configs/python-scitokens.spec`

 * *Files 5% similar despite different names*

```diff
@@ -1,69 +1,89 @@
 # Created by pyp2rpm-3.2.3
 %global pypi_name scitokens
 
 Name:           python-%{pypi_name}
-Version:        1.7.2
+Version:        1.8.0
 Release:        1%{?dist}
 Summary:        SciToken reference implementation library
 
-License:        Apache 2.0
+License:        Apache-2.0
 URL:            https://scitokens.org
-Source0:        https://files.pythonhosted.org/packages/source/s/%{pypi_name}/%{pypi_name}-%{version}.tar.gz
+Source0:        %{pypi_source %{pypi_name}}
 BuildArch:      noarch
 
 # build requirements
 BuildRequires:  python3-devel
-BuildRequires:  python%{python3_pkgversion}-setuptools
+BuildRequires:  python3-setuptools
 
 # test requirements
+%if 0%{?rhel} == 7
 BuildRequires:  python%{python3_pkgversion}-cryptography
 BuildRequires:  python%{python3_pkgversion}-pytest
 BuildRequires:  python%{python3_pkgversion}-jwt >= 1.6.1
+BuildRequires:  python%{python3_pkgversion}-requests
+%else
+BuildRequires:  python3-cryptography
+BuildRequires:  python3-pytest
+BuildRequires:  python3-jwt >= 1.6.1
+BuildRequires:  python3-requests
+%endif
 
 %description
 SciToken reference implementation library
 
-%package -n     python%{python3_pkgversion}-%{pypi_name}
-Requires:       python%{python3_pkgversion}-jwt >= 1.6.1
-Requires:       python%{python3_pkgversion}-cryptography
+%package -n     python3-%{pypi_name}
 Obsoletes:      python3-scitokens < 1.6.2-2
 Summary:        %{summary}
-%{?python_provide:%python_provide python%{python3_pkgversion}-%{pypi_name}}
 
-%description -n python%{python3_pkgversion}-%{pypi_name}
+%description -n python3-%{pypi_name}
 SciToken reference implementation library
 
 %prep
 %autosetup -n %{pypi_name}-%{version}
 # Remove bundled egg-info
 rm -rf %{pypi_name}.egg-info
 
 %build
 %py3_build
 
 %install
-# Must do the subpackages' install first because the scripts in /usr/bin are
-# overwritten with every setup.py install.
 %py3_install
 
 %check
+%if 0%{?rhel} == 7
 export PYTHONPATH="%{buildroot}%{python3_sitelib}"
 (cd tests/ && %{__python3} -m pytest --verbose -ra .)
+%else
+%pytest --verbose -ra tests/
+%endif
 
-%files -n python%{python3_pkgversion}-%{pypi_name}
+%files -n python3-%{pypi_name}
 %license LICENSE
-%{python3_sitelib}/%{pypi_name}
+%{python3_sitelib}/%{pypi_name}/
 %{python3_sitelib}/%{pypi_name}-%{version}-py*.egg-info
 %doc README.rst
 %{_bindir}/scitokens-admin-create-key
 %{_bindir}/scitokens-admin-create-token
-
+%{_bindir}/scitokens-verify-token
 
 %changelog
+* Tue Aug 08 2023 Derek Weitzel <dweitzel@unl.edu> - 1.8.0-1
+- Add demo token issuer convenience functions
+- Improve testing of deserialization
+- Add RPM improvements for EPEL
+
+* Tue Nov 22 2022 Derek Weitzel <dweitzel@unl.edu> - 1.7.4-1
+- Fix the version within the package
+
+* Tue Nov 22 2022 Derek Weitzel <dweitzel@unl.edu> - 1.7.3-1
+- Remove aud enforcement from deserailize function
+- Add configuration for readthedocs
+- Remove six dependency
+
 * Tue Oct 04 2022 Derek Weitzel <dweitzel@unl.edu> - 1.7.2-1
 - Documentation updates
 
 * Wed Sep 28 2022 Derek Weitzel <dweitzel@unl.edu> - 1.7.1-1
 - Documentation updates
 - Fix setup tools and add pyproject.toml
```

### Comparing `scitokens-1.7.4/setup.py` & `scitokens-1.8.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,22 +54,23 @@
         "scitokens.tools",
         "scitokens.utils",
     ],
     entry_points={
         "console_scripts": [
             "scitokens-admin-create-key=scitokens.tools.admin_create_key:main",
             "scitokens-admin-create-token=scitokens.tools.admin_create_token:main",
+            "scitokens-verify-token=scitokens.tools.verify_token:main",
         ],
     },
     # requirements
     python_requires=">=3.5",
     install_requires=[
         'cryptography',
         'PyJWT>=1.6.1',
-        'setuptools'
+        'requests',
     ],
     extras_require={
         "docs": [
             "Sphinx",
         ],
     },
     # classifiers
```

### Comparing `scitokens-1.7.4/src/scitokens/scitokens.py` & `scitokens-1.8.0/src/scitokens/scitokens.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,14 +290,17 @@
                                         audience=audience,
                                         options={"verify_signature": False,
                                                  "verify_aud": False})
         
         # Get the public key from the issuer
         keycache = KeyCache.KeyCache().getinstance()
         if public_key == None:
+            if 'iss' not in unverified_payload:
+                raise MissingIssuerException('Issuer not provided')
+
             issuer_public_key = keycache.getkeyinfo(unverified_payload['iss'],
                                 key_id=unverified_headers['kid'] if 'kid' in unverified_headers else None,
                                 insecure=insecure)
         else:
             issuer_public_key = load_pem_public_key(public_key, backend=backends.default_backend())
         
         claims = jwt.decode(serialized_token, issuer_public_key, algorithms=['RS256', 'ES256'],
```

### Comparing `scitokens-1.7.4/src/scitokens/tools/admin_create_key.py` & `scitokens-1.8.0/src/scitokens/tools/admin_create_key.py`

 * *Files identical despite different names*

### Comparing `scitokens-1.7.4/src/scitokens/tools/admin_create_token.py` & `scitokens-1.8.0/src/scitokens/tools/admin_create_token.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,20 +6,23 @@
 import argparse
 
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.backends import default_backend
 
 import scitokens
 
+import scitokens.utils.demo
+
 
 def add_args():
     """
     Generate the ArgumentParser object for the CLI.
     """
     parser = argparse.ArgumentParser(description='Create a new SciToken')
+    parser.add_argument('--demo', action='store_true', help='The payload that needs encrypting')
     parser.add_argument('claims', metavar='C', type=str, nargs='+',
                         help='Claims in the format key=value')
     parser.add_argument('--keyfile',
                         help='Location of the private key file')
     parser.add_argument('--key_id', help='The string key identifier')
     parser.add_argument('--issuer', help="Issuer for the token")
     parser.add_argument('--lifetime', help="Lifetime of the token, in seconds from now. Default: 1200 seconds (20 minutes)",
@@ -30,29 +33,37 @@
 
 
 def main():
     """
     Given a set of command line parameters, generate a corresponding SciToken.
     """
     args = add_args()
+    # If the demo option is called
+    if args.demo:
+        payload = {}
+        for claim in args.claims:
+            (key, value) = claim.split('=', 1)
+            payload[key] = value
+        print(scitokens.utils.demo.token(payload))
+
+    else:
+        with open(args.keyfile, "r") as file_pointer:
+            private_key_contents = file_pointer.read()
+
+        loaded_private_key = serialization.load_pem_private_key(
+            private_key_contents.encode(),
+            password=None, # Hey, it's a sample file committed to disk...
+            backend=default_backend()
+        )
+
+        token = scitokens.SciToken(key=loaded_private_key, key_id=args.key_id)
+
+        for claim in args.claims:
+            (key, value) = claim.split('=', 1)
+            token.update_claims({key: value})
 
-    with open(args.keyfile, "r") as file_pointer:
-        private_key_contents = file_pointer.read()
-
-    loaded_private_key = serialization.load_pem_private_key(
-        private_key_contents.encode(),
-        password=None, # Hey, it's a sample file committed to disk...
-        backend=default_backend()
-    )
-
-    token = scitokens.SciToken(key=loaded_private_key, key_id=args.key_id)
-
-    for claim in args.claims:
-        (key, value) = claim.split('=', 1)
-        token.update_claims({key: value})
-
-    serialized_token = token.serialize(issuer=args.issuer, lifetime=args.lifetime)
-    print(serialized_token.decode())
+        serialized_token = token.serialize(issuer=args.issuer, lifetime=args.lifetime)
+        print(serialized_token.decode())
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `scitokens-1.7.4/src/scitokens/urltools.py` & `scitokens-1.8.0/src/scitokens/urltools.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 
 def unquote(text, exceptions=''):
     """Unquote a text but ignore the exceptions.
     >>> unquote('foo%23bar')
     'foo#bar'
     >>> unquote('foo%23bar', ['#'])
     'foo%23bar'
+
+    Unmodified function from python-urltools
     """
     if not text:
         if text is None:
             raise TypeError('None object cannot be unquoted')
         else:
             return text
     if '%' not in text:
@@ -48,14 +50,18 @@
     return ''.join(res)
 
 
 def normalize_path(path):
     """Normalize path: collapse etc.
     >>> normalize_path('/a/b///c')
     '/a/b/c'
+
+    Modified function from python-urltools to include reducing the starting slashes, ie
+    "//a/b/c" -> "/a/b/c"
+
     """
     if path in ['//', '/', '']:
         return '/'
     npath = posixpath.normpath(unquote(path, exceptions='/?+#'))
     if path[-1] == '/' and npath != '/':
         npath += '/'
     while npath.startswith("//"):
```

### Comparing `scitokens-1.7.4/src/scitokens/utils/__init__.py` & `scitokens-1.8.0/src/scitokens/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `scitokens-1.7.4/src/scitokens/utils/config.py` & `scitokens-1.8.0/src/scitokens/utils/config.py`

 * *Files identical despite different names*

### Comparing `scitokens-1.7.4/src/scitokens/utils/errors.py` & `scitokens-1.8.0/src/scitokens/utils/errors.py`

 * *Files identical despite different names*

### Comparing `scitokens-1.7.4/src/scitokens/utils/keycache.py` & `scitokens-1.8.0/src/scitokens/utils/keycache.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,23 +2,16 @@
 """
 A module for effectively caching the public keys of various token issuer endpoints.
 """
 
 import os
 import sqlite3
 import time
-import pkg_resources  # part of setuptools
 import re
 import logging
-try:
-    PKG_VERSION = pkg_resources.require("scitokens")[0].version
-except pkg_resources.DistributionNotFound as error:
-    # During testing, scitokens won't be installed, so requiring it will fail
-    # Instead, fake it
-    PKG_VERSION = '1.0.0'
 
 try:
     import urllib.request as request
 except ImportError:
     import urllib2 as request
 
 try:
@@ -225,14 +218,16 @@
     def _get_issuer_publickey(issuer, key_id=None, insecure=False):
         """
         :return: Tuple containing (public_key, cache_lifetime).  Cache_lifetime how
             the public key is valid
         """
 
         # Set the user agent so Cloudflare isn't mad at us
+        # Import the __version__ value in scitokens for the scitokens version
+        from scitokens import __version__ as PKG_VERSION
         headers={'User-Agent' : 'SciTokens/{}'.format(PKG_VERSION)}
 
         # Go to the issuer's website, and download the OAuth well known bits
         # https://tools.ietf.org/html/draft-ietf-oauth-discovery-07
         well_known_uri = ".well-known/openid-configuration"
         if not issuer.endswith("/"):
             issuer = issuer + "/"
@@ -336,16 +331,19 @@
         if not os.path.exists(cache_dir):
             try:
                 os.makedirs(cache_dir)
             except OSError as ose:
                 raise UnableToCreateCache("Unable to create cache: {}".format(str(ose)))
 
         keycache_dir = os.path.join(cache_dir, "scitokens")
-        if not os.path.exists(keycache_dir):
-            os.makedirs(keycache_dir)
+        try:
+            if not os.path.exists(keycache_dir):
+                os.makedirs(keycache_dir)
+        except OSError as ose:
+            raise UnableToCreateCache("Unable to create cache: {}".format(str(ose)))
 
         keycache_file = os.path.join(keycache_dir, CACHE_FILENAME)
         if not os.path.exists(keycache_file):
             self._initialize_cachedb(keycache_file)
 
         return keycache_file
```

### Comparing `scitokens-1.7.4/src/scitokens.egg-info/PKG-INFO` & `scitokens-1.8.0/src/scitokens.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scitokens
-Version: 1.7.4
+Version: 1.8.0
 Summary: SciToken reference implementation library
 Home-page: https://scitokens.org
 Author: Brian Bockelman
 Author-email: team@scitokens.org
 License: Apache-2.0
 Project-URL: Documentation, https://scitokens.readthedocs.io/
 Project-URL: Issue Tracker, https://github.com/scitokens/scitokens/issues
@@ -219,14 +219,51 @@
     >>> enf.test(stoken, "write", "/store/user/bbockelm/foo")
     True
 
 The ``test`` method uses the SciTokens built-in path parsing to validate the
 authorization.  The ``generate_acls`` method allows the caller to cache
 the ACL information from the token.
 
+Creating Sample Tokens
+----------------------
+
+Typically, an access token is generated during an OAuth2 workflow to facilitate 
+authentication and authorization. However, for testing and experimentation purposes, 
+`the demo token generator <https://demo.scitokens.org/>`__ provides users with the
+ability to create sample tokens with customized payload:
+
+::
+    
+    >>> payload = {"sub": "<email adress>", "scope": "read:/protected"}
+    >>> token = scitokens.utils.demo.token(payload)
+
+The ``token`` method makes a request to the generator to create a serialized token 
+for the specified payload. Users can also retrieve a parsed token by calling the 
+``parsed_token`` method, which returns a SciToken object corresponding to the 
+token. The object contains the decoded token data, including the claims and signature. 
+
+Decorator
+-------------
+
+This protect decorator is designed to be used with a `flask <https://flask.palletsprojects.com/>`_ application. It can be used like:
+
+.. code-block:: python
+
+    @scitokens_protect.protect(audience="https://demo.scitokens.org", scope="read:/secret", issuer="https://demo.scitokens.org")
+    def Secret(token: SciToken):
+        # ... token is now available.
+
+The possible arguments are:
+
+- ``audience`` (str or list): Audience expected in the client token
+- ``scope`` (str): Scope required to access the function
+- ``issuer`` (str): The issuer to require of the client token
+
+The protected function can optionally take an argument ``token``, which is the parsed SciToken object.
+
 Configuration
 -------------
 
 An optional configuration file can be provided that will alter the behavior of 
 the SciTokens library.  Configuration options include:
 
 ================== ========================================================================================
```

### Comparing `scitokens-1.7.4/src/scitokens.egg-info/SOURCES.txt` & `scitokens-1.8.0/src/scitokens.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -13,25 +13,29 @@
 src/scitokens.egg-info/dependency_links.txt
 src/scitokens.egg-info/entry_points.txt
 src/scitokens.egg-info/requires.txt
 src/scitokens.egg-info/top_level.txt
 src/scitokens/tools/__init__.py
 src/scitokens/tools/admin_create_key.py
 src/scitokens/tools/admin_create_token.py
+src/scitokens/tools/verify_token.py
 src/scitokens/utils/__init__.py
 src/scitokens/utils/config.py
+src/scitokens/utils/demo.py
 src/scitokens/utils/errors.py
 src/scitokens/utils/keycache.py
+src/scitokens/utils/scitokens_protect.py
 tests/create_sample_token.py
 tests/create_webserver.py
 tests/load_token.py
 tests/sample_ecdsa_keypair.pem
 tests/simple_ec_private_key.pem
 tests/simple_private_key.pem
 tests/test_admin_create_key.py
 tests/test_config.ini
 tests/test_config.py
 tests/test_create_scitoken.py
+tests/test_demo.py
 tests/test_keycache.py
 tests/test_scitokens.py
 tests/test_urltools.py
 tests/test_with_http.py
```

### Comparing `scitokens-1.7.4/tests/create_sample_token.py` & `scitokens-1.8.0/tests/create_sample_token.py`

 * *Files identical despite different names*

### Comparing `scitokens-1.7.4/tests/create_webserver.py` & `scitokens-1.8.0/tests/create_webserver.py`

 * *Files identical despite different names*

### Comparing `scitokens-1.7.4/tests/sample_ecdsa_keypair.pem` & `scitokens-1.8.0/tests/sample_ecdsa_keypair.pem`

 * *Files identical despite different names*

### Comparing `scitokens-1.7.4/tests/simple_private_key.pem` & `scitokens-1.8.0/tests/simple_private_key.pem`

 * *Files identical despite different names*

### Comparing `scitokens-1.7.4/tests/test_admin_create_key.py` & `scitokens-1.8.0/tests/test_admin_create_key.py`

 * *Files identical despite different names*

### Comparing `scitokens-1.7.4/tests/test_config.py` & `scitokens-1.8.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `scitokens-1.7.4/tests/test_create_scitoken.py` & `scitokens-1.8.0/tests/test_create_scitoken.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,21 +3,23 @@
 """
 
 import os
 import sys
 import unittest
 import tempfile
 import shutil
+import datetime
 
 # Allow unittests to be run from within the project base.
 if os.path.exists("src"):
     sys.path.append("src")
 if os.path.exists("../src"):
     sys.path.append("../src")
 
+import jwt
 import scitokens
 from cryptography.hazmat.primitives.asymmetric.rsa import generate_private_key
 import cryptography.hazmat.primitives.asymmetric.ec as ec
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import serialization
 from jwt import DecodeError, InvalidAudienceError
 from scitokens.utils.errors import UnsupportedKeyException
@@ -415,10 +417,33 @@
         # clean up the files and directories created
         shutil.rmtree(xdg_dir)
         os.remove(bearer_token_file)
         os.remove(bt_path)
         if os.path.isfile(bt_tmp):
             shutil.move(bt_tmp, bt_path)
 
+    def test_noiss(self):
+        """
+        Verify that tokens without the `iss` are not accepted.
+        """
+        encoded_jwt = jwt.encode(
+            {
+                "ver": "scitoken:2.0",
+                "aud": "https://demo.scitokens.org",
+                "exp": datetime.datetime.now(tz=datetime.timezone.utc) + datetime.timedelta(seconds=30),
+                "iat": datetime.datetime.now(tz=datetime.timezone.utc),
+                "nbf": datetime.datetime.now(tz=datetime.timezone.utc),
+                "jti": "eab04181-b63a-42aa-b77d-804742829fc5",
+                "kid": "key-rs256"
+            },
+            "secret",
+            algorithm="HS256",
+            headers={"typ": "JWT", "alg": "HS256", "kid": "key-hs256"}
+        )
+
+        # Test when we give it without issuer
+        with self.assertRaises(scitokens.scitokens.MissingIssuerException):
+           scitokens.SciToken.deserialize(encoded_jwt)
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `scitokens-1.7.4/tests/test_keycache.py` & `scitokens-1.8.0/tests/test_keycache.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Test the keycache
 """
 
-import os
+import os, stat
+import sys
 import tempfile
 import shutil
 import unittest
 from unittest import mock
 from scitokens.utils.keycache import KeyCache
 from scitokens.utils.errors import UnableToCreateCache
 from cryptography.hazmat.primitives.asymmetric.rsa import generate_private_key
@@ -56,14 +57,43 @@
         os.environ['XDG_CACHE_HOME'] = "/does/not/exists"
 
         # Make sure it raises an unable to create cache exception
         with self.assertRaises(UnableToCreateCache):
             keycache = KeyCache()
             del keycache
 
+    @unittest.skipIf(sys.platform.startswith("win"), "Test doesn't work on Windows")
+    @unittest.skipIf(not sys.platform.startswith("win") and os.getuid() == 0, "Test doesn't work when root")
+    def test_cannot_make_cache_permission_denied(self):
+        """
+        Test when the keycache shouldn't be able to make the cache due to access privilege
+        """
+        os.environ['XDG_CACHE_HOME'] = self.tmp_dir
+
+        # Limiting access privilege to read-only for the $XDG_CACHE_HOME
+        os.chmod(
+            self.tmp_dir,
+            stat.S_IRUSR |  # Read for user
+            stat.S_IRGRP |  # Read for group
+            stat.S_IROTH    # Read for other
+        )
+
+        # Make sure it raises an unable to create cache exception
+        with self.assertRaises(UnableToCreateCache):
+            keycache = KeyCache()
+            del keycache
+
+        # Revert the access privilege alteration for the $XDG_CACHE_HOME
+        os.chmod(
+            self.tmp_dir,
+            stat.S_IRWXU |  # Read, write, and execute for user
+            stat.S_IRWXG |  # Read, write, and execute for group
+            stat.S_IRWXO    # Read, write, and execute for other
+        )
+
     def test_empty(self):
         """
         Test when the keycache should be empty
         """
         # Stand up an HTTP server
         private_key = generate_private_key(
             public_exponent=65537,
@@ -229,7 +259,10 @@
             format=serialization.PublicFormat.SubjectPublicKeyInfo
         )
 
         self.assertEqual(public_pem, pubkey_pem_from_keycache)
 
         create_webserver.shutdown_server()
 
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `scitokens-1.7.4/tests/test_scitokens.py` & `scitokens-1.8.0/tests/test_scitokens.py`

 * *Files identical despite different names*

### Comparing `scitokens-1.7.4/tests/test_urltools.py` & `scitokens-1.8.0/tests/test_urltools.py`

 * *Files identical despite different names*

### Comparing `scitokens-1.7.4/tests/test_with_http.py` & `scitokens-1.8.0/tests/test_with_http.py`

 * *Files identical despite different names*

