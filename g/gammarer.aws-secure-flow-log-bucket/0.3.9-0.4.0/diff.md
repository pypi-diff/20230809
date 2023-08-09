# Comparing `tmp/gammarer.aws-secure-flow-log-bucket-0.3.9.tar.gz` & `tmp/gammarer.aws-secure-flow-log-bucket-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-secure-flow-log-bucket-0.3.9.tar", last modified: Wed Jul 26 18:15:30 2023, max compression
+gzip compressed data, was "gammarer.aws-secure-flow-log-bucket-0.4.0.tar", last modified: Wed Aug  9 04:52:58 2023, max compression
```

## Comparing `gammarer.aws-secure-flow-log-bucket-0.3.9.tar` & `gammarer.aws-secure-flow-log-bucket-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:15:30.697463 gammarer.aws-secure-flow-log-bucket-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-26 18:15:18.000000 gammarer.aws-secure-flow-log-bucket-0.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-26 18:15:18.000000 gammarer.aws-secure-flow-log-bucket-0.3.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-07-26 18:15:30.697463 gammarer.aws-secure-flow-log-bucket-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-26 18:15:18.000000 gammarer.aws-secure-flow-log-bucket-0.3.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-26 18:15:18.000000 gammarer.aws-secure-flow-log-bucket-0.3.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 18:15:30.697463 gammarer.aws-secure-flow-log-bucket-0.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-26 18:15:18.000000 gammarer.aws-secure-flow-log-bucket-0.3.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:15:30.697463 gammarer.aws-secure-flow-log-bucket-0.3.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:15:30.697463 gammarer.aws-secure-flow-log-bucket-0.3.9/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:15:30.697463 gammarer.aws-secure-flow-log-bucket-0.3.9/src/gammarer/aws_secure_flow_log_bucket/
--rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-07-26 18:15:18.000000 gammarer.aws-secure-flow-log-bucket-0.3.9/src/gammarer/aws_secure_flow_log_bucket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:15:30.697463 gammarer.aws-secure-flow-log-bucket-0.3.9/src/gammarer/aws_secure_flow_log_bucket/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-26 18:15:18.000000 gammarer.aws-secure-flow-log-bucket-0.3.9/src/gammarer/aws_secure_flow_log_bucket/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24016 2023-07-26 18:15:18.000000 gammarer.aws-secure-flow-log-bucket-0.3.9/src/gammarer/aws_secure_flow_log_bucket/_jsii/aws-secure-flow-log-bucket@0.3.9.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 18:15:18.000000 gammarer.aws-secure-flow-log-bucket-0.3.9/src/gammarer/aws_secure_flow_log_bucket/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:15:30.697463 gammarer.aws-secure-flow-log-bucket-0.3.9/src/gammarer.aws_secure_flow_log_bucket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-07-26 18:15:30.000000 gammarer.aws-secure-flow-log-bucket-0.3.9/src/gammarer.aws_secure_flow_log_bucket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-26 18:15:30.000000 gammarer.aws-secure-flow-log-bucket-0.3.9/src/gammarer.aws_secure_flow_log_bucket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 18:15:30.000000 gammarer.aws-secure-flow-log-bucket-0.3.9/src/gammarer.aws_secure_flow_log_bucket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-26 18:15:30.000000 gammarer.aws-secure-flow-log-bucket-0.3.9/src/gammarer.aws_secure_flow_log_bucket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 18:15:30.000000 gammarer.aws-secure-flow-log-bucket-0.3.9/src/gammarer.aws_secure_flow_log_bucket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 04:52:58.251342 gammarer.aws-secure-flow-log-bucket-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-09 04:52:42.000000 gammarer.aws-secure-flow-log-bucket-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-09 04:52:42.000000 gammarer.aws-secure-flow-log-bucket-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-08-09 04:52:58.251342 gammarer.aws-secure-flow-log-bucket-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-08-09 04:52:42.000000 gammarer.aws-secure-flow-log-bucket-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-09 04:52:42.000000 gammarer.aws-secure-flow-log-bucket-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-09 04:52:58.251342 gammarer.aws-secure-flow-log-bucket-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-08-09 04:52:42.000000 gammarer.aws-secure-flow-log-bucket-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 04:52:58.251342 gammarer.aws-secure-flow-log-bucket-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 04:52:58.251342 gammarer.aws-secure-flow-log-bucket-0.4.0/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 04:52:58.251342 gammarer.aws-secure-flow-log-bucket-0.4.0/src/gammarer/aws_secure_flow_log_bucket/
+-rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-08-09 04:52:42.000000 gammarer.aws-secure-flow-log-bucket-0.4.0/src/gammarer/aws_secure_flow_log_bucket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 04:52:58.251342 gammarer.aws-secure-flow-log-bucket-0.4.0/src/gammarer/aws_secure_flow_log_bucket/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-08-09 04:52:42.000000 gammarer.aws-secure-flow-log-bucket-0.4.0/src/gammarer/aws_secure_flow_log_bucket/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25182 2023-08-09 04:52:42.000000 gammarer.aws-secure-flow-log-bucket-0.4.0/src/gammarer/aws_secure_flow_log_bucket/_jsii/aws-secure-flow-log-bucket@0.4.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 04:52:42.000000 gammarer.aws-secure-flow-log-bucket-0.4.0/src/gammarer/aws_secure_flow_log_bucket/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 04:52:58.251342 gammarer.aws-secure-flow-log-bucket-0.4.0/src/gammarer.aws_secure_flow_log_bucket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-08-09 04:52:58.000000 gammarer.aws-secure-flow-log-bucket-0.4.0/src/gammarer.aws_secure_flow_log_bucket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-08-09 04:52:58.000000 gammarer.aws-secure-flow-log-bucket-0.4.0/src/gammarer.aws_secure_flow_log_bucket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 04:52:58.000000 gammarer.aws-secure-flow-log-bucket-0.4.0/src/gammarer.aws_secure_flow_log_bucket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-08-09 04:52:58.000000 gammarer.aws-secure-flow-log-bucket-0.4.0/src/gammarer.aws_secure_flow_log_bucket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-09 04:52:58.000000 gammarer.aws-secure-flow-log-bucket-0.4.0/src/gammarer.aws_secure_flow_log_bucket.egg-info/top_level.txt
```

### Comparing `gammarer.aws-secure-flow-log-bucket-0.3.9/LICENSE` & `gammarer.aws-secure-flow-log-bucket-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-flow-log-bucket-0.3.9/setup.py` & `gammarer.aws-secure-flow-log-bucket-0.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-secure-flow-log-bucket",
-    "version": "0.3.9",
+    "version": "0.4.0",
     "description": "Specific AWS VPC FlowLog Bucket",
     "license": "Apache-2.0",
     "url": "https://github.com/yicr/aws-secure-flow-log-bucket.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,26 +22,27 @@
     },
     "packages": [
         "gammarer.aws_secure_flow_log_bucket",
         "gammarer.aws_secure_flow_log_bucket._jsii"
     ],
     "package_data": {
         "gammarer.aws_secure_flow_log_bucket._jsii": [
-            "aws-secure-flow-log-bucket@0.3.9.jsii.tgz"
+            "aws-secure-flow-log-bucket@0.4.0.jsii.tgz"
         ],
         "gammarer.aws_secure_flow_log_bucket": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.80.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "gammarer.aws-secure-log-bucket>=0.9.8, <0.10.0",
-        "jsii>=1.85.0, <2.0.0",
+        "gammarer.aws-secure-bucket>=0.11.5, <0.12.0",
+        "gammarer.aws-secure-log-bucket>=0.11.1, <0.12.0",
+        "jsii>=1.86.1, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `gammarer.aws-secure-flow-log-bucket-0.3.9/src/gammarer.aws_secure_flow_log_bucket.egg-info/SOURCES.txt` & `gammarer.aws-secure-flow-log-bucket-0.4.0/src/gammarer.aws_secure_flow_log_bucket.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_secure_flow_log_bucket.egg-info/SOURCES.txt
 src/gammarer.aws_secure_flow_log_bucket.egg-info/dependency_links.txt
 src/gammarer.aws_secure_flow_log_bucket.egg-info/requires.txt
 src/gammarer.aws_secure_flow_log_bucket.egg-info/top_level.txt
 src/gammarer/aws_secure_flow_log_bucket/__init__.py
 src/gammarer/aws_secure_flow_log_bucket/py.typed
 src/gammarer/aws_secure_flow_log_bucket/_jsii/__init__.py
-src/gammarer/aws_secure_flow_log_bucket/_jsii/aws-secure-flow-log-bucket@0.3.9.jsii.tgz
+src/gammarer/aws_secure_flow_log_bucket/_jsii/aws-secure-flow-log-bucket@0.4.0.jsii.tgz
```

