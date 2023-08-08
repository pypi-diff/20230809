# Comparing `tmp/globus-compute-common-0.2.0.tar.gz` & `tmp/globus-compute-common-0.3.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globus-compute-common-0.2.0.tar", last modified: Wed May 10 20:14:55 2023, max compression
+gzip compressed data, was "globus-compute-common-0.3.0a1.tar", last modified: Tue Aug  8 17:05:14 2023, max compression
```

## Comparing `globus-compute-common-0.2.0.tar` & `globus-compute-common-0.3.0a1.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-10 20:14:55.566807 globus-compute-common-0.2.0/
--rw-r--r--   0 chris      (501) staff       (20)      996 2023-05-10 20:14:55.566916 globus-compute-common-0.2.0/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)      426 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/README.md
--rw-r--r--   0 chris      (501) staff       (20)     1362 2023-05-10 20:14:55.567547 globus-compute-common-0.2.0/setup.cfg
--rw-r--r--   0 chris      (501) staff       (20)       38 2022-05-26 18:40:18.000000 globus-compute-common-0.2.0/setup.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-10 20:14:55.556995 globus-compute-common-0.2.0/src/
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-10 20:14:55.559657 globus-compute-common-0.2.0/src/globus_compute_common/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     3652 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/globus_compute_flake8.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-10 20:14:55.561339 globus-compute-common-0.2.0/src/globus_compute_common/messagepack/
--rw-r--r--   0 chris      (501) staff       (20)      501 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/messagepack/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)      523 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/messagepack/exceptions.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-10 20:14:55.563481 globus-compute-common-0.2.0/src/globus_compute_common/messagepack/message_types/
--rw-r--r--   0 chris      (501) staff       (20)      771 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/messagepack/message_types/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     1830 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/messagepack/message_types/base.py
--rw-r--r--   0 chris      (501) staff       (20)      545 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/messagepack/message_types/container.py
--rw-r--r--   0 chris      (501) staff       (20)      599 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/messagepack/message_types/ep_status_report.py
--rw-r--r--   0 chris      (501) staff       (20)      376 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/messagepack/message_types/manager_status_report.py
--rw-r--r--   0 chris      (501) staff       (20)      631 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/messagepack/message_types/result.py
--rw-r--r--   0 chris      (501) staff       (20)      363 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/messagepack/message_types/task.py
--rw-r--r--   0 chris      (501) staff       (20)      131 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/messagepack/message_types/task_cancel.py
--rw-r--r--   0 chris      (501) staff       (20)      428 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/messagepack/message_types/task_transition.py
--rw-r--r--   0 chris      (501) staff       (20)     1568 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/messagepack/packer.py
--rw-r--r--   0 chris      (501) staff       (20)      519 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/messagepack/protocol.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-10 20:14:55.563841 globus-compute-common-0.2.0/src/globus_compute_common/messagepack/protocol_versions/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/messagepack/protocol_versions/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     4305 2023-05-10 18:57:48.000000 globus-compute-common-0.2.0/src/globus_compute_common/messagepack/protocol_versions/proto1.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-10 20:14:55.565147 globus-compute-common-0.2.0/src/globus_compute_common/redis/
--rw-r--r--   0 chris      (501) staff       (20)      898 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/redis/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     1672 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/redis/connection.py
--rw-r--r--   0 chris      (501) staff       (20)     2163 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/redis/fields.py
--rw-r--r--   0 chris      (501) staff       (20)     7499 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/redis/pubsub.py
--rw-r--r--   0 chris      (501) staff       (20)     1654 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/redis/serde.py
--rw-r--r--   0 chris      (501) staff       (20)     1198 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/redis/task_queue.py
--rw-r--r--   0 chris      (501) staff       (20)     3676 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/redis_endpoint_lock.py
--rw-r--r--   0 chris      (501) staff       (20)     8212 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/redis_task.py
--rw-r--r--   0 chris      (501) staff       (20)      666 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/sdk_version_sharing.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-10 20:14:55.566107 globus-compute-common-0.2.0/src/globus_compute_common/task_storage/
--rw-r--r--   0 chris      (501) staff       (20)      313 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/task_storage/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     1513 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/task_storage/base.py
--rw-r--r--   0 chris      (501) staff       (20)     1048 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/task_storage/default_storage.py
--rw-r--r--   0 chris      (501) staff       (20)     1036 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/task_storage/redis.py
--rw-r--r--   0 chris      (501) staff       (20)     6640 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/task_storage/s3.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-10 20:14:55.566664 globus-compute-common-0.2.0/src/globus_compute_common/tasks/
--rw-r--r--   0 chris      (501) staff       (20)      192 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/tasks/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     1256 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/tasks/constants.py
--rw-r--r--   0 chris      (501) staff       (20)      592 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/tasks/protocol.py
--rw-r--r--   0 chris      (501) staff       (20)      520 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/testing.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-10 20:14:55.560558 globus-compute-common-0.2.0/src/globus_compute_common.egg-info/
--rw-r--r--   0 chris      (501) staff       (20)      996 2023-05-10 20:14:55.000000 globus-compute-common-0.2.0/src/globus_compute_common.egg-info/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)     2111 2023-05-10 20:14:55.000000 globus-compute-common-0.2.0/src/globus_compute_common.egg-info/SOURCES.txt
--rw-r--r--   0 chris      (501) staff       (20)        1 2023-05-10 20:14:55.000000 globus-compute-common-0.2.0/src/globus_compute_common.egg-info/dependency_links.txt
--rw-r--r--   0 chris      (501) staff       (20)      138 2023-05-10 20:14:55.000000 globus-compute-common-0.2.0/src/globus_compute_common.egg-info/requires.txt
--rw-r--r--   0 chris      (501) staff       (20)       22 2023-05-10 20:14:55.000000 globus-compute-common-0.2.0/src/globus_compute_common.egg-info/top_level.txt
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-08-08 17:05:14.781544 globus-compute-common-0.3.0a1/
+-rw-r--r--   0 lei        (501) staff       (20)    11357 2023-08-02 18:17:28.000000 globus-compute-common-0.3.0a1/LICENSE
+-rw-r--r--   0 lei        (501) staff       (20)     1020 2023-08-08 17:05:14.781603 globus-compute-common-0.3.0a1/PKG-INFO
+-rw-r--r--   0 lei        (501) staff       (20)      426 2023-03-09 15:52:23.000000 globus-compute-common-0.3.0a1/README.md
+-rw-r--r--   0 lei        (501) staff       (20)     1364 2023-08-08 17:05:14.781955 globus-compute-common-0.3.0a1/setup.cfg
+-rw-r--r--   0 lei        (501) staff       (20)       38 2022-06-21 19:08:30.000000 globus-compute-common-0.3.0a1/setup.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-08-08 17:05:14.770426 globus-compute-common-0.3.0a1/src/
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-08-08 17:05:14.777352 globus-compute-common-0.3.0a1/src/globus_compute_common/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-03-09 15:52:23.000000 globus-compute-common-0.3.0a1/src/globus_compute_common/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     3652 2023-03-09 15:52:23.000000 globus-compute-common-0.3.0a1/src/globus_compute_common/globus_compute_flake8.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-08-08 17:05:14.778606 globus-compute-common-0.3.0a1/src/globus_compute_common/messagepack/
+-rw-r--r--   0 lei        (501) staff       (20)      501 2023-03-09 15:52:23.000000 globus-compute-common-0.3.0a1/src/globus_compute_common/messagepack/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)      523 2023-03-09 15:52:23.000000 globus-compute-common-0.3.0a1/src/globus_compute_common/messagepack/exceptions.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-08-08 17:05:14.779669 globus-compute-common-0.3.0a1/src/globus_compute_common/messagepack/message_types/
+-rw-r--r--   0 lei        (501) staff       (20)      771 2023-08-07 16:36:05.000000 globus-compute-common-0.3.0a1/src/globus_compute_common/messagepack/message_types/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     1830 2023-03-09 15:52:23.000000 globus-compute-common-0.3.0a1/src/globus_compute_common/messagepack/message_types/base.py
+-rw-r--r--   0 lei        (501) staff       (20)      545 2023-03-09 15:52:23.000000 globus-compute-common-0.3.0a1/src/globus_compute_common/messagepack/message_types/container.py
+-rw-r--r--   0 lei        (501) staff       (20)      599 2023-03-09 15:52:23.000000 globus-compute-common-0.3.0a1/src/globus_compute_common/messagepack/message_types/ep_status_report.py
+-rw-r--r--   0 lei        (501) staff       (20)      376 2023-03-09 15:52:23.000000 globus-compute-common-0.3.0a1/src/globus_compute_common/messagepack/message_types/manager_status_report.py
+-rw-r--r--   0 lei        (501) staff       (20)      967 2023-08-07 19:43:50.000000 globus-compute-common-0.3.0a1/src/globus_compute_common/messagepack/message_types/result.py
+-rw-r--r--   0 lei        (501) staff       (20)      363 2023-03-09 15:52:23.000000 globus-compute-common-0.3.0a1/src/globus_compute_common/messagepack/message_types/task.py
+-rw-r--r--   0 lei        (501) staff       (20)      131 2023-03-09 15:52:23.000000 globus-compute-common-0.3.0a1/src/globus_compute_common/messagepack/message_types/task_cancel.py
+-rw-r--r--   0 lei        (501) staff       (20)      428 2023-03-09 15:52:23.000000 globus-compute-common-0.3.0a1/src/globus_compute_common/messagepack/message_types/task_transition.py
+-rw-r--r--   0 lei        (501) staff       (20)     1568 2023-08-07 19:50:56.000000 globus-compute-common-0.3.0a1/src/globus_compute_common/messagepack/packer.py
+-rw-r--r--   0 lei        (501) staff       (20)      518 2023-08-07 19:50:56.000000 globus-compute-common-0.3.0a1/src/globus_compute_common/messagepack/protocol.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-08-08 17:05:14.779874 globus-compute-common-0.3.0a1/src/globus_compute_common/messagepack/protocol_versions/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-03-09 15:52:23.000000 globus-compute-common-0.3.0a1/src/globus_compute_common/messagepack/protocol_versions/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     4297 2023-08-07 19:50:56.000000 globus-compute-common-0.3.0a1/src/globus_compute_common/messagepack/protocol_versions/proto1.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-08-08 17:05:14.780555 globus-compute-common-0.3.0a1/src/globus_compute_common/redis/
+-rw-r--r--   0 lei        (501) staff       (20)      898 2023-03-09 15:52:23.000000 globus-compute-common-0.3.0a1/src/globus_compute_common/redis/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     1672 2023-03-09 15:52:23.000000 globus-compute-common-0.3.0a1/src/globus_compute_common/redis/connection.py
+-rw-r--r--   0 lei        (501) staff       (20)     2163 2023-03-09 15:52:23.000000 globus-compute-common-0.3.0a1/src/globus_compute_common/redis/fields.py
+-rw-r--r--   0 lei        (501) staff       (20)     7499 2023-03-09 15:52:23.000000 globus-compute-common-0.3.0a1/src/globus_compute_common/redis/pubsub.py
+-rw-r--r--   0 lei        (501) staff       (20)     1654 2023-03-09 15:52:23.000000 globus-compute-common-0.3.0a1/src/globus_compute_common/redis/serde.py
+-rw-r--r--   0 lei        (501) staff       (20)     1198 2023-03-09 15:52:23.000000 globus-compute-common-0.3.0a1/src/globus_compute_common/redis/task_queue.py
+-rw-r--r--   0 lei        (501) staff       (20)     3676 2023-03-09 15:52:23.000000 globus-compute-common-0.3.0a1/src/globus_compute_common/redis_endpoint_lock.py
+-rw-r--r--   0 lei        (501) staff       (20)     8212 2023-03-09 15:52:23.000000 globus-compute-common-0.3.0a1/src/globus_compute_common/redis_task.py
+-rw-r--r--   0 lei        (501) staff       (20)      666 2023-03-09 15:52:23.000000 globus-compute-common-0.3.0a1/src/globus_compute_common/sdk_version_sharing.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-08-08 17:05:14.781113 globus-compute-common-0.3.0a1/src/globus_compute_common/task_storage/
+-rw-r--r--   0 lei        (501) staff       (20)      313 2023-03-09 15:52:23.000000 globus-compute-common-0.3.0a1/src/globus_compute_common/task_storage/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     1513 2023-03-09 15:52:23.000000 globus-compute-common-0.3.0a1/src/globus_compute_common/task_storage/base.py
+-rw-r--r--   0 lei        (501) staff       (20)     1048 2023-03-09 15:52:23.000000 globus-compute-common-0.3.0a1/src/globus_compute_common/task_storage/default_storage.py
+-rw-r--r--   0 lei        (501) staff       (20)     1036 2023-03-09 15:52:23.000000 globus-compute-common-0.3.0a1/src/globus_compute_common/task_storage/redis.py
+-rw-r--r--   0 lei        (501) staff       (20)     6640 2023-03-09 15:52:23.000000 globus-compute-common-0.3.0a1/src/globus_compute_common/task_storage/s3.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-08-08 17:05:14.781448 globus-compute-common-0.3.0a1/src/globus_compute_common/tasks/
+-rw-r--r--   0 lei        (501) staff       (20)      192 2023-03-09 15:52:23.000000 globus-compute-common-0.3.0a1/src/globus_compute_common/tasks/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     1256 2023-03-09 15:52:23.000000 globus-compute-common-0.3.0a1/src/globus_compute_common/tasks/constants.py
+-rw-r--r--   0 lei        (501) staff       (20)      592 2023-03-09 15:52:23.000000 globus-compute-common-0.3.0a1/src/globus_compute_common/tasks/protocol.py
+-rw-r--r--   0 lei        (501) staff       (20)      520 2023-03-09 15:52:23.000000 globus-compute-common-0.3.0a1/src/globus_compute_common/testing.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-08-08 17:05:14.778137 globus-compute-common-0.3.0a1/src/globus_compute_common.egg-info/
+-rw-r--r--   0 lei        (501) staff       (20)     1020 2023-08-08 17:05:14.000000 globus-compute-common-0.3.0a1/src/globus_compute_common.egg-info/PKG-INFO
+-rw-r--r--   0 lei        (501) staff       (20)     2119 2023-08-08 17:05:14.000000 globus-compute-common-0.3.0a1/src/globus_compute_common.egg-info/SOURCES.txt
+-rw-r--r--   0 lei        (501) staff       (20)        1 2023-08-08 17:05:14.000000 globus-compute-common-0.3.0a1/src/globus_compute_common.egg-info/dependency_links.txt
+-rw-r--r--   0 lei        (501) staff       (20)      138 2023-08-08 17:05:14.000000 globus-compute-common-0.3.0a1/src/globus_compute_common.egg-info/requires.txt
+-rw-r--r--   0 lei        (501) staff       (20)       22 2023-08-08 17:05:14.000000 globus-compute-common-0.3.0a1/src/globus_compute_common.egg-info/top_level.txt
```

### Comparing `globus-compute-common-0.2.0/PKG-INFO` & `globus-compute-common-0.3.0a1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: globus-compute-common
-Version: 0.2.0
+Version: 0.3.0a1
 Summary: Common tools for Globus Compute projects
 Home-page: https://github.com/funcX-faas/funcx-common
 Author: Globus Team
 Author-email: support@globus.org
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: moto
 Provides-Extra: redis
 Provides-Extra: boto3
