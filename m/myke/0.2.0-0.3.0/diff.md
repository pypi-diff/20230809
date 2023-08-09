# Comparing `tmp/myke-0.2.0.tar.gz` & `tmp/myke-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myke-0.2.0.tar", last modified: Thu Jul 20 04:46:21 2023, max compression
+gzip compressed data, was "myke-0.3.0.tar", last modified: Wed Aug  9 05:10:36 2023, max compression
```

## Comparing `myke-0.2.0.tar` & `myke-0.3.0.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 04:46:21.363426 myke-0.2.0/
--rw-r--r--   0 root         (0) root         (0)    34487 2023-07-20 04:38:03.000000 myke-0.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    44669 2023-07-20 04:46:21.363426 myke-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4219 2023-07-20 04:38:03.000000 myke-0.2.0/README.md
--rw-r--r--   0 root         (0) root         (0)     5059 2023-07-20 04:38:03.000000 myke-0.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 04:46:21.363426 myke-0.2.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 04:46:21.347426 myke-0.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 04:46:21.351426 myke-0.2.0/src/myke/
--rw-r--r--   0 root         (0) root         (0)      871 2023-07-20 04:38:03.000000 myke-0.2.0/src/myke/__init__.py
--rw-r--r--   0 root         (0) root         (0)       62 2023-07-20 04:38:03.000000 myke-0.2.0/src/myke/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 04:46:21.359426 myke-0.2.0/src/myke/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      921 2023-07-20 04:38:42.000000 myke-0.2.0/src/myke/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)      195 2023-07-20 04:38:42.000000 myke-0.2.0/src/myke/__pycache__/__main__.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)      148 2023-07-20 04:46:00.000000 myke-0.2.0/src/myke/__pycache__/__version__.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)      479 2023-07-20 04:38:42.000000 myke-0.2.0/src/myke/__pycache__/exceptions.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)      421 2023-07-20 04:38:42.000000 myke-0.2.0/src/myke/__pycache__/globals.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     3966 2023-07-20 04:38:42.000000 myke-0.2.0/src/myke/__pycache__/main.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     5373 2023-07-20 04:38:42.000000 myke-0.2.0/src/myke/__pycache__/run.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     5906 2023-07-20 04:38:42.000000 myke-0.2.0/src/myke/__pycache__/tasks.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)      577 2023-07-20 04:38:42.000000 myke-0.2.0/src/myke/__pycache__/types.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     4640 2023-07-20 04:38:42.000000 myke-0.2.0/src/myke/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-20 04:46:00.000000 myke-0.2.0/src/myke/__version__.py
--rw-r--r--   0 root         (0) root         (0)      832 2023-07-20 04:38:03.000000 myke-0.2.0/src/myke/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      206 2023-07-20 04:38:03.000000 myke-0.2.0/src/myke/globals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 04:46:21.359426 myke-0.2.0/src/myke/io/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 04:38:03.000000 myke-0.2.0/src/myke/io/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 04:46:21.359426 myke-0.2.0/src/myke/io/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      127 2023-07-20 04:38:42.000000 myke-0.2.0/src/myke/io/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     6365 2023-07-20 04:38:42.000000 myke-0.2.0/src/myke/io/__pycache__/echo.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     8474 2023-07-20 04:38:42.000000 myke-0.2.0/src/myke/io/__pycache__/read.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     3654 2023-07-20 04:38:42.000000 myke-0.2.0/src/myke/io/__pycache__/write.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     5929 2023-07-20 04:38:03.000000 myke-0.2.0/src/myke/io/echo.py
--rw-r--r--   0 root         (0) root         (0)     7195 2023-07-20 04:38:03.000000 myke-0.2.0/src/myke/io/read.py
--rw-r--r--   0 root         (0) root         (0)     3669 2023-07-20 04:38:03.000000 myke-0.2.0/src/myke/io/write.py
--rw-r--r--   0 root         (0) root         (0)     5582 2023-07-20 04:38:03.000000 myke-0.2.0/src/myke/main.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 04:38:03.000000 myke-0.2.0/src/myke/py.typed
--rw-r--r--   0 root         (0) root         (0)     5815 2023-07-20 04:38:03.000000 myke-0.2.0/src/myke/run.py
--rw-r--r--   0 root         (0) root         (0)     5865 2023-07-20 04:38:03.000000 myke-0.2.0/src/myke/tasks.py
--rw-r--r--   0 root         (0) root         (0)      429 2023-07-20 04:38:03.000000 myke-0.2.0/src/myke/types.py
--rw-r--r--   0 root         (0) root         (0)     3988 2023-07-20 04:38:03.000000 myke-0.2.0/src/myke/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 04:46:21.355426 myke-0.2.0/src/myke.egg-info/
--rw-r--r--   0 root         (0) root         (0)    44669 2023-07-20 04:46:21.000000 myke-0.2.0/src/myke.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1253 2023-07-20 04:46:21.000000 myke-0.2.0/src/myke.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 04:46:21.000000 myke-0.2.0/src/myke.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-07-20 04:46:21.000000 myke-0.2.0/src/myke.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      830 2023-07-20 04:46:21.000000 myke-0.2.0/src/myke.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-07-20 04:46:21.000000 myke-0.2.0/src/myke.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 04:46:21.363426 myke-0.2.0/tests/
--rw-r--r--   0 root         (0) root         (0)     4891 2023-07-20 04:38:03.000000 myke-0.2.0/tests/test_Mykefile.py
--rw-r--r--   0 root         (0) root         (0)     4933 2023-07-20 04:38:03.000000 myke-0.2.0/tests/test_io.py
--rw-r--r--   0 root         (0) root         (0)     1830 2023-07-20 04:38:03.000000 myke-0.2.0/tests/test_main.py
--rw-r--r--   0 root         (0) root         (0)     2944 2023-07-20 04:38:03.000000 myke-0.2.0/tests/test_run.py
--rw-r--r--   0 root         (0) root         (0)      777 2023-07-20 04:38:03.000000 myke-0.2.0/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 05:10:36.154899 myke-0.3.0/
+-rw-r--r--   0 root         (0) root         (0)    34487 2023-08-09 05:01:28.000000 myke-0.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    40510 2023-08-09 05:10:36.154899 myke-0.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2199 2023-08-09 05:01:28.000000 myke-0.3.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       59 2023-08-09 05:01:28.000000 myke-0.3.0/README.pypi.md
+-rw-r--r--   0 root         (0) root         (0)     5137 2023-08-09 05:01:28.000000 myke-0.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-09 05:10:36.154899 myke-0.3.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 05:10:36.142899 myke-0.3.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 05:10:36.146899 myke-0.3.0/src/myke/
+-rw-r--r--   0 root         (0) root         (0)      871 2023-08-09 05:01:28.000000 myke-0.3.0/src/myke/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       62 2023-08-09 05:01:28.000000 myke-0.3.0/src/myke/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 05:10:36.150899 myke-0.3.0/src/myke/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      921 2023-08-09 05:02:11.000000 myke-0.3.0/src/myke/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      195 2023-08-09 05:02:12.000000 myke-0.3.0/src/myke/__pycache__/__main__.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      148 2023-08-09 05:10:16.000000 myke-0.3.0/src/myke/__pycache__/__version__.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      479 2023-08-09 05:02:12.000000 myke-0.3.0/src/myke/__pycache__/exceptions.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      421 2023-08-09 05:02:12.000000 myke-0.3.0/src/myke/__pycache__/globals.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     3939 2023-08-09 05:02:12.000000 myke-0.3.0/src/myke/__pycache__/main.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     5373 2023-08-09 05:02:12.000000 myke-0.3.0/src/myke/__pycache__/run.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     5906 2023-08-09 05:02:12.000000 myke-0.3.0/src/myke/__pycache__/tasks.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      577 2023-08-09 05:02:12.000000 myke-0.3.0/src/myke/__pycache__/types.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     4640 2023-08-09 05:02:12.000000 myke-0.3.0/src/myke/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)       22 2023-08-09 05:10:16.000000 myke-0.3.0/src/myke/__version__.py
+-rw-r--r--   0 root         (0) root         (0)      832 2023-08-09 05:01:28.000000 myke-0.3.0/src/myke/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      206 2023-08-09 05:01:28.000000 myke-0.3.0/src/myke/globals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 05:10:36.150899 myke-0.3.0/src/myke/io/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-09 05:01:28.000000 myke-0.3.0/src/myke/io/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 05:10:36.150899 myke-0.3.0/src/myke/io/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      127 2023-08-09 05:02:12.000000 myke-0.3.0/src/myke/io/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     6365 2023-08-09 05:02:12.000000 myke-0.3.0/src/myke/io/__pycache__/echo.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     8474 2023-08-09 05:02:12.000000 myke-0.3.0/src/myke/io/__pycache__/read.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     3654 2023-08-09 05:02:12.000000 myke-0.3.0/src/myke/io/__pycache__/write.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     5929 2023-08-09 05:01:28.000000 myke-0.3.0/src/myke/io/echo.py
+-rw-r--r--   0 root         (0) root         (0)     7195 2023-08-09 05:01:28.000000 myke-0.3.0/src/myke/io/read.py
+-rw-r--r--   0 root         (0) root         (0)     3669 2023-08-09 05:01:28.000000 myke-0.3.0/src/myke/io/write.py
+-rw-r--r--   0 root         (0) root         (0)     5513 2023-08-09 05:01:28.000000 myke-0.3.0/src/myke/main.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-09 05:01:28.000000 myke-0.3.0/src/myke/py.typed
+-rw-r--r--   0 root         (0) root         (0)     5815 2023-08-09 05:01:28.000000 myke-0.3.0/src/myke/run.py
+-rw-r--r--   0 root         (0) root         (0)     5865 2023-08-09 05:01:28.000000 myke-0.3.0/src/myke/tasks.py
+-rw-r--r--   0 root         (0) root         (0)      429 2023-08-09 05:01:28.000000 myke-0.3.0/src/myke/types.py
+-rw-r--r--   0 root         (0) root         (0)     3988 2023-08-09 05:01:28.000000 myke-0.3.0/src/myke/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 05:10:36.146899 myke-0.3.0/src/myke.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    40510 2023-08-09 05:10:36.000000 myke-0.3.0/src/myke.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1268 2023-08-09 05:10:36.000000 myke-0.3.0/src/myke.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-09 05:10:36.000000 myke-0.3.0/src/myke.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-08-09 05:10:36.000000 myke-0.3.0/src/myke.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      884 2023-08-09 05:10:36.000000 myke-0.3.0/src/myke.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-08-09 05:10:36.000000 myke-0.3.0/src/myke.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 05:10:36.150899 myke-0.3.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     5193 2023-08-09 05:01:28.000000 myke-0.3.0/tests/test_Mykefile.py
+-rw-r--r--   0 root         (0) root         (0)     4933 2023-08-09 05:01:28.000000 myke-0.3.0/tests/test_io.py
+-rw-r--r--   0 root         (0) root         (0)     1830 2023-08-09 05:01:28.000000 myke-0.3.0/tests/test_main.py
+-rw-r--r--   0 root         (0) root         (0)     2944 2023-08-09 05:01:28.000000 myke-0.3.0/tests/test_run.py
+-rw-r--r--   0 root         (0) root         (0)      777 2023-08-09 05:01:28.000000 myke-0.3.0/tests/test_utils.py
```

### Comparing `myke-0.2.0/LICENSE` & `myke-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `myke-0.2.0/PKG-INFO` & `myke-0.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: myke
-Version: 0.2.0
-Summary: The dynamic Python CLI for task execution.
+Version: 0.3.0
+Summary: The dynamic Python CLI for convenient task execution.
 Author-email: Donald Mellenbruch <hello@f2dv.com>
 License: GNU GENERAL PUBLIC LICENSE
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
         Everyone is permitted to copy and distribute verbatim copies
         of this license document, but changing it is not allowed.
@@ -674,112 +674,21 @@
         The GNU General Public License does not permit incorporating your program
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
-Project-URL: Homepage, https://www.f2dv.com/code/r/myke/i
+Project-URL: Homepage, https://www.f2dv.com/r/myke
 Project-URL: Repository, https://www.github.com/fresh2dev/myke
-Project-URL: Funding, https://www.f2dv.com/funding
+Project-URL: Funding, https://www.f2dv.com/fund
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: io
 Provides-Extra: extras
 License-File: LICENSE
 
-# myke
-
-> The dynamic Python CLI for task execution.
-
-| Links         |                                              |
-|---------------|----------------------------------------------|
-| Code Repo     | https://www.github.com/fresh2dev/myke        |
-| Mirror Repo   | https://www.f2dv.com/code/r/myke             |
-| Documentation | https://www.f2dv.com/code/r/myke/i           |
-| Changelog     | https://www.f2dv.com/code/r/myke/i/changelog |
-| License       | https://www.f2dv.com/code/r/myke/i/license   |
-| Funding       | https://www.f2dv.com/funding                 |
-
-[![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/fresh2dev/myke?color=blue&style=for-the-badge)](https://www.github.com/fresh2dev/myke/releases)
-[![GitHub Release Date](https://img.shields.io/github/release-date/fresh2dev/myke?color=blue&style=for-the-badge)](https://www.github.com/fresh2dev/myke/releases)
-[![License](https://img.shields.io/github/license/fresh2dev/myke?color=blue&style=for-the-badge)](https://www.f2dv.com/code/r/myke/i/license)
-[![GitHub issues](https://img.shields.io/github/issues-raw/fresh2dev/myke?color=blue&style=for-the-badge)](https://www.github.com/fresh2dev/myke/issues)
-[![GitHub pull requests](https://img.shields.io/github/issues-pr-raw/fresh2dev/myke?color=blue&style=for-the-badge)](https://www.github.com/fresh2dev/myke/pulls)
-[![GitHub Repo stars](https://img.shields.io/github/stars/fresh2dev/myke?color=blue&style=for-the-badge)](https://star-history.com/#fresh2dev/myke&Date)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/myke?color=blue&style=for-the-badge)](https://pypi.org/project/myke)
-[![Docker Pulls](https://img.shields.io/docker/pulls/fresh2dev/myke?color=blue&style=for-the-badge)](https://hub.docker.com/r/fresh2dev/myke)
-[![Docs Website](https://img.shields.io/website?down_message=unavailable&label=docs&style=for-the-badge&up_color=blue&up_message=available&url=https://www.f2dv.com/code/r/myke/i)](https://www.f2dv.com/code/r/myke/i)
-[![Coverage Website](https://img.shields.io/website?down_message=unavailable&label=coverage&style=for-the-badge&up_color=blue&up_message=available&url=https://www.f2dv.com/code/r/myke/i/tests/coverage)](https://www.f2dv.com/code/r/myke/i/tests/coverage)
-[![Funding](https://img.shields.io/badge/funding-%24%24%24-blue?style=for-the-badge)](https://www.f2dv.com/fund)
-
-## Overview
-
-Meet `myke`, the dynamic Python CLI for task exection.
-
-I built `myke` to replace my personal need for `make` and Makefiles. myke has probably 1% of the functionality of make, and that's a good thing.
-
-> Note: `myke` is in *beta* status. Please report ideas and issues [here](https://github.com/fresh2dev/myke/issues).
-
-## Install
-
-myke is a CLI application, so I recommend installing it using [pipx](https://github.com/pypa/pipx).
-
-```sh
-pipx install 'myke[extras]'
-```
-
-What's in `myke[extras]`?
-
-- `myke[io]` --> Libraries to read/write various file formats (yaml, toml, etc.)
-- `myke[pydantic]` --> Includes the [Pydantic](https://github.com/pydantic/pydantic) library to support additional types.
-- `myke[tui]` --> Includes the [Trogon](https://github.com/Textualize/trogon) library to present a TUI for myke.
-
-## Use
-
-Paste the following into a file named `Mykefile`:
-
-```python title="Mykefile"
-from myke import task
-
-@task
-def say_hello(name):
-    print(f"Hello {name}.")
-
-@task
-def say_goodbye(name):
-    print(f"Goodbye {name}.")
-```
-
-Invoke a task:
-
-```sh
-myke say-hello --name world
-```
-
-View available tasks:
-
-```sh
-myke
-```
-
-### Read More
-
-myke is an instantiation of the `yapx` project, the CLI builder for Python. The information contained in the [yapx docs](https://www.f2dv.com/code/r/yapx/i/) also applies to myke.
-
-Read more about myke @ https://www.f2dv.com/code/r/myke/i
-
-Read more about yapx @ https://www.f2dv.com/code/r/yapx/i
-
-## Support
-
-If this project delivers value to you, please [provide feedback](https://www.github.com/fresh2dev/myke/issues), code contributions, and/or [funding](https://www.f2dv.com/fund).
-
-See all of my projects @ https://www.f2dv.com/code/r
-
-*Brought to you by...*
-
-<a href="https://www.f2dv.com"><img src="https://img.fresh2.dev/fresh2dev.svg" style="filter: invert(50%);"></img></a>
+[https://www.f2dv.com/r/myke](https://www.f2dv.com/r/myke)
```

