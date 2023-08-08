# Comparing `tmp/openpmd-beamphysics-0.7.8.tar.gz` & `tmp/openpmd-beamphysics-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/openPMD-beamphysics/openPMD-beamphysics/dist/.tmp-hv9qnal5/openpmd-beamphysics-0.7.8.tar", last modified: Wed Aug  2 16:41:41 2023, max compression
+gzip compressed data, was "/home/runner/work/openPMD-beamphysics/openPMD-beamphysics/dist/.tmp-683u7c6c/openpmd-beamphysics-0.7.9.tar", last modified: Tue Aug  8 23:39:04 2023, max compression
```

## Comparing `openpmd-beamphysics-0.7.8.tar` & `openpmd-beamphysics-0.7.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:41:41.000000 openpmd-beamphysics-0.7.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-08-02 16:41:41.000000 openpmd-beamphysics-0.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:41:41.000000 openpmd-beamphysics-0.7.8/openpmd_beamphysics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-08-02 16:41:41.000000 openpmd-beamphysics-0.7.8/openpmd_beamphysics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-08-02 16:41:41.000000 openpmd-beamphysics-0.7.8/openpmd_beamphysics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 16:41:41.000000 openpmd-beamphysics-0.7.8/openpmd_beamphysics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 16:41:41.000000 openpmd-beamphysics-0.7.8/openpmd_beamphysics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-02 16:41:41.000000 openpmd-beamphysics-0.7.8/openpmd_beamphysics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:41:41.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-02 16:41:41.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:41:41.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/fields/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12849 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/fields/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/fields/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/fields/expansion.py
--rw-r--r--   0 runner    (1001) docker     (123)    24315 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/fields/fieldmesh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:41:41.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/ansys.py
--rw-r--r--   0 runner    (1001) docker     (123)    14199 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/astra.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/bmad.py
--rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/elegant.py
--rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/genesis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)    22750 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/impact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/litrack.py
--rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/lucretia.py
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/opal.py
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/simion.py
--rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/superfish.py
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/particles.py
--rw-r--r--   0 runner    (1001) docker     (123)    12072 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    10189 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/species.py
--rw-r--r--   0 runner    (1001) docker     (123)    12643 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    14211 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/writers.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-08-02 16:41:41.000000 openpmd-beamphysics-0.7.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:41:41.000000 openpmd-beamphysics-0.7.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/tests/test_particlegroup.py
--rw-r--r--   0 runner    (1001) docker     (123)    78254 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:39:04.000000 openpmd-beamphysics-0.7.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-08 23:38:52.000000 openpmd-beamphysics-0.7.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-08 23:38:52.000000 openpmd-beamphysics-0.7.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-08-08 23:39:04.000000 openpmd-beamphysics-0.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-08-08 23:38:52.000000 openpmd-beamphysics-0.7.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:39:04.000000 openpmd-beamphysics-0.7.9/openpmd_beamphysics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-08-08 23:39:04.000000 openpmd-beamphysics-0.7.9/openpmd_beamphysics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-08-08 23:39:04.000000 openpmd-beamphysics-0.7.9/openpmd_beamphysics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 23:39:04.000000 openpmd-beamphysics-0.7.9/openpmd_beamphysics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-08 23:39:04.000000 openpmd-beamphysics-0.7.9/openpmd_beamphysics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-08 23:39:04.000000 openpmd-beamphysics-0.7.9/openpmd_beamphysics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:39:04.000000 openpmd-beamphysics-0.7.9/pmd_beamphysics/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-08-08 23:38:52.000000 openpmd-beamphysics-0.7.9/pmd_beamphysics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-08 23:39:04.000000 openpmd-beamphysics-0.7.9/pmd_beamphysics/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:39:04.000000 openpmd-beamphysics-0.7.9/pmd_beamphysics/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 23:38:52.000000 openpmd-beamphysics-0.7.9/pmd_beamphysics/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12849 2023-08-08 23:38:52.000000 openpmd-beamphysics-0.7.9/pmd_beamphysics/fields/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-08-08 23:38:52.000000 openpmd-beamphysics-0.7.9/pmd_beamphysics/fields/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-08-08 23:38:52.000000 openpmd-beamphysics-0.7.9/pmd_beamphysics/fields/expansion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24315 2023-08-08 23:38:52.000000 openpmd-beamphysics-0.7.9/pmd_beamphysics/fields/fieldmesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:39:04.000000 openpmd-beamphysics-0.7.9/pmd_beamphysics/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 23:38:52.000000 openpmd-beamphysics-0.7.9/pmd_beamphysics/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-08-08 23:38:52.000000 openpmd-beamphysics-0.7.9/pmd_beamphysics/interfaces/ansys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14199 2023-08-08 23:38:52.000000 openpmd-beamphysics-0.7.9/pmd_beamphysics/interfaces/astra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-08-08 23:38:52.000000 openpmd-beamphysics-0.7.9/pmd_beamphysics/interfaces/bmad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-08-08 23:38:52.000000 openpmd-beamphysics-0.7.9/pmd_beamphysics/interfaces/elegant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-08-08 23:38:52.000000 openpmd-beamphysics-0.7.9/pmd_beamphysics/interfaces/genesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-08-08 23:38:52.000000 openpmd-beamphysics-0.7.9/pmd_beamphysics/interfaces/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22750 2023-08-08 23:38:52.000000 openpmd-beamphysics-0.7.9/pmd_beamphysics/interfaces/impact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-08-08 23:38:52.000000 openpmd-beamphysics-0.7.9/pmd_beamphysics/interfaces/litrack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-08-08 23:38:52.000000 openpmd-beamphysics-0.7.9/pmd_beamphysics/interfaces/lucretia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-08-08 23:38:52.000000 openpmd-beamphysics-0.7.9/pmd_beamphysics/interfaces/opal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-08-08 23:38:52.000000 openpmd-beamphysics-0.7.9/pmd_beamphysics/interfaces/simion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-08-08 23:38:52.000000 openpmd-beamphysics-0.7.9/pmd_beamphysics/interfaces/superfish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-08-08 23:38:52.000000 openpmd-beamphysics-0.7.9/pmd_beamphysics/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37374 2023-08-08 23:38:52.000000 openpmd-beamphysics-0.7.9/pmd_beamphysics/particles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14578 2023-08-08 23:38:52.000000 openpmd-beamphysics-0.7.9/pmd_beamphysics/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10189 2023-08-08 23:38:52.000000 openpmd-beamphysics-0.7.9/pmd_beamphysics/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-08 23:38:52.000000 openpmd-beamphysics-0.7.9/pmd_beamphysics/species.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12643 2023-08-08 23:38:52.000000 openpmd-beamphysics-0.7.9/pmd_beamphysics/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-08-08 23:38:52.000000 openpmd-beamphysics-0.7.9/pmd_beamphysics/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-08-08 23:38:52.000000 openpmd-beamphysics-0.7.9/pmd_beamphysics/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15245 2023-08-08 23:38:52.000000 openpmd-beamphysics-0.7.9/pmd_beamphysics/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-08-08 23:38:52.000000 openpmd-beamphysics-0.7.9/pmd_beamphysics/writers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-08 23:38:52.000000 openpmd-beamphysics-0.7.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-08-08 23:39:04.000000 openpmd-beamphysics-0.7.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-08-08 23:38:52.000000 openpmd-beamphysics-0.7.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 23:39:04.000000 openpmd-beamphysics-0.7.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-08 23:38:52.000000 openpmd-beamphysics-0.7.9/tests/test_particlegroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78254 2023-08-08 23:38:52.000000 openpmd-beamphysics-0.7.9/versioneer.py
```

### Comparing `openpmd-beamphysics-0.7.8/LICENSE` & `openpmd-beamphysics-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.8/PKG-INFO` & `openpmd-beamphysics-0.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openpmd-beamphysics
-Version: 0.7.8
+Version: 0.7.9
 Home-page: https://github.com/ChristopherMayes/openPMD-beamphysics
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # openPMD-beamphysics
```

### Comparing `openpmd-beamphysics-0.7.8/README.md` & `openpmd-beamphysics-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.8/openpmd_beamphysics.egg-info/PKG-INFO` & `openpmd-beamphysics-0.7.9/openpmd_beamphysics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openpmd-beamphysics
-Version: 0.7.8
+Version: 0.7.9
 Home-page: https://github.com/ChristopherMayes/openPMD-beamphysics
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # openPMD-beamphysics
```

### Comparing `openpmd-beamphysics-0.7.8/openpmd_beamphysics.egg-info/SOURCES.txt` & `openpmd-beamphysics-0.7.9/openpmd_beamphysics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.8/pmd_beamphysics/fields/analysis.py` & `openpmd-beamphysics-0.7.9/pmd_beamphysics/fields/analysis.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.8/pmd_beamphysics/fields/conversion.py` & `openpmd-beamphysics-0.7.9/pmd_beamphysics/fields/conversion.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.8/pmd_beamphysics/fields/expansion.py` & `openpmd-beamphysics-0.7.9/pmd_beamphysics/fields/expansion.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.8/pmd_beamphysics/fields/fieldmesh.py` & `openpmd-beamphysics-0.7.9/pmd_beamphysics/fields/fieldmesh.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/ansys.py` & `openpmd-beamphysics-0.7.9/pmd_beamphysics/interfaces/ansys.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/astra.py` & `openpmd-beamphysics-0.7.9/pmd_beamphysics/interfaces/astra.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/bmad.py` & `openpmd-beamphysics-0.7.9/pmd_beamphysics/interfaces/bmad.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/elegant.py` & `openpmd-beamphysics-0.7.9/pmd_beamphysics/interfaces/elegant.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/genesis.py` & `openpmd-beamphysics-0.7.9/pmd_beamphysics/interfaces/genesis.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/gpt.py` & `openpmd-beamphysics-0.7.9/pmd_beamphysics/interfaces/gpt.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/impact.py` & `openpmd-beamphysics-0.7.9/pmd_beamphysics/interfaces/impact.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/litrack.py` & `openpmd-beamphysics-0.7.9/pmd_beamphysics/interfaces/litrack.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/lucretia.py` & `openpmd-beamphysics-0.7.9/pmd_beamphysics/interfaces/lucretia.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/opal.py` & `openpmd-beamphysics-0.7.9/pmd_beamphysics/interfaces/opal.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/simion.py` & `openpmd-beamphysics-0.7.9/pmd_beamphysics/interfaces/simion.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/superfish.py` & `openpmd-beamphysics-0.7.9/pmd_beamphysics/interfaces/superfish.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.8/pmd_beamphysics/labels.py` & `openpmd-beamphysics-0.7.9/pmd_beamphysics/labels.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.8/pmd_beamphysics/particles.py` & `openpmd-beamphysics-0.7.9/pmd_beamphysics/particles.py`

 * *Files 3% similar despite different names*

```diff
@@ -817,34 +817,101 @@
             g = h5
     
         write_pmd_bunch(g, self, name=name)        
         
         
     # Plotting
     # --------
