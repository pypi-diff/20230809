# Comparing `tmp/MLTF-0.1.tar.gz` & `tmp/MLTF-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/users/aanavarroa/original_gitrepos/MLTF/dist/tmp3el4v80o/MLTF-0.1.tar", last modified: Thu Mar 30 18:25:33 2023, max compression
+gzip compressed data, was "MLTF-0.1.1.tar", last modified: Tue Aug  8 22:31:37 2023, max compression
```

## Comparing `MLTF-0.1.tar` & `MLTF-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,30 @@
-drwxr-xr-x   0 aanavarroa (12499) users      (100)        0 2023-03-30 18:25:33.000000 MLTF-0.1/
--rw-r--r--   0 aanavarroa (12499) users      (100)      588 2023-03-30 18:09:21.000000 MLTF-0.1/pyproject.toml
--rw-r--r--   0 aanavarroa (12499) users      (100)      273 2023-03-30 18:08:39.000000 MLTF-0.1/README.md
--rw-r--r--   0 aanavarroa (12499) users      (100)     1068 2023-03-29 12:40:58.000000 MLTF-0.1/LICENSE
--rw-r--r--   0 aanavarroa (12499) users      (100)      201 2023-03-30 18:25:33.000000 MLTF-0.1/PKG-INFO
--rw-r--r--   0 aanavarroa (12499) users      (100)      300 2023-03-30 18:07:16.000000 MLTF-0.1/setup.py
--rw-r--r--   0 aanavarroa (12499) users      (100)       38 2023-03-30 18:25:33.000000 MLTF-0.1/setup.cfg
-drwxr-xr-x   0 aanavarroa (12499) users      (100)        0 2023-03-30 18:25:33.000000 MLTF-0.1/python/
-drwxr-xr-x   0 aanavarroa (12499) users      (100)        0 2023-03-30 18:25:33.000000 MLTF-0.1/python/MLTF.egg-info/
--rw-r--r--   0 aanavarroa (12499) users      (100)      415 2023-03-30 18:25:33.000000 MLTF-0.1/python/MLTF.egg-info/SOURCES.txt
--rw-r--r--   0 aanavarroa (12499) users      (100)        5 2023-03-30 18:25:33.000000 MLTF-0.1/python/MLTF.egg-info/top_level.txt
--rw-r--r--   0 aanavarroa (12499) users      (100)      201 2023-03-30 18:25:33.000000 MLTF-0.1/python/MLTF.egg-info/PKG-INFO
--rw-r--r--   0 aanavarroa (12499) users      (100)       17 2023-03-30 18:25:33.000000 MLTF-0.1/python/MLTF.egg-info/requires.txt
--rw-r--r--   0 aanavarroa (12499) users      (100)        1 2023-03-30 18:25:33.000000 MLTF-0.1/python/MLTF.egg-info/dependency_links.txt
-drwxr-xr-x   0 aanavarroa (12499) users      (100)        0 2023-03-30 18:25:33.000000 MLTF-0.1/python/MLTF/
--rw-r--r--   0 aanavarroa (12499) users      (100)     2917 2023-03-30 18:12:15.000000 MLTF-0.1/python/MLTF/layer.py
--rw-r--r--   0 aanavarroa (12499) users      (100)    10572 2023-03-30 18:12:57.000000 MLTF-0.1/python/MLTF/plot.py
--rw-r--r--   0 aanavarroa (12499) users      (100)     5413 2022-09-13 16:00:59.000000 MLTF-0.1/python/MLTF/normer.py
--rw-r--r--   0 aanavarroa (12499) users      (100)      248 2023-03-30 18:16:59.000000 MLTF-0.1/python/MLTF/__init__.py
--rw-r--r--   0 aanavarroa (12499) users      (100)     8601 2023-03-30 18:12:26.000000 MLTF-0.1/python/MLTF/loss_functions.py
--rw-r--r--   0 aanavarroa (12499) users      (100)      297 2020-08-04 19:23:24.000000 MLTF-0.1/python/MLTF/info.py
--rw-r--r--   0 aanavarroa (12499) users      (100)     2683 2023-03-30 18:13:27.000000 MLTF-0.1/python/MLTF/tools.py
--rw-r--r--   0 aanavarroa (12499) users      (100)    25414 2023-03-30 18:12:43.000000 MLTF-0.1/python/MLTF/models.py
--rw-r--r--   0 aanavarroa (12499) users      (100)     3545 2023-03-30 18:11:47.000000 MLTF-0.1/python/MLTF/calc.py
+drwxr-xr-x   0 andres    (1000) users      (984)        0 2023-08-08 22:31:37.369822 MLTF-0.1.1/
+-rw-r--r--   0 andres    (1000) users      (984)     1068 2023-08-04 13:38:34.000000 MLTF-0.1.1/LICENSE
+-rw-r--r--   0 andres    (1000) users      (984)     1084 2023-08-08 22:31:37.366488 MLTF-0.1.1/PKG-INFO
+-rw-r--r--   0 andres    (1000) users      (984)      466 2023-08-08 22:15:14.000000 MLTF-0.1.1/README.md
+-rw-r--r--   0 andres    (1000) users      (984)      675 2023-08-08 22:31:22.000000 MLTF-0.1.1/pyproject.toml
+drwxr-xr-x   0 andres    (1000) users      (984)        0 2023-08-08 22:31:37.359821 MLTF-0.1.1/python/
+drwxr-xr-x   0 andres    (1000) users      (984)        0 2023-08-08 22:31:37.363155 MLTF-0.1.1/python/MLTF/
+-rw-r--r--   0 andres    (1000) users      (984)      248 2023-08-04 13:38:34.000000 MLTF-0.1.1/python/MLTF/__init__.py
+-rw-r--r--   0 andres    (1000) users      (984)     3545 2023-08-04 13:38:34.000000 MLTF-0.1.1/python/MLTF/calc.py
+-rw-r--r--   0 andres    (1000) users      (984)      297 2023-08-04 13:38:34.000000 MLTF-0.1.1/python/MLTF/info.py
+-rw-r--r--   0 andres    (1000) users      (984)     2917 2023-08-04 13:38:34.000000 MLTF-0.1.1/python/MLTF/layer.py
+-rw-r--r--   0 andres    (1000) users      (984)     8614 2023-08-04 13:38:34.000000 MLTF-0.1.1/python/MLTF/loss_functions.py
+-rw-r--r--   0 andres    (1000) users      (984)    26114 2023-08-04 13:38:34.000000 MLTF-0.1.1/python/MLTF/models.py
+-rw-r--r--   0 andres    (1000) users      (984)     5413 2023-08-04 13:38:34.000000 MLTF-0.1.1/python/MLTF/normer.py
+-rw-r--r--   0 andres    (1000) users      (984)    10572 2023-08-04 13:38:34.000000 MLTF-0.1.1/python/MLTF/plot.py
+-rw-r--r--   0 andres    (1000) users      (984)     2683 2023-08-04 13:38:34.000000 MLTF-0.1.1/python/MLTF/tools.py
+drwxr-xr-x   0 andres    (1000) users      (984)        0 2023-08-08 22:31:37.366488 MLTF-0.1.1/python/MLTF.egg-info/
+-rw-r--r--   0 andres    (1000) users      (984)     1084 2023-08-08 22:31:37.000000 MLTF-0.1.1/python/MLTF.egg-info/PKG-INFO
+-rw-r--r--   0 andres    (1000) users      (984)      534 2023-08-08 22:31:37.000000 MLTF-0.1.1/python/MLTF.egg-info/SOURCES.txt
+-rw-r--r--   0 andres    (1000) users      (984)        1 2023-08-08 22:31:37.000000 MLTF-0.1.1/python/MLTF.egg-info/dependency_links.txt
+-rw-r--r--   0 andres    (1000) users      (984)       17 2023-08-08 22:31:37.000000 MLTF-0.1.1/python/MLTF.egg-info/requires.txt
+-rw-r--r--   0 andres    (1000) users      (984)        5 2023-08-08 22:31:37.000000 MLTF-0.1.1/python/MLTF.egg-info/top_level.txt
+-rw-r--r--   0 andres    (1000) users      (984)       38 2023-08-08 22:31:37.369822 MLTF-0.1.1/setup.cfg
+-rw-r--r--   0 andres    (1000) users      (984)      300 2023-08-04 13:38:34.000000 MLTF-0.1.1/setup.py
+drwxr-xr-x   0 andres    (1000) users      (984)        0 2023-08-08 22:31:37.366488 MLTF-0.1.1/tests/
+-rw-r--r--   0 andres    (1000) users      (984)      268 2023-08-04 13:38:34.000000 MLTF-0.1.1/tests/test_MLTF.py
+-rw-r--r--   0 andres    (1000) users      (984)     1194 2023-08-04 13:38:34.000000 MLTF-0.1.1/tests/test_MLTF_layer.py
+-rw-r--r--   0 andres    (1000) users      (984)     2256 2023-08-04 13:38:34.000000 MLTF-0.1.1/tests/test_MLTF_loss.py
+-rw-r--r--   0 andres    (1000) users      (984)      789 2023-08-04 13:38:34.000000 MLTF-0.1.1/tests/test_MLTF_model.py
+-rw-r--r--   0 andres    (1000) users      (984)      845 2023-08-04 13:38:34.000000 MLTF-0.1.1/tests/test_MLTF_normer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `MLTF-0.1/pyproject.toml` & `MLTF-0.1.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["setuptools>=38", "wheel", "pybind11>=2.2"]
 
 [project]
 name = "MLTF"
-version = "0.0.1"
+version = "0.1.1"
 authors = [
   { name="Andres Navarro Alsina", email="a.navarro.alsina@gmail.com" },
 ]
-description = "Basic modules for ML model based on TensorFlow"
+description = "Toolkit for creating ML models using tensorflow. Designed to short-cut implementation of widely used neuronal networks architectures."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `MLTF-0.1/LICENSE` & `MLTF-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `MLTF-0.1/python/MLTF/layer.py` & `MLTF-0.1.1/python/MLTF/layer.py`

 * *Files identical despite different names*

