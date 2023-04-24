# Comparing `tmp/CodonU-0.0.1.tar.gz` & `tmp/CodonU-1.0.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CodonU-0.0.1.tar", last modified: Mon Feb 20 19:14:59 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