-    # TODO: more general plotting
-    def plot(self, key1='x', key2=None, bins=None, return_figure=False, 
-             tex=True, **kwargs):
+    def plot(self, key1='x', key2=None,
+             bins=None,
+             *,
+             xlim=None,
+             ylim=None,
+             return_figure=False, 
+             tex=True, nice=True,
+             **kwargs):
         """
         1d or 2d density plot. 
+        
+        If one key is given, this will plot the density of that key.
+        Example:
+            .plot('x')
+        
+        If two keys arg given, this will plot a 2d marginal plot.
+        Example:
+            .plot('x', 'px')
+            
+        
+        Parameters
+        ----------
+        particle_group: ParticleGroup
+            The object to plot
+        
+        key1: str, default = 't'
+            Key to bin on the x-axis
+            
+        key2: str, default = None
+            Key to bin on the y-axis. 
+            
+        bins: int, default = None
+           Number of bins. If None, this will use a heuristic: bins = sqrt(n_particle/4)
+    
+        xlim: tuple, default = None
+            Manual setting of the x-axis limits. Note that these are in raw, unscaled units. 
+            
+        ylim: tuple, default = None
+            Manual setting of the y-axis limits. Note that these are in raw, unscaled units. 
+            
+        tex: bool, default = True
+            Use TEX for labels   
+            
+        nice: bool, default = True
+            Scale to nice units
+            
+        return_figure: bool, default = False
+            If true, return a matplotlib.figure.Figure object
+            
+        **kwargs
+            Any additional kwargs to send to the the plot in: plt.subplots(**kwargs)
+            
+        
+        Returns
+        -------
+        None or fig: matplotlib.figure.Figure
+            This only returns a figure object if return_figure=T, otherwise returns None
+            
         """
         
         if not key2:
-            fig = density_plot(self, key=key1, bins=bins, tex=tex, **kwargs)
+            fig = density_plot(self, key=key1,
+                               bins=bins,
+                               xlim=xlim,
+                               tex=tex,
+                               nice=nice,
+                               **kwargs)
         else:
-            fig = marginal_plot(self, key1=key1, key2=key2, bins=bins, tex=tex, **kwargs)
+            fig = marginal_plot(self, key1=key1, key2=key2,
+                                bins=bins,
+                                xlim=xlim,
+                                ylim=ylim,
+                                tex=tex,
+                                nice=nice,
+                                **kwargs)
         
         if return_figure:
             return fig
         
     def slice_plot(self, key='sigma_x', 
                    n_slice=100,
                    slice_key=None,
                    tex=True,
+                   nice=True,
                    return_figure=False,
+                   xlim=None,
+                   ylim=None,
                    **kwargs):
         """
         Slice statistics plot. 
         
         """        
                   
         if not slice_key:
@@ -853,14 +920,17 @@
             else:
                 slice_key = 't'
             
         fig = slice_plot(self, stat_key=key,
                          n_slice=n_slice,
                          slice_key=slice_key,
                          tex=tex,
+                         nice=nice,
+                         xlim=xlim,
+                         ylim=ylim,
                          **kwargs)
         
         if return_figure:
             return fig
         
         
     # New constructors