### Comparing `MLTF-0.1/python/MLTF/plot.py` & `MLTF-0.1.1/python/MLTF/plot.py`

 * *Files identical despite different names*

### Comparing `MLTF-0.1/python/MLTF/normer.py` & `MLTF-0.1.1/python/MLTF/normer.py`

 * *Files identical despite different names*

### Comparing `MLTF-0.1/python/MLTF/loss_functions.py` & `MLTF-0.1.1/python/MLTF/loss_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,35 +19,36 @@
 Created on: 13/09/22
 Author: Andres Navarro
 """
 import logging
 import tensorflow as tf
 
 logger = logging.getLogger(__name__)
+PRECISION=tf.float32 
 
 def mse(targets, preds, mask=None):
     #assert preds[0].get_shape() ==mask[0].get_shape()     
     #assert tf.shape(preds[0])==tf.shape(mask[0])
     if tf.keras.backend.ndim(preds) == 3:
         if mask is not None:
-            npoints=tf.cast(tf.shape(preds)[0]*tf.shape(preds)[1], tf.float32)
+            npoints=tf.cast(tf.shape(preds)[0]*tf.shape(preds)[1], PRECISION)
             mask_factor=npoints/tf.keras.backend.sum(mask)
             squarebias=mask_factor*tf.keras.backend.square(mask*(preds-targets))
         else:
             squarebias=tf.keras.backend.square(preds-targets)
         mse_val=tf.keras.backend.mean(squarebias)
             
 
     return mse_val
 
 def msb(targets, preds, mask=None, caseweights=None):
     #assert preds[0].get_shape() ==mask[0].get_shape()
     if tf.keras.backend.ndim(preds) == 3:
         if mask is not None:        
-            nrea= tf.cast(tf.shape(preds)[1],tf.float32)
+            nrea= tf.cast(tf.shape(preds)[1],PRECISION)
             masked_preds=preds*mask
             mask_factor=nrea/tf.keras.backend.sum(mask,axis=1, keepdims=True)
             means=mask_factor*tf.keras.backend.mean(masked_preds, axis=1, keepdims=True)
         else:
             means=tf.keras.backend.mean(preds, axis=1, keepdims=True)
             
         biases = means - targets
@@ -87,15 +88,15 @@
         else:
             num = tf.keras.backend.mean(preds*point_preds, axis=1, keepdims=True) 
             den = tf.keras.backend.mean(preds , axis=1, keepdims=True) 
         biases = num/den - targets
         mswb_val=tf.keras.backend.mean(tf.keras.backend.square(biases))
 
         if mask is not None:
-            nrea= tf.cast(tf.shape(preds)[1],tf.float32)
+            nrea= tf.cast(tf.shape(preds)[1],PRECISION)
             mask_factor=nrea/tf.keras.backend.sum(mask,axis=1, keepdims=True)
             mean_preds_rea=mask_factor*tf.keras.backend.mean(masked_preds, axis=1, keepdims=True)
             mean_preds= tf.keras.backend.mean(mean_preds_rea)
         else:
             mean_preds = tf.keras.backend.mean(preds)
         lagrange_term=lamb*tf.keras.backend.square(mean_preds -0.5)
     return mswb_val+lagrange_term
@@ -106,31 +107,31 @@
     if tf.keras.backend.ndim(preds) == 3:
         if mask is not None:
             masked_preds=preds*mask
             #mask factor cancel out for this case
             num = tf.keras.backend.mean(masked_preds*point_preds, axis=1, keepdims=True) 
             den = tf.keras.backend.mean(masked_preds , axis=1, keepdims=True)
 
-            nrea= tf.cast(tf.shape(preds)[1],tf.float32)
+            nrea= tf.cast(tf.shape(preds)[1],PRECISION)
             mask_factor=nrea/tf.keras.backend.sum(mask,axis=1, keepdims=True)
             lagrange_term= lamb*tf.keras.backend.square(mask_factor*den-mweight)
         else:
             num = tf.keras.backend.mean(preds*point_preds, axis=1, keepdims=True) 
             den = tf.keras.backend.mean(preds , axis=1, keepdims=True)
             lagrange_term= lamb*tf.keras.backend.square(den-mweight)
         biases = num/den - targets
         mswb_val=tf.keras.backend.mean(tf.keras.backend.square(biases)+tf.keras.backend.square(lagrange_term))
 
     return mswb_val
 
 def msmb(targets, preds, point_preds, mask=None):
     if tf.keras.backend.ndim(preds) == 3:
         if mask is not None:
-            #nrea= tf.constant(preds.get_shape().as_list()[1],tf.float32)
-            nrea= tf.cast(tf.shape(preds)[1],tf.float32)
+            #nrea= tf.constant(preds.get_shape().as_list()[1],PRECISION)
+            nrea= tf.cast(tf.shape(preds)[1],PRECISION)
             mask_factor=nrea/tf.keras.backend.sum(mask,axis=1, keepdims=True)
             masked_preds=(1+preds)*mask
             #masked_preds=(0.5+preds)*mask
             pred_masked_mean= mask_factor*tf.keras.backend.mean(masked_preds,axis=1,keepdims=True)
             num = mask_factor*tf.keras.backend.mean(masked_preds*point_preds,axis=1,keepdims=True)
         else:
             num = tf.keras.backend.mean(( 1+preds)*point_preds, axis=1, keepdims=True)
@@ -159,33 +160,33 @@
 
 # NEGATIVE LOG LIKELIHOOD
 def nll(targets, pred_distribution , mask=None):
     if tf.keras.backend.ndim(pred_distribution) == 2:
         targets=tf.reshape(targets, tf.shape(targets)[:2])
         if mask is not None:
             mask=tf.keras.backend.sum(mask, axis=2, keepdims=False)
-            nrea=tf.cast(tf.shape(mask)[1], tf.float32)
+            nrea=tf.cast(tf.shape(mask)[1], PRECISION)
             mask_factor=nrea/tf.keras.backend.sum(mask, axis=1, keepdims=True)
             nll=-pred_distribution.log_prob(targets)
             NLL=mask_factor*mask*nll            
         else:
             NLL=-pred_distribution.log_prob(targets)
        
 
     if tf.keras.backend.ndim(pred_distribution) == 3:
         if mask is not None:
             #assert tf.shape(pred_distribution)[0]==tf.shape(mask)[0]
         
-            nrea=tf.cast(tf.shape(mask)[1], tf.float32)
+            nrea=tf.cast(tf.shape(mask)[1], PRECISION)
             mask_factor=nrea/tf.keras.backend.sum(mask,axis=1, keepdims=True)
             nll=tf.reshape(-pred_distribution.log_prob(targets),tf.shape(mask))
             NLL=mask_factor*mask*nll
             
             '''
-            npoints=tf.cast(tf.shape(mask)[0]*tf.shape(mask)[1], tf.float32)
+            npoints=tf.cast(tf.shape(mask)[0]*tf.shape(mask)[1], PRECISION)
             mask_factor=npoints/tf.keras.backend.sum(mask)
             nll=tf.reshape(-pred_distribution.log_prob(targets),tf.shape(mask))
             NLL=mask_factor*mask*nll
             '''
             
         else:
             NLL=-pred_distribution.log_prob(targets)
```

### Comparing `MLTF-0.1/python/MLTF/tools.py` & `MLTF-0.1.1/python/MLTF/tools.py`

 * *Files identical despite different names*

### Comparing `MLTF-0.1/python/MLTF/models.py` & `MLTF-0.1.1/python/MLTF/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 
 Created on: 13/09/22
 Author: Andres Navarro
 """
 
 import logging
 from . import layer
