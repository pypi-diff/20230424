# Comparing `tmp/tarina-0.3.1.tar.gz` & `tmp/tarina-0.3.2-cp38-cp38-win32.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarina-0.3.1.tar", last modified: Sun Apr 23 14:34:17 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