```

### Comparing `openpmd-beamphysics-0.7.8/pmd_beamphysics/plot.py` & `openpmd-beamphysics-0.7.9/pmd_beamphysics/plot.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 
 
 """
 
-from  pmd_beamphysics.units import nice_array, nice_scale_prefix
+from pmd_beamphysics.units import nice_array, plottable_array, nice_scale_prefix
 from pmd_beamphysics.labels import mathlabel
 
 
 from .statistics import slice_statistics
 import matplotlib.pyplot as plt
 import matplotlib
 from matplotlib.gridspec import GridSpec
@@ -37,83 +37,123 @@
 
     
     
 def slice_plot(particle_group, 
                stat_key='sigma_x',
                n_slice=40,
                slice_key='z',
+               xlim=None,
+               ylim=None,
                tex=True,
+               nice=True,
                **kwargs):
     """
     Complete slice plotting routine. Will plot the density of the slice key on the right axis. 
+    
+    Parameters
+    ----------
+    particle_group: ParticleGroup
+        The object to plot
+    
+    stat_key: str, default = 'sigma_x'
+        Key to calculate the statistics
+        
+    n_slice: int, default = 40
+        Number of slices 
+        
+    slice_key: str, default = 'z'
+        Should be 'z' or 't'
+        
+    ylim: tuple, default = None
+        Manual setting of the y-axis limits. 
+        
+    tex: bool, defaul = True
+        Use TEX for labels
+        
+    
+    Returns
+    -------
+    fig: matplotlib.figure.Figure
+
     """
     
     x_key = 'mean_'+slice_key
     y_key = stat_key
     slice_dat = slice_statistics(particle_group, n_slice=n_slice, slice_key=slice_key,
                             keys=[x_key, y_key, 'ptp_'+slice_key, 'charge'])
     
     
     slice_dat['density'] = slice_dat['charge']/ slice_dat['ptp_'+slice_key]
     y2_key = 'density'
     fig, ax = plt.subplots(**kwargs)
     
     # Get nice arrays
-    x, _, prex = nice_array(slice_dat[x_key])
-    y, _, prey = nice_array(slice_dat[y_key])
-    y2, _, prey2 = nice_array(slice_dat[y2_key])
+    x, f1, prex, xmin, xmax       = plottable_array(slice_dat[x_key], nice=nice, lim=xlim)
+    y, f2, prey, ymin, ymax = plottable_array(slice_dat[y_key], nice=nice, lim=ylim)
+    # Density on r.h.s
+    y2, _, prey2, _, _ = plottable_array(slice_dat[y2_key], nice=nice, lim=None)
     
     x_units = f'{prex}{particle_group.units(x_key)}'
     y_units = f'{prey}{particle_group.units(y_key)}'    
     
     # Convert to Amps if possible
     y2_units = f'C/{particle_group.units(x_key)}'
     if y2_units == 'C/s':
         y2_units = 'A'
     y2_units = prey2+y2_units 
     
     # Labels
-    
-
     labelx = mathlabel(slice_key, units=x_units, tex=tex)
     labely = mathlabel(y_key, units=y_units, tex=tex)    
     labely2 = mathlabel(y2_key, units=y2_units, tex=tex)        
     
     ax.set_xlabel(labelx)
     ax.set_ylabel(labely)
     
     # Main plot
     ax.plot(x, y, color = 'black')
-    
-    #ax.set_ylim(0, 1.1*ymax )
 
+    # rhs plot
     ax2 = ax.twinx()
     ax2.set_ylabel(labely2)
     ax2.fill_between(x, 0, y2, color='black', alpha = 0.2)  
+    ax2.set_ylim(0, None)
     
+    # Actual plot limits, considering scaling
+    if xlim:
+        ax.set_xlim( xmin/f1, xmax/f1) 
+    if ylim:
+        ax.set_ylim( ymin/f2, ymax/f2)              
+
     return fig
 
     
     
-def density_plot(particle_group, key='x', bins=None, tex=True, **kwargs):
+def density_plot(particle_group, key='x',
+                 bins=None,
+                 *, 
+                 xlim=None,
+                 tex=True,
+                 nice=True,
+                 **kwargs):
     """
     1D density plot. Also see: marginal_plot
     
     Example:
     
         density_plot(P, 'x', bins=100)   
     
     """
     
     if not bins:
         n = len(particle_group)
         bins = int(n/100)
 
     # Scale to nice units and get the factor, unit prefix
-    x, f1, p1 = nice_array(particle_group[key])
+    x, f1, p1, xmin, xmax = plottable_array(particle_group[key], nice=nice, lim=xlim)
     w = particle_group['weight']
     u1 = particle_group.units(key).unitSymbol
     ux = p1+u1
     
     # mathtext label
     labelx = mathlabel(key, units=ux, tex=tex)
 
@@ -130,34 +170,80 @@
         ax.set_ylabel(f'{hist_prefix}A')
     else:
         ax.set_ylabel(f'{hist_prefix}C/{ux}')
     
 
     ax.set_xlabel(labelx)  
     
+    # Limits
+    if xlim:
+        ax.set_xlim(xmin/f1, xmax/f1)
+    
     return fig
         
-def marginal_plot(particle_group, key1='t', key2='p', bins=None, tex=True, **kwargs):
+def marginal_plot(particle_group, key1='t', key2='p', 
+                  bins=None,
+                  *,
+                  xlim=None,
+                  ylim=None,
+                  tex=True,
+                  nice=True,
+                  **kwargs):
     """
     Density plot and projections
     
     Example:
     
         marginal_plot(P, 't', 'energy', bins=200)   