-from . import loss_functions
 import tensorflow as tf
 import numpy as np
 
 logger = logging.getLogger(__name__)
 
 def get_model(hidden_sizes=(5,5), activation='sigmoid', layer=layer.TfbilacLayer, dropout_prob=0.0, outnodes=1):
     model = tf.keras.Sequential()
@@ -41,26 +40,30 @@
     if outnodes>0: model.add(layer(outnodes))
 
     return model
 
     #print(model.summary(line_length=100))
 
 
-def create_model(input_shape=None, hidden_sizes=(5,5), layer=layer.TfbilacLayer, activation='sigmoid', out_activation=None, loss_name='msb', use_mask=False, use_caseweights=False, lamb=None, dropout_prob=0.0,training=None):
+def create_model(input_shape=None, hidden_sizes=(5,5), layer=layer.TfbilacLayer, activation='sigmoid', out_activation=None, loss_name='msb', use_mask=False, use_caseweights=False, lamb=None, dropout_prob=0.0,training=None,dtype='float32'):
+    from . import loss_functions
+    if dtype=='float32':
+        loss_functions.PRECISION=tf.float32
+    if dtype=='float16':
+        loss_functions.PRECISION=tf.float16 
     #lamb: value for lagrange multiplier if loss function involves it.
-    tf.keras.backend.clear_session()
     if input_shape is not None:
         nreas = input_shape[0]
         nfeas = input_shape[1]
     else:
         nreas=None
         nfeas=None
         input_shape=(nreas,nfeas)
