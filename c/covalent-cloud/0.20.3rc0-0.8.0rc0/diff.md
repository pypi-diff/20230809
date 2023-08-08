# Comparing `tmp/covalent-cloud-0.20.3rc0.tar.gz` & `tmp/covalent-cloud-0.8.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "covalent-cloud-0.20.3rc0.tar", last modified: Tue Aug  8 19:19:29 2023, max compression
+gzip compressed data, was "covalent-cloud-0.8.0rc0.tar", last modified: Sat Apr 29 00:10:27 2023, max compression
```

## Comparing `covalent-cloud-0.20.3rc0.tar` & `covalent-cloud-0.8.0rc0.tar`

### file list

```diff
@@ -1,100 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:19:29.896203 covalent-cloud-0.20.3rc0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-08-08 19:19:29.896203 covalent-cloud-0.20.3rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:19:29.888203 covalent-cloud-0.20.3rc0/covalent_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:19:29.888203 covalent-cloud-0.20.3rc0/covalent_cloud/_serialize/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/_serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/_serialize/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/_serialize/electron.py
--rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/_serialize/lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/_serialize/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/_serialize/transport_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:19:29.888203 covalent-cloud-0.20.3rc0/covalent_cloud/analytics/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/analytics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:19:29.888203 covalent-cloud-0.20.3rc0/covalent_cloud/cloud_executor/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/cloud_executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/cloud_executor/cloud_executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:19:29.888203 covalent-cloud-0.20.3rc0/covalent_cloud/cloud_executor/models/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/cloud_executor/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/cloud_executor/models/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/cloud_executor/models/sw_environment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:19:29.888203 covalent-cloud-0.20.3rc0/covalent_cloud/dispatch_management/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/dispatch_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10505 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/dispatch_management/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/dispatch_management/interface_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16648 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/dispatch_management/results_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:19:29.888203 covalent-cloud-0.20.3rc0/covalent_cloud/qelectron_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/qelectron_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:19:29.888203 covalent-cloud-0.20.3rc0/covalent_cloud/qelectron_sdk/core/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/qelectron_sdk/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/qelectron_sdk/core/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/qelectron_sdk/core/future_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/qelectron_sdk/core/qelectron.py
--rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/qelectron_sdk/core/qnode_qe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:19:29.892202 covalent-cloud-0.20.3rc0/covalent_cloud/qelectron_sdk/executors/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/qelectron_sdk/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/qelectron_sdk/executors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/qelectron_sdk/executors/qiskit_executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:19:29.892202 covalent-cloud-0.20.3rc0/covalent_cloud/qelectron_sdk/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/qelectron_sdk/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/qelectron_sdk/middleware/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:19:29.892202 covalent-cloud-0.20.3rc0/covalent_cloud/qelectron_sdk/middleware/qclients/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/qelectron_sdk/middleware/qclients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/qelectron_sdk/middleware/qclients/base_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/qelectron_sdk/middleware/qclients/cloud_qclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/qelectron_sdk/middleware/qclients/remote_qclient.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:19:29.892202 covalent-cloud-0.20.3rc0/covalent_cloud/qelectron_sdk/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/qelectron_sdk/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/qelectron_sdk/schemas/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:19:29.892202 covalent-cloud-0.20.3rc0/covalent_cloud/service_account_interface/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/service_account_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/service_account_interface/auth_config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/service_account_interface/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:19:29.892202 covalent-cloud-0.20.3rc0/covalent_cloud/shared/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/shared/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:19:29.892202 covalent-cloud-0.20.3rc0/covalent_cloud/shared/classes/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/shared/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/shared/classes/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/shared/classes/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/shared/classes/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:19:29.892202 covalent-cloud-0.20.3rc0/covalent_cloud/shared/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/shared/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/shared/schemas/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/shared/schemas/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/shared/schemas/electron.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/shared/schemas/lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/shared/schemas/result.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/shared/schemas/transport_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:19:29.892202 covalent-cloud-0.20.3rc0/covalent_cloud/software_environment/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/software_environment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:19:29.892202 covalent-cloud-0.20.3rc0/covalent_cloud/swe_management/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/swe_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/covalent_cloud/swe_management/swe_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:19:29.888203 covalent-cloud-0.20.3rc0/covalent_cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-08-08 19:19:29.000000 covalent-cloud-0.20.3rc0/covalent_cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-08-08 19:19:29.000000 covalent-cloud-0.20.3rc0/covalent_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 19:19:29.000000 covalent-cloud-0.20.3rc0/covalent_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 19:19:29.000000 covalent-cloud-0.20.3rc0/covalent_cloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-08 19:19:29.000000 covalent-cloud-0.20.3rc0/covalent_cloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-08 19:19:29.896203 covalent-cloud-0.20.3rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:19:29.888203 covalent-cloud-0.20.3rc0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:19:29.892202 covalent-cloud-0.20.3rc0/tests/dispatch_management_tests/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/tests/dispatch_management_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/tests/dispatch_management_tests/future_classes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/tests/dispatch_management_tests/helpers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/tests/dispatch_management_tests/interface_functions_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:19:29.892202 covalent-cloud-0.20.3rc0/tests/shared/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/tests/shared/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:19:29.892202 covalent-cloud-0.20.3rc0/tests/shared/classes/
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/tests/shared/classes/APIClient_test.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/tests/shared/classes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:19:29.896203 covalent-cloud-0.20.3rc0/tests/swe_management_tests/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/tests/swe_management_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-08-08 19:19:20.000000 covalent-cloud-0.20.3rc0/tests/swe_management_tests/swe_manager_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.444949 covalent-cloud-0.8.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-29 00:10:27.444949 covalent-cloud-0.8.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.436949 covalent-cloud-0.8.0rc0/covalent_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.436949 covalent-cloud-0.8.0rc0/covalent_cloud/_serialize/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/_serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/_serialize/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/_serialize/electron.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/_serialize/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/_serialize/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/_serialize/transport_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.436949 covalent-cloud-0.8.0rc0/covalent_cloud/analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/analytics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.436949 covalent-cloud-0.8.0rc0/covalent_cloud/cloud_executor/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/cloud_executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/cloud_executor/cloud_executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/covalent_cloud/cloud_executor/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/cloud_executor/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/cloud_executor/models/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/cloud_executor/models/sw_environment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/covalent_cloud/dispatch_management/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/dispatch_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/dispatch_management/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/dispatch_management/interface_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16648 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/dispatch_management/results_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/covalent_cloud/service_account_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/service_account_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/service_account_interface/auth_config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/service_account_interface/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/covalent_cloud/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/covalent_cloud/shared/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/classes/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/classes/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/covalent_cloud/shared/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/schemas/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/schemas/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/schemas/electron.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/schemas/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/schemas/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/schemas/transport_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/covalent_cloud/software_environment/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/software_environment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/covalent_cloud/swe_management/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/swe_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/swe_management/swe_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.436949 covalent-cloud-0.8.0rc0/covalent_cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-29 00:10:27.000000 covalent-cloud-0.8.0rc0/covalent_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-29 00:10:27.000000 covalent-cloud-0.8.0rc0/covalent_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 00:10:27.000000 covalent-cloud-0.8.0rc0/covalent_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-29 00:10:27.000000 covalent-cloud-0.8.0rc0/covalent_cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-29 00:10:27.000000 covalent-cloud-0.8.0rc0/covalent_cloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-29 00:10:27.444949 covalent-cloud-0.8.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.436949 covalent-cloud-0.8.0rc0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/tests/dispatch_management_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/tests/dispatch_management_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/tests/dispatch_management_tests/future_classes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/tests/dispatch_management_tests/helpers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/tests/dispatch_management_tests/interface_functions_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/tests/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/tests/shared/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/tests/shared/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/tests/shared/classes/APIClient_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/tests/shared/classes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/tests/swe_management_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/tests/swe_management_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/tests/swe_management_tests/swe_manager_test.py
```

### Comparing `covalent-cloud-0.20.3rc0/LICENSE` & `covalent-cloud-0.8.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `covalent-cloud-0.20.3rc0/covalent_cloud/_serialize/common.py` & `covalent-cloud-0.8.0rc0/covalent_cloud/_serialize/common.py`

 * *Files identical despite different names*

