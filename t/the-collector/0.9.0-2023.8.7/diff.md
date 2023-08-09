# Comparing `tmp/the_collector-0.9.0.tar.gz` & `tmp/the_collector-2023.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "the_collector-0.9.0.tar", max compression
+gzip compressed data, was "the_collector-2023.8.7.tar", max compression
```

## Comparing `the_collector-0.9.0.tar` & `the_collector-2023.8.7.tar`

### file list

```diff
@@ -1,17 +1,10 @@
--rw-r--r--   0        0        0     1070 2021-11-25 03:56:15.956306 the_collector-0.9.0/LICENSE
--rw-r--r--   0        0        0     1214 2021-11-25 04:25:28.797256 the_collector-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     6327 2021-11-25 03:56:16.013522 the_collector-0.9.0/readme.md
--rw-r--r--   0        0        0      950 2021-11-25 04:25:20.012746 the_collector-0.9.0/the_collector/__init__.py
--rw-r--r--   0        0        0     3283 2021-11-25 03:56:16.016001 the_collector-0.9.0/the_collector/archive/BagReader.py
--rw-r--r--   0        0        0     5459 2021-11-25 03:56:16.016324 the_collector-0.9.0/the_collector/archive/BagWriter.py
--rwxr-xr-x   0        0        0     6606 2021-11-25 03:56:16.016605 the_collector-0.9.0/the_collector/archive/bagitjson.py
--rwxr-xr-x   0        0        0     1662 2021-11-25 03:58:28.208955 the_collector-0.9.0/the_collector/archive/circular_buffer.py
--rw-r--r--   0        0        0     1285 2021-11-25 03:56:16.018113 the_collector-0.9.0/the_collector/archive/extra_msgpack.py
--rw-r--r--   0        0        0     9857 2021-11-25 03:56:16.016802 the_collector-0.9.0/the_collector/archive/messages.py
--rw-r--r--   0        0        0     1798 2021-11-25 03:56:16.018839 the_collector-0.9.0/the_collector/archive/utils.py
--rw-r--r--   0        0        0     3188 2021-11-25 04:15:52.585221 the_collector-0.9.0/the_collector/bagit.py
--rw-r--r--   0        0        0      671 2021-11-25 04:01:01.902081 the_collector-0.9.0/the_collector/data.py
--rw-r--r--   0        0        0      744 2021-11-25 03:56:16.018387 the_collector-0.9.0/the_collector/extra_numpy.py
--rw-r--r--   0        0        0     2032 2021-11-25 04:15:21.851007 the_collector-0.9.0/the_collector/protocols.py
--rw-r--r--   0        0        0     7231 2021-11-25 04:26:05.414610 the_collector-0.9.0/setup.py
--rw-r--r--   0        0        0     7422 2021-11-25 04:26:05.415262 the_collector-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-08-09 02:02:54.056656 the_collector-2023.8.7/LICENSE
+-rw-r--r--   0        0        0     1196 2023-08-09 02:15:00.309007 the_collector-2023.8.7/pyproject.toml
+-rw-r--r--   0        0        0     3502 2023-08-09 02:47:08.661105 the_collector-2023.8.7/readme.md
+-rw-r--r--   0        0        0      836 2023-08-09 02:16:05.115328 the_collector-2023.8.7/the_collector/__init__.py
+-rw-r--r--   0        0        0     3360 2023-08-09 02:18:54.103485 the_collector-2023.8.7/the_collector/bagit.py
+-rw-r--r--   0        0        0      711 2023-08-09 02:19:08.578507 the_collector-2023.8.7/the_collector/data.py
+-rw-r--r--   0        0        0      792 2023-08-09 02:19:21.096384 the_collector-2023.8.7/the_collector/extra_numpy.py
+-rw-r--r--   0        0        0     2152 2023-08-09 02:19:31.422913 the_collector-2023.8.7/the_collector/protocols.py
+-rw-r--r--   0        0        0     4290 2023-08-09 02:20:42.288707 the_collector-2023.8.7/the_collector/ver_2/collector.py
+-rw-r--r--   0        0        0     4494 1970-01-01 00:00:00.000000 the_collector-2023.8.7/PKG-INFO
```

### Comparing `the_collector-0.9.0/LICENSE` & `the_collector-2023.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `the_collector-0.9.0/pyproject.toml` & `the_collector-2023.8.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 [tool.poetry]
 name = "the_collector"
-version = "0.9.0"
-description = "A library to store robot data in common formats"
+version = "2023.08.07"
+description = "A library to store data in common formats"
 authors = ["walchko <walchko@users.noreply.github.com>"]
 readme = "readme.md"
 license = "MIT"
 homepage = "https://pypi.org/project/the-collector/"
 repository = 'http://github.com/MomsFriendlyRobotCompany/the_collector'
 # documentation = "http://..."
-keywords = ['library', 'robotics', 'robot', 'storage', 'json', 'pickle']
+keywords = ['library', 'robotics', 'robot', 'storage', 'json', 'pickle', "gzip", "csv"]
 classifiers = [
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
-    'Programming Language :: Python :: 3.8',
-    'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
     'Topic :: Software Development :: Libraries',
     'Topic :: Software Development :: Libraries :: Python Modules',
     'Topic :: Software Development :: Libraries :: Application Frameworks'
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8"
-numpy = { version = "*", optional = true }
+python = ">=3.10"
+# numpy = { version = "*", optional = true }
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
 
-[tool.poetry.extras]
-numpy = ["numpy"]
+# [tool.poetry.extras]
+# numpy = ["numpy"]
 
 [build-system]
-requires = ["poetry>=1.0.0"]
+requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `the_collector-0.9.0/the_collector/bagit.py` & `the_collector-2023.8.7/the_collector/bagit.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,104 +1,104 @@
-##############################################
-# The MIT License (MIT)
-# Copyright (c) 2017 Kevin Walchko
-# see LICENSE for full details
-##############################################
-from the_collector.protocols import Pickle, Json
-import datetime
-from collections import defaultdict
-import os
-
-
-class BagIt(object):
-    """
-    """
-    __slots__ = ('buffer', 'packer')
-
-    def __init__(self, packer):
-        """
-        filename: either a string containing the desired file name (note that
-          .bag is appended) OR a file-like object from io.Bytes or something
-        buffer_size: number of Bytes, default 10MB
-        """
-        # self.buffer = {}
-        self.buffer = defaultdict(list)
-        self.packer = packer()
-        # print(">> ", self.packer.proto)
-
-    def __del__(self):
-        # self.write()  # this kills me on BytesIO, it closes the buffer
-        pass
-
-    def info(self):
-        print('Bag keys:')
-        print('-'*50)
-        for k in self.buffer.keys():
-            print(f'  {k:>10}: {len(self.buffer[k]):<7}')
-
-    def fill(self, data):
-        """
-        Clears buffer and fills it data (dictionary)
-        """
-        if not isinstance(data, dict):
-            raise Exception(f"data is not a dict, it is: {type(data)}")
-
-        self.buffer.clear()
-        print(".fill() ----------------------------")
-        for key, val in data.items():
-            print("- {key}: {len(val)}")
-            for v in val:
-                self.push(key, v)
-
-    def push(self, key, msg):
-        """
-        Push another message and a key into the buffer. Once the buffer limit
-        is reached it is written to a file.
-        """
-        # if key not in self.buffer.keys():
-        #     self.buffer[key] = []
-
-        self.buffer[key].append(msg)
-
-    def write(self, filename='data', timestamp=True):
-        filename = os.path.expanduser(filename)
-        if len(self.buffer) == 0:
-            return None
-
-        if timestamp:
-            dt = str(datetime.datetime.now()).replace(' ', '-')
-            filename = f"{filename}.{dt}.{self.packer.proto}.bag"
-        else:
-            filename = f"{filename}.{self.packer.proto}.bag"
-
-        with open(filename, 'wb') as fd:
-            d = self.packer.pack(self.buffer)
-            fd.write(d)
-
-        # self.buffer = {}
-        self.buffer.clear()
-
-        return filename
-
-    def read(self, filename):
-        """
-        Given a filename, it opens it and read all data into memory and return
-        Inputs:
-          filename - name of file
-        Return:
-          dict() with keys for each recorded data stream and a list/tuple of
-          data points
-        """
-        filename = os.path.expanduser(filename)
-        t = filename.split('.')
-        p = t[-2]
-
-        if p in ['msgpack', 'pickle', 'json', "json-gz"]:
-            print(f">> Reading[{p}]: {filename}")
-            if p != self.packer.proto:
-                raise Exception(f"File is {p} protocol, this Bagit is {self.packer.proto}")
-
-            return self.packer.unpack(filename)
-        else:
-            raise Exception("Couldn't determine protocol of file:", filename)
+# ##############################################
+# # The MIT License (MIT)
+# # Copyright (c) 2017 Kevin Walchko
+# # see LICENSE for full details
+# ##############################################
+# from the_collector.protocols import Pickle, Json
+# import datetime
+# from collections import defaultdict
+# import os
+
+
+# class BagIt(object):
+#     """
+#     """
+#     __slots__ = ('buffer', 'packer')
+
+#     def __init__(self, packer):
+#         """
+#         filename: either a string containing the desired file name (note that
+#           .bag is appended) OR a file-like object from io.Bytes or something
+#         buffer_size: number of Bytes, default 10MB
+#         """
+#         # self.buffer = {}
+#         self.buffer = defaultdict(list)
+#         self.packer = packer()
+#         # print(">> ", self.packer.proto)
+
+#     def __del__(self):
+#         # self.write()  # this kills me on BytesIO, it closes the buffer
+#         pass
+
+#     def info(self):
+#         print('Bag keys:')
+#         print('-'*50)
+#         for k in self.buffer.keys():
+#             print(f'  {k:>10}: {len(self.buffer[k]):<7}')
+
+#     def fill(self, data):
+#         """
+#         Clears buffer and fills it data (dictionary)
+#         """
+#         if not isinstance(data, dict):
+#             raise Exception(f"data is not a dict, it is: {type(data)}")
+
+#         self.buffer.clear()
+#         print(".fill() ----------------------------")
+#         for key, val in data.items():
+#             print("- {key}: {len(val)}")
+#             for v in val:
+#                 self.push(key, v)
+
+#     def push(self, key, msg):
+#         """
+#         Push another message and a key into the buffer. Once the buffer limit
+#         is reached it is written to a file.
+#         """
+#         # if key not in self.buffer.keys():
+#         #     self.buffer[key] = []
+
+#         self.buffer[key].append(msg)
+
+#     def write(self, filename='data', timestamp=True):
+#         filename = os.path.expanduser(filename)
+#         if len(self.buffer) == 0:
+#             return None
+
+#         if timestamp:
+#             dt = str(datetime.datetime.now()).replace(' ', '-')
+#             filename = f"{filename}.{dt}.{self.packer.proto}.bag"
+#         else:
+#             filename = f"{filename}.{self.packer.proto}.bag"
+
+#         with open(filename, 'wb') as fd:
+#             d = self.packer.pack(self.buffer)
+#             fd.write(d)
+
+#         # self.buffer = {}
+#         self.buffer.clear()
+
+#         return filename
+
+#     def read(self, filename):
+#         """
+#         Given a filename, it opens it and read all data into memory and return
+#         Inputs:
+#           filename - name of file
+#         Return:
+#           dict() with keys for each recorded data stream and a list/tuple of
+#           data points
+#         """
+#         filename = os.path.expanduser(filename)
+#         t = filename.split('.')
+#         p = t[-2]
+
+#         if p in ['msgpack', 'pickle', 'json', "json-gz"]:
+#             print(f">> Reading[{p}]: {filename}")
+#             if p != self.packer.proto:
+#                 raise Exception(f"File is {p} protocol, this Bagit is {self.packer.proto}")
+
+#             return self.packer.unpack(filename)
+#         else:
+#             raise Exception("Couldn't determine protocol of file:", filename)
 
