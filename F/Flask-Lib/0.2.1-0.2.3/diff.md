# Comparing `tmp/Flask-Lib-0.2.1.tar.gz` & `tmp/Flask-Lib-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-Lib-0.2.1.tar", last modified: Thu Jul 27 15:26:49 2023, max compression
+gzip compressed data, was "Flask-Lib-0.2.3.tar", last modified: Tue Aug  8 23:37:03 2023, max compression
```

## Comparing `Flask-Lib-0.2.1.tar` & `Flask-Lib-0.2.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 15:26:49.615145 Flask-Lib-0.2.1/
--rw-rw-rw-   0        0        0     1529 2023-05-04 01:08:33.000000 Flask-Lib-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      701 2023-07-27 15:26:49.616143 Flask-Lib-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-05-09 00:54:20.000000 Flask-Lib-0.2.1/README.md
--rw-rw-rw-   0        0        0      801 2023-07-27 15:26:49.617140 Flask-Lib-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0       36 2023-05-09 00:43:43.000000 Flask-Lib-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-27 15:26:49.595199 Flask-Lib-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-27 15:26:49.609161 Flask-Lib-0.2.1/src/Flask_Lib.egg-info/
--rw-rw-rw-   0        0        0      701 2023-07-27 15:26:49.000000 Flask-Lib-0.2.1/src/Flask_Lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      448 2023-07-27 15:26:49.000000 Flask-Lib-0.2.1/src/Flask_Lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 15:26:49.000000 Flask-Lib-0.2.1/src/Flask_Lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      291 2023-07-27 15:26:49.000000 Flask-Lib-0.2.1/src/Flask_Lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-27 15:26:49.000000 Flask-Lib-0.2.1/src/Flask_Lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-27 15:26:49.613151 Flask-Lib-0.2.1/src/flasklib/
--rw-rw-rw-   0        0        0      218 2023-07-27 14:10:28.000000 Flask-Lib-0.2.1/src/flasklib/__init__.py
--rw-rw-rw-   0        0        0     2840 2023-05-04 22:19:44.000000 Flask-Lib-0.2.1/src/flasklib/dates.py
--rw-rw-rw-   0        0        0     1062 2023-05-04 22:19:44.000000 Flask-Lib-0.2.1/src/flasklib/errors.py
--rw-rw-rw-   0        0        0      836 2023-05-09 00:44:22.000000 Flask-Lib-0.2.1/src/flasklib/jinja.py
--rw-rw-rw-   0        0        0     1376 2023-05-04 01:27:16.000000 Flask-Lib-0.2.1/src/flasklib/json.py
-drwxrwxrwx   0        0        0        0 2023-07-27 15:26:49.615145 Flask-Lib-0.2.1/src/flasklib/mappers/
--rw-rw-rw-   0        0        0      129 2023-05-04 01:41:47.000000 Flask-Lib-0.2.1/src/flasklib/mappers/__init__.py
--rw-rw-rw-   0        0        0     1492 2023-07-27 15:25:17.000000 Flask-Lib-0.2.1/src/flasklib/mappers/mappers.py
--rw-rw-rw-   0        0        0     1937 2023-05-04 22:19:44.000000 Flask-Lib-0.2.1/src/flasklib/responses.py
--rw-rw-rw-   0        0        0      427 2023-05-04 22:19:44.000000 Flask-Lib-0.2.1/src/flasklib/startup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 23:37:03.102483 Flask-Lib-0.2.3/
+-rw-rw-rw-   0        0        0     1529 2023-05-04 01:08:33.000000 Flask-Lib-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0      698 2023-08-08 23:37:03.102483 Flask-Lib-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-05-09 00:54:20.000000 Flask-Lib-0.2.3/README.md
+-rw-rw-rw-   0        0        0      798 2023-08-08 23:37:03.103482 Flask-Lib-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0       36 2023-05-09 00:43:43.000000 Flask-Lib-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 23:37:03.084592 Flask-Lib-0.2.3/src/
+drwxrwxrwx   0        0        0        0 2023-08-08 23:37:03.095562 Flask-Lib-0.2.3/src/Flask_Lib.egg-info/
+-rw-rw-rw-   0        0        0      698 2023-08-08 23:37:03.000000 Flask-Lib-0.2.3/src/Flask_Lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2023-08-08 23:37:03.000000 Flask-Lib-0.2.3/src/Flask_Lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 23:37:03.000000 Flask-Lib-0.2.3/src/Flask_Lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      291 2023-08-08 23:37:03.000000 Flask-Lib-0.2.3/src/Flask_Lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-08 23:37:03.000000 Flask-Lib-0.2.3/src/Flask_Lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-08 23:37:03.099820 Flask-Lib-0.2.3/src/flasklib/
+-rw-rw-rw-   0        0        0      218 2023-07-27 14:10:28.000000 Flask-Lib-0.2.3/src/flasklib/__init__.py
+-rw-rw-rw-   0        0        0     2840 2023-05-04 22:19:44.000000 Flask-Lib-0.2.3/src/flasklib/dates.py
+-rw-rw-rw-   0        0        0     1062 2023-05-04 22:19:44.000000 Flask-Lib-0.2.3/src/flasklib/errors.py
+-rw-rw-rw-   0        0        0      836 2023-05-09 00:44:22.000000 Flask-Lib-0.2.3/src/flasklib/jinja.py
+-rw-rw-rw-   0        0        0     1376 2023-05-04 01:27:16.000000 Flask-Lib-0.2.3/src/flasklib/json.py
+drwxrwxrwx   0        0        0        0 2023-08-08 23:37:03.100818 Flask-Lib-0.2.3/src/flasklib/mappers/
+-rw-rw-rw-   0        0        0      129 2023-05-04 01:41:47.000000 Flask-Lib-0.2.3/src/flasklib/mappers/__init__.py
+-rw-rw-rw-   0        0        0     1492 2023-07-27 15:25:17.000000 Flask-Lib-0.2.3/src/flasklib/mappers/mappers.py
+-rw-rw-rw-   0        0        0     1937 2023-05-04 22:19:44.000000 Flask-Lib-0.2.3/src/flasklib/responses.py
+-rw-rw-rw-   0        0        0      427 2023-05-04 22:19:44.000000 Flask-Lib-0.2.3/src/flasklib/startup.py
```

### Comparing `Flask-Lib-0.2.1/LICENSE` & `Flask-Lib-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-Lib-0.2.1/PKG-INFO` & `Flask-Lib-0.2.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: Flask-Lib
-Version: 0.2.1
+Version: 0.2.3
 Summary: Premade Flask tools to speed up development.
 Home-page: https://github.com/rrickgauer/Flask-Lib
 Author: Ryan Rickgauer
 Author-email: rrickgauer1@gmail.com
 License: UNKNOWN
 Description: # Flask-Lib
         Premade Flask tools to speed up development.
