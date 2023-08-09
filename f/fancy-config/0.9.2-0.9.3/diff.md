# Comparing `tmp/fancy-config-0.9.2.tar.gz` & `tmp/fancy-config-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fancy-config-0.9.2.tar", last modified: Thu Dec  9 04:09:39 2021, max compression
+gzip compressed data, was "dist/fancy-config-0.9.3.tar", last modified: Thu Dec  9 04:29:02 2021, max compression
```

## Comparing `fancy-config-0.9.2.tar` & `fancy-config-0.9.3.tar`

### file list

```diff
@@ -1,48 +1,46 @@
-drwxrwxr-x   0 ansible   (1000) ansible   (1000)        0 2021-12-09 04:09:39.000000 fancy-config-0.9.2/
--rw-rw-r--   0 ansible   (1000) ansible   (1000)      479 2021-12-09 04:09:39.000000 fancy-config-0.9.2/PKG-INFO
--rw-rw-r--   0 ansible   (1000) ansible   (1000)      103 2021-10-13 22:46:52.000000 fancy-config-0.9.2/README.md
-drwxrwxr-x   0 ansible   (1000) ansible   (1000)        0 2021-12-09 04:09:39.000000 fancy-config-0.9.2/fancy/
-drwxrwxr-x   0 ansible   (1000) ansible   (1000)        0 2021-12-09 04:09:39.000000 fancy-config-0.9.2/fancy/config/
--rw-rw-r--   0 ansible   (1000) ansible   (1000)     1045 2021-10-13 22:46:52.000000 fancy-config-0.9.2/fancy/config/LICENSE.txt
--rw-rw-r--   0 ansible   (1000) ansible   (1000)       15 2021-10-13 22:46:52.000000 fancy-config-0.9.2/fancy/config/README.md
--rw-rw-r--   0 ansible   (1000) ansible   (1000)      705 2021-10-13 22:46:52.000000 fancy-config-0.9.2/fancy/config/__init__.py
--rw-rw-r--   0 ansible   (1000) ansible   (1000)      954 2021-10-13 22:46:52.000000 fancy-config-0.9.2/fancy/config/attribute_setters.py
--rw-rw-r--   0 ansible   (1000) ansible   (1000)     2980 2021-10-13 22:50:54.000000 fancy-config-0.9.2/fancy/config/base_config.py
--rw-rw-r--   0 ansible   (1000) ansible   (1000)      224 2021-10-13 22:46:52.000000 fancy-config-0.9.2/fancy/config/config_context.py
--rw-rw-r--   0 ansible   (1000) ansible   (1000)     1158 2021-10-13 22:46:52.000000 fancy-config-0.9.2/fancy/config/config_factory.py
--rw-rw-r--   0 ansible   (1000) ansible   (1000)      696 2021-10-13 22:46:52.000000 fancy-config-0.9.2/fancy/config/config_list_struct.py
--rw-rw-r--   0 ansible   (1000) ansible   (1000)     1101 2021-10-13 22:46:52.000000 fancy-config-0.9.2/fancy/config/config_loader_factory.py
--rw-rw-r--   0 ansible   (1000) ansible   (1000)     2970 2021-10-13 22:46:52.000000 fancy-config-0.9.2/fancy/config/config_loaders.py
--rw-rw-r--   0 ansible   (1000) ansible   (1000)      190 2021-10-13 22:46:52.000000 fancy-config-0.9.2/fancy/config/config_structure.py
-drwxrwxr-x   0 ansible   (1000) ansible   (1000)        0 2021-12-09 04:09:39.000000 fancy-config-0.9.2/fancy/config/converter/
--rw-rw-r--   0 ansible   (1000) ansible   (1000)       90 2021-10-13 22:46:52.000000 fancy-config-0.9.2/fancy/config/converter/__init__.py
--rw-rw-r--   0 ansible   (1000) ansible   (1000)      571 2021-10-13 22:46:52.000000 fancy-config-0.9.2/fancy/config/converter/base_option_converter.py
-drwxrwxr-x   0 ansible   (1000) ansible   (1000)        0 2021-12-09 04:09:39.000000 fancy-config-0.9.2/fancy/config/exceptions/
--rw-rw-r--   0 ansible   (1000) ansible   (1000)       96 2021-10-13 22:46:52.000000 fancy-config-0.9.2/fancy/config/exceptions/__init__.py
--rw-rw-r--   0 ansible   (1000) ansible   (1000)      132 2021-10-13 22:46:52.000000 fancy-config-0.9.2/fancy/config/exceptions/class_not_found.py
--rw-rw-r--   0 ansible   (1000) ansible   (1000)     2476 2021-10-13 22:46:52.000000 fancy-config-0.9.2/fancy/config/option.py
--rw-rw-r--   0 ansible   (1000) ansible   (1000)      970 2021-10-13 22:46:52.000000 fancy-config-0.9.2/fancy/config/option_preprocessing.py
-drwxrwxr-x   0 ansible   (1000) ansible   (1000)        0 2021-12-09 04:09:39.000000 fancy-config-0.9.2/fancy/config/process/
--rw-rw-r--   0 ansible   (1000) ansible   (1000)      234 2021-10-13 22:46:52.000000 fancy-config-0.9.2/fancy/config/process/__init__.py
--rw-rw-r--   0 ansible   (1000) ansible   (1000)      483 2021-10-13 22:46:52.000000 fancy-config-0.9.2/fancy/config/process/auto_process_typ.py
--rw-rw-r--   0 ansible   (1000) ansible   (1000)      932 2021-10-13 22:46:52.000000 fancy-config-0.9.2/fancy/config/process/boolean.py
--rw-rw-r--   0 ansible   (1000) ansible   (1000)      405 2021-10-13 22:46:52.000000 fancy-config-0.9.2/fancy/config/process/config.py
--rw-rw-r--   0 ansible   (1000) ansible   (1000)      309 2021-10-13 22:46:52.000000 fancy-config-0.9.2/fancy/config/process/config_list.py
--rw-rw-r--   0 ansible   (1000) ansible   (1000)      877 2021-12-09 04:05:04.000000 fancy-config-0.9.2/fancy/config/process/flag_container.py
--rw-rw-r--   0 ansible   (1000) ansible   (1000)      577 2021-10-13 22:46:52.000000 fancy-config-0.9.2/fancy/config/process/flag_string.py
-drwxrwxr-x   0 ansible   (1000) ansible   (1000)        0 2021-12-09 04:09:39.000000 fancy-config-0.9.2/fancy/config/utils/
--rw-rw-r--   0 ansible   (1000) ansible   (1000)       54 2021-10-13 22:46:52.000000 fancy-config-0.9.2/fancy/config/utils/__init__.py
--rw-rw-r--   0 ansible   (1000) ansible   (1000)      263 2021-10-13 22:46:52.000000 fancy-config-0.9.2/fancy/config/utils/reflections.py
-drwxrwxr-x   0 ansible   (1000) ansible   (1000)        0 2021-12-09 04:09:39.000000 fancy-config-0.9.2/fancy_config.egg-info/
--rw-rw-r--   0 ansible   (1000) ansible   (1000)      479 2021-12-09 04:09:39.000000 fancy-config-0.9.2/fancy_config.egg-info/PKG-INFO
--rw-rw-r--   0 ansible   (1000) ansible   (1000)     1128 2021-12-09 04:09:39.000000 fancy-config-0.9.2/fancy_config.egg-info/SOURCES.txt
--rw-rw-r--   0 ansible   (1000) ansible   (1000)        1 2021-12-09 04:09:39.000000 fancy-config-0.9.2/fancy_config.egg-info/dependency_links.txt
--rw-rw-r--   0 ansible   (1000) ansible   (1000)       12 2021-12-09 04:09:39.000000 fancy-config-0.9.2/fancy_config.egg-info/requires.txt
--rw-rw-r--   0 ansible   (1000) ansible   (1000)       12 2021-12-09 04:09:39.000000 fancy-config-0.9.2/fancy_config.egg-info/top_level.txt
--rw-rw-r--   0 ansible   (1000) ansible   (1000)       38 2021-12-09 04:09:39.000000 fancy-config-0.9.2/setup.cfg
--rw-rw-r--   0 ansible   (1000) ansible   (1000)     1182 2021-12-09 04:08:26.000000 fancy-config-0.9.2/setup.py
-drwxrwxr-x   0 ansible   (1000) ansible   (1000)        0 2021-12-09 04:09:39.000000 fancy-config-0.9.2/tests/
--rw-rw-r--   0 ansible   (1000) ansible   (1000)        0 2021-10-13 22:46:52.000000 fancy-config-0.9.2/tests/__init__.py
--rw-rw-r--   0 ansible   (1000) ansible   (1000)     1009 2021-10-13 22:46:52.000000 fancy-config-0.9.2/tests/test_config.py
-drwxrwxr-x   0 ansible   (1000) ansible   (1000)        0 2021-12-09 04:09:39.000000 fancy-config-0.9.2/tests/unit/
--rw-rw-r--   0 ansible   (1000) ansible   (1000)        0 2021-10-13 22:46:52.000000 fancy-config-0.9.2/tests/unit/__init__.py
+drwxrwxr-x   0 ansible   (1000) ansible   (1000)        0 2021-12-09 04:29:02.000000 fancy-config-0.9.3/
+-rw-rw-r--   0 ansible   (1000) ansible   (1000)      479 2021-12-09 04:29:02.000000 fancy-config-0.9.3/PKG-INFO
+-rw-rw-r--   0 ansible   (1000) ansible   (1000)      103 2021-10-13 22:46:52.000000 fancy-config-0.9.3/README.md
+drwxrwxr-x   0 ansible   (1000) ansible   (1000)        0 2021-12-09 04:29:02.000000 fancy-config-0.9.3/fancy/
+drwxrwxr-x   0 ansible   (1000) ansible   (1000)        0 2021-12-09 04:29:02.000000 fancy-config-0.9.3/fancy/config/
+-rw-rw-r--   0 ansible   (1000) ansible   (1000)     1045 2021-10-13 22:46:52.000000 fancy-config-0.9.3/fancy/config/LICENSE.txt
+-rw-rw-r--   0 ansible   (1000) ansible   (1000)       15 2021-10-13 22:46:52.000000 fancy-config-0.9.3/fancy/config/README.md
+-rw-rw-r--   0 ansible   (1000) ansible   (1000)      705 2021-10-13 22:46:52.000000 fancy-config-0.9.3/fancy/config/__init__.py
+-rw-rw-r--   0 ansible   (1000) ansible   (1000)      954 2021-10-13 22:46:52.000000 fancy-config-0.9.3/fancy/config/attribute_setters.py
+-rw-rw-r--   0 ansible   (1000) ansible   (1000)     3153 2021-12-09 04:26:49.000000 fancy-config-0.9.3/fancy/config/base_config.py
+-rw-rw-r--   0 ansible   (1000) ansible   (1000)      314 2021-12-09 04:26:49.000000 fancy-config-0.9.3/fancy/config/config_context.py
+-rw-rw-r--   0 ansible   (1000) ansible   (1000)     1151 2021-12-09 04:26:49.000000 fancy-config-0.9.3/fancy/config/config_factory.py
+-rw-rw-r--   0 ansible   (1000) ansible   (1000)      696 2021-10-13 22:46:52.000000 fancy-config-0.9.3/fancy/config/config_list_struct.py
+-rw-rw-r--   0 ansible   (1000) ansible   (1000)     1087 2021-12-09 04:26:49.000000 fancy-config-0.9.3/fancy/config/config_loader_factory.py
+-rw-rw-r--   0 ansible   (1000) ansible   (1000)     2970 2021-10-13 22:46:52.000000 fancy-config-0.9.3/fancy/config/config_loaders.py
+-rw-rw-r--   0 ansible   (1000) ansible   (1000)      190 2021-10-13 22:46:52.000000 fancy-config-0.9.3/fancy/config/config_structure.py
+drwxrwxr-x   0 ansible   (1000) ansible   (1000)        0 2021-12-09 04:29:02.000000 fancy-config-0.9.3/fancy/config/converter/
+-rw-rw-r--   0 ansible   (1000) ansible   (1000)       90 2021-10-13 22:46:52.000000 fancy-config-0.9.3/fancy/config/converter/__init__.py
+-rw-rw-r--   0 ansible   (1000) ansible   (1000)      571 2021-10-13 22:46:52.000000 fancy-config-0.9.3/fancy/config/converter/base_option_converter.py
+-rw-rw-r--   0 ansible   (1000) ansible   (1000)      200 2021-12-09 04:26:49.000000 fancy-config-0.9.3/fancy/config/exc.py
+-rw-rw-r--   0 ansible   (1000) ansible   (1000)     2476 2021-10-13 22:46:52.000000 fancy-config-0.9.3/fancy/config/option.py
+-rw-rw-r--   0 ansible   (1000) ansible   (1000)      970 2021-10-13 22:46:52.000000 fancy-config-0.9.3/fancy/config/option_preprocessing.py
+drwxrwxr-x   0 ansible   (1000) ansible   (1000)        0 2021-12-09 04:29:02.000000 fancy-config-0.9.3/fancy/config/process/
+-rw-rw-r--   0 ansible   (1000) ansible   (1000)      234 2021-10-13 22:46:52.000000 fancy-config-0.9.3/fancy/config/process/__init__.py
+-rw-rw-r--   0 ansible   (1000) ansible   (1000)      483 2021-10-13 22:46:52.000000 fancy-config-0.9.3/fancy/config/process/auto_process_typ.py
+-rw-rw-r--   0 ansible   (1000) ansible   (1000)      932 2021-10-13 22:46:52.000000 fancy-config-0.9.3/fancy/config/process/boolean.py
+-rw-rw-r--   0 ansible   (1000) ansible   (1000)      405 2021-10-13 22:46:52.000000 fancy-config-0.9.3/fancy/config/process/config.py
+-rw-rw-r--   0 ansible   (1000) ansible   (1000)      309 2021-10-13 22:46:52.000000 fancy-config-0.9.3/fancy/config/process/config_list.py
+-rw-rw-r--   0 ansible   (1000) ansible   (1000)      877 2021-12-09 04:05:04.000000 fancy-config-0.9.3/fancy/config/process/flag_container.py
+-rw-rw-r--   0 ansible   (1000) ansible   (1000)      577 2021-10-13 22:46:52.000000 fancy-config-0.9.3/fancy/config/process/flag_string.py
+drwxrwxr-x   0 ansible   (1000) ansible   (1000)        0 2021-12-09 04:29:02.000000 fancy-config-0.9.3/fancy/config/utils/
+-rw-rw-r--   0 ansible   (1000) ansible   (1000)       54 2021-10-13 22:46:52.000000 fancy-config-0.9.3/fancy/config/utils/__init__.py
+-rw-rw-r--   0 ansible   (1000) ansible   (1000)      263 2021-10-13 22:46:52.000000 fancy-config-0.9.3/fancy/config/utils/reflections.py
+drwxrwxr-x   0 ansible   (1000) ansible   (1000)        0 2021-12-09 04:29:02.000000 fancy-config-0.9.3/fancy_config.egg-info/
+-rw-rw-r--   0 ansible   (1000) ansible   (1000)      479 2021-12-09 04:29:02.000000 fancy-config-0.9.3/fancy_config.egg-info/PKG-INFO
+-rw-rw-r--   0 ansible   (1000) ansible   (1000)     1069 2021-12-09 04:29:02.000000 fancy-config-0.9.3/fancy_config.egg-info/SOURCES.txt
+-rw-rw-r--   0 ansible   (1000) ansible   (1000)        1 2021-12-09 04:29:02.000000 fancy-config-0.9.3/fancy_config.egg-info/dependency_links.txt
+-rw-rw-r--   0 ansible   (1000) ansible   (1000)       12 2021-12-09 04:29:02.000000 fancy-config-0.9.3/fancy_config.egg-info/requires.txt
+-rw-rw-r--   0 ansible   (1000) ansible   (1000)       12 2021-12-09 04:29:02.000000 fancy-config-0.9.3/fancy_config.egg-info/top_level.txt
+-rw-rw-r--   0 ansible   (1000) ansible   (1000)       38 2021-12-09 04:29:02.000000 fancy-config-0.9.3/setup.cfg
+-rw-rw-r--   0 ansible   (1000) ansible   (1000)     1182 2021-12-09 04:26:49.000000 fancy-config-0.9.3/setup.py
+drwxrwxr-x   0 ansible   (1000) ansible   (1000)        0 2021-12-09 04:29:02.000000 fancy-config-0.9.3/tests/
+-rw-rw-r--   0 ansible   (1000) ansible   (1000)        0 2021-10-13 22:46:52.000000 fancy-config-0.9.3/tests/__init__.py
+-rw-rw-r--   0 ansible   (1000) ansible   (1000)     1009 2021-10-13 22:46:52.000000 fancy-config-0.9.3/tests/test_config.py
+drwxrwxr-x   0 ansible   (1000) ansible   (1000)        0 2021-12-09 04:29:02.000000 fancy-config-0.9.3/tests/unit/
+-rw-rw-r--   0 ansible   (1000) ansible   (1000)        0 2021-10-13 22:46:52.000000 fancy-config-0.9.3/tests/unit/__init__.py
```

### Comparing `fancy-config-0.9.2/fancy/config/LICENSE.txt` & `fancy-config-0.9.3/fancy/config/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fancy-config-0.9.2/fancy/config/__init__.py` & `fancy-config-0.9.3/fancy/config/__init__.py`

 * *Files identical despite different names*

### Comparing `fancy-config-0.9.2/fancy/config/attribute_setters.py` & `fancy-config-0.9.3/fancy/config/attribute_setters.py`

 * *Files identical despite different names*

### Comparing `fancy-config-0.9.2/fancy/config/base_config.py` & `fancy-config-0.9.3/fancy/config/base_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import inspect
 from abc import ABC
 from typing import TYPE_CHECKING, Dict, List, Optional
 
