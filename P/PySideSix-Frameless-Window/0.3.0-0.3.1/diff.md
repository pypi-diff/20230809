# Comparing `tmp/PySideSix-Frameless-Window-0.3.0.tar.gz` & `tmp/PySideSix-Frameless-Window-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PySideSix-Frameless-Window-0.3.0.tar", last modified: Mon Aug  7 07:30:54 2023, max compression
+gzip compressed data, was "dist\PySideSix-Frameless-Window-0.3.1.tar", last modified: Wed Aug  9 01:46:17 2023, max compression
```

## Comparing `PySideSix-Frameless-Window-0.3.0.tar` & `PySideSix-Frameless-Window-0.3.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 07:30:54.892009 PySideSix-Frameless-Window-0.3.0/
--rw-rw-rw-   0        0        0     7815 2023-08-07 07:18:10.000000 PySideSix-Frameless-Window-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     5672 2023-08-07 07:30:54.890999 PySideSix-Frameless-Window-0.3.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-07 07:30:54.856305 PySideSix-Frameless-Window-0.3.0/PySideSix_Frameless_Window.egg-info/
--rw-rw-rw-   0        0        0     5672 2023-08-07 07:30:54.000000 PySideSix-Frameless-Window-0.3.0/PySideSix_Frameless_Window.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      868 2023-08-07 07:30:54.000000 PySideSix-Frameless-Window-0.3.0/PySideSix_Frameless_Window.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 07:30:54.000000 PySideSix-Frameless-Window-0.3.0/PySideSix_Frameless_Window.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-08-07 07:30:54.000000 PySideSix-Frameless-Window-0.3.0/PySideSix_Frameless_Window.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-08-07 07:30:54.000000 PySideSix-Frameless-Window-0.3.0/PySideSix_Frameless_Window.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5057 2023-08-07 07:18:10.000000 PySideSix-Frameless-Window-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-07 07:30:54.865691 PySideSix-Frameless-Window-0.3.0/qframelesswindow/
--rw-rw-rw-   0        0        0     1628 2023-08-07 07:26:28.000000 PySideSix-Frameless-Window-0.3.0/qframelesswindow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-07 07:30:54.868705 PySideSix-Frameless-Window-0.3.0/qframelesswindow/_rc/
--rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PySideSix-Frameless-Window-0.3.0/qframelesswindow/_rc/__init__.py
--rw-rw-rw-   0        0        0     1477 2023-08-07 07:18:10.000000 PySideSix-Frameless-Window-0.3.0/qframelesswindow/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2023-08-07 07:30:54.871705 PySideSix-Frameless-Window-0.3.0/qframelesswindow/linux/
--rw-rw-rw-   0        0        0     4320 2023-08-07 07:18:10.000000 PySideSix-Frameless-Window-0.3.0/qframelesswindow/linux/__init__.py
--rw-rw-rw-   0        0        0     3147 2023-08-07 07:18:10.000000 PySideSix-Frameless-Window-0.3.0/qframelesswindow/linux/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-08-07 07:30:54.875223 PySideSix-Frameless-Window-0.3.0/qframelesswindow/mac/
--rw-rw-rw-   0        0        0     4529 2023-08-07 07:18:10.000000 PySideSix-Frameless-Window-0.3.0/qframelesswindow/mac/__init__.py
--rw-rw-rw-   0        0        0     4549 2023-08-07 07:18:10.000000 PySideSix-Frameless-Window-0.3.0/qframelesswindow/mac/window_effect.py
-drwxrwxrwx   0        0        0        0 2023-08-07 07:30:54.879027 PySideSix-Frameless-Window-0.3.0/qframelesswindow/titlebar/
--rw-rw-rw-   0        0        0     5208 2023-08-07 07:19:54.000000 PySideSix-Frameless-Window-0.3.0/qframelesswindow/titlebar/__init__.py
--rw-rw-rw-   0        0        0     9039 2023-08-07 07:18:10.000000 PySideSix-Frameless-Window-0.3.0/qframelesswindow/titlebar/title_bar_buttons.py
-drwxrwxrwx   0        0        0        0 2023-08-07 07:30:54.884198 PySideSix-Frameless-Window-0.3.0/qframelesswindow/utils/
--rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PySideSix-Frameless-Window-0.3.0/qframelesswindow/utils/__init__.py
--rw-rw-rw-   0        0        0     1216 2023-08-07 07:18:10.000000 PySideSix-Frameless-Window-0.3.0/qframelesswindow/utils/linux_utils.py
--rw-rw-rw-   0        0        0     1844 2023-08-07 07:18:10.000000 PySideSix-Frameless-Window-0.3.0/qframelesswindow/utils/mac_utils.py
--rw-rw-rw-   0        0        0     8093 2023-08-07 07:18:10.000000 PySideSix-Frameless-Window-0.3.0/qframelesswindow/utils/win32_utils.py
-drwxrwxrwx   0        0        0        0 2023-08-07 07:30:54.889612 PySideSix-Frameless-Window-0.3.0/qframelesswindow/windows/
--rw-rw-rw-   0        0        0     8379 2023-08-07 07:18:10.000000 PySideSix-Frameless-Window-0.3.0/qframelesswindow/windows/__init__.py
--rw-rw-rw-   0        0        0     4261 2023-08-07 07:18:10.000000 PySideSix-Frameless-Window-0.3.0/qframelesswindow/windows/c_structures.py
--rw-rw-rw-   0        0        0     9369 2023-08-07 07:18:10.000000 PySideSix-Frameless-Window-0.3.0/qframelesswindow/windows/window_effect.py
--rw-rw-rw-   0        0        0       42 2023-08-07 07:30:54.892009 PySideSix-Frameless-Window-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1003 2023-08-07 07:26:35.000000 PySideSix-Frameless-Window-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-09 01:46:17.062455 PySideSix-Frameless-Window-0.3.1/
+-rw-rw-rw-   0        0        0     7815 2023-08-09 01:45:02.000000 PySideSix-Frameless-Window-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0     5672 2023-08-09 01:46:17.061453 PySideSix-Frameless-Window-0.3.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-09 01:46:17.021126 PySideSix-Frameless-Window-0.3.1/PySideSix_Frameless_Window.egg-info/
+-rw-rw-rw-   0        0        0     5672 2023-08-09 01:46:16.000000 PySideSix-Frameless-Window-0.3.1/PySideSix_Frameless_Window.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      868 2023-08-09 01:46:16.000000 PySideSix-Frameless-Window-0.3.1/PySideSix_Frameless_Window.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-09 01:46:16.000000 PySideSix-Frameless-Window-0.3.1/PySideSix_Frameless_Window.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-08-09 01:46:16.000000 PySideSix-Frameless-Window-0.3.1/PySideSix_Frameless_Window.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-09 01:46:16.000000 PySideSix-Frameless-Window-0.3.1/PySideSix_Frameless_Window.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5057 2023-08-09 01:45:02.000000 PySideSix-Frameless-Window-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-09 01:46:17.024135 PySideSix-Frameless-Window-0.3.1/qframelesswindow/
+-rw-rw-rw-   0        0        0     1628 2023-08-09 01:45:14.000000 PySideSix-Frameless-Window-0.3.1/qframelesswindow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-09 01:46:17.028533 PySideSix-Frameless-Window-0.3.1/qframelesswindow/_rc/
+-rw-rw-rw-   0        0        0        0 2023-01-28 14:21:55.000000 PySideSix-Frameless-Window-0.3.1/qframelesswindow/_rc/__init__.py
+-rw-rw-rw-   0        0        0     1477 2023-08-09 01:45:02.000000 PySideSix-Frameless-Window-0.3.1/qframelesswindow/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2023-08-09 01:46:17.032081 PySideSix-Frameless-Window-0.3.1/qframelesswindow/linux/
+-rw-rw-rw-   0        0        0     4320 2023-08-09 01:45:02.000000 PySideSix-Frameless-Window-0.3.1/qframelesswindow/linux/__init__.py
+-rw-rw-rw-   0        0        0     3243 2023-08-09 01:45:14.000000 PySideSix-Frameless-Window-0.3.1/qframelesswindow/linux/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-08-09 01:46:17.036263 PySideSix-Frameless-Window-0.3.1/qframelesswindow/mac/
+-rw-rw-rw-   0        0        0     4529 2023-08-09 01:45:02.000000 PySideSix-Frameless-Window-0.3.1/qframelesswindow/mac/__init__.py
+-rw-rw-rw-   0        0        0     4645 2023-08-09 01:45:14.000000 PySideSix-Frameless-Window-0.3.1/qframelesswindow/mac/window_effect.py
+drwxrwxrwx   0        0        0        0 2023-08-09 01:46:17.041986 PySideSix-Frameless-Window-0.3.1/qframelesswindow/titlebar/
+-rw-rw-rw-   0        0        0     5208 2023-08-09 01:45:02.000000 PySideSix-Frameless-Window-0.3.1/qframelesswindow/titlebar/__init__.py
+-rw-rw-rw-   0        0        0     9039 2023-08-09 01:45:02.000000 PySideSix-Frameless-Window-0.3.1/qframelesswindow/titlebar/title_bar_buttons.py
+drwxrwxrwx   0        0        0        0 2023-08-09 01:46:17.052449 PySideSix-Frameless-Window-0.3.1/qframelesswindow/utils/
+-rw-rw-rw-   0        0        0      885 2022-07-25 01:20:40.000000 PySideSix-Frameless-Window-0.3.1/qframelesswindow/utils/__init__.py
+-rw-rw-rw-   0        0        0     1216 2023-08-09 01:45:02.000000 PySideSix-Frameless-Window-0.3.1/qframelesswindow/utils/linux_utils.py
+-rw-rw-rw-   0        0        0     1844 2023-08-09 01:45:02.000000 PySideSix-Frameless-Window-0.3.1/qframelesswindow/utils/mac_utils.py
+-rw-rw-rw-   0        0        0     8093 2023-08-09 01:45:02.000000 PySideSix-Frameless-Window-0.3.1/qframelesswindow/utils/win32_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-09 01:46:17.059447 PySideSix-Frameless-Window-0.3.1/qframelesswindow/windows/
+-rw-rw-rw-   0        0        0     8379 2023-08-09 01:45:02.000000 PySideSix-Frameless-Window-0.3.1/qframelesswindow/windows/__init__.py
+-rw-rw-rw-   0        0        0     4261 2023-08-09 01:45:02.000000 PySideSix-Frameless-Window-0.3.1/qframelesswindow/windows/c_structures.py
+-rw-rw-rw-   0        0        0     9448 2023-08-09 01:45:14.000000 PySideSix-Frameless-Window-0.3.1/qframelesswindow/windows/window_effect.py
+-rw-rw-rw-   0        0        0       42 2023-08-09 01:46:17.062974 PySideSix-Frameless-Window-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2023-08-09 01:45:19.000000 PySideSix-Frameless-Window-0.3.1/setup.py
```

### Comparing `PySideSix-Frameless-Window-0.3.0/LICENSE` & `PySideSix-Frameless-Window-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.3.0/PKG-INFO` & `PySideSix-Frameless-Window-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySideSix-Frameless-Window
-Version: 0.3.0
+Version: 0.3.1
 Summary: A cross-platform frameless window based on pyside6, support Win32, Linux and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PySide6
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: LGPLv3
 Keywords: pyside6 frameless
 Platform: UNKNOWN