@@ -26,8 +26,8 @@
         * jinja
         * errors
         * mappers
         
         
         
 Platform: UNKNOWN
-Requires-Python: >=3.9.12
+Requires-Python: >=3.8
```

### Comparing `Flask-Lib-0.2.1/setup.cfg` & `Flask-Lib-0.2.3/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2046 6c61 736b 2d4c 6962 0d0a 7665   = Flask-Lib..ve
-00000020: 7273 696f 6e20 3d20 302e 322e 310d 0a64  rsion = 0.2.1..d
+00000020: 7273 696f 6e20 3d20 302e 322e 330d 0a64  rsion = 0.2.3..d
 00000030: 6573 6372 6970 7469 6f6e 203d 2050 7265  escription = Pre
 00000040: 6d61 6465 2046 6c61 736b 2074 6f6f 6c73  made Flask tools
 00000050: 2074 6f20 7370 6565 6420 7570 2064 6576   to speed up dev
 00000060: 656c 6f70 6d65 6e74 2e0d 0a61 7574 686f  elopment...autho
 00000070: 7220 3d20 5279 616e 2052 6963 6b67 6175  r = Ryan Rickgau
 00000080: 6572 0d0a 6175 7468 6f72 5f65 6d61 696c  er..author_email
 00000090: 203d 2072 7269 636b 6761 7565 7231 4067   = rrickgauer1@g
@@ -12,40 +12,39 @@
 000000b0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
 000000c0: 6f6d 2f72 7269 636b 6761 7565 722f 466c  om/rrickgauer/Fl
 000000d0: 6173 6b2d 4c69 620d 0a6c 6f6e 675f 6465  ask-Lib..long_de
 000000e0: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
 000000f0: 3a20 5245 4144 4d45 2e6d 640d 0a0d 0a5b  : README.md....[
 00000100: 6f70 7469 6f6e 735d 0d0a 7079 7468 6f6e  options]..python
 00000110: 5f72 6571 7569 7265 7320 3d20 3e3d 332e  _requires = >=3.
