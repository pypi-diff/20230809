# Comparing `tmp/chainedci-1.5.42.tar.gz` & `tmp/chainedci-1.5.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainedci-1.5.42.tar", last modified: Fri Aug  4 11:15:57 2023, max compression
+gzip compressed data, was "chainedci-1.5.43.tar", last modified: Tue Aug  8 06:16:07 2023, max compression
```

## Comparing `chainedci-1.5.42.tar` & `chainedci-1.5.43.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 11:15:57.010563 chainedci-1.5.42/
--rw-rw-rw-   0 root         (0) root         (0)      331 2023-08-04 11:15:39.000000 chainedci-1.5.42/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      923 2023-08-04 11:15:57.010563 chainedci-1.5.42/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-08-04 11:15:39.000000 chainedci-1.5.42/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 11:15:57.006563 chainedci-1.5.42/chainedci/
--rw-rw-rw-   0 root         (0) root         (0)      285 2023-08-04 11:15:39.000000 chainedci-1.5.42/chainedci/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11472 2023-08-04 11:15:39.000000 chainedci-1.5.42/chainedci/artifact.py
--rw-rw-rw-   0 root         (0) root         (0)     9356 2023-08-04 11:15:39.000000 chainedci-1.5.42/chainedci/artifact_src.py
--rwxrwxrwx   0 root         (0) root         (0)      131 2023-08-04 11:15:39.000000 chainedci-1.5.42/chainedci/chainedci
--rw-rw-rw-   0 root         (0) root         (0)     6338 2023-08-04 11:15:39.000000 chainedci-1.5.42/chainedci/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     6819 2023-08-04 11:15:39.000000 chainedci-1.5.42/chainedci/config.py
--rw-rw-rw-   0 root         (0) root         (0)     3663 2023-08-04 11:15:39.000000 chainedci-1.5.42/chainedci/default_chainedci.yml
--rw-rw-rw-   0 root         (0) root         (0)     3926 2023-08-04 11:15:39.000000 chainedci-1.5.42/chainedci/env_vars.py
--rw-rw-rw-   0 root         (0) root         (0)     2924 2023-08-04 11:15:39.000000 chainedci-1.5.42/chainedci/http_adapter.py
--rw-rw-rw-   0 root         (0) root         (0)     3932 2023-08-04 11:15:39.000000 chainedci-1.5.42/chainedci/init_project.py
--rw-rw-rw-   0 root         (0) root         (0)     4174 2023-08-04 11:15:39.000000 chainedci-1.5.42/chainedci/inventory.py
--rw-rw-rw-   0 root         (0) root         (0)     4850 2023-08-04 11:15:39.000000 chainedci-1.5.42/chainedci/log.py
--rw-rw-rw-   0 root         (0) root         (0)     5935 2023-08-04 11:15:39.000000 chainedci-1.5.42/chainedci/options.py
--rw-rw-rw-   0 root         (0) root         (0)     3888 2023-08-04 11:15:39.000000 chainedci-1.5.42/chainedci/parser.py
--rw-rw-rw-   0 root         (0) root         (0)    10532 2023-08-04 11:15:39.000000 chainedci-1.5.42/chainedci/pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)     4890 2023-08-04 11:15:39.000000 chainedci-1.5.42/chainedci/scenario.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 11:15:57.009563 chainedci-1.5.42/chainedci/static/
--rw-rw-rw-   0 root         (0) root         (0)        8 2023-08-04 11:15:39.000000 chainedci-1.5.42/chainedci/static/inventory
--rw-rw-rw-   0 root         (0) root         (0)      390 2023-08-04 11:15:39.000000 chainedci-1.5.42/chainedci/static/projectA.yml
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-08-04 11:15:39.000000 chainedci-1.5.42/chainedci/static/projectA_config1.yml
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-08-04 11:15:39.000000 chainedci-1.5.42/chainedci/static/projectA_config2.yml
--rw-rw-rw-   0 root         (0) root         (0)    15020 2023-08-04 11:15:39.000000 chainedci-1.5.42/chainedci/step.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 11:15:57.009563 chainedci-1.5.42/chainedci/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1165 2023-08-04 11:15:39.000000 chainedci-1.5.42/chainedci/templates/all.yml.tpl
--rw-rw-rw-   0 root         (0) root         (0)     3974 2023-08-04 11:15:39.000000 chainedci-1.5.42/chainedci/templates/main.yml.tpl
--rw-rw-rw-   0 root         (0) root         (0)     2532 2023-08-04 11:15:39.000000 chainedci-1.5.42/chainedci/templates/scenario.yml.tpl
--rw-rw-rw-   0 root         (0) root         (0)     2782 2023-08-04 11:15:39.000000 chainedci-1.5.42/chainedci/tools.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-08-04 11:15:39.000000 chainedci-1.5.42/chainedci/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 11:15:57.008563 chainedci-1.5.42/chainedci.egg-info/
--rw-r--r--   0 root         (0) root         (0)      923 2023-08-04 11:15:56.000000 chainedci-1.5.42/chainedci.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      924 2023-08-04 11:15:56.000000 chainedci-1.5.42/chainedci.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 11:15:56.000000 chainedci-1.5.42/chainedci.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 11:15:56.000000 chainedci-1.5.42/chainedci.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       99 2023-08-04 11:15:56.000000 chainedci-1.5.42/chainedci.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-08-04 11:15:56.000000 chainedci-1.5.42/chainedci.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      240 2023-08-04 11:15:57.011563 chainedci-1.5.42/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1241 2023-08-04 11:15:39.000000 chainedci-1.5.42/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 11:15:57.010563 chainedci-1.5.42/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-04 11:15:39.000000 chainedci-1.5.42/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1318 2023-08-04 11:15:39.000000 chainedci-1.5.42/tests/tests_lib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 06:16:07.617296 chainedci-1.5.43/
+-rw-rw-rw-   0 root         (0) root         (0)      331 2023-08-08 06:15:50.000000 chainedci-1.5.43/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      923 2023-08-08 06:16:07.618296 chainedci-1.5.43/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-08-08 06:15:50.000000 chainedci-1.5.43/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 06:16:07.614296 chainedci-1.5.43/chainedci/
+-rw-rw-rw-   0 root         (0) root         (0)      285 2023-08-08 06:15:50.000000 chainedci-1.5.43/chainedci/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11472 2023-08-08 06:15:50.000000 chainedci-1.5.43/chainedci/artifact.py
+-rw-rw-rw-   0 root         (0) root         (0)     9356 2023-08-08 06:15:50.000000 chainedci-1.5.43/chainedci/artifact_src.py
+-rwxrwxrwx   0 root         (0) root         (0)      131 2023-08-08 06:15:50.000000 chainedci-1.5.43/chainedci/chainedci
+-rw-rw-rw-   0 root         (0) root         (0)     6338 2023-08-08 06:15:50.000000 chainedci-1.5.43/chainedci/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     6819 2023-08-08 06:15:50.000000 chainedci-1.5.43/chainedci/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3663 2023-08-08 06:15:50.000000 chainedci-1.5.43/chainedci/default_chainedci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     3926 2023-08-08 06:15:50.000000 chainedci-1.5.43/chainedci/env_vars.py
+-rw-rw-rw-   0 root         (0) root         (0)     2924 2023-08-08 06:15:50.000000 chainedci-1.5.43/chainedci/http_adapter.py
+-rw-rw-rw-   0 root         (0) root         (0)     3932 2023-08-08 06:15:50.000000 chainedci-1.5.43/chainedci/init_project.py
+-rw-rw-rw-   0 root         (0) root         (0)     4174 2023-08-08 06:15:50.000000 chainedci-1.5.43/chainedci/inventory.py
+-rw-rw-rw-   0 root         (0) root         (0)     4850 2023-08-08 06:15:50.000000 chainedci-1.5.43/chainedci/log.py
+-rw-rw-rw-   0 root         (0) root         (0)     5935 2023-08-08 06:15:50.000000 chainedci-1.5.43/chainedci/options.py
+-rw-rw-rw-   0 root         (0) root         (0)     3888 2023-08-08 06:15:50.000000 chainedci-1.5.43/chainedci/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)    10532 2023-08-08 06:15:50.000000 chainedci-1.5.43/chainedci/pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     4890 2023-08-08 06:15:50.000000 chainedci-1.5.43/chainedci/scenario.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 06:16:07.616296 chainedci-1.5.43/chainedci/static/
+-rw-rw-rw-   0 root         (0) root         (0)        8 2023-08-08 06:15:50.000000 chainedci-1.5.43/chainedci/static/inventory
+-rw-rw-rw-   0 root         (0) root         (0)      390 2023-08-08 06:15:50.000000 chainedci-1.5.43/chainedci/static/projectA.yml
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-08-08 06:15:50.000000 chainedci-1.5.43/chainedci/static/projectA_config1.yml
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-08-08 06:15:50.000000 chainedci-1.5.43/chainedci/static/projectA_config2.yml
+-rw-rw-rw-   0 root         (0) root         (0)    15020 2023-08-08 06:15:50.000000 chainedci-1.5.43/chainedci/step.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 06:16:07.617296 chainedci-1.5.43/chainedci/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1165 2023-08-08 06:15:50.000000 chainedci-1.5.43/chainedci/templates/all.yml.tpl
+-rw-rw-rw-   0 root         (0) root         (0)     3974 2023-08-08 06:15:50.000000 chainedci-1.5.43/chainedci/templates/main.yml.tpl
+-rw-rw-rw-   0 root         (0) root         (0)     2532 2023-08-08 06:15:50.000000 chainedci-1.5.43/chainedci/templates/scenario.yml.tpl
+-rw-rw-rw-   0 root         (0) root         (0)     2782 2023-08-08 06:15:50.000000 chainedci-1.5.43/chainedci/tools.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-08-08 06:15:50.000000 chainedci-1.5.43/chainedci/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 06:16:07.616296 chainedci-1.5.43/chainedci.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      923 2023-08-08 06:16:07.000000 chainedci-1.5.43/chainedci.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      924 2023-08-08 06:16:07.000000 chainedci-1.5.43/chainedci.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 06:16:07.000000 chainedci-1.5.43/chainedci.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 06:16:07.000000 chainedci-1.5.43/chainedci.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       99 2023-08-08 06:16:07.000000 chainedci-1.5.43/chainedci.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-08-08 06:16:07.000000 chainedci-1.5.43/chainedci.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      240 2023-08-08 06:16:07.618296 chainedci-1.5.43/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1241 2023-08-08 06:15:50.000000 chainedci-1.5.43/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 06:16:07.617296 chainedci-1.5.43/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 06:15:50.000000 chainedci-1.5.43/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1318 2023-08-08 06:15:50.000000 chainedci-1.5.43/tests/tests_lib.py
```

### Comparing `chainedci-1.5.42/PKG-INFO` & `chainedci-1.5.43/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainedci
-Version: 1.5.42
+Version: 1.5.43
 Summary: Chaine Gitlab CI pipelines
 Home-page: https://gitlab.com/Orange-OpenSource/lfn/ci_cd/chained-ci
 Author: Orange OpenSource
 License: Apache 2.0
 Description-Content-Type: text/markdown
 
 # Chained-ci-py
