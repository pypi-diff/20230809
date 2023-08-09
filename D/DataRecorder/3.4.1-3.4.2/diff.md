# Comparing `tmp/DataRecorder-3.4.1.tar.gz` & `tmp/DataRecorder-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DataRecorder-3.4.1.tar", last modified: Sat Aug  5 04:34:32 2023, max compression
+gzip compressed data, was "DataRecorder-3.4.2.tar", last modified: Wed Aug  9 01:00:34 2023, max compression
```

## Comparing `DataRecorder-3.4.1.tar` & `DataRecorder-3.4.2.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 04:34:32.273028 DataRecorder-3.4.1/
-drwxrwxrwx   0        0        0        0 2023-08-05 04:34:32.258514 DataRecorder-3.4.1/DataRecorder/
--rw-rw-rw-   0        0        0      138 2023-08-05 02:21:57.000000 DataRecorder-3.4.1/DataRecorder/__init__.py
--rw-rw-rw-   0        0        0     7043 2023-07-31 14:26:40.000000 DataRecorder-3.4.1/DataRecorder/base.py
--rw-rw-rw-   0        0        0     1967 2023-07-31 14:26:40.000000 DataRecorder-3.4.1/DataRecorder/base.pyi
--rw-rw-rw-   0        0        0     1721 2023-07-31 14:26:40.000000 DataRecorder-3.4.1/DataRecorder/byte_recorder.py
--rw-rw-rw-   0        0        0      487 2023-07-31 14:26:40.000000 DataRecorder-3.4.1/DataRecorder/byte_recorder.pyi
--rw-rw-rw-   0        0        0     5360 2023-08-05 04:20:45.000000 DataRecorder-3.4.1/DataRecorder/db_recorder.py
--rw-rw-rw-   0        0        0      929 2023-07-31 14:26:40.000000 DataRecorder-3.4.1/DataRecorder/db_recorder.pyi
--rw-rw-rw-   0        0        0    15875 2023-08-05 02:21:57.000000 DataRecorder-3.4.1/DataRecorder/filler.py
--rw-rw-rw-   0        0        0     2266 2023-08-05 02:21:57.000000 DataRecorder-3.4.1/DataRecorder/filler.pyi
--rw-rw-rw-   0        0        0     6488 2023-08-05 02:21:57.000000 DataRecorder-3.4.1/DataRecorder/recorder.py
--rw-rw-rw-   0        0        0      893 2023-08-05 02:21:57.000000 DataRecorder-3.4.1/DataRecorder/recorder.pyi
--rw-rw-rw-   0        0        0    11628 2023-08-02 15:43:22.000000 DataRecorder-3.4.1/DataRecorder/setter.py
--rw-rw-rw-   0        0        0     2839 2023-07-31 14:26:40.000000 DataRecorder-3.4.1/DataRecorder/setter.pyI
-drwxrwxrwx   0        0        0        0 2023-08-05 04:34:32.273028 DataRecorder-3.4.1/DataRecorder/style/
--rw-rw-rw-   0        0        0       77 2023-08-05 02:21:57.000000 DataRecorder-3.4.1/DataRecorder/style/__init__.py
--rw-rw-rw-   0        0        0    28558 2023-08-05 02:21:57.000000 DataRecorder-3.4.1/DataRecorder/style/cell_style.py
--rw-rw-rw-   0        0        0     8328 2023-07-31 14:26:40.000000 DataRecorder-3.4.1/DataRecorder/tools.py
--rw-rw-rw-   0        0        0      915 2023-07-31 14:26:40.000000 DataRecorder-3.4.1/DataRecorder/tools.pyi
-drwxrwxrwx   0        0        0        0 2023-08-05 04:34:32.271823 DataRecorder-3.4.1/DataRecorder.egg-info/
--rw-rw-rw-   0        0        0     4961 2023-08-05 04:34:32.000000 DataRecorder-3.4.1/DataRecorder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      657 2023-08-05 04:34:32.000000 DataRecorder-3.4.1/DataRecorder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 04:34:32.000000 DataRecorder-3.4.1/DataRecorder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-08-05 04:34:32.000000 DataRecorder-3.4.1/DataRecorder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-08-05 04:34:32.000000 DataRecorder-3.4.1/DataRecorder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1083 2022-01-26 11:22:47.000000 DataRecorder-3.4.1/LICENSE
--rw-rw-rw-   0        0        0       26 2023-03-26 03:46:04.000000 DataRecorder-3.4.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4961 2023-08-05 04:34:32.273028 DataRecorder-3.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     4462 2023-05-25 16:24:32.000000 DataRecorder-3.4.1/README.md
--rw-rw-rw-   0        0        0       42 2023-08-05 04:34:32.273028 DataRecorder-3.4.1/setup.cfg
--rw-rw-rw-   0        0        0      863 2023-08-05 04:23:24.000000 DataRecorder-3.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-09 01:00:34.437167 DataRecorder-3.4.2/
+drwxrwxrwx   0        0        0        0 2023-08-09 01:00:34.405924 DataRecorder-3.4.2/DataRecorder/
+-rw-rw-rw-   0        0        0     2858 2023-08-07 00:54:29.000000 DataRecorder-3.4.2/DataRecorder/DataRecorder按照表头自动存对应列.py
+-rw-rw-rw-   0        0        0      138 2023-08-04 02:16:31.000000 DataRecorder-3.4.2/DataRecorder/__init__.py
+-rw-rw-rw-   0        0        0     7043 2023-08-04 03:31:42.000000 DataRecorder-3.4.2/DataRecorder/base.py
+-rw-rw-rw-   0        0        0     1967 2023-08-04 03:31:42.000000 DataRecorder-3.4.2/DataRecorder/base.pyi
+-rw-rw-rw-   0        0        0     1721 2023-08-04 03:31:42.000000 DataRecorder-3.4.2/DataRecorder/byte_recorder.py
+-rw-rw-rw-   0        0        0      487 2023-08-04 03:31:42.000000 DataRecorder-3.4.2/DataRecorder/byte_recorder.pyi
+-rw-rw-rw-   0        0        0     5488 2023-08-08 03:30:22.000000 DataRecorder-3.4.2/DataRecorder/db_recorder.py
+-rw-rw-rw-   0        0        0      929 2023-08-04 03:31:42.000000 DataRecorder-3.4.2/DataRecorder/db_recorder.pyi
+-rw-rw-rw-   0        0        0    15875 2023-08-04 03:31:42.000000 DataRecorder-3.4.2/DataRecorder/filler.py
+-rw-rw-rw-   0        0        0     2266 2023-08-04 03:31:42.000000 DataRecorder-3.4.2/DataRecorder/filler.pyi
+-rw-rw-rw-   0        0        0     6488 2023-08-04 03:31:42.000000 DataRecorder-3.4.2/DataRecorder/recorder.py
+-rw-rw-rw-   0        0        0      893 2023-08-04 03:31:42.000000 DataRecorder-3.4.2/DataRecorder/recorder.pyi
+-rw-rw-rw-   0        0        0    11628 2023-08-04 03:31:42.000000 DataRecorder-3.4.2/DataRecorder/setter.py
+-rw-rw-rw-   0        0        0     2839 2023-08-04 03:31:42.000000 DataRecorder-3.4.2/DataRecorder/setter.pyI
+drwxrwxrwx   0        0        0        0 2023-08-09 01:00:34.421517 DataRecorder-3.4.2/DataRecorder/style/
+-rw-rw-rw-   0        0        0       77 2023-08-04 03:31:42.000000 DataRecorder-3.4.2/DataRecorder/style/__init__.py
+-rw-rw-rw-   0        0        0    28558 2023-08-04 03:31:42.000000 DataRecorder-3.4.2/DataRecorder/style/cell_style.py
+-rw-rw-rw-   0        0        0     8328 2023-08-04 03:31:42.000000 DataRecorder-3.4.2/DataRecorder/tools.py
+-rw-rw-rw-   0        0        0      915 2023-08-04 03:31:42.000000 DataRecorder-3.4.2/DataRecorder/tools.pyi
+drwxrwxrwx   0        0        0        0 2023-08-09 01:00:34.421517 DataRecorder-3.4.2/DataRecorder.egg-info/
+-rw-rw-rw-   0        0        0     4961 2023-08-09 01:00:33.000000 DataRecorder-3.4.2/DataRecorder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      716 2023-08-09 01:00:33.000000 DataRecorder-3.4.2/DataRecorder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-09 01:00:33.000000 DataRecorder-3.4.2/DataRecorder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-09 01:00:33.000000 DataRecorder-3.4.2/DataRecorder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-08-09 01:00:33.000000 DataRecorder-3.4.2/DataRecorder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1083 2021-08-17 07:03:54.000000 DataRecorder-3.4.2/LICENSE
+-rw-rw-rw-   0        0        0       26 2023-04-28 02:15:42.000000 DataRecorder-3.4.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4961 2023-08-09 01:00:34.437167 DataRecorder-3.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4462 2023-05-26 08:55:32.000000 DataRecorder-3.4.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-09 01:00:34.437167 DataRecorder-3.4.2/setup.cfg
+-rw-rw-rw-   0        0        0      863 2023-08-09 00:59:07.000000 DataRecorder-3.4.2/setup.py
```

### Comparing `DataRecorder-3.4.1/DataRecorder/base.py` & `DataRecorder-3.4.2/DataRecorder/base.py`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.1/DataRecorder/base.pyi` & `DataRecorder-3.4.2/DataRecorder/base.pyi`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.1/DataRecorder/byte_recorder.py` & `DataRecorder-3.4.2/DataRecorder/byte_recorder.py`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.1/DataRecorder/db_recorder.py` & `DataRecorder-3.4.2/DataRecorder/db_recorder.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,41 +102,42 @@
                 d = data[0][0] if isinstance(data[0], (list, tuple)) else data[0]  # 获取第一个数据
                 name, cols = _create_table(self._cur, table, d)
                 tables[table] = cols
 
             now_data = (data,) if not isinstance(data[0], (list, tuple, dict)) else data
 
             for d in now_data:
-                long = len(d)
                 if isinstance(d, dict):
-                    question_masks = ','.join('?' * long)
                     d = data_to_list_or_dict(self, d)
+                    question_masks = ','.join('?' * len(d))
                     keys = d.keys()
 
                     for key in keys:  # 检查是否要新增列
                         if key not in tables[table]:
                             sql = f'ALTER TABLE {table} ADD COLUMN {key}'
                             self._cur.execute(sql)
                             tables[table].append(key)
 
                     keys_txt = ','.join(keys)
                     values = list(d.values())
                     sql = f'INSERT INTO {table} ({keys_txt}) values ({question_masks})'
 
                 else:
                     d = self._data_to_list(d)
+                    long = len(d)
                     cols_num = len(tables[table])
                     if long > cols_num:
                         raise RuntimeError('数据个数大于列数。')
                     d.extend([None] * (cols_num - long))
                     question_masks = ','.join('?' * cols_num)
 
                     values = d
                     sql = f'INSERT INTO {table} values ({question_masks})'
 
+                values = [str(i) if i is not None and not isinstance(i, (str, float, int, bool)) else i for i in values]
                 self._cur.execute(sql, values)
 
         self._conn.commit()
 
 
 def _create_table(cursor, table_name: str, data: dict) -> tuple:
     """创建表格
```

