# Comparing `tmp/duckdb-0.7.2.dev2366.tar.gz` & `tmp/duckdb-0.7.2.dev2410-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/duckdb-0.7.2.dev2366.tar", last modified: Fri Apr 21 04:15:15 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

