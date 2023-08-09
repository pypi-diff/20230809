# Comparing `tmp/inviz-0.2.8a2.tar.gz` & `tmp/inviz-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inviz-0.2.8a2.tar", last modified: Sat Aug  5 07:28:54 2023, max compression
+gzip compressed data, was "inviz-0.3.0.tar", last modified: Wed Aug  9 00:53:53 2023, max compression
```

## Comparing `inviz-0.2.8a2.tar` & `inviz-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-08-05 07:28:54.922172 inviz-0.2.8a2/
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1066 2023-03-27 21:46:04.000000 inviz-0.2.8a2/LICENSE
--rw-r--r--   0 jswen     (1000) jswen     (1000)       42 2023-03-27 21:46:04.000000 inviz-0.2.8a2/MANIFEST.in
--rw-r--r--   0 jswen     (1000) jswen     (1000)     2165 2023-08-05 07:28:54.922172 inviz-0.2.8a2/PKG-INFO
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1642 2023-07-13 22:19:19.000000 inviz-0.2.8a2/README.md
--rw-r--r--   0 jswen     (1000) jswen     (1000)       38 2023-08-05 07:28:54.922172 inviz-0.2.8a2/setup.cfg
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1150 2023-08-05 07:28:36.000000 inviz-0.2.8a2/setup.py
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-08-05 07:28:54.912172 inviz-0.2.8a2/src/
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-08-05 07:28:54.922172 inviz-0.2.8a2/src/cosmo/
--rw-r--r--   0 jswen     (1000) jswen     (1000)       22 2023-08-05 07:28:45.000000 inviz-0.2.8a2/src/cosmo/__init__.py
--rw-r--r--   0 jswen     (1000) jswen     (1000)     2605 2023-08-04 04:36:54.000000 inviz-0.2.8a2/src/cosmo/cosmo.py
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-08-05 07:28:54.922172 inviz-0.2.8a2/src/inviz.egg-info/
--rw-r--r--   0 jswen     (1000) jswen     (1000)     2165 2023-08-05 07:28:54.000000 inviz-0.2.8a2/src/inviz.egg-info/PKG-INFO
--rw-r--r--   0 jswen     (1000) jswen     (1000)      243 2023-08-05 07:28:54.000000 inviz-0.2.8a2/src/inviz.egg-info/SOURCES.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)        1 2023-08-05 07:28:54.000000 inviz-0.2.8a2/src/inviz.egg-info/dependency_links.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)      119 2023-08-05 07:28:54.000000 inviz-0.2.8a2/src/inviz.egg-info/requires.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)        6 2023-08-05 07:28:54.000000 inviz-0.2.8a2/src/inviz.egg-info/top_level.txt
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-08-09 00:53:53.641550 inviz-0.3.0/
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1066 2023-03-27 21:46:04.000000 inviz-0.3.0/LICENSE
+-rw-r--r--   0 jswen     (1000) jswen     (1000)       42 2023-03-27 21:46:04.000000 inviz-0.3.0/MANIFEST.in
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     2172 2023-08-09 00:53:53.641550 inviz-0.3.0/PKG-INFO
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1642 2023-07-13 22:19:19.000000 inviz-0.3.0/README.md
+-rw-r--r--   0 jswen     (1000) jswen     (1000)       38 2023-08-09 00:53:53.641550 inviz-0.3.0/setup.cfg
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1281 2023-08-09 00:49:10.000000 inviz-0.3.0/setup.py
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-08-09 00:53:53.641550 inviz-0.3.0/src/
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-08-09 00:53:53.641550 inviz-0.3.0/src/cosmo/
+-rw-r--r--   0 jswen     (1000) jswen     (1000)       20 2023-08-05 07:38:29.000000 inviz-0.3.0/src/cosmo/__init__.py
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     2652 2023-08-09 00:30:13.000000 inviz-0.3.0/src/cosmo/cosmo.py
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-08-09 00:53:53.641550 inviz-0.3.0/src/inviz.egg-info/
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     2172 2023-08-09 00:53:53.000000 inviz-0.3.0/src/inviz.egg-info/PKG-INFO
+-rw-r--r--   0 jswen     (1000) jswen     (1000)      243 2023-08-09 00:53:53.000000 inviz-0.3.0/src/inviz.egg-info/SOURCES.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)        1 2023-08-09 00:53:53.000000 inviz-0.3.0/src/inviz.egg-info/dependency_links.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)      132 2023-08-09 00:53:53.000000 inviz-0.3.0/src/inviz.egg-info/requires.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)        6 2023-08-09 00:53:53.000000 inviz-0.3.0/src/inviz.egg-info/top_level.txt
```

### Comparing `inviz-0.2.8a2/LICENSE` & `inviz-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inviz-0.2.8a2/PKG-INFO` & `inviz-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: inviz
-Version: 0.2.8a2
-Summary: An interactive visualizer to help explore high-dimensional data and its observables.
+Version: 0.3.0
+Summary: An interactive visualizer to help explore high-dimensional likelihoods and their observables.
 Home-page: http://packages.python.org/inviz
 Author: James Wen
 Author-email: jswen@usc.edu
 License: MIT
 Keywords: interactive visualizer cosmology
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `inviz-0.2.8a2/README.md` & `inviz-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `inviz-0.2.8a2/setup.py` & `inviz-0.3.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "inviz",
-    version = "0.2.8a2",
+    version = "0.3.0",
     author = "James Wen",
     author_email = "jswen@usc.edu",