-    input_fea=tf.keras.Input(input_shape,dtype='float32') #feat
-    input_tar=tf.keras.Input((1, 1),dtype='float32') #targets
+    input_fea=tf.keras.Input(input_shape,dtype=dtype) #feat
+    input_tar=tf.keras.Input((1, 1),dtype=dtype) #targets
     inputs= [input_fea,input_tar]
     
     model = get_model(hidden_sizes=hidden_sizes, activation=activation,  layer=layer,dropout_prob=dropout_prob )
 
     shift=False; shiftval=1.0
     
     if out_activation is None:
@@ -82,80 +85,80 @@
                 model.add(tf.keras.layers.Activation(out_activation))
 
     x=model(inputs[0], training=training)
 
     if loss_name == 'mse':
         logger.info("Using %s"%(loss_name))
         if use_mask:
-            input_mask = tf.keras.Input((nreas,1),dtype='float32')
+            input_mask = tf.keras.Input((nreas,1),dtype=dtype)
             inputs.append(input_mask)
             loss_func =loss_functions.mse( inputs[1], x, mask=inputs[2])
         else:
             loss_func=loss_functions.mse( inputs[1], x)
     
     if loss_name == 'msb':
         logger.info("Using %s"%(loss_name))
         if use_mask&(~use_caseweights):
-            #input_mask = tf.keras.Input(input_shape,dtype='float32')
-            input_mask = tf.keras.Input((nreas,1),dtype='float32')
+            #input_mask = tf.keras.Input(input_shape,dtype=dtype)
+            input_mask = tf.keras.Input((nreas,1),dtype=dtype)
             inputs.append(input_mask)
             loss_func =loss_functions.msb( inputs[1], x, mask=inputs[2])
         elif use_mask&use_caseweights:
-            input_mask = tf.keras.Input((nreas,1),dtype='float32'); inputs.append(input_mask)
-            input_caseweights = tf.keras.Input((1,1),dtype='float32'); inputs.append(input_caseweights)
+            input_mask = tf.keras.Input((nreas,1),dtype=dtype); inputs.append(input_mask)
+            input_caseweights = tf.keras.Input((1,1),dtype=dtype); inputs.append(input_caseweights)
             loss_func =loss_functions.msb( inputs[1], x, mask=inputs[2], caseweights=inputs[3])
         else:
             loss_func=loss_functions.msb( inputs[1], x)
 
     if loss_name == 'msmb':
         logger.info("Using %s"%(loss_name))
 
