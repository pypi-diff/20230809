# Comparing `tmp/PyQt6-Frameless-Window-0.3.0.tar.gz` & `tmp/PyQt6-Frameless-Window-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PyQt6-Frameless-Window-0.3.0.tar", last modified: Mon Aug  7 07:41:00 2023, max compression
+gzip compressed data, was "dist\PyQt6-Frameless-Window-0.3.1.tar", last modified: Wed Aug  9 01:44:34 2023, max compression
```

## Comparing `PyQt6-Frameless-Window-0.3.0.tar` & `PyQt6-Frameless-Window-0.3.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 07:41:00.137366 PyQt6-Frameless-Window-0.3.0/
--rw-rw-rw-   0        0        0    35823 2023-08-07 07:36:58.000000 PyQt6-Frameless-Window-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     5603 2023-08-07 07:41:00.136355 PyQt6-Frameless-Window-0.3.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-07 07:41:00.099927 PyQt6-Frameless-Window-0.3.0/PyQt6_Frameless_Window.egg-info/
--rw-rw-rw-   0        0        0     5603 2023-08-07 07:40:59.000000 PyQt6-Frameless-Window-0.3.0/PyQt6_Frameless_Window.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      848 2023-08-07 07:41:00.000000 PyQt6-Frameless-Window-0.3.0/PyQt6_Frameless_Window.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 07:40:59.000000 PyQt6-Frameless-Window-0.3.0/PyQt6_Frameless_Window.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-08-07 07:40:59.000000 PyQt6-Frameless-Window-0.3.0/PyQt6_Frameless_Window.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-08-07 07:40:59.000000 PyQt6-Frameless-Window-0.3.0/PyQt6_Frameless_Window.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5007 2023-08-07 07:36:58.000000 PyQt6-Frameless-Window-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-07 07:41:00.109857 PyQt6-Frameless-Window-0.3.0/qframelesswindow/
--rw-rw-rw-   0        0        0     1692 2023-08-07 07:38:21.000000 PyQt6-Frameless-Window-0.3.0/qframelesswindow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-07 07:41:00.113252 PyQt6-Frameless-Window-0.3.0/qframelesswindow/_rc/
--rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PyQt6-Frameless-Window-0.3.0/qframelesswindow/_rc/__init__.py
--rw-rw-rw-   0        0        0     2728 2023-08-07 07:36:58.000000 PyQt6-Frameless-Window-0.3.0/qframelesswindow/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2023-08-07 07:41:00.116649 PyQt6-Frameless-Window-0.3.0/qframelesswindow/linux/
--rw-rw-rw-   0        0        0     3110 2023-08-07 07:36:58.000000 PyQt6-Frameless-Window-0.3.0/qframelesswindow/linux/__init__.py
--rw-rw-rw-   0        0        0     3149 2023-08-07 07:36:58.000000 PyQt6-Frameless-Window-0.3.0/qframelesswindow/linux/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-08-07 07:41:00.120211 PyQt6-Frameless-Window-0.3.0/qframelesswindow/mac/
--rw-rw-rw-   0        0        0     3015 2023-08-07 07:36:58.000000 PyQt6-Frameless-Window-0.3.0/qframelesswindow/mac/__init__.py
--rw-rw-rw-   0        0        0     4563 2023-08-07 07:36:58.000000 PyQt6-Frameless-Window-0.3.0/qframelesswindow/mac/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-08-07 07:41:00.123614 PyQt6-Frameless-Window-0.3.0/qframelesswindow/titlebar/
--rw-rw-rw-   0        0        0     5235 2023-08-07 07:37:45.000000 PyQt6-Frameless-Window-0.3.0/qframelesswindow/titlebar/__init__.py
--rw-rw-rw-   0        0        0     9205 2023-08-07 07:36:58.000000 PyQt6-Frameless-Window-0.3.0/qframelesswindow/titlebar/title_bar_buttons.py
-drwxrwxrwx   0        0        0        0 2023-08-07 07:41:00.129851 PyQt6-Frameless-Window-0.3.0/qframelesswindow/utils/
--rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PyQt6-Frameless-Window-0.3.0/qframelesswindow/utils/__init__.py
--rw-rw-rw-   0        0        0      644 2023-08-07 07:36:58.000000 PyQt6-Frameless-Window-0.3.0/qframelesswindow/utils/linux_utils.py
--rw-rw-rw-   0        0        0     1850 2023-08-07 07:36:58.000000 PyQt6-Frameless-Window-0.3.0/qframelesswindow/utils/mac_utils.py
--rw-rw-rw-   0        0        0     8352 2023-08-07 07:36:58.000000 PyQt6-Frameless-Window-0.3.0/qframelesswindow/utils/win32_utils.py
-drwxrwxrwx   0        0        0        0 2023-08-07 07:41:00.135348 PyQt6-Frameless-Window-0.3.0/qframelesswindow/windows/
--rw-rw-rw-   0        0        0     6760 2023-08-07 07:36:58.000000 PyQt6-Frameless-Window-0.3.0/qframelesswindow/windows/__init__.py
--rw-rw-rw-   0        0        0     4261 2023-08-07 07:36:58.000000 PyQt6-Frameless-Window-0.3.0/qframelesswindow/windows/c_structures.py
--rw-rw-rw-   0        0        0     9413 2023-08-07 07:36:58.000000 PyQt6-Frameless-Window-0.3.0/qframelesswindow/windows/window_effect.py
--rw-rw-rw-   0        0        0       42 2023-08-07 07:41:00.137366 PyQt6-Frameless-Window-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      984 2023-08-07 07:39:13.000000 PyQt6-Frameless-Window-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-09 01:44:34.029286 PyQt6-Frameless-Window-0.3.1/
+-rw-rw-rw-   0        0        0    35823 2023-08-07 07:47:32.000000 PyQt6-Frameless-Window-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0     5603 2023-08-09 01:44:34.028178 PyQt6-Frameless-Window-0.3.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-09 01:44:33.969834 PyQt6-Frameless-Window-0.3.1/PyQt6_Frameless_Window.egg-info/
+-rw-rw-rw-   0        0        0     5603 2023-08-09 01:44:33.000000 PyQt6-Frameless-Window-0.3.1/PyQt6_Frameless_Window.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      848 2023-08-09 01:44:33.000000 PyQt6-Frameless-Window-0.3.1/PyQt6_Frameless_Window.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-09 01:44:33.000000 PyQt6-Frameless-Window-0.3.1/PyQt6_Frameless_Window.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-08-09 01:44:33.000000 PyQt6-Frameless-Window-0.3.1/PyQt6_Frameless_Window.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-09 01:44:33.000000 PyQt6-Frameless-Window-0.3.1/PyQt6_Frameless_Window.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5007 2023-08-09 01:42:22.000000 PyQt6-Frameless-Window-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-09 01:44:33.980972 PyQt6-Frameless-Window-0.3.1/qframelesswindow/
+-rw-rw-rw-   0        0        0     1692 2023-08-09 01:42:50.000000 PyQt6-Frameless-Window-0.3.1/qframelesswindow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-09 01:44:33.987617 PyQt6-Frameless-Window-0.3.1/qframelesswindow/_rc/
+-rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PyQt6-Frameless-Window-0.3.1/qframelesswindow/_rc/__init__.py
+-rw-rw-rw-   0        0        0     2728 2023-08-09 01:42:22.000000 PyQt6-Frameless-Window-0.3.1/qframelesswindow/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2023-08-09 01:44:33.994289 PyQt6-Frameless-Window-0.3.1/qframelesswindow/linux/
+-rw-rw-rw-   0        0        0     3110 2023-08-09 01:42:22.000000 PyQt6-Frameless-Window-0.3.1/qframelesswindow/linux/__init__.py
+-rw-rw-rw-   0        0        0     3245 2023-08-09 01:42:50.000000 PyQt6-Frameless-Window-0.3.1/qframelesswindow/linux/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-08-09 01:44:33.999827 PyQt6-Frameless-Window-0.3.1/qframelesswindow/mac/
+-rw-rw-rw-   0        0        0     3015 2023-08-09 01:42:22.000000 PyQt6-Frameless-Window-0.3.1/qframelesswindow/mac/__init__.py
+-rw-rw-rw-   0        0        0     4659 2023-08-09 01:42:50.000000 PyQt6-Frameless-Window-0.3.1/qframelesswindow/mac/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-08-09 01:44:34.005417 PyQt6-Frameless-Window-0.3.1/qframelesswindow/titlebar/
+-rw-rw-rw-   0        0        0     5235 2023-08-09 01:42:22.000000 PyQt6-Frameless-Window-0.3.1/qframelesswindow/titlebar/__init__.py
+-rw-rw-rw-   0        0        0     9205 2023-08-09 01:42:22.000000 PyQt6-Frameless-Window-0.3.1/qframelesswindow/titlebar/title_bar_buttons.py
+drwxrwxrwx   0        0        0        0 2023-08-09 01:44:34.016835 PyQt6-Frameless-Window-0.3.1/qframelesswindow/utils/
+-rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PyQt6-Frameless-Window-0.3.1/qframelesswindow/utils/__init__.py
+-rw-rw-rw-   0        0        0      644 2023-08-09 01:42:22.000000 PyQt6-Frameless-Window-0.3.1/qframelesswindow/utils/linux_utils.py
+-rw-rw-rw-   0        0        0     1850 2023-08-09 01:42:22.000000 PyQt6-Frameless-Window-0.3.1/qframelesswindow/utils/mac_utils.py
+-rw-rw-rw-   0        0        0     8352 2023-08-09 01:42:22.000000 PyQt6-Frameless-Window-0.3.1/qframelesswindow/utils/win32_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-09 01:44:34.025915 PyQt6-Frameless-Window-0.3.1/qframelesswindow/windows/
+-rw-rw-rw-   0        0        0     6760 2023-08-09 01:42:22.000000 PyQt6-Frameless-Window-0.3.1/qframelesswindow/windows/__init__.py
+-rw-rw-rw-   0        0        0     4261 2023-08-09 01:42:22.000000 PyQt6-Frameless-Window-0.3.1/qframelesswindow/windows/c_structures.py
+-rw-rw-rw-   0        0        0     9492 2023-08-09 01:42:50.000000 PyQt6-Frameless-Window-0.3.1/qframelesswindow/windows/window_effect.py
+-rw-rw-rw-   0        0        0       42 2023-08-09 01:44:34.029286 PyQt6-Frameless-Window-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      984 2023-08-09 01:42:56.000000 PyQt6-Frameless-Window-0.3.1/setup.py
```

### Comparing `PyQt6-Frameless-Window-0.3.0/LICENSE` & `PyQt6-Frameless-Window-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.3.0/PKG-INFO` & `PyQt6-Frameless-Window-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt6-Frameless-Window
-Version: 0.3.0
+Version: 0.3.1
 Summary: A cross-platform frameless window based on pyqt6, support Win32, Linux and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PyQt6
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Keywords: pyqt6 frameless
 Platform: UNKNOWN
