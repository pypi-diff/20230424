# Comparing `tmp/autoDownload-0.0.7.tar.gz` & `tmp/autoDownload-0.0.8.win-amd64.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoDownload-0.0.7.tar", last modified: Fri Mar 31 07:12:27 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