### Comparing `DataRecorder-3.4.1/DataRecorder/db_recorder.pyi` & `DataRecorder-3.4.2/DataRecorder/db_recorder.pyi`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.1/DataRecorder/filler.py` & `DataRecorder-3.4.2/DataRecorder/filler.py`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.1/DataRecorder/filler.pyi` & `DataRecorder-3.4.2/DataRecorder/filler.pyi`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.1/DataRecorder/recorder.py` & `DataRecorder-3.4.2/DataRecorder/recorder.py`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.1/DataRecorder/recorder.pyi` & `DataRecorder-3.4.2/DataRecorder/recorder.pyi`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.1/DataRecorder/setter.py` & `DataRecorder-3.4.2/DataRecorder/setter.py`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.1/DataRecorder/setter.pyI` & `DataRecorder-3.4.2/DataRecorder/setter.pyI`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.1/DataRecorder/style/cell_style.py` & `DataRecorder-3.4.2/DataRecorder/style/cell_style.py`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.1/DataRecorder/tools.py` & `DataRecorder-3.4.2/DataRecorder/tools.py`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.1/DataRecorder/tools.pyi` & `DataRecorder-3.4.2/DataRecorder/tools.pyi`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.1/DataRecorder.egg-info/PKG-INFO` & `DataRecorder-3.4.2/DataRecorder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataRecorder
-Version: 3.4.1
+Version: 3.4.2
 Summary: 用于记录数据的模块。
 Home-page: https://gitee.com/g1879/DataRecorder
 Author: g1879
 Author-email: g1879@qq.com
 License: MIT
 Keywords: DataRecorder
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `DataRecorder-3.4.1/DataRecorder.egg-info/SOURCES.txt` & `DataRecorder-3.4.2/DataRecorder.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
+DataRecorder/DataRecorder按照表头自动存对应列.py
 DataRecorder/__init__.py
 DataRecorder/base.py
 DataRecorder/base.pyi
 DataRecorder/byte_recorder.py
 DataRecorder/byte_recorder.pyi
 DataRecorder/db_recorder.py
 DataRecorder/db_recorder.pyi
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `DataRecorder-3.4.1/LICENSE` & `DataRecorder-3.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.1/PKG-INFO` & `DataRecorder-3.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataRecorder
-Version: 3.4.1
+Version: 3.4.2
 Summary: 用于记录数据的模块。
 Home-page: https://gitee.com/g1879/DataRecorder
 Author: g1879
 Author-email: g1879@qq.com
 License: MIT
 Keywords: DataRecorder
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `DataRecorder-3.4.1/README.md` & `DataRecorder-3.4.2/README.md`

 * *Files identical despite different names*

### Comparing `DataRecorder-3.4.1/setup.py` & `DataRecorder-3.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="DataRecorder",
-    version="3.4.1",
+    version="3.4.2",
     author="g1879",
     author_email="g1879@qq.com",
     description="用于记录数据的模块。",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     keywords="DataRecorder",
```