```

### Comparing `PyQt6-Frameless-Window-0.3.0/PyQt6_Frameless_Window.egg-info/PKG-INFO` & `PyQt6-Frameless-Window-0.3.1/PyQt6_Frameless_Window.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt6-Frameless-Window
-Version: 0.3.0
+Version: 0.3.1
 Summary: A cross-platform frameless window based on pyqt6, support Win32, Linux and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PyQt6
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Keywords: pyqt6 frameless
 Platform: UNKNOWN
```

### Comparing `PyQt6-Frameless-Window-0.3.0/PyQt6_Frameless_Window.egg-info/SOURCES.txt` & `PyQt6-Frameless-Window-0.3.1/PyQt6_Frameless_Window.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.3.0/README.md` & `PyQt6-Frameless-Window-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.3.0/qframelesswindow/__init__.py` & `PyQt6-Frameless-Window-0.3.1/qframelesswindow/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 Examples are available at https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PyQt6/examples.
 
 :copyright: (c) 2021 by zhiyiYo.
 :license: GPLv3, see LICENSE for more details.
 """
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 
 import sys
 
 from PyQt6.QtWidgets import QDialog, QMainWindow
 
 from .titlebar import TitleBar, TitleBarButton, SvgTitleBarButton, StandardTitleBar, TitleBarBase
```

### Comparing `PyQt6-Frameless-Window-0.3.0/qframelesswindow/_rc/resource.py` & `PyQt6-Frameless-Window-0.3.1/qframelesswindow/_rc/resource.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.3.0/qframelesswindow/linux/__init__.py` & `PyQt6-Frameless-Window-0.3.1/qframelesswindow/linux/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.3.0/qframelesswindow/linux/window_effect.py` & `PyQt6-Frameless-Window-0.3.1/qframelesswindow/linux/window_effect.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,21 +21,24 @@
             whether to enable window shadow
 
         animationId: int
             turn on blur animation or not
         """
         pass
 