+License-File: LICENSE
 
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/funcx-faas/funcx-common/main.svg)](https://results.pre-commit.ci/latest/github/funcx-faas/funcx-common/main)
 
 # globus-compute-common
 
 This package contains common utilities for use across various Globus Compute projects.
```

### Comparing `globus-compute-common-0.2.0/setup.cfg` & `globus-compute-common-0.3.0a1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = globus-compute-common
-version = 0.2.0
+version = 0.3.0a1
 description = Common tools for Globus Compute projects
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/funcX-faas/funcx-common
 author = Globus Team
 author_email = support@globus.org
 classifiers =
```

### Comparing `globus-compute-common-0.2.0/src/globus_compute_common/globus_compute_flake8.py` & `globus-compute-common-0.3.0a1/src/globus_compute_common/globus_compute_flake8.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.2.0/src/globus_compute_common/messagepack/exceptions.py` & `globus-compute-common-0.3.0a1/src/globus_compute_common/messagepack/exceptions.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.2.0/src/globus_compute_common/messagepack/message_types/__init__.py` & `globus-compute-common-0.3.0a1/src/globus_compute_common/messagepack/message_types/__init__.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.2.0/src/globus_compute_common/messagepack/message_types/base.py` & `globus-compute-common-0.3.0a1/src/globus_compute_common/messagepack/message_types/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.2.0/src/globus_compute_common/messagepack/message_types/container.py` & `globus-compute-common-0.3.0a1/src/globus_compute_common/messagepack/message_types/container.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.2.0/src/globus_compute_common/messagepack/message_types/ep_status_report.py` & `globus-compute-common-0.3.0a1/src/globus_compute_common/messagepack/message_types/ep_status_report.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.2.0/src/globus_compute_common/messagepack/packer.py` & `globus-compute-common-0.3.0a1/src/globus_compute_common/messagepack/packer.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.2.0/src/globus_compute_common/messagepack/protocol.py` & `globus-compute-common-0.3.0a1/src/globus_compute_common/messagepack/protocol.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 A MessagePackProtocol only needs to define two actions:
   - pack()
   - unpack()
 
 And the two must be inverses on any valid inputs.
 """
-
 import abc
 
 from .message_types import Message
 
 
 class MessagePackProtocol(abc.ABC):
     @abc.abstractmethod
```

### Comparing `globus-compute-common-0.2.0/src/globus_compute_common/messagepack/protocol_versions/proto1.py` & `globus-compute-common-0.3.0a1/src/globus_compute_common/messagepack/protocol_versions/proto1.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         message_type = data["message_type"]
     elif issubclass(model, Message):
         outer_type = "data"
         message_type = model.Meta.message_type
     else:
         raise NotImplementedError
 
-    model_ = t.cast("type[pydantic.BaseModel]", model)
+    model_ = t.cast(pydantic.BaseModel, model)
 
     unknown_fields = set(data)
     for name, field in model_.__fields__.items():
         unknown_fields.discard(name)
         unknown_fields.discard(field.alias)
 
     if unknown_fields:
```

### Comparing `globus-compute-common-0.2.0/src/globus_compute_common/redis/__init__.py` & `globus-compute-common-0.3.0a1/src/globus_compute_common/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.2.0/src/globus_compute_common/redis/connection.py` & `globus-compute-common-0.3.0a1/src/globus_compute_common/redis/connection.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.2.0/src/globus_compute_common/redis/fields.py` & `globus-compute-common-0.3.0a1/src/globus_compute_common/redis/fields.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.2.0/src/globus_compute_common/redis/pubsub.py` & `globus-compute-common-0.3.0a1/src/globus_compute_common/redis/pubsub.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.2.0/src/globus_compute_common/redis/serde.py` & `globus-compute-common-0.3.0a1/src/globus_compute_common/redis/serde.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.2.0/src/globus_compute_common/redis/task_queue.py` & `globus-compute-common-0.3.0a1/src/globus_compute_common/redis/task_queue.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.2.0/src/globus_compute_common/redis_endpoint_lock.py` & `globus-compute-common-0.3.0a1/src/globus_compute_common/redis_endpoint_lock.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.2.0/src/globus_compute_common/redis_task.py` & `globus-compute-common-0.3.0a1/src/globus_compute_common/redis_task.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.2.0/src/globus_compute_common/sdk_version_sharing.py` & `globus-compute-common-0.3.0a1/src/globus_compute_common/sdk_version_sharing.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.2.0/src/globus_compute_common/task_storage/base.py` & `globus-compute-common-0.3.0a1/src/globus_compute_common/task_storage/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.2.0/src/globus_compute_common/task_storage/default_storage.py` & `globus-compute-common-0.3.0a1/src/globus_compute_common/task_storage/default_storage.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.2.0/src/globus_compute_common/task_storage/redis.py` & `globus-compute-common-0.3.0a1/src/globus_compute_common/task_storage/redis.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.2.0/src/globus_compute_common/task_storage/s3.py` & `globus-compute-common-0.3.0a1/src/globus_compute_common/task_storage/s3.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.2.0/src/globus_compute_common/tasks/constants.py` & `globus-compute-common-0.3.0a1/src/globus_compute_common/tasks/constants.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.2.0/src/globus_compute_common/tasks/protocol.py` & `globus-compute-common-0.3.0a1/src/globus_compute_common/tasks/protocol.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.2.0/src/globus_compute_common/testing.py` & `globus-compute-common-0.3.0a1/src/globus_compute_common/testing.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.2.0/src/globus_compute_common.egg-info/PKG-INFO` & `globus-compute-common-0.3.0a1/src/globus_compute_common.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: globus-compute-common
-Version: 0.2.0
+Version: 0.3.0a1
 Summary: Common tools for Globus Compute projects
 Home-page: https://github.com/funcX-faas/funcx-common
 Author: Globus Team
 Author-email: support@globus.org
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: moto
 Provides-Extra: redis
 Provides-Extra: boto3
+License-File: LICENSE
 
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/funcx-faas/funcx-common/main.svg)](https://results.pre-commit.ci/latest/github/funcx-faas/funcx-common/main)
 
 # globus-compute-common
 
 This package contains common utilities for use across various Globus Compute projects.
```

### Comparing `globus-compute-common-0.2.0/src/globus_compute_common.egg-info/SOURCES.txt` & `globus-compute-common-0.3.0a1/src/globus_compute_common.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.cfg
 setup.py
 src/globus_compute_common/__init__.py
 src/globus_compute_common/globus_compute_flake8.py
 src/globus_compute_common/redis_endpoint_lock.py
 src/globus_compute_common/redis_task.py
```

