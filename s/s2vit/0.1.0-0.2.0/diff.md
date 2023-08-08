# Comparing `tmp/s2vit-0.1.0.tar.gz` & `tmp/s2vit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2vit-0.1.0.tar", last modified: Mon Aug  7 14:05:08 2023, max compression
+gzip compressed data, was "s2vit-0.2.0.tar", last modified: Tue Aug  8 22:48:56 2023, max compression
```

## Comparing `s2vit-0.1.0.tar` & `s2vit-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 miller    (1000) miller    (1000)        0 2023-08-07 14:05:08.620372 s2vit-0.1.0/
--rw-rw-r--   0 miller    (1000) miller    (1000)     1070 2023-08-07 13:58:36.000000 s2vit-0.1.0/LICENSE
--rw-rw-r--   0 miller    (1000) miller    (1000)     2093 2023-08-07 14:05:08.620372 s2vit-0.1.0/PKG-INFO
--rw-rw-r--   0 miller    (1000) miller    (1000)     1867 2023-08-07 14:02:12.000000 s2vit-0.1.0/README.md
--rw-rw-r--   0 miller    (1000) miller    (1000)      606 2023-08-07 01:18:08.000000 s2vit-0.1.0/pyproject.toml
-drwxrwxr-x   0 miller    (1000) miller    (1000)        0 2023-08-07 14:05:08.620372 s2vit-0.1.0/requirements/
--rw-rw-r--   0 miller    (1000) miller    (1000)       30 2023-08-06 19:43:34.000000 s2vit-0.1.0/requirements/requirements.in
--rw-rw-r--   0 miller    (1000) miller    (1000)       38 2023-08-07 14:05:08.620372 s2vit-0.1.0/setup.cfg
-drwxrwxr-x   0 miller    (1000) miller    (1000)        0 2023-08-07 14:05:08.620372 s2vit-0.1.0/src/
-drwxrwxr-x   0 miller    (1000) miller    (1000)        0 2023-08-07 14:05:08.620372 s2vit-0.1.0/src/s2vit/
--rw-rw-r--   0 miller    (1000) miller    (1000)      102 2023-08-07 01:18:08.000000 s2vit-0.1.0/src/s2vit/__init__.py
--rw-rw-r--   0 miller    (1000) miller    (1000)      188 2023-08-07 01:18:08.000000 s2vit-0.1.0/src/s2vit/_version.py
--rw-rw-r--   0 miller    (1000) miller    (1000)     4386 2023-08-07 13:52:30.000000 s2vit-0.1.0/src/s2vit/nn.py
--rw-rw-r--   0 miller    (1000) miller    (1000)      308 2023-08-07 01:18:08.000000 s2vit-0.1.0/src/s2vit/nn_test.py
--rw-rw-r--   0 miller    (1000) miller    (1000)     5639 2023-08-07 13:52:30.000000 s2vit-0.1.0/src/s2vit/transformer.py
--rw-rw-r--   0 miller    (1000) miller    (1000)      410 2023-08-07 01:18:08.000000 s2vit-0.1.0/src/s2vit/utils.py
-drwxrwxr-x   0 miller    (1000) miller    (1000)        0 2023-08-07 14:05:08.620372 s2vit-0.1.0/src/s2vit.egg-info/
--rw-rw-r--   0 miller    (1000) miller    (1000)     2093 2023-08-07 14:05:08.000000 s2vit-0.1.0/src/s2vit.egg-info/PKG-INFO
--rw-rw-r--   0 miller    (1000) miller    (1000)      350 2023-08-07 14:05:08.000000 s2vit-0.1.0/src/s2vit.egg-info/SOURCES.txt
--rw-rw-r--   0 miller    (1000) miller    (1000)        1 2023-08-07 14:05:08.000000 s2vit-0.1.0/src/s2vit.egg-info/dependency_links.txt
--rw-rw-r--   0 miller    (1000) miller    (1000)       30 2023-08-07 14:05:08.000000 s2vit-0.1.0/src/s2vit.egg-info/requires.txt
--rw-rw-r--   0 miller    (1000) miller    (1000)        6 2023-08-07 14:05:08.000000 s2vit-0.1.0/src/s2vit.egg-info/top_level.txt
+drwxrwxr-x   0 miller    (1000) miller    (1000)        0 2023-08-08 22:48:56.620265 s2vit-0.2.0/
+-rw-rw-r--   0 miller    (1000) miller    (1000)     1070 2023-08-07 13:58:36.000000 s2vit-0.2.0/LICENSE
+-rw-rw-r--   0 miller    (1000) miller    (1000)     2093 2023-08-08 22:48:56.620265 s2vit-0.2.0/PKG-INFO
+-rw-rw-r--   0 miller    (1000) miller    (1000)     1867 2023-08-07 14:02:12.000000 s2vit-0.2.0/README.md
+-rw-rw-r--   0 miller    (1000) miller    (1000)      606 2023-08-08 22:46:53.000000 s2vit-0.2.0/pyproject.toml
+drwxrwxr-x   0 miller    (1000) miller    (1000)        0 2023-08-08 22:48:56.616265 s2vit-0.2.0/requirements/
+-rw-rw-r--   0 miller    (1000) miller    (1000)       30 2023-08-06 19:43:34.000000 s2vit-0.2.0/requirements/requirements.in
+-rw-rw-r--   0 miller    (1000) miller    (1000)       38 2023-08-08 22:48:56.620265 s2vit-0.2.0/setup.cfg
+drwxrwxr-x   0 miller    (1000) miller    (1000)        0 2023-08-08 22:48:56.616265 s2vit-0.2.0/src/
+drwxrwxr-x   0 miller    (1000) miller    (1000)        0 2023-08-08 22:48:56.616265 s2vit-0.2.0/src/s2vit/
+-rw-rw-r--   0 miller    (1000) miller    (1000)      102 2023-08-07 01:18:08.000000 s2vit-0.2.0/src/s2vit/__init__.py
+-rw-rw-r--   0 miller    (1000) miller    (1000)      188 2023-08-07 01:18:08.000000 s2vit-0.2.0/src/s2vit/_version.py
+-rw-rw-r--   0 miller    (1000) miller    (1000)     4386 2023-08-07 13:52:30.000000 s2vit-0.2.0/src/s2vit/nn.py
+-rw-rw-r--   0 miller    (1000) miller    (1000)      308 2023-08-07 01:18:08.000000 s2vit-0.2.0/src/s2vit/nn_test.py
+-rw-rw-r--   0 miller    (1000) miller    (1000)     5686 2023-08-08 22:46:29.000000 s2vit-0.2.0/src/s2vit/transformer.py
+-rw-rw-r--   0 miller    (1000) miller    (1000)      410 2023-08-07 01:18:08.000000 s2vit-0.2.0/src/s2vit/utils.py
+drwxrwxr-x   0 miller    (1000) miller    (1000)        0 2023-08-08 22:48:56.616265 s2vit-0.2.0/src/s2vit.egg-info/
+-rw-rw-r--   0 miller    (1000) miller    (1000)     2093 2023-08-08 22:48:56.000000 s2vit-0.2.0/src/s2vit.egg-info/PKG-INFO
+-rw-rw-r--   0 miller    (1000) miller    (1000)      350 2023-08-08 22:48:56.000000 s2vit-0.2.0/src/s2vit.egg-info/SOURCES.txt
+-rw-rw-r--   0 miller    (1000) miller    (1000)        1 2023-08-08 22:48:56.000000 s2vit-0.2.0/src/s2vit.egg-info/dependency_links.txt
+-rw-rw-r--   0 miller    (1000) miller    (1000)       30 2023-08-08 22:48:56.000000 s2vit-0.2.0/src/s2vit.egg-info/requires.txt
+-rw-rw-r--   0 miller    (1000) miller    (1000)        6 2023-08-08 22:48:56.000000 s2vit-0.2.0/src/s2vit.egg-info/top_level.txt
```

### Comparing `s2vit-0.1.0/LICENSE` & `s2vit-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `s2vit-0.1.0/PKG-INFO` & `s2vit-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s2vit
-Version: 0.1.0
+Version: 0.2.0
 Summary: Spatial Shift Vision Transformer
 Author-email: Miller Wilt <miller@pyriteai.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Spatial Shift ViT
```