### Comparing `covalent-cloud-0.20.3rc0/covalent_cloud/_serialize/electron.py` & `covalent-cloud-0.8.0rc0/covalent_cloud/_serialize/electron.py`

 * *Files identical despite different names*

### Comparing `covalent-cloud-0.20.3rc0/covalent_cloud/_serialize/lattice.py` & `covalent-cloud-0.8.0rc0/covalent_cloud/_serialize/lattice.py`

 * *Files identical despite different names*

### Comparing `covalent-cloud-0.20.3rc0/covalent_cloud/_serialize/result.py` & `covalent-cloud-0.8.0rc0/covalent_cloud/_serialize/result.py`

 * *Files identical despite different names*

### Comparing `covalent-cloud-0.20.3rc0/covalent_cloud/_serialize/transport_graph.py` & `covalent-cloud-0.8.0rc0/covalent_cloud/_serialize/transport_graph.py`

 * *Files identical despite different names*

### Comparing `covalent-cloud-0.20.3rc0/covalent_cloud/dispatch_management/helpers.py` & `covalent-cloud-0.8.0rc0/covalent_cloud/dispatch_management/helpers.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,82 +9,63 @@
 from copy import deepcopy
 from functools import wraps
 from pathlib import Path
 from typing import Callable, List, Optional
 
 import requests
 from covalent._results_manager.result import Result