-        # return self.packer.unpack(filename)
+#         # return self.packer.unpack(filename)
```

### Comparing `the_collector-0.9.0/the_collector/extra_numpy.py` & `the_collector-2023.8.7/the_collector/extra_numpy.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-##############################################
-# The MIT License (MIT)
-# Copyright (c) 2017 Kevin Walchko
-# see LICENSE for full details
-##############################################
-import numpy as np
+# ##############################################
+# # The MIT License (MIT)
+# # Copyright (c) 2017 Kevin Walchko
+# # see LICENSE for full details
+# ##############################################
+# import numpy as np
 
 
-def array_pack(img):
-    """
-    img: numpy array. I primarily use this for OpenCV images
-    """
-    d = img.tobytes()
-    s = img.shape
-    t = img.dtype
+# def array_pack(img):
+#     """
+#     img: numpy array. I primarily use this for OpenCV images
+#     """
+#     d = img.tobytes()
+#     s = img.shape
+#     t = img.dtype
 
-    return (s, t, d)
+#     return (s, t, d)
 
-def array_unpack(shape, data, dtype=np.uint8):
-    """
-    I primarily use this with OpenCV images, so I think in those terms
-    shape: tuple(height, width, colors)
-    dtype: numpy data type like np.uint8
-    data: byte array that needs to be turned back into an array
-    """
-    img = np.frombytes(data, dtype=dtype)
-    img.reshape(shape)
+# def array_unpack(shape, data, dtype=np.uint8):
+#     """
+#     I primarily use this with OpenCV images, so I think in those terms
+#     shape: tuple(height, width, colors)
+#     dtype: numpy data type like np.uint8
+#     data: byte array that needs to be turned back into an array
+#     """
+#     img = np.frombytes(data, dtype=dtype)
+#     img.reshape(shape)
 
