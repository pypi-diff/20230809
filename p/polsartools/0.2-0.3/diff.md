# Comparing `tmp/polsartools-0.2.tar.gz` & `tmp/polsartools-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polsartools-0.2.tar", last modified: Thu Sep 29 17:26:17 2022, max compression
+gzip compressed data, was "polsartools-0.3.tar", last modified: Tue Aug  8 22:41:27 2023, max compression
```

## Comparing `polsartools-0.2.tar` & `polsartools-0.3.tar`

### file list

```diff
@@ -1,33 +1,38 @@
-drwxrwxrwx   0        0        0        0 2022-09-29 17:26:17.123362 polsartools-0.2/
--rw-rw-rw-   0        0        0    35803 2022-07-13 13:45:28.000000 polsartools-0.2/LICENSE
--rw-rw-rw-   0        0        0     1163 2022-09-29 17:26:17.123751 polsartools-0.2/PKG-INFO
--rw-rw-rw-   0        0        0      575 2022-09-29 03:22:39.000000 polsartools-0.2/README.md
--rw-rw-rw-   0        0        0      115 2022-09-29 16:34:38.000000 polsartools-0.2/pyproject.toml
--rw-rw-rw-   0        0        0      701 2022-09-29 17:26:17.130898 polsartools-0.2/setup.cfg
--rw-rw-rw-   0        0        0      772 2022-09-29 16:42:49.000000 polsartools-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2022-09-29 17:26:16.931535 polsartools-0.2/src/
-drwxrwxrwx   0        0        0        0 2022-09-29 17:26:17.103822 polsartools-0.2/src/polsartools/
--rw-rw-rw-   0        0        0      699 2022-09-29 17:16:37.000000 polsartools-0.2/src/polsartools/__init__.py
--rw-rw-rw-   0        0        0     3549 2022-09-29 16:53:42.000000 polsartools-0.2/src/polsartools/basic_func.py
--rw-rw-rw-   0        0        0     5092 2022-08-23 21:01:30.000000 polsartools-0.2/src/polsartools/convert.py
--rw-rw-rw-   0        0        0     4095 2022-09-29 16:56:38.000000 polsartools-0.2/src/polsartools/cprvi.py
--rw-rw-rw-   0        0        0     1744 2022-09-29 16:57:07.000000 polsartools-0.2/src/polsartools/dopcp.py
--rw-rw-rw-   0        0        0     1507 2022-09-29 16:57:34.000000 polsartools-0.2/src/polsartools/dopdp.py
--rw-rw-rw-   0        0        0     3120 2022-09-29 17:13:27.000000 polsartools-0.2/src/polsartools/dopfp.py
--rw-rw-rw-   0        0        0     1761 2022-09-29 16:59:17.000000 polsartools-0.2/src/polsartools/dprvi.py
--rw-rw-rw-   0        0        0    11535 2022-09-29 17:21:09.000000 polsartools-0.2/src/polsartools/grvi.py
--rw-rw-rw-   0        0        0     2546 2022-09-29 17:01:33.000000 polsartools-0.2/src/polsartools/mf3cc.py
--rw-rw-rw-   0        0        0     2179 2022-09-29 17:04:06.000000 polsartools-0.2/src/polsartools/mf3cd.py
--rw-rw-rw-   0        0        0     4198 2022-09-29 17:15:35.000000 polsartools-0.2/src/polsartools/mf3cf.py
--rw-rw-rw-   0        0        0     4873 2022-09-29 17:15:49.000000 polsartools-0.2/src/polsartools/mf4cf.py
--rw-rw-rw-   0        0        0     4084 2022-09-29 17:11:17.000000 polsartools-0.2/src/polsartools/mod_is_omega.py
--rw-rw-rw-   0        0        0     1524 2022-09-29 17:23:32.000000 polsartools-0.2/src/polsartools/prvidp.py
--rw-rw-rw-   0        0        0     3513 2022-09-29 17:14:43.000000 polsartools-0.2/src/polsartools/prvifp.py
--rw-rw-rw-   0        0        0     1451 2022-09-29 17:14:51.000000 polsartools-0.2/src/polsartools/rvidp.py
--rw-rw-rw-   0        0        0     4819 2022-09-29 17:21:18.000000 polsartools-0.2/src/polsartools/rvifp.py
-drwxrwxrwx   0        0        0        0 2022-09-29 17:26:17.122252 polsartools-0.2/src/polsartools.egg-info/
--rw-rw-rw-   0        0        0     1163 2022-09-29 17:26:16.000000 polsartools-0.2/src/polsartools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      713 2022-09-29 17:26:16.000000 polsartools-0.2/src/polsartools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-29 17:26:16.000000 polsartools-0.2/src/polsartools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2022-09-29 17:26:16.000000 polsartools-0.2/src/polsartools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-09-29 17:26:16.000000 polsartools-0.2/src/polsartools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-08 22:41:27.353123 polsartools-0.3/
+-rw-rw-rw-   0        0        0    35803 2022-07-13 13:45:28.000000 polsartools-0.3/LICENSE
+-rw-rw-rw-   0        0        0     6987 2023-08-08 22:41:27.353123 polsartools-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6399 2023-08-08 22:34:59.000000 polsartools-0.3/README.md
+-rw-rw-rw-   0        0        0      115 2022-09-29 16:34:38.000000 polsartools-0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      701 2023-08-08 22:41:27.354723 polsartools-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      772 2023-08-08 21:30:05.000000 polsartools-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 22:41:27.228108 polsartools-0.3/src/
+drwxrwxrwx   0        0        0        0 2023-08-08 22:41:27.338758 polsartools-0.3/src/polsartools/
+-rw-rw-rw-   0        0        0      754 2023-08-08 21:40:06.000000 polsartools-0.3/src/polsartools/__init__.py
+-rw-rw-rw-   0        0        0     3549 2022-09-29 16:53:42.000000 polsartools-0.3/src/polsartools/basic_func.py
+-rw-rw-rw-   0        0        0     6620 2022-10-01 01:19:18.000000 polsartools-0.3/src/polsartools/convert.py
+-rw-rw-rw-   0        0        0     4095 2022-09-29 16:56:38.000000 polsartools-0.3/src/polsartools/cprvi.py
+-rw-rw-rw-   0        0        0     1744 2022-09-29 16:57:07.000000 polsartools-0.3/src/polsartools/dopcp.py
+-rw-rw-rw-   0        0        0     1507 2022-09-29 16:57:34.000000 polsartools-0.3/src/polsartools/dopdp.py
+-rw-rw-rw-   0        0        0     3120 2022-09-29 17:13:27.000000 polsartools-0.3/src/polsartools/dopfp.py
+-rw-rw-rw-   0        0        0     1027 2022-10-01 21:34:19.000000 polsartools-0.3/src/polsartools/dpdesc.py
+-rw-rw-rw-   0        0        0     1761 2022-09-29 16:59:17.000000 polsartools-0.3/src/polsartools/dprvi.py
+-rw-rw-rw-   0        0        0      680 2022-10-01 01:57:36.000000 polsartools-0.3/src/polsartools/dprvic.py
+-rw-rw-rw-   0        0        0    11535 2022-09-29 17:21:09.000000 polsartools-0.3/src/polsartools/grvi.py
+-rw-rw-rw-   0        0        0     5392 2023-08-08 22:30:43.000000 polsartools-0.3/src/polsartools/import_uavsar.py
+-rw-rw-rw-   0        0        0     2546 2022-09-29 17:01:33.000000 polsartools-0.3/src/polsartools/mf3cc.py
+-rw-rw-rw-   0        0        0     2179 2022-09-29 17:04:06.000000 polsartools-0.3/src/polsartools/mf3cd.py
+-rw-rw-rw-   0        0        0     4198 2022-09-29 17:15:35.000000 polsartools-0.3/src/polsartools/mf3cf.py
+-rw-rw-rw-   0        0        0     4873 2022-09-29 17:15:49.000000 polsartools-0.3/src/polsartools/mf4cf.py
+-rw-rw-rw-   0        0        0     4084 2022-09-29 17:11:17.000000 polsartools-0.3/src/polsartools/mod_is_omega.py
+-rw-rw-rw-   0        0        0     1524 2022-09-29 17:23:32.000000 polsartools-0.3/src/polsartools/prvidp.py
+-rw-rw-rw-   0        0        0     3513 2022-09-29 17:14:43.000000 polsartools-0.3/src/polsartools/prvifp.py
+-rw-rw-rw-   0        0        0     1451 2022-09-29 17:14:51.000000 polsartools-0.3/src/polsartools/rvidp.py
+-rw-rw-rw-   0        0        0     4819 2022-09-29 17:21:18.000000 polsartools-0.3/src/polsartools/rvifp.py
+drwxrwxrwx   0        0        0        0 2023-08-08 22:41:27.348125 polsartools-0.3/src/polsartools.egg-info/
+-rw-rw-rw-   0        0        0     6987 2023-08-08 22:41:27.000000 polsartools-0.3/src/polsartools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      822 2023-08-08 22:41:27.000000 polsartools-0.3/src/polsartools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 22:41:27.000000 polsartools-0.3/src/polsartools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-08-08 22:41:27.000000 polsartools-0.3/src/polsartools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-08-08 22:41:27.000000 polsartools-0.3/src/polsartools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-08 22:41:27.352131 polsartools-0.3/tests/
+-rw-rw-rw-   0        0        0     1094 2022-09-29 17:24:38.000000 polsartools-0.3/tests/test_functions.py
```

### Comparing `polsartools-0.2/LICENSE` & `polsartools-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `polsartools-0.2/setup.cfg` & `polsartools-0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `polsartools-0.2/setup.py` & `polsartools-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='polsartools',
-    version='0.2',    
+    version='0.3',    
     description='A package to process Synthetic Aperture Radar data',
     url='https://github.com/Narayana-Rao/polsartools',
     author='Narayanarao Bhogapurapu',
     author_email='bnarayanarao@iitb.ac.in',
     license='GPL-3.0 license',
     packages=['polsartools'],
     install_requires=['gdal',
```

### Comparing `polsartools-0.2/src/polsartools/__init__.py` & `polsartools-0.3/src/polsartools/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 from .rvidp import rvidp
 from .prvidp import prvidp
 
 from .cprvi import cprvi
 from .dopcp import dopcp
 from .mf3cc import mf3cc
 from .mod_is_omega import mod_is_omega
-
+from .import_uavsar import uavsar_grd_c3, uavsar_mlc_c3
 
 from .convert import T3_C3, C3_compact_C2, C3_c2, S2_T3
 
 
 ############################
-__version__ = "0.2"
+__version__ = "0.3"
 __author__ = 'Narayanarao Bhogapurapu'
 __credits__ = 'Microwave Remote Sensing Lab (MRSLab)'
```

### Comparing `polsartools-0.2/src/polsartools/basic_func.py` & `polsartools-0.3/src/polsartools/basic_func.py`

 * *Files identical despite different names*

### Comparing `polsartools-0.2/src/polsartools/convert.py` & `polsartools-0.3/src/polsartools/convert.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,14 +18,28 @@
     TT1 = TT1[0,:,:]
     TT1 = np.reshape(TT1,(TT1.shape[0],3,3))
     TT1 = np.matmul(np.matmul((D.T),TT1),D)
     TT1 = np.reshape(TT1,(TT1.shape[0],9))
 
     return np.reshape(TT1,(nrows,ncols,9)) 
 
+def C3_T3(C3_stack):
+    nrows = np.size(C3_stack,0)
+    ncols = np.size(C3_stack,1)
+    
+    D = (1/np.sqrt(2))*np.array([[1,0,1], [1,0,-1],[0,np.sqrt(2),0]])
+    CC1 = np.dstack((C3_stack[:,:,0].flatten(), C3_stack[:,:,1].flatten(), C3_stack[:,:,2].flatten(),
+                     C3_stack[:,:,3].flatten(), C3_stack[:,:,4].flatten(), C3_stack[:,:,5].flatten(),
+                     C3_stack[:,:,6].flatten(), C3_stack[:,:,7].flatten(), C3_stack[:,:,8].flatten()))
+    CC1 = CC1[0,:,:]
+    CC1 = np.reshape(CC1,(CC1.shape[0],3,3))
+    CC1 = np.matmul(np.matmul((D),CC1),D.T)
+    CC1 = np.reshape(CC1,(CC1.shape[0],9))
+
+    return np.reshape(CC1,(nrows,ncols,9)) 
 
 def C3_compact_C2(C3,psi,chi):
 
 
 	C11 = C3[:,:,0]
 	C12 = C3[:,:,1]
 	C13 = C3[:,:,2]
@@ -57,15 +71,26 @@
 
 	CP22 = 0.5*(0.5*(1+np.cos(2*psi)*np.cos(2*chi))*C3[:,:,4]+
 	                (1-np.cos(2*psi)*np.cos(2*chi))*C3[:,:,8]+
 	              (1/np.sqrt(2))*(np.sin(2*psi)*np.cos(2*chi))*(C3[:,:,5]+np.conj(C3[:,:,5]))+
 	                (1j/np.sqrt(2))*np.sin(2*chi)*(C3[:,:,5]-np.conj(C3[:,:,5])) 
 	            )
 
-	return CP11, CP12, CP22
+	return np.dstack((CP11, CP12, np.conjugate(CP12),CP22))
+
+
+def C3_c21(C3_stack):
+	return np.dstack((np.real(C3_stack[:,:,0]),np.real((C3_stack[:,:,1])/np.sqrt(2))+1j*np.imag((C3_stack[:,:,1])/np.sqrt(2)), np.real((C3_stack[:,:,1])/np.sqrt(2))-1j*np.imag((C3_stack[:,:,1])/np.sqrt(2)), np.real((C3_stack[:,:,4])/(2))))
+
+def C3_c22(C3_stack):
+	return np.dstack((np.real(C3_stack[:,:,8]),np.real((C3_stack[:,:,5])/np.sqrt(2))+1j*np.imag((C3_stack[:,:,5])/np.sqrt(2)), np.real((C3_stack[:,:,5])/np.sqrt(2))-1j*np.imag((C3_stack[:,:,5])/np.sqrt(2)), np.real((C3_stack[:,:,4])/(2))))
+	
+def C3_c23(C3_stack):
+	return np.dstack((np.real(C3_stack[:,:,0]),np.real((C3_stack[:,:,2])/np.sqrt(2))+1j*np.imag((C3_stack[:,:,2])/np.sqrt(2)), np.real((C3_stack[:,:,2])/np.sqrt(2))-1j*np.imag((C3_stack[:,:,2])/np.sqrt(2)), np.real((C3_stack[:,:,8])/(2))))
+	
 
 def C3_c2(inFolder):
 
 	if os.path.isfile(inFolder+'/C11.bin'):
 	    
 	    C3_stack = load_C3(inFolder)
 	    # T3_stack = C3_T3(C3_stack)
@@ -144,7 +169,18 @@
 	T22 = np.abs(Kp[1])**2
 	T33 = np.abs(Kp[2])**2
 
 	T12 = Kp[0]*np.conj(Kp[1])
 	T13 = Kp[0]*np.conj(Kp[2])
 	T23 = Kp[1]*np.conj(Kp[2])
 	return np.dstack((T11,T12,T13,np.conjugate(T12),T22,T23,np.conjugate(T13),T23,T33))
+
+
+
+
+
+
+
+
+
+
+
```

### Comparing `polsartools-0.2/src/polsartools/cprvi.py` & `polsartools-0.3/src/polsartools/cprvi.py`

 * *Files identical despite different names*

### Comparing `polsartools-0.2/src/polsartools/dopcp.py` & `polsartools-0.3/src/polsartools/dopcp.py`

 * *Files identical despite different names*

### Comparing `polsartools-0.2/src/polsartools/dopdp.py` & `polsartools-0.3/src/polsartools/dopdp.py`

 * *Files identical despite different names*

### Comparing `polsartools-0.2/src/polsartools/dopfp.py` & `polsartools-0.3/src/polsartools/dopfp.py`

 * *Files identical despite different names*

### Comparing `polsartools-0.2/src/polsartools/dprvi.py` & `polsartools-0.3/src/polsartools/dprvi.py`

 * *Files identical despite different names*

### Comparing `polsartools-0.2/src/polsartools/grvi.py` & `polsartools-0.3/src/polsartools/grvi.py`

 * *Files identical despite different names*

### Comparing `polsartools-0.2/src/polsartools/mf3cc.py` & `polsartools-0.3/src/polsartools/mf3cc.py`

 * *Files identical despite different names*

### Comparing `polsartools-0.2/src/polsartools/mf3cd.py` & `polsartools-0.3/src/polsartools/mf3cd.py`

 * *Files identical despite different names*

### Comparing `polsartools-0.2/src/polsartools/mf3cf.py` & `polsartools-0.3/src/polsartools/mf3cf.py`

 * *Files identical despite different names*

### Comparing `polsartools-0.2/src/polsartools/mf4cf.py` & `polsartools-0.3/src/polsartools/mf4cf.py`

 * *Files identical despite different names*

### Comparing `polsartools-0.2/src/polsartools/mod_is_omega.py` & `polsartools-0.3/src/polsartools/mod_is_omega.py`

 * *Files identical despite different names*

### Comparing `polsartools-0.2/src/polsartools/prvidp.py` & `polsartools-0.3/src/polsartools/prvidp.py`

 * *Files identical despite different names*

### Comparing `polsartools-0.2/src/polsartools/prvifp.py` & `polsartools-0.3/src/polsartools/prvifp.py`

 * *Files identical despite different names*

### Comparing `polsartools-0.2/src/polsartools/rvidp.py` & `polsartools-0.3/src/polsartools/rvidp.py`

 * *Files identical despite different names*

### Comparing `polsartools-0.2/src/polsartools/rvifp.py` & `polsartools-0.3/src/polsartools/rvifp.py`

 * *Files identical despite different names*

### Comparing `polsartools-0.2/src/polsartools.egg-info/SOURCES.txt` & `polsartools-0.3/src/polsartools.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -6,23 +6,27 @@
 src/polsartools/__init__.py
 src/polsartools/basic_func.py
 src/polsartools/convert.py
 src/polsartools/cprvi.py
 src/polsartools/dopcp.py
 src/polsartools/dopdp.py
 src/polsartools/dopfp.py
+src/polsartools/dpdesc.py
 src/polsartools/dprvi.py
+src/polsartools/dprvic.py
 src/polsartools/grvi.py
+src/polsartools/import_uavsar.py
 src/polsartools/mf3cc.py
 src/polsartools/mf3cd.py
 src/polsartools/mf3cf.py
 src/polsartools/mf4cf.py
 src/polsartools/mod_is_omega.py
 src/polsartools/prvidp.py
 src/polsartools/prvifp.py
 src/polsartools/rvidp.py
 src/polsartools/rvifp.py
 src/polsartools.egg-info/PKG-INFO
 src/polsartools.egg-info/SOURCES.txt
 src/polsartools.egg-info/dependency_links.txt
 src/polsartools.egg-info/requires.txt
-src/polsartools.egg-info/top_level.txt
+src/polsartools.egg-info/top_level.txt
+tests/test_functions.py
```