-    def setMicaEffect(self, hWnd):
+    def setMicaEffect(self, hWnd, isDarkMode=False):
         """ Add mica effect to the window (Win11 only)
 
         Parameters
         ----------
         hWnd: int or `sip.voidptr`
             Window handle
+
+        isDarkMode: bool
+            whether to use dark mode mica effect
         """
         pass
 
     def setAeroEffect(self, hWnd):
         """ add Aero effect to the window
 
         Parameter
```

### Comparing `PyQt6-Frameless-Window-0.3.0/qframelesswindow/mac/__init__.py` & `PyQt6-Frameless-Window-0.3.1/qframelesswindow/mac/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.3.0/qframelesswindow/mac/window_effect.py` & `PyQt6-Frameless-Window-0.3.1/qframelesswindow/mac/window_effect.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,21 +50,24 @@
 
         nsWindow = getNSWindow(self.window.winId())
         content = nsWindow.contentView()
         container = QMacCocoaViewContainer(0, self.window)
         content.addSubview_positioned_relativeTo_(
             visualEffectView, Cocoa.NSWindowBelow, container)
 
-    def setMicaEffect(self, hWnd):
+    def setMicaEffect(self, hWnd, isDarkMode=False):
         """ Add mica effect to the window (Win11 only)
 
         Parameters
         ----------
         hWnd: int or `sip.voidptr`
             Window handle