```

### Comparing `PySideSix-Frameless-Window-0.3.0/PySideSix_Frameless_Window.egg-info/PKG-INFO` & `PySideSix-Frameless-Window-0.3.1/PySideSix_Frameless_Window.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySideSix-Frameless-Window
-Version: 0.3.0
+Version: 0.3.1
 Summary: A cross-platform frameless window based on pyside6, support Win32, Linux and macOS.
 Home-page: https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PySide6
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: LGPLv3
 Keywords: pyside6 frameless
 Platform: UNKNOWN
```

### Comparing `PySideSix-Frameless-Window-0.3.0/PySideSix_Frameless_Window.egg-info/SOURCES.txt` & `PySideSix-Frameless-Window-0.3.1/PySideSix_Frameless_Window.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.3.0/README.md` & `PySideSix-Frameless-Window-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.3.0/qframelesswindow/__init__.py` & `PySideSix-Frameless-Window-0.3.1/qframelesswindow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 Examples are available at https://github.com/zhiyiYo/PyQt-Frameless-Window/tree/PySide6/examples.
 
 :copyright: (c) 2021 by zhiyiYo.
 :license: LGPLv3, see LICENSE for more details.
 """
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 
 import sys
 
 from PySide6.QtCore import Qt
 from PySide6.QtWidgets import QDialog, QMainWindow
 
 from .titlebar import TitleBar, TitleBarButton, SvgTitleBarButton, StandardTitleBar, TitleBarBase
```

### Comparing `PySideSix-Frameless-Window-0.3.0/qframelesswindow/_rc/resource.py` & `PySideSix-Frameless-Window-0.3.1/qframelesswindow/_rc/resource.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.3.0/qframelesswindow/linux/__init__.py` & `PySideSix-Frameless-Window-0.3.1/qframelesswindow/linux/__init__.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.3.0/qframelesswindow/linux/window_effect.py` & `PySideSix-Frameless-Window-0.3.1/qframelesswindow/linux/window_effect.py`

 * *Files 9% similar despite different names*

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

### Comparing `PySideSix-Frameless-Window-0.3.0/qframelesswindow/mac/__init__.py` & `PySideSix-Frameless-Window-0.3.1/qframelesswindow/mac/__init__.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.3.0/qframelesswindow/mac/window_effect.py` & `PySideSix-Frameless-Window-0.3.1/qframelesswindow/mac/window_effect.py`

 * *Files 2% similar despite different names*

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

### Comparing `PySideSix-Frameless-Window-0.3.0/qframelesswindow/titlebar/__init__.py` & `PySideSix-Frameless-Window-0.3.1/qframelesswindow/titlebar/__init__.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.3.0/qframelesswindow/titlebar/title_bar_buttons.py` & `PySideSix-Frameless-Window-0.3.1/qframelesswindow/titlebar/title_bar_buttons.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.3.0/qframelesswindow/utils/__init__.py` & `PySideSix-Frameless-Window-0.3.1/qframelesswindow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.3.0/qframelesswindow/utils/linux_utils.py` & `PySideSix-Frameless-Window-0.3.1/qframelesswindow/utils/linux_utils.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.3.0/qframelesswindow/utils/mac_utils.py` & `PySideSix-Frameless-Window-0.3.1/qframelesswindow/utils/mac_utils.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.3.0/qframelesswindow/utils/win32_utils.py` & `PySideSix-Frameless-Window-0.3.1/qframelesswindow/utils/win32_utils.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.3.0/qframelesswindow/windows/__init__.py` & `PySideSix-Frameless-Window-0.3.1/qframelesswindow/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.3.0/qframelesswindow/windows/c_structures.py` & `PySideSix-Frameless-Window-0.3.1/qframelesswindow/windows/c_structures.py`

 * *Files identical despite different names*

### Comparing `PySideSix-Frameless-Window-0.3.0/qframelesswindow/windows/window_effect.py` & `PySideSix-Frameless-Window-0.3.1/qframelesswindow/windows/window_effect.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,14 +110,16 @@
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

### Comparing `PySideSix-Frameless-Window-0.3.0/setup.py` & `PySideSix-Frameless-Window-0.3.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PySideSix-Frameless-Window",
-    version="0.3.0",
+    version="0.3.1",
     keywords="pyside6 frameless",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A cross-platform frameless window based on pyside6, support Win32, Linux and macOS.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="LGPLv3",
```

