# Comparing `tmp/shopcloud_eventbus-1.2.0.tar.gz` & `tmp/shopcloud_eventbus-1.3.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shopcloud_eventbus-1.2.0.tar", last modified: Wed Mar 22 06:11:31 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

