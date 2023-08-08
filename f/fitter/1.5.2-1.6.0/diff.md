# Comparing `tmp/fitter-1.5.2.tar.gz` & `tmp/fitter-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fitter-1.5.2.tar", last modified: Sun Jan  1 21:19:40 2023, max compression
+gzip compressed data, was "fitter-1.6.0.tar", max compression
```

## Comparing `fitter-1.5.2.tar` & `fitter-1.6.0.tar`

### file list

```diff
@@ -1,26 +1,9 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-01 21:19:40.000000 fitter-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-01-01 21:19:32.000000 fitter-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-01-01 21:19:32.000000 fitter-1.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7859 2023-01-01 21:19:40.000000 fitter-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5745 2023-01-01 21:19:32.000000 fitter-1.5.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)       54 2023-01-01 21:19:32.000000 fitter-1.5.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      262 2023-01-01 21:19:40.000000 fitter-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2247 2023-01-01 21:19:32.000000 fitter-1.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-01 21:19:40.000000 fitter-1.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-01 21:19:40.000000 fitter-1.5.2/src/fitter/
--rw-r--r--   0 runner    (1001) docker     (122)      248 2023-01-01 21:19:32.000000 fitter-1.5.2/src/fitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18477 2023-01-01 21:19:32.000000 fitter-1.5.2/src/fitter/fitter.py
--rw-r--r--   0 runner    (1001) docker     (122)     5450 2023-01-01 21:19:32.000000 fitter-1.5.2/src/fitter/histfit.py
--rw-r--r--   0 runner    (1001) docker     (122)     2847 2023-01-01 21:19:32.000000 fitter-1.5.2/src/fitter/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-01 21:19:40.000000 fitter-1.5.2/src/fitter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7859 2023-01-01 21:19:40.000000 fitter-1.5.2/src/fitter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      449 2023-01-01 21:19:40.000000 fitter-1.5.2/src/fitter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-01 21:19:40.000000 fitter-1.5.2/src/fitter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-01-01 21:19:40.000000 fitter-1.5.2/src/fitter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-01 21:19:40.000000 fitter-1.5.2/src/fitter.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       54 2023-01-01 21:19:40.000000 fitter-1.5.2/src/fitter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-01-01 21:19:40.000000 fitter-1.5.2/src/fitter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-01 21:19:40.000000 fitter-1.5.2/test/
--rw-r--r--   0 runner    (1001) docker     (122)     1714 2023-01-01 21:19:32.000000 fitter-1.5.2/test/test_fitter.py
--rw-r--r--   0 runner    (1001) docker     (122)      646 2023-01-01 21:19:32.000000 fitter-1.5.2/test/test_histfit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1212 2023-01-01 21:19:32.000000 fitter-1.5.2/test/test_main.py
+-rw-r--r--   0        0        0    35149 2020-06-03 17:27:56.378512 fitter-1.6.0/LICENSE
+-rw-r--r--   0        0        0     6272 2023-08-08 21:35:41.062039 fitter-1.6.0/README.rst
+-rw-r--r--   0        0        0     1481 2023-08-08 21:35:41.048038 fitter-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0      248 2021-09-02 19:40:23.829489 fitter-1.6.0/src/fitter/__init__.py
+-rw-r--r--   0        0        0    19339 2023-08-08 21:35:41.057038 fitter-1.6.0/src/fitter/fitter.py
+-rw-r--r--   0        0        0     5502 2023-08-08 21:35:41.054038 fitter-1.6.0/src/fitter/histfit.py
+-rw-r--r--   0        0        0     2946 2023-08-08 21:35:41.055039 fitter-1.6.0/src/fitter/main.py
+-rw-r--r--   0        0        0     7364 1970-01-01 00:00:00.000000 fitter-1.6.0/setup.py
+-rw-r--r--   0        0        0     7846 1970-01-01 00:00:00.000000 fitter-1.6.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `fitter-1.5.2/LICENSE` & `fitter-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fitter-1.5.2/PKG-INFO` & `fitter-1.6.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,175 +1,188 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: fitter
-Version: 1.5.2
-Summary: A tool to fit data to many distributions and best one(s)
-Home-page: https://github.com/cokelaer/fitter
-Author: Thomas Cokelaer
-Author-email: cokelaer@gmail.com
-Maintainer: Thomas Cokelaer
-Maintainer-email: cokelaer@gmail.com
+Version: 1.6.0
+Summary: A tool to fit data to many distributions and get the best one(s)
 License: GPL
-Download-URL: https://github.com/cokelaer/fitter
-Description: 
-        
-        #############################
-        FITTER documentation
-        #############################
-        
-        .. image:: https://badge.fury.io/py/fitter.svg
-            :target: https://pypi.python.org/pypi/fitter
-        
-        .. image:: https://github.com/cokelaer/fitter/actions/workflows/main.yml/badge.svg?branch=main
-            :target: https://github.com/cokelaer/fitter/actions/workflows/main.yml
-        
-        .. image:: https://coveralls.io/repos/cokelaer/fitter/badge.png?branch=main
-            :target: https://coveralls.io/r/cokelaer/fitter?branch=main
-        
-        .. image:: http://readthedocs.org/projects/fitter/badge/?version=latest
-            :target: http://fitter.readthedocs.org/en/latest/?badge=latest
-            :alt: Documentation Status
-        
-        .. image:: https://zenodo.org/badge/23078551.svg
-           :target: https://zenodo.org/badge/latestdoi/23078551
-        
-        Compatible with Python 3.7, and 3.8, 3.9
-        
-        
-        What is it ?
-        ################
-        
-        **fitter** package provides a simple class to identify the distribution from which a data samples 
-        is generated from. It uses 80 distributions from Scipy and allows you to plot the results to check 
-        what is the most probable distribution and the best parameters.
-        
-        
-        Installation
-        ###################
-        
-        ::
-        
-            pip install fitter
-        
-        **fitter** is also available on **conda** (bioconda channel)::
-         
-             conda install fitter
-        
-        
-        Usage
-        ##################
-        
-        standalone
-        ===========
-        
-        A standalone application (very simple) is also provided and works with input CSV
-        files::
-          
-            fitter fitdist data.csv --column-number 1 --distributions gamma,normal
-         
-        It creates a file called fitter.png and a log fitter.log
-        
-        From Python shell
-        ==================
-        
-        First, let us create a data samples with N = 10,000 points from a gamma distribution::
-        
-            from scipy import stats
-            data = stats.gamma.rvs(2, loc=1.5, scale=2, size=10000)
-        
-        .. note:: the fitting is slow so keep the size value to reasonable value.
-        
-        Now, without any knowledge about the distribution or its parameter, what is the distribution that fits the data best ? Scipy has 80 distributions and the **Fitter** class will scan all of them, call the fit function for you, ignoring those that fail or run forever and finally give you a summary of the best distributions in the sense of sum of the square errors. The best is to give an example::
-        
-        
-            from fitter import Fitter
-            f = Fitter(data)
-            f.fit()
-            # may take some time since by default, all distributions are tried
-            # but you call manually provide a smaller set of distributions 
-            f.summary()
-        
-        
-        .. image:: http://pythonhosted.org/fitter/_images/index-1.png
-            :target: http://pythonhosted.org/fitter/_images/index-1.png
-        
-        
-        See the `online <http://fitter.readthedocs.io/>`_ documentation for details.
-        
-        
-        Contributors
-        =============
-        
-        
-        Setting up and maintaining Fitter has been possible thanks to users and contributors.
-        Thanks to all:
-        
-        .. image:: https://contrib.rocks/image?repo=cokelaer/fitter
-            :target: https://github.com/cokelaer/fitter/graphs/contributors
-        
-        
-        
-        
-        Changelog
-        ~~~~~~~~~
-        ========= ==========================================================================
-        Version   Description
-        ========= ==========================================================================
-        1.5.2     * PR https://github.com/cokelaer/fitter/pull/74 to fix logger
-        1.5.1     * fixed regression putting back joblib
-        1.5.0     * removed easydev and replaced by tqdm for progress bar
-                  * progressbar from tqdm also allows replacement of joblib need
-        1.4.1     * Update timeout in docs from 10 to 30 seconds by @mpadge in 
-                    https://github.com/cokelaer/fitter/pull/47
-                  * Add Kolmogorov-Smirnov goodness-of-fit statistic by @lahdjirayhan in 
-                    https://github.com/cokelaer/fitter/pull/58
-                  * switch branch from master to main
-        1.4.0     * get_best function now returns the parameters as a dictionary 
-                    of parameter names and their values rather than just a list of
-                    values (https://github.com/cokelaer/fitter/issues/23) thanks to 
-                    contributor @kabirmdasraful
-                  * Accepting PR to fix progress bar issue reported in 
-                    https://github.com/cokelaer/fitter/pull/37
-        1.3.0     * parallel process implemented https://github.com/cokelaer/fitter/pull/25
-                    thanks to @arsenyinfo 
-        1.2.3     * remove vervose arguments in Fitter class. Using the logging module 
-                    instead
-                  * the Fitter.fit has now a progress bar
-                  * add a standalone application called … fitter (see the doc)
-        1.2.2     was not released
-        1.2.1     adding new class called histfit (see documentation)
-        1.2       * Fixed the version. Previous version switched from 
-                    1.0.9 to 1.1.11. To start a fresh version, we increase to 1.2.0
-                  * Merged pull request required by bioconda
-                  * Merged pull request related to implementation of 
-                    AIC/BIC/KL criteria (https://github.com/cokelaer/fitter/pull/19). 
-                    This also fixes https://github.com/cokelaer/fitter/issues/9
-                  * Implement two functions to get all distributions, or a list of 
-                    common distributions to help users decreading computational time 
-                    (https://github.com/cokelaer/fitter/issues/20). Also added a FAQS 
-                    section.
-                  * travis tested Python 3.6 and 3.7 (not 3.5 anymore)
-        1.1       * Fixed deprecated warning
-                  * fitter is now in readthedocs at fitter.readthedocs.io
-        1.0.9     * https://github.com/cokelaer/fitter/pull/8 and 11
-                    PR https://github.com/cokelaer/fitter/pull/8
-        1.0.6     * summary() now returns the dataframe (instead of printing it)
-        1.0.5      https://github.com/cokelaer/fitter/issues
-        1.0.2     add manifest to fix missing source in the pypi repository.
-        ========= ==========================================================================
-        
-        
-        
-        
-        
 Keywords: fit,distribution,fitting,scipy
-Platform: Linux
-Platform: Unix
-Platform: MacOsX
-Platform: Windows
+Author: Thomas Cokelaer
+Author-email: cokelaer@gmail.com
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: click (>=8.1.6,<9.0.0)
+Requires-Dist: joblib (>=1.3.1,<2.0.0)
+Requires-Dist: matplotlib (>=3.7.2)
+Requires-Dist: numpy (>=1.20)
+Requires-Dist: pandas (>=2.0.3,<3.0.0)
+Requires-Dist: scipy (>=0.18)
+Requires-Dist: tqdm (>=4.65.1,<5.0.0)
+Description-Content-Type: text/x-rst
+
+
+
+#############################
+FITTER documentation
+#############################
+
+.. image:: https://badge.fury.io/py/fitter.svg
+    :target: https://pypi.python.org/pypi/fitter
+
+.. image:: https://github.com/cokelaer/fitter/actions/workflows/main.yml/badge.svg?branch=main
+    :target: https://github.com/cokelaer/fitter/actions/workflows/main.yml
+
+.. image:: https://coveralls.io/repos/cokelaer/fitter/badge.png?branch=main
+    :target: https://coveralls.io/r/cokelaer/fitter?branch=main
+
+.. image:: http://readthedocs.org/projects/fitter/badge/?version=latest
+    :target: http://fitter.readthedocs.org/en/latest/?badge=latest
+    :alt: Documentation Status
+
+.. image:: https://zenodo.org/badge/23078551.svg
+   :target: https://zenodo.org/badge/latestdoi/23078551
+
+Compatible with Python 3.7, and 3.8, 3.9
+
+
+What is it ?
+################
+
+The **fitter** package is a Python library used for fitting probability distributions to data. It provides a straightforward and and intuitive interface to estimate parameters for various types of distributions, both continuous and discrete. Using **fitter**, you can easily fit a range of distributions to your data and compare their fit, aiding in the selection of the most suitable distribution. The package is designed to be user-friendly and requires minimal setup, making it a useful tool for data scientists and statisticians working with probability distributions.
+
+Installation
+###################
+
+::
+
+    pip install fitter
+
+**fitter** is also available on **conda** (bioconda channel)::
+ 
+     conda install fitter
+
+
+Usage
+##################
+
+standalone
+===========
+
+A standalone application (very simple) is also provided and works with input CSV
+files::
+  
+    fitter fitdist data.csv --column-number 1 --distributions gamma,normal
+ 
+It creates a file called fitter.png and a log fitter.log
+
+From Python shell
+==================
+
+First, let us create a data samples with N = 10,000 points from a gamma distribution::
+
+    from scipy import stats
+    data = stats.gamma.rvs(2, loc=1.5, scale=2, size=10000)
+
+.. note:: the fitting is slow so keep the size value to reasonable value.
+
+Now, without any knowledge about the distribution or its parameter, what is the distribution that fits the data best ? Scipy has 80 distributions and the **Fitter** class will scan all of them, call the fit function for you, ignoring those that fail or run forever and finally give you a summary of the best distributions in the sense of sum of the square errors. The best is to give an example::
+
+
+    from fitter import Fitter
+    f = Fitter(data)
+    f.fit()
+    # may take some time since by default, all distributions are tried
+    # but you call manually provide a smaller set of distributions 
+    f.summary()
+
+
+.. image:: http://pythonhosted.org/fitter/_images/index-1.png
+    :target: http://pythonhosted.org/fitter/_images/index-1.png
+
+
+See the `online <http://fitter.readthedocs.io/>`_ documentation for details.
+
+
+Contributors
+=============
+
+
+Setting up and maintaining Fitter has been possible thanks to users and contributors.
+Thanks to all:
+
+.. image:: https://contrib.rocks/image?repo=cokelaer/fitter
+    :target: https://github.com/cokelaer/fitter/graphs/contributors
+
+
+
+
+Changelog
+~~~~~~~~~
+========= ==========================================================================
+Version   Description
+========= ==========================================================================
+1.6.0     * for developers: uses pyproject.toml instead of setup.py
+          * Fix progress bar fixing https://github.com/cokelaer/fitter/pull/74
+          * Fix BIC formula https://github.com/cokelaer/fitter/pull/77
+1.5.2     * PR https://github.com/cokelaer/fitter/pull/74 to fix logger
+1.5.1     * fixed regression putting back joblib
+1.5.0     * removed easydev and replaced by tqdm for progress bar
+          * progressbar from tqdm also allows replacement of joblib need
+1.4.1     * Update timeout in docs from 10 to 30 seconds by @mpadge in 
+            https://github.com/cokelaer/fitter/pull/47
+          * Add Kolmogorov-Smirnov goodness-of-fit statistic by @lahdjirayhan in 
+            https://github.com/cokelaer/fitter/pull/58
+          * switch branch from master to main
+1.4.0     * get_best function now returns the parameters as a dictionary 
+            of parameter names and their values rather than just a list of
+            values (https://github.com/cokelaer/fitter/issues/23) thanks to 
+            contributor @kabirmdasraful
+          * Accepting PR to fix progress bar issue reported in 
+            https://github.com/cokelaer/fitter/pull/37
+1.3.0     * parallel process implemented https://github.com/cokelaer/fitter/pull/25
+            thanks to @arsenyinfo 
+1.2.3     * remove vervose arguments in Fitter class. Using the logging module 
+            instead
+          * the Fitter.fit has now a progress bar
+          * add a standalone application called … fitter (see the doc)
+1.2.2     was not released
+1.2.1     adding new class called histfit (see documentation)
+1.2       * Fixed the version. Previous version switched from 
+            1.0.9 to 1.1.11. To start a fresh version, we increase to 1.2.0
+          * Merged pull request required by bioconda
+          * Merged pull request related to implementation of 
+            AIC/BIC/KL criteria (https://github.com/cokelaer/fitter/pull/19). 
+            This also fixes https://github.com/cokelaer/fitter/issues/9
+          * Implement two functions to get all distributions, or a list of 
+            common distributions to help users decreading computational time 
+            (https://github.com/cokelaer/fitter/issues/20). Also added a FAQS 
+            section.
+          * travis tested Python 3.6 and 3.7 (not 3.5 anymore)
+1.1       * Fixed deprecated warning
+          * fitter is now in readthedocs at fitter.readthedocs.io
+1.0.9     * https://github.com/cokelaer/fitter/pull/8 and 11
+            PR https://github.com/cokelaer/fitter/pull/8
+1.0.6     * summary() now returns the dataframe (instead of printing it)
+1.0.5      https://github.com/cokelaer/fitter/issues
+1.0.2     add manifest to fix missing source in the pypi repository.
+========= ==========================================================================
+
+
+
+
+
```

### Comparing `fitter-1.5.2/README.rst` & `fitter-1.6.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -22,18 +22,15 @@
 
 Compatible with Python 3.7, and 3.8, 3.9
 
 
 What is it ?
 ################
 
-**fitter** package provides a simple class to identify the distribution from which a data samples 
-is generated from. It uses 80 distributions from Scipy and allows you to plot the results to check 
-what is the most probable distribution and the best parameters.
-
+The **fitter** package is a Python library used for fitting probability distributions to data. It provides a straightforward and and intuitive interface to estimate parameters for various types of distributions, both continuous and discrete. Using **fitter**, you can easily fit a range of distributions to your data and compare their fit, aiding in the selection of the most suitable distribution. The package is designed to be user-friendly and requires minimal setup, making it a useful tool for data scientists and statisticians working with probability distributions.
 
 Installation
 ###################
 
 ::
 
     pip install fitter
@@ -98,14 +95,17 @@
 
 
 Changelog
 ~~~~~~~~~
 ========= ==========================================================================
 Version   Description
 ========= ==========================================================================
+1.6.0     * for developers: uses pyproject.toml instead of setup.py
+          * Fix progress bar fixing https://github.com/cokelaer/fitter/pull/74
+          * Fix BIC formula https://github.com/cokelaer/fitter/pull/77
 1.5.2     * PR https://github.com/cokelaer/fitter/pull/74 to fix logger
 1.5.1     * fixed regression putting back joblib
 1.5.0     * removed easydev and replaced by tqdm for progress bar
           * progressbar from tqdm also allows replacement of joblib need
 1.4.1     * Update timeout in docs from 10 to 30 seconds by @mpadge in 
             https://github.com/cokelaer/fitter/pull/47
           * Add Kolmogorov-Smirnov goodness-of-fit statistic by @lahdjirayhan in
```

### Comparing `fitter-1.5.2/src/fitter/fitter.py` & `fitter-1.6.0/src/fitter/fitter.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,16 +36,15 @@
 from scipy.stats import entropy as kl_div, kstest
 
 logger = logging.getLogger(__name__)
 
 __all__ = ["get_common_distributions", "get_distributions", "Fitter"]
 
 
-
-# A solution to wrap joblib parallel call in tqdm from 
+# A solution to wrap joblib parallel call in tqdm from
 # https://stackoverflow.com/questions/24983493/tracking-progress-of-joblib-parallel-execution/58936697#58936697
 # and https://github.com/louisabraham/tqdm_joblib
 @contextlib.contextmanager
 def tqdm_joblib(*args, **kwargs):
     """Context manager to patch joblib to report into tqdm progress bar
     given as argument"""
 
@@ -64,20 +63,14 @@
     try:
         yield tqdm_object
     finally:
         joblib.parallel.BatchCompletionCallBack = old_batch_callback
         tqdm_object.close()
 
 
-
-
-
-
-
-
 def get_distributions():
     distributions = []
     for this in dir(scipy.stats):
         if "fit" in eval("dir(scipy.stats." + this + ")"):
             distributions.append(this)
     return distributions
 
@@ -130,23 +123,31 @@
 
         >>> # just a trick to use only 10 distributions instead of 80 to speed up the fitting
         >>> f.distributions = f.distributions[0:10] + ['gamma']
 
         >>> # fit and plot
         >>> f.fit()
         >>> f.summary()
-                sumsquare_error
-        gamma          0.000095
-        beta           0.000179
-        chi            0.012247
-        cauchy         0.044443
-        anglit         0.051672
-        [5 rows x 1 columns]
 
-    Once the data has been fitted, the :meth:`summary` metod returns a sorted dataframe where the
+                      sumsquare_error     aic            bic     kl_div  ks_statistic  ks_pvalue
+        loggamma            0.001176  995.866732 -159536.164644     inf      0.008459   0.469031
+        gennorm             0.001181  993.145832 -159489.437372     inf      0.006833   0.736164
+        norm                0.001189  992.975187 -159427.247523     inf      0.007138   0.685416
+        truncnorm           0.001189  996.975182 -159408.826771     inf      0.007138   0.685416
+        crystalball         0.001189  996.975078 -159408.821960     inf      0.007138   0.685434
+
+    Once the data has been fitted, the :meth:`summary` method returns a sorted dataframe where 
+    the index represents the distribution names. 
+
+    The AIC is computed using :math:`aic = 2 * k - 2 * log(Lik)`,
+    and the BIC is computed as :math:`k * log(n) - 2 * log(Lik)`.
+
+
+    where Lik is the maximized value of the likelihood function of the model, 
+    n the number of data point and k the number of parameter.
 
     Looping over the 80 distributions in SciPy could takes some times so you can overwrite the
     :attr:`distributions` with a subset if you want. In order to reload all distributions,
     call :meth:`load_all_distributions`.
 
     Some distributions do not converge when fitting. There is a timeout of 30 seconds after which
     the fitting procedure is cancelled. You can change this :attr:`timeout` attribute if needed.
@@ -233,15 +234,15 @@
         self._fitted_errors = {}
         self._aic = {}
         self._bic = {}
         self._kldiv = {}
         self._ks_stat = {}
         self._ks_pval = {}
         self._fit_i = 0  # fit progress
-        #self.pb = None
+        # self.pb = None
 
     def _update_data_pdf(self):
         # histogram retuns X with N+1 values. So, we rearrange the X output into only N
         self.y, self.x = np.histogram(self._data, bins=self.bins, density=self._density)
         self.x = [(this + self.x[i + 1]) / 2.0 for i, this in enumerate(self.x[0:-1])]
 
     def _trim_data(self):
@@ -319,15 +320,19 @@
             sq_error = pylab.sum((self.fitted_pdf[distribution] - self.y) ** 2)
 
             # calculate information criteria
             logLik = np.sum(dist.logpdf(self.x, *param))
             k = len(param[:])
             n = len(self._data)
             aic = 2 * k - 2 * logLik
-            bic = n * np.log(sq_error / n) + k * np.log(n)
+
+            # special case of gaussian distribution
+            #bic = n * np.log(sq_error / n) + k * np.log(n)
+            # general case:
+            bic = k * pylab.log(n) - 2 * logLik
 
             # calculate kullback leibler divergence
             kullback_leibler = kl_div(self.fitted_pdf[distribution], self.y)
 
             # calculate goodness-of-fit statistic
             dist_fitted = dist(*param)
             ks_stat, ks_pval = kstest(self._data, dist_fitted.cdf)
@@ -364,17 +369,18 @@
 
         """
         import warnings
 
         warnings.filterwarnings("ignore", category=RuntimeWarning)
 
         N = len(self.distributions)
-        with tqdm_joblib(desc=f"Fitting {N} distributions", total=N) as progress_bar:
-            Parallel(n_jobs=max_workers, backend='threading')(delayed(self._fit_single_distribution)(dist) for dist in self.distributions)
-
+        with tqdm_joblib(desc=f"Fitting {N} distributions", total=N, disable=not progress) as progress_bar:
+            Parallel(n_jobs=max_workers, backend="threading")(
+                delayed(self._fit_single_distribution)(dist) for dist in self.distributions
+            )
 
         self.df_errors = pd.DataFrame(
             {
                 "sumsquare_error": self._fitted_errors,
                 "aic": self._aic,
                 "bic": self._bic,
                 "kl_div": self._kldiv,
@@ -429,15 +435,15 @@
 
         param_dict = {}
         for d_key, d_val in zip(param_names, params):
             param_dict[d_key] = d_val
         return {name: param_dict}
 
     def summary(self, Nbest=5, lw=2, plot=True, method="sumsquare_error", clf=True):
-        """Plots the distribution of the data and Nbest distribution"""
+        """Plots the distribution of the data and N best distributions"""
         if plot:
             if clf:
                 pylab.clf()
             self.hist()
             self.plot_pdf(Nbest=Nbest, lw=lw, method=method)
             pylab.grid(True)
```

### Comparing `fitter-1.5.2/src/fitter/histfit.py` & `fitter-1.6.0/src/fitter/histfit.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,23 +3,21 @@
 from pylab import mean, sqrt, std
 
 
 __all__ = ["HistFit"]
 
 
 class HistFit:
-    """Plot the histogram of the data (barplot) and the fitted histogram.
+    """Plot the histogram of the data (barplot) and the fitted histogram (gaussian case only)
 
     The input data can be a series. In this case, we compute the histogram.
     Then, we fit a curve on top on the histogram that best fit the histogram.
 
-    If you already have the histogram, you can provide the arguments.
-    In this case, X should be evenly spaced
-
-
+    If you already have the histogram, you can provide the density function..
+    In such case, we assume the data to be evenly spaced from 1 to N.
 
     If you have some data, histogram is computed, then we add some noise during
     the fitting process and repeat the process Nfit=20 times. This gives us a
     better estimate of the underlying mu and sigma parameters of the distribution.
 
     .. plot::
```

### Comparing `fitter-1.5.2/src/fitter/main.py` & `fitter-1.6.0/src/fitter/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,27 +36,31 @@
 def main():  # pragma: no cover
     """This is the main help"""
     pass
 
 
 @main.command()
 @click.argument("filename", type=click.STRING)
-@click.option("--column-number", type=click.INT, default=1)
-@click.option("--delimiter", type=click.STRING, default=",", help="look at the first column")
+@click.option("--column-number", type=click.INT, default=1, help="data column to use (first column by default)")
+@click.option("--delimiter", type=click.STRING, default=",", help="column delimiter (comma by default)")
 @click.option(
     "--distributions",
     type=click.STRING,
     default="gamma,beta",
-    help="llist of distribution",
+    help="list of distribution",
 )
 @click.option("--tag", type=click.STRING, default="fitter", help="tag to name output files")
 @click.option("--progress/--no-progress", default=True)
 @click.option("--verbose/--no-verbose", default=True)
 def fitdist(**kwargs):
-    """"""
+    """
+
+    fitter fitdist data.csv
+
+    """
     import csv
 
     col = kwargs["column_number"]
     with open(kwargs["filename"], "r") as csvfile:
         data = csv.reader(csvfile, delimiter=kwargs["delimiter"])
         data = [float(x[col - 1]) for x in data]
 
@@ -85,16 +89,17 @@
     msg = f"Fitter version {version}\nBest fit is {bestname} distribution\nparameters: "
     msg += f"{values}\n The parameters have to be used in that order in scipy"
     if kwargs["verbose"]:
         print(msg)
     with open("{}.log".format(tag), "w") as fout:
         fout.write(msg)
 
+
 @main.command()
 def show_distributions(**kwargs):
     from fitter import get_distributions
-    print("\n".join(get_distributions()))
 
+    print("\n".join(get_distributions()))
 
 
 if __name__ == "__main__":  # pragma: no cover
     main()
```

### Comparing `fitter-1.5.2/src/fitter.egg-info/PKG-INFO` & `fitter-1.6.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,175 +1,44 @@
-Metadata-Version: 1.2
-Name: fitter
-Version: 1.5.2
-Summary: A tool to fit data to many distributions and best one(s)
-Home-page: https://github.com/cokelaer/fitter
-Author: Thomas Cokelaer
-Author-email: cokelaer@gmail.com
-Maintainer: Thomas Cokelaer
-Maintainer-email: cokelaer@gmail.com
-License: GPL
-Download-URL: https://github.com/cokelaer/fitter
-Description: 
-        
-        #############################
-        FITTER documentation
-        #############################
-        
-        .. image:: https://badge.fury.io/py/fitter.svg
-            :target: https://pypi.python.org/pypi/fitter
-        
-        .. image:: https://github.com/cokelaer/fitter/actions/workflows/main.yml/badge.svg?branch=main
-            :target: https://github.com/cokelaer/fitter/actions/workflows/main.yml
-        
-        .. image:: https://coveralls.io/repos/cokelaer/fitter/badge.png?branch=main
-            :target: https://coveralls.io/r/cokelaer/fitter?branch=main
-        
-        .. image:: http://readthedocs.org/projects/fitter/badge/?version=latest
-            :target: http://fitter.readthedocs.org/en/latest/?badge=latest
-            :alt: Documentation Status
-        
-        .. image:: https://zenodo.org/badge/23078551.svg
-           :target: https://zenodo.org/badge/latestdoi/23078551
-        
-        Compatible with Python 3.7, and 3.8, 3.9
-        
-        
-        What is it ?
-        ################
-        
-        **fitter** package provides a simple class to identify the distribution from which a data samples 
-        is generated from. It uses 80 distributions from Scipy and allows you to plot the results to check 
-        what is the most probable distribution and the best parameters.
-        
-        
-        Installation
-        ###################
-        
-        ::
-        
-            pip install fitter
-        
-        **fitter** is also available on **conda** (bioconda channel)::
-         
-             conda install fitter
-        
-        
-        Usage
-        ##################
-        
-        standalone
-        ===========
-        
-        A standalone application (very simple) is also provided and works with input CSV
-        files::
-          
-            fitter fitdist data.csv --column-number 1 --distributions gamma,normal
-         
-        It creates a file called fitter.png and a log fitter.log
-        
-        From Python shell
-        ==================
-        
-        First, let us create a data samples with N = 10,000 points from a gamma distribution::
-        
-            from scipy import stats
-            data = stats.gamma.rvs(2, loc=1.5, scale=2, size=10000)
-        
-        .. note:: the fitting is slow so keep the size value to reasonable value.
-        
-        Now, without any knowledge about the distribution or its parameter, what is the distribution that fits the data best ? Scipy has 80 distributions and the **Fitter** class will scan all of them, call the fit function for you, ignoring those that fail or run forever and finally give you a summary of the best distributions in the sense of sum of the square errors. The best is to give an example::
-        
-        
-            from fitter import Fitter
-            f = Fitter(data)
-            f.fit()
-            # may take some time since by default, all distributions are tried
-            # but you call manually provide a smaller set of distributions 
-            f.summary()
-        
-        
-        .. image:: http://pythonhosted.org/fitter/_images/index-1.png
-            :target: http://pythonhosted.org/fitter/_images/index-1.png
-        
-        
-        See the `online <http://fitter.readthedocs.io/>`_ documentation for details.
-        
-        
-        Contributors
-        =============
-        
-        
-        Setting up and maintaining Fitter has been possible thanks to users and contributors.
-        Thanks to all:
-        
-        .. image:: https://contrib.rocks/image?repo=cokelaer/fitter
-            :target: https://github.com/cokelaer/fitter/graphs/contributors
-        
-        
-        
-        
-        Changelog
-        ~~~~~~~~~
-        ========= ==========================================================================
-        Version   Description
-        ========= ==========================================================================
-        1.5.2     * PR https://github.com/cokelaer/fitter/pull/74 to fix logger
-        1.5.1     * fixed regression putting back joblib
-        1.5.0     * removed easydev and replaced by tqdm for progress bar
-                  * progressbar from tqdm also allows replacement of joblib need
-        1.4.1     * Update timeout in docs from 10 to 30 seconds by @mpadge in 
-                    https://github.com/cokelaer/fitter/pull/47
-                  * Add Kolmogorov-Smirnov goodness-of-fit statistic by @lahdjirayhan in 
-                    https://github.com/cokelaer/fitter/pull/58
-                  * switch branch from master to main
-        1.4.0     * get_best function now returns the parameters as a dictionary 
-                    of parameter names and their values rather than just a list of
-                    values (https://github.com/cokelaer/fitter/issues/23) thanks to 
-                    contributor @kabirmdasraful
-                  * Accepting PR to fix progress bar issue reported in 
-                    https://github.com/cokelaer/fitter/pull/37
-        1.3.0     * parallel process implemented https://github.com/cokelaer/fitter/pull/25
-                    thanks to @arsenyinfo 
-        1.2.3     * remove vervose arguments in Fitter class. Using the logging module 
-                    instead
-                  * the Fitter.fit has now a progress bar
-                  * add a standalone application called … fitter (see the doc)
-        1.2.2     was not released
-        1.2.1     adding new class called histfit (see documentation)
-        1.2       * Fixed the version. Previous version switched from 
-                    1.0.9 to 1.1.11. To start a fresh version, we increase to 1.2.0
-                  * Merged pull request required by bioconda
-                  * Merged pull request related to implementation of 
-                    AIC/BIC/KL criteria (https://github.com/cokelaer/fitter/pull/19). 
-                    This also fixes https://github.com/cokelaer/fitter/issues/9
-                  * Implement two functions to get all distributions, or a list of 
-                    common distributions to help users decreading computational time 
-                    (https://github.com/cokelaer/fitter/issues/20). Also added a FAQS 
-                    section.
-                  * travis tested Python 3.6 and 3.7 (not 3.5 anymore)
-        1.1       * Fixed deprecated warning
-                  * fitter is now in readthedocs at fitter.readthedocs.io
-        1.0.9     * https://github.com/cokelaer/fitter/pull/8 and 11
-                    PR https://github.com/cokelaer/fitter/pull/8
-        1.0.6     * summary() now returns the dataframe (instead of printing it)
-        1.0.5      https://github.com/cokelaer/fitter/issues
-        1.0.2     add manifest to fix missing source in the pypi repository.
-        ========= ==========================================================================
-        
-        
-        
-        
-        
-Keywords: fit,distribution,fitting,scipy
-Platform: Linux
-Platform: Unix
-Platform: MacOsX
-Platform: Windows
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
+# -*- coding: utf-8 -*-
+from setuptools import setup
+
+package_dir = \
+{'': 'src'}
+
+packages = \
+['fitter']
+
+package_data = \
+{'': ['*']}
+
+install_requires = \
+['click>=8.1.6,<9.0.0',
+ 'joblib>=1.3.1,<2.0.0',
+ 'matplotlib>=3.7.2',
+ 'numpy>=1.20',
+ 'pandas>=2.0.3,<3.0.0',
+ 'scipy>=0.18',
+ 'tqdm>=4.65.1,<5.0.0']
+
+entry_points = \
+{'console_scripts': ['fitter = fitter.main:main']}
+
+setup_kwargs = {
+    'name': 'fitter',
+    'version': '1.6.0',
+    'description': 'A tool to fit data to many distributions and get the best one(s)',
+    'long_description': '\n\n#############################\nFITTER documentation\n#############################\n\n.. image:: https://badge.fury.io/py/fitter.svg\n    :target: https://pypi.python.org/pypi/fitter\n\n.. image:: https://github.com/cokelaer/fitter/actions/workflows/main.yml/badge.svg?branch=main\n    :target: https://github.com/cokelaer/fitter/actions/workflows/main.yml\n\n.. image:: https://coveralls.io/repos/cokelaer/fitter/badge.png?branch=main\n    :target: https://coveralls.io/r/cokelaer/fitter?branch=main\n\n.. image:: http://readthedocs.org/projects/fitter/badge/?version=latest\n    :target: http://fitter.readthedocs.org/en/latest/?badge=latest\n    :alt: Documentation Status\n\n.. image:: https://zenodo.org/badge/23078551.svg\n   :target: https://zenodo.org/badge/latestdoi/23078551\n\nCompatible with Python 3.7, and 3.8, 3.9\n\n\nWhat is it ?\n################\n\nThe **fitter** package is a Python library used for fitting probability distributions to data. It provides a straightforward and and intuitive interface to estimate parameters for various types of distributions, both continuous and discrete. Using **fitter**, you can easily fit a range of distributions to your data and compare their fit, aiding in the selection of the most suitable distribution. The package is designed to be user-friendly and requires minimal setup, making it a useful tool for data scientists and statisticians working with probability distributions.\n\nInstallation\n###################\n\n::\n\n    pip install fitter\n\n**fitter** is also available on **conda** (bioconda channel)::\n \n     conda install fitter\n\n\nUsage\n##################\n\nstandalone\n===========\n\nA standalone application (very simple) is also provided and works with input CSV\nfiles::\n  \n    fitter fitdist data.csv --column-number 1 --distributions gamma,normal\n \nIt creates a file called fitter.png and a log fitter.log\n\nFrom Python shell\n==================\n\nFirst, let us create a data samples with N = 10,000 points from a gamma distribution::\n\n    from scipy import stats\n    data = stats.gamma.rvs(2, loc=1.5, scale=2, size=10000)\n\n.. note:: the fitting is slow so keep the size value to reasonable value.\n\nNow, without any knowledge about the distribution or its parameter, what is the distribution that fits the data best ? Scipy has 80 distributions and the **Fitter** class will scan all of them, call the fit function for you, ignoring those that fail or run forever and finally give you a summary of the best distributions in the sense of sum of the square errors. The best is to give an example::\n\n\n    from fitter import Fitter\n    f = Fitter(data)\n    f.fit()\n    # may take some time since by default, all distributions are tried\n    # but you call manually provide a smaller set of distributions \n    f.summary()\n\n\n.. image:: http://pythonhosted.org/fitter/_images/index-1.png\n    :target: http://pythonhosted.org/fitter/_images/index-1.png\n\n\nSee the `online <http://fitter.readthedocs.io/>`_ documentation for details.\n\n\nContributors\n=============\n\n\nSetting up and maintaining Fitter has been possible thanks to users and contributors.\nThanks to all:\n\n.. image:: https://contrib.rocks/image?repo=cokelaer/fitter\n    :target: https://github.com/cokelaer/fitter/graphs/contributors\n\n\n\n\nChangelog\n~~~~~~~~~\n========= ==========================================================================\nVersion   Description\n========= ==========================================================================\n1.6.0     * for developers: uses pyproject.toml instead of setup.py\n          * Fix progress bar fixing https://github.com/cokelaer/fitter/pull/74\n          * Fix BIC formula https://github.com/cokelaer/fitter/pull/77\n1.5.2     * PR https://github.com/cokelaer/fitter/pull/74 to fix logger\n1.5.1     * fixed regression putting back joblib\n1.5.0     * removed easydev and replaced by tqdm for progress bar\n          * progressbar from tqdm also allows replacement of joblib need\n1.4.1     * Update timeout in docs from 10 to 30 seconds by @mpadge in \n            https://github.com/cokelaer/fitter/pull/47\n          * Add Kolmogorov-Smirnov goodness-of-fit statistic by @lahdjirayhan in \n            https://github.com/cokelaer/fitter/pull/58\n          * switch branch from master to main\n1.4.0     * get_best function now returns the parameters as a dictionary \n            of parameter names and their values rather than just a list of\n            values (https://github.com/cokelaer/fitter/issues/23) thanks to \n            contributor @kabirmdasraful\n          * Accepting PR to fix progress bar issue reported in \n            https://github.com/cokelaer/fitter/pull/37\n1.3.0     * parallel process implemented https://github.com/cokelaer/fitter/pull/25\n            thanks to @arsenyinfo \n1.2.3     * remove vervose arguments in Fitter class. Using the logging module \n            instead\n          * the Fitter.fit has now a progress bar\n          * add a standalone application called … fitter (see the doc)\n1.2.2     was not released\n1.2.1     adding new class called histfit (see documentation)\n1.2       * Fixed the version. Previous version switched from \n            1.0.9 to 1.1.11. To start a fresh version, we increase to 1.2.0\n          * Merged pull request required by bioconda\n          * Merged pull request related to implementation of \n            AIC/BIC/KL criteria (https://github.com/cokelaer/fitter/pull/19). \n            This also fixes https://github.com/cokelaer/fitter/issues/9\n          * Implement two functions to get all distributions, or a list of \n            common distributions to help users decreading computational time \n            (https://github.com/cokelaer/fitter/issues/20). Also added a FAQS \n            section.\n          * travis tested Python 3.6 and 3.7 (not 3.5 anymore)\n1.1       * Fixed deprecated warning\n          * fitter is now in readthedocs at fitter.readthedocs.io\n1.0.9     * https://github.com/cokelaer/fitter/pull/8 and 11\n            PR https://github.com/cokelaer/fitter/pull/8\n1.0.6     * summary() now returns the dataframe (instead of printing it)\n1.0.5      https://github.com/cokelaer/fitter/issues\n1.0.2     add manifest to fix missing source in the pypi repository.\n========= ==========================================================================\n\n\n\n\n',
+    'author': 'Thomas Cokelaer',
+    'author_email': 'cokelaer@gmail.com',
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
+    'package_dir': package_dir,
+    'packages': packages,
+    'package_data': package_data,
+    'install_requires': install_requires,
+    'entry_points': entry_points,
+    'python_requires': '>=3.8,<4.0',
+}
+
+
+setup(**setup_kwargs)
```

