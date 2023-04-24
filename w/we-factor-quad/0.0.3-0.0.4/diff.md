# Comparing `tmp/we_factor_quad-0.0.3.tar.gz` & `tmp/we_factor_quad-0.0.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "we_factor_quad-0.0.3.tar", last modified: Fri Apr  7 09:22:57 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

