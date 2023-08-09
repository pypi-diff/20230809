# Comparing `tmp/isqmap-0.2.tar.gz` & `tmp/isqmap-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/isqmap-0.2.tar", last modified: Thu Apr 13 10:34:20 2023, max compression
+gzip compressed data, was "dist/isqmap-0.3.tar", last modified: Wed Aug  9 03:42:02 2023, max compression
```

## Comparing `isqmap-0.2.tar` & `isqmap-0.3.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-04-13 10:34:20.000000 isqmap-0.2/
--rw-r--r--   0 huazhelou   (501) staff       (20)      361 2023-04-13 10:34:20.000000 isqmap-0.2/PKG-INFO
--rw-r--r--   0 huazhelou   (501) staff       (20)       88 2023-04-13 09:21:20.000000 isqmap-0.2/README.md
-drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-04-13 10:34:20.000000 isqmap-0.2/isqmap/
--rw-r--r--   0 huazhelou   (501) staff       (20)       83 2023-04-13 09:17:21.000000 isqmap-0.2/isqmap/__init__.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     3127 2023-04-13 08:41:16.000000 isqmap-0.2/isqmap/ag.py
--rw-rw-r--   0 huazhelou   (501) staff       (20)    20082 2023-04-13 10:24:17.000000 isqmap-0.2/isqmap/cir_dg.py
--rw-rw-r--   0 huazhelou   (501) staff       (20)    22082 2023-04-13 10:26:03.000000 isqmap-0.2/isqmap/cir_dg_swap_depth_opt.py
--rw-r--r--   0 huazhelou   (501) staff       (20)    18182 2023-04-13 08:41:16.000000 isqmap-0.2/isqmap/front_circuit.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     9907 2023-04-13 09:15:52.000000 isqmap-0.2/isqmap/genetic_swap_depth_opt.py
-drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-04-13 10:34:20.000000 isqmap-0.2/isqmap/init_mapping/
-drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-04-13 10:34:20.000000 isqmap-0.2/isqmap/init_mapping/FiDLS/
--rw-r--r--   0 huazhelou   (501) staff       (20)     3588 2023-04-13 08:41:16.000000 isqmap-0.2/isqmap/init_mapping/FiDLS/FiDLS_inimap.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     6792 2023-04-13 08:41:16.000000 isqmap-0.2/isqmap/init_mapping/FiDLS/FiDLS_run.py
--rw-r--r--   0 huazhelou   (501) staff       (20)        0 2023-04-13 09:32:01.000000 isqmap-0.2/isqmap/init_mapping/FiDLS/__init__.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     4608 2023-04-13 08:41:16.000000 isqmap-0.2/isqmap/init_mapping/FiDLS/ag.py
--rw-r--r--   0 huazhelou   (501) staff       (20)    12890 2023-04-13 08:41:16.000000 isqmap-0.2/isqmap/init_mapping/FiDLS/fidls_d.py
--rw-r--r--   0 huazhelou   (501) staff       (20)    12595 2023-04-13 08:41:16.000000 isqmap-0.2/isqmap/init_mapping/FiDLS/fidls_g.py
--rw-r--r--   0 huazhelou   (501) staff       (20)    13641 2023-04-13 08:41:16.000000 isqmap-0.2/isqmap/init_mapping/FiDLS/inimap.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     1742 2023-04-13 08:41:16.000000 isqmap-0.2/isqmap/init_mapping/FiDLS/maps.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     2154 2023-04-13 08:41:16.000000 isqmap-0.2/isqmap/init_mapping/FiDLS/readme.txt
--rw-r--r--   0 huazhelou   (501) staff       (20)     4949 2023-04-13 08:41:16.000000 isqmap-0.2/isqmap/init_mapping/FiDLS/sqatest0.py
--rw-r--r--   0 huazhelou   (501) staff       (20)    18164 2023-04-13 08:41:16.000000 isqmap-0.2/isqmap/init_mapping/FiDLS/utils.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     7502 2023-04-13 08:41:16.000000 isqmap-0.2/isqmap/init_mapping/FiDLS/vfs.py
--rw-r--r--   0 huazhelou   (501) staff       (20)    24314 2023-04-13 08:41:16.000000 isqmap-0.2/isqmap/init_mapping/FiDLS/vfstest.py
--rw-r--r--   0 huazhelou   (501) staff       (20)        0 2023-04-13 09:26:43.000000 isqmap-0.2/isqmap/init_mapping/__init__.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     2212 2023-04-13 08:41:16.000000 isqmap-0.2/isqmap/init_mapping/get_init_map.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     5991 2023-04-13 09:17:07.000000 isqmap-0.2/isqmap/init_mapping/sa_mapping.py
--rw-r--r--   0 huazhelou   (501) staff       (20)     1289 2023-04-13 08:41:16.000000 isqmap-0.2/isqmap/init_mapping/subgraph_isomorphism_mapping.py
--rw-r--r--   0 huazhelou   (501) staff       (20)    12348 2023-04-13 10:29:02.000000 isqmap-0.2/isqmap/mapping.py
--rw-r--r--   0 huazhelou   (501) staff       (20)    36930 2023-04-13 09:16:43.000000 isqmap-0.2/isqmap/monte_carlo_tree.py
-drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-04-13 10:34:20.000000 isqmap-0.2/isqmap.egg-info/
--rw-r--r--   0 huazhelou   (501) staff       (20)      361 2023-04-13 10:34:20.000000 isqmap-0.2/isqmap.egg-info/PKG-INFO
--rw-r--r--   0 huazhelou   (501) staff       (20)     1018 2023-04-13 10:34:20.000000 isqmap-0.2/isqmap.egg-info/SOURCES.txt
--rw-r--r--   0 huazhelou   (501) staff       (20)        1 2023-04-13 10:34:20.000000 isqmap-0.2/isqmap.egg-info/dependency_links.txt
--rw-r--r--   0 huazhelou   (501) staff       (20)        1 2023-04-13 10:34:20.000000 isqmap-0.2/isqmap.egg-info/not-zip-safe
--rw-r--r--   0 huazhelou   (501) staff       (20)       33 2023-04-13 10:34:20.000000 isqmap-0.2/isqmap.egg-info/requires.txt
--rw-r--r--   0 huazhelou   (501) staff       (20)        7 2023-04-13 10:34:20.000000 isqmap-0.2/isqmap.egg-info/top_level.txt
--rw-r--r--   0 huazhelou   (501) staff       (20)      107 2023-04-13 10:34:20.000000 isqmap-0.2/setup.cfg
--rw-r--r--   0 huazhelou   (501) staff       (20)      688 2023-04-13 10:34:15.000000 isqmap-0.2/setup.py
+drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-08-09 03:42:02.854288 isqmap-0.3/
+-rw-r--r--   0 huazhelou   (501) staff       (20)     1093 2023-04-13 09:36:30.000000 isqmap-0.3/LICENSE
+-rw-r--r--   0 huazhelou   (501) staff       (20)      319 2023-08-09 03:42:02.854412 isqmap-0.3/PKG-INFO
+-rw-r--r--   0 huazhelou   (501) staff       (20)       88 2023-04-13 09:21:20.000000 isqmap-0.3/README.md
+drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-08-09 03:42:02.844081 isqmap-0.3/isqmap/
+-rw-r--r--   0 huazhelou   (501) staff       (20)       83 2023-04-13 09:17:21.000000 isqmap-0.3/isqmap/__init__.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     3127 2023-04-13 08:41:16.000000 isqmap-0.3/isqmap/ag.py
+-rw-rw-r--   0 huazhelou   (501) staff       (20)    20082 2023-04-13 10:24:17.000000 isqmap-0.3/isqmap/cir_dg.py
+-rw-rw-r--   0 huazhelou   (501) staff       (20)    22082 2023-04-13 10:26:03.000000 isqmap-0.3/isqmap/cir_dg_swap_depth_opt.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)    18182 2023-04-13 08:41:16.000000 isqmap-0.3/isqmap/front_circuit.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     9907 2023-04-13 09:15:52.000000 isqmap-0.3/isqmap/genetic_swap_depth_opt.py
+drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-08-09 03:42:02.849765 isqmap-0.3/isqmap/init_mapping/
+drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-08-09 03:42:02.853981 isqmap-0.3/isqmap/init_mapping/FiDLS/
+-rw-r--r--   0 huazhelou   (501) staff       (20)     3588 2023-04-13 08:41:16.000000 isqmap-0.3/isqmap/init_mapping/FiDLS/FiDLS_inimap.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     6792 2023-04-13 08:41:16.000000 isqmap-0.3/isqmap/init_mapping/FiDLS/FiDLS_run.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)        0 2023-04-13 09:32:01.000000 isqmap-0.3/isqmap/init_mapping/FiDLS/__init__.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     4608 2023-04-13 08:41:16.000000 isqmap-0.3/isqmap/init_mapping/FiDLS/ag.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)    12890 2023-04-13 08:41:16.000000 isqmap-0.3/isqmap/init_mapping/FiDLS/fidls_d.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)    12595 2023-04-13 08:41:16.000000 isqmap-0.3/isqmap/init_mapping/FiDLS/fidls_g.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)    13641 2023-04-13 08:41:16.000000 isqmap-0.3/isqmap/init_mapping/FiDLS/inimap.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     1742 2023-04-13 08:41:16.000000 isqmap-0.3/isqmap/init_mapping/FiDLS/maps.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     2154 2023-04-13 08:41:16.000000 isqmap-0.3/isqmap/init_mapping/FiDLS/readme.txt
+-rw-r--r--   0 huazhelou   (501) staff       (20)     4949 2023-04-13 08:41:16.000000 isqmap-0.3/isqmap/init_mapping/FiDLS/sqatest0.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)    18164 2023-04-13 08:41:16.000000 isqmap-0.3/isqmap/init_mapping/FiDLS/utils.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     7502 2023-04-13 08:41:16.000000 isqmap-0.3/isqmap/init_mapping/FiDLS/vfs.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)    24314 2023-04-13 08:41:16.000000 isqmap-0.3/isqmap/init_mapping/FiDLS/vfstest.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)        0 2023-04-13 09:26:43.000000 isqmap-0.3/isqmap/init_mapping/__init__.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     2212 2023-04-13 08:41:16.000000 isqmap-0.3/isqmap/init_mapping/get_init_map.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     5991 2023-04-13 09:17:07.000000 isqmap-0.3/isqmap/init_mapping/sa_mapping.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)     1289 2023-04-13 08:41:16.000000 isqmap-0.3/isqmap/init_mapping/subgraph_isomorphism_mapping.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)    12342 2023-08-09 03:39:02.000000 isqmap-0.3/isqmap/mapping.py
+-rw-r--r--   0 huazhelou   (501) staff       (20)    36930 2023-04-13 09:16:43.000000 isqmap-0.3/isqmap/monte_carlo_tree.py
+drwxr-xr-x   0 huazhelou   (501) staff       (20)        0 2023-08-09 03:42:02.846032 isqmap-0.3/isqmap.egg-info/
+-rw-r--r--   0 huazhelou   (501) staff       (20)      319 2023-08-09 03:42:02.000000 isqmap-0.3/isqmap.egg-info/PKG-INFO
+-rw-r--r--   0 huazhelou   (501) staff       (20)     1026 2023-08-09 03:42:02.000000 isqmap-0.3/isqmap.egg-info/SOURCES.txt
+-rw-r--r--   0 huazhelou   (501) staff       (20)        1 2023-08-09 03:42:02.000000 isqmap-0.3/isqmap.egg-info/dependency_links.txt
+-rw-r--r--   0 huazhelou   (501) staff       (20)        1 2023-08-09 03:42:02.000000 isqmap-0.3/isqmap.egg-info/not-zip-safe
+-rw-r--r--   0 huazhelou   (501) staff       (20)       33 2023-08-09 03:42:02.000000 isqmap-0.3/isqmap.egg-info/requires.txt
+-rw-r--r--   0 huazhelou   (501) staff       (20)        7 2023-08-09 03:42:02.000000 isqmap-0.3/isqmap.egg-info/top_level.txt
+-rw-r--r--   0 huazhelou   (501) staff       (20)      107 2023-08-09 03:42:02.854922 isqmap-0.3/setup.cfg
+-rw-r--r--   0 huazhelou   (501) staff       (20)      688 2023-08-09 03:41:37.000000 isqmap-0.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `isqmap-0.2/isqmap/ag.py` & `isqmap-0.3/isqmap/ag.py`

 * *Files identical despite different names*

