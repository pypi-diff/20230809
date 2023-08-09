# Comparing `tmp/thunder-ase-0.4.3.tar.gz` & `tmp/thunder-ase-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thunder-ase-0.4.3.tar", last modified: Wed Aug  9 03:17:43 2023, max compression
+gzip compressed data, was "thunder-ase-0.4.4.tar", last modified: Wed Aug  9 05:19:03 2023, max compression
```

## Comparing `thunder-ase-0.4.3.tar` & `thunder-ase-0.4.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:17:43.497895 thunder-ase-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-08-09 03:17:43.497895 thunder-ase-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-08-09 03:17:31.000000 thunder-ase-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-08-09 03:17:31.000000 thunder-ase-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-09 03:17:43.497895 thunder-ase-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-09 03:17:31.000000 thunder-ase-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:17:43.497895 thunder-ase-0.4.3/thunder_ase/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-09 03:17:31.000000 thunder-ase-0.4.3/thunder_ase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32641 2023-08-09 03:17:31.000000 thunder-ase-0.4.3/thunder_ase/fireball.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:17:43.497895 thunder-ase-0.4.3/thunder_ase/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-08-09 03:17:31.000000 thunder-ase-0.4.3/thunder_ase/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11490 2023-08-09 03:17:31.000000 thunder-ase-0.4.3/thunder_ase/utils/basis_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-08-09 03:17:31.000000 thunder-ase-0.4.3/thunder_ase/utils/mwfn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-08-09 03:17:31.000000 thunder-ase-0.4.3/thunder_ase/utils/shell_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:17:43.497895 thunder-ase-0.4.3/thunder_ase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-08-09 03:17:43.000000 thunder-ase-0.4.3/thunder_ase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-08-09 03:17:43.000000 thunder-ase-0.4.3/thunder_ase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 03:17:43.000000 thunder-ase-0.4.3/thunder_ase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-09 03:17:43.000000 thunder-ase-0.4.3/thunder_ase.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-09 03:17:43.000000 thunder-ase-0.4.3/thunder_ase.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 05:19:03.413036 thunder-ase-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-08-09 05:19:03.413036 thunder-ase-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-08-09 05:18:47.000000 thunder-ase-0.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-08-09 05:18:47.000000 thunder-ase-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-09 05:19:03.413036 thunder-ase-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-09 05:18:47.000000 thunder-ase-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 05:19:03.409036 thunder-ase-0.4.4/thunder_ase/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-09 05:18:47.000000 thunder-ase-0.4.4/thunder_ase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31987 2023-08-09 05:18:47.000000 thunder-ase-0.4.4/thunder_ase/fireball.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 05:19:03.413036 thunder-ase-0.4.4/thunder_ase/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-08-09 05:18:47.000000 thunder-ase-0.4.4/thunder_ase/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11490 2023-08-09 05:18:47.000000 thunder-ase-0.4.4/thunder_ase/utils/basis_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-08-09 05:18:47.000000 thunder-ase-0.4.4/thunder_ase/utils/mwfn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-08-09 05:18:47.000000 thunder-ase-0.4.4/thunder_ase/utils/shell_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 05:19:03.413036 thunder-ase-0.4.4/thunder_ase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-08-09 05:19:03.000000 thunder-ase-0.4.4/thunder_ase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-08-09 05:19:03.000000 thunder-ase-0.4.4/thunder_ase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 05:19:03.000000 thunder-ase-0.4.4/thunder_ase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-09 05:19:03.000000 thunder-ase-0.4.4/thunder_ase.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-09 05:19:03.000000 thunder-ase-0.4.4/thunder_ase.egg-info/top_level.txt
```

### Comparing `thunder-ase-0.4.3/PKG-INFO` & `thunder-ase-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thunder-ase
-Version: 0.4.3
+Version: 0.4.4
 Summary: ASE calculator interface for FIREBALL code
 Author-email: PJ Ren <openrpj@gmail.com>
 Project-URL: Homepage, https://github.com/thunder-dft/thunder-ase
 Project-URL: Bug Tracker, https://github.com/thunder-dft/thunder-ase/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `thunder-ase-0.4.3/README.md` & `thunder-ase-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `thunder-ase-0.4.3/pyproject.toml` & `thunder-ase-0.4.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "thunder-ase"
