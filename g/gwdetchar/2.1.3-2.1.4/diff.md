# Comparing `tmp/gwdetchar-2.1.3.tar.gz` & `tmp/gwdetchar-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwdetchar-2.1.3.tar", last modified: Fri Aug  4 22:14:23 2023, max compression
+gzip compressed data, was "gwdetchar-2.1.4.tar", last modified: Wed Aug  9 00:44:40 2023, max compression
```

## Comparing `gwdetchar-2.1.3.tar` & `gwdetchar-2.1.4.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.508633 gwdetchar-2.1.3/
--rw-r--r--   0 egoetz     (501) staff       (20)      184 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/.codecov.yml
--rw-r--r--   0 egoetz     (501) staff       (20)      134 2023-06-16 22:43:20.000000 gwdetchar-2.1.3/.flake8
--rw-r--r--   0 egoetz     (501) staff       (20)       35 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/.gitattributes
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.440055 gwdetchar-2.1.3/.github/
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.454956 gwdetchar-2.1.3/.github/workflows/
--rw-r--r--   0 egoetz     (501) staff       (20)     2885 2023-06-16 22:43:20.000000 gwdetchar-2.1.3/.github/workflows/build.yml
--rw-r--r--   0 egoetz     (501) staff       (20)     1334 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/.github/workflows/docs.yml
--rw-r--r--   0 egoetz     (501) staff       (20)     1377 2023-06-28 17:53:22.000000 gwdetchar-2.1.3/.github/workflows/lint.yml
--rw-r--r--   0 egoetz     (501) staff       (20)      617 2023-06-16 22:43:20.000000 gwdetchar-2.1.3/.gitignore
--rw-r--r--   0 egoetz     (501) staff       (20)      525 2023-06-28 17:53:22.000000 gwdetchar-2.1.3/.readthedocs.yml
--rw-r--r--   0 egoetz     (501) staff       (20)     2638 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/CONTRIBUTING.md
--rw-r--r--   0 egoetz     (501) staff       (20)    35147 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/LICENSE
--rw-r--r--   0 egoetz     (501) staff       (20)       69 2023-06-16 22:43:20.000000 gwdetchar-2.1.3/MANIFEST.in
--rw-r--r--   0 egoetz     (501) staff       (20)     3726 2023-08-04 22:14:23.508179 gwdetchar-2.1.3/PKG-INFO
--rw-r--r--   0 egoetz     (501) staff       (20)     2328 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/README.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.455667 gwdetchar-2.1.3/ci/
--rw-r--r--   0 egoetz     (501) staff       (20)     1135 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/ci/test-cli.sh
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.457642 gwdetchar-2.1.3/docs/
--rw-r--r--   0 egoetz     (501) staff       (20)     6857 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/docs/Makefile
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.440757 gwdetchar-2.1.3/docs/_static/
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.458463 gwdetchar-2.1.3/docs/_static/css/
--rw-r--r--   0 egoetz     (501) staff       (20)     4997 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/docs/_static/css/custom.css
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.458943 gwdetchar-2.1.3/docs/api/
--rw-r--r--   0 egoetz     (501) staff       (20)       54 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/docs/api/index.rst
--rw-r--r--   0 egoetz     (501) staff       (20)    10994 2023-06-16 22:43:20.000000 gwdetchar-2.1.3/docs/conf.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.459526 gwdetchar-2.1.3/docs/conlog/
--rw-r--r--   0 egoetz     (501) staff       (20)      964 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/docs/conlog/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.460354 gwdetchar-2.1.3/docs/daq/
--rw-r--r--   0 egoetz     (501) staff       (20)     1807 2023-06-16 22:43:20.000000 gwdetchar-2.1.3/docs/daq/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.460951 gwdetchar-2.1.3/docs/data/
--rw-r--r--   0 egoetz     (501) staff       (20)      863 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/docs/data/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.461486 gwdetchar-2.1.3/docs/html/
--rw-r--r--   0 egoetz     (501) staff       (20)     1488 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/docs/html/index.rst
--rw-r--r--   0 egoetz     (501) staff       (20)     2968 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/docs/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.462069 gwdetchar-2.1.3/docs/lasso/
--rw-r--r--   0 egoetz     (501) staff       (20)     1439 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/docs/lasso/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.462613 gwdetchar-2.1.3/docs/nagios/
--rw-r--r--   0 egoetz     (501) staff       (20)      941 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/docs/nagios/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.463143 gwdetchar-2.1.3/docs/omega/
--rw-r--r--   0 egoetz     (501) staff       (20)     3035 2023-06-16 22:43:20.000000 gwdetchar-2.1.3/docs/omega/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.463539 gwdetchar-2.1.3/docs/saturation/
--rw-r--r--   0 egoetz     (501) staff       (20)     1638 2023-06-16 22:43:20.000000 gwdetchar-2.1.3/docs/saturation/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.463922 gwdetchar-2.1.3/docs/scattering/
--rw-r--r--   0 egoetz     (501) staff       (20)     2926 2023-06-16 22:43:20.000000 gwdetchar-2.1.3/docs/scattering/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.470661 gwdetchar-2.1.3/gwdetchar/
--rw-r--r--   0 egoetz     (501) staff       (20)     1408 2023-06-16 22:43:20.000000 gwdetchar-2.1.3/gwdetchar/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)      160 2023-08-04 22:14:23.000000 gwdetchar-2.1.3/gwdetchar/_version.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3732 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/cds.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4738 2023-05-16 23:56:26.000000 gwdetchar-2.1.3/gwdetchar/cli.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2773 2023-04-25 15:49:41.000000 gwdetchar-2.1.3/gwdetchar/condor.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2703 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/conftest.py
--rw-r--r--   0 egoetz     (501) staff       (20)     7363 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/conlog.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2997 2023-05-17 00:05:55.000000 gwdetchar-2.1.3/gwdetchar/const.py
--rw-r--r--   0 egoetz     (501) staff       (20)     7440 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/daq.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.475402 gwdetchar-2.1.3/gwdetchar/io/
--rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/io/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     7584 2023-06-19 18:12:55.000000 gwdetchar-2.1.3/gwdetchar/io/datafind.py
--rw-r--r--   0 egoetz     (501) staff       (20)    41413 2023-06-16 22:43:20.000000 gwdetchar-2.1.3/gwdetchar/io/html.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3764 2023-06-19 18:12:55.000000 gwdetchar-2.1.3/gwdetchar/io/ligolw.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.478542 gwdetchar-2.1.3/gwdetchar/io/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      827 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/io/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4834 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/io/tests/test_datafind.py
--rw-r--r--   0 egoetz     (501) staff       (20)    24146 2023-06-16 22:43:20.000000 gwdetchar-2.1.3/gwdetchar/io/tests/test_html.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2451 2023-06-19 18:12:55.000000 gwdetchar-2.1.3/gwdetchar/io/tests/test_ligolw.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.483087 gwdetchar-2.1.3/gwdetchar/lasso/
--rw-r--r--   0 egoetz     (501) staff       (20)     1063 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/lasso/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    50279 2023-08-04 18:20:44.000000 gwdetchar-2.1.3/gwdetchar/lasso/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6652 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/lasso/core.py
--rw-r--r--   0 egoetz     (501) staff       (20)    20595 2022-10-03 17:36:21.000000 gwdetchar-2.1.3/gwdetchar/lasso/old.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4946 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/lasso/plot.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.486941 gwdetchar-2.1.3/gwdetchar/lasso/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      830 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/lasso/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3984 2023-04-27 00:53:55.000000 gwdetchar-2.1.3/gwdetchar/lasso/tests/test_core.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1549 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/lasso/tests/test_main.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2142 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/lasso/tests/test_plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6744 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/mct.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.488297 gwdetchar-2.1.3/gwdetchar/nagios/
--rw-r--r--   0 egoetz     (501) staff       (20)      887 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/nagios/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2959 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/nagios/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2166 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/nagios/core.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.489067 gwdetchar-2.1.3/gwdetchar/nagios/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      826 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/nagios/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2131 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/nagios/tests/test_main.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.492846 gwdetchar-2.1.3/gwdetchar/omega/
--rw-r--r--   0 egoetz     (501) staff       (20)     1188 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/omega/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    14012 2023-08-04 18:20:44.000000 gwdetchar-2.1.3/gwdetchar/omega/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    12682 2023-05-16 23:56:26.000000 gwdetchar-2.1.3/gwdetchar/omega/batch.py
--rw-r--r--   0 egoetz     (501) staff       (20)    15875 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/omega/config.py
--rw-r--r--   0 egoetz     (501) staff       (20)    10365 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/omega/core.py
--rw-r--r--   0 egoetz     (501) staff       (20)    20699 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/omega/html.py
--rw-r--r--   0 egoetz     (501) staff       (20)     8871 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/omega/plot.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.496633 gwdetchar-2.1.3/gwdetchar/omega/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      830 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/omega/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3689 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/omega/tests/test_batch.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6970 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/omega/tests/test_config.py
--rw-r--r--   0 egoetz     (501) staff       (20)     5493 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/omega/tests/test_core.py
--rw-r--r--   0 egoetz     (501) staff       (20)    13502 2023-06-16 22:43:20.000000 gwdetchar-2.1.3/gwdetchar/omega/tests/test_html.py
--rw-r--r--   0 egoetz     (501) staff       (20)     9824 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/omega/tests/test_main.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2702 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/omega/tests/test_plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)    17732 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/overflow.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2244 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/plot.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.498553 gwdetchar-2.1.3/gwdetchar/saturation/
--rw-r--r--   0 egoetz     (501) staff       (20)     1039 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/saturation/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    13870 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/saturation/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     7654 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/saturation/core.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.499333 gwdetchar-2.1.3/gwdetchar/saturation/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/saturation/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3510 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/saturation/tests/test_saturation.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.501452 gwdetchar-2.1.3/gwdetchar/scattering/
--rw-r--r--   0 egoetz     (501) staff       (20)     1983 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/scattering/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    32277 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/scattering/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6413 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/scattering/core.py
--rw-r--r--   0 egoetz     (501) staff       (20)     5282 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/scattering/plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)     8523 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/scattering/simple.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.503507 gwdetchar-2.1.3/gwdetchar/scattering/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/scattering/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2238 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/scattering/tests/test_core.py
--rw-r--r--   0 egoetz     (501) staff       (20)     5520 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/scattering/tests/test_main.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1831 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/scattering/tests/test_plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3156 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/scattering/tests/test_simple.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.507641 gwdetchar-2.1.3/gwdetchar/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      826 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3276 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/tests/test_cds.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3181 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/tests/test_cli.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1918 2023-04-25 15:49:41.000000 gwdetchar-2.1.3/gwdetchar/tests/test_condor.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4819 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/tests/test_conlog.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1928 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/tests/test_const.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3306 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/tests/test_daq.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2077 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/tests/test_plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2831 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/tests/test_utils.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4531 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/utils.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.473016 gwdetchar-2.1.3/gwdetchar.egg-info/
--rw-r--r--   0 egoetz     (501) staff       (20)     3726 2023-08-04 22:14:23.000000 gwdetchar-2.1.3/gwdetchar.egg-info/PKG-INFO
--rw-r--r--   0 egoetz     (501) staff       (20)     2832 2023-08-04 22:14:23.000000 gwdetchar-2.1.3/gwdetchar.egg-info/SOURCES.txt
--rw-r--r--   0 egoetz     (501) staff       (20)        1 2023-08-04 22:14:23.000000 gwdetchar-2.1.3/gwdetchar.egg-info/dependency_links.txt
--rw-r--r--   0 egoetz     (501) staff       (20)      591 2023-08-04 22:14:23.000000 gwdetchar-2.1.3/gwdetchar.egg-info/entry_points.txt
--rw-r--r--   0 egoetz     (501) staff       (20)      356 2023-08-04 22:14:23.000000 gwdetchar-2.1.3/gwdetchar.egg-info/requires.txt
--rw-r--r--   0 egoetz     (501) staff       (20)       10 2023-08-04 22:14:23.000000 gwdetchar-2.1.3/gwdetchar.egg-info/top_level.txt
--rw-r--r--   0 egoetz     (501) staff       (20)     3465 2023-08-04 22:13:43.000000 gwdetchar-2.1.3/pyproject.toml
--rw-r--r--   0 egoetz     (501) staff       (20)       38 2023-08-04 22:14:23.508761 gwdetchar-2.1.3/setup.cfg
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-09 00:44:40.754695 gwdetchar-2.1.4/
+-rw-r--r--   0 egoetz     (501) staff       (20)      184 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/.codecov.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)      134 2023-06-16 22:43:20.000000 gwdetchar-2.1.4/.flake8
+-rw-r--r--   0 egoetz     (501) staff       (20)       35 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/.gitattributes
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-09 00:44:40.687961 gwdetchar-2.1.4/.github/
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-09 00:44:40.701260 gwdetchar-2.1.4/.github/workflows/
+-rw-r--r--   0 egoetz     (501) staff       (20)     2885 2023-06-16 22:43:20.000000 gwdetchar-2.1.4/.github/workflows/build.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)     1334 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/.github/workflows/docs.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)     1377 2023-06-28 17:53:22.000000 gwdetchar-2.1.4/.github/workflows/lint.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)      617 2023-06-16 22:43:20.000000 gwdetchar-2.1.4/.gitignore
+-rw-r--r--   0 egoetz     (501) staff       (20)      525 2023-06-28 17:53:22.000000 gwdetchar-2.1.4/.readthedocs.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)     2638 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/CONTRIBUTING.md
+-rw-r--r--   0 egoetz     (501) staff       (20)    35147 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/LICENSE
+-rw-r--r--   0 egoetz     (501) staff       (20)       69 2023-06-16 22:43:20.000000 gwdetchar-2.1.4/MANIFEST.in
+-rw-r--r--   0 egoetz     (501) staff       (20)     3726 2023-08-09 00:44:40.754364 gwdetchar-2.1.4/PKG-INFO
+-rw-r--r--   0 egoetz     (501) staff       (20)     2328 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/README.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-09 00:44:40.701884 gwdetchar-2.1.4/ci/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1135 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/ci/test-cli.sh
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-09 00:44:40.703578 gwdetchar-2.1.4/docs/
+-rw-r--r--   0 egoetz     (501) staff       (20)     6857 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/docs/Makefile
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-09 00:44:40.688642 gwdetchar-2.1.4/docs/_static/
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-09 00:44:40.704225 gwdetchar-2.1.4/docs/_static/css/
+-rw-r--r--   0 egoetz     (501) staff       (20)     4997 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/docs/_static/css/custom.css
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-09 00:44:40.704822 gwdetchar-2.1.4/docs/api/
+-rw-r--r--   0 egoetz     (501) staff       (20)       54 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/docs/api/index.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)    10994 2023-06-16 22:43:20.000000 gwdetchar-2.1.4/docs/conf.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-09 00:44:40.705401 gwdetchar-2.1.4/docs/conlog/
+-rw-r--r--   0 egoetz     (501) staff       (20)      964 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/docs/conlog/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-09 00:44:40.706194 gwdetchar-2.1.4/docs/daq/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1807 2023-06-16 22:43:20.000000 gwdetchar-2.1.4/docs/daq/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-09 00:44:40.706757 gwdetchar-2.1.4/docs/data/
+-rw-r--r--   0 egoetz     (501) staff       (20)      863 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/docs/data/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-09 00:44:40.707246 gwdetchar-2.1.4/docs/html/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1488 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/docs/html/index.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)     2968 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/docs/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-09 00:44:40.707662 gwdetchar-2.1.4/docs/lasso/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1439 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/docs/lasso/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-09 00:44:40.708142 gwdetchar-2.1.4/docs/nagios/
+-rw-r--r--   0 egoetz     (501) staff       (20)      941 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/docs/nagios/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-09 00:44:40.708613 gwdetchar-2.1.4/docs/omega/
+-rw-r--r--   0 egoetz     (501) staff       (20)     3035 2023-06-16 22:43:20.000000 gwdetchar-2.1.4/docs/omega/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-09 00:44:40.709249 gwdetchar-2.1.4/docs/saturation/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1638 2023-06-16 22:43:20.000000 gwdetchar-2.1.4/docs/saturation/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-09 00:44:40.709738 gwdetchar-2.1.4/docs/scattering/
+-rw-r--r--   0 egoetz     (501) staff       (20)     2926 2023-06-16 22:43:20.000000 gwdetchar-2.1.4/docs/scattering/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-09 00:44:40.716819 gwdetchar-2.1.4/gwdetchar/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1408 2023-06-16 22:43:20.000000 gwdetchar-2.1.4/gwdetchar/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)      160 2023-08-09 00:44:40.000000 gwdetchar-2.1.4/gwdetchar/_version.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3732 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/cds.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4738 2023-05-16 23:56:26.000000 gwdetchar-2.1.4/gwdetchar/cli.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2773 2023-04-25 15:49:41.000000 gwdetchar-2.1.4/gwdetchar/condor.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2703 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/conftest.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     7363 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/conlog.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2997 2023-05-17 00:05:55.000000 gwdetchar-2.1.4/gwdetchar/const.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     7440 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/daq.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-09 00:44:40.721192 gwdetchar-2.1.4/gwdetchar/io/
+-rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/io/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     7584 2023-06-19 18:12:55.000000 gwdetchar-2.1.4/gwdetchar/io/datafind.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    41413 2023-06-16 22:43:20.000000 gwdetchar-2.1.4/gwdetchar/io/html.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3764 2023-06-19 18:12:55.000000 gwdetchar-2.1.4/gwdetchar/io/ligolw.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-09 00:44:40.724103 gwdetchar-2.1.4/gwdetchar/io/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      827 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/io/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4834 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/io/tests/test_datafind.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    24146 2023-06-16 22:43:20.000000 gwdetchar-2.1.4/gwdetchar/io/tests/test_html.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2451 2023-06-19 18:12:55.000000 gwdetchar-2.1.4/gwdetchar/io/tests/test_ligolw.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-09 00:44:40.727368 gwdetchar-2.1.4/gwdetchar/lasso/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1063 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/lasso/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    50249 2023-08-09 00:41:53.000000 gwdetchar-2.1.4/gwdetchar/lasso/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6652 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/lasso/core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    20595 2022-10-03 17:36:21.000000 gwdetchar-2.1.4/gwdetchar/lasso/old.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4946 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/lasso/plot.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-09 00:44:40.730215 gwdetchar-2.1.4/gwdetchar/lasso/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      830 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/lasso/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3984 2023-04-27 00:53:55.000000 gwdetchar-2.1.4/gwdetchar/lasso/tests/test_core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1549 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/lasso/tests/test_main.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2142 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/lasso/tests/test_plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6744 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/mct.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-09 00:44:40.732185 gwdetchar-2.1.4/gwdetchar/nagios/
+-rw-r--r--   0 egoetz     (501) staff       (20)      887 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/nagios/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2959 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/nagios/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2166 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/nagios/core.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-09 00:44:40.733535 gwdetchar-2.1.4/gwdetchar/nagios/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      826 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/nagios/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2131 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/nagios/tests/test_main.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-09 00:44:40.739042 gwdetchar-2.1.4/gwdetchar/omega/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1188 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/omega/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    14012 2023-08-04 18:20:44.000000 gwdetchar-2.1.4/gwdetchar/omega/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    12682 2023-05-16 23:56:26.000000 gwdetchar-2.1.4/gwdetchar/omega/batch.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    15875 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/omega/config.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    10365 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/omega/core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    20699 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/omega/html.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     8871 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/omega/plot.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-09 00:44:40.742992 gwdetchar-2.1.4/gwdetchar/omega/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      830 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/omega/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3689 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/omega/tests/test_batch.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6970 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/omega/tests/test_config.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     5493 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/omega/tests/test_core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    13502 2023-06-16 22:43:20.000000 gwdetchar-2.1.4/gwdetchar/omega/tests/test_html.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     9824 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/omega/tests/test_main.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2702 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/omega/tests/test_plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    17732 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/overflow.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2244 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/plot.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-09 00:44:40.744709 gwdetchar-2.1.4/gwdetchar/saturation/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1039 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/saturation/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    13870 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/saturation/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     7654 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/saturation/core.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-09 00:44:40.745599 gwdetchar-2.1.4/gwdetchar/saturation/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/saturation/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3510 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/saturation/tests/test_saturation.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-09 00:44:40.747865 gwdetchar-2.1.4/gwdetchar/scattering/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1983 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/scattering/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    32277 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/scattering/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6413 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/scattering/core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     5282 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/scattering/plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     8523 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/scattering/simple.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-09 00:44:40.749917 gwdetchar-2.1.4/gwdetchar/scattering/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/scattering/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2238 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/scattering/tests/test_core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     5520 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/scattering/tests/test_main.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1831 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/scattering/tests/test_plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3156 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/scattering/tests/test_simple.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-09 00:44:40.753827 gwdetchar-2.1.4/gwdetchar/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      826 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3276 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/tests/test_cds.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3181 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/tests/test_cli.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1918 2023-04-25 15:49:41.000000 gwdetchar-2.1.4/gwdetchar/tests/test_condor.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4819 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/tests/test_conlog.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1928 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/tests/test_const.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3306 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/tests/test_daq.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2077 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/tests/test_plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2831 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/tests/test_utils.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4531 2022-08-23 18:11:03.000000 gwdetchar-2.1.4/gwdetchar/utils.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-09 00:44:40.719129 gwdetchar-2.1.4/gwdetchar.egg-info/
+-rw-r--r--   0 egoetz     (501) staff       (20)     3726 2023-08-09 00:44:40.000000 gwdetchar-2.1.4/gwdetchar.egg-info/PKG-INFO
+-rw-r--r--   0 egoetz     (501) staff       (20)     2832 2023-08-09 00:44:40.000000 gwdetchar-2.1.4/gwdetchar.egg-info/SOURCES.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)        1 2023-08-09 00:44:40.000000 gwdetchar-2.1.4/gwdetchar.egg-info/dependency_links.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)      591 2023-08-09 00:44:40.000000 gwdetchar-2.1.4/gwdetchar.egg-info/entry_points.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)      356 2023-08-09 00:44:40.000000 gwdetchar-2.1.4/gwdetchar.egg-info/requires.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)       10 2023-08-09 00:44:40.000000 gwdetchar-2.1.4/gwdetchar.egg-info/top_level.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)     3465 2023-08-04 22:13:43.000000 gwdetchar-2.1.4/pyproject.toml
+-rw-r--r--   0 egoetz     (501) staff       (20)       38 2023-08-09 00:44:40.754777 gwdetchar-2.1.4/setup.cfg
```

### Comparing `gwdetchar-2.1.3/.github/workflows/build.yml` & `gwdetchar-2.1.4/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/.github/workflows/docs.yml` & `gwdetchar-2.1.4/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/.github/workflows/lint.yml` & `gwdetchar-2.1.4/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/.gitignore` & `gwdetchar-2.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/.readthedocs.yml` & `gwdetchar-2.1.4/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/CONTRIBUTING.md` & `gwdetchar-2.1.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/LICENSE` & `gwdetchar-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/PKG-INFO` & `gwdetchar-2.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwdetchar
-Version: 2.1.3
+Version: 2.1.4
 Summary: A python package for gravitational-wave detector characterisation
 Author-email: Alex Urban <alex.urban@ligo.org>, Duncan Macleod <duncan.macleod@ligo.org>
 Maintainer-email: Evan Goetz <evan.goetz@ligo.org>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://gwdetchar.readthedocs.io
 Project-URL: Source Code, https://github.com/gwdetchar/gwdetchar
 Project-URL: Bug Tracker, https://github.com/gwdetchar/gwdetchar/issues