### Comparing `isqmap-0.2/isqmap/cir_dg.py` & `isqmap-0.3/isqmap/cir_dg.py`

 * *Files identical despite different names*

### Comparing `isqmap-0.2/isqmap/cir_dg_swap_depth_opt.py` & `isqmap-0.3/isqmap/cir_dg_swap_depth_opt.py`

 * *Files identical despite different names*

### Comparing `isqmap-0.2/isqmap/front_circuit.py` & `isqmap-0.3/isqmap/front_circuit.py`

 * *Files identical despite different names*

### Comparing `isqmap-0.2/isqmap/genetic_swap_depth_opt.py` & `isqmap-0.3/isqmap/genetic_swap_depth_opt.py`

 * *Files identical despite different names*

### Comparing `isqmap-0.2/isqmap/init_mapping/FiDLS/FiDLS_inimap.py` & `isqmap-0.3/isqmap/init_mapping/FiDLS/FiDLS_inimap.py`

 * *Files identical despite different names*

### Comparing `isqmap-0.2/isqmap/init_mapping/FiDLS/FiDLS_run.py` & `isqmap-0.3/isqmap/init_mapping/FiDLS/FiDLS_run.py`

 * *Files identical despite different names*

### Comparing `isqmap-0.2/isqmap/init_mapping/FiDLS/ag.py` & `isqmap-0.3/isqmap/init_mapping/FiDLS/ag.py`

 * *Files identical despite different names*

