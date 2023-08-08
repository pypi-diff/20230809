# Comparing `tmp/m_json_db-0.1.0.tar.gz` & `tmp/m_json_db-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m_json_db-0.1.0.tar", max compression
+gzip compressed data, was "m_json_db-0.1.1.tar", max compression
```

## Comparing `m_json_db-0.1.0.tar` & `m_json_db-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      552 2023-08-08 22:53:21.174710 m_json_db-0.1.0/m_json_db/__init__.py
--rw-r--r--   0        0        0      286 2023-08-08 22:42:19.806205 m_json_db-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      499 2023-08-08 22:54:22.986494 m_json_db-0.1.0/setup.py
--rw-r--r--   0        0        0      346 2023-08-08 22:54:22.986718 m_json_db-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      559 2023-08-08 23:37:02.690105 m_json_db-0.1.1/m_json_db/__init__.py
+-rw-r--r--   0        0        0      286 2023-08-08 23:37:45.181906 m_json_db-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      499 2023-08-08 23:37:57.690242 m_json_db-0.1.1/setup.py
+-rw-r--r--   0        0        0      346 2023-08-08 23:37:57.690409 m_json_db-0.1.1/PKG-INFO
```

### Comparing `m_json_db-0.1.0/m_json_db/__init__.py` & `m_json_db-0.1.1/m_json_db/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
                 self.value = json.loads(f.read())
         except FileNotFoundError:
             self.value = default
 
     def __enter__(self):
         pass
 
-    def __exit__(self):
+    def __exit__(self, *args):
         with open(self.path, "w", encoding="utf-8") as f:
             f.write(json.dumps(self.value, ensure_ascii=False))
 
     def __getattr__(self, attrname):
         getattr(self.value, attrname)
 
 __all__ = ["Db"]
```

