# Comparing `tmp/whyshift-0.0.4.tar.gz` & `tmp/whyshift-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/whyshift-0.0.4.tar", last modified: Fri Jul 14 08:15:19 2023, max compression
+gzip compressed data, was "dist/whyshift-0.0.5.tar", last modified: Wed Aug  9 02:29:12 2023, max compression
```

## Comparing `whyshift-0.0.4.tar` & `whyshift-0.0.5.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-14 08:15:19.000000 whyshift-0.0.4/
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-11 11:02:02.000000 whyshift-0.0.4/LICENSE
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      630 2023-07-14 08:15:19.000000 whyshift-0.0.4/PKG-INFO
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     9650 2023-07-13 06:06:43.000000 whyshift-0.0.4/README.md
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)       38 2023-07-14 08:15:19.000000 whyshift-0.0.4/setup.cfg
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      961 2023-07-14 08:15:09.000000 whyshift-0.0.4/setup.py
-drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-14 08:15:19.000000 whyshift-0.0.4/whyshift/
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      257 2023-07-14 08:15:13.000000 whyshift-0.0.4/whyshift/__init__.py
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     1878 2023-07-14 07:22:05.000000 whyshift-0.0.4/whyshift/algorithm.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)    13969 2023-07-12 14:48:26.000000 whyshift-0.0.4/whyshift/dataset.py
-drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-14 08:15:19.000000 whyshift-0.0.4/whyshift/folktables/
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      165 2023-07-11 11:01:26.000000 whyshift-0.0.4/whyshift/folktables/__init__.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     8357 2023-07-11 11:01:26.000000 whyshift-0.0.4/whyshift/folktables/acs.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      747 2023-07-11 11:01:26.000000 whyshift-0.0.4/whyshift/folktables/dataset.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      987 2023-07-11 11:01:26.000000 whyshift-0.0.4/whyshift/folktables/exceptions.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     4568 2023-07-11 11:01:26.000000 whyshift-0.0.4/whyshift/folktables/folktables.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     8782 2023-07-11 11:01:26.000000 whyshift-0.0.4/whyshift/folktables/load_acs.py
-drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-14 08:15:19.000000 whyshift-0.0.4/whyshift/folktables/utils/
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-11 11:01:26.000000 whyshift-0.0.4/whyshift/folktables/utils/__init__.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     4043 2023-07-11 11:01:26.000000 whyshift-0.0.4/whyshift/folktables/utils/download_utils.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      998 2023-07-11 11:01:26.000000 whyshift-0.0.4/whyshift/folktables/utils/files_resources.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     1443 2023-07-11 11:01:26.000000 whyshift-0.0.4/whyshift/folktables/utils/load_utils.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     7466 2023-07-11 11:01:26.000000 whyshift-0.0.4/whyshift/folktables_utils.py
-drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-14 08:15:19.000000 whyshift-0.0.4/whyshift/methods/
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)       27 2023-07-14 06:56:16.000000 whyshift-0.0.4/whyshift/methods/__init__.py
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)    17633 2023-07-14 07:10:32.000000 whyshift-0.0.4/whyshift/methods/marginal_dro_criterion.py
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)    61208 2023-07-14 07:08:27.000000 whyshift-0.0.4/whyshift/methods/model_family.py
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     1215 2023-07-14 07:10:04.000000 whyshift-0.0.4/whyshift/methods/model_util.py
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)    10357 2023-07-14 07:03:31.000000 whyshift-0.0.4/whyshift/methods/robust_loss.py
--rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     4547 2023-07-11 11:10:30.000000 whyshift-0.0.4/whyshift/utils.py
-drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-14 08:15:19.000000 whyshift-0.0.4/whyshift.egg-info/
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      630 2023-07-14 08:15:19.000000 whyshift-0.0.4/whyshift.egg-info/PKG-INFO
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      820 2023-07-14 08:15:19.000000 whyshift-0.0.4/whyshift.egg-info/SOURCES.txt
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)        1 2023-07-14 08:15:19.000000 whyshift-0.0.4/whyshift.egg-info/dependency_links.txt
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)       70 2023-07-14 08:15:19.000000 whyshift-0.0.4/whyshift.egg-info/requires.txt
--rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)        9 2023-07-14 08:15:19.000000 whyshift-0.0.4/whyshift.egg-info/top_level.txt
+drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-08-09 02:29:12.000000 whyshift-0.0.5/
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-11 11:02:02.000000 whyshift-0.0.5/LICENSE
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      630 2023-08-09 02:29:12.000000 whyshift-0.0.5/PKG-INFO
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)    10586 2023-07-14 08:37:35.000000 whyshift-0.0.5/README.md
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)       38 2023-08-09 02:29:12.000000 whyshift-0.0.5/setup.cfg
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      961 2023-08-09 02:21:06.000000 whyshift-0.0.5/setup.py
+drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-08-09 02:29:12.000000 whyshift-0.0.5/whyshift/
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      295 2023-08-09 02:20:58.000000 whyshift-0.0.5/whyshift/__init__.py
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     1878 2023-07-14 07:22:05.000000 whyshift-0.0.5/whyshift/algorithm.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)    13969 2023-07-12 14:48:26.000000 whyshift-0.0.5/whyshift/dataset.py
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     5073 2023-08-09 02:20:26.000000 whyshift-0.0.5/whyshift/disde.py
+drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-08-09 02:29:12.000000 whyshift-0.0.5/whyshift/folktables/
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      165 2023-07-11 11:01:26.000000 whyshift-0.0.5/whyshift/folktables/__init__.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     8357 2023-07-11 11:01:26.000000 whyshift-0.0.5/whyshift/folktables/acs.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      747 2023-07-11 11:01:26.000000 whyshift-0.0.5/whyshift/folktables/dataset.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      987 2023-07-11 11:01:26.000000 whyshift-0.0.5/whyshift/folktables/exceptions.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     4568 2023-07-11 11:01:26.000000 whyshift-0.0.5/whyshift/folktables/folktables.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     8782 2023-07-11 11:01:26.000000 whyshift-0.0.5/whyshift/folktables/load_acs.py
+drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-08-09 02:29:12.000000 whyshift-0.0.5/whyshift/folktables/utils/
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-07-11 11:01:26.000000 whyshift-0.0.5/whyshift/folktables/utils/__init__.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     4043 2023-07-11 11:01:26.000000 whyshift-0.0.5/whyshift/folktables/utils/download_utils.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      998 2023-07-11 11:01:26.000000 whyshift-0.0.5/whyshift/folktables/utils/files_resources.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     1443 2023-07-11 11:01:26.000000 whyshift-0.0.5/whyshift/folktables/utils/load_utils.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     7466 2023-07-11 11:01:26.000000 whyshift-0.0.5/whyshift/folktables_utils.py
+drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-08-09 02:29:12.000000 whyshift-0.0.5/whyshift/methods/
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)       27 2023-07-14 06:56:16.000000 whyshift-0.0.5/whyshift/methods/__init__.py
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)    17633 2023-07-14 07:10:32.000000 whyshift-0.0.5/whyshift/methods/marginal_dro_criterion.py
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)    61208 2023-07-14 07:08:27.000000 whyshift-0.0.5/whyshift/methods/model_family.py
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     1215 2023-07-14 07:10:04.000000 whyshift-0.0.5/whyshift/methods/model_util.py
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)    10357 2023-07-14 07:03:31.000000 whyshift-0.0.5/whyshift/methods/robust_loss.py
+-rw-r--r--   0 jiashuoliu  (1002) jiashuoliu  (1002)     4547 2023-07-11 11:10:30.000000 whyshift-0.0.5/whyshift/utils.py
+drwxrwxr-x   0 jiashuoliu  (1002) jiashuoliu  (1002)        0 2023-08-09 02:29:12.000000 whyshift-0.0.5/whyshift.egg-info/
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      630 2023-08-09 02:29:12.000000 whyshift-0.0.5/whyshift.egg-info/PKG-INFO
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)      838 2023-08-09 02:29:12.000000 whyshift-0.0.5/whyshift.egg-info/SOURCES.txt
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)        1 2023-08-09 02:29:12.000000 whyshift-0.0.5/whyshift.egg-info/dependency_links.txt
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)       70 2023-08-09 02:29:12.000000 whyshift-0.0.5/whyshift.egg-info/requires.txt
+-rw-rw-r--   0 jiashuoliu  (1002) jiashuoliu  (1002)        9 2023-08-09 02:29:12.000000 whyshift-0.0.5/whyshift.egg-info/top_level.txt
```

### Comparing `whyshift-0.0.4/PKG-INFO` & `whyshift-0.0.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whyshift
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package of various specified distribution shift patterns of out-of-distributoin generalization problem on tabular data
 Home-page: https://github.com/namkoong-lab/whyshift
 Author: Jiashuo Liu, Tianyu Wang, Peng Cui, Hongseok Namkoong
 Author-email: liujiashuo77@gmail.com, tw2837@columbia.edu, cuip@tsinghua.edu.cn, namkoong@gsb.columbia.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