### Comparing `s2vit-0.1.0/README.md` & `s2vit-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `s2vit-0.1.0/pyproject.toml` & `s2vit-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "s2vit"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
     { name = "Miller Wilt", email = "miller@pyriteai.com" },
 ]
 description = "Spatial Shift Vision Transformer"
 readme = "README.md"
 requires-python = ">=3.10"
 dynamic = ["dependencies"]
```

### Comparing `s2vit-0.1.0/src/s2vit/nn.py` & `s2vit-0.2.0/src/s2vit/nn.py`

 * *Files identical despite different names*

### Comparing `s2vit-0.1.0/src/s2vit/transformer.py` & `s2vit-0.2.0/src/s2vit/transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,30 +108,30 @@
         dims: Sequence[int] = (64, 128, 160, 320),
         patch_sizes: Sequence[int | tuple[int, int]] = (4, 2, 2, 2),
         in_channels: int = 3,
         global_pool: bool = False,
         num_classes: int | None = None,
         use_peg: bool = True,
         dim_head: int = 32,
-        block_size: int = 8,
+        block_sizes: Sequence[int] = (8, 8, 8, 8),
         ff_expansions: Sequence[int] = (4, 4, 4, 4),
         norm_layer: Callable[[int], nn.Module] = LayerNormNoBias2d,
         input_norm: Callable[[int], nn.Module] = LayerNormNoBias2d,
         output_norm: Callable[[int], nn.Module] = LayerNormNoBias,
         drop_rate: float = 0.0,
         attn_drop_rate: float = 0.0,
         drop_block_rate: float = 0.0,
         drop_block_size: int = 7,
         bias: bool = False,
     ):
         super().__init__()
 
         stages: list[S2ViTStage] = []
-        for dim_in, dim_out, depth, patch_size, ff_expansion in zip(
-            (in_channels, *dims[:-1]), dims, depths, patch_sizes, ff_expansions, strict=True
+        for dim_in, dim_out, depth, patch_size, block_size, ff_expansion in zip(
+            (in_channels, *dims[:-1]), dims, depths, patch_sizes, block_sizes, ff_expansions, strict=True
         ):
             stage = S2ViTStage(
                 dim_in,
                 dim_out,
                 depth,
                 use_peg=use_peg,
                 patch_size=patch_size,
```

### Comparing `s2vit-0.1.0/src/s2vit.egg-info/PKG-INFO` & `s2vit-0.2.0/src/s2vit.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s2vit
-Version: 0.1.0
+Version: 0.2.0
 Summary: Spatial Shift Vision Transformer
 Author-email: Miller Wilt <miller@pyriteai.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Spatial Shift ViT
```