+from covalent._shared_files import logger
 from covalent._shared_files.defaults import parameter_prefix
 from covalent._workflow.lattice import Lattice
-from rich.progress import BarColumn, MofNCompleteColumn, Progress, TaskID
 
 from .._serialize.result import merge_response_manifest, serialize_result, strip_local_uris
 from ..shared.classes.api import APIClient
-from ..shared.classes.exceptions import CovalentAPIKeyError, CovalentSDKError
 from ..shared.classes.settings import Settings, settings
 from ..shared.schemas.asset import AssetSchema
 from ..shared.schemas.result import ResultSchema
 
 _dispatch_executor = ThreadPoolExecutor()
 
 _VALID_EXECUTORS = {"cloud"}
 
+app_log = logger.app_log
 dispatch_cache_dir = Path(settings.dispatch_cache_dir)
 dispatch_cache_dir.mkdir(parents=True, exist_ok=True)
 
 
-class AssetUploadThreadFailure(CovalentSDKError):
-    message: str = "One or more asset upload threads did not finish execution."
-    code: str = "dispatch/asset-upload-thread/fail"
-
-    def __init__(self) -> None:
-        super().__init__(self.message, self.code)
-
-
-class AssetUploadException(CovalentSDKError):
-    message: str = "One or more asset upload raised exceptions."
-    code: str = "dispatch/asset-upload/exception"
-
-    def __init__(self, msg: str = ""):
-        super().__init__(message=msg, code=self.code)
-
-
 def validate_executors(lat: Lattice) -> bool:
 
     # Check lattice default executor and workflow_executor
 
     valid_lattice_executors = True
     valid_electron_executors = True
 
     if lat.metadata["executor"] not in _VALID_EXECUTORS:
-        app_log.debug(f"Found illegal lattice executor: {lat.metadata['executor']}")
         valid_lattice_executors = False
     if lat.metadata["workflow_executor"] not in _VALID_EXECUTORS:
-        app_log.debug(f"Found illegal lattice workflow executor: {lat.metadata['workflow_executor']}")
         valid_lattice_executors = False
 
     tg = lat.transport_graph
 
     for i in tg._graph.nodes:
         name = tg.get_node_value(i, "name")
 
         if name.startswith(parameter_prefix):
             continue
 
         metadata = tg.get_node_value(i, "metadata")
         if metadata["executor"] not in _VALID_EXECUTORS:
-            app_log.debug(f"Found illegal electron executor: {metadata['executor']} in node {i}")
-            valid_electron_executors = False
+            invalid_electron_executors = False
             break
 
     return valid_lattice_executors and valid_electron_executors
 
 
 def inject_parameter_outputs(lat: Lattice):
-    # Hack to pre-compute the output of parameter nodes. This will be
+    # Hack to precompute the output of parameter nodes. This will be
     # no longer needed once OS develop does the same during
     # `build_graph`.
 
     tg = lat.transport_graph
     if not tg._graph.nodes:
         return
 