-    description = ("An interactive visualizer to help explore high-dimensional data and its observables."),
+    description = ("An interactive visualizer to help explore high-dimensional likelihoods and their observables."),
     license = "MIT",
     keywords = "interactive visualizer cosmology",
     url = "http://packages.python.org/inviz",
     packages=setuptools.find_packages(where='src'),
     # packages=['inviz', 'inviz.cosmo'],
     package_dir={'': 'src'},
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: POSIX :: Linux",
     ],
     python_requires='>=3.8',
-    install_requires=["holoviews==1.15.4",
-                      "panel==0.14.4",
+    install_requires=["holoviews>=1.15.4",
+                      "bokeh==2.4.3", # locking bokeh here until v3 works with latex
+                      "panel==0.14.4", # same here
                       "spatialpandas==0.4.8",
-                      "dask<=2023.5.0",
+                      "dask<=2023.5.0", # python 3.8 compatibility
                       "param==1.13.0",
                       "numpy>=1.21, <=1.24",
                       "matplotlib==3.7.1"]
     )
```

### Comparing `inviz-0.2.8a2/src/cosmo/cosmo.py` & `inviz-0.3.0/src/cosmo/cosmo.py`

 * *Files 27% similar despite different names*

```diff
@@ -18,58 +18,58 @@
 
 # create a DataFrame with the chain files as rows and use a list of parameters as the column names
 def load_data(filename, column_names):
     data = np.loadtxt(filename)
     df = pd.DataFrame(data[:,1:], columns=column_names)
     return df
 
-# run class on the user's selection
-def run_class(selection):
+# run class on the user's selection with default settings
+def run_class(index, sample):
+    selection = sample.iloc[[index]].to_dict('index')
+
     cosmo = Class()
-    cosmo.set(selection)
+    cosmo.set(selection[index])
     cosmo.set({'output':'mPk, tCl, pCl, lCl','P_k_max_1/Mpc':3.0, 'lensing':'yes'})
     cosmo.compute()
 
     # set variables for matter power spectrum and lensed CMB angular power spectra
     kk = np.logspace(-4,np.log10(3),1000)
     Pk = []
     h = cosmo.h()
     for k in kk:
         Pk.append(cosmo.pk(k*h,0.)*h**3)
     Pk = np.array(Pk)
     l = np.array(range(2,2501))
     factor = l*(l+1)/(2*np.pi)
     lensed_cl = cosmo.lensed_cl(2500)
     
