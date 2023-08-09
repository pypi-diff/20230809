# Comparing `tmp/swiftbat-0.1.4.tar.gz` & `tmp/swiftbat-0.1a15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftbat-0.1.4.tar", last modified: Wed Aug  9 01:11:57 2023, max compression
+gzip compressed data, was "swiftbat-0.1a15.tar", last modified: Sun Jan 23 01:33:33 2022, max compression
```

## Comparing `swiftbat-0.1.4.tar` & `swiftbat-0.1a15.tar`

### file list

```diff
@@ -1,27 +1,22 @@
-drwxr-xr-x   0 palmer   (34507)      501        0 2023-08-09 01:11:57.487509 swiftbat-0.1.4/
--rw-r--r--   0 palmer   (34507)      501     2920 2022-05-21 16:44:28.000000 swiftbat-0.1.4/LICENSE
--rw-r--r--   0 palmer   (34507)      501     2641 2023-08-09 01:11:57.487157 swiftbat-0.1.4/PKG-INFO
--rw-r--r--   0 palmer   (34507)      501     1961 2022-05-21 16:44:28.000000 swiftbat-0.1.4/README.md
--rw-r--r--   0 palmer   (34507)      501       38 2023-08-09 01:11:57.487625 swiftbat-0.1.4/setup.cfg
--rw-r--r--   0 palmer   (34507)      501     4005 2023-08-09 01:11:22.000000 swiftbat-0.1.4/setup.py
-drwxr-xr-x   0 palmer   (34507)      501        0 2023-08-09 01:11:57.483333 swiftbat-0.1.4/swiftbat/
--rw-r--r--   0 palmer   (34507)      501     2545 2023-08-09 00:33:15.000000 swiftbat-0.1.4/swiftbat/__init__.py
--rw-r--r--   0 palmer   (34507)      501     6304 2023-08-09 00:33:15.000000 swiftbat-0.1.4/swiftbat/batcatalog.py
--rw-r--r--   0 palmer   (34507)      501   245000 2022-05-21 16:44:28.000000 swiftbat-0.1.4/swiftbat/catalog
--rw-r--r--   0 palmer   (34507)      501     7893 2023-08-09 00:33:15.000000 swiftbat-0.1.4/swiftbat/clockinfo.py
--rw-r--r--   0 palmer   (34507)      501    15556 2023-08-09 00:33:15.000000 swiftbat-0.1.4/swiftbat/generaldir.py
--rw-r--r--   0 palmer   (34507)      501    27260 2023-08-09 00:33:15.000000 swiftbat-0.1.4/swiftbat/recent_bcttb.fits.gz
--rw-r--r--   0 palmer   (34507)      501     6892 2023-08-09 00:33:15.000000 swiftbat-0.1.4/swiftbat/sfmisc.py
--rwxr-xr-x   0 palmer   (34507)      501    50377 2023-08-09 00:33:15.000000 swiftbat-0.1.4/swiftbat/swinfo.py
--rwxr-xr-x   0 palmer   (34507)      501    16734 2023-08-09 00:33:15.000000 swiftbat-0.1.4/swiftbat/swutil.py
-drwxr-xr-x   0 palmer   (34507)      501        0 2023-08-09 01:11:57.485500 swiftbat-0.1.4/swiftbat.egg-info/
--rw-r--r--   0 palmer   (34507)      501     2641 2023-08-09 01:11:57.000000 swiftbat-0.1.4/swiftbat.egg-info/PKG-INFO
--rw-r--r--   0 palmer   (34507)      501      468 2023-08-09 01:11:57.000000 swiftbat-0.1.4/swiftbat.egg-info/SOURCES.txt
--rw-r--r--   0 palmer   (34507)      501        1 2023-08-09 01:11:57.000000 swiftbat-0.1.4/swiftbat.egg-info/dependency_links.txt
--rw-r--r--   0 palmer   (34507)      501       55 2023-08-09 01:11:57.000000 swiftbat-0.1.4/swiftbat.egg-info/entry_points.txt
--rw-r--r--   0 palmer   (34507)      501       69 2023-08-09 01:11:57.000000 swiftbat-0.1.4/swiftbat.egg-info/requires.txt
--rw-r--r--   0 palmer   (34507)      501        9 2023-08-09 01:11:57.000000 swiftbat-0.1.4/swiftbat.egg-info/top_level.txt
-drwxr-xr-x   0 palmer   (34507)      501        0 2023-08-09 01:11:57.486656 swiftbat-0.1.4/tests/
--rw-r--r--   0 palmer   (34507)      501     1003 2023-08-09 00:33:15.000000 swiftbat-0.1.4/tests/testclock.py
--rw-r--r--   0 palmer   (34507)      501     1568 2023-08-09 00:33:15.000000 swiftbat-0.1.4/tests/testswinfo.py
--rw-r--r--   0 palmer   (34507)      501     1426 2023-08-09 00:33:15.000000 swiftbat-0.1.4/tests/testxy.py
+drwxr-xr-x   0 tparsota (291073623) staff       (20)        0 2022-01-23 01:33:33.640972 swiftbat-0.1a15/
+-rw-r--r--   0 tparsota (291073623) staff       (20)     2920 2022-01-17 22:40:55.000000 swiftbat-0.1a15/LICENSE
+-rw-r--r--   0 tparsota (291073623) staff       (20)     2577 2022-01-23 01:33:33.640772 swiftbat-0.1a15/PKG-INFO
+-rw-r--r--   0 tparsota (291073623) staff       (20)     1961 2022-01-17 22:40:55.000000 swiftbat-0.1a15/README.md
+-rw-r--r--   0 tparsota (291073623) staff       (20)       38 2022-01-23 01:33:33.641045 swiftbat-0.1a15/setup.cfg
+-rw-r--r--   0 tparsota (291073623) staff       (20)     3788 2022-01-23 01:32:47.000000 swiftbat-0.1a15/setup.py
+drwxr-xr-x   0 tparsota (291073623) staff       (20)        0 2022-01-23 01:33:33.638794 swiftbat-0.1a15/swiftbat/
+-rw-r--r--   0 tparsota (291073623) staff       (20)     2540 2022-01-17 22:40:55.000000 swiftbat-0.1a15/swiftbat/__init__.py
+-rw-r--r--   0 tparsota (291073623) staff       (20)     6305 2022-01-23 01:26:47.000000 swiftbat-0.1a15/swiftbat/batcatalog.py
+-rw-r--r--   0 tparsota (291073623) staff       (20)   245000 2022-01-17 22:40:55.000000 swiftbat-0.1a15/swiftbat/catalog
+-rw-r--r--   0 tparsota (291073623) staff       (20)     8112 2022-01-23 01:26:47.000000 swiftbat-0.1a15/swiftbat/clockinfo.py
+-rw-r--r--   0 tparsota (291073623) staff       (20)    14752 2022-01-23 01:26:47.000000 swiftbat-0.1a15/swiftbat/generaldir.py
+-rw-r--r--   0 tparsota (291073623) staff       (20)    26834 2022-01-17 22:40:55.000000 swiftbat-0.1a15/swiftbat/recent_bcttb.fits.gz
+-rwxr-xr-x   0 tparsota (291073623) staff       (20)    57445 2022-01-23 01:26:47.000000 swiftbat-0.1a15/swiftbat/swinfo.py
+-rwxr-xr-x   0 tparsota (291073623) staff       (20)    15187 2022-01-17 22:40:55.000000 swiftbat-0.1a15/swiftbat/swutil.py
+drwxr-xr-x   0 tparsota (291073623) staff       (20)        0 2022-01-23 01:33:33.640467 swiftbat-0.1a15/swiftbat.egg-info/
+-rw-r--r--   0 tparsota (291073623) staff       (20)     2577 2022-01-23 01:33:33.000000 swiftbat-0.1a15/swiftbat.egg-info/PKG-INFO
+-rw-r--r--   0 tparsota (291073623) staff       (20)      394 2022-01-23 01:33:33.000000 swiftbat-0.1a15/swiftbat.egg-info/SOURCES.txt
+-rw-r--r--   0 tparsota (291073623) staff       (20)        1 2022-01-23 01:33:33.000000 swiftbat-0.1a15/swiftbat.egg-info/dependency_links.txt
+-rw-r--r--   0 tparsota (291073623) staff       (20)       49 2022-01-23 01:33:33.000000 swiftbat-0.1a15/swiftbat.egg-info/entry_points.txt
+-rw-r--r--   0 tparsota (291073623) staff       (20)       40 2022-01-23 01:33:33.000000 swiftbat-0.1a15/swiftbat.egg-info/requires.txt
+-rw-r--r--   0 tparsota (291073623) staff       (20)        9 2022-01-23 01:33:33.000000 swiftbat-0.1a15/swiftbat.egg-info/top_level.txt
```

### Comparing `swiftbat-0.1.4/LICENSE` & `swiftbat-0.1a15/LICENSE`

 * *Files identical despite different names*

### Comparing `swiftbat-0.1.4/PKG-INFO` & `swiftbat-0.1a15/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: swiftbat
-Version: 0.1.4
+Version: 0.1a15
 Summary: Routines for dealing with data from BAT on the Neil Gehrels Swift Observatory
 Home-page: https://github.com/lanl/swiftbat_python/
-Download-URL: https://github.com/lanl/swiftbat_python/archive/refs/tags/v0.1.4.tar.gz
 Author: David M. Palmer
 Author-email: palmer@lanl.gov
 License: BSD-3-Clause
-Classifier: Development Status :: 4 - Beta
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Astronomy
-Requires-Python: >=3.9
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Swiftbat is a set of Python library routines and command-line utilities that have been developed for the purpose
 of retrieving, analyzing, and displaying data from NASA's Swift spacecraft, especially the data from the
 Swift Burst Alert Telescope (BAT). Development started before the launch of Swift for private use by the
 author and was how he learned Python. As a result, it is not a well-packaged, well-written, coherent library.
@@ -49,7 +49,9 @@
 Obs Date and Times:           2020-05-05   12:32:37 - 13:01:34
 Obs Pointing(ra,dec,roll):    293.724, 21.897, 62.77
 Cyg_X-1_imageloc (boresight_dist, angle): (14, -133)
 Cyg_X-1_exposure (cm^2 cos adjusted): 4230
 Cyg_X-1_altitude: 29 (up)
 ```
 Use `swinfo --help` for more details.
+
+
```

### Comparing `swiftbat-0.1.4/README.md` & `swiftbat-0.1a15/README.md`

 * *Files identical despite different names*

### Comparing `swiftbat-0.1.4/setup.py` & `swiftbat-0.1a15/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-copyright = """
+copyright="""
 Copyright (c) 2018, Triad National Security, LLC. All rights reserved.
  
 This program was produced under U.S. Government contract
 89233218CNA000001 for Los Alamos National Laboratory (LANL),
 which is operated by Triad National Security, LLC for the U.S.
 Department of Energy/National Nuclear Security Administration.
 
@@ -24,43 +24,31 @@
 3.       Neither the name of Triad National Security, LLC, Los Alamos National Laboratory, LANL, the U.S. Government, nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
  
 THIS SOFTWARE IS PROVIDED BY TRIAD NATIONAL SECURITY, LLC AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL TRIAD NATIONAL SECURITY, LLC OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """
 
 try:
-    with open("README.md", "r") as f:
+    with open("README.md", 'r') as f:
         long_description = f.read()
 except FileNotFoundError:
-    long_description = ""
+    long_description = ''
 
 setup(
-    name="swiftbat",
-    version="0.1.4",
-    packages=["swiftbat"],
-    package_data={"": ["catalog", "recent_bcttb.fits.gz"]},
-    url="https://github.com/lanl/swiftbat_python/",
-    download_url="https://github.com/lanl/swiftbat_python/archive/refs/tags/v0.1.4.tar.gz",
-    license="BSD-3-Clause",
-    author="David M. Palmer",
-    author_email="palmer@lanl.gov",
-    description="Routines for dealing with data from BAT on the Neil Gehrels Swift Observatory",
+    name='swiftbat',
+    version='0.1a15',
+    packages=['swiftbat'],
+    package_data={'':['catalog', 'recent_bcttb.fits.gz']},
+    url='https://github.com/lanl/swiftbat_python/',
+    license='BSD-3-Clause',
+    author='David M. Palmer',
+    author_email='palmer@lanl.gov',
+    description='Routines for dealing with data from BAT on the Neil Gehrels Swift Observatory',
     long_description=long_description,
-    long_description_content_type="text/markdown",
-    entry_points={"console_scripts": ["swinfo=swiftbat.swinfo:swinfo_main"]},
-    install_requires=[
-        "astropy>=5",
-        "astroquery",
-        "numpy",
-        "python-dateutil",
-        "skyfield>=1.4",
-        "swifttools",
-    ],
-    classifiers=[
-        "Development Status :: 4 - Beta",
-        "Intended Audience :: Science/Research",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 3",
-        "Topic :: Scientific/Engineering :: Astronomy",
-    ],
-    python_requires=">=3.9",
+    long_description_content_type='text/markdown',
+    entry_points={'console_scripts': ['swinfo=swiftbat.swinfo:main']},
+    install_requires = ['beautifulsoup4', 'ephem', 'astropy', 'astroquery'],
+    classifiers=['Development Status :: 3 - Alpha', 'Intended Audience :: Science/Research', 'Programming Language :: Python',
+        'Programming Language :: Python :: 3',
+        'Topic :: Scientific/Engineering :: Astronomy', ],
+    python_requires='>=3.6',
 )
```

### Comparing `swiftbat-0.1.4/swiftbat/__init__.py` & `swiftbat-0.1a15/swiftbat/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,13 +13,13 @@
 2.       Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 3.       Neither the name of Triad National Security, LLC, Los Alamos National Laboratory, LANL, the U.S. Government, nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 
 THIS SOFTWARE IS PROVIDED BY TRIAD NATIONAL SECURITY, LLC AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL TRIAD NATIONAL SECURITY, LLC OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """
 
-from .sfmisc import sftime, sfts, loadsfephem
+from __future__ import print_function, division, absolute_import
+
 from .clockinfo import utcf
 from .swutil import *
 from .swinfo import *
 from .batcatalog import BATCatalog
-from . import generaldir
```

### Comparing `swiftbat-0.1.4/swiftbat/batcatalog.py` & `swiftbat-0.1a15/swiftbat/batcatalog.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,20 +21,20 @@
 
 """
 
 from functools import lru_cache
 from astropy.io import fits
 import numpy as np
 from pathlib import Path
-from swiftbat import simbadlocation
+from swiftbat import simbadnames, simbadlocation
 import re
 
 
-class BATCatalog:
-    filebasename = "recent_bcttb.fits.gz"
+class BATCatalog():
+    filebasename = 'recent_bcttb.fits.gz'
     thisdir = Path(__file__).parent
 
     def __init__(self, catalogfilename=None):
         self.cattable = self._cattable(catalogfilename=catalogfilename)
         self.makeindices()
 
     def __getitem__(self, item):
@@ -82,44 +82,42 @@
                 pass
             raise e  # The KeyError, even though the last failure was by simbadmatch
 
         # IMPROVEME: Go to SIMBAD and resolve the source, get its position, and find BAT source near that
 
     def simbadmatch(self, item, tolerance=0.2):
         """
-        What rows match the catalogued
-        :param item:
-        :param tolerance:
-        :return:
+        What rows match the catalogued 
+        :param item: 
+        :param tolerance: 
+        :return: 
         """
         ra, dec = simbadlocation(item)
         return self.positionmatch(ra, dec, tolerance)
 
     def positionmatch(self, radeg, decdeg, tolerance=0.2):
         rascale = np.cos(np.deg2rad(decdeg))
-        tol2 = tolerance**2
-        raoff = (
-            (self.cattable["RA_OBJ"] - radeg) + 180
-        ) % 360 - 180  # Handle the 360-0 wrap
-        dist2 = (raoff * rascale) ** 2 + (self.cattable["DEC_OBJ"] - decdeg) ** 2
+        tol2 = tolerance ** 2
+        raoff = (((self.cattable['RA_OBJ'] - radeg) + 180) % 360 - 180)  # Handle the 360-0 wrap
+        dist2 = (raoff * rascale) ** 2 + (self.cattable['DEC_OBJ'] - decdeg) ** 2
         return self.cattable[dist2 < tol2]
 
     def allnames(self):
-        return set([row["NAME"] for row in self.cattable if row["NAME"]])
+        return set([row['NAME'] for row in self.cattable if row['NAME']])
 
     def makeindices(self):
         self.bycatnum = {}
         self.byname = {}
         self.bysimplename = {}
         for row in self.cattable:
-            if not row["CATNUM"]:
+            if not row['CATNUM']:
                 continue
-            self.bycatnum.setdefault(row["CATNUM"], []).append(row)
-            self.byname.setdefault(row["NAME"], []).append(row)
-            self.bysimplename.setdefault(self.simplename(row["NAME"]), []).append(row)
+            self.bycatnum.setdefault(row['CATNUM'], []).append(row)
+            self.byname.setdefault(row['NAME'], []).append(row)
+            self.bysimplename.setdefault(self.simplename(row['NAME']), []).append(row)
 
     @lru_cache(maxsize=0)
     def _cattable(self, catalogfilename=None):
         # Recent catalog file e.g.
         # wget https://heasarc.gsfc.nasa.gov/FTP/swift/data/trend/2021_05/bat/bcatalog/sw03110986012bcttb.fits.gz -O recent_bcttb.fits.gz
         # Currently  2021_09  0654020283
         if catalogfilename is None:
@@ -130,8 +128,8 @@
     def simplename(self, name):
         """
         A simple name is the alphanumerics of the name in lower case.
         This folds + and - dec designations, but in practice not a problem
         :param name:
         :return:
         """
-        return re.sub("[^a-z0-9]", "", name.lower())
+        return re.sub('[^a-z0-9]', '', name.lower())
```

### Comparing `swiftbat-0.1.4/swiftbat/catalog` & `swiftbat-0.1a15/swiftbat/catalog`

 * *Files identical despite different names*

### Comparing `swiftbat-0.1.4/swiftbat/generaldir.py` & `swiftbat-0.1a15/swiftbat/generaldir.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 #! /usr/bin/env python
 
+from __future__ import print_function, division, absolute_import
+
 """
 generaldir:
 Treat http, ftp, and local files equally as a general directory structure
 Requires that the http server be apache with autoindex.
 The ftp requirements are that the dir listing begin with the flags and end with the name
 
 David Palmer   palmer@lanl.gov
@@ -15,21 +17,20 @@
 import os
 from urllib.request import urlopen
 import re
 import shutil
 import stat
 
 
-def subTemplate(
-    origstring, keydict, allcaps=True
-):  # if string includes '${FOO}' and keydict['FOO'] defined, substitute
+def subTemplate(origstring, keydict,
+                allcaps=True):  # if string includes '${FOO}' and keydict['FOO'] defined, substitute
     # The Template class in Python 2.4 would be the better way to do it, except that 2.4 was released yesterday (11/30/04)
     # If allcaps is true, the keys of keydict must be all caps, although the ${foo} need not be
     s = origstring
-    found = re.compile(r"""\$\{([^}]+)\}""").findall(s)
+    found = re.compile(r'''\$\{([^}]+)\}''').findall(s)
     # print(s," found ",found)
     for v in found:
         if allcaps:
             vu = v.upper()
         else:
             vu = v
         try:
@@ -39,38 +40,33 @@
         except:
             print("replace of ${%s} failed" % v)
             raise
     return s
 
 
 class generalDir:
-    _rewildsplitter = re.compile(
-        r"""(?P<unwild>(/*[^$/]+[/]+)*)(?P<firstwild>[^/]*)/*(?P<restwild>.*)"""
-    )
+    _rewildsplitter = re.compile(r'''(?P<unwild>(/*[^$/]+[/]+)*)(?P<firstwild>[^/]*)/*(?P<restwild>.*)''')
 
     def __init__(self, url):
         self.url = url
         self.lastsubpath = None
         self.lastreadout = None
 
     def getMatches(self, subpath, reg):
-        return re.compile(reg).findall(self.gettext(subpath))
-
-    def gettext(self, subpath):
-        return self.getdata(subpath).decode("utf8")
+        return re.compile(reg).findall(self.get(subpath))
 
-    def getdata(self, subpath):
+    def get(self, subpath):
         if self.lastsubpath != subpath or self.lastreadout == None:
             # Cache value so that when we request both files and dirs, only one net trans. made
             self.lastsubpath = subpath
-            self.lastreadout = self.openSub(subpath).read()
+            self.lastreadout = self.openSub(subpath).read().decode('utf-8')
         return self.lastreadout
 
-    def exists(self, subpath=""):
-        """Check if referenced object exists by trying to open it"""
+    def exists(self, subpath=''):
+        """ Check if referenced object exists by trying to open it """
         try:
             o = self.openSub(subpath)
             o.close()
             return True
         except:
             return False
 
@@ -83,242 +79,197 @@
             print("Unexpected error:", sys.exc_info()[0])
             print(self.url + "/" + subpath)
             raise
 
     def makeDirectoryForFile(self, fname):
         try:
             os.makedirs(os.path.dirname(fname))
-        except FileExistsError:
+        except:
             pass  # catch exception thrown when dir already present
 
     def copyToFile(self, subpath, fname):
         self.makeDirectoryForFile(fname)
-        shutil.copyfileobj(
-            self.openSub(subpath), open(fname, "wb")
-        )  # order is src, dest
+        shutil.copyfileobj(self.openSub(subpath), open(fname, "wb"))  # order is src, dest
 
     def matchPath(self, subpath, wildpath, matchdict=None, regexdict=None):
-        """given a subpath and a wildcard path, with named values and
+        """ given a subpath and a wildcard path, with named values and
         regular expressions in matchdict and regexdict, find directories that match
         the pattern and the pattern matched as a list of tuples (path, matchingdict)
         """
         # print("subpath = ",subpath)
-        if subpath == None:
-            subpath = ""
-        (unwild, firstwild, restwild) = self._splitAndSub(
-            wildpath, matchdict, regexdict
-        )
+        if subpath == None: subpath = ''
+        (unwild, firstwild, restwild) = self._splitAndSub(wildpath, matchdict, regexdict)
         # print("join (%s,%s)" % (subpath,unwild))
         subpath = os.path.join(subpath, unwild)  # Add the non-wild stuff to the subpath
         # print("->",subpath)
-        if not self.exists(
-            subpath
-        ):  # if the unwild stuff doesn't exist then this is a dead end
+        if not self.exists(subpath):  # if the unwild stuff doesn't exist then this is a dead end
             # print("Deadend : %s / %s" % (self.url,subpath))
             return []
         if not firstwild:  # if there is no wild part
-            assert not restwild  # there must not be any more wild part
+            assert (not restwild)  # there must not be any more wild part
             # we already checked for existence, so this is a good match
             return [(subpath, matchdict.copy())]
         else:  # There is still some wildness left
             results = []
             matchstring = subTemplate(firstwild, regexdict)
             if -1 != matchstring.find("$"):
-                print(
-                    "Did not substitute variable regular expression in %s" % matchstring
-                )
-                raise RuntimeError(
-                    "Did not substitute variable regular expression in %s" % matchstring
-                )
-            dirmatchre = re.compile(
-                matchstring + "/*$"
-            )  # optional / allowed for directory
+                print("Did not substitute variable regular expression in %s" % matchstring)
+                raise RuntimeError("Did not substitute variable regular expression in %s" % matchstring)
+            dirmatchre = re.compile(matchstring + "/*$")  # optional / allowed for directory
             dirlist = self.dirs(subpath)
             # print("in",subpath,"trying to match string",matchstring,"against",dirlist)
             # print("wildness remaining:",restwild)
             for d in dirlist:
                 m = dirmatchre.match(d)
                 if m:  # d matches the first wild bit
                     newsubpath = os.path.join(subpath, d)
                     # print("adding",d,"to get",newsubpath)
-                    md = (
-                        matchdict.copy()
-                    )  # don't disturb original from one recursion level up
+                    md = matchdict.copy()  # don't disturb original from one recursion level up
                     md.update(m.groupdict())  # add newly discovered variables
                     if restwild:  # more to match
-                        results.extend(
-                            self.matchPath(newsubpath, restwild, md, regexdict)
-                        )
+                        results.extend(self.matchPath(newsubpath, restwild, md, regexdict))
                     else:  # nothing more
                         results.append((newsubpath, md))
             if not restwild:  # If there is no more wildness, then match might be a file
                 filelist = self.files(subpath)
                 filematchre = re.compile(matchstring + "$")  # ending slash is forbidden
                 for f in filelist:
                     m = filematchre.match(f)
                     if m:  # file match
                         newsubpath = os.path.join(subpath, f)
-                        md = (
-                            matchdict.copy()
-                        )  # don't disturb original from one recursion level up
+                        md = matchdict.copy()  # don't disturb original from one recursion level up
                         md.update(m.groupdict())  # add newly discovered variables
                         results.append((newsubpath, md))
             return results
 
     def _splitAndSub(self, wildpath, matchdict, regexdict):
-        """returns a (topUNwildpath, firstwildness, restofwildpath) tuple with matches and regexes subbed in"""
+        """ returns a (topUNwildpath, firstwildness, restofwildpath) tuple with matches and regexes subbed in """
         wildpath = subTemplate(wildpath, matchdict)  # Do all the matching you can
         if -1 == wildpath.find("$"):
-            return (wildpath, "", "")
+            return (wildpath, '', '')
         m = self._rewildsplitter.match(wildpath)
         # print(wildpath+"-->",m.groupdict())
-        if not m or (not m.groupdict()["firstwild"] and m.groupdict()["restwild"]):
+        if not m or (not m.groupdict()['firstwild'] and m.groupdict()['restwild']):
             # no match if totally non-wild and unslashed.  Not /-terminated, but handled above
-            assert False
-            assert -1 == wildpath.find("$")
-            return (wildpath, "", "")
-        return (
-            m.groupdict()["unwild"],
-            m.groupdict()["firstwild"],
-            m.groupdict()["restwild"],
-        )
+            assert (False)
+            assert (-1 == wildpath.find("$"))
+            return (wildpath, '', '')
+        return (m.groupdict()['unwild'], m.groupdict()['firstwild'], m.groupdict()['restwild'])
 
 
 class httpDir(generalDir):
-    """HTTP specialization for the directory generalization
+    """ HTTP specialization for the directory generalization
     Works on apache servers with autoindex generation
     A directory is read by reading from its URL with a trailing /.  (Reading without
     a trailing slash gives a redirection that this lib can't follow.)  In the
     text that comes out, subdirectories and files are represented by links where
     the href is the name (with a trailing slash for subdirs.) with the close quotes,
     close angle brackets, and then a repetition of the name (likewise with the trailing /
     for dirs), except the name is truncated if it is too long.   In Swift, filenames
     can be long, but directory names are short enough to not be truncated.
-
+    
     This can be fixed by adding ?F=0  (fancy listing off) to the end of the URL.  See
     http://httpd.apache.org/docs-2.0/mod/mod_autoindex.html
     """
-
     # 2008-06-30 added star to " " because some HTTP servers do not put a space in front
-    dirmatch = re.compile(
-        r"""(?P<foundname>[^\?"/]+)/"> *(?P=foundname)/""", re.MULTILINE | re.IGNORECASE
-    )
-    filematch = re.compile(
-        r"""(?P<foundname>[^\?"/]+)"> *(?P=foundname)""", re.MULTILINE | re.IGNORECASE
-    )
+    dirmatch = re.compile(r'''(?P<foundname>[^\?"/]+)/"> *(?P=foundname)/''', re.MULTILINE | re.IGNORECASE)
+    filematch = re.compile(r'''(?P<foundname>[^\?"/]+)"> *(?P=foundname)''', re.MULTILINE | re.IGNORECASE)
     # And some servers do not evevn understand the /?F=0 non-fancy readout
-    filenofancymatch = re.compile(
-        r"""HREF="(?P<foundname>[^\?"/]+)">""", re.MULTILINE | re.IGNORECASE
-    )
+    filenofancymatch = re.compile(r'''HREF="(?P<foundname>[^\?"/]+)">''', re.MULTILINE | re.IGNORECASE)
 
-    validurlmatch = re.compile("https?://", re.IGNORECASE)
+    # FIXME allow https
+    validurlmatch = re.compile("http://", re.IGNORECASE)
 
     def __init__(self, url):
         if not self.validurlmatch.search(url):
             raise RuntimeError("Not an http url: %s" % url)
         generalDir.__init__(self, url)
         self.filecache = {}
         self.dircache = {}
         # print("HTTP works on %s", url)
 
     def files(self, subdir=""):
         try:
             return self.filecache[subdir]
         except:
-            files = self.getMatches(subdir + "/?F=0", self.filematch)
+            files = self.getMatches(subdir + '/?F=0', self.filematch)
             self.filecache[subdir] = files
             return files
 
     def filesNoFancy(self, subdir=""):  #
-        files = self.getMatches(subdir + "/?F=0", self.filenofancymatch)
+        files = self.getMatches(subdir + '/?F=0', self.filenofancymatch)
         return files
 
     def dirs(self, subdir=""):
         try:
             return self.dircache[subdir]
         except:
-            dirs = self.getMatches(subdir + "/?F=0", self.dirmatch)
+            dirs = self.getMatches(subdir + '/?F=0', self.dirmatch)
             self.dircache[subdir] = dirs
             return dirs
 
     def getFullPath(self, urlrelativepathname):
         return os.path.join(self.url, urlrelativepathname)
 
 
 class ftpDir(generalDir):
-    _filelinematch = re.compile(
-        r"""(?<=^-[r-][w-].[r-][w-].r..\s).+$""", re.MULTILINE | re.IGNORECASE
-    )
-    _dirlinematch = re.compile(
-        r"""(?<=^d[r-][w-].[r-][w-].r..\s).+$""", re.MULTILINE | re.IGNORECASE
-    )
+    _filelinematch = re.compile(r'''(?<=^-[r-][w-].[r-][w-].r..\s).+$''', re.MULTILINE | re.IGNORECASE)
+    _dirlinematch = re.compile(r'''(?<=^d[r-][w-].[r-][w-].r..\s).+$''', re.MULTILINE | re.IGNORECASE)
     _namematch = re.compile("\S+\s*$")  # last string of nonwhite characters before eol
 
     def __init__(self, url):
         if not re.compile("ftp://", re.IGNORECASE).search(url):
             raise RuntimeError("Not a valid ftp url: %s" % url)
         generalDir.__init__(self, url)
 
     def files(self, subdir=""):
-        lines = self.getMatches(subdir + "/", self._filelinematch)
+        lines = self.getMatches(subdir + '/', self._filelinematch)
         return [self._namematch.findall(l.strip())[0] for l in lines]
 
     def dirs(self, subdir=""):
-        lines = self.getMatches(subdir + "/", self._dirlinematch)
+        lines = self.getMatches(subdir + '/', self._dirlinematch)
         return [self._namematch.findall(l.strip())[0] for l in lines]
 
 
 class localDir(generalDir):
     def __init__(self, url):
         # print("Trying %s as local file" % url)
-        nofileurl = re.compile(r"""(?<=FILE://)([^>]*)""", re.IGNORECASE).findall(url)
+        nofileurl = re.compile(r'''(?<=FILE://)([^>]*)''', re.IGNORECASE).findall(url)
         if len(nofileurl):
             self.dirname = os.path.realpath(nofileurl[0])
         else:
             self.dirname = os.path.realpath(url)
         generalDir.__init__(self, "FILE://" + self.dirname)
 
     def dirs(self, subdir=""):
         d = os.path.join(self.dirname, subdir)
         # IMPROVEME  use os.scandir for python >= 3.5
-        if hasattr(os, "scandir"):
+        if hasattr(os, 'scandir'):
             # Python >= 3.5
-            return [
-                x.name for x in os.scandir("/Volumes/DATA/Swift/swift") if x.is_dir()
-            ]
+            return [x.name for x in os.scandir('/Volumes/DATA/Swift/swift') if x.is_dir()]
         else:
             allindir = os.listdir(d)
             # FIXME chokes on aliases or links to files that don't exist
             # IMPROVEME  use os.path.isdir
-            return [
-                x
-                for x in allindir
-                if stat.S_ISDIR(os.stat(os.path.join(d, x))[stat.ST_MODE])
-            ]
+            return [x for x in allindir if stat.S_ISDIR(os.stat(os.path.join(d, x))[stat.ST_MODE])]
 
     def files(self, subdir=""):
         d = os.path.join(self.dirname, subdir)
-        if hasattr(os, "scandir"):
+        if hasattr(os, 'scandir'):
             # Python >= 3.5
-            return [
-                x.name for x in os.scandir("/Volumes/DATA/Swift/swift") if x.is_file()
-            ]
+            return [x.name for x in os.scandir('/Volumes/DATA/Swift/swift') if x.is_file()]
         else:
             allindir = os.listdir(d)
-            return [
-                x
-                for x in allindir
-                if stat.S_ISREG(os.stat(os.path.join(d, x))[stat.ST_MODE])
-            ]
+            return [x for x in allindir if stat.S_ISREG(os.stat(os.path.join(d, x))[stat.ST_MODE])]
 
     def openSub(self, subpath):
         open(os.path.join(self.dirname, subpath))
 
-    def exists(self, subpath=""):
-        """Check if referenced object exists by trying to open it"""
+    def exists(self, subpath=''):
+        """ Check if referenced object exists by trying to open it """
         try:
             # print("does %s exist?" % os.path.join(self.dirname,subpath))
             mode = os.stat(os.path.join(self.dirname, subpath))[stat.ST_MODE]
         except:
             # print("No")
             # print(os.stat(os.path.join(self.dirname,subpath)))
             return False
@@ -326,16 +277,16 @@
             # print("Yes")
             return True
         else:
             # print("Not as a file or directory")
             return False
 
     def makedirs(self, subpath):
-        """No analog method or HTTP and FTP genDirectories.
-        Make the entire string of directories to the given subpath"""
+        """ No analog method or HTTP and FTP genDirectories.
+        Make the entire string of directories to the given subpath """
         try:
             os.makedirs(os.path.join(self.dirname, subpath))
         except:
             pass
 
     def getFullPath(self, urlrelativepathname):
         return os.path.join(self.dirname, urlrelativepathname)
@@ -355,52 +306,44 @@
     d = getDir(url)
     if d:
         dirs = d.dirs()
         files = d.files()
         instring = ("%%%0is" % indent) % " "
         print(instring, "%s:" % url)
         instring += "    "
-        if len(files):
-            print(instring, files)
+        if len(files): print(instring, files)
         if depth > 0:
             for subdir in dirs:
                 dive(url + "/" + subdir, depth - 1, indent + 4)
         elif len(dirs):
             print(instring, "D:", dirs)
 
 
 def main():
-    regexdict = {
-        "SEQNUM": "(?P<SEQNUM>[0-9][0-9][0-9][0-9][0-9][0-9][0-9][0-9][0-9][0-9][0-9])",
-        "OBSERVATORY": "(?P<OBSERVATORY>sw)",
-        "VERSION": "(?P<VERSION>[0-9][0-9][0-9])",
-        "TYPE": "(?P<TYPE>\\W+)",
-        "CODINGSUFFIXES": "(?P<CODINGSUFFIXES>(.gz|.pgp)*)",
-    }
-    for url in (
-        "https://heasarc.gsfc.nasa.gov/FTP/swift/data/",
-        "https://heasarc.gsfc.nasa.gov/FTP/swift/data/obs/2005_04",
-        # 'http://swift.gsfc.nasa.gov/SDC/data/local/data1/data', # Previous location of quicklook
-        # 'https://swift.gsfc.nasa.gov/data/swift/'  # No longer works (gives a page instead of a dir listing)
-    ):
+    regexdict = {'SEQNUM': '(?P<SEQNUM>[0-9][0-9][0-9][0-9][0-9][0-9][0-9][0-9][0-9][0-9][0-9])',
+                 'OBSERVATORY': '(?P<OBSERVATORY>sw)', 'VERSION': '(?P<VERSION>[0-9][0-9][0-9])',
+                 'TYPE': '(?P<TYPE>\\W+)', 'CODINGSUFFIXES': '(?P<CODINGSUFFIXES>(.gz|.pgp)*)'}
+    for url in ('http://heasarc.gsfc.nasa.gov/FTP/swift/data/',
+                'http://heasarc.gsfc.nasa.gov/FTP/swift/data/obs/2005_04',
+                'http://swift.gsfc.nasa.gov/SDC/data/local/data1/data'):
         print(url)
         archive = getDir(url)
         print("----------------")
-        dirpaths = archive.matchPath("", "(sw)?${seqnum}(.${version})?", {}, regexdict)
+        dirpaths = archive.matchPath('', '(sw)?${seqnum}(.${version})?', {}, regexdict)
         print("----------------")
-        for obsdir, d in dirpaths:
-            print(obsdir, d["SEQNUM"], d["VERSION"])
+        for (obsdir, d) in dirpaths:
+            print(obsdir, d['SEQNUM'], d['VERSION'])
     print("----------------")
     # print(archdir.matchPath("","sw${seqnum}.${version}",{},cache.regexdict))
     # print(archdir.matchPath("","sw${seqnum}.023"+"/"+cache.typepatterns['pob.cat']+'${CODINGSUFFIXES}',{},cache.regexdict))
     # print(archdir.matchPath("",cache.hierdict['DIRPATTERN']+"/"+cache.typepatterns['pob.cat']+'${CODINGSUFFIXES}',{},cache.regexdict))
     if len(sys.argv) <= 1:
         # dive("http://swift.gsfc.nasa.gov/SDC/data/local/data1/data/", 2)
         # dive("file:///tmp", 3)
-        # dive("ftp://anonymous:palmer%40lanl.gov@heasarc.gsfc.nasa.gov/swift/data/", 2)
+        # dive("ftp://anonymous:palmer%40lanl.gov@legacy.gsfc.nasa.gov/swift/data/", 2)
         # print(swiftCache()
         pass
     else:
         dive(sys.argv[1], 2)
 
 
 if __name__ == "__main__":
```

### Comparing `swiftbat-0.1.4/swiftbat/swinfo.py` & `swiftbat-0.1a15/swiftbat/swinfo.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 #! /usr/bin/env python
 
+
+from __future__ import print_function, division, absolute_import
+
+import functools
+from pathlib import Path
+
 """
 swinfo
 More utilities for dealing with Swift Data
 David Palmer   palmer@lanl.gov
 
 
 """
@@ -30,59 +36,68 @@
 2.       Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 3.       Neither the name of Triad National Security, LLC, Los Alamos National Laboratory, LANL, the U.S. Government, nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
  
 THIS SOFTWARE IS PROVIDED BY TRIAD NATIONAL SECURITY, LLC AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL TRIAD NATIONAL SECURITY, LLC OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """
 
-
 import os
 import sys
-import functools
-from pathlib import Path
+
+# add the path of this module to the searchpath to let helpers in
+execdir = os.path.dirname(os.path.abspath(os.path.realpath(__file__)))
+if not execdir in map(os.path.abspath, sys.path):
+    sys.path.append(execdir)
+
 import re
 import datetime
 import shutil
+
 import glob
 import gzip
 import traceback
 import getopt
 import time
-from . import swutil
-from .clockinfo import utcf
-from . import sftime, sfts, loadsfephem
+import math
+from swiftbat import swutil
+from swiftbat.clockinfo import utcf
 import astropy.units as u
 from astropy.io import fits
 from astropy import coordinates
-from astropy.coordinates import ICRS, SkyCoord, Angle as apAngle
 import numpy as np
+
 from io import StringIO
-from functools import lru_cache as __lru_cache
-import swifttools.swift_too as swto
+
+# Running into certificate problems from 2018-10-23 for
+# https://stackoverflow.com/questions/27835619/urllib-and-ssl-certificate-verify-failed-error
+
+import ssl
+
+unsafe_context = ssl._create_unverified_context()
+
 from urllib.request import urlopen, quote
 from swiftbat import generaldir
-import skyfield.api as sf_api
-from skyfield.trigonometry import position_angle_of as sf_position_angle_of
-from skyfield.positionlib import ICRF as sf_ICRF
-import sqlite3  # Good sqlite3 tutorial at http://www.w3schools.com/sql/default.asp
-from typing import List, Tuple
-
+import bs4 as BeautifulSoup
+import ephem
 
+import sqlite3  # Good sqlite3 tutorial at http://www.w3schools.com/sql/default.asp
 split_translate = str.maketrans("][, \t;", "      ")
-# Skyfield interfaces
-_sf_load = sf_api.Loader("~/.skyfield", verbose=False)
-_sf_ts = _sf_load.timescale(builtin=True)
-
 
-@__lru_cache(0)
-def loadsfephem():
-    return _sf_load("de421.bsp")
 
 
-_sf_timescale = sf_api.load.timescale(builtin=True)
+# Pointings database (as opposed to an observations database) has two tables, 'pointings' and 'days'
+# pdbfile = os.path.join(swiftcache.theCache.params['LOCAL'][0],"pointings.db")
+pdbfile = '/Volumes/Data/Swift/swift/pointings.db'
+pdbfields_text = '''time_begin text unique primary key, time_end text, seqnum text, target_name text, ra_pnt real, dec_pnt real, roll_pnt real, asflown boolean'''
+pdbfields = [s.split() for s in pdbfields_text.split(',')]
+pdbfieldnames = [s[0] for s in pdbfields]
+
+pdbdayfields_text = '''date text unique primary key, asflown_complete boolean, asflow_partial boolean, preplanned boolean'''
+pdbdayfields = [s.split() for s in pdbdayfields_text.split(',')]
+pdbdayfieldnames = [s[0] for s in pdbdayfields]
 
 
 def adapt_boolean(bol):
     if bol:
         return "True"
     else:
         return "False"
@@ -96,98 +111,90 @@
     else:
         raise ValueError("Unknown value of bool attribute '%s'" % bolStr)
 
 
 sqlite3.register_adapter(bool, adapt_boolean)
 sqlite3.register_converter("boolean", convert_boolean)
 
-execdir = os.path.dirname(os.path.abspath(os.path.realpath(__file__)))
-
 basecatalog = os.path.join(execdir, "catalog")
 fitscatalog = os.path.join(execdir, "recent_bcttb.fits.gz")
 # FIXME should be handled by dotswift
 catalogdir = "/opt/data/Swift/analysis/sourcelist"
 newcatalogfile = os.path.join(catalogdir, "newcatalog")
-cataloglist = [
-    os.path.join(catalogdir, "trumpcatalog"),
-    os.path.join(catalogdir, "grbcatalog"),
-    os.path.join(catalogdir, "catalog"),
-    newcatalogfile,
-]
-
+cataloglist = [os.path.join(catalogdir, "trumpcatalog"),
+               os.path.join(catalogdir, "grbcatalog"),
+               os.path.join(catalogdir, "catalog"),
+               newcatalogfile]
+
+earthradius_m = 6378100.0  # meters
+r2d = 180 / 3.1415926  # this should be somewhere
+atm_thickness = 100e3  # How deep in the atmosphere you should report attenuation
 
 # define machineReadable=False
 
+
+asflownURLpattern = "http://www.swift.psu.edu/operations/obsSchedule.php?d=%Y-%m-%d&a=1"
+preplannedURLpattern = "http://www.swift.psu.edu/operations/obsSchedule.php?d=%Y-%m-%d&a=0"
+
 ydhms = "%Y-%j-%H:%M:%S"
 
 # TLEpattern = ["ftp://heasarc.gsfc.nasa.gov/swift/data/obs/%Y_%m/",".*","auxil","SWIFT_TLE_ARCHIVE.*.gz"]
-TLEpattern = [
-    "http://heasarc.gsfc.nasa.gov/FTP/swift/data/obs/%Y_%m/",
-    ".*",
-    "auxil",
-    "SWIFT_TLE_ARCHIVE.*.gz",
-]
+TLEpattern = ["http://heasarc.gsfc.nasa.gov/FTP/swift/data/obs/%Y_%m/", ".*", "auxil", "SWIFT_TLE_ARCHIVE.*.gz"]
 
 tlefile = "/tmp/latest_swift_tle.gz"
 tlebackup = os.path.expanduser("~/.swift/recent_swift_tle.gz")
 
-radecnameRE = re.compile(r"""^(?P<rastring>[0-9.]+)_+(?P<decstring>([-+]*[0-9.]+))$""")
+radecnameRE = re.compile(r'''^(?P<rastring>[0-9.]+)_+(?P<decstring>([-+]*[0-9.]+))$''')
 
-ipntimeRE = re.compile(
-    r"""'(?P<mission>[^']+)'\s*'(?P<d>[ 0-9]+)/(?P<m>[ 0-9]+)/(?P<y>[ 0-9]+)'\s+(?P<s>[0-9.]+)"""
-)
+ipntimeRE = re.compile(r"""'(?P<mission>[^']+)'\s*'(?P<d>[ 0-9]+)/(?P<m>[ 0-9]+)/(?P<y>[ 0-9]+)'\s+(?P<s>[0-9.]+)""")
 
+_maxobslength = datetime.timedelta(minutes=90)
 
 verbose = False  # Verbose controls diagnositc output
 terse = False  # Terse controls the format of ordinary output
 
 
 # Old fashioned
 def simbadnames(query):
     """Given a source name, or other SIMBAD query, generates a list of identifier matches
-    See http://simbad.u-strasbg.fr/simbad/sim-fscript
+       See http://simbad.u-strasbg.fr/simbad/sim-fscript
     """
-    url_ = urlopen(
-        """http://simbad.u-strasbg.fr/simbad/sim-script?submit=submit+script&script=format+object+%%22+%%25IDLIST%%22%%0D%%0Aquery++%s"""
-        % (quote(query),),
-        None,
-        60,
-    )
+    u = urlopen(
+        """http://simbad.u-strasbg.fr/simbad/sim-script?submit=submit+script&script=format+object+%%22+%%25IDLIST%%22%%0D%%0Aquery++%s""" % (
+            quote(query),), None, 60)
     names = []
-    while url_:
-        l = url_.readline().decode()
+    while u:
+        l = u.readline().decode()
         if re.match("""^::error::*""", l):
             raise ValueError(query)
         if re.match("""^::data::*""", l):
             break
-    for l in url_.readlines():
+    for l in u.readlines():
         s = l.decode().strip().split()
         if len(s) > 0:
-            if s[0] == "NAME":
+            if s[0] == 'NAME':
                 s = s[1:]
             names.append(" ".join(s))
     return names
 
 
 # Astroquery
 def simbadlocation(objectname):
     """
-    Location according to
-    :param objectname:
+    Location according to 
+    :param objectname: 
     :return: (ra_deg, dec_deg)
     """
     from astroquery.simbad import Simbad
-
     try:
         table = Simbad.query_object(objectname)
         if len(table) != 1:
             raise RuntimeError(f"No unique match for {objectname}")
-        co = coordinates.SkyCoord(
-            table["RA"][0], table["DEC"][0], unit=(u.hour, u.deg), frame="fk5"
-        )
+        co = coordinates.SkyCoord(table['RA'][0], table['DEC'][0],
+                                  unit=(u.hour, u.deg), frame='fk5')
         return (co.ra.degree, co.dec.degree)
     except Exception as e:
         raise RuntimeError(f"{e}")
 
 
 class orbit:
     def __init__(self):
@@ -197,99 +204,81 @@
         # TLE in this case is Two Line Element, not 3
         global verbose
         if verbose:
             print("Updating TLE")
         self.updateTLE()
         if verbose:
             print("Reading TLE from %s" % (tlefile))
-        allTLE = gzip.open(
-            tlefile, "rt" if sys.version_info.major == 3 else "r"
-        ).readlines()
+        allTLE = gzip.open(tlefile, "rt" if sys.version_info.major == 3 else "r").readlines()
         # Some TLE files seem to have additional blank lines
         # Actually, what they have is \r\n in some cases and \n in others
         # Nevertheless, put this in in case they change the format
         allTLE = [l.strip() for l in allTLE if len(l.strip()) == 69]
         nTLE = len(allTLE) // 2
-        self._tleByTime = [
-            (
-                datetime.datetime(2000 + int(allTLE[2 * i][18:20]), 1, 1, 0, 0, 0)
-                + datetime.timedelta(float(allTLE[2 * i][20:32]) - 1),
-                ("Swift", allTLE[2 * i], allTLE[2 * i + 1]),
-            )
-            for i in range(nTLE)
-        ]
+        self._tleByTime = [(datetime.datetime(2000 + int(allTLE[2 * i][18:20]), 1, 1, 0, 0, 0)
+                            + datetime.timedelta(float(allTLE[2 * i][20:32]) - 1),
+                            ("Swift", allTLE[2 * i], allTLE[2 * i + 1]))
+                           for i in range(nTLE)]
+        # for (ttle,tle) in self._tleByTime :
+        #    print ("%s" %ttle)
         self.pickTLE(datetime.datetime.utcnow())
+        self._earthcenter = ephem.Observer()
+        self._earthcenter.lat = 0.0
+        self._earthcenter.long = 0.0
+        self._earthcenter.elev = -6378137.0  # equatorial radius of WGS84
+        self._earthcenter.date = ephem.now()
 
     def pickTLE(self, t):
         if self._tleByTime[-1][0] < t:
             self._tle = self._tleByTime[-1][1]
-            self._tletimes = [
-                self._tleByTime[-1][0],
-                datetime.datetime(datetime.MAXYEAR, 1, 1),
-            ]
+            self._tletimes = [self._tleByTime[-1][0], datetime.datetime(datetime.MAXYEAR, 1, 1)]
         else:
             for w in range(len(self._tleByTime) - 1, -1, -1):
                 if self._tleByTime[w][0] < t or w == 0:
                     self._tle = self._tleByTime[w][1]
                     self._tletimes = [self._tleByTime[w][0], self._tleByTime[w + 1][0]]
                     break
 
-    def getSatellite(self, t) -> Tuple[sf_api.EarthSatellite, sf_api.Time]:
-        """Produces skyfield.EarthSatellite and its location for Swift at the given time
-
-        Args:
-            t (_type_): _description_
-
-        Returns:
-            _type_: _description_
-        """
+    def getSatellite(self, t):
         global verbose
         # print(t, self._tletimes)
         if t < self._tletimes[0] or self._tletimes[1] < t:
             if verbose:
                 print("Picking TLE for time %s" % (t,))
             self.pickTLE(t)
         if verbose:
-            print(
-                "Picked TLE for %s < %s < %s"
-                % (self._tletimes[0], t, self._tletimes[1])
-            )
-        sat = sf_api.EarthSatellite(self._tle[1], self._tle[2], name=self._tle[0])
-        sft = sftime(t)
-        return sat, sat.at(sft)
+            print("Picked TLE for %s < %s < %s" % (self._tletimes[0], t, self._tletimes[1]))
+        sat = ephem.readtle(self._tle[0], self._tle[1], self._tle[2])
+        self._earthcenter.date = t
+        sat.compute(self._earthcenter)
+        return sat
 
     def usetledb(self, catnum=28485):
-        """Use spacetrack tles from database (not publicly available)"""
-        import tledb  # pyright: ignore[reportMissingImports]
-
+        """Use spacetrack tles from database"""
+        import tledb
         tles = tledb.getTLEs(catnums=[catnum], all_in_time=True)
         self._tleByTime = [(t.epoch, t.threelines(split=True)) for t in tles]
         return self.getSatellite(self._earthcenter.date.datetime())
 
     def satname(self):
         return self._tleByTime[0][1][0]
 
     def updateTLE(self):
         global verbose
         try:
             # time.clock() is not what was wanted, since that doesn't give you the clock time
-            checksecs = time.mktime(
-                (datetime.datetime.now() + datetime.timedelta(days=-1)).timetuple()
-            )
+            checksecs = time.mktime((datetime.datetime.now() + datetime.timedelta(days=-1)).timetuple())
             if os.stat(tlefile).st_mtime > checksecs:
                 return  # The TLE file exists and is less than a day old
         except:
+
             pass
         tlematch = re.compile(TLEpattern[-1])
-        for url_month in (
-            datetime.datetime.utcnow().strftime(TLEpattern[0]),
-            (datetime.datetime.utcnow() - datetime.timedelta(30)).strftime(
-                TLEpattern[0]
-            ),
-        ):
+        for url_month in (datetime.datetime.utcnow().strftime(TLEpattern[0]),
+                          (datetime.datetime.utcnow() - datetime.timedelta(30)).strftime(TLEpattern[0])):
             try:
                 if verbose:
                     print("Trying to get TLE from %s" % (url_month,))
                 httpdir = generaldir.httpDir(url_month)
                 obsmonth = httpdir.dirs()
                 obsmonth.reverse()
                 for obs in obsmonth:
@@ -323,59 +312,54 @@
     """
     Given theta,phi in radians, returns (open_coded_area_in_cm^2, cosfactor)
 
     theta = distance from center of FOV (boresight) in radians
     phi = angle around boresight in radians.
     This is moderate accuracy, but does not take into account, e.g. dead detectors.
     """
-    theta = apAngle(theta, u.rad)
-    phi = apAngle(phi, u.rad)
-
-    if np.cos(theta) < 0:
-        return (0.0, np.cos(theta))
+    if math.cos(theta) < 0:
+        return (0.0, math.cos(theta))
     # BAT dimensions
-    detL = 286 * 4.2e-3  # Amynote: each det element is has length 4.2e-3 m
-    detW = 173 * 4.2e-3  # Amynote: each det element is has length 4.2e-3 m
+    detL = 286 * 4.2e-3  ## Amynote: each det element is has length 4.2e-3 m
+    detW = 173 * 4.2e-3  ## Amynote: each det element is has length 4.2e-3 m
     maskL = 487 * 5.0e-3  # Using the 5 mm mask cells, true size is 95.9" x 47.8"
     maskW = 243 * 5.0e-3
     efl = 1.00
     # Calculate dx, but reverse it if necessary to put projected detector to left of mask center
-    dx = (maskL - detL) / 2 - efl * np.tan(theta) * abs(np.cos(phi))
-    dy = (maskW - detW) / 2 + efl * np.tan(theta) * np.sin(phi)
+    dx = (maskL - detL) / 2 - efl * math.tan(theta) * abs(math.cos(phi))
+    dy = (maskW - detW) / 2 + efl * math.tan(theta) * math.sin(phi)
     # Boundaries of the detector as clipped to rectangle of mask
     x1 = max(0, -dx)
     x2 = min(detL, maskL - dx)
     deltaX = x2 - x1
     y1 = max(0, -dy)
     y2 = min(detW, maskW - dy)
     deltaY = y2 - y1
     # Now adjust for the cut corners, which first attacks the upper left detector corner
     # as described by the (if-necessary-reversed) coord. system
-    xint = (
-        (y1 + dy) - maskW / 2 - (dx + x1)
-    )  # line of corner clip extends through (x1 + xint, y1)
+    xint = (y1 + dy) - maskW / 2 - (dx + x1)  # line of corner clip extends through (x1 + xint, y1)
     if deltaX < 0 or deltaY < 0:
         area = 0
-    elif xint <= -deltaY:  # no clipping
+    elif xint <= - deltaY:  # no clipping
         area = deltaX * deltaY
     elif xint <= 0:  # upper left corner clipped along left edge
         if deltaY <= deltaX - xint:  # clip from left edge, to top edge
             area = deltaX * deltaY - ((deltaY + xint) ** 2) / 2
         else:  # clip from left edge to right edge
-            area = deltaX * -xint + (deltaX**2) / 2
+            area = deltaX * -xint + (deltaX ** 2) / 2
     elif xint <= deltaX:  # clipped at bottom edge
         if xint <= deltaX - deltaY:  # clipped bottom and top
-            area = (deltaX - xint) * deltaY - (deltaY**2) / 2
+            area = (deltaX - xint) * deltaY - (deltaY ** 2) / 2
         else:  # clipped bottom and right
             area = ((deltaX - xint) ** 2) / 2
     else:
         area = 0
     # if you want to see what the corners do: area = max(0,deltaX * deltaY) - area
     # multiply by 1e4 for cm^2, 1/2 for open area
-    return (area * 1e4 / 2, np.cos(theta))
+    return (area * 1e4 / 2, math.cos(theta))
 
 
 def detid2xy(detids):
     """
     Convert detector ids to x,y positions
 
     This is tricky.  You can understand it, but it isn't worth it.
@@ -402,296 +386,202 @@
     # 126                          70  57                          1
     # 125                          69  58                          2   ^
     # 124                          68  59                          3   |
     # 123                          67  60                          4   jmod
     # 122                          66  61                          5
     # 121                          65  62                          6    imod  ->
     # 120 112 104  96  88  80  72  64  63  55  47  39  31  23  15  7
-    # bit7 is left or right half
-    bit6, bit5_0 = np.divmod(det_in_mod, np.int16(64))
-    bit6_3, bit2_0 = np.divmod(
-        det_in_mod, np.int16(8)
-    )  # bits 6-3 determine the imod, bits 2-0 jmod
+    bit6, bit5_0 = np.divmod(det_in_mod, np.int16(64))  # bit7 is left or right half
+    bit6_3, bit2_0 = np.divmod(det_in_mod, np.int16(8))  # bits 6-3 determine the imod, bits 2-0 jmod
     imod = np.int16(15) - bit6_3
     jmod = np.where(bit6, bit2_0, np.int16(7) - bit2_0)
 
     # for block 0-7, half-DMs are arranged
     # 1    9
     # 0    8
     # 3    11     ^
     # 2    10     |
     # 5    13     |
     # 4    12   jblock
     # 7    15
     # 6    14          iblock ---->
 
     bit10, bit9_7 = np.divmod(mod_in_block, np.int16(8))
-    # 16 detectors + 2-space gap for second column
-    iblock = imod + np.int16(18) * bit10
+    iblock = imod + np.int16(18) * bit10  # 16 detectors + 2-space gap for second column
     jmodrow = (np.array([6, 7, 4, 5, 2, 3, 0, 1]) * 11).astype(
-        np.int16
-    )  # 8 detectors and 3-space gap for each row of modules
+        np.int16)  # 8 detectors and 3-space gap for each row of modules
     jblock = jmod + jmodrow[bit9_7]
 
     # blocks are arranged:
     #       0  1  2  3  4  5  6  7
     #       8  9  10 11 12 13 14 15
     # and blocks 8-15 are rotated 180 degrees
     bit15, bit14_11 = np.divmod(block, np.int16(8))
     #                      8-15        0-7
-    y = np.where(bit15, np.int16(85) - jblock - 1, np.int16(88) + jblock)
-    x = np.where(bit15, np.int16(34) - iblock - 1, iblock) + np.int16(36) * bit14_11
+    y = np.where(bit15, np.int16(85) - jblock, np.int16(88) + jblock)
+    x = np.where(bit15, np.int16(34) - iblock, iblock) + np.int16(36) * bit14_11
     if scalar:
         x = np.int16(x)
         y = np.int16(y)
     return x, y
 
-
 @functools.lru_cache(maxsize=0)
-def xy2detidmap():
+def _xy2detidmap():
     """
     Produce a detector map filled with detector IDs
 
     -1 for unpopulated detector locations
 
     :return: detids[y, x]
     :rtype: uint16, shape = (173, 286)
     """
-    detids = np.arange(0, 2**15)
-    x, y = detid2xy(detids)
-    result = np.full((y.max() + 1, x.max() + 1), np.int16(-1))
-    result[y, x] = detids
+    detids = np.arange(0,2**15)
+    x,y = detid2xy(detids)
+    result = np.full((y.max()+1, x.max()+1), np.int16(-1))
+    result[y,x] = detids
     return result
 
-
 def xy2detid(x, y):
-    dmap = xy2detidmap()
+    dmap = _xy2detidmap()
     return dmap[y, x]
 
 
 def loadsourcecat():
     """Read in source catalog
-
+    
     FIXME, should be more automatic
     """
     global sourcecat
     global verbose
     try:
         id(sourcecat)
     except NameError:
         if os.path.exists(cataloglist[3]):
             if verbose:
                 print("Loading catalogs:\n %s" % "\n ".join(cataloglist[0:3]))
-            sourcecat = sourcelist(
-                cataloglist[0:3] + [fitscatalog], verbose=verbose
-            )  # Exclude newcatalog
+            sourcecat = sourcelist(cataloglist[0:3] + [fitscatalog], verbose=verbose)  # Exclude newcatalog
         else:
             if verbose:
                 print("Using old catalog %s" % (basecatalog,))
             sourcecat = sourcelist((basecatalog, fitscatalog), verbose=verbose)
         if verbose:
             print("Loaded")
         # print(" ".join(sourcecat.allsources.keys()))
 
 
 class source:
     def __init__(self, initstring=None, **kwargs):
         """
         A source location with the ability to calculate BAT-relative angles and exposure
 
-        :param initstring: String from source table ('|' delimited), or object recognized by Simbad
+        :param initstring: String from source table, or an ephem function name (such as 'Sun')
         :param kwargs: {ra:ra_deg, dec:dec_deg, <name:'a name'>, <catnum:catnum>}
         """
-        # This is where the Sun was implemented
-        # if initstring in ephem.__dict__:
-        #     self.needs_computing = True
-        #     self.computable = ephem.__dict__[initstring]()
-        # elif...
-        if "ra" in kwargs and "dec" in kwargs:
+        if initstring in ephem.__dict__:
+            self.needs_computing = True
+            self.computable = ephem.__dict__[initstring]()
+        elif 'ra' in kwargs and 'dec' in kwargs:
             if initstring:
                 raise RuntimeError("Give ra=,dec= or an initstring but not both")
-            self.set_radec(kwargs["ra"], kwargs["dec"])
-            self.name = kwargs.get("name", "unnamed")
-            self.catnum = kwargs.get("catnum", 0)
+            self.eq = ephem.Equatorial(kwargs['ra'] * ephem.degree,
+                                       kwargs['dec'] * ephem.degree)
+            self.name = kwargs.get('name', 'unnamed')
+            self.catnum = kwargs.get('catnum', 0)
         else:
             self.needs_computing = False
-            if "|" in initstring:
-                s = initstring.split("|")
-                self.name = s[3].strip().replace(" ", "_")
-                self.catnum = int(s[5])
-                self.set_radec(float(s[9]), float(s[10]))
-            else:
-                try:
-                    ra, dec = simbadlocation(initstring)
-                    self.set_radec(ra, dec)
-                    self.name = initstring
-                    self.catnum = -1
-                except:
-                    raise NameError(
-                        f"Source name {initstring} not recognized by Simbad"
-                    )
-
-    def set_radec(self, ra_deg, dec_deg):
-        self.skyloc = SkyCoord(
-            ICRS(ra=apAngle(ra_deg, u.deg), dec=apAngle(dec_deg, u.deg))
-        )
-
-    @property
-    def ra_deg(self):
-        return self.skyloc.ra.degree
-
-    @property
-    def dec_deg(self):
-        return self.skyloc.dec.degree
+            s = initstring.split("|")
+            self.name = s[3].strip().replace(" ", "_")
+            self.catnum = int(s[5])
+            self.eq = ephem.Equatorial(ephem.degrees(float(s[9]) * ephem.degree),
+                                       ephem.degrees(float(s[10]) * ephem.degree))
+        # All input is in degrees, output is in ephem angles
 
     @classmethod
-    def source(cls, ra, dec, name="anonymous", catnum=-1) -> str:
-        """The source as a '|'-delimted string as used in ASCII catalog tables
-
-        Args:
-            ra (float): degrees
-            dec (float): degrees
-            name (str, optional): _description_. Defaults to "anonymous".
-            catnum (int, optional): _description_. Defaults to -1.
-
-        Returns:
-            str: _description_
-        """
-        return cls(
-            f"|||{name}||{catnum}||||{apAngle(ra, u.deg).degree}|{apAngle(dec, u.deg).degree}"
-        )
-
-    def sf_position(self) -> sf_ICRF:
-        """Position of source as a skyfield.Position"""
-        return sf_api.position_of_radec(
-            ra_hours=self.ra_deg / 15, dec_degrees=self.dec_deg
-        )
+    def source(cls, ra, dec, name="anonymous", catnum=-1):
+        return cls("|||{}||{}||||{}|{}".format(name, catnum, ra, dec))
 
     def exposure(self, ra, dec, roll):
         # returns (projected_area, cos(theta))
         (thetangle, phi) = self.thetangle_phi(ra, dec, roll)
-        if thetangle > apAngle(90, u.deg):
+        if thetangle.norm >= ephem.halfpi:
             return 0.0, 0.0
         return batExposure(thetangle, phi)
 
-    def thetangle_phi(
-        self, ra: float, dec: float, roll: float
-    ) -> Tuple[(apAngle, apAngle)]:
-        """_Source position in instrument FOV given instrument pointing direction
+    def distance(self, ra, dec):
+        return ephem.separation((self.eq.ra, self.eq.dec),
+                                (ephem.degrees(ra * ephem.degree), ephem.degrees(dec * ephem.degree)))
+
+    def posang_from(self, ra, dec):
+        """ Position angle East of North from the given location to self """
+        # Stolen from idl posang.pro, with self as point 2
+        decrad = ephem.degrees(dec * ephem.degree)
+        radiff = self.eq.ra - ephem.degrees(ra * ephem.degree)
+        ang = ephem.degrees(math.atan2(math.sin(radiff),
+                                       math.cos(decrad) * math.tan(self.eq.dec) - math.sin(decrad) * math.cos(radiff)))
+        return ang
+
+    def thetangle_phi(self, ra, dec, roll):
+        """ Source position in instrument FOV given instrument pointing direction
             returns (thetangle,phi) where thetangle is the angular distance from
             the boresight and phi is the angle from the phi=0 axis of BAT.
-
+            
             theta = tan(thetangle) gives the theta we use, which is the projected distance to a flat plane,
             but it is not useful for thetangle > 90 degrees
-
-        Args:
-            ra (float): ra of spacecraft boresight in degrees
-            dec (float): dec of spacecraft boresight in degrees
-            roll (float): roll is 'roll left' (CCW as seen from behind looking out along boresight) in degrees
-        Returns:
-            (theta:degree, phi:apAngle): location of source in spacecraft spherical coordinates
         """
-        # Use astropy coordinates
-        boreloc = SkyCoord(ICRS(ra=apAngle(ra, u.deg), dec=apAngle(dec, u.deg)))
-        thetangle = boreloc.separation(self.skyloc).to(u.deg)
-        # posang is CCW, phi is CCW from +Y so (posang - roll - 90deg) gives phi
-        phi = (
-            (
-                coordinates.position_angle(
-                    boreloc.ra, boreloc.dec, self.skyloc.ra, self.skyloc.dec
-                )
-                - apAngle(roll, u.deg)
-                - apAngle(90, u.deg)
-            )
-            .wrap_at(180 * u.deg)
-            .to(u.deg)
-        )
+        thetangle = self.distance(ra, dec)
+        # roll is 'roll right', posang is CCW, phi is CCW from +Y so roll + posang gives phi
+        phi = self.posang_from(ra, dec) - ephem.degrees(roll * ephem.degree) - ephem.halfpi
+        # print("posang = %f E of N, roll = %f" % (self.posang_from(ra,dec),0+ephem.degrees( roll * ephem.degree)))
         return (thetangle, phi)
 
     def compute(self, t):
-        """Default implementation does nothing
-
-        Args:
-            t (time): _description_
-        """
-        pass
+        if self.needs_computing:
+            obs = ephem.Observer()
+            obs.elev = -6378137.0  # equatorial radius of WGS84
+            obs.date = t
+            # print(obs, self.computable)
+            self.computable.compute(obs)
+            self.name = self.computable.name
+            self.catname = 0
+            # print(self.computable)
+            self.eq = ephem.Equatorial(self.computable)
 
     def __str__(self):
-        return "|||%s||%d||||%f|%f|" % (
-            self.name,
-            self.catnum,
-            self.skyloc.ra.degree,
-            self.skyloc.dec.degree,
-        )
-
-
-class sunsource(source):
-    def __init__(self, t=None, bodyname="Sun"):
-        self.body = loadsfephem()[bodyname]
-        self.earth = loadsfephem()["Earth"]
-        skyloc = self._skyloc_at(t)
-        super().__init__(ra=skyloc.ra.degree, dec=skyloc.dec.degree, name=bodyname)
-
-    def _skyloc_at(self, t=None) -> ICRS:
-        # Cached so it only downloads the DE422 once and only reads it once per run
-        if t is None:
-            t = datetime.datetime.now(tz=datetime.timezone.utc)
-        t = sftime(t)
-        app = self.earth.at(t).observe(self.body).apparent()
-        ra, dec, _ = app.radec()
-        skyloc = SkyCoord(
-            ICRS(ra=apAngle(ra._degrees, u.deg), dec=apAngle(dec._degrees, u.deg))
-        )
-        return skyloc
-
-    def compute(self, t):
-        self.skyloc = self._skyloc_at(t)
+        return "|||%s||%d||||%f|%f|" % (self.name, self.catnum, self.eq.ra / ephem.degree, self.eq.dec / ephem.degree)
 
 
 # This is a truncated version of catalog.  It should become the parent of catalog someday (FIXME 2008-09-17)
 class sourcelist:
-    def __init__(self, filelist=None, verbose=False):
+    def __init__(self, filelist=None,
+                 verbose=False):
         if filelist is None:
-            filelist = [
-                os.path.join(catalogdir, "catalog"),
-                os.path.join(catalogdir, "grbcatalog"),
-            ]
+            filelist = [os.path.join(catalogdir, "catalog"), os.path.join(catalogdir, "grbcatalog")]
         self.allsources = {}
         for file in filelist:
             # print(file)
             try:
                 self.addFromFile(file, verbose=verbose)
             except:
                 traceback.print_exc()
                 pass
 
     def addFromFile(self, file, verbose=False):
         if verbose:
             print(file)
         if ".fits" in file:
             for row in fits.getdata(file):
-                aSource = source.source(
-                    ra=row.field("RA_OBJ"),
-                    dec=row.field("DEC_OBJ"),
-                    name=row.field("NAME"),
-                )
+                aSource = source.source(ra=row.field('RA_OBJ'),
+                                        dec=row.field('DEC_OBJ'),
+                                        name=row.field('NAME'))
                 if verbose:
                     print(aSource)
                 # print(line,aSource.name)
                 self.allsources[self.canonName(aSource.name)] = aSource
         else:
             for line in open(file).readlines():
-                line = line.strip()
-                if (
-                    "+------+------------+" in line
-                    or "|   ROW|        TIME|           NAME|" in line
-                    or line.startswith("#")
-                    or line == ""
-                ):
-                    continue
                 try:
                     aSource = source(line)
                     if verbose:
                         print(aSource)
                     # print(line,aSource.name)
                     self.allsources[self.canonName(aSource.name)] = aSource
                 except:
@@ -709,14 +599,318 @@
                 return s
         return None
 
     def canonName(self, name):
         return name.lower().replace(" ", "_")[0:15].replace("_", "")
 
 
+def strip_nbsp(s):
+    """ Replace '&nbsp' with spaces and then strip (beginning and end) spaces.
+        An interior &nbsp; will remain an interior space"""
+    return re.sub("&nbsp;", " ", s).strip()
+
+
+class pointingEntry:
+    def __init__(self, tstart, tslewend, tend, ra, dec, roll, obs, segment, sourcename, planned):
+        self._tstart = tstart
+        self._tslewend = tslewend
+        if tend == None:  # How to handle the stubs  FIXME doesn't handle the case of reading day n then n-1
+            self._tend = tstart + _maxobslength
+        else:
+            self._tend = tend
+        self._ra = ra
+        self._dec = dec
+        self._roll = roll
+        self._obs = obs
+        self._segment = segment
+        self._sourcename = sourcename
+        self._planned = planned
+
+    def fromTableRow(row, preplanned):
+        """ row is a table row parsed by BeautifulSoup in the format listed below
+            Returns a pointingEntry if it can, otherwise raises a ValueError"""
+        try:
+            entries = row.findAll('td')
+
+            tstart = datetime.datetime.strptime(strip_nbsp(soupCatStrings(entries[0], True)), "%Y-%m-%d %H:%M:%S")
+            tend = datetime.datetime.strptime(strip_nbsp(soupCatStrings(entries[1], True)), "%Y-%m-%d %H:%M:%S")
+            obs = int(strip_nbsp(soupCatStrings(entries[2], True)))
+            segment = int(strip_nbsp(soupCatStrings(entries[3], True)))
+            sourcename = strip_nbsp(soupCatStrings(entries[4], True))
+            ra = float(strip_nbsp(soupCatStrings(entries[5], True)))
+            dec = float(strip_nbsp(soupCatStrings(entries[6], True)))
+            roll = float(strip_nbsp(soupCatStrings(entries[7], True)))
+            # Remaining fields not relevant
+            pe = pointingEntry(tstart, tstart, tend, ra, dec, roll, obs, segment, sourcename, preplanned)
+            if verbose:
+                print(pe)
+            return pe
+        except:
+            if verbose:
+                print("Failed to parse row", row)
+            raise ValueError("pointingEntry: Failed to parse row: %s", row)
+
+    fromTableRow = staticmethod(fromTableRow)
+
+    def fContains(self, t):
+        return self._tstart <= t and t < self._tend
+
+    def compareTime(self, t):
+        if t < self._tstart:
+            return -2  # Before the observation
+        elif t < self._tslewend:
+            return -1  # Before stable
+        elif t < self._tend:
+            return 0  # During stable observation
+        else:
+            return 1  # after observation
+
+    def fOverlaps(self, trange, tend=None):
+        if tend != None and len(trange) == 1:
+            return self.fOverlaps((trange, tend))  # Convert from fOverlaps(x,y) to fOverlaps( (x,y) )
+        else:
+            return self._tstart <= trange[1] and self._tend >= trange[0]
+
+    def __str__(self):
+        if self._planned:
+            if self._planned == True:
+                plannedstring = "(Preplanned)"
+            else:
+                plannedstring = "(planned %s)" % self._planned
+        else:
+            plannedstring = ""
+        return "%08d%03d  %s - %s - %s [%7.3f, %7.3f, %7.3f] %s %s" % (
+            self._obs, self._segment,
+            self._tstart.strftime("%Y-%j-%H:%M:%S"),
+            self._tslewend.strftime("%H:%M:%S"),
+            self._tend.strftime("%H:%M:%S"),
+            self._ra, self._dec, self._roll,
+            self._sourcename,
+            plannedstring)
+
+
+# The pre-planned is like
+# 2007-086-00:00:00 | PPT | Begin | J2043+1255 | 36281 | 2 | 33590713 | 310.817427802637 | 12.9223455711058 | 85.6387273417218 | 0 | 0 | 12525 | 50 | 1471 | Paolo Giommi and Roger Romani Fill in Target | targ_20070850000_20070870000_01_DB.tcl
+# 2007-086-00:00:00 | mnv | Begin | J2043+1255
+# 2007-086-00:02:00 | mnv | End | J2043+1255
+# 2007-086-00:27:00 | PPT | End | J2043+1255 | 36281 | 2 | 33590713 | 310.817427802637 | 12.9223455711058 | 85.6387273417218 | 0 | 0 | 12525 | 50 | 1471 | Paolo Giommi and Roger Romani Fill in Target | targ_20070850000_20070870000_01_DB.tcl
+# the as-flown when unzipped is like
+# |2007-077-11:50:02.127500|PPT|Begin|saa-cold-77-10|74566|74566|2|2|33628998|33628998|183.604|14.053|346.321|0|0|10|100.000|Validated|SAA @ 2007-077-11:51:11|00074566002|
+# |2007-077-11:53:25.727381|Slew Settled|Begin|saa-cold-77-10|74566|74566|2|2|33628998|33628998|317.522|-30.014|60.266|0|0|10|100.000|Validated|SAA @ 2007-077-11:51:11|00074566002|
+# |2007-077-11:55:00.000000|SAA|Begin|||||||||||||||Validated|||
+# |2007-077-12:03:10.726820|PPT|End|saa-cold-77-10|74566|74566|2|2|33628998|33628998|317.522|-30.014|60.265|0|0|10|100.000|Validated|SAA @ 2007-077-11:51:11|00074566002|
+# The preplanned HTML file is like
+# <TR><TD> <FONT size="2">2008-246-03:25:00<TD> <FONT size="2">2008-246-03:37:00<TD> <FONT size="2"><a href = "SDSSJ140642.0+031940_ppt.html">SDSS J140642.0+031940</a><TD> <FONT size="2">211.65111<TD> <FONT size="2">3.3351599<TD> <FONT size="2">287.17465<TD> <FONT size="2">37754<TD> <FONT size="2">1<TD> <FONT size="2">AUTO<TD> <FONT size="2">0x20AB<TD> <FONT size="2">50<TD> <FONT size="2">720
+# <TR><TD> <FONT size="2">2008-246-03:37:00<TD> <FONT size="2">2008-246-03:59:00<TD> <FONT size="2"><a href = "saa-cold-246-20_ppt.html">saa-cold-246-20</a><TD> <FONT size="2">313.82042<TD> <FONT size="2">55.000000<TD> <FONT size="2">329.87982<TD> <FONT size="2">74218<TD> <FONT size="2">3<TD> <FONT size="2">AUTO<TD> <FONT size="2">0x0009<TD> <FONT size="2">100<TD> <FONT size="2">1320
+# <TR><TD> <FONT size="2">2008-246-03:59:00<TD> <FONT size="2">2008-246-04:29:00<TD> <FONT size="2"><a href = "SGR0501+4516_ppt.html">SGR 0501+4516</a><TD> <FONT size="2">75.278000<TD> <FONT size="2">45.276230<TD> <FONT size="2">81.400000<TD> <FONT size="2">321174<TD> <FONT size="2">11<TD> <FONT size="2">WT<TD> <FONT size="2">0x2227<TD> <FONT size="2">99<TD> <FONT size="2">1800
+
+# The new table format is
+# <tr class='header'><td><br />&nbsp;Begin&nbsp;</td><td><br />&nbsp;End&nbsp;</td><td>&nbsp;Target&nbsp;<br />&nbsp;ID&nbsp;</td><td><br />&nbsp;Seg.&nbsp;</td><td><br />&nbsp;Target Name&nbsp;</td><td><br />&nbsp;R.A.&nbsp;</td><td><br />&nbsp;Dec.&nbsp;</td><td><br />&nbsp;Roll&nbsp;</td><td>&nbsp;XRT&nbsp;<br />&nbsp;Mode&nbsp;</td><td>&nbsp;UVOT&nbsp;<br />&nbsp;Mode&nbsp;</td><td><br />&nbsp;FoM&nbsp;</td><td>&nbsp;Time&nbsp;<br />&nbsp;(s)&nbsp;</td></tr>
+#		<tr class='norm1'>
+#			<td>&nbsp;2009-12-15 00:00:02&nbsp;</td>
+#			<td>&nbsp;2009-12-15 00:13:59&nbsp;</td>
+#			<td>&nbsp;<a href='https://www.swift.psu.edu/operations/obsSchedule.php?t=30793'>30793</a>&nbsp;</td>
+#			<td>&nbsp;<a href='https://www.swift.psu.edu/operations/obsSchedule.php?t=30793&amp;s=103&amp;a=1'>103</a>&nbsp;</td>
+#			<td style='text-align:left;'>&nbsp;Mkn501&nbsp;</td>
+#			<td>&nbsp;253.473&nbsp;</td>
+#			<td>&nbsp;39.792&nbsp;</td>
+#			<td>&nbsp;179.670&nbsp;</td>
+#			<td>&nbsp;WT&nbsp;</td>
+#			<td>&nbsp;0x308f&nbsp;</td>
+#			<td>&nbsp;72&nbsp;</td>
+#			<td>&nbsp;837&nbsp;</td>
+
+
+# Old patterns for pointingTable.oldLoad*:
+# use datatime.strftime(asflownpattern)
+# asflownpattern="/Volumes/Data/Swift/swift-trend/%Y_%m/misc/asflown/AFST_%Y%j*.txt.gz"
+# preplannedpattern="/Users/palmer/Documents/networking/downloads/ppst-mail/PPST_%Y%j*.txt*"
+# preplannedhtmldir="http://www.swift.psu.edu/operations/PPST/%Y%j/"
+# asflownpattern="/Volumes/Data/Swift/swift-trend/%Y_%m/misc/asflown/AFST_%Y%j*.txt.gz"
+# preplannedpattern="/Users/palmer/Documents/networking/downloads/ppst-mail/PPST_%Y%j*.txt*"
+# preplannedhtmldir="http://www.swift.psu.edu/operations/PPST/%Y%j/"
+
+
+class pointingTable:
+    def __init__(self, ppstfile=None):
+        self._daylist = []  # Stored as int(YYYYdoy)
+        self._entries = []
+        if ppstfile:
+            self._explicitPPST = ppstfile
+            for f in self._explicitPPST:
+                self.loadURLHTML("file://%s" % os.path.realpath(f), 0)
+                if verbose:
+                    for e in self._entries:
+                        print(e)
+        else:
+            self._explicitPPST = []
+
+    def getPointings(self, trange):
+        try:
+            tfullrange = (min(trange), max(trange))
+        except TypeError:
+            tfullrange = (trange, trange)
+        if not self._explicitPPST:
+            tmin = tfullrange[0] - _maxobslength
+            tmax = tfullrange[1] + _maxobslength + datetime.timedelta(days=1,
+                                                                      minutes=90)  # Read an extra day for the end of day case
+            t = tmin
+            while t < tmax:
+                try:
+                    self.loadDay(t)
+                except:
+                    if t == tmin:  # First day of range, try stepping back 5 days to see if you hit any useful files
+                        if verbose:
+                            print("Searching backwards")
+                        for lookback in range(-1, -5, -1):
+                            try:
+                                self.loadDay(t + datetime.timedelta(days=lookback))
+                                # print("Found ")
+                                break  # If it works, break out
+                            except:
+                                if verbose:
+                                    traceback.print_exc()
+                                pass
+                t += datetime.timedelta(days=1)
+        return self._findEntries(tfullrange)
+
+    def loadDay(self, t):
+        day = t.strftime("%Y-%m-%d")
+        if verbose:
+            print("Loading day %s " % day)
+        if day in self._daylist:
+            return True  # already loaded
+        (daypointlist, asflowncomplete) = self.loadURLHTML(t.strftime(asflownURLpattern), False)
+        if not daypointlist or not asflowncomplete:
+            if verbose:
+                print("%s : %d observations as flown, asflowncomplete = %s" % (day, len(daypointlist), asflowncomplete))
+            (ppstdaylist, ppstread) = self.loadURLHTML(t.strftime(preplannedURLpattern), True)
+            if not daypointlist:
+                daypointlist = ppstdaylist  # No asflown data
+            else:
+                lastasflown = max([p._tend for p in daypointlist])  # assume there are no gaps in the as-flown
+                daypointlist.extend([p for p in ppstdaylist if p._tstart > lastasflown])
+        self._entries.extend(daypointlist)
+        self._daylist.append(day)
+
+    def loadURLHTML(self, u, preplanned):
+        """ Returns (pointlist, complete)
+        """
+        pointlist = []
+        complete = False
+        moretocome = False
+        if verbose:
+            print(u)
+        try:
+            s = BeautifulSoup.BeautifulSoup(urlopen(u, None, timeout=10, context=unsafe_context), "html.parser")
+            table = s.find('table')  # , {"class": "ppst"})  # Even the as-flown table has class ppst
+            for row in table.findAll('tr'):
+                try:
+                    pe = pointingEntry.fromTableRow(row, preplanned)
+                    pointlist.append(pe)
+                except:
+                    text = strip_nbsp(soupCatStrings(row))
+                    if verbose:
+                        print(text)
+                    try:
+                        # Crude way of checking whether the AFST is complete.  Better would be to check the time
+                        if (text[0:9] == 'There may'
+                                or text[0:10] == 'There will'):  # be later observations for this date
+                            break  # Do not execute else clause
+                    except:
+                        pass
+            else:
+                if len(pointlist) != 0:  # Reached end of table and actually read something
+                    # Check if what was read is within 20 min before to 5 minutes after end of day 
+                    complete = (pointlist[-1]._tend + datetime.timedelta(minutes=20)).time() < datetime.time(0, 25, 0)
+                else:
+                    complete = False
+        except:
+            return (None, False)
+        return (pointlist, complete)
+
+    def _findEntries(self, trange):
+        try:
+            if len(trange) == 1:
+                return [p for p in self._entries if p.fContains(trange)]
+            else:
+                return [p for p in self._entries if p.fOverlaps(trange)]
+        except:
+            return [p for p in self._entries if p.fContains(trange)]
+
+
+def soupCatStrings(soupnode, stripit=False):
+    """Traverse the tree starting from soupnode, and return the 
+    strings of the leaf nodes concatenated together"""
+    if isinstance(soupnode, str):
+        s = soupnode
+    else:
+        s = "".join([soupCatStrings(sn, stripit) for sn in soupnode.contents])
+    if stripit:
+        s.strip()
+    return s
+
+
+class PointingsDatabase:
+    """ Database of pointings.  The database is only populated day-by-day as needed"""
+
+    def __init__(self):
+        try:
+            os.stat(self.Filename)
+        except:
+            self.CreateFile()
+
+    def ReadDay(self, t, force=False):
+        if force or self.CheckDay(t) != 3:
+            raise RuntimeError("Not yet implemented")
+
+    def Filename():
+        return pdbfile
+
+    Filename = staticmethod(Filename)
+
+    def CheckDay(self, t):
+        """ Returns the status of a day in the database:
+            0 not loaded
+            1 PPST only
+            2 PPST and partial AFST
+            3 final AFST """
+        tstr = t.strftime("%Y-%m-%d")
+        conn = sqlite3.connect(pdbfile, detect_types=sqlite3.PARSE_DECLTYPES)
+        result = 0
+        try:
+            daystatus = conn.cursor()
+            daystatus.execute('''select asflown_complete,asflow_partial,preplanned from days where date=?''', (tstr,))
+            (af, af_partial, preplanned) = daystatus.fetchone()
+            if af:
+                result = 3
+            elif af_partial:
+                result = 2
+            elif preplanned:
+                result = 1
+        except:
+            pass
+        conn.close()
+        return result
+
+    def CreateFile(self, delete=False):
+        try:
+            if delete:
+                os.remove(pdbfile)
+                raise EOFError("No error")
+            else:
+                os.stat(pdbfile)
+        except:
+            conn = sqlite3.connect(pdbfile, detect_types=sqlite3.PARSE_DECLTYPES)
+            conn.execute('''create table pointings (%s)''' % pdbfields_text)
+            conn.execute('''create table days (%s)''' % pdbdayfields_text)
+            conn.commit()
+            conn.close()
+
+
 def hasLength(x):
     try:
         len(x)
         return True
     except:
         return False
 
@@ -731,20 +925,20 @@
     dec_deg = None
     strippers = "\xc2\xa0 \t\n"  # some strange characters when Mail.app saves mail
     for l in lines:
         l = swutil.removeNonAscii(l)
         ipntime = ipntimeRE.search(l)
         if ipntime:
             g = ipntime.groupdict()
-            ss = float(g["s"])
+            ss = float(g['s'])
             h = int(ss / 3600)
             ss -= h * 3600
             m = int(ss / 60)
             ss -= m * 60
-            ymdT = "20%s-%s-%sT" % (g["y"], g["m"], g["d"])
+            ymdT = "20%s-%s-%sT" % (g['y'], g['m'], g['d'])
             hms = "%02d:%02d:%05.3f" % (h, m, ss)
         else:
             ls = l.split()
             if len(ls) > 1:
                 if ls[0] in ["GRB_RA:", "SRC_RA:"]:
                     ra_deg = float(ls[1].split("d")[0].strip(strippers))
                 elif ls[0] in ["GRB_DEC:", "SRC_DEC:"]:
@@ -754,234 +948,105 @@
                 elif ls[0] in ["GRB_TIME:", "DISCOVERY_TIME:"]:
                     hms = ls[3].strip(strippers + "{}")
 
                 if ls[0] in ["GRB_RA:", "SRC_RA:", "EVENT_RA:"]:
                     ra_deg = float(ls[1].split("d")[0].strip(strippers))
                 elif ls[0] in ["GRB_DEC:", "SRC_DEC:", "EVENT_DEC:"]:
                     dec_deg = float(ls[1].split("d")[0].strip(strippers))
-                elif ls[0] in [
-                    "GRB_DATE:",
-                    "EVENT_DATE:",
-                    "DISCOVERY_DATE:",
-                    "TRIGGER_DATE:",
-                ]:
+                elif ls[0] in ["GRB_DATE:", "EVENT_DATE:", "DISCOVERY_DATE:", "TRIGGER_DATE:"]:
                     ymdT = "20%s-%s-%sT" % tuple(ls[5].strip(strippers).split("/"))
-                elif ls[0] in [
-                    "GRB_TIME:",
-                    "DISCOVERY_TIME:",
-                    "EVENT_TIME:",
-                    "TRIGGER_TIME:",
-                ]:
+                elif ls[0] in ["GRB_TIME:", "DISCOVERY_TIME:", "EVENT_TIME:", "TRIGGER_TIME:"]:
                     hms = ls[3].strip(strippers + "{}")
     met = swutil.string2met(ymdT + hms, nocomplaint=True, correct=True)
     return (ra_deg, dec_deg, met)
 
 
-def lineofsight(satpos, source):
+def lineofsight(sat, source):
     """Calculate the
-    (elevation_above_Earth_limb_degrees, losheight_m, description)
-    of the line of sight from the satellite position to the source.
-    minimum_elevation_above_sea_level is 0 if LOS intersects Earth, sat.elevation if LOS is upwards
+    (elevation_above_Earth_limb_degrees, minimum_elevation_above_sea_level_meters, description)
+    of the line of sight from the satellite to the source.
+    minimum_elevation_above_sea_level is 0 if LOS intersects Earth, sat.elevation if it LOS is upwards
     """
-    atm_thickness_m = 100e3  # How deep in the atmosphere you should report attenuation
-    # Using Skyfield positions for separation, thereafter raw radians
-    zenangle_rad = satpos.separation_from(source.sf_position()).radians
-    _, _, satradius = satpos.radec()
-    satradius_m = satradius.m
-    earthrad_m = u.earthRad.to(u.m)
-    # Hard earth horizon (equatorial radius)
-    zenhoriz_rad = np.pi / 2 + np.arccos(earthrad_m / satradius_m)
-    if zenangle_rad < np.pi / 2:
-        losheight_m = satradius_m - earthrad_m
+    zenangle = source.distance(sat.a_ra * r2d, sat.a_dec * r2d).norm
+    zenhoriz = ephem.halfpi + math.acos(earthradius_m / (sat.elevation + earthradius_m))
+    if zenangle < ephem.halfpi:
+        losheight = sat.elevation
         description = "up"
-    elif zenangle_rad > zenhoriz_rad:
-        losheight_m = 0.0
+    elif zenangle > zenhoriz:
+        losheight = 0.0
         description = "down"
     else:
-        losheight_m = (satradius_m * np.cos(zenangle_rad - np.pi / 2)) - earthrad_m
-        if losheight_m > atm_thickness_m:
+        losheight = ((sat.elevation + earthradius_m) * math.cos(zenangle - ephem.halfpi)) - earthradius_m
+        if losheight > atm_thickness:
             description = "depressed but unattenuated"
         else:
-            description = "attenuated by atmosphere at %.0f km" % (
-                losheight_m / 1000.0,
-            )
-    return (np.rad2deg(zenhoriz_rad - zenangle_rad), losheight_m, description)
-
-
-class PointingEntry:
-    def __init__(
-        self, tstart, tslewend, tend, ra, dec, roll, obs, segment, sourcename, planned
-    ):
-        self._tstart = tstart
-        self._tslewend = tslewend
-        if tend == None:  # How to handle the stubs
-            self._tend = tstart + datetime.timedelta(seconds=90 * 60)
-        else:
-            self._tend = tend
-        self._ra = ra
-        self._dec = dec
-        self._roll = roll
-        self._obs = obs
-        self._segment = segment
-        self._sourcename = sourcename
-        self._planned = planned
-
-    @classmethod
-    def listfromquery(cls, query: swto.ObsQuery) -> List["PointingEntry"]:
-        result = []
-        for entry in query:
-            # query.to_utctime()
-            pointent = cls(
-                entry.begin,
-                entry.begin + entry.slewtime,
-                entry.end,
-                entry.ra,
-                entry.dec,
-                entry.roll,
-                int(entry.obsid[:-3]),
-                entry.seg,
-                entry.targname,
-                False,
-            )
-            result.append(pointent)
-        return result
-
-    @classmethod
-    def listfortimes(cls, times: list[datetime.datetime], allinrange=False):
-        if allinrange:
-            begin = min(times)
-            end = max(times)
-            queries = [swto.ObsQuery(begin=begin, end=end)]
-        else:
-            queries = [swto.ObsQuery(t) for t in times]
-
-        result = []
-        for query in queries:
-            if query.submit():
-                result.extend(cls.listfromquery(query))
-        return result
-
-    def __str__(self):
-        if self._planned:
-            if self._planned == True:
-                plannedstring = "(Preplanned)"
-            else:
-                plannedstring = "(planned %s)" % self._planned
-        else:
-            plannedstring = ""
-        return "%08d%03d  %s - %s - %s [%7.3f, %7.3f, %7.3f] %s %s" % (
-            self._obs,
-            self._segment,
-            self._tstart.strftime("%Y-%j-%H:%M:%S"),
-            self._tslewend.strftime("%H:%M:%S"),
-            self._tend.strftime("%H:%M:%S"),
-            self._ra,
-            self._dec,
-            self._roll,
-            self._sourcename,
-            plannedstring,
-        )
+            description = "attenuated by atmosphere at %.0f km" % (losheight / 1000.0,)
+    return ((zenhoriz - zenangle) * r2d, losheight, description)
 
 
 def usage(progname):
     print("Usage: %s MET [MET....]" % progname)
     print("        -v --verbose                    diagnostic information")
     print("           --terse                      produce terse output")
     print("        -o --orbit                      satellite position")
-    print(
-        "        -s --source sourcename          source visibility.  Sourcename can be '123.4_-56.7' for RA_dec"
-    )
+    print("        -s --source sourcename          source visibility.  Sourcename can be '123.4_-56.7' for RA_dec")
     print("        -S --sun --Sun                  Sun visibility")
     print("            --visible                   Only when the source is in the FOV")
-    print(
-        "        -x --excelvis                   source visibility list in CSV Excelable format (grep vis)"
-    )
+    print("        -x --excelvis                   source visibility list in CSV Excelable format (grep vis)")
     # print("        -m --machine                    machine-convenient format with printouts on single lines")
-    print('        -p --position "ra_deg dec_deg"  position visibility')
-    print(
-        "        -t --timerange                  use all pointings in the range of times"
-    )
-    print(
-        "           --steptime seconds           cover the range fo times with this interval"
-    )
+    print("        -p --position \"ra_deg dec_deg\"  position visibility")
+    print("        -t --timerange                  use all pointings in the range of times")
+    print("           --steptime seconds           cover the range fo times with this interval")
     print("        -c --clipboard                  use times in the current clipboard")
-    print(
-        "        -f --format '%Y-%m-%dT%H:%M:%S' use given time format.  (Example is default)"
-    )
-    print(
-        "        -P --ppst   ppstfile            use local PPST file instead of getting from web"
-    )
-    print(
-        '        -a --attitude "ra dec roll"     manually include an attitude rather than PPST'
-    )
-    print(
-        "           --notice                     process GCN notice piped to stdin to extract time and position"
-    )
+    print("        -f --format '%Y-%m-%dT%H:%M:%S' use given time format.  (Example is default)")
+    print("        -P --ppst   ppstfile            use local PPST file instead of getting from web")
+    print("        -a --attitude \"ra dec roll\"     manually include an attitude rather than PPST")
+    print("           --notice                     process GCN notice piped to stdin to extract time and position")
     # print("           --METonly                    print out nothing but the MET")
     # print("           --UTConly                    print out nothing but the UTC")
     print("        -h --help                       this printout")
 
 
 # @swutil.timeout(60)
-def swinfo_main(argv=None, debug=None):
+def main(argv=None, debug=None):
     global verbose
     global terse
     global sourcecat
     if argv is None:
         argv = sys.argv
     sources = []
     orbits = False
     ppstfile = []
     timerange = False
     visible_only = False
     timestep = 0
     manualAttitudes = []
     excelvis = False
+    sunsource = None
     # debug=open("/tmp/swinfo.debug","a")
     # debug = None
 
     # if debug :
     #    sys.stdout = swutil.TeeFile(debug, sys.stdout)
 
     if debug:
-        debug.write(
-            "%s (%d): %s\n" % (datetime.datetime.now(), os.getpid(), " ".join(argv))
-        )
+        debug.write("%s (%d): %s\n" % (datetime.datetime.now(), os.getpid(), " ".join(argv)))
         vebose = True
         debug.flush()
 
     format = swutil.fitstimeformat
     try:
-        opt, timeargs = getopt.gnu_getopt(
-            argv[1:],
-            "vos:Sxp:tcf:P:a:h",
-            [
-                "verbose",
-                "terse",
-                "orbit",
-                "source=",
-                "sun",
-                "Sun",
-                "visible",
-                "excelvis",
-                "position=",
-                "timerange",
-                "steptime=",
-                "clipboard",
-                "format=",
-                "ppst=",
-                "attitude=",
-                "notice",
-                "help",
-            ],
-        )
+        opt, timeargs = getopt.gnu_getopt(argv[1:], "vos:Sxp:tcf:P:a:h",
+                                          ["verbose", "terse", "orbit", "source=", "sun", "Sun", "visible",
+                                           "excelvis", "position=", "timerange", "steptime=", "clipboard",
+                                           "format=", "ppst=", "attitude=", "notice", "help"])
         # print(opt)
         # print(timeargs)
         metvalues = [swutil.string2met(a, correct=True) for a in timeargs]
-        for o, v in opt:  # option value
+        for (o, v) in opt:  # option value
             if o in ("-v", "--verbose"):
                 verbose = True
                 print(" ".join(argv))
             elif o in ("--terse"):
                 terse = True
             elif o in ("-o", "--orbit"):
                 orbits = orbit()
@@ -992,25 +1057,21 @@
                     # print(v)
                     s = sourcecat.byName(v)
                     # print(s)
                     sources.append(s)
                 except:
                     m = radecnameRE.match(v)
                     if m:
-                        s = (
-                            "|||"
-                            + v
-                            + ("||0||||%(rastring)s|%(decstring)s|" % m.groupdict())
-                        )
+                        s = "|||" + v + ("||0||||%(rastring)s|%(decstring)s|" % m.groupdict())
                         sources.append(source(s))
                     else:
                         print("Source %s not found in catalog" % v)
                         return
             elif o in ("-S", "--sun", "--Sun"):
-                s = sunsource()
+                s = source("Sun")
                 sources.append(s)
             elif "--visible".startswith(o):
                 visible_only = True
             elif o in ("-t", "--timerange"):
                 timerange = True
             elif o in ("--steptime",):
                 timestep = datetime.timedelta(seconds=float(v))
@@ -1022,16 +1083,16 @@
                             metvalues.append(t)
                     except:
                         pass
             elif o in ("-f", "--format"):
                 format = v
             elif o in ("-p", "--position"):
                 try:
-                    ra, dec = [float(s) for s in v.translate(split_translate).split()]
-                    string = "|||%s||%d||||%f|%f|" % (v, len(sources), ra, dec)
+                    ra, dec = [ephem.degrees(s) for s in v.translate(split_translate).split()]
+                    string = "|||%s||%d||||%f|%f|" % (v, len(sources), ra / ephem.degree, dec / ephem.degree)
                     newsource = source(string)
                     sources.append(newsource)
                 except:
                     print("Could not add source at position " + v)
                     return
             elif o in ("-P", "--ppst"):
                 ppstfile.append(v)
@@ -1043,96 +1104,54 @@
                     roll = float(vsplit[2])
                 except:
                     print("Could not get ra,dec,roll out of argument '%s'" % (v,))
                     usage(argv[0])
                     return
                 ztime = datetime.datetime(2000, 1, 1, 0, 0, 0)
                 manualAttitudes.append(
-                    PointingEntry(
-                        ztime,
-                        ztime,
-                        ztime,
-                        ra,
-                        dec,
-                        roll,
-                        0,
-                        0,
-                        "(from command line)",
-                        False,
-                    )
-                )
+                    pointingEntry(ztime, ztime, ztime, ra, dec, roll, 0, 0, "(from command line)", False))
             elif o in ("--notice",):
                 (ra, dec, met) = parseNotice(sys.stdin)
                 metvalues.append(met)
                 if ra != None and dec != None:
-                    string = "|||%.2f_%.2f||%d||||%f|%f|" % (
-                        ra,
-                        dec,
-                        len(sources),
-                        ra,
-                        dec,
-                    )
+                    string = "|||%.2f_%.2f||%d||||%f|%f|" % (ra, dec, len(sources), ra, dec)
                     newsource = source(string)
                     sources.append(newsource)
             elif o in ("-x", "--excelvis"):
                 excelvis = True
             elif o in ("-h", "--help"):
                 usage(argv[0])
                 return
 
-        if debug:
-            debug.write("Arguments processed\n")
+        if debug: debug.write("Arguments processed\n")
 
-        # thePointingTable = pointingTable(ppstfile)
+        thePointingTable = pointingTable(ppstfile)
 
-        if debug:
-            debug.write("Pointing table received \n")
+        if debug: debug.write("Pointing table received \n")
 
         if timerange:
-            pytimes = (
-                swutil.met2datetime(min(metvalues), correct=True),
-                swutil.met2datetime(max(metvalues), correct=True),
-            )
+            pytimes = (swutil.met2datetime(min(metvalues), correct=True),
+                       swutil.met2datetime(max(metvalues), correct=True))
             print("Time range = %s - %s " % pytimes)
             # print(thePointingTable.getPointings(pytimes))
             # Get the METs of the middles of the observations
-            pointings = PointingEntry.listfortimes(pytimes, allinrange=True)
-            metvalues = [
-                swutil.datetime2met(
-                    p._tstart
-                    + datetime.timedelta(
-                        seconds=(p._tend - p._tstart).total_seconds() / 2.0
-                    ),
-                    correct=True,
-                )
-                for p in pointings
-            ]
+            metvalues = [swutil.datetime2met(p._tstart +
+                                             datetime.timedelta(seconds=
+                                                                (p._tend - p._tstart).total_seconds() / 2.0),
+                                             correct=True)
+                         for p in thePointingTable.getPointings(pytimes)]
 
         if timestep:
-            pytimes = (
-                swutil.met2datetime(min(metvalues), correct=True),
-                swutil.met2datetime(max(metvalues), correct=True),
-            )
-            print(
-                "Time range = %s - %s by %f seconds"
-                % (pytimes + (timestep.total_seconds(),))
-            )
-
-            metvalues = [
-                swutil.datetime2met(pytimes[0] + i * timestep, correct=True)
-                for i in range(
-                    1
-                    + int(
-                        np.ceil(
-                            (pytimes[1] - pytimes[0]).total_seconds()
-                            / timestep.total_seconds()
-                        )
-                    )
-                )
-            ]
+            pytimes = (swutil.met2datetime(min(metvalues), correct=True),
+                       swutil.met2datetime(max(metvalues), correct=True))
+            print("Time range = %s - %s by %f seconds" % (pytimes + (timestep.total_seconds(),)))
+
+            metvalues = [swutil.datetime2met(pytimes[0] + i * timestep, correct=True)
+                         for i in range(1 + int(math.ceil((pytimes[1] - pytimes[0]).total_seconds()
+                                                          / timestep.total_seconds())))]
             # Get the METs of the middles of the observations
 
         if excelvis:
             print("vis,Source,slewstart,slewend,obsend,exposure,elevstart,elevend")
             # Excel visibility output requires orbit information
             # to calculate elevation at start of observation=end of slew, end of observation
             if not orbits:
@@ -1143,203 +1162,122 @@
 
         if debug:
             debug.write("About to loop through metvalues: %s\n" % (metvalues,))
             debug.flush()
 
         for t in metvalues:
             pointprint = StringIO()
-            # even if visible_only, print if no sources
-            visible = len(sources) == 0
-            utcf_ = utcf(t, verbose)
-            udelta = datetime.timedelta(seconds=utcf_)
-            if hasLength(utcf_):
-                ulist = utcf_
+            visible = len(sources) == 0  # even if visible_only, print if no sources
+            u = utcf(t, verbose)
+            udelta = datetime.timedelta(seconds=u)
+            if hasLength(u):
+                ulist = u
                 tlist = t
                 pytime = [swutil.met2datetime(t_, correct=True) for t_ in t]
                 pystarttime = pytime[0]
             else:
-                ulist = [utcf_]
+                ulist = [u]
                 tlist = [t]
                 pytime = swutil.met2datetime(t, correct=True)
                 pystarttime = pytime
             for i in range(len(ulist)):
                 if not terse:
-                    print("Time(MET + UTCF -> UT):   ", file=pointprint, end="")
-                print(
-                    "%.3f + %.3f -> %s"
-                    % (
-                        tlist[i] + 5e-4,
-                        ulist[i],
-                        swutil.met2fitsString(
-                            tlist[i], milliseconds=True, correct=True, format=format
-                        ),
-                    ),
-                    file=pointprint,
-                )
+                    print("Time(MET + UTCF -> UT):   ", file=pointprint, end='')
+                print("%.3f + %.3f -> %s" % (tlist[i] + 5e-4, ulist[i],
+                                             swutil.met2fitsString(tlist[i], milliseconds=True, correct=True,
+                                                                   format=format)), file=pointprint)
                 if not terse:
-                    print(
-                        swutil.met2fitsString(
-                            tlist[i],
-                            milliseconds=True,
-                            correct=True,
-                            format="YYMMDD_SOD:                   %y%m%d_%q       DOY=%j",
-                        ),
-                        file=pointprint,
-                    )
+                    print(swutil.met2fitsString(tlist[i], milliseconds=True, correct=True,
+                                                format="YYMMDD_SOD:                   %y%m%d_%q       DOY=%j"),
+                          file=pointprint)
             if manualAttitudes:
                 pointings = manualAttitudes
             else:
-                pointings = PointingEntry.listfortimes([pytime])
+                pointings = thePointingTable.getPointings(pytime)
             if orbits:
                 if debug:
-                    debug.write(
-                        "About to get the satellite position for %s\n" % (pystarttime,)
-                    )
+                    debug.write("About to get the satellite position for %s\n" % (pystarttime,))
                     debug.flush()
-                sat, satpos = orbits.getSatellite(pystarttime)
-                satra, satdec, satradius = satpos.radec()
-                satlat, satlon = sf_api.wgs84.latlon_of(satpos)
+                sat = orbits.getSatellite(pystarttime)
                 if debug:
                     debug.write("Got the satellite position\n")
                     debug.flush()
                 if terse:
-                    print(
-                        "Satellite zenith RA=%.2f, dec=%.2f, lat=%.2f N, lon=%.2f E"
-                        % (
-                            satra._degrees,
-                            satdec.degrees,
-                            satlat.degrees,
-                            satlon.degrees,
-                        )
-                    )
+                    print("Satellite zenith RA=%.2f, dec=%.2f, lat=%.2f N, lon=%.2f E" % (
+                        sat.a_ra * r2d, sat.a_dec * r2d, sat.sublat * r2d, sat.sublong * r2d))
                 else:
-                    print(
-                        "Swift Zenith(RA,dec):         %.2f, %.2f"
-                        % (satra._degrees, satdec.degrees)
-                    )
-                    print(
-                        "Swift Location(lon,lat,alt):  %.2f E, %.2f N, %.0f km"
-                        % (
-                            satlon.degrees,
-                            satlat.degrees,
-                            (satradius.km - u.earthRad.to("km")),
-                        )
-                    )
+                    print("Swift Zenith(RA,dec):         %.2f, %.2f" % (sat.a_ra * r2d, sat.a_dec * r2d))
+                    print("Swift Location(lon,lat,alt):  %.2f E, %.2f N, %.0f km" % (
+                        sat.sublong * r2d, sat.sublat * r2d, sat.elevation / 1000))
             for p in pointings:
                 if not excelvis:
                     if terse:
                         print(p, file=pointprint)
                     else:
-                        print(
-                            "Obs Sequence Number:          %08d%03d"
-                            % (p._obs, p._segment),
-                            file=pointprint,
-                        )
-                        print(
-                            "Obs Target Name:              %s%s"
-                            % (p._sourcename, (" (planned)" if p._planned else "")),
-                            file=pointprint,
-                        )
-                        print(
-                            "Obs Date and Times:           %s - %s"
-                            % (
-                                (p._tstart + udelta).strftime("%Y-%m-%d   %H:%M:%S"),
-                                (p._tend + udelta).strftime("%H:%M:%S"),
-                            ),
-                            file=pointprint,
-                        )
-                        print(
-                            "Obs Pointing(ra,dec,roll):    %.3f, %.3f, %.2f"
-                            % (p._ra, p._dec, p._roll),
-                            file=pointprint,
-                        )
+                        print("Obs Sequence Number:          %08d%03d" % (p._obs, p._segment), file=pointprint)
+                        print("Obs Target Name:              %s%s" % (
+                            p._sourcename, (" (planned)" if p._planned else "")), file=pointprint)
+                        print("Obs Date and Times:           %s - %s" % (
+                            (p._tstart + udelta).strftime("%Y-%m-%d   %H:%M:%S"),
+                            (p._tend + udelta).strftime("%H:%M:%S")),
+                              file=pointprint)
+                        print("Obs Pointing(ra,dec,roll):    %.3f, %.3f, %.2f" % (p._ra, p._dec, p._roll),
+                              file=pointprint)
                 for s in sources:
                     try:
                         s.compute(pystarttime)
                         theta, phi = s.thetangle_phi(p._ra, p._dec, p._roll)
                         # print("exp,cosangle = ",s.exposure(p._ra, p._dec, p._roll) )
                         exp, cosangle = s.exposure(p._ra, p._dec, p._roll)
                         visible = visible or (exp > 0)
                         if orbits:
-                            (elev, _, description) = lineofsight(satpos, s)
+                            (elev, losheight, description) = lineofsight(sat, s)
                             relhoriz = " (%s)" % (description,)
                         else:
                             relhoriz = ""
                         if terse:
-                            print(
-                                "%s: (theta,phi) = (%.4f, %.4f); exposure = %.0f cm^2%s"
-                                % (
-                                    s.name,
-                                    theta.deg,
-                                    phi.wrap_at(180 * u.deg).deg,
-                                    exp * cosangle,
-                                    relhoriz,
-                                ),
-                                file=pointprint,
-                            )
+                            print("%s: (theta,phi) = (%.4f, %.4f); exposure = %.0f cm^2%s" % (
+                                s.name, theta, ephem.degrees(phi).znorm, exp * cosangle, relhoriz), file=pointprint)
                         elif excelvis:
-                            (elevstart, _, descriptionstart) = lineofsight(
-                                orbits.getSatellite(p._tslewend)[1], s
-                            )
-                            (elevend, _, descriptionend) = lineofsight(
-                                orbits.getSatellite(p._tend)[1], s
-                            )
-                            print(
-                                "vis,%s,%s,%s,%s,%.0f,%.1f,%.1f"
-                                % (
-                                    s.name,
-                                    p._tstart.strftime("%Y-%m-%d %H:%M:%S"),
-                                    p._tslewend.strftime("%Y-%m-%d %H:%M:%S"),
-                                    p._tend.strftime("%Y-%m-%d %H:%M:%S"),
-                                    exp * cosangle,
-                                    elevstart,
-                                    elevend,
-                                ),
-                                file=pointprint,
-                            )
+                            (elevstart, losheightstart, descriptionstart) = lineofsight(
+                                orbits.getSatellite(p._tslewend), s)
+                            (elevend, losheightend, descriptionend) = lineofsight(orbits.getSatellite(p._tend), s)
+                            print("vis,%s,%s,%s,%s,%.0f,%.1f,%.1f" % (s.name,
+                                                                      p._tstart.strftime("%Y-%m-%d %H:%M:%S"),
+                                                                      p._tslewend.strftime("%Y-%m-%d %H:%M:%S"),
+                                                                      p._tend.strftime("%Y-%m-%d %H:%M:%S"),
+                                                                      exp * cosangle,
+                                                                      elevstart,
+                                                                      elevend), file=pointprint)
                         else:
-                            print(
-                                "%s_imageloc (boresight_dist, angle): (%.0f, %.0f)"
-                                % (s.name, theta.deg, phi.wrap_at(180 * u.deg).deg),
-                                file=pointprint,
-                            )
-                            print(
-                                "%s_exposure (cm^2 cos adjusted): %.0f"
-                                % (s.name, exp * cosangle),
-                                file=pointprint,
-                            )
+                            print("%s_imageloc (boresight_dist, angle): (%.0f, %.0f)" % (
+                                s.name, theta * r2d, ephem.degrees(phi).znorm * r2d), file=pointprint)
+                            print("%s_exposure (cm^2 cos adjusted): %.0f" % (s.name, exp * cosangle), file=pointprint)
                             if len(relhoriz) > 3:
-                                print(
-                                    "%s_altitude: %.0f (%s)"
-                                    % (s.name, elev, description),
-                                    file=pointprint,
-                                )
+                                print("%s_altitude: %.0f (%s)" % (s.name, elev, description), file=pointprint)
                     except:
                         traceback.print_exc()
                         # traceback.print_tb(sys.exc_info()[2])
-                        print(str(s.catnum) + "ran into trouble in calculations")
+                        print(s.catnum + "ran into trouble in calculations")
                         return
             if visible or not visible_only:
                 sys.stdout.write(pointprint.getvalue())
-    except getopt.GetoptError:
-        usage(argv[0])
     except:
         usage(argv[0])
         traceback.print_exc()
-        if debug:
-            traceback.print_exc(None, debug)
+        if debug: traceback.print_exc(None, debug)
         # traceback.print_tb(sys.exc_info()[2])
     if debug:
         debug.write("%s: swinfo main() completed\n" % (datetime.datetime.now(),))
         debug.flush()
 
 
 def checkParse():
-    """Go through all the parsed mail messages to see which ones weren't parsed properly"""
-    for f in glob.glob("/tmp/latesttrigger.*.processed"):
+    """ Go through all the parsed mail messages to see which ones weren't parsed properly"""
+    for f in glob.glob('/tmp/latesttrigger.*.processed'):
         parsed = parseNotice(open(f).readlines())
         if len(parsed) != 3 or parsed[2] < 3e8:
             print("%s %s" % (f, parsed))
 
 
 if __name__ == "__main__":
     # for i in range(len(sys.argv)) :
@@ -1347,10 +1285,10 @@
     # Turn on debugging
     debug = None
     debug = open("/tmp/swinfo.debug", "a")
     # if debug:
     #     swutil.dumponsignal(fname="/tmp/swinfo.debug")
     #     main = swutil.TeeStdoutDecorator(main, debug)
     if len(sys.argv) > 1:
-        swinfo_main(sys.argv, debug=debug)
+        main(sys.argv, debug=debug)
     else:
-        swinfo_main([l for l in os.popen("/usr/bin/pbpaste | tr '\r' '\n'")])
+        main([l for l in os.popen("/usr/bin/pbpaste | tr '\r' '\n'")])
```

### Comparing `swiftbat-0.1.4/swiftbat/swutil.py` & `swiftbat-0.1a15/swiftbat/swutil.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 #! /usr/bin/env python
 
+from __future__ import print_function, division, absolute_import
+
 """
 swutil
 Utilities for dealing with Swift Data
 Python datatime objects are UTC, MET is spacecraft MET which needs application of UTCF to get datetime
 David Palmer   palmer@lanl.gov
 
 """
@@ -35,96 +37,65 @@
 
 This code was developed using funding from the National Aeronautics and Space Administration (NASA).
 
 """
 
 import os
 import sys
+
+# print __file__
+# add the path of this module to the searchpath to let helpers in 
+execdir = os.path.dirname(os.path.abspath(os.path.realpath(__file__)))
+if not execdir in map(os.path.abspath, sys.path):
+    sys.path.append(execdir)
+
 import re
 import datetime
 from .clockinfo import utcf
 import io
 
 # 2004-12-05T19:43:27
 refitstime = re.compile(
     r"(?P<year>[0-9]{4,4})-(?P<month>[0-9]{1,2})-(?P<day>[0-9]{1,2})([T ]+(?P<hour>[0-9]{1,2}):(?P<minute>[0-9]{2,2})(:(?P<second>[0-9]{2,2})([.](?P<fracsecond>[0-9]*))?)?)?",
-    re.I,
-)
+    re.I)
 # 2004:329:12:15:07
 redoytime = re.compile(
-    r"(?P<year>[0-9]{4,4}):(?P<doy>[0-9]{3,3})(:(?P<hour>[0-9]{2,2}):(?P<minute>[0-9]{2,2})(:(?P<second>[0-9]{2,2})([.](?P<fracsecond>[0-9]*))?)?)?"
-)
+    r"(?P<year>[0-9]{4,4}):(?P<doy>[0-9]{3,3})(:(?P<hour>[0-9]{2,2}):(?P<minute>[0-9]{2,2})(:(?P<second>[0-9]{2,2})([.](?P<fracsecond>[0-9]*))?)?)?")
 # JD2454192.8273
 rejdtime = re.compile(r"JD[ ]*24(?P<mytruncjd>[0-9]+(.[0-9]*)?)", re.I)
 # MJD14192.5273
 remjdtime = re.compile(r"MJD[ ]*(?P<mjd>[0-9]+(.[0-9]*)?)", re.I)
 # 140308_13764   IPN seconds of day type format
-reIPNsod = re.compile(
-    r"(?P<year>[0-9]{2,4})-?(?P<month>[0-9]{2})-?(?P<day>[0-9]{2})_(T?)(?P<sod>[0-9]{5}(\.[0-9]*)?)"
-)
+reIPNsod = re.compile(r"(?P<year>[0-9]{2,4})-?(?P<month>[0-9]{2})-?(?P<day>[0-9]{2})_(T?)(?P<sod>[0-9]{5}(\.[0-9]*)?)")
 # General time with multiple options for date and time
 # Using slashes to separate ymd is disallowed because it could also
 # be m/d/y or d/m/y.  '-' or nothing may be (consistently) used
 # ydoy , y-doy or y:doy allowed with y 2 or 4 dig, doy always 3 dig
-reday_s = (
-    r"""((?P<year>(\d{2})|(\d{4}))"""  # 2 or 4 digit year
-    r"""("""  # either DOY or Month,day
-    r"""([:-]?(?P<doy>\d{3}))|"""
-    r"""((?P<ymdsep>-?)(?P<month>[0-9]{1,2})(?P=ymdsep)(?P<day>[0-9]{1,2}))))"""
-)
+reday_s = (r"""((?P<year>(\d{2})|(\d{4}))"""  # 2 or 4 digit year
+           r"""("""  # either DOY or Month,day
+           r"""([:-]?(?P<doy>\d{3}))|"""
+           r"""((?P<ymdsep>-?)(?P<month>[0-9]{1,2})(?P=ymdsep)(?P<day>[0-9]{1,2}))))""")
 # sod must be 5 integer digits plus optional decimal and fraction
-retime_s = (
-    r"[ _]*?(([ _ST](?P<sod>[0-9]{5}(\.[0-9]*)?))"
-    r"|([ _T](?P<hour>[0-9]{2})"
-    r"(?P<tsep>:?)(?P<minute>[0-9]{2})"
-    r"((?P=tsep)(?P<second>[0-9]{2}(\.[0-9]*)?))?))"
-)
+retime_s = (r"[ _]*?(([ _ST](?P<sod>[0-9]{5}(\.[0-9]*)?))"
+            r"|([ _T](?P<hour>[0-9]{2})"
+            r"(?P<tsep>:?)(?P<minute>[0-9]{2})"
+            r"((?P=tsep)(?P<second>[0-9]{2}(\.[0-9]*)?))?))")
 reGeneral = re.compile(reday_s + retime_s, re.I)
 # 2004:329:12:15:07)
 
 swiftepoch = datetime.datetime(year=2001, month=1, day=1, hour=0, minute=0, second=0)
 swiftlaunchtime = datetime.datetime(year=2004, month=11, day=20, hour=17, minute=16)
 mjdepoch = datetime.datetime(year=1858, month=11, day=17, hour=0, minute=0, second=0)
 # mytruncjd is jd with the 24 stripped off the head, but without the 0.5 day adjustment
 mytruncjdepoch = mjdepoch - datetime.timedelta(days=0.5)
-_jd_mjd_diff = 2400000.5
 
 fitstimeformat = r"%Y-%m-%dT%H:%M:%S"  # for strftime
 yearDOYsecstimeformat = r"%Y_%j_%q"  # %q -> SOD in 00000 (non-standard)
 
 
-def any2datetime(arg, correct=True, mjd=False, jd=False):
-    """Change the argument into a (naive) datetime
-
-    Understands:
-        strings as accepted by string2datetime
-        astropy, skyfield, or pyephem dates
-        int/floats representing a Swift MET (uses the 'correct' argument for utcf)
-            unless mjd or jd set (for Mod. Julian Day and Julian Day, respectively)
-        iterables of any of these, returning a list of datetimes
-    """
-    if isinstance(arg, str):
-        return string2datetime(arg, correct=correct)
-    for convname in ("to_datetime", "utc_datetime", "datetime"):
-        # astropy, skyfield, pyephem
-        if hasattr(arg, convname):
-            return getattr(arg, convname)(arg)
-    if isinstance(arg, (float, int)):
-        if mjd:
-            return mjd2datetime(arg)
-        elif jd:
-            return mjd2datetime(arg - _jd_mjd_diff)
-        else:
-            return met2datetime(arg, correct=correct)
-    try:
-        return [any2datetime(arg_, correct=True, mjd=mjd, jd=jd) for arg_ in arg]
-    except TypeError:  # Not iterable (assuming thrown by 'for')
-        pass
-
-
 def string2datetime(s, nocomplaint=False, correct=False):
     """
     Convert a string (which may be a Swift MET) to a datetime
 
     In the case of an MET, is corrected for UTCF if correct==True
     :param s: string with time information
     :param nocomplaint: Don't complain if something is wrong
@@ -133,159 +104,127 @@
     :rtype: datetime.datetime
     """
     try:
         m = reGeneral.match(s)
         if m:
             mgd = m.groupdict()
             try:
-                year = int(mgd["year"])
+                year = int(mgd['year'])
                 if year < 100:
                     # Use 1960-2060 for 2-digit years
                     year += 2000 if (year < 60) else 1900
-                if mgd["doy"] is not None:
-                    doy = int(mgd["doy"])
+                if mgd['doy'] is not None:
+                    doy = int(mgd['doy'])
                     date = datetime.date(year=year) + datetime.timedelta(days=doy - 1)
                 else:
-                    month = int(mgd["month"])
-                    day = int(mgd["day"])
+                    month = int(mgd['month'])
+                    day = int(mgd['day'])
                     date = datetime.date(year=year, month=month, day=day)
-                if mgd["sod"] is not None:
-                    addseconds = float(mgd["sod"])
+                if mgd['sod'] is not None:
+                    addseconds = float(mgd['sod'])
                     tod = datetime.time(0)
                 else:
-                    hour = int(mgd["hour"])
-                    minute = int(mgd["minute"])
+                    hour = int(mgd['hour'])
+                    minute = int(mgd['minute'])
                     try:
-                        addseconds = float(mgd["second"])
+                        addseconds = float(mgd['second'])
                     except:
                         addseconds = 0.0
                     tod = datetime.time(hour=hour, minute=minute)
-                d = datetime.datetime.combine(date, tod) + datetime.timedelta(
-                    seconds=addseconds
-                )
+                d = (datetime.datetime.combine(date, tod)
+                     + datetime.timedelta(seconds=addseconds))
                 return d
             except Exception as e:
                 print(e)
                 print("Time parser failed for {} giving {}".format(s, mgd))
         m = reIPNsod.match(s)
         if m:  # 140308_13764
             mgd = m.groupdict()
-            year = int(mgd["year"])
+            year = int(mgd['year'])
             if year < 100:
                 # Use 1960-2060 for 2-digit years
                 year += 2000 if (year < 60) else 1900
-            month = int(mgd["month"])
-            day = int(mgd["day"])
-            sod = float(mgd["sod"])
-            d = datetime.datetime(year=year, month=month, day=day) + datetime.timedelta(
-                seconds=sod
-            )
+            month = int(mgd['month'])
+            day = int(mgd['day'])
+            sod = float(mgd['sod'])
+            d = datetime.datetime(year=year, month=month, day=day) + datetime.timedelta(seconds=sod)
             return d
         m = refitstime.match(s)
         if m:  # 2004-12-05T19:43:27
             mgd = m.groupdict()
-            if mgd["fracsecond"] == None:
-                mgd["microsecond"] = 0
+            if mgd['fracsecond'] == None:
+                mgd['microsecond'] = 0
             else:
-                mgd["microsecond"] = int(1e6 * float("0." + mgd["fracsecond"]))
+                mgd['microsecond'] = int(1e6 * float("0." + mgd['fracsecond']))
             for k in mgd.keys():
                 if mgd[k]:
                     mgd[k] = int(mgd[k])
                 else:
                     mgd[k] = 0
-            d = datetime.datetime(
-                year=mgd["year"],
-                month=mgd["month"],
-                day=mgd["day"],
-                hour=mgd["hour"],
-                minute=mgd["minute"],
-                second=mgd["second"],
-                microsecond=mgd["microsecond"],
-            )
+            d = datetime.datetime(year=mgd['year'], month=mgd['month'], day=mgd['day'], hour=mgd['hour'],
+                                  minute=mgd['minute'], second=mgd['second'], microsecond=mgd['microsecond'])
             return d
         m = redoytime.match(s)
         if m:  # 2004:329:12:15:07
             mgd = m.groupdict()
-            if mgd["fracsecond"] == None:
-                mgd["microsecond"] = 0
+            if mgd['fracsecond'] == None:
+                mgd['microsecond'] = 0
             else:
-                mgd["microsecond"] = int(1e6 * float("0." + mgd["fracsecond"]))
+                mgd['microsecond'] = int(1e6 * float("0." + mgd['fracsecond']))
             for k in mgd.keys():
                 if mgd[k]:
                     mgd[k] = int(mgd[k])
                 else:
                     mgd[k] = 0
-            d = datetime.datetime(
-                year=mgd["year"],
-                month=1,
-                day=1,
-                hour=mgd["hour"],
-                minute=mgd["minute"],
-                second=mgd["second"],
-                microsecond=mgd["microsecond"],
-            )
-            d += datetime.timedelta(days=mgd["doy"] - 1)
+            d = datetime.datetime(year=mgd['year'], month=1, day=1, hour=mgd['hour'], minute=mgd['minute'],
+                                  second=mgd['second'], microsecond=mgd['microsecond'])
+            d += datetime.timedelta(days=mgd['doy'] - 1)
             return d
         m = remjdtime.match(s)
         if m:  # MJD 14192.5273
-            d = mjdepoch + datetime.timedelta(days=float(m.groupdict()["mjd"]))
+            d = mjdepoch + datetime.timedelta(days=float(m.groupdict()['mjd']))
             return d
         m = rejdtime.match(s)
-        if (
-            m
-        ):  # JD2454192.8273  Note that the 'JD24' is found by the regex, leaving the truncated JD
-            d = mytruncjdepoch + datetime.timedelta(
-                days=float(m.groupdict()["mytruncjd"])
-            )
+        if m:  # JD2454192.8273
+            d = mytruncjdepoch + datetime.timedelta(days=float(m.groupdict()['mytruncjd']))
             return d
         # None of the patterns match, try treating it as a straight number of seconds
         met = float(s)
         if correct:
             utcf_ = utcf(met, not nocomplaint, False)
             met += utcf_
         return met2datetime(met)
     except:
         if nocomplaint:
             return None
         else:
             print(
-                "Invalid time '%s'.  Valid formats: 2004-12-05T19:43:27, 2004:329:12:15:07, 123456789.01234, JD2454192.8273, MJD14192.5273, 140308_13764"
-                % (s),
-                file=sys.stderr,
-            )
+                "Invalid time '%s'.  Valid formats: 2004-12-05T19:43:27, 2004:329:12:15:07, 123456789.01234, JD2454192.8273, MJD 14192.5273, 140308_13764" % (
+                    s))
             raise
 
 
 def string2met(s, nocomplaint=False, correct=False):
     d = string2datetime(s, nocomplaint, correct=correct)
-    if d == None:
+    if (d == None):
         return 0
     else:
         return datetime2met(d, correct=correct)
 
 
-# FIXME replace with .total_seconds() throughout
 def timedelta2seconds(td):
     return td.days * 86400.0 + (td.seconds * 1.0 + td.microseconds * 1e-6)
 
 
 def met2datetime(met, correct=False):
     if correct:
         met += utcf(met, False, False)
     return swiftepoch + datetime.timedelta(seconds=met)
 
 
-def datetime2mjd(dt):
-    return (dt - mjdepoch).total_seconds() / 86400
-
-
-def mjd2datetime(mjd):
-    return mjdepoch + datetime.timedelta(days=mjd)
-
-
 def datetime2met(dt, correct=False):
     met = timedelta2seconds(dt - swiftepoch)
     if correct:
         met -= utcf(met, False, False)
     return met
 
 
@@ -293,17 +232,15 @@
     d = met2datetime(met, correct=correct)
     if milliseconds:
         ms_string = ".%03d" % min(int(d.microsecond / 1000.0 + 0.5), 999)
     else:
         ms_string = ""
     qspformat = format.split("%q")  # Handle the %q -> seconds of day extension
     if len(qspformat) > 1:
-        sod_string = (
-            "%05d" % (((60 * d.hour + d.minute) * 60) + d.second,)
-        ) + ms_string
+        sod_string = ("%05d" % (((60 * d.hour + d.minute) * 60) + d.second,)) + ms_string
         s = sod_string.join([d.strftime(subformat) for subformat in qspformat])
     else:
         s = d.strftime(format) + ms_string
     return s
 
 
 def met2mjd(met, correct=False):
@@ -311,15 +248,15 @@
         met += utcf(met, False, False)
     deltamjd = swiftepoch - mjdepoch
     mjd = met / 86400.0 + deltamjd.days + deltamjd.seconds / 86400.0
     return mjd
 
 
 def removeNonAscii(s):
-    """Useful utilitiy to fix up, e.g. email files"""
+    """ Useful utilitiy to fix up, e.g. email files"""
     # http://stackoverflow.com/questions/1342000/how-to-replace-non-ascii-characters-in-string
     return "".join(i for i in s if ord(i) < 128)
 
 
 def findInSearchPath(envname, pathlist, basename):
     """
     Look for file: If ${envname} in in environment, return it, else search
@@ -385,15 +322,14 @@
         return new_f
 
     return decorate
 
 
 # Decorator to tee stdout to an open file
 
-
 def TeeStdoutDecorator(fn, __teefile):
     def inner(*args, **kwargs):
         ostdout = sys.stdout
         try:
             sys.stdout = TeeFile(__teefile, sys.stdout)
             ret = fn(*args, **kwargs)
             sys.stdout = ostdout
@@ -406,61 +342,51 @@
 
 
 def testTeeStdoutDecorator():
     def testTeeStdoutUndecorated(x):
         print(x)
         print(1 / x)
 
-    testTeeStdout = TeeStdoutDecorator(
-        testTeeStdoutUndecorated, open("/tmp/teetest", "a")
-    )
+    testTeeStdout = TeeStdoutDecorator(testTeeStdoutUndecorated, open('/tmp/teetest', 'a'))
     testTeeStdout(5)
     testTeeStdout(0)
 
 
 # http://stackoverflow.com/questions/132058/showing-the-stack-trace-from-a-running-python-application
-#
-def dumponsignal(fname="/tmp/python_trace"):
+# 
+def dumponsignal(fname='/tmp/python_trace'):
     import threading, sys, traceback
-
     def dumpstacks(signal, frame):
         id2name = dict([(th.ident, th.name) for th in threading.enumerate()])
         code = []
         for threadId, stack in sys._current_frames().items():
             code.append("\n# Thread: %s(%d)" % (id2name.get(threadId, ""), threadId))
             for filename, lineno, name, line in traceback.extract_stack(stack):
                 code.append('File: "%s", line %d, in %s' % (filename, lineno, name))
                 if line:
                     code.append("  %s" % (line.strip()))
         print("\n".join(code))
-        open(fname, "a").write("\n".join(code))
+        open(fname, 'a').write("\n".join(code))
 
     import signal
-
     signal.signal(signal.SIGQUIT, dumpstacks)
 
 
 def main(argv):
     for s in argv:
-        print(
-            "%-30s -> %23s (corrected) = MET %f"
-            % (s, string2datetime(s, False, True), datetime2met(string2datetime(s)))
-        )
+        print("%-30s -> %23s (corrected) = MET %f" % (
+        s, string2datetime(s, False, True), datetime2met(string2datetime(s))))
 
 
 if __name__ == "__main__":
     if len(sys.argv) > 1:
         main(sys.argv[1:])
     else:
-        main(
-            [
-                "20041225_S12345.67",
-                "2004-12-25_12345",
-                "20041225_12345",
-                "2004-12-25_12345.67",
-                "2004-12-05T19:43:27.23",
-                "2004-12-25",
-                "2004:329:12:15:07.45",
-                "123456789.01234",
-                "20041225_S12345.67",
-            ]
-        )
+        main(['20041225_S12345.67',
+              '2004-12-25_12345',
+              '20041225_12345',
+              '2004-12-25_12345.67',
+              '2004-12-05T19:43:27.23',
+              '2004-12-25',
+              '2004:329:12:15:07.45',
+              '123456789.01234',
+              '20041225_S12345.67'])
```

### Comparing `swiftbat-0.1.4/swiftbat.egg-info/PKG-INFO` & `swiftbat-0.1a15/swiftbat.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: swiftbat
-Version: 0.1.4
+Version: 0.1a15
 Summary: Routines for dealing with data from BAT on the Neil Gehrels Swift Observatory
 Home-page: https://github.com/lanl/swiftbat_python/
-Download-URL: https://github.com/lanl/swiftbat_python/archive/refs/tags/v0.1.4.tar.gz
 Author: David M. Palmer
 Author-email: palmer@lanl.gov
 License: BSD-3-Clause
-Classifier: Development Status :: 4 - Beta
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Astronomy
-Requires-Python: >=3.9
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Swiftbat is a set of Python library routines and command-line utilities that have been developed for the purpose
 of retrieving, analyzing, and displaying data from NASA's Swift spacecraft, especially the data from the
 Swift Burst Alert Telescope (BAT). Development started before the launch of Swift for private use by the
 author and was how he learned Python. As a result, it is not a well-packaged, well-written, coherent library.
@@ -49,7 +49,9 @@
 Obs Date and Times:           2020-05-05   12:32:37 - 13:01:34
 Obs Pointing(ra,dec,roll):    293.724, 21.897, 62.77
 Cyg_X-1_imageloc (boresight_dist, angle): (14, -133)
 Cyg_X-1_exposure (cm^2 cos adjusted): 4230
 Cyg_X-1_altitude: 29 (up)
 ```
 Use `swinfo --help` for more details.
+
+
```