@@ -141,14 +122,15 @@
         # does this during `build_graph.
 
         inject_parameter_outputs(lattice)
 
         with tempfile.TemporaryDirectory() as tmp_dir:
             manifest = prepare_manifest(lattice, tmp_dir)
             return_manifest = register_manifest(manifest, settings)
+
             dispatch_id = return_manifest.metadata.dispatch_id
 
             path = dispatch_cache_dir / f"{dispatch_id}"
 
             with open(path, "w") as f:
                 f.write(manifest.json())
 
@@ -178,15 +160,15 @@
         Wrapper function which takes the inputs of the workflow as arguments
     """
 
     dispatcher_addr = settings.dispatcher_uri
 
     test_url = f"{dispatcher_addr}/api/v1/dispatchv2/start/{dispatch_id}"
 
-    client = APIClient(host_uri=dispatcher_addr, settings=settings)
+    client = APIClient(host_uri=dispatcher_addr)
     endpoint = f"/api/v1/dispatchv2/start/{dispatch_id}"
 
     try:
         r = client.put(endpoint)
     except requests.exceptions.HTTPError as e:
         print(e.response.text, file=sys.stderr)
         raise e
@@ -210,134 +192,85 @@
 
     Returns:
         Dictionary representation of manifest with asset remote_uris filled in
 
     Side effect:
         If push_assets is False, the server will
         automatically pull the task assets from the submitted asset URIs.
-
-    Raises:
-        CovalentAPIKeyError: If the API key is invalid.
-
     """
+
     dispatcher_addr = settings.dispatcher_uri
 
-    stripped = strip_local_uris(manifest) if push_assets else manifest
-    client = APIClient(host_uri=dispatcher_addr, settings=settings)
+    if push_assets:
+        stripped = strip_local_uris(manifest)
+    else:
+        stripped = manifest
+
+    client = APIClient(host_uri=dispatcher_addr)
     endpoint = "/api/v1/dispatchv2/register"
 
     if parent_dispatch_id:
         endpoint = f"{endpoint}/{parent_dispatch_id}"
 
     try:
         r = client.post(endpoint, request_options={"data": stripped.json()})
     except requests.exceptions.HTTPError as e:
-        if e.response.status_code == 401 and e.response.json()["code"] == "auth/unauthorized":
-            raise CovalentAPIKeyError(
-                message="A valid API key is required to register a dispatch.",
-                code=e.response.json()["code"],
-            ) from e
-        else:
-            raise
+        print(e.response.text, file=sys.stderr)
+        raise e
 
     parsed_resp = ResultSchema.parse_obj(r.json())
 
     return merge_response_manifest(manifest, parsed_resp)
 
 
 def upload_assets(manifest: ResultSchema):
     assets = _extract_assets(manifest)
     _upload(assets)
 
 
 def _extract_assets(manifest: ResultSchema) -> List[AssetSchema]:
+    assets = []
+
     # workflow-level assets
     dispatch_assets = manifest.assets
-    assets = [asset for key, asset in dispatch_assets]
+    for key, asset in dispatch_assets:
+        assets.append(asset)
+
     lattice = manifest.lattice
     lattice_assets = lattice.assets
-    assets.extend(asset for key, asset in lattice_assets)
+    for key, asset in lattice_assets:
+        assets.append(asset)
+
     # Node assets
     tg = lattice.transport_graph
     nodes = tg.nodes
     for node in nodes:
         node_assets = node.assets
-        assets.extend(asset for key, asset in node_assets)
+        for key, asset in node_assets:
+            assets.append(asset)
     return assets
 
 
-def _upload(assets: List[AssetSchema]) -> None:
-    """Upload assets to remote storage.
-
-    Args:
-        assets: List of AssetSchema objects to upload.
-
-    Raises:
-        RuntimeError: If any of the assets fail to upload.
-
-    Returns:
-        None
-
-    """
-    total_assets = len(assets)
+def _upload(assets: List[AssetSchema]):
+    local_scheme_prefix = "file://"
+    total = len(assets)
     _upload_futures = []
