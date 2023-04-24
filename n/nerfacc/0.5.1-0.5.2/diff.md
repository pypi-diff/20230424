# Comparing `tmp/nerfacc-0.5.1.tar.gz` & `tmp/nerfacc-0.5.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/nerfacc/nerfacc/dist/.tmp-xeko1dq4/nerfacc-0.5.1.tar", last modified: Sun Apr  9 10:22:38 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