-        input_pointpreds=tf.keras.Input((nreas, 1),dtype='float32')
+        input_pointpreds=tf.keras.Input((nreas, 1),dtype=dtype)
         inputs.append(input_pointpreds)
         if use_mask:
-            input_mask = tf.keras.Input((nreas,1),dtype='float32')
+            input_mask = tf.keras.Input((nreas,1),dtype=dtype)
             inputs.append(input_mask)
             loss_func =loss_functions.msmb( inputs[1], x, inputs[2], mask=inputs[3])
         else:
             loss_func =loss_functions.msmb( inputs[1], x, inputs[2])
             
     if loss_name == 'mswb':
         logger.info("Using %s"%(loss_name))
 
-        input_pointpreds=tf.keras.Input((nreas, 1),dtype='float32')
+        input_pointpreds=tf.keras.Input((nreas, 1),dtype=dtype)
         inputs.append(input_pointpreds)
         if use_mask & ~use_caseweights:
-            #input_mask = tf.keras.Input(input_shape,dtype='float32')
-            input_mask = tf.keras.Input((nreas,1),dtype='float32')
+            #input_mask = tf.keras.Input(input_shape,dtype=dtype)
+            input_mask = tf.keras.Input((nreas,1),dtype=dtype)
             inputs.append(input_mask)
             loss_func =loss_functions.mswb( inputs[1], x, inputs[2], mask=inputs[3])
         elif use_mask & use_caseweights:
-            input_mask = tf.keras.Input((nreas,1),dtype='float32'); inputs.append(input_mask)
-            input_caseweights = tf.keras.Input((1,1),dtype='float32'); inputs.append(input_caseweights)
+            input_mask = tf.keras.Input((nreas,1),dtype=dtype); inputs.append(input_mask)
+            input_caseweights = tf.keras.Input((1,1),dtype=dtype); inputs.append(input_caseweights)
             loss_func =loss_functions.msb( inputs[1], x, inputs[2], mask=inputs[3], caseweights=inputs[4])
         else:
             loss_func =loss_functions.mswb( inputs[1], x, inputs[2])
 
     if lamb is not None: logger.info("Using lambda %.3f"%(lamb))
     if loss_name == 'mswb_lagrange1':
         logger.info("Using %s"%(loss_name))
-        input_pointpreds=tf.keras.Input((nreas, 1),dtype='float32')
+        input_pointpreds=tf.keras.Input((nreas, 1),dtype=dtype)
         inputs.append(input_pointpreds)
         if use_mask:
-            input_mask = tf.keras.Input((nreas,1),dtype='float32')
+            input_mask = tf.keras.Input((nreas,1),dtype=dtype)
             inputs.append(input_mask)
             loss_func =loss_functions.mswb_lagrange1( inputs[1], x, inputs[2], mask=inputs[3], lamb=lamb)
         else:
             loss_func =loss_functions.mswb_lagrange1( inputs[1], x, inputs[2], lamb=lamb)
     if loss_name == 'mswb_lagrange2':
         logger.info("Using %s"%(loss_name))
-        input_pointpreds=tf.keras.Input((nreas, 1),dtype='float32')
+        input_pointpreds=tf.keras.Input((nreas, 1),dtype=dtype)
         inputs.append(input_pointpreds)
         if use_mask:
-            input_mask = tf.keras.Input((nreas,1),dtype='float32')
+            input_mask = tf.keras.Input((nreas,1),dtype=dtype)
             inputs.append(input_mask)
             loss_func =loss_functions.mswb_lagrange2( inputs[1], x, inputs[2], mask=inputs[3], lamb=lamb)
         else:
             loss_func =loss_functions.mswb_lagrange2( inputs[1], x, inputs[2], lamb=lamb)
 
     # Adding loss function is problematic when trying multiprocessing
 
@@ -166,26 +169,32 @@
     
     logger.debug("Loss function successfully added to the the model")
     
     return model
 
 
 #two concatenated networks
-def create_mw_model(input_shape_w=None, hidden_sizes_w=(5,5), layer_w=layer.TfbilacLayer, activation_w='sigmoid', out_activation_w=None, input_shape_m=None, hidden_sizes_m=(5,5), layer_m=layer.TfbilacLayer, activation_m='sigmoid', out_activation_m='sigmoid', loss_name='mswcb', use_mask=True, lamb=None ):
+def create_mw_model(input_shape_w=None, hidden_sizes_w=(5,5), layer_w=layer.TfbilacLayer, activation_w='sigmoid', out_activation_w=None, input_shape_m=None, hidden_sizes_m=(5,5), layer_m=layer.TfbilacLayer, activation_m='sigmoid', out_activation_m='sigmoid', loss_name='mswcb', use_mask=True, lamb=None, dtype='float32' ):
 
     import tensorflow as tf
     tf.keras.backend.clear_session()
+    from . import loss_functions
+    if dtype=='float32':
+        loss_functions.PRECISION=tf.float32
+    if dtype=='float16':
+        loss_functions.PRECISION=tf.float16 
+
     nreas_w = input_shape_w[0]; nreas_m = input_shape_m[0]
     nfeas_w = input_shape_w[1]; nreas_m = input_shape_m[0]
     assert nreas_w ==nreas_m
     