### Comparing `myke-0.2.0/pyproject.toml` & `myke-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "myke"
 authors = [
     {name = "Donald Mellenbruch", email = "hello@f2dv.com"},
 ]
-description = "The dynamic Python CLI for task execution."
-readme = "README.md"
+description = "The dynamic Python CLI for convenient task execution."
+readme = "README.pypi.md"
 license = {file = "LICENSE"}
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dynamic = ["version"]
 dependencies = [
     "typing-extensions; python_version<'3.10'",
-    "yapx[extras]==0.2.*",
+    "yapx[extras]>=0.2.4,<1",
     "pip>=22.2",  # enables "pip --dry-run ..."
 ]
 
 [project.optional-dependencies]
 dev = [
     "python-lsp-server[rope]==1.*",
     "pylint==2.*",
@@ -56,35 +56,38 @@
     "packaging==23.*",
     "mockish==0.1.*",
     #
     "requests==2.*",
     "pyyaml",
     "python-dotenv",
     "tomli; python_version<'3.11'",
-    "tabulate",
+    "tabulate<1",
+    "ppqueue==0.4.*"
 ]
 io = [
     "requests==2.*",
     "pyyaml",
     "python-dotenv",
     "tomli; python_version<'3.11'",
-    "tabulate",
+    "tabulate<1",
+    "ppqueue==0.4.*"
 ]
 extras = [
     "requests==2.*",
     "pyyaml",
     "python-dotenv",
     "tomli; python_version<'3.11'",
-    "tabulate",
+    "tabulate<1",
+    "ppqueue==0.4.*"
 ]
 
 [project.urls]
-Homepage = "https://www.f2dv.com/code/r/myke/i"
+Homepage = "https://www.f2dv.com/r/myke"
 Repository = "https://www.github.com/fresh2dev/myke"
-Funding = "https://www.f2dv.com/funding"
+Funding = "https://www.f2dv.com/fund"
 
 [project.scripts]
 myke = "myke.__main__:main"
 
 [tool.setuptools.package-data]
 "*" = ["**"]
 [tool.setuptools.packages.find]
```

### Comparing `myke-0.2.0/src/myke/__init__.py` & `myke-0.3.0/src/myke/__init__.py`

 * *Files identical despite different names*

### Comparing `myke-0.2.0/src/myke/__pycache__/__init__.cpython-310.pyc` & `myke-0.3.0/src/myke/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jul 20 04:38:03 2023 UTC, .py size: 871 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2bba b864 6703 0000  o.......+..dg...
+00000000: 6f0d 0d0a 0000 0000 a81d d364 6703 0000  o..........dg...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 c400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a02 0100 6400 6402 6c03  d.l.m.Z...d.d.l.
 00000040: 6d04 5a04 0100 6403 6404 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000050: 6d07 5a07 6d08 5a08 0100 6403 6405 6c09  m.Z.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6403 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6403 6407 6c0c 6d0d 5a0d 0100 6403  ..d.d.l.m.Z...d.
```

### Comparing `myke-0.2.0/src/myke/__pycache__/main.cpython-310.pyc` & `myke-0.3.0/src/myke/__pycache__/main.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jul 20 04:38:03 2023 UTC, .py size: 5582 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2bba b864 ce15 0000  o.......+..d....
+00000000: 6f0d 0d0a 0000 0000 a81d d364 8915 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 1001 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d06 5a06  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c07 6d08 5a08 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6406 6c09 6d0a 5a0a 0100 6400 6407 6c0b  d.l.m.Z...d.d.l.
@@ -37,212 +37,211 @@
 00000240: 5f6d 6f64 756c 65da 0f69 6d70 6f72 745f  _module..import_
 00000250: 6d79 6b65 6669 6c65 2901 da09 416e 6e6f  mykefile)...Anno
 00000260: 7461 7465 6429 01da 0d67 6574 5f72 6570  tated)...get_rep
 00000270: 6f5f 726f 6f74 2903 720d 0000 00da 046d  o_root).r......m
 00000280: 6169 6eda 0373 7973 da05 5f66 696c 65da  ain..sys.._file.
 00000290: 0672 6574 7572 6e63 0100 0000 0000 0000  .returnc........
 000002a0: 0000 0000 0f00 0000 0f00 0000 0300 0000  ................
-000002b0: 739c 0300 0074 0047 0087 0066 0164 0164  s....t.G...f.d.d
+000002b0: 7388 0300 0074 0047 0087 0066 0164 0164  s....t.G...f.d.d
 000002c0: 0284 0864 0274 016a 026a 0383 0383 017d  ...d.t.j.j.....}
 000002d0: 0188 0072 1474 0488 0083 016e 0174 057d  ...r.t.....n.t.}
 000002e0: 0274 016a 067c 0274 0764 0367 0164 0467  .t.j.|.t.d.g.d.g
 000002f0: 0167 0064 058d 057d 037c 03a0 087c 01a1  .g.d...}.|...|..
 00000300: 0101 0074 096a 0a64 0664 0085 0219 007d  ...t.j.d.d.....}
