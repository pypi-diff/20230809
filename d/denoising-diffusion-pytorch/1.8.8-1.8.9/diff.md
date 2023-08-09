# Comparing `tmp/denoising-diffusion-pytorch-1.8.8.tar.gz` & `tmp/denoising-diffusion-pytorch-1.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denoising-diffusion-pytorch-1.8.8.tar", last modified: Fri Jul 14 14:35:24 2023, max compression
+gzip compressed data, was "denoising-diffusion-pytorch-1.8.9.tar", last modified: Wed Aug  9 02:52:39 2023, max compression
```

## Comparing `denoising-diffusion-pytorch-1.8.8.tar` & `denoising-diffusion-pytorch-1.8.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:35:24.631085 denoising-diffusion-pytorch-1.8.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-14 14:35:13.000000 denoising-diffusion-pytorch-1.8.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-14 14:35:24.631085 denoising-diffusion-pytorch-1.8.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-07-14 14:35:13.000000 denoising-diffusion-pytorch-1.8.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:35:24.631085 denoising-diffusion-pytorch-1.8.8/denoising_diffusion_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-14 14:35:13.000000 denoising-diffusion-pytorch-1.8.8/denoising_diffusion_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-07-14 14:35:13.000000 denoising-diffusion-pytorch-1.8.8/denoising_diffusion_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    27920 2023-07-14 14:35:13.000000 denoising-diffusion-pytorch-1.8.8/denoising_diffusion_pytorch/classifier_free_guidance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-07-14 14:35:13.000000 denoising-diffusion-pytorch-1.8.8/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    37332 2023-07-14 14:35:13.000000 denoising-diffusion-pytorch-1.8.8/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    30027 2023-07-14 14:35:13.000000 denoising-diffusion-pytorch-1.8.8/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-07-14 14:35:13.000000 denoising-diffusion-pytorch-1.8.8/denoising_diffusion_pytorch/elucidated_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-14 14:35:13.000000 denoising-diffusion-pytorch-1.8.8/denoising_diffusion_pytorch/fid_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    35629 2023-07-14 14:35:13.000000 denoising-diffusion-pytorch-1.8.8/denoising_diffusion_pytorch/guided_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-07-14 14:35:13.000000 denoising-diffusion-pytorch-1.8.8/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    21236 2023-07-14 14:35:13.000000 denoising-diffusion-pytorch-1.8.8/denoising_diffusion_pytorch/simple_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-07-14 14:35:13.000000 denoising-diffusion-pytorch-1.8.8/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 14:35:13.000000 denoising-diffusion-pytorch-1.8.8/denoising_diffusion_pytorch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-14 14:35:13.000000 denoising-diffusion-pytorch-1.8.8/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 14:35:24.631085 denoising-diffusion-pytorch-1.8.8/denoising_diffusion_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-14 14:35:24.000000 denoising-diffusion-pytorch-1.8.8/denoising_diffusion_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-14 14:35:24.000000 denoising-diffusion-pytorch-1.8.8/denoising_diffusion_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 14:35:24.000000 denoising-diffusion-pytorch-1.8.8/denoising_diffusion_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-14 14:35:24.000000 denoising-diffusion-pytorch-1.8.8/denoising_diffusion_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-14 14:35:24.000000 denoising-diffusion-pytorch-1.8.8/denoising_diffusion_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 14:35:24.631085 denoising-diffusion-pytorch-1.8.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-14 14:35:13.000000 denoising-diffusion-pytorch-1.8.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 02:52:39.010712 denoising-diffusion-pytorch-1.8.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-09 02:52:26.000000 denoising-diffusion-pytorch-1.8.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-08-09 02:52:39.010712 denoising-diffusion-pytorch-1.8.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-08-09 02:52:26.000000 denoising-diffusion-pytorch-1.8.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 02:52:39.010712 denoising-diffusion-pytorch-1.8.9/denoising_diffusion_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-08-09 02:52:26.000000 denoising-diffusion-pytorch-1.8.9/denoising_diffusion_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-08-09 02:52:26.000000 denoising-diffusion-pytorch-1.8.9/denoising_diffusion_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27920 2023-08-09 02:52:26.000000 denoising-diffusion-pytorch-1.8.9/denoising_diffusion_pytorch/classifier_free_guidance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-08-09 02:52:26.000000 denoising-diffusion-pytorch-1.8.9/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37381 2023-08-09 02:52:26.000000 denoising-diffusion-pytorch-1.8.9/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30027 2023-08-09 02:52:26.000000 denoising-diffusion-pytorch-1.8.9/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-08-09 02:52:26.000000 denoising-diffusion-pytorch-1.8.9/denoising_diffusion_pytorch/elucidated_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-08-09 02:52:26.000000 denoising-diffusion-pytorch-1.8.9/denoising_diffusion_pytorch/fid_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35629 2023-08-09 02:52:26.000000 denoising-diffusion-pytorch-1.8.9/denoising_diffusion_pytorch/guided_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-08-09 02:52:26.000000 denoising-diffusion-pytorch-1.8.9/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21236 2023-08-09 02:52:26.000000 denoising-diffusion-pytorch-1.8.9/denoising_diffusion_pytorch/simple_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-08-09 02:52:26.000000 denoising-diffusion-pytorch-1.8.9/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-09 02:52:26.000000 denoising-diffusion-pytorch-1.8.9/denoising_diffusion_pytorch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-08-09 02:52:26.000000 denoising-diffusion-pytorch-1.8.9/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 02:52:39.010712 denoising-diffusion-pytorch-1.8.9/denoising_diffusion_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-08-09 02:52:38.000000 denoising-diffusion-pytorch-1.8.9/denoising_diffusion_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-08-09 02:52:38.000000 denoising-diffusion-pytorch-1.8.9/denoising_diffusion_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 02:52:38.000000 denoising-diffusion-pytorch-1.8.9/denoising_diffusion_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-09 02:52:38.000000 denoising-diffusion-pytorch-1.8.9/denoising_diffusion_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-09 02:52:38.000000 denoising-diffusion-pytorch-1.8.9/denoising_diffusion_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-09 02:52:39.014712 denoising-diffusion-pytorch-1.8.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-08-09 02:52:26.000000 denoising-diffusion-pytorch-1.8.9/setup.py
```

### Comparing `denoising-diffusion-pytorch-1.8.8/LICENSE` & `denoising-diffusion-pytorch-1.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.8/PKG-INFO` & `denoising-diffusion-pytorch-1.8.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.8.8
+Version: 1.8.9
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.8.8/README.md` & `denoising-diffusion-pytorch-1.8.9/README.md`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.8/denoising_diffusion_pytorch/__init__.py` & `denoising-diffusion-pytorch-1.8.9/denoising_diffusion_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.8/denoising_diffusion_pytorch/attend.py` & `denoising-diffusion-pytorch-1.8.9/denoising_diffusion_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.8/denoising_diffusion_pytorch/classifier_free_guidance.py` & `denoising-diffusion-pytorch-1.8.9/denoising_diffusion_pytorch/classifier_free_guidance.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.8/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.8.9/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.8/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py` & `denoising-diffusion-pytorch-1.8.9/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -873,14 +873,15 @@
             mixed_precision = mixed_precision_type if amp else 'no'
         )
 
         # model
 
         self.model = diffusion_model
         self.channels = diffusion_model.channels
+        is_ddim_sampling = diffusion_model.is_ddim_sampling
 
         # sampling and training hyperparameters
 
         assert has_int_squareroot(num_samples), 'number of samples must have an integer square root'
         self.num_samples = num_samples
         self.save_and_sample_every = save_and_sample_every
 
@@ -926,15 +927,15 @@
         self.model, self.opt = self.accelerator.prepare(self.model, self.opt)
 
         # FID-score computation
 
         self.calculate_fid = calculate_fid and self.accelerator.is_main_process
 
         if self.calculate_fid:
-            if not self.model.is_ddim_sampling:
+            if not is_ddim_sampling:
                 self.accelerator.print(
                     "WARNING: Robust FID computation requires a lot of generated samples and can therefore be very time consuming."\
                     "Consider using DDIM sampling to save time."
                 )
             self.fid_scorer = FIDEvaluation(
                 batch_size=self.batch_size,
                 dl=self.dl,
```

