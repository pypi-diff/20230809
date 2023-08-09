# Comparing `tmp/thunder-ase-0.4.2.tar.gz` & `tmp/thunder-ase-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thunder-ase-0.4.2.tar", last modified: Tue Aug  8 01:37:41 2023, max compression
+gzip compressed data, was "thunder-ase-0.4.3.tar", last modified: Wed Aug  9 03:17:43 2023, max compression
```

## Comparing `thunder-ase-0.4.2.tar` & `thunder-ase-0.4.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:37:41.968806 thunder-ase-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-08-08 01:37:41.968806 thunder-ase-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-08-08 01:37:26.000000 thunder-ase-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-08-08 01:37:26.000000 thunder-ase-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:37:41.968806 thunder-ase-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 01:37:26.000000 thunder-ase-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:37:41.968806 thunder-ase-0.4.2/thunder_ase/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 01:37:26.000000 thunder-ase-0.4.2/thunder_ase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32610 2023-08-08 01:37:26.000000 thunder-ase-0.4.2/thunder_ase/fireball.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:37:41.968806 thunder-ase-0.4.2/thunder_ase/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-08-08 01:37:26.000000 thunder-ase-0.4.2/thunder_ase/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11490 2023-08-08 01:37:26.000000 thunder-ase-0.4.2/thunder_ase/utils/basis_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-08-08 01:37:26.000000 thunder-ase-0.4.2/thunder_ase/utils/mwfn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-08-08 01:37:26.000000 thunder-ase-0.4.2/thunder_ase/utils/shell_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 01:37:41.968806 thunder-ase-0.4.2/thunder_ase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-08-08 01:37:41.000000 thunder-ase-0.4.2/thunder_ase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-08-08 01:37:41.000000 thunder-ase-0.4.2/thunder_ase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 01:37:41.000000 thunder-ase-0.4.2/thunder_ase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-08 01:37:41.000000 thunder-ase-0.4.2/thunder_ase.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-08 01:37:41.000000 thunder-ase-0.4.2/thunder_ase.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:17:43.497895 thunder-ase-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-08-09 03:17:43.497895 thunder-ase-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-08-09 03:17:31.000000 thunder-ase-0.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-08-09 03:17:31.000000 thunder-ase-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-09 03:17:43.497895 thunder-ase-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-09 03:17:31.000000 thunder-ase-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:17:43.497895 thunder-ase-0.4.3/thunder_ase/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-09 03:17:31.000000 thunder-ase-0.4.3/thunder_ase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32641 2023-08-09 03:17:31.000000 thunder-ase-0.4.3/thunder_ase/fireball.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:17:43.497895 thunder-ase-0.4.3/thunder_ase/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-08-09 03:17:31.000000 thunder-ase-0.4.3/thunder_ase/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11490 2023-08-09 03:17:31.000000 thunder-ase-0.4.3/thunder_ase/utils/basis_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-08-09 03:17:31.000000 thunder-ase-0.4.3/thunder_ase/utils/mwfn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-08-09 03:17:31.000000 thunder-ase-0.4.3/thunder_ase/utils/shell_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 03:17:43.497895 thunder-ase-0.4.3/thunder_ase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-08-09 03:17:43.000000 thunder-ase-0.4.3/thunder_ase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-08-09 03:17:43.000000 thunder-ase-0.4.3/thunder_ase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 03:17:43.000000 thunder-ase-0.4.3/thunder_ase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-09 03:17:43.000000 thunder-ase-0.4.3/thunder_ase.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-09 03:17:43.000000 thunder-ase-0.4.3/thunder_ase.egg-info/top_level.txt
```

### Comparing `thunder-ase-0.4.2/PKG-INFO` & `thunder-ase-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thunder-ase
-Version: 0.4.2
+Version: 0.4.3
 Summary: ASE calculator interface for FIREBALL code
 Author-email: PJ Ren <openrpj@gmail.com>
 Project-URL: Homepage, https://github.com/thunder-dft/thunder-ase
 Project-URL: Bug Tracker, https://github.com/thunder-dft/thunder-ase/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `thunder-ase-0.4.2/README.md` & `thunder-ase-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `thunder-ase-0.4.2/pyproject.toml` & `thunder-ase-0.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "thunder-ase"