-
-    with Progress(
-        "[progress.description]{task.description}",
-        BarColumn(),
-        "[progress.percentage]{task.percentage:>4.1f}%",
-        MofNCompleteColumn(),
-    ) as progress:
-        task = progress.add_task("[green]Uploading assets...", total=total_assets)
-
-        for asset in assets:
-            fut = _dispatch_executor.submit(
-                _upload_asset, asset.uri, asset.remote_uri, task, progress
-            )
-            _upload_futures.append(fut)
-
-        done, _ = wait(_upload_futures)
-
-        if len(done) < total_assets:
-            raise AssetUploadThreadFailure
-
-        _exceptions = []
-        for fut in done:
-            if ex := fut.exception(timeout=0.1):
-                _exceptions.append(ex)
-
-        if _exceptions:
-            msg = f"Failed to upload {len(_exceptions)} out of {total_assets} due to raised exceptions."
-            print(msg, file=sys.stderr)
-            raise AssetUploadException(msg)
+    for i, asset in enumerate(assets):
+        # _upload_asset(asset.uri, asset.remote_uri)
+        fut = _dispatch_executor.submit(_upload_asset, asset.uri, asset.remote_uri)
+        _upload_futures.append(fut)
+        # app_log.debug(f"uploading {i+1} out of {total} assets.")
+    wait(_upload_futures)
 
 
-def _upload_asset(local_uri: str, remote_uri: str, task: TaskID, progress: Progress) -> None:
-    """Upload a single asset to remote storage.
-
-    Args:
-        local_uri: Local URI of the asset to upload.
-        remote_uri: Remote URI to upload the asset to.
-        task: Task ID of the progress bar task.
-        progress: Progress bar object.
-
-    Raises:
-        requests.exceptions.HTTPError: If the upload fails.
-
-    Returns:
-        None
-
-    """
+def _upload_asset(local_uri, remote_uri):
     scheme_prefix = "file://"
     if local_uri.startswith(scheme_prefix):
         local_path = local_uri[len(scheme_prefix) :]
     else:
         local_path = local_uri
 
     with open(local_path, "rb") as f:
         files = {"asset_file": f}
+        # app_log.debug(f"uploading to {remote_uri}")
         r = requests.post(remote_uri, files=files)
         r.raise_for_status()
-
-    if r.status_code == requests.codes.ok:
-        progress.advance(task, advance=1)
-        progress.refresh()
```

### Comparing `covalent-cloud-0.20.3rc0/covalent_cloud/dispatch_management/results_manager.py` & `covalent-cloud-0.8.0rc0/covalent_cloud/dispatch_management/results_manager.py`

 * *Files identical despite different names*

### Comparing `covalent-cloud-0.20.3rc0/covalent_cloud/shared/schemas/electron.py` & `covalent-cloud-0.8.0rc0/covalent_cloud/shared/schemas/electron.py`

 * *Files identical despite different names*

### Comparing `covalent-cloud-0.20.3rc0/covalent_cloud/shared/schemas/lattice.py` & `covalent-cloud-0.8.0rc0/covalent_cloud/shared/schemas/lattice.py`

 * *Files identical despite different names*

### Comparing `covalent-cloud-0.20.3rc0/covalent_cloud/shared/schemas/result.py` & `covalent-cloud-0.8.0rc0/covalent_cloud/shared/schemas/result.py`

 * *Files identical despite different names*

### Comparing `covalent-cloud-0.20.3rc0/covalent_cloud/swe_management/swe_manager.py` & `covalent-cloud-0.8.0rc0/covalent_cloud/swe_management/swe_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 # Copyright 2023 Agnostiq Inc.
 
 """Software environment management module."""
 
 import json
 import tempfile
-from typing import Dict, List, Optional, Tuple, Union
+from typing import Dict, List, Tuple, Union
 
 import requests
 import yaml
 
 from covalent_cloud import get_client
 
-from ..shared.classes.exceptions import CovalentAPIKeyError
-
 COVALENT_CLOUD_URL = "fake.fake"
 API_KEY = "fake"  # pragma: allowlist secret
 
 
 def get_pip_pkgs(pip: Union[str, List[str]]) -> List[str]:
-    """
-    Unpacks the pip packages in the requirements.txt file and combines it into a list of required pip packages.
-
-    """
-
+    """Unpacks the pip packages in the requirements.txt file and combines it into a list of required pip packages."""
     if not isinstance(pip, list):
         pip = [pip]
 
     pip_pkgs = []
     for pkg in pip:
         if pkg.endswith(".txt"):
             with open(pkg, "r") as f:
@@ -34,51 +28,46 @@
         else:
             pip_pkgs.append(pkg)
     return pip_pkgs
 
 
 def unpack_conda_pkgs(
     conda: Union[str, List[str], Dict[str, List[str]]]
-) -> Tuple[List[str], List[str]]:
-    """
-    Unpacks the conda packages in the environment.yml file and combines it into a dictionary of required conda packages.
+) -> Tuple[List[str], List[str], List[str]]:
+    """Unpacks the conda packages in the environment.yml file and combines it into a dictionary of required conda packages.
 
     Returns:
-        channels, dependencies: channels and dependencies according to the conda environment.yml file. Note that these terms are chosen according to the conda nomenclature.
-
+        channels, dependencies, variables: channels, dependencies and variables according to the conda environment.yml file. Note that these terms are chosen according to the conda nomenclature.
     """
-
-    channels, dependencies = [], []
+    channels, dependencies, variables = [], [], []
 
     if isinstance(conda, dict):
         channels = conda.get("channels", [])
         dependencies = conda.get("dependencies", [])
+        variables = conda.get("variables", [])
 
     elif isinstance(conda, str):
         if conda.endswith(".yml"):
             with open(conda, "r") as f:
                 parsed_conda_env_yaml = yaml.safe_load(f)
 
             channels = parsed_conda_env_yaml.get("channels", [])
             dependencies = parsed_conda_env_yaml.get("dependencies", [])
+            variables = parsed_conda_env_yaml.get("variables", [])
 
     elif isinstance(conda, list):
         dependencies = conda
 
-    return channels, dependencies
+    return channels, dependencies, variables
 
 
 def create_env(
-    name: str,
-    pip: Union[str, List[str]],
-    conda: Union[str, List[str], Dict[str, List[str]]],
-    variables: Optional[List] = None,
+    name: str, pip: Union[str, List[str]], conda: Union[str, List[str], Dict[str, List[str]]]
 ) -> None:
-    """
-    Sends the create request to the Covalent Cloud server with the environment dependency list.
+    """Sends the create request to the Covalent Cloud server with the environment dependency list.
 
     Args:
         name: Identifier/name for the software environment.
 
         pip: Python packages to be installed in the environment using pip. This value can be a string `requirements.txt` and/or a list of packages. Note, that if it's a list, it's possible that one of the values is the string `requirements.txt`. In case a `requirements.txt` is passed, it will be parsed into a list of packages and combined with the list of packages passed.`
 
         conda: List of packages to be installed in the environment using conda. This value can either be a list of packages, a filepath to `environment.yml`. It could also be a dictionary with channels, dependencies, and (optionally) variables as keys, and a list of strings as their values. For example:
@@ -86,17 +75,14 @@
             conda={
                         "channels": ["conda-forge", "defaults"],
                         "dependencies": ["numpy=1.21.*", "xarray=0.15.1"],
                         "variables": [{'name': 'mock-variable-1', 'value': '1', 'sensitive': True}]
             }
 
         Whatever is passed, it will be parsed into a dictionary as shown above and sent as JSON to the Covalent Cloud server. If a list of packages is provided, they will be installed using the default conda channel.
-    
-    Returns:
-        None
 
     Examples:
         Create an environment with a list of packages:
             >>> create_env("test-env", ["typing"], ["numpy=1.21.*", "xarray=0.15.1"])
 
         Create an environment with a filepath to `environment.yml`:
             >>> create_env("test-env", "requirements.txt", "environment.yml")
@@ -104,20 +90,16 @@
         Create an environment with a dictionary of channels, dependencies, and variables:
             >>> create_env("test-env", "requirements.txt", {"channels": ["conda-forge", "defaults"], "dependencies": ["numpy=1.21.*", "xarray=0.15.1"], "variables": [{'name': 'mock-variable-1', 'value': '1', 'sensitive': True}]})
 
     Note:
         In case of a conflict of package between pip and conda, pip will take precedence and the conda one will be ignored.
 
     """
