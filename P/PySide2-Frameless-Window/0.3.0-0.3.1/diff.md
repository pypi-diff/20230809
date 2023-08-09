# Comparing `tmp/PySide2-Frameless-Window-0.3.0.tar.gz` & `tmp/PySide2-Frameless-Window-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PySide2-Frameless-Window-0.3.0.tar", last modified: Mon Aug  7 07:43:47 2023, max compression
+gzip compressed data, was "dist\PySide2-Frameless-Window-0.3.1.tar", last modified: Wed Aug  9 01:48:00 2023, max compression
```

## Comparing `PySide2-Frameless-Window-0.3.0.tar` & `PySide2-Frameless-Window-0.3.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 07:43:47.217928 PySide2-Frameless-Window-0.3.0/
--rw-rw-rw-   0        0        0     7815 2023-08-07 07:43:41.000000 PySide2-Frameless-Window-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     5649 2023-08-07 07:43:47.216270 PySide2-Frameless-Window-0.3.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-07 07:43:47.186791 PySide2-Frameless-Window-0.3.0/PySide2_Frameless_Window.egg-info/
--rw-rw-rw-   0        0        0     5649 2023-08-07 07:43:47.000000 PySide2-Frameless-Window-0.3.0/PySide2_Frameless_Window.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      858 2023-08-07 07:43:47.000000 PySide2-Frameless-Window-0.3.0/PySide2_Frameless_Window.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 07:43:47.000000 PySide2-Frameless-Window-0.3.0/PySide2_Frameless_Window.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-08-07 07:43:47.000000 PySide2-Frameless-Window-0.3.0/PySide2_Frameless_Window.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-08-07 07:43:47.000000 PySide2-Frameless-Window-0.3.0/PySide2_Frameless_Window.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5036 2023-08-07 07:43:41.000000 PySide2-Frameless-Window-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-07 07:43:47.189996 PySide2-Frameless-Window-0.3.0/qframelesswindow/
--rw-rw-rw-   0        0        0     2328 2023-08-07 07:43:41.000000 PySide2-Frameless-Window-0.3.0/qframelesswindow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-07 07:43:47.192946 PySide2-Frameless-Window-0.3.0/qframelesswindow/_rc/
--rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PySide2-Frameless-Window-0.3.0/qframelesswindow/_rc/__init__.py
--rw-rw-rw-   0        0        0     2730 2023-08-07 07:43:41.000000 PySide2-Frameless-Window-0.3.0/qframelesswindow/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2023-08-07 07:43:47.196346 PySide2-Frameless-Window-0.3.0/qframelesswindow/linux/
--rw-rw-rw-   0        0        0     2878 2023-08-07 07:43:41.000000 PySide2-Frameless-Window-0.3.0/qframelesswindow/linux/__init__.py
--rw-rw-rw-   0        0        0     2912 2023-08-07 07:43:41.000000 PySide2-Frameless-Window-0.3.0/qframelesswindow/linux/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-08-07 07:43:47.199549 PySide2-Frameless-Window-0.3.0/qframelesswindow/mac/
--rw-rw-rw-   0        0        0     3024 2023-08-07 07:43:41.000000 PySide2-Frameless-Window-0.3.0/qframelesswindow/mac/__init__.py
--rw-rw-rw-   0        0        0     4314 2023-08-07 07:43:41.000000 PySide2-Frameless-Window-0.3.0/qframelesswindow/mac/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-08-07 07:43:47.203735 PySide2-Frameless-Window-0.3.0/qframelesswindow/titlebar/
--rw-rw-rw-   0        0        0     5086 2023-08-07 07:43:41.000000 PySide2-Frameless-Window-0.3.0/qframelesswindow/titlebar/__init__.py
--rw-rw-rw-   0        0        0     9039 2023-08-07 07:43:41.000000 PySide2-Frameless-Window-0.3.0/qframelesswindow/titlebar/title_bar_buttons.py
-drwxrwxrwx   0        0        0        0 2023-08-07 07:43:47.210261 PySide2-Frameless-Window-0.3.0/qframelesswindow/utils/
--rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PySide2-Frameless-Window-0.3.0/qframelesswindow/utils/__init__.py
--rw-rw-rw-   0        0        0     1216 2023-08-07 07:43:41.000000 PySide2-Frameless-Window-0.3.0/qframelesswindow/utils/linux_utils.py
--rw-rw-rw-   0        0        0     1844 2023-08-07 07:43:41.000000 PySide2-Frameless-Window-0.3.0/qframelesswindow/utils/mac_utils.py
--rw-rw-rw-   0        0        0     7973 2023-08-07 07:43:41.000000 PySide2-Frameless-Window-0.3.0/qframelesswindow/utils/win32_utils.py
-drwxrwxrwx   0        0        0        0 2023-08-07 07:43:47.215269 PySide2-Frameless-Window-0.3.0/qframelesswindow/windows/
--rw-rw-rw-   0        0        0     7214 2023-08-07 07:43:41.000000 PySide2-Frameless-Window-0.3.0/qframelesswindow/windows/__init__.py
--rw-rw-rw-   0        0        0     4013 2023-08-07 07:43:41.000000 PySide2-Frameless-Window-0.3.0/qframelesswindow/windows/c_structures.py
--rw-rw-rw-   0        0        0     8810 2023-08-07 07:43:41.000000 PySide2-Frameless-Window-0.3.0/qframelesswindow/windows/window_effect.py
--rw-rw-rw-   0        0        0       42 2023-08-07 07:43:47.217928 PySide2-Frameless-Window-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1001 2023-08-07 07:43:41.000000 PySide2-Frameless-Window-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-09 01:48:00.394154 PySide2-Frameless-Window-0.3.1/
+-rw-rw-rw-   0        0        0     7815 2023-08-09 01:45:02.000000 PySide2-Frameless-Window-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0     5649 2023-08-09 01:48:00.393102 PySide2-Frameless-Window-0.3.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-09 01:48:00.353174 PySide2-Frameless-Window-0.3.1/PySide2_Frameless_Window.egg-info/
+-rw-rw-rw-   0        0        0     5649 2023-08-09 01:48:00.000000 PySide2-Frameless-Window-0.3.1/PySide2_Frameless_Window.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      858 2023-08-09 01:48:00.000000 PySide2-Frameless-Window-0.3.1/PySide2_Frameless_Window.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-09 01:48:00.000000 PySide2-Frameless-Window-0.3.1/PySide2_Frameless_Window.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-08-09 01:48:00.000000 PySide2-Frameless-Window-0.3.1/PySide2_Frameless_Window.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-09 01:48:00.000000 PySide2-Frameless-Window-0.3.1/PySide2_Frameless_Window.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5036 2023-08-09 01:46:48.000000 PySide2-Frameless-Window-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-09 01:48:00.356193 PySide2-Frameless-Window-0.3.1/qframelesswindow/
+-rw-rw-rw-   0        0        0     2328 2023-08-09 01:47:01.000000 PySide2-Frameless-Window-0.3.1/qframelesswindow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-09 01:48:00.359542 PySide2-Frameless-Window-0.3.1/qframelesswindow/_rc/
+-rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PySide2-Frameless-Window-0.3.1/qframelesswindow/_rc/__init__.py
+-rw-rw-rw-   0        0        0     2730 2023-08-09 01:46:48.000000 PySide2-Frameless-Window-0.3.1/qframelesswindow/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2023-08-09 01:48:00.365186 PySide2-Frameless-Window-0.3.1/qframelesswindow/linux/
+-rw-rw-rw-   0        0        0     2878 2023-08-09 01:46:48.000000 PySide2-Frameless-Window-0.3.1/qframelesswindow/linux/__init__.py
+-rw-rw-rw-   0        0        0     3008 2023-08-09 01:47:01.000000 PySide2-Frameless-Window-0.3.1/qframelesswindow/linux/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-08-09 01:48:00.369134 PySide2-Frameless-Window-0.3.1/qframelesswindow/mac/
+-rw-rw-rw-   0        0        0     3024 2023-08-09 01:46:48.000000 PySide2-Frameless-Window-0.3.1/qframelesswindow/mac/__init__.py
+-rw-rw-rw-   0        0        0     4410 2023-08-09 01:47:01.000000 PySide2-Frameless-Window-0.3.1/qframelesswindow/mac/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-08-09 01:48:00.372677 PySide2-Frameless-Window-0.3.1/qframelesswindow/titlebar/
+-rw-rw-rw-   0        0        0     5086 2023-08-09 01:46:48.000000 PySide2-Frameless-Window-0.3.1/qframelesswindow/titlebar/__init__.py
+-rw-rw-rw-   0        0        0     9039 2023-08-09 01:46:48.000000 PySide2-Frameless-Window-0.3.1/qframelesswindow/titlebar/title_bar_buttons.py
+drwxrwxrwx   0        0        0        0 2023-08-09 01:48:00.384181 PySide2-Frameless-Window-0.3.1/qframelesswindow/utils/
+-rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PySide2-Frameless-Window-0.3.1/qframelesswindow/utils/__init__.py
+-rw-rw-rw-   0        0        0     1216 2023-08-09 01:46:48.000000 PySide2-Frameless-Window-0.3.1/qframelesswindow/utils/linux_utils.py
+-rw-rw-rw-   0        0        0     1844 2023-08-09 01:46:48.000000 PySide2-Frameless-Window-0.3.1/qframelesswindow/utils/mac_utils.py
+-rw-rw-rw-   0        0        0     7973 2023-08-09 01:46:48.000000 PySide2-Frameless-Window-0.3.1/qframelesswindow/utils/win32_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-09 01:48:00.390596 PySide2-Frameless-Window-0.3.1/qframelesswindow/windows/
+-rw-rw-rw-   0        0        0     7214 2023-08-09 01:46:48.000000 PySide2-Frameless-Window-0.3.1/qframelesswindow/windows/__init__.py
+-rw-rw-rw-   0        0        0     4013 2023-08-09 01:46:48.000000 PySide2-Frameless-Window-0.3.1/qframelesswindow/windows/c_structures.py
+-rw-rw-rw-   0        0        0     8889 2023-08-09 01:47:01.000000 PySide2-Frameless-Window-0.3.1/qframelesswindow/windows/window_effect.py
+-rw-rw-rw-   0        0        0       42 2023-08-09 01:48:00.394154 PySide2-Frameless-Window-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1001 2023-08-09 01:47:05.000000 PySide2-Frameless-Window-0.3.1/setup.py
```

### Comparing `PySide2-Frameless-Window-0.3.0/LICENSE` & `PySide2-Frameless-Window-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.3.0/PKG-INFO` & `PySide2-Frameless-Window-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySide2-Frameless-Window
-Version: 0.3.0
+Version: 0.3.1
 Summary: A cross-platform frameless window based on pyside2, support Win32, Linux and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/Pyside2
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: LGPLv3
 Keywords: pyside2 frameless
 Platform: UNKNOWN
