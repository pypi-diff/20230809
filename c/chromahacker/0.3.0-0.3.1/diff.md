# Comparing `tmp/chromahacker-0.3.0.tar.gz` & `tmp/chromahacker-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromahacker-0.3.0.tar", max compression
+gzip compressed data, was "chromahacker-0.3.1.tar", max compression
```

## Comparing `chromahacker-0.3.0.tar` & `chromahacker-0.3.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-06-06 19:05:27.000000 chromahacker-0.3.0/README.md
--rw-r--r--   0        0        0     6148 2023-07-21 18:41:22.475897 chromahacker-0.3.0/chromahacker/.DS_Store
--rw-r--r--   0        0        0       89 2023-06-08 16:47:40.000000 chromahacker-0.3.0/chromahacker/__init__.py
--rw-r--r--   0        0        0     6621 2023-06-09 00:51:51.000000 chromahacker-0.3.0/chromahacker/color_input.py
--rw-r--r--   0        0        0      669 2023-07-28 01:39:26.539405 chromahacker-0.3.0/chromahacker/palettize.py
--rw-r--r--   0        0        0      266 2023-06-09 00:21:03.000000 chromahacker-0.3.0/chromahacker/process_image.py
--rw-r--r--   0        0        0      469 2023-07-21 17:43:15.983637 chromahacker-0.3.0/chromahacker/spline.py
--rw-r--r--   0        0        0      337 2023-07-28 01:41:42.672092 chromahacker-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 chromahacker-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-06 19:05:27.000000 chromahacker-0.3.1/README.md
+-rw-r--r--   0        0        0     6148 2023-08-09 00:33:22.911225 chromahacker-0.3.1/chromahacker/.DS_Store
+-rw-r--r--   0        0        0       89 2023-06-08 16:47:40.000000 chromahacker-0.3.1/chromahacker/__init__.py
+-rw-r--r--   0        0        0     6627 2023-08-09 00:37:19.110581 chromahacker-0.3.1/chromahacker/color_input.py
+-rw-r--r--   0        0        0      701 2023-08-09 00:34:32.328680 chromahacker-0.3.1/chromahacker/palettize.py
+-rw-r--r--   0        0        0      266 2023-06-09 00:21:03.000000 chromahacker-0.3.1/chromahacker/process_image.py
+-rw-r--r--   0        0        0     1188 2023-08-07 01:52:09.983561 chromahacker-0.3.1/chromahacker/spline.py
+-rw-r--r--   0        0        0      384 2023-08-09 01:18:04.043147 chromahacker-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 chromahacker-0.3.1/PKG-INFO
```

### Comparing `chromahacker-0.3.0/chromahacker/color_input.py` & `chromahacker-0.3.1/chromahacker/color_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
             "white": (255, 255, 255),
             "whitesmoke": (245, 245, 245),
             "yellow": (255, 255, 0),
             "yellowgreen": (154, 205, 50),
         }
 
     if color_string in css_colors:
-        return np.array(css_colors[color_string], dtype=np.uint8)
+        return np.array(css_colors[color_string][::-1], dtype=np.uint8)
 
     if color_string.startswith("#") and len(color_string) == 7:
         try:
             red = int(color_string[1:3], 16)
             green = int(color_string[3:5], 16)
             blue = int(color_string[5:7], 16)
             return np.array([blue, green, red], dtype=np.uint8)
```