+        
+        
+    Parameters
+    ----------
+    particle_group: ParticleGroup
+        The object to plot
     
-    """
+    key1: str, default = 't'
+        Key to bin on the x-axis
+        
+    key2: str, default = 'p'
+        Key to bin on the y-axis        
+        
+    bins: int, default = None
+       Number of bins. If None, this will use a heuristic: bins = sqrt(n_particle/4)
+
+    xlim: tuple, default = None
+        Manual setting of the x-axis limits. 
+        
+    ylim: tuple, default = None
+        Manual setting of the y-axis limits. 
+        
+    tex: bool, default = True
+        Use TEX for labels
+        
+    nice: bool, default = True
+        
+    
+    Returns
+    -------
+    fig: matplotlib.figure.Figure        
+        
     
+    """    
     if not bins:
         n = len(particle_group)
         bins = int(np.sqrt(n/4) )
 
     # Scale to nice units and get the factor, unit prefix
-    x, f1, p1 = nice_array(particle_group[key1])
-    y, f2, p2 = nice_array(particle_group[key2])
-
+    x = particle_group[key1]
+    y = particle_group[key2]
+    
+    # Form nice arrays
+    x, f1, p1, xmin, xmax = plottable_array(x, nice=nice, lim=xlim)
+    y, f2, p2, ymin, ymax = plottable_array(y, nice=nice, lim=ylim)
+    
     w = particle_group['weight']
     
     u1 = particle_group.units(key1).unitSymbol
     u2 = particle_group.units(key2).unitSymbol
     ux = p1+u1
     uy = p2+u2
     