-00000310: 047c 0473 387c 03a0 0ba1 0001 007c 03a0  .|.s8|.......|..
-00000320: 0ca1 0001 007c 036a 0d7c 047c 0164 0764  .....|.j.|.|.d.d
-00000330: 088d 035c 027d 057d 0674 0e7c 057c 0183  ...\.}.}.t.|.|..
-00000340: 0273 494a 0082 0188 0072 6674 0e88 0074  .sIJ.....rft...t
-00000350: 0f83 0273 5474 0f88 0083 0189 0088 00a0  ...sTt..........
-00000360: 10a1 0073 5c74 1188 0083 0182 0174 1273  ...s\t.......t.s
-00000370: 6274 1388 0083 0182 0188 00a0 14a1 0089  bt..............
-00000380: 007c 056a 1572 7364 0964 0a84 007c 056a  .|.j.rsd.d...|.j
-00000390: 1544 0083 017c 055f 156e 0e74 0f74 1683  .D...|._.n.t.t..
-000003a0: 01a0 10a1 0072 8174 0f74 1683 01a0 14a1  .....r.t.t......
-000003b0: 0067 017c 055f 1574 1774 1183 018f 1201  .g.|._.t.t......
-000003c0: 0074 1883 007d 077c 0772 9074 19a0 1a7c  .t...}.|.r.t...|
-000003d0: 07a1 0101 0057 0064 0004 0004 0083 0301  .....W.d........
-000003e0: 006e 0831 0073 9a77 0101 0001 0001 0059  .n.1.s.w.......Y
-000003f0: 0001 007c 056a 1573 b474 0f74 1683 01a0  ...|.j.s.t.t....
-00000400: 10a1 0072 b174 0f74 1683 01a0 14a1 0067  ...r.t.t.......g
-00000410: 017c 055f 156e 0367 007c 055f 157c 056a  .|._.n.g.|._.|.j
-00000420: 1b72 d57c 056a 1572 bf7c 056a 1564 0b19  .r.|.j.r.|.j.d..
-00000430: 006e 0374 0f74 1683 017d 0874 1ca0 1d74  .n.t.t...}.t...t
-00000440: 047c 0883 01a1 0101 0074 1e64 0c7c 089b  .|.......t.d.|..
-00000450: 009d 0283 0101 007c 03a0 0ca1 0001 007a  .......|.......z
-00000460: 5e7a 177c 056a 1544 005d 117d 097c 0972  ^z.|.j.D.].}.|.r
-00000470: eb88 0072 e57c 09a0 1f88 00a1 0173 eb74  ...r.|.......s.t
-00000480: 2074 047c 0983 0183 0101 0071 da57 006e   t.|.......q.W.n
-00000490: 3504 0074 1190 0179 2201 007d 0a01 007a  5..t...y"..}...z
-000004a0: 287c 03a0 0ba1 0001 0074 1e74 196a 219b  (|.......t.t.j!.
-000004b0: 0064 0d7c 0a6a 229b 0064 0e74 196a 219b  .d.|.j"..d.t.j!.
-000004c0: 0064 0f7c 029b 0064 107c 0a6a 229b 0064  .d.|...d.|.j"..d
-000004d0: 0d74 196a 219b 009d 0b83 0101 007c 03a0  .t.j!........|..
-000004e0: 0ca1 0001 0057 0059 0064 007d 0a7e 0a6e  .....W.Y.d.}.~.n
-000004f0: 0564 007d 0a7e 0a77 0177 007c 056a 2390  .d.}.~.w.w.|.j#.
-00000500: 0172 327c 056a 2344 005d 077d 0b74 247c  .r2|.j#D.].}.t$|
-00000510: 0b83 0101 0090 0171 2a57 006e 1a04 0074  .......q*W.n...t
-00000520: 2590 0179 4d01 007d 0a01 007a 0d7c 03a0  %..yM..}...z.|..
-00000530: 2674 047c 0a83 01a1 0101 0057 0059 0064  &t.|.......W.Y.d
-00000540: 007d 0a7e 0a6e 0564 007d 0a7e 0a77 0177  .}.~.n.d.}.~.w.w
-00000550: 0074 12a0 2774 2864 00a1 027d 0c7c 056a  .t..'t(d...}.|.j
-00000560: 2990 0172 9464 007d 0d7c 0690 0172 657c  )..r.d.}.|...re|
-00000570: 0664 0b19 00a0 2a64 11a1 0190 0172 717c  .d....*d.....rq|
-00000580: 0c7d 0d7c 0d64 0075 0090 0172 7074 1e64  .}.|.d.u...rpt.d
-00000590: 1283 0101 006e 1674 12a0 2b7c 0664 0b19  .....n.t..+|.d..
-000005a0: 0064 00a1 027d 0d7c 0d64 0075 0090 0172  .d...}.|.d.u...r
-000005b0: 8774 1e64 137c 0664 0b19 009b 009d 0283  .t.d.|.d........
-000005c0: 0101 007c 0d90 0172 9074 1e74 2c7c 0d83  ...|...r.t.t,|..
-000005d0: 0183 0101 007c 03a0 0ca1 0001 007c 056a  .....|.......|.j
-000005e0: 2d90 0172 a274 1e6a 2e7c 0264 148d 0101  -..r.t.j.|.d....
-000005f0: 007c 03a0 0ca1 0001 007c 0690 0172 c07c  .|.......|...r.|
-00000600: 0664 0b19 00a0 2a64 15a1 0190 0173 c074  .d....*d.....s.t
-00000610: 2f74 1283 0144 005d 0e7d 0e74 307c 0e7c  /t...D.].}.t0|.|
-00000620: 0664 0b19 0083 0290 0173 be74 127c 0e3d  .d.......s.t.|.=
-00000630: 0090 0171 b174 016a 317c 0c74 127c 0664  ...q.t.j1|.t.|.d
-00000640: 1667 017c 0274 0764 178d 0601 0064 0053  .g.|.t.d.....d.S
-00000650: 0029 184e 6300 0000 0000 0000 0000 0000  .).Nc...........
-00000660: 0000 0000 0008 0000 0000 0000 0073 d200  .............s..
-00000670: 0000 6500 5a01 6400 5a02 5500 6503 6504  ..e.Z.d.Z.U.e.e.
-00000680: 6505 6506 1900 1900 6507 6a08 9400 7211  e.e.....e.j...r.
-00000690: 9400 6e01 6401 6402 6701 6403 6404 6405  ..n.d.d.g.d.d.d.
-000006a0: 8d04 6602 1900 6509 6406 3c00 6503 6504  ..f...e.d.<.e.e.
-000006b0: 6505 650a 1900 1900 6507 6a08 6401 6407  e.e.....e.j.d.d.
-000006c0: 6701 6408 6404 6405 8d04 6602 1900 6509  g.d.d.d...f...e.
-000006d0: 6409 3c00 6503 6504 650b 1900 6507 6a08  d.<.e.e.e...e.j.
-000006e0: 6401 6404 640a 640b 6701 640c 8d04 6602  d.d.d.d.g.d...f.
-000006f0: 1900 6509 640d 3c00 6503 6504 650b 1900  ..e.d.<.e.e.e...
-00000700: 6507 6a08 6401 6404 640a 640e 6701 640c  e.j.d.d.d.d.g.d.
-00000710: 8d04 6602 1900 6509 640f 3c00 6503 6504  ..f...e.d.<.e.e.
-00000720: 650b 1900 6507 6a08 6401 6404 640a 6410  e...e.j.d.d.d.d.
-00000730: 6701 640c 8d04 6602 1900 6509 6411 3c00  g.d...f...e.d.<.
-00000740: 6401 5300 2912 7a16 6d61 696e 2e3c 6c6f  d.S.).z.main.<lo
-00000750: 6361 6c73 3e2e 4d79 6b65 4172 6773 4e7a  cals>.MykeArgsNz
-00000760: 0b2d 2d6d 796b 652d 6669 6c65 5a09 4d59  .--myke-fileZ.MY
-00000770: 4b45 5f46 494c 457a 0f6d 796b 6520 7061  KE_FILEz.myke pa
-00000780: 7261 6d65 7465 7273 2904 da07 6465 6661  rameters)...defa
-00000790: 756c 74da 0566 6c61 6773 da03 656e 76da  ult..flags..env.
-000007a0: 0567 726f 7570 da04 6669 6c65 7a0d 2d2d  .group..filez.--
-000007b0: 6d79 6b65 2d6d 6f64 756c 655a 0b4d 594b  myke-moduleZ.MYK
-000007c0: 455f 4d4f 4455 4c45 da06 6d6f 6475 6c65  E_MODULE..module
-000007d0: 547a 0c2d 2d6d 796b 652d 7461 736b 7329  Tz.--myke-tasks)
-000007e0: 0472 1e00 0000 7221 0000 00da 0965 7863  .r....r!.....exc
-000007f0: 6c75 7369 7665 721f 0000 00da 0a6c 6973  lusiver......lis
-00000800: 745f 7461 736b 737a 0e2d 2d6d 796b 652d  t_tasksz.--myke-
-00000810: 6578 706c 6169 6eda 0765 7870 6c61 696e  explain..explain
-00000820: 7a0d 2d2d 6d79 6b65 2d63 7265 6174 65da  z.--myke-create.
-00000830: 0663 7265 6174 6529 0cda 085f 5f6e 616d  .create)...__nam
-00000840: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-00000850: 0c5f 5f71 7561 6c6e 616d 655f 5f72 1800  .__qualname__r..
-00000860: 0000 720a 0000 0072 0900 0000 7206 0000  ..r....r....r...
-00000870: 00da 0479 6170 78da 0361 7267 da0f 5f5f  ...yapx..arg..__
-00000880: 616e 6e6f 7461 7469 6f6e 735f 5fda 0373  annotations__..s
-00000890: 7472 da04 626f 6f6c a900 a901 721c 0000  tr..bool....r...
-000008a0: 0072 3000 0000 fa1b 2f64 726f 6e65 2f73  .r0...../drone/s
-000008b0: 7263 2f73 7263 2f6d 796b 652f 6d61 696e  rc/src/myke/main
-000008c0: 2e70 79da 084d 796b 6541 7267 7319 0000  .py..MykeArgs...
-000008d0: 0073 6600 0000 0a00 0202 0a01 0401 0a01  .sf.............
-000008e0: 0401 0201 0201 04fc 02ff 08ff 0209 0a01  ................
-000008f0: 0401 0201 0401 0201 0201 04fc 02ff 08ff  ................
+00000310: 047c 036a 0b7c 047c 0164 0764 088d 035c  .|.j.|.|.d.d...\
+00000320: 027d 057d 0674 0c7c 057c 0183 0273 3f4a  .}.}.t.|.|...s?J
+00000330: 0082 0188 0072 5c74 0c88 0074 0d83 0273  .....r\t...t...s
+00000340: 4a74 0d88 0083 0189 0088 00a0 0ea1 0073  Jt.............s
+00000350: 5274 0f88 0083 0182 0174 1073 5874 1188  Rt.......t.sXt..
+00000360: 0083 0182 0188 00a0 12a1 0089 007c 056a  .............|.j
+00000370: 1372 6964 0964 0a84 007c 056a 1344 0083  .rid.d...|.j.D..
+00000380: 017c 055f 136e 0e74 0d74 1483 01a0 0ea1  .|._.n.t.t......
+00000390: 0072 7774 0d74 1483 01a0 12a1 0067 017c  .rwt.t.......g.|
+000003a0: 055f 1374 1574 0f83 018f 1201 0074 1683  ._.t.t.......t..
+000003b0: 007d 077c 0772 8674 17a0 187c 07a1 0101  .}.|.r.t...|....
+000003c0: 0057 0064 0004 0004 0083 0301 006e 0831  .W.d.........n.1
+000003d0: 0073 9077 0101 0001 0001 0059 0001 007c  .s.w.......Y...|
+000003e0: 056a 1373 aa74 0d74 1483 01a0 0ea1 0072  .j.s.t.t.......r
+000003f0: a774 0d74 1483 01a0 12a1 0067 017c 055f  .t.t.......g.|._
+00000400: 136e 0367 007c 055f 137c 056a 1972 cb7c  .n.g.|._.|.j.r.|
+00000410: 056a 1372 b57c 056a 1364 0b19 006e 0374  .j.r.|.j.d...n.t
+00000420: 0d74 1483 017d 0874 1aa0 1b74 047c 0883  .t...}.t...t.|..
+00000430: 01a1 0101 0074 1c64 0c7c 089b 009d 0283  .....t.d.|......
+00000440: 0101 007c 03a0 1da1 0001 007a 5e7a 177c  ...|.......z^z.|
+00000450: 056a 1344 005d 117d 097c 0972 e188 0072  .j.D.].}.|.r...r
+00000460: db7c 09a0 1e88 00a1 0173 e174 1f74 047c  .|.......s.t.t.|
+00000470: 0983 0183 0101 0071 d057 006e 3504 0074  .......q.W.n5..t
+00000480: 0f90 0179 1801 007d 0a01 007a 287c 03a0  ...y...}...z(|..
+00000490: 20a1 0001 0074 1c74 176a 219b 0064 0d7c   ....t.t.j!..d.|
+000004a0: 0a6a 229b 0064 0e74 176a 219b 0064 0f7c  .j"..d.t.j!..d.|
+000004b0: 029b 0064 107c 0a6a 229b 0064 0d74 176a  ...d.|.j"..d.t.j
+000004c0: 219b 009d 0b83 0101 007c 03a0 1da1 0001  !........|......
+000004d0: 0057 0059 0064 007d 0a7e 0a6e 0564 007d  .W.Y.d.}.~.n.d.}
+000004e0: 0a7e 0a77 0177 007c 056a 2390 0172 287c  .~.w.w.|.j#..r(|
+000004f0: 056a 2344 005d 077d 0b74 247c 0b83 0101  .j#D.].}.t$|....
+00000500: 0090 0171 2057 006e 1a04 0074 2590 0179  ...q W.n...t%..y
+00000510: 4301 007d 0a01 007a 0d7c 03a0 2674 047c  C..}...z.|..&t.|
+00000520: 0a83 01a1 0101 0057 0059 0064 007d 0a7e  .......W.Y.d.}.~
+00000530: 0a6e 0564 007d 0a7e 0a77 0177 0074 10a0  .n.d.}.~.w.w.t..
+00000540: 2774 2864 00a1 027d 0c7c 056a 2990 0172  't(d...}.|.j)..r
+00000550: 8a64 007d 0d7c 0690 0172 5b7c 0664 0b19  .d.}.|...r[|.d..
+00000560: 00a0 2a64 11a1 0190 0172 677c 0c7d 0d7c  ..*d.....rg|.}.|
+00000570: 0d64 0075 0090 0172 6674 1c64 1283 0101  .d.u...rft.d....
+00000580: 006e 1674 10a0 2b7c 0664 0b19 0064 00a1  .n.t..+|.d...d..
+00000590: 027d 0d7c 0d64 0075 0090 0172 7d74 1c64  .}.|.d.u...r}t.d
+000005a0: 137c 0664 0b19 009b 009d 0283 0101 007c  .|.d...........|
+000005b0: 0d90 0172 8674 1c74 2c7c 0d83 0183 0101  ...r.t.t,|......
+000005c0: 007c 03a0 1da1 0001 007c 056a 2d90 0172  .|.......|.j-..r
+000005d0: 9874 1c6a 2e7c 0264 148d 0101 007c 03a0  .t.j.|.d.....|..
+000005e0: 1da1 0001 007c 0690 0172 b67c 0664 0b19  .....|...r.|.d..
+000005f0: 00a0 2a64 15a1 0190 0173 b674 2f74 1083  ..*d.....s.t/t..
+00000600: 0144 005d 0e7d 0e74 307c 0e7c 0664 0b19  .D.].}.t0|.|.d..
+00000610: 0083 0290 0173 b474 107c 0e3d 0090 0171  .....s.t.|.=...q
+00000620: a774 016a 317c 0c74 107c 0664 1667 017c  .t.j1|.t.|.d.g.|
+00000630: 0274 0764 178d 0601 0064 0053 0029 184e  .t.d.....d.S.).N
+00000640: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000650: 0008 0000 0000 0000 0073 d200 0000 6500  .........s....e.
+00000660: 5a01 6400 5a02 5500 6503 6504 6505 6506  Z.d.Z.U.e.e.e.e.
+00000670: 1900 1900 6507 6a08 9400 7211 9400 6e01  ....e.j...r...n.
+00000680: 6401 6402 6701 6403 6404 6405 8d04 6602  d.d.g.d.d.d...f.
+00000690: 1900 6509 6406 3c00 6503 6504 6505 650a  ..e.d.<.e.e.e.e.
+000006a0: 1900 1900 6507 6a08 6401 6407 6701 6408  ....e.j.d.d.g.d.
+000006b0: 6404 6405 8d04 6602 1900 6509 6409 3c00  d.d...f...e.d.<.
+000006c0: 6503 6504 650b 1900 6507 6a08 6401 6404  e.e.e...e.j.d.d.
+000006d0: 640a 640b 6701 640c 8d04 6602 1900 6509  d.d.g.d...f...e.
+000006e0: 640d 3c00 6503 6504 650b 1900 6507 6a08  d.<.e.e.e...e.j.
+000006f0: 6401 6404 640a 640e 6701 640c 8d04 6602  d.d.d.d.g.d...f.
+00000700: 1900 6509 640f 3c00 6503 6504 650b 1900  ..e.d.<.e.e.e...
+00000710: 6507 6a08 6401 6404 640a 6410 6701 640c  e.j.d.d.d.d.g.d.
+00000720: 8d04 6602 1900 6509 6411 3c00 6401 5300  ..f...e.d.<.d.S.
+00000730: 2912 7a16 6d61 696e 2e3c 6c6f 6361 6c73  ).z.main.<locals
+00000740: 3e2e 4d79 6b65 4172 6773 4e7a 0b2d 2d6d  >.MykeArgsNz.--m
+00000750: 796b 652d 6669 6c65 5a09 4d59 4b45 5f46  yke-fileZ.MYKE_F
+00000760: 494c 457a 0f6d 796b 6520 7061 7261 6d65  ILEz.myke parame
+00000770: 7465 7273 2904 da07 6465 6661 756c 74da  ters)...default.
+00000780: 0566 6c61 6773 da03 656e 76da 0567 726f  .flags..env..gro
+00000790: 7570 da04 6669 6c65 7a0d 2d2d 6d79 6b65  up..filez.--myke
+000007a0: 2d6d 6f64 756c 655a 0b4d 594b 455f 4d4f  -moduleZ.MYKE_MO
+000007b0: 4455 4c45 da06 6d6f 6475 6c65 547a 0c2d  DULE..moduleTz.-
+000007c0: 2d6d 796b 652d 7461 736b 7329 0472 1e00  -myke-tasks).r..
+000007d0: 0000 7221 0000 00da 0965 7863 6c75 7369  ..r!.....exclusi
+000007e0: 7665 721f 0000 00da 0a6c 6973 745f 7461  ver......list_ta
+000007f0: 736b 737a 0e2d 2d6d 796b 652d 6578 706c  sksz.--myke-expl
+00000800: 6169 6eda 0765 7870 6c61 696e 7a0d 2d2d  ain..explainz.--
+00000810: 6d79 6b65 2d63 7265 6174 65da 0663 7265  myke-create..cre
+00000820: 6174 6529 0cda 085f 5f6e 616d 655f 5fda  ate)...__name__.
+00000830: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+00000840: 7561 6c6e 616d 655f 5f72 1800 0000 720a  ualname__r....r.
+00000850: 0000 0072 0900 0000 7206 0000 00da 0479  ...r....r......y
+00000860: 6170 78da 0361 7267 da0f 5f5f 616e 6e6f  apx..arg..__anno
+00000870: 7461 7469 6f6e 735f 5fda 0373 7472 da04  tations__..str..
+00000880: 626f 6f6c a900 a901 721c 0000 0072 3000  bool....r....r0.
+00000890: 0000 fa1b 2f64 726f 6e65 2f73 7263 2f73  ..../drone/src/s
+000008a0: 7263 2f6d 796b 652f 6d61 696e 2e70 79da  rc/myke/main.py.
+000008b0: 084d 796b 6541 7267 7319 0000 0073 6600  .MykeArgs....sf.
+000008c0: 0000 0a00 0202 0a01 0401 0a01 0401 0201  ................
+000008d0: 0201 04fc 02ff 08ff 0209 0a01 0401 0201  ................
+000008e0: 0401 0201 0201 04fc 02ff 08ff 0209 0601  ................
+000008f0: 0401 0201 0201 0201 0401 04fc 02ff 08ff  ................
 00000900: 0209 0601 0401 0201 0201 0201 0401 04fc  ................
 00000910: 02ff 08ff 0209 0601 0401 0201 0201 0201  ................
