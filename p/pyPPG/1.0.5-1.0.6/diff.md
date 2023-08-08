# Comparing `tmp/pyPPG-1.0.5.tar.gz` & `tmp/pyPPG-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPPG-1.0.5.tar", last modified: Sun Aug  6 10:13:16 2023, max compression
+gzip compressed data, was "pyPPG-1.0.6.tar", last modified: Tue Aug  8 21:37:13 2023, max compression
```

## Comparing `pyPPG-1.0.5.tar` & `pyPPG-1.0.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 10:13:16.383415 pyPPG-1.0.5/
--rw-rw-rw-   0        0        0      105 2023-05-03 11:40:28.000000 pyPPG-1.0.5/AUTHORS.rst
--rw-rw-rw-   0        0        0    35972 2023-07-18 09:12:28.000000 pyPPG-1.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0     4069 2023-08-06 10:13:16.383415 pyPPG-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3448 2023-08-06 10:11:22.000000 pyPPG-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-08-06 10:13:16.369561 pyPPG-1.0.5/pyPPG/
--rw-rw-rw-   0        0        0     3195 2023-07-31 14:17:03.000000 pyPPG-1.0.5/pyPPG/Biomarkers.py
--rw-rw-rw-   0        0        0     9414 2023-07-31 12:37:20.000000 pyPPG-1.0.5/pyPPG/DataHandling.py
--rw-rw-rw-   0        0        0     2206 2023-08-06 08:07:59.000000 pyPPG-1.0.5/pyPPG/EXAMPLE.py
--rw-rw-rw-   0        0        0    49740 2023-07-31 14:17:03.000000 pyPPG-1.0.5/pyPPG/FiducialPoints.py
--rw-rw-rw-   0        0        0     1846 2023-07-31 14:32:01.000000 pyPPG-1.0.5/pyPPG/Preprocessing.py
--rw-rw-rw-   0        0        0     1907 2023-07-31 14:33:15.000000 pyPPG-1.0.5/pyPPG/Statistics.py
--rw-rw-rw-   0        0        0        0 2023-07-23 10:03:08.000000 pyPPG-1.0.5/pyPPG/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-06 10:13:16.379084 pyPPG-1.0.5/pyPPG/pack_ppg/
--rw-rw-rw-   0        0        0      487 2022-11-08 13:38:06.000000 pyPPG-1.0.5/pyPPG/pack_ppg/_ErrorHandler.py
--rw-rw-rw-   0        0        0        0 2023-07-23 10:03:08.000000 pyPPG-1.0.5/pyPPG/pack_ppg/__init__.py
--rw-rw-rw-   0        0        0     4963 2023-07-31 14:33:15.000000 pyPPG-1.0.5/pyPPG/ppgSQI.py
-drwxrwxrwx   0        0        0        0 2023-08-06 10:13:16.382359 pyPPG-1.0.5/pyPPG/ppg_bm/
--rw-rw-rw-   0        0        0        0 2023-07-21 19:27:04.000000 pyPPG-1.0.5/pyPPG/ppg_bm/__init__.py
--rw-rw-rw-   0        0        0    49194 2023-07-26 11:16:42.000000 pyPPG-1.0.5/pyPPG/ppg_bm/get_biomarkers.py
--rw-rw-rw-   0        0        0     4754 2023-07-23 15:47:56.000000 pyPPG-1.0.5/pyPPG/ppg_bm/get_bm_derivs_ratios.py
--rw-rw-rw-   0        0        0     3230 2023-07-23 15:47:56.000000 pyPPG-1.0.5/pyPPG/ppg_bm/get_bm_ppg_derivs.py
--rw-rw-rw-   0        0        0     6086 2023-07-23 15:49:12.000000 pyPPG-1.0.5/pyPPG/ppg_bm/get_bm_ppg_sig.py
--rw-rw-rw-   0        0        0     4313 2023-07-23 15:47:56.000000 pyPPG-1.0.5/pyPPG/ppg_bm/get_bm_sig_ratios.py
-drwxrwxrwx   0        0        0        0 2023-08-06 10:13:16.378141 pyPPG-1.0.5/pyPPG.egg-info/
--rw-rw-rw-   0        0        0     4069 2023-08-06 10:13:16.000000 pyPPG-1.0.5/pyPPG.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      612 2023-08-06 10:13:16.000000 pyPPG-1.0.5/pyPPG.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 10:13:16.000000 pyPPG-1.0.5/pyPPG.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-08-06 10:13:16.000000 pyPPG-1.0.5/pyPPG.egg-info/requires.txt
--rw-rw-rw-   0        0        0       34 2023-08-06 10:13:16.000000 pyPPG-1.0.5/pyPPG.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      190 2023-07-27 13:48:40.000000 pyPPG-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-06 10:13:16.384016 pyPPG-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1079 2023-08-06 10:11:45.000000 pyPPG-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 21:37:13.954845 pyPPG-1.0.6/
+-rw-rw-rw-   0        0        0      105 2023-05-03 11:40:28.000000 pyPPG-1.0.6/AUTHORS.rst
+-rw-rw-rw-   0        0        0    35972 2023-07-18 09:12:28.000000 pyPPG-1.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     4638 2023-08-08 21:37:13.954845 pyPPG-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4017 2023-08-06 13:20:20.000000 pyPPG-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 21:37:13.932827 pyPPG-1.0.6/pyPPG/
+-rw-rw-rw-   0        0        0     3593 2023-08-08 17:27:20.000000 pyPPG-1.0.6/pyPPG/Biomarkers.py
+-rw-rw-rw-   0        0        0    11223 2023-08-08 14:17:10.000000 pyPPG-1.0.6/pyPPG/DataHandling.py
+-rw-rw-rw-   0        0        0     3567 2023-08-08 21:27:20.000000 pyPPG-1.0.6/pyPPG/EXAMPLE.py
+-rw-rw-rw-   0        0        0    49739 2023-08-07 10:37:58.000000 pyPPG-1.0.6/pyPPG/FiducialPoints.py
+-rw-rw-rw-   0        0        0     1846 2023-07-31 14:32:01.000000 pyPPG-1.0.6/pyPPG/Preprocessing.py
+-rw-rw-rw-   0        0        0     1907 2023-07-31 14:33:15.000000 pyPPG-1.0.6/pyPPG/Statistics.py
+-rw-rw-rw-   0        0        0        0 2023-07-23 10:03:08.000000 pyPPG-1.0.6/pyPPG/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 21:37:13.950095 pyPPG-1.0.6/pyPPG/pack_ppg/
+-rw-rw-rw-   0        0        0      487 2022-11-08 13:38:06.000000 pyPPG-1.0.6/pyPPG/pack_ppg/_ErrorHandler.py
+-rw-rw-rw-   0        0        0        0 2023-07-23 10:03:08.000000 pyPPG-1.0.6/pyPPG/pack_ppg/__init__.py
+-rw-rw-rw-   0        0        0     4963 2023-07-31 14:33:15.000000 pyPPG-1.0.6/pyPPG/ppgSQI.py
+drwxrwxrwx   0        0        0        0 2023-08-08 21:37:13.954845 pyPPG-1.0.6/pyPPG/ppg_bm/
+-rw-rw-rw-   0        0        0        0 2023-07-21 19:27:04.000000 pyPPG-1.0.6/pyPPG/ppg_bm/__init__.py
+-rw-rw-rw-   0        0        0    49162 2023-08-08 15:59:12.000000 pyPPG-1.0.6/pyPPG/ppg_bm/biomarker_extractor.py
+-rw-rw-rw-   0        0        0     5213 2023-08-08 17:30:48.000000 pyPPG-1.0.6/pyPPG/ppg_bm/get_bm_derivs_ratios.py
+-rw-rw-rw-   0        0        0     3567 2023-08-08 18:05:34.000000 pyPPG-1.0.6/pyPPG/ppg_bm/get_bm_ppg_derivs.py
+-rw-rw-rw-   0        0        0     6670 2023-08-08 17:35:55.000000 pyPPG-1.0.6/pyPPG/ppg_bm/get_bm_ppg_sig.py
+-rw-rw-rw-   0        0        0     4727 2023-08-08 17:30:48.000000 pyPPG-1.0.6/pyPPG/ppg_bm/get_bm_sig_ratios.py
+drwxrwxrwx   0        0        0        0 2023-08-08 21:37:13.948474 pyPPG-1.0.6/pyPPG.egg-info/
+-rw-rw-rw-   0        0        0     4638 2023-08-08 21:37:13.000000 pyPPG-1.0.6/pyPPG.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      617 2023-08-08 21:37:13.000000 pyPPG-1.0.6/pyPPG.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 21:37:13.000000 pyPPG-1.0.6/pyPPG.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-08-08 21:37:13.000000 pyPPG-1.0.6/pyPPG.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       34 2023-08-08 21:37:13.000000 pyPPG-1.0.6/pyPPG.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      190 2023-07-27 13:48:40.000000 pyPPG-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-08 21:37:13.954845 pyPPG-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1079 2023-08-08 21:35:23.000000 pyPPG-1.0.6/setup.py
```

### Comparing `pyPPG-1.0.5/LICENSE.txt` & `pyPPG-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.5/PKG-INFO` & `pyPPG-1.0.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,41 @@
-Metadata-Version: 2.1
-Name: pyPPG
-Version: 1.0.5
-Summary: pyPPG: a python toolbox for PPG morphological analysis.
-Home-page: https://github.com/godamartonaron/GODA_pyPPG
-Author: Marton A. Goda, PhD
-Author-email: marton.goda@campus.technion.ac.il
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-License-File: AUTHORS.rst
-
 
 # *pyPPG* toolbox documentation
 
 Photoplethysmogram (PPG) beat detection, fiducial points detection, and comprhessive assessment of standard biomarkers.
 
 ## Introduction