```

### Comparing `gwdetchar-2.1.3/README.rst` & `gwdetchar-2.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/ci/test-cli.sh` & `gwdetchar-2.1.4/ci/test-cli.sh`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/docs/Makefile` & `gwdetchar-2.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/docs/_static/css/custom.css` & `gwdetchar-2.1.4/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/docs/conf.py` & `gwdetchar-2.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/docs/conlog/index.rst` & `gwdetchar-2.1.4/docs/conlog/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/docs/daq/index.rst` & `gwdetchar-2.1.4/docs/daq/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/docs/data/index.rst` & `gwdetchar-2.1.4/docs/data/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/docs/html/index.rst` & `gwdetchar-2.1.4/docs/html/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/docs/index.rst` & `gwdetchar-2.1.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/docs/lasso/index.rst` & `gwdetchar-2.1.4/docs/lasso/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/docs/nagios/index.rst` & `gwdetchar-2.1.4/docs/nagios/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/docs/omega/index.rst` & `gwdetchar-2.1.4/docs/omega/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/docs/saturation/index.rst` & `gwdetchar-2.1.4/docs/saturation/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/docs/scattering/index.rst` & `gwdetchar-2.1.4/docs/scattering/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/__init__.py` & `gwdetchar-2.1.4/gwdetchar/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/cds.py` & `gwdetchar-2.1.4/gwdetchar/cds.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/cli.py` & `gwdetchar-2.1.4/gwdetchar/cli.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/condor.py` & `gwdetchar-2.1.4/gwdetchar/condor.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/conftest.py` & `gwdetchar-2.1.4/gwdetchar/conftest.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/conlog.py` & `gwdetchar-2.1.4/gwdetchar/conlog.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/const.py` & `gwdetchar-2.1.4/gwdetchar/const.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/daq.py` & `gwdetchar-2.1.4/gwdetchar/daq.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/io/__init__.py` & `gwdetchar-2.1.4/gwdetchar/io/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/io/datafind.py` & `gwdetchar-2.1.4/gwdetchar/io/datafind.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/io/html.py` & `gwdetchar-2.1.4/gwdetchar/io/html.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/io/ligolw.py` & `gwdetchar-2.1.4/gwdetchar/io/ligolw.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/io/tests/__init__.py` & `gwdetchar-2.1.4/gwdetchar/io/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/io/tests/test_datafind.py` & `gwdetchar-2.1.4/gwdetchar/io/tests/test_datafind.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/io/tests/test_html.py` & `gwdetchar-2.1.4/gwdetchar/io/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/io/tests/test_ligolw.py` & `gwdetchar-2.1.4/gwdetchar/io/tests/test_ligolw.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/lasso/__init__.py` & `gwdetchar-2.1.4/gwdetchar/lasso/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/lasso/__main__.py` & `gwdetchar-2.1.4/gwdetchar/lasso/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -899,26 +899,26 @@
 
         channelsfile = f'{args.ifo}-CHANNELS-{gpsstub}.csv'
         numpy.savetxt(channelsfile, aux_channels, delimiter=',', fmt='%s')
 
         # -- Generate a segment summary page
 
         # write html
-        trange = f'{seg[0]}-{seg[1]}'
-        title = f'{args.ifo} Lasso Correlation: {trange}'
+        title = f'{args.ifo} Lasso Correlation: {gpsblock}'
         if args.band_pass:
-            links = [trange] + [(s, '#%s' % s.lower()) for s in
-                                ['Parameters', 'Spectra', 'Model', 'Results']]
+            links = [gpsblock] + [(s, f'#{s.lower()}') for s in
+                                  ['Parameters', 'Spectra', 'Model',
+                                   'Results']]
         else:
-            links = [trange] + [(s, '#%s' % s.lower()) for s in
-                                ['Parameters', 'Model', 'Results']]
+            links = [gpsblock] + [(s, f'#{s.lower()}') for s in
+                                  ['Parameters', 'Model', 'Results']]
         (brand, class_) = htmlio.get_brand(args.ifo, 'Lasso', seg[0])
         navbar = htmlio.navbar(links, class_=class_, brand=brand)
         page = htmlio.new_bootstrap_page(
-            title=f'{args.ifo} Lasso | {trange}',
+            title=f'{args.ifo} Lasso | {gpsblock}',
             navbar=navbar)
         page.h1(title, class_='pb-2 mt-3 mb-2 border-bottom')
 
         # -- summary table
         content = [
             ('Primary channel', markup.oneliner.code(primary)),
             ('Primary frametype', markup.oneliner.code(
@@ -1176,15 +1176,15 @@
                 seg_plot_links[i] = summations_plot_link
 
     # generate HTML page
     title = f'Lasso Slow Correlations: {start}-{end}'
     sections = [[f'{i+1}: {gpsblocks[i]}', f'#{gpsblocks[i]}']
                 for i, seg in enumerate(gpsblocks)]
     date = tconvert(start)
-    links = ['-'.join([date.year, date.month, date.day]),
+    links = [date.strftime('%Y-%m-%d'),
              ['Summary', '#'],
              ['Segments', [['Analyses', sections]]]]
     (brand, class_) = htmlio.get_brand(args.ifo, 'Daily Lasso', start)
     navbar = htmlio.navbar(links, class_=class_, brand=brand)
     page = htmlio.new_bootstrap_page(title=title, navbar=navbar)
 
     # page header
@@ -1229,22 +1229,22 @@
     page.h2('Results Summary', id_='summary')
     page.div.close()  # banner
 
     if len(lasso_segs) == 0:
         page.add(htmlio.alert(
             f'No segments of length {args.segment_min_length/3600} hours or '
             f'longer were found in state <code>{state_flag}</code> on '
-            f'{date.year}-{date.month}-{date.day}',
+            f"{date.strftime('%Y-%m-%d')}",
             dismiss=False,
         ))
     else:
         page.add(htmlio.alert(
             f'A total of {len(segs)} segments were found in state '
-            f'<code>{state_flag}</code> on {date.year}-{date.month}-'
-            f'{date.day}, of which {len(lasso_segs)} are at least '
+            f"<code>{state_flag}</code> on {date.strftime('%Y-%m-%d')} "
+            f'of which {len(lasso_segs)} are at least '
             f'{args.segment_min_length/3600} hours long. These are '
             'summarized and linked below. The list of channels for each '
             'segment represents the largest contributors in modeling '
             f'{primary_nickname}.',
         ))
 
     for i, link in enumerate(seg_page_links):
```