-from . import ConfigStructure, ConfigContext
+from . import ConfigStructure, ConfigContext, exc
 from . import Option
 
 if TYPE_CHECKING:
     from ..config import BaseConfigLoader
 
 
 class BaseConfig(ConfigStructure, ConfigContext, ABC):  # TODO more accurate error msg
@@ -43,16 +43,22 @@
             raise TypeError(f'index must be str, not {type(key)}')
         if key not in self.get_name_mapping().keys():
             raise KeyError(f'not contains the config named {key}, value: {repr(value)}')
         key = self.get_name_mapping()[key]
         self.__setattr__(key, value)
 
     def get_loader(self) -> 'BaseConfigLoader':
+        if self._loader is None:
+            raise exc.ContextNotLoadedError(self)
         return self._loader
 
+    @property
+    def loaded(self) -> bool:
+        return self._loader is not None
+
     def post_load(self):
         pass
 
     @classmethod
     def get_all_options(cls) -> Dict[str, Option]:
         if "_all_options" not in vars(cls):
             cls._all_options = {name: option for name, option in inspect.getmembers(cls) if isinstance(option, Option)}
```

### Comparing `fancy-config-0.9.2/fancy/config/config_factory.py` & `fancy-config-0.9.3/fancy/config/config_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict, Type, TYPE_CHECKING
 
 from . import BaseConfig, utils
