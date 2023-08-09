# Comparing `tmp/pyncm-1.6.9.1.tar.gz` & `tmp/pyncm-1.6.9.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyncm-1.6.9.1.tar", last modified: Wed Jun 28 10:49:41 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