### Comparing `isqmap-0.2/isqmap/init_mapping/FiDLS/fidls_d.py` & `isqmap-0.3/isqmap/init_mapping/FiDLS/fidls_d.py`

 * *Files identical despite different names*

### Comparing `isqmap-0.2/isqmap/init_mapping/FiDLS/fidls_g.py` & `isqmap-0.3/isqmap/init_mapping/FiDLS/fidls_g.py`

 * *Files identical despite different names*

### Comparing `isqmap-0.2/isqmap/init_mapping/FiDLS/inimap.py` & `isqmap-0.3/isqmap/init_mapping/FiDLS/inimap.py`

 * *Files identical despite different names*

### Comparing `isqmap-0.2/isqmap/init_mapping/FiDLS/maps.py` & `isqmap-0.3/isqmap/init_mapping/FiDLS/maps.py`

 * *Files identical despite different names*

### Comparing `isqmap-0.2/isqmap/init_mapping/FiDLS/readme.txt` & `isqmap-0.3/isqmap/init_mapping/FiDLS/readme.txt`

 * *Files identical despite different names*

### Comparing `isqmap-0.2/isqmap/init_mapping/FiDLS/sqatest0.py` & `isqmap-0.3/isqmap/init_mapping/FiDLS/sqatest0.py`

 * *Files identical despite different names*