-version = "0.4.2"
+version = "0.4.3"
 authors = [
   { name="PJ Ren", email="openrpj@gmail.com" },
 ]
 description = "ASE calculator interface for FIREBALL code"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `thunder-ase-0.4.2/thunder_ase/fireball.py` & `thunder-ase-0.4.3/thunder_ase/fireball.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,14 +167,15 @@
             self._atoms = atoms.copy()
         else:
             self._atoms = None
         self.sname = '001'
         self.output_params = {}
         self.options_params = {}
         self.xsfoptions_params = {}
+        self.Fdata_path = None
 
         self.kpt_size = fireball_params['kpt_size']['default']
         self.kpt_interval = fireball_params['kpt_interval']['default']
         self.kpt_offset = fireball_params['kpt_offset']['default']
         self.kpt_path = fireball_params['kpt_path']['default']
         self.nkpt = fireball_params['nkpt']['default']
         self.kpt_reduced = fireball_params['kpt_reduced']['default']
@@ -333,18 +334,18 @@
         :return:
         """
         with open(self.sname + '.KPOINTS', 'w') as f:
             f.write("{}\n".format(len(self.get_kpoints(reduced=reduced, **kwargs))))
             for k in self.get_kpoints(reduced=reduced, **kwargs):
                 f.write("{:8.6f} {:8.6f} {:8.6f} {:8.6f}\n".format(*k))
 
-    def write_input(self, atoms=None, Fdata_path=None):
+    def write_input(self, atoms=None, properties=None, system_changes=None):
         if atoms is not None:
             self.atoms = atoms.copy()
-        self.write_Fdata_inp(atoms=self.atoms, Fdata_path=Fdata_path)
+        self.write_Fdata_inp(atoms=self.atoms, Fdata_path=self.Fdata_path)
         self.write_options()
         self.write_atoms(pbc=self.atoms.pbc)
         if np.any(self.atoms.pbc):
             self.write_kpts(reduced=self.kpt_reduced)
 
     def read_options(self, input_file='structures.inp', read_atoms=False):
         # read structures.inp, get names for atoms and kpoints
@@ -461,15 +462,15 @@
         execute fireball. After execution, the energy, forces. etc. are read
         from the fireball output files.
         """
 
         if atoms is not None:
             self.atoms = atoms.copy()
 
-        self.write_input(Fdata_path=self.Fdata_path)
+        self.write_input()
 
         errorcode = self._run(command=self.command,
                               directory=self.directory)
 
         if errorcode:
             raise CalculationFailed(
                 '{} in {} returned an error: {:d}'.format(
```

### Comparing `thunder-ase-0.4.2/thunder_ase/utils/basis_set.py` & `thunder-ase-0.4.3/thunder_ase/utils/basis_set.py`

 * *Files identical despite different names*

### Comparing `thunder-ase-0.4.2/thunder_ase/utils/mwfn.py` & `thunder-ase-0.4.3/thunder_ase/utils/mwfn.py`

 * *Files identical despite different names*

### Comparing `thunder-ase-0.4.2/thunder_ase/utils/shell_dict.py` & `thunder-ase-0.4.3/thunder_ase/utils/shell_dict.py`

 * *Files identical despite different names*

### Comparing `thunder-ase-0.4.2/thunder_ase.egg-info/PKG-INFO` & `thunder-ase-0.4.3/thunder_ase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thunder-ase
-Version: 0.4.2
+Version: 0.4.3
 Summary: ASE calculator interface for FIREBALL code
 Author-email: PJ Ren <openrpj@gmail.com>
 Project-URL: Homepage, https://github.com/thunder-dft/thunder-ase
 Project-URL: Bug Tracker, https://github.com/thunder-dft/thunder-ase/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