```

### Comparing `chainedci-1.5.42/README.md` & `chainedci-1.5.43/README.md`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.42/chainedci/artifact.py` & `chainedci-1.5.43/chainedci/artifact.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.42/chainedci/artifact_src.py` & `chainedci-1.5.43/chainedci/artifact_src.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.42/chainedci/cli.py` & `chainedci-1.5.43/chainedci/cli.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.42/chainedci/config.py` & `chainedci-1.5.43/chainedci/config.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.42/chainedci/default_chainedci.yml` & `chainedci-1.5.43/chainedci/default_chainedci.yml`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.42/chainedci/env_vars.py` & `chainedci-1.5.43/chainedci/env_vars.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.42/chainedci/http_adapter.py` & `chainedci-1.5.43/chainedci/http_adapter.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.42/chainedci/init_project.py` & `chainedci-1.5.43/chainedci/init_project.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.42/chainedci/inventory.py` & `chainedci-1.5.43/chainedci/inventory.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.42/chainedci/log.py` & `chainedci-1.5.43/chainedci/log.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.42/chainedci/options.py` & `chainedci-1.5.43/chainedci/options.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.42/chainedci/parser.py` & `chainedci-1.5.43/chainedci/parser.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.42/chainedci/pipeline.py` & `chainedci-1.5.43/chainedci/pipeline.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.42/chainedci/scenario.py` & `chainedci-1.5.43/chainedci/scenario.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.42/chainedci/step.py` & `chainedci-1.5.43/chainedci/step.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.42/chainedci/templates/all.yml.tpl` & `chainedci-1.5.43/chainedci/templates/all.yml.tpl`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.42/chainedci/templates/main.yml.tpl` & `chainedci-1.5.43/chainedci/templates/main.yml.tpl`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.42/chainedci/templates/scenario.yml.tpl` & `chainedci-1.5.43/chainedci/templates/scenario.yml.tpl`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.42/chainedci/tools.py` & `chainedci-1.5.43/chainedci/tools.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.42/chainedci/version.py` & `chainedci-1.5.43/chainedci/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 """Version module."""
 
-__version__ = "1.5.42"
+__version__ = "1.5.43"
```