-00000920: 0401 04fc 02ff 08ff 0209 0601 0401 0201  ................
-00000930: 0201 0201 0401 04fc 02ff 0cff 7233 0000  ............r3..
-00000940: 007a 0b2d 2d6d 796b 652d 6865 6c70 7a0e  .z.--myke-helpz.
-00000950: 2d2d 6d79 6b65 2d76 6572 7369 6f6e 2905  --myke-version).
-00000960: da04 7072 6f67 da0c 7072 6f67 5f76 6572  ..prog..prog_ver
-00000970: 7369 6f6e da0a 6865 6c70 5f66 6c61 6773  sion..help_flags
-00000980: da0d 7665 7273 696f 6e5f 666c 6167 73da  ..version_flags.
-00000990: 1063 6f6d 706c 6574 696f 6e5f 666c 6167  .completion_flag
-000009a0: 7372 0c00 0000 5429 02da 0a61 7267 735f  sr....T)...args_
-000009b0: 6d6f 6465 6cda 1873 6b69 705f 7079 6461  model..skip_pyda
-000009c0: 6e74 6963 5f76 616c 6964 6174 696f 6e63  ntic_validationc
-000009d0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-000009e0: 0400 0000 5300 0000 7314 0000 0067 007c  ....S...s....g.|
-000009f0: 005d 067d 017c 01a0 00a1 0091 0271 0253  .].}.|.......q.S
-00000a00: 0072 3000 0000 2901 da08 6162 736f 6c75  .r0...)...absolu
-00000a10: 7465 2902 da02 2e30 da01 7872 3000 0000  te)....0..xr0...
-00000a20: 7230 0000 0072 3200 0000 da0a 3c6c 6973  r0...r2.....<lis
-00000a30: 7463 6f6d 703e 6d00 0000 7302 0000 0014  tcomp>m...s.....
-00000a40: 007a 186d 6169 6e2e 3c6c 6f63 616c 733e  .z.main.<locals>
-00000a50: 2e3c 6c69 7374 636f 6d70 3e72 0100 0000  .<listcomp>r....
-00000a60: 7a09 4372 6561 7465 643a 20fa 0127 7a1d  z.Created: ..'z.
-00000a70: 2720 6e6f 7420 666f 756e 642e 2043 7265  ' not found. Cre
-00000a80: 6174 6520 6974 2075 7369 6e67 3a7a 0224  ate it using:z.$
-00000a90: 207a 1c20 2d2d 6d79 6b65 2d63 7265 6174   z. --myke-creat
-00000aa0: 6520 2d2d 6d79 6b65 2d66 696c 6520 27fa  e --myke-file '.
-00000ab0: 012d 7a36 5468 6572 6520 6973 206e 6f20  .-z6There is no 
-00000ac0: 726f 6f74 2074 6173 6b2e 2050 726f 7669  root task. Provi
-00000ad0: 6465 2061 2074 6173 6b20 6e61 6d65 2074  de a task name t
-00000ae0: 6f20 6578 706c 6169 6e2e 7a1b 4769 7665  o explain.z.Give
-00000af0: 6e20 7461 736b 206e 616d 6520 6e6f 7420  n task name not 
-00000b00: 666f 756e 643a 2029 0172 3400 0000 7a02  found: ).r4...z.
-00000b10: 2d2d 7a06 2d2d 6865 6c70 2905 da11 6e61  --z.--help)...na
-00000b20: 6d65 645f 7375 6263 6f6d 6d61 6e64 73da  med_subcommands.
-00000b30: 0461 7267 73da 0c64 6566 6175 6c74 5f61  .args..default_a
-00000b40: 7267 7372 3400 0000 7235 0000 0029 3272  rgsr4...r5...)2r
-00000b50: 0300 0000 722b 0000 00da 0574 7970 6573  ....r+.....types
-00000b60: da09 4461 7461 636c 6173 7372 2e00 0000  ..Dataclassr....
-00000b70: 7211 0000 00da 0e41 7267 756d 656e 7450  r......ArgumentP
-00000b80: 6172 7365 7272 0d00 0000 da0d 6164 645f  arserr......add_
-00000b90: 6172 6775 6d65 6e74 7372 1b00 0000 da04  argumentsr......
-00000ba0: 6172 6776 da0a 7072 696e 745f 6865 6c70  argv..print_help
-00000bb0: da04 6578 6974 da19 7061 7273 655f 6b6e  ..exit..parse_kn
-00000bc0: 6f77 6e5f 6172 6773 5f74 6f5f 6d6f 6465  own_args_to_mode
-00000bd0: 6cda 0a69 7369 6e73 7461 6e63 6572 0600  l..isinstancer..
-00000be0: 0000 da06 6578 6973 7473 da11 4669 6c65  ....exists..File
-00000bf0: 4e6f 7446 6f75 6e64 4572 726f 7272 1300  NotFoundErrorr..
-00000c00: 0000 720e 0000 0072 3b00 0000 7222 0000  ..r....r;...r"..
-00000c10: 0072 1000 0000 7202 0000 0072 1900 0000  .r....r....r....
-00000c20: da02 6f73 da05 6368 6469 7272 2700 0000  ..os..chdirr'...
-00000c30: 7215 0000 00da 086d 796b 6566 696c 6572  r......mykefiler
-00000c40: 1400 0000 da08 7361 6d65 6669 6c65 7217  ......samefiler.
-00000c50: 0000 00da 076c 696e 6573 6570 da08 6669  .....linesep..fi
-00000c60: 6c65 6e61 6d65 7223 0000 0072 1600 0000  lenamer#...r....
-00000c70: 720f 0000 00da 0565 7272 6f72 da03 706f  r......error..po
-00000c80: 7072 1200 0000 7226 0000 00da 0a73 7461  pr....r&.....sta
-00000c90: 7274 7377 6974 68da 0367 6574 7205 0000  rtswith..getr...
-00000ca0: 0072 2500 0000 da05 7461 736b 73da 046c  .r%.....tasks..l
-00000cb0: 6973 7472 0400 0000 da03 7275 6e29 0f72  istr......run).r
-00000cc0: 1c00 0000 7233 0000 0072 3400 0000 da06  ....r3...r4.....
-00000cd0: 7061 7273 6572 7242 0000 005a 096d 796b  parserrB...Z.myk
-00000ce0: 655f 6172 6773 5a09 7461 736b 5f61 7267  e_argsZ.task_arg
-00000cf0: 735a 0972 6570 6f5f 726f 6f74 da08 6f75  sZ.repo_root..ou
-00000d00: 745f 6669 6c65 da01 66da 0165 da01 6d5a  t_file..f..e..mZ
-00000d10: 0972 6f6f 745f 7461 736b 5a0c 6578 706c  .root_taskZ.expl
-00000d20: 6169 6e5f 7468 6973 da01 6b72 3000 0000  ain_this..kr0...
-00000d30: 7231 0000 0072 3200 0000 721a 0000 0018  r1...r2...r.....
-00000d40: 0000 0073 de00 0000 0201 1a01 102f 0402  ...s........./..
-00000d50: 0201 0201 0401 0401 0201 06fb 0a07 0e02  ................
-00000d60: 0402 0801 0801 0404 0201 0201 0201 0afd  ................
-00000d70: 0e05 0402 0a01 0801 0801 0801 0401 0801  ................
-00000d80: 0801 0602 1401 0c01 1001 0a02 0601 0401  ................
-00000d90: 0a01 0280 1cfd 0605 0c01 1201 0602 0602  ................
-00000da0: 1801 0e01 0e01 0801 0202 0201 0a01 1201  ................
-00000db0: 0c01 0280 04fe 1004 0801 0201 0802 0401  ................
-00000dc0: 04ff 0402 04fe 0203 04fd 0403 04fd 0404  ................
-00000dd0: 04fc 04fe 1409 0880 02f5 080d 0a01 0c01  ................
-00000de0: 0480 1002 1a01 0880 02ff 0c03 0802 0401  ................
-00000df0: 1602 0401 0a01 0801 0280 1002 0a01 1201  ................
-00000e00: 0602 0c01 0802 0802 0c01 0801 1602 0c01  ................
-00000e10: 1001 0601 0480 0402 0201 0201 0201 0401  ................
-00000e20: 0201 0201 0afa 721a 0000 0029 014e 2929  ......r....).N))
-00000e30: 724f 0000 0072 1b00 0000 da0a 636f 6e74  rO...r......cont
-00000e40: 6578 746c 6962 7202 0000 00da 0b64 6174  extlibr......dat
-00000e50: 6163 6c61 7373 6573 7203 0000 0072 0400  aclassesr....r..
-00000e60: 0000 da07 696e 7370 6563 7472 0500 0000  ....inspectr....
-00000e70: da07 7061 7468 6c69 6272 0600 0000 da06  ..pathlibr......
-00000e80: 7479 7069 6e67 7207 0000 0072 0800 0000  typingr....r....
-00000e90: 7209 0000 0072 0a00 0000 720b 0000 0072  r....r....r....r
-00000ea0: 2b00 0000 720d 0000 00da 0a65 7863 6570  +...r......excep
-00000eb0: 7469 6f6e 7372 0e00 0000 720f 0000 00da  tionsr....r.....
-00000ec0: 0767 6c6f 6261 6c73 7210 0000 0072 1100  .globalsr....r..
-00000ed0: 0000 7212 0000 0072 1300 0000 da07 696f  ..r....r......io
-00000ee0: 2e65 6368 6f72 1400 0000 da08 696f 2e77  .echor......io.w
-00000ef0: 7269 7465 7215 0000 0072 5900 0000 7216  riter....rY...r.
-00000f00: 0000 0072 1700 0000 7244 0000 0072 1800  ...r....rD...r..
-00000f10: 0000 da05 7574 696c 7372 1900 0000 da07  ....utilsr......
-00000f20: 5f5f 616c 6c5f 5f72 2e00 0000 721a 0000  __all__r....r...
-00000f30: 0072 3000 0000 7230 0000 0072 3000 0000  .r0...r0...r0...
-00000f40: 7232 0000 00da 083c 6d6f 6475 6c65 3e01  r2.....<module>.
-00000f50: 0000 0073 2600 0000 0800 0801 0c01 0c01  ...s&...........
-00000f60: 0c01 0c01 0c01 1c01 0802 0c02 1001 1801  ................
-00000f70: 0c01 0c01 1001 0c01 0c01 0802 2403       ............$.
+00000920: 0401 04fc 02ff 0cff 7233 0000 007a 0b2d  ........r3...z.-
+00000930: 2d6d 796b 652d 6865 6c70 7a0e 2d2d 6d79  -myke-helpz.--my
+00000940: 6b65 2d76 6572 7369 6f6e 2905 da04 7072  ke-version)...pr
+00000950: 6f67 da0c 7072 6f67 5f76 6572 7369 6f6e  og..prog_version
+00000960: da0a 6865 6c70 5f66 6c61 6773 da0d 7665  ..help_flags..ve
+00000970: 7273 696f 6e5f 666c 6167 73da 1063 6f6d  rsion_flags..com
+00000980: 706c 6574 696f 6e5f 666c 6167 7372 0c00  pletion_flagsr..
+00000990: 0000 5429 02da 0a61 7267 735f 6d6f 6465  ..T)...args_mode
+000009a0: 6cda 1873 6b69 705f 7079 6461 6e74 6963  l..skip_pydantic
+000009b0: 5f76 616c 6964 6174 696f 6e63 0100 0000  _validationc....
+000009c0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+000009d0: 5300 0000 7314 0000 0067 007c 005d 067d  S...s....g.|.].}
+000009e0: 017c 01a0 00a1 0091 0271 0253 0072 3000  .|.......q.S.r0.
+000009f0: 0000 2901 da08 6162 736f 6c75 7465 2902  ..)...absolute).
+00000a00: da02 2e30 da01 7872 3000 0000 7230 0000  ...0..xr0...r0..
+00000a10: 0072 3200 0000 da0a 3c6c 6973 7463 6f6d  .r2.....<listcom
+00000a20: 703e 6900 0000 7302 0000 0014 007a 186d  p>i...s......z.m
+00000a30: 6169 6e2e 3c6c 6f63 616c 733e 2e3c 6c69  ain.<locals>.<li
+00000a40: 7374 636f 6d70 3e72 0100 0000 7a09 4372  stcomp>r....z.Cr
+00000a50: 6561 7465 643a 20fa 0127 7a1d 2720 6e6f  eated: ..'z.' no
+00000a60: 7420 666f 756e 642e 2043 7265 6174 6520  t found. Create 
+00000a70: 6974 2075 7369 6e67 3a7a 0224 207a 1c20  it using:z.$ z. 
+00000a80: 2d2d 6d79 6b65 2d63 7265 6174 6520 2d2d  --myke-create --
+00000a90: 6d79 6b65 2d66 696c 6520 27fa 012d 7a36  myke-file '..-z6
+00000aa0: 5468 6572 6520 6973 206e 6f20 726f 6f74  There is no root
+00000ab0: 2074 6173 6b2e 2050 726f 7669 6465 2061   task. Provide a
+00000ac0: 2074 6173 6b20 6e61 6d65 2074 6f20 6578   task name to ex
+00000ad0: 706c 6169 6e2e 7a1b 4769 7665 6e20 7461  plain.z.Given ta
+00000ae0: 736b 206e 616d 6520 6e6f 7420 666f 756e  sk name not foun
+00000af0: 643a 2029 0172 3400 0000 7a02 2d2d 7a05  d: ).r4...z.--z.
+00000b00: 2d2d 7475 6929 05da 116e 616d 6564 5f73  --tui)...named_s
+00000b10: 7562 636f 6d6d 616e 6473 da04 6172 6773  ubcommands..args
+00000b20: da0c 6465 6661 756c 745f 6172 6773 7234  ..default_argsr4
+00000b30: 0000 0072 3500 0000 2932 7203 0000 0072  ...r5...)2r....r
+00000b40: 2b00 0000 da05 7479 7065 73da 0944 6174  +.....types..Dat
+00000b50: 6163 6c61 7373 722e 0000 0072 1100 0000  aclassr....r....
+00000b60: da0e 4172 6775 6d65 6e74 5061 7273 6572  ..ArgumentParser
+00000b70: 720d 0000 00da 0d61 6464 5f61 7267 756d  r......add_argum
+00000b80: 656e 7473 721b 0000 00da 0461 7267 76da  entsr......argv.
+00000b90: 1970 6172 7365 5f6b 6e6f 776e 5f61 7267  .parse_known_arg
+00000ba0: 735f 746f 5f6d 6f64 656c da0a 6973 696e  s_to_model..isin
+00000bb0: 7374 616e 6365 7206 0000 00da 0665 7869  stancer......exi
+00000bc0: 7374 73da 1146 696c 654e 6f74 466f 756e  sts..FileNotFoun
+00000bd0: 6445 7272 6f72 7213 0000 0072 0e00 0000  dErrorr....r....
+00000be0: 723b 0000 0072 2200 0000 7210 0000 0072  r;...r"...r....r
+00000bf0: 0200 0000 7219 0000 00da 026f 73da 0563  ....r......os..c
+00000c00: 6864 6972 7227 0000 0072 1500 0000 da08  hdirr'...r......
+00000c10: 6d79 6b65 6669 6c65 7214 0000 00da 0465  mykefiler......e
+00000c20: 7869 74da 0873 616d 6566 696c 6572 1700  xit..samefiler..
+00000c30: 0000 da0a 7072 696e 745f 6865 6c70 da07  ....print_help..
+00000c40: 6c69 6e65 7365 70da 0866 696c 656e 616d  linesep..filenam
+00000c50: 6572 2300 0000 7216 0000 0072 0f00 0000  er#...r....r....
+00000c60: da05 6572 726f 72da 0370 6f70 7212 0000  ..error..popr...
+00000c70: 0072 2600 0000 da0a 7374 6172 7473 7769  .r&.....startswi
+00000c80: 7468 da03 6765 7472 0500 0000 7225 0000  th..getr....r%..
+00000c90: 00da 0574 6173 6b73 da04 6c69 7374 7204  ...tasks..listr.
+00000ca0: 0000 00da 0372 756e 290f 721c 0000 0072  .....run).r....r
+00000cb0: 3300 0000 7234 0000 00da 0670 6172 7365  3...r4.....parse
+00000cc0: 7272 4200 0000 5a09 6d79 6b65 5f61 7267  rrB...Z.myke_arg
+00000cd0: 735a 0974 6173 6b5f 6172 6773 5a09 7265  sZ.task_argsZ.re
+00000ce0: 706f 5f72 6f6f 74da 086f 7574 5f66 696c  po_root..out_fil
+00000cf0: 65da 0166 da01 65da 016d 5a09 726f 6f74  e..f..e..mZ.root
+00000d00: 5f74 6173 6b5a 0c65 7870 6c61 696e 5f74  _taskZ.explain_t
+00000d10: 6869 73da 016b 7230 0000 0072 3100 0000  his..kr0...r1...
+00000d20: 7232 0000 0072 1a00 0000 1800 0000 73d8  r2...r........s.
+00000d30: 0000 0002 011a 0110 2f04 0202 0102 0104  ......../.......
+00000d40: 0104 0102 0106 fb0a 070e 0204 0402 0102  ................
+00000d50: 0102 010a fd0e 0504 020a 0108 0108 0108  ................
+00000d60: 0104 0108 0108 0106 0214 010c 0110 010a  ................
+00000d70: 0206 0104 010a 0102 801c fd06 050c 0112  ................
+00000d80: 0106 0206 0218 010e 010e 0108 0102 0202  ................
+00000d90: 010a 0112 010c 0102 8004 fe10 0408 0102  ................
+00000da0: 0108 0204 0104 ff04 0204 fe02 0304 fd04  ................
+00000db0: 0304 fd04 0404 fc04 fe14 0908 8002 f508  ................
+00000dc0: 0d0a 010c 0104 8010 021a 0108 8002 ff0c  ................
+00000dd0: 0308 0204 0116 0204 010a 0108 0102 8010  ................
+00000de0: 020a 0112 0106 020c 0108 0208 020c 0108  ................
+00000df0: 0116 020c 0110 0106 0104 8004 0202 0102  ................
+00000e00: 0102 0104 0102 0102 010a fa72 1a00 0000  ...........r....
+00000e10: 2901 4e29 2972 4d00 0000 721b 0000 00da  ).N))rM...r.....
+00000e20: 0a63 6f6e 7465 7874 6c69 6272 0200 0000  .contextlibr....
+00000e30: da0b 6461 7461 636c 6173 7365 7372 0300  ..dataclassesr..
+00000e40: 0000 7204 0000 00da 0769 6e73 7065 6374  ..r......inspect
+00000e50: 7205 0000 00da 0770 6174 686c 6962 7206  r......pathlibr.
+00000e60: 0000 00da 0674 7970 696e 6772 0700 0000  .....typingr....
+00000e70: 7208 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
+00000e80: 0b00 0000 722b 0000 0072 0d00 0000 da0a  ....r+...r......
+00000e90: 6578 6365 7074 696f 6e73 720e 0000 0072  exceptionsr....r
+00000ea0: 0f00 0000 da07 676c 6f62 616c 7372 1000  ......globalsr..
+00000eb0: 0000 7211 0000 0072 1200 0000 7213 0000  ..r....r....r...
+00000ec0: 00da 0769 6f2e 6563 686f 7214 0000 00da  ...io.echor.....
+00000ed0: 0869 6f2e 7772 6974 6572 1500 0000 7259  .io.writer....rY
+00000ee0: 0000 0072 1600 0000 7217 0000 0072 4400  ...r....r....rD.
+00000ef0: 0000 7218 0000 00da 0575 7469 6c73 7219  ..r......utilsr.
+00000f00: 0000 00da 075f 5f61 6c6c 5f5f 722e 0000  .....__all__r...
+00000f10: 0072 1a00 0000 7230 0000 0072 3000 0000  .r....r0...r0...
+00000f20: 7230 0000 0072 3200 0000 da08 3c6d 6f64  r0...r2.....<mod
+00000f30: 756c 653e 0100 0000 7326 0000 0008 0008  ule>....s&......
+00000f40: 010c 010c 010c 010c 010c 011c 0108 020c  ................
+00000f50: 0210 0118 010c 010c 0110 010c 010c 0108  ................
+00000f60: 0224 03                                  .$.
```

### Comparing `myke-0.2.0/src/myke/__pycache__/run.cpython-310.pyc` & `myke-0.3.0/src/myke/__pycache__/run.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jul 20 04:38:03 2023 UTC, .py size: 5815 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2bba b864 b716 0000  o.......+..d....
+00000000: 6f0d 0d0a 0000 0000 a81d d364 b716 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0173 fc00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a03 6401 6403 6c04 5a04 6401  d.l.Z.d.d.l.Z.d.
 00000050: 6403 6c05 5a05 6401 6403 6c06 5a06 6401  d.l.Z.d.d.l.Z.d.
 00000060: 6404 6c07 6d08 5a08 0100 6401 6405 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 6d0b 5a0b 0100 6406 6407 6c0c  m.Z.m.Z...d.d.l.
