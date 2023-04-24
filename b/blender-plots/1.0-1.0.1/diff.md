# Comparing `tmp/blender-plots-1.0.tar.gz` & `tmp/blender_plots-1.0.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blender-plots-1.0.tar", last modified: Sat Apr 22 09:29:49 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

