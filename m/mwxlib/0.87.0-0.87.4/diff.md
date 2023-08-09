# Comparing `tmp/mwxlib-0.87.0-py3-none-any.whl.zip` & `tmp/mwxlib-0.87.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 164364 bytes, number of entries: 22
+Zip file size: 164459 bytes, number of entries: 22
 -rw-rw-rw-  2.0 fat     2514 b- defN 23-Jun-23 06:26 mwx/__init__.py
--rw-rw-rw-  2.0 fat    46456 b- defN 23-Jul-12 13:46 mwx/controls.py
--rw-rw-rw-  2.0 fat    73403 b- defN 23-Aug-02 13:07 mwx/framework.py
--rw-rw-rw-  2.0 fat    69312 b- defN 23-Aug-02 02:00 mwx/graphman.py
+-rw-rw-rw-  2.0 fat    46527 b- defN 23-Aug-09 04:55 mwx/controls.py
+-rw-rw-rw-  2.0 fat    73709 b- defN 23-Aug-09 04:55 mwx/framework.py
+-rw-rw-rw-  2.0 fat    69256 b- defN 23-Aug-09 04:55 mwx/graphman.py
 -rw-rw-rw-  2.0 fat    49957 b- defN 23-Jul-11 09:28 mwx/images.py
 -rw-rw-rw-  2.0 fat    36006 b- defN 23-Jul-13 01:15 mwx/matplot2.py
 -rw-rw-rw-  2.0 fat    66355 b- defN 23-Jul-31 01:16 mwx/matplot2g.py
 -rw-rw-rw-  2.0 fat    28267 b- defN 23-Jul-13 01:15 mwx/matplot2lg.py
 -rw-rw-rw-  2.0 fat     6878 b- defN 23-Feb-21 08:50 mwx/mgplt.py
--rw-rw-rw-  2.0 fat   138504 b- defN 23-Aug-02 03:38 mwx/nutshell.py
--rw-rw-rw-  2.0 fat    37560 b- defN 23-Aug-02 03:37 mwx/utilus.py
+-rw-rw-rw-  2.0 fat   138523 b- defN 23-Aug-09 04:55 mwx/nutshell.py
+-rw-rw-rw-  2.0 fat    37560 b- defN 23-Aug-02 14:08 mwx/utilus.py
 -rw-rw-rw-  2.0 fat    11238 b- defN 23-Aug-01 15:56 mwx/wxmon.py
 -rw-rw-rw-  2.0 fat    19529 b- defN 23-Jul-13 01:23 mwx/wxpdb.py
 -rw-rw-rw-  2.0 fat     5552 b- defN 23-Aug-01 15:56 mwx/wxwil.py
 -rw-rw-rw-  2.0 fat     8314 b- defN 23-Aug-01 15:51 mwx/wxwit.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-23 14:06 mwx/py/__init__.py
 -rw-rw-rw-  2.0 fat    16794 b- defN 23-Jun-19 10:27 mwx/py/filling.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Aug-02 13:20 mwxlib-0.87.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1893 b- defN 23-Aug-02 13:20 mwxlib-0.87.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-02 13:20 mwxlib-0.87.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 23-Aug-02 13:20 mwxlib-0.87.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1609 b- defN 23-Aug-02 13:20 mwxlib-0.87.0.dist-info/RECORD
-22 files, 621328 bytes uncompressed, 161862 bytes compressed:  73.9%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Aug-09 04:57 mwxlib-0.87.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1893 b- defN 23-Aug-09 04:57 mwxlib-0.87.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-09 04:57 mwxlib-0.87.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 23-Aug-09 04:57 mwxlib-0.87.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1609 b- defN 23-Aug-09 04:57 mwxlib-0.87.4.dist-info/RECORD
+22 files, 621668 bytes uncompressed, 161957 bytes compressed:  73.9%
```

## zipnote {}

```diff
@@ -45,23 +45,23 @@
 
 Filename: mwx/py/__init__.py
 Comment: 
 
 Filename: mwx/py/filling.py
 Comment: 
 
-Filename: mwxlib-0.87.0.dist-info/LICENSE
+Filename: mwxlib-0.87.4.dist-info/LICENSE
 Comment: 
 
