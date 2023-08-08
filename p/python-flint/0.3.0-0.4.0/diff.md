# Comparing `tmp/python-flint-0.3.0.tar.gz` & `tmp/python_flint-0.4.0-cp310-cp310-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-flint-0.3.0.tar", last modified: Fri Dec  7 17:18:28 2018, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

