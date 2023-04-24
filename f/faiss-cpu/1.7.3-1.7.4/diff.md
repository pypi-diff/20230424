# Comparing `tmp/faiss-cpu-1.7.3.tar.gz` & `tmp/faiss_cpu-1.7.4-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faiss-cpu-1.7.3.tar", last modified: Thu Nov 24 13:14:32 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