### Comparing `whyshift-0.0.4/README.md` & `whyshift-0.0.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -16,16 +16,17 @@
 
 
 
 ## Table of Contents
 1. [Dataset Access](#basic-installation-instructions)
 2. [Python Package: `whyshift`](#python-package-whyshift)
 3. [Different Distribution Shift Patterns](#different-distribution-shift-patterns)
-3. [License and terms of use](#license-and-terms-of-use)
-4. [References](#references)
+4. [Implemented Algorithms](#implemented-algorithms)
+5. [License and terms of use](#license-and-terms-of-use)
+6. [References](#references)
 
 
 
 ## Dataset Access
 Here we provide the access links for the 5 datasets used in our benchmark.
 
 #### ACS Income
@@ -137,21 +138,40 @@
 | 19 | ACS Pub.Cov | Temporal | 18 | Public Ins. Coverage | Year 2010 (NY) | 73,208 | 3 | X: 2/2 |
 | 20 | ACS Pub.Cov | Temporal | 18 | Public Ins. Coverage | Year 2010 (CA) | 149,441 | 3 | X: 2/2 |
 | 21 | ACS Income | Synthetic | 9 | Income≥50k | Younger People (80%) | 20,000 | 1 | X: 1/1 |
 | 22 | ACS Income | Synthetic | 9 | Income≥50k | Younger People (90%) | 20,000 | 1 | X: 1/1 |
 
 In our benchmark, each setting has multiple target domains (except the last setting). In our main body, we select only one target domain for each setting. We report the `Dom. Ratio` to represent the dominant ratio of $Y|X$ shifts or $X$ shifts in source-target pairs with performance degradation larger than **5** percentage points in each setting. For example, "$Y|X$: 13/14" means that there are 14 source-target pairs in Setting 1 with degradation larger than 5 percentage points and 13 out of them with over 50\% degradation attributed to $Y|X$ shifts. We use XGBoost to measure this.
 
+
+## Implemented Algorithms
+In our `whyshift` package, we also implement several algorithms for tabular data classification, including `Logistic Regression`, `MLP`, `SVM`, `Random Forest`, `XGBoost`, `LightGBM`, `GBM`, $\chi^2$/CVaR-`DRO/DORO`, `Group DRO`, `Simple-Reweighting`, `JTT`, `Fairness-In/Postprocess` and `DWR` methods.
+
+```python
+# use the implemented methods
+algo = fetch_model(method_name)
+```
+
+Note that the supported method names are:
+
+```python
+method_name_list = ['lr','svm','xgb', 'lightgbm', 'rf',  'dwr', 'jtt','suby', 'subg', 'rwy', 'rwg', 'FairPostprocess_exp','FairInprocess_dp', 'FairPostprocess_threshold', 'FairInprocess_eo', 'FairInprocess_error_parity','chi_dro', 'chi_doro','cvar_dro','cvar_doro','group_dro']
+```
+
+
+
+
 ## License and terms of use
 Our benchmark is built upon `Folktables`. The License of `Folktables` is:
 
 ```
 Folktables provides code to download data from the American Community Survey (ACS) Public Use Microdata Sample (PUMS) files managed by the US Census Bureau. The data itself is governed by the terms of use provided by the Census Bureau. For more information, see https://www.census.gov/data/developers/about/terms-of-service.html
 
 The Adult reconstruction dataset is a subsample of the IPUMS CPS data available from https://cps.ipums.org/. The data are intended for replication purposes only. Individuals analyzing the data for other purposes must submit a separate data extract request directly via IPUMS CPS. Individuals are not to redistribute the data without permission. Contact ipums@umn.edu for redistribution requests.
 ```
 Besides, for US Accident and Taxi data from `kaggle`, individuals should follow the their Licenses, see https://www.kaggle.com/datasets/sobhanmoosavi/us-accidents and https://www.kaggle.com/competitions/nyc-taxi-trip-duration/data.
 
 ## References
 [1] Ding, F., Hardt, M., Miller, J., & Schmidt, L. (2021). Retiring adult: New datasets for fair machine learning. Advances in neural information processing systems, 34, 6478-6490.
 
-ps: we modify the <a href="https://github.com/socialfoundations/folktables">`folktables`</a> code to support `year` before 2014, and therefore we involve it in our package. 
+* We modify the <a href="https://github.com/socialfoundations/folktables">`folktables`</a> code to support `year` before 2014, and involve the revised version in our package. 
+* Part of the algorithm codes are used from the <a href="https://github.com/jpgard/subgroup-robustness-grows-on-trees">codebase</a>.
```

#### html2text {}

```diff
@@ -8,42 +8,43 @@
 Wang, Peng Cui, Hongseok Namkoong > Tsinghua University, Columbia University
 `WhyShift` is a python package that provides a benchmark with various specified
 distribution shift patterns on real-world tabular data. Our testbed highlights
 the importance of future research that builds an understanding of how
 distributions differ. For more details, please refer to our paper. ## Table of
 Contents 1. [Dataset Access](#basic-installation-instructions) 2. [Python
 Package: `whyshift`](#python-package-whyshift) 3. [Different Distribution Shift
-Patterns](#different-distribution-shift-patterns) 3. [License and terms of use]
-(#license-and-terms-of-use) 4. [References](#references) ## Dataset Access Here
-we provide the access links for the 5 datasets used in our benchmark. #### ACS
-Income * The task is to predict whether an individualâs income is above
-\$50,000. * Access link: https://github.com/socialfoundations/folktables *
-Reference: Ding, F., Hardt, M., Miller, J., & Schmidt, L. (2021). Retiring
-adult: New datasets for fair machine learning. Advances in neural information
-processing systems, 34, 6478-6490. * License: MIT License #### ACS PubCov * The
-task is to predict whether an individual has public health insurance. * Access
-link: https://github.com/socialfoundations/folktables * Reference: Ding, F.,
-Hardt, M., Miller, J., & Schmidt, L. (2021). Retiring adult: New datasets for
-fair machine learning. Advances in neural information processing systems, 34,
-6478-6490. * License: MIT License #### ACS Mobility * The task is to predict
-whether an individual had the same residential address one year ago. * Access
-link: https://github.com/socialfoundations/folktables * Reference: Ding, F.,
-Hardt, M., Miller, J., & Schmidt, L. (2021). Retiring adult: New datasets for
-fair machine learning. Advances in neural information processing systems, 34,
-6478-6490. * License: MIT License #### Taxi Dataset * The task is to predict
-whether the total ride duration time exceeds 30 minutes, based on location and
-temporal features. * Access link: * https://www.kaggle.com/datasets/mnavas/
-taxi-routes-for-mexico-city-and-quito * https://www.kaggle.com/competitions/
-nyc-taxi-trip-duration/data * License: CC BY-SA 4.0 #### US Accident Dataset *
-The task is to predict whether an accident is severe (long delay) or not (short
-delay) based on weather features and Road condition features. * Access link:
-https://www.kaggle.com/datasets/sobhanmoosavi/us-accidents * License: CC BY-SA
-4.0 ## Python Package: `whyshift` Here we provide the scripts to get data in
-our proposed settings. #### Install the package ``` pip3 install whyshift ```
-#### For settings utilizing ACS Income, Public Coverage, Mobility datasets *
+Patterns](#different-distribution-shift-patterns) 4. [Implemented Algorithms]
+(#implemented-algorithms) 5. [License and terms of use](#license-and-terms-of-
+use) 6. [References](#references) ## Dataset Access Here we provide the access
+links for the 5 datasets used in our benchmark. #### ACS Income * The task is
+to predict whether an individualâs income is above \$50,000. * Access link:
+https://github.com/socialfoundations/folktables * Reference: Ding, F., Hardt,
+M., Miller, J., & Schmidt, L. (2021). Retiring adult: New datasets for fair
+machine learning. Advances in neural information processing systems, 34, 6478-
+6490. * License: MIT License #### ACS PubCov * The task is to predict whether
+an individual has public health insurance. * Access link: https://github.com/
+socialfoundations/folktables * Reference: Ding, F., Hardt, M., Miller, J., &
+Schmidt, L. (2021). Retiring adult: New datasets for fair machine learning.
+Advances in neural information processing systems, 34, 6478-6490. * License:
+MIT License #### ACS Mobility * The task is to predict whether an individual
+had the same residential address one year ago. * Access link: https://
+github.com/socialfoundations/folktables * Reference: Ding, F., Hardt, M.,
+Miller, J., & Schmidt, L. (2021). Retiring adult: New datasets for fair machine
+learning. Advances in neural information processing systems, 34, 6478-6490. *
+License: MIT License #### Taxi Dataset * The task is to predict whether the
+total ride duration time exceeds 30 minutes, based on location and temporal
+features. * Access link: * https://www.kaggle.com/datasets/mnavas/taxi-routes-
+for-mexico-city-and-quito * https://www.kaggle.com/competitions/nyc-taxi-trip-
+duration/data * License: CC BY-SA 4.0 #### US Accident Dataset * The task is to
+predict whether an accident is severe (long delay) or not (short delay) based
+on weather features and Road condition features. * Access link: https://
+www.kaggle.com/datasets/sobhanmoosavi/us-accidents * License: CC BY-SA 4.0 ##
+Python Package: `whyshift` Here we provide the scripts to get data in our
+proposed settings. #### Install the package ``` pip3 install whyshift ``` ####
+For settings utilizing ACS Income, Public Coverage, Mobility datasets *
 `get_data(task, state, year, need_preprocess, root_dir)` function * `task`
 values: 'income', 'pubcov', 'mobility' * examples: ```python from whyshift
 import get_data # for ACS Income X, y, feature_names = get_data("income", "CA",
 True, './datasets/acs/', 2018) # for ACS Public Coverage X, y, feature_names =
 get_data("pubcov", "CA", True, './datasets/acs/', 2018) # for ACS Mobility X,
 y, feature_names = get_data("mobility", "CA", True, './datasets/acs/', 2018)
 ``` * support `state` values: * ['AL', 'AK', 'AZ', 'AR', 'CA', 'CO', 'CT',
@@ -98,26 +99,37 @@
 target domains (except the last setting). In our main body, we select only one
 target domain for each setting. We report the `Dom. Ratio` to represent the
 dominant ratio of $Y|X$ shifts or $X$ shifts in source-target pairs with
 performance degradation larger than **5** percentage points in each setting.
 For example, "$Y|X$: 13/14" means that there are 14 source-target pairs in
 Setting 1 with degradation larger than 5 percentage points and 13 out of them
 with over 50\% degradation attributed to $Y|X$ shifts. We use XGBoost to
-measure this. ## License and terms of use Our benchmark is built upon
-`Folktables`. The License of `Folktables` is: ``` Folktables provides code to
-download data from the American Community Survey (ACS) Public Use Microdata
-Sample (PUMS) files managed by the US Census Bureau. The data itself is
-governed by the terms of use provided by the Census Bureau. For more
-information, see https://www.census.gov/data/developers/about/terms-of-
-service.html The Adult reconstruction dataset is a subsample of the IPUMS CPS
-data available from https://cps.ipums.org/. The data are intended for
+measure this. ## Implemented Algorithms In our `whyshift` package, we also
+implement several algorithms for tabular data classification, including
+`Logistic Regression`, `MLP`, `SVM`, `Random Forest`, `XGBoost`, `LightGBM`,
+`GBM`, $\chi^2$/CVaR-`DRO/DORO`, `Group DRO`, `Simple-Reweighting`, `JTT`,
+`Fairness-In/Postprocess` and `DWR` methods. ```python # use the implemented
+methods algo = fetch_model(method_name) ``` Note that the supported method
+names are: ```python method_name_list = ['lr','svm','xgb', 'lightgbm', 'rf',
+'dwr', 'jtt','suby', 'subg', 'rwy', 'rwg',
+'FairPostprocess_exp','FairInprocess_dp', 'FairPostprocess_threshold',
+'FairInprocess_eo', 'FairInprocess_error_parity','chi_dro',
+'chi_doro','cvar_dro','cvar_doro','group_dro'] ``` ## License and terms of use
+Our benchmark is built upon `Folktables`. The License of `Folktables` is: ```
+Folktables provides code to download data from the American Community Survey
+(ACS) Public Use Microdata Sample (PUMS) files managed by the US Census Bureau.
+The data itself is governed by the terms of use provided by the Census Bureau.
+For more information, see https://www.census.gov/data/developers/about/terms-
+of-service.html The Adult reconstruction dataset is a subsample of the IPUMS
+CPS data available from https://cps.ipums.org/. The data are intended for
 replication purposes only. Individuals analyzing the data for other purposes
 must submit a separate data extract request directly via IPUMS CPS. Individuals
 are not to redistribute the data without permission. Contact ipums@umn.edu for
 redistribution requests. ``` Besides, for US Accident and Taxi data from
 `kaggle`, individuals should follow the their Licenses, see https://
 www.kaggle.com/datasets/sobhanmoosavi/us-accidents and https://www.kaggle.com/
 competitions/nyc-taxi-trip-duration/data. ## References [1] Ding, F., Hardt,
 M., Miller, J., & Schmidt, L. (2021). Retiring adult: New datasets for fair
 machine learning. Advances in neural information processing systems, 34, 6478-
-6490. ps: we modify the `folktables` code to support `year` before 2014, and
-therefore we involve it in our package.
+6490. * We modify the `folktables` code to support `year` before 2014, and
+involve the revised version in our package. * Part of the algorithm codes are
+used from the codebase.
```

### Comparing `whyshift-0.0.4/setup.py` & `whyshift-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_packages
 
 setup(
     name='whyshift',
-    version='0.0.4',    
+    version='0.0.5',    
     description='A package of various specified distribution shift patterns of out-of-distributoin generalization problem on tabular data',
     url='https://github.com/namkoong-lab/whyshift',
     author='Jiashuo Liu, Tianyu Wang, Peng Cui, Hongseok Namkoong',
     author_email='liujiashuo77@gmail.com, tw2837@columbia.edu, cuip@tsinghua.edu.cn, namkoong@gsb.columbia.edu',
     packages=find_packages(),
     install_requires=['pandas',
                       'numpy',
```

### Comparing `whyshift-0.0.4/whyshift/algorithm.py` & `whyshift-0.0.5/whyshift/algorithm.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.4/whyshift/dataset.py` & `whyshift-0.0.5/whyshift/dataset.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.4/whyshift/folktables/acs.py` & `whyshift-0.0.5/whyshift/folktables/acs.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.4/whyshift/folktables/dataset.py` & `whyshift-0.0.5/whyshift/folktables/dataset.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.4/whyshift/folktables/exceptions.py` & `whyshift-0.0.5/whyshift/folktables/exceptions.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.4/whyshift/folktables/folktables.py` & `whyshift-0.0.5/whyshift/folktables/folktables.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.4/whyshift/folktables/load_acs.py` & `whyshift-0.0.5/whyshift/folktables/load_acs.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.4/whyshift/folktables/utils/download_utils.py` & `whyshift-0.0.5/whyshift/folktables/utils/download_utils.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.4/whyshift/folktables/utils/files_resources.py` & `whyshift-0.0.5/whyshift/folktables/utils/files_resources.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.4/whyshift/folktables/utils/load_utils.py` & `whyshift-0.0.5/whyshift/folktables/utils/load_utils.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.4/whyshift/folktables_utils.py` & `whyshift-0.0.5/whyshift/folktables_utils.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.4/whyshift/methods/marginal_dro_criterion.py` & `whyshift-0.0.5/whyshift/methods/marginal_dro_criterion.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.4/whyshift/methods/model_family.py` & `whyshift-0.0.5/whyshift/methods/model_family.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.4/whyshift/methods/model_util.py` & `whyshift-0.0.5/whyshift/methods/model_util.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.4/whyshift/methods/robust_loss.py` & `whyshift-0.0.5/whyshift/methods/robust_loss.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.4/whyshift/utils.py` & `whyshift-0.0.5/whyshift/utils.py`

 * *Files identical despite different names*

### Comparing `whyshift-0.0.4/whyshift.egg-info/PKG-INFO` & `whyshift-0.0.5/whyshift.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whyshift
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package of various specified distribution shift patterns of out-of-distributoin generalization problem on tabular data
 Home-page: https://github.com/namkoong-lab/whyshift
 Author: Jiashuo Liu, Tianyu Wang, Peng Cui, Hongseok Namkoong
 Author-email: liujiashuo77@gmail.com, tw2837@columbia.edu, cuip@tsinghua.edu.cn, namkoong@gsb.columbia.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

### Comparing `whyshift-0.0.4/whyshift.egg-info/SOURCES.txt` & `whyshift-0.0.5/whyshift.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 setup.py
 whyshift/__init__.py
 whyshift/algorithm.py
 whyshift/dataset.py
+whyshift/disde.py
 whyshift/folktables_utils.py
 whyshift/utils.py
 whyshift.egg-info/PKG-INFO
 whyshift.egg-info/SOURCES.txt
 whyshift.egg-info/dependency_links.txt
 whyshift.egg-info/requires.txt
 whyshift.egg-info/top_level.txt
```

