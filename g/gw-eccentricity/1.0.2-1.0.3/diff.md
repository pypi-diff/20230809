# Comparing `tmp/gw_eccentricity-1.0.2.tar.gz` & `tmp/gw_eccentricity-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gw_eccentricity-1.0.2.tar", last modified: Mon Jun 19 13:15:28 2023, max compression
+gzip compressed data, was "gw_eccentricity-1.0.3.tar", last modified: Wed Aug  9 02:01:19 2023, max compression
```

## Comparing `gw_eccentricity-1.0.2.tar` & `gw_eccentricity-1.0.3.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 arif      (1000) arif      (1000)        0 2023-06-19 13:15:28.916770 gw_eccentricity-1.0.2/
--rw-r--r--   0 arif      (1000) arif      (1000)     1084 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.2/LICENSE
--rw-r--r--   0 arif      (1000) arif      (1000)     4390 2023-06-19 13:15:28.916770 gw_eccentricity-1.0.2/PKG-INFO
--rw-r--r--   0 arif      (1000) arif      (1000)     3638 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.2/README.md
-drwxr-xr-x   0 arif      (1000) arif      (1000)        0 2023-06-19 13:15:28.870770 gw_eccentricity-1.0.2/gw_eccentricity/
--rw-r--r--   0 arif      (1000) arif      (1000)      435 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.2/gw_eccentricity/__init__.py
--rw-r--r--   0 arif      (1000) arif      (1000)     4505 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.2/gw_eccentricity/compare_methods.py
--rw-r--r--   0 arif      (1000) arif      (1000)   140682 2023-06-19 06:13:53.000000 gw_eccentricity-1.0.2/gw_eccentricity/eccDefinition.py
--rw-r--r--   0 arif      (1000) arif      (1000)     1884 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.2/gw_eccentricity/eccDefinitionUsingAmplitude.py
--rw-r--r--   0 arif      (1000) arif      (1000)     2545 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.2/gw_eccentricity/eccDefinitionUsingAmplitudeFits.py
--rw-r--r--   0 arif      (1000) arif      (1000)      810 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.2/gw_eccentricity/eccDefinitionUsingFrequency.py
--rw-r--r--   0 arif      (1000) arif      (1000)    47793 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.2/gw_eccentricity/eccDefinitionUsingFrequencyFits.py
--rw-r--r--   0 arif      (1000) arif      (1000)     2184 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.2/gw_eccentricity/eccDefinitionUsingResidualAmplitude.py
--rw-r--r--   0 arif      (1000) arif      (1000)     1294 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.2/gw_eccentricity/eccDefinitionUsingResidualFrequency.py
--rw-r--r--   0 arif      (1000) arif      (1000)    18175 2023-06-19 06:14:17.000000 gw_eccentricity-1.0.2/gw_eccentricity/gw_eccentricity.py
--rw-r--r--   0 arif      (1000) arif      (1000)    49295 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.2/gw_eccentricity/load_data.py
--rw-r--r--   0 arif      (1000) arif      (1000)     6103 2023-06-17 09:38:49.000000 gw_eccentricity-1.0.2/gw_eccentricity/plot_settings.py
--rw-r--r--   0 arif      (1000) arif      (1000)     5299 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.2/gw_eccentricity/truncate_waveform_by_flow.py
--rw-r--r--   0 arif      (1000) arif      (1000)    12416 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.2/gw_eccentricity/utils.py
-drwxr-xr-x   0 arif      (1000) arif      (1000)        0 2023-06-19 13:15:28.871770 gw_eccentricity-1.0.2/gw_eccentricity.egg-info/
--rw-r--r--   0 arif      (1000) arif      (1000)     4390 2023-06-19 13:15:28.000000 gw_eccentricity-1.0.2/gw_eccentricity.egg-info/PKG-INFO
--rw-r--r--   0 arif      (1000) arif      (1000)      930 2023-06-19 13:15:28.000000 gw_eccentricity-1.0.2/gw_eccentricity.egg-info/SOURCES.txt
--rw-r--r--   0 arif      (1000) arif      (1000)        1 2023-06-19 13:15:28.000000 gw_eccentricity-1.0.2/gw_eccentricity.egg-info/dependency_links.txt
--rw-r--r--   0 arif      (1000) arif      (1000)       26 2023-06-19 13:15:28.000000 gw_eccentricity-1.0.2/gw_eccentricity.egg-info/requires.txt
--rw-r--r--   0 arif      (1000) arif      (1000)       16 2023-06-19 13:15:28.000000 gw_eccentricity-1.0.2/gw_eccentricity.egg-info/top_level.txt
--rw-r--r--   0 arif      (1000) arif      (1000)       38 2023-06-19 13:15:28.916770 gw_eccentricity-1.0.2/setup.cfg
--rw-r--r--   0 arif      (1000) arif      (1000)     1393 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.2/setup.py
-drwxr-xr-x   0 arif      (1000) arif      (1000)        0 2023-06-19 13:15:28.915770 gw_eccentricity-1.0.2/test/
--rw-r--r--   0 arif      (1000) arif      (1000)     1524 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.2/test/test_example_notebooks.py
--rw-r--r--   0 arif      (1000) arif      (1000)     2275 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.2/test/test_interface.py
--rw-r--r--   0 arif      (1000) arif      (1000)     9161 2023-06-19 06:13:53.000000 gw_eccentricity-1.0.2/test/test_mks_vs_dimless_units.py
--rw-r--r--   0 arif      (1000) arif      (1000)     2871 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.2/test/test_regression.py
--rw-r--r--   0 arif      (1000) arif      (1000)     2498 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.2/test/test_time_convention.py
+drwxr-xr-x   0 arif      (1000) arif      (1000)        0 2023-08-09 02:01:19.396566 gw_eccentricity-1.0.3/
+-rw-r--r--   0 arif      (1000) arif      (1000)     1084 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.3/LICENSE
+-rw-r--r--   0 arif      (1000) arif      (1000)     4814 2023-08-09 02:01:19.395566 gw_eccentricity-1.0.3/PKG-INFO
+-rw-r--r--   0 arif      (1000) arif      (1000)     4062 2023-07-10 13:50:44.000000 gw_eccentricity-1.0.3/README.md
+drwxr-xr-x   0 arif      (1000) arif      (1000)        0 2023-08-09 02:01:19.394566 gw_eccentricity-1.0.3/gw_eccentricity/
+-rw-r--r--   0 arif      (1000) arif      (1000)      435 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.3/gw_eccentricity/__init__.py
+-rw-r--r--   0 arif      (1000) arif      (1000)     4505 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.3/gw_eccentricity/compare_methods.py
+-rw-r--r--   0 arif      (1000) arif      (1000)   152670 2023-08-09 01:55:57.000000 gw_eccentricity-1.0.3/gw_eccentricity/eccDefinition.py
+-rw-r--r--   0 arif      (1000) arif      (1000)     1884 2023-07-11 01:21:26.000000 gw_eccentricity-1.0.3/gw_eccentricity/eccDefinitionUsingAmplitude.py
+-rw-r--r--   0 arif      (1000) arif      (1000)     2545 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.3/gw_eccentricity/eccDefinitionUsingAmplitudeFits.py
+-rw-r--r--   0 arif      (1000) arif      (1000)      810 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.3/gw_eccentricity/eccDefinitionUsingFrequency.py
+-rw-r--r--   0 arif      (1000) arif      (1000)    47793 2023-07-11 01:21:35.000000 gw_eccentricity-1.0.3/gw_eccentricity/eccDefinitionUsingFrequencyFits.py
+-rw-r--r--   0 arif      (1000) arif      (1000)     2642 2023-08-09 01:55:57.000000 gw_eccentricity-1.0.3/gw_eccentricity/eccDefinitionUsingResidualAmplitude.py
+-rw-r--r--   0 arif      (1000) arif      (1000)     1294 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.3/gw_eccentricity/eccDefinitionUsingResidualFrequency.py
+-rw-r--r--   0 arif      (1000) arif      (1000)    20573 2023-08-09 01:57:08.000000 gw_eccentricity-1.0.3/gw_eccentricity/gw_eccentricity.py
+-rw-r--r--   0 arif      (1000) arif      (1000)    49295 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.3/gw_eccentricity/load_data.py
+-rw-r--r--   0 arif      (1000) arif      (1000)     6103 2023-06-17 09:38:49.000000 gw_eccentricity-1.0.3/gw_eccentricity/plot_settings.py
+-rw-r--r--   0 arif      (1000) arif      (1000)     5299 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.3/gw_eccentricity/truncate_waveform_by_flow.py
+-rw-r--r--   0 arif      (1000) arif      (1000)    12741 2023-08-09 01:55:57.000000 gw_eccentricity-1.0.3/gw_eccentricity/utils.py
+drwxr-xr-x   0 arif      (1000) arif      (1000)        0 2023-08-09 02:01:19.394566 gw_eccentricity-1.0.3/gw_eccentricity.egg-info/
+-rw-r--r--   0 arif      (1000) arif      (1000)     4814 2023-08-09 02:01:19.000000 gw_eccentricity-1.0.3/gw_eccentricity.egg-info/PKG-INFO
+-rw-r--r--   0 arif      (1000) arif      (1000)      952 2023-08-09 02:01:19.000000 gw_eccentricity-1.0.3/gw_eccentricity.egg-info/SOURCES.txt
+-rw-r--r--   0 arif      (1000) arif      (1000)        1 2023-08-09 02:01:19.000000 gw_eccentricity-1.0.3/gw_eccentricity.egg-info/dependency_links.txt
+-rw-r--r--   0 arif      (1000) arif      (1000)       26 2023-08-09 02:01:19.000000 gw_eccentricity-1.0.3/gw_eccentricity.egg-info/requires.txt
+-rw-r--r--   0 arif      (1000) arif      (1000)       16 2023-08-09 02:01:19.000000 gw_eccentricity-1.0.3/gw_eccentricity.egg-info/top_level.txt
+-rw-r--r--   0 arif      (1000) arif      (1000)       38 2023-08-09 02:01:19.396566 gw_eccentricity-1.0.3/setup.cfg
+-rw-r--r--   0 arif      (1000) arif      (1000)     1393 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.3/setup.py
+drwxr-xr-x   0 arif      (1000) arif      (1000)        0 2023-08-09 02:01:19.395566 gw_eccentricity-1.0.3/test/
+-rw-r--r--   0 arif      (1000) arif      (1000)     8948 2023-08-09 01:55:57.000000 gw_eccentricity-1.0.3/test/test_dataDict.py
+-rw-r--r--   0 arif      (1000) arif      (1000)     1524 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.3/test/test_example_notebooks.py
+-rw-r--r--   0 arif      (1000) arif      (1000)     2275 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.3/test/test_interface.py
+-rw-r--r--   0 arif      (1000) arif      (1000)     9161 2023-06-19 06:13:53.000000 gw_eccentricity-1.0.3/test/test_mks_vs_dimless_units.py
+-rw-r--r--   0 arif      (1000) arif      (1000)     2871 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.3/test/test_regression.py
+-rw-r--r--   0 arif      (1000) arif      (1000)     2498 2023-06-16 04:18:38.000000 gw_eccentricity-1.0.3/test/test_time_convention.py
```

### Comparing `gw_eccentricity-1.0.2/LICENSE` & `gw_eccentricity-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.2/PKG-INFO` & `gw_eccentricity-1.0.3/gw_eccentricity.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gw_eccentricity
-Version: 1.0.2
+Name: gw-eccentricity
+Version: 1.0.3
 Summary: Defining eccentricity for gravitational wave astronomy.
 Home-page: https://github.com/vijayvarma392/gw_eccentricity
 Author: Md Arif Shaikh, Vijay Varma, Harald Pfeiffer
 Author-email: arifshaikh.astro@gmail.com, vijay.varma392@gmail.com
 Keywords: black-holes gravitational-waves
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
@@ -20,16 +20,18 @@
 
 <h3 align="center"> Defining eccentricity for gravitational wave astronomy </h4>
 
 <div align="center">
 
 [![github](https://img.shields.io/badge/GitHub-gw_eccentricity-blue.svg)](https://github.com/vijayvarma392/gw_eccentricity)
 [![PyPI version](https://badge.fury.io/py/gw_eccentricity.svg?kill_cache=1)](https://pypi.org/project/gw_eccentricity)
+[![Conda (channel only)](https://img.shields.io/conda/vn/conda-forge/gw_eccentricity)](https://anaconda.org/conda-forge/gw_eccentricity)
 [![license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/vijayvarma392/gw_eccentricity/blob/main/LICENSE)
 [![Build Status](https://github.com/vijayvarma392/gw_eccentricity/actions/workflows/test.yml/badge.svg?kill_cache=1)](https://github.com/vijayvarma392/gw_eccentricity/actions/workflows/test.yml)
+[![Documentation Status](https://readthedocs.org/projects/gw-eccentricity/badge/?version=latest)](https://gw-eccentricity.readthedocs.io/en/latest/?badge=latest)
 
 </div>
 
 # About
 
 **gw_eccentricity** provides methods to measure eccentricity and mean anomaly
 from gravitational waveforms.
@@ -49,14 +51,20 @@
 ## PyPI
 **gw_eccentricity** is available through [PyPI](https://pypi.org/project/gw_eccentricity/):
 
 ```shell
 pip install gw_eccentricity
 ```
 
+## Conda
+**gw_eccentricity** can be installed using `conda` also:
+```shell
+conda install -c conda-forge gw_eccentricity
+```
+
 ## From source
 
 ```shell
 git clone git@github.com:vijayvarma392/gw_eccentricity.git
 cd gw_eccentricity
 python setup.py install
 ```
```

### Comparing `gw_eccentricity-1.0.2/README.md` & `gw_eccentricity-1.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 
 <h3 align="center"> Defining eccentricity for gravitational wave astronomy </h4>
 
 <div align="center">
 
 [![github](https://img.shields.io/badge/GitHub-gw_eccentricity-blue.svg)](https://github.com/vijayvarma392/gw_eccentricity)
 [![PyPI version](https://badge.fury.io/py/gw_eccentricity.svg?kill_cache=1)](https://pypi.org/project/gw_eccentricity)
+[![Conda (channel only)](https://img.shields.io/conda/vn/conda-forge/gw_eccentricity)](https://anaconda.org/conda-forge/gw_eccentricity)
 [![license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/vijayvarma392/gw_eccentricity/blob/main/LICENSE)
 [![Build Status](https://github.com/vijayvarma392/gw_eccentricity/actions/workflows/test.yml/badge.svg?kill_cache=1)](https://github.com/vijayvarma392/gw_eccentricity/actions/workflows/test.yml)
+[![Documentation Status](https://readthedocs.org/projects/gw-eccentricity/badge/?version=latest)](https://gw-eccentricity.readthedocs.io/en/latest/?badge=latest)
 
 </div>
 
 # About
 
 **gw_eccentricity** provides methods to measure eccentricity and mean anomaly
 from gravitational waveforms.
@@ -31,14 +33,20 @@
 ## PyPI
 **gw_eccentricity** is available through [PyPI](https://pypi.org/project/gw_eccentricity/):
 
 ```shell
 pip install gw_eccentricity
 ```
 
+## Conda
+**gw_eccentricity** can be installed using `conda` also:
+```shell
+conda install -c conda-forge gw_eccentricity
+```
+
 ## From source
 
 ```shell
 git clone git@github.com:vijayvarma392/gw_eccentricity.git
 cd gw_eccentricity
 python setup.py install
 ```
```

### Comparing `gw_eccentricity-1.0.2/gw_eccentricity/compare_methods.py` & `gw_eccentricity-1.0.3/gw_eccentricity/compare_methods.py`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.2/gw_eccentricity/eccDefinition.py` & `gw_eccentricity-1.0.3/gw_eccentricity/eccDefinition.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,65 +13,118 @@
 from .utils import interpolate
 from .utils import get_interpolant
 from .utils import get_default_spline_kwargs
 from .utils import debug_message
 from .plot_settings import use_fancy_plotsettings, colorsDict, labelsDict
 from .plot_settings import figWidthsTwoColDict, figHeightsDict
 import matplotlib.pyplot as plt
-import copy
 
 
 class eccDefinition:
     """Base class to define eccentricity for given waveform data dictionary."""
 
     def __init__(self, dataDict, num_orbits_to_exclude_before_merger=2,
                  extra_kwargs=None):
         """Init eccDefinition class.
 
         parameters:
         ---------
         dataDict: dict
             Dictionary containing waveform modes dict, time etc. Should follow
-            the format:
+            the format::
+
             dataDict = {"t": time,
                         "hlm": modeDict,
+                        "amplm": ampDict,
+                        "phaselm": phaseDict,
+                        "omegalm": omegaDict,
                         "t_zeroecc": time,
                         "hlm_zeroecc": modeDict,
-                       },
-            "t" and "hlm" are mandatory. "t_zeroecc" and "hlm_zeroecc"
-            are only required for `ResidualAmplitude` and
-            `ResidualFrequency` methods, but if provided, they are
-            used for additional diagnostic plots, which can be helpful
-            for all methods. Any other keys in dataDict will be
+                        "amplm_zeroecc": ampDict,
+                        "phaselm_zeroecc": phaseDict,
+                        "omegalm_zeroecc": omegaDict,
+                       }
+
+            "t" and one of the following is mandatory:
+
+            1. "hlm" OR
+            2. "amplm" and "phaselm"
+                but not both 1 and 2 at the same time.
+
+            Apart from specifying "hlm" or "amplm" and "phaselm", the user can
+            also provide "omegalm". If the "omegalm" key is not explicitly
+            provided, it is computed from the given "hlm" or "phaselm" using
+            finite difference method.
+
+            The keys with suffix "zeroecc" are only required for
+            `ResidualAmplitude` and `ResidualFrequency` methods, where
+            "t_zeroecc" and one of the following is to be provided:
+
+            1. "hlm_zeroecc" OR
+            2. "amplm_zeroecc" and "phaselm_zeroecc"
+               but not both 1 and 2 at the same time.
+
+            Similar to "omegalm", the user can also provide "omegalm_zeroecc".
+            If it is not provided in `dataDict`, it is computed from the given
+            "hlm_zeroecc" or "phaselm_zeroecc" using finite difference method.
+
+            If zeroecc data are provided for methods other than
+            `ResidualAmplitude` and `ResidualFrequency`, they are used for
+            additional diagnostic plots, which can be helpful for all
+            methods.
+
+            Any keys in `dataDict` other than the recognized ones will be
             ignored, with a warning.
 
             The recognized keys are:
+
             - "t": 1d array of times.
-                - Should be uniformly sampled, with a small enough time step
-                  so that omega22(t) can be accurately computed. We use a
-                  4th-order finite difference scheme. In dimensionless units,
-                  we recommend a time step of dtM = 0.1M to be conservative,
-                  but one may be able to get away with larger time steps like
-                  dtM = 1M. The corresponding time step in seconds would be dtM
-                  * M * lal.MTSUN_SI, where M is the total mass in Solar
-                  masses.
+
+                - Should be uniformly sampled, with a small enough time step so
+                  that omega22(t) can be accurately computed, if necessary. We
+                  use a 4th-order finite difference scheme. In dimensionless
+                  units, we recommend a time step of dtM = 0.1M to be
+                  conservative, but one may be able to get away with larger
+                  time steps like dtM = 1M. The corresponding time step in
+                  seconds would be dtM * M * lal.MTSUN_SI, where M is the total
+                  mass in Solar masses.
                 - We do not require the waveform peak amplitude to occur at any
                   specific time, but tref_in should follow the same convention
                   for peak time as "t".
+
             - "hlm": Dictionary of waveform modes associated with "t".
-                - Should have the format:
+                Should have the format::
+
                     modeDict = {(l1, m1): h_{l1, m1},
                                 (l2, m2): h_{l2, m2},
                                 ...
                                },
                     where h_{l, m} is a 1d complex array representing the (l,
                     m) waveform mode. Should contain at least the (2, 2) mode,
                     but more modes can be included, as indicated by the
                     ellipsis '...'  above.
+
+            - "amplm": Dictionary of amplitudes of waveform modes associated
+              with "t". Should have the same format as "hlm", except that the
+              amplitude is real.
+
+            - "phaselm": Dictionary of phases of waveform modes associated
+              with "t". Should have the same format as "hlm", except that the
+              phase is real. The phaselm is related to hlm as hlm = amplm *
+              exp(- i phaselm) ensuring that the phaselm is monotonically
+              increasing for m > 0 modes.
+
+            - "omegalm": Dictionary of the frequencies of the waveform modes
+              associated with "t". Should have the same format as "hlm", except
+              that the omegalm is real. omegalm is related to the phaselm
+              (see above) as omegalm = d/dt phaselm, which means that the
+              omegalm is positive for m > 0 modes.
+
             - "t_zeroecc" and "hlm_zeroecc":
+
                 - Same as above, but for the quasicircular counterpart to the
                   eccentric waveform. The quasicircular counterpart can be
                   obtained by evaluating a waveform model by keeping the rest
                   of the binary parameters fixed (same as the ones used to
                   generate "hlm") but setting the eccentricity to zero. For NR,
                   if such a quasicircular counterpart is not available, we
                   recommend using quasicircular models like NRHybSur3dq8 or
@@ -79,14 +132,18 @@
                 - "t_zeroecc" should be uniformly spaced, but does not have to
                   follow the same time step as that of "t", as long as the step
                   size is small enough to compute the frequency. Similarly,
                   peak time does not have to match that of "t".
                 - We require that "hlm_zeroecc" be at least as long as "hlm" so
                   that residual amplitude/frequency can be computed.
 
+            - "amplm_zeroecc", "phaselm_zeroecc" and "omegalm_zeroecc":
+                Same as "amplm", "phaselm" and "omegalm", respectively, but
+                for the quasicircular counterpart to the eccentric waveform.
+
         num_orbits_to_exclude_before_merger:
                 Can be None or a non negative number.  If None, the full
                 waveform data (even post-merger) is used for finding extrema,
                 but this might cause interpolation issues.  For a non negative
                 num_orbits_to_exclude_before_merger, that many orbits before
                 the merger are excluded when finding extrema.  If your waveform
                 does not have a merger (e.g. PN/EMRI), use
@@ -177,31 +234,29 @@
 
             kwargs_for_fits_methods:
                 Extra kwargs to be passed to FrequencyFits and AmplitudeFits
                 methods. See
                 eccDefinitionUsingFrequencyFits.get_default_kwargs_for_fits_methods
                 for allowed keys.
         """
-        # Truncate dataDict if num_orbits_to_exclude_before_merger is not None
-        self.dataDict, self.t_merger, self.amp22_merger, min_width_for_extrema \
-            = self.truncate_dataDict_if_necessary(
+        # Get data necessary for eccentricity measurement
+        self.dataDict, self.t_merger, self.amp22_merger, \
+            min_width_for_extrema = self.process_data_dict(
                 dataDict, num_orbits_to_exclude_before_merger, extra_kwargs)
         self.t = self.dataDict["t"]
         # check if the time steps are equal, the derivative function
         # requires uniform time steps
         self.t_diff = np.diff(self.t)
         if not np.allclose(self.t_diff, self.t_diff[0]):
             raise Exception("Input time array must have uniform time steps.\n"
                             f"Time steps are {self.t_diff}")
-        self.hlm = self.dataDict["hlm"]
-        self.h22 = self.hlm[(2, 2)]
-        self.amp22 = np.abs(self.h22)
-        self.phase22 = - np.unwrap(np.angle(self.h22))
-        self.omega22 = time_deriv_4thOrder(self.phase22,
-                                           self.t[1] - self.t[0])
+        # get amplitude, phase and omega of 22 mode
+        self.amp22 = self.dataDict["amplm"][(2, 2)]
+        self.phase22 = self.dataDict["phaselm"][(2, 2)]
+        self.omega22 = self.dataDict["omegalm"][(2, 2)]
         # Sanity check various kwargs and set default values
         self.extra_kwargs = check_kwargs_and_set_defaults(
             extra_kwargs, self.get_default_extra_kwargs(),
             "extra_kwargs",
             "eccDefinition.get_default_extra_kwargs()")
         self.extrema_finding_kwargs = check_kwargs_and_set_defaults(
             self.extra_kwargs['extrema_finding_kwargs'],
@@ -247,97 +302,298 @@
         # omega22_average and the associated time array. omega22_average is
         # used to convert a given fref to a tref. If fref is not specified,
         # these will remain as None. However, if get_omega22_average() is
         # called, these get set in that function.
         self.t_for_omega22_average = None
         self.omega22_average = None
 
-        if "hlm_zeroecc" in self.dataDict:
-            self.compute_res_amp_and_omega22()
+        # compute residual data
+        if "amplm_zeroecc" in self.dataDict and "omegalm_zeroecc" in self.dataDict:
+            self.compute_res_amp22_and_res_omega22()
 
     def get_recognized_dataDict_keys(self):
         """Get the list of recognized keys in dataDict."""
         list_of_keys = [
             "t",                # time array of waveform modes
             "hlm",              # Dict of eccentric waveform modes
+            "amplm",            # Dict of amplitude of eccentric waveform modes
+            "phaselm",          # Dict of phase of eccentric waveform modes
+            "omegalm",          # Dict of omega of eccentric waveform modes
             "t_zeroecc",        # time array of quasicircular waveform
             "hlm_zeroecc",      # Dict of quasicircular waveform modes
+            "amplm_zeroecc",    # Dict of amplitude of quasicircular waveform modes
+            "phaselm_zeroecc",  # Dict of phase of quasicircular waveform modes
+            "omegalm_zeroecc",  # Dict of omega of quasicircular waveform modes
         ]
         return list_of_keys
 
-    def truncate_dataDict_if_necessary(self,
-                                       dataDict,
-                                       num_orbits_to_exclude_before_merger,
-                                       extra_kwargs):
-        """Truncate dataDict if "num_orbits_to_exclude_before_merger" is not None.
+    def get_amp_phase_omega_data(self, dataDict):
+        """
+        Extract the dictionary of amplitude, omega, and phase from `dataDict`.
+
+        The `dataDict` provided by the user can contain any of the data
+        corresponding to the keys in `get_recognized_dataDict_keys`. To compute
+        eccentricity and mean anomaly, we need amplitude, phase, and
+        omega. This function extracts these data from `dataDict` and creates a
+        new dictionary containing only the amplitude, phase, and omega of the
+        available modes.
+
+        For example, if `dataDict` contains only the complex hlm modes, this
+        function uses the hlm modes to create a new dictionary containing the
+        amplitude, phase, and omega by decomposing the hlm modes.  Afterwards,
+        only these waveform data in the new dataDict will be used for all
+        further computations.
+
+        Parameters
+        ----------
+        dataDict : dict
+            A dictionary containing waveform data.
+
+        Returns
+        -------
+        amp_phase_omega_dict : dict
+            A new dictionary containing only the amplitude, phase, and omega
+            dict of available modes.
+        """
+        amp_phase_omega_dict = {}
+        # add amplm and amplm_zeroecc if zeroecc data provided
+        amp_phase_omega_dict.update(self.get_amplm_from_dataDict(dataDict))
+        # add phaselm and phaselm_zeroecc if zeroecc data provided
+        amp_phase_omega_dict.update(self.get_phaselm_from_dataDict(dataDict))
+        # add omegalm
+        if "omegalm" in dataDict:
+            amp_phase_omega_dict.update({"omegalm": dataDict["omegalm"]})
+        else:
+            # compute it from phaselm that is already in amp_phase_omega_dict
+            amp_phase_omega_dict.update(
+                {"omegalm": self.get_omegalm_from_phaselm(
+                    dataDict["t"],
+                    amp_phase_omega_dict["phaselm"])})
+
+        # add omegalm_zeroecc if zeroecc data is provided
+        if "omegalm_zeroecc" in dataDict:
+            amp_phase_omega_dict.update(
+                {"omegalm_zeroecc": dataDict["omegalm_zeroecc"]})
+        # Look for zeroecc phaselm is amp_phase_omega_dict and compute
+        # omegalm_zeroecc from it if phaselm_zeroecc is present
+        elif "phaselm_zeroecc" in amp_phase_omega_dict \
+             and "t_zeroecc" in dataDict:
+            amp_phase_omega_dict.update(
+                {"omegalm_zeroecc": self.get_omegalm_from_phaselm(
+                    dataDict["t_zeroecc"],
+                    amp_phase_omega_dict["phaselm_zeroecc"])})
+        return amp_phase_omega_dict
+
+    def get_amplm_from_dataDict(self, dataDict):
+        """Get amplm dict from dataDict.
+
+        Returns the dictionary of amplitudes of waveform modes.
+        """
+        amplm = {}
+        amplm_zeroecc = {}
+        for suffix, ampDict in zip(["", "_zeroecc"], [amplm, amplm_zeroecc]):
+            if "amplm" + suffix in dataDict:
+                # Add the amplitude dictionary from dataDict to ampDict
+                ampDict.update(dataDict["amplm" + suffix])
+            elif "hlm" + suffix in dataDict:
+                # compute amplitude of each hlm mode and add to ampDict
+                for k in dataDict["hlm" + suffix]:
+                    ampDict.update({k: np.abs(dataDict["hlm" + suffix][k])})
+            elif suffix == "":
+                raise Exception("`dataDict` should contain either 'amplm' or "
+                                " 'hlm' for computing amplitude of the "
+                                "waveform modes.")
+        amplmDict = {"amplm": amplm}
+        if amplm_zeroecc:
+            amplmDict.update({"amplm_zeroecc": amplm_zeroecc})
+        return amplmDict
+
+    def get_phaselm_from_dataDict(self, dataDict):
+        """Get phaselm dict from dataDict.
+
+        When the dataDict contains only the complex hlm modes, the phaselm is
+        obtained using the relation hlm = amplm * exp(-i phaselm).
+        """
+        phaselm = {}
+        phaselm_zeroecc = {}
+        for suffix, phaseDict in zip(["", "_zeroecc"],
+                                     [phaselm, phaselm_zeroecc]):
+            if "phaselm" + suffix in dataDict:
+                # Add the phase dictionary from dataDict to phaseDict
+                phaseDict.update(dataDict["phaselm" + suffix])
+            elif "hlm" + suffix in dataDict:
+                # Compute phase of each mode in hlm and add to phaselm
+                for k in dataDict["hlm" + suffix]:
+                    phaseDict.update(
+                        {k: - np.unwrap(
+                            np.angle(dataDict["hlm" + suffix][k]))})
+            elif suffix == "":
+                raise Exception("`dataDict` should contain either 'phaselm' "
+                                "or 'hlm' for computing phase of the waveform "
+                                "modes.")
+        phaselmDict = {"phaselm": phaselm}
+        if phaselm_zeroecc:
+            phaselmDict.update({"phaselm_zeroecc": phaselm_zeroecc})
+        return phaselmDict
+
+    def get_omegalm_from_phaselm(self, t, phaselm):
+        """Get omegalm dict from phaselm dict.
+
+        omegalm is computed using the relation omegalm = d phaselm/dt.
+        """
+        omegalm = phaselm.copy()
+        for mode in phaselm:
+            omegalm[mode] = time_deriv_4thOrder(phaselm[mode], t[1] - t[0])
+        return omegalm
+
+    def process_data_dict(self,
+                          dataDict,
+                          num_orbits_to_exclude_before_merger,
+                          extra_kwargs):
+        """Get necessary data for eccentricity measurement from `dataDict`.
+
+        To measure the eccentricity, several waveform data are required,
+        including:
+
+        - amplitude: Used to locate the merger time from its global maxima and
+          may also be utilized to find the pericenters/apocenters depending on
+          the method.
+        - phase: Helps estimate the time at a given number of orbits before the
+          merger.
+        - omega: Required to compute the frequency at the
+          pericenters/apocenters, which are essential for building the
+          interpolant through them. It may also be used to find the
+          pericenters/apocenters depending on the method.
+
+        These waveform data are also used for various checks and diagnostic
+        plots.
+
+        The `dataDict` provided by the user may contain any of the data
+        mentioned in `get_recognized_dataDict_keys`. From `dataDict`, the
+        amplitude, phase, and omega data are obtained. If
+        `num_orbits_to_exclude_before_merger` is not None, then these data
+        (corresponding to the eccentric waveform) are truncated before
+        returning.
+
+        In addition to the above data, this function returns a few more
+        variables -- `t_merger`, `amp22_merger`, and `min_width_for_extrema`
+        for future usage. See the details below.
 
-        parameters
+        Parameters
         ----------
-        dataDict:
+        dataDict : dict
             Dictionary containing modes and times.
-        num_orbits_to_exclude_before_merger: Number of orbits to exclude before
-            merger to get the truncated dataDict.
+        num_orbits_to_exclude_before_merger : int or None
+            Number of orbits to exclude before the merger to get the truncated
+            dataDict. If None, no truncation is performed.
         extra_kwargs:
-            Extra kwargs passed to the measure eccentricity.
+            Extra keyword arguments passed to the measure eccentricity.
 
         Returns
         -------
-        dataDict:
-            Truncated if num_orbits_to_exclude_before_merger is not None
-            else the unchanged dataDict.
-        t_merger:
+        newDataDict : dict
+            Dictionary containing the amplitude, phase, and omega of the
+            eccentric waveform modes. Includes the same of the zeroecc waveform
+            modes when present in the input `dataDict`. If
+            `num_orbits_to_exclude_before_merger` is not None, then the
+            eccentric data, i.e., amplitude, phase, and omega of the available
+            modes, are truncated before newDataDict is returned.
+        t_merger : float
             Merger time evaluated as the time of the global maximum of
-            amplitude_using_all_modes. This is computed before the truncation.
-        amp22_merger:
+            `amplitude_using_all_modes`. This is computed before the
+            truncation.
+        amp22_merger : float
             Amplitude of the (2, 2) mode at t_merger. This is computed before
             the truncation.
-        min_width_for_extrema:
-            Minimum width for find_peaks function. This is computed before the
-            truncation.
-        """
-        t = dataDict["t"]
-        phase22 = - np.unwrap(np.angle(dataDict["hlm"][(2, 2)]))
+        min_width_for_extrema : float
+            Minimum width for the `find_peaks` function. This is computed
+            before the truncation.
+        """
+        # Test that exactly one of either hlm or (amplm and phaselm) is
+        # provided.
+        # Raise exception if hlm is provided and amplm and/or phaselm is also
+        # provided.
+        for suffix in ["", "_zeroecc"]:
+            if ("hlm"+suffix in dataDict) and any(
+                    ["amplm"+suffix in dataDict,
+                     "phaselm"+suffix in dataDict]):
+                raise Exception(
+                    f"`dataDict` {'should' if suffix == '' else 'may'} "
+                    "contain one of the following: \n"
+                    f"1. 'hlm{suffix}' OR \n"
+                    f"2. 'amplm{suffix}' and 'phaselm{suffix}'\n"
+                    "But not both 1. and 2. at the same time.")
+        # Raise exception if hlm is not provided but either amplm and/or
+        # phaselm is also not provided
+        if ("hlm" not in dataDict) and any(["amplm" not in dataDict,
+                                            "phaselm" not in dataDict]):
+            raise Exception((
+                "`dataDict` should contain one of the following: \n"
+                "1. 'hlm' OR \n"
+                "2. 'amplm' and 'phaselm'\n"
+                "But not both 1. and 2. at the same time."))
+        # Create a new dictionary that will contain the data necessary for
+        # eccentricity measurement.
+        newDataDict = {}
+        if "t" in dataDict:
+            newDataDict.update({"t": dataDict["t"]})
+        else:
+            raise Exception("`dataDict` must contain 't', the times associated"
+                            " with the eccentric waveform data.")
+        # add t_zeroecc if present
+        if "t_zeroecc" in dataDict:
+            newDataDict.update({"t_zeroecc": dataDict["t_zeroecc"]})
+        # From the user dataDict get the amplitude, phase, omega data and add
+        # to newDataDict
+        newDataDict.update(self.get_amp_phase_omega_data(dataDict))
+
+        # Now we compute data using newDataDict and then truncate it if
+        # required.
         # We need to know the merger time of eccentric waveform.
         # This is useful, for example, to subtract the quasi circular
         # amplitude from eccentric amplitude in residual amplitude method
         # We also compute amp22 and phase22 at the merger which are needed
         # to compute location at certain number orbits earlier than merger
         # and to rescale amp22 by it's value at the merger (in AmplitudeFits)
         # respectively.
         t_merger = peak_time_via_quadratic_fit(
-            t,
-            amplitude_using_all_modes(dataDict["hlm"]))[0]
-        merger_idx = np.argmin(np.abs(t - t_merger))
-        amp22_merger = np.abs(dataDict["hlm"][(2, 2)])[merger_idx]
+            newDataDict["t"],
+            amplitude_using_all_modes(newDataDict["amplm"], "amplm"))[0]
+        merger_idx = np.argmin(np.abs(newDataDict["t"] - t_merger))
+        amp22_merger = newDataDict["amplm"][(2, 2)][merger_idx]
+        phase22 = newDataDict["phaselm"][(2, 2)]
         phase22_merger = phase22[merger_idx]
         # Minimum width for peak finding function
         min_width_for_extrema = self.get_width_for_peak_finder_from_phase22(
-            t, phase22, phase22_merger)
+            newDataDict["t"],
+            phase22,
+            phase22_merger)
         if num_orbits_to_exclude_before_merger is not None:
             # Truncate the last num_orbits_to_exclude_before_merger number of
             # orbits before merger.
             # This helps in avoiding non-physical features in the omega22
             # interpolants through the pericenters and the apocenters due
             # to the data being too close to the merger.
             if num_orbits_to_exclude_before_merger < 0:
                 raise ValueError(
                     "num_orbits_to_exclude_before_merger must be non-negative."
                     " Given value was {num_orbits}")
             index_num_orbits_earlier_than_merger \
                 = self.get_index_at_num_orbits_earlier_than_merger(
-                    phase22, phase22_merger,
+                    phase22,
+                    phase22_merger,
                     num_orbits_to_exclude_before_merger)
-            dataDict = copy.deepcopy(dataDict)
-            for mode in dataDict["hlm"]:
-                dataDict["hlm"][mode] \
-                    = dataDict["hlm"][mode][
+            # Truncate amp, phase, omega in eccentric waveform data.
+            for k in ["amplm", "phaselm", "omegalm"]:
+                for mode in newDataDict[k]:
+                    newDataDict[k][mode] = newDataDict[k][mode][
+                        :index_num_orbits_earlier_than_merger]
+                    newDataDict["t"] = newDataDict["t"][
                         :index_num_orbits_earlier_than_merger]
-            dataDict["t"] \
-                = dataDict["t"][:index_num_orbits_earlier_than_merger]
-        return dataDict, t_merger, amp22_merger, min_width_for_extrema
+        return newDataDict, t_merger, amp22_merger, min_width_for_extrema
 
     def get_width_for_peak_finder_from_phase22(self,
                                                t,
                                                phase22,
                                                phase22_merger,
                                                num_orbits_before_merger=2):
         """Get the minimal value of `width` parameter for extrema finding.
@@ -1426,31 +1682,33 @@
             # time differences in t_diff should be positive
             if any(t_diff < 0):
                 debug_message(
                     "There is at least one instance where "
                     "pericenters and apocenters do not appear alternately.",
                     self.debug_level, important=False)
 
-    def compute_res_amp_and_omega22(self):
-        """Compute residual amp22 and omega22."""
-        self.hlm_zeroecc = self.dataDict["hlm_zeroecc"]
+    def compute_res_amp22_and_res_omega22(self):
+        """Compute residual amp22 and residual omega22."""
         self.t_zeroecc = self.dataDict["t_zeroecc"]
         # check that the time steps are equal
         self.t_zeroecc_diff = np.diff(self.t_zeroecc)
         if not np.allclose(self.t_zeroecc_diff, self.t_zeroecc_diff[0]):
             raise Exception(
                 "Input time array t_zeroecc must have uniform time steps\n"
                 f"Time steps are {self.t_zeroecc_diff}")
-        self.h22_zeroecc = self.hlm_zeroecc[(2, 2)]
+        # get amplitude and omega of 22 mode
+        self.amp22_zeroecc = self.dataDict["amplm_zeroecc"][(2, 2)]
+        self.omega22_zeroecc = self.dataDict["omegalm_zeroecc"][(2, 2)]
         # to get the residual amplitude and omega, we need to shift the
         # zeroecc time axis such that the merger of the zeroecc is at the
         # same time as that of the eccentric waveform
+        amp = amplitude_using_all_modes(
+            self.dataDict["amplm_zeroecc"], "amplm")  # total amplitude
         self.t_merger_zeroecc = peak_time_via_quadratic_fit(
-            self.t_zeroecc,
-            amplitude_using_all_modes(self.dataDict["hlm_zeroecc"]))[0]
+            self.t_zeroecc, amp)[0]
         self.t_zeroecc_shifted = (self.t_zeroecc
                                   - self.t_merger_zeroecc
                                   + self.t_merger)
         # check that the length of zeroecc waveform is greater than equal
         # to the length of the eccentric waveform.
         # This is important to satisfy. Otherwise there will be extrapolation
         # when we interpolate zeroecc ecc waveform data on the eccentric
@@ -1469,21 +1727,17 @@
                             f"zeroecc time={self.t_zeroecc_shifted[-1]}")
         # In case the post-merger part of the zeroecc waveform is shorter than
         # that of the the ecc waveform, we allow extrapolation so that the
         # residual quantities can be computed. Above, we check that this
         # extrapolation does not happen before t_merger, which is where
         # eccentricity is normally measured.
         self.amp22_zeroecc_interp = self.interp(
-            self.t, self.t_zeroecc_shifted, np.abs(self.h22_zeroecc),
+            self.t, self.t_zeroecc_shifted, self.amp22_zeroecc,
             allowExtrapolation=True)
         self.res_amp22 = self.amp22 - self.amp22_zeroecc_interp
-
-        self.phase22_zeroecc = - np.unwrap(np.angle(self.h22_zeroecc))
-        self.omega22_zeroecc = time_deriv_4thOrder(
-            self.phase22_zeroecc, self.t_zeroecc[1] - self.t_zeroecc[0])
         self.omega22_zeroecc_interp = self.interp(
             self.t, self.t_zeroecc_shifted, self.omega22_zeroecc,
             allowExtrapolation=True)
         self.res_omega22 = (self.omega22 - self.omega22_zeroecc_interp)
 
     def get_t_average_for_orbit_averaged_omega22(self):
         """Get the times associated with the fref for orbit averaged omega22.
```

### Comparing `gw_eccentricity-1.0.2/gw_eccentricity/eccDefinitionUsingAmplitude.py` & `gw_eccentricity-1.0.3/gw_eccentricity/eccDefinitionUsingAmplitude.py`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.2/gw_eccentricity/eccDefinitionUsingAmplitudeFits.py` & `gw_eccentricity-1.0.3/gw_eccentricity/eccDefinitionUsingAmplitudeFits.py`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.2/gw_eccentricity/eccDefinitionUsingFrequency.py` & `gw_eccentricity-1.0.3/gw_eccentricity/eccDefinitionUsingFrequency.py`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.2/gw_eccentricity/eccDefinitionUsingFrequencyFits.py` & `gw_eccentricity-1.0.3/gw_eccentricity/eccDefinitionUsingFrequencyFits.py`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.2/gw_eccentricity/eccDefinitionUsingResidualAmplitude.py` & `gw_eccentricity-1.0.3/gw_eccentricity/eccDefinitionUsingResidualAmplitude.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,16 +36,24 @@
 
         In the dataDict, these are provided using the keys
         - t_zeroecc: 1d array of times of quasicircular waveform.
         - hlm_zeroecc: Dictionary of modes of the quasicircular waveform.
         For more details on the format of the dataDict, see documentation
         of gw_eccentricity.measure_eccentricity.
         """
-        for k in ["t_zeroecc", "hlm_zeroecc"]:
+        # suggest what data to provide when zeroecc amplitude/omega is missing
+        # for Residual methods
+        suggested_keys = {
+            "t_zeroecc": ["t_zeroecc"],
+            "amplm_zeroecc": ["amplm_zeroecc", "hlm_zeroecc"],
+            "omegalm_zeroecc": ["omegalm_zeroecc", "hlm_zeroecc", "phaselm_zeroecc"]}
+        for k in suggested_keys:
             if k not in self.dataDict:
                 raise Exception(f"Method {method} must have zeroecc data in "
-                                f"dataDict. {k} data not found.")
+                                f"dataDict. {k} data not found. "
+                                "At least one of the following data should be "
+                                f"provided: {suggested_keys[k]}")
 
     def get_data_for_finding_extrema(self):
         """Get the data for extrema finding."""
         self.check_and_raise_zeroecc_data_not_found("ResidualAmplitude")
         return self.res_amp22
```

### Comparing `gw_eccentricity-1.0.2/gw_eccentricity/eccDefinitionUsingResidualFrequency.py` & `gw_eccentricity-1.0.3/gw_eccentricity/eccDefinitionUsingResidualFrequency.py`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.2/gw_eccentricity/gw_eccentricity.py` & `gw_eccentricity-1.0.3/gw_eccentricity/gw_eccentricity.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 See our paper https://arxiv.org/abs/2302.11257 and
 https://pypi.org/project/gw_eccentricity for more details.
 """
 __copyright__ = "Copyright (C) 2023 Md Arif Shaikh, Vijay Varma, Harald Pfeiffer"
 __email__ = "arifshaikh.astro@gmail.com, vijay.varma392@gmail.com"
 __status__ = "testing"
 __author__ = "Md Arif Shaikh, Vijay Varma, Harald Pfeiffer"
-__version__ = "1.0.2"
+__version__ = "1.0.3"
 __license__ = """
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -153,53 +153,100 @@
         ResidualAmplitude/AmplitudeFits/Amplitude
 
     dataDict : dict
         Dictionary containing waveform modes dict, time etc. Should follow the
         format::
 
             dataDict = {"t": time,
-                       "hlm": modeDict,
-                       "t_zeroecc": time,
-                       "hlm_zeroecc": modeDict,
-                       }
-
-        "t" and "hlm" are mandatory. "t_zeroecc" and "hlm_zeroecc" are only
-        required for ResidualAmplitude and ResidualFrequency methods, but if
-        provided, they are used for additional diagnostic plots, which can be
-        helpful for all methods. Any other keys in dataDict will be ignored,
+                        "hlm": modeDict,
+                        "amplm": ampDict,
+                        "phaselm": phaseDict,
+                        "omegalm": omegaDict,
+                        "t_zeroecc": time,
+                        "hlm_zeroecc": modeDict,
+                        "amplm_zeroecc": ampDict,
+                        "phaselm_zeroecc": phaseDict,
+                        "omegalm_zeroecc": omegaDict,
+                      }
+
+        "t" and one of the following is mandatory:
+
+        1. "hlm" OR
+        2. "amplm" and "phaselm"
+            but not both 1 and 2 at the same time.
+
+        Apart from specifying "hlm" or "amplm" and "phaselm", the user can also
+        provide "omegalm". If the "omegalm" key is not explicitly provided, it
+        is computed from the given "hlm" or "phaselm" using finite difference
+        method.
+
+        The keys with suffix "zeroecc" are only required for
+        `ResidualAmplitude` and `ResidualFrequency` methods, where
+        "t_zeroecc" and one of the following is to be provided:
+
+        1. "hlm_zeroecc" OR
+        2. "amplm_zeroecc" and "phaselm_zeroecc"
+            but not both 1 and 2 at the same time.
+
+        Note that providing "hlm_zeroecc" and "amplm_zeroecc" or
+        "phaselm_zeroecc" at the same time will raise error.
+        Similar to "omegalm", the user can also provide "omegalm_zeroecc". If
+        it is not provided in `dataDict`, it is computed from the given
+        "hlm_zeroecc" or "phaselm_zeroecc" using finite difference method.
+
+        If zeroecc data are provided for methods other than `ResidualAmplitude`
+        and `ResidualFrequency`, they are used for additional diagnostic plots,
+        which can be helpful for all methods.
+
+        Any keys in `dataDict` other than the recognized ones will be ignored,
         with a warning.
 
         The recognized keys are:
 
-        - "t" : 1d array of times.
+        - "t": 1d array of times.
 
             - Should be uniformly sampled, with a small enough time step so
-              that omega22(t) can be accurately computed. We use a 4th-order
-              finite difference scheme. In dimensionless units, we recommend a
-              time step of dtM = 0.1M to be conservative, but you may be able
-              to get away with larger time steps like dtM = 1M. The
-              corresponding time step in seconds would be
-              dtM * M * lal.MTSUN_SI, where M is the total mass in Solar
-              masses.
+              that omega22(t) can be accurately computed, if necessary. We use
+              a 4th-order finite difference scheme. In dimensionless units, we
+              recommend a time step of dtM = 0.1M to be conservative, but one
+              may be able to get away with larger time steps like dtM = 1M. The
+              corresponding time step in seconds would be dtM * M *
+              lal.MTSUN_SI, where M is the total mass in Solar masses.
             - We do not require the waveform peak amplitude to occur at any
-              specific time, but tref_in should follow the same convention for
-              peak time as "t".
+              specific time, but tref_in should follow the same convention
+              for peak time as "t".
 
         - "hlm": Dictionary of waveform modes associated with "t".
             Should have the format::
 
                 modeDict = {(l1, m1): h_{l1, m1},
                             (l2, m2): h_{l2, m2},
                             ...
                            }
 
             where h_{l, m} is a 1d complex array representing the (l, m)
-            waveform mode. Should contain at least the (2, 2) mode, but
-            more modes can be included, as indicated by the ellipsis '...'
-            above.
+            waveform mode. Should contain at least the (2, 2) mode, but more
+            modes can be included, as indicated by the ellipsis '...'  above.
+
+        - "amplm": Dictionary of amplitudes of waveform modes associated with
+          "t". Should have the same format as "hlm", except that the amplitude
+          is real.
+
+        - "phaselm": Dictionary of phases of waveform modes associated with
+          "t". Should have the same format as "hlm", except that the phase is
+          real. The phaselm is related to hlm as hlm = amplm * exp(- i phaselm)
+          ensuring that the phaselm is monotonically increasing for m > 0
+          modes.
+
+        - "omegalm": Dictionary of the frequencies of the waveform modes
+          associated with "t". Should have the same format as "hlm", except
+          that the omegalm is real. omegalm is related the phaselm (see above)
+          as omegalm = d/dt phaselm, which means that the omegalm is positive
+          for m > 0 modes.
+
         - "t_zeroecc" and "hlm_zeroecc":
 
             - Same as above, but for the quasicircular counterpart to the
               eccentric waveform. The quasicircular counterpart can be obtained
               by evaluating a waveform model by keeping the rest of the binary
               parameters fixed (same as the ones used to generate "hlm") but
               setting the eccentricity to zero. For NR, if such a quasicircular
@@ -209,14 +256,19 @@
             - "t_zeroecc" should be uniformly spaced, but does not have to
               follow the same time step as that of "t", as long as the step
               size is small enough to compute the frequency. Similarly, peak
               time does not have to match that of "t".
             - We require that "hlm_zeroecc" be at least as long as "hlm" so
               that residual amplitude/frequency can be computed.
 
+        - "amplm_zeroecc", "phaselm_zeroecc" and "omegalm_zeroecc":
+            Same as "amplm", "phaselm" and "omegalm", respectively, but for the
+            quasicircular counterpart to the eccentric waveform.
+
+
     num_orbits_to_exclude_before_merger:
         Can be None or a non negative number.
         If None, the full waveform data (even post-merger) is used for
         finding extrema, but this might cause interpolation issues.
         For a non negative num_orbits_to_exclude_before_merger, that
         many orbits before the merger are excluded when finding extrema.
         If your waveform does not have a merger (e.g. PN/EMRI), use
```

### Comparing `gw_eccentricity-1.0.2/gw_eccentricity/load_data.py` & `gw_eccentricity-1.0.3/gw_eccentricity/load_data.py`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.2/gw_eccentricity/plot_settings.py` & `gw_eccentricity-1.0.3/gw_eccentricity/plot_settings.py`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.2/gw_eccentricity/truncate_waveform_by_flow.py` & `gw_eccentricity-1.0.3/gw_eccentricity/truncate_waveform_by_flow.py`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.2/gw_eccentricity/utils.py` & `gw_eccentricity-1.0.3/gw_eccentricity/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,30 +2,38 @@
 import numpy as np
 import argparse
 from scipy.interpolate import InterpolatedUnivariateSpline
 from scipy.interpolate import PchipInterpolator
 import warnings
 
 
-def amplitude_using_all_modes(mode_dict):
+def amplitude_using_all_modes(mode_dict, data_type="hlm"):
     """Get the amplitude using all the available modes.
 
     Parameters
     ----------
-    mode_dict:
+    mode_dict: dict
         Dictionary containing waveform modes.
+    data_type: str
+        Indicate whether the dictionary contains hlm or amplm.
+        Default is "hlm".
 
     Returns
     -------
         Square root of the qudrature sum of the amplitudes of all the
         available modes in mode_dict.
     """
     amp = 0
     for mode in mode_dict.keys():
-        amp += np.abs(mode_dict[mode])**2
+        if data_type == "hlm":
+            amp += np.abs(mode_dict[mode])**2
+        elif data_type == "amplm":
+            amp += mode_dict[mode]**2
+        else:
+            raise KeyError("data_type must be either `hlm` or `amplm`.")
     return np.sqrt(amp)
 
 
 def peak_time_via_quadratic_fit(t, func):
     """
     Find the peak time of a function quadratically.
```

### Comparing `gw_eccentricity-1.0.2/gw_eccentricity.egg-info/PKG-INFO` & `gw_eccentricity-1.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gw-eccentricity
-Version: 1.0.2
+Name: gw_eccentricity
+Version: 1.0.3
 Summary: Defining eccentricity for gravitational wave astronomy.
 Home-page: https://github.com/vijayvarma392/gw_eccentricity
 Author: Md Arif Shaikh, Vijay Varma, Harald Pfeiffer
 Author-email: arifshaikh.astro@gmail.com, vijay.varma392@gmail.com
 Keywords: black-holes gravitational-waves
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
@@ -20,16 +20,18 @@
 
 <h3 align="center"> Defining eccentricity for gravitational wave astronomy </h4>
 
 <div align="center">
 
 [![github](https://img.shields.io/badge/GitHub-gw_eccentricity-blue.svg)](https://github.com/vijayvarma392/gw_eccentricity)
 [![PyPI version](https://badge.fury.io/py/gw_eccentricity.svg?kill_cache=1)](https://pypi.org/project/gw_eccentricity)
+[![Conda (channel only)](https://img.shields.io/conda/vn/conda-forge/gw_eccentricity)](https://anaconda.org/conda-forge/gw_eccentricity)
 [![license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/vijayvarma392/gw_eccentricity/blob/main/LICENSE)
 [![Build Status](https://github.com/vijayvarma392/gw_eccentricity/actions/workflows/test.yml/badge.svg?kill_cache=1)](https://github.com/vijayvarma392/gw_eccentricity/actions/workflows/test.yml)
+[![Documentation Status](https://readthedocs.org/projects/gw-eccentricity/badge/?version=latest)](https://gw-eccentricity.readthedocs.io/en/latest/?badge=latest)
 
 </div>
 
 # About
 
 **gw_eccentricity** provides methods to measure eccentricity and mean anomaly
 from gravitational waveforms.
@@ -49,14 +51,20 @@
 ## PyPI
 **gw_eccentricity** is available through [PyPI](https://pypi.org/project/gw_eccentricity/):
 
 ```shell
 pip install gw_eccentricity
 ```
 
+## Conda
+**gw_eccentricity** can be installed using `conda` also:
+```shell
+conda install -c conda-forge gw_eccentricity
+```
+
 ## From source
 
 ```shell
 git clone git@github.com:vijayvarma392/gw_eccentricity.git
 cd gw_eccentricity
 python setup.py install
 ```
```

### Comparing `gw_eccentricity-1.0.2/gw_eccentricity.egg-info/SOURCES.txt` & `gw_eccentricity-1.0.3/gw_eccentricity.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -16,12 +16,13 @@
 gw_eccentricity/truncate_waveform_by_flow.py
 gw_eccentricity/utils.py
 gw_eccentricity.egg-info/PKG-INFO
 gw_eccentricity.egg-info/SOURCES.txt
 gw_eccentricity.egg-info/dependency_links.txt
 gw_eccentricity.egg-info/requires.txt
 gw_eccentricity.egg-info/top_level.txt
+test/test_dataDict.py
 test/test_example_notebooks.py
 test/test_interface.py
 test/test_mks_vs_dimless_units.py
 test/test_regression.py
 test/test_time_convention.py
```

### Comparing `gw_eccentricity-1.0.2/setup.py` & `gw_eccentricity-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.2/test/test_example_notebooks.py` & `gw_eccentricity-1.0.3/test/test_example_notebooks.py`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.2/test/test_interface.py` & `gw_eccentricity-1.0.3/test/test_interface.py`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.2/test/test_mks_vs_dimless_units.py` & `gw_eccentricity-1.0.3/test/test_mks_vs_dimless_units.py`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.2/test/test_regression.py` & `gw_eccentricity-1.0.3/test/test_regression.py`

 * *Files identical despite different names*

### Comparing `gw_eccentricity-1.0.2/test/test_time_convention.py` & `gw_eccentricity-1.0.3/test/test_time_convention.py`

 * *Files identical despite different names*