-    return img
+#     return img
```

### Comparing `the_collector-0.9.0/the_collector/protocols.py` & `the_collector-2023.8.7/the_collector/protocols.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-##############################################
-# The MIT License (MIT)
-# Copyright (c) 2017 Kevin Walchko
-# see LICENSE for full details
-##############################################
-import pickle
-import io    # gzip to string
-import gzip  # compression
-
-try:
-    import simplejson as json
-except ImportError:
-    import json
-
-class Pickle:
-    __slots__ = ("proto")
-
-    def __init__(self):
-        self.proto = "pickle"
-    # proto = attr.ib(init=False, default="pickle")
-
-    def pack(self, data):
-        return pickle.dumps(data)
-
-    def unpack(self, filename):
-        # return pickle.loads(data)
-        with open(filename, 'rb') as fd:
-            data = pickle.load(fd)
-        return data
-
-
-class Json:
-    def __init__(self, compress=False, use_tuples=True):
-        self.use_tuples = use_tuples
-        self.compress(compress)
-
-
-    def compress(self, compress):
-        if compress:
-            self.proto = "json-gz"
-        else:
-            self.proto = "json"
-
-    def pack(self, data):
-        if self.proto == "json-gz":
-            # with gzip.open(filename, 'rb') as f:
-            #     data = json.load(f)
-            out = io.BytesIO()
-            with gzip.GzipFile(fileobj=out, mode='wb') as fo:
-                fo.write(json.dumps(data).encode("utf-8"))
-            return out.getvalue()
-        else:
-            return json.dumps(data).encode("utf-8")
-
-    def unpack(self, filename):
-        if self.proto == "json-gz":
-            with gzip.open(filename, 'rb') as fd:
-                data = json.load(fd)
-        else:
-            with open(filename, 'rb') as fd:
-                data = json.load(fd)
-
-        if self.use_tuples:
-            for key, val in data.items():
-                if isinstance(val[0], list):
-                    for i in range(len(val)):
-                        data[key][i] = tuple(data[key][i])
-        return data
+# ##############################################
+# # The MIT License (MIT)
+# # Copyright (c) 2017 Kevin Walchko
+# # see LICENSE for full details
+# ##############################################
+# import pickle
+# import io    # gzip to string
+# import gzip  # compression
+
+# try:
+#     import simplejson as json
+# except ImportError:
+#     import json
+
+# class Pickle:
+#     __slots__ = ("proto")
+
+#     def __init__(self):
+#         self.proto = "pickle"
+#     # proto = attr.ib(init=False, default="pickle")
+
+#     def pack(self, data):
+#         return pickle.dumps(data)
+
+#     def unpack(self, filename):
+#         # return pickle.loads(data)
+#         with open(filename, 'rb') as fd:
+#             data = pickle.load(fd)
+#         return data
+
+
+# class Json:
+#     def __init__(self, compress=False, use_tuples=True):
+#         self.use_tuples = use_tuples
+#         self.compress(compress)
+
+
+#     def compress(self, compress):
+#         if compress:
+#             self.proto = "json-gz"
+#         else:
+#             self.proto = "json"
+
+#     def pack(self, data):
+#         if self.proto == "json-gz":
+#             # with gzip.open(filename, 'rb') as f:
+#             #     data = json.load(f)
+#             out = io.BytesIO()
+#             with gzip.GzipFile(fileobj=out, mode='wb') as fo:
+#                 fo.write(json.dumps(data).encode("utf-8"))
+#             return out.getvalue()
+#         else:
+#             return json.dumps(data).encode("utf-8")
+
+#     def unpack(self, filename):
+#         if self.proto == "json-gz":
+#             with gzip.open(filename, 'rb') as fd:
+#                 data = json.load(fd)
+#         else:
+#             with open(filename, 'rb') as fd:
+#                 data = json.load(fd)
+
+#         if self.use_tuples:
+#             for key, val in data.items():
+#                 if isinstance(val[0], list):
+#                     for i in range(len(val)):
+#                         data[key][i] = tuple(data[key][i])
+#         return data
 
-    def packs(self, s):
-        raise NotImplementedError("Json.unpacks()")
+#     def packs(self, s):
+#         raise NotImplementedError("Json.unpacks()")
 
-    def unpacks(self, s):
-        raise NotImplementedError("Json.unpacks()")
+#     def unpacks(self, s):
+#         raise NotImplementedError("Json.unpacks()")
```