### Comparing `gwdetchar-2.1.3/gwdetchar/lasso/core.py` & `gwdetchar-2.1.4/gwdetchar/lasso/core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/lasso/old.py` & `gwdetchar-2.1.4/gwdetchar/lasso/old.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/lasso/plot.py` & `gwdetchar-2.1.4/gwdetchar/lasso/plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/lasso/tests/__init__.py` & `gwdetchar-2.1.4/gwdetchar/lasso/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/lasso/tests/test_core.py` & `gwdetchar-2.1.4/gwdetchar/lasso/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/lasso/tests/test_main.py` & `gwdetchar-2.1.4/gwdetchar/lasso/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/lasso/tests/test_plot.py` & `gwdetchar-2.1.4/gwdetchar/lasso/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/mct.py` & `gwdetchar-2.1.4/gwdetchar/mct.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/nagios/__init__.py` & `gwdetchar-2.1.4/gwdetchar/nagios/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/nagios/__main__.py` & `gwdetchar-2.1.4/gwdetchar/nagios/__main__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/nagios/core.py` & `gwdetchar-2.1.4/gwdetchar/nagios/core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/nagios/tests/__init__.py` & `gwdetchar-2.1.4/gwdetchar/nagios/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/nagios/tests/test_main.py` & `gwdetchar-2.1.4/gwdetchar/nagios/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/omega/__init__.py` & `gwdetchar-2.1.4/gwdetchar/omega/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/omega/__main__.py` & `gwdetchar-2.1.4/gwdetchar/omega/__main__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/omega/batch.py` & `gwdetchar-2.1.4/gwdetchar/omega/batch.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/omega/config.py` & `gwdetchar-2.1.4/gwdetchar/omega/config.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/omega/core.py` & `gwdetchar-2.1.4/gwdetchar/omega/core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/omega/html.py` & `gwdetchar-2.1.4/gwdetchar/omega/html.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/omega/plot.py` & `gwdetchar-2.1.4/gwdetchar/omega/plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/omega/tests/__init__.py` & `gwdetchar-2.1.4/gwdetchar/omega/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/omega/tests/test_batch.py` & `gwdetchar-2.1.4/gwdetchar/omega/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/omega/tests/test_config.py` & `gwdetchar-2.1.4/gwdetchar/omega/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/omega/tests/test_core.py` & `gwdetchar-2.1.4/gwdetchar/omega/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/omega/tests/test_html.py` & `gwdetchar-2.1.4/gwdetchar/omega/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/omega/tests/test_main.py` & `gwdetchar-2.1.4/gwdetchar/omega/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/omega/tests/test_plot.py` & `gwdetchar-2.1.4/gwdetchar/omega/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/overflow.py` & `gwdetchar-2.1.4/gwdetchar/overflow.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/plot.py` & `gwdetchar-2.1.4/gwdetchar/plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/saturation/__init__.py` & `gwdetchar-2.1.4/gwdetchar/saturation/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/saturation/__main__.py` & `gwdetchar-2.1.4/gwdetchar/saturation/__main__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/saturation/core.py` & `gwdetchar-2.1.4/gwdetchar/saturation/core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/saturation/tests/__init__.py` & `gwdetchar-2.1.4/gwdetchar/saturation/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/saturation/tests/test_saturation.py` & `gwdetchar-2.1.4/gwdetchar/saturation/tests/test_saturation.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/scattering/__init__.py` & `gwdetchar-2.1.4/gwdetchar/scattering/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/scattering/__main__.py` & `gwdetchar-2.1.4/gwdetchar/scattering/__main__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/scattering/core.py` & `gwdetchar-2.1.4/gwdetchar/scattering/core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/scattering/plot.py` & `gwdetchar-2.1.4/gwdetchar/scattering/plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/scattering/simple.py` & `gwdetchar-2.1.4/gwdetchar/scattering/simple.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/scattering/tests/__init__.py` & `gwdetchar-2.1.4/gwdetchar/scattering/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/scattering/tests/test_core.py` & `gwdetchar-2.1.4/gwdetchar/scattering/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/scattering/tests/test_main.py` & `gwdetchar-2.1.4/gwdetchar/scattering/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/scattering/tests/test_plot.py` & `gwdetchar-2.1.4/gwdetchar/scattering/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/scattering/tests/test_simple.py` & `gwdetchar-2.1.4/gwdetchar/scattering/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/tests/__init__.py` & `gwdetchar-2.1.4/gwdetchar/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/tests/test_cds.py` & `gwdetchar-2.1.4/gwdetchar/tests/test_cds.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/tests/test_cli.py` & `gwdetchar-2.1.4/gwdetchar/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/tests/test_condor.py` & `gwdetchar-2.1.4/gwdetchar/tests/test_condor.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/tests/test_conlog.py` & `gwdetchar-2.1.4/gwdetchar/tests/test_conlog.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/tests/test_const.py` & `gwdetchar-2.1.4/gwdetchar/tests/test_const.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/tests/test_daq.py` & `gwdetchar-2.1.4/gwdetchar/tests/test_daq.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/tests/test_plot.py` & `gwdetchar-2.1.4/gwdetchar/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/tests/test_utils.py` & `gwdetchar-2.1.4/gwdetchar/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar/utils.py` & `gwdetchar-2.1.4/gwdetchar/utils.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar.egg-info/PKG-INFO` & `gwdetchar-2.1.4/gwdetchar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwdetchar
-Version: 2.1.3
+Version: 2.1.4
 Summary: A python package for gravitational-wave detector characterisation
 Author-email: Alex Urban <alex.urban@ligo.org>, Duncan Macleod <duncan.macleod@ligo.org>
 Maintainer-email: Evan Goetz <evan.goetz@ligo.org>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://gwdetchar.readthedocs.io
 Project-URL: Source Code, https://github.com/gwdetchar/gwdetchar
 Project-URL: Bug Tracker, https://github.com/gwdetchar/gwdetchar/issues
```

### Comparing `gwdetchar-2.1.3/gwdetchar.egg-info/SOURCES.txt` & `gwdetchar-2.1.4/gwdetchar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/gwdetchar.egg-info/entry_points.txt` & `gwdetchar-2.1.4/gwdetchar.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.3/pyproject.toml` & `gwdetchar-2.1.4/pyproject.toml`

 * *Files identical despite different names*