-    input_fea_w=tf.keras.Input(input_shape_w,dtype='float32') #feats for training the weights part
-    input_fea_m=tf.keras.Input(input_shape_m,dtype='float32') #feats for training the multiplicative bias
-    input_tar=tf.keras.Input((1, 1),dtype='float32') #targets trug1
-    input_pointpreds=tf.keras.Input((nreas_w, 1),dtype='float32') # point predicion by point NN
+    input_fea_w=tf.keras.Input(input_shape_w,dtype=dtype) #feats for training the weights part
+    input_fea_m=tf.keras.Input(input_shape_m,dtype=dtype) #feats for training the multiplicative bias
+    input_tar=tf.keras.Input((1, 1),dtype=dtype) #targets trug1
+    input_pointpreds=tf.keras.Input((nreas_w, 1),dtype=dtype) # point predicion by point NN
 
     inputs=[input_fea_w, input_fea_m,input_tar, input_pointpreds] 
 
     model_w=get_model(hidden_sizes=hidden_sizes_w, activation=activation_w, layer=layer_w)
 
     shift=False; shiftval=1.0
     if out_activation_w is None:
@@ -208,43 +217,43 @@
     
     x=model_w(inputs[0])
     y=model_m(inputs[1])
 
     if loss_name == 'mswcb':
         logger.info("Using %s"%(loss_name))
         if use_mask:
-            input_mask = tf.keras.Input((nreas_w,1),dtype='float32')
+            input_mask = tf.keras.Input((nreas_w,1),dtype=dtype)
             inputs.append(input_mask)
             loss_func =loss_functions.mswcb( inputs[2], x, y, inputs[3], mask=inputs[4])
         else:
             loss_func =loss_functions.mswcb( inputs[2], x, y, inputs[3])
 
     if loss_name=='mswrb':
         logger.info("Using %s"%(loss_name))
         if use_mask:
-            input_mask = tf.keras.Input((nreas_w,1),dtype='float32')
+            input_mask = tf.keras.Input((nreas_w,1),dtype=dtype)
             inputs.append(input_mask)
             loss_func =loss_functions.mswrb( inputs[2], x, y, inputs[3], mask=inputs[4])
         else:
             loss_func =loss_functions.mswrb( inputs[2], x, y, inputs[3])
 
 
     if lamb is not None: logger.info("Using lambda %.3f"%(lamb))
     if loss_name == 'mswcb_lagrange1':
         logger.info("Using %s"%(loss_name))
         if use_mask:
-            input_mask = tf.keras.Input((nreas_w,1),dtype='float32')
+            input_mask = tf.keras.Input((nreas_w,1),dtype=dtype)
             inputs.append(input_mask)
             loss_func =loss_functions.mswcb_lagrange1( inputs[2], x, y, inputs[3], mask=inputs[4], lamb=lamb)
         else:
             loss_func =loss_functions.mswcb_lagrange1( inputs[2], x, y, inputs[3], lamb=lamb)
     if loss_name == 'mswcb_lagrange2':
         logger.info("Using %s"%(loss_name))
         if use_mask:
-            input_mask = tf.keras.Input((nreas_w,1),dtype='float32')
+            input_mask = tf.keras.Input((nreas_w,1),dtype=dtype)
             inputs.append(input_mask)
             loss_func =loss_functions.mswcb_lagrange2( inputs[2], x, y, inputs[3], mask=inputs[4], lamb=lamb)
         else:
             loss_func =loss_functions.mswcb_lagrange2( inputs[2], x, y, inputs[3], lamb=lamb)
     
     #concatenation would be needed if I wanted to build another loss function in terms of m and w
     # For instance, to use m as a feature of w, i.e, large m should have small weights
@@ -253,27 +262,33 @@
     full_model = tf.keras.Model(inputs=inputs, outputs=[x,y])
     full_model.add_loss(loss_func)
     return full_model
 
 
 
 # PROBABILITY NETWORKS 
-def create_probabilistic_model_independentnormal(input_shape=None, hidden_sizes=(5,5), layer=layer.TfbilacLayer, activation='sigmoid', out_activation=None, loss_name='nll', use_mask=False, use_caseweights=False, lamb=None ):
+def create_probabilistic_model_independentnormal(input_shape=None, hidden_sizes=(5,5), layer=layer.TfbilacLayer, activation='sigmoid', out_activation=None, loss_name='nll', use_mask=False, use_caseweights=False, lamb=None, dtype='float32' ):
     import tensorflow as tf
     import tensorflow_probability as tfp
     tf.keras.backend.clear_session()
+    from . import loss_functions
+    if dtype=='float32':
+        loss_functions.PRECISION=tf.float32
+    if dtype=='float16':
+        loss_functions.PRECISION=tf.float16 
+    
     if input_shape is not None:
         nreas = input_shape[0]
         nfeas = input_shape[1]
     else:
         nreas=None
         nfeas=None
         input_shape=(nreas,nfeas)
-    input_fea=tf.keras.Input(input_shape,dtype='float32') #feat
-    input_tar=tf.keras.Input((1, 1),dtype='float32') #targets
+    input_fea=tf.keras.Input(input_shape,dtype=dtype) #feat
+    input_tar=tf.keras.Input((1, 1),dtype=dtype) #targets
     inputs= [input_fea,input_tar]
     
     model = get_model(hidden_sizes=hidden_sizes, activation=activation, layer=layer, outnodes=0)
     shift=False; shiftval=1.0
 
     #give the mean and the standard deviation
     distribution_params = tf.keras.layers.Dense(units=2)(model(inputs[0]))