-version = "0.4.3"
+version = "0.4.4"
 authors = [
   { name="PJ Ren", email="openrpj@gmail.com" },
 ]
 description = "ASE calculator interface for FIREBALL code"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `thunder-ase-0.4.3/thunder_ase/fireball.py` & `thunder-ase-0.4.4/thunder_ase/fireball.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,16 @@
     'ifix_neighbors': {'type': (int,), 'name': 'ifix_neighbors', 'default': 0},
     'ifix_charges': {'type': (int,), 'name': 'ifix_CHARGES', 'default': 1},
     'max_scf_iterations_set': {'type': (int,), 'name': 'max_scf_iterations_set', 'default': 50},
     'scf_tolerance_set': {'type': (int, float), 'name': 'scf_tolerance_set', 'default': 0.000001},
     'beta_set': {'type': (int, float), 'name': 'beta_set', 'default': 0.08},  # mix factor
     'ecut_set': {'type': (int, float), 'name': 'Ecut_set', 'default': 200.0},  # control mesh grid number
     'ipi': {'type': (int,), 'name': 'ipi', 'default': 0},  # open I-PI socket
+    'inet': {'type': (int,), 'name': 'inet', 'default': 0},  # socket protocol, 0: unixsocket, 1: port
+    'host': {'type': (str,), 'name': 'host', 'default': 'thunder-ase'},
 }
 
 output_params = {
     'iwriteout_me_sandh': {'type': (int,), 'name': 'iwriteout_ME_SandH', 'default': 0},
     'iwriteout_density': {'type': (int,), 'name': 'iwriteout_density', 'default': 0},
     'iwriteout_cdcoeffs': {'type': (int,), 'name': 'iwriteout_cdcoeffs', 'default': 0},
     'iwriteout_charges': {'type': (int,), 'name': 'iwriteout_charges', 'default': 0},
@@ -120,29 +122,25 @@
     'iwriteout_forces': {'type': (int,), 'name': 'iwriteout_forces', 'default': 0},
     'iwriteout_neighbors': {'type': (int,), 'name': 'iwriteout_neighbors', 'default': 0},
     'iwriteout_dos': {'type': (int,), 'name': 'iwriteout_dos', 'default': 0},
     'iwriteout_abs': {'type': (int,), 'name': 'iwriteout_abs', 'default': 0},
     'iwriteout_ewf': {'type': (int,), 'name': 'iwriteout_ewf', 'default': 0},
 }
 
-xsfoptions_params = {
-    'rho_surface_min': {'type': (int, float), 'name': 'rho_surface_min', 'default': 0.0005},
-    'rho_surface_max': {'type': (int, float), 'name': 'rho_surface_max', 'default': 0.1},
-}
 
 calc_params = {
     'kpt_size': {'type': (list, np.array), 'name': 'kpt_size', 'default': None},
     'kpt_offset': {'type': (list, np.array), 'name': 'kpt_offset', 'default': None},
     'kpt_interval': {'type': (list, np.array, float, int), 'name': 'kpt_interval', 'default': None},
     'kpt_path': {'type': (BandPath, str, list, np.array), 'name': 'kpt_path', 'default': None},
     'nkpt': {'type': (int,), 'name': 'nkpt', 'default': None},  # n kpoints on path. Used if kpt_path is string.
     'kpt_reduced': {'type': (bool,), 'name': 'kpt_reduced', 'default': False},
 }
 
-fireball_params = options_params | output_params | xsfoptions_params | calc_params
+fireball_params = options_params | output_params | calc_params
 
 
 def get_params_from_string(s):
     k, v = s.split('=')
     k = k.strip().lower()
     v = v.strip()
     if k not in fireball_params:
@@ -166,15 +164,14 @@
         if atoms is not None:
             self._atoms = atoms.copy()
         else:
             self._atoms = None
         self.sname = '001'
         self.output_params = {}
         self.options_params = {}
-        self.xsfoptions_params = {}
         self.Fdata_path = None
 
         self.kpt_size = fireball_params['kpt_size']['default']
         self.kpt_interval = fireball_params['kpt_interval']['default']
         self.kpt_offset = fireball_params['kpt_offset']['default']
         self.kpt_path = fireball_params['kpt_path']['default']
         self.nkpt = fireball_params['nkpt']['default']
@@ -262,16 +259,14 @@
                 print("The type of {} should be {}, but type {} is provided!".format(k, ' or '.join(
                     [i.__name__ for i in fireball_params[k]['type']]), type(v).__name__))
                 raise TypeError
             if k in output_params:
                 self.output_params[k] = v
             elif k in options_params:
                 self.options_params[k] = v
-            elif k in xsfoptions_params:
-                self.xsfoptions_params[k] = v
             elif k == 'kpt_size':
                 self.kpt_size = v
             elif k == 'kpt_offset':
                 self.kpt_offset = v
             elif k == 'kpt_interval':
                 self.kpt_interval = v
             elif k == 'kpt_path':
@@ -293,18 +288,14 @@
             write_params(self.output_params, f)
             f.write("&END\n")
 
             f.write("&OPTIONS\n")
             write_params(self.options_params, f)
             f.write("&END\n")
 
-            f.write("&XSFOPTIONS\n")
-            write_params(self.xsfoptions_params, f)
-            f.write("&END\n")
-
     def write_atoms(self, atoms=None, pbc=None):
         """
         TODO: for non-PBC system, set cell to [0.000] * 9
         :param atoms:
         :param pbc:
         :return:
         """
@@ -353,51 +344,42 @@
             lines = f.readlines()
 
         natoms_list = int(lines[0].strip())
         sname_list = []
         for iline in lines[1:natoms_list + 1]:
             sname_list.append(iline.strip().strip('.inp'))
 
-        loption, loutput, lxsfoptions = False, False, False
+        loption, loutput = False, False
         for line in lines[natoms_list + 1:]:
             content = line.strip()
             if '!' in content:
                 content = content.split('!')[0]
             if len(content) == 0:
                 continue
 
             if '&OPTIONS' in content:
                 loption = True
                 continue
             if '&OUTPUT' in content:
                 loutput = True
                 continue
-            if "&XSFOPTIONS" in content:
-                lxsfoptions = True
-                continue
 
             if loption:
                 if '&END' in content:
                     loption = False
                     continue
                 k, v = get_params_from_string(content)
                 self.options_params[k] = v
 
             elif loutput:
                 if '&END' in content:
                     loutput = False
                     continue
                 k, v = get_params_from_string(content)
                 self.output_params[k] = v
-            elif lxsfoptions:
-                if '&END' in content:
-                    lxsfoptions = False
-                    continue
-                k, v = get_params_from_string(content)
-                self.xsfoptions_params[k] = v
 
         if read_atoms:
             return sname_list
 
     def read_kpts(self, input_file=None):
         with open(input_file, 'r') as f:
             lines = f.readlines()
```

### Comparing `thunder-ase-0.4.3/thunder_ase/utils/basis_set.py` & `thunder-ase-0.4.4/thunder_ase/utils/basis_set.py`

 * *Files identical despite different names*

### Comparing `thunder-ase-0.4.3/thunder_ase/utils/mwfn.py` & `thunder-ase-0.4.4/thunder_ase/utils/mwfn.py`

 * *Files identical despite different names*

### Comparing `thunder-ase-0.4.3/thunder_ase/utils/shell_dict.py` & `thunder-ase-0.4.4/thunder_ase/utils/shell_dict.py`

 * *Files identical despite different names*

### Comparing `thunder-ase-0.4.3/thunder_ase.egg-info/PKG-INFO` & `thunder-ase-0.4.4/thunder_ase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thunder-ase
-Version: 0.4.3
+Version: 0.4.4
 Summary: ASE calculator interface for FIREBALL code
 Author-email: PJ Ren <openrpj@gmail.com>
 Project-URL: Homepage, https://github.com/thunder-dft/thunder-ase
 Project-URL: Bug Tracker, https://github.com/thunder-dft/thunder-ase/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