-Filename: mwxlib-0.87.0.dist-info/METADATA
+Filename: mwxlib-0.87.4.dist-info/METADATA
 Comment: 
 
-Filename: mwxlib-0.87.0.dist-info/WHEEL
+Filename: mwxlib-0.87.4.dist-info/WHEEL
 Comment: 
 
-Filename: mwxlib-0.87.0.dist-info/top_level.txt
+Filename: mwxlib-0.87.4.dist-info/top_level.txt
 Comment: 
 
-Filename: mwxlib-0.87.0.dist-info/RECORD
+Filename: mwxlib-0.87.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mwx/controls.py

```diff
@@ -939,19 +939,20 @@
 
 def Iconify(icon, w, h):
     ## if wx.VERSION >= (4,1,0):
     try:
         import wx.svg
         import requests
         url = "https://api.iconify.design/{}.svg".format(icon.replace(':', '/'))
-        content = requests.get(url).content
-        img = wx.svg.SVGimage.CreateFromBytes(content)
+        res = requests.get(url, timeout=3.0)
+        img = wx.svg.SVGimage.CreateFromBytes(res.content)
         bmp = img.ConvertToScaledBitmap(wx.Size(w, h))
         return bmp
     except Exception:
+        print("- Failed to load iconify.design/{}".format(icon))
         pass
 
 
 def _Icon(v):
     if isinstance(v, (str, bytes)):
         return Icon(v)
     if isinstance(v, wx.lib.embeddedimage.PyEmbeddedImage):
```

## mwx/framework.py

```diff
@@ -1,14 +1,14 @@
 #! python3
 # -*- coding: utf-8 -*-
 """mwxlib framework
 
 Author: Kazuya O'moto <komoto@jeol.co.jp>
 """
-__version__ = "0.87.0"
+__version__ = "0.87.4"
 __author__ = "Kazuya O'moto <komoto@jeol.co.jp>"
 
 from functools import wraps, partial
 from importlib import reload
 import traceback
 import builtins
 import datetime
@@ -808,18 +808,22 @@
             org = self.CurrentPage
             if j != self.Selection:
                 self.Selection = j # the focus is moved
             if wnd and wnd is not org: # restore focus other window
                 wnd.SetFocus()
     
     def get_caption(self, win):
+        """Get caption of tab/page for specifiend window."""
         tab, page = self.find_tab(win)
         return page.caption
     
     def set_caption(self, win, caption):
+        """Set caption of tab/page for specifiend window.
+        Returns True if the caption has changed.
+        """
         tab, page = self.find_tab(win)
         if page.caption != caption:
             page.caption = caption
             tab.Refresh()
             return True
     
     def find_tab(self, win):
@@ -855,14 +859,18 @@
     
     ## Methods to save / load the perspectives.
     ## *** Inspired by wx.lib.agw.aui.AuiNotebook ***
     
     def savePerspective(self):
         """Saves the entire user interface layout into an encoded string,
         which can then be stored by the application.
+        
+        Note:
+            Perspectives are saved according to page.window.Name.
+            User should give it (not page.caption) a unique name.
         """
         for j, pane in enumerate(self.all_panes):
             pane.name = f"pane{j+1}"
         spec = ""
         for j, tabs in enumerate(self.all_tabs):
             k = next(k for k, page in enumerate(tabs.Pages)
                                    if page.window.Shown) # get active window
@@ -873,16 +881,16 @@
     
     ## Note: Should be called after all pages have been added.
     @postcall
     def loadPerspective(self, spec):
         """Loads a saved perspective.
         
         Note:
-            This function will be called after the session is loaded.
-            At that point, some pages may be missing.
+            Perspectives are loaded after the session is resumed.
+            At that point, some user-cusotm pages may be missing.
         """
         tabs, frames = spec.split('@')
         tabinfo = re.findall(r"pane\w+?=(.*?);(.*?)\|", tabs)
         try:
             self.Parent.Freeze()
             ## Collapse all tabs to main tabctrl
             maintab = self.all_tabs[0]
@@ -1441,15 +1449,15 @@
                 break
             j = nb.GetPageIndex(win) # find and select page
             if j != -1:
                 if j != nb.Selection:
                     nb.Selection = j # the focus is moved
                 break
         else:
-            return # no such pane.windows
+            return # no such pane.window
         
         if show is None:
             show = not pane.IsShown() # toggle show
         
         if focus and win.IsShown():
             win.SetFocus() # move focus
         elif wnd:
@@ -1485,41 +1493,39 @@
     def _load(self, filename, lineno, book, verbose=False):
         """Load file in the session (internal use only)."""
         try:
             if isinstance(book, str):
                 book = getattr(self, book)
         except AttributeError:
             return False
-        
-        if re.match(r"https?://[\w/:%#$&?()~.=+-]+", filename): # url_re
-            return book.load_url(filename, lineno, verbose)
-        else:
-            return book.load_file(filename, lineno, verbose)
+        return book.load_file(filename, lineno, verbose)
     
-    def load(self, filename, lineno=0):
+    def load(self, filename, lineno=0, show=True, focus=False):
         """Load file @where the object is defined.
         
         Args:
             filename : target filename:str or object.
                        It also supports <'filename:lineno'> format.
             lineno   : Set mark to lineno on load.
+            show     : Show the book.
+            focus    : Focus the window if visible.
         """
         if not isinstance(filename, str):
             filename = where(filename)
             if filename is None:
                 return False
         if not lineno:
             m = re.match("(.*?):([0-9]+)", filename)
             if m:
                 filename, ln = m.groups()
                 lineno = int(ln)
         book = next((x for x in self.all_books
                         if x.find_buffer(filename)), self.Log)
         if self._load(filename, lineno, book, verbose=1):
-            self.popup_window(book, focus=0)
+            self.popup_window(book, show, focus)
     
     def info(self, obj):
         self.rootshell.info(obj)
     
     def help(self, obj):
         self.rootshell.help(obj)
```