@@ -288,15 +303,15 @@
     
     x = tfp.layers.IndependentNormal(1)(pars)
     #x = tfp.layers.IndependentNormal(1)(distribution_params)
     
     if loss_name == 'nll':
         logger.info("Using %s"%(loss_name))
         if use_mask:
-            input_mask = tf.keras.Input((nreas,1),dtype='float32')
+            input_mask = tf.keras.Input((nreas,1),dtype=dtype)
             inputs.append(input_mask)
             loss_func =loss_functions.nll( inputs[1], x, mask=inputs[2])
         else:
             loss_func=loss_functions.nll( inputs[1], x)
 
     # Adding loss function is problematic when trying multiprocessing
     logger.debug("Trying to add model to loss function")
@@ -304,27 +319,33 @@
     model.add_loss(loss_func)
     
     logger.debug("Loss function successfully added to the the model")
     #model.compile(loss=None, optimizer=tf.keras.optimizers.Adam(learning_rate=0.01), metrics = [])
     return model
 
 
-def create_probabilistic_model_mixturenormal(input_shape=None, hidden_sizes=(5,5), layer=layer.TfbilacLayer, activation='sigmoid', out_activation=None, loss_name='nll', ncomp=1, use_mask=False, use_caseweights=False, lamb=None ):
+def create_probabilistic_model_mixturenormal(input_shape=None, hidden_sizes=(5,5), layer=layer.TfbilacLayer, activation='sigmoid', out_activation=None, loss_name='nll', ncomp=1, use_mask=False, use_caseweights=False, lamb=None, dtype='float32' ):
     import tensorflow as tf
     import tensorflow_probability as tfp
     tf.keras.backend.clear_session()
+    from . import loss_functions
+    if dtype=='float32':
+        loss_functions.PRECISION=tf.float32
+    if dtype=='float16':
+        loss_functions.PRECISION=tf.float16
+        
     if input_shape is not None:
         nreas = input_shape[0]
         nfeas = input_shape[1]
     else:
         nreas=None
         nfeas=None
         input_shape=(nreas,nfeas)
-    input_fea=tf.keras.Input(input_shape,dtype='float32') #feat
-    input_tar=tf.keras.Input((1, 1),dtype='float32') #targets
+    input_fea=tf.keras.Input(input_shape,dtype=dtype) #feat
+    input_tar=tf.keras.Input((1, 1),dtype=dtype) #targets
     inputs= [input_fea,input_tar]
     
     model = get_model(hidden_sizes=hidden_sizes, activation=activation, layer=layer, outnodes=0)
     shift=False; shiftval=1.0
 
     #give the mean and the standard deviation
     distribution_params = tf.keras.layers.Dense(units=ncomp*3)(model(inputs[0]))
@@ -345,15 +366,15 @@
     #pars=distribution_params
     
     x = tfp.layers.MixtureNormal(ncomp)(pars)
 
     if loss_name == 'nll':
         logger.info("Using %s"%(loss_name))
         if use_mask:
-            input_mask = tf.keras.Input((nreas,1),dtype='float32')
+            input_mask = tf.keras.Input((nreas,1),dtype=dtype)
             inputs.append(input_mask)
             loss_func =loss_functions.nll( inputs[1], x, mask=inputs[2])
         else:
             loss_func=loss_functions.nll( inputs[1], x)
 
     # Adding loss function is problematic when trying multiprocessing
     logger.debug("Trying to add model to loss function")
@@ -467,26 +488,32 @@
 
     # And the output layer, without activation:
     lay=tfp.layers.DenseVariational(units=1, make_prior_fn= prior,make_posterior_fn=posterior )
     model.add(lay)
     
     return model
 
-def create_bayesian_model(input_shape=None, hidden_sizes=(5,5),  activation='sigmoid', out_activation=None, loss_name='msb', use_mask=False,use_caseweights=False, lamb=None, kl_weight=None):
+def create_bayesian_model(input_shape=None, hidden_sizes=(5,5),  activation='sigmoid', out_activation=None, loss_name='msb', use_mask=False,use_caseweights=False, lamb=None, kl_weight=None, dtype='float32'):
     import tensorflow as tf
+    from . import loss_functions
+    if dtype=='float32':
+        loss_functions.PRECISION=tf.float32
+    if dtype=='float16':
+        loss_functions.PRECISION=tf.float16
+        
     tf.keras.backend.clear_session()
     if input_shape is not None:
         nreas = input_shape[0]
         nfeas = input_shape[1]
     else:
         nreas=None
         nfeas=None
         input_shape=(nreas,nfeas)
-    input_fea=tf.keras.Input(input_shape,dtype='float32') #feat
-    input_tar=tf.keras.Input((1, 1),dtype='float32') #targets
+    input_fea=tf.keras.Input(input_shape,dtype=dtype) #feat
+    input_tar=tf.keras.Input((1, 1),dtype=dtype) #targets
     inputs= [input_fea,input_tar]
     
     model = get_bayesian_model(hidden_sizes=hidden_sizes, activation=activation, kl_weight=kl_weight)
     shift=False; shiftval=1.0
 
     
     if out_activation is None:
@@ -512,81 +539,81 @@
     
     #distribution_params = tf.keras.layers.Dense(units=2)(x)
     #x = tfp.layers.IndependentNormal(1)(distribution_params)
 
     if loss_name == 'mse':
         logger.info("Using %s"%(loss_name))
         if use_mask:
-            input_mask = tf.keras.Input((nreas,1),dtype='float32')
+            input_mask = tf.keras.Input((nreas,1),dtype=dtype)
             inputs.append(input_mask)
             loss_func =loss_functions.mse( inputs[1], x, mask=inputs[2])
         else:
             loss_func=loss_functions.mse( inputs[1], x)
     
 
     if loss_name == 'msb':
         logger.info("Using %s"%(loss_name))
         if use_mask&(~use_caseweights):
-            #input_mask = tf.keras.Input(input_shape,dtype='float32')
-            input_mask = tf.keras.Input((nreas,1),dtype='float32')
+            #input_mask = tf.keras.Input(input_shape,dtype=dtype)
+            input_mask = tf.keras.Input((nreas,1),dtype=dtype)
             inputs.append(input_mask)
             loss_func =loss_functions.msb( inputs[1], x, mask=inputs[2])
         elif use_mask&use_caseweights:
-            input_mask = tf.keras.Input((nreas,1),dtype='float32'); inputs.append(input_mask)
-            input_caseweights = tf.keras.Input((1,1),dtype='float32'); inputs.append(input_caseweights)
+            input_mask = tf.keras.Input((nreas,1),dtype=dtype); inputs.append(input_mask)
+            input_caseweights = tf.keras.Input((1,1),dtype=dtype); inputs.append(input_caseweights)
             loss_func =loss_functions.msb( inputs[1], x, mask=inputs[2], caseweights=inputs[3])
         else:
             loss_func=loss_functions.msb( inputs[1], x)
 
     if loss_name == 'msmb':
         logger.info("Using %s"%(loss_name))
 
-        input_pointpreds=tf.keras.Input((nreas, 1),dtype='float32')
+        input_pointpreds=tf.keras.Input((nreas, 1),dtype=dtype)
         inputs.append(input_pointpreds)
         if use_mask:
-            input_mask = tf.keras.Input((nreas,1),dtype='float32')
+            input_mask = tf.keras.Input((nreas,1),dtype=dtype)
             inputs.append(input_mask)
             loss_func =loss_functions.msmb( inputs[1], x, inputs[2], mask=inputs[3])
         else:
             loss_func =loss_functions.msmb( inputs[1], x, inputs[2])
             
     if loss_name == 'mswb':
         logger.info("Using %s"%(loss_name))
 
-        input_pointpreds=tf.keras.Input((nreas, 1),dtype='float32')
+        input_pointpreds=tf.keras.Input((nreas, 1),dtype=dtype)
         inputs.append(input_pointpreds)
         if use_mask & ~use_caseweights:
-            #input_mask = tf.keras.Input(input_shape,dtype='float32')
-            input_mask = tf.keras.Input((nreas,1),dtype='float32')
+            #input_mask = tf.keras.Input(input_shape,dtype=dtype)
+            input_mask = tf.keras.Input((nreas,1),dtype=dtype)
             inputs.append(input_mask)
             loss_func =loss_functions.mswb( inputs[1], x, inputs[2], mask=inputs[3])
         elif use_mask & use_caseweights:
-            input_mask = tf.keras.Input((nreas,1),dtype='float32'); inputs.append(input_mask)
-            input_caseweights = tf.keras.Input((1,1),dtype='float32'); inputs.append(input_caseweights)
+            input_mask = tf.keras.Input((nreas,1),dtype=dtype); inputs.append(input_mask)
+            input_caseweights = tf.keras.Input((1,1),dtype=dtype); inputs.append(input_caseweights)
             loss_func =loss_functions.msb( inputs[1], x, inputs[2], mask=inputs[3], caseweights=inputs[4])
         else:
             loss_func =loss_functions.mswb( inputs[1], x, inputs[2])
 
     if lamb is not None: logger.info("Using lambda %.3f"%(lamb))
     if loss_name == 'mswb_lagrange1':
         logger.info("Using %s"%(loss_name))
-        input_pointpreds=tf.keras.Input((nreas, 1),dtype='float32')
+        input_pointpreds=tf.keras.Input((nreas, 1),dtype=dtype)
         inputs.append(input_pointpreds)
         if use_mask:
-            input_mask = tf.keras.Input((nreas,1),dtype='float32')
+            input_mask = tf.keras.Input((nreas,1),dtype=dtype)
             inputs.append(input_mask)
             loss_func =loss_functions.mswb_lagrange1( inputs[1], x, inputs[2], mask=inputs[3], lamb=lamb)
         else:
             loss_func =loss_functions.mswb_lagrange1( inputs[1], x, inputs[2], lamb=lamb)
     if loss_name == 'mswb_lagrange2':
         logger.info("Using %s"%(loss_name))
-        input_pointpreds=tf.keras.Input((nreas, 1),dtype='float32')
+        input_pointpreds=tf.keras.Input((nreas, 1),dtype=dtype)
         inputs.append(input_pointpreds)
         if use_mask:
-            input_mask = tf.keras.Input((nreas,1),dtype='float32')
+            input_mask = tf.keras.Input((nreas,1),dtype=dtype)
             inputs.append(input_mask)
             loss_func =loss_functions.mswb_lagrange2( inputs[1], x, inputs[2], mask=inputs[3], lamb=lamb)
         else:
             loss_func =loss_functions.mswb_lagrange2( inputs[1], x, inputs[2], lamb=lamb)
 
 
     # Adding loss function is problematic when trying multiprocessing
```

### Comparing `MLTF-0.1/python/MLTF/calc.py` & `MLTF-0.1.1/python/MLTF/calc.py`

 * *Files identical despite different names*