```

### Comparing `myke-0.2.0/src/myke/__pycache__/tasks.cpython-310.pyc` & `myke-0.3.0/src/myke/__pycache__/tasks.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jul 20 04:38:03 2023 UTC, .py size: 5865 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2bba b864 e916 0000  o.......+..d....
+00000000: 6f0d 0d0a 0000 0000 a81d d364 e916 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000c 0000 0040 0000 0173 fa00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a04 6401 6403 6c05 5a05 6401  d.l.Z.d.d.l.Z.d.
 00000050: 6404 6c06 6d07 5a07 6d08 5a08 0100 6401  d.l.m.Z.m.Z...d.
 00000060: 6405 6c09 6d0a 5a0a 0100 6401 6406 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6401 6407 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `myke-0.2.0/src/myke/__pycache__/types.cpython-310.pyc` & `myke-0.3.0/src/myke/__pycache__/types.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jul 20 04:38:03 2023 UTC, .py size: 429 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2bba b864 ad01 0000  o.......+..d....
+00000000: 6f0d 0d0a 0000 0000 a81d d364 ad01 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0173 5800 0000 6400  .....@...sX...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c04 6d06 5a06 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c04 6d07 5a07 0100 6700 6406 a201  d.l.m.Z...g.d...
 00000070: 5a08 4700 6407 6408 8400 6408 6507 8303  Z.G.d.d...d.e...
```

