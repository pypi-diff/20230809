# Comparing `tmp/metricsoperator-0.0.12.1.tar.gz` & `tmp/metricsoperator-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metricsoperator-0.0.12.1.tar", last modified: Mon Aug  7 23:24:43 2023, max compression
+gzip compressed data, was "metricsoperator-0.0.13.tar", last modified: Tue Aug  8 15:53:13 2023, max compression
```

## Comparing `metricsoperator-0.0.12.1.tar` & `metricsoperator-0.0.13.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-08-07 23:24:43.988249 metricsoperator-0.0.12.1/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      169 2023-08-06 22:03:40.000000 metricsoperator-0.0.12.1/MANIFEST.in
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1957 2023-08-07 23:24:43.988249 metricsoperator-0.0.12.1/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1100 2023-08-06 22:12:21.000000 metricsoperator-0.0.12.1/README.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-08-07 23:24:43.988249 metricsoperator-0.0.12.1/metricsoperator/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       44 2023-08-06 22:03:40.000000 metricsoperator-0.0.12.1/metricsoperator/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1542 2023-08-07 23:24:08.000000 metricsoperator-0.0.12.1/metricsoperator/client.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-08-07 23:24:43.988249 metricsoperator-0.0.12.1/metricsoperator/metrics/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      539 2023-08-07 19:31:15.000000 metricsoperator-0.0.12.1/metricsoperator/metrics/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7156 2023-08-07 23:24:08.000000 metricsoperator-0.0.12.1/metricsoperator/metrics/base.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4171 2023-08-07 23:24:08.000000 metricsoperator-0.0.12.1/metricsoperator/metrics/network.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      799 2023-08-07 23:24:08.000000 metricsoperator-0.0.12.1/metricsoperator/metrics/storage.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      613 2023-08-07 05:09:52.000000 metricsoperator-0.0.12.1/metricsoperator/utils.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-08-07 23:24:43.988249 metricsoperator-0.0.12.1/metricsoperator.egg-info/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1957 2023-08-07 23:24:43.000000 metricsoperator-0.0.12.1/metricsoperator.egg-info/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      494 2023-08-07 23:24:43.000000 metricsoperator-0.0.12.1/metricsoperator.egg-info/SOURCES.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-08-07 23:24:43.000000 metricsoperator-0.0.12.1/metricsoperator.egg-info/dependency_links.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-08-06 04:14:56.000000 metricsoperator-0.0.12.1/metricsoperator.egg-info/not-zip-safe
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       27 2023-08-07 23:24:43.000000 metricsoperator-0.0.12.1/metricsoperator.egg-info/requires.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       16 2023-08-07 23:24:43.000000 metricsoperator-0.0.12.1/metricsoperator.egg-info/top_level.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      132 2023-08-06 22:03:40.000000 metricsoperator-0.0.12.1/pyproject.toml
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       38 2023-08-07 23:24:43.988249 metricsoperator-0.0.12.1/setup.cfg
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2259 2023-08-07 23:24:08.000000 metricsoperator-0.0.12.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:13.903001 metricsoperator-0.0.13/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-08-08 15:52:32.000000 metricsoperator-0.0.13/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-08-08 15:53:13.903001 metricsoperator-0.0.13/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-08 15:52:32.000000 metricsoperator-0.0.13/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:13.899001 metricsoperator-0.0.13/metricsoperator/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-08 15:52:32.000000 metricsoperator-0.0.13/metricsoperator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-08-08 15:52:32.000000 metricsoperator-0.0.13/metricsoperator/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:13.903001 metricsoperator-0.0.13/metricsoperator/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-08 15:52:32.000000 metricsoperator-0.0.13/metricsoperator/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7156 2023-08-08 15:52:32.000000 metricsoperator-0.0.13/metricsoperator/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-08-08 15:52:32.000000 metricsoperator-0.0.13/metricsoperator/metrics/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-08-08 15:52:32.000000 metricsoperator-0.0.13/metricsoperator/metrics/perf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-08-08 15:52:32.000000 metricsoperator-0.0.13/metricsoperator/metrics/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-08-08 15:52:32.000000 metricsoperator-0.0.13/metricsoperator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:53:13.899001 metricsoperator-0.0.13/metricsoperator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-08-08 15:53:13.000000 metricsoperator-0.0.13/metricsoperator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-08-08 15:53:13.000000 metricsoperator-0.0.13/metricsoperator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 15:53:13.000000 metricsoperator-0.0.13/metricsoperator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 15:53:13.000000 metricsoperator-0.0.13/metricsoperator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-08 15:53:13.000000 metricsoperator-0.0.13/metricsoperator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-08 15:53:13.000000 metricsoperator-0.0.13/metricsoperator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-08-08 15:52:32.000000 metricsoperator-0.0.13/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 15:53:13.903001 metricsoperator-0.0.13/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-08-08 15:52:32.000000 metricsoperator-0.0.13/setup.py
```

### Comparing `metricsoperator-0.0.12.1/PKG-INFO` & `metricsoperator-0.0.13/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: metricsoperator
-Version: 0.0.12.1
+Version: 0.0.13
 Summary: Python helpers for the Metrics Operator
 Home-page: https://github.com/converged-computing/metrics-operator/tree/main/python-sdk/v1alpha1
 Author: Vanessasaurus
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessasaurus
 License: MIT
 Keywords: metrics-operator,hpc,kubernetes,metrics,storage,applications
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
@@ -38,9 +37,7 @@
 See [LICENSE](https://github.com/converged-computing/cloud-select/blob/main/LICENSE),
 [COPYRIGHT](https://github.com/converged-computing/cloud-select/blob/main/COPYRIGHT), and
 [NOTICE](https://github.com/converged-computing/cloud-select/blob/main/NOTICE) for details.
 
 SPDX-License-Identifier: (MIT)
 
 LLNL-CODE- 842614
-
-
```

### Comparing `metricsoperator-0.0.12.1/README.md` & `metricsoperator-0.0.13/README.md`

 * *Files identical despite different names*

### Comparing `metricsoperator-0.0.12.1/metricsoperator/client.py` & `metricsoperator-0.0.13/metricsoperator/client.py`

 * *Files identical despite different names*

### Comparing `metricsoperator-0.0.12.1/metricsoperator/metrics/__init__.py` & `metricsoperator-0.0.13/metricsoperator/metrics/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # Copyright 2023 Lawrence Livermore National Security, LLC
 # (c.f. AUTHORS, NOTICE.LLNS, COPYING)
 
 from .network import network_netmark, network_osu_benchmark
+from .perf import perf_sysstat
 from .storage import io_sysstat
 
 metrics = {
     "io-sysstat": io_sysstat,
     "network-osu-benchmark": network_osu_benchmark,
     "network-netmark": network_netmark,
+    "perf-sysstat": perf_sysstat,
 }
 
 
 def get_metric(name):
     """
     Get a named metric parser.
     """
```

### Comparing `metricsoperator-0.0.12.1/metricsoperator/metrics/base.py` & `metricsoperator-0.0.13/metricsoperator/metrics/base.py`

 * *Files identical despite different names*

### Comparing `metricsoperator-0.0.12.1/metricsoperator/metrics/network.py` & `metricsoperator-0.0.13/metricsoperator/metrics/network.py`

 * *Files identical despite different names*

### Comparing `metricsoperator-0.0.12.1/metricsoperator/metrics/storage.py` & `metricsoperator-0.0.13/metricsoperator/metrics/storage.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     def parse_log(self, lines):
         """
         Given lines of output, parse and return json
         """
         # Get the log metadata
         metadata = self.get_log_metadata(lines)
 
-        # Split lines by IOSTAT TIMEPOINT
+        # Split and parse output lines
         results = []
         sections = self.get_log_sections(lines)
         for section in sections:
             if not section.strip():
                 continue
             results.append(json.loads(section))
         return {"data": results, "metadata": metadata, "spec": self.spec}
```

### Comparing `metricsoperator-0.0.12.1/metricsoperator/utils.py` & `metricsoperator-0.0.13/metricsoperator/utils.py`

 * *Files identical despite different names*

### Comparing `metricsoperator-0.0.12.1/metricsoperator.egg-info/PKG-INFO` & `metricsoperator-0.0.13/metricsoperator.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: metricsoperator
-Version: 0.0.12.1
+Version: 0.0.13
 Summary: Python helpers for the Metrics Operator
 Home-page: https://github.com/converged-computing/metrics-operator/tree/main/python-sdk/v1alpha1
 Author: Vanessasaurus
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessasaurus
 License: MIT
 Keywords: metrics-operator,hpc,kubernetes,metrics,storage,applications
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
@@ -38,9 +37,7 @@
 See [LICENSE](https://github.com/converged-computing/cloud-select/blob/main/LICENSE),
 [COPYRIGHT](https://github.com/converged-computing/cloud-select/blob/main/COPYRIGHT), and
 [NOTICE](https://github.com/converged-computing/cloud-select/blob/main/NOTICE) for details.
 
 SPDX-License-Identifier: (MIT)
 
 LLNL-CODE- 842614
-
-
```

### Comparing `metricsoperator-0.0.12.1/setup.py` & `metricsoperator-0.0.13/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ################################################################################
 # MAIN #########################################################################
 ################################################################################
 
 if __name__ == "__main__":
     setup(
         name="metricsoperator",
-        version="0.0.12.1",
+        version="0.0.13",
         author="Vanessasaurus",
         author_email="vsoch@users.noreply.github.com",
         maintainer="Vanessasaurus",
         packages=find_packages(),
         include_package_data=True,
         zip_safe=False,
         url="https://github.com/converged-computing/metrics-operator/tree/main/python-sdk/v1alpha1",
```