## mwx/graphman.py

```diff
@@ -200,15 +200,15 @@
         unloadable  : flag to set the Layer to be unloadable
     
     Note:
         parent <Frame> is not always equal to Parent when floating.
         Parent type can be <Frame>, <AuiFloatingFrame>, or <AuiNotebook>.
     """
     MENU = "Plugins" # default menu for Plugins
-    menukey = property(lambda self: "{}/&{}".format(self.MENU, self.__module__))
+    menukey = "Plugins/"
     caption = True
     category = None
     dockable = True
     editable = True # to be deprecated
     reloadable = True
     unloadable = True
```

## mwx/nutshell.py

```diff
@@ -1421,36 +1421,33 @@
     
     @filename.setter
     def filename(self, f):
         if f and os.path.isfile(f):
             self.__mtime = os.path.getmtime(f)
         else:
             self.__mtime = None
-        try:
-            renamed = (self.__filename != f)
-        except AttributeError:
-            renamed = False
-        self.__filename = f
-        if renamed:
+        if self.__filename != f:
+            self.__filename = f
             self.parent.handler('buffer_filename_reset', self)
+            self.update_caption()
     
     @property
     def mtdelta(self):
         """Timestamp delta (for checking external mod).
         
         Returns:
             None : No file
             = 0  : a file
             > 0  : a file edited externally
             < 0  : a url file
         """
         f = self.filename
         if f and os.path.isfile(f):
             return os.path.getmtime(f) - self.__mtime
-        elif f and re.match(url_re, f):
+        if f and re.match(url_re, f):
             return -1
     
     @property
     def caption_prefix(self):
         prefix = ''
         dt = self.mtdelta
         if dt is not None:
@@ -1466,17 +1463,16 @@
     
     @property
     def caption(self):
         return self.caption_prefix + self.name
     
     def update_caption(self):
         try:
-            if self.mtdelta is not None:
-                if self.parent.set_caption(self, self.caption):
-                    self.parent.handler('buffer_caption_reset', self)
+            if self.parent.set_caption(self, self.caption):
+                self.parent.handler('buffer_caption_reset', self)
         except AttributeError:
             pass
     
     @property
     def need_buffer_save(self):
         """Returns whether the buffer should be saved.
         The file has been modified internally.
@@ -1501,14 +1497,15 @@
     post_command_hook.__name__ = str('post_command_dispatch') # alias
     
     def __init__(self, parent, filename=None, **kwargs):
         EditWindow.__init__(self, parent, **kwargs)
         EditorInterface.__init__(self)
         
         self.parent = parent
+        self.__filename = filename
         self.filename = filename
         self.code = None
         
         self.Bind(stc.EVT_STC_UPDATEUI, self.OnUpdate) # skip to brace matching
         
         self.Bind(stc.EVT_STC_INDICATOR_CLICK, self.OnIndicatorClick)
         
@@ -1617,29 +1614,25 @@
         self.message("ESC {}".format(evt.key))
         self.AnnotationClearAll()
     
     ## --------------------------------
     ## File I/O
     ## --------------------------------
     
-    def _load_textfile(self, text, filename, lineno=0):
+    def _load_textfile(self, text, filename):
         with self.off_readonly():
             self.Text = text
             self.EmptyUndoBuffer()
             self.SetSavePoint()
-        self.markline = lineno - 1
-        self.goto_marker(1)
         self.filename = filename
         self.handler('buffer_loaded', self)
     
-    def _load_file(self, filename, lineno=0):
+    def _load_file(self, filename):
         """Wrapped method of LoadFile."""
         if self.LoadFile(filename):
-            self.markline = lineno - 1
-            self.goto_marker(1)
             self.filename = filename
             self.EmptyUndoBuffer()
             self.SetSavePoint()
             self.handler('buffer_loaded', self)
             return True
         return False
     
@@ -1897,17 +1890,29 @@
     @property
     def buffer(self):
         """Returns the currently selected page or None."""
         return self.CurrentPage
     
     def find_buffer(self, f):
         """Find buffer with specified f:filename or code."""
-        for buf in self.all_buffers:
-            if f is buf or f in buf or f == buf.filename: # check code
-                return buf
+        if isinstance(f, str):
+            g = os.path.realpath(f)
+            for buf in self.all_buffers:
+                if f == buf.filename or g == os.path.realpath(buf.filename):
+                    return buf
+        else:
+            for buf in self.all_buffers:
+                if f is buf or f in buf: # check code
+                    return buf
+    
+    def swap_buffer(self, buf, lineno=0):
+        self.swap_page(buf)
+        if lineno:
+            buf.markline = lineno - 1
+            buf.goto_marker(1)
     
     def create_buffer(self, filename, index=None):
         """Create a new buffer (internal use only)."""
         try:
             self.Freeze()
             buf = Buffer(self, filename)
             self.set_attributes(buf, **self.defaultBufferStyle)
@@ -1956,87 +1961,87 @@
     ## File I/O
     ## --------------------------------
     wildcards = [
         "PY files (*.py)|*.py",
         "ALL files (*.*)|*.*",
     ]
     
-    def load_url(self, url, lineno=0, verbose=True):
-        if verbose:
-            surl = re.sub(r"(https?://.+?)/(.+)/(.+)", r"\1 ... \3", url)
-            if wx.MessageBox( # Confirm URL load.
-                    "You are loading URL contents.\n\n"
-                    "Continue loading?",
-                    "Load {!r}".format(surl),
-                    style=wx.YES_NO|wx.ICON_INFORMATION) != wx.YES:
-                self.post_message("The load has been canceled.")
-                return None
-        try:
-            import requests
-            res = requests.get(url)
-        except Exception as e:
-            self.post_message("Failed to load URL: {}".format(e))
-            return None
-        if res.status_code == 200: # success
-            buf = self.find_buffer(url) or self.create_buffer(url)
-            buf._load_textfile(res.text, url, lineno)
-            self.swap_page(buf)
-            return True
-        return False
-    
     def load_cache(self, filename, lineno=0):
         """Load a file from cache using linecache.
         Note:
             The filename should be an absolute path.
             The buffer will be reloaded without confirmation.
         """
         linecache.checkcache(filename)
         lines = linecache.getlines(filename)
         if lines:
-            buf = self.find_buffer(filename) or self.create_buffer(filename)
-            buf._load_textfile(''.join(lines), filename, lineno)
-            self.swap_page(buf)
+            buf = self.find_buffer(filename)
+            if not buf:
+                buf = self.create_buffer(filename)
+            elif not buf.need_buffer_load:
+                self.swap_buffer(buf, lineno)
+                return True
+            buf._load_textfile(''.join(lines), filename)
+            self.swap_buffer(buf, lineno)
             return True
         return False
     
     def load_file(self, filename, lineno=0, verbose=True):
         """Load a file into an existing or new buffer.
         """
-        buf = self.find_buffer(filename) or self.create_buffer(filename)
-        if buf.need_buffer_save and verbose:
+        buf = self.find_buffer(filename)
+        if not buf:
+            buf = self.create_buffer(filename)
+        elif buf.need_buffer_save and verbose:
             if wx.MessageBox( # Confirm load.
                     "You are leaving unsaved content.\n\n"
                     "The changes will be discarded.\n"
                     "Continue loading?",
                     "Load {!r}".format(buf.name),
                     style=wx.YES_NO|wx.ICON_INFORMATION) != wx.YES:
                 self.post_message("The load has been canceled.")
                 return None
+        elif not buf.need_buffer_load:
+            self.swap_buffer(buf, lineno)
+            return True
         try:
+            ## busy = wx.BusyInfo("One moment please.\n"
+            ##                    "Loading {!r}...".format(filename))
             self.Freeze()
             org = self.buffer
-            if buf._load_file(buf.filename, lineno):
-                self.swap_page(buf)
-                return True
-            return False
+            if re.match(url_re, filename):
+                import requests
+                res = requests.get(filename, timeout=3.0)
+                if res.status_code == requests.codes.ok:
+                    buf._load_textfile(res.text, filename)
+                    self.swap_buffer(buf, lineno)
+                    return True
+                return False
+            else:
+                if buf._load_file(buf.filename):
+                    self.swap_buffer(buf, lineno)
+                    return True
+                return False
         except Exception as e:
             self.post_message("Failed to load {!r}: {}".format(buf.name, e))
             self.delete_buffer(buf)
             if org:
-                self.swap_page(org)
+                self.swap_buffer(org)
             return False
         finally:
             self.Thaw()
     
+    load_url = load_file # for backward compatibility
+    
     def save_file(self, filename, buf=None, verbose=True):
         """Save the current buffer to a file.
         """
         buf = buf or self.buffer
         if buf.need_buffer_load and verbose:
-            self.swap_page(buf)
+            self.swap_buffer(buf)
             if wx.MessageBox( # Confirm save.
                     "The file has been modified externally.\n\n"
                     "The contents of the file will be overwritten.\n"
                     "Continue saving?",
                     "Save {!r}".format(buf.name),
                     style=wx.YES_NO|wx.ICON_INFORMATION) != wx.YES:
                 self.post_message("The save has been canceled.")
@@ -2057,18 +2062,16 @@
         dt = buf.mtdelta
         if dt is None:
             self.post_message("No filename.")
             return None
         elif dt == 0 and not buf.IsModified():
             self.post_message("No need to load.")
             return None
-        elif dt < 0:
-            return self.load_url(buf.filename, buf.markline+1)
         else:
-            return self.load_file(buf, buf.markline+1)
+            return self.load_file(buf.filename, buf.markline+1)
     
     def save_buffer(self, buf=None):
         """Confirm the save with the dialog."""
         buf = buf or self.buffer
         dt = buf.mtdelta
         if dt is None:
             self.post_message("No filename.")
```