### Comparing `myke-0.2.0/src/myke/__pycache__/utils.cpython-310.pyc` & `myke-0.3.0/src/myke/__pycache__/utils.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jul 20 04:38:03 2023 UTC, .py size: 3988 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2bba b864 940f 0000  o.......+..d....
+00000000: 6f0d 0d0a 0000 0000 a81d d364 940f 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0173 c200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 5a03 6400 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c08 6d09 5a09 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6406 6c0a 6d0b 5a0b 0100 6400 6407 6c0c  d.l.m.Z...d.d.l.
```

### Comparing `myke-0.2.0/src/myke/exceptions.py` & `myke-0.3.0/src/myke/exceptions.py`

 * *Files identical despite different names*

### Comparing `myke-0.2.0/src/myke/io/__pycache__/echo.cpython-310.pyc` & `myke-0.3.0/src/myke/io/__pycache__/echo.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jul 20 04:38:03 2023 UTC, .py size: 5929 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2bba b864 2917 0000  o.......+..d)...
+00000000: 6f0d 0d0a 0000 0000 a81d d364 2917 0000  o..........d)...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5e00 0000 6400  .....@...s^...d.
 00000030: 5a00 6401 6402 6c01 5a02 6401 6402 6c03  Z.d.d.l.Z.d.d.l.
 00000040: 5a03 6401 6403 6c04 6d05 5a05 6d06 5a06  Z.d.d.l.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0b 5a0b 6d0c 5a0c 0100 6404 6405 6c0d  m.Z.m.Z...d.d.l.
 00000070: 6d0e 5a0e 6d0f 5a0f 0100 4700 6406 6407  m.Z.m.Z...G.d.d.
```

### Comparing `myke-0.2.0/src/myke/io/__pycache__/read.cpython-310.pyc` & `myke-0.3.0/src/myke/io/__pycache__/read.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jul 20 04:38:03 2023 UTC, .py size: 7195 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2bba b864 1b1c 0000  o.......+..d....
+00000000: 6f0d 0d0a 0000 0000 a81d d364 1b1c 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7c00 0000 6400  .....@...s|...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6401 6404 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6401 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  m.Z.m.Z.m.Z.m.Z.
 00000070: 0100 6501 6a0d 6406 6b05 722e 6401 6407  ..e.j.d.k.r.d.d.
@@ -380,15 +380,15 @@
 000017b0: 2020 3e3e 3e20 6d79 6b65 2e72 6561 642e    >>> myke.read.
 000017c0: 646f 7466 696c 6528 272f 7061 7468 2f74  dotfile('/path/t
 000017d0: 6f2f 7661 7273 2e65 6e76 2729 2020 2320  o/vars.env')  # 
 000017e0: 646f 6374 6573 743a 202b 534b 4950 0a20  doctest: +SKIP. 
 000017f0: 2020 2020 2020 2072 0100 0000 2901 da08         r....)...
 00001800: 5374 7269 6e67 494f 2901 da0d 646f 7465  StringIO)...dote
 00001810: 6e76 5f76 616c 7565 7329 01da 0673 7472  nv_values)...str
-00001820: 6561 6d29 07da 0269 6f72 5100 0000 da06  eam)...iorQ.....
+00001820: 6561 6d29 07da 0269 6f72 5100 0000 5a06  eam)...iorQ...Z.
 00001830: 646f 7465 6e76 7252 0000 0072 2600 0000  dotenvrR...r&...
 00001840: 7202 0000 0072 1300 0000 2905 7214 0000  r....r....).r...
 00001850: 0072 2900 0000 7223 0000 0072 5100 0000  .r)...r#...rQ...
 00001860: 7252 0000 0072 1500 0000 7215 0000 0072  rR...r....r....r
 00001870: 1600 0000 da07 646f 7466 696c 65a6 0000  ......dotfile...
 00001880: 0073 0a00 0000 0c0a 0c02 0402 1a01 04ff  .s..............
 00001890: 7a0c 7265 6164 2e64 6f74 6669 6c65 6301  z.read.dotfilec.