```

### Comparing `PySide2-Frameless-Window-0.3.0/PySide2_Frameless_Window.egg-info/PKG-INFO` & `PySide2-Frameless-Window-0.3.1/PySide2_Frameless_Window.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySide2-Frameless-Window
-Version: 0.3.0
+Version: 0.3.1
 Summary: A cross-platform frameless window based on pyside2, support Win32, Linux and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/Pyside2
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: LGPLv3
 Keywords: pyside2 frameless
 Platform: UNKNOWN
```

### Comparing `PySide2-Frameless-Window-0.3.0/PySide2_Frameless_Window.egg-info/SOURCES.txt` & `PySide2-Frameless-Window-0.3.1/PySide2_Frameless_Window.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.3.0/README.md` & `PySide2-Frameless-Window-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.3.0/qframelesswindow/__init__.py` & `PySide2-Frameless-Window-0.3.1/qframelesswindow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 Examples are available at https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/Pyside2/examples.
 
 :copyright: (c) 2021 by zhiyiYo.
 :license: LGPLv3, see LICENSE for more details.
 """
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 
 import sys
 
 from PySide2.QtWidgets import QDialog, QMainWindow
 
 from .titlebar import TitleBar, TitleBarButton, SvgTitleBarButton, StandardTitleBar, TitleBarBase
```

### Comparing `PySide2-Frameless-Window-0.3.0/qframelesswindow/_rc/resource.py` & `PySide2-Frameless-Window-0.3.1/qframelesswindow/_rc/resource.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.3.0/qframelesswindow/linux/__init__.py` & `PySide2-Frameless-Window-0.3.1/qframelesswindow/linux/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.3.0/qframelesswindow/linux/window_effect.py` & `PySide2-Frameless-Window-0.3.1/qframelesswindow/linux/window_effect.py`

 * *Files 20% similar despite different names*

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

### Comparing `PySide2-Frameless-Window-0.3.0/qframelesswindow/mac/__init__.py` & `PySide2-Frameless-Window-0.3.1/qframelesswindow/mac/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.3.0/qframelesswindow/mac/window_effect.py` & `PySide2-Frameless-Window-0.3.1/qframelesswindow/mac/window_effect.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,21 +51,24 @@
 
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

### Comparing `PySide2-Frameless-Window-0.3.0/qframelesswindow/titlebar/__init__.py` & `PySide2-Frameless-Window-0.3.1/qframelesswindow/titlebar/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.3.0/qframelesswindow/titlebar/title_bar_buttons.py` & `PySide2-Frameless-Window-0.3.1/qframelesswindow/titlebar/title_bar_buttons.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.3.0/qframelesswindow/utils/__init__.py` & `PySide2-Frameless-Window-0.3.1/qframelesswindow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.3.0/qframelesswindow/utils/linux_utils.py` & `PySide2-Frameless-Window-0.3.1/qframelesswindow/utils/linux_utils.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.3.0/qframelesswindow/utils/mac_utils.py` & `PySide2-Frameless-Window-0.3.1/qframelesswindow/utils/mac_utils.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.3.0/qframelesswindow/utils/win32_utils.py` & `PySide2-Frameless-Window-0.3.1/qframelesswindow/utils/win32_utils.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.3.0/qframelesswindow/windows/__init__.py` & `PySide2-Frameless-Window-0.3.1/qframelesswindow/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.3.0/qframelesswindow/windows/c_structures.py` & `PySide2-Frameless-Window-0.3.1/qframelesswindow/windows/c_structures.py`

 * *Files identical despite different names*

### Comparing `PySide2-Frameless-Window-0.3.0/qframelesswindow/windows/window_effect.py` & `PySide2-Frameless-Window-0.3.1/qframelesswindow/windows/window_effect.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,14 +106,16 @@
             self.SetWindowCompositionAttribute(hWnd, pointer(self.winCompAttrData))
 
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

### Comparing `PySide2-Frameless-Window-0.3.0/setup.py` & `PySide2-Frameless-Window-0.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PySide2-Frameless-Window",
-    version="0.3.0",
+    version="0.3.1",
     keywords="pyside2 frameless",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A cross-platform frameless window based on pyside2, support Win32, Linux and macOS.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="LGPLv3",
```