### Comparing `isqmap-0.2/isqmap/init_mapping/FiDLS/utils.py` & `isqmap-0.3/isqmap/init_mapping/FiDLS/utils.py`

 * *Files identical despite different names*

### Comparing `isqmap-0.2/isqmap/init_mapping/FiDLS/vfs.py` & `isqmap-0.3/isqmap/init_mapping/FiDLS/vfs.py`

 * *Files identical despite different names*

### Comparing `isqmap-0.2/isqmap/init_mapping/FiDLS/vfstest.py` & `isqmap-0.3/isqmap/init_mapping/FiDLS/vfstest.py`

 * *Files identical despite different names*

### Comparing `isqmap-0.2/isqmap/init_mapping/get_init_map.py` & `isqmap-0.3/isqmap/init_mapping/get_init_map.py`

 * *Files identical despite different names*

### Comparing `isqmap-0.2/isqmap/init_mapping/sa_mapping.py` & `isqmap-0.3/isqmap/init_mapping/sa_mapping.py`

 * *Files identical despite different names*

### Comparing `isqmap-0.2/isqmap/init_mapping/subgraph_isomorphism_mapping.py` & `isqmap-0.3/isqmap/init_mapping/subgraph_isomorphism_mapping.py`

 * *Files identical despite different names*

### Comparing `isqmap-0.2/isqmap/mapping.py` & `isqmap-0.3/isqmap/mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,19 +74,19 @@
     return layout_dict_r
 
 def import_qpu_file(file_path, disable_qubits=[]):
     qpu_config_dice = {}
     import json
     with open(file_path, 'r') as f:
         config = json.load(f)
-    couplers = config['twoQubitGate']['czGate']['gate error']['qubit_used']
+    coupler_map = config['overview']['coupler_map']
     adjacency_list = []
-    for c in couplers:
-        q1 = int(c[1:3])
-        q2 = int(c[3:])
+    for Q1, Q2 in coupler_map.values():
+        q1 = int(Q1[1:])
+        q2 = int(Q2[1:])
         if q1 in disable_qubits or q2 in disable_qubits: continue
         adjacency_list.append([q1, q2])
     qpu_config_dice['adjacency_list'] = adjacency_list
     return qpu_config_dice
 
 def transpile(qasm_str, qpu_file, initial_layout=None, objective='size',
               seed=None, use_post_opt=False,):
```

### Comparing `isqmap-0.2/isqmap/monte_carlo_tree.py` & `isqmap-0.3/isqmap/monte_carlo_tree.py`

 * *Files identical despite different names*

### Comparing `isqmap-0.2/isqmap.egg-info/SOURCES.txt` & `isqmap-0.3/isqmap.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.cfg
 setup.py
 isqmap/__init__.py
 isqmap/ag.py
 isqmap/cir_dg.py
 isqmap/cir_dg_swap_depth_opt.py
```

### Comparing `isqmap-0.2/setup.py` & `isqmap-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name = "isqmap",
-    version = "0.2",
+    version = "0.3",
     keyword = {"mapping", "ustc"},
     description = "a qubit mapping package",
     platforms='python 3.7+',
     long_description=long_description,
 	long_description_content_type="text/markdown",
     author = "arclightquantum",
     author_email = "louhz@arclightquantum.com",
```