@@ -402,32 +402,32 @@
 00001910: 2020 2020 203e 3e3e 2069 6d70 6f72 7420       >>> import 
 00001920: 6d79 6b65 0a20 2020 2020 2020 2020 2020  myke.           
 00001930: 202e 2e2e 0a20 2020 2020 2020 2020 2020   ....           
 00001940: 203e 3e3e 206d 796b 652e 7265 6164 2e65   >>> myke.read.e
 00001950: 6e76 6669 6c65 2827 2f70 6174 682f 746f  nvfile('/path/to
 00001960: 2f76 6172 732e 656e 7627 2920 2023 2064  /vars.env')  # d
 00001970: 6f63 7465 7374 3a20 2b53 4b49 500a 2020  octest: +SKIP.  
-00001980: 2020 2020 2020 2901 7256 0000 0072 2e00        ).rV...r..
+00001980: 2020 2020 2020 2901 7255 0000 0072 2e00        ).rU...r..
 00001990: 0000 7215 0000 0072 1500 0000 7216 0000  ..r....r....r...
 000019a0: 00da 0765 6e76 6669 6c65 b800 0000 7250  ...envfile....rP
 000019b0: 0000 007a 0c72 6561 642e 656e 7666 696c  ...z.read.envfil
 000019c0: 65da 0461 6464 7263 0100 0000 0000 0000  e..addrc........
 000019d0: 0000 0000 0600 0000 0600 0000 4b00 0000  ............K...
 000019e0: 7348 0000 0064 0164 006c 007d 027c 01a0  sH...d.d.l.}.|..
 000019f0: 0164 027c 00a1 027d 007c 01a0 0164 0364  .d.|...}.|...d.d
 00001a00: 04a1 027d 037c 01a0 0164 0564 06a1 027d  ...}.|...d.d...}
 00001a10: 047c 026a 0264 087c 037c 007c 0464 079c  .|.j.d.|.|.|.d..
 00001a20: 037c 01a4 018e 017d 057c 0553 0029 094e  .|.....}.|.S.).N
 00001a30: 7201 0000 00da 0375 726c da06 6d65 7468  r......url..meth
 00001a40: 6f64 da03 4745 54da 0774 696d 656f 7574  od..GET..timeout
-00001a50: 720b 0000 0029 0372 5a00 0000 7259 0000  r....).rZ...rY..
-00001a60: 0072 5c00 0000 7215 0000 0029 03da 0872  .r\...r....)...r
+00001a50: 720b 0000 0029 0372 5900 0000 7258 0000  r....).rY...rX..
+00001a60: 0072 5b00 0000 7215 0000 0029 03da 0872  .r[...r....)...r
 00001a70: 6571 7565 7374 73da 0370 6f70 5a07 7265  equests..popZ.re
-00001a80: 7175 6573 7429 0672 5800 0000 7223 0000  quest).rX...r#..
-00001a90: 0072 5d00 0000 725a 0000 0072 5c00 0000  .r]...rZ...r\...
+00001a80: 7175 6573 7429 0672 5700 0000 7223 0000  quest).rW...r#..
+00001a90: 0072 5c00 0000 7259 0000 0072 5b00 0000  .r\...rY...r[...
 00001aa0: da04 7265 7370 7215 0000 0072 1500 0000  ..respr....r....
 00001ab0: 7216 0000 00da 045f 7572 6cc4 0000 0073  r......_url....s
 00001ac0: 1800 0000 0802 0c02 0c01 0c01 0601 0201  ................
 00001ad0: 0201 0201 04fd 0204 06fc 0406 7a09 7265  ............z.re
 00001ae0: 6164 2e5f 7572 6c63 0200 0000 0000 0000  ad._urlc........
 00001af0: 0000 0000 0400 0000 0400 0000 4b00 0000  ............K...
 00001b00: 731a 0000 007c 006a 0064 0364 017c 0169  s....|.j.d.d.|.i
@@ -447,19 +447,19 @@
 00001be0: 706f 7274 206d 796b 650a 2020 2020 2020  port myke.      
 00001bf0: 2020 2020 2020 2e2e 2e0a 2020 2020 2020        ....      
 00001c00: 2020 2020 2020 3e3e 3e20 6d79 6b65 2e72        >>> myke.r
 00001c10: 6561 642e 7572 6c28 2768 7474 7073 3a2f  ead.url('https:/
 00001c20: 2f67 6974 6875 622e 636f 6d2f 2e2e 2e2f  /github.com/.../
 00001c30: 5245 4144 4d45 2e6d 6427 2920 2023 2064  README.md')  # d
 00001c40: 6f63 7465 7374 3a20 2b53 4b49 500a 2020  octest: +SKIP.  
-00001c50: 2020 2020 2020 7258 0000 004e 7215 0000        rX...Nr...
-00001c60: 0029 0272 6000 0000 7213 0000 0029 0472  .).r`...r....).r
-00001c70: 1400 0000 7258 0000 0072 2300 0000 5a09  ....rX...r#...Z.
+00001c50: 2020 2020 2020 7257 0000 004e 7215 0000        rW...Nr...
+00001c60: 0029 0272 5f00 0000 7213 0000 0029 0472  .).r_...r....).r
+00001c70: 1400 0000 7257 0000 0072 2300 0000 5a09  ....rW...r#...Z.
 00001c80: 7265 7370 5f74 6578 7472 1500 0000 7215  resp_textr....r.
-00001c90: 0000 0072 1600 0000 7259 0000 00d3 0000  ...r....rY......
+00001c90: 0000 0072 1600 0000 7258 0000 00d3 0000  ...r....rX......
 00001ca0: 0073 0400 0000 160d 0401 7a08 7265 6164  .s........z.read
 00001cb0: 2e75 726c 6302 0000 0000 0000 0000 0000  .urlc...........
 00001cc0: 0004 0000 0005 0000 000b 0000 0073 2e00  .............s..
 00001cd0: 0000 7c00 6a00 6405 6401 7c01 6901 7c02  ..|.j.d.d.|.i.|.
 00001ce0: a401 8e01 a001 a100 8900 7c00 a002 8700  ..........|.....
 00001cf0: 6601 6402 6403 8408 a101 7d03 7c03 5300  f.d.d.....}.|.S.
 00001d00: 2906 6134 0100 0050 6172 7365 204a 534f  ).a4...Parse JSO
@@ -477,41 +477,41 @@
 00001dc0: 706f 7274 206d 796b 650a 2020 2020 2020  port myke.      
 00001dd0: 2020 2020 2020 2e2e 2e0a 2020 2020 2020        ....      
 00001de0: 2020 2020 2020 3e3e 3e20 6d79 6b65 2e72        >>> myke.r
 00001df0: 6561 642e 7572 6c5f 6a73 6f6e 2827 6874  ead.url_json('ht
 00001e00: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 00001e10: 2f2e 2e2e 2f64 6174 612e 6a73 6f6e 2729  /.../data.json')
 00001e20: 2020 2320 646f 6374 6573 743a 202b 534b    # doctest: +SK
-00001e30: 4950 0a20 2020 2020 2020 2072 5800 0000  IP.        rX...
+00001e30: 4950 0a20 2020 2020 2020 2072 5700 0000  IP.        rW...
 00001e40: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
 00001e50: 0001 0000 0013 0000 0073 0400 0000 8800  .........s......
 00001e60: 5300 7219 0000 0072 1500 0000 7215 0000  S.r....r....r...
-00001e70: 00a9 0172 5f00 0000 7215 0000 0072 1600  ...r_...r....r..
+00001e70: 00a9 0172 5e00 0000 7215 0000 0072 1600  ...r^...r....r..
 00001e80: 0000 7238 0000 00f1 0000 0072 3900 0000  ..r8.......r9...
 00001e90: 7a1f 7265 6164 2e75 726c 5f6a 736f 6e2e  z.read.url_json.
 00001ea0: 3c6c 6f63 616c 733e 2e3c 6c61 6d62 6461  <locals>.<lambda
-00001eb0: 3e4e 7215 0000 0029 0372 6000 0000 7231  >Nr....).r`...r1
+00001eb0: 3e4e 7215 0000 0029 0372 5f00 0000 7231  >Nr....).r_...r1
 00001ec0: 0000 0072 2600 0000 2904 7214 0000 0072  ...r&...).r....r
-00001ed0: 5800 0000 7223 0000 005a 0972 6573 705f  X...r#...Z.resp_
-00001ee0: 6469 6374 7215 0000 0072 6100 0000 7216  dictr....ra...r.
+00001ed0: 5700 0000 7223 0000 005a 0972 6573 705f  W...r#...Z.resp_
+00001ee0: 6469 6374 7215 0000 0072 6000 0000 7216  dictr....r`...r.
 00001ef0: 0000 00da 0875 726c 5f6a 736f 6ee3 0000  .....url_json...
 00001f00: 0073 0600 0000 180d 1201 0401 7a0d 7265  .s..........z.re
 00001f10: 6164 2e75 726c 5f6a 736f 6e4e 2901 720e  ad.url_jsonN).r.
 00001f20: 0000 0029 1eda 085f 5f6e 616d 655f 5fda  ...)...__name__.
 00001f30: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
 00001f40: 7561 6c6e 616d 655f 5f72 1b00 0000 7217  ualname__r....r.
 00001f50: 0000 00da 0c73 7461 7469 636d 6574 686f  .....staticmetho
 00001f60: 6472 0500 0000 720c 0000 0072 0700 0000  dr....r....r....
 00001f70: 7221 0000 00da 0b63 6c61 7373 6d65 7468  r!.....classmeth
 00001f80: 6f64 7206 0000 0072 2600 0000 7209 0000  odr....r&...r...
 00001f90: 0072 0400 0000 7213 0000 0072 0300 0000  .r....r....r....
 00001fa0: 7208 0000 0072 2f00 0000 7231 0000 0072  r....r/...r1...r
 00001fb0: 3400 0000 723e 0000 0072 4200 0000 724d  4...r>...rB...rM
-00001fc0: 0000 0072 4f00 0000 7256 0000 0072 5700  ...rO...rV...rW.
-00001fd0: 0000 7260 0000 0072 5900 0000 7262 0000  ..r`...rY...rb..
+00001fc0: 0000 0072 4f00 0000 7255 0000 0072 5600  ...rO...rU...rV.
+00001fd0: 0000 725f 0000 0072 5800 0000 7261 0000  ..r_...rX...ra..
 00001fe0: 0072 1500 0000 7215 0000 0072 1500 0000  .r....r....r....
 00001ff0: 7216 0000 0072 0d00 0000 0e00 0000 735e  r....r........s^
 00002000: 0000 0008 0018 0102 0320 0102 0502 010a  ......... ......
 00002010: 0202 fe02 0302 fd0a 040c fc02 0a22 0102  ............."..
 00002020: 1206 011e 0102 0c06 0122 0102 0c06 0122  ........."....."
 00002030: 0102 0e06 0126 0102 1206 0122 0102 0f06  .....&....."....
 00002040: 0122 0102 1106 0122 0102 0a06 0122 0102  ."....."....."..
