# Comparing `tmp/adcpipeline-0.2.1.tar.gz` & `tmp/adcpipeline-0.2.1a0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\adcpipeline-0.2.1.tar", last modified: Mon Apr 24 11:34:19 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