-from .exceptions import ClassNotFoundException
+from .exc import ClassNotFoundException
 
 
 if TYPE_CHECKING:
     from . import BaseConfigLoader
 
 
 class ConfigFactory:
```

### Comparing `fancy-config-0.9.2/fancy/config/config_list_struct.py` & `fancy-config-0.9.3/fancy/config/config_list_struct.py`

 * *Files identical despite different names*

### Comparing `fancy-config-0.9.2/fancy/config/config_loader_factory.py` & `fancy-config-0.9.3/fancy/config/config_loader_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from typing import Dict, Type
 
 from .. import config as cfg
-from fancy.config import exceptions, utils
+from fancy.config import utils, exc
 
 
 class ConfigLoaderFactory:
     suffix: str = "ConfigLoader"
     loaders = None
 
     @classmethod
     def create_loader(cls, method: str = 'yaml') -> cfg.BaseConfigLoader:
         loaders = cls.get_all_loaders()
         if method + cls.suffix in loaders:
             method += cls.suffix
         elif method.capitalize() + cls.suffix in loaders:
             method = method.capitalize() + cls.suffix
         elif method not in loaders:
-            raise exceptions.ClassNotFoundException(method)
+            raise exc.ClassNotFoundException(method)
         return loaders[method]()
 
     @classmethod
     def get_all_loaders(cls) -> Dict[str, Type[cfg.BaseConfigLoader]]:
         if cls.loaders is None:
             cls.loaders = {
                 loader.__name__: loader for loader in utils.reflections.find_subclasses(cfg.BaseConfigLoader)
```

### Comparing `fancy-config-0.9.2/fancy/config/config_loaders.py` & `fancy-config-0.9.3/fancy/config/config_loaders.py`

 * *Files identical despite different names*

### Comparing `fancy-config-0.9.2/fancy/config/converter/base_option_converter.py` & `fancy-config-0.9.3/fancy/config/converter/base_option_converter.py`

 * *Files identical despite different names*

### Comparing `fancy-config-0.9.2/fancy/config/option.py` & `fancy-config-0.9.3/fancy/config/option.py`

 * *Files identical despite different names*

### Comparing `fancy-config-0.9.2/fancy/config/option_preprocessing.py` & `fancy-config-0.9.3/fancy/config/option_preprocessing.py`

 * *Files identical despite different names*

### Comparing `fancy-config-0.9.2/fancy/config/process/boolean.py` & `fancy-config-0.9.3/fancy/config/process/boolean.py`

 * *Files identical despite different names*

### Comparing `fancy-config-0.9.2/fancy/config/process/flag_container.py` & `fancy-config-0.9.3/fancy/config/process/flag_container.py`

 * *Files identical despite different names*

### Comparing `fancy-config-0.9.2/fancy/config/process/flag_string.py` & `fancy-config-0.9.3/fancy/config/process/flag_string.py`

 * *Files identical despite different names*

### Comparing `fancy-config-0.9.2/fancy_config.egg-info/SOURCES.txt` & `fancy-config-0.9.3/fancy_config.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,19 @@
 fancy/config/base_config.py
 fancy/config/config_context.py
 fancy/config/config_factory.py
 fancy/config/config_list_struct.py
 fancy/config/config_loader_factory.py
 fancy/config/config_loaders.py
 fancy/config/config_structure.py
+fancy/config/exc.py
 fancy/config/option.py
 fancy/config/option_preprocessing.py
 fancy/config/converter/__init__.py
 fancy/config/converter/base_option_converter.py
-fancy/config/exceptions/__init__.py
-fancy/config/exceptions/class_not_found.py
 fancy/config/process/__init__.py
 fancy/config/process/auto_process_typ.py
 fancy/config/process/boolean.py
 fancy/config/process/config.py
 fancy/config/process/config_list.py
 fancy/config/process/flag_container.py
 fancy/config/process/flag_string.py
```

### Comparing `fancy-config-0.9.2/setup.py` & `fancy-config-0.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 with requirements_file.open() as fp:
     requirements = [r.strip() for r in fp.readlines()]
 
 
 setup(
     name="fancy-config",
-    version="0.9.2",
+    version="0.9.3",
     packages=find_namespace_packages(),
     package_data={
         # If any package contains *.txt or *.rst files, include them:
         "": ["*.md", "*.txt"],
     },
 
     # metadata to display on PyPI
```

### Comparing `fancy-config-0.9.2/tests/test_config.py` & `fancy-config-0.9.3/tests/test_config.py`

 * *Files identical despite different names*

