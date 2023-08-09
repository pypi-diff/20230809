# Comparing `tmp/allin1-0.0.3.tar.gz` & `tmp/allin1-0.0.4.tar.gz`

## Comparing `allin1-0.0.3.tar` & `allin1-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 allin1-0.0.3/MANIFEST.in
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 allin1-0.0.3/src/allin1/__init__.py
--rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 allin1-0.0.3/src/allin1/cli.py
--rw-r--r--   0        0        0     4128 2020-02-02 00:00:00.000000 allin1-0.0.3/src/allin1/config.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 allin1-0.0.3/src/allin1/demix.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allin1-0.0.3/src/allin1/py.typed
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 allin1-0.0.3/src/allin1/run.py
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 allin1-0.0.3/src/allin1/spectrogram.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 allin1-0.0.3/src/allin1/typings.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 allin1-0.0.3/src/allin1/models/__init__.py
--rw-r--r--   0        0        0     8084 2020-02-02 00:00:00.000000 allin1-0.0.3/src/allin1/models/allinone.py
--rw-r--r--   0        0        0    13952 2020-02-02 00:00:00.000000 allin1-0.0.3/src/allin1/models/dinat.py
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 allin1-0.0.3/src/allin1/models/loaders.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 allin1-0.0.3/src/allin1/models/utils.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 allin1-0.0.3/src/allin1/postprocessing/__init__.py
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 allin1-0.0.3/src/allin1/postprocessing/functional.py
--rw-r--r--   0        0        0     6986 2020-02-02 00:00:00.000000 allin1-0.0.3/src/allin1/postprocessing/helpers.py
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 allin1-0.0.3/src/allin1/postprocessing/metrical.py
--rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 allin1-0.0.3/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 allin1-0.0.3/LICENSE
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 allin1-0.0.3/README.md
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 allin1-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 allin1-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 allin1-0.0.4/MANIFEST.in
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 allin1-0.0.4/src/allin1/__init__.py
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 allin1-0.0.4/src/allin1/cli.py
+-rw-r--r--   0        0        0     4128 2020-02-02 00:00:00.000000 allin1-0.0.4/src/allin1/config.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 allin1-0.0.4/src/allin1/demix.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allin1-0.0.4/src/allin1/py.typed
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 allin1-0.0.4/src/allin1/run.py
+-rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 allin1-0.0.4/src/allin1/spectrogram.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 allin1-0.0.4/src/allin1/typings.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 allin1-0.0.4/src/allin1/models/__init__.py
+-rw-r--r--   0        0        0     8084 2020-02-02 00:00:00.000000 allin1-0.0.4/src/allin1/models/allinone.py
+-rw-r--r--   0        0        0    13952 2020-02-02 00:00:00.000000 allin1-0.0.4/src/allin1/models/dinat.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 allin1-0.0.4/src/allin1/models/loaders.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 allin1-0.0.4/src/allin1/models/utils.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 allin1-0.0.4/src/allin1/postprocessing/__init__.py
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 allin1-0.0.4/src/allin1/postprocessing/functional.py
+-rw-r--r--   0        0        0     6979 2020-02-02 00:00:00.000000 allin1-0.0.4/src/allin1/postprocessing/helpers.py
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 allin1-0.0.4/src/allin1/postprocessing/metrical.py
+-rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 allin1-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 allin1-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 allin1-0.0.4/README.md
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 allin1-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 allin1-0.0.4/PKG-INFO
```

### Comparing `allin1-0.0.3/src/allin1/cli.py` & `allin1-0.0.4/src/allin1/cli.py`

 * *Files identical despite different names*

### Comparing `allin1-0.0.3/src/allin1/config.py` & `allin1-0.0.4/src/allin1/config.py`

 * *Files identical despite different names*

### Comparing `allin1-0.0.3/src/allin1/demix.py` & `allin1-0.0.4/src/allin1/demix.py`

 * *Files identical despite different names*

### Comparing `allin1-0.0.3/src/allin1/run.py` & `allin1-0.0.4/src/allin1/run.py`

 * *Files identical despite different names*

### Comparing `allin1-0.0.3/src/allin1/spectrogram.py` & `allin1-0.0.4/src/allin1/spectrogram.py`

 * *Files identical despite different names*

### Comparing `allin1-0.0.3/src/allin1/typings.py` & `allin1-0.0.4/src/allin1/typings.py`

 * *Files identical despite different names*

### Comparing `allin1-0.0.3/src/allin1/models/allinone.py` & `allin1-0.0.4/src/allin1/models/allinone.py`

 * *Files identical despite different names*

### Comparing `allin1-0.0.3/src/allin1/models/dinat.py` & `allin1-0.0.4/src/allin1/models/dinat.py`

 * *Files identical despite different names*

### Comparing `allin1-0.0.3/src/allin1/models/loaders.py` & `allin1-0.0.4/src/allin1/models/loaders.py`

 * *Files identical despite different names*

### Comparing `allin1-0.0.3/src/allin1/models/utils.py` & `allin1-0.0.4/src/allin1/models/utils.py`

 * *Files identical despite different names*

### Comparing `allin1-0.0.3/src/allin1/postprocessing/functional.py` & `allin1-0.0.4/src/allin1/postprocessing/functional.py`

 * *Files identical despite different names*

### Comparing `allin1-0.0.3/src/allin1/postprocessing/helpers.py` & `allin1-0.0.4/src/allin1/postprocessing/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import torch.nn.functional as F
 import torch
 import librosa
 from scipy.signal import argrelextrema
 from scipy.interpolate import interp1d
 from numpy.lib.stride_tricks import sliding_window_view
 from numpy.typing import NDArray
-from allinone.config import Config
+from ..config import Config
 
 def event_frames_to_time(
   tensor: torch.Tensor | NDArray,
   cfg: Config = None,
   sample_rate: int = None,
   hop_size: int = None,
 ):
```

### Comparing `allin1-0.0.3/src/allin1/postprocessing/metrical.py` & `allin1-0.0.4/src/allin1/postprocessing/metrical.py`

 * *Files identical despite different names*

### Comparing `allin1-0.0.3/.gitignore` & `allin1-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `allin1-0.0.3/LICENSE` & `allin1-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `allin1-0.0.3/README.md` & `allin1-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `allin1-0.0.3/pyproject.toml` & `allin1-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "allin1"
-version = "0.0.3"
+version = "0.0.4"
 description = "All-In-One Metrical and Functional Music Structure Analysis"
 readme = "README.md"
 dependencies = [
   "numpy",
   "madmom",
   "librosa",
   "natten",
```

### Comparing `allin1-0.0.3/PKG-INFO` & `allin1-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allin1
-Version: 0.0.3
+Version: 0.0.4
 Summary: All-In-One Metrical and Functional Music Structure Analysis
 License-File: LICENSE
 Requires-Dist: demucs
 Requires-Dist: huggingface-hub
 Requires-Dist: hydra-core
 Requires-Dist: librosa
 Requires-Dist: madmom
```