-
-    if variables is None:
-        variables = []
-
     pip_pkgs = get_pip_pkgs(pip)
-    channels, dependencies = unpack_conda_pkgs(conda)
+    channels, dependencies, variables = unpack_conda_pkgs(conda)
 
     dependencies.append({"pip": pip_pkgs})
     yaml_template = {
         "name": name,
         "channels": channels,
         "dependencies": dependencies,
     }
@@ -127,61 +109,45 @@
     with tempfile.NamedTemporaryFile(mode="w", suffix=".yml", delete=False) as definition_file:
 
         yaml.dump(yaml_template, definition_file, default_flow_style=False)
 
         client = get_client()
 
         # Open a separate reader in binary mode per Requests doc
-        try:
-            with open(definition_file.name, "rb") as def_file_reader:
-                response = client.post(
-                    "/api/v2/envs",
-                    {
-                        "files": {"definition": def_file_reader},
-                        "data": {"name": name, "variables": json.dumps(variables)},
-                    },
-                )
-        except requests.exceptions.HTTPError as e:
-            if e.response.status_code == 400:
-                print("Environment Already Exists.")
-                return
-            elif (
-                e.response.status_code == 401 and e.response.json()["code"] == "auth/unauthorized"
-            ):
-                CovalentAPIKeyError(
-                    message="A valid API key is required to create an environment.",
-                    code=e.response.json()["code"],
-                ).rich_print(level="error")
-                return
-            else:
-                raise
+        with open(definition_file.name, "rb") as def_file_reader:
+            response = client.post(
+                "/api/v2/envs",
+                {
+                    "files": {"definition": def_file_reader},
+                    "data": {"name": name, "variables": json.dumps(variables)},
+                },
+            )
+
+        if response.status_code == 400:
+            print("Environment Already Exists.")
+            return
 
+        response.raise_for_status()
         response_body = response.json()
 
     print(f"Name: {response_body['name']}")
     print(f"Status: {response_body['status']}")
-    print(f"Estimated Time: {response_body['estimated_time']} seconds")
+    print(f"Estimated Time: {response_body['estimated_time']}")
 
     print("Environment file contains:")
     print("==========================")
     print(yaml.dump(yaml_template, default_flow_style=False))
 
 
 def delete_env(env_name: str) -> None:
-    """
-    Sends the delete request to the Covalent Cloud server with the environment name to be deleted.
+    """Sends the delete request to the Covalent Cloud server with the environment name to be deleted.
 
     Args:
         env_name: Identifier/name for the software environment.