### Comparing `chainedci-1.5.42/chainedci.egg-info/PKG-INFO` & `chainedci-1.5.43/chainedci.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainedci
-Version: 1.5.42
+Version: 1.5.43
 Summary: Chaine Gitlab CI pipelines
 Home-page: https://gitlab.com/Orange-OpenSource/lfn/ci_cd/chained-ci
 Author: Orange OpenSource
 License: Apache 2.0
 Description-Content-Type: text/markdown
 
 # Chained-ci-py
```

### Comparing `chainedci-1.5.42/chainedci.egg-info/SOURCES.txt` & `chainedci-1.5.43/chainedci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.42/setup.py` & `chainedci-1.5.43/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 def readme():
     """Set Readme from file."""
     with open('README.md', encoding="utf-8") as f:
         return f.read()
 
 
 setup(name='chainedci',
-      version='1.5.42',
+      version='1.5.43',
       description='Chaine Gitlab CI pipelines',
       long_description=readme(),
       long_description_content_type='text/markdown',
       url='https://gitlab.com/Orange-OpenSource/lfn/ci_cd/chained-ci',
       author='Orange OpenSource',
       license='Apache 2.0',
       packages=find_packages(),
```

### Comparing `chainedci-1.5.42/tests/tests_lib.py` & `chainedci-1.5.43/tests/tests_lib.py`

 * *Files identical despite different names*