## Comparing `mwxlib-0.87.0.dist-info/LICENSE` & `mwxlib-0.87.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mwxlib-0.87.0.dist-info/METADATA` & `mwxlib-0.87.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwxlib
-Version: 0.87.0
+Version: 0.87.4
 Summary: A wrapper of matplotlib and wxPython (phoenix)
 Home-page: https://github.com/komoto48g/mwxlib
 Author: Kazuya O'moto <komoto@jeol.co.jp>
 Author-email: komoto@jeol.co.jp
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `mwxlib-0.87.0.dist-info/RECORD` & `mwxlib-0.87.4.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 mwx/__init__.py,sha256=6vaRq60B9cLrnsiaoytM9JAIheZvDs2R1Kqv3I9rf3g,2514
-mwx/controls.py,sha256=YZwCw-LgEvtBL58SahDn1vI7KLgsGiPBQZTbfRSw_L4,46456
-mwx/framework.py,sha256=o4M47czsN1lEpNQxD9R-80o1McuR2pOcRPi2Fp0xOhs,73403
-mwx/graphman.py,sha256=iJb1kHM_vCuoz7KE4uZl5EH1_yKDeO9ynf8pncAbAek,69312
+mwx/controls.py,sha256=QmdDwm2RUVTfbFToQQZwYBfxnWVX3xLPXrOr-umaDUw,46527
+mwx/framework.py,sha256=1BdnUZ9O8lRMGIeDHJLCB-VTgVRSFsap5WEtZ60zbuE,73709
+mwx/graphman.py,sha256=Wf05SNXKCVGJJ4VsRZmFIxl0dJwV42LsFeHdSStKGzQ,69256
 mwx/images.py,sha256=mrnUYH12I3XLVSZcEXlpVltX0XMxufbl2yRvDIQJZqc,49957
 mwx/matplot2.py,sha256=7fe9yJqyK57dOX4oFsR-_1eLejOfG4hy0sH042iaPvE,36006
 mwx/matplot2g.py,sha256=JY1VUl2jpnkQ69WT2VRga1eLj6Bgf0gXb1myPE_ey_M,66355
 mwx/matplot2lg.py,sha256=sBLGYxUn-7bVoZ-x9Fik3VSPHcoTZxboO3j-Cjgo89o,28267
 mwx/mgplt.py,sha256=49_wpFZUEKErQmtobqrlNKDjWlAsdLft-izlqSyGPD0,6878
-mwx/nutshell.py,sha256=01y0pKhjkAMPheZNe5M0s_iwcH0lsiJXtzNO19jlBBs,138504
+mwx/nutshell.py,sha256=xs9z7nfYPQUwZSHuChqyydh7J8gSCg1BWGeU-2I3Nes,138523
 mwx/utilus.py,sha256=jx2sNwtVfJCm_HM_ZWhJwEvxPc2goiAAEEmj1Y02RJ4,37560
 mwx/wxmon.py,sha256=Y1ClT4c1kNl-59JyCHtxGa5LIX_c6v7ozehGxXMq3k4,11238
 mwx/wxpdb.py,sha256=Qtrd87IS_HQQFcpL-VHYNG21OiTORoglzq3vKNJHVjk,19529
 mwx/wxwil.py,sha256=_DPLd_6bEgQf4CGBUJqYyM31-KAczUj6heQOWUg8Dgc,5552
 mwx/wxwit.py,sha256=G_86UM-99fPq7s8aiYoTXS1TiEWiFV9PbtgUfbrEmT4,8314
 mwx/py/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mwx/py/filling.py,sha256=f6KMBcBv7gwrl6qmJYLTL-O0Z47bWNAdTCZtUZIo8vM,16794
-mwxlib-0.87.0.dist-info/LICENSE,sha256=PGtRKCaTkmUDlBQwpptJAxJtdqxIUtAmdBsaT9nUVkA,1091
-mwxlib-0.87.0.dist-info/METADATA,sha256=YITiwBHn7A53QHCrYw2709TCuxknKH5E8-61Nnp0Y8k,1893
-mwxlib-0.87.0.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-mwxlib-0.87.0.dist-info/top_level.txt,sha256=SI1Mh118AstnUFGPNq5aMNKiAnVNmZk1S9Ij-OwAEpY,4
-mwxlib-0.87.0.dist-info/RECORD,,
+mwxlib-0.87.4.dist-info/LICENSE,sha256=PGtRKCaTkmUDlBQwpptJAxJtdqxIUtAmdBsaT9nUVkA,1091
+mwxlib-0.87.4.dist-info/METADATA,sha256=Zx_lgfyc2kEOk9HwM_htwNtHa_QnsQtYYYsT4KG_atg,1893
+mwxlib-0.87.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+mwxlib-0.87.4.dist-info/top_level.txt,sha256=SI1Mh118AstnUFGPNq5aMNKiAnVNmZk1S9Ij-OwAEpY,4
+mwxlib-0.87.4.dist-info/RECORD,,
```