@@ -179,16 +265,14 @@
     ax_joint.hexbin(x, y, C=w, reduce_C_function=np.sum, gridsize=bins, cmap=CMAP0, vmin=1e-20)
     
     # Manual histogramming version
     #H, xedges, yedges = np.histogram2d(x, y, weights=w, bins=bins)
     #extent = [xedges[0], xedges[-1], yedges[0], yedges[-1]]
     #ax_joint.imshow(H.T, cmap=cmap, vmin=1e-16, origin='lower', extent=extent, aspect='auto')
     
-    
-    
     # Top histogram
     # Old method:
     #dx = x.ptp()/bins
     #ax_marg_x.hist(x, weights=w/dx/f1, bins=bins, color='gray')
     hist, bin_edges = np.histogram(x, bins=bins, weights=w)
     hist_x = bin_edges[:-1] + np.diff(bin_edges) / 2
     hist_width =  np.diff(bin_edges)
@@ -216,31 +300,40 @@
     # Turn off tick labels on marginals
     plt.setp(ax_marg_x.get_xticklabels(), visible=False)
     plt.setp(ax_marg_y.get_yticklabels(), visible=False)
     
     # Set labels on joint
     ax_joint.set_xlabel(labelx)
     ax_joint.set_ylabel(labely)
+    
+    # Actual plot limits, considering scaling
+    if xlim:
+        ax_joint.set_xlim( xmin/f1, xmax/f1)      
+        ax_marg_x.set_xlim(xmin/f1, xmax/f1)
+        
+    if ylim:
+        ax_joint.set_ylim( ymin/f2, ymax/f2)     
+        ax_marg_y.set_ylim(ymin/f2, ymax/f2)
 
-    return fig    
+    return fig   
     
     
 def density_and_slice_plot(particle_group, key1='t', key2='p', stat_keys=['norm_emit_x', 'norm_emit_y'], bins=100, n_slice=30, tex=True):
     """
     Density plot and projections
     
     Example:
     
         marginal_plot(P, 't', 'energy', bins=200)   
     
     """
 
     # Scale to nice units and get the factor, unit prefix