```

### Comparing `myke-0.2.0/src/myke/io/__pycache__/write.cpython-310.pyc` & `myke-0.3.0/src/myke/io/__pycache__/write.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jul 20 04:38:03 2023 UTC, .py size: 3669 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2bba b864 550e 0000  o.......+..dU...
+00000000: 6f0d 0d0a 0000 0000 a81d d364 550e 0000  o..........dU...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5a00 0000 6400  .....@...sZ...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 6405  m.Z.m.Z.m.Z...d.
 00000060: 6406 6c09 6d0a 5a0a 0100 6405 6407 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 4700 6408 6409 8400 6409  m.Z...G.d.d...d.
```

### Comparing `myke-0.2.0/src/myke/io/echo.py` & `myke-0.3.0/src/myke/io/echo.py`

 * *Files identical despite different names*

### Comparing `myke-0.2.0/src/myke/io/read.py` & `myke-0.3.0/src/myke/io/read.py`

 * *Files identical despite different names*

### Comparing `myke-0.2.0/src/myke/io/write.py` & `myke-0.3.0/src/myke/io/write.py`

 * *Files identical despite different names*

### Comparing `myke-0.2.0/src/myke/main.py` & `myke-0.3.0/src/myke/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,18 +79,14 @@
         version_flags=["--myke-version"],
         completion_flags=[],
     )
     parser.add_arguments(MykeArgs)
 
     args = sys.argv[1:]
 
-    if not args:
-        parser.print_help()
-        parser.exit()
-
     myke_args: MykeArgs
     task_args: List[str]
     myke_args, task_args = parser.parse_known_args_to_model(
         args,
         args_model=MykeArgs,
         skip_pydantic_validation=True,
     )
@@ -181,11 +177,11 @@
             if not fnmatch(k, task_args[0]):
                 del TASKS[k]
 
     yapx.run(
         root_task,
         named_subcommands=TASKS,
         args=task_args,
-        default_args=["--help"],
+        default_args=["--tui"],
         prog=prog,
         prog_version=__version__,
     )
```

### Comparing `myke-0.2.0/src/myke/run.py` & `myke-0.3.0/src/myke/run.py`

 * *Files identical despite different names*

### Comparing `myke-0.2.0/src/myke/tasks.py` & `myke-0.3.0/src/myke/tasks.py`

 * *Files identical despite different names*

### Comparing `myke-0.2.0/src/myke/utils.py` & `myke-0.3.0/src/myke/utils.py`

 * *Files identical despite different names*

### Comparing `myke-0.2.0/src/myke.egg-info/PKG-INFO` & `myke-0.3.0/src/myke.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: myke
-Version: 0.2.0
-Summary: The dynamic Python CLI for task execution.
+Version: 0.3.0
+Summary: The dynamic Python CLI for convenient task execution.
 Author-email: Donald Mellenbruch <hello@f2dv.com>
 License: GNU GENERAL PUBLIC LICENSE
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
         Everyone is permitted to copy and distribute verbatim copies
         of this license document, but changing it is not allowed.
@@ -674,112 +674,21 @@
         The GNU General Public License does not permit incorporating your program
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
-Project-URL: Homepage, https://www.f2dv.com/code/r/myke/i
+Project-URL: Homepage, https://www.f2dv.com/r/myke
 Project-URL: Repository, https://www.github.com/fresh2dev/myke
-Project-URL: Funding, https://www.f2dv.com/funding
+Project-URL: Funding, https://www.f2dv.com/fund
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: io
 Provides-Extra: extras
 License-File: LICENSE
 
-# myke
-
-> The dynamic Python CLI for task execution.
-
-| Links         |                                              |
-|---------------|----------------------------------------------|
-| Code Repo     | https://www.github.com/fresh2dev/myke        |
-| Mirror Repo   | https://www.f2dv.com/code/r/myke             |
-| Documentation | https://www.f2dv.com/code/r/myke/i           |
-| Changelog     | https://www.f2dv.com/code/r/myke/i/changelog |
-| License       | https://www.f2dv.com/code/r/myke/i/license   |
-| Funding       | https://www.f2dv.com/funding                 |
-
-[![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/fresh2dev/myke?color=blue&style=for-the-badge)](https://www.github.com/fresh2dev/myke/releases)
-[![GitHub Release Date](https://img.shields.io/github/release-date/fresh2dev/myke?color=blue&style=for-the-badge)](https://www.github.com/fresh2dev/myke/releases)
-[![License](https://img.shields.io/github/license/fresh2dev/myke?color=blue&style=for-the-badge)](https://www.f2dv.com/code/r/myke/i/license)
-[![GitHub issues](https://img.shields.io/github/issues-raw/fresh2dev/myke?color=blue&style=for-the-badge)](https://www.github.com/fresh2dev/myke/issues)
-[![GitHub pull requests](https://img.shields.io/github/issues-pr-raw/fresh2dev/myke?color=blue&style=for-the-badge)](https://www.github.com/fresh2dev/myke/pulls)
-[![GitHub Repo stars](https://img.shields.io/github/stars/fresh2dev/myke?color=blue&style=for-the-badge)](https://star-history.com/#fresh2dev/myke&Date)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/myke?color=blue&style=for-the-badge)](https://pypi.org/project/myke)
-[![Docker Pulls](https://img.shields.io/docker/pulls/fresh2dev/myke?color=blue&style=for-the-badge)](https://hub.docker.com/r/fresh2dev/myke)
-[![Docs Website](https://img.shields.io/website?down_message=unavailable&label=docs&style=for-the-badge&up_color=blue&up_message=available&url=https://www.f2dv.com/code/r/myke/i)](https://www.f2dv.com/code/r/myke/i)
-[![Coverage Website](https://img.shields.io/website?down_message=unavailable&label=coverage&style=for-the-badge&up_color=blue&up_message=available&url=https://www.f2dv.com/code/r/myke/i/tests/coverage)](https://www.f2dv.com/code/r/myke/i/tests/coverage)
-[![Funding](https://img.shields.io/badge/funding-%24%24%24-blue?style=for-the-badge)](https://www.f2dv.com/fund)
-
-## Overview
-
-Meet `myke`, the dynamic Python CLI for task exection.
-
-I built `myke` to replace my personal need for `make` and Makefiles. myke has probably 1% of the functionality of make, and that's a good thing.
-
-> Note: `myke` is in *beta* status. Please report ideas and issues [here](https://github.com/fresh2dev/myke/issues).
-
-## Install
-
-myke is a CLI application, so I recommend installing it using [pipx](https://github.com/pypa/pipx).
-
-```sh
-pipx install 'myke[extras]'
-```
-
-What's in `myke[extras]`?
-
-- `myke[io]` --> Libraries to read/write various file formats (yaml, toml, etc.)
-- `myke[pydantic]` --> Includes the [Pydantic](https://github.com/pydantic/pydantic) library to support additional types.
-- `myke[tui]` --> Includes the [Trogon](https://github.com/Textualize/trogon) library to present a TUI for myke.
-
-## Use
-
-Paste the following into a file named `Mykefile`:
-
-```python title="Mykefile"
-from myke import task
-
-@task
-def say_hello(name):
-    print(f"Hello {name}.")
-
-@task
-def say_goodbye(name):
-    print(f"Goodbye {name}.")
-```
-
-Invoke a task:
-
-```sh
-myke say-hello --name world
-```
-
-View available tasks:
-
-```sh
-myke
-```
-
-### Read More
-
-myke is an instantiation of the `yapx` project, the CLI builder for Python. The information contained in the [yapx docs](https://www.f2dv.com/code/r/yapx/i/) also applies to myke.
-
-Read more about myke @ https://www.f2dv.com/code/r/myke/i
-
-Read more about yapx @ https://www.f2dv.com/code/r/yapx/i
-
-## Support
-
-If this project delivers value to you, please [provide feedback](https://www.github.com/fresh2dev/myke/issues), code contributions, and/or [funding](https://www.f2dv.com/fund).
-
-See all of my projects @ https://www.f2dv.com/code/r
-
-*Brought to you by...*
-
-<a href="https://www.f2dv.com"><img src="https://img.fresh2.dev/fresh2dev.svg" style="filter: invert(50%);"></img></a>
+[https://www.f2dv.com/r/myke](https://www.f2dv.com/r/myke)
```

### Comparing `myke-0.2.0/src/myke.egg-info/SOURCES.txt` & `myke-0.3.0/src/myke.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+README.pypi.md
 pyproject.toml
 src/myke/__init__.py
 src/myke/__main__.py
 src/myke/__version__.py
 src/myke/exceptions.py
 src/myke/globals.py
 src/myke/main.py
```

### Comparing `myke-0.2.0/src/myke.egg-info/requires.txt` & `myke-0.3.0/src/myke.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-yapx[extras]==0.2.*
+yapx[extras]<1,>=0.2.4
 pip>=22.2
 
 [:python_version < "3.10"]
 typing-extensions
 
 [dev]
 python-lsp-server[rope]==1.*
@@ -26,24 +26,26 @@
 mkdocs-autorefs==0.*
 mkdocs-include-dir-to-nav==1.*
 
 [extras]
 requests==2.*
 pyyaml
 python-dotenv
-tabulate
+tabulate<1
+ppqueue==0.4.*
 
 [extras:python_version < "3.11"]
 tomli
 
 [io]
 requests==2.*
 pyyaml
 python-dotenv
-tabulate
+tabulate<1
+ppqueue==0.4.*
 
 [io:python_version < "3.11"]
 tomli
 
 [tests]
 pytest==7.*
 pytest-cov==4.*
@@ -53,11 +55,12 @@
 pylint==2.*
 pylint-pytest==1.*
 packaging==23.*
 mockish==0.1.*
 requests==2.*
 pyyaml
 python-dotenv
-tabulate
+tabulate<1
+ppqueue==0.4.*
 
 [tests:python_version < "3.11"]
 tomli
```

### Comparing `myke-0.2.0/tests/test_Mykefile.py` & `myke-0.3.0/tests/test_Mykefile.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import subprocess
 from typing import List, Union
 from unittest import mock
 from uuid import uuid4
 
 import pytest
 
-from myke import sh_stdout
+from myke import run, sh_stdout
 
 
 def _common(
     capsys,
     resources_dir: str,
     cli_args: List[str],
     expected_txt: Union[str, List[str]],
@@ -140,14 +140,15 @@
 
     _ = _common(capsys, resources_dir, cli_args=cli_args, expected_txt=None)
 
 
 def test_Mykefile_executable(capsys, resources_dir: str):
     # 1. ARRANGE
     mykefile: str = os.path.join(resources_dir, "Mykefile")
+    assert os.path.exists(mykefile)
 
     expected_txt: str = str(uuid4())
 
     # 2. ACT
     output: str = sh_stdout(
         f"""
     PYTHONPATH=./src python -m myke --myke-file {mykefile} hello --name {expected_txt}
@@ -159,7 +160,17 @@
     assert output
     assert expected_txt in output
 
     captured = capsys.readouterr()
     assert captured.out
     assert not captured.err
     assert expected_txt in captured.out
+
+
+def test_Mykefile_ppqueue(resources_dir: str):
+    mykefile: str = os.path.join(resources_dir, "Mykefile-ppqueue")
+    assert os.path.exists(mykefile)
+    _ = run(
+        f"""
+    PYTHONPATH=./src python -m myke --myke-file {mykefile} hello-again
+""",
+    )
```

### Comparing `myke-0.2.0/tests/test_io.py` & `myke-0.3.0/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `myke-0.2.0/tests/test_main.py` & `myke-0.3.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `myke-0.2.0/tests/test_run.py` & `myke-0.3.0/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `myke-0.2.0/tests/test_utils.py` & `myke-0.3.0/tests/test_utils.py`

 * *Files identical despite different names*

