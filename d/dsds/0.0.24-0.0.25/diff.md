# Comparing `tmp/dsds-0.0.24.tar.gz` & `tmp/dsds-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsds-0.0.24.tar", last modified: Fri Jul 28 04:51:50 2023, max compression
+gzip compressed data
```

## Comparing `dsds-0.0.24.tar` & `dsds-0.0.25.tar`

### file list

```diff
@@ -1,26 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 04:51:50.610767 dsds-0.0.24/
--rw-rw-rw-   0        0        0     1079 2023-06-23 04:44:14.000000 dsds-0.0.24/LICENSE
--rw-rw-rw-   0        0        0     9216 2023-07-28 04:51:50.610767 dsds-0.0.24/PKG-INFO
--rw-rw-rw-   0        0        0     6844 2023-07-27 22:37:38.000000 dsds-0.0.24/README.md
--rw-rw-rw-   0        0        0     1396 2023-07-28 04:45:59.000000 dsds-0.0.24/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-28 04:51:50.610767 dsds-0.0.24/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-28 04:51:50.577413 dsds-0.0.24/src/
-drwxrwxrwx   0        0        0        0 2023-07-28 04:51:50.595138 dsds-0.0.24/src/dsds/
--rw-rw-rw-   0        0        0       87 2023-07-28 04:46:03.000000 dsds-0.0.24/src/dsds/__init__.py
--rw-rw-rw-   0        0        0    14005 2023-07-28 04:44:23.000000 dsds-0.0.24/src/dsds/blueprint.py
--rw-rw-rw-   0        0        0      206 2023-07-27 04:58:44.000000 dsds-0.0.24/src/dsds/compare.py
--rw-rw-rw-   0        0        0     3766 2023-06-20 23:18:47.000000 dsds-0.0.24/src/dsds/eda_text.py
--rw-rw-rw-   0        0        0    26636 2023-07-27 05:09:06.000000 dsds-0.0.24/src/dsds/encoders.py
--rw-rw-rw-   0        0        0    37634 2023-07-25 05:03:42.000000 dsds-0.0.24/src/dsds/fs.py
--rw-rw-rw-   0        0        0    11007 2023-07-26 03:13:51.000000 dsds-0.0.24/src/dsds/metrics.py
--rw-rw-rw-   0        0        0    38259 2023-07-28 04:30:11.000000 dsds-0.0.24/src/dsds/prescreen.py
--rw-rw-rw-   0        0        0    20420 2023-07-28 04:43:26.000000 dsds-0.0.24/src/dsds/sample.py
--rw-rw-rw-   0        0        0    28954 2023-07-28 04:16:34.000000 dsds-0.0.24/src/dsds/transform.py
--rw-rw-rw-   0        0        0     3522 2023-07-28 04:50:51.000000 dsds-0.0.24/src/dsds/type_alias.py
--rw-rw-rw-   0        0        0    14259 2023-07-27 04:37:24.000000 dsds-0.0.24/src/dsds/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-28 04:51:50.610767 dsds-0.0.24/src/dsds.egg-info/
--rw-rw-rw-   0        0        0     9216 2023-07-28 04:51:50.000000 dsds-0.0.24/src/dsds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      435 2023-07-28 04:51:50.000000 dsds-0.0.24/src/dsds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 04:51:50.000000 dsds-0.0.24/src/dsds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      171 2023-07-28 04:51:50.000000 dsds-0.0.24/src/dsds.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-28 04:51:50.000000 dsds-0.0.24/src/dsds.egg-info/top_level.txt
+-rw-r--r--   0        0        0      545 1970-01-01 00:00:00.000000 dsds-0.0.25/Cargo.toml
+-rw-rw-r--   0     1000     1000     2807 2023-08-04 22:21:44.000000 dsds-0.0.25/.github/workflows/CI.yml
+-rw-rw-r--   0     1000     1000     3570 2023-08-09 05:13:31.000000 dsds-0.0.25/.gitignore
+-rw-rw-r--   0     1000     1000     4575 2023-08-04 22:21:44.000000 dsds-0.0.25/CONTRIBUTING.md
+-rw-rw-r--   0     1000     1000    50219 2023-08-09 05:13:34.000000 dsds-0.0.25/Cargo.lock
+-rw-rw-r--   0     1000     1000     1059 2023-07-02 13:17:50.000000 dsds-0.0.25/LICENSE
+-rw-rw-r--   0     1000     1000     6912 2023-08-04 22:21:44.000000 dsds-0.0.25/README.md
+-rw-rw-r--   0     1000     1000   126109 2023-07-02 13:17:50.000000 dsds-0.0.25/data/advertising.csv
+-rw-rw-r--   0     1000     1000    21830 2023-08-04 22:21:44.000000 dsds-0.0.25/examples/dsds_comparisons.ipynb
+-rw-rw-r--   0     1000     1000    37625 2023-08-04 22:21:44.000000 dsds-0.0.25/examples/encoders.ipynb
+-rw-rw-r--   0     1000     1000    95281 2023-08-04 22:21:44.000000 dsds-0.0.25/examples/general_usage.ipynb
+-rw-rw-r--   0     1000     1000     5602 2023-08-04 22:21:44.000000 dsds-0.0.25/examples/pipeline.ipynb
+-rw-rw-r--   0     1000     1000     5204 2023-08-09 05:35:19.000000 dsds-0.0.25/examples/test.ipynb
+-rw-rw-r--   0     1000     1000    60821 2023-08-04 22:21:44.000000 dsds-0.0.25/pics/impute.PNG
+-rw-rw-r--   0     1000     1000    54079 2023-08-04 22:21:44.000000 dsds-0.0.25/pics/logloss.PNG
+-rw-rw-r--   0     1000     1000    34494 2023-08-04 22:21:44.000000 dsds-0.0.25/pics/nlp.PNG
+-rw-rw-r--   0     1000     1000     1377 2023-08-09 05:32:47.000000 dsds-0.0.25/pyproject.toml
+-rw-rw-r--   0     1000     1000       81 2023-08-04 22:21:44.000000 dsds-0.0.25/python/dsds/__init__.py
+-rw-rw-r--   0     1000     1000    15099 2023-08-04 22:21:44.000000 dsds-0.0.25/python/dsds/blueprint.py
+-rw-rw-r--   0     1000     1000      201 2023-08-04 22:21:44.000000 dsds-0.0.25/python/dsds/compare.py
+-rw-rw-r--   0     1000     1000    26143 2023-08-09 05:13:31.000000 dsds-0.0.25/python/dsds/encoders.py
+-rw-rw-r--   0     1000     1000    36542 2023-08-09 05:13:31.000000 dsds-0.0.25/python/dsds/fs.py
+-rw-rw-r--   0     1000     1000    18562 2023-08-09 05:13:31.000000 dsds-0.0.25/python/dsds/metrics.py
+-rw-rw-r--   0     1000     1000    41634 2023-08-09 05:13:31.000000 dsds-0.0.25/python/dsds/prescreen.py
+-rw-rw-r--   0     1000     1000    30338 2023-08-04 22:21:44.000000 dsds-0.0.25/python/dsds/sample.py
+-rw-rw-r--   0     1000     1000    14077 2023-08-09 05:13:31.000000 dsds-0.0.25/python/dsds/text.py
+-rw-rw-r--   0     1000     1000    35523 2023-08-09 05:13:31.000000 dsds-0.0.25/python/dsds/transform.py
+-rw-rw-r--   0     1000     1000     3713 2023-08-09 05:13:31.000000 dsds-0.0.25/python/dsds/type_alias.py
+-rw-rw-r--   0     1000     1000    13639 2023-08-04 22:21:44.000000 dsds-0.0.25/python/dsds/utils.py
+-rw-rw-r--   0     1000     1000     5868 2023-08-09 05:20:03.000000 dsds-0.0.25/src/functions/metrics.rs
+-rw-rw-r--   0     1000     1000     1127 2023-08-09 05:13:31.000000 dsds-0.0.25/src/functions/mod.rs
+-rw-rw-r--   0     1000     1000      514 2023-08-09 05:13:31.000000 dsds-0.0.25/src/functions/utils.rs
+-rw-rw-r--   0     1000     1000     1739 2023-08-09 05:20:03.000000 dsds-0.0.25/src/lib.rs
+-rw-rw-r--   0     1000     1000      775 2023-08-09 05:13:31.000000 dsds-0.0.25/src/main.rs
+-rw-rw-r--   0     1000     1000    24192 2023-08-04 22:21:44.000000 dsds-0.0.25/src/snowball/algorithms/english_stemmer.rs
+-rw-rw-r--   0     1000     1000      110 2023-08-04 22:21:44.000000 dsds-0.0.25/src/snowball/algorithms/mod.rs
+-rw-rw-r--   0     1000     1000      260 2023-08-04 22:21:44.000000 dsds-0.0.25/src/snowball/among.rs
+-rw-rw-r--   0     1000     1000      219 2023-08-04 22:21:44.000000 dsds-0.0.25/src/snowball/mod.rs
+-rw-rw-r--   0     1000     1000    12897 2023-08-04 22:21:44.000000 dsds-0.0.25/src/snowball/snowball_env.rs
+-rw-rw-r--   0     1000     1000     2289 2023-08-09 05:13:31.000000 dsds-0.0.25/src/text/consts.rs
+-rw-rw-r--   0     1000     1000     3076 2023-08-09 05:20:03.000000 dsds-0.0.25/src/text/mod.rs
+-rw-rw-r--   0     1000     1000     7188 2023-08-09 05:20:03.000000 dsds-0.0.25/src/text/text.rs
+-rw-r--r--   0        0        0     8505 1970-01-01 00:00:00.000000 dsds-0.0.25/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `dsds-0.0.24/LICENSE` & `dsds-0.0.25/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 T.Q
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2023 T.Q
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `dsds-0.0.24/PKG-INFO` & `dsds-0.0.25/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,162 +1,150 @@
-Metadata-Version: 2.1
-Name: dsds
-Version: 0.0.24
-Summary: A feature screening, selection, EDA, pipeline building and management tool centered around Polars dataframe.
-Author-email: Tianren Qin <tq9695@gmail.com>
-License: MIT License
-        
-        Copyright (c) 2023 T.Q
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-Project-URL: Homepage, https://github.com/abstractqqq/dsds
-Keywords: data pipeline,EDA,feature-screening,feature-selection
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: scikit-learn
-Provides-Extra: xgboost
-Provides-Extra: lightgbm
-Provides-Extra: all
-License-File: LICENSE
-
-# Welcome to the Dark Side of Data Science (DSDS)
-
-This package is in pre-alpha stage. Please read CONTRIBUTING.md if you are a developer interested in contributing to this package. Also see disclaimer in the end.
-
-Welcome to DSDS, a data science package that aims to be an improvement over a subset of sklearn's functionality, primarily in the following areas:
-
-1. Providing practical feature prescreen (immediate detection and removal of useless featuers, data profiling, etc.)
-2. Fast and furious feature selection (significantly faster F-score, MRMR, mutual_info_score, etc.)
-3. Cleaner pipeline construction and management (See examples below.)
-4. Compatible with Polars LazyFrames (Yes! Pipelines can enjoy the benefits of query optimization too!)
-5. Functional interface and fully typed functions for a better developer experience. No mixins, no multiple inheritance. No classes. No nonsenses.
-
-DSDS is built around your favorite: [Polars Dataframe](https://github.com/pola-rs/polars)
-
-## Usage
-
-Practical Feature Prescreen
-```python
-from dsds.prescreen import (
-    remove_if_exists
-    , regex_removal
-    , pattern_removal
-    , var_removal
-    , null_removal
-    , unique_removal
-    , constant_removal
-    , date_removal
-    , non_numeric_removal
-    , get_unique_count
-    , get_string_cols
-    , suggest_normal
-    , discrete_inferral
-) # and a lot more!
-
-```
-
-Functional Pipeline Interface which supports both Eager and LazyFrames! And it can be pickled and load back and reapplied! See more in the examples on github.
-
-```python
-from dsds.prescreen import *
-from dsds.transform import *
-
-input_df = df.lazy()
-output = input_df.pipe(var_removal, threshold = 0.5, target = "Clicked on Ad")\
-    .pipe(binary_encode)\
-    .pipe(ordinal_auto_encode, cols = ["City", "Country"])\
-    .pipe(impute, cols=["Daily Internet Usage", "Daily Internet Usage Band", "Area Income Band"], strategy="median")\
-    .pipe(impute, cols=["Area Income"], strategy = "mean")\
-    .pipe(scale, cols=["Area Income", "Daily Internet Usage"])\
-    .pipe(one_hot_encode, cols= ["One_Hot_Test"])\
-    .pipe(remove_if_exists, cols = ["Ad Topic Line", "Timestamp"])\
-    .pipe(mutual_info_selector, target = "Clicked on Ad", top_k = 12)
-```
-
-Performance without sacrificing user experience. See ./examples/dsds_comparisons.ipynb
-
-![Screenshot](./pics/impute.PNG)
-
-## Dependencies
-
-Python 3.9, 3.10, 3.11+ is recommended. We are forward looking. 
-
-It should run on all versions >= 3.9. But I haven't tested 3.9 and 3.10 thoroughly.
-
-pip install polars scipy numpy
-
-pip install dsds[all]
-
-Note: scikit-learn, lightgbm, xgboost are needed for full functionalities. 
-
-# Why DSDS?
-
-(1) Fast and furious
-
-(2) Simple, single-purpose, clean, optimized and fully typed functions
-
-(3) Easy to extend
-
-(4) Supports Polars LazyFrame, and therefore query optimizations in pipeline.
-
-(5) No boilerplate
-
-# Why the name DSDS?
-
-I choose the name Dark Side of Data Science because data pipelines are like real life pipelines, buried under the ground. It is the most foundational work that is also the most under-appreciated component of any data science project. Feature selection is often considered a dark art, too. So the name DarkSide/dsds really makes sense to me.
-
-# Why is this package dependent on Sklearn?
-
-You are right in the sense that this package does its best to separate itself from sklearn because of its focus and design. You do not need sklearn for pipelines, transformations, metrics, or the prescreen modules. However, for the fs (feature selection) module, right now there is no other high quality, tried and true package for random forest and logistic regression. The feature importance from these two models are used in some feature selection algorithms. Feel free to let me know if there are alternatives.
-
-# Why not write more functionalities in Rust?
-
-Yes. I will. I am not confident enough with my Rust skill at the moment. I am slowly learning more Rust and hopefully we can delegate more heavy work to Rust. The immediate benefit of using more Rust will be (1) slightly more memory efficient, and (2) slightly faster. I do not expect huge speed boost because most code are written in Polars already. There are some cases when a lot of Python stuff is added (lists and for loops, etc.). But we definitely need to evaluate the gain by using Rust more carefully in the future.
-
-# Disclaimer
-
-I do not claim dsds is a superior package to any other traditional machine learning libraries. In fact no one can make this claim. Each package has their own flavor, and there are things that people can disagree with. Disagreements do not translate to contempt or hatred. I primarily set out to make this project because:
-
-1. I want to learn more about machine learning engineering
-2. I want to improve my coding skill
-3. I see opportunies to make things run faster using Polars without relying on bigger machines on the cloud. I want to make this happen for everybody.
-4. I don't think OOP is right for scientific computing.
-
-Everyone has their own bias. I believe in the functional style for scientific computing. I don't like the OOP style adopted by so many other packages, especially the one used in Sklearn pipelines. If you want to discuss, please kindly send me a message on discord. Please do not cherry pick points and claim that my code is **** just because you have never seen functional codebase or projects done in this style. I do not claim to have the best style of code either. OOP elements are still used in this project because it is inevitable in Python.
-
-That said, since performance and functional design are the two major pillars of this project, I will include a lot of benchmarks and code that showcase the style differences. A lot of benchmarks will be done vs. Scikit-learn because Scikit-learn is the de facto "standard" in the tranditional machine learning space. I do this not because I want to prove dsds is superior, but because I want to show the improvement and show people that dsds achieves what it aims to achieve, an improvement over a subset of Scikit-learn's functionalities (in the areas that I set out to improve on, e.g. performance and 'style').
-
-Every few days there is a new javascript framework. Why can't data scientists challenge the design of Scikit-learn? I started learning using Scikit-learn, like 90% of all the data scientists out there. I am free to express my opinions and criticisms. 
-
-No package is perfect and you are free to like/hate it. Just don't be complaining online without ever thinking deeply about machine learning infra and bottlenecks in machine learning pipelines. Don't hate on things because they are different.
-
-# Contribution
-
-See CONTRIBUTING.md for my contact info.
+Metadata-Version: 2.1
+Name: dsds
+Version: 0.0.25
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Rust
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
+Requires-Dist: polars >=0.18.10
+Requires-Dist: scipy >=1.11.1
+Requires-Dist: numpy
+Requires-Dist: tqdm
+Requires-Dist: pyarrow >=12.0
+Requires-Dist: typing_extensions >=4.0.1
+Requires-Dist: scikit-learn ; extra == 'scikit-learn'
+Requires-Dist: xgboost ; extra == 'xgboost'
+Requires-Dist: lightgbm ; extra == 'lightgbm'
+Requires-Dist: scikit-learn ; extra == 'all'
+Requires-Dist: xgboost ; extra == 'all'
+Requires-Dist: lightgbm ; extra == 'all'
+Requires-Dist: data-pipeline ; extra == 'keywords'
+Requires-Dist: EDA ; extra == 'keywords'
+Requires-Dist: feature-screening ; extra == 'keywords'
+Requires-Dist: feature-selection ; extra == 'keywords'
+Provides-Extra: scikit-learn
+Provides-Extra: xgboost
+Provides-Extra: lightgbm
+Provides-Extra: all
+Provides-Extra: keywords
+License-File: LICENSE
+Author-email: Tianren Qin <tq9695@gmail.com>
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+
+# Welcome to the Dark Side of Data Science (DSDS)
+
+This package is in pre-alpha stage. Please read CONTRIBUTING.md if you are a developer interested in contributing to this package. Also see disclaimer in the end.
+
+Welcome to DSDS, a data science package that aims to be an improvement over a subset of sklearn's functionality, primarily in the following areas:
+
+1. Providing practical feature prescreen (immediate detection and removal of useless featuers, data profiling, etc.)
+2. Fast and furious feature selection (significantly faster F-score, MRMR, mutual_info_score, etc.)
+3. Cleaner pipeline construction and management (See examples below.)
+4. Compatible with Polars LazyFrames (Yes! Pipelines can enjoy the benefits of query optimization too!)
+5. Functional interface and fully typed functions for a better developer experience. No mixins, no multiple inheritance. No classes. No nonsenses.
+6. Even more performance for all of the above with the power of Rust!
+
+DSDS is built around your favorite: [Polars Dataframe](https://github.com/pola-rs/polars)
+
+## Usage
+
+Practical Feature Prescreen
+```python
+from dsds.prescreen import (
+    remove_if_exists
+    , regex_removal
+    , pattern_removal
+    , var_removal
+    , null_removal
+    , unique_removal
+    , constant_removal
+    , date_removal
+    , non_numeric_removal
+    , get_unique_count
+    , get_string_cols
+    , suggest_normal
+    , discrete_inferral
+) # and a lot more!
+
+```
+
+Functional Pipeline Interface which supports both Eager and LazyFrames! And it can be pickled and load back and reapplied! See more in the examples on github.
+
+```python
+from dsds.prescreen import *
+from dsds.transform import *
+
+input_df = df.lazy()
+output = input_df.pipe(var_removal, threshold = 0.5, target = "Clicked on Ad")\
+    .pipe(binary_encode)\
+    .pipe(ordinal_auto_encode, cols = ["City", "Country"])\
+    .pipe(impute, cols=["Daily Internet Usage", "Daily Internet Usage Band", "Area Income Band"], strategy="median")\
+    .pipe(impute, cols=["Area Income"], strategy = "mean")\
+    .pipe(scale, cols=["Area Income", "Daily Internet Usage"])\
+    .pipe(one_hot_encode, cols= ["One_Hot_Test"])\
+    .pipe(remove_if_exists, cols = ["Ad Topic Line", "Timestamp"])\
+    .pipe(mutual_info_selector, target = "Clicked on Ad", top_k = 12)
+```
+
+Performance without sacrificing user experience.
+
+![Screenshot](./pics/impute.PNG)
+
+And yes, significantly faster than NumPy in many cases
+
+![Screenshot](./pics/logloss.PNG)
+
+Fast and Ergonomic traditional NLP. In comparison, Scikit-learn's CountVectorizer does not perform stemming, and treats words with the same stem differently, does not filter out useless words like 'an', and took 2.2s for the same run.
+
+![Screenshot](./pics/nlp.PNG)
+
+## Dependencies
+
+Python 3.9, 3.10, 3.11+ is recommended.
+
+It should run on all versions >= 3.9.
+
+Note: scikit-learn, lightgbm, xgboost and nltk are needed for full functionalities. 
+
+
+# Why the name DSDS?
+
+I choose the name Dark Side of Data Science because data pipelines are like real life pipelines, buried under the ground. It is the most foundational work that is also the most under-appreciated component of any data science project. Feature selection is often considered a dark art, too. So the name DarkSide/dsds really makes sense to me.
+
+# Why is this package dependent on Sklearn?
+
+You are right in the sense that this package does its best to separate itself from sklearn because of its focus and design. You do not need sklearn for pipelines, transformations, metrics, or the prescreen modules. However, for the fs (feature selection) module, right now there is no other high quality, tried and true package for random forest and logistic regression. The feature importance from these two models are used in some feature selection algorithms. Feel free to let me know if there are alternatives.
+
+# Why not write more in Rust?
+
+Yes. I am. I recently resumed working on traditional NLP, and this is an area where Rust really shines. It is well-known that Stemmers in NLTK has terrible performance, but stemming is an important operations for many traditional NLP algorithms. To combat this, I have decided to move stemming and other heavy string manipulations to Rust and leave only a very thin wrapper in Python. That said, using Rust can greatly improve performance in many other modules, not just dsds.text. But because development in Rust is relatively slow, I do not want to blindly 'rewrite' in Rust. In near future, I do not have plans to 'rewrite' in Rust, if performance gain is less than 10%.
+
+# Disclaimer
+
+I do not claim dsds is a superior package to any other traditional machine learning libraries. In fact no one can make this claim. Each package has their own flavor, and there are things that people can disagree with. Disagreements do not translate to contempt or hatred. I primarily set out to make this project because:
+
+1. I want to learn more about machine learning engineering
+2. I want to improve my coding skill
+3. I see opportunies to make things run faster using Polars without relying on bigger machines on the cloud. I want to make this happen for everybody.
+4. I don't think OOP is right for scientific computing.
+
+Everyone has their own bias. I believe in the functional style for scientific computing. I don't like the OOP style adopted by so many other packages, especially the one used in Sklearn pipelines. If you want to discuss, please kindly send me a message on discord. Please do not cherry pick points and claim that my code is **** just because you have never seen functional codebase or projects done in this style. I do not claim to have the best style of code either. OOP elements are still used in this project because it is inevitable in Python.
+
+That said, since performance and functional design are the two major pillars of this project, I will include a lot of benchmarks and code that showcase the style differences. A lot of benchmarks will be done vs. Scikit-learn because Scikit-learn is the de facto "standard" in the tranditional machine learning space. I do this not because I want to prove dsds is superior, but because I want to show the improvement and show people that dsds achieves what it aims to achieve, an improvement over a subset of Scikit-learn's functionalities (in the areas that I set out to improve on, e.g. performance and 'style').
+
+Every few days there is a new javascript framework. Why can't data scientists challenge the design of Scikit-learn? I started learning using Scikit-learn, like 90% of all the data scientists out there. I am free to express my opinions and criticisms. 
+
+No package is perfect and you are free to like/hate it. Just don't be complaining online without ever thinking deeply about machine learning infra and bottlenecks in machine learning pipelines. Don't hate on things because they are different.
+
+# Contribution
+
+See CONTRIBUTING.md for my contact info.
```

### Comparing `dsds-0.0.24/README.md` & `dsds-0.0.25/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,114 +1,108 @@
-# Welcome to the Dark Side of Data Science (DSDS)
-
-This package is in pre-alpha stage. Please read CONTRIBUTING.md if you are a developer interested in contributing to this package. Also see disclaimer in the end.
-
-Welcome to DSDS, a data science package that aims to be an improvement over a subset of sklearn's functionality, primarily in the following areas:
-
-1. Providing practical feature prescreen (immediate detection and removal of useless featuers, data profiling, etc.)
-2. Fast and furious feature selection (significantly faster F-score, MRMR, mutual_info_score, etc.)
-3. Cleaner pipeline construction and management (See examples below.)
-4. Compatible with Polars LazyFrames (Yes! Pipelines can enjoy the benefits of query optimization too!)
-5. Functional interface and fully typed functions for a better developer experience. No mixins, no multiple inheritance. No classes. No nonsenses.
-
-DSDS is built around your favorite: [Polars Dataframe](https://github.com/pola-rs/polars)
-
-## Usage
-
-Practical Feature Prescreen
-```python
-from dsds.prescreen import (
-    remove_if_exists
-    , regex_removal
-    , pattern_removal
-    , var_removal
-    , null_removal
-    , unique_removal
-    , constant_removal
-    , date_removal
-    , non_numeric_removal
-    , get_unique_count
-    , get_string_cols
-    , suggest_normal
-    , discrete_inferral
-) # and a lot more!
-
-```
-
-Functional Pipeline Interface which supports both Eager and LazyFrames! And it can be pickled and load back and reapplied! See more in the examples on github.
-
-```python
-from dsds.prescreen import *
-from dsds.transform import *
-
-input_df = df.lazy()
-output = input_df.pipe(var_removal, threshold = 0.5, target = "Clicked on Ad")\
-    .pipe(binary_encode)\
-    .pipe(ordinal_auto_encode, cols = ["City", "Country"])\
-    .pipe(impute, cols=["Daily Internet Usage", "Daily Internet Usage Band", "Area Income Band"], strategy="median")\
-    .pipe(impute, cols=["Area Income"], strategy = "mean")\
-    .pipe(scale, cols=["Area Income", "Daily Internet Usage"])\
-    .pipe(one_hot_encode, cols= ["One_Hot_Test"])\
-    .pipe(remove_if_exists, cols = ["Ad Topic Line", "Timestamp"])\
-    .pipe(mutual_info_selector, target = "Clicked on Ad", top_k = 12)
-```
-
-Performance without sacrificing user experience. See ./examples/dsds_comparisons.ipynb
-
-![Screenshot](./pics/impute.PNG)
-
-## Dependencies
-
-Python 3.9, 3.10, 3.11+ is recommended. We are forward looking. 
-
-It should run on all versions >= 3.9. But I haven't tested 3.9 and 3.10 thoroughly.
-
-pip install polars scipy numpy
-
-pip install dsds[all]
-
-Note: scikit-learn, lightgbm, xgboost are needed for full functionalities. 
-
-# Why DSDS?
-
-(1) Fast and furious
-
-(2) Simple, single-purpose, clean, optimized and fully typed functions
-
-(3) Easy to extend
-
-(4) Supports Polars LazyFrame, and therefore query optimizations in pipeline.
-
-(5) No boilerplate
-
-# Why the name DSDS?
-
-I choose the name Dark Side of Data Science because data pipelines are like real life pipelines, buried under the ground. It is the most foundational work that is also the most under-appreciated component of any data science project. Feature selection is often considered a dark art, too. So the name DarkSide/dsds really makes sense to me.
-
-# Why is this package dependent on Sklearn?
-
-You are right in the sense that this package does its best to separate itself from sklearn because of its focus and design. You do not need sklearn for pipelines, transformations, metrics, or the prescreen modules. However, for the fs (feature selection) module, right now there is no other high quality, tried and true package for random forest and logistic regression. The feature importance from these two models are used in some feature selection algorithms. Feel free to let me know if there are alternatives.
-
-# Why not write more functionalities in Rust?
-
-Yes. I will. I am not confident enough with my Rust skill at the moment. I am slowly learning more Rust and hopefully we can delegate more heavy work to Rust. The immediate benefit of using more Rust will be (1) slightly more memory efficient, and (2) slightly faster. I do not expect huge speed boost because most code are written in Polars already. There are some cases when a lot of Python stuff is added (lists and for loops, etc.). But we definitely need to evaluate the gain by using Rust more carefully in the future.
-
-# Disclaimer
-
-I do not claim dsds is a superior package to any other traditional machine learning libraries. In fact no one can make this claim. Each package has their own flavor, and there are things that people can disagree with. Disagreements do not translate to contempt or hatred. I primarily set out to make this project because:
-
-1. I want to learn more about machine learning engineering
-2. I want to improve my coding skill
-3. I see opportunies to make things run faster using Polars without relying on bigger machines on the cloud. I want to make this happen for everybody.
-4. I don't think OOP is right for scientific computing.
-
-Everyone has their own bias. I believe in the functional style for scientific computing. I don't like the OOP style adopted by so many other packages, especially the one used in Sklearn pipelines. If you want to discuss, please kindly send me a message on discord. Please do not cherry pick points and claim that my code is **** just because you have never seen functional codebase or projects done in this style. I do not claim to have the best style of code either. OOP elements are still used in this project because it is inevitable in Python.
-
-That said, since performance and functional design are the two major pillars of this project, I will include a lot of benchmarks and code that showcase the style differences. A lot of benchmarks will be done vs. Scikit-learn because Scikit-learn is the de facto "standard" in the tranditional machine learning space. I do this not because I want to prove dsds is superior, but because I want to show the improvement and show people that dsds achieves what it aims to achieve, an improvement over a subset of Scikit-learn's functionalities (in the areas that I set out to improve on, e.g. performance and 'style').
-
-Every few days there is a new javascript framework. Why can't data scientists challenge the design of Scikit-learn? I started learning using Scikit-learn, like 90% of all the data scientists out there. I am free to express my opinions and criticisms. 
-
-No package is perfect and you are free to like/hate it. Just don't be complaining online without ever thinking deeply about machine learning infra and bottlenecks in machine learning pipelines. Don't hate on things because they are different.
-
-# Contribution
-
+# Welcome to the Dark Side of Data Science (DSDS)
+
+This package is in pre-alpha stage. Please read CONTRIBUTING.md if you are a developer interested in contributing to this package. Also see disclaimer in the end.
+
+Welcome to DSDS, a data science package that aims to be an improvement over a subset of sklearn's functionality, primarily in the following areas:
+
+1. Providing practical feature prescreen (immediate detection and removal of useless featuers, data profiling, etc.)
+2. Fast and furious feature selection (significantly faster F-score, MRMR, mutual_info_score, etc.)
+3. Cleaner pipeline construction and management (See examples below.)
+4. Compatible with Polars LazyFrames (Yes! Pipelines can enjoy the benefits of query optimization too!)
+5. Functional interface and fully typed functions for a better developer experience. No mixins, no multiple inheritance. No classes. No nonsenses.
+6. Even more performance for all of the above with the power of Rust!
+
+DSDS is built around your favorite: [Polars Dataframe](https://github.com/pola-rs/polars)
+
+## Usage
+
+Practical Feature Prescreen
+```python
+from dsds.prescreen import (
+    remove_if_exists
+    , regex_removal
+    , pattern_removal
+    , var_removal
+    , null_removal
+    , unique_removal
+    , constant_removal
+    , date_removal
+    , non_numeric_removal
+    , get_unique_count
+    , get_string_cols
+    , suggest_normal
+    , discrete_inferral
+) # and a lot more!
+
+```
+
+Functional Pipeline Interface which supports both Eager and LazyFrames! And it can be pickled and load back and reapplied! See more in the examples on github.
+
+```python
+from dsds.prescreen import *
+from dsds.transform import *
+
+input_df = df.lazy()
+output = input_df.pipe(var_removal, threshold = 0.5, target = "Clicked on Ad")\
+    .pipe(binary_encode)\
+    .pipe(ordinal_auto_encode, cols = ["City", "Country"])\
+    .pipe(impute, cols=["Daily Internet Usage", "Daily Internet Usage Band", "Area Income Band"], strategy="median")\
+    .pipe(impute, cols=["Area Income"], strategy = "mean")\
+    .pipe(scale, cols=["Area Income", "Daily Internet Usage"])\
+    .pipe(one_hot_encode, cols= ["One_Hot_Test"])\
+    .pipe(remove_if_exists, cols = ["Ad Topic Line", "Timestamp"])\
+    .pipe(mutual_info_selector, target = "Clicked on Ad", top_k = 12)
+```
+
+Performance without sacrificing user experience.
+
+![Screenshot](./pics/impute.PNG)
+
+And yes, significantly faster than NumPy in many cases
+
+![Screenshot](./pics/logloss.PNG)
+
+Fast and Ergonomic traditional NLP. In comparison, Scikit-learn's CountVectorizer does not perform stemming, and treats words with the same stem differently, does not filter out useless words like 'an', and took 2.2s for the same run.
+
+![Screenshot](./pics/nlp.PNG)
+
+## Dependencies
+
+Python 3.9, 3.10, 3.11+ is recommended.
+
+It should run on all versions >= 3.9.
+
+Note: scikit-learn, lightgbm, xgboost and nltk are needed for full functionalities. 
+
+
+# Why the name DSDS?
+
+I choose the name Dark Side of Data Science because data pipelines are like real life pipelines, buried under the ground. It is the most foundational work that is also the most under-appreciated component of any data science project. Feature selection is often considered a dark art, too. So the name DarkSide/dsds really makes sense to me.
+
+# Why is this package dependent on Sklearn?
+
+You are right in the sense that this package does its best to separate itself from sklearn because of its focus and design. You do not need sklearn for pipelines, transformations, metrics, or the prescreen modules. However, for the fs (feature selection) module, right now there is no other high quality, tried and true package for random forest and logistic regression. The feature importance from these two models are used in some feature selection algorithms. Feel free to let me know if there are alternatives.
+
+# Why not write more in Rust?
+
+Yes. I am. I recently resumed working on traditional NLP, and this is an area where Rust really shines. It is well-known that Stemmers in NLTK has terrible performance, but stemming is an important operations for many traditional NLP algorithms. To combat this, I have decided to move stemming and other heavy string manipulations to Rust and leave only a very thin wrapper in Python. That said, using Rust can greatly improve performance in many other modules, not just dsds.text. But because development in Rust is relatively slow, I do not want to blindly 'rewrite' in Rust. In near future, I do not have plans to 'rewrite' in Rust, if performance gain is less than 10%.
+
+# Disclaimer
+
+I do not claim dsds is a superior package to any other traditional machine learning libraries. In fact no one can make this claim. Each package has their own flavor, and there are things that people can disagree with. Disagreements do not translate to contempt or hatred. I primarily set out to make this project because:
+
+1. I want to learn more about machine learning engineering
+2. I want to improve my coding skill
+3. I see opportunies to make things run faster using Polars without relying on bigger machines on the cloud. I want to make this happen for everybody.
+4. I don't think OOP is right for scientific computing.
+
+Everyone has their own bias. I believe in the functional style for scientific computing. I don't like the OOP style adopted by so many other packages, especially the one used in Sklearn pipelines. If you want to discuss, please kindly send me a message on discord. Please do not cherry pick points and claim that my code is **** just because you have never seen functional codebase or projects done in this style. I do not claim to have the best style of code either. OOP elements are still used in this project because it is inevitable in Python.
+
+That said, since performance and functional design are the two major pillars of this project, I will include a lot of benchmarks and code that showcase the style differences. A lot of benchmarks will be done vs. Scikit-learn because Scikit-learn is the de facto "standard" in the tranditional machine learning space. I do this not because I want to prove dsds is superior, but because I want to show the improvement and show people that dsds achieves what it aims to achieve, an improvement over a subset of Scikit-learn's functionalities (in the areas that I set out to improve on, e.g. performance and 'style').
+
+Every few days there is a new javascript framework. Why can't data scientists challenge the design of Scikit-learn? I started learning using Scikit-learn, like 90% of all the data scientists out there. I am free to express my opinions and criticisms. 
+
+No package is perfect and you are free to like/hate it. Just don't be complaining online without ever thinking deeply about machine learning infra and bottlenecks in machine learning pipelines. Don't hate on things because they are different.
+
+# Contribution
+
 See CONTRIBUTING.md for my contact info.
```

### Comparing `dsds-0.0.24/src/dsds/blueprint.py` & `dsds-0.0.25/python/dsds/blueprint.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,357 +1,393 @@
-import pickle
-import polars as pl
-import importlib
-import polars.selectors as cs
-from pathlib import Path
-from polars import LazyFrame, DataFrame
-from dataclasses import dataclass
-from typing import (
-    Any
-    , Union
-    , Iterable
-    , Optional
-)
-from polars.type_aliases import IntoExpr
-from .type_alias import (
-    PolarsFrame
-    , ActionType
-    , PipeFunction
-    , ClassifModel
-    , RegressionModel
-)
-
-# P = ParamSpec("P")
-
-@dataclass
-class MapDict:
-    left_col: str # Join on this column, and this column will be replaced by right and dropped.
-    ref: dict # The right table as a dictionary
-    right_col: str
-    default: Optional[Any]
-
-@dataclass
-class Step:
-    action:ActionType
-    associated_data: Union[list[pl.Expr], MapDict, list[str], cs._selector_proxy_, dict[str, Any], pl.Expr]
-    # First is everything that can be done with with_columns
-    # Second is a 1-to-1 encoder (MapDict)
-    # Third is a drop/select (list[str] and cs._selector_proxy_)
-    # Fourth is add_func (dict[str, Any]), or add_classif/add_regression
-    # Fifth is a filter statement (pl.Expr)
-
-# Break associated_data into parts?
-
-@pl.api.register_lazyframe_namespace("blueprint")
-class Blueprint:
-    def __init__(self, ldf: LazyFrame):
-        self._ldf = ldf
-        self.steps:list[Step] = []
-
-    def as_str(self, n:int) -> str:
-        output = ""
-        start = max(len(self.steps) + n, 0) if n < 0 else 0
-        till = len(self.steps) if n < 0 else min(n, len(self.steps))
-        for k,s in enumerate(self.steps):
-            if k < start:
-                continue
-            output += f"Step {k} | Action: {s.action}\n"
-            if s.action == "with_columns":
-                output += "Details: \n"
-                for i,expr in enumerate(s.associated_data):
-                    output += f"({i+1}) {expr}\n"
-            elif s.action == "apply_func":
-                d:dict = s.associated_data
-                output += f"Function Module: {d['module']}, Function Name: {d['name']}\n"
-                output += "Parameters:\n"
-                for k,v in d["kwargs"].items():
-                    output += f"{k} = {v},\n"
-            elif s.action == "filter":
-                output += f"By condition: {s.associated_data}\n"
-            elif s.action in ("classif", "regression"):
-                output += f"Model: {s.associated_data['model'].__class__}\n"
-                features = s.associated_data.get('features', None)
-                if features is None:
-                    output += "Using all non-target columns as features.\n"
-                else:
-                    output += f"Using the features {s.associated_data['features']}\n"
-                output += f"Appends {s.associated_data['score_col']} to dataframe."
-            else:
-                output += str(s.associated_data)
-            output += "\n\n"
-            if k > till:
-                break
-
-        return output
-    
-    def show(self, n:int) -> None:
-        print(self.as_str(n))
-
-    def __str__(self) -> str:
-        return self.as_str(len(self.steps))
-    
-    def __len__(self) -> int:
-        return len(self.steps)
-    
-    def _ipython_display_(self):
-        print(self)
-
-    @staticmethod
-    def _map_dict(df:PolarsFrame, map_dict:MapDict) -> PolarsFrame:
-        temp = pl.from_dict(map_dict.ref) # Always an eager read
-        if isinstance(df, pl.LazyFrame):
-            temp = temp.lazy()
-        
-        if map_dict.default is None:
-            return df.join(temp, on = map_dict.left_col).with_columns(
-                pl.col(map_dict.right_col).alias(map_dict.left_col)
-            ).drop(map_dict.right_col)
-        else:
-            return df.join(temp, on = map_dict.left_col, how = "left").with_columns(
-                pl.col(map_dict.right_col).fill_null(map_dict.default).alias(map_dict.left_col)
-            ).drop(map_dict.right_col)
-        
-    @staticmethod
-    def _process_classif(
-        df: PolarsFrame
-        , model:ClassifModel
-        , target: Optional[str] = None
-        , features: Optional[list[str]] = None
-        , score_idx:int = -1 
-        , score_col:str = "model_score"
-    ) -> PolarsFrame:
-        
-        if features is None:
-            features = df.columns
-        if target is not None:
-            if target in features:
-                features.remove(target)
-
-        data = df.lazy().collect()
-        output = data.insert_at_idx(0, pl.Series(
-            score_col, model.predict_proba(data.select(features))[:, score_idx]
-        ))
-        if isinstance(df, pl.LazyFrame):
-            return output.lazy()
-        return output
-    
-    @staticmethod
-    def _process_regression(
-        df: PolarsFrame
-        , model:RegressionModel
-        , target: Optional[str] = None
-        , features: Optional[list[str]] = None
-        , score_col:str = "model_score"
-    ) -> DataFrame:
-        
-        if features is None:
-            features = df.columns
-        if target is not None:
-            if target in features:
-                features.remove(target)
-
-        data = df.lazy().collect()
-        output = data.insert_at_idx(0, pl.Series(
-            score_col, model.predict(data.select(features))[:, -1]
-        ))
-        if isinstance(df, pl.LazyFrame):
-            return output.lazy()
-        return output
-
-
-    # Feature Transformations that requires a 1-1 mapping as given by the ref dict. This will be
-    # carried out using a join logic to avoid the use of Python UDF.
-    def map_dict(self, left_col:str, ref:dict, right_col:str, default:Optional[Any]) -> LazyFrame:
-        map_dict = MapDict(left_col = left_col, ref = ref, right_col = right_col, default = default)
-        output = Blueprint._map_dict(self._ldf, map_dict)
-        output.blueprint.steps = self.steps.copy() 
-        output.blueprint.steps.append(
-            Step(action = "map_dict", associated_data = map_dict)
-        )
-        return output
-    
-    # Shallow copy should work
-    # Just make sure exprs are not lazy structures like generators
-    
-    # Transformations are just with_columns(exprs)
-    def with_columns(self, exprs:Iterable[IntoExpr]) -> LazyFrame:
-        output = self._ldf.with_columns(exprs)
-        output.blueprint.steps = self.steps.copy() # Shallow copy should work
-        output.blueprint.steps.append(
-            Step(action = "with_columns", associated_data = exprs)
-        )
-        return output
-    
-    def filter(self, expr:pl.Expr) -> LazyFrame:
-        output = self._ldf.filter(expr)
-        output.blueprint.steps = self.steps.copy() # Shallow copy should work
-        output.blueprint.steps.append(
-            Step(action = "filter", associated_data = expr)
-        )
-        return output
-    
-    # Transformations are just select, used mostly in selector functions
-    def select(self, to_select:list[str]) -> LazyFrame:
-        output = self._ldf.select(to_select)
-        output.blueprint.steps = self.steps.copy() 
-        output.blueprint.steps.append(
-            Step(action = "select", associated_data = to_select)
-        )
-        return output
-    
-    # Transformations that drops, used mostly in removal functions
-    def drop(self, drop_cols:list[str]) -> LazyFrame:
-        output = self._ldf.drop(drop_cols)
-        output.blueprint.steps = self.steps.copy() 
-        output.blueprint.steps.append(
-            Step(action = "drop", associated_data = drop_cols)
-        )
-        return output
-    
-    def add_func(self
-        , df:LazyFrame # The input to the function that needs to be persisted.
-        , func:PipeFunction 
-        , kwargs:dict[str, Any]
-    ) -> LazyFrame:
-        # df: The input lazyframe to the function that needs to be persisted. We need this because:
-        # When running the function, the reference to df might be changed, therefore losing the steps
-
-        # When this is called, the actual function should be already applied.
-        output = self._ldf # .lazy()
-        output.blueprint.steps = df.blueprint.steps.copy() 
-        output.blueprint.steps.append(
-            Step(action="add_func", associated_data={"module":func.__module__, "name":func.__name__, "kwargs":kwargs})
-        )
-        return output
-
-    def add_classif(self
-        , model:ClassifModel
-        , target: Optional[str] = None
-        , features: Optional[list[str]] = None
-        , score_idx:int = -1 
-        , score_col:str = "model_score"
-    ) -> LazyFrame:
-        '''
-        Appends a classification model at given index. This step will collect the lazy frame. All non-target
-        column will be used as features.
-
-        Parameters
-        ----------
-        at
-            Index at which to insert the model step
-        model
-            The trained classification model
-        target
-            The target of the model, which will not be used in making the prediction. It is only used so that we can 
-            remove it from feature list.
-        features
-            The features the model takes. If none, will use all non-target features.
-        score_idx
-            The index of the score column in predict_proba you want to append to the dataframe. E.g. -1 will take the 
-            score of the positive class in a binary classification
-        score_col
-            The name of the score column
-        '''
-        output = Blueprint._process_classif(self._ldf, model, target, features, score_idx, score_col)
-        output.blueprint.steps = self.steps.copy()
-        output.blueprint.steps.append(
-            Step(action = "classif", associated_data={"model":model,
-                                                      "target": target,
-                                                      "features": features,
-                                                      "score_idx": score_idx,
-                                                      "score_col":score_col})
-        )
-        return output
-    
-    def add_regression(self
-        , model:RegressionModel
-        , target: Optional[str] = None
-        , features: Optional[list[str]] = None
-        , score_col:str = "model_score"
-    ) -> LazyFrame:
-        '''
-        Appends a classification model at given index. This step will collect the lazy frame. All non-target
-        column will be used as features.
-
-        Parameters
-        ----------
-        at
-            Index at which to insert the model step
-        model
-            The trained classification model
-        target
-            The target of the model, which will not be used in making the prediction. It is only used so that we can 
-            remove it from feature list.
-        features
-            The features the model takes. If none, will use all non-target features.
-        score_idx
-            The index of the score column in predict_proba you want to append to the dataframe. E.g. -1 will take the 
-            score of the positive class in a binary classification
-        score_col
-            The name of the score column
-        '''        
-        output = Blueprint._process_regression(self._ldf, model, target, features, score_col)
-        output.blueprint.steps = self.steps.copy()
-        output.blueprint.steps.append(
-            Step(action = "classif", associated_data={"model":model,
-                                                      "target": target,
-                                                      "features": features,
-                                                      "score_col":score_col})
-        )
-        return output
-    
-    def preserve(self, path:Union[str,Path]) -> None:
-        '''
-        Writes the blueprint to disk as a Python pickle file at the given path.
-
-        Parameters
-        ----------
-        path
-            A valid path to write to
-        '''
-        with open(path, "wb") as f:
-            pickle.dump(self, f)
-
-    def apply(self, df:PolarsFrame, up_to:int=-1) -> PolarsFrame:
-        '''
-        Apply all the steps to the given df. The result will be lazy if df is lazy, and eager if df is eager.
-
-        Parameters
-        ----------
-        df
-            Either an eager or lazy Polars Dataframe
-        up_to
-            If > 0, will perform the steps up to this number
-        '''
-        _up_to = len(self.steps) if up_to <=0 else min(up_to, len(self.steps))
-        for i,s in enumerate(self.steps):
-            if i < _up_to:
-                if s.action == "drop":
-                    df = df.drop(s.associated_data)
-                elif s.action == "with_columns":
-                    df = df.with_columns(s.associated_data)
-                elif s.action == "map_dict":
-                    df = self._map_dict(df, s.associated_data)
-                elif s.action == "select":
-                    df = df.select(s.associated_data)
-                elif s.action == "filter":
-                    df = df.filter(s.associated_data)
-                elif s.action == "add_func":
-                    func = getattr(importlib.import_module(s.associated_data["module"]), s.associated_data["name"])
-                    df = df.pipe(func, **s.associated_data["kwargs"])
-                elif s.action == "classif":
-                    df = df.pipe(Blueprint._process_classif, **s.associated_data)
-                elif s.action == "regression":
-                    df = df.pipe(Blueprint._process_regression, **s.associated_data)
-            else:
-                break
-        return df
-
-def from_pkl(path: Union[str,Path]) -> Blueprint:
-    with open(path, "rb") as f:
-        obj = pickle.loads(f.read())
-        if isinstance(obj, Blueprint):
-            return obj
-        else:
-            raise ValueError("The pickled object is not a blueprint.")
-
-
+from pathlib import Path
+from polars import LazyFrame, DataFrame
+from dataclasses import dataclass, fields
+from typing import (
+    Any
+    , Union
+    , Optional
+)
+
+from .type_alias import (
+    PolarsFrame
+    , ActionType
+    , PipeFunction
+    , ClassifModel
+    , RegressionModel
+)
+import pickle
+import polars as pl
+import importlib
+import logging
+
+logger = logging.getLogger(__name__)
+
+# P = ParamSpec("P")
+
+@dataclass
+class MapDict:
+    left_col: str # Join on this column, and this column will be replaced by right and dropped.
+    ref: dict # The right table as a dictionary
+    right_col: str
+    default: Optional[Any]
+
+# action + the only non-None field name is a unique identifier for this Step (fully classifies all steps)
+@dataclass
+class Step:
+    action:ActionType
+    with_columns: Optional[list[pl.Expr]] = None
+    map_dict: Optional[MapDict] = None
+    add_func: Optional[dict[str, Any]] = None
+    filter: Optional[pl.Expr] = None 
+    select_or_drop: Optional[list[str]] = None
+    model_step: Optional[dict[str, Any]] = None
+
+    def validate(self) -> bool:
+        not_nones:list[str] = []
+        for field in fields(self):
+            if field.name in ["with_columns", "map_dict", "select_or_drop", "add_func", "filter", "model_step"]:
+                if getattr(self, field.name) is not None:
+                    not_nones.append(field.name)
+            elif field.name == "action":
+                continue
+            else:
+                logger.warning(f"Found unknown action: {field.name}")
+                return False
+
+        if len(not_nones) == 1:
+            return True
+        elif len(not_nones) == 0:
+            logger.warning(f"The Step {self.action} does not have any action value associated with it.")
+            return False
+        else:
+            logger.warning(f"The step {self.action} has two action values associated with it: {not_nones}")
+            return False
+        
+    def get_action_value(self) -> Any:
+        for field in fields(self):
+            value = getattr(self, field.name)
+            if field.name != "action" and value is not None:
+                return value
+
+# Break associated_data into parts?
+
+@pl.api.register_lazyframe_namespace("blueprint")
+class Blueprint:
+    def __init__(self, ldf: LazyFrame):
+        self._ldf = ldf
+        self.steps:list[Step] = []
+
+    def as_str(self, n:int) -> str:
+        output = ""
+        start = max(len(self.steps) + n, 0) if n < 0 else 0
+        till = len(self.steps) if n < 0 else min(n, len(self.steps))
+        for k,s in enumerate(self.steps):
+            if k < start:
+                continue
+            output += f"Step {k} | Action: {s.action}\n"
+            if s.action == "with_columns":
+                output += "Details: \n"
+                for i,expr in enumerate(s.with_columns):
+                    output += f"({i+1}) {expr}\n"
+            elif s.action == "add_func":
+                d:dict = s.add_func
+                output += f"Function Module: {d['module']}, Function Name: {d['name']}\n"
+                output += "Parameters:\n"
+                for key,value in d["kwargs"].items():
+                    output += f"{key} = {value},\n"
+            elif s.action == "filter":
+                output += f"By condition: {s.filter}\n"
+            elif s.action in ("classif", "regression"):
+                output += f"Model: {s.model_step['model'].__class__}\n"
+                features = s.model_step.get('features', None)
+                if features is None:
+                    output += "Using all non-target columns as features.\n"
+                else:
+                    output += f"Using the features {features}\n"
+                output += f"Appends {s.model_step['score_col']} to dataframe."
+            elif s.action == "map_dict":
+                output += f"Encoder/Mapper for column: {s.map_dict.left_col}\n"
+                ref_table = pl.from_dict(s.map_dict.ref)
+                output += f"The encoding/map is:\n{ref_table.head(10)}\n"                
+            else:
+                output += str(s.get_action_value())
+            output += "\n\n"
+            if k > till:
+                break
+        return output
+    
+    def show(self, n:int) -> None:
+        print(self.as_str(n))
+
+    def __str__(self) -> str:
+        return self.as_str(len(self.steps))
+    
+    def __len__(self) -> int:
+        return len(self.steps)
+    
+    def _ipython_display_(self):
+        print(self)
+
+    @staticmethod
+    def _map_dict(df:PolarsFrame, map_dict:MapDict) -> PolarsFrame:
+        temp = pl.from_dict(map_dict.ref) # Always an eager read
+        if isinstance(df, pl.LazyFrame):
+            temp = temp.lazy()
+        
+        if map_dict.default is None:
+            return df.join(temp, on = map_dict.left_col).with_columns(
+                pl.col(map_dict.right_col).alias(map_dict.left_col)
+            ).drop(map_dict.right_col)
+        else:
+            return df.join(temp, on = map_dict.left_col, how = "left").with_columns(
+                pl.col(map_dict.right_col).fill_null(map_dict.default).alias(map_dict.left_col)
+            ).drop(map_dict.right_col)
+        
+    @staticmethod
+    def _process_classif(
+        df: PolarsFrame
+        , model:ClassifModel
+        , features: list[str]
+        , target: Optional[str] = None
+        , score_idx:int = -1 
+        , score_col:str = "model_score"
+    ) -> PolarsFrame:
+        
+        if target is not None:
+            if target in features:
+                features.remove(target)
+
+        data = df.lazy().collect()
+        score = pl.DataFrame({
+            score_col: model.predict_proba(data.select(features))[:, score_idx]
+        })
+        output = pl.concat([data, score], how="horizontal")
+        if isinstance(df, pl.LazyFrame):
+            return output.lazy()
+        return output
+    
+    @staticmethod
+    def _process_regression(
+        df: PolarsFrame
+        , model:RegressionModel
+        , features: list[str]
+        , target: Optional[str] = None
+        , score_col:str = "model_score"
+    ) -> DataFrame:
+        
+        if target is not None:
+            if target in features:
+                features.remove(target)
+
+        data = df.lazy().collect()
+        score = pl.DataFrame({
+            score_col: model.predict(data.select(features)).ravel()
+        })
+        output = pl.concat([data, score], how="horizontal")
+        if isinstance(df, pl.LazyFrame):
+            return output.lazy()
+        return output
+
+    # Feature Transformations that requires a 1-1 mapping as given by the ref dict. This will be
+    # carried out using a join logic to avoid the use of Python UDF.
+    def map_dict(self, left_col:str, ref:dict, right_col:str, default:Optional[Any]) -> LazyFrame:
+        map_dict = MapDict(left_col = left_col, ref = ref, right_col = right_col, default = default)
+        output = Blueprint._map_dict(self._ldf, map_dict)
+        output.blueprint.steps = self.steps.copy() 
+        output.blueprint.steps.append(
+            Step(action = "map_dict", map_dict = map_dict)
+        )
+        return output
+    
+    # Shallow copy should work
+    # Just make sure exprs are not lazy structures like generators
+    
+    # Transformations are just with_columns(exprs)
+    def with_columns(self, exprs:list[pl.Expr]) -> LazyFrame:
+        output = self._ldf.with_columns(exprs)
+        output.blueprint.steps = self.steps.copy() # Shallow copy should work
+        output.blueprint.steps.append(
+            Step(action = "with_columns", with_columns = exprs)
+        )
+        return output
+    
+    def filter(self, expr:pl.Expr) -> LazyFrame:
+        output = self._ldf.filter(expr)
+        output.blueprint.steps = self.steps.copy() # Shallow copy should work
+        output.blueprint.steps.append(
+            Step(action = "filter", filter = expr)
+        )
+        return output
+    
+    # Transformations are just select, used mostly in selector functions
+    def select(self, select_cols:list[str]) -> LazyFrame:
+        output = self._ldf.select(select_cols)
+        output.blueprint.steps = self.steps.copy() 
+        output.blueprint.steps.append(
+            Step(action = "select", select_or_drop = select_cols)
+        )
+        return output
+    
+    # Transformations that drops, used mostly in removal functions
+    def drop(self, drop_cols:list[str]) -> LazyFrame:
+        output = self._ldf.drop(drop_cols)
+        output.blueprint.steps = self.steps.copy() 
+        output.blueprint.steps.append(
+            Step(action = "drop", select_or_drop = drop_cols)
+        )
+        return output
+    
+    def add_func(self
+        , df:LazyFrame # The input to the function that needs to be persisted.
+        , func:PipeFunction 
+        , kwargs:dict[str, Any]
+    ) -> LazyFrame:
+        # df: The input lazyframe to the function that needs to be persisted. We need this because:
+        # When running the function, the reference to df might be changed, therefore losing the steps
+
+        # When this is called, the actual function should be already applied.
+        output = self._ldf # .lazy()
+        output.blueprint.steps = df.blueprint.steps.copy() 
+        output.blueprint.steps.append(
+            Step(action="add_func", add_func={"module":func.__module__, "name":func.__name__, "kwargs":kwargs})
+        )
+        return output
+
+    def add_classif(self
+        , model:ClassifModel
+        , features: list[str]
+        , target: Optional[str] = None
+        , score_idx:int = -1 
+        , score_col:str = "model_score"
+    ) -> LazyFrame:
+        '''
+        Appends a classification model at given index. This step will collect the lazy frame. All non-target
+        column will be used as features.
+
+        Parameters
+        ----------
+        at
+            Index at which to insert the model step
+        model
+            The trained classification model
+        target
+            The target of the model, which will not be used in making the prediction. It is only used so that we can 
+            remove it from feature list.
+        features
+            The features the model takes. If none, will use all non-target features.
+        score_idx
+            The index of the score column in predict_proba you want to append to the dataframe. E.g. -1 will take the 
+            score of the positive class in a binary classification
+        score_col
+            The name of the score column
+        '''
+        output = Blueprint._process_classif(self._ldf, model, features, target, score_idx, score_col)
+        output.blueprint.steps = self.steps.copy()
+        output.blueprint.steps.append(
+            Step(action = "classif", model_step = {"model":model,
+                                                    "target": target,
+                                                    "features": features,
+                                                    "score_idx": score_idx,
+                                                    "score_col":score_col})
+        )
+        return output
+    
+    def add_regression(self
+        , model:RegressionModel
+        , features: list[str]
+        , target: Optional[str] = None
+        , score_col:str = "model_score"
+    ) -> LazyFrame:
+        '''
+        Appends a classification model at given index. This step will collect the lazy frame. All non-target
+        column will be used as features.
+
+        Parameters
+        ----------
+        at
+            Index at which to insert the model step
+        model
+            The trained classification model
+        target
+            The target of the model, which will not be used in making the prediction. It is only used so that we can 
+            remove it from feature list.
+        features
+            The features the model takes. If none, will use all non-target features.
+        score_idx
+            The index of the score column in predict_proba you want to append to the dataframe. E.g. -1 will take the 
+            score of the positive class in a binary classification
+        score_col
+            The name of the score column
+        '''        
+        output = Blueprint._process_regression(self._ldf, model, features, target, score_col)
+        output.blueprint.steps = self.steps.copy()
+        output.blueprint.steps.append(
+            Step(action = "regression", model_step = {"model":model,
+                                                        "target": target,
+                                                        "features": features,
+                                                        "score_col":score_col})
+        )
+        return output
+    
+    def preserve(self, path:Union[str,Path]) -> None:
+        '''
+        Writes the blueprint to disk as a Python pickle file at the given path.
+
+        Parameters
+        ----------
+        path
+            A valid path to write to
+        '''
+        with open(path, "wb") as f:
+            pickle.dump(self, f)
+
+    def apply(self, df:PolarsFrame, up_to:int=-1, collect:bool=False) -> PolarsFrame:
+        '''
+        Apply all the steps to the given df. The result will be lazy if df is lazy, and eager if df is eager.
+
+        Parameters
+        ----------
+        df
+            Either an eager or lazy Polars Dataframe
+        up_to
+            If > 0, will perform the steps up to this number
+        collect
+            If input is lazy and collect = True, then this will collect the result at the end. If streaming
+            collect is desired, please set this to False and collect manually.
+        '''
+        _up_to = len(self.steps) if up_to <=0 else min(up_to, len(self.steps))
+        for i,s in enumerate(self.steps):
+            if i < _up_to:
+                if s.action == "drop":
+                    df = df.drop(s.select_or_drop)
+                elif s.action == "with_columns":
+                    df = df.with_columns(s.with_columns)
+                elif s.action == "map_dict":
+                    df = self._map_dict(df, s.map_dict)
+                elif s.action == "select":
+                    df = df.select(s.select_or_drop)
+                elif s.action == "filter":
+                    df = df.filter(s.filter)
+                elif s.action == "add_func":
+                    module, name = s.add_func["module"], s.add_func["name"]
+                    func = getattr(importlib.import_module(module), name)
+                    df = df.pipe(func, **s.add_func["kwargs"])
+                elif s.action == "classif":
+                    df = df.pipe(Blueprint._process_classif, **s.model_step)
+                elif s.action == "regression":
+                    df = df.pipe(Blueprint._process_regression, **s.model_step)
+            else:
+                break
+
+        if isinstance(df, pl.LazyFrame) and collect:
+            return df.collect()
+        return df
+
+def from_pkl(path: Union[str,Path]) -> Blueprint:
+    with open(path, "rb") as f:
+        obj = pickle.loads(f.read())
+        if isinstance(obj, Blueprint):
+            return obj
+        else:
+            raise ValueError("The object in the pickled file is not a Blueprint object.")
+
+
```

### Comparing `dsds-0.0.24/src/dsds/encoders.py` & `dsds-0.0.25/python/dsds/encoders.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,712 +1,714 @@
-from __future__ import annotations
-
-from .type_alias import (
-    PolarsFrame
-)
-from .prescreen import (
-    get_bool_cols
-    , get_string_cols
-    , get_unique_count
-    , check_binary_target
-    , type_checker
-)
-from .blueprint import( # Need this for Polars extension to work
-    Blueprint  # noqa: F401
-)
-from typing import Optional, Union, Any
-import logging
-import numpy as np
-import polars as pl
-
-logger = logging.getLogger(__name__)
-
-def boolean_encode(df:PolarsFrame, keep_null:bool=True) -> PolarsFrame:
-    '''
-    Converts all boolean columns into binary 0, 1 columns.
-
-    This will be remembered by blueprint by default.
-
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars DataFrame
-    keep_null
-        If true, null will be kept. If false, null will be mapped to 0.
-    '''
-    bool_cols = get_bool_cols(df)
-    if keep_null: # Directly cast. If null, then cast will also return null
-        exprs = (pl.col(c).cast(pl.UInt8) for c in bool_cols)
-    else: # Cast. Then fill null to 0s.
-        exprs = (pl.col(c).cast(pl.UInt8).fill_null(0) for c in bool_cols)
-
-    if isinstance(df, pl.LazyFrame):
-        return df.blueprint.with_columns(exprs)
-    return df.with_columns(exprs)
-
-def missing_indicator(
-    df: PolarsFrame
-    , cols: Optional[list[str]] = None
-    , suffix: str = "_missing"
-) -> PolarsFrame:
-    '''
-    Add one-hot columns for missing values in the given columns.
-
-    This will be remembered by blueprint by default.
-
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars DataFrame
-    cols
-        If not provided, will create missing indicators for all columns
-    suffix
-        The suffix given to the missing indicator columns
-    '''
-    if cols is None:
-        to_add = df.columns
-    else:
-        to_add = cols
-    one = pl.lit(1, dtype=pl.UInt8)
-    zero = pl.lit(0, dtype=pl.UInt8)
-    exprs = (pl.when(pl.col(c).is_null()).then(one).otherwise(zero).suffix(suffix) for c in to_add)
-    if isinstance(df, pl.LazyFrame):
-        return df.blueprint.with_columns(list(exprs))
-    return df.with_columns(exprs)
-
-def one_hot_encode(
-    df:PolarsFrame
-    , cols:Optional[list[str]]=None
-    , separator:str="_"
-    , drop_first:bool=False
-) -> PolarsFrame:
-    '''
-    One-hot-encode the given columns.
-
-    This will be remembered by blueprint by default.
-
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars DataFrame
-    cols
-        If not provided, will use all string columns
-    separator
-        The separator used in the names of the new columns
-    drop_first
-        If true, the first category in the each column will be dropped. E.g. if column "D" has 3 distinct values, 
-        say 'A', 'B', 'C', then only two binary indicators 'D_B' and 'D_C' will be created. This is useful for
-        reducing dimensions and also good for optimization methods that require data to be non-degenerate.
-    '''
-    if isinstance(cols, list):
-        _ = type_checker(df, cols, "string", "one_hot_encode")
-        str_cols = cols
-    else:
-        str_cols = get_string_cols(df)
-
-    if isinstance(df, pl.LazyFrame):
-        temp = df.lazy().select(str_cols).groupby(1).agg(
-            pl.all().unique().sort()
-        ).select(str_cols)
-        exprs:list[pl.Expr] = []
-        start_index = int(drop_first)
-        one = pl.lit(1, dtype=pl.UInt8) # Avoid casting 
-        zero = pl.lit(0, dtype=pl.UInt8) # Avoid casting
-        for t in temp.collect().get_columns():
-            u:pl.List = t[0] # t is a Series which contains a single series/list, so u is a series/list
-            if len(u) > 1:
-                exprs.extend(
-                    pl.when(pl.col(t.name) == u[i]).then(one).otherwise(zero).alias(t.name + separator + u[i])
-                    for i in range(start_index, len(u))
-                )
-            else:
-                logger.info(f"During one-hot-encoding, the column {t.name} is found to have 1 unique value. Dropped.")
-        
-        return df.blueprint.with_columns(exprs).blueprint.drop(str_cols)
-    else:
-        return df.to_dummies(columns=str_cols, separator=separator, drop_first=drop_first)
-    
-def binary_encode(
-    df:PolarsFrame
-    , cols:Optional[list[str]]=None
-    , separator: str = "_"
-    , exclude:Optional[list[str]]=None
-) -> PolarsFrame:
-    '''
-    Encode binary string columns as 0s and 1s depending on the order of the 2 unique strings. E.g. if the two unique 
-    values are 'N' and 'Y', then 'N' will be mapped to 0 and 'Y' to 1 because 'N' < 'Y'. This is essentially 
-    one-hot-encode for binary string columns with drop_first = True.
-
-    This will be remembered by blueprint by default.
-
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars DataFrame
-    cols
-        If not provided, will use all string columns
-    separator
-        The separator used in the names of the new columns
-    '''
-    if cols is None:
-        str_cols = get_string_cols(df)
-        exclude = [] if exclude is None else exclude
-        binary_list = get_unique_count(df)\
-            .filter( # Binary + Not Exclude + Only String
-                (pl.col("n_unique") == 2) & (~pl.col("column").is_in(exclude)) & (pl.col("column").is_in(str_cols))
-            ).get_column("column").to_list()
-    else:
-        binary_list = cols
-    
-    return one_hot_encode(df, cols=binary_list, drop_first=True, separator=separator)
-
-def force_binary(df:PolarsFrame) -> PolarsFrame:
-    '''
-    Force every binary column, no matter what data type, to be turned into 0s and 1s according to the order of the 
-    elements. If a column has two unique values like [null, "haha"], then null will be mapped to 0 and "haha" to 1.
-
-    This will be remembered by blueprint by default.
-
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars DataFrame
-    '''
-    binary_list = get_unique_count(df).filter(pl.col("n_unique") == 2).get_column("column")
-    temp = df.lazy().select(binary_list).groupby(1).agg(
-            pl.all().unique().sort()
-        ).select(binary_list)
-    exprs:list[pl.Expr] = []
-    one = pl.lit(1, dtype=pl.UInt8) # Avoid casting 
-    zero = pl.lit(0, dtype=pl.UInt8) # Avoid casting
-    for t in temp.collect().get_columns():
-        u:pl.List = t[0] # t is a Series which contains a single list which contains the 2 unique values 
-        exprs.append(
-            pl.when(pl.col(t.name) == u[0]).then(zero).otherwise(one).alias(t.name)
-        )
-
-    if isinstance(df, pl.LazyFrame):
-        return df.blueprint.with_columns(exprs)
-    return df.with_columns(exprs)
-
-def multicat_one_hot_encode(
-    df:PolarsFrame
-    , cols: list[str]
-    , delimiter: str
-    , drop_first: bool = False
-) -> PolarsFrame:
-    '''
-    Expands multicategorical columns into several one-hot-encoded columns respectively. A multicategorical column is a 
-    column with strings like `aaa|bbb|ccc`, which means this row belongs to categories aaa, bbb, and ccc. Typically, 
-    such a column will contain strings separated by a delimiter. This method will collect all unique strings separated 
-    by the delimiter and one hot encode the corresponding column.
-
-    This will be remembered by blueprint by default.
-
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars DataFrame
-    cols
-        If not provided, will use all string columns
-    separator
-        The separator used in the names of the new columns
-    drop_first
-        If true, the first category in the each column will be dropped.
-
-    Example
-    -------
-    >>> df = pl.DataFrame({
-    ... "text1":["abc|ggg", "abc|sss", "ccc|abc"],
-    ... "text2":["aaa|bbb", "ccc|aaa", "bbb|ccc"]
-    ... })
-    >>> df
-    shape: (3, 2)
-    ┌─────────┬─────────┐
-    │ text1   ┆ text2   │
-    │ ---     ┆ ---     │
-    │ str     ┆ str     │
-    ╞═════════╪═════════╡
-    │ abc|ggg ┆ aaa|bbb │
-    │ abc|sss ┆ ccc|aaa │
-    │ ccc|abc ┆ bbb|ccc │
-    └─────────┴─────────┘
-    >>> multicat_one_hot_encode(df, cols=["text1", "text2"], delimiter="|")
-    shape: (3, 7)
-    ┌───────────┬───────────┬───────────┬───────────┬───────────┬───────────┬───────────┐
-    │ text1|abc ┆ text1|ccc ┆ text1|ggg ┆ text1|sss ┆ text2|aaa ┆ text2|bbb ┆ text2|ccc │
-    │ ---       ┆ ---       ┆ ---       ┆ ---       ┆ ---       ┆ ---       ┆ ---       │
-    │ u8        ┆ u8        ┆ u8        ┆ u8        ┆ u8        ┆ u8        ┆ u8        │
-    ╞═══════════╪═══════════╪═══════════╪═══════════╪═══════════╪═══════════╪═══════════╡
-    │ 1         ┆ 0         ┆ 1         ┆ 0         ┆ 1         ┆ 1         ┆ 0         │
-    │ 1         ┆ 0         ┆ 0         ┆ 1         ┆ 1         ┆ 0         ┆ 1         │
-    │ 1         ┆ 1         ┆ 0         ┆ 0         ┆ 0         ┆ 1         ┆ 1         │
-    └───────────┴───────────┴───────────┴───────────┴───────────┴───────────┴───────────┘
-    '''
-    _ = type_checker(df, cols, "string", "multicat_one_hot_encode")
-    temp = df.lazy().select(cols).groupby(1).agg(
-        pl.all().str.split(delimiter).explode().unique().sort()
-    ).select(cols)
-    one = pl.lit(1, dtype=pl.UInt8) # Avoid casting
-    zero = pl.lit(0, dtype=pl.UInt8) # Avoid casting
-    exprs = []
-    start_index = int(drop_first)
-    for c in temp.collect().get_columns():
-        u = c[0]
-        if len(u) > 1:
-            exprs.extend(
-                pl.when(pl.col(c.name).str.contains(u[i])).then(one).otherwise(zero).alias(c.name + delimiter + u[i])
-                for i in range(start_index, len(u))
-            )
-        else:
-            logger.info(f"The multicategorical column {c.name} seems to have only 1 unique value. Dropped.")
-
-    if isinstance(df, pl.LazyFrame):
-        return df.blueprint.with_columns(exprs).blueprint.drop(cols)
-    return df.with_columns(exprs).drop(cols)
-
-
-def ordinal_auto_encode(
-    df:PolarsFrame
-    , cols:Optional[list[str]]=None
-    , descending:bool = False
-    , exclude:Optional[list[str]]=None
-) -> PolarsFrame:
-    '''
-    Automatically applies ordinal encoding to the provided columns by the order of the elements. This method is 
-    great for string columns like age ranges, with values like ["10-20", "20-30"], etc. (Beware of string lengths,
-    e.g. if "100-110" exists in age range, then it may mess up the natural order.)
-
-    This will be remembered by blueprint by default.
-        
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars DataFrame
-    cols
-        If not provided, will use all string columns
-    descending
-        If true, will use descending order (0 will be mapped to largest element)
-    exclude
-        Columns to exclude. This is only used when cols is not provided.
-    '''
-    if isinstance(cols, list):
-        _ = type_checker(df, cols, "string", "ordinal_auto_encode")
-        ordinal_list = cols
-    else:
-        ordinal_list = get_string_cols(df, exclude=exclude)
-
-    temp = df.lazy().select(ordinal_list).groupby(1).agg(
-        pl.all().unique().sort(descending=descending) 
-    ).select(ordinal_list)
-    for t in temp.collect().get_columns():
-        uniques:pl.Series = t[0]
-        mapping = {t.name: uniques, "to": list(range(len(uniques)))}
-        if isinstance(df, pl.LazyFrame):
-            df = df.blueprint.map_dict(t.name, mapping, "to", None)
-        else:
-            map_tb = pl.DataFrame(mapping)
-            df = df.join(map_tb, on = t.name).with_columns(
-                pl.col("to").alias(t.name)
-            ).drop("to")
-    return df
-
-def ordinal_encode(
-    df:PolarsFrame
-    , ordinal_mapping:dict[str, dict[str,int]]
-    , default:Optional[int] = None
-) -> PolarsFrame:
-    '''
-    Ordinal encode the columns in the ordinal_mapping dictionary.
-
-    This will be remembered by blueprint by default.
-        
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars DataFrame
-    ordinal_mapping
-        A dictionary that looks like {"a":{"a1":1, "a2":2}, ...}
-    default
-        Default value for values not mentioned in the ordinal_mapping dict.
-    '''
-    for c in ordinal_mapping:
-        if c in df.columns:
-            mapping = ordinal_mapping[c]
-            if isinstance(df, pl.LazyFrame):
-                # This relies on the fact that dicts in Python is ordered
-                mapping = {c: mapping.keys(), "to": mapping.values()}
-                df = df.blueprint.map_dict(c, mapping, "to", default)
-            else:
-                mapping = pl.DataFrame((mapping.keys(), mapping.values()), schema=[c, "to"])
-                df = df.join(mapping, on = c, how="left").with_columns(
-                    pl.col("to").fill_null(default).alias(c)
-                ).drop("to")
-        else:
-            logger.warning(f"Found that column {c} is not in df. Skipped.")
-    return df
-
-def smooth_target_encode(
-    df:PolarsFrame
-    , target:str
-    , cols:list[str]
-    , min_samples_leaf:int
-    , smoothing:float
-    , check_binary:bool=True
-) -> PolarsFrame:
-    '''
-    Smooth target encoding for binary classification. Currently only implemented for binary target.
-
-    This will be remembered by blueprint by default.
-    
-    See https://towardsdatascience.com/dealing-with-categorical-variables-by-using-target-encoder-a0f1733a4c69
-
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars DataFrame
-    target
-        Name of the target column
-    cols
-        If not provided, will use all string columns
-    min_samples_leaf
-        The k in the smoothing factor equation
-    smoothing
-        The f of the smoothing factor equation 
-    check_binary
-        Checks if target is binary. If not, throw an error
-    '''
-    if isinstance(cols, list):
-        _ = type_checker(df, cols, "string", "smooth_target_encode")
-        str_cols = cols
-    else:
-        str_cols = get_string_cols(df)
-    
-    # Only works for binary target for now. There is a non-binary ver of target encode, but I
-    # am just delaying the implementation...
-    if check_binary:
-        if not check_binary_target(df, target):
-            raise ValueError("Target is not binary or not properly encoded.")
-
-    # probability of target = 1
-    p = df.lazy().select(pl.col(target).mean()).collect().item(0,0)
-    is_lazy = isinstance(df, pl.LazyFrame)
-    # If c has null, null will become a group when we group by.
-    for c in str_cols:
-        ref = df.groupby(c).agg(
-            pl.count().alias("cnt"),
-            pl.col(target).mean().alias("cond_p")
-        ).with_columns(
-            (1./(1. + ((-(pl.col("cnt").cast(pl.Float64) - min_samples_leaf))/smoothing).exp())).alias("alpha")
-        ).select(
-            pl.col(c),
-            to = pl.col("alpha") * pl.col("cond_p") + (pl.lit(1) - pl.col("alpha")) * pl.lit(p)
-        ) # If df is lazy, ref is lazy. If df is eager, ref is eager
-        if is_lazy:
-            df = df.blueprint.map_dict(c, ref.collect().to_dict(), "to", None)
-        else: # It is ok to do inner join because all values of c are present in ref.
-            df = df.join(ref, on = c).with_columns(
-                pl.col("to").alias(c)
-            ).drop("to")
-    return df
-
-def _when_then_repl(c:str, repl_map:dict):
-    expr = pl.col(c)
-    for og, repl in repl_map.items():
-        expr = pl.when(pl.col(c).eq(og)).then(repl).otherwise(expr)
-    
-    return expr.alias(c)
-
-def feature_mapping(
-    df:PolarsFrame
-    , mapping: Union[dict[str, dict[Any, Any]], list[pl.Expr] , pl.Expr]
-) -> PolarsFrame:
-    '''
-    Maps specific values of a feature into values provided. This is a common task when the feature columns come with 
-    error codes.
-
-    This will be remembered by blueprint by default.
-
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars dataframe
-    mapping
-        Either a dict like {"a": {999: None, 998: None, 997: None}, ...}, meaning that 999, 998 and 997 in column "a" 
-        should be replaced by null, or a list/a single Polars (when-then) expression(s) like the following,  
-        pl.when(pl.col("a") >= 997).then(None).otherwise(pl.col("a")).alias("a"), which will perform the same mapping 
-        as the dict example. Note that using Polars expression can tackle more complex replacement.
-
-    Example
-    -------
-    >>> df = pl.DataFrame({
-    ...     "a": [1,2,3,998,999],
-    ...     "b": [999, 1,2,3,4]
-    ... })
-    >>> print(df)
-    shape: (5, 2)
-    ┌─────┬─────┐
-    │ a   ┆ b   │
-    │ --- ┆ --- │
-    │ i64 ┆ i64 │
-    ╞═════╪═════╡
-    │ 1   ┆ 999 │
-    │ 2   ┆ 1   │
-    │ 3   ┆ 2   │
-    │ 998 ┆ 3   │
-    │ 999 ┆ 4   │
-    └─────┴─────┘
-    >>> feature_mapping(df, mapping = {"a":{998:None,999:None}, "b":{999:None}})
-    shape: (5, 2)
-    ┌──────┬──────┐
-    │ a    ┆ b    │
-    │ ---  ┆ ---  │
-    │ i64  ┆ i64  │
-    ╞══════╪══════╡
-    │ 1    ┆ null │
-    │ 2    ┆ 1    │
-    │ 3    ┆ 2    │
-    │ null ┆ 3    │
-    │ null ┆ 4    │
-    └──────┴──────┘
-    >>> mapping = [pl.when(pl.col("a")>=998).then(None).otherwise(pl.col("a")).alias("a")
-    ...          , pl.when(pl.col("b")==999).then(None).otherwise(pl.col("b")).alias("b")]
-    >>> feature_mapping(df, mapping)
-    shape: (5, 2)
-    ┌──────┬──────┐
-    │ a    ┆ b    │
-    │ ---  ┆ ---  │
-    │ i64  ┆ i64  │
-    ╞══════╪══════╡
-    │ 1    ┆ null │
-    │ 2    ┆ 1    │
-    │ 3    ┆ 2    │
-    │ null ┆ 3    │
-    │ null ┆ 4    │
-    └──────┴──────┘
-    '''
-    if isinstance(mapping, dict):
-        exprs = []
-        for c, repl_map in mapping.items():
-            exprs.append(_when_then_repl(c, repl_map))
-    elif isinstance(mapping, list):
-        exprs = []
-        for f in mapping:
-            if isinstance(f, pl.Expr):
-                exprs.append(f)
-            else:
-                logger.warn(f"Found {f} is not a Polars expression. Ignored.")
-    elif isinstance(mapping, pl.Expr):
-        exprs = [mapping]
-    else:
-        raise TypeError("The argument `mapping` must be one of the following types: "
-                        "dict[str, dict[Any, Any]] | list[pl.Expr] | pl.Expr")
-    
-    if isinstance(df, pl.LazyFrame):
-        return df.blueprint.with_columns(exprs)
-    return df.with_columns(exprs)
-
-def custom_binning(
-    df:PolarsFrame
-    , cols:list[str]
-    , cuts:list[float]
-    , suffix:str = ""
-) -> PolarsFrame:
-    '''
-    Bins according to the cuts provided. The same cuts will be applied to all columns in cols.
-
-    This will be remembered by blueprint by default.
-
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars DataFrame
-    cols
-        Numerical columns that will be binned
-    cuts
-        A list of floats representing break points in the intervals
-    suffix
-        If you don't want to replace the original columns, you have the option to give the binned column a suffix
-    '''
-    if isinstance(df, pl.LazyFrame):
-        exprs = [
-            pl.col(c).cut(cuts).cast(pl.Utf8).suffix(suffix) for c in cols
-        ]
-        return df.blueprint.with_columns(exprs)
-    else:
-        return df.with_columns(
-            pl.col(c).cut(cuts).cast(pl.Utf8).suffix(suffix) for c in cols
-        )
-    
-def fixed_sized_binning(
-    df:PolarsFrame
-    , cols:list[str]
-    , interval: float
-    , suffix:str = ""
-) -> PolarsFrame:
-    '''
-    Bins according to fixed interval size. The same cuts will be applied to all columns in cols. Bin will 
-    start from min(feature) to max(feature) + interval with step length = interval.
-
-    This will be remembered by blueprint by default.
-
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars DataFrame
-    cols
-        Numerical columns that will be binned
-    interval
-        The fixed sized interval
-    suffix
-        If you don't want to replace the original columns, you have the option to give the binned column a suffix
-    '''
-    bounds = df.lazy().select(cols).select(
-        pl.all().min().prefix("min:")
-        , pl.all().max().prefix("max:")
-    ).collect().row(0)
-    exprs = []
-    n = len(cols)
-    for i, c in enumerate(cols):
-        cut = np.arange(bounds[i], bounds[n+i] + interval, step=interval).tolist()
-        exprs.append(pl.col(c).cut(cut).cast(pl.Utf8).suffix(suffix))
-
-    if isinstance(df, pl.LazyFrame):
-        return df.blueprint.with_columns(exprs)
-    return df.with_columns(exprs)
-
-def quantile_binning(
-    df:PolarsFrame
-    , cols:list[str]
-    , n_bins:int
-    , suffix:str = ""
-) -> PolarsFrame:
-    '''
-    Bin a continuous variable into categories, based on quantile. Null values will be its own category. The same binning
-    rule will be applied to all columns in cols. If you want different n_bins for different columns, chain another 
-    quantile_binning with different cols and n_bins.
-
-    This will be remembered by blueprint by default.
-
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars dataframe
-    cols
-        A list of numeric columns. This has to be supplied by the user because it is not recommended
-        to bin all numerical variables
-    n_bins
-        The number of desired bins. If n_bins = 4, the quantile cuts will be [0.25,0.5,0.74], and 4 
-        categories will be created, which represent values ranging from (-inf, 0.25 quantile value],
-        (0.25 quantile value, 0.5 quantile value],...(0.75 quantile value, inf]
-    suffix
-        If you don't want to replace the original columns, you have the option to give the binned column a suffix
-
-    Example
-    -------
-    >>> df = pl.DataFrame({
-    ...     "a":range(5)
-    ... })
-    >>> df
-    shape: (5, 1)
-    ┌─────┐
-    │ a   │
-    │ --- │
-    │ i64 │
-    ╞═════╡
-    │ 0   │
-    │ 1   │
-    │ 2   │
-    │ 3   │
-    │ 4   │
-    └─────┘
-    >>> quantile_binning(df, cols=["a"], n_bins=4)
-    shape: (5, 1)
-    ┌───────────┐
-    │ a         │
-    │ ---       │
-    │ str       │
-    ╞═══════════╡
-    │ (-inf, 1] │
-    │ (-inf, 1] │
-    │ (1, 2]    │
-    │ (2, 3]    │
-    │ (3, inf]  │
-    └───────────┘
-    '''
-    _ = type_checker(df, cols, "numeric", "quantile_binning")
-    qcuts = np.arange(start=1/n_bins, stop=1.0, step = 1/n_bins)
-    if isinstance(df, pl.LazyFrame):
-        cuts = df.select(cols).select(
-            pl.all().qcut(qcuts).unique().cast(pl.Utf8).str.extract(r"\((.*?),")
-            .cast(pl.Float64).sort().tail(len(qcuts))
-        ).collect()
-        exprs = [
-            pl.col(c).cut(cuts.drop_in_place(c).to_list()).cast(pl.Utf8).suffix(suffix) for c in cols
-        ]
-        return df.blueprint.with_columns(exprs)
-    else: # Eager frame
-        return df.with_columns(
-            pl.col(c).qcut(qcuts).cast(pl.Utf8).suffix(suffix) for c in cols 
-        )
-
-def woe_cat_encode(
-    df:PolarsFrame
-    , target:str
-    , cols:Optional[list[str]]=None
-    , min_count:float = 1.
-    , default: float = -10.
-    , check_binary:bool = True
-) -> PolarsFrame:
-    '''
-    Performs WOE encoding for categorical features. To WOE encode numerical columns, first bin them using
-    custom_binning or quantile_binning. This only works for binary target.
-
-    This will be remembered by blueprint by default.
-
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars dataframe
-    target
-        The name of the target column
-    cols
-        If not provided, all string columns will be used
-    min_count
-        A numerical factor that prevents values like infinity to occur when taking log
-    default
-        Null values will be mapped to default
-    check_binary
-        Whether to check target is binary or not.
-    '''
-    if isinstance(cols, list):
-        _ = type_checker(df, cols, "string", "woe_cat_encode")
-        str_cols = cols
-    else:
-        str_cols = get_string_cols(df)
-
-    if check_binary:
-        if not check_binary_target(df, target):
-            raise ValueError("Target is not binary or not properly encoded.")
-
-    is_lazy = isinstance(df, pl.LazyFrame)
-    for s in str_cols:
-        ref = df.lazy().groupby(s).agg(
-            ev = pl.col(target).sum()
-            , nonev = (pl.lit(1) - pl.col(target)).sum()
-        ).with_columns(
-            ev_rate = (pl.col("ev") + min_count)/(pl.col("ev").sum() + 2.0*min_count)
-            , nonev_rate = (pl.col("nonev") + min_count)/(pl.col("nonev").sum() + 2.0*min_count)
-        ).with_columns(
-            woe = (pl.col("ev_rate")/pl.col("nonev_rate")).log()
-        ).select(
-            pl.col(s)
-            , pl.col("woe")
-        ).collect()
-        if is_lazy:
-            df = df.blueprint.map_dict(s, ref.to_dict(), "woe", default)
-        else:
-            df = df.join(ref, on = s, how="left").with_columns(
-                pl.col("woe").fill_null(default).alias(s)
-            ).drop("woe")
-
+from __future__ import annotations
+
+from .type_alias import (
+    PolarsFrame
+)
+from .prescreen import (
+    get_bool_cols
+    , get_string_cols
+    , get_unique_count
+    , check_binary_target
+    , type_checker
+)
+from .blueprint import( # Need this for Polars extension to work
+    Blueprint  # noqa: F401
+)
+from typing import Optional, Union, Any
+import numpy as np
+import polars as pl
+import logging
+
+logger = logging.getLogger(__name__)
+
+def boolean_encode(df:PolarsFrame, keep_null:bool=True) -> PolarsFrame:
+    '''
+    Converts all boolean columns into binary 0, 1 columns.
+
+    This will be remembered by blueprint by default.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars DataFrame
+    keep_null
+        If true, null will be kept. If false, null will be mapped to 0.
+    '''
+    bool_cols = get_bool_cols(df)
+    if keep_null: # Directly cast. If null, then cast will also return null
+        exprs = (pl.col(c).cast(pl.UInt8) for c in bool_cols)
+    else: # Cast. Then fill null to 0s.
+        exprs = (pl.col(c).cast(pl.UInt8).fill_null(0) for c in bool_cols)
+
+    if isinstance(df, pl.LazyFrame):
+        return df.blueprint.with_columns(exprs)
+    return df.with_columns(exprs)
+
+def missing_indicator(
+    df: PolarsFrame
+    , cols: Optional[list[str]] = None
+    , suffix: str = "_missing"
+) -> PolarsFrame:
+    '''
+    Add one-hot columns for missing values in the given columns.
+
+    This will be remembered by blueprint by default.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars DataFrame
+    cols
+        If not provided, will create missing indicators for all columns
+    suffix
+        The suffix given to the missing indicator columns
+    '''
+    if cols is None:
+        to_add = df.columns
+    else:
+        to_add = cols
+    one = pl.lit(1, dtype=pl.UInt8)
+    zero = pl.lit(0, dtype=pl.UInt8)
+    exprs = (pl.when(pl.col(c).is_null()).then(one).otherwise(zero).suffix(suffix) for c in to_add)
+    if isinstance(df, pl.LazyFrame):
+        return df.blueprint.with_columns(list(exprs))
+    return df.with_columns(exprs)
+
+def one_hot_encode(
+    df:PolarsFrame
+    , cols:Optional[list[str]]=None
+    , separator:str="_"
+    , drop_first:bool=False
+) -> PolarsFrame:
+    '''
+    One-hot-encode the given columns.
+
+    This will be remembered by blueprint by default.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars DataFrame
+    cols
+        If not provided, will use all string columns
+    separator
+        The separator used in the names of the new columns
+    drop_first
+        If true, the first category in the each column will be dropped. E.g. if column "D" has 3 distinct values, 
+        say 'A', 'B', 'C', then only two binary indicators 'D_B' and 'D_C' will be created. This is useful for
+        reducing dimensions and also good for optimization methods that require data to be non-degenerate.
+    '''
+    if isinstance(cols, list):
+        _ = type_checker(df, cols, "string", "one_hot_encode")
+        str_cols = cols
+    else:
+        str_cols = get_string_cols(df)
+
+    if isinstance(df, pl.LazyFrame):
+        temp = df.lazy().select(str_cols).select(
+            pl.all().unique().implode().list.sort()
+        )
+        exprs:list[pl.Expr] = []
+        start_index = int(drop_first)
+        one = pl.lit(1, dtype=pl.UInt8) # Avoid casting 
+        zero = pl.lit(0, dtype=pl.UInt8) # Avoid casting
+        for t in temp.collect().get_columns():
+            u:pl.List = t[0] # t is a Series which contains a single series/list, so u is a series/list
+            if len(u) > 1:
+                exprs.extend(
+                    pl.when(pl.col(t.name) == u[i]).then(one).otherwise(zero).alias(t.name + separator + u[i])
+                    for i in range(start_index, len(u))
+                )
+            else:
+                logger.info(f"During one-hot-encoding, the column {t.name} is found to have 1 unique value. Dropped.")
+        
+        return df.blueprint.with_columns(exprs).blueprint.drop(str_cols)
+    else:
+        return df.to_dummies(columns=str_cols, separator=separator, drop_first=drop_first)
+    
+def binary_encode(
+    df:PolarsFrame
+    , cols:Optional[list[str]]=None
+    , separator: str = "_"
+    , exclude:Optional[list[str]]=None
+) -> PolarsFrame:
+    '''
+    Encode binary string columns as 0s and 1s depending on the order of the 2 unique strings. E.g. if the two unique 
+    values are 'N' and 'Y', then 'N' will be mapped to 0 and 'Y' to 1 because 'N' < 'Y'. This is essentially 
+    one-hot-encode for binary string columns with drop_first = True.
+
+    This will be remembered by blueprint by default.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars DataFrame
+    cols
+        If not provided, will use all string columns
+    separator
+        The separator used in the names of the new columns
+    '''
+    if cols is None:
+        str_cols = get_string_cols(df)
+        exclude = [] if exclude is None else exclude
+        binary_list = get_unique_count(df)\
+            .filter( # Binary + Not Exclude + Only String
+                (pl.col("n_unique") == 2) & (~pl.col("column").is_in(exclude)) & (pl.col("column").is_in(str_cols))
+            )["column"].to_list()
+    else:
+        binary_list = cols
+    
+    return one_hot_encode(df, cols=binary_list, drop_first=True, separator=separator)
+
+def force_binary(df:PolarsFrame) -> PolarsFrame:
+    '''
+    Force every binary column, no matter what data type, to be turned into 0s and 1s according to the order of the 
+    elements. If a column has two unique values like [null, "haha"], then null will be mapped to 0 and "haha" to 1.
+
+    This will be remembered by blueprint by default.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars DataFrame
+    '''
+    binary_list = get_unique_count(df).filter(pl.col("n_unique") == 2)["column"]
+    temp = df.lazy().select(binary_list).select(
+            pl.all().unique().implode().list.sort()
+        )
+    exprs:list[pl.Expr] = []
+    one = pl.lit(1, dtype=pl.UInt8) # Avoid casting 
+    zero = pl.lit(0, dtype=pl.UInt8) # Avoid casting
+    for t in temp.collect().get_columns():
+        u:pl.List = t[0] # t is a Series which contains a single list which contains the 2 unique values 
+        exprs.append(
+            pl.when(pl.col(t.name) == u[0]).then(zero).otherwise(one).alias(t.name)
+        )
+
+    if isinstance(df, pl.LazyFrame):
+        return df.blueprint.with_columns(exprs)
+    return df.with_columns(exprs)
+
+def multicat_one_hot_encode(
+    df:PolarsFrame
+    , cols: list[str]
+    , delimiter: str = "|"
+    , drop_first: bool = False
+) -> PolarsFrame:
+    '''
+    Expands multicategorical columns into several one-hot-encoded columns respectively. A multicategorical column is a 
+    column with strings like `aaa|bbb|ccc`, which means this row belongs to categories aaa, bbb, and ccc. Typically, 
+    such a column will contain strings separated by a delimiter. This method will collect all unique strings separated 
+    by the delimiter and one hot encode the corresponding column, e.g. by checking if `aaa` is contained in values of this
+    column. Nulls will be mapped to 0 in the generated one-hot columns. If you wish to have a null mask, take a look 
+    at `dsds.encoders.missing_indicator`.
+
+    This will be remembered by blueprint by default.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars DataFrame
+    cols
+        If not provided, will use all string columns
+    separator
+        The separator used in the names of the new columns
+    drop_first
+        If true, the first category in the each column will be dropped.
+
+    Example
+    -------
+    >>> df = pl.DataFrame({
+    ... "text1":["abc|ggg", "abc|sss", "ccc|abc"],
+    ... "text2":["aaa|bbb", "ccc|aaa", "bbb|ccc"]
+    ... })
+    >>> df
+    shape: (3, 2)
+    ┌─────────┬─────────┐
+    │ text1   ┆ text2   │
+    │ ---     ┆ ---     │
+    │ str     ┆ str     │
+    ╞═════════╪═════════╡
+    │ abc|ggg ┆ aaa|bbb │
+    │ abc|sss ┆ ccc|aaa │
+    │ ccc|abc ┆ bbb|ccc │
+    └─────────┴─────────┘
+    >>> multicat_one_hot_encode(df, cols=["text1", "text2"], delimiter="|")
+    shape: (3, 7)
+    ┌───────────┬───────────┬───────────┬───────────┬───────────┬───────────┬───────────┐
+    │ text1|abc ┆ text1|ccc ┆ text1|ggg ┆ text1|sss ┆ text2|aaa ┆ text2|bbb ┆ text2|ccc │
+    │ ---       ┆ ---       ┆ ---       ┆ ---       ┆ ---       ┆ ---       ┆ ---       │
+    │ u8        ┆ u8        ┆ u8        ┆ u8        ┆ u8        ┆ u8        ┆ u8        │
+    ╞═══════════╪═══════════╪═══════════╪═══════════╪═══════════╪═══════════╪═══════════╡
+    │ 1         ┆ 0         ┆ 1         ┆ 0         ┆ 1         ┆ 1         ┆ 0         │
+    │ 1         ┆ 0         ┆ 0         ┆ 1         ┆ 1         ┆ 0         ┆ 1         │
+    │ 1         ┆ 1         ┆ 0         ┆ 0         ┆ 0         ┆ 1         ┆ 1         │
+    └───────────┴───────────┴───────────┴───────────┴───────────┴───────────┴───────────┘
+    '''
+    _ = type_checker(df, cols, "string", "multicat_one_hot_encode")
+    temp = df.lazy().select(cols).select(
+        pl.all().str.split("|").explode().unique().implode().list.sort()
+    ).select(cols)
+    one = pl.lit(1, dtype=pl.UInt8) # Avoid casting
+    zero = pl.lit(0, dtype=pl.UInt8) # Avoid casting
+    exprs = []
+    start_index = int(drop_first)
+    for c in temp.collect().get_columns():
+        u = c[0]
+        if len(u) > 1:
+            exprs.extend(
+                pl.when(pl.col(c.name).str.contains(u[i])).then(one).otherwise(zero).alias(c.name + delimiter + u[i])
+                for i in range(start_index, len(u)) if isinstance(u[i], str)
+            )
+        else:
+            logger.info(f"The multicategorical column {c.name} seems to have only 1 unique value. Dropped.")
+
+    if isinstance(df, pl.LazyFrame):
+        return df.blueprint.with_columns(exprs).blueprint.drop(cols)
+    return df.with_columns(exprs).drop(cols)
+
+
+def ordinal_auto_encode(
+    df:PolarsFrame
+    , cols:Optional[list[str]]=None
+    , descending:bool = False
+    , exclude:Optional[list[str]]=None
+) -> PolarsFrame:
+    '''
+    Automatically applies ordinal encoding to the provided columns by the order of the elements. This method is 
+    great for string columns like age ranges, with values like ["10-20", "20-30"], etc. (Beware of string lengths,
+    e.g. if "100-110" exists in age range, then it may mess up the natural order.)
+
+    This will be remembered by blueprint by default.
+        
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars DataFrame
+    cols
+        If not provided, will use all string columns
+    descending
+        If true, will use descending order (0 will be mapped to largest element)
+    exclude
+        Columns to exclude. This is only used when cols is not provided.
+    '''
+    if isinstance(cols, list):
+        _ = type_checker(df, cols, "string", "ordinal_auto_encode")
+        ordinal_list = cols
+    else:
+        ordinal_list = get_string_cols(df, exclude=exclude)
+
+    temp = df.lazy().select(ordinal_list).select(
+        pl.all().unique().implode().list.sort(descending=descending)
+    )
+    for t in temp.collect().get_columns():
+        uniques:pl.Series = t[0]
+        mapping = {t.name: uniques, "to": list(range(len(uniques)))}
+        if isinstance(df, pl.LazyFrame):
+            df = df.blueprint.map_dict(t.name, mapping, "to", None)
+        else:
+            map_tb = pl.DataFrame(mapping)
+            df = df.join(map_tb, on = t.name).with_columns(
+                pl.col("to").alias(t.name)
+            ).drop("to")
+    return df
+
+def ordinal_encode(
+    df:PolarsFrame
+    , ordinal_mapping:dict[str, dict[str,int]]
+    , default:Optional[int] = None
+) -> PolarsFrame:
+    '''
+    Ordinal encode the columns in the ordinal_mapping dictionary.
+
+    This will be remembered by blueprint by default.
+        
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars DataFrame
+    ordinal_mapping
+        A dictionary that looks like {"a":{"a1":1, "a2":2}, ...}
+    default
+        Default value for values not mentioned in the ordinal_mapping dict.
+    '''
+    for c in ordinal_mapping:
+        if c in df.columns:
+            mapping = ordinal_mapping[c]
+            if isinstance(df, pl.LazyFrame):
+                # This relies on the fact that dicts in Python is ordered
+                mapping = {c: mapping.keys(), "to": mapping.values()}
+                df = df.blueprint.map_dict(c, mapping, "to", default)
+            else:
+                mapping = pl.DataFrame((mapping.keys(), mapping.values()), schema=[c, "to"])
+                df = df.join(mapping, on = c, how="left").with_columns(
+                    pl.col("to").fill_null(default).alias(c)
+                ).drop("to")
+        else:
+            logger.warning(f"Found that column {c} is not in df. Skipped.")
+    return df
+
+def smooth_target_encode(
+    df:PolarsFrame
+    , target:str
+    , cols:list[str]
+    , min_samples_leaf:int = 20
+    , smoothing:float = 10.
+    , check_binary:bool=True
+) -> PolarsFrame:
+    '''
+    Smooth target encoding for binary classification. Currently only implemented for binary target.
+
+    This will be remembered by blueprint by default.
+    
+    See https://towardsdatascience.com/dealing-with-categorical-variables-by-using-target-encoder-a0f1733a4c69
+
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars DataFrame
+    target
+        Name of the target column
+    cols
+        If not provided, will use all string columns
+    min_samples_leaf
+        The k in the smoothing factor equation
+    smoothing
+        The f of the smoothing factor equation 
+    check_binary
+        Checks if target is binary. If not, throw an error
+    '''
+    if isinstance(cols, list):
+        _ = type_checker(df, cols, "string", "smooth_target_encode")
+        str_cols = cols
+    else:
+        str_cols = get_string_cols(df)
+    
+    # Only works for binary target for now. There is a non-binary ver of target encode, but I
+    # am just delaying the implementation...
+    if check_binary:
+        if not check_binary_target(df, target):
+            raise ValueError("Target is not binary or not properly encoded.")
+
+    # probability of target = 1
+    p = df.lazy().select(pl.col(target).mean()).collect().item(0,0)
+    is_lazy = isinstance(df, pl.LazyFrame)
+    # If c has null, null will become a group when we group by.
+    for c in str_cols:
+        ref = df.groupby(c).agg(
+            pl.count().alias("cnt"),
+            pl.col(target).mean().alias("cond_p")
+        ).with_columns(
+            (1./(1. + ((-(pl.col("cnt").cast(pl.Float64) - min_samples_leaf))/smoothing).exp())).alias("alpha")
+        ).select(
+            pl.col(c),
+            to = pl.col("alpha") * pl.col("cond_p") + (pl.lit(1) - pl.col("alpha")) * pl.lit(p)
+        ) # If df is lazy, ref is lazy. If df is eager, ref is eager
+        if is_lazy:
+            df = df.blueprint.map_dict(c, ref.collect().to_dict(), "to", None)
+        else: # It is ok to do inner join because all values of c are present in ref.
+            df = df.join(ref, on = c).with_columns(
+                pl.col("to").alias(c)
+            ).drop("to")
+    return df
+
+def _when_then_repl(c:str, repl_map:dict):
+    expr = pl.col(c)
+    for og, repl in repl_map.items():
+        expr = pl.when(pl.col(c).eq(og)).then(repl).otherwise(expr)
+    
+    return expr.alias(c)
+
+def feature_mapping(
+    df:PolarsFrame
+    , mapping: Union[dict[str, dict[Any, Any]], list[pl.Expr] , pl.Expr]
+) -> PolarsFrame:
+    '''
+    Maps specific values of a feature into values provided. This is a common task when the feature columns come with 
+    error codes.
+
+    This will be remembered by blueprint by default.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars dataframe
+    mapping
+        Either a dict like {"a": {999: None, 998: None, 997: None}, ...}, meaning that 999, 998 and 997 in column "a" 
+        should be replaced by null, or a list/a single Polars (when-then) expression(s) like the following,  
+        pl.when(pl.col("a") >= 997).then(None).otherwise(pl.col("a")).alias("a"), which will perform the same mapping 
+        as the dict example. Note that using Polars expression can tackle more complex replacement.
+
+    Example
+    -------
+    >>> df = pl.DataFrame({
+    ...     "a": [1,2,3,998,999],
+    ...     "b": [999, 1,2,3,4]
+    ... })
+    >>> print(df)
+    shape: (5, 2)
+    ┌─────┬─────┐
+    │ a   ┆ b   │
+    │ --- ┆ --- │
+    │ i64 ┆ i64 │
+    ╞═════╪═════╡
+    │ 1   ┆ 999 │
+    │ 2   ┆ 1   │
+    │ 3   ┆ 2   │
+    │ 998 ┆ 3   │
+    │ 999 ┆ 4   │
+    └─────┴─────┘
+    >>> feature_mapping(df, mapping = {"a":{998:None,999:None}, "b":{999:None}})
+    shape: (5, 2)
+    ┌──────┬──────┐
+    │ a    ┆ b    │
+    │ ---  ┆ ---  │
+    │ i64  ┆ i64  │
+    ╞══════╪══════╡
+    │ 1    ┆ null │
+    │ 2    ┆ 1    │
+    │ 3    ┆ 2    │
+    │ null ┆ 3    │
+    │ null ┆ 4    │
+    └──────┴──────┘
+    >>> mapping = [pl.when(pl.col("a")>=998).then(None).otherwise(pl.col("a")).alias("a")
+    ...          , pl.when(pl.col("b")==999).then(None).otherwise(pl.col("b")).alias("b")]
+    >>> feature_mapping(df, mapping)
+    shape: (5, 2)
+    ┌──────┬──────┐
+    │ a    ┆ b    │
+    │ ---  ┆ ---  │
+    │ i64  ┆ i64  │
+    ╞══════╪══════╡
+    │ 1    ┆ null │
+    │ 2    ┆ 1    │
+    │ 3    ┆ 2    │
+    │ null ┆ 3    │
+    │ null ┆ 4    │
+    └──────┴──────┘
+    '''
+    if isinstance(mapping, dict):
+        exprs = []
+        for c, repl_map in mapping.items():
+            exprs.append(_when_then_repl(c, repl_map))
+    elif isinstance(mapping, list):
+        exprs = []
+        for f in mapping:
+            if isinstance(f, pl.Expr):
+                exprs.append(f)
+            else:
+                logger.warn(f"Found {f} is not a Polars expression. Ignored.")
+    elif isinstance(mapping, pl.Expr):
+        exprs = [mapping]
+    else:
+        raise TypeError("The argument `mapping` must be one of the following types: "
+                        "dict[str, dict[Any, Any]] | list[pl.Expr] | pl.Expr")
+    
+    if isinstance(df, pl.LazyFrame):
+        return df.blueprint.with_columns(exprs)
+    return df.with_columns(exprs)
+
+def custom_binning(
+    df:PolarsFrame
+    , cols:list[str]
+    , cuts:list[float]
+    , suffix:str = ""
+) -> PolarsFrame:
+    '''
+    Bins according to the cuts provided. The same cuts will be applied to all columns in cols.
+
+    This will be remembered by blueprint by default.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars DataFrame
+    cols
+        Numerical columns that will be binned
+    cuts
+        A list of floats representing break points in the intervals
+    suffix
+        If you don't want to replace the original columns, you have the option to give the binned column a suffix
+    '''
+    if isinstance(df, pl.LazyFrame):
+        exprs = [
+            pl.col(c).cut(cuts).cast(pl.Utf8).suffix(suffix) for c in cols
+        ]
+        return df.blueprint.with_columns(exprs)
+    else:
+        return df.with_columns(
+            pl.col(c).cut(cuts).cast(pl.Utf8).suffix(suffix) for c in cols
+        )
+    
+def fixed_sized_binning(
+    df:PolarsFrame
+    , cols:list[str]
+    , interval: float
+    , suffix:str = ""
+) -> PolarsFrame:
+    '''
+    Bins according to fixed interval size. The same cuts will be applied to all columns in cols. Bin will 
+    start from min(feature) to max(feature) + interval with step length = interval.
+
+    This will be remembered by blueprint by default.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars DataFrame
+    cols
+        Numerical columns that will be binned
+    interval
+        The fixed sized interval
+    suffix
+        If you don't want to replace the original columns, you have the option to give the binned column a suffix
+    '''
+    bounds = df.lazy().select(cols).select(
+        pl.all().min().prefix("min:")
+        , pl.all().max().prefix("max:")
+    ).collect().row(0)
+    exprs = []
+    n = len(cols)
+    for i, c in enumerate(cols):
+        cut = np.arange(bounds[i], bounds[n+i] + interval, step=interval).tolist()
+        exprs.append(pl.col(c).cut(cut).cast(pl.Utf8).suffix(suffix))
+
+    if isinstance(df, pl.LazyFrame):
+        return df.blueprint.with_columns(exprs)
+    return df.with_columns(exprs)
+
+def quantile_binning(
+    df:PolarsFrame
+    , cols:list[str]
+    , n_bins:int
+    , suffix:str = ""
+) -> PolarsFrame:
+    '''
+    Bin a continuous variable into categories, based on quantile. Null values will be its own category. The same binning
+    rule will be applied to all columns in cols. If you want different n_bins for different columns, chain another 
+    quantile_binning with different cols and n_bins.
+
+    This will be remembered by blueprint by default.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars dataframe
+    cols
+        A list of numeric columns. This has to be supplied by the user because it is not recommended
+        to bin all numerical variables
+    n_bins
+        The number of desired bins. If n_bins = 4, the quantile cuts will be [0.25,0.5,0.74], and 4 
+        categories will be created, which represent values ranging from (-inf, 0.25 quantile value],
+        (0.25 quantile value, 0.5 quantile value],...(0.75 quantile value, inf]
+    suffix
+        If you don't want to replace the original columns, you have the option to give the binned column a suffix
+
+    Example
+    -------
+    >>> df = pl.DataFrame({
+    ...     "a":range(5)
+    ... })
+    >>> df
+    shape: (5, 1)
+    ┌─────┐
+    │ a   │
+    │ --- │
+    │ i64 │
+    ╞═════╡
+    │ 0   │
+    │ 1   │
+    │ 2   │
+    │ 3   │
+    │ 4   │
+    └─────┘
+    >>> quantile_binning(df, cols=["a"], n_bins=4)
+    shape: (5, 1)
+    ┌───────────┐
+    │ a         │
+    │ ---       │
+    │ str       │
+    ╞═══════════╡
+    │ (-inf, 1] │
+    │ (-inf, 1] │
+    │ (1, 2]    │
+    │ (2, 3]    │
+    │ (3, inf]  │
+    └───────────┘
+    '''
+    _ = type_checker(df, cols, "numeric", "quantile_binning")
+    qcuts = np.arange(start=1/n_bins, stop=1.0, step = 1/n_bins)
+    if isinstance(df, pl.LazyFrame):
+        cuts = df.select(cols).select(
+            pl.all().qcut(qcuts).unique().cast(pl.Utf8).str.extract(r"\((.*?),")
+            .cast(pl.Float64).sort().tail(len(qcuts))
+        ).collect()
+        exprs = [
+            pl.col(c).cut(cuts.drop_in_place(c).to_list()).cast(pl.Utf8).suffix(suffix) for c in cols
+        ]
+        return df.blueprint.with_columns(exprs)
+    else: # Eager frame
+        return df.with_columns(
+            pl.col(c).qcut(qcuts).cast(pl.Utf8).suffix(suffix) for c in cols 
+        )
+
+def woe_cat_encode(
+    df:PolarsFrame
+    , target:str
+    , cols:Optional[list[str]]=None
+    , min_count:float = 1.
+    , default: float = -10.
+    , check_binary:bool = True
+) -> PolarsFrame:
+    '''
+    Performs WOE encoding for categorical features. To WOE encode numerical columns, first bin them using
+    custom_binning or quantile_binning. This only works for binary target.
+
+    This will be remembered by blueprint by default.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars dataframe
+    target
+        The name of the target column
+    cols
+        If not provided, all string columns will be used
+    min_count
+        A numerical factor that prevents values like infinity to occur when taking log
+    default
+        Null values will be mapped to default
+    check_binary
+        Whether to check target is binary or not.
+    '''
+    if isinstance(cols, list):
+        _ = type_checker(df, cols, "string", "woe_cat_encode")
+        str_cols = cols
+    else:
+        str_cols = get_string_cols(df)
+
+    if check_binary:
+        if not check_binary_target(df, target):
+            raise ValueError("Target is not binary or not properly encoded or contains nulls.")
+
+    is_lazy = isinstance(df, pl.LazyFrame)
+    for s in str_cols:
+        ref = df.lazy().groupby(s).agg(
+            ev = pl.col(target).sum()
+            , nonev = (pl.lit(1) - pl.col(target)).sum()
+        ).with_columns(
+            ev_rate = (pl.col("ev") + min_count)/(pl.col("ev").sum() + 2.0*min_count)
+            , nonev_rate = (pl.col("nonev") + min_count)/(pl.col("nonev").sum() + 2.0*min_count)
+        ).with_columns(
+            woe = (pl.col("ev_rate")/pl.col("nonev_rate")).log()
+        ).select(
+            pl.col(s)
+            , pl.col("woe")
+        ).collect()
+        if is_lazy:
+            df = df.blueprint.map_dict(s, ref.to_dict(), "woe", default)
+        else:
+            df = df.join(ref, on = s, how="left").with_columns(
+                pl.col("woe").fill_null(default).alias(s)
+            ).drop("woe")
+
     return df
```

### Comparing `dsds-0.0.24/src/dsds/fs.py` & `dsds-0.0.25/python/dsds/fs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,1033 +1,1032 @@
-from .prescreen import (
-    discrete_inferral
-    , check_binary_target
-    , get_numeric_cols
-    , get_unique_count
-    , get_string_cols
-    , type_checker
-    , select
-)
-
-from .type_alias import (
-    PolarsFrame
-    , MRMRStrategy
-    , BinaryModels
-    , CPU_M1
-    , clean_strategy_str
-    , ClassifModel
-)
-from .blueprint import( # Need this for Polars extension to work
-    Blueprint
-)
-from .sample import (
-    train_test_split
-)
-from .metrics import (
-    logloss
-    , roc_auc
-)
-import polars as pl
-import numpy as np
-from typing import Any, Optional, Tuple, Union
-from scipy.spatial import KDTree
-from scipy.special import fdtrc, psi
-from concurrent.futures import ThreadPoolExecutor, as_completed
-import logging
-from tqdm import tqdm
-import math
-from itertools import combinations
-
-logger = logging.getLogger(__name__)
-
-def corr(
-    df: PolarsFrame
-    , target: str
-    , cols: Optional[list[str]] = None
-) -> pl.DataFrame:
-    '''
-    Returns a dataframe with features and their correlation with target.
-
-    Parameters
-    ----------
-    df 
-        Either an eager or lazy Polars dataframe
-    target
-        The target column
-    cols
-        List of numerical columns. If not provided, will use all numerical columns
-    '''
-    if isinstance(cols, list):
-        _ = type_checker(df, cols, "numeric", "corr_filter")
-        nums = cols
-    else:
-        nums = get_numeric_cols(df)
-
-    return df.lazy().select(pl.corr(c, target).abs() for c in nums)\
-        .collect()\
-        .transpose(include_header=True, column_names=["abs_corr"])
-
-def corr_selector(
-    df: PolarsFrame
-    , target: str
-    , threshold: float
-) -> PolarsFrame:
-    '''
-    Keeps only the columns that have |correlation with target| > threshold and the ones that cannot be 
-    processed by the algorithm.
-
-    Parameters
-    ----------
-    df
-        Either an eager or a lazy Polars DataFrame.
-    target
-        The target column
-    threshold
-        The threshold above which the features will be selected
-    '''
-    nums = get_numeric_cols(df, exclude=[target])
-    complement = [f for f in df.columns if f not in nums]
-    # select high corr columns
-    to_select = corr(df, target, nums)\
-                .filter(pl.col("abs_corr") >= threshold)\
-                .get_column("column").to_list()
-    print(f"Selected {len(to_select)} features. There are {len(complement)} columns the algorithm "
-          "cannot process. They are also returned.")
-    # add the complement set
-    return select(df, to_select + complement, persist=True)
-
-def discrete_ig(
-    df:pl.DataFrame
-    , target:str
-    , cols:Optional[list[str]] = None
-) -> pl.DataFrame:
-
-    if isinstance(cols, list):
-        discretes = cols
-    else: # If discrete_cols is not passed, infer it
-        discretes = discrete_inferral(df, exclude=[target])
-
-    # Compute target entropy. This only needs to be done once.
-    target_entropy = df.groupby(target).agg(
-                        (pl.count()).alias("prob(target)") / len(df)
-                    ).get_column("prob(target)").entropy()
-
-    # Get unique count for selected columns. This is because higher unique percentage may skew information gain
-    unique_count = get_unique_count(df.select(discretes)).with_columns(
-        (pl.col("n_unique") / len(df)).alias("unique_pct")
-    ).rename({"column":"feature"})
-
-    conditional_entropy = (
-        df.lazy().groupby(target, pred).agg(
-            pl.count()
-        ).with_columns(
-            (pl.col("count").sum().over(pred) / len(df)).alias("prob(predictive)"),
-            (pl.col("count") / pl.col("count").sum()).alias("prob(target,predictive)")
-        ).select(
-            pl.lit(pred, dtype=pl.Utf8).alias("feature"),
-            (-((pl.col("prob(target,predictive)")/pl.col("prob(predictive)")).log() 
-            * pl.col("prob(target,predictive)")).sum()).alias("conditional_entropy") 
-        )
-        for pred in discretes
-    )
-
-    return pl.concat(conditional_entropy)\
-        .with_columns(
-            target_entropy = pl.lit(target_entropy),
-            information_gain = pl.max(pl.lit(target_entropy) - pl.col("conditional_entropy"), 0)
-        ).join(unique_count, on="feature")\
-        .select("feature", "target_entropy", "conditional_entropy", "unique_pct", "information_gain")\
-        .with_columns(
-            weighted_information_gain = (1 - pl.col("unique_pct")) * pl.col("information_gain")
-        ).collect()
-
-discrete_mi = discrete_ig
-
-def discrete_ig_selector(
-    df:PolarsFrame
-    , target:str
-    , top_k:int
-) -> PolarsFrame:
-    '''
-    Keeps only the top_k features in terms of discrete_ig and the ones that cannot be processed by the algorithm.
-
-    Parameters
-    ----------
-    df
-        Either an eager or lazy dataframe. If lazy, it will be collected
-    target
-        The target column
-    top_k
-        Only the top_k features in terms of discrete_ig will be selected 
-    '''
-    if isinstance(df, pl.LazyFrame):
-        input_data:pl.DataFrame = df.collect()
-    else:
-        input_data:pl.DataFrame = df
-
-    discrete_cols = discrete_inferral(df, exclude=[target])
-    complement = [f for f in df.columns if f not in discrete_cols]
-    to_select = discrete_ig(input_data, target, discrete_cols)\
-        .top_k(by="information_gain", k = top_k)\
-        .get_column("feature").to_list()
-
-    print(f"Selected {len(to_select)} features. There are {len(complement)} columns the "
-          "algorithm cannot process. They are also returned.")
-
-    return select(df, to_select + complement, persist=True)
-
-def mutual_info(
-    df:pl.DataFrame
-    , target:str
-    , conti_cols:list[str]
-    , n_neighbors:int=3
-    , seed:int=42
-    , n_threads:int=CPU_M1
-) -> pl.DataFrame:
-    '''
-    Approximates mutual information (information gain) between the continuous variables and the target. This
-    is essentially the same as sklearn's implementation, except that
-
-    1. This uses Scipy library's kdtree, instead of sklearn's kdtree and nearneighbors
-    2. This uses all cores by default
-    3. There are less "checks" and "safeguards", meaning input data quality is expected to be "good".
-    4. Conti_cols are supposed to be "continuous" variables. In sklearn's mutual_info_classif, if you input a dense 
-        matrix X, it will always be treated as continuous, and if X is sparse, it will be treated as discrete.
-
-    Parameters
-    ----------
-    df
-        An eager dataframe
-    target
-        The target column
-    conti_cols
-        A list of columns with continuous values
-    n_neighbors
-        Number of neighbors. Used in the approximation method provided by the paper
-    seed
-        The random seed used to generate noise, which prevents points to collide and cause difficulty for the
-        nearest neighbor method used in the approximation
-    n_threads
-        The number of threads used in scipy's Kdtree
-
-    Sources
-    -------
-        (1). B. C. Ross “Mutual Information between Discrete and Continuous Data Sets”. PLoS ONE 9(2), 2014.\n
-        (2). A. Kraskov, H. Stogbauer and P. Grassberger, “Estimating mutual information”. Phys. Rev. E 69, 2004. 
-    '''
-    n = len(df)
-    rng = np.random.default_rng(seed)
-    target_col = df.get_column(target).to_numpy().ravel()
-    unique_targets = np.unique(target_col)
-    all_masks = {}
-    for t in unique_targets:
-        all_masks[t] = target_col == t
-        if np.sum(all_masks[t]) <= n_neighbors:
-            raise ValueError(f"The target class {t} must have more than {n_neighbors} values in the dataset.")        
-
-    estimates = []
-    psi_n_and_k = psi(n) + psi(n_neighbors)
-    pbar = tqdm(total = len(conti_cols), desc = "Mutual Info")
-    for col in df.select(conti_cols).get_columns():
-        if col.null_count() > 0:
-            logger.warn(f"Found column {col.name} has null values. It is filled with the mean of the column. "
-                        "It is highly recommended that you impute the column beforehand.")
-            c = col.fill_null(col.mean()).cast(pl.Float64).to_numpy().reshape(-1,1)
-        else:
-            c = col.cast(pl.Float64).to_numpy().reshape(-1,1)
-        # Add random noise here because if inpute data is too big, then adding
-        # a random matrix of the same size will require a lot of memory upfront.
-        c = c + (1e-10 * np.mean(c) * rng.standard_normal(size=c.shape)) 
-        radius = np.empty(n)
-        label_counts = np.empty(n)
-        for t in unique_targets:
-            mask = all_masks[t]
-            c_masked = c[mask]
-            kd1 = KDTree(data=c_masked, leafsize=40)
-            # dd = distances from the points the the k nearest points. +1 because this starts from 0. It is 1 off from 
-            # sklearn's kdtree.
-            dd, _ = kd1.query(c_masked, k = n_neighbors + 1, workers=n_threads)
-            radius[mask] = np.nextafter(dd[:, -1], 0)
-            label_counts[mask] = np.sum(mask)
-
-        kd2 = KDTree(data=c, leafsize=40) 
-        m_all = kd2.query_ball_point(c, r = radius, return_length=True, workers=n_threads)
-        estimates.append(
-            max(0, psi_n_and_k - np.mean(psi(label_counts) + psi(m_all)))
-        ) # smallest is 0
-        pbar.update(1)
-
-    pbar.close()
-    return pl.from_records((conti_cols, estimates), schema=["feature", "estimated_mi"])
-
-# Selectors should always return target
-def mutual_info_selector(
-    df:PolarsFrame
-    , target:str
-    , n_neighbors:int=3
-    , top_k:int = 50
-    , n_threads:int=CPU_M1
-    , seed:int=42
-) -> PolarsFrame:
-    '''
-    Keeps only the top_k features in terms of mutual_info_score and the ones that cannot be processed by the algorithm.
-
-    Parameters
-    ----------
-    df
-        Either an eager or lazy Polars dataframe. If lazy, it will be collected
-    target
-        The target column
-    n_neighbors
-        The n_neighbors parameter in the approximation method
-    top_k
-        The top_k features will ke kept
-    n_threads
-        The max number of workers for multithreading
-    seed
-        Random seed used in approximation to generate noise
-    '''
-    if isinstance(df, pl.LazyFrame):
-        input_data:pl.DataFrame = df.collect()
-    else:
-        input_data:pl.DataFrame = df
-
-    nums = get_numeric_cols(df, exclude=[target])
-    complement = [f for f in df.columns if f not in nums]
-    to_select = mutual_info(input_data, target, nums, n_neighbors, seed, n_threads)\
-                .top_k(by="estimated_mi", k = top_k)\
-                .get_column("feature").to_list()
-
-    logger.info(f"Selected {len(to_select)} features. There are {len(complement)} columns the "
-          "algorithm cannot process. They are also returned.")
-
-    return select(df, to_select + complement, persist=True)
-
-def _f_score(
-    df:PolarsFrame
-    , target:str
-    , num_list:list[str]
-) -> np.ndarray:
-    '''
-    This is the same as what is in f_classif to compute f_score. Except that this only 
-    returns a numpy array of f scores and this does not error check.
-    '''
-    
-    step_one_expr:list[pl.Expr] = [pl.count().alias("cnt")] 
-    step_two_expr:list[pl.Expr] = []
-    for n in num_list:
-        n_sum:str = n + "_sum" # sum of class
-        n_var:str = n + "_var" # var within class
-        step_one_expr.append(
-            pl.col(n).sum().alias(n_sum)
-        )
-        step_one_expr.append(
-            pl.col(n).var(ddof=0).alias(n_var) 
-        )
-        step_two_expr.append(
-            (pl.col(n_sum)/pl.col("cnt") - pl.col(n_sum).sum()/pl.col("cnt").sum()).pow(2).dot(pl.col("cnt")) 
-            / pl.col(n_var).dot(pl.col("cnt"))
-        )
-
-    ref = (
-        df.lazy().groupby(target).agg(step_one_expr)
-        .select(
-            pl.col("cnt").sum().alias("n_samples")
-            , pl.col(target).len().alias("n_classes")
-            , *step_two_expr
-        ).collect()
-    )
-    
-    n_samples = ref.drop_in_place("n_samples")[0]
-    n_classes = ref.drop_in_place("n_classes")[0]
-    df_btw_class = n_classes - 1 
-    df_in_class = n_samples - n_classes
-
-    return ref.to_numpy().ravel() * (df_in_class / df_btw_class)
-
-def f_classif(
-    df:PolarsFrame
-    , target:str
-    , cols:Optional[list[str]]=None
-) -> pl.DataFrame:
-    '''
-    Computes ANOVA one way test, the f value/score and the p value. Equivalent to f_classif in sklearn.feature_selection
-    , but is more dataframe-friendly and faster. 
-
-    Parameters
-    ----------
-    df
-        Either a lazy or an eager Polars DataFrame
-    target
-        The target column
-    cols
-        If not provided, will use all inferred numeric columns
-    '''
-    if isinstance(cols, list):
-        nums = cols
-    else:
-        nums = get_numeric_cols(df, exclude=[target])
-
-    step_one_expr:list[pl.Expr] = [pl.count().alias("cnt")] 
-    step_two_expr:list[pl.Expr] = []
-    for n in nums:
-        n_sum:str = n + "_sum" # sum of class
-        n_var:str = n + "_var" # var within class
-        step_one_expr.append(
-            pl.col(n).sum().alias(n_sum)
-        )
-        step_one_expr.append(
-            pl.col(n).var(ddof=0).alias(n_var) 
-        )
-        step_two_expr.append(
-            (pl.col(n_sum)/pl.col("cnt") - pl.col(n_sum).sum()/pl.col("cnt").sum()).pow(2).dot(pl.col("cnt")) 
-            / pl.col(n_var).dot(pl.col("cnt"))
-        )
-
-    ref = (
-        df.lazy().groupby(target).agg(step_one_expr)
-        .select(
-            pl.col("cnt").sum().alias("n_samples")
-            , pl.col(target).len().alias("n_classes")
-            , *step_two_expr
-        ).collect()
-    )
-    n_samples = ref.drop_in_place("n_samples")[0]
-    n_classes = ref.drop_in_place("n_classes")[0]
-    df_btw_class = n_classes - 1 
-    df_in_class = n_samples - n_classes
-
-    if df_btw_class == 0:
-        raise ZeroDivisionError("Target has only one class.")
-    
-    f_values = ref.to_numpy().ravel() * (df_in_class / df_btw_class)
-    # We should scale this by (df_in_class / df_btw_class) because we did not do this earlier
-    # At this point, f_values should be a pretty small dataframe. 
-    # Cast to numpy, so that fdtrc can process it properly.
-
-    p_values = fdtrc(df_btw_class, df_in_class, f_values) # get p values 
-    return pl.from_records((nums, f_values, p_values), schema=["feature","f_value","p_value"])
-
-def f_score_selector(
-    df:PolarsFrame
-    , target:str
-    , top_k:int
-) -> PolarsFrame:
-    '''
-    Keeps only the top_k features in terms of f-score and the ones that cannot be processed by the algorithm.
-
-    Parameters
-    ----------
-    df
-        Either an eager or lazy Polars dataframe. If lazy, it will be collected
-    target
-        The target column
-    top_k
-        The top_k features will ke kept
-    '''
-    
-    if isinstance(df, pl.LazyFrame):
-        input_data:pl.DataFrame = df.collect()
-    else:
-        input_data:pl.DataFrame = df
-
-    nums = get_numeric_cols(input_data, exclude=[target])
-    complement = [f for f in df.columns if f not in nums]
-    scores = _f_score(input_data, target, nums)
-    to_select = pl.DataFrame({"feature":nums, "fscore":scores})\
-        .top_k(by = "fscore", k = top_k)\
-        .get_column("feature").to_list()
-
-    print(f"Selected {len(to_select)} features. There are {len(complement)} columns the "
-          "algorithm cannot process. They are also returned.")
-
-    return select(df, to_select + complement, persist=True)
-
-def _mrmr_underlying_score(
-    df:pl.DataFrame
-    , target:str
-    , nums:list[str]
-    , strategy:MRMRStrategy
-    , params:dict[str,Any]
-) -> np.ndarray:
-    
-    logger.info(f"Running {strategy} to determine feature relevance...")
-    s = clean_strategy_str(strategy)
-    if s in ("fscore", "f", "f_score"):
-        scores = _f_score(df, target, nums)
-    elif s in ("rf", "random_forest"):
-        from sklearn.ensemble import RandomForestClassifier
-        print("Random forest is not deterministic by default. Results may vary.")
-        rf = RandomForestClassifier(**params)
-        rf.fit(df[nums].to_numpy(), df[target].to_numpy().ravel())
-        scores = rf.feature_importances_
-    elif s in ("xgb", "xgboost"):
-        from xgboost import XGBClassifier
-        print("XGB is not deterministic by default. Results may vary.")
-        xgb = XGBClassifier(**params)
-        xgb.fit(df[nums].to_numpy(), df[target].to_numpy().ravel())
-        scores = xgb.feature_importances_
-    elif s in ("mis", "mutual_info_score"):
-        scores = mutual_info(df, conti_cols=nums, target=target).get_column("estimated_mi").to_numpy().ravel()
-    elif s in ("lgbm", "lightgbm"):
-        from lightgbm import LGBMClassifier
-        print("LightGBM is not deterministic by default. Results may vary.")
-        lgbm = LGBMClassifier(**params)
-        lgbm.fit(df[nums].to_numpy(), df[target].to_numpy().ravel())
-        scores = lgbm.feature_importances_
-    else: # Pythonic nonsense
-        raise ValueError(f"The strategy {strategy} is not a valid MRMR Strategy.")
-    
-    return scores
-
-def mrmr(
-    df:pl.DataFrame
-    , target:str
-    , k:int
-    , cols:Optional[list[str]] = None
-    , strategy: MRMRStrategy = "fscore"
-    , params:Optional[dict[str,Any]] = None
-    , low_memory:bool=False
-) -> list[str]:
-    '''
-    Implements MRMR. Will add a few more strategies in the future. Likely only strategies for numerators
-    , aka relevance. Right now xgb, lgbm and rf strategies only work for classification problems.
-
-    Currently this only supports classification.
-
-    Parameters
-    ----------
-    df
-        An eager Polars Dataframe
-    target
-        Target column
-    k
-        Top k features to keep
-    cols
-        Optional. A list of numerical columns. If not provided, all numerical columns will be used.
-    strategy
-        MRMR strategy. By default, `fscore` will be used.
-    params
-        Optional. If a model strategy is selected (`rf`, `xgb`, `lgbm`), params is a dict of 
-        parameters for the model.
-    low_memory
-        Whether to do some computation all at once, which uses more memory at once, or do some 
-        computation when needed, which uses less memory at any given time.
-    '''
-    if isinstance(cols, list):
-        nums = cols
-    else:
-        nums = get_numeric_cols(df, exclude=[target])
-
-    s = clean_strategy_str(strategy)
-    scores = _mrmr_underlying_score(df
-        , target = target
-        , nums = nums
-        , strategy = s
-        , params = {} if params is None else params
-    )
-
-    if low_memory:
-        df_local = df.select(nums)
-    else: # this could potentially double memory usage. so I provided a low_memory flag.
-        df_local = df.select(nums).with_columns(
-            (pl.col(f) - pl.col(f).mean())/pl.col(f).std() for f in nums
-        ) # Note that if we get a const column, the entire column will be NaN
-
-    output_size = min(k, len(nums))
-    print(f"Found {len(nums)} total features to select from. Proceeding to select top {output_size} features.")
-    cumulating_abs_corr = np.zeros(len(nums)) # For each feature at index i, we keep a cumulating sum
-    top_idx = np.argmax(scores)
-    selected = [nums[top_idx]]
-    pbar = tqdm(total=output_size, desc = f"MRMR, {s}")
-    pbar.update(1)
-    for j in range(1, output_size): 
-        argmax = -1
-        current_max = -1
-        last_selected_col = df_local.drop_in_place(selected[-1])
-        if low_memory: # normalize if in low memory mode.
-            last_selected_col = (last_selected_col - last_selected_col.mean())/last_selected_col.std()
-        for i,f in enumerate(nums):
-            if f not in selected:
-                # Left = cumulating sum of abs corr
-                # Right = abs correlation btw last_selected and f
-                candidate_col = df_local.get_column(f)
-                if low_memory: # normalize if in low memory mode.
-                    candidate_col = (candidate_col - candidate_col.mean())/candidate_col.std()
-
-                a = (last_selected_col*candidate_col).mean()
-                # In the rare case this calculation yields a NaN, we punish by adding 1.
-                # Otherwise, proceed as usual. +1 is a punishment because
-                # |corr| can be at most 1. So we are enlarging the denominator, thus reducing the score.
-                cumulating_abs_corr[i] += 1 if np.isnan(a) else np.abs(a)
-                denominator = cumulating_abs_corr[i]/j 
-                new_score = scores[i] / denominator
-                if new_score > current_max:
-                    current_max = new_score
-                    argmax = i
-        selected.append(nums[argmax])
-        pbar.update(1)
-
-    pbar.close()
-    print("Output is sorted in order of selection (max relevance min redundancy).")
-    return selected
-
-def mrmr_selector(
-    df:PolarsFrame
-    , target:str
-    , top_k:int
-    , strategy:MRMRStrategy = "fscore"
-    , params:Optional[dict[str,Any]] = None
-    , low_memory:bool=False
-) -> PolarsFrame:
-    '''
-    Keeps only the top_k (first k) features selected by MRMR and the ones that cannot be processed by the algorithm.
-
-    Parameters
-    ----------
-    df
-        Either an eager or lazy Polars dataframe. If lazy, it will be collected
-    target
-        The target column
-    top_k
-        The top_k features will ke kept
-    strategy
-        One of 'f', 'xgb', 'rf', 'mis', 'lgbm'. It will use the corresponding method to compute feature relevance
-    params
-        If any modeled relevance is used, e.g. 'rf', 'lgbm' or 'xgb', then this will be the param dict for the model
-    low_memory
-        If true, use less memory. But the computation will take longer
-    '''
-    if isinstance(df, pl.LazyFrame):
-        input_data:pl.DataFrame = df.collect()
-    else:
-        input_data:pl.DataFrame = df
-
-    nums = get_numeric_cols(input_data, exclude=[target])
-    s = clean_strategy_str(strategy)
-    to_select = mrmr(input_data, target, top_k, nums, s, params, low_memory)
-    logger.info(f"Selected {len(to_select)} features. There are {len(df.columns) - len(to_select)} columns the "
-          "algorithm cannot process. They are also returned.")
-    to_select.extend(f for f in df.columns if f not in nums)
-    return select(df, to_select, persist=True)
-
-def knock_out_mrmr(
-    df:pl.DataFrame
-    , target:str
-    , k:int 
-    , cols:Optional[list[str]] = None
-    , corr_threshold:float = 0.7
-    , strategy:MRMRStrategy = "fscore"
-    , params:Optional[dict[str,Any]] = None
-) -> list[str]:
-    '''
-    Essentially the same as vanilla MRMR. Instead of using sum(abs(corr)) to "weigh down" correlated 
-    variables, here we use a simpler knock out rule based on absolute correlation. We go down the list
-    according to importance, take top one, knock out all other features that are highly correlated with
-    it, take the next top feature that has not been knocked out, continue, until we pick enough features
-    or there is no feature left.
-
-    Inspired by the package Featurewiz and its creator.
-
-    Parameters
-    ----------
-    df
-        An eager Polars Dataframe
-    target
-        The target column
-    k
-        The top k features to return
-    cols
-        Numerical columns to select from. If not provided, all numeric columns will be used
-    corr_threshold
-        The threshold above which correlation is considered too high. This means if A has high correlation to B, then
-        B will not be selected if A is
-    strategy
-        One of 'f', 'xgb', 'rf', 'mis', 'lgbm'. It will use the corresponding method to compute feature relevance
-    params
-        If any modeled relevance is used, e.g. 'rf', 'lgbm' or 'xgb', then this will be the param dict for the model
-    '''
-    if isinstance(cols, list):
-        nums = cols
-    else:
-        nums = get_numeric_cols(df, exclude=[target])
-
-    s = clean_strategy_str(strategy)
-    scores = _mrmr_underlying_score(df
-        , target = target
-        , nums = nums
-        , strategy = s
-        , params = {} if params is None else params
-    )
-
-    # Set up
-    low_corr = np.abs(df[nums].corr().to_numpy()) < corr_threshold
-    surviving_indices = np.full(shape=len(nums), fill_value=True) # an array of booleans
-    scores = sorted(enumerate(scores), key=lambda x:x[1], reverse=True)
-    selected = []
-    count = 0
-    output_size = min(k, len(nums))
-    pbar = tqdm(total=output_size)
-    # Run the knock outs
-    for i, _ in scores:
-        if surviving_indices[i]:
-            selected.append(nums[i])
-            surviving_indices = surviving_indices & low_corr[:,i]
-            count += 1
-            pbar.update(1)
-        if count >= output_size:
-            break
-
-    pbar.close()
-    if count < k:
-        print(f"Found only {count}/{k} number of values because most of them are highly correlated and the knock out "
-              "rule eliminates most of them.")
-
-    print("Output is sorted in order of selection (max relevance min redundancy).")
-    return selected
-
-def knock_out_mrmr_selector(
-    df:PolarsFrame
-    , target:str
-    , top_k:int 
-    , corr_threshold:float = 0.7
-    , strategy:MRMRStrategy = "fscore"
-    , params:Optional[dict[str,Any]] = None
-) -> PolarsFrame:
-    '''
-    Keeps only the top_k (first k) features selected by MRMR and the ones that cannot be processed by the algorithm.
-
-    Parameters
-    ----------
-    df
-        Either an eager or lazy Polars dataframe. If lazy, it will be collected
-    target
-        The target column
-    top_k
-        The top_k features will ke kept
-    corr_threshold
-        The threshold above which correlation is considered too high. This means if A has high correlation to B, then
-        B will not be selected if A is
-    strategy
-        One of 'f', 'xgb', 'rf', 'mis', 'lgbm'. It will use the corresponding method to compute feature relevance
-    params
-        If any modeled relevance is used, e.g. 'rf', 'lgbm' or 'xgb', then this will be the param dict for the model
-    '''
-    if isinstance(df, pl.LazyFrame):
-        input_data:pl.DataFrame = df.collect()
-    else:
-        input_data:pl.DataFrame = df
-
-    nums = get_numeric_cols(df, exclude=[target])
-    complement = [f for f in df.columns if f not in nums]
-    s = clean_strategy_str(strategy)
-    to_select = knock_out_mrmr(input_data, target, top_k, nums, s, corr_threshold, params)
-    print(f"Selected {len(to_select)} features. There are {len(complement)} columns the "
-          "algorithm cannot process. They are also returned.")
-    
-    return select(df, to_select + complement, persist=True)
-
-# Selectors for the methods below are not yet implemented
-
-def woe_iv(
-    df:PolarsFrame
-    , target:str
-    , cols:Optional[list[str]]=None
-    , min_count:float = 1.
-    , check_binary:bool = True
-) -> pl.DataFrame:
-    '''
-    Computes information values for categorical variables. Notice that by using binning methods provided in 
-    dsds.transform, you can turn numerical values into categorical bins.
-
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars Dataframe
-    target
-        The target column
-    cols
-        If not provided, will use all string columns
-    min_count
-        A regularization term that prevents ln(0). This is the same as category_encoders package's 
-        regularization parameter.
-    check_binary
-        Whether to check if target is binary or not
-    '''
-    if isinstance(cols, list):
-        _ = type_checker(df, cols, "string", "woe_iv")
-        input_cols = cols
-    else:
-        input_cols = get_string_cols(df)
-
-    if check_binary:
-        if not check_binary_target(df, target):
-            raise ValueError("Target is not binary or not properly encoded.")
-
-    results = (
-        df.lazy().groupby(s).agg(
-            ev = pl.col(target).sum()
-            , nonev = (pl.lit(1) - pl.col(target)).sum()
-        ).with_columns(
-            ev_rate = (pl.col("ev") + min_count)/(pl.col("ev").sum() + 2.0*min_count)
-            , nonev_rate = (pl.col("nonev") + min_count)/(pl.col("nonev").sum() + 2.0*min_count)
-        ).with_columns(
-            woe = (pl.col("ev_rate")/pl.col("nonev_rate")).log()
-        ).select(
-            pl.lit(s).alias("feature")
-            , pl.col(s).alias("value")
-            , pl.col("woe")
-            , information_value = ((pl.col("ev_rate")-pl.col("nonev_rate")) * pl.col("woe")).sum()
-        )
-        for s in input_cols
-    )
-    return pl.concat(results).collect()
-
-def _binary_model_init(
-    model_str:BinaryModels
-    , params: dict[str, Any]
-) -> ClassifModel:
-    '''
-    Returns a classification model. If n_job parameter is not specified, it will default to -1.
-
-    Parameters
-    ----------
-    model_str
-        One of 'lr', 'lgbm', 'xgb', 'rf'
-    params
-        The parameters for the model specified
-    '''
-    if "n_jobs" not in params:
-        params["n_jobs"] = -1
-
-    if model_str in ("logistic", "lr"):
-        from sklearn.linear_model import LogisticRegression
-        model = LogisticRegression(**params)
-    elif model_str in ("rf", "random_forest"):
-        from sklearn.ensemble import RandomForestClassifier
-        model = RandomForestClassifier(**params)
-    elif model_str in ("xgb", "xgboost"):
-        from xgboost import XGBClassifier
-        model = XGBClassifier(**params)
-    elif model_str in ("lgbm", "lightgbm"):
-        from lightgbm import LGBMClassifier
-        model = LGBMClassifier(**params)
-    else:
-        raise ValueError(f"The model {model_str} is not available.")
-    
-    return model
-
-def _fc_fi(
-    model_str:str
-    , params:dict[str, Any]
-    , target:str
-    , features: Union[Tuple,list[str]]
-    , train: pl.DataFrame
-    , test: pl.DataFrame
-)-> Tuple[Tuple[Tuple, float, float], np.ndarray]:
-    '''
-    Creates a classification model, evaluations model with log loss and roc_auc for each feature combination
-    (fc) and feature importance (fi). It will return a tuple of the following structure: 
-    ( (feature combination, log loss, roc_auc), feature_importance array) 
-
-    Parameters
-    ----------
-    model_str
-        One of 'lr', 'lgbm', 'xgb', 'rf'
-    params
-        The parameters for the model specified
-    target
-        The target column
-    features
-        Either a tuple or a list which represents the current feature combination
-    train
-        The training dataset. Must be eager
-    test
-        The testing dataset on which log loss and roc_auc will be evaluation. Must be eager
-    '''
-    estimator = _binary_model_init(model_str, params)
-    _ = estimator.fit(train.select(features), train[target])
-    y_pred = estimator.predict_proba(test.select(features))[:,1]
-    y_test = test[target].to_numpy()
-    fc_rec = (
-        features,
-        logloss(y_test, y_pred, check_binary=False),
-        roc_auc(y_test, y_pred, check_binary=False)
-    )
-    if model_str in ("lr", "logistic"):
-        fi_rec = np.abs(estimator.coef_).ravel()
-    else:
-        fi_rec = estimator.feature_importances_
-    # fc_rec feature comb record, fi_rec feature importance record
-    return fc_rec, fi_rec
-
-# ebfs: stands for Exhaustive Binary Feature Selection
-def ebfs(
-    df:pl.DataFrame
-    , target:str
-    , model_str:BinaryModels
-    , params:dict[str, Any]
-    , n_comb: int = 3
-    , train_frac:float = 0.75
-) -> Tuple[pl.DataFrame, pl.DataFrame]:
-    '''
-    Suppose we have n features and n_comb = 2. This method will select all (n choose 2) 
-    combinations of features, split dataset into a train and a test for each combination, 
-    train a model on train, and compute feature importance and roc_auc and logloss, and 
-    then finally put everything into two separate dataframes, the first of which will contain 
-    the feature combinations and model performances, and the second will contain the min, avg, 
-    max and var of feature importance of each feature in all its occurences in the training rounds.
-
-    Notice since we split data into train and test every time for a different feature combination, the 
-    average feature importance we derive naturally are `cross-validated` to a certain degree.
-
-    This method will be extremely slow if (n choose n_comb) is a big number. All numerical columns 
-    will be taken as potential features. Please encode the string columns if you want to use them
-    as features here.
-
-    If n_jobs is not provided in params, it will be defaulted to -1.
-
-    This will return a feature combination (fc) summary and a feature importance (fi) summary. 
-
-    Parameters
-    ----------
-    df
-        An eager Polars DataFrame
-    target
-        The target column
-    model_str
-        one of 'lr', 'lgbm', 'xgb', 'rf'
-    params
-        Parameters for the model
-    n_comb
-        We will run this for all n choose n_comb combinations of features
-    '''
-    features = get_numeric_cols(df, exclude=[target])
-    fi = {f:[] for f in features}
-    records = []
-    pbar = tqdm(total=math.comb(len(features), n_comb), desc="Tested Combinations")
-    df_keep = df.select(features + [target])
-    for comb in combinations(features, r=n_comb):
-        train, test = train_test_split(df_keep, train_frac)
-        fc_rec, fi_rec = _fc_fi(model_str, params, target, comb, train, test) 
-        records.append(fc_rec)
-        for f, i in zip(fc_rec[0], fi_rec):
-            fi[f].append(i)
-        pbar.update(1)
-
-    fc_summary = pl.from_records(records, schema=["combination", "logloss", "roc_auc"])
-    stats = [
-        (f, len(fi[f]), np.min(fi[f]), np.mean(fi[f]), np.max(fi[f]), np.std(fi[f])) for f in fi
-    ]
-    fi_summary = pl.from_records(stats, schema=["feature", "occurrences", "fi_min", "fi_mean", "fi_max", "fi_std"])
-    pbar.close()
-    return fc_summary, fi_summary
-
-def ebfs_fc_filter(
-    fc: pl.DataFrame
-    , logloss_threshold:float
-    , roc_auc_threshold:float
-) -> list[str]:
-    '''
-    A filter method based on the feature combination result of ebfs.
-
-    Parameters
-    ----------
-    fc
-        The feature combination result from ebfs
-    logloss_threshold
-        The maximum logloss for the combination to be kept
-    roc_auc_threshold
-        The minimum roc_auc for the combination to be kept
-    '''
-    return fc.filter(
-        (pl.col("logloss") <= logloss_threshold)
-        & (pl.col("roc_auc") >= roc_auc_threshold)
-    ).get_column("combination").explode().unique().to_list()
-
-def _permute_importance(
-    model:ClassifModel
-    , X:pl.DataFrame
-    , y: np.ndarray
-    , index:int
-    , k: int
-) -> Tuple[float, int]:
-    '''
-    Computes permutation importance for a single feature.
-
-    Parameters
-    ----------
-    model
-        A trained classification model
-    X
-        An eager dataframe on which we shuffle the column at the given index and train the model
-    y
-        The target column turned into np.ndarray
-    index
-        The index of the column in X to shuffle
-    k
-        The number of times to repeat the shuffling
-    '''
-    test_score = 0.
-    c = X.columns[index] # column to shuffle
-    for _ in range(k):
-        shuffled_df = X.with_columns(
-            pl.col(c).shuffle(seed=42)
-        )
-        test_score += roc_auc(y, model.predict_proba(shuffled_df)[:, -1])
-
-    return test_score, index
-
-def permutation_importance(
-    df:pl.DataFrame
-    , target:str
-    , model_str:BinaryModels
-    , params:dict[str, Any]
-    , k:int = 5
-) -> pl.DataFrame:
-    '''
-    Computes permutation importance for every non-target column in df. Please make sure all columns are properly encoded
-    or transformed before calling this.
-    
-    Only works for binary classification and score = roc_auc for now.
-
-    Parameters
-    ----------
-    df
-        An eager Polars DataFrame
-    target
-        The target column
-    model_str
-        One of 'lr', 'lgbm', 'xgb', 'rf'
-    params
-        Parameters for the model
-    k
-        Permute the same feature k times
-    '''
-    features = df.columns
-    features.remove(target)
-    _ = type_checker(df, features, "numeric", "permutation_importance")
-    estimator = _binary_model_init(model_str, params)
-    estimator.fit(df[features], df[target])
-    X = df[features]
-    y = df[target].to_numpy()
-    score = roc_auc(y, estimator.predict_proba(X)[:, -1])
-    pbar = tqdm(total=len(features), desc="Analyzing Features")
-    imp = np.zeros(shape=len(features))
-    with ThreadPoolExecutor(max_workers=CPU_M1) as ex:
-        futures = (
-            ex.submit(
-                _permute_importance,
-                estimator,
-                X,
-                y,
-                j,
-                k
-            )
-            for j in range(len(features))
-        )
-        for f in as_completed(futures):
-            test_score, i = f.result()
-            imp[i] = score - (1/k)*test_score
-            pbar.update(1)
-
+from .prescreen import (
+    discrete_inferral
+    , check_binary_target
+    , get_numeric_cols
+    , get_unique_count
+    , get_string_cols
+    , type_checker
+    , select
+)
+
+from .type_alias import (
+    PolarsFrame
+    , MRMRStrategy
+    , BinaryModels
+    , CPU_M1
+    , clean_strategy_str
+    , ClassifModel
+)
+from .blueprint import( # Need this for Polars extension to work
+    Blueprint
+)
+from .sample import (
+    train_test_split
+)
+from .metrics import (
+    logloss
+    , roc_auc
+)
+import polars as pl
+import numpy as np
+from typing import Any, Optional, Tuple, Union
+from scipy.spatial import KDTree
+from scipy.special import fdtrc, psi
+from concurrent.futures import ThreadPoolExecutor, as_completed
+import logging
+from tqdm import tqdm
+import math
+from itertools import combinations
+
+logger = logging.getLogger(__name__)
+
+# todo()!
+# 
+
+def corr(
+    df: PolarsFrame
+    , target: str
+    , cols: Optional[list[str]] = None
+) -> pl.DataFrame:
+    '''
+    Returns a dataframe with features and their correlation with target.
+
+    Parameters
+    ----------
+    df 
+        Either an eager or lazy Polars dataframe
+    target
+        The target column
+    cols
+        List of numerical columns. If not provided, will use all numerical columns
+    '''
+    if isinstance(cols, list):
+        _ = type_checker(df, cols, "numeric", "corr_filter")
+        nums = cols
+    else:
+        nums = get_numeric_cols(df)
+
+    return df.lazy().select(pl.corr(c, target).abs() for c in nums)\
+        .collect()\
+        .transpose(include_header=True, column_names=["abs_corr"])
+
+def corr_selector(
+    df: PolarsFrame
+    , target: str
+    , threshold: float
+) -> PolarsFrame:
+    '''
+    Keeps only the columns that have |correlation with target| > threshold and the ones that cannot be 
+    processed by the algorithm.
+
+    Parameters
+    ----------
+    df
+        Either an eager or a lazy Polars DataFrame.
+    target
+        The target column
+    threshold
+        The threshold above which the features will be selected
+    '''
+    nums = get_numeric_cols(df, exclude=[target])
+    complement = [f for f in df.columns if f not in nums]
+    # select high corr columns
+    to_select = corr(df, target, nums)\
+                .filter(pl.col("abs_corr") >= threshold)["column"].to_list()
+    print(f"Selected {len(to_select)} features. There are {len(complement)} columns the algorithm "
+          "cannot process. They are also returned.")
+    # add the complement set
+    return select(df, to_select + complement, persist=True)
+
+def discrete_ig(
+    df:pl.DataFrame
+    , target:str
+    , cols:Optional[list[str]] = None
+) -> pl.DataFrame:
+
+    if isinstance(cols, list):
+        discretes = cols
+    else: # If discrete_cols is not passed, infer it.
+        discretes = discrete_inferral(df, exclude=[target])
+
+    # Compute target entropy. This only needs to be done once.
+    target_entropy = df.groupby(target).agg(
+                        (pl.count()).alias("prob(target)") / len(df)
+                    )["prob(target)"].entropy()
+
+    # Get unique count for selected columns. This is because higher unique percentage may skew information gain
+    unique_count = get_unique_count(df.select(discretes)).with_columns(
+        (pl.col("n_unique") / len(df)).alias("unique_pct")
+    ).rename({"column":"feature"})
+
+    conditional_entropy = [
+        df.lazy().groupby(target, pred).agg(
+            pl.count()
+        ).with_columns(
+            (pl.col("count").sum().over(pred) / len(df)).alias("prob(predictive)"),
+            (pl.col("count") / pl.col("count").sum()).alias("prob(target,predictive)")
+        ).select(
+            pl.lit(pred, dtype=pl.Utf8).alias("feature"),
+            (-((pl.col("prob(target,predictive)")/pl.col("prob(predictive)")).log() 
+            * pl.col("prob(target,predictive)")).sum()).alias("conditional_entropy") 
+        )
+        for pred in discretes
+    ]
+
+    return pl.concat(pl.collect_all(conditional_entropy))\
+        .with_columns(
+            target_entropy = pl.lit(target_entropy),
+            information_gain = pl.max(pl.lit(target_entropy) - pl.col("conditional_entropy"), 0)
+        ).join(unique_count, on="feature")\
+        .select("feature", "target_entropy", "conditional_entropy", "unique_pct", "information_gain")\
+        .with_columns(
+            weighted_information_gain = (1 - pl.col("unique_pct")) * pl.col("information_gain")
+        )
+
+discrete_mi = discrete_ig
+
+def discrete_ig_selector(
+    df:PolarsFrame
+    , target:str
+    , top_k:int
+) -> PolarsFrame:
+    '''
+    Keeps only the top_k features in terms of discrete_ig and the ones that cannot be processed by the algorithm.
+
+    Parameters
+    ----------
+    df
+        Either an eager or lazy dataframe. If lazy, it will be collected
+    target
+        The target column
+    top_k
+        Only the top_k features in terms of discrete_ig will be selected 
+    '''
+    if isinstance(df, pl.LazyFrame):
+        input_data:pl.DataFrame = df.collect()
+    else:
+        input_data:pl.DataFrame = df
+
+    discrete_cols = discrete_inferral(df, exclude=[target])
+    complement = [f for f in df.columns if f not in discrete_cols]
+    to_select = discrete_ig(input_data, target, discrete_cols)\
+        .top_k(by="information_gain", k = top_k)["feature"].to_list()
+
+    print(f"Selected {len(to_select)} features. There are {len(complement)} columns the "
+          "algorithm cannot process. They are also returned.")
+
+    return select(df, to_select + complement, persist=True)
+
+def mutual_info(
+    df:pl.DataFrame
+    , target:str
+    , conti_cols:list[str]
+    , n_neighbors:int=3
+    , seed:int=42
+    , n_threads:int=CPU_M1
+) -> pl.DataFrame:
+    '''
+    Approximates mutual information (information gain) between the continuous variables and the target. This
+    is essentially the same as sklearn's implementation, except that
+
+    1. This uses Scipy library's kdtree, instead of sklearn's kdtree and nearneighbors
+    2. This uses all cores by default
+    3. There are less "checks" and "safeguards", meaning input data quality is expected to be "good".
+    4. Conti_cols are supposed to be "continuous" variables. In sklearn's mutual_info_classif, if you input a dense 
+        matrix X, it will always be treated as continuous, and if X is sparse, it will be treated as discrete.
+
+    Parameters
+    ----------
+    df
+        An eager dataframe
+    target
+        The target column
+    conti_cols
+        A list of columns with continuous values
+    n_neighbors
+        Number of neighbors. Used in the approximation method provided by the paper
+    seed
+        The random seed used to generate noise, which prevents points to collide and cause difficulty for the
+        nearest neighbor method used in the approximation
+    n_threads
+        The number of threads used in scipy's Kdtree
+
+    Sources
+    -------
+        (1). B. C. Ross “Mutual Information between Discrete and Continuous Data Sets”. PLoS ONE 9(2), 2014.\n
+        (2). A. Kraskov, H. Stogbauer and P. Grassberger, “Estimating mutual information”. Phys. Rev. E 69, 2004. 
+    '''
+    n = len(df)
+    rng = np.random.default_rng(seed)
+    target_col = df[target].to_numpy().ravel()
+    unique_targets = np.unique(target_col)
+    all_masks = {}
+    for t in unique_targets:
+        all_masks[t] = target_col == t
+        if np.sum(all_masks[t]) <= n_neighbors:
+            raise ValueError(f"The target class {t} must have more than {n_neighbors} values in the dataset.")        
+
+    estimates = []
+    psi_n_and_k = psi(n) + psi(n_neighbors)
+    pbar = tqdm(total = len(conti_cols), desc = "Mutual Info")
+    for col in df.select(conti_cols).get_columns():
+        if col.null_count() > 0:
+            logger.warn(f"Found column {col.name} has null values. It is filled with the mean of the column. "
+                        "It is highly recommended that you impute the column beforehand.")
+            c = col.fill_null(col.mean()).cast(pl.Float64).to_numpy().reshape(-1,1)
+        else:
+            c = col.cast(pl.Float64).to_numpy().reshape(-1,1)
+        # Add random noise here because if inpute data is too big, then adding
+        # a random matrix of the same size will require a lot of memory upfront.
+        c = c + (1e-10 * np.mean(c) * rng.standard_normal(size=c.shape)) 
+        radius = np.empty(n)
+        label_counts = np.empty(n)
+        for t in unique_targets:
+            mask = all_masks[t]
+            c_masked = c[mask]
+            kd1 = KDTree(data=c_masked, leafsize=40)
+            # dd = distances from the points the the k nearest points. +1 because this starts from 0. It is 1 off from 
+            # sklearn's kdtree.
+            dd, _ = kd1.query(c_masked, k = n_neighbors + 1, workers=n_threads)
+            radius[mask] = np.nextafter(dd[:, -1], 0)
+            label_counts[mask] = np.sum(mask)
+
+        kd2 = KDTree(data=c, leafsize=40) 
+        m_all = kd2.query_ball_point(c, r = radius, return_length=True, workers=n_threads)
+        estimates.append(
+            max(0, psi_n_and_k - np.mean(psi(label_counts) + psi(m_all)))
+        ) # smallest is 0
+        pbar.update(1)
+
+    pbar.close()
+    return pl.from_records((conti_cols, estimates), schema=["feature", "estimated_mi"])
+
+# Selectors should always return target
+def mutual_info_selector(
+    df:PolarsFrame
+    , target:str
+    , n_neighbors:int=3
+    , top_k:int = 50
+    , n_threads:int=CPU_M1
+    , seed:int=42
+) -> PolarsFrame:
+    '''
+    Keeps only the top_k features in terms of mutual_info_score and the ones that cannot be processed by the algorithm.
+
+    Parameters
+    ----------
+    df
+        Either an eager or lazy Polars dataframe. If lazy, it will be collected
+    target
+        The target column
+    n_neighbors
+        The n_neighbors parameter in the approximation method
+    top_k
+        The top_k features will ke kept
+    n_threads
+        The max number of workers for multithreading
+    seed
+        Random seed used in approximation to generate noise
+    '''
+    if isinstance(df, pl.LazyFrame):
+        input_data:pl.DataFrame = df.collect()
+    else:
+        input_data:pl.DataFrame = df
+
+    nums = get_numeric_cols(df, exclude=[target])
+    complement = [f for f in df.columns if f not in nums]
+    to_select = mutual_info(input_data, target, nums, n_neighbors, seed, n_threads)\
+                .top_k(by="estimated_mi", k = top_k)["feature"].to_list()
+
+    logger.info(f"Selected {len(to_select)} features. There are {len(complement)} columns the "
+          "algorithm cannot process. They are also returned.")
+
+    return select(df, to_select + complement, persist=True)
+
+def _f_score(
+    df:PolarsFrame
+    , target:str
+    , num_list:list[str]
+) -> np.ndarray:
+    '''
+    This is the same as what is in f_classif to compute f_score. Except that this only 
+    returns a numpy array of f scores and this does not error check.
+    '''
+    
+    step_one_expr:list[pl.Expr] = [pl.count().alias("cnt")] 
+    step_two_expr:list[pl.Expr] = []
+    for n in num_list:
+        n_sum:str = n + "_sum" # sum of class
+        n_var:str = n + "_var" # var within class
+        step_one_expr.append(
+            pl.col(n).sum().alias(n_sum)
+        )
+        step_one_expr.append(
+            pl.col(n).var(ddof=0).alias(n_var) 
+        )
+        step_two_expr.append(
+            (pl.col(n_sum)/pl.col("cnt") - pl.col(n_sum).sum()/pl.col("cnt").sum()).pow(2).dot(pl.col("cnt")) 
+            / pl.col(n_var).dot(pl.col("cnt"))
+        )
+
+    ref = (
+        df.lazy().groupby(target).agg(step_one_expr)
+        .select(
+            pl.col("cnt").sum().alias("n_samples")
+            , pl.col(target).count().alias("n_classes")
+            , *step_two_expr
+        ).collect()
+    )
+    
+    n_samples = ref.drop_in_place("n_samples")[0]
+    n_classes = ref.drop_in_place("n_classes")[0]
+    df_btw_class = n_classes - 1 
+    df_in_class = n_samples - n_classes
+
+    return ref.to_numpy().ravel() * (df_in_class / df_btw_class)
+
+def f_classif(
+    df:PolarsFrame
+    , target:str
+    , cols:Optional[list[str]]=None
+) -> pl.DataFrame:
+    '''
+    Computes ANOVA one way test, the f value/score and the p value. Equivalent to f_classif in sklearn.feature_selection
+    , but is more dataframe-friendly and faster. 
+
+    Parameters
+    ----------
+    df
+        Either a lazy or an eager Polars DataFrame
+    target
+        The target column
+    cols
+        If not provided, will use all inferred numeric columns
+    '''
+    if isinstance(cols, list):
+        nums = cols
+    else:
+        nums = get_numeric_cols(df, exclude=[target])
+
+    step_one_expr:list[pl.Expr] = [pl.count().alias("cnt")] 
+    step_two_expr:list[pl.Expr] = []
+    for n in nums:
+        n_sum:str = n + "_sum" # sum of class
+        n_var:str = n + "_var" # var within class
+        step_one_expr.append(
+            pl.col(n).sum().alias(n_sum)
+        )
+        step_one_expr.append(
+            pl.col(n).var(ddof=0).alias(n_var) 
+        )
+        step_two_expr.append(
+            (pl.col(n_sum)/pl.col("cnt") - pl.col(n_sum).sum()/pl.col("cnt").sum()).pow(2).dot(pl.col("cnt")) 
+            / pl.col(n_var).dot(pl.col("cnt"))
+        )
+
+    ref = (
+        df.lazy().groupby(target).agg(step_one_expr)
+        .select(
+            pl.col("cnt").sum().alias("n_samples")
+            , pl.col(target).len().alias("n_classes")
+            , *step_two_expr
+        ).collect()
+    )
+    n_samples = ref.drop_in_place("n_samples")[0]
+    n_classes = ref.drop_in_place("n_classes")[0]
+    df_btw_class = n_classes - 1 
+    df_in_class = n_samples - n_classes
+
+    if df_btw_class == 0:
+        raise ZeroDivisionError("Target has only one class.")
+    
+    f_values = ref.to_numpy().ravel() * (df_in_class / df_btw_class)
+    # We should scale this by (df_in_class / df_btw_class) because we did not do this earlier
+    # At this point, f_values should be a pretty small dataframe. 
+    # Cast to numpy, so that fdtrc can process it properly.
+
+    p_values = fdtrc(df_btw_class, df_in_class, f_values) # get p values 
+    return pl.from_records((nums, f_values, p_values), schema=["feature","f_value","p_value"])
+
+def f_score_selector(
+    df:PolarsFrame
+    , target:str
+    , top_k:int
+) -> PolarsFrame:
+    '''
+    Keeps only the top_k features in terms of f-score and the ones that cannot be processed by the algorithm.
+
+    Parameters
+    ----------
+    df
+        Either an eager or lazy Polars dataframe. If lazy, it will be collected
+    target
+        The target column
+    top_k
+        The top_k features will ke kept
+    '''
+    if isinstance(df, pl.LazyFrame):
+        input_data:pl.DataFrame = df.collect()
+    else:
+        input_data:pl.DataFrame = df
+
+    nums = get_numeric_cols(input_data, exclude=[target])
+    complement = [f for f in df.columns if f not in nums]
+    scores = _f_score(input_data, target, nums)
+    to_select = pl.DataFrame({"feature":nums, "fscore":scores})\
+        .top_k(by = "fscore", k = top_k)\
+        .get_column("feature").to_list()
+
+    print(f"Selected {len(to_select)} features. There are {len(complement)} columns the "
+          "algorithm cannot process. They are also returned.")
+
+    return select(df, to_select + complement, persist=True)
+
+def _mrmr_underlying_score(
+    df:pl.DataFrame
+    , target:str
+    , nums:list[str]
+    , strategy:MRMRStrategy
+    , params:dict[str,Any]
+) -> np.ndarray:
+    
+    logger.info(f"Running {strategy} to determine feature relevance...")
+    s = clean_strategy_str(strategy)
+    if s in ("fscore", "f", "f_score"):
+        scores = _f_score(df, target, nums)
+    elif s in ("rf", "random_forest"):
+        from sklearn.ensemble import RandomForestClassifier
+        print("Random forest is not deterministic by default. Results may vary.")
+        rf = RandomForestClassifier(**params)
+        rf.fit(df[nums].to_numpy(), df[target].to_numpy().ravel())
+        scores = rf.feature_importances_
+    elif s in ("xgb", "xgboost"):
+        from xgboost import XGBClassifier
+        print("XGB is not deterministic by default. Results may vary.")
+        xgb = XGBClassifier(**params)
+        xgb.fit(df[nums].to_numpy(), df[target].to_numpy().ravel())
+        scores = xgb.feature_importances_
+    elif s in ("mis", "mutual_info_score"):
+        scores = mutual_info(df, conti_cols=nums, target=target).get_column("estimated_mi").to_numpy().ravel()
+    elif s in ("lgbm", "lightgbm"):
+        from lightgbm import LGBMClassifier
+        print("LightGBM is not deterministic by default. Results may vary.")
+        lgbm = LGBMClassifier(**params)
+        lgbm.fit(df[nums].to_numpy(), df[target].to_numpy().ravel())
+        scores = lgbm.feature_importances_
+    else: # Pythonic nonsense
+        raise ValueError(f"The strategy {strategy} is not a valid MRMR Strategy.")
+    
+    return scores
+
+def mrmr(
+    df:pl.DataFrame
+    , target:str
+    , k:int
+    , cols:Optional[list[str]] = None
+    , strategy: MRMRStrategy = "fscore"
+    , params:Optional[dict[str,Any]] = None
+    , low_memory:bool=False
+) -> list[str]:
+    '''
+    Implements MRMR. Will add a few more strategies in the future. Likely only strategies for numerators
+    , aka relevance. Right now xgb, lgbm and rf strategies only work for classification problems.
+
+    Currently this only supports classification.
+
+    Parameters
+    ----------
+    df
+        An eager Polars Dataframe
+    target
+        Target column
+    k
+        Top k features to keep
+    cols
+        Optional. A list of numerical columns. If not provided, all numerical columns will be used.
+    strategy
+        MRMR strategy. By default, `fscore` will be used.
+    params
+        Optional. If a model strategy is selected (`rf`, `xgb`, `lgbm`), params is a dict of 
+        parameters for the model.
+    low_memory
+        Whether to do some computation all at once, which uses more memory at once, or do some 
+        computation when needed, which uses less memory at any given time.
+    '''
+    if isinstance(cols, list):
+        nums = cols
+    else:
+        nums = get_numeric_cols(df, exclude=[target])
+
+    s = clean_strategy_str(strategy)
+    scores = _mrmr_underlying_score(df
+        , target = target
+        , nums = nums
+        , strategy = s
+        , params = {} if params is None else params
+    )
+
+    if low_memory:
+        df_local = df.select(nums)
+    else: # this could potentially double memory usage. so I provided a low_memory flag.
+        df_local = df.select(nums).with_columns(
+            (pl.col(f) - pl.col(f).mean())/pl.col(f).std() for f in nums
+        ) # Note that if we get a const column, the entire column will be NaN
+
+    output_size = min(k, len(nums))
+    print(f"Found {len(nums)} total features to select from. Proceeding to select top {output_size} features.")
+    cumulating_abs_corr = np.zeros(len(nums)) # For each feature at index i, we keep a cumulating sum
+    top_idx = np.argmax(scores)
+    selected = [nums[top_idx]]
+    pbar = tqdm(total=output_size, desc = f"MRMR, {s}")
+    pbar.update(1)
+    for j in range(1, output_size):
+        argmax = -1
+        current_max = -1
+        last_selected_col = df_local.drop_in_place(selected[-1])
+        if low_memory: # normalize if in low memory mode.
+            last_selected_col = (last_selected_col - last_selected_col.mean())/last_selected_col.std()
+        for i,f in enumerate(nums):
+            if f not in selected:
+                # Left = cumulating sum of abs corr
+                # Right = abs correlation btw last_selected and f
+                candidate_col = df_local.get_column(f)
+                if low_memory: # normalize if in low memory mode.
+                    candidate_col = (candidate_col - candidate_col.mean())/candidate_col.std()
+
+                a = (last_selected_col*candidate_col).mean()
+                # In the rare case this calculation yields a NaN, we punish by adding 1.
+                # Otherwise, proceed as usual. +1 is a punishment because
+                # |corr| can be at most 1. So we are enlarging the denominator, thus reducing the score.
+                cumulating_abs_corr[i] += 1 if np.isnan(a) else np.abs(a)
+                denominator = cumulating_abs_corr[i]/j 
+                new_score = scores[i] / denominator
+                if new_score > current_max:
+                    current_max = new_score
+                    argmax = i
+        selected.append(nums[argmax])
+        pbar.update(1)
+
+    pbar.close()
+    print("Output is sorted in order of selection (max relevance min redundancy).")
+    return selected
+
+def mrmr_selector(
+    df:PolarsFrame
+    , target:str
+    , top_k:int
+    , strategy:MRMRStrategy = "fscore"
+    , params:Optional[dict[str,Any]] = None
+    , low_memory:bool=False
+) -> PolarsFrame:
+    '''
+    Keeps only the top_k (first k) features selected by MRMR and the ones that cannot be processed by the algorithm.
+
+    Parameters
+    ----------
+    df
+        Either an eager or lazy Polars dataframe. If lazy, it will be collected
+    target
+        The target column
+    top_k
+        The top_k features will ke kept
+    strategy
+        One of 'f', 'xgb', 'rf', 'mis', 'lgbm'. It will use the corresponding method to compute feature relevance
+    params
+        If any modeled relevance is used, e.g. 'rf', 'lgbm' or 'xgb', then this will be the param dict for the model
+    low_memory
+        If true, use less memory. But the computation will take longer
+    '''
+    if isinstance(df, pl.LazyFrame):
+        input_data:pl.DataFrame = df.collect()
+    else:
+        input_data:pl.DataFrame = df
+
+    nums = get_numeric_cols(input_data, exclude=[target])
+    s = clean_strategy_str(strategy)
+    to_select = mrmr(input_data, target, top_k, nums, s, params, low_memory)
+    logger.info(f"Selected {len(to_select)} features. There are {len(df.columns) - len(to_select)} columns the "
+          "algorithm cannot process. They are also returned.")
+    to_select.extend(f for f in df.columns if f not in nums)
+    return select(df, to_select, persist=True)
+
+def knock_out_mrmr(
+    df:pl.DataFrame
+    , target:str
+    , k:int 
+    , cols:Optional[list[str]] = None
+    , corr_threshold:float = 0.7
+    , strategy:MRMRStrategy = "fscore"
+    , params:Optional[dict[str,Any]] = None
+) -> list[str]:
+    '''
+    Essentially the same as vanilla MRMR. Instead of using sum(abs(corr)) to "weigh down" correlated 
+    variables, here we use a simpler knock out rule based on absolute correlation. We go down the list
+    according to importance, take top one, knock out all other features that are highly correlated with
+    it, take the next top feature that has not been knocked out, continue, until we pick enough features
+    or there is no feature left.
+
+    Inspired by the package Featurewiz and its creator.
+
+    Parameters
+    ----------
+    df
+        An eager Polars Dataframe
+    target
+        The target column
+    k
+        The top k features to return
+    cols
+        Numerical columns to select from. If not provided, all numeric columns will be used
+    corr_threshold
+        The threshold above which correlation is considered too high. This means if A has high correlation to B, then
+        B will not be selected if A is
+    strategy
+        One of 'f', 'xgb', 'rf', 'mis', 'lgbm'. It will use the corresponding method to compute feature relevance
+    params
+        If any modeled relevance is used, e.g. 'rf', 'lgbm' or 'xgb', then this will be the param dict for the model
+    '''
+    if isinstance(cols, list):
+        nums = cols
+    else:
+        nums = get_numeric_cols(df, exclude=[target])
+
+    s = clean_strategy_str(strategy)
+    scores = _mrmr_underlying_score(df
+        , target = target
+        , nums = nums
+        , strategy = s
+        , params = {} if params is None else params
+    )
+
+    # Set up
+    low_corr = np.abs(df[nums].corr().to_numpy()) < corr_threshold
+    surviving_indices = np.full(shape=len(nums), fill_value=True) # an array of booleans
+    scores = sorted(enumerate(scores), key=lambda x:x[1], reverse=True)
+    selected = []
+    count = 0
+    output_size = min(k, len(nums))
+    pbar = tqdm(total=output_size)
+    # Run the knock outs
+    for i, _ in scores:
+        if surviving_indices[i]:
+            selected.append(nums[i])
+            surviving_indices = surviving_indices & low_corr[:,i]
+            count += 1
+            pbar.update(1)
+        if count >= output_size:
+            break
+
+    pbar.close()
+    if count < k:
+        print(f"Found only {count}/{k} number of values because most of them are highly correlated and the knock out "
+              "rule eliminates most of them.")
+
+    print("Output is sorted in order of selection (max relevance min redundancy).")
+    return selected
+
+def knock_out_mrmr_selector(
+    df:PolarsFrame
+    , target:str
+    , top_k:int 
+    , corr_threshold:float = 0.7
+    , strategy:MRMRStrategy = "fscore"
+    , params:Optional[dict[str,Any]] = None
+) -> PolarsFrame:
+    '''
+    Keeps only the top_k (first k) features selected by MRMR and the ones that cannot be processed by the algorithm.
+
+    Parameters
+    ----------
+    df
+        Either an eager or lazy Polars dataframe. If lazy, it will be collected
+    target
+        The target column
+    top_k
+        The top_k features will ke kept
+    corr_threshold
+        The threshold above which correlation is considered too high. This means if A has high correlation to B, then
+        B will not be selected if A is
+    strategy
+        One of 'f', 'xgb', 'rf', 'mis', 'lgbm'. It will use the corresponding method to compute feature relevance
+    params
+        If any modeled relevance is used, e.g. 'rf', 'lgbm' or 'xgb', then this will be the param dict for the model
+    '''
+    if isinstance(df, pl.LazyFrame):
+        input_data:pl.DataFrame = df.collect()
+    else:
+        input_data:pl.DataFrame = df
+
+    nums = get_numeric_cols(df, exclude=[target])
+    complement = [f for f in df.columns if f not in nums]
+    s = clean_strategy_str(strategy)
+    to_select = knock_out_mrmr(input_data, target, top_k, nums, s, corr_threshold, params)
+    print(f"Selected {len(to_select)} features. There are {len(complement)} columns the "
+          "algorithm cannot process. They are also returned.")
+    
+    return select(df, to_select + complement, persist=True)
+
+# Selectors for the methods below are not yet implemented
+
+def woe_iv(
+    df:PolarsFrame
+    , target:str
+    , cols:Optional[list[str]]=None
+    , min_count:float = 1.
+    , check_binary:bool = True
+) -> pl.DataFrame:
+    '''
+    Computes information values for categorical variables. Notice that by using binning methods provided in 
+    dsds.transform, you can turn numerical values into categorical bins.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars Dataframe
+    target
+        The target column
+    cols
+        If not provided, will use all string columns
+    min_count
+        A regularization term that prevents ln(0). This is the same as category_encoders package's 
+        regularization parameter.
+    check_binary
+        Whether to check if target is binary or not
+    '''
+    if isinstance(cols, list):
+        _ = type_checker(df, cols, "string", "woe_iv")
+        input_cols = cols
+    else:
+        input_cols = get_string_cols(df)
+
+    if check_binary:
+        if not check_binary_target(df, target):
+            raise ValueError("Target is not binary or not properly encoded or contains nulls.")
+
+    results = (
+        df.lazy().groupby(s).agg(
+            ev = pl.col(target).sum()
+            , nonev = (pl.lit(1) - pl.col(target)).sum()
+        ).with_columns(
+            ev_rate = (pl.col("ev") + min_count)/(pl.col("ev").sum() + 2.0*min_count)
+            , nonev_rate = (pl.col("nonev") + min_count)/(pl.col("nonev").sum() + 2.0*min_count)
+        ).with_columns(
+            woe = (pl.col("ev_rate")/pl.col("nonev_rate")).log()
+        ).select(
+            pl.lit(s).alias("feature")
+            , pl.col(s).alias("value")
+            , pl.col("woe")
+            , information_value = ((pl.col("ev_rate")-pl.col("nonev_rate")) * pl.col("woe")).sum()
+        )
+        for s in input_cols
+    )
+    return pl.concat(pl.collect_all(results))
+
+def _binary_model_init(
+    model_str:BinaryModels
+    , params: dict[str, Any]
+) -> ClassifModel:
+    '''
+    Returns a classification model. If n_job parameter is not specified, it will default to -1.
+
+    Parameters
+    ----------
+    model_str
+        One of 'lr', 'lgbm', 'xgb', 'rf'
+    params
+        The parameters for the model specified
+    '''
+    if "n_jobs" not in params:
+        params["n_jobs"] = -1
+
+    if model_str in ("logistic", "lr"):
+        from sklearn.linear_model import LogisticRegression
+        model = LogisticRegression(**params)
+    elif model_str in ("rf", "random_forest"):
+        from sklearn.ensemble import RandomForestClassifier
+        model = RandomForestClassifier(**params)
+    elif model_str in ("xgb", "xgboost"):
+        from xgboost import XGBClassifier
+        model = XGBClassifier(**params)
+    elif model_str in ("lgbm", "lightgbm"):
+        from lightgbm import LGBMClassifier
+        model = LGBMClassifier(**params)
+    else:
+        raise ValueError(f"The model {model_str} is not available.")
+    
+    return model
+
+def _fc_fi(
+    model_str:str
+    , params:dict[str, Any]
+    , target:str
+    , features: Union[Tuple,list[str]]
+    , train: pl.DataFrame
+    , test: pl.DataFrame
+)-> Tuple[Tuple[Tuple, float, float], np.ndarray]:
+    '''
+    Creates a classification model, evaluations model with log loss and roc_auc for each feature combination
+    (fc) and feature importance (fi). It will return a tuple of the following structure: 
+    ( (feature combination, log loss, roc_auc), feature_importance array) 
+
+    Parameters
+    ----------
+    model_str
+        One of 'lr', 'lgbm', 'xgb', 'rf'
+    params
+        The parameters for the model specified
+    target
+        The target column
+    features
+        Either a tuple or a list which represents the current feature combination
+    train
+        The training dataset. Must be eager
+    test
+        The testing dataset on which log loss and roc_auc will be evaluation. Must be eager
+    '''
+    estimator = _binary_model_init(model_str, params)
+    _ = estimator.fit(train.select(features), train[target])
+    y_pred = estimator.predict_proba(test.select(features))[:,1]
+    y_test = test[target].to_numpy()
+    fc_rec = (
+        features,
+        logloss(y_test, y_pred, check_binary=False),
+        roc_auc(y_test, y_pred, check_binary=False)
+    )
+    if model_str in ("lr", "logistic"):
+        fi_rec = np.abs(estimator.coef_).ravel()
+    else:
+        fi_rec = estimator.feature_importances_
+    # fc_rec feature comb record, fi_rec feature importance record
+    return fc_rec, fi_rec
+
+# ebfs: stands for Exhaustive Binary Feature Selection
+def ebfs(
+    df:pl.DataFrame
+    , target:str
+    , model_str:BinaryModels
+    , params:dict[str, Any]
+    , n_comb: int = 3
+    , train_frac:float = 0.75
+) -> Tuple[pl.DataFrame, pl.DataFrame]:
+    '''
+    Suppose we have n features and n_comb = 2. This method will select all (n choose 2) 
+    combinations of features, split dataset into a train and a test for each combination, 
+    train a model on train, and compute feature importance and roc_auc and logloss, and 
+    then finally put everything into two separate dataframes, the first of which will contain 
+    the feature combinations and model performances, and the second will contain the min, avg, 
+    max and var of feature importance of each feature in all its occurences in the training rounds.
+
+    Notice since we split data into train and test every time for a different feature combination, the 
+    average feature importance we derive naturally are `cross-validated` to a certain degree.
+
+    This method will be extremely slow if (n choose n_comb) is a big number. All numerical columns 
+    will be taken as potential features. Please encode the string columns if you want to use them
+    as features here.
+
+    If n_jobs is not provided in params, it will be defaulted to -1.
+
+    This will return a feature combination (fc) summary and a feature importance (fi) summary. 
+
+    Parameters
+    ----------
+    df
+        An eager Polars DataFrame
+    target
+        The target column
+    model_str
+        one of 'lr', 'lgbm', 'xgb', 'rf'
+    params
+        Parameters for the model
+    n_comb
+        We will run this for all n choose n_comb combinations of features
+    '''
+    features = get_numeric_cols(df, exclude=[target])
+    fi = {f:[] for f in features}
+    records = []
+    pbar = tqdm(total=math.comb(len(features), n_comb), desc="Tested Combinations")
+    df_keep = df.select(features + [target])
+    for comb in combinations(features, r=n_comb):
+        train, test = train_test_split(df_keep, train_frac)
+        fc_rec, fi_rec = _fc_fi(model_str, params, target, comb, train, test) 
+        records.append(fc_rec)
+        for f, i in zip(fc_rec[0], fi_rec):
+            fi[f].append(i)
+        pbar.update(1)
+
+    fc_summary = pl.from_records(records, schema=["combination", "logloss", "roc_auc"])
+    stats = [
+        (f, len(fi[f]), np.min(fi[f]), np.mean(fi[f]), np.max(fi[f]), np.std(fi[f])) for f in fi
+    ]
+    fi_summary = pl.from_records(stats, schema=["feature", "occurrences", "fi_min", "fi_mean", "fi_max", "fi_std"])
+    pbar.close()
+    return fc_summary, fi_summary
+
+def ebfs_fc_filter(
+    fc: pl.DataFrame
+    , logloss_threshold:float
+    , roc_auc_threshold:float
+) -> list[str]:
+    '''
+    A filter method based on the feature combination result of ebfs.
+
+    Parameters
+    ----------
+    fc
+        The feature combination result from ebfs
+    logloss_threshold
+        The maximum logloss for the combination to be kept
+    roc_auc_threshold
+        The minimum roc_auc for the combination to be kept
+    '''
+    return fc.filter(
+        (pl.col("logloss") <= logloss_threshold)
+        & (pl.col("roc_auc") >= roc_auc_threshold)
+    ).get_column("combination").explode().unique().to_list()
+
+def _permute_importance(
+    model:ClassifModel
+    , X:pl.DataFrame
+    , y: np.ndarray
+    , index:int
+    , k: int
+) -> Tuple[float, int]:
+    '''
+    Computes permutation importance for a single feature.
+
+    Parameters
+    ----------
+    model
+        A trained classification model
+    X
+        An eager dataframe on which we shuffle the column at the given index and train the model
+    y
+        The target column turned into np.ndarray
+    index
+        The index of the column in X to shuffle
+    k
+        The number of times to repeat the shuffling
+    '''
+    test_score = 0.
+    c = X.columns[index] # column to shuffle
+    for _ in range(k):
+        shuffled_df = X.with_columns(
+            pl.col(c).shuffle(seed=42)
+        )
+        test_score += roc_auc(y, model.predict_proba(shuffled_df)[:, -1])
+
+    return test_score, index
+
+def permutation_importance(
+    df:pl.DataFrame
+    , target:str
+    , model_str:BinaryModels
+    , params:dict[str, Any]
+    , k:int = 5
+) -> pl.DataFrame:
+    '''
+    Computes permutation importance for every non-target column in df. Please make sure all columns are properly encoded
+    or transformed before calling this.
+    
+    Only works for binary classification and score = roc_auc for now.
+
+    Parameters
+    ----------
+    df
+        An eager Polars DataFrame
+    target
+        The target column
+    model_str
+        One of 'lr', 'lgbm', 'xgb', 'rf'
+    params
+        Parameters for the model
+    k
+        Permute the same feature k times
+    '''
+    features = df.columns
+    features.remove(target)
+    _ = type_checker(df, features, "numeric", "permutation_importance")
+    estimator = _binary_model_init(model_str, params)
+    estimator.fit(df[features], df[target])
+    X = df[features]
+    y = df[target].to_numpy()
+    score = roc_auc(y, estimator.predict_proba(X)[:, -1])
+    pbar = tqdm(total=len(features), desc="Analyzing Features")
+    imp = np.zeros(shape=len(features))
+    with ThreadPoolExecutor(max_workers=CPU_M1) as ex:
+        futures = (
+            ex.submit(
+                _permute_importance,
+                estimator,
+                X,
+                y,
+                j,
+                k
+            )
+            for j in range(len(features))
+        )
+        for f in as_completed(futures):
+            test_score, i = f.result()
+            imp[i] = score - (1/k)*test_score
+            pbar.update(1)
+
     return pl.from_records((features, imp), schema=["feature", "permutation_importance"])
```

### Comparing `dsds-0.0.24/src/dsds/prescreen.py` & `dsds-0.0.25/python/dsds/prescreen.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,976 +1,1116 @@
-from .type_alias import (
-    PolarsFrame
-    , Alternatives
-    , CommonContiDist
-    , SimpleDtypes
-    , CPU_COUNT
-    , POLARS_DATETIME_TYPES
-    , POLARS_NUMERICAL_TYPES
-)
-from .sample import (
-    lazy_sample
-)
-from .blueprint import(
-    Blueprint  # noqa: F401
-)
-from datetime import datetime 
-from typing import Any, Optional, Tuple, Union
-from itertools import combinations
-from scipy.stats import (
-    ks_2samp
-    , kstest
-)
-from concurrent.futures import as_completed, ThreadPoolExecutor
-from tqdm import tqdm
-from math import comb
-import re
-import polars.selectors as cs
-import polars as pl
-import logging  
-
-logger = logging.getLogger(__name__)
-
-#----------------------------------------------------------------------------------------------#
-# Generic columns checks | Only works with Polars because Pandas's data types suck!            #
-#----------------------------------------------------------------------------------------------#
-
-def get_numeric_cols(df:PolarsFrame, exclude:Optional[list[str]]=None) -> list[str]:
-    '''Returns numerical columns except those in exclude.'''
-    if exclude is None:
-        selector = cs.numeric()
-    else:
-        selector = cs.numeric() & ~cs.by_name(exclude)
-    return df.select(selector).columns
-
-def get_string_cols(df:PolarsFrame, exclude:Optional[list[str]]=None) -> list[str]:
-    '''Returns string columns except those in exclude.'''
-    if exclude is None:
-        selector = cs.string()
-    else:
-        selector = cs.string() & ~cs.by_name(exclude)
-    return df.select(selector).columns
-
-def get_datetime_cols(df:PolarsFrame) -> list[str]:
-    '''Returns only datetime columns. This will not try to infer date from strings.'''
-    return df.select(cs.datetime()).columns
-
-def get_bool_cols(df:PolarsFrame) -> list[str]:
-    '''Returns boolean columns.'''
-    return df.select(cs.by_dtype(pl.Boolean)).columns
-
-def get_cols_regex(df:PolarsFrame, pattern:str, lowercase:bool=False) -> list[str]:
-    '''
-    Returns columns that have names matching the regex pattern.
-    
-    
-    '''
-    if lowercase:
-        return (
-            df.rename({c:c.lower() for c in df.columns})
-            .select(cs.matches(pattern=pattern)).columns
-        )
-    else:
-        return df.select(cs.matches(pattern=pattern)).columns
-
-
-def rename(df:PolarsFrame, rename_dict:dict[str, str], persist:bool=False) -> PolarsFrame:
-    '''
-    A wrapper function for df.rename() so that it works with pipeline.
-
-    Set persist = True if this needs to be remembered by the blueprint.
-    '''
-    output = df.rename(rename_dict)
-    if isinstance(df, pl.LazyFrame) and persist:
-        return output.blueprint.add_func(df, rename, kwargs = {"rename_dict": rename_dict})
-    return output
-
-def lowercase(df:PolarsFrame, persist:bool=False) -> PolarsFrame:
-    '''
-    Lowercases all column names.
-
-    Set persist = True if this needs to be remembered by the blueprint.
-    '''
-    return rename(df, {c: c.lower() for c in df.columns}, persist)
-
-def snake_case(df:PolarsFrame, persist:bool=False) -> PolarsFrame:
-    '''
-    Turn all camel case column names into snake case.
-
-    Set persist = True if this needs to be remembered by the blueprint.
-    '''
-    pat = re.compile(r"(?<!^)(?=[A-Z])")
-    return rename(df, {c: pat.sub('_', c).lower() for c in df.columns}, persist)
-
-def select(
-    df:PolarsFrame
-    , selector: Union[list[str], cs._selector_proxy_]
-    , persist:bool=False
-) -> PolarsFrame:
-    '''
-    A select wrapper that makes it pipeline compatible.
-
-    Set persist = True if this needs to be remembered by the blueprint.
-    '''
-    if isinstance(df, pl.LazyFrame) and persist:
-        return df.blueprint.select(selector)
-    return df.select(selector)
-
-def drop_nulls(
-    df:PolarsFrame
-    , subset:Optional[list[str]] = None
-    , persist:bool=False
-) -> PolarsFrame:
-    '''
-    A wrapper function for Polars' drop_nulls so that it can be used in pipeline.
-
-    Set persist = True if this needs to be remembered by the blueprint.
-    '''
-    if subset is None:
-        by = df.columns
-    else:
-        by = subset
-
-    output = df.drop_nulls(subset=by)
-    if isinstance(df, pl.LazyFrame) and persist:
-        return output.blueprint.add_func(df, drop_nulls, {"subset":subset})
-    return output
-
-def filter(
-    df:PolarsFrame
-    , condition: pl.Expr
-    , persist: bool = False
-) -> PolarsFrame:
-    ''' 
-    A wrapper function for Polars' filter so that it can be used in pipeline.
-
-    Set persist = True if this needs to be remembered by the blueprint.
-    '''
-    if isinstance(df, pl.LazyFrame) and persist:
-        return df.blueprint.filter(condition)
-    return df.filter(condition)
-
-def order_by(
-    df: PolarsFrame
-    , by: Union[str, list[str]]
-    , descending:bool = False
-    , nulls_last:bool = False
-    , persist: bool = False
-) -> PolarsFrame:
-    ''' 
-    A wrapper function for Polars' sort so that it can be used in pipeline.
-
-    Set persist = True if this needs to be remembered by the blueprint.
-    '''
-    output = df.sort(by=by, descending=descending, nulls_last=nulls_last)
-    if isinstance(df, pl.LazyFrame) and persist:
-        return output.blueprint.add_func(df, order_by, {"by":by,"descending":descending, "nulls_last":nulls_last})
-    return output
-
-def check_binary_target(df:PolarsFrame, target:str) -> bool:
-    '''Checks if target is binary or not. Only binary targets with 0s and 1s will pass.'''
-    target_uniques = df.lazy().select(pl.col(target).unique()).collect().get_column(target)
-    if len(target_uniques) != 2:
-        logger.error("Target is not binary.")
-        return False
-    elif not (0 in target_uniques and 1 in target_uniques):
-        logger.error("The binary target is not encoded as 0s and 1s.")
-        return False
-    return True
-    
-def check_target_cardinality(df:PolarsFrame, target:str, raise_null:bool=True) -> pl.DataFrame:
-    '''
-    Returns a dataframe showing the cardinality of different target values. If raise_null = True, raise 
-    an exception if target column has any null values.
-    '''
-    output = df.lazy().groupby(target).count().sort(target).with_columns(
-        pct = pl.col("count")/pl.col("count").sum()
-    ).collect()
-    if raise_null and output.get_column(target).null_count() > 0:
-        raise ValueError("Target contains null.")
-    return output
-
-def check_columns_types(df:PolarsFrame, cols:Optional[list[str]]=None) -> str:
-    '''
-    Returns the unique types of given columns in a single string. If multiple types are present
-    they are joined by a |. If cols is not given, automatically uses all columns.
-    '''
-    if cols is None:
-        check_cols:list[str] = df.columns
-    else:
-        check_cols:list[str] = cols 
-
-    types = sorted(set(dtype_mapping(t) for t in df.select(check_cols).dtypes))
-    return "|".join(types) if len(types) > 0 else "other/unknown"
-
-def type_checker(df:PolarsFrame, cols:list[str], expected_type:SimpleDtypes, caller_name:str) -> bool:
-    types = check_columns_types(df, cols)
-    if types != expected_type:
-        raise ValueError(f"The call `{caller_name}` can only be used on {expected_type} columns, not {types} types.")
-    return True
-
-# dtype can be a "pl.datatype" or just some random data for which we want to infer a generic type.
-def dtype_mapping(d: Any) -> SimpleDtypes:
-    if isinstance(d, str) or d == pl.Utf8:
-        return "string"
-    elif isinstance(d, bool) or d == pl.Boolean:
-        return "bool"
-    elif isinstance(d, (int,float)) or d in POLARS_NUMERICAL_TYPES:
-        return "numeric"
-    elif isinstance(d, pl.List):
-        return "list" # Too many possibilities. Keep it to list for now.
-    elif isinstance(d, datetime) or d in POLARS_DATETIME_TYPES:
-        return "datetime"
-    else:
-        return "other/unknown"
-
-#----------------------------------------------------------------------------------------------#
-# Prescreen Inferral, Removal Methods                                                          #
-#----------------------------------------------------------------------------------------------#
-
-# Add a slim option that returns fewer stats? This is generic describe.
-def describe(
-    df:PolarsFrame
-    , sample_frac:float = 1.0
-    , percentiles: list[float] = [0.25, 0.75]
-    , exclude: Optional[list[str]] = None
-) -> pl.DataFrame:
-    '''
-    A more detailed profile the data than Polars' default. This is an expensive function. Please sample 
-    and exclude some columns if runtime is important.
-
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars dataframe
-    sample_frac
-        If > 0 and < 1, will run profiling on a sample. This is recommended for bigger dataframes
-    percentiles
-        Percentile cuts that will be returned
-    exclude
-        List of columns to exclude
-    '''
-    selector = cs.all()
-    if exclude is not None:
-        selector = selector & ~cs.by_name(exclude)
-        
-    if sample_frac > 0 and sample_frac < 1:
-        if isinstance(df, pl.LazyFrame):
-            df_local = lazy_sample(df.select(selector), sample_frac=sample_frac).collect()
-        else:
-            df_local = df.select(selector).sample(fraction=sample_frac)
-    else:
-        df_local = df.lazy().select(selector).collect()
-
-    temp = df_local.describe(percentiles)
-    desc = temp.drop_in_place("describe")
-    # Get unique
-    unique_counts = get_unique_count(df_local).with_columns(
-        unique_pct = pl.col("n_unique") / len(df_local)
-    )
-    # Skew and Kurtosis
-    skew_and_kt_data = df_local.lazy().select(
-        pl.all().skew().prefix("skew:")
-        , pl.all().skew().prefix("kurtosis:")
-    ).collect().row(0)
-
-    n_cols = len(df_local.columns)
-    skew_and_kt = pl.from_records((df_local.columns, skew_and_kt_data[:n_cols], skew_and_kt_data[n_cols:])
-                                  , schema=["column", "skew", "kurtosis"])
-
-    # Get a basic string description of the data type.
-    dtypes_dict = dict(zip(df_local.columns, map(dtype_mapping, df_local.dtypes)))
-    # Get all percentiles
-    pat = re.compile("^\d+%$")
-    pctls = [d for d in desc if pat.search(d)]
-    # Numerical stuff
-    nums = ["null_count", "mean", "std", "median"] + pctls
-    # Combine all
-    final = temp.transpose(include_header=True, column_names=desc).with_columns(
-        pl.col(c).cast(pl.Float64) for c in nums
-    ).with_columns(
-        null_pct = pl.col("null_count")/pl.col("count")
-        , non_null_count = pl.col("count") - pl.col("null_count")
-        , CoV = pl.col("std") / pl.col("mean")
-        , dtype = pl.col("column").map_dict(dtypes_dict)
-    ).join(unique_counts, on="column").join(skew_and_kt, on="column")
-    # select only the stuff we need
-    return final.select('column', 'dtype', "non_null_count", 'null_count','null_pct','n_unique'
-                        , 'unique_pct','mean','std', 'CoV','min','max','median',"skew", "kurtosis"
-                        , *pctls)
-
-# Numeric only describe. Be more detailed.
-
-# String only describe. Be more detailed about interesting string stats.
-
-def describe_str(
-    df:PolarsFrame
-    , words_to_count:Optional[list[str]]=None
-    , sample_frac:float = 0.75
-) -> pl.DataFrame:
-    '''
-    Computes some statistics about the string columns. Optionally you may pass a list
-    of strings to compute the total occurrences of each of the words in the string columns. If input is a LazyFrame, 
-    a sample of sample_pct will be used, and sample_pct will only be used in the lazy case. 
-    '''
-    strs = get_string_cols(df)
-    df_str = df.select(strs)
-    if isinstance(df, pl.LazyFrame):
-        df_str = lazy_sample(df_str, sample_frac=sample_frac).collect()
-
-    nstrs = len(strs)
-    stats = df.select(strs).select(
-        pl.all().null_count().prefix("nc:"),
-        pl.all().max().prefix("max:"),
-        pl.all().min().prefix("min:"),
-        pl.all().mode().first().prefix("mode:"),
-        pl.all().str.lengths().min().prefix("min_byte_len:"),
-        pl.all().str.lengths().max().prefix("max_byte_len:"),
-        pl.all().str.lengths().mean().prefix("avg_byte_len:"),
-        pl.all().str.lengths().median().prefix("median_byte_len:"),
-        pl.all().str.count_match(r"\s").mean().prefix("avg_space_cnt:"),
-        pl.all().str.count_match(r"[0-9]").mean().prefix("avg_digit_cnt:"),
-        pl.all().str.count_match(r"[A-Z]").mean().prefix("avg_cap_cnt:"),
-        pl.all().str.count_match(r"[a-z]").mean().prefix("avg_lower_cnt:")
-    ).row(0)
-    output = {
-        "features":strs,
-        "null_count": stats[:nstrs],
-        "min": stats[nstrs: 2*nstrs],
-        "max": stats[2*nstrs: 3*nstrs],
-        "mode": stats[3*nstrs: 4*nstrs],
-        "min_byte_len": stats[4*nstrs: 5*nstrs],
-        "max_byte_len": stats[5*nstrs: 6*nstrs],
-        "avg_byte_len": stats[6*nstrs: 7*nstrs],
-        "median_byte_len": stats[7*nstrs: 8*nstrs],
-        "avg_space_cnt": stats[8*nstrs: 9*nstrs],
-        "avg_digit_cnt": stats[9*nstrs: 10*nstrs],
-        "avg_cap_cnt": stats[10*nstrs: 11*nstrs],
-        "avg_lower_cnt": stats[11*nstrs: ],
-    }
-
-    if isinstance(words_to_count, list):
-        for w in words_to_count:
-            t = df_str.select(pl.all().str.count_match(w).sum().prefix("wc:")).row(0)
-            output["total_"+ w + "_count"] = t
-
-    return pl.from_dict(output)
-
-# -----------------------------------------------------------------------------------------------
-def drop(df:PolarsFrame, to_drop:list[str]) -> PolarsFrame:
-    '''
-    A pipeline compatible way to drop the given columns, which will be remembered by the blueprint
-    by default.
-    '''
-    if isinstance(df, pl.LazyFrame):
-        return df.blueprint.drop(to_drop)
-    return df.drop(to_drop)
-
-def non_numeric_removal(df:PolarsFrame, include_bools:bool=False) -> PolarsFrame:
-    '''
-    Removes all non-numeric columns. If include_bools = True, then keep boolean columns.
-    '''
-    if include_bools:
-        selector = ~(cs.numeric()|cs.by_dtype(pl.Boolean))
-    else:
-        selector = ~cs.numeric()
-
-    non_nums = df.select(selector).columns
-    logger.info(f"The following columns are dropped because they are not numeric: {non_nums}.\n"
-                f"Removed a total of {len(non_nums)} columns.")
-    
-    return drop(df, non_nums)
-
-# Check if columns are duplicates. Might take time.
-def duplicate_inferral():
-    # Get profiles first.
-    # Divide into categories: bools, strings, numerics, datetimes.
-    # Then cut down list to columns that have the same min, max, n_unique and null_count.
-    # Then check equality..
-    pass
-
-def pattern_inferral(
-    df: PolarsFrame
-    , pattern:str
-    , sample_frac:float = 0.75
-    , sample_count:int = 100_000
-    , sample_rounds:int = 3
-    , threshold:float = 0.9
-    , count_null:bool = True
-) -> list[str]:
-    '''
-    Find all string columns whose elements reasonably match the given pattern. The match logic can 
-    be tuned using the all the parameters.
-
-    Parameters
-    ----------
-    sample_frac
-        The pct of the total dataframe to use as pool
-    sample_count
-        From the pool, how many rows to sample for each round 
-    sample_rounds
-        How many rounds of sampling we are doing
-    threshold
-        For each round, what is the match% that is needed to be a counted as a success. For instance, 
-        in round 1, for column x, we have 92% match rate, and threshold = 0.9. We count column x as a match for 
-        this round. In the end, the column must match for every round to be considered a real match.
-    count_null
-        For individual matches, do we want to count null as a match or not? If the column has high null pct,
-        the non-null values might mostly match the pattern. In this case, using count_null = True will match the column, 
-        while count_null = False will most likely exclude the column.
-
-    Returns:
-        a list of columns that pass the matching test
-    
-    '''
-    strs = get_string_cols(df)
-    df_local = lazy_sample(df.lazy(), sample_frac=sample_frac).collect()    
-    matches:set[str] = set(strs)
-    sample_size = min(sample_count, len(df_local))
-    for _ in range(sample_rounds):
-        df_sample = df_local.sample(n = sample_size)
-        fail = df_sample.select(
-            (
-                pl.when(pl.col(s).is_null()).then(count_null).otherwise(
-                    pl.col(s).str.contains(pattern)
-                ).sum()/sample_size
-            ).alias(s) 
-            for s in strs
-        ).transpose(include_header=True, column_names=["pattern_match_pct"])\
-        .filter(pl.col("pattern_match_pct") < threshold).get_column("column")
-        # If the match failes in this round, remove the column.
-        matches.difference_update(fail)
-
-    return list(matches)
-
-def pattern_removal(
-    df: PolarsFrame
-    , pattern:str
-    , sample_pct:float = 0.75
-    , sample_count:int = 100_000
-    , sample_rounds:int = 3
-    , threshold:float = 0.9
-    , count_null:bool = True
-) -> PolarsFrame:
-    
-    remove_cols = pattern_inferral(
-        df
-        , pattern
-        , sample_pct
-        , sample_count
-        , sample_rounds
-        , threshold 
-        , count_null
-    )
-    logger.info(f"The following columns are dropped because they match the element pattern: {pattern}.\n"
-                f"{remove_cols}\n"
-                f"Removed a total of {len(remove_cols)} columns.")
-    
-    return drop(df, remove_cols)
-
-def email_inferral(
-    df: PolarsFrame
-    , sample_pct:float = 0.75
-    , sample_count:int = 100_000
-    , sample_rounds:int = 3
-    , threshold:float = 0.9
-    , count_null:bool = True
-) -> list[str]:
-    # Why does this regex not work?
-    # r'([A-Za-z0-9]+[.-_])*[A-Za-z0-9]+@[A-Za-z0-9-]+(\.[A-Z|a-z]{2,})+'
-    return pattern_inferral(
-        df
-        , r'\S+@\S+\.\S+'
-        , sample_pct
-        , sample_count
-        , sample_rounds
-        , threshold 
-        , count_null
-    )
-
-def email_removal(
-    df: PolarsFrame
-    , sample_pct:float = 0.75
-    , sample_count:int = 100_000
-    , sample_rounds:int = 3
-    , threshold:float = 0.9
-    , count_null:bool = True
-) -> PolarsFrame:
-    
-    emails = email_inferral(df, sample_pct, sample_count, sample_rounds, threshold, count_null)
-    logger.info(f"The following columns are dropped because they are emails. {emails}.\n"
-            f"Removed a total of {len(emails)} columns.")
-    
-    return drop(df, emails)
-
-# Check for columns that are US zip codes.
-# Might add options for other countries later.
-def zipcode_inferral():
-    # Match string using pattern inferral
-    # Take a look at integers too, are they always 5 digits? 
-    pass
-
-def date_inferral(df:PolarsFrame) -> list[str]:
-    '''Infers date columns in dataframe. This inferral is not perfect.'''
-    logger.info("Date Inferral is error prone due to the huge variety of date formats. Please use with caution.")
-    
-    dates = [c for c,t in zip(df.columns, df.dtypes) if t in POLARS_DATETIME_TYPES]
-    strings = get_string_cols(df)
-    # MIGHT REWRITE THIS LOGIC
-    # Might be memory intensive on big dataframes.
-    sample_size = min(len(df), 100_000)
-    sample_df = df.lazy().select(strings)\
-        .drop_nulls().collect()\
-        .sample(n = sample_size).select(
-            # Cleaning the string first. Only try to catch string dates which are in the first split by space
-           pl.col(s).str.strip().str.replace_all("(/|\.)", "-").str.split(by=" ").list.first() 
-           for s in strings
-        )
-    for s in strings:
-        try:
-            c = sample_df[s].str.to_date(strict=False)
-            if 1 - c.null_count()/sample_size >= 0.15: # if at least 15% valid (able to be converted)
-                # This last check is to account for single digit months.
-                # 3/3/1995 will not be parsed to a string because standard formats require 03/03/1995
-                # At least 15% of dates naturally have both month and day as 2 digits numbers
-                dates.append(s)
-        except: # noqa: E722
-            # Very stupid code, but I have to do it...
-            pass
-    
-    return dates
-
-def date_removal(df:PolarsFrame) -> PolarsFrame:
-    '''Removes all date columns from dataframe. This algorithm will try to infer if string column is date.'''
-
-    remove_cols = date_inferral(df) 
-    logger.info(f"The following columns are dropped because they are dates. {remove_cols}.\n"
-                f"Removed a total of {len(remove_cols)} columns.")
-    return drop(df, remove_cols)
-
-def invalid_inferral(df:PolarsFrame, threshold:float=0.5, include_null:bool=False) -> list[str]:
-    '''
-    Infers numeric columns that have more than threshold pct of invalid (NaN) values.
-    
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars dataframe
-    threshold
-        Columns with higher than threshold null pct will be dropped. Threshold should be between 0 and 1.
-    include_null
-        If true, then null values will also be counted as invalid.
-    '''
-    nums = get_numeric_cols(df)
-    df_local = df.lazy().select(nums).with_row_count(offset=1).set_sorted("row_nr")
-    if include_null:
-        expr = (pl.all().is_nan().sum() + pl.all().is_null().sum())/pl.col("row_nr").max()
-    else:
-        expr = pl.all().is_nan().sum()/pl.col("row_nr").max()
-    
-    return (
-        df_local.select(
-            expr
-        ).select(~cs.by_name(["row_nr"]))
-        .collect()
-        .transpose(include_header=True, column_names=["nan_pct"])
-        .filter(pl.col("nan_pct") >= threshold)
-        .get_column("column")
-        .to_list()
-    )
-
-def invalid_removal(df:PolarsFrame, threshold:float=0.5, include_null:bool=False) -> PolarsFrame:
-    '''
-    Removes numeric columns that have more than threshold pct of invalid (NaN) values.
-    
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars dataframe
-    threshold
-        Columns with higher than threshold null pct will be dropped. Threshold should be between 0 and 1.
-    include_null
-        If true, then null values will also be counted as invalid.
-    '''
-    remove_cols = invalid_inferral(df, threshold, include_null) 
-    logger.info(f"The following columns are dropped because they have more than {threshold*100:.2f}%"
-                f" not valid values. {remove_cols}.\n"
-                f"Removed a total of {len(remove_cols)} columns.")
-    return drop(df, remove_cols)
-
-def null_inferral(df:PolarsFrame, threshold:float=0.5) -> list[str]:
-    '''
-    Infers columns that have more than threshold pct of null values.
-    
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars dataframe
-    threshold
-        Columns with higher than threshold null pct will be dropped. Threshold should be between 0 and 1.
-    '''
-    return (df.lazy().null_count().collect()/len(df)).transpose(include_header=True, column_names=["null_pct"])\
-                    .filter(pl.col("null_pct") >= threshold)\
-                    .get_column("column").to_list()
-
-def null_removal(df:PolarsFrame, threshold:float=0.5) -> PolarsFrame:
-    '''
-    Removes columns with more than threshold pct of null values.
-
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars dataframe
-    threshold
-        Columns with higher than threshold null pct will be dropped. Threshold should be between 0 and 1.
-    '''
-    remove_cols = null_inferral(df, threshold) 
-    logger.info(f"The following columns are dropped because they have more than {threshold*100:.2f}%"
-                f" null values. {remove_cols}.\n"
-                f"Removed a total of {len(remove_cols)} columns.")
-    return drop(df, remove_cols)
-
-def var_inferral(df:PolarsFrame, threshold:float, target:str) -> list[str]:
-    '''Infers columns that have lower than threshold variance. Target will not be included.'''
-    return df.lazy().select(
-                pl.col(x).var() for x in get_numeric_cols(df) if x != target
-            ).collect().transpose(include_header=True, column_names=["var"])\
-            .filter(pl.col("var") < threshold).get_column("column").to_list() 
-
-def var_removal(df:PolarsFrame, threshold:float, target:str) -> PolarsFrame:
-    '''Removes features with low variance. Features with > threshold variance will be kept. 
-        Threshold should be positive.'''
-
-    remove_cols = var_inferral(df, threshold, target) 
-    logger.info(f"The following columns are dropped because they have lower than {threshold} variance. {remove_cols}.\n"
-                f"Removed a total of {len(remove_cols)} columns.")
-    return drop(df, remove_cols)
-
-# Really this is just an alias
-regex_inferral = get_cols_regex
-
-def regex_removal(df:PolarsFrame, pattern:str, lowercase:bool=False) -> PolarsFrame:
-    '''
-    Remove columns if their names satisfy the given regex rules. This is common when you want to remove columns 
-    with certain prefixes that may not be allowed to use in models.
-
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars dataframe
-    pattern
-        The regex pattern
-    lowercase
-        Whether to lowercase everything and then match
-    '''
-    remove_cols = get_cols_regex(df, pattern, lowercase)
-    logger.info(f"The following columns are dropped because their names satisfy the regex rule: {pattern}."
-                f" {remove_cols}.\n"
-                f"Removed a total of {len(remove_cols)} columns.")
-    
-    return drop(df, remove_cols)
-
-def get_unique_count(df:PolarsFrame, include_null_count:bool=False) -> pl.DataFrame:
-    '''
-    Gets unique counts for columns and returns a dataframe with schema = ["column", "n_unique"]. Null count
-    is useful in knowing if null is one of the unique values and thus is included as an option. Note that
-    null != NaN.
-
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars dataframe
-    include_null_count
-        If true, this will return a dataframe with schema = ["column", "n_unique", "null_count"]
-    '''
-    if include_null_count:
-        temp = df.lazy().select(
-            pl.all().n_unique().suffix("_n_unique"),
-            pl.all().null_count().suffix("_null_count")
-        ).collect().row(0)
-        n = len(df.columns)
-        return pl.from_records((df.columns, temp[:n], temp[n:]), schema=["column", "n_unique", "null_count"])
-    else:
-        return df.lazy().select(
-            pl.all().n_unique()
-        ).collect().transpose(include_header=True, column_names=["n_unique"])
-
-# Really this is just an alias
-def unique_inferral(df:PolarsFrame, threshold:float=0.9) -> list[str]:
-    '''
-    Infers columns that have higher than threshold unique pct.
-
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars dataframe
-    threshold
-        Every column with unique pct higher than this threshold will be returned. Note that 
-        threshold will be clipped between 0.01 and 0.99.
-    '''
-    clipped_threshold = min(0.99, max(threshold, 0.01))
-    temp = get_unique_count(df.with_row_count(offset=1))
-    len_df:int = temp.filter(pl.col("column") == "row_nr").item(0,1)
-    return (
-        temp.with_columns(
-            (pl.col("n_unique")/len_df).alias("unique_pct")
-        ).filter((pl.col("unique_pct") >= clipped_threshold) & (pl.col("column") != "row_nr"))\
-        .get_column("column")
-        .to_list()
-    )
-
-def unique_removal(df:PolarsFrame, threshold:float=0.9) -> PolarsFrame:
-    '''
-    Remove columns that have higher than threshold pct of unique values. Usually this is done to filter
-    out id-like columns
-
-    Parameters
-    ----------
-    df
-        Either a lazy or an eager Polars dataframe
-    threshold
-        The threshold for unique pct. Columns with higher than this threshold unique pct will be removed 
-    '''
-    remove_cols = unique_inferral(df, threshold)
-    logger.info(f"The following columns are dropped because more than {threshold*100:.2f}% of unique values."
-                f" {remove_cols}.\n"
-                f"Removed a total of {len(remove_cols)} columns.")
-    return drop(df, remove_cols)
-
-# Once there is a config, add a discrete criterion config
-def discrete_inferral(df:PolarsFrame
-    , threshold:float=0.1
-    , max_n_unique:int=100
-    , exclude:Optional[list[str]]=None
-) -> list[str]:
-    '''
-    A column that satisfies either n_unique < max_n_unique or unique_pct < threshold 
-    will be considered discrete. E.g. threshold = 0.1 and max_n_unique = 100 means if a 
-    column has < 100 unique values, or the unique pct is < 10%, then it will be considered
-    as discrete.
-
-    Parameters
-    ----------
-    df
-        Either a lazy or an eager Polars dataframe
-    threshold
-        The threshold for unique pct
-    max_n_unique
-        The maximum number of unique values allowed for a column to be considered discrete
-    exclude
-        List of columns to exclude
-    '''
-    exclude_list = [] if exclude is None else exclude
-    exclude_list.append("row_nr")
-    temp = get_unique_count(df.with_row_count(offset=1).set_sorted("row_nr"))
-    len_df = temp.filter(pl.col("column") == "row_nr").item(0,1)
-    return temp.filter(
-        ((pl.col("n_unique") < max_n_unique) | (pl.col("n_unique")/len_df < threshold)) 
-        & (~pl.col("column").is_in(exclude_list)) # is not in
-    ).get_column("column").to_list()
-
-def conti_inferral(
-    df:PolarsFrame
-    , discrete_threshold:float = 0.1
-    , discrete_max_n_unique:int = 100
-    , exclude:Optional[list[str]]=None
-) -> list[str]:
-    '''
-    Returns everything that is not considered discrete.
-
-    Parameters
-    ----------
-    df
-        Either a lazy or an eager Polars dataframe
-    discrete_threshold
-        The threshold for unique pct in discrete inferral
-    discrete_max_n_unique
-        The maximum number of unique values allowed for a column to be considered discrete
-    exclude
-        List of columns to exclude
-    '''
-    exclude_list = [] if exclude is None else exclude
-    discrete = discrete_inferral(df, discrete_threshold, discrete_max_n_unique)
-    return df.select(cs.numeric() & ~cs.by_name(exclude_list) & ~cs.by_name(discrete)).columns
-
-def constant_inferral(df:PolarsFrame, include_null:bool=True) -> list[str]:
-    '''
-    Returns a list of inferred constant columns.
-    
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars dataframe
-    include_null
-        If true, then columns with two distinct values like [value_1, null] will be considered a 
-        constant column
-    '''
-    if include_null:
-        return get_unique_count(df, include_null_count=True).filter(
-            ((pl.col("n_unique") == 1) | ((pl.col("n_unique") == 2) & (pl.col("null_count") > 0)))
-        ).get_column("column").to_list()
-    else:
-        return get_unique_count(df).filter(pl.col("n_unique") == 1).get_column("column").to_list()
-
-def constant_removal(df:PolarsFrame, include_null:bool=True) -> PolarsFrame:
-    '''
-    Removes all constant columns from dataframe.
-    
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars dataframe
-    include_null
-        If true, then columns with two distinct values like [value_1, null] will be considered a 
-        constant column
-    '''
-    remove_cols = constant_inferral(df, include_null)
-    logger.info(f"The following columns are dropped because they are constants. {remove_cols}.\n"
-                f"Removed a total of {len(remove_cols)} columns.")
-    return drop(df, remove_cols)
-
-def remove_if_exists(df:PolarsFrame, cols:list[str]) -> PolarsFrame:
-    '''Removes the given columns if they exist in the dataframe.'''
-    remove_cols = list(set(cols).intersection(df.columns))
-    logger.info(f"The following columns are dropped. {remove_cols}.\nRemoved a total of {len(remove_cols)} columns.")
-    return drop(df, remove_cols)
-
-#----------------------------------------------------------------------------------------------#
-# More statistical Methods
-#----------------------------------------------------------------------------------------------#
-
-def _ks_compare(
-    df:pl.DataFrame
-    , pair:Tuple[str, str]
-    , alt:Alternatives="two-sided"
-) -> Tuple[Tuple[str, str], float, float]:
-    res = ks_2samp(df.get_column(pair[0]), df.get_column(pair[1]), alt)
-    return (pair, res.statistic, res.pvalue)
-
-def ks_compare(
-    df:PolarsFrame
-    , target:Optional[str] = None
-    , smaple_frac:float = 0.75
-    , test_cols:Optional[list[str]] = None
-    , alt: Alternatives = "two-sided"
-    , skip:int = 0
-    , max_comp:int = 1000
-) -> pl.DataFrame:
-    '''
-    Run ks-stats on all non-discrete columns in the dataframe. If test_cols is None, it will infer non-discrete 
-    continuous columns. See docstring of discrete_inferral to see what is considered discrete. Provide the target 
-    so that it will not be included in the comparisons. Since ks 2 sample comparison is relatively expensive, we will
-    always sample 75% of the dataset, unless the user specifies a different sample_frac.
-
-    Note: this will only run on all 2 combinations of columns, starting from skip and end at skip + max_comp.
-
-    Note: The null hypothesis is that the two columns come from the same distribution. Therefore a small p-value means
-    that they do not come from the same distribution. Having p-value > threshold does not mean they have the same 
-    distribution automatically, and it requires more examination to reach the conclusion.
-    '''
-    if test_cols is None:
-        nums = [f for f in get_numeric_cols(df) if f not in discrete_inferral(df)]
-    else:
-        nums = test_cols
-
-    if target in nums:
-        nums.remove(target)
-
-    nums.sort()
-    if isinstance(df, pl.LazyFrame):
-        df_test = lazy_sample(df.select(nums).lazy(), sample_frac=smaple_frac).collect()
-    else:
-        df_test = df.select(nums).sample(fraction=smaple_frac)
-
-    n_c2 = comb(len(nums), 2)
-    last = min(skip + max_comp, n_c2)
-    results = []
-    to_test = enumerate(combinations(nums, 2))
-    pbar = tqdm(total=min(max_comp, n_c2 - skip), desc="Comparisons")
-    with ThreadPoolExecutor(max_workers=CPU_COUNT) as ex:
-        for f in as_completed(ex.submit(_ks_compare, df_test, pair, alt) 
-                              for i, pair in to_test if i < last and i > skip):
-            results.append(f.result())
-            pbar.update(1)
-
-    pbar.close()
-    return pl.from_records(results, schema=["combination", "ks-stats", "p-value"])
-
-def _dist_inferral(df:pl.DataFrame, c:str, dist:CommonContiDist) -> Tuple[str, float, float]:
-    res = kstest(df[c], dist)
-    return (c, res.statistic, res.pvalue)
-
-def dist_test(
-    df: PolarsFrame
-    , which_dist:CommonContiDist
-    , smaple_frac:float = 0.75
-    , target: Optional[str] = None
-) -> pl.DataFrame:
-    '''
-    Tests if the numeric columns follow the given distribution by using the KS test. If
-    target is provided it will be excluded. The null hypothesis is that the columns follow the given distribution. 
-    We sample 75% of data because ks test is relatively expensive.
-    '''
-    nums = get_numeric_cols(df, exclude=[target])
-    if isinstance(df, pl.LazyFrame):
-        df_test = lazy_sample(df.select(nums).lazy(), sample_frac=smaple_frac).collect()
-    else:
-        df_test = df.select(nums).sample(fraction=smaple_frac)
-
-    results = []
-    pbar = tqdm(total=len(nums), desc="Comparisons")
-    with ThreadPoolExecutor(max_workers=CPU_COUNT) as ex:
-        for f in as_completed(ex.submit(_dist_inferral, df_test, c, which_dist) for c in nums):
-            results.append(f.result())
-            pbar.update(1)
-
-    pbar.close()
-    return pl.from_records(results, schema=["feature", "ks-stats", "p_value"])
-
-def suggest_normal(
-    df:PolarsFrame
-    , target: Optional[str] = None
-    , threshold:float = 0.05
-) -> list[str]:
-    '''
-    Suggests which columns are normally distributed. This takes the columns for which the null hypothesis
-    cannot be rejected in the dist_test (KS test).
-    '''
-    return dist_test(df, "norm", target=target).filter(pl.col("p_value") > threshold)\
-        .get_column("feature").to_list()
-
-def suggest_uniform(
-    df:PolarsFrame
-    , target: Optional[str] = None
-    , threshold:float = 0.05
-) -> list[str]:
-    '''
-    Suggests which columns are uniformly distributed. This takes the columns for which the null hypothesis
-    cannot be rejected in the dist_test (KS test).
-    '''
-    return dist_test(df, "uniform", target=target).filter(pl.col("p_value") > threshold)\
-        .get_column("feature").to_list()
-
-def suggest_lognormal(
-    df:PolarsFrame
-    , target: Optional[str] = None
-    , threshold:float = 0.05
-) -> list[str]:
-    '''
-    Suggests which columns are log-normally distributed. This takes the columns which the null hypothesis
-    cannot be rejected in the dist_test (KS test).
-    '''
-    return dist_test(df, "lognorm", target=target).filter(pl.col("p_value") > threshold)\
-        .get_column("feature").to_list()
-
-def suggest_dist(
-    df:PolarsFrame
-    , target: Optional[str] = None
-    , threshold:float = 0.05
-    , dist: CommonContiDist = "norm"
-) -> list[str]:
-    '''
-    Suggests which columns follow the given distribution. This returns the columns which the null hypothesis
-    cannot be rejected in the dist_test (KS test).
-    '''
-    return dist_test(df, dist, target=target).filter(pl.col("p_value") > threshold)\
-        .get_column("feature").to_list()
+from .type_alias import (
+    PolarsFrame
+    , Alternatives
+    , CommonContiDist
+    , SimpleDtypes
+    , CPU_COUNT
+    , POLARS_DATETIME_TYPES
+    , POLARS_NUMERICAL_TYPES
+)
+from .sample import (
+    lazy_sample
+)
+from .blueprint import(
+    Blueprint  # noqa: F401
+)
+from datetime import datetime 
+from typing import Any, Optional, Tuple, Union
+from itertools import combinations
+from scipy.stats import (
+    ks_2samp
+    , kstest
+)
+from concurrent.futures import as_completed, ThreadPoolExecutor
+from tqdm import tqdm
+from math import comb
+import re
+import polars.selectors as cs
+import polars as pl
+import logging  
+
+logger = logging.getLogger(__name__)
+
+#----------------------------------------------------------------------------------------------#
+# Generic columns checks | Only works with Polars because Pandas's data types suck!            #
+#----------------------------------------------------------------------------------------------#
+def type_checker(df:PolarsFrame, cols:list[str], expected_type:SimpleDtypes, caller_name:str) -> bool:
+    types = check_columns_types(df, cols)
+    if types != expected_type:
+        raise ValueError(f"The call `{caller_name}` can only be used on {expected_type} columns, not {types} types.")
+    return True
+
+def get_numeric_cols(df:PolarsFrame, exclude:Optional[list[str]]=None) -> list[str]:
+    '''Returns numerical columns except those in exclude.'''
+    if exclude is None:
+        selector = cs.numeric()
+    else:
+        selector = cs.numeric() & ~cs.by_name(exclude)
+    return df.select(selector).columns
+
+def get_string_cols(df:PolarsFrame, exclude:Optional[list[str]]=None) -> list[str]:
+    '''Returns string columns except those in exclude.'''
+    if exclude is None:
+        selector = cs.string()
+    else:
+        selector = cs.string() & ~cs.by_name(exclude)
+    return df.select(selector).columns
+
+def get_datetime_cols(df:PolarsFrame) -> list[str]:
+    '''Returns only datetime columns. This will not try to infer date from strings.'''
+    return df.select(cs.datetime()).columns
+
+def get_bool_cols(df:PolarsFrame) -> list[str]:
+    '''Returns boolean columns.'''
+    return df.select(cs.by_dtype(pl.Boolean)).columns
+
+def get_cols_regex(df:PolarsFrame, pattern:str, lowercase:bool=False) -> list[str]:
+    '''
+    Returns columns that have names matching the regex pattern.
+    
+    
+    '''
+    if lowercase:
+        return (
+            df.rename({c:c.lower() for c in df.columns})
+            .select(cs.matches(pattern=pattern)).columns
+        )
+    else:
+        return df.select(cs.matches(pattern=pattern)).columns
+
+
+def rename(df:PolarsFrame, rename_dict:dict[str, str], persist:bool=False) -> PolarsFrame:
+    '''
+    A wrapper function for df.rename() so that it works with pipeline.
+
+    Set persist = True if this needs to be remembered by the blueprint.
+    '''
+    output = df.rename(rename_dict)
+    if isinstance(df, pl.LazyFrame) and persist:
+        return output.blueprint.add_func(df, rename, kwargs = {"rename_dict": rename_dict})
+    return output
+
+def lowercase(df:PolarsFrame, persist:bool=False) -> PolarsFrame:
+    '''
+    Lowercases all column names.
+
+    Set persist = True if this needs to be remembered by the blueprint.
+    '''
+    return rename(df, {c: c.lower() for c in df.columns}, persist)
+
+def snake_case(df:PolarsFrame, persist:bool=False) -> PolarsFrame:
+    '''
+    Turn all camel case column names into snake case.
+
+    Set persist = True if this needs to be remembered by the blueprint.
+    '''
+    pat = re.compile(r"(?<!^)(?=[A-Z])")
+    return rename(df, {c: pat.sub('_', c).lower() for c in df.columns}, persist)
+
+def select(
+    df:PolarsFrame
+    , selector: Union[list[str], cs._selector_proxy_]
+    , persist: bool = True
+) -> PolarsFrame:
+    '''
+    A select wrapper that makes it pipeline compatible.
+
+    Set persist = True if this needs to be remembered by the blueprint.
+    '''
+    if isinstance(df, pl.LazyFrame) and persist:
+        return df.blueprint.select(selector)
+    return df.select(selector)
+
+def drop(df:PolarsFrame, to_drop:list[str], persist:bool=True) -> PolarsFrame:
+    '''
+    A pipeline compatible way to drop the given columns, which will be remembered by the blueprint
+    by default.
+    '''
+    if isinstance(df, pl.LazyFrame) and persist:
+        return df.blueprint.drop(to_drop)
+    return df.drop(to_drop)
+
+def drop_nulls(
+    df:PolarsFrame
+    , subset:Optional[Union[list[str], str]] = None
+    , persist: bool = False
+) -> PolarsFrame:
+    '''
+    A wrapper function for Polars' drop_nulls so that it can be used in pipeline. Equivalent to
+    filter by pl.all_horizontal([pl.col(c).is_null() for c in subset]).
+
+    Set persist = True if this needs to be remembered by the blueprint.
+    '''
+    if isinstance(df, pl.LazyFrame) and persist:
+        if subset is None:
+            by = df.columns
+        elif isinstance(subset, str):
+            by = [subset]
+        else:
+            by = subset
+        expr = pl.all_horizontal([pl.col(c).is_null() for c in by])
+        return df.blueprint.filter(expr)
+    return df.drop_nulls(subset)
+
+def filter(
+    df:PolarsFrame
+    , condition: pl.Expr
+    , persist: bool = False
+) -> PolarsFrame:
+    ''' 
+    A wrapper function for Polars' filter so that it can be used in pipeline.
+
+    This will be remembered by blueprint by default.
+    '''
+    if isinstance(df, pl.LazyFrame) and persist:
+        return df.blueprint.filter(condition)
+    return df.filter(condition)
+
+def order_by(
+    df: PolarsFrame
+    , by: Union[str, list[str]]
+    , descending:bool = False
+    , nulls_last:bool = False
+    , persist: bool = False
+) -> PolarsFrame:
+    ''' 
+    A wrapper function for Polars' sort so that it can be used in pipeline.
+
+    Set persist = True if this needs to be remembered by the blueprint.
+    '''
+    output = df.sort(by=by, descending=descending, nulls_last=nulls_last)
+    if isinstance(df, pl.LazyFrame) and persist:
+        return output.blueprint.add_func(df, order_by, {"by":by,"descending":descending, "nulls_last":nulls_last})
+    return output
+
+def check_binary_target(df:PolarsFrame, target:str) -> bool:
+    '''
+    Checks if target is binary or not. Returns true only when binary target has 0s and 1s.
+    '''
+    target_uniques = df.lazy().select(pl.col(target).unique()).collect()[target]
+    if len(target_uniques) != 2:
+        logger.error("Target is not binary.")
+        return False
+    elif not (0 in target_uniques and 1 in target_uniques):
+        logger.error("The binary target is not encoded as 0s and 1s.")
+        return False
+    return True
+    
+def check_target_cardinality(df:PolarsFrame, target:str, raise_null:bool=True) -> pl.DataFrame:
+    '''
+    Returns a dataframe showing the cardinality of different target values. If raise_null = True, raise 
+    an exception if target column has any null values.
+    '''
+    output = df.lazy().groupby(target).count().sort(target).with_columns(
+        pct = pl.col("count")/pl.col("count").sum()
+    ).collect()
+    if raise_null and output[target].null_count() > 0:
+        raise ValueError("Target contains null.")
+    return output
+
+def format_categorical_target(
+    df:PolarsFrame
+    , target:str
+) -> Tuple[PolarsFrame, dict[Union[str, int], int]]:
+    '''
+    Apply an ordinal encoding to the target column for classification problems. This step helps you quickly
+    turn strings into multiple categories, but is not pipeline compatbile. This returns a target-modified df
+    and a mapping dict. It is recommended that you do this step outside the pipeline.
+
+    !!! This will NOT be persisted in blueprint and does NOT work in pipeline. !!!
+
+    Parameters
+    ----------
+    df
+        Either a lazy or an eager Polars dataframe
+    target
+        Name of target column
+    persist
+        Wheter or not this will be persisted by the blueprint
+
+    Example
+    -------
+    >>> import dsds.prescreen as ps
+    ... df = pl.DataFrame({
+    ...     "target":["A", "B", "C", "A", "B"]
+    ... })
+    ... new_df, mapping = ps.format_categorical_target(df, target="target")
+    >>> print(new_df)
+    >>> print(mapping)
+    shape: (5, 1)
+    ┌────────┐
+    │ target │
+    │ ---    │
+    │ u16    │
+    ╞════════╡
+    │ 0      │
+    │ 1      │
+    │ 2      │
+    │ 0      │
+    │ 1      │
+    └────────┘
+    {'A': 0, 'B': 1, 'C': 2}
+    '''
+    uniques = df.lazy().select(
+        t = pl.col(target).unique().sort()
+    ).collect().drop_in_place("t")
+    mapping = dict(zip(uniques, range(len(uniques))))
+    output = df.with_columns(
+        pl.col(target).map_dict(mapping, return_dtype=pl.UInt16)
+    )
+    return output, mapping
+
+def sparse_to_dense_target(df:PolarsFrame, target:str) -> PolarsFrame:
+    '''
+    If target column's elements are like [0,0,1], [0,1,0], etc. for a multicategorical 
+    classification problem, this will turn the target column into 2, 1, etc. This may return 
+    non-sensical results if you have more than one element >= 1 in the list.
+
+    !!! This step will NOT be remembered by the blueprint !!!
+
+    Parameters
+    ----------
+    df
+        Either a lazy or an eager Polars dataframe
+    target
+        Name of target column
+
+    Example
+    -------
+    >>> import dsds.prescreen as ps
+    ... df = pl.DataFrame({
+    ...     "target":[[0,0,1], [0,1,0], [1,0,0], [0,1,0], [1,0,0]]
+    ... })
+    >>> print(ps.sparse_to_dense_target(df, target="target"))
+    shape: (5, 1)
+    ┌────────┐
+    │ target │
+    │ ---    │
+    │ u32    │
+    ╞════════╡
+    │ 2      │
+    │ 1      │
+    │ 0      │
+    │ 1      │
+    │ 0      │
+    └────────┘
+    '''
+    _ = type_checker(df, [target], "list", "sparse_to_dense_target")
+    return df.with_columns(
+        pl.col(target).list.arg_max().alias(target)
+    )
+
+def dense_to_sparse_target(df:PolarsFrame, target:str) -> PolarsFrame:
+    '''
+    This turns dense target column into a sparse column. This steps assume your classification target 
+    is dense, meaning all categories have already been encoded to values in range 0,...,n_classes-1. If
+    your target is not dense, see `dsds.prescreen.format_categorical_target`.
+
+    !!! This step will NOT be remembered by the blueprint !!!
+
+    Parameters
+    ----------
+    df
+        Either a lazy or an eager Polars dataframe
+    target
+        Name of target column
+
+    Example
+    -------
+    >>> import dsds.prescreen as ps
+    ... df = pl.DataFrame({
+    ...     "target":[0,1,2,1,2,0]
+    ... })
+    >>> print(ps.dense_to_sparse_target(df, target="target"))
+    shape: (6, 1)
+    ┌───────────┐
+    │ target    │
+    │ ---       │
+    │ list[u8]  │
+    ╞═══════════╡
+    │ [1, 0, 0] │
+    │ [0, 1, 0] │
+    │ [0, 0, 1] │
+    │ [0, 1, 0] │
+    │ [0, 0, 1] │
+    │ [1, 0, 0] │
+    └───────────┘
+    '''
+    _ = type_checker(df, [target], "numeric", "dense_to_sparse_target")
+    n_unique = df.lazy().select(
+        n_unique = pl.col(target).max() + 1
+    ).collect().item(0,0)
+    return df.with_columns(
+        pl.col(target).apply(
+            lambda i: pl.zeros(n_unique, dtype=pl.UInt8, eager=True).set_at_idx(i, 1)
+        )
+    )
+
+def check_columns_types(df:PolarsFrame, cols:Optional[list[str]]=None) -> str:
+    '''
+    Returns the unique types of given columns in a single string. If multiple types are present
+    they are joined by a |. If cols is not given, automatically uses all columns.
+    '''
+    if cols is None:
+        check_cols:list[str] = df.columns
+    else:
+        check_cols:list[str] = cols 
+
+    types = sorted(set(dtype_mapping(t) for t in df.select(check_cols).dtypes))
+    return "|".join(types) if len(types) > 0 else "other/unknown"
+
+# dtype can be a "pl.datatype" or just some random data for which we want to infer a generic type.
+def dtype_mapping(d: Any) -> SimpleDtypes:
+    if isinstance(d, str) or d == pl.Utf8:
+        return "string"
+    elif isinstance(d, bool) or d == pl.Boolean:
+        return "bool"
+    elif isinstance(d, (int,float)) or d in POLARS_NUMERICAL_TYPES:
+        return "numeric"
+    elif isinstance(d, pl.List):
+        return "list" # Too many possibilities. Keep it to list for now.
+    elif isinstance(d, datetime) or d in POLARS_DATETIME_TYPES:
+        return "datetime"
+    else:
+        return "other/unknown"
+
+#----------------------------------------------------------------------------------------------#
+# Prescreen Inferral, Removal Methods                                                          #
+#----------------------------------------------------------------------------------------------#
+
+# Add a slim option that returns fewer stats? This is generic describe.
+def describe(
+    df:PolarsFrame
+    , sample_frac:float = 1.0
+    , percentiles: list[float] = [0.25, 0.75]
+    , exclude: Optional[list[str]] = None
+) -> pl.DataFrame:
+    '''
+    A more detailed profile the data than Polars' default. This is an expensive function. Please sample 
+    and exclude some columns if runtime is important.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars dataframe
+    sample_frac
+        If > 0 and < 1, will run profiling on a sample. This is recommended for bigger dataframes
+    percentiles
+        Percentile cuts that will be returned
+    exclude
+        List of columns to exclude
+    '''
+    selector = cs.all()
+    if exclude is not None:
+        selector = selector & ~cs.by_name(exclude)
+        
+    if sample_frac > 0 and sample_frac < 1:
+        if isinstance(df, pl.LazyFrame):
+            df_local = lazy_sample(df.select(selector), sample_frac=sample_frac).collect()
+        else:
+            df_local = df.select(selector).sample(fraction=sample_frac)
+    else:
+        df_local = df.lazy().select(selector).collect()
+
+    temp = df_local.describe(percentiles)
+    desc = temp.drop_in_place("describe")
+    # Get unique
+    unique_counts = get_unique_count(df_local).with_columns(
+        unique_pct = pl.col("n_unique") / len(df_local)
+    )
+    # Skew and Kurtosis
+    skew_and_kt_data = df_local.lazy().select(
+        pl.all().skew().prefix("skew:")
+        , pl.all().skew().prefix("kurtosis:")
+    ).collect().row(0)
+
+    n_cols = len(df_local.columns)
+    skew_and_kt = pl.from_records((df_local.columns, skew_and_kt_data[:n_cols], skew_and_kt_data[n_cols:])
+                                  , schema=["column", "skew", "kurtosis"])
+
+    # Get a basic string description of the data type.
+    dtypes_dict = dict(zip(df_local.columns, map(dtype_mapping, df_local.dtypes)))
+    # Get all percentiles
+    pat = re.compile("^\d+%$")
+    pctls = [d for d in desc if pat.search(d)]
+    # Numerical stuff
+    nums = ["count" ,"null_count", "mean", "std", "median"] + pctls
+    # Combine all
+    final = temp.transpose(include_header=True, column_names=desc).with_columns(
+        pl.col(c).cast(pl.Float64) for c in nums
+    ).with_columns(
+        null_pct = pl.col("null_count")/pl.col("count")
+        , non_null_count = pl.col("count") - pl.col("null_count")
+        , CoV = pl.col("std") / pl.col("mean")
+        , dtype = pl.col("column").map_dict(dtypes_dict)
+    ).join(unique_counts, on="column").join(skew_and_kt, on="column")
+    # select only the stuff we need
+    return final.select('column', 'dtype', "non_null_count", 'null_count','null_pct','n_unique'
+                        , 'unique_pct','mean','std', 'CoV','min','max','median',"skew", "kurtosis"
+                        , *pctls)
+
+# Numeric only describe. Be more detailed.
+
+# String only describe. Be more detailed about interesting string stats.
+
+def describe_str(
+    df:PolarsFrame
+    , words_to_count:Optional[list[str]]=None
+    , sample_frac:float = 0.75
+) -> pl.DataFrame:
+    '''
+    Computes some statistics about the string columns. Optionally you may pass a list
+    of strings to compute the total occurrences of each of the words in the string columns. If input is a LazyFrame, 
+    a sample of sample_pct will be used, and sample_pct will only be used in the lazy case. 
+    '''
+    strs = get_string_cols(df)
+    df_str = df.select(strs)
+    if isinstance(df, pl.LazyFrame):
+        df_str = lazy_sample(df_str, sample_frac=sample_frac).collect()
+
+    nstrs = len(strs)
+    stats = df.select(strs).select(
+        pl.all().null_count().prefix("nc:"),
+        pl.all().max().prefix("max:"),
+        pl.all().min().prefix("min:"),
+        pl.all().mode().first().prefix("mode:"),
+        pl.all().str.lengths().min().prefix("min_byte_len:"),
+        pl.all().str.lengths().max().prefix("max_byte_len:"),
+        pl.all().str.lengths().mean().prefix("avg_byte_len:"),
+        pl.all().str.lengths().median().prefix("median_byte_len:"),
+        pl.all().str.count_match(r"\s").mean().prefix("avg_space_cnt:"),
+        pl.all().str.count_match(r"[0-9]").mean().prefix("avg_digit_cnt:"),
+        pl.all().str.count_match(r"[A-Z]").mean().prefix("avg_cap_cnt:"),
+        pl.all().str.count_match(r"[a-z]").mean().prefix("avg_lower_cnt:")
+    ).row(0)
+    output = {
+        "features":strs,
+        "null_count": stats[:nstrs],
+        "min": stats[nstrs: 2*nstrs],
+        "max": stats[2*nstrs: 3*nstrs],
+        "mode": stats[3*nstrs: 4*nstrs],
+        "min_byte_len": stats[4*nstrs: 5*nstrs],
+        "max_byte_len": stats[5*nstrs: 6*nstrs],
+        "avg_byte_len": stats[6*nstrs: 7*nstrs],
+        "median_byte_len": stats[7*nstrs: 8*nstrs],
+        "avg_space_cnt": stats[8*nstrs: 9*nstrs],
+        "avg_digit_cnt": stats[9*nstrs: 10*nstrs],
+        "avg_cap_cnt": stats[10*nstrs: 11*nstrs],
+        "avg_lower_cnt": stats[11*nstrs: ],
+    }
+
+    if isinstance(words_to_count, list):
+        for w in words_to_count:
+            output["total_"+ w + "_count"] = df_str.select(
+                                                pl.all().str.count_match(w).sum().prefix("wc:")
+                                            ).row(0)
+
+    return pl.from_dict(output)
+
+# Add an outlier description
+
+# -----------------------------------------------------------------------------------------------
+def non_numeric_removal(df:PolarsFrame, include_bools:bool=False) -> PolarsFrame:
+    '''
+    Removes all non-numeric columns. If include_bools = True, then keep boolean columns.
+    '''
+    if include_bools:
+        selector = ~(cs.numeric()|cs.by_dtype(pl.Boolean))
+    else:
+        selector = ~cs.numeric()
+
+    non_nums = df.select(selector).columns
+    logger.info(f"The following columns are dropped because they are not numeric: {non_nums}.\n"
+                f"Removed a total of {len(non_nums)} columns.")
+    
+    return drop(df, non_nums)
+
+# Check if columns are duplicates. Might take time.
+def duplicate_inferral():
+    # Get profiles first.
+    # Divide into categories: bools, strings, numerics, datetimes.
+    # Then cut down list to columns that have the same min, max, n_unique and null_count.
+    # Then check equality..
+    pass
+
+def pattern_inferral(
+    df: PolarsFrame
+    , pattern:str
+    , sample_frac:float = 0.75
+    , sample_count:int = 100_000
+    , sample_rounds:int = 3
+    , threshold:float = 0.9
+    , count_null:bool = False
+) -> list[str]:
+    '''
+    Find all string columns whose elements reasonably match the given pattern. The match logic can 
+    be tuned using the all the parameters.
+
+    Parameters
+    ----------
+    sample_frac
+        The pct of the total dataframe to use as pool
+    sample_count
+        From the pool, how many rows to sample for each round 
+    sample_rounds
+        How many rounds of sampling we are doing
+    threshold
+        For each round, what is the match% that is needed to be a counted as a success. For instance, 
+        in round 1, for column x, we have 92% match rate, and threshold = 0.9. We count column x as a match for 
+        this round. In the end, the column must match for every round to be considered a real match.
+    count_null
+        For individual matches, do we want to count null as a match or not? If the column has high null pct,
+        the non-null values might mostly match the pattern. In this case, using count_null = True will match the column, 
+        while count_null = False will most likely exclude the column.
+
+    Returns:
+        a list of columns that pass the matching test
+    
+    '''
+    strs = get_string_cols(df)
+    df_local = lazy_sample(df.lazy(), sample_frac=sample_frac).collect()    
+    matches:set[str] = set(strs)
+    sample_size = min(sample_count, len(df_local)-1)
+    for _ in range(sample_rounds):
+        df_sample = df_local.sample(n = sample_size)
+        fail = df_sample.select(
+            (
+                pl.when(pl.col(s).is_null()).then(count_null).otherwise(
+                    pl.col(s).str.contains(pattern)
+                ).sum()/sample_size
+            ).alias(s) 
+            for s in strs
+        ).transpose(include_header=True, column_names=["pattern_match_pct"])\
+        .filter(pl.col("pattern_match_pct") < threshold)["column"]
+        # If the match failes in this round, remove the column.
+        matches.difference_update(fail)
+
+    return list(matches)
+
+def pattern_removal(
+    df: PolarsFrame
+    , pattern:str
+    , sample_pct:float = 0.75
+    , sample_count:int = 100_000
+    , sample_rounds:int = 3
+    , threshold:float = 0.9
+    , count_null:bool = False
+) -> PolarsFrame:
+    
+    remove_cols = pattern_inferral(
+        df
+        , pattern
+        , sample_pct
+        , sample_count
+        , sample_rounds
+        , threshold 
+        , count_null
+    )
+    logger.info(f"The following columns are dropped because they match the element pattern: {pattern}.\n"
+                f"{remove_cols}\n"
+                f"Removed a total of {len(remove_cols)} columns.")
+    
+    return drop(df, remove_cols)
+
+def email_inferral(
+    df: PolarsFrame
+    , sample_pct:float = 0.75
+    , sample_count:int = 100_000
+    , sample_rounds:int = 3
+    , threshold:float = 0.9
+    , count_null:bool = False
+) -> list[str]:
+    # Why does this regex not work?
+    # r'([A-Za-z0-9]+[.-_])*[A-Za-z0-9]+@[A-Za-z0-9-]+(\.[A-Z|a-z]{2,})+'
+    return pattern_inferral(
+        df
+        , r'\S+@\S+\.\S+'
+        , sample_pct
+        , sample_count
+        , sample_rounds
+        , threshold 
+        , count_null
+    )
+
+def email_removal(
+    df: PolarsFrame
+    , sample_pct:float = 0.75
+    , sample_count:int = 100_000
+    , sample_rounds:int = 3
+    , threshold:float = 0.9
+    , count_null:bool = False
+) -> PolarsFrame:
+    
+    emails = email_inferral(df, sample_pct, sample_count, sample_rounds, threshold, count_null)
+    logger.info(f"The following columns are dropped because they are emails. {emails}.\n"
+            f"Removed a total of {len(emails)} columns.")
+    
+    return drop(df, emails)
+
+# Check for columns that are US zip codes.
+# Might add options for other countries later.
+def zipcode_inferral():
+    # Match string using pattern inferral
+    # Take a look at integers too, are they always 5 digits? 
+    pass
+
+def date_inferral(df:PolarsFrame) -> list[str]:
+    '''Infers date columns in dataframe. This inferral is not perfect.'''
+    logger.info("Date Inferral is error prone due to the huge variety of date formats. Please use with caution.")
+    
+    dates = [c for c,t in zip(df.columns, df.dtypes) if t in POLARS_DATETIME_TYPES]
+    strings = get_string_cols(df)
+    # MIGHT REWRITE THIS LOGIC
+    # Might be memory intensive on big dataframes.
+    sample_size = min(len(df), 100_000)
+    sample_df = df.lazy().select(strings)\
+        .drop_nulls().collect()\
+        .sample(n = sample_size).select(
+            # Cleaning the string first. Only try to catch string dates which are in the first split by space
+           pl.col(s).str.strip().str.replace_all("(/|\.)", "-").str.split(by=" ").list.first() 
+           for s in strings
+        )
+    for s in strings:
+        try:
+            c = sample_df[s].str.to_date(strict=False)
+            if 1 - c.null_count()/sample_size >= 0.15: # if at least 15% valid (able to be converted)
+                # This last check is to account for single digit months.
+                # 3/3/1995 will not be parsed to a string because standard formats require 03/03/1995
+                # At least 15% of dates naturally have both month and day as 2 digits numbers
+                dates.append(s)
+        except: # noqa: E722
+            # Very stupid code, but I have to do it...
+            pass
+    
+    return dates
+
+def date_removal(df:PolarsFrame) -> PolarsFrame:
+    '''Removes all date columns from dataframe. This algorithm will try to infer if string column is date.'''
+
+    remove_cols = date_inferral(df) 
+    logger.info(f"The following columns are dropped because they are dates. {remove_cols}.\n"
+                f"Removed a total of {len(remove_cols)} columns.")
+    return drop(df, remove_cols)
+
+def invalid_inferral(df:PolarsFrame, threshold:float=0.5, include_null:bool=False) -> list[str]:
+    '''
+    Infers numeric columns that have more than threshold pct of invalid (NaN) values.
+    
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars dataframe
+    threshold
+        Columns with higher than threshold null pct will be dropped. Threshold should be between 0 and 1.
+    include_null
+        If true, then null values will also be counted as invalid.
+    '''
+    nums = get_numeric_cols(df)
+    df_local = df.lazy().select(nums).with_row_count(offset=1).set_sorted("row_nr")
+    if include_null:
+        expr = (pl.all().is_nan().sum() + pl.all().is_null().sum())/pl.col("row_nr").max()
+    else:
+        expr = pl.all().is_nan().sum()/pl.col("row_nr").max()
+    
+    return (
+        df_local.select(
+            expr
+        ).select(~cs.by_name(["row_nr"]))
+        .collect()
+        .transpose(include_header=True, column_names=["nan_pct"])
+        .filter(pl.col("nan_pct") >= threshold)["column"]
+        .to_list()
+    )
+
+def invalid_removal(df:PolarsFrame, threshold:float=0.5, include_null:bool=False) -> PolarsFrame:
+    '''
+    Removes numeric columns that have more than threshold pct of invalid (NaN) values.
+    
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars dataframe
+    threshold
+        Columns with higher than threshold null pct will be dropped. Threshold should be between 0 and 1.
+    include_null
+        If true, then null values will also be counted as invalid.
+    '''
+    remove_cols = invalid_inferral(df, threshold, include_null) 
+    logger.info(f"The following columns are dropped because they have more than {threshold*100:.2f}%"
+                f" not valid values. {remove_cols}.\n"
+                f"Removed a total of {len(remove_cols)} columns.")
+    return drop(df, remove_cols)
+
+def null_inferral(df:PolarsFrame, threshold:float=0.5) -> list[str]:
+    '''
+    Infers columns that have more than threshold pct of null values.
+    
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars dataframe
+    threshold
+        Columns with higher than threshold null pct will be dropped. Threshold should be between 0 and 1.
+    '''
+    return (df.lazy().null_count().collect()/len(df)).transpose(include_header=True, column_names=["null_pct"])\
+                    .filter(pl.col("null_pct") >= threshold)["column"].to_list()
+
+def null_removal(df:PolarsFrame, threshold:float=0.5) -> PolarsFrame:
+    '''
+    Removes columns with more than threshold pct of null values.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars dataframe
+    threshold
+        Columns with higher than threshold null pct will be dropped. Threshold should be between 0 and 1.
+    '''
+    remove_cols = null_inferral(df, threshold) 
+    logger.info(f"The following columns are dropped because they have more than {threshold*100:.2f}%"
+                f" null values. {remove_cols}.\n"
+                f"Removed a total of {len(remove_cols)} columns.")
+    return drop(df, remove_cols)
+
+def var_inferral(df:PolarsFrame, threshold:float, target:str) -> list[str]:
+    '''Infers columns that have lower than threshold variance. Target will not be included.'''
+    return df.lazy().select(
+                pl.col(x).var() for x in get_numeric_cols(df) if x != target
+            ).collect().transpose(include_header=True, column_names=["var"])\
+            .filter(pl.col("var") < threshold)["column"].to_list() 
+
+def var_removal(df:PolarsFrame, threshold:float, target:str) -> PolarsFrame:
+    '''Removes features with low variance. Features with > threshold variance will be kept. 
+        Threshold should be positive.'''
+
+    remove_cols = var_inferral(df, threshold, target) 
+    logger.info(f"The following columns are dropped because they have lower than {threshold} variance. {remove_cols}.\n"
+                f"Removed a total of {len(remove_cols)} columns.")
+    return drop(df, remove_cols)
+
+# Really this is just an alias
+regex_inferral = get_cols_regex
+
+def regex_removal(df:PolarsFrame, pattern:str, lowercase:bool=False) -> PolarsFrame:
+    '''
+    Remove columns if their names satisfy the given regex rules. This is common when you want to remove columns 
+    with certain prefixes that may not be allowed to use in models.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars dataframe
+    pattern
+        The regex pattern
+    lowercase
+        Whether to lowercase everything and then match
+    '''
+    remove_cols = get_cols_regex(df, pattern, lowercase)
+    logger.info(f"The following columns are dropped because their names satisfy the regex rule: {pattern}."
+                f" {remove_cols}.\n"
+                f"Removed a total of {len(remove_cols)} columns.")
+    
+    return drop(df, remove_cols)
+
+def get_unique_count(df:PolarsFrame, include_null_count:bool=False) -> pl.DataFrame:
+    '''
+    Gets unique counts for columns and returns a dataframe with schema = ["column", "n_unique"]. Null count
+    is useful in knowing if null is one of the unique values and thus is included as an option. Note that
+    null != NaN.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars dataframe
+    include_null_count
+        If true, this will return a dataframe with schema = ["column", "n_unique", "null_count"]
+    '''
+    if include_null_count:
+        temp = df.lazy().select(
+            pl.all().n_unique().suffix("_n_unique"),
+            pl.all().null_count().suffix("_null_count")
+        ).collect().row(0)
+        n = len(df.columns)
+        return pl.from_records((df.columns, temp[:n], temp[n:]), schema=["column", "n_unique", "null_count"])
+    else:
+        return df.lazy().select(
+            pl.all().n_unique()
+        ).collect().transpose(include_header=True, column_names=["n_unique"])
+
+# Really this is just an alias
+def unique_inferral(df:PolarsFrame, threshold:float=0.9) -> list[str]:
+    '''
+    Infers columns that have higher than threshold unique pct.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars dataframe
+    threshold
+        Every column with unique pct higher than this threshold will be returned. Note that 
+        threshold will be clipped between 0.01 and 0.99.
+    '''
+    clipped_threshold = min(0.99, max(threshold, 0.01))
+    temp = get_unique_count(df.with_row_count(offset=1))
+    len_df:int = temp.filter(pl.col("column") == "row_nr").item(0,1)
+    return (
+        temp.with_columns(
+            (pl.col("n_unique")/len_df).alias("unique_pct")
+        ).filter((pl.col("unique_pct") >= clipped_threshold) & (pl.col("column") != "row_nr"))["column"]
+        .to_list()
+    )
+
+def unique_removal(df:PolarsFrame, threshold:float=0.9) -> PolarsFrame:
+    '''
+    Remove columns that have higher than threshold pct of unique values. Usually this is done to filter
+    out id-like columns
+
+    Parameters
+    ----------
+    df
+        Either a lazy or an eager Polars dataframe
+    threshold
+        The threshold for unique pct. Columns with higher than this threshold unique pct will be removed 
+    '''
+    remove_cols = unique_inferral(df, threshold)
+    logger.info(f"The following columns are dropped because more than {threshold*100:.2f}% of unique values."
+                f" {remove_cols}.\n"
+                f"Removed a total of {len(remove_cols)} columns.")
+    return drop(df, remove_cols)
+
+# Once there is a config, add a discrete criterion config
+def discrete_inferral(df:PolarsFrame
+    , threshold:float=0.1
+    , max_n_unique:int=100
+    , exclude:Optional[list[str]]=None
+) -> list[str]:
+    '''
+    A column that satisfies either n_unique < max_n_unique or unique_pct < threshold 
+    will be considered discrete. E.g. threshold = 0.1 and max_n_unique = 100 means if a 
+    column has < 100 unique values, or the unique pct is < 10%, then it will be considered
+    as discrete.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or an eager Polars dataframe
+    threshold
+        The threshold for unique pct
+    max_n_unique
+        The maximum number of unique values allowed for a column to be considered discrete
+    exclude
+        List of columns to exclude
+    '''
+    exclude_list = [] if exclude is None else exclude
+    exclude_list.append("row_nr")
+    temp = get_unique_count(df.with_row_count(offset=1).set_sorted("row_nr"))
+    len_df = temp.filter(pl.col("column") == "row_nr").item(0,1)
+    return temp.filter(
+        ((pl.col("n_unique") < max_n_unique) | (pl.col("n_unique")/len_df < threshold)) 
+        & (~pl.col("column").is_in(exclude_list)) # is not in
+    )["column"].to_list()
+
+def conti_inferral(
+    df:PolarsFrame
+    , discrete_threshold:float = 0.1
+    , discrete_max_n_unique:int = 100
+    , exclude:Optional[list[str]]=None
+) -> list[str]:
+    '''
+    Returns everything that is not considered discrete.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or an eager Polars dataframe
+    discrete_threshold
+        The threshold for unique pct in discrete inferral
+    discrete_max_n_unique
+        The maximum number of unique values allowed for a column to be considered discrete
+    exclude
+        List of columns to exclude
+    '''
+    exclude_list = [] if exclude is None else exclude
+    discrete = discrete_inferral(df, discrete_threshold, discrete_max_n_unique)
+    return df.select(cs.numeric() & ~cs.by_name(exclude_list) & ~cs.by_name(discrete)).columns
+
+def constant_inferral(df:PolarsFrame, include_null:bool=True) -> list[str]:
+    '''
+    Returns a list of inferred constant columns.
+    
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars dataframe
+    include_null
+        If true, then columns with two distinct values like [value_1, null] will be considered a 
+        constant column
+    '''
+    if include_null:
+        return get_unique_count(df, include_null_count=True).filter(
+            ((pl.col("n_unique") == 1) | ((pl.col("n_unique") == 2) & (pl.col("null_count") > 0)))
+        )["column"].to_list()
+    else:
+        return get_unique_count(df).filter(pl.col("n_unique") == 1)["column"].to_list()
+
+def constant_removal(df:PolarsFrame, include_null:bool=True) -> PolarsFrame:
+    '''
+    Removes all constant columns from dataframe.
+    
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars dataframe
+    include_null
+        If true, then columns with two distinct values like [value_1, null] will be considered a 
+        constant column
+    '''
+    remove_cols = constant_inferral(df, include_null)
+    logger.info(f"The following columns are dropped because they are constants. {remove_cols}.\n"
+                f"Removed a total of {len(remove_cols)} columns.")
+    return drop(df, remove_cols)
+
+def remove_if_exists(df:PolarsFrame, cols:list[str]) -> PolarsFrame:
+    '''Removes the given columns if they exist in the dataframe.'''
+    remove_cols = list(set(cols).intersection(df.columns))
+    logger.info(f"The following columns are dropped. {remove_cols}.\nRemoved a total of {len(remove_cols)} columns.")
+    return drop(df, remove_cols)
+
+#----------------------------------------------------------------------------------------------#
+# More statistical Methods
+#----------------------------------------------------------------------------------------------#
+
+def _ks_compare(
+    df:pl.DataFrame
+    , pair:Tuple[str, str]
+    , alt:Alternatives="two-sided"
+) -> Tuple[Tuple[str, str], float, float]:
+    res = ks_2samp(df[pair[0]], df[pair[1]], alt)
+    return (pair, res.statistic, res.pvalue)
+
+def ks_compare(
+    df:PolarsFrame
+    , target:Optional[str] = None
+    , smaple_frac:float = 0.75
+    , test_cols:Optional[list[str]] = None
+    , alt: Alternatives = "two-sided"
+    , skip:int = 0
+    , max_comp:int = 1000
+) -> pl.DataFrame:
+    '''
+    Run ks-stats on all non-discrete columns in the dataframe. If test_cols is None, it will infer non-discrete 
+    continuous columns. See docstring of discrete_inferral to see what is considered discrete. Provide the target 
+    so that it will not be included in the comparisons. Since ks 2 sample comparison is relatively expensive, we will
+    always sample 75% of the dataset, unless the user specifies a different sample_frac.
+
+    Note: this will only run on all 2 combinations of columns, starting from skip and end at skip + max_comp.
+
+    Note: The null hypothesis is that the two columns come from the same distribution. Therefore a small p-value means
+    that they do not come from the same distribution. Having p-value > threshold does not mean they have the same 
+    distribution automatically, and it requires more examination to reach the conclusion.
+    '''
+    if test_cols is None:
+        nums = [f for f in get_numeric_cols(df) if f not in discrete_inferral(df)]
+    else:
+        nums = test_cols
+
+    if target in nums:
+        nums.remove(target)
+
+    nums.sort()
+    if isinstance(df, pl.LazyFrame):
+        df_test = lazy_sample(df.select(nums).lazy(), sample_frac=smaple_frac).collect()
+    else:
+        df_test = df.select(nums).sample(fraction=smaple_frac)
+
+    n_c2 = comb(len(nums), 2)
+    last = min(skip + max_comp, n_c2)
+    results = []
+    to_test = enumerate(combinations(nums, 2))
+    pbar = tqdm(total=min(max_comp, n_c2 - skip), desc="Comparisons")
+    with ThreadPoolExecutor(max_workers=CPU_COUNT) as ex:
+        for f in as_completed(ex.submit(_ks_compare, df_test, pair, alt) 
+                              for i, pair in to_test if i < last and i > skip):
+            results.append(f.result())
+            pbar.update(1)
+
+    pbar.close()
+    return pl.from_records(results, schema=["combination", "ks-stats", "p-value"])
+
+def _dist_inferral(df:pl.DataFrame, c:str, dist:CommonContiDist) -> Tuple[str, float, float]:
+    res = kstest(df[c], dist)
+    return (c, res.statistic, res.pvalue)
+
+def dist_test(
+    df: PolarsFrame
+    , which_dist:CommonContiDist
+    , smaple_frac:float = 0.75
+    , target: Optional[str] = None
+) -> pl.DataFrame:
+    '''
+    Tests if the numeric columns follow the given distribution by using the KS test. If
+    target is provided it will be excluded. The null hypothesis is that the columns follow the given distribution. 
+    We sample 75% of data because ks test is relatively expensive.
+    '''
+    nums = get_numeric_cols(df, exclude=[target])
+    if isinstance(df, pl.LazyFrame):
+        df_test = lazy_sample(df.select(nums).lazy(), sample_frac=smaple_frac).collect()
+    else:
+        df_test = df.select(nums).sample(fraction=smaple_frac)
+
+    results = []
+    pbar = tqdm(total=len(nums), desc="Comparisons")
+    with ThreadPoolExecutor(max_workers=CPU_COUNT) as ex:
+        for f in as_completed(ex.submit(_dist_inferral, df_test, c, which_dist) for c in nums):
+            results.append(f.result())
+            pbar.update(1)
+
+    pbar.close()
+    return pl.from_records(results, schema=["feature", "ks-stats", "p_value"])
+
+def suggest_normal(
+    df:PolarsFrame
+    , target: Optional[str] = None
+    , threshold:float = 0.05
+) -> list[str]:
+    '''
+    Suggests which columns are normally distributed. This takes the columns for which the null hypothesis
+    cannot be rejected in the dist_test (KS test).
+    '''
+    return dist_test(df, "norm", target=target)\
+        .filter(pl.col("p_value") > threshold)["feature"].to_list()
+
+def suggest_uniform(
+    df:PolarsFrame
+    , target: Optional[str] = None
+    , threshold:float = 0.05
+) -> list[str]:
+    '''
+    Suggests which columns are uniformly distributed. This takes the columns for which the null hypothesis
+    cannot be rejected in the dist_test (KS test).
+    '''
+    return dist_test(df, "uniform", target=target)\
+        .filter(pl.col("p_value") > threshold)["feature"].to_list()
+
+def suggest_lognormal(
+    df:PolarsFrame
+    , target: Optional[str] = None
+    , threshold:float = 0.05
+) -> list[str]:
+    '''
+    Suggests which columns are log-normally distributed. This takes the columns which the null hypothesis
+    cannot be rejected in the dist_test (KS test).
+    '''
+    return dist_test(df, "lognorm", target=target)\
+        .filter(pl.col("p_value") > threshold)["feature"].to_list()
+
+def suggest_dist(
+    df:PolarsFrame
+    , target: Optional[str] = None
+    , threshold:float = 0.05
+    , dist: CommonContiDist = "norm"
+) -> list[str]:
+    '''
+    Suggests which columns follow the given distribution. This returns the columns which the null hypothesis
+    cannot be rejected in the dist_test (KS test).
+    '''
+    return dist_test(df, dist, target=target).filter(pl.col("p_value") > threshold)["feature"].to_list()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dsds-0.0.24/src/dsds/transform.py` & `dsds-0.0.25/python/dsds/transform.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,742 +1,890 @@
-from __future__ import annotations
-
-from .type_alias import (
-    PolarsFrame
-    , ImputationStrategy
-    , ScalingStrategy
-    , PowerTransformStrategy
-    , DateExtract
-    , ListExtract
-    , HorizontalExtract
-    , ZeroOneCombineRules
-    , clean_strategy_str
-)
-from .prescreen import type_checker
-from .blueprint import( # Need this for Polars extension to work
-    Blueprint  # noqa: F401
-)
-from typing import Optional, Union
-from scipy.stats import (
-    yeojohnson_normmax
-    , boxcox_normmax
-)
-import logging
-import math
-# import numpy as np
-import polars as pl
-
-# A lot of companies are still using Python < 3.10
-# So I am not using match statements
-
-logger = logging.getLogger(__name__)
-
-def impute(
-    df:PolarsFrame
-    , cols:list[str]
-    , strategy:ImputationStrategy = 'median'
-    , const:float = 1.
-) -> PolarsFrame:
-    '''
-    Impute the given columns with the given strategy.
-
-    This will be remembered by blueprint by default.
-
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars DataFrame
-    cols
-        The columns to impute
-    strategy
-        One of 'median', 'mean', 'const' or 'mode'. If 'const', the const argument should be provided. Note that
-        if strategy is mode and if two values occur the same number of times, a random one will be picked.
-    const
-        The constant value to impute by if strategy = 'const'    
-    '''
-    s = clean_strategy_str(strategy)
-    if s == "median":
-        all_medians = df.lazy().select(cols).median().collect().row(0)
-        exprs = (pl.col(c).fill_null(all_medians[i]) for i,c in enumerate(cols))
-    elif s in ("mean", "avg", "average"):
-        all_means = df.lazy().select(cols).mean().collect().row(0)
-        exprs = (pl.col(c).fill_null(all_means[i]) for i,c in enumerate(cols))
-    elif s in ("const", "constant"):
-        exprs = (pl.col(c).fill_null(const) for c in cols)
-    elif s in ("mode", "most_frequent"):
-        all_modes = df.lazy().select(cols).select(pl.all().mode().first()).collect().row(0)
-        exprs = (pl.col(c).fill_null(all_modes[i]) for i,c in enumerate(cols))
-    else:
-        raise TypeError(f"Unknown imputation strategy: {strategy}")
-
-    if isinstance(df, pl.LazyFrame):
-        return df.blueprint.with_columns(list(exprs))
-    return df.with_columns(exprs)
-
-def scale(
-    df:PolarsFrame
-    , cols:list[str]
-    , strategy:ScalingStrategy="standard"
-    , const:float = 1.0
-) -> PolarsFrame:
-    '''
-    Scale the given columns with the given strategy.
-
-    This will be remembered by blueprint by default.
-
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars DataFrame
-    cols
-        The columns to scale
-    strategy
-        One of 'standard', 'min_max', 'const'. If 'const', the const argument should be provided
-    const
-        The constant value to scale by if strategy = 'const'    
-    '''
-    _ = type_checker(df, cols, "numeric", "scale")
-    s = clean_strategy_str(strategy)
-    if s == "standard":
-        mean_std = df.lazy().select(cols).select(
-            pl.all().mean().prefix("mean:")
-            , pl.all().std().prefix("std:")
-        ).collect().row(0)
-        exprs = ( (pl.col(c) - mean_std[i])/(mean_std[i + len(cols)]) for i,c in enumerate(cols) )
-    elif s == "min_max":
-        min_max = df.lazy().select(cols).select(
-            pl.all().min().prefix("min:"),
-            pl.all().max().prefix("max:")
-        ).collect().row(0) # All mins come first, then maxs
-        exprs = ( (pl.col(c) - min_max[i])/((min_max[i + len(cols)] - min_max[i])) for i,c in enumerate(cols) )
-    elif s in ("const", "constant"):
-        exprs = (pl.col(c)/const for c in cols)
-    else:
-        raise TypeError(f"Unknown scaling strategy: {strategy}")
-
-    if isinstance(df, pl.LazyFrame):
-        return df.blueprint.with_columns(list(exprs))
-    return df.with_columns(exprs)
-
-def merge_infreq_values(
-    df: PolarsFrame
-    , cols: list[str]
-    , min_count: Optional[int] = 10
-    , min_frac: Optional[float] = None
-    , separator: str = '|'
-) -> PolarsFrame:
-    '''
-    Combines infrequent categories in string columns together.
-
-    This will be remembered by blueprint by default.
-
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars DataFrame
-    cols
-        List of string columns to perform this operation
-    min_count
-        Define a category to be infrequent if it occurs less than min_count. This defaults to 10 if both min_count and 
-        min_frac are None.
-    min_frac
-        Define category to be infrequent if it occurs less than this percentage of times. If both min_count and min_frac
-        are set, min_frac takes priority
-    separator
-        The separator for the new value representing the combined categories
-
-    Example
-    -------
-    >>> import dsds.transform as t
-    ... df = pl.DataFrame({
-    ...     "a":["a", "b", "c", "c", "c", "c", "c", "c", "c", "c", "c", "c", "c", "c"],
-    ...     "b":["a", "b", "c", "d", "d", "d", "d", "d", "d", "d", "d", "d", "d", "d"]
-    ... })
-    >>> df
-    shape: (14, 2)
-    ┌─────┬─────┐
-    │ a   ┆ b   │
-    │ --- ┆ --- │
-    │ str ┆ str │
-    ╞═════╪═════╡
-    │ a   ┆ a   │
-    │ b   ┆ b   │
-    │ c   ┆ c   │
-    │ c   ┆ d   │
-    │ …   ┆ …   │
-    │ c   ┆ d   │
-    │ c   ┆ d   │
-    │ c   ┆ d   │
-    │ c   ┆ d   │
-    └─────┴─────┘
-    >>> t.merge_infreq_values(df, ["a", "b"], min_count=3)
-    shape: (14, 2)
-    ┌─────┬───────┐
-    │ a   ┆ b     │
-    │ --- ┆ ---   │
-    │ str ┆ str   │
-    ╞═════╪═══════╡
-    │ a|b ┆ a|c|b │
-    │ a|b ┆ a|c|b │
-    │ c   ┆ a|c|b │
-    │ c   ┆ d     │
-    │ …   ┆ …     │
-    │ c   ┆ d     │
-    │ c   ┆ d     │
-    │ c   ┆ d     │
-    │ c   ┆ d     │
-    └─────┴───────┘
-    '''
-    _ = type_checker(df, cols, "string", "merge_infreq_values")
-    if min_frac is None:
-        if min_count is None:
-            comp = pl.col("count") < 10
-        else:
-            comp = pl.col("count") < min_count
-    else:
-        comp = pl.col("count")/pl.col("count").sum() < min_frac
-
-    exprs = []
-    for c in cols:
-        infreq = df.lazy().groupby(c).count().filter(
-            comp
-        ).collect().get_column(c)
-        value = separator.join(infreq)
-        exprs.append(
-            pl.when(pl.col(c).is_in(infreq)).then(value).otherwise(pl.col(c)).alias(c)
-        )
-    
-    if isinstance(df, pl.LazyFrame):
-        return df.blueprint.with_columns(exprs)
-    return df.with_columns(exprs)
-
-def combine_zero_ones(
-    df: PolarsFrame
-    , cols: list[str]
-    , new_name: str
-    , rule: ZeroOneCombineRules = "union"
-    , drop_original:bool = True
-) -> PolarsFrame:
-    '''
-    Take columns that are all binary 0, 1 columns, combine them according to the rule. Please make sure 
-    the columns only contain binary 0s and 1s. Depending on the rule, this can be used, for example, to 
-    quickly combine many one hot encoded columns into one, or reducing the same binary columns into one.
-
-    This will be remembered by blueprint by default.
-
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars DataFrame
-    cols
-        List of binary 0, 1 columns to combine
-    new_name
-        Name for the combined column
-    rule
-        One of 'union', 'intersection', 'same'.
-    drop_original
-        If true, drop column in cols
-
-    Examples
-    --------
-    >>> import dsds.transform as t
-    ... df = pl.DataFrame({
-    ...     "a": [1, 1, 0],
-    ...     "b":[1, 0, 1],
-    ...     "c":[1, 1, 1]
-    ... })
-    >>> t.combine_zero_ones(df, cols=["a", "b", "c"], new_name="abc", rule="same")
-    shape: (3, 1)
-    ┌─────┐
-    │ abc │
-    │ --- │
-    │ u8  │
-    ╞═════╡
-    │ 1   │
-    │ 0   │
-    │ 0   │
-    └─────┘
-    >>> t.combine_zero_ones(df, cols=["a", "b", "c"], new_name="abc", rule="union")
-    shape: (3, 1)
-    ┌─────┐
-    │ abc │
-    │ --- │
-    │ u8  │
-    ╞═════╡
-    │ 1   │
-    │ 1   │
-    │ 1   │
-    └─────┘
-    '''
-    if rule == "union":
-        expr = pl.max_horizontal([pl.col(c) for c in cols]).cast(pl.UInt8).alias(new_name)
-    elif rule == "intersection":
-        expr = pl.min_horizontal([pl.col(c) for c in cols]).cast(pl.UInt8).alias(new_name)
-    elif rule == "same":
-        expr = pl.when(sum(pl.col(c) for c in cols).is_in((0, len(cols)))).then(
-                    pl.lit(1, dtype=pl.UInt8)
-                ).otherwise(
-                    pl.lit(0, dtype=pl.UInt8)
-                ).alias(new_name)
-    else:
-        raise TypeError(f"The input `{rule}` is not a valid ZeroOneCombineRule.")
-
-    if isinstance(df, pl.LazyFrame):
-        if drop_original:
-            return df.blueprint.with_columns(expr).blueprint.drop(cols)
-        return df.blueprint.with_columns(expr)
-    if drop_original:
-        return df.with_columns(expr).drop(cols)
-    return df.with_columns(expr)
-
-def power_transform(
-    df: PolarsFrame
-    , cols: list[str]
-    , strategy: PowerTransformStrategy = "yeo_johnson"
-    # , lmbda: Optional[float] = None
-) -> PolarsFrame:
-    '''
-    Performs power transform on the numerical columns.
-
-    This will be remembered by blueprint by default.
-
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars dataframe
-    cols
-        Must be explicitly provided and must all be numerical
-    strategy
-        Either 'yeo_johnson' or 'box_cox'
-    '''
-    _ = type_checker(df, cols, "numeric", "power_transform")
-    s = clean_strategy_str(strategy)
-    exprs:list[pl.Expr] = []
-    # Ensure columns do not have missing values
-    non_null_list = []
-    with_null_list = []
-    for c, count in zip(cols, df.lazy().select(cols).null_count().collect().row(0)):
-        if count > 0:
-            with_null_list.append(c)
-        else:
-            non_null_list.append(c)
-
-    if len(with_null_list) > 0:
-        logger.info("The following columns will not be processed by power_transform because they contain missing "
-                    f"values. Please impute them:\n{with_null_list}")
-        
-    if s in ("yeo_johnson", "yeojohnson"):
-        lmaxs = df.lazy().select(non_null_list).groupby(1).agg(
-            pl.all()
-            .apply(lambda x: yeojohnson_normmax(x))
-            .cast(pl.Float64)
-        ).select(non_null_list).collect().row(0)
-        for c, lmax in zip(non_null_list, lmaxs):
-            if lmax == 0: # log(x + 1)
-                x_ge_0_sub_expr = (pl.col(c).add(1)).log()
-            else: # ((x + 1)**lmbda - 1) / lmbda
-                x_ge_0_sub_expr = ((pl.col(c).add(1)).pow(lmax) - 1) / lmax
-
-            if lmax == 2: # -log(-x + 1)
-                x_lt_0_sub_expr = pl.lit(-1) * (1 - pl.col(c)).log()
-            else: #  -((-x + 1)**(2 - lmbda) - 1) / (2 - lmbda)
-                t = 2 - lmax
-                x_lt_0_sub_expr = pl.lit(-1/t) * ((1 - pl.col(c)).pow(t) - 1)
-
-            exprs.append(
-                pl.when(pl.col(c).ge(0)).then(x_ge_0_sub_expr).otherwise(x_lt_0_sub_expr).alias(c)
-            )
-    elif s in ("box_cox", "boxcox"):
-        lmaxs = df.lazy().select(non_null_list).groupby(1).agg(
-            pl.all()
-            .apply(lambda x: boxcox_normmax(x, method="mle"))
-            .cast(pl.Float64)
-        ).select(non_null_list).collect().row(0)
-        exprs.extend(
-            pl.col(c).log() if lmax == 0 else (pl.col(c).pow(lmax) - 1) / lmax 
-            for c, lmax in zip(non_null_list, lmaxs)
-        )
-    else:
-        raise TypeError(f"The input strategy {strategy} is not a valid strategy. Valid strategies are: yeo_johnson "
-                        "or box_cox")
-    
-    if isinstance(df, pl.LazyFrame):
-        return df.blueprint.with_columns(exprs)
-    return df.with_columns(exprs)
-
-def normalize(
-    df: PolarsFrame
-    , cols:list[str]
-) -> PolarsFrame:
-    '''
-    Normalize the given columns by dividing them with the respective column sum.
-
-    !!! Note this will NOT be remembered by the blueprint !!!
-
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars dataframe
-    cols
-        Must be explicitly provided and should all be numeric columns
-    '''
-    _ = type_checker(df, cols, "numeric", "normalize")
-    return df.with_columns(pl.col(c)/pl.col(c).sum() for c in cols)
-
-def clip(
-    df: PolarsFrame
-    , cols: list[str]
-    , min_clip: Optional[float] = None
-    , max_clip: Optional[float] = None
-) -> PolarsFrame:
-    '''
-    Clips the columns within the min and max_clip bounds. This can be used to control outliers. If both min_clip and
-    max_clip are provided, perform two-sided clipping. If only one bound is provided, only one side will be clipped.
-    It will throw an error if both min and max_clips are not provided.
-
-    This will be remembered by blueprint by default.
-
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars dataframe
-    cols
-        Must be explicitly provided and should all be numeric columns
-    min_clip
-        Every value smaller than min_clip will be replaced by min_cap
-    max_clip
-        Every value bigger than max_clip will be replaced by max_cap
-    '''
-    _ = type_checker(df, cols, "numeric", "clip")
-    a:bool = min_clip is None
-    b:bool = max_clip is None
-    if a & (not b):
-        exprs = (pl.col(c).clip_max(max_clip) for c in cols)
-    elif (not a) & b:
-        exprs = (pl.col(c).clip_min(min_clip) for c in cols)
-    elif not (a | b):
-        exprs = (pl.col(c).clip(min_clip, max_clip) for c in cols)
-    else:
-        raise ValueError("At least one of min_cap and max_cap should be provided.")
-    
-    if isinstance(df, pl.LazyFrame):
-        return df.blueprint.with_columns(list(exprs))
-    return df.with_columns(exprs)
-
-def log_transform(
-    df: PolarsFrame
-    , cols:list[str]
-    , base:float = math.e
-    , cast_non_positive: Optional[float] = None
-    , plus_one:bool = False
-    , suffix:str = "_log"
-) -> PolarsFrame:
-    '''
-    Performs classical log transform on the given columns, e.g. log(x). You may set plus_one to perform ln(1 + x).
-    If you want to replace the original column, simply set suffix = "". If you intend to drop original columns, please
-    insert a `dsds.prescreen.drop` step in the pipeline.
-
-    This will be remembered by blueprint by default.
-
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars dataframe
-    cols
-        Must be explicitly provided and should all be numeric columns
-    base
-        Base of log. Default is math.e
-    cast_non_positive
-        How to deal with non positive values (<=0). None means turn them into null
-    plus_one
-        If plus_one is true, this will perform ln(1+x) and ignore base and cast_non_positive arguments
-    suffix
-        Choice of a suffix to the transformed columns. If this is the empty string "", then the original column
-        will be replaced. If plus_one = True, then suffix will always be "_log1p".
-    '''
-    _ = type_checker(df, cols, "numeric", "log_transform")
-    if plus_one:
-        exprs = (
-            pl.col(c).log1p().suffix("_log1p") for c in cols
-        )
-    else:
-        exprs = (
-            pl.when(pl.col(c) <= 0).then(cast_non_positive).otherwise(pl.col(c).log(base)).suffix(suffix) for c in cols
-        )
-    if isinstance(df, pl.LazyFrame):
-        return df.blueprint.with_columns(list(exprs))
-    return df.with_columns(exprs)
-
-def extract_dt_features(
-    df: PolarsFrame
-    , cols: list[str]
-    , extract: Union[DateExtract, list[DateExtract]] = ["year", "quarter", "month"]
-    , sunday_first: bool = False
-    , drop_original: bool = True
-) -> PolarsFrame:
-    '''
-    Extracts additional date related features from existing date/datetime columns.
-
-    This will be remembered by blueprint by default.
-
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars dataframe
-    cols
-        Must be explicitly provided and should all be date/datetime columns
-    extract
-        One of "year", "quarter", "month", "week", "day_of_week", "day_of_year", or a list of these values 
-        such as ["year", "quarter"], which means extract year and quarter from all the columns provided 
-    sunday_first
-        For day_of_week, by default, Monday maps to 1, and so on. If sunday_first = True, then Sunday will be
-        mapped to 1 and so on
-    drop_original
-        Whether to drop columns in cols
-
-    Example
-    -------
-    >>> import dsds.transform as t
-    ... df = pl.DataFrame({
-    ...     "date1":["2021-01-01", "2022-02-03", "2023-11-23"]
-    ...     , "date2":["2021-01-01", "2022-02-03", "2023-11-23"]
-    ... }).with_columns(
-    ...     pl.col(c).str.to_date() for c in ["date1", "date2"]
-    ... )
-    >>> print(df)
-    shape: (3, 2)
-    ┌────────────┬────────────┐
-    │ date1      ┆ date2      │
-    │ ---        ┆ ---        │
-    │ date       ┆ date       │
-    ╞════════════╪════════════╡
-    │ 2021-01-01 ┆ 2021-01-01 │
-    │ 2022-02-03 ┆ 2022-02-03 │
-    │ 2023-11-23 ┆ 2023-11-23 │
-    └────────────┴────────────┘
-    >>> cols = ["date1", "date2"]
-    >>> print(t.extract_dt_features(df, cols=cols, drop_original=False))
-    shape: (3, 8)
-    ┌────────────┬────────────┬────────────┬───────────┬───────────┬───────────┬───────────┬───────────┐
-    │ date1      ┆ date2      ┆ date1_year ┆ date2_yea ┆ date1_qua ┆ date2_qua ┆ date1_mon ┆ date2_mon │
-    │ ---        ┆ ---        ┆ ---        ┆ r         ┆ rter      ┆ rter      ┆ th        ┆ th        │
-    │ date       ┆ date       ┆ u32        ┆ ---       ┆ ---       ┆ ---       ┆ ---       ┆ ---       │
-    │            ┆            ┆            ┆ u32       ┆ u32       ┆ u32       ┆ u32       ┆ u32       │
-    ╞════════════╪════════════╪════════════╪═══════════╪═══════════╪═══════════╪═══════════╪═══════════╡
-    │ 2021-01-01 ┆ 2021-01-01 ┆ 2021       ┆ 2021      ┆ 1         ┆ 1         ┆ 1         ┆ 1         │
-    │ 2022-02-03 ┆ 2022-02-03 ┆ 2022       ┆ 2022      ┆ 1         ┆ 1         ┆ 2         ┆ 2         │
-    │ 2023-11-23 ┆ 2023-11-23 ┆ 2023       ┆ 2023      ┆ 4         ┆ 4         ┆ 11        ┆ 11        │
-    └────────────┴────────────┴────────────┴───────────┴───────────┴───────────┴───────────┴───────────┘
-    '''
-    _ = type_checker(df, cols, "datetime", "extract_dt_features")
-    exprs = []
-    if isinstance(extract, list):
-        to_extract = extract
-    else:
-        to_extract = [extract]
-    
-    for e in to_extract:
-        if e == "month":
-            exprs.extend(pl.col(c).dt.month().suffix("_month") for c in cols)
-        elif e == "year":
-            exprs.extend(pl.col(c).dt.year().suffix("_year") for c in cols)
-        elif e == "quarter":
-            exprs.extend(pl.col(c).dt.quarter().suffix("_quarter") for c in cols)
-        elif e == "week":
-            exprs.extend(pl.col(c).dt.week().suffix("_week") for c in cols)
-        elif e == "day_of_week":
-            if sunday_first:
-                exprs.extend(
-                    pl.when(pl.col(c).dt.weekday() == 7).then(1).otherwise(pl.col(c).dt.weekday()+1)
-                    .suffix("_day_of_week") 
-                    for c in cols
-                )
-            else:
-                exprs.extend(pl.col(c).dt.weekday().suffix("_day_of_week") for c in cols)
-        elif e == "day_of_year":
-            exprs.extend(pl.col(c).dt.ordinal_day().suffix("_day_of_year") for c in cols)
-        else:
-            logger.info(f"Found {e} in extract, but it is not a valid DateExtract value. Ignored.")
-
-    if isinstance(df, pl.LazyFrame):
-        if drop_original:
-            return df.blueprint.with_columns(exprs).blueprint.drop(cols)
-        return df.blueprint.with_columns(exprs)
-    if drop_original:
-        return df.with_columns(exprs).drop(cols)
-    return df.with_columns(exprs)
-    
-def extract_horizontally(
-    df:PolarsFrame
-    , cols: list[str]
-    , extract: Union[HorizontalExtract, list[HorizontalExtract]] = ["min", "max"]
-    , drop_original: bool = True
-) -> PolarsFrame:
-    '''
-    Extract features horizontally across a few columns.
-
-    This will be remembered by blueprint by default.
-
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars dataframe
-    cols
-        List of columns to extract feature from
-    extract
-        One of "min", "max", "sum", "any", "all". Note that "any" and "all" only make practical sense when 
-        all of cols are boolean columns, but they work even when cols are numbers.
-    drop_original
-        Whether to drop columns in cols
-
-    Example
-    -------
-    >>> import dsds.transform as t
-    ... df = pl.DataFrame({
-    ...     "a":[1, 2, 3],
-    ...     "b":[1, 2, 3],
-    ...     "c":[1, 2, 3]
-    ... })
-    >>> t.extract_horizontally(df, cols=["a", "b", "c"], extract=["min", "max", "sum"])
-    shape: (3, 3)
-    ┌────────────┬────────────┬────────────┐
-    │ min(a,b,c) ┆ max(a,b,c) ┆ sum(a,b,c) │
-    │ ---        ┆ ---        ┆ ---        │
-    │ i64        ┆ i64        ┆ i64        │
-    ╞════════════╪════════════╪════════════╡
-    │ 1          ┆ 1          ┆ 3          │
-    │ 2          ┆ 2          ┆ 6          │
-    │ 3          ┆ 3          ┆ 9          │
-    └────────────┴────────────┴────────────┘
-    '''
-    if isinstance(extract, list):
-        to_extract = extract
-    else:
-        to_extract = [extract]
-    
-    exprs = []
-    for e in to_extract:
-        if e == "min":
-            exprs.append(pl.min_horizontal([pl.col(c) for c in cols]).alias(f"{e}({','.join(cols)})"))
-        elif e == "max":
-            exprs.append(pl.max_horizontal([pl.col(c) for c in cols]).alias(f"{e}({','.join(cols)})"))
-        elif e == "sum":
-            exprs.append(pl.sum_horizontal([pl.col(c) for c in cols]).alias(f"{e}({','.join(cols)})"))
-        elif e == "any":
-            exprs.append(pl.any_horizontal([pl.col(c) for c in cols]).alias(f"{e}({','.join(cols)})"))
-        elif e == "all":
-            exprs.append(pl.all_horizontal([pl.col(c) for c in cols]).alias(f"{e}({','.join(cols)})"))
-        else:
-            logger.info(f"Found {e} in extract, but it is not a valid HorizontalExtract value. Ignored.")
-
-    if isinstance(df, pl.LazyFrame):
-        if drop_original:
-            return df.blueprint.with_columns(exprs).blueprint.drop(cols)
-        return df.blueprint.with_columns(exprs)
-    if drop_original:
-        return df.with_columns(exprs).drop(cols)
-    return df.with_columns(exprs)
-
-def extract_list_features(
-    df: PolarsFrame
-    , cols: list[str]
-    , extract: Union[ListExtract, list[ListExtract]] = ["min", "max"]
-    , drop_original: bool = True
-) -> PolarsFrame:
-    '''
-    Extract data from columns that contains lists.
-
-    This will be remembered by blueprint by default.
-
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars dataframe
-    cols
-        Must be explicitly provided and should all be date/datetime columns
-    extract
-        One of "min", "max", "mean", "len", "first", "last" or a list of these values such as ["min", "max"], 
-        which means extract min and max from all the columns provided. Notice if mean is provided, then the 
-        column must be list of numbers.
-    drop_original
-        Whether to drop columns in cols
-
-    Example
-    -------
-    >>> import dsds.transform as t
-    ... df = pl.DataFrame({
-    ...     "a":[["a"],["b"], ["c"]],
-    ...     "b":[[1,2], [3,3], [4,5,6]]
-    ... })
-    >>> t.extract_list_features(df, ["a","b"], extract=["min", "max", "len"])
-    shape: (3, 6)
-    ┌───────┬───────┬───────┬───────┬───────┬───────┐
-    │ a_min ┆ b_min ┆ a_max ┆ b_max ┆ a_len ┆ b_len │
-    │ ---   ┆ ---   ┆ ---   ┆ ---   ┆ ---   ┆ ---   │
-    │ str   ┆ i64   ┆ str   ┆ i64   ┆ u32   ┆ u32   │
-    ╞═══════╪═══════╪═══════╪═══════╪═══════╪═══════╡
-    │ a     ┆ 1     ┆ a     ┆ 2     ┆ 1     ┆ 2     │
-    │ b     ┆ 3     ┆ b     ┆ 3     ┆ 1     ┆ 2     │
-    │ c     ┆ 4     ┆ c     ┆ 6     ┆ 1     ┆ 3     │
-    └───────┴───────┴───────┴───────┴───────┴───────┘
-    '''
-    _ = type_checker(df, cols, "list", "extract_list_features")
-    exprs = []
-    if isinstance(extract, list):
-        to_extract = extract
-    else:
-        to_extract = [extract]
-    
-    for e in to_extract:
-        if e == "min":
-            exprs.extend(pl.col(c).list.min().suffix("_min") for c in cols)
-        elif e == "max":
-            exprs.extend(pl.col(c).list.max().suffix("_max") for c in cols)
-        elif e in ("mean", "avg"):
-            exprs.extend(pl.col(c).list.mean().suffix("_mean") for c in cols)
-        elif e == "len":
-            exprs.extend(pl.col(c).list.lengths().suffix("_len") for c in cols)
-        elif e == "first":
-            exprs.extend(pl.col(c).list.first().suffix("_first") for c in cols)
-        elif e == "last":
-            exprs.extend(pl.col(c).list.last().suffix("_last") for c in cols)
-        else:
-            logger.info(f"Found {e} in extract, but it is not a valid ListExtract value. Ignored.")
-
-    if isinstance(df, pl.LazyFrame):
-        if drop_original:
-            return df.blueprint.with_columns(exprs).blueprint.drop(cols)
-        return df.blueprint.with_columns(exprs)
-    if drop_original:
-        return df.with_columns(exprs).drop(cols)
-    return df.with_columns(exprs)
-
-def moving_avgs(
-    df:PolarsFrame
-    , c: str
-    , window_sizes:list[int]
-    , min_periods: Optional[int] = None,
-) -> PolarsFrame:
-    '''
-    Computes moving averages for column c with given window_sizes. Please make sure the dataframe is sorted
-    before this. For a pipeline compatible sort, see `dsds.prescreen.order_by`.
-
-    This will be remembered by blueprint by default.
-    
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars dataframe
-    c
-        Name of the column to compute moving averages
-    window_sizes
-        A list of positive integers > 1, representing the different moving average periods for the column c.
-        Everything <= 1 will be ignored
-    min_periods
-        The number of values in the window that should be non-null before computing a result. If None, 
-        it will be set equal to window size.
-    '''
-    exprs = (pl.col(c).rolling_mean(i, min_periods=min_periods).suffix(f"_ma_{i}") 
-             for i in window_sizes if i > 1)
-    if isinstance(df, pl.LazyFrame):
-        return df.blueprint.with_columns(list(exprs))
+from __future__ import annotations
+
+from .type_alias import (
+    PolarsFrame
+    , ImputationStrategy
+    , ScalingStrategy
+    , PowerTransformStrategy
+    , DateExtract
+    , ListExtract
+    , StrExtract
+    , HorizontalExtract
+    , ZeroOneCombineStrategy
+)
+from .prescreen import type_checker
+from .blueprint import( # Need this for Polars extension to work
+    Blueprint  # noqa: F401
+)
+from typing import Optional, Union
+from scipy.stats import (
+    yeojohnson_normmax
+    , boxcox_normmax
+)
+from functools import partial
+import logging
+import math
+# import numpy as np
+import polars as pl
+
+# A lot of companies are still using Python < 3.10
+# So I am not using match statements
+
+logger = logging.getLogger(__name__)
+
+def impute(
+    df:PolarsFrame
+    , cols:list[str]
+    , strategy:ImputationStrategy = 'median'
+    , const:float = 1.
+) -> PolarsFrame:
+    '''
+    Impute the given columns with the given strategy.
+
+    This will be remembered by blueprint by default.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars DataFrame
+    cols
+        The columns to impute
+    strategy
+        One of 'median', 'mean', 'const' or 'mode'. If 'const', the const argument should be provided. Note that
+        if strategy is mode and if two values occur the same number of times, a random one will be picked.
+    const
+        The constant value to impute by if strategy = 'const'
+    '''
+    if strategy == "median":
+        all_medians = df.lazy().select(cols).median().collect().row(0)
+        exprs = (pl.col(c).fill_null(all_medians[i]) for i,c in enumerate(cols))
+    elif strategy in ("mean", "avg", "average"):
+        all_means = df.lazy().select(cols).mean().collect().row(0)
+        exprs = (pl.col(c).fill_null(all_means[i]) for i,c in enumerate(cols))
+    elif strategy in ("const", "constant"):
+        exprs = (pl.col(c).fill_null(const) for c in cols)
+    elif strategy in ("mode", "most_frequent"):
+        all_modes = df.lazy().select(cols).select(pl.all().mode().first()).collect().row(0)
+        exprs = (pl.col(c).fill_null(all_modes[i]) for i,c in enumerate(cols))
+    else:
+        raise TypeError(f"Unknown imputation strategy: {strategy}")
+
+    if isinstance(df, pl.LazyFrame):
+        return df.blueprint.with_columns(list(exprs))
+    return df.with_columns(exprs)
+
+def scale(
+    df:PolarsFrame
+    , cols:list[str]
+    , strategy:ScalingStrategy="standard"
+    , const:float = 1.0
+) -> PolarsFrame:
+    '''
+    Scale the given columns with the given strategy.
+
+    This will be remembered by blueprint by default.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars DataFrame
+    cols
+        The columns to scale
+    strategy
+        One of 'standard', 'min_max', 'const'. If 'const', the const argument should be provided
+    const
+        The constant value to scale by if strategy = 'const'    
+    '''
+    _ = type_checker(df, cols, "numeric", "scale")
+    if strategy == "standard":
+        mean_std = df.lazy().select(cols).select(
+            pl.all().mean().prefix("mean:"),
+            pl.all().std().prefix("std:")
+        ).collect().row(0)
+        exprs = ((pl.col(c) - mean_std[i])/(mean_std[i + len(cols)]) for i,c in enumerate(cols))
+    elif strategy == "min_max":
+        min_max = df.lazy().select(cols).select(
+            pl.all().min().prefix("min:"),
+            pl.all().max().prefix("max:")
+        ).collect().row(0) # All mins come first, then maxs
+        exprs = ((pl.col(c) - min_max[i])/((min_max[i + len(cols)] - min_max[i])) for i,c in enumerate(cols))
+    elif strategy in ("const", "constant"):
+        exprs = (pl.col(c)/const for c in cols)
+    else:
+        raise TypeError(f"Unknown scaling strategy: {strategy}")
+
+    if isinstance(df, pl.LazyFrame):
+        return df.blueprint.with_columns(list(exprs))
+    return df.with_columns(exprs)
+
+def merge_infreq_values(
+    df: PolarsFrame
+    , cols: list[str]
+    , min_count: Optional[int] = 10
+    , min_frac: Optional[float] = None
+    , separator: str = '|'
+) -> PolarsFrame:
+    '''
+    Combines infrequent categories in string columns together.
+
+    This will be remembered by blueprint by default.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars DataFrame
+    cols
+        List of string columns to perform this operation
+    min_count
+        Define a category to be infrequent if it occurs less than min_count. This defaults to 10 if both min_count and 
+        min_frac are None.
+    min_frac
+        Define category to be infrequent if it occurs less than this percentage of times. If both min_count and min_frac
+        are set, min_frac takes priority
+    separator
+        The separator for the new value representing the combined categories
+
+    Example
+    -------
+    >>> import dsds.transform as t
+    ... df = pl.DataFrame({
+    ...     "a":["a", "b", "c", "c", "c", "c", "c", "c", "c", "c", "c", "c", "c", "c"],
+    ...     "b":["a", "b", "c", "d", "d", "d", "d", "d", "d", "d", "d", "d", "d", "d"]
+    ... })
+    >>> df
+    shape: (14, 2)
+    ┌─────┬─────┐
+    │ a   ┆ b   │
+    │ --- ┆ --- │
+    │ str ┆ str │
+    ╞═════╪═════╡
+    │ a   ┆ a   │
+    │ b   ┆ b   │
+    │ c   ┆ c   │
+    │ c   ┆ d   │
+    │ …   ┆ …   │
+    │ c   ┆ d   │
+    │ c   ┆ d   │
+    │ c   ┆ d   │
+    │ c   ┆ d   │
+    └─────┴─────┘
+    >>> t.merge_infreq_values(df, ["a", "b"], min_count=3)
+    shape: (14, 2)
+    ┌─────┬───────┐
+    │ a   ┆ b     │
+    │ --- ┆ ---   │
+    │ str ┆ str   │
+    ╞═════╪═══════╡
+    │ a|b ┆ a|c|b │
+    │ a|b ┆ a|c|b │
+    │ c   ┆ a|c|b │
+    │ c   ┆ d     │
+    │ …   ┆ …     │
+    │ c   ┆ d     │
+    │ c   ┆ d     │
+    │ c   ┆ d     │
+    │ c   ┆ d     │
+    └─────┴───────┘
+    '''
+    _ = type_checker(df, cols, "string", "merge_infreq_values")
+    if min_frac is None:
+        if min_count is None:
+            comp = pl.col("count") < 10
+        else:
+            comp = pl.col("count") < min_count
+    else:
+        comp = pl.col("count")/pl.col("count").sum() < min_frac
+
+    exprs = []
+    for c in cols:
+        infreq = df.lazy().groupby(c).count().filter(
+            comp
+        ).collect()[c]
+        value = separator.join(infreq)
+        exprs.append(
+            pl.when(pl.col(c).is_in(infreq)).then(value).otherwise(pl.col(c)).alias(c)
+        )
+    
+    if isinstance(df, pl.LazyFrame):
+        return df.blueprint.with_columns(exprs)
+    return df.with_columns(exprs)
+
+def combine_zero_ones(
+    df: PolarsFrame
+    , cols: list[str]
+    , new_name: str
+    , rule: ZeroOneCombineStrategy = "union"
+    , drop_original:bool = True
+) -> PolarsFrame:
+    '''
+    Take columns that are all binary 0, 1 columns, combine them according to the rule. Please make sure 
+    the columns only contain binary 0s and 1s. Depending on the rule, this can be used, for example, to 
+    quickly combine many one hot encoded columns into one, or reducing the same binary columns into one.
+
+    This will be remembered by blueprint by default.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars DataFrame
+    cols
+        List of binary 0, 1 columns to combine
+    new_name
+        Name for the combined column
+    rule
+        One of 'union', 'intersection', 'same'.
+    drop_original
+        If true, drop column in cols
+
+    Examples
+    --------
+    >>> import dsds.transform as t
+    ... df = pl.DataFrame({
+    ...     "a": [1, 1, 0],
+    ...     "b":[1, 0, 1],
+    ...     "c":[1, 1, 1]
+    ... })
+    >>> t.combine_zero_ones(df, cols=["a", "b", "c"], new_name="abc", rule="same")
+    shape: (3, 1)
+    ┌─────┐
+    │ abc │
+    │ --- │
+    │ u8  │
+    ╞═════╡
+    │ 1   │
+    │ 0   │
+    │ 0   │
+    └─────┘
+    >>> t.combine_zero_ones(df, cols=["a", "b", "c"], new_name="abc", rule="union")
+    shape: (3, 1)
+    ┌─────┐
+    │ abc │
+    │ --- │
+    │ u8  │
+    ╞═════╡
+    │ 1   │
+    │ 1   │
+    │ 1   │
+    └─────┘
+    '''
+    if rule == "union":
+        expr = pl.max_horizontal([pl.col(c) for c in cols]).cast(pl.UInt8).alias(new_name)
+    elif rule == "intersection":
+        expr = pl.min_horizontal([pl.col(c) for c in cols]).cast(pl.UInt8).alias(new_name)
+    elif rule == "same":
+        expr = pl.when(sum(pl.col(c) for c in cols).is_in((0, len(cols)))).then(
+                    pl.lit(1, dtype=pl.UInt8)
+                ).otherwise(
+                    pl.lit(0, dtype=pl.UInt8)
+                ).alias(new_name)
+    else:
+        raise TypeError(f"The input `{rule}` is not a valid ZeroOneCombineStrategy.")
+
+    if isinstance(df, pl.LazyFrame):
+        if drop_original:
+            return df.blueprint.with_columns(expr).blueprint.drop(cols)
+        return df.blueprint.with_columns(expr)
+    if drop_original:
+        return df.with_columns(expr).drop(cols)
+    return df.with_columns(expr)
+
+def power_transform(
+    df: PolarsFrame
+    , cols: list[str]
+    , strategy: PowerTransformStrategy = "yeo_johnson"
+    # , lmbda: Optional[float] = None
+) -> PolarsFrame:
+    '''
+    Performs power transform on the numerical columns. This will skip null values in the columns. If strategy is
+    box_cox, all values in cols must be positive.
+
+    This will be remembered by blueprint by default.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars dataframe
+    cols
+        Must be explicitly provided and must all be numerical
+    strategy
+        Either 'yeo_johnson' or 'box_cox'
+    '''
+    _ = type_checker(df, cols, "numeric", "power_transform")
+    exprs:list[pl.Expr] = []
+    if strategy in ("yeo_johnson", "yeojohnson"):
+        lmaxs = df.lazy().select(cols).groupby(pl.lit(1)).agg(
+            pl.col(c)
+            .apply(yeojohnson_normmax, strategy="threading", return_dtype=pl.Float64).alias(c)
+            for c in cols
+        ).select(cols).collect().row(0)
+        for c, lmax in zip(cols, lmaxs):
+            if lmax == 0: # log(x + 1)
+                x_ge_0_sub_expr = (pl.col(c).add(1)).log()
+            else: # ((x + 1)**lmbda - 1) / lmbda
+                x_ge_0_sub_expr = ((pl.col(c).add(1)).pow(lmax) - 1) / lmax
+
+            if lmax == 2: # -log(-x + 1)
+                x_lt_0_sub_expr = pl.lit(-1) * (1 - pl.col(c)).log()
+            else: #  -((-x + 1)**(2 - lmbda) - 1) / (2 - lmbda)
+                t = 2 - lmax
+                x_lt_0_sub_expr = pl.lit(-1/t) * ((1 - pl.col(c)).pow(t) - 1)
+
+            exprs.append(
+                pl.when(pl.col(c).ge(0)).then(x_ge_0_sub_expr).otherwise(x_lt_0_sub_expr).alias(c)
+            )
+    elif strategy in ("box_cox", "boxcox"):
+        bc_normmax = partial(boxcox_normmax, method="mle")
+        lmaxs = df.lazy().select(cols).groupby(pl.lit(1)).agg(
+            pl.col(c)
+            .apply(bc_normmax, strategy="threading", return_dtype=pl.Float64).alias(c)
+            for c in cols
+        ).select(cols).collect().row(0)
+        exprs.extend(
+            pl.col(c).log() if lmax == 0 else (pl.col(c).pow(lmax) - 1) / lmax 
+            for c, lmax in zip(cols, lmaxs)
+        )
+    else:
+        raise TypeError(f"The input strategy {strategy} is not a valid strategy. Valid strategies are: yeo_johnson "
+                        "or box_cox")
+    
+    if isinstance(df, pl.LazyFrame):
+        return df.blueprint.with_columns(exprs)
+    return df.with_columns(exprs)
+
+def normalize(
+    df: PolarsFrame
+    , cols:list[str]
+) -> PolarsFrame:
+    '''
+    Normalize the given columns by dividing them with the respective column sum.
+
+    !!! Note this will NOT be remembered by the blueprint !!!
+
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars dataframe
+    cols
+        Must be explicitly provided and should all be numeric columns
+    '''
+    _ = type_checker(df, cols, "numeric", "normalize")
+    return df.with_columns(pl.col(c)/pl.col(c).sum() for c in cols)
+
+def clip(
+    df: PolarsFrame
+    , cols: list[str]
+    , min_clip: Optional[float] = None
+    , max_clip: Optional[float] = None
+) -> PolarsFrame:
+    '''
+    Clips the columns within the min and max_clip bounds. This can be used to control outliers. If both min_clip and
+    max_clip are provided, perform two-sided clipping. If only one bound is provided, only one side will be clipped.
+    It will throw an error if both min and max_clips are not provided.
+
+    This will be remembered by blueprint by default.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars dataframe
+    cols
+        Must be explicitly provided and should all be numeric columns
+    min_clip
+        Every value smaller than min_clip will be replaced by min_cap
+    max_clip
+        Every value bigger than max_clip will be replaced by max_cap
+    '''
+    _ = type_checker(df, cols, "numeric", "clip")
+    a:bool = min_clip is None
+    b:bool = max_clip is None
+    if a & (not b):
+        exprs = (pl.col(c).clip_max(max_clip) for c in cols)
+    elif (not a) & b:
+        exprs = (pl.col(c).clip_min(min_clip) for c in cols)
+    elif not (a | b):
+        exprs = (pl.col(c).clip(min_clip, max_clip) for c in cols)
+    else:
+        raise ValueError("At least one of min_cap and max_cap should be provided.")
+    
+    if isinstance(df, pl.LazyFrame):
+        return df.blueprint.with_columns(list(exprs))
+    return df.with_columns(exprs)
+
+def log_transform(
+    df: PolarsFrame
+    , cols:list[str]
+    , base:float = math.e
+    , plus_one:bool = False
+    , suffix:str = "_log"
+) -> PolarsFrame:
+    '''
+    Performs classical log transform on the given columns, e.g. log(x), or if plus_one = True, ln(1 + x).
+    
+    Important: If input to log is <= 0, (in the case plus_one = True, if 1 + x <= 0), then result will be NaN. 
+    Some algorithms may break if there exists NaN in the columns. Users should perform their due diligence before 
+    calling the log transform.
+
+    This will be remembered by blueprint by default.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars dataframe
+    cols
+        Must be explicitly provided and should all be numeric columns
+    base
+        Base of log. Default is math.e
+    plus_one
+        If plus_one is true, this will perform ln(1+x) and ignore the `base` input.
+    suffix
+        Choice of a suffix to the transformed columns. If this is the empty string "", then the original column
+        will be replaced, except when plus_one = True, in which case the suffix will always be "_log1p". In that
+        case, please use a `dsds.prescreen.drop` step if you want the original columns to be dropped.
+    '''
+    _ = type_checker(df, cols, "numeric", "log_transform")
+    if plus_one:
+        exprs = [pl.col(c).log1p().suffix("_log1p") for c in cols]
+    else:
+        exprs = [pl.col(c).log(base).suffix(suffix) for c in cols]
+    if isinstance(df, pl.LazyFrame):
+        return df.blueprint.with_columns(exprs)
+    return df.with_columns(exprs)
+
+def extract_dt_features(
+    df: PolarsFrame
+    , cols: list[str]
+    , extract: Union[DateExtract, list[DateExtract]] = ["year", "quarter", "month"]
+    , sunday_first: bool = False
+    , drop_original: bool = True
+) -> PolarsFrame:
+    '''
+    Extracts additional date related features from existing date/datetime columns.
+
+    This will be remembered by blueprint by default.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars dataframe
+    cols
+        Must be explicitly provided and should all be date/datetime columns
+    extract
+        One of "year", "quarter", "month", "week", "day_of_week", "day_of_year", or a list of these values 
+        such as ["year", "quarter"], which means extract year and quarter from all the columns provided 
+    sunday_first
+        For day_of_week, by default, Monday maps to 1, and so on. If sunday_first = True, then Sunday will be
+        mapped to 1 and so on
+    drop_original
+        Whether to drop columns in cols
+
+    Example
+    -------
+    >>> import dsds.transform as t
+    ... df = pl.DataFrame({
+    ...     "date1":["2021-01-01", "2022-02-03", "2023-11-23"]
+    ...     , "date2":["2021-01-01", "2022-02-03", "2023-11-23"]
+    ... }).with_columns(
+    ...     pl.col(c).str.to_date() for c in ["date1", "date2"]
+    ... )
+    >>> print(df)
+    shape: (3, 2)
+    ┌────────────┬────────────┐
+    │ date1      ┆ date2      │
+    │ ---        ┆ ---        │
+    │ date       ┆ date       │
+    ╞════════════╪════════════╡
+    │ 2021-01-01 ┆ 2021-01-01 │
+    │ 2022-02-03 ┆ 2022-02-03 │
+    │ 2023-11-23 ┆ 2023-11-23 │
+    └────────────┴────────────┘
+    >>> cols = ["date1", "date2"]
+    >>> print(t.extract_dt_features(df, cols=cols, drop_original=False))
+    shape: (3, 8)
+    ┌────────────┬────────────┬────────────┬───────────┬───────────┬───────────┬───────────┬───────────┐
+    │ date1      ┆ date2      ┆ date1_year ┆ date2_yea ┆ date1_qua ┆ date2_qua ┆ date1_mon ┆ date2_mon │
+    │ ---        ┆ ---        ┆ ---        ┆ r         ┆ rter      ┆ rter      ┆ th        ┆ th        │
+    │ date       ┆ date       ┆ u32        ┆ ---       ┆ ---       ┆ ---       ┆ ---       ┆ ---       │
+    │            ┆            ┆            ┆ u32       ┆ u32       ┆ u32       ┆ u32       ┆ u32       │
+    ╞════════════╪════════════╪════════════╪═══════════╪═══════════╪═══════════╪═══════════╪═══════════╡
+    │ 2021-01-01 ┆ 2021-01-01 ┆ 2021       ┆ 2021      ┆ 1         ┆ 1         ┆ 1         ┆ 1         │
+    │ 2022-02-03 ┆ 2022-02-03 ┆ 2022       ┆ 2022      ┆ 1         ┆ 1         ┆ 2         ┆ 2         │
+    │ 2023-11-23 ┆ 2023-11-23 ┆ 2023       ┆ 2023      ┆ 4         ┆ 4         ┆ 11        ┆ 11        │
+    └────────────┴────────────┴────────────┴───────────┴───────────┴───────────┴───────────┴───────────┘
+    '''
+    _ = type_checker(df, cols, "datetime", "extract_dt_features")
+    exprs = []
+    if isinstance(extract, list):
+        to_extract = extract
+    else:
+        to_extract = [extract]
+    
+    for e in to_extract:
+        if e == "month":
+            exprs.extend(pl.col(c).dt.month().suffix("_month") for c in cols)
+        elif e == "year":
+            exprs.extend(pl.col(c).dt.year().suffix("_year") for c in cols)
+        elif e == "quarter":
+            exprs.extend(pl.col(c).dt.quarter().suffix("_quarter") for c in cols)
+        elif e == "week":
+            exprs.extend(pl.col(c).dt.week().suffix("_week") for c in cols)
+        elif e == "day_of_week":
+            if sunday_first:
+                exprs.extend(
+                    pl.when(pl.col(c).dt.weekday() == 7).then(1).otherwise(pl.col(c).dt.weekday()+1)
+                    .suffix("_day_of_week") 
+                    for c in cols
+                )
+            else:
+                exprs.extend(pl.col(c).dt.weekday().suffix("_day_of_week") for c in cols)
+        elif e == "day_of_year":
+            exprs.extend(pl.col(c).dt.ordinal_day().suffix("_day_of_year") for c in cols)
+        else:
+            logger.info(f"Found {e} in extract, but it is not a valid DateExtract value. Ignored.")
+
+    if isinstance(df, pl.LazyFrame):
+        if drop_original:
+            return df.blueprint.with_columns(exprs).blueprint.drop(cols)
+        return df.blueprint.with_columns(exprs)
+    if drop_original:
+        return df.with_columns(exprs).drop(cols)
+    return df.with_columns(exprs)
+    
+def extract_horizontally(
+    df:PolarsFrame
+    , cols: list[str]
+    , extract: Union[HorizontalExtract, list[HorizontalExtract]] = ["min", "max"]
+    , drop_original: bool = True
+) -> PolarsFrame:
+    '''
+    Extract features horizontally across a few columns.
+
+    This will be remembered by blueprint by default.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars dataframe
+    cols
+        List of columns to extract feature from
+    extract
+        One of "min", "max", "sum", "any", "all". Note that "any" and "all" only make practical sense when 
+        all of cols are boolean columns, but they work even when cols are numbers.
+    drop_original
+        Whether to drop columns in cols
+
+    Example
+    -------
+    >>> import dsds.transform as t
+    ... df = pl.DataFrame({
+    ...     "a":[1, 2, 3],
+    ...     "b":[1, 2, 3],
+    ...     "c":[1, 2, 3]
+    ... })
+    >>> t.extract_horizontally(df, cols=["a", "b", "c"], extract=["min", "max", "sum"])
+    shape: (3, 3)
+    ┌────────────┬────────────┬────────────┐
+    │ min(a,b,c) ┆ max(a,b,c) ┆ sum(a,b,c) │
+    │ ---        ┆ ---        ┆ ---        │
+    │ i64        ┆ i64        ┆ i64        │
+    ╞════════════╪════════════╪════════════╡
+    │ 1          ┆ 1          ┆ 3          │
+    │ 2          ┆ 2          ┆ 6          │
+    │ 3          ┆ 3          ┆ 9          │
+    └────────────┴────────────┴────────────┘
+    '''
+    if isinstance(extract, list):
+        to_extract = extract
+    else:
+        to_extract = [extract]
+    
+    exprs = []
+    for e in to_extract:
+        alias = f"{e}({','.join(cols)})"
+        if e == "min":
+            exprs.append(pl.min_horizontal([pl.col(c) for c in cols]).alias(alias))
+        elif e == "max":
+            exprs.append(pl.max_horizontal([pl.col(c) for c in cols]).alias(alias))
+        elif e == "sum":
+            exprs.append(pl.sum_horizontal([pl.col(c) for c in cols]).alias(alias))
+        elif e == "any":
+            exprs.append(pl.any_horizontal([pl.col(c) for c in cols]).alias(alias))
+        elif e == "all":
+            exprs.append(pl.all_horizontal([pl.col(c) for c in cols]).alias(alias))
+        else:
+            logger.info(f"Found {e} in extract, but it is not a valid HorizontalExtract value. Ignored.")
+
+    if isinstance(df, pl.LazyFrame):
+        if drop_original:
+            return df.blueprint.with_columns(exprs).blueprint.drop(cols)
+        return df.blueprint.with_columns(exprs)
+    if drop_original:
+        return df.with_columns(exprs).drop(cols)
+    return df.with_columns(exprs)
+
+def extract_word_count(
+    df: PolarsFrame
+    , cols: Union[str, list[str]]
+    , words: list[str]
+    , lower: bool = True
+    , drop_original: bool = True
+) -> PolarsFrame:
+    '''
+    Extract word counts from the cols.
+
+    This will be remembered by blueprint by default.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars dataframe
+    cols
+        Either a string representing a name of a column, or a list of column names.
+    words
+        Words/Patterns to count
+    lower
+        Whether a lowercase() step should be done before the count match
+    drop_original
+        Whether to drop columns in cols
+
+    Example
+    -------
+    >>> import dsds.transform as t
+    ... df = pl.DataFrame({
+    ...     "test_str": ["hello world hello", "hello Tom", "test", "world hello"],
+    ...     "test_str2": ["hello world hello", "hello Tom", "test", "world hello"]
+    ... })
+    >>> t.extract_word_count(df, cols=["test_str", "test_str2"], words=["hello", "world"])
+    shape: (4, 4)
+    ┌──────────────────────┬──────────────────────┬───────────────────────┬───────────────────────┐
+    │ test_str_count_hello ┆ test_str_count_world ┆ test_str2_count_hello ┆ test_str2_count_world │
+    │ ---                  ┆ ---                  ┆ ---                   ┆ ---                   │
+    │ u32                  ┆ u32                  ┆ u32                   ┆ u32                   │
+    ╞══════════════════════╪══════════════════════╪═══════════════════════╪═══════════════════════╡
+    │ 2                    ┆ 1                    ┆ 2                     ┆ 1                     │
+    │ 1                    ┆ 0                    ┆ 1                     ┆ 0                     │
+    │ 0                    ┆ 0                    ┆ 0                     ┆ 0                     │
+    │ 1                    ┆ 1                    ┆ 1                     ┆ 1                     │
+    └──────────────────────┴──────────────────────┴───────────────────────┴───────────────────────┘
+    '''
+    if isinstance(cols, str):
+        str_cols = [cols]
+    else:
+        str_cols = cols
+
+    _ = type_checker(df, str_cols, "string", "extract_word_count")
+    exprs = []
+    if lower:
+        for c in str_cols:
+            exprs.extend(pl.col(c).str.to_lowercase().str.count_match(w).suffix(f"_count_{w}") for w in words)
+    else:
+        for c in str_cols:
+            exprs.extend(pl.col(c).str.count_match(w).suffix(f"_count_{w}") for w in words)
+
+    if isinstance(df, pl.LazyFrame):
+        if drop_original:
+            return df.blueprint.with_columns(exprs).blueprint.drop(cols)
+        return df.blueprint.with_columns(exprs)
+    if drop_original:
+        return df.with_columns(exprs).drop(cols)
+    return df.with_columns(exprs)
+
+def extract_from_str(
+    df: PolarsFrame
+    , cols: list[str]
+    , extract: Union[StrExtract, list[StrExtract]]
+    , pattern: Optional[str] = None
+    , use_bool: bool = False
+    , drop_original: bool = True
+) -> PolarsFrame:
+    '''
+    Extract data from string columns. For multiple word counts on the same column, see extract_word_count.
+    Note that for 'starts_with' and 'ends_with', pattern will be used as a substring instead of a regex pattern.
+
+    This will be remembered by blueprint by default.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars dataframe
+    cols
+        Must be explicitly provided and should all be string columns
+    extract
+        One of "count", "len", "contains", "starts_with", "ends_with" or a list of these values such as 
+        ["len", "starts_with"]. If non-"len" extract type is provided, pattern must not be None.
+    pattern
+        The pattern for every non-"len" extract.
+    use_bool
+        If true, results of "starts_with", "ends_with", and "contains" will be boolean columns instead of binary
+        0s and 1s.
+    drop_original
+        Whether to drop columns in cols
+
+    Example
+    -------
+    >>> import dsds.transform as t
+    ... df = pl.DataFrame({
+    ...     "test_str": ["a_1", "x_2", "c_3", "x_22"]
+    ... })
+    >>> t.extract_from_str(df, cols=["test_str"], extract=["len", "contains"], pattern="^(a_|x_)")
+    shape: (4, 2)
+    ┌──────────────┬───────────────────────────┐
+    │ test_str_len ┆ test_str_contains_(a_|x_) │
+    │ ---          ┆ ---                       │
+    │ u32          ┆ u8                        │
+    ╞══════════════╪═══════════════════════════╡
+    │ 3            ┆ 1                         │
+    │ 3            ┆ 1                         │
+    │ 3            ┆ 0                         │
+    │ 4            ┆ 1                         │
+    └──────────────┴───────────────────────────┘
+    '''    
+    _ = type_checker(df, cols, "string", "extract_from_str")
+    if isinstance(extract, list):
+        to_extract = extract
+    else:
+        to_extract = [extract]
+    
+    if (len(to_extract) > 1 or (len(to_extract) == 1 and to_extract[0] != 'len')) and pattern is None:
+        raise ValueError("The argument `pattern` has to be supplied when extract contains non-'len' types.")
+    
+    exprs = []
+    for e in to_extract:
+        if e == "len":
+            exprs.extend(pl.col(c).str.lengths().suffix("_len") for c in cols)
+        elif e == "starts_with":
+            if use_bool:
+                exprs.extend(pl.col(c).str.starts_with(pattern).suffix(f"_starts_with_{pattern}") 
+                            for c in cols)
+            else:
+                exprs.extend(pl.col(c).str.starts_with(pattern).cast(pl.UInt8).suffix(f"_starts_with_{pattern}") 
+                            for c in cols)
+        elif e == "ends_with":
+            if use_bool:
+                exprs.extend(pl.col(c).str.ends_with(pattern).suffix(f"_ends_with_{pattern}")
+                            for c in cols)
+            else:
+                exprs.extend(pl.col(c).str.ends_with(pattern).cast(pl.UInt8).suffix(f"_ends_with_{pattern}") 
+                            for c in cols)
+        elif e == "count":
+            exprs.extend(pl.col(c).str.count_match(pattern).suffix(f"_{pattern}_count") for c in cols)
+        elif e == "contains":
+            if use_bool:
+                exprs.extend(pl.col(c).str.contains(pattern).suffix(f"_contains_{pattern}") 
+                            for c in cols)
+            else:
+                exprs.extend(pl.col(c).str.contains(pattern).cast(pl.UInt8).suffix(f"_contains_{pattern}") 
+                            for c in cols)
+        else:
+            logger.info(f"Found {e} in extract, but it is not a valid StrExtract value. Ignored.")
+
+    if isinstance(df, pl.LazyFrame):
+        if drop_original:
+            return df.blueprint.with_columns(exprs).blueprint.drop(cols)
+        return df.blueprint.with_columns(exprs)
+    if drop_original:
+        return df.with_columns(exprs).drop(cols)
+    return df.with_columns(exprs)
+
+def extract_list_features(
+    df: PolarsFrame
+    , cols: list[str]
+    , extract: Union[ListExtract, list[ListExtract]] = ["min", "max"]
+    , drop_original: bool = True
+) -> PolarsFrame:
+    '''
+    Extract data from columns that contains lists.
+
+    This will be remembered by blueprint by default.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars dataframe
+    cols
+        Must be explicitly provided and should all be date/datetime columns
+    extract
+        One of "min", "max", "mean", "len", "first", "last" or a list of these values such as ["min", "max"], 
+        which means extract min and max from all the columns provided. Notice if mean is provided, then the 
+        column must be list of numbers.
+    drop_original
+        Whether to drop columns in cols
+
+    Example
+    -------
+    >>> import dsds.transform as t
+    ... df = pl.DataFrame({
+    ...     "a":[["a"],["b"], ["c"]],
+    ...     "b":[[1,2], [3,3], [4,5,6]]
+    ... })
+    >>> t.extract_list_features(df, ["a","b"], extract=["min", "max", "len"])
+    shape: (3, 6)
+    ┌───────┬───────┬───────┬───────┬───────┬───────┐
+    │ a_min ┆ b_min ┆ a_max ┆ b_max ┆ a_len ┆ b_len │
+    │ ---   ┆ ---   ┆ ---   ┆ ---   ┆ ---   ┆ ---   │
+    │ str   ┆ i64   ┆ str   ┆ i64   ┆ u32   ┆ u32   │
+    ╞═══════╪═══════╪═══════╪═══════╪═══════╪═══════╡
+    │ a     ┆ 1     ┆ a     ┆ 2     ┆ 1     ┆ 2     │
+    │ b     ┆ 3     ┆ b     ┆ 3     ┆ 1     ┆ 2     │
+    │ c     ┆ 4     ┆ c     ┆ 6     ┆ 1     ┆ 3     │
+    └───────┴───────┴───────┴───────┴───────┴───────┘
+    '''
+    _ = type_checker(df, cols, "list", "extract_list_features")
+    exprs = []
+    if isinstance(extract, list):
+        to_extract = extract
+    else:
+        to_extract = [extract]
+    
+    for e in to_extract:
+        if e == "min":
+            exprs.extend(pl.col(c).list.min().suffix("_min") for c in cols)
+        elif e == "max":
+            exprs.extend(pl.col(c).list.max().suffix("_max") for c in cols)
+        elif e in ("mean", "avg"):
+            exprs.extend(pl.col(c).list.mean().suffix("_mean") for c in cols)
+        elif e == "len":
+            exprs.extend(pl.col(c).list.lengths().suffix("_len") for c in cols)
+        elif e == "first":
+            exprs.extend(pl.col(c).list.first().suffix("_first") for c in cols)
+        elif e == "last":
+            exprs.extend(pl.col(c).list.last().suffix("_last") for c in cols)
+        else:
+            logger.info(f"Found {e} in extract, but it is not a valid ListExtract value. Ignored.")
+
+    if isinstance(df, pl.LazyFrame):
+        if drop_original:
+            return df.blueprint.with_columns(exprs).blueprint.drop(cols)
+        return df.blueprint.with_columns(exprs)
+    if drop_original:
+        return df.with_columns(exprs).drop(cols)
+    return df.with_columns(exprs)
+
+def moving_avgs(
+    df:PolarsFrame
+    , c: str
+    , window_sizes:list[int]
+    , min_periods: Optional[int] = None,
+) -> PolarsFrame:
+    '''
+    Computes moving averages for column c with given window_sizes. Please make sure the dataframe is sorted
+    before this. For a pipeline compatible sort, see `dsds.prescreen.order_by`.
+
+    This will be remembered by blueprint by default.
+    
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars dataframe
+    c
+        Name of the column to compute moving averages
+    window_sizes
+        A list of positive integers > 1, representing the different moving average periods for the column c.
+        Everything <= 1 will be ignored
+    min_periods
+        The number of values in the window that should be non-null before computing a result. If None, 
+        it will be set equal to window size.
+    '''
+    exprs = [pl.col(c).rolling_mean(i, min_periods=min_periods).suffix(f"_ma_{i}") 
+             for i in window_sizes if i > 1]
+    if isinstance(df, pl.LazyFrame):
+        return df.blueprint.with_columns(exprs)
     return df.with_columns(exprs)
```

### Comparing `dsds-0.0.24/src/dsds/type_alias.py` & `dsds-0.0.25/python/dsds/type_alias.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,86 +1,92 @@
-from typing import (
-    Literal
-    , Final
-    , Tuple
-    , Union
-    , Callable
-)
-from abc import ABC, abstractmethod
-import polars as pl
-import sys
-if sys.version_info >= (3, 10):
-    from typing import TypeAlias, Concatenate, ParamSpec
-    P = ParamSpec('P')
-    PolarsFrame:TypeAlias = Union[pl.DataFrame, pl.LazyFrame]
-    PipeFunction = Callable[Concatenate[PolarsFrame, P], PolarsFrame]
-else: # 3.9
-    from typing_extensions import TypeAlias
-    PolarsFrame:TypeAlias = Union[pl.DataFrame, pl.LazyFrame]
-    PipeFunction = Callable
-
-import os
-import numpy as np
-
-# --- Constants ---
-CPU_COUNT:Final[int] = os.cpu_count()
-CPU_M1: Final[int] = CPU_COUNT - 1
-POLARS_NUMERICAL_TYPES:Final[Tuple[pl.DataType]] = (pl.UInt8, pl.UInt16, pl.UInt32, pl.UInt64, pl.Float32, pl.Float64
-                                                    , pl.Int8, pl.Int16, pl.Int32, pl.Int64)
-POLARS_DATETIME_TYPES:Final[Tuple[pl.DataType]] = (pl.Datetime, pl.Date)
-
-# --- Strategies ---
-MRMRStrategy:TypeAlias = Literal["fscore", "f", "f_score", "xgb", "xgboost", "rf", "random_forest", "mis"
-                                , "mutual_info_score", "lgbm", "lightgbm"]
-ScalingStrategy:TypeAlias = Literal["standard", "min_max", "const", "constant"]
-ImputationStrategy:TypeAlias = Literal["mean", "avg", "average", "median", "const", "constant", "mode", "most_frequent"]
-PowerTransformStrategy:TypeAlias = Literal["yeo_johnson", "yeojohnson", "box_cox", "boxcox"]
-
-# --- Models ---
-BinaryModels:TypeAlias = Literal["logistic", "lr", "lightgbm", "lgbm", "xgboost", "xgb", "random_forest", "rf"]
-
-# --- Extracts ---
-DateExtract:TypeAlias = Literal["year", "quarter", "month", "week", "day_of_week", "day_of_year"]
-ListExtract:TypeAlias = Literal["min", "max", "mean", "len", "first", "last"]
-HorizontalExtract:TypeAlias = Literal["min", "max", "sum", "any", "all"]
-
-# --- Stats Related ---
-Alternatives = Literal["two-sided", "greater", "less"]
-# This is just a subset of Scipy.stats's distributions which can be named by strings. 
-# All scipy.stats's string-name-able distributions should work when the arguments asks 
-# for a CommonContinuousDist.
-CommonContiDist:TypeAlias = Literal["norm", "lognorm", "truncnorm", "uniform", "t", "beta", "cauchy", "expon", "gamma"]
-
-# --- Other ---
-ZeroOneCombineRules = Literal["union", "intersection", "same"]
-SimpleDtypes:TypeAlias = Literal["numeric", "datetime", "bool", "string", "other/unknown"]
-ActionType:TypeAlias = Literal["with_columns", "map_dict", "drop", "select", "add_func", "filter", "classif"
-                               , "regression"]
-
-# --- Utils ---
-def clean_strategy_str(s:str):
-    '''Strategy strings will only have _, no -, and all lowercase.'''
-    return s.strip().replace("-", "_").lower()
-
-# --- ABC ---
-class ClassifModel(ABC):
-
-    @abstractmethod
-    def predict(self, X:Union[np.ndarray,pl.DataFrame]) -> np.ndarray:
-        ...
-
-    @abstractmethod
-    def predict_proba(self, X: Union[np.ndarray,pl.DataFrame]) -> np.ndarray:
-        ...
-
-    @abstractmethod
-    def fit(self, X:Union[np.ndarray,pl.DataFrame], y:Union[np.ndarray,pl.Series,pl.DataFrame]): # Should return self
-        ...
-    
-class RegressionModel(ABC):
-    @abstractmethod
-    def predict(self, X: Union[np.ndarray,pl.DataFrame]) -> np.ndarray:
-        ...
-
-    @abstractmethod
-    def fit(self, X:Union[np.ndarray,pl.DataFrame], y:Union[np.ndarray,pl.Series,pl.DataFrame]): # Should return self
+from typing import (
+    Literal
+    , Final
+    , Tuple
+    , Union
+    , Callable
+)
+from abc import ABC, abstractmethod
+import polars as pl
+import sys
+if sys.version_info >= (3, 10):
+    from typing import TypeAlias, Concatenate, ParamSpec
+    P = ParamSpec('P')
+    PolarsFrame:TypeAlias = Union[pl.DataFrame, pl.LazyFrame]
+    PipeFunction = Callable[Concatenate[PolarsFrame, P], PolarsFrame]
+else: # 3.9
+    from typing_extensions import TypeAlias
+    PolarsFrame:TypeAlias = Union[pl.DataFrame, pl.LazyFrame]
+    PipeFunction = Callable
+
+import os
+import numpy as np
+
+# --- Constants ---
+CPU_COUNT:Final[int] = os.cpu_count()
+CPU_M1: Final[int] = CPU_COUNT - 1
+POLARS_NUMERICAL_TYPES:Final[Tuple[pl.DataType]] = (pl.UInt8, pl.UInt16, pl.UInt32, pl.UInt64, pl.Float32, pl.Float64
+                                                    , pl.Int8, pl.Int16, pl.Int32, pl.Int64)
+POLARS_DATETIME_TYPES:Final[Tuple[pl.DataType]] = (pl.Datetime, pl.Date)
+
+# --- Strategies ---
+MRMRStrategy:TypeAlias = Literal["fscore", "f", "f_score", "xgb", "xgboost", "rf", "random_forest", "mis"
+                                , "mutual_info_score", "lgbm", "lightgbm"]
+ScalingStrategy:TypeAlias = Literal["standard", "min_max", "const", "constant"]
+ImputationStrategy:TypeAlias = Literal["mean", "avg", "average", "median", "const", "constant", "mode", "most_frequent"]
+PowerTransformStrategy:TypeAlias = Literal["yeo_johnson", "yeojohnson", "box_cox", "boxcox"]
+WeightStrategy: TypeAlias = Literal["none", "balanced", "custom"]
+ZeroOneCombineStrategy = Literal["union", "intersection", "same"]
+
+# --- Models ---
+BinaryModels:TypeAlias = Literal["logistic", "lr", "lightgbm", "lgbm", "xgboost", "xgb", "random_forest", "rf"]
+
+# --- Extracts ---
+DateExtract:TypeAlias = Literal["year", "quarter", "month", "week", "day_of_week", "day_of_year"]
+ListExtract:TypeAlias = Literal["min", "max", "mean", "len", "first", "last"]
+HorizontalExtract:TypeAlias = Literal["min", "max", "sum", "any", "all"]
+StrExtract: TypeAlias = Literal["count", "len", "contains", "starts_with", "ends_with"]
+
+# --- Stats Related ---
+Alternatives = Literal["two-sided", "greater", "less"]
+# This is just a subset of Scipy.stats's distributions which can be named by strings. 
+# All scipy.stats's string-name-able distributions should work when the arguments asks 
+# for a CommonContinuousDist.
+CommonContiDist:TypeAlias = Literal["norm", "lognorm", "truncnorm", "uniform", "t", "beta", "cauchy", "expon", "gamma"]
+
+# --- Blueprint ---
+ActionType:TypeAlias = Literal["with_columns", "map_dict", "select", "drop", "add_func", "filter", "classif"
+                               , "regression"]
+# --- Other ---
+SimpleDtypes:TypeAlias = Literal["numeric", "datetime", "bool", "list", "string", "other/unknown"]
+InnerDtypes:TypeAlias = Literal["int", "str"]
+Stemmer:TypeAlias = Literal["snowball", ""]
+
+
+# --- Utils ---
+def clean_strategy_str(s:str):
+    '''Strategy strings will only have _, no -, and all lowercase.'''
+    return s.strip().replace("-", "_").lower()
+
+# --- ABC ---
+class ClassifModel(ABC):
+
+    @abstractmethod
+    def predict(self, X:Union[np.ndarray,pl.DataFrame]) -> np.ndarray:
+        ...
+
+    @abstractmethod
+    def predict_proba(self, X: Union[np.ndarray,pl.DataFrame]) -> np.ndarray:
+        ...
+
+    @abstractmethod
+    def fit(self, X:Union[np.ndarray,pl.DataFrame], y:Union[np.ndarray,pl.Series,pl.DataFrame]): # Should return self
+        ...
+    
+class RegressionModel(ABC):
+    @abstractmethod
+    def predict(self, X: Union[np.ndarray,pl.DataFrame]) -> np.ndarray:
+        ...
+
+    @abstractmethod
+    def fit(self, X:Union[np.ndarray,pl.DataFrame], y:Union[np.ndarray,pl.Series,pl.DataFrame]): # Should return self
         ...
```

### Comparing `dsds-0.0.24/src/dsds/utils.py` & `dsds-0.0.25/python/dsds/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,403 +1,401 @@
-from scipy.special import expit
-from typing import Optional, Union
-from .blueprint import Blueprint
-from dataclasses import dataclass
-from pathlib import Path
-from .type_alias import (
-    PolarsFrame
-    , ClassifModel
-    , RegressionModel
-)
-import gc
-import polars as pl
-import numpy as np
-
-# --------------------- Other, miscellaneous helper functions ----------------------------------------------
-@dataclass
-class NumPyDataCube:
-    X: np.ndarray
-    y: np.ndarray
-    features: list[str]
-    target: str
-
-    def to_df(self) -> pl.DataFrame:
-        if self.X.shape[0] != len(self.y.ravel()):
-            raise ValueError("NumPyDataCube's X and y must have the same number of rows.") 
-
-        df = pl.from_numpy(self.X, schema=self.features)
-        t = pl.Series(self.target, self.y)
-        return df.insert_at_idx(0, t)
-
-def get_numpy(
-    df:PolarsFrame
-    , target:str
-    , flatten:bool=True
-    , low_memory:bool=True
-) -> NumPyDataCube:
-    '''
-    Create NumPy feature matrix X and target y from dataframe and target. Note that this implementation will 
-    "clear df" at the end.
-
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars dataframe
-    target
-        The name of the target column
-    flatten
-        Whether to flatten target or not
-    low_memory
-        Whether to do NumPy conversion column by column or all at once     
-    '''
-    features:list[str] = df.columns 
-    features.remove(target)
-    df_local = df.lazy().collect()
-    y = df_local.drop_in_place(target).to_numpy()
-    if flatten:
-        y = y.ravel()
-    
-    if low_memory:
-        columns = []
-        for c in features:
-            columns.append(
-                df_local.drop_in_place(c).to_numpy().reshape((-1,1))
-            )
-        X = np.concatenate(columns, axis=1)
-    else:
-        X = df_local[features].to_numpy()
-
-    df = df.clear() # Reset to empty.
-    return NumPyDataCube(X, y, features, target)
-
-def dump_blueprint(df:pl.LazyFrame, path:str|Path) -> pl.LazyFrame:
-    if isinstance(df, pl.LazyFrame):
-        df.blueprint.preserve(path)
-        return df
-    raise TypeError("Blueprints only work with LazyFrame.")
-
-def checkpoint(
-    df:PolarsFrame
-    , temp_file_path:str|Path
-    , limit:int = -1
-    , **kwargs) -> PolarsFrame:
-    '''
-    A wrapper to save a temp copy of the data so far in either parquet or csv format at the given path. This
-    is purely a side effect. The difference between this and sink is that this gives you the option to save 
-    the temp file as a .csv, which can be checked by a human.
-
-    This step is pipeline compatible but will not be persisted in the blueprint.
-
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars dataframe
-    temp_file_path
-        Path to write to. Must either end with .csv or .parquet
-    limit
-        Limit the number of rows to write. If <= 0, write all
-    
-    All other keyword arguments will be passed to Polars' write_csv or write_parquet
-    '''
-    ext = temp_file_path.split(".")[-1]
-    if ext == "csv":
-        if limit > 0:
-            df.lazy().limit(limit).collect().write_csv(temp_file_path, **kwargs)
-        else:
-            df.lazy().collect().write_csv(temp_file_path, **kwargs)
-    elif ext == "parquet":
-        if limit > 0:
-            df.lazy().limit(limit).collect().write_parquet(temp_file_path, **kwargs)
-        else:
-            df.lazy().collect().write_parquet(temp_file_path, **kwargs)
-    else:
-        raise ValueError(f"Temp file path must end with .csv or .parquet, not {ext}.")
-    
-    return df
-
-def sink_parquet(
-    df: pl.LazyFrame
-    , path: str | Path
-    , **kwargs
-) -> pl.LazyFrame:
-    '''
-    A wrapper for sink_parquet so that it is pipeline compatible. This will not be persisted in the blueprint.
-    '''
-    df.sink_parquet(path, **kwargs)
-    return df
-
-def sink_ipc(
-    df: pl.LazyFrame
-    , path: str | Path
-    , **kwargs
-) -> pl.LazyFrame:
-    '''
-    A wrapper for sink_ipc so that it is pipeline compatible. This will not be persisted in the blueprint.
-    '''
-    df.sink_ipc(path, **kwargs)
-    return df
-
-def garbage_collect(df:PolarsFrame, persist:bool=False) -> PolarsFrame:
-    '''
-    A wrapper so that garbage collect can be part of the pipeline. This is purely a side effect.
-
-    Parameters
-    ----------
-    df
-        Either a lazy or eager Polars dataframe
-    persist
-        Set it to true if df is lazy and you want to persist this step in the pipeline
-    '''
-    _ = gc.collect()
-    if isinstance(df, pl.LazyFrame) and persist:
-        return df.blueprint.add_func(df, garbage_collect, {})
-    return df
-
-def append_classif_score(
-    df: PolarsFrame
-    , model:ClassifModel
-    , target: Optional[str] = None
-    , features: Optional[list[str]] = None
-    , score_idx:int = -1 
-    , score_col:str = "model_score"
-) -> PolarsFrame:
-    '''
-    Appends a classification model to the pipeline. This step will collect the lazy frame.
-
-    If input df is lazy, this step will be remembered by the pipelien by default.
-
-    Parameters
-    ----------
-    model
-        The trained classification model
-    target
-        The target of the model, which will not be used in making the prediction. It is only here so that 
-        we can remove it from feature list if it is in features by mistake.
-    features
-        The features the model takes. If none, will use all non-target features. If target not provided, it will use all
-        columns
-    score_idx
-        The index of the score column in predict_proba you want to append to the dataframe. E.g. -1 will take the 
-        score of the positive class in a binary classification
-    score_col
-        The name of the score column
-    '''
-    if isinstance(df, pl.LazyFrame):
-        return df.blueprint.add_classif(model, target, features, score_idx, score_col)
-    return Blueprint._process_classif(df, model, target, features, score_idx, score_col)
-
-def append_regression(
-    df: PolarsFrame
-    , model:RegressionModel
-    , target: Optional[str] = None
-    , features: Optional[list[str]] = None
-    , score_col:str = "model_score"
-) -> PolarsFrame:
-    '''
-    Appends a regression model to the pipeline. This step will collect the lazy frame.
-
-    If input df is lazy, this step will be remembered by the pipelien by default.
-
-    Parameters
-    ----------
-    model
-        The trained classification model
-    target
-        The target of the model, which will not be used in making the prediction. It is only here so that we can 
-        remove it from feature list if it is in features by mistake.
-    features
-        The features the model takes. If none, will use all non-target features. If target not provided, it will use all
-        columns
-    score_col
-        The name of the score column
-    '''
-    if isinstance(df, pl.LazyFrame):
-        return df.blueprint.add_regression(model, target, features, score_col)
-    return Blueprint._process_regression(df, model, target, features, score_col)
-    
-class Identity(ClassifModel, RegressionModel):
-
-    def __init__(self, col:str="", idx:int=-1):
-        '''
-        A identity passthrough. When incoming data is a Polars DataFrame, please supply a column name.
-        If incoming data is a NumPy matrix, please supply a positive index for the passthrough column.
-        This is built for use in Polars pipelines. But NumPy compatibility is also considered.
-        '''
-        self.col = col
-        self.idx = idx
-    
-    def fit(self, _:Union[np.ndarray,pl.DataFrame]):
-        return
-    
-    def predict_proba(self, X:Union[np.ndarray,pl.DataFrame]) -> np.ndarray:
-        if isinstance(X, pl.DataFrame) and self.col in X.columns:
-            return X[self.col].to_numpy()
-        elif isinstance(X, np.ndarray) and self.idx > 0:
-            return X[:, self.idx]
-        raise ValueError(f"Either the column {self.col} is not in X. Or X is a NumPy matrix, but idx "
-                         "is not initialized. Cannot do a passthrough.")
-    
-    # They are the same in the identity case
-    def predict(self, X:Union[np.ndarray,pl.DataFrame]) -> np.ndarray:
-        return self.predict_proba(X)
-
-def id_passthrough(
-    df: PolarsFrame
-    , col: str
-    , as_reg: bool = True
-    , score_col:str = "score"
-) -> PolarsFrame:
-    '''
-    Appends an identity passthrough to the pipeline. This step will collect the lazy frame. 
-
-    If input df is lazy, this step will be remembered by the pipelien by default.
-
-    Parameters
-    ----------
-    df
-        Either an eager or a lazy Polars DataFrame
-    col
-        The col that will be used as x in the linear function
-    as_reg
-        If true, treat this identity as a regression. Otherwise, treat it as a classification.
-    score_col
-        The name of the score column
-    '''
-    model = Identity(col=col)
-    if isinstance(df, pl.LazyFrame):
-        if as_reg:
-            return df.blueprint.add_regression(model, None, None, -1, score_col)
-        else:
-            return df.blueprint.add_classif(model, None, None, -1, score_col)
-    else:
-        if as_reg:
-            return Blueprint._process_regression(df, model, None, None, -1, score_col)
-        else:
-            return Blueprint._process_classif(df, model, None, None, -1, score_col)
-
-class Logistic(ClassifModel):
-
-    def __init__(self, col:str="", idx:int=-1, coeff:float = 1.0, const:float=0., k:float=1.0):
-        '''
-        A logistic passthrough. When incoming data is a Polars DataFrame, please supply a column name.
-        If incoming data is a NumPy matrix, please supply a positive index for the passthrough column.
-        This is built for use in Polars pipelines. But NumPy compatibility is also considered.
-
-        The formula used is 1/(1 + exp(-k(coeff*x + const)))
-        '''
-        self.col = col
-        self.idx = idx
-        self.coeff = coeff
-        self.const = const
-        self.k = k
-
-    def fit(self, _:Union[np.ndarray,pl.DataFrame]):
-        return 
-    
-    def predict_proba(self, X:Union[np.ndarray,pl.DataFrame]) -> np.ndarray:
-        if isinstance(X, pl.DataFrame) and self.col in X.columns:
-            x = X.select(self.col).to_numpy()
-        elif isinstance(X, np.ndarray) and self.idx > 0:
-            x = X[:, self.idx].reshape((-1, 1))
-        else:
-            raise ValueError(f"Either the column {self.col} is not in X. Or X is a NumPy matrix, but idx "
-                            "is not initialized. Cannot do a passthrough.")
-        
-        return expit(self.k * (self.coeff * x + self.const))
-    
-    def predict(self, X:Union[np.ndarray,pl.DataFrame]) -> np.ndarray:
-        '''Predict using 0.5 as threshold.'''
-        return np.round(self.predict_proba(X)).astype(np.int8)
-
-def logistic_passthrough(
-    df: PolarsFrame
-    , col: str
-    , coeff: float = 1.
-    , const: float = 0.
-    , k: float = 1.
-    , score_col:str = "logistic_score"
-) -> PolarsFrame:
-    '''
-    Appends a linear model to the pipeline. This step will collect the lazy frame. 
-    
-    The formula used is 1/(1 + exp(-k(coeff*x + const)))
-
-    If input df is lazy, this step will be remembered by the pipelien by default.
-
-    Parameters
-    ----------
-    df
-        Either an eager or a lazy Polars DataFrame
-    col
-        The col that will be used as x in the logistic function
-    k
-        The logistic scaling term
-    midpoint
-        The midpoint of the logistic function
-    score_col
-        The name of the score column
-    '''
-    model = Logistic(col=col, coeff=coeff, const=const, k=k)
-    if isinstance(df, pl.LazyFrame):
-        return df.blueprint.add_classif(model, None, None, -1, score_col)
-    return Blueprint._process_classif(df, model, None, None, -1, score_col)
-
-class Linear(RegressionModel):
-
-    def __init__(self, col:str="", idx:int=-1, coeff:float=1.0, const:float=0.):
-        '''
-        A linear passthrough. When incoming data is a Polars DataFrame, please supply a column name.
-        If incoming data is a NumPy matrix, please supply a positive index for the passthrough column.
-        This is built for use in Polars pipelines. But NumPy compatibility is also considered.
-
-        The formula is coeff * x + const
-        '''
-        self.col = col
-        self.idx = idx
-        self.coeff = coeff
-        self.const = const
-
-    def fit(self, _:Union[np.ndarray,pl.DataFrame]):
-        return
-    
-    def predict(self, X:Union[np.ndarray,pl.DataFrame]) -> np.ndarray:
-        if isinstance(X, pl.DataFrame) and self.col in X.columns:
-            x = X.select(self.col).to_numpy()
-        elif isinstance(X, np.ndarray) and self.idx > 0:
-            x = X[:, self.idx].reshape((-1, 1))
-        else:
-            raise ValueError(f"Either the column {self.col} is not in X. Or X is a NumPy matrix, but idx "
-                            "is not initialized. Cannot do a passthrough.")
-        
-        return self.coeff * x + self.const
-
-def linear_passthrough(
-    df: PolarsFrame
-    , col: str
-    , coeff: float = 1.
-    , const: float = 0.
-    , score_col:str = "linear_score"
-) -> PolarsFrame:
-    '''
-    Appends a linear model to the pipeline. This step will collect the lazy frame. 
-    
-    The formula is coeff * x + const
-
-    If input df is lazy, this step will be remembered by the pipelien by default.
-
-    Parameters
-    ----------
-    df
-        Either an eager or a lazy Polars DataFrame
-    col
-        The col that will be used as x in the linear function
-    coeff
-        The coefficient of the linear function
-    const
-        The constant term of the linear function
-    score_col
-        The name of the score column
-    '''
-    model = Linear(col=col, coeff=coeff, const=const)
-    if isinstance(df, pl.LazyFrame):
-        return df.blueprint.add_regression(model, None, None, -1, score_col)
-    return Blueprint._process_regression(df, model, None, None, -1, score_col)
+from typing import Optional, Union
+from .blueprint import Blueprint
+from pathlib import Path
+from .type_alias import (
+    PolarsFrame
+    , ClassifModel
+    , RegressionModel
+)
+from dataclasses import dataclass
+from scipy.special import expit
+import gc
+import polars as pl
+import numpy as np
+
+# --------------------- Other, miscellaneous helper functions ----------------------------------------------
+@dataclass
+class NumPyDataCube:
+    X:np.ndarray
+    y:np.ndarray
+    features:list[str]
+    target:str
+
+    def to_df(self) -> pl.DataFrame:
+        if self.X.shape[0] != len(self.y.ravel()):
+            raise ValueError("NumPyDataCube's X and y must have the same number of rows.") 
+
+        df = pl.from_numpy(self.X, schema=self.features)
+        t = pl.Series(self.target, self.y)
+        return df.insert_at_idx(0, t)
+
+def get_numpy(
+    df:PolarsFrame
+    , target:str
+    , flatten:bool=True
+    , low_memory:bool=True
+) -> NumPyDataCube:
+    '''
+    Create NumPy feature matrix X and target y from dataframe and target. Note that this implementation will 
+    "clear df" at the end.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars dataframe
+    target
+        The name of the target column
+    flatten
+        Whether to flatten target or not
+    low_memory
+        Whether to do NumPy conversion column by column or all at once     
+    '''
+    features:list[str] = df.columns 
+    features.remove(target)
+    df_local = df.lazy().collect()
+    y = df_local.drop_in_place(target).to_numpy()
+    if flatten:
+        y = y.ravel()
+    
+    if low_memory:
+        columns = []
+        for c in features:
+            columns.append(
+                df_local.drop_in_place(c).to_numpy().reshape((-1,1))
+            )
+        X = np.concatenate(columns, axis=1)
+    else:
+        X = df_local[features].to_numpy()
+
+    df = df.clear() # Reset to empty.
+    return NumPyDataCube(X, y, features, target)
+
+def dump_blueprint(df:pl.LazyFrame, path:Union[str,Path]) -> pl.LazyFrame:
+    if isinstance(df, pl.LazyFrame):
+        df.blueprint.preserve(path)
+        return df
+    raise TypeError("Blueprints only work with LazyFrame.")
+
+def checkpoint(
+    df:PolarsFrame
+    , temp_file_path:Union[str,Path]
+    , limit:int = -1
+    , **kwargs) -> PolarsFrame:
+    '''
+    A wrapper to save a temp copy of the data so far in either parquet or csv format at the given path. This
+    is purely a side effect. The difference between this and sink is that this gives you the option to save 
+    the temp file as a .csv, which can be checked by a human.
+
+    This step is pipeline compatible but will not be persisted in the blueprint.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars dataframe
+    temp_file_path
+        Path to write to. Must either end with .csv or .parquet
+    limit
+        Limit the number of rows to write. If <= 0, write all
+    
+    All other keyword arguments will be passed to Polars' write_csv or write_parquet
+    '''
+    ext = temp_file_path.split(".")[-1]
+    if ext == "csv":
+        if limit > 0:
+            df.lazy().limit(limit).collect().write_csv(temp_file_path, **kwargs)
+        else:
+            df.lazy().collect().write_csv(temp_file_path, **kwargs)
+    elif ext == "parquet":
+        if limit > 0:
+            df.lazy().limit(limit).collect().write_parquet(temp_file_path, **kwargs)
+        else:
+            df.lazy().collect().write_parquet(temp_file_path, **kwargs)
+    else:
+        raise ValueError(f"Temp file path must end with .csv or .parquet, not {ext}.")
+    
+    return df
+
+def sink_parquet(
+    df: pl.LazyFrame
+    , path: Union[str,Path]
+    , **kwargs
+) -> pl.LazyFrame:
+    '''
+    A wrapper for sink_parquet so that it is pipeline compatible. This will not be persisted in the blueprint.
+    '''
+    df.sink_parquet(path, **kwargs)
+    return df
+
+def sink_ipc(
+    df: pl.LazyFrame
+    , path: Union[str,Path]
+    , **kwargs
+) -> pl.LazyFrame:
+    '''
+    A wrapper for sink_ipc so that it is pipeline compatible. This will not be persisted in the blueprint.
+    '''
+    df.sink_ipc(path, **kwargs)
+    return df
+
+def garbage_collect(df:PolarsFrame, persist:bool=False) -> PolarsFrame:
+    '''
+    A wrapper so that garbage collect can be part of the pipeline. This is purely a side effect.
+
+    Parameters
+    ----------
+    df
+        Either a lazy or eager Polars dataframe
+    persist
+        Set it to true if df is lazy and you want to persist this step in the pipeline
+    '''
+    _ = gc.collect()
+    if isinstance(df, pl.LazyFrame) and persist:
+        return df.blueprint.add_func(df, garbage_collect, {})
+    return df
+
+def append_classif_score(
+    df: PolarsFrame
+    , model:ClassifModel
+    , features: list[str]
+    , target: Optional[str] = None
+    , score_idx:int = -1 
+    , score_col:str = "model_score"
+) -> PolarsFrame:
+    '''
+    Appends a classification model to the pipeline. This step will collect the lazy frame.
+
+    If input df is lazy, this step will be remembered by the blueprint by default.
+
+    Parameters
+    ----------
+    model
+        The trained classification model
+    features
+        The features the model takes
+    target
+        The target of the model, which will not be used in making the prediction. It is only here so that 
+        we can remove it from feature list if it is in features by mistake.
+    score_idx
+        The index of the score column in predict_proba you want to append to the dataframe. E.g. -1 will take the 
+        score of the positive class in a binary classification
+    score_col
+        The name of the score column
+    '''
+    if isinstance(df, pl.LazyFrame):
+        return df.blueprint.add_classif(model, features, target, score_idx, score_col)
+    return Blueprint._process_classif(df, model, features, target, score_idx, score_col)
+
+def append_regression(
+    df: PolarsFrame
+    , model:RegressionModel
+    , features: list[str]
+    , target: Optional[str] = None
+    , score_col:str = "model_score"
+) -> PolarsFrame:
+    '''
+    Appends a regression model to the pipeline. This step will collect the lazy frame.
+
+    If input df is lazy, this step will be remembered by the blueprint by default.
+
+    Parameters
+    ----------
+    model
+        The trained classification model
+    features
+        The features the model takes
+    target
+        The target of the model, which will not be used in making the prediction. It is only here so that we can 
+        remove it from feature list if it is in features by mistake.
+    score_col
+        The name of the score column
+    '''
+    if isinstance(df, pl.LazyFrame):
+        return df.blueprint.add_regression(model, features, target, score_col)
+    return Blueprint._process_regression(df, model, features, target, score_col)
+    
+class Identity(ClassifModel, RegressionModel):
+
+    def __init__(self, col:str="", idx:int=-1):
+        '''
+        A identity passthrough. When incoming data is a Polars DataFrame, please supply a column name.
+        If incoming data is a NumPy matrix, please supply a positive index for the passthrough column.
+        This is built for use in Polars pipelines. But NumPy compatibility is also considered.
+        '''
+        self.col = col
+        self.idx = idx
+    
+    def fit(self, _:Union[np.ndarray,pl.DataFrame]):
+        return
+    
+    def predict_proba(self, X:Union[np.ndarray,pl.DataFrame]) -> np.ndarray:
+        if isinstance(X, pl.DataFrame) and self.col in X.columns:
+            return X[self.col].to_numpy()
+        elif isinstance(X, np.ndarray) and self.idx > 0:
+            return X[:, self.idx]
+        raise ValueError(f"Either the column {self.col} is not in X. Or X is a NumPy matrix, but idx "
+                         "is not initialized. Cannot do a passthrough.")
+    
+    # They are the same in the identity case
+    def predict(self, X:Union[np.ndarray,pl.DataFrame]) -> np.ndarray:
+        return self.predict_proba(X)
+
+def id_passthrough(
+    df: PolarsFrame
+    , col:str
+    , as_reg: bool = False
+    , score_col:str = "score"
+) -> PolarsFrame:
+    '''
+    Appends an identity passthrough to the pipeline. This step will collect the lazy frame. 
+
+    If input df is lazy, this step will be remembered by the blueprint by default.
+
+    Parameters
+    ----------
+    df
+        Either an eager or a lazy Polars DataFrame
+    col
+        The col that will be used as x in the linear function
+    as_reg
+        If true, treat this identity as a regression. Otherwise, treat it as a classification.
+    score_col
+        The name of the score column
+    '''
+    model = Identity(col=col)
+    if isinstance(df, pl.LazyFrame):
+        if as_reg:
+            return df.blueprint.add_regression(model, [col], None, score_col)
+        else:
+            return df.blueprint.add_classif(model, [col], None, -1, score_col)
+    else:
+        if as_reg:
+            return Blueprint._process_regression(df, model, [col], None, score_col)
+        else:
+            return Blueprint._process_classif(df, model, [col], None, -1, score_col)
+
+class Logistic(ClassifModel):
+
+    def __init__(self, col:str="", idx:int=-1, coeff:float = 1.0, const:float=0., k:float=1.0):
+        '''
+        A logistic passthrough. When incoming data is a Polars DataFrame, please supply a column name.
+        If incoming data is a NumPy matrix, please supply a positive index for the passthrough column.
+        This is built for use in Polars pipelines. But NumPy compatibility is also considered.
+
+        The formula used is 1/(1 + exp(-k(coeff*x + const)))
+        '''
+        self.col = col
+        self.idx = idx
+        self.coeff = coeff
+        self.const = const
+        self.k = k
+
+    def fit(self, _:Union[np.ndarray,pl.DataFrame]):
+        return 
+    
+    def predict_proba(self, X:Union[np.ndarray,pl.DataFrame]) -> np.ndarray:
+        if isinstance(X, pl.DataFrame) and self.col in X.columns:
+            x = X.select(self.col).to_numpy()
+        elif isinstance(X, np.ndarray) and self.idx > 0:
+            x = X[:, self.idx].reshape((-1, 1))
+        else:
+            raise ValueError(f"Either the column {self.col} is not in X. Or X is a NumPy matrix, but idx "
+                            "is not initialized. Cannot do a passthrough.")
+        
+        return expit(self.k * (self.coeff * x + self.const))
+    
+    def predict(self, X:Union[np.ndarray,pl.DataFrame]) -> np.ndarray:
+        '''Predict using 0.5 as threshold.'''
+        return np.round(self.predict_proba(X)).astype(np.int8)
+
+def logistic_passthrough(
+    df: PolarsFrame
+    , col: str
+    , coeff: float = 1.
+    , const: float = 0.
+    , k: float = 1.
+    , score_col:str = "logistic_score"
+) -> PolarsFrame:
+    '''
+    Appends a linear model to the pipeline. This step will collect the lazy frame.
+    
+    The formula used is 1/(1 + exp(-k(coeff*x + const)))
+
+    If input df is lazy, this step will be remembered by the blueprint by default.
+
+    Parameters
+    ----------
+    df
+        Either an eager or a lazy Polars DataFrame
+    col
+        The col that will be used as x in the logistic function
+    k
+        The logistic scaling term
+    midpoint
+        The midpoint of the logistic function
+    score_col
+        The name of the score column
+    '''
+    model = Logistic(col=col, coeff=coeff, const=const, k=k)
+    if isinstance(df, pl.LazyFrame):
+        return df.blueprint.add_classif(model, [col], None, -1, score_col)
+    return Blueprint._process_classif(df, model, [col], None, -1, score_col)
+
+class Linear(RegressionModel):
+
+    def __init__(self, col:str="", idx:int=-1, coeff:float=1.0, const:float=0.):
+        '''
+        A linear passthrough. When incoming data is a Polars DataFrame, please supply a column name.
+        If incoming data is a NumPy matrix, please supply a positive index for the passthrough column.
+        This is built for use in Polars pipelines. But NumPy compatibility is also considered.
+
+        The formula is coeff * x + const
+        '''
+        self.col = col
+        self.idx = idx
+        self.coeff = coeff
+        self.const = const
+
+    def fit(self, _:Union[np.ndarray,pl.DataFrame]):
+        return
+    
+    def predict(self, X:Union[np.ndarray,pl.DataFrame]) -> np.ndarray:
+        if isinstance(X, pl.DataFrame) and self.col in X.columns:
+            x = X.select(self.col).to_numpy()
+        elif isinstance(X, np.ndarray) and self.idx > 0:
+            x = X[:, self.idx].reshape((-1, 1))
+        else:
+            raise ValueError(f"Either the column {self.col} is not in X. Or X is a NumPy matrix, but idx "
+                            "is not initialized. Cannot do a passthrough.")
+        
+        return self.coeff * x + self.const
+
+def linear_passthrough(
+    df: PolarsFrame
+    , col: str
+    , coeff: float = 1.
+    , const: float = 0.
+    , score_col:str = "linear_score"
+) -> PolarsFrame:
+    '''
+    Appends a linear model to the pipeline. This step will collect the lazy frame. 
+    
+    The formula is coeff * x + const
+
+    If input df is lazy, this step will be remembered by the blueprint by default.
+
+    Parameters
+    ----------
+    df
+        Either an eager or a lazy Polars DataFrame
+    col
+        The col that will be used as x in the linear function
+    coeff
+        The coefficient of the linear function
+    const
+        The constant term of the linear function
+    score_col
+        The name of the score column
+    '''
+    model = Linear(col=col, coeff=coeff, const=const)
+    if isinstance(df, pl.LazyFrame):
+        return df.blueprint.add_regression(model, [col], None, score_col)
+    return Blueprint._process_regression(df, model, [col], None, score_col)
```

