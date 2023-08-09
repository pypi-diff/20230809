# Comparing `tmp/robson_package-0.0.26.tar.gz` & `tmp/robson_package-0.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robson_package-0.0.26.tar", last modified: Wed Aug  9 00:45:33 2023, max compression
+gzip compressed data, was "robson_package-0.0.27.tar", last modified: Wed Aug  9 00:49:09 2023, max compression
```

## Comparing `robson_package-0.0.26.tar` & `robson_package-0.0.27.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-09 00:45:33.536118 robson_package-0.0.26/
--rw-rw-rw-   0        0        0     1088 2023-08-08 11:50:54.000000 robson_package-0.0.26/LICENSE
--rw-rw-rw-   0        0        0      315 2023-08-09 00:45:33.535123 robson_package-0.0.26/PKG-INFO
--rw-rw-rw-   0        0        0       41 2023-08-08 11:50:54.000000 robson_package-0.0.26/README.md
-drwxrwxrwx   0        0        0        0 2023-08-09 00:45:33.525116 robson_package-0.0.26/robson_package/
--rw-rw-rw-   0        0        0       16 2023-08-09 00:44:58.000000 robson_package-0.0.26/robson_package/__init__.py
--rw-rw-rw-   0        0        0      515 2023-08-08 11:56:48.000000 robson_package-0.0.26/robson_package/conversor.py
-drwxrwxrwx   0        0        0        0 2023-08-09 00:45:33.533119 robson_package-0.0.26/robson_package.egg-info/
--rw-rw-rw-   0        0        0      315 2023-08-09 00:45:33.000000 robson_package-0.0.26/robson_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-08-09 00:45:33.000000 robson_package-0.0.26/robson_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-09 00:45:33.000000 robson_package-0.0.26/robson_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-08-09 00:45:33.000000 robson_package-0.0.26/robson_package.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-09 00:45:33.536118 robson_package-0.0.26/setup.cfg
--rw-rw-rw-   0        0        0      542 2023-08-09 00:44:25.000000 robson_package-0.0.26/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-09 00:49:09.752596 robson_package-0.0.27/
+-rw-rw-rw-   0        0        0     1088 2023-08-08 11:50:54.000000 robson_package-0.0.27/LICENSE
+-rw-rw-rw-   0        0        0      315 2023-08-09 00:49:09.750592 robson_package-0.0.27/PKG-INFO
+-rw-rw-rw-   0        0        0       41 2023-08-08 11:50:54.000000 robson_package-0.0.27/README.md
+drwxrwxrwx   0        0        0        0 2023-08-09 00:49:09.741592 robson_package-0.0.27/robson_package/
+-rw-rw-rw-   0        0        0       33 2023-08-09 00:48:57.000000 robson_package-0.0.27/robson_package/__init__.py
+-rw-rw-rw-   0        0        0      519 2023-08-09 00:48:42.000000 robson_package-0.0.27/robson_package/conversor.py
+drwxrwxrwx   0        0        0        0 2023-08-09 00:49:09.748595 robson_package-0.0.27/robson_package.egg-info/
+-rw-rw-rw-   0        0        0      315 2023-08-09 00:49:09.000000 robson_package-0.0.27/robson_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-08-09 00:49:09.000000 robson_package-0.0.27/robson_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-09 00:49:09.000000 robson_package-0.0.27/robson_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-08-09 00:49:09.000000 robson_package-0.0.27/robson_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-09 00:49:09.753600 robson_package-0.0.27/setup.cfg
+-rw-rw-rw-   0        0        0      542 2023-08-09 00:48:48.000000 robson_package-0.0.27/setup.py
```

### Comparing `robson_package-0.0.26/LICENSE` & `robson_package-0.0.27/LICENSE`

 * *Files identical despite different names*

### Comparing `robson_package-0.0.26/robson_package/conversor.py` & `robson_package-0.0.27/robson_package/conversor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-class Conversor:
+class Temperatura:
     def __init__(self, celsius):
         self.valor = celsius
 
     def converter_farenheit(self):
         return self.valor * 1.8 + 32
     
     def converter_kelvin(self):
         return self.valor + 273.15
     
 
 if __name__ == "__main__":
     celsius = float(input("Digite a temperatura em Celsius: "))
-    conversor = Conversor(celsius)
+    conversor = Temperatura(celsius)
     print(f"{celsius}°C equivale a {conversor.converter_farenheit()}°F")
     print(f"{celsius}°C equivale a {conversor.converter_kelvin()}K")
```

### Comparing `robson_package-0.0.26/setup.py` & `robson_package-0.0.27/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = '0.0.26'
+VERSION = '0.0.27'
 DESCRIPTION = 'Meu primeiro pacote em Python'
 LONG_DESCRIPTION = 'Meu primeiro pacote em Python com uma descrição um pouco mais longa'
 
 # Setting up
 setup(
     name="robson_package",
     version=VERSION,
```

