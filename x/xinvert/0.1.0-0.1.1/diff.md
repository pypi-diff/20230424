# Comparing `tmp/xinvert-0.1.0.tar.gz` & `tmp/xinvert-0.1.1-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xinvert-0.1.0.tar", last modified: Mon Apr 24 09:12:50 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