-    results = {
-        'k': kk, 
-        'Pk': Pk, 
-        'l': l, 
-        'Cl_tt': factor*lensed_cl['tt'][2:], 
-        'Cl_ee': factor*lensed_cl['ee'][2:], 
-    }
-    # cleanups reqd for backwards compat w CLASS 2.x
+    results = [
+        {'k': kk, 'Pk': Pk},
+        {'l': l, 'Cl_tt': factor*lensed_cl['tt'][2:]},
+        {'l': l, 'Cl_ee': factor*lensed_cl['ee'][2:]}, 
+    ]
+    # cleanups requried for backwards compat w CLASS 2.x
     cosmo.struct_cleanup()
     cosmo.empty()
     return results
 
 # calculate percentage difference between model of interest and LambdaCDM model
 def compute_residuals(index, sample, sample_CDM):
-    selection = sample.iloc[[index]].to_dict('index')
-    selection_CDM = sample_CDM.iloc[[index]].to_dict('index')
     if __name__ == '__main__':
         with Pool() as p:
-            [mycosmo, LambdaCDM] = p.map(run_class, [selection[index], selection_CDM[index]])
+            [mycosmo, LambdaCDM] = p.starmap(run_class, [(index, sample), (index, sample_CDM)])
     else:
-        mycosmo = run_class(selection[index])
-        LambdaCDM = run_class(selection_CDM[index])
+        mycosmo = run_class(index, sample)
+        LambdaCDM = run_class((index, sample_CDM))
 
-    pk_residuals = (mycosmo['Pk'] - LambdaCDM['Pk'])/LambdaCDM['Pk']*100
-    cl_tt_residuals = (mycosmo['Cl_tt'] - LambdaCDM['Cl_tt'])/LambdaCDM['Cl_tt']*100
-    cl_ee_residuals = (mycosmo['Cl_ee'] - LambdaCDM['Cl_ee'])/LambdaCDM['Cl_ee']*100
+    myPk, myCl_tt, myCl_ee = mycosmo
+    LCDM_Pk, LCDM_Cl_tt, LCDM_Cl_ee = LambdaCDM
+    pk_residuals = (myPk['Pk'] - LCDM_Pk['Pk'])/LCDM_Pk['Pk']*100
+    cl_tt_residuals = (myCl_tt['Cl_tt'] - LCDM_Cl_tt['Cl_tt'])/LCDM_Cl_tt['Cl_tt']*100
+    cl_ee_residuals = (myCl_ee['Cl_ee'] - LCDM_Cl_ee['Cl_ee'])/LCDM_Cl_ee['Cl_ee']*100
     
     residuals = [
-        {'k': mycosmo['k'], 'pk_residuals': pk_residuals}, 
-        {'l': mycosmo['l'], 'cl_tt_residuals': cl_tt_residuals}, 
-        {'l': mycosmo['l'], 'cl_ee_residuals': cl_ee_residuals},
+        {'k': myPk['k'], 'pk_residuals': pk_residuals}, 
+        {'l': myCl_tt['l'], 'cl_tt_residuals': cl_tt_residuals}, 
+        {'l': myCl_ee['l'], 'cl_ee_residuals': cl_ee_residuals},
     ]
     return residuals
```

### Comparing `inviz-0.2.8a2/src/inviz.egg-info/PKG-INFO` & `inviz-0.3.0/src/inviz.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: inviz
-Version: 0.2.8a2
-Summary: An interactive visualizer to help explore high-dimensional data and its observables.
+Version: 0.3.0
+Summary: An interactive visualizer to help explore high-dimensional likelihoods and their observables.
 Home-page: http://packages.python.org/inviz
 Author: James Wen
 Author-email: jswen@usc.edu
 License: MIT
 Keywords: interactive visualizer cosmology
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