+
+        isDarkMode: bool
+            whether to use dark mode mica effect
         """
         self.setAcrylicEffect(hWnd)
 
     def setAeroEffect(self, hWnd):
         """ add Aero effect to the window
 
         Parameter
```

### Comparing `PyQt6-Frameless-Window-0.3.0/qframelesswindow/titlebar/__init__.py` & `PyQt6-Frameless-Window-0.3.1/qframelesswindow/titlebar/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.3.0/qframelesswindow/titlebar/title_bar_buttons.py` & `PyQt6-Frameless-Window-0.3.1/qframelesswindow/titlebar/title_bar_buttons.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.3.0/qframelesswindow/utils/__init__.py` & `PyQt6-Frameless-Window-0.3.1/qframelesswindow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.3.0/qframelesswindow/utils/linux_utils.py` & `PyQt6-Frameless-Window-0.3.1/qframelesswindow/utils/linux_utils.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.3.0/qframelesswindow/utils/mac_utils.py` & `PyQt6-Frameless-Window-0.3.1/qframelesswindow/utils/mac_utils.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.3.0/qframelesswindow/utils/win32_utils.py` & `PyQt6-Frameless-Window-0.3.1/qframelesswindow/utils/win32_utils.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.3.0/qframelesswindow/windows/__init__.py` & `PyQt6-Frameless-Window-0.3.1/qframelesswindow/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.3.0/qframelesswindow/windows/c_structures.py` & `PyQt6-Frameless-Window-0.3.1/qframelesswindow/windows/c_structures.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Frameless-Window-0.3.0/qframelesswindow/windows/window_effect.py` & `PyQt6-Frameless-Window-0.3.1/qframelesswindow/windows/window_effect.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,16 @@
                 hWnd, pointer(self.winCompAttrData))
 
         if sys.getwindowsversion().build < 22523:
             self.DwmSetWindowAttribute(hWnd, 1029, byref(c_int(1)), 4)
         else:
             self.DwmSetWindowAttribute(hWnd, 38, byref(c_int(2)), 4)
 
+        self.DwmSetWindowAttribute(hWnd, 20, byref(c_int(1*isDarkMode)), 4)
+
     def setAeroEffect(self, hWnd):
         """ Add the aero effect to the window
 
         Parameters
         ----------
         hWnd: int or `sip.voidptr`
             Window handle
```

### Comparing `PyQt6-Frameless-Window-0.3.0/setup.py` & `PyQt6-Frameless-Window-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PyQt6-Frameless-Window",
-    version="0.3.0",
+    version="0.3.1",
     keywords="pyqt6 frameless",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A cross-platform frameless window based on pyqt6, support Win32, Linux and macOS.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="GPLv3",
```