### Comparing `denoising-diffusion-pytorch-1.8.8/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py` & `denoising-diffusion-pytorch-1.8.9/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.8/denoising_diffusion_pytorch/elucidated_diffusion.py` & `denoising-diffusion-pytorch-1.8.9/denoising_diffusion_pytorch/elucidated_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.8/denoising_diffusion_pytorch/fid_evaluation.py` & `denoising-diffusion-pytorch-1.8.9/denoising_diffusion_pytorch/fid_evaluation.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.8/denoising_diffusion_pytorch/guided_diffusion.py` & `denoising-diffusion-pytorch-1.8.9/denoising_diffusion_pytorch/guided_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.8/denoising_diffusion_pytorch/learned_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.8.9/denoising_diffusion_pytorch/learned_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.8/denoising_diffusion_pytorch/simple_diffusion.py` & `denoising-diffusion-pytorch-1.8.9/denoising_diffusion_pytorch/simple_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.8/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.8.9/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.8/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.8.9/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.8/denoising_diffusion_pytorch.egg-info/PKG-INFO` & `denoising-diffusion-pytorch-1.8.9/denoising_diffusion_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.8.8
+Version: 1.8.9
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.8.8/denoising_diffusion_pytorch.egg-info/SOURCES.txt` & `denoising-diffusion-pytorch-1.8.9/denoising_diffusion_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.8/setup.py` & `denoising-diffusion-pytorch-1.8.9/setup.py`

 * *Files identical despite different names*

