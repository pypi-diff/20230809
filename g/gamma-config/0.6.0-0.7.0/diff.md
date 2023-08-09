# Comparing `tmp/gamma-config-0.6.0.tar.gz` & `tmp/gamma_config-0.7.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamma-config-0.6.0.tar", last modified: Sat Feb 11 21:17:48 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