-The ***pyPPG*** is a standardised toolbox to analyze long-term finger PPG recordings in real-time. The state-of-the-art PPG biomarkers have been identified, implemented in the *pyPPG* toolbox, and validated on standard, public available PPG databases.
-The *pyPPG* using the improved *Automatic Beat Detector* [(*Aboy et al. 2005*)](https://ieeexplore.ieee.org/abstract/document/1510850).  The PPG peak and onset detection are implemented with. The *pyPPG* offers a robust beat detection, and a comprhessive assessment of clinically relevant biomarkers of continuous PPG time series.
+***pyPPG*** is a standardised toolbox to analyze long-term finger PPG recordings in real-time. The toolbox extracts state-of-the-art PPG biomarkers (_i.e._ pulse wave features) from PPG signals. The algorithms implemented in the *pyPPG* toolbox have been validated on publicly available PPG databases.
+Consequently, *pyPPG* offers robust and comprhessive assessment of clinically relevant biomarkers from continuous PPG signals.
 
 ## Description
 The following steps are implemented in the ***pyPPG*** toolbox:
-1. **Loading a raw PPG signal**: The toolbox can accept various file formats such as *.mat*, *.csv*, *.txt*, or *.edf*. These files should contain raw PPG data along with the corresponding sampling rate.
-2. **Preprocessing**: The raw signal is filtered to remove unwanted noise and artifacts. Subsequently, the signal is resampled to a uniform rate of 75 Hz.
-3. **Pulse wave segmentation**: The toolbox employs a peak detector to identify the systolic peaks. Based on the peak locations, the toolbox also detects the pulse onsets and offsets, which indicate the start and end of the PPG pulse waves.
+
+![PPG processing pipeline](figs/pyPPG_pipeline.svg).
+
+1. **Loading a raw PPG signal**: The toolbox can accept PPG signals in various file formats such as *.mat*, *.csv*, *.txt*, or *.edf*. These files should contain raw PPG data along with the corresponding sampling rate.
+2. **Preprocessing**: The raw signal is filtered to remove unwanted noise and artifacts. Subsequently, the signal is resampled to 75 Hz.
+3. **Pulse wave segmentation**: The toolbox employs a peak detector to identify the systolic peaks. It uses an [improved version](https://arxiv.org/abs/2307.10398) of a beat detection algorithm originally proposed in [(*Aboy et al. 2005*)](https://doi.org/10.1109/TBME.2005.855725). Based on the peak locations, the toolbox also detects the pulse onsets and offsets, which indicate the start and end of the PPG pulse waves.
 4. **Fiducial points identification**: For each pulse wave, the toolbox detects a set of fiducial points.
-5. **Biomarker engineering**: Based on the fiducial points, a set of 74 PPG digital biomarkers are engineered.
+5. **Biomarker engineering**: Based on the fiducial points, a set of 74 PPG digital biomarkers (_i.e._ pulse wave features) are calculated.
+
+![Fiducial point identification and biomarker engineering](figs/PPG_sample.svg)
 
 The *pyPPG* toolbox also provides an optional PPG signal quality index based on the Matlab implementation of the work by [(*Li et al. 2015*)](https://github.com/MIT-LCP/PhysioNetChallengePublic/blob/master/2015/sample-submission/ppgSQI.m).
 
+<<<<<<< HEAD
 ![](figs/pyPPG_pipeline.svg).
 
 The toolbox identifies individual pulse waves in a PPG signal by identifying ***systolic peaks (sp)***, and then
 identifying the ***pulse onset (on)*** and ***offset (off)*** on either side of each systolic peak which indicate the
 start and end of the pulse wave, respectively.
 
 ![](figs/PPG_sample.svg)
 
+=======
 ## Installation
 Available on pip, with the command: 
 ***pip install pyPPG***
 
 pip project: https://pypi.org/project/pyPPG/
 
 ## Requirements
@@ -60,21 +51,27 @@
 
 pandas == 1.5.0
 
 wfdb == 4.0.0
 
 mne == 1.2.0
 
-All the python requirements are installed when the toolbox is installed, no need for additional commands.
+All the python requirements are installed when the toolbox is installed, so there is no need for any additional commands.
 
 ## Documentation:
 https://pyppg.readthedocs.io/en/latest/
 
 ## The main components:
 1. **Software**
-    - An open-source algorithmic ***pyPPG*** toolbox, which implements the PPG peak and onsets detection algorithms and prefiltering routines. This can be used within your own data analysis code using the ***pyPPG*** API.
+    - An open-source algorithmic ***pyPPG*** toolbox, which loads a PPG signal, preprocesses it, segments individual pulse waves, identifies fiducial points, and calculates a set of biomarkers. This can be used within your own data analysis code using the ***pyPPG*** API.
 2. **Databases**
-    - The PPG signals are based on the ***PhysioNet Databases***. Available [here](https://physionet.org/about/database/) .
+    - The ***pyPPG*** signal analysis is based on the following datasets: 
+      - [BIDMC Dataset](https://physionet.org/content/bidmc/1.0.0/)
+      - [MESA Dataset](https://sleepdata.org/datasets/mesa)
+    - Further PPG datasets:
+      - [Collection of Peter Charlton](https://peterhcharlton.github.io/post/ppg_datasets/) 
+      - [Collection of Physionet](https://physionet.org/content/?topic=ppg)
+
 3. **Configuration**
     - A set of configuration files that adapt the PPG peak detection and ***pyPPG*** algorithms to work with sleep PPG data.
 
 All PPG measures can be further adapted for the analysis for efficient heart rate measurement as well as health assessment with clinically relevant biomarkers.
```

### Comparing `pyPPG-1.0.5/README.md` & `pyPPG-1.0.6/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,57 @@
+Metadata-Version: 2.1
+Name: pyPPG
+Version: 1.0.6
+Summary: pyPPG: a python toolbox for PPG morphological analysis.
+Home-page: https://github.com/godamartonaron/GODA_pyPPG
+Author: Marton A. Goda, PhD
+Author-email: marton.goda@campus.technion.ac.il
+Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+License-File: AUTHORS.rst
+
 
 # *pyPPG* toolbox documentation
 
 Photoplethysmogram (PPG) beat detection, fiducial points detection, and comprhessive assessment of standard biomarkers.
 
 ## Introduction
-The ***pyPPG*** is a standardised toolbox to analyze long-term finger PPG recordings in real-time. The state-of-the-art PPG biomarkers have been identified, implemented in the *pyPPG* toolbox, and validated on standard, public available PPG databases.
-The *pyPPG* using the improved *Automatic Beat Detector* [(*Aboy et al. 2005*)](https://ieeexplore.ieee.org/abstract/document/1510850).  The PPG peak and onset detection are implemented with. The *pyPPG* offers a robust beat detection, and a comprhessive assessment of clinically relevant biomarkers of continuous PPG time series.
+***pyPPG*** is a standardised toolbox to analyze long-term finger PPG recordings in real-time. The toolbox extracts state-of-the-art PPG biomarkers (_i.e._ pulse wave features) from PPG signals. The algorithms implemented in the *pyPPG* toolbox have been validated on publicly available PPG databases.
+Consequently, *pyPPG* offers robust and comprhessive assessment of clinically relevant biomarkers from continuous PPG signals.
 
 ## Description
 The following steps are implemented in the ***pyPPG*** toolbox:
-1. **Loading a raw PPG signal**: The toolbox can accept various file formats such as *.mat*, *.csv*, *.txt*, or *.edf*. These files should contain raw PPG data along with the corresponding sampling rate.
-2. **Preprocessing**: The raw signal is filtered to remove unwanted noise and artifacts. Subsequently, the signal is resampled to a uniform rate of 75 Hz.
-3. **Pulse wave segmentation**: The toolbox employs a peak detector to identify the systolic peaks. Based on the peak locations, the toolbox also detects the pulse onsets and offsets, which indicate the start and end of the PPG pulse waves.
+
+![PPG processing pipeline](figs/pyPPG_pipeline.svg).
+
+1. **Loading a raw PPG signal**: The toolbox can accept PPG signals in various file formats such as *.mat*, *.csv*, *.txt*, or *.edf*. These files should contain raw PPG data along with the corresponding sampling rate.
+2. **Preprocessing**: The raw signal is filtered to remove unwanted noise and artifacts. Subsequently, the signal is resampled to 75 Hz.
+3. **Pulse wave segmentation**: The toolbox employs a peak detector to identify the systolic peaks. It uses an [improved version](https://arxiv.org/abs/2307.10398) of a beat detection algorithm originally proposed in [(*Aboy et al. 2005*)](https://doi.org/10.1109/TBME.2005.855725). Based on the peak locations, the toolbox also detects the pulse onsets and offsets, which indicate the start and end of the PPG pulse waves.
 4. **Fiducial points identification**: For each pulse wave, the toolbox detects a set of fiducial points.
-5. **Biomarker engineering**: Based on the fiducial points, a set of 74 PPG digital biomarkers are engineered.
+5. **Biomarker engineering**: Based on the fiducial points, a set of 74 PPG digital biomarkers (_i.e._ pulse wave features) are calculated.
+
+![Fiducial point identification and biomarker engineering](figs/PPG_sample.svg)
 
 The *pyPPG* toolbox also provides an optional PPG signal quality index based on the Matlab implementation of the work by [(*Li et al. 2015*)](https://github.com/MIT-LCP/PhysioNetChallengePublic/blob/master/2015/sample-submission/ppgSQI.m).
 
+<<<<<<< HEAD
 ![](figs/pyPPG_pipeline.svg).
 
 The toolbox identifies individual pulse waves in a PPG signal by identifying ***systolic peaks (sp)***, and then
 identifying the ***pulse onset (on)*** and ***offset (off)*** on either side of each systolic peak which indicate the
 start and end of the pulse wave, respectively.
 
 ![](figs/PPG_sample.svg)
 
+=======
 ## Installation
 Available on pip, with the command: 
 ***pip install pyPPG***
 
 pip project: https://pypi.org/project/pyPPG/
 
 ## Requirements
@@ -44,21 +67,27 @@
 
 pandas == 1.5.0
 
 wfdb == 4.0.0
 
 mne == 1.2.0
 
-All the python requirements are installed when the toolbox is installed, no need for additional commands.
+All the python requirements are installed when the toolbox is installed, so there is no need for any additional commands.
 
 ## Documentation:
 https://pyppg.readthedocs.io/en/latest/
 
 ## The main components:
 1. **Software**
-    - An open-source algorithmic ***pyPPG*** toolbox, which implements the PPG peak and onsets detection algorithms and prefiltering routines. This can be used within your own data analysis code using the ***pyPPG*** API.
+    - An open-source algorithmic ***pyPPG*** toolbox, which loads a PPG signal, preprocesses it, segments individual pulse waves, identifies fiducial points, and calculates a set of biomarkers. This can be used within your own data analysis code using the ***pyPPG*** API.
 2. **Databases**
-    - The PPG signals are based on the ***PhysioNet Databases***. Available [here](https://physionet.org/about/database/) .
+    - The ***pyPPG*** signal analysis is based on the following datasets: 
+      - [BIDMC Dataset](https://physionet.org/content/bidmc/1.0.0/)
+      - [MESA Dataset](https://sleepdata.org/datasets/mesa)
+    - Further PPG datasets:
+      - [Collection of Peter Charlton](https://peterhcharlton.github.io/post/ppg_datasets/) 
+      - [Collection of Physionet](https://physionet.org/content/?topic=ppg)
+
 3. **Configuration**
     - A set of configuration files that adapt the PPG peak detection and ***pyPPG*** algorithms to work with sleep PPG data.
 
 All PPG measures can be further adapted for the analysis for efficient heart rate measurement as well as health assessment with clinically relevant biomarkers.
```

### Comparing `pyPPG-1.0.5/pyPPG/Biomarkers.py` & `pyPPG-1.0.6/pyPPG/Biomarkers.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,25 +42,31 @@
     ###########################################################################
     ############################ Get PPG Biomarkers ###########################
     ###########################################################################
     def getBiomarkers (self):
         """
         This function returns the PPG biomarkers.
 
-        :return: biomarkers dictionary of biomarkers in different categories:
+        :return: bm_vals: dictionary of biomarkers in different categories:
+            - PPG signal
+            - Signal ratios
+            - PPG derivatives
+            - Derivatives ratios
+        :return: bm_defs: dictionary of biomarkers with name, definition and unit:
             - PPG signal
             - Signal ratios
             - PPG derivatives
             - Derivatives ratios
         """
 
         s=self.s
         fiducials = self.fiducials
 
-        bm_ppg_sig = get_bm_ppg_sig(s,fiducials)
-        bm_sig_ratios = get_bm_sig_ratios(s,fiducials)
-        bm_ppg_derivs = get_bm_ppg_derivs(s,fiducials)
-        bm_derivs_ratios = get_bm_derivs_ratios(s,fiducials)
+        bm_ppg_sig, lst_ppg_sig = get_bm_ppg_sig(s,fiducials)
+        bm_sig_ratios, lst_sig_ratios = get_bm_sig_ratios(s, fiducials)
+        bm_ppg_derivs, lst_ppg_derivs = get_bm_ppg_derivs(s,fiducials)
+        bm_derivs_ratios, lst_derivs_ratios = get_bm_derivs_ratios(s,fiducials)
 
-        biomarkers={'bm_ppg_sig': bm_ppg_sig , 'bm_sig_ratios': bm_sig_ratios, 'bm_ppg_derivs': bm_ppg_derivs, 'bm_derivs_ratios': bm_derivs_ratios}
+        bm_vals={'ppg_sig': bm_ppg_sig , 'sig_ratios': bm_sig_ratios, 'ppg_derivs': bm_ppg_derivs, 'derivs_ratios': bm_derivs_ratios}
+        bm_defs = {'ppg_sig': lst_ppg_sig, 'sig_ratios': lst_sig_ratios, 'ppg_derivs': lst_ppg_derivs, 'derivs_ratios': lst_derivs_ratios}
 
-        return biomarkers
+        return bm_vals, bm_defs
```

### Comparing `pyPPG-1.0.5/pyPPG/DataHandling.py` & `pyPPG-1.0.6/pyPPG/DataHandling.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import pandas as pd
 
-from pyPPG.Preprocessing import*
+from Preprocessing import*
 
 import matplotlib.pyplot as plt
 import scipy.io
 import numpy as np
 from dotmap import DotMap
 from tkinter import filedialog
 import mne
 from matplotlib.backends.backend_agg import FigureCanvasAgg as FigureCanvas
 import os
 
 ###########################################################################
 ####################### Data Acquisition from Files #######################
 ###########################################################################
-def load_data(filtering: bool):
+def load_data(data_path:str,filtering: bool):
     """
     Load PPG data function load the raw PPG data.
 
+    :param data_path: path of the PPG signal
+    :type data_path: str
     :param filtering: a bool for filtering
     :type filtering: bool
 
     :return s: a struct of PPG signal:
         - s.v: a vector of PPG values
         - s.fs: the sampling frequency of the PPG in Hz
         - s.name: name of the record
@@ -29,26 +31,32 @@
         - s.fs: the sampling frequency of the PPG in Hz
         - s.filt_sig: 1-d array, a vector of the filtered PPG values
         - s.filt_d1: 1-d array, a vector of the filtered PPG' values
         - s.filt_d2: 1-d array, a vector of the filtered PPG" values
         - s.filt_d3: 1-d array, a vector of the filtered PPG'" values
     """
 
-    sig_path = filedialog.askopenfilename(title='Select SIGNAL file', filetypes=[("Input Files", ".mat .csv .edf .pkl .txt")])
+    if data_path=="":
+        sig_path = filedialog.askopenfilename(title='Select SIGNAL file', filetypes=[("Input Files", ".mat .csv .edf .pkl .txt")])
+    else:
+        sig_path=data_path
 
     if sig_path.rfind('/')>0:
         start_c = sig_path.rfind('/')+1
     else:
         start_c = sig_path.rfind('\\')
 
     stop_c=sig_path.rfind('.')
     rec_name=sig_path[start_c:stop_c]
 
+    try:
+        sig_format=sig_path[len(sig_path)-sig_path[::-1].index('.'):]
+    except:
+        print('Invalid signal path!')
 
-    sig_format=sig_path[len(sig_path)-sig_path[::-1].index('.'):]
     if sig_format=='mat':
         input_sig = scipy.io.loadmat(sig_path)
         hr = np.float64(np.squeeze(input_sig.get("Data")))[0:]
         try:
             fs = np.squeeze(input_sig.get("Fs"))
         except:
             fs = 100
@@ -86,15 +94,15 @@
     s.filt_sig, s.filt_d1, s.filt_d2, s.filt_d3 = Preprocessing(s, True)
 
     return s
 
 ###########################################################################
 ########################### Plot Fiducial points ##########################
 ###########################################################################
-def plot_fiducials(s: DotMap, fiducials: pd.DataFrame, savefig: bool):
+def plot_fiducials(s: DotMap, fiducials: pd.DataFrame):
     """
     Plot fiducial points of the filtered PPG signal.
 
     :param s: a struct of PPG signal:
         - s.v: a vector of PPG values
         - s.fs: the sampling frequency of the PPG in Hz
         - s.name: name of the record
@@ -103,16 +111,14 @@
         - s.filt_sig: 1-d array, a vector of the filtered PPG values
         - s.filt_d1: 1-d array, a vector of the filtered PPG' values
         - s.filt_d2: 1-d array, a vector of the filtered PPG" values
         - s.filt_d3: 1-d array, a vector of the filtered PPG'" values
     :type s: DotMap
     :param fiducials: a dictionary where the key is the name of the fiducial pints and the value is the list of fiducial points.
     :type fiducials: DataFrame
-    :param savefig: a bool for fiducial points saving
-    :type savefig: bool
     """
 
     fig = plt.figure(figsize=(20, 12))
     ax1 = plt.subplot(411)
     plt.plot(s.filt_sig, 'k', label=None)
     ax2 = plt.subplot(412, sharex=ax1)
     plt.plot(s.filt_d1, 'k', label=None)
@@ -173,27 +179,26 @@
 
         plt.yticks([])
 
     plt.xlabel('Time [s]', fontsize=20)
     plt.xticks(major_ticks,major_ticks_names, fontsize=20)
     plt.show()
 
-    if savefig:
-        canvas = FigureCanvas(fig)
-        tmp_dir='temp_dir'+os.sep+'PPG_Figures'+os.sep
-        os.makedirs(tmp_dir, exist_ok=True)
+    canvas = FigureCanvas(fig)
+    tmp_dir='temp_dir'+os.sep+'PPG_Figures'+os.sep
+    os.makedirs(tmp_dir, exist_ok=True)
 
-        canvas.print_png((tmp_dir+'%s.png') % (s.name))
-        print('Figure has been saved in the "temp_dir".')
+    canvas.print_png((tmp_dir+'%s.png') % (s.name))
+    print('Figure has been saved in the "temp_dir".')
 
 ###########################################################################
 ################################# Save Data ###############################
 ###########################################################################
 
-def save_data(s: DotMap, fiducials: pd.DataFrame, ppg_biomarkers: dict, ppg_statistics: dict):
+def save_data(s: DotMap, fiducials: pd.DataFrame, biomarkers_vals: dict, biomarkers_defs: dict, ppg_statistics: dict, savingformat: str,savingfolder: str):
     """
     Save the results of the filtered PPG analysis.
 
     :param s: a struct of PPG signal:
         - s.v: a vector of PPG values
         - s.fs: the sampling frequency of the PPG in Hz
         - s.name: name of the record
@@ -202,33 +207,70 @@
         - s.filt_sig: 1-d array, a vector of the filtered PPG values
         - s.filt_d1: 1-d array, a vector of the filtered PPG' values
         - s.filt_d2: 1-d array, a vector of the filtered PPG" values
         - s.filt_d3: 1-d array, a vector of the filtered PPG'" values
     :type s: DotMap
     :param fiducials: a dictionary where the key is the name of the fiducial pints and the value is the list of fiducial points
     :type fiducials: DataFrame
-    :param biomarkers: dictionary of biomarkers in different categories
+    :param biomarkers_vals: dictionary of biomarkers in different categories:
+        - PPG signal
+        - Signal ratios
+        - PPG derivatives
+        - Derivatives ratios
+    :type biomarkers_vals: dict
+    :param biomarkers_defs: dictionary of biomarkers with name, definition and unit:
         - PPG signal
         - Signal ratios
         - PPG derivatives
         - Derivatives ratios
-    :type ppg_biomarkers: dict
+    :type biomarkers_defs: dict
     :param Statistics: data frame with summary of PPG features
     :type Statistics: dict
+    :param savingformat: file format of the saved date, the provided file formats .mat and .csv
+    :type savingformat: str
+    :param savingfolder: location of the saved data
+    :type savingfolder: str
     """
 
-    tmp_dir = 'temp_dir'
+    tmp_dir = savingfolder
     os.makedirs(tmp_dir, exist_ok=True)
 
-    temp_dirs= ['PPG_Fiducials','PPG_Biomarkers','PPG_Statistics']
+    temp_dirs= ['Fiducials','Biomarkers','Statistics','Biomarkers_defs']
     for i in temp_dirs:
-        temp_dir = 'temp_dir'+os.sep+i+os.sep
+        temp_dir = tmp_dir+os.sep+i+os.sep
         if not os.path.exists(temp_dir):
             os.mkdir(temp_dir)
 
-    fiducials.to_csv((r'.'+os.sep+'temp_dir'+os.sep+temp_dirs[0]+os.sep+s.name+'_'+'Fiducial.csv'))
-    BM_keys=ppg_biomarkers.keys()
-    for key in BM_keys:
-        ppg_biomarkers[key].to_csv((r'.'+os.sep+'temp_dir'+os.sep+temp_dirs[1]+os.sep+'%s.csv')% (s.name+'_'+key),index=True,header=True)
-        ppg_statistics[key].to_csv((r'.'+os.sep+'temp_dir'+os.sep+temp_dirs[2]+os.sep+'%s.csv') % (s.name+'_'+key), index=True, header=True)
+    BM_keys = biomarkers_vals.keys()
+
+    if savingformat=="csv":
+        file_name = (r'.'+os.sep+tmp_dir+os.sep+temp_dirs[0]+os.sep+s.name+'_'+'Fiducial.csv')
+        fiducials.to_csv(file_name)
+
+        for key in BM_keys:
+            file_name = (r'.'+os.sep+tmp_dir+os.sep+temp_dirs[1]+os.sep+'%s.csv')% (s.name+'_'+key)
+            biomarkers_vals[key].to_csv(file_name,index=True,header=True)
+
+            file_name = (r'.'+os.sep+tmp_dir+os.sep+temp_dirs[2]+os.sep+'%s.csv') % (s.name+'_'+key)
+            ppg_statistics[key].to_csv(file_name, index=True, header=True)
+
+    elif savingformat=="mat":
+        matlab_struct = fiducials.to_dict(orient='list')
+        file_name = (r'.'+os.sep+tmp_dir+os.sep+temp_dirs[0]+os.sep+s.name+'_'+'Fiducial.mat')
+        scipy.io.savemat(file_name,matlab_struct)
+
+        for key in BM_keys:
+            matlab_struct = biomarkers_defs[key].to_dict(orient='list')
+            file_name = (r'.'+os.sep+tmp_dir+os.sep+temp_dirs[3]+os.sep+'%s.mat')% (key)
+            scipy.io.savemat(file_name,matlab_struct)
+
+            matlab_struct = biomarkers_vals[key].to_dict(orient='list')
+            file_name = (r'.'+os.sep+tmp_dir+os.sep+temp_dirs[1]+os.sep+'%s.mat')% (s.name+'_'+key)
+            scipy.io.savemat(file_name,matlab_struct)
+
+            file_name = (r'.'+os.sep+tmp_dir+os.sep+temp_dirs[2]+os.sep+'%s.mat') % (s.name+'_'+key)
+            ppg_statistics[key].to_csv(file_name, index=True, header=True)
+            scipy.io.savemat(file_name, matlab_struct)
+    else:
+        print('The file format is not suported for data saving! You can use "mat" or "csv" file formats.')
 
-    print('Results have been saved in the "temp_dir".')
+    print('Results have been saved into the "'+tmp_dir+'".')
```

### Comparing `pyPPG-1.0.5/pyPPG/FiducialPoints.py` & `pyPPG-1.0.6/pyPPG/FiducialPoints.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             - Original signal: List of pulse onset, pea and dicrotic notch
             - 1st derivative: List of points of 1st maximum and minimum in 1st derivitive between the onset to onset intervals (u,v)
             - 2nd derivative: List of maximum and minimum points in 2nd derivitive between the onset to onset intervals (a, b, c, d, e)
 
         :param correct: a bool for fiducials points corretion
         :type correct: bool
 
-        :return: fiducial points, a dictionary where the key is the name of the fiducial pints and the value is the list of fiducial points.
+        :return: fiducial points, a dictionary where the key is the name of the fiducial pints and the value is the list of fiducial points
         '''
 
         # 'abp' refers the improved Aboy++, and 'aby' refers the original Aboy peak detector
         peak_detector='abp'
 
         # Extract Fiducial Points
         drt0_fp=pd.DataFrame()
```

### Comparing `pyPPG-1.0.5/pyPPG/Preprocessing.py` & `pyPPG-1.0.6/pyPPG/Preprocessing.py`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.5/pyPPG/Statistics.py` & `pyPPG-1.0.6/pyPPG/Statistics.py`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.5/pyPPG/ppgSQI.py` & `pyPPG-1.0.6/pyPPG/ppgSQI.py`

 * *Files identical despite different names*

### Comparing `pyPPG-1.0.5/pyPPG/ppg_bm/get_biomarkers.py` & `pyPPG-1.0.6/pyPPG/ppg_bm/biomarker_extractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pandas as pd
 from scipy.signal import find_peaks
 
 ###########################################################################
 ####################### PPG biomarkers extraction #########################
 ###########################################################################
 
-class biomarkers_extract_PPG:
+class BmExtractor:
     """
     Class that extracts the PPG biomarkers.
     """
 
     def __init__(self, data: DotMap, peak_value: float, peak_time: float, next_peak_value: float, next_peak_time: float, onsets_values: np.array, onsets_times: np.array,
                  sample_rate: int, list_biomarkers: list, fiducials: pd.DataFrame):
         """
@@ -142,20 +142,20 @@
                     "Tw": self.get_Tw(),
                     "Ta": self.get_Ta(),
                     "Tb": self.get_Tb(),
                     "Tc": self.get_Tc(),
                     "Td": self.get_Td(),
                     "Te": self.get_Te(),
                     "Tf": self.get_Tf(),
-                    "Tb–c": self.get_Tbc(),
-                    "Tb–d": self.get_Tbd(),
+                    "Tb-c": self.get_Tbc(),
+                    "Tb-d": self.get_Tbd(),
                     "Tp1": self.get_Tp1(),
                     "Tp2": self.get_Tp2(),
-                    "Tp1–dp": self.get_Tp1_dp(),
-                    "Tp2–dp": self.get_Tp2_dp(),
+                    "Tp1-dp": self.get_Tp1_dp(),
+                    "Tp2-dp": self.get_Tp2_dp(),
 
                     # Derivatives ratios
                     "Tu/Tpi": self.get_ratio_Tu_Tpi(),
                     "Tv/Tpi": self.get_ratio_Tv_Tpi(),
                     "Tw/Tpi": self.get_ratio_Tw_Tpi(),
                     "Ta/Tpi": self.get_ratio_Ta_Tpi(),
                     "Tb/Tpi": self.get_ratio_Tb_Tpi(),
@@ -1187,15 +1187,14 @@
         Ae = self.segment_d2[self.get_e()]
         Af = self.segment_d2[self.get_e()]
         return (Ab-Ac-Ad-Ae-Af)/Aa
 
 ###########################################################################
 ############################# Get PPG biomarkers ############################
 ###########################################################################
-
 def get_biomarkers(s, fiducials, biomarkers_lst):
     """
     The function calculates the biomedical biomarkers of PPG signal.
 
     :param s: a struct of PPG signal:
         - s.v: a vector of PPG values
         - s.fs: the sampling frequency of the PPG in Hz
@@ -1259,15 +1258,15 @@
             next_peak_value = ppg[peaks[idx + 1].astype('int64')][0]
             next_peak_time = peaks[idx + 1] / fs
             next_peak_time = next_peak_time[0]
             #         plt.plot(data.sig)
             #         plt.show()
             #         print(peak_value,peak_time,next_peak_value,next_peak_time,onsets_values,onsets_times)
             try:
-                biomarkers_extractor = biomarkers_extract_PPG(data, peak_value, peak_time, next_peak_value, next_peak_time,
+                biomarkers_extractor = BmExtractor(data, peak_value, peak_time, next_peak_value, next_peak_time,
                                                           onsets_values, onsets_times, fs, biomarkers_lst,temp_fiducials)
                 biomarkers_vec = biomarkers_extractor.get_feature_extract_func()
                 lst = list(biomarkers_vec)
                 df_biomarkers.loc[len(df_biomarkers.index)] = lst
                 #         display(df_biomarkers)
                 df = pd.concat({'onset': onset, 'offset': offset, 'peak': peak}, ignore_index=True)
             except:
```

### Comparing `pyPPG-1.0.5/pyPPG/ppg_bm/get_bm_ppg_derivs.py` & `pyPPG-1.0.6/pyPPG/ppg_bm/get_bm_ppg_derivs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pyPPG.ppg_bm.get_biomarkers import*
+from pyPPG.ppg_bm.biomarker_extractor import*
 
 ###########################################################################
 ##################### Get Biomarkers of PPG Derivatives ###################
 ###########################################################################
 def get_bm_ppg_derivs(s, fiducials):
     """
     This function returns the biomarkers of PPG derivatives.
@@ -20,29 +20,34 @@
     :param fiducials: a dictionary where the key is the name of the fiducial pints and the value is the list of fiducial points PPG Fiducials Points.
         - PPG signal: List of pulse onset, systolic peak, dicrotic notch, diastolic peak
         - 1st derivative: List of points of 1st maximum and minimum in 1st derivitive between the onset to onset intervals (u,v)
         - 2nd derivative: List of maximum and minimum points in 2nd derivitive between the onset to onset intervals (a, b, c, d, e)
         - 3rd derivative: List of points of 1st maximum and minimum in 3rd derivitive between the onset to onset intervals (p1, p2)
 
     :return biomarkers: dictionary of biomarkers of PPG derivatives
+    :return biomarkers_lst: list a biomarkers with name, definition and unit
     """
 
-    biomarkers_lst = ["Tu",       # u-point time, the time between the pulse onset and u-point
-                    "Tv",       # v-point time, the time between the pulse onset and v-point
-                    "Tw",       # w-point time, the time between the pulse onset and w-point
-                    "Ta",       # a-point time, the time between the pulse onset and a-point
-                    "Tb",       # b-point time, the time between the pulse onset and b-point
-                    "Tc",       # c-point time, the time between the pulse onset and c-point
-                    "Td",       # d-point time, the time between the pulse onset and d-point
-                    "Te",       # e-point time, the time between the pulse onset and e-point
-                    "Tf",       # f-point time, the time between the pulse onset and f-point
-                    "Tb–c",	    # b–c interval time, the time between the b-point and c-point
-                    "Tb–d",	    # b–d interval time, the time between the b-point and d-point
-                    "Tp1",	    # p1-point time, the time between the pulse onset and p1-point
-                    "Tp2",      # p2-point time, the time between the pulse onset and p2-point
-                    "Tp1–dp",   # p1–dia interval time, the time between the p1-point and diastolic peak
-                    "Tp2–dp",   # p2–dia interval time, the time between the p2-point and diastolic peak
+    biomarkers_lst = [
+                    ["Tu",       "u-point time, the time between the pulse onset and u-point", "[s]"],
+                    ["Tv",       "v-point time, the time between the pulse onset and v-point", "[s]"],
+                    ["Tw",       "w-point time, the time between the pulse onset and w-point", "[s]"],
+                    ["Ta",       "a-point time, the time between the pulse onset and a-point", "[s]"],
+                    ["Tb",       "b-point time, the time between the pulse onset and b-point", "[s]"],
+                    ["Tc",       "c-point time, the time between the pulse onset and c-point", "[s]"],
+                    ["Td",       "d-point time, the time between the pulse onset and d-point", "[s]"],
+                    ["Te",       "e-point time, the time between the pulse onset and e-point", "[s]"],
+                    ["Tf",       "f-point time, the time between the pulse onset and f-point", "[s]"],
+                    ["Tb-c",	 "b-c time, the time between the b-point and c-point", "[s]"],
+                    ["Tb-d",	 "b-d time, the time between the b-point and d-point", "[s]"],
+                    ["Tp1",	     "p1-point time, the time between the pulse onset and p1-point", "[s]"],
+                    ["Tp2",      "p2-point time, the time between the pulse onset and p2-point", "[s]"],
+                    ["Tp1-dp",   "p1-dia time, the time between the p1-point and diastolic peak", "[s]"],
+                    ["Tp2-dp",   "p2-dia time, the time between the p2-point and diastolic peak", "[s]"],
     ]
 
-    df, df_biomarkers = get_biomarkers(s, fiducials, biomarkers_lst)
+    header = ['name', 'definition', 'unit']
+    biomarkers_lst = pd.DataFrame(biomarkers_lst, columns=header)
 
-    return df_biomarkers
+    df, df_biomarkers = get_biomarkers(s, fiducials, biomarkers_lst.name)
+    
+    return df_biomarkers, biomarkers_lst
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyPPG-1.0.5/pyPPG/ppg_bm/get_bm_ppg_sig.py` & `pyPPG-1.0.6/pyPPG/ppg_bm/get_bm_ppg_sig.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pyPPG.ppg_bm.get_biomarkers import*
+from pyPPG.ppg_bm.biomarker_extractor import*
 
 ###########################################################################
 ####################### Get Biomarkers of PPG Signal ######################
 ###########################################################################
 def get_bm_ppg_sig(s, fiducials):
     """
     This function returns the biomarkers of PPG signal.
@@ -21,48 +21,54 @@
     :param fiducials: a dictionary where the key is the name of the fiducial pints and the value is the list of fiducial points PPG Fiducials Points.
         - PPG signal: List of pulse onset, systolic peak, dicrotic notch, diastolic peak
         - 1st derivative: List of points of 1st maximum and minimum in 1st derivitive between the onset to onset intervals (u,v)
         - 2nd derivative: List of maximum and minimum points in 2nd derivitive between the onset to onset intervals (a, b, c, d, e)
         - 3rd derivative: List of points of 1st maximum and minimum in 3rd derivitive between the onset to onset intervals (p1, p2)
 
     :return biomarkers: dictionary of biomarkers of PPG signal
+    :return biomarkers_lst: list a biomarkers with name, definition and unit
     """
 
-    biomarkers_lst = ["Tpi",   # Pulse Interval, the time between the pulse onset and pulse offset
-                    "Tpp",   # Peak-to-Peak Interval, the time between two consecutive systolic peaks
-                    "Tsys",	 # Systolic Time, the time between the pulse onset and dicrotic notch
-                    "Tdia",  # Diastolic Time, the time is between the dicrotic notch and pulse offset
-                    "Tsp",   # Systolic Peak Time, the time between the pulse onset and systolic peak
-                    "Tdp",	 # Diastolic Peak Time, the time between the pulse onset and diastolic peak
-                    "deltaT",# Time Delay, the time between the systolic peak and diastolic peak
-                    "Tsw10", # Systolic Width, the width at 10% of the Systolic Peak Amplitude between the pulse onset and systolic peak
-                    "Tsw25", # Systolic Width, the width at 25% of the Systolic Peak Amplitude between the pulse onset and systolic peak
-                    "Tsw33", # Systolic Width, the width at 33% of the Systolic Peak Amplitude between the pulse onset and systolic peak
-                    "Tsw50", # Systolic Width, the width at 50% of the Systolic Peak Amplitude between the pulse onset and systolic peak
-                    "Tsw66", # Systolic Width, the width at 66% of the Systolic Peak Amplitude between the pulse onset and systolic peak
-                    "Tsw75", # Systolic Width, the width at 75% of the Systolic Peak Amplitude between the pulse onset and systolic peak
-                    "Tsw90", # Systolic Width, the width at 90% of the Systolic Peak Amplitude between the pulse onset and systolic peak
-                    "Tdw10", # Diastolic Width, the width at 10% of the Systolic Peak Amplitude between the systolic peak and pulse offset
-                    "Tdw25", # Diastolic Width, the width at 25% of the Systolic Peak Amplitude between the systolic peak and pulse offset
-                    "Tdw33", # Diastolic Width, the width at 33% of the Systolic Peak Amplitude between the systolic peak and pulse offset
-                    "Tdw50", # Diastolic Width, the width at 50% of the Systolic Peak Amplitude between the systolic peak and pulse offset
-                    "Tdw66", # Diastolic Width, the width at 66% of the Systolic Peak Amplitude between the systolic peak and pulse offset
-                    "Tdw75", # Diastolic Width, the width at 75% of the Systolic Peak Amplitude between the systolic peak and pulse offset
-                    "Tdw90", # Diastolic Width, the width at 90% of the Systolic Peak Amplitude between the systolic peak and pulse offset
-                    "Tpw10", # Pulse Width, the sum of the Systolic Width and the Diastolic Width at 10%
-                    "Tpw25", # Pulse Width, the sum of the Systolic Width and the Diastolic Width at 25%
-                    "Tpw33", # Pulse Width, the sum of the Systolic Width and the Diastolic Width at 33%
-                    "Tpw50", # Pulse Width, the sum of the Systolic Width and the Diastolic Width at 50%
-                    "Tpw66", # Pulse Width, the sum of the Systolic Width and the Diastolic Width at 66%
-                    "Tpw75", # Pulse Width, the sum of the Systolic Width and the Diastolic Width at 75%
-                    "Tpw90", # Pulse Width, the sum of the Systolic Width and the Diastolic Width at 90%
-                    "Asp",   # Systolic Peak Amplitude, the difference in amplitude between the pulse onset and systolic peak
-                    "Adn",   # Dicrotic Notch Amplitude, the difference in amplitude between the pulse onset and dicrotic notch
-                    "Adp",   # Diastolic Peak Amplitude, the difference in amplitude between the pulse onset and diastolic peak
-                    "Aoff",  # Pulse Onset Amplitude, the difference in amplitude between the pulse onset and pulse offset
-                    "AUCpi", # Area Under Pulse Interval Curve, the area under the pulse wave between pulse onset and pulse offset
-                    "AUCsys",# Area Under Systolic Curve, the area under the pulse wave between the pulse onset and the dicrotic notch
-                    "AUCdia",# Area Under Diastolic Curve, the area under the pulse wave between the dicrotic notch and pulse offset
-                    ]
-    df, df_biomarkers = get_biomarkers(s, fiducials, biomarkers_lst)
+    biomarkers_lst = [
+                    ["Tpi",   "Pulse interval, the time between the pulse onset and pulse offset", "[s]"],
+                    ["Tpp",   "Peak-to-peak interval, the time between two consecutive systolic peaks", "[s]"],
+                    ["Tsys",  "Systolic time, the time between the pulse onset and dicrotic notch", "[s]"],
+                    ["Tdia",  "Diastolic time, the time is between the dicrotic notch and pulse offset", "[s]"],
+                    ["Tsp",   "Systolic peak time, the time between the pulse onset and systolic peak", "[s]"],
+                    ["Tdp",	  "Diastolic peak time, the time between the pulse onset and diastolic peak", "[s]"],
+                    ["deltaT","Time delay, the time between the systolic peak and diastolic peak", "[s]"],
+                    ["Tsw10", "Systolic width, the width at 10% of the systolic peak amplitude between the pulse onset and systolic peak", "[s]"],
+                    ["Tsw25", "Systolic width, the width at 25% of the systolic peak amplitude between the pulse onset and systolic peak", "[s]"],
+                    ["Tsw33", "Systolic width, the width at 33% of the systolic peak amplitude between the pulse onset and systolic peak", "[s]"],
+                    ["Tsw50", "Systolic width, the width at 50% of the systolic peak amplitude between the pulse onset and systolic peak", "[s]"],
+                    ["Tsw66", "Systolic width, the width at 66% of the systolic peak amplitude between the pulse onset and systolic peak", "[s]"],
+                    ["Tsw75", "Systolic width, the width at 75% of the systolic peak amplitude between the pulse onset and systolic peak", "[s]"],
+                    ["Tsw90", "Systolic width, the width at 90% of the systolic peak amplitude between the pulse onset and systolic peak", "[s]"],
+                    ["Tdw10", "Diastolic width, the width at 10% of the systolic peak amplitude between the systolic peak and pulse offset", "[s]"],
+                    ["Tdw25", "Diastolic width, the width at 25% of the systolic peak amplitude between the systolic peak and pulse offset", "[s]"],
+                    ["Tdw33", "Diastolic width, the width at 33% of the systolic peak amplitude between the systolic peak and pulse offset", "[s]"],
+                    ["Tdw50", "Diastolic width, the width at 50% of the systolic peak amplitude between the systolic peak and pulse offset", "[s]"],
+                    ["Tdw66", "Diastolic width, the width at 66% of the systolic peak amplitude between the systolic peak and pulse offset", "[s]"],
+                    ["Tdw75", "Diastolic width, the width at 75% of the systolic peak amplitude between the systolic peak and pulse offset", "[s]"],
+                    ["Tdw90", "Diastolic width, the width at 90% of the systolic peak amplitude between the systolic peak and pulse offset", "[s]"],
+                    ["Tpw10", "Pulse width, the sum of the systolic width and the diastolic width at 10%", "[s]"],
+                    ["Tpw25", "Pulse width, the sum of the systolic width and the diastolic width at 25%", "[s]"],
+                    ["Tpw33", "Pulse width, the sum of the systolic width and the diastolic width at 33%", "[s]"],
+                    ["Tpw50", "Pulse width, the sum of the systolic width and the diastolic width at 50%", "[s]"],
+                    ["Tpw66", "Pulse width, the sum of the systolic width and the diastolic width at 66%", "[s]"],
+                    ["Tpw75", "Pulse width, the sum of the systolic width and the diastolic width at 75%", "[s]"],
+                    ["Tpw90", "Pulse width, the sum of the systolic width and the diastolic width at 90%", "[s]"],
+                    ["Asp",   "Systolic peak amplitude, the difference in amplitude between the pulse onset and systolic peak", "[nu]"],
+                    ["Adn",   "Dicrotic notch amplitude, the difference in amplitude between the pulse onset and dicrotic notch", "[nu]"],
+                    ["Adp",   "Diastolic peak amplitude, the difference in amplitude between the pulse onset and diastolic peak", "[nu]"],
+                    ["Aoff",  "Pulse onset amplitude, the difference in amplitude between the pulse onset and pulse offset", "[nu]"],
+                    ["AUCpi", "Area under pulse interval curve, the area under the pulse wave between pulse onset and pulse offset", "[nu]"],
+                    ["AUCsys","Area under systolic curve, the area under the pulse wave between the pulse onset and the dicrotic notch", "[nu]"],
+                    ["AUCdia","Area under diastolic curve, the area under the pulse wave between the dicrotic notch and pulse offset", "[nu]"],
+    ]
 
-    return df_biomarkers
+    header = ['name', 'definition', 'unit']
+    biomarkers_lst = pd.DataFrame(biomarkers_lst, columns=header)
+
+    df, df_biomarkers = get_biomarkers(s, fiducials, biomarkers_lst.name)
+
+    return df_biomarkers, biomarkers_lst
```

### Comparing `pyPPG-1.0.5/pyPPG.egg-info/PKG-INFO` & `pyPPG-1.0.6/pyPPG.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPPG
-Version: 1.0.5
+Version: 1.0.6
 Summary: pyPPG: a python toolbox for PPG morphological analysis.
 Home-page: https://github.com/godamartonaron/GODA_pyPPG
 Author: Marton A. Goda, PhD
 Author-email: marton.goda@campus.technion.ac.il
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -16,35 +16,42 @@
 
 
 # *pyPPG* toolbox documentation
 
 Photoplethysmogram (PPG) beat detection, fiducial points detection, and comprhessive assessment of standard biomarkers.
 
 ## Introduction
-The ***pyPPG*** is a standardised toolbox to analyze long-term finger PPG recordings in real-time. The state-of-the-art PPG biomarkers have been identified, implemented in the *pyPPG* toolbox, and validated on standard, public available PPG databases.
-The *pyPPG* using the improved *Automatic Beat Detector* [(*Aboy et al. 2005*)](https://ieeexplore.ieee.org/abstract/document/1510850).  The PPG peak and onset detection are implemented with. The *pyPPG* offers a robust beat detection, and a comprhessive assessment of clinically relevant biomarkers of continuous PPG time series.
+***pyPPG*** is a standardised toolbox to analyze long-term finger PPG recordings in real-time. The toolbox extracts state-of-the-art PPG biomarkers (_i.e._ pulse wave features) from PPG signals. The algorithms implemented in the *pyPPG* toolbox have been validated on publicly available PPG databases.
+Consequently, *pyPPG* offers robust and comprhessive assessment of clinically relevant biomarkers from continuous PPG signals.
 
 ## Description
 The following steps are implemented in the ***pyPPG*** toolbox:
-1. **Loading a raw PPG signal**: The toolbox can accept various file formats such as *.mat*, *.csv*, *.txt*, or *.edf*. These files should contain raw PPG data along with the corresponding sampling rate.
-2. **Preprocessing**: The raw signal is filtered to remove unwanted noise and artifacts. Subsequently, the signal is resampled to a uniform rate of 75 Hz.
-3. **Pulse wave segmentation**: The toolbox employs a peak detector to identify the systolic peaks. Based on the peak locations, the toolbox also detects the pulse onsets and offsets, which indicate the start and end of the PPG pulse waves.
+
+![PPG processing pipeline](figs/pyPPG_pipeline.svg).
+
+1. **Loading a raw PPG signal**: The toolbox can accept PPG signals in various file formats such as *.mat*, *.csv*, *.txt*, or *.edf*. These files should contain raw PPG data along with the corresponding sampling rate.
+2. **Preprocessing**: The raw signal is filtered to remove unwanted noise and artifacts. Subsequently, the signal is resampled to 75 Hz.
+3. **Pulse wave segmentation**: The toolbox employs a peak detector to identify the systolic peaks. It uses an [improved version](https://arxiv.org/abs/2307.10398) of a beat detection algorithm originally proposed in [(*Aboy et al. 2005*)](https://doi.org/10.1109/TBME.2005.855725). Based on the peak locations, the toolbox also detects the pulse onsets and offsets, which indicate the start and end of the PPG pulse waves.
 4. **Fiducial points identification**: For each pulse wave, the toolbox detects a set of fiducial points.
-5. **Biomarker engineering**: Based on the fiducial points, a set of 74 PPG digital biomarkers are engineered.
+5. **Biomarker engineering**: Based on the fiducial points, a set of 74 PPG digital biomarkers (_i.e._ pulse wave features) are calculated.
+
+![Fiducial point identification and biomarker engineering](figs/PPG_sample.svg)
 
 The *pyPPG* toolbox also provides an optional PPG signal quality index based on the Matlab implementation of the work by [(*Li et al. 2015*)](https://github.com/MIT-LCP/PhysioNetChallengePublic/blob/master/2015/sample-submission/ppgSQI.m).
 
+<<<<<<< HEAD
 ![](figs/pyPPG_pipeline.svg).
 
 The toolbox identifies individual pulse waves in a PPG signal by identifying ***systolic peaks (sp)***, and then
 identifying the ***pulse onset (on)*** and ***offset (off)*** on either side of each systolic peak which indicate the
 start and end of the pulse wave, respectively.
 
 ![](figs/PPG_sample.svg)
 
+=======
 ## Installation
 Available on pip, with the command: 
 ***pip install pyPPG***
 
 pip project: https://pypi.org/project/pyPPG/
 
 ## Requirements
@@ -60,21 +67,27 @@
 
 pandas == 1.5.0
 
 wfdb == 4.0.0
 
 mne == 1.2.0
 
-All the python requirements are installed when the toolbox is installed, no need for additional commands.
+All the python requirements are installed when the toolbox is installed, so there is no need for any additional commands.
 
 ## Documentation:
 https://pyppg.readthedocs.io/en/latest/
 
 ## The main components:
 1. **Software**
-    - An open-source algorithmic ***pyPPG*** toolbox, which implements the PPG peak and onsets detection algorithms and prefiltering routines. This can be used within your own data analysis code using the ***pyPPG*** API.
+    - An open-source algorithmic ***pyPPG*** toolbox, which loads a PPG signal, preprocesses it, segments individual pulse waves, identifies fiducial points, and calculates a set of biomarkers. This can be used within your own data analysis code using the ***pyPPG*** API.
 2. **Databases**
-    - The PPG signals are based on the ***PhysioNet Databases***. Available [here](https://physionet.org/about/database/) .
+    - The ***pyPPG*** signal analysis is based on the following datasets: 
+      - [BIDMC Dataset](https://physionet.org/content/bidmc/1.0.0/)
+      - [MESA Dataset](https://sleepdata.org/datasets/mesa)
+    - Further PPG datasets:
+      - [Collection of Peter Charlton](https://peterhcharlton.github.io/post/ppg_datasets/) 
+      - [Collection of Physionet](https://physionet.org/content/?topic=ppg)
+
 3. **Configuration**
     - A set of configuration files that adapt the PPG peak detection and ***pyPPG*** algorithms to work with sleep PPG data.
 
 All PPG measures can be further adapted for the analysis for efficient heart rate measurement as well as health assessment with clinically relevant biomarkers.
```

### Comparing `pyPPG-1.0.5/pyPPG.egg-info/SOURCES.txt` & `pyPPG-1.0.6/pyPPG.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -15,12 +15,12 @@
 pyPPG.egg-info/SOURCES.txt
 pyPPG.egg-info/dependency_links.txt
 pyPPG.egg-info/requires.txt
 pyPPG.egg-info/top_level.txt
 pyPPG/pack_ppg/_ErrorHandler.py
 pyPPG/pack_ppg/__init__.py
 pyPPG/ppg_bm/__init__.py
-pyPPG/ppg_bm/get_biomarkers.py
+pyPPG/ppg_bm/biomarker_extractor.py
 pyPPG/ppg_bm/get_bm_derivs_ratios.py
 pyPPG/ppg_bm/get_bm_ppg_derivs.py
 pyPPG/ppg_bm/get_bm_ppg_sig.py
 pyPPG/ppg_bm/get_bm_sig_ratios.py
```

### Comparing `pyPPG-1.0.5/setup.py` & `pyPPG-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import io
 
 with io.open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pyPPG',
-    version='1.0.5',
+    version='1.0.6',
     description='pyPPG: a python toolbox for PPG morphological analysis.',
     author='Marton A. Goda, PhD',
     author_email="marton.goda@campus.technion.ac.il",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/godamartonaron/GODA_pyPPG",
     project_urls={"Bug Tracker": "https://github.com/pypa/sampleproject/issues",},
```