-    
-    Returns:
-        None
-
     """
-
     params = {"env_name": env_name, "api_key": API_KEY}
 
     response = requests.delete(f"{COVALENT_CLOUD_URL}/delete_env", params=params)
     response.raise_for_status()
 
     response_body = {
         "name": "Deleting",
```

### Comparing `covalent-cloud-0.20.3rc0/pyproject.toml` & `covalent-cloud-0.8.0rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `covalent-cloud-0.20.3rc0/setup.py` & `covalent-cloud-0.8.0rc0/setup.py`

 * *Files identical despite different names*

### Comparing `covalent-cloud-0.20.3rc0/tests/dispatch_management_tests/future_classes_test.py` & `covalent-cloud-0.8.0rc0/tests/dispatch_management_tests/future_classes_test.py`

 * *Files identical despite different names*

### Comparing `covalent-cloud-0.20.3rc0/tests/dispatch_management_tests/helpers_test.py` & `covalent-cloud-0.8.0rc0/tests/dispatch_management_tests/helpers_test.py`

 * *Files identical despite different names*

### Comparing `covalent-cloud-0.20.3rc0/tests/dispatch_management_tests/interface_functions_test.py` & `covalent-cloud-0.8.0rc0/tests/dispatch_management_tests/interface_functions_test.py`

 * *Files identical despite different names*

### Comparing `covalent-cloud-0.20.3rc0/tests/shared/classes/APIClient_test.py` & `covalent-cloud-0.8.0rc0/tests/shared/classes/APIClient_test.py`

 * *Files identical despite different names*

### Comparing `covalent-cloud-0.20.3rc0/tests/swe_management_tests/swe_manager_test.py` & `covalent-cloud-0.8.0rc0/tests/swe_management_tests/swe_manager_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     "bokeh=2.4.2",
     "conda-forge::numpy=1.21.*",
     "nodejs=16.13.*",
     "flask",
     "pip",
     {"pip": ["Flask-Testing"]},
 ]
+CONDA_VARIABLES = []
 MOCK_CONDA_ENV_NAME = "mockenv"
 MOCK_PIP_PKGS = ["mock-package-1", "mock-package-2"]
 MOCK_CHANNELS = ["mock-channel-1", "mock-channel-2"]
 MOCK_DEPENDENCIES = [
     "mock-dependency-1",
     "mock-dependency-2",
     {"pip": ["mock-pip-dependency-1", "mock-pip-dependency-2"]},
@@ -112,40 +113,43 @@
     assert pip_pkgs == ["mock-package"] + PIP_PKGS + ["mock-package-2"]
     remove_temp_requirement_file()
 
 
 def test_unpack_conda_pkgs_str():
     """Test the unpack conda packages function."""
     create_conda_env_file()
-    channels, dependencies = unpack_conda_pkgs(TEMP_ENV_YML_FILEPATH)
+    channels, dependencies, variables = unpack_conda_pkgs(TEMP_ENV_YML_FILEPATH)
     assert channels == CONDA_CHANNELS
     assert dependencies == CONDA_DEPENDENCIES
+    assert variables == CONDA_VARIABLES
     remove_conda_env_file()
 
 
 def test_unpack_conda_pkgs_list():
     """Test the unpack conda packages function."""
     create_conda_env_file()
-    channels, dependencies = unpack_conda_pkgs(CONDA_DEPENDENCIES)
-    assert channels == []
+    channels, dependencies, variables = unpack_conda_pkgs(CONDA_DEPENDENCIES)
+    assert channels == variables == []
     assert dependencies == CONDA_DEPENDENCIES
     remove_conda_env_file()
 
 
 def test_unpack_conda_pkgs_dict():
     """Test the unpack conda packages function."""
     create_conda_env_file()
-    channels, dependencies = unpack_conda_pkgs(
+    channels, dependencies, variables = unpack_conda_pkgs(
         {
             "channels": CONDA_CHANNELS,
             "dependencies": CONDA_DEPENDENCIES,
+            "variables": CONDA_VARIABLES,
         }
     )
     assert channels == CONDA_CHANNELS
     assert dependencies == CONDA_DEPENDENCIES
+    assert variables == CONDA_VARIABLES
     remove_conda_env_file()
 
 
 def test_create_env(mocker):
     """Test the create environment function."""
     MOCK_CREATE_DEPENDENCIES = ["mock-dependency-1", "mock-dependency-2"]
     AuthConfigManager.save_api_key(API_KEY)  # This will overite your local key
@@ -161,18 +165,18 @@
     mocker.patch("covalent_cloud.swe_management.swe_manager.open", return_value=mock_ctx_mgr)
 
     get_pip_pkgs_mock = mocker.patch(
         "covalent_cloud.swe_management.swe_manager.get_pip_pkgs", return_value=MOCK_PIP_PKGS
     )
     unpack_conda_pkgs_mock = mocker.patch(
         "covalent_cloud.swe_management.swe_manager.unpack_conda_pkgs",
-        return_value=(MOCK_CHANNELS, MOCK_CREATE_DEPENDENCIES),
+        return_value=(MOCK_CHANNELS, MOCK_CREATE_DEPENDENCIES, MOCK_VARIABLES),
     )
 
-    create_env(MOCK_CONDA_ENV_NAME, MOCK_PIP_PKGS, MOCK_CREATE_DEPENDENCIES, MOCK_VARIABLES)
+    create_env(MOCK_CONDA_ENV_NAME, MOCK_PIP_PKGS, MOCK_CREATE_DEPENDENCIES)
 
     get_pip_pkgs_mock.assert_called_once_with(MOCK_PIP_PKGS)
     unpack_conda_pkgs_mock.assert_called_once_with(MOCK_CREATE_DEPENDENCIES)
 
     data = {
         "name": MOCK_CONDA_ENV_NAME,
         "variables": json.dumps(MOCK_VARIABLES),
```