-00000120: 392e 3132 0d0a 7061 636b 6167 6573 203d  9.12..packages =
-00000130: 2066 696e 643a 0d0a 7061 636b 6167 655f   find:..package_
-00000140: 6469 7220 3d20 3d20 7372 630d 0a69 6e73  dir = = src..ins
-00000150: 7461 6c6c 5f72 6571 7569 7265 7320 3d20  tall_requires = 
-00000160: 0d0a 0962 6c69 6e6b 6572 203e 3d20 312e  ...blinker >= 1.
-00000170: 362e 320d 0a09 6365 7274 6966 6920 3e3d  6.2...certifi >=
-00000180: 2032 3032 322e 3132 2e37 0d0a 0963 6861   2022.12.7...cha
-00000190: 7273 6574 2d6e 6f72 6d61 6c69 7a65 7220  rset-normalizer 
-000001a0: 3e3d 2033 2e31 2e30 0d0a 0963 6c69 636b  >= 3.1.0...click
-000001b0: 203e 3d20 382e 312e 330d 0a09 636f 6c6f   >= 8.1.3...colo
-000001c0: 7261 6d61 203e 3d20 302e 342e 360d 0a09  rama >= 0.4.6...
-000001d0: 6461 6369 7465 203e 3d20 312e 382e 300d  dacite >= 1.8.0.
-000001e0: 0a09 646f 636f 7074 203e 3d20 302e 362e  ..docopt >= 0.6.
-000001f0: 320d 0a09 466c 6173 6b20 3e3d 2032 2e33  2...Flask >= 2.3
-00000200: 2e32 0d0a 0969 646e 6120 3e3d 2033 2e34  .2...idna >= 3.4
-00000210: 0d0a 0969 6d70 6f72 746c 6962 2d6d 6574  ...importlib-met
-00000220: 6164 6174 6120 3e3d 2036 2e36 2e30 0d0a  adata >= 6.6.0..
-00000230: 0969 7473 6461 6e67 6572 6f75 7320 3e3d  .itsdangerous >=
-00000240: 2032 2e31 2e32 0d0a 094a 696e 6a61 3220   2.1.2...Jinja2 
-00000250: 3e3d 2033 2e31 2e32 0d0a 094d 6172 6b75  >= 3.1.2...Marku
-00000260: 7053 6166 6520 3e3d 2032 2e31 2e32 0d0a  pSafe >= 2.1.2..
-00000270: 0972 6571 7565 7374 7320 3e3d 2032 2e33  .requests >= 2.3
-00000280: 302e 300d 0a09 7572 6c6c 6962 3320 3e3d  0.0...urllib3 >=
-00000290: 2032 2e30 2e32 0d0a 0957 6572 6b7a 6575   2.0.2...Werkzeu
-000002a0: 6720 3e3d 2032 2e33 2e33 0d0a 0979 6172  g >= 2.3.3...yar
-000002b0: 6720 3e3d 2030 2e31 2e39 0d0a 097a 6970  g >= 0.1.9...zip
-000002c0: 7020 3e3d 2033 2e31 352e 300d 0a0d 0a5b  p >= 3.15.0....[
-000002d0: 6f70 7469 6f6e 732e 7061 636b 6167 6573  options.packages
-000002e0: 2e66 696e 645d 0d0a 7768 6572 6520 3d20  .find]..where = 
-000002f0: 7372 630d 0a0d 0a5b 6567 675f 696e 666f  src....[egg_info
-00000300: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
-00000310: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
-00000320: 0a                                       .
+00000120: 380d 0a70 6163 6b61 6765 7320 3d20 6669  8..packages = fi
+00000130: 6e64 3a0d 0a70 6163 6b61 6765 5f64 6972  nd:..package_dir
+00000140: 203d 203d 2073 7263 0d0a 696e 7374 616c   = = src..instal
+00000150: 6c5f 7265 7175 6972 6573 203d 200d 0a09  l_requires = ...
+00000160: 626c 696e 6b65 7220 3e3d 2031 2e36 2e32  blinker >= 1.6.2
+00000170: 0d0a 0963 6572 7469 6669 203e 3d20 3230  ...certifi >= 20
+00000180: 3232 2e31 322e 370d 0a09 6368 6172 7365  22.12.7...charse
+00000190: 742d 6e6f 726d 616c 697a 6572 203e 3d20  t-normalizer >= 
+000001a0: 332e 312e 300d 0a09 636c 6963 6b20 3e3d  3.1.0...click >=
+000001b0: 2038 2e31 2e33 0d0a 0963 6f6c 6f72 616d   8.1.3...coloram
+000001c0: 6120 3e3d 2030 2e34 2e36 0d0a 0964 6163  a >= 0.4.6...dac
+000001d0: 6974 6520 3e3d 2031 2e38 2e30 0d0a 0964  ite >= 1.8.0...d
+000001e0: 6f63 6f70 7420 3e3d 2030 2e36 2e32 0d0a  ocopt >= 0.6.2..
+000001f0: 0946 6c61 736b 203e 3d20 322e 332e 320d  .Flask >= 2.3.2.
+00000200: 0a09 6964 6e61 203e 3d20 332e 340d 0a09  ..idna >= 3.4...
+00000210: 696d 706f 7274 6c69 622d 6d65 7461 6461  importlib-metada
+00000220: 7461 203e 3d20 362e 362e 300d 0a09 6974  ta >= 6.6.0...it
+00000230: 7364 616e 6765 726f 7573 203e 3d20 322e  sdangerous >= 2.
+00000240: 312e 320d 0a09 4a69 6e6a 6132 203e 3d20  1.2...Jinja2 >= 
+00000250: 332e 312e 320d 0a09 4d61 726b 7570 5361  3.1.2...MarkupSa
+00000260: 6665 203e 3d20 322e 312e 320d 0a09 7265  fe >= 2.1.2...re
+00000270: 7175 6573 7473 203e 3d20 322e 3330 2e30  quests >= 2.30.0
+00000280: 0d0a 0975 726c 6c69 6233 203e 3d20 322e  ...urllib3 >= 2.
+00000290: 302e 320d 0a09 5765 726b 7a65 7567 203e  0.2...Werkzeug >
+000002a0: 3d20 322e 332e 330d 0a09 7961 7267 203e  = 2.3.3...yarg >
+000002b0: 3d20 302e 312e 390d 0a09 7a69 7070 203e  = 0.1.9...zipp >
+000002c0: 3d20 332e 3135 2e30 0d0a 0d0a 5b6f 7074  = 3.15.0....[opt
+000002d0: 696f 6e73 2e70 6163 6b61 6765 732e 6669  ions.packages.fi
+000002e0: 6e64 5d0d 0a77 6865 7265 203d 2073 7263  nd]..where = src
+000002f0: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
+00000300: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
+00000310: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
```

### Comparing `Flask-Lib-0.2.1/src/Flask_Lib.egg-info/PKG-INFO` & `Flask-Lib-0.2.3/src/Flask_Lib.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: Flask-Lib
-Version: 0.2.1
+Version: 0.2.3
 Summary: Premade Flask tools to speed up development.
 Home-page: https://github.com/rrickgauer/Flask-Lib
 Author: Ryan Rickgauer
 Author-email: rrickgauer1@gmail.com
 License: UNKNOWN
 Description: # Flask-Lib
         Premade Flask tools to speed up development.
@@ -26,8 +26,8 @@
         * jinja
         * errors
         * mappers
         
         
         
 Platform: UNKNOWN
-Requires-Python: >=3.9.12
+Requires-Python: >=3.8
```

### Comparing `Flask-Lib-0.2.1/src/flasklib/dates.py` & `Flask-Lib-0.2.3/src/flasklib/dates.py`

 * *Files identical despite different names*

### Comparing `Flask-Lib-0.2.1/src/flasklib/errors.py` & `Flask-Lib-0.2.3/src/flasklib/errors.py`

 * *Files identical despite different names*

### Comparing `Flask-Lib-0.2.1/src/flasklib/jinja.py` & `Flask-Lib-0.2.3/src/flasklib/jinja.py`

 * *Files identical despite different names*

### Comparing `Flask-Lib-0.2.1/src/flasklib/json.py` & `Flask-Lib-0.2.3/src/flasklib/json.py`

 * *Files identical despite different names*

### Comparing `Flask-Lib-0.2.1/src/flasklib/mappers/mappers.py` & `Flask-Lib-0.2.3/src/flasklib/mappers/mappers.py`

 * *Files identical despite different names*

### Comparing `Flask-Lib-0.2.1/src/flasklib/responses.py` & `Flask-Lib-0.2.3/src/flasklib/responses.py`

 * *Files identical despite different names*