-    x, f1, p1 = nice_array(particle_group[key1])
-    y, f2, p2 = nice_array(particle_group[key2])
+    x, f1, p1, xmin, xmax = plottable_array(particle_group[key1])
+    y, f2, p2, ymin, ymax = plottable_array(particle_group[key2])
     w = particle_group['weight']
     
     u1 = particle_group.units(key1).unitSymbol
     u2 = particle_group.units(key2).unitSymbol
     ux = p1+u1
     uy = p2+u2
```

### Comparing `openpmd-beamphysics-0.7.8/pmd_beamphysics/readers.py` & `openpmd-beamphysics-0.7.9/pmd_beamphysics/readers.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.8/pmd_beamphysics/species.py` & `openpmd-beamphysics-0.7.9/pmd_beamphysics/species.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.8/pmd_beamphysics/statistics.py` & `openpmd-beamphysics-0.7.9/pmd_beamphysics/statistics.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.8/pmd_beamphysics/tools.py` & `openpmd-beamphysics-0.7.9/pmd_beamphysics/tools.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.8/pmd_beamphysics/units.py` & `openpmd-beamphysics-0.7.9/pmd_beamphysics/units.py`

 * *Files 4% similar despite different names*

```diff
@@ -171,34 +171,34 @@
         symbol = fr'\sqrt{{ {symbol} }}'
     
     unitSI = np.sqrt(u.unitSI)
     dim = tuple( x/2 for x in u.unitDimension)
     
     return pmd_unit(unitSymbol=symbol, unitSI=unitSI, unitDimension=dim)   
         
-        
+# length mass time current temperature mol luminous
 DIMENSION = { 
     '1'              : (0,0,0,0,0,0,0),
      # Base units
     'length'         : (1,0,0,0,0,0,0),
     'mass'           : (0,1,0,0,0,0,0),
     'time'           : (0,0,1,0,0,0,0),
     'current'        : (0,0,0,1,0,0,0),
     'temperture'     : (0,0,0,0,1,0,0),
     'mol'            : (0,0,0,0,0,1,0),
     'luminous'       : (0,0,0,0,0,0,1),
     #
-    'charge'         : (0,0,1,1,0,0,0),
-    'electric_field'  : (1,1,-3,-1,0,0,0),
+    'charge'             : (0,0,1,1,0,0,0),
+    'electric_field'     : (1,1,-3,-1,0,0,0),
     'electric_potential' : (1,2,-3,-1,0,0,0),
-    'magnetic_field' : (0,1,-2,-1,0,0,0),    
-    'velocity'       : (1,0,-1,0,0,0,0),
-    'energy'         : (2,1,-2,0,0,0,0),
-    'momentum'       : (1,1,-1,0,0,0,0)
-}
+    'magnetic_field'     : (0,1,-2,-1,0,0,0),    
+    'velocity'           : (1,0,-1,0,0,0,0),
+    'energy'             : (2,1,-2,0,0,0,0),
+    'momentum'           : (1,1,-1,0,0,0,0)
+}    
 # Inverse
 DIMENSION_NAME = {v: k for k, v in DIMENSION.items()}
 
 def dimension(name):
     if name in DIMENSION:
         return DIMENSION[name]
     else:
@@ -223,15 +223,15 @@
     'energy'         : 'J',
     'momentum'       : 'kg*m/s',
     'magnetic_field' : 'T'
 }
 # Inverse
 SI_name = {v: k for k, v in SI_symbol.items()}
 
-
+# length mass time current temperature mol luminous
 known_unit = { 
     '1'          : pmd_unit('', 1, '1'),
     'degree'     : pmd_unit('degree', np.pi/180, '1'),
     'rad'        : pmd_unit('rad', 1, '1'),
     'm'          : pmd_unit('m', 1, 'length'),
     'kg'         : pmd_unit('kg', 1, 'mass'),
     'g'          : pmd_unit('g', .001, 'mass'),
@@ -246,19 +246,22 @@
     'V'          : pmd_unit('V', 1, 'electric_potential'),
     'c_light'    : pmd_unit('vel/c', c_light, 'velocity'),
     'm/s'        : pmd_unit('m/s', 1, 'velocity'),
     'eV'         : pmd_unit('eV', e_charge, 'energy'),
     'J'          : pmd_unit('J', 1, 'energy'),
     'eV/c'       : pmd_unit('eV/c', e_charge/c_light, 'momentum'),
     'eV/m'       : pmd_unit('eV/m', e_charge, (1, 1, -2, 0, 0, 0, 0)),
-    'W/m^2'      : pmd_unit('W/m^2', 1, (1, 0, -3, 0, 0, 0, 0)),
-    'W'          : pmd_unit('W', 1, (1, 2, -3, 0, 0, 0, 0)),
+    'W'          : pmd_unit('W',       1, (2, 1, -3, 0, 0, 0, 0)),
+    'W/rad^2'    : pmd_unit('W/rad^2', 1, (2, 1, -3, 0, 0, 0, 0)),       
+    'W/m^2'      : pmd_unit('W/m^2',   1, (0, 1, -3, 0, 0, 0, 0)),
     'T'          : pmd_unit('T', 1, 'magnetic_field')
     } 
 
+
+
 def unit(symbol):
     """
     Returns a pmd_unit from a known symbol.
     
     * is allowed between two known symbols: 
     """
     if symbol in known_unit:
@@ -363,30 +366,70 @@
     Returns a scaled array, the scaling, and a unit prefix
     
     Example: 
         nice_array( np.array([2e-10, 3e-10]) )
     Returns:
         (array([200., 300.]), 1e-12, 'p')
     
-    """
-    #print('a', a.tolist())
-    
+    """    
     if np.isscalar(a):
         x = a
     elif len(a) == 1:
         x = a[0]
     else:
         a = np.array(a)
         x = max(a.ptp(), abs(np.mean(a))) # Account for tiny spread
         
     fac, prefix = nice_scale_prefix( x )
     
     return a/fac, fac,  prefix
 
 
+def plottable_array(x, nice=True, lim=None):
+    """
+    Similar to nice_array, but also considers limits for plotting
+    
+    Parameters
+    ----------
+    x: array-like
+    nice: bool, default = True
+        Scale array by some nice factor. 
+    xlim: tuple, default = None
+    
+    Returns
+    -------
+    scaled_array: np.ndarray
+    factor: float
+    prefix: str
+    xmin: float
+    xmax : float
+    
+    """
+    if lim is not None:
+        if lim[0] is None:
+            xmin = x.min()
+        else:
+            xmin = lim[0]
+        if lim[1] is None:
+            xmax = x.max()
+        else:
+            xmax = lim[1]            
+ 
+    else:
+        xmin = x.min()
+        xmax = x.max() 
+    
+    if nice:
+        _, factor, p1 = nice_array([xmin, xmax]) 
+    else:
+        factor, p1 = 1, ''
+        
+    return x/factor, factor, p1, xmin, xmax
+
+
 
 
 # -------------------------
 # Units for ParticleGroup
 
 PARTICLEGROUP_UNITS = {}
 for k in ['n_particle', 'status', 'id', 'n_alive', 'n_dead']:
```

### Comparing `openpmd-beamphysics-0.7.8/pmd_beamphysics/writers.py` & `openpmd-beamphysics-0.7.9/pmd_beamphysics/writers.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.8/setup.py` & `openpmd-beamphysics-0.7.9/setup.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.8/tests/test_particlegroup.py` & `openpmd-beamphysics-0.7.9/tests/test_particlegroup.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.8/versioneer.py` & `openpmd-beamphysics-0.7.9/versioneer.py`

 * *Files identical despite different names*

