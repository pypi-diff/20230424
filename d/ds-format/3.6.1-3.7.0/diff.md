# Comparing `tmp/ds-format-3.6.1.tar.gz` & `tmp/ds-format-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ds-format-3.6.1.tar", last modified: Fri Apr 21 22:03:28 2023, max compression
+gzip compressed data, was "ds-format-3.7.0.tar", last modified: Mon Apr 24 17:28:36 2023, max compression
```

## Comparing `ds-format-3.6.1.tar` & `ds-format-3.7.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:03:28.054612 ds-format-3.6.1/
--rw-r--r--   0 peter     (1000) peter     (1000)      699 2023-04-21 22:03:28.054612 ds-format-3.6.1/PKG-INFO
--rw-r--r--   0 peter     (1000) peter     (1000)      563 2023-04-21 22:00:10.000000 ds-format-3.6.1/README.md
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:03:28.050612 ds-format-3.6.1/bin/
--rwxr-xr-x   0 peter     (1000) peter     (1000)      247 2023-04-21 22:00:10.000000 ds-format-3.6.1/bin/ds
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:03:28.050612 ds-format-3.6.1/ds_format/
--rw-r--r--   0 peter     (1000) peter     (1000)      623 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/__init__.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:03:28.050612 ds-format-3.6.1/ds_format/cmd/
--rw-r--r--   0 peter     (1000) peter     (1000)      578 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/cmd/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1645 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/cmd/attrs.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2487 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/cmd/cat.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1212 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/cmd/dims.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2565 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/cmd/ls.py
--rw-r--r--   0 peter     (1000) peter     (1000)     5039 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/cmd/main.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2965 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/cmd/merge.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1335 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/cmd/meta.py
--rw-r--r--   0 peter     (1000) peter     (1000)     3076 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/cmd/rename.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1231 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/cmd/rename_dim.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2244 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/cmd/rm.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2594 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/cmd/select.py
--rw-r--r--   0 peter     (1000) peter     (1000)     5279 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/cmd/set_.py
--rw-r--r--   0 peter     (1000) peter     (1000)      850 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/cmd/size.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1984 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/cmd/stats.py
--rw-r--r--   0 peter     (1000) peter     (1000)      859 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/cmd/type_.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:03:28.050612 ds-format-3.6.1/ds_format/drivers/
--rw-r--r--   0 peter     (1000) peter     (1000)      179 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/drivers/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1655 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/drivers/csv.py
--rw-r--r--   0 peter     (1000) peter     (1000)     5574 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/drivers/ds.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2768 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/drivers/hdf.py
--rw-r--r--   0 peter     (1000) peter     (1000)      602 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/drivers/json.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2361 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/drivers/netcdf.py
--rw-r--r--   0 peter     (1000) peter     (1000)     4874 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/help.py
--rw-r--r--   0 peter     (1000) peter     (1000)     8527 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/io.py
--rw-r--r--   0 peter     (1000) peter     (1000)     5067 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/misc.py
--rw-r--r--   0 peter     (1000) peter     (1000)    34168 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/op.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1122 2023-04-21 22:00:10.000000 ds-format-3.6.1/ds_format/validate.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:03:28.050612 ds-format-3.6.1/ds_format.egg-info/
--rw-r--r--   0 peter     (1000) peter     (1000)      699 2023-04-21 22:03:27.000000 ds-format-3.6.1/ds_format.egg-info/PKG-INFO
--rw-r--r--   0 peter     (1000) peter     (1000)     1139 2023-04-21 22:03:27.000000 ds-format-3.6.1/ds_format.egg-info/SOURCES.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        1 2023-04-21 22:03:27.000000 ds-format-3.6.1/ds_format.egg-info/dependency_links.txt
--rw-r--r--   0 peter     (1000) peter     (1000)      131 2023-04-21 22:03:27.000000 ds-format-3.6.1/ds_format.egg-info/requires.txt
--rw-r--r--   0 peter     (1000) peter     (1000)       10 2023-04-21 22:03:27.000000 ds-format-3.6.1/ds_format.egg-info/top_level.txt
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-21 22:03:28.054612 ds-format-3.6.1/man/
--rw-r--r--   0 peter     (1000) peter     (1000)     1186 2023-04-21 22:00:10.000000 ds-format-3.6.1/man/ds-attrs.1
--rw-r--r--   0 peter     (1000) peter     (1000)     1717 2023-04-21 22:00:10.000000 ds-format-3.6.1/man/ds-cat.1
--rw-r--r--   0 peter     (1000) peter     (1000)      809 2023-04-21 22:00:10.000000 ds-format-3.6.1/man/ds-dims.1
--rw-r--r--   0 peter     (1000) peter     (1000)      299 2023-04-21 22:00:10.000000 ds-format-3.6.1/man/ds-get.1
--rw-r--r--   0 peter     (1000) peter     (1000)     1599 2023-04-21 22:00:10.000000 ds-format-3.6.1/man/ds-ls.1
--rw-r--r--   0 peter     (1000) peter     (1000)     2713 2023-04-21 22:00:10.000000 ds-format-3.6.1/man/ds-merge.1
--rw-r--r--   0 peter     (1000) peter     (1000)      877 2023-04-21 22:00:10.000000 ds-format-3.6.1/man/ds-meta.1
--rw-r--r--   0 peter     (1000) peter     (1000)     1859 2023-04-21 22:00:10.000000 ds-format-3.6.1/man/ds-rename.1
--rw-r--r--   0 peter     (1000) peter     (1000)     1023 2023-04-21 22:00:10.000000 ds-format-3.6.1/man/ds-rename_attr.1
--rw-r--r--   0 peter     (1000) peter     (1000)      912 2023-04-21 22:00:10.000000 ds-format-3.6.1/man/ds-rename_dim.1
--rw-r--r--   0 peter     (1000) peter     (1000)     1388 2023-04-21 22:00:10.000000 ds-format-3.6.1/man/ds-rm.1
--rw-r--r--   0 peter     (1000) peter     (1000)      896 2023-04-21 22:00:10.000000 ds-format-3.6.1/man/ds-rm_attr.1
--rw-r--r--   0 peter     (1000) peter     (1000)     2143 2023-04-21 22:00:10.000000 ds-format-3.6.1/man/ds-select.1
--rw-r--r--   0 peter     (1000) peter     (1000)     3777 2023-04-21 22:00:10.000000 ds-format-3.6.1/man/ds-set.1
--rw-r--r--   0 peter     (1000) peter     (1000)      688 2023-04-21 22:00:10.000000 ds-format-3.6.1/man/ds-set_attrs.1
--rw-r--r--   0 peter     (1000) peter     (1000)      750 2023-04-21 22:00:10.000000 ds-format-3.6.1/man/ds-set_dims.1
--rw-r--r--   0 peter     (1000) peter     (1000)      542 2023-04-21 22:00:10.000000 ds-format-3.6.1/man/ds-size.1
--rw-r--r--   0 peter     (1000) peter     (1000)     1278 2023-04-21 22:00:10.000000 ds-format-3.6.1/man/ds-stats.1
--rw-r--r--   0 peter     (1000) peter     (1000)      548 2023-04-21 22:00:10.000000 ds-format-3.6.1/man/ds-type.1
--rw-r--r--   0 peter     (1000) peter     (1000)     1195 2023-04-21 22:00:10.000000 ds-format-3.6.1/man/ds-write.1
--rw-r--r--   0 peter     (1000) peter     (1000)     3353 2023-04-21 22:00:10.000000 ds-format-3.6.1/man/ds.1
--rw-r--r--   0 peter     (1000) peter     (1000)       38 2023-04-21 22:03:28.054612 ds-format-3.6.1/setup.cfg
--rwxr-xr-x   0 peter     (1000) peter     (1000)     1089 2023-04-21 22:00:10.000000 ds-format-3.6.1/setup.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-24 17:28:36.191125 ds-format-3.7.0/
+-rw-r--r--   0 peter     (1000) peter     (1000)      699 2023-04-24 17:28:36.191125 ds-format-3.7.0/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)      563 2023-04-24 17:23:36.000000 ds-format-3.7.0/README.md
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-24 17:28:36.187125 ds-format-3.7.0/bin/
+-rwxr-xr-x   0 peter     (1000) peter     (1000)      247 2023-04-24 17:23:36.000000 ds-format-3.7.0/bin/ds
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-24 17:28:36.187125 ds-format-3.7.0/ds_format/
+-rw-r--r--   0 peter     (1000) peter     (1000)      671 2023-04-24 17:23:36.000000 ds-format-3.7.0/ds_format/__init__.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-24 17:28:36.191125 ds-format-3.7.0/ds_format/cmd/
+-rw-r--r--   0 peter     (1000) peter     (1000)      578 2023-04-24 17:23:36.000000 ds-format-3.7.0/ds_format/cmd/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1645 2023-04-24 17:23:36.000000 ds-format-3.7.0/ds_format/cmd/attrs.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2487 2023-04-24 17:23:36.000000 ds-format-3.7.0/ds_format/cmd/cat.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1212 2023-04-24 17:23:36.000000 ds-format-3.7.0/ds_format/cmd/dims.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2565 2023-04-24 17:23:36.000000 ds-format-3.7.0/ds_format/cmd/ls.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     5039 2023-04-24 17:23:36.000000 ds-format-3.7.0/ds_format/cmd/main.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2965 2023-04-24 17:23:36.000000 ds-format-3.7.0/ds_format/cmd/merge.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1335 2023-04-24 17:23:36.000000 ds-format-3.7.0/ds_format/cmd/meta.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2971 2023-04-24 17:23:36.000000 ds-format-3.7.0/ds_format/cmd/rename.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1266 2023-04-24 17:23:36.000000 ds-format-3.7.0/ds_format/cmd/rename_dim.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2244 2023-04-24 17:23:36.000000 ds-format-3.7.0/ds_format/cmd/rm.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2594 2023-04-24 17:23:36.000000 ds-format-3.7.0/ds_format/cmd/select.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     5279 2023-04-24 17:23:36.000000 ds-format-3.7.0/ds_format/cmd/set_.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      850 2023-04-24 17:23:36.000000 ds-format-3.7.0/ds_format/cmd/size.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1984 2023-04-24 17:23:36.000000 ds-format-3.7.0/ds_format/cmd/stats.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      859 2023-04-24 17:23:36.000000 ds-format-3.7.0/ds_format/cmd/type_.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-24 17:28:36.191125 ds-format-3.7.0/ds_format/drivers/
+-rw-r--r--   0 peter     (1000) peter     (1000)      179 2023-04-24 17:23:36.000000 ds-format-3.7.0/ds_format/drivers/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1655 2023-04-24 17:23:36.000000 ds-format-3.7.0/ds_format/drivers/csv.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     5574 2023-04-24 17:23:36.000000 ds-format-3.7.0/ds_format/drivers/ds.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2768 2023-04-24 17:23:36.000000 ds-format-3.7.0/ds_format/drivers/hdf.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      602 2023-04-24 17:23:36.000000 ds-format-3.7.0/ds_format/drivers/json.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2361 2023-04-24 17:23:36.000000 ds-format-3.7.0/ds_format/drivers/netcdf.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     4874 2023-04-24 17:23:36.000000 ds-format-3.7.0/ds_format/help.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     8527 2023-04-24 17:23:36.000000 ds-format-3.7.0/ds_format/io.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     5067 2023-04-24 17:23:36.000000 ds-format-3.7.0/ds_format/misc.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    37498 2023-04-24 17:23:36.000000 ds-format-3.7.0/ds_format/op.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1122 2023-04-24 17:23:36.000000 ds-format-3.7.0/ds_format/validate.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-24 17:28:36.187125 ds-format-3.7.0/ds_format.egg-info/
+-rw-r--r--   0 peter     (1000) peter     (1000)      699 2023-04-24 17:28:35.000000 ds-format-3.7.0/ds_format.egg-info/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)     1139 2023-04-24 17:28:36.000000 ds-format-3.7.0/ds_format.egg-info/SOURCES.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        1 2023-04-24 17:28:35.000000 ds-format-3.7.0/ds_format.egg-info/dependency_links.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)      131 2023-04-24 17:28:35.000000 ds-format-3.7.0/ds_format.egg-info/requires.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)       10 2023-04-24 17:28:35.000000 ds-format-3.7.0/ds_format.egg-info/top_level.txt
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-04-24 17:28:36.191125 ds-format-3.7.0/man/
+-rw-r--r--   0 peter     (1000) peter     (1000)     1186 2023-04-24 17:23:36.000000 ds-format-3.7.0/man/ds-attrs.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     1717 2023-04-24 17:23:36.000000 ds-format-3.7.0/man/ds-cat.1
+-rw-r--r--   0 peter     (1000) peter     (1000)      809 2023-04-24 17:23:36.000000 ds-format-3.7.0/man/ds-dims.1
+-rw-r--r--   0 peter     (1000) peter     (1000)      299 2023-04-24 17:23:36.000000 ds-format-3.7.0/man/ds-get.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     1599 2023-04-24 17:23:36.000000 ds-format-3.7.0/man/ds-ls.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     2713 2023-04-24 17:23:36.000000 ds-format-3.7.0/man/ds-merge.1
+-rw-r--r--   0 peter     (1000) peter     (1000)      877 2023-04-24 17:23:36.000000 ds-format-3.7.0/man/ds-meta.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     1857 2023-04-24 17:23:36.000000 ds-format-3.7.0/man/ds-rename.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     1023 2023-04-24 17:23:36.000000 ds-format-3.7.0/man/ds-rename_attr.1
+-rw-r--r--   0 peter     (1000) peter     (1000)      912 2023-04-24 17:23:36.000000 ds-format-3.7.0/man/ds-rename_dim.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     1388 2023-04-24 17:23:36.000000 ds-format-3.7.0/man/ds-rm.1
+-rw-r--r--   0 peter     (1000) peter     (1000)      896 2023-04-24 17:23:36.000000 ds-format-3.7.0/man/ds-rm_attr.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     2143 2023-04-24 17:23:36.000000 ds-format-3.7.0/man/ds-select.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     3777 2023-04-24 17:23:36.000000 ds-format-3.7.0/man/ds-set.1
+-rw-r--r--   0 peter     (1000) peter     (1000)      688 2023-04-24 17:23:36.000000 ds-format-3.7.0/man/ds-set_attrs.1
+-rw-r--r--   0 peter     (1000) peter     (1000)      750 2023-04-24 17:23:36.000000 ds-format-3.7.0/man/ds-set_dims.1
+-rw-r--r--   0 peter     (1000) peter     (1000)      542 2023-04-24 17:23:36.000000 ds-format-3.7.0/man/ds-size.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     1278 2023-04-24 17:23:36.000000 ds-format-3.7.0/man/ds-stats.1
+-rw-r--r--   0 peter     (1000) peter     (1000)      548 2023-04-24 17:23:36.000000 ds-format-3.7.0/man/ds-type.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     1195 2023-04-24 17:23:36.000000 ds-format-3.7.0/man/ds-write.1
+-rw-r--r--   0 peter     (1000) peter     (1000)     3353 2023-04-24 17:23:36.000000 ds-format-3.7.0/man/ds.1
+-rw-r--r--   0 peter     (1000) peter     (1000)       38 2023-04-24 17:28:36.191125 ds-format-3.7.0/setup.cfg
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     1089 2023-04-24 17:23:36.000000 ds-format-3.7.0/setup.py
```

### Comparing `ds-format-3.6.1/PKG-INFO` & `ds-format-3.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ds-format
-Version: 3.6.1
+Version: 3.7.0
 Summary: ds-format is an open source program, a Python package and a storage format which provides an interface for reading and writing NetCDF files, as well as its own data file format.
 Home-page: https://ds-format.peterkuma.net
 Author: Peter Kuma
 Author-email: peter@peterkuma.net
 License: MIT
 Description: UNKNOWN
 Keywords: dataset,netcdf,hdf,json,numpy
```

### Comparing `ds-format-3.6.1/README.md` & `ds-format-3.7.0/README.md`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/ds_format/cmd/__init__.py` & `ds-format-3.7.0/ds_format/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/ds_format/cmd/attrs.py` & `ds-format-3.7.0/ds_format/cmd/attrs.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/ds_format/cmd/cat.py` & `ds-format-3.7.0/ds_format/cmd/cat.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/ds_format/cmd/dims.py` & `ds-format-3.7.0/ds_format/cmd/dims.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/ds_format/cmd/ls.py` & `ds-format-3.7.0/ds_format/cmd/ls.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/ds_format/cmd/main.py` & `ds-format-3.7.0/ds_format/cmd/main.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/ds_format/cmd/merge.py` & `ds-format-3.7.0/ds_format/cmd/merge.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/ds_format/cmd/meta.py` & `ds-format-3.7.0/ds_format/cmd/meta.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/ds_format/cmd/rename.py` & `ds-format-3.7.0/ds_format/cmd/rename.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 	usage: {
 		"`ds rename` *vars* *input* *output* [*options*]"
 		"`ds rename` *var* *attrs* *input* *output* [*options*]"
 		"`ds rename` `{` *var* *attrs* `}`... *input* *output* [*options*]"
 	}
 	arguments: {{
 		*var*: "Variable name, or an array of variable names whose attributes to rename, or `none` to rename dataset attributes."
-		*vars*: "Pairs of old and new variable names as *oldvar*`:` *newvar*. If *newattr* is `none`, remove the attribute."
+		*vars*: "Pairs of old and new variable names as *oldvar*`:` *newvar*. If *newvar* is `none`, remove the variable."
 		*attrs*: "Pairs of old and new attribute names as *oldattr*`:` *newattr*. If *newattr* is `none`, remove the attribute."
 		*input*: "Input file."
 		*output*: "Output file."
 		*options*: "See help for ds for global options. Note that with this command *options* can only be supplied before the command name or at the end of the command line."
 	}}
 	examples: {{
 		"Rename variables `time` to `newtime` and `temperature` to `newtemperature` in `dataset.nc` and save the output in `output.nc`.":
@@ -66,21 +66,19 @@
 		if not opts.get('F'):
 			vars_ = {ds.find(d, 'var', k): v for k, v in vars_.items()}
 			var = [x \
 				for var1 in var \
 				for x in (
 					ds.findall(d, 'var', var1) if var1 is not None else [None]
 				)]
-		for oldvar, newvar in vars_.items():
-			ds.rename(d, oldvar, newvar)
+		ds.rename_m(d, vars_)
 		for var1 in var:
 			if not opts.get('F'):
 				attrs1 = {
 					ds.find(d, 'attr', k, var1): v
 					for var1 in var
 					for k, v in attrs.items()
 				}
-			for oldattr, newattr in attrs1.items():
-				ds.rename_attr(d, oldattr, newattr, var=var1)
+			ds.rename_attr_m(d, attrs1, var1)
 	ds.write(output, d)
 
 rename.disable_cmd_opts = True
```

### Comparing `ds-format-3.6.1/ds_format/cmd/rename_dim.py` & `ds-format-3.7.0/ds_format/cmd/rename_dim.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 	output = args[2]
 
 	check(dims, 'dims', dict, str, str)
 	check(input_, 'input', str)
 	check(output, 'output', str)
 
 	d = ds.read(input_)
+	mapping = {}
 	for olddim, newdim in dims.items():
 		if not opts.get('F'):
 			olddim = ds.find(d, 'dim', olddim)
-		ds.rename_dim(d, olddim, newdim)
+		mapping[olddim] = newdim
+	ds.rename_dim_m(d, mapping)
 	ds.write(output, d)
 
 rename_dim.disable_cmd_opts = True
```

### Comparing `ds-format-3.6.1/ds_format/cmd/rm.py` & `ds-format-3.7.0/ds_format/cmd/rm.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/ds_format/cmd/select.py` & `ds-format-3.7.0/ds_format/cmd/select.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/ds_format/cmd/set_.py` & `ds-format-3.7.0/ds_format/cmd/set_.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/ds_format/cmd/size.py` & `ds-format-3.7.0/ds_format/cmd/size.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/ds_format/cmd/stats.py` & `ds-format-3.7.0/ds_format/cmd/stats.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/ds_format/cmd/type_.py` & `ds-format-3.7.0/ds_format/cmd/type_.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/ds_format/drivers/csv.py` & `ds-format-3.7.0/ds_format/drivers/csv.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/ds_format/drivers/ds.py` & `ds-format-3.7.0/ds_format/drivers/ds.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/ds_format/drivers/hdf.py` & `ds-format-3.7.0/ds_format/drivers/hdf.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/ds_format/drivers/json.py` & `ds-format-3.7.0/ds_format/drivers/json.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/ds_format/drivers/netcdf.py` & `ds-format-3.7.0/ds_format/drivers/netcdf.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/ds_format/help.py` & `ds-format-3.7.0/ds_format/help.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/ds_format/io.py` & `ds-format-3.7.0/ds_format/io.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -178,18 +178,18 @@
 			for filename in files
 		])
 	except Exception:
 		if ex is not None: ex.__exit__()
 		raise
 	dd = []
 	for d, w in res:
+		warnings += w
 		if d is None:
 			continue
 		dd += [d]
-		warnings += w
 	if merge is None:
 		return dd
 	else:
 		n = 0
 		for n, d in enumerate(dd):
 			m = ds.dims(d, size=True)[merge]
 			ds.var(d, 'n', np.full(m, n))
```

### Comparing `ds-format-3.6.1/ds_format/misc.py` & `ds-format-3.7.0/ds_format/misc.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/ds_format/op.py` & `ds-format-3.7.0/ds_format/op.py`

 * *Files 2% similar despite different names*

```diff
@@ -670,31 +670,21 @@
 $ ds.vars(d)
 ['new_temperature', 'time']"
 	}}
 	'''
 	check(d, 'd', dict)
 	check(old, 'old', str)
 	check(new, 'new', [str, None])
-	new_e = ds.escape(new)
-	old_e = ds.escape(old)
-	if require(d, 'var', old):
-		if old == new:
-			return
-		if new is not None:
-			d[new_e] = d[old_e]
-			d['.'][new_e] = d['.'][old_e]
-		del d[old_e]
-		del d['.'][old_e]
-		if new is not None:
-			rename_dim(d, old, new)
+	return rename_m(d, {old: new})
 
 def rename_attr(d, old, new, var=None):
 	'''
 	title: rename_attr
 	caption: "Rename a dataset or variable attribute."
+	usage: "`rename_attr`(*d*, *old*, *new*, *var*=`None`)"
 	arguments: {{
 		*d*: "Dataset (`dict`)."
 		*old*: "Old attribute name (`str`)."
 		*new*: "New attribute name (`str`)."
 	}}
 	options: {{
 		*var*: "Variable name (`str`) to rename a variable attribute or `None` to rename a dataset attribute."
@@ -714,23 +704,59 @@
 $ ds.rename_attr(d, 'title', 'new_title')
 $ ds.attrs(d)
 {'new_title': 'Temperature data'}"
 	}}
 	'''
 	check(d, 'd', dict)
 	check(old, 'old', str)
-	check(new, 'new', str)
+	check(new, 'new', [str, None])
 	check(var, 'var', [str, None])
-	old_e = ds.escape(old)
-	new_e = ds.escape(new)
-	if require(d, 'attr', old, var):
-		meta = ds.meta(d, '' if var is None else var)
-		if new is not None:
-			meta[new_e] = meta[old_e]
-		del meta[old_e]
+	return rename_attr_m(d, {old: new}, var)
+
+def rename_attr_m(d, mapping, var=None):
+	'''
+	title: rename_attr_m
+	caption: "Rename one or more dataset or variable attributes."
+	arguments: {{
+		*d*: "Dataset (`dict`)."
+		*mapping*: "A dictionary where the key is an old attribute name (`str`) and the value is a new attribute name (`str`) or `None` to remove the attribute. Swapping of atrributes is also supported."
+	}}
+	options: {{
+		*var*: "Variable name (`str`) to rename a variable attribute or `None` to rename a dataset attribute."
+	}}
+	returns: `None`
+	examples: {{
+		"Rename an attribute `long_name` to `new_long_name` and `units` to `new_units` of a variable `temperature` in a dataset read from `dataset.nc`.":
+"$ d = ds.read('dataset.nc')
+$ ds.attrs(d, 'temperature')
+{'long_name': 'temperature', 'units': 'celsius'}
+$ ds.rename_attr_m(d, {'long_name': 'new_long_name', 'units': 'new_units'}, var='temperature')
+$ ds.attrs(d, 'temperature')
+{'new_long_name': 'temperature', 'new_units': 'celsius'}"
+		"Rename a dataset attribute `title` to `new_title`.":
+"$ ds.attrs(d)
+{'title': 'Temperature data'}
+$ ds.rename_attr_m(d, {'title': 'new_title'})
+$ ds.attrs(d)
+{'new_title': 'Temperature data'}"
+	}}
+	'''
+	check(d, 'd', dict)
+	check(mapping, 'mapping', dict, str, [str, None])
+	tmp = {}
+	for old in mapping.keys():
+		if not require(d, 'attr', old, var):
+			continue
+		tmp[old] = ds.attr(d, old, var=var)
+		ds.rm_attr(d, old, var)
+	for old in tmp.keys():
+		new = mapping[old]
+		if new is None:
+			continue
+		ds.attr(d, new, tmp[old], var=var)
 
 def rename_dim(d, old, new):
 	'''
 	title: rename_dim
 	caption: "Rename a dimension."
 	usage: "`rename_dim`(*d*, *old*, *new*)"
 	arguments: {{
@@ -748,26 +774,95 @@
 $ ds.dims(d)
 ['new_time']"
 	}}
 	'''
 	check(d, 'd', dict)
 	check(old, 'old', str)
 	check(new, 'new', str)
-	if old == new:
-		return
-	for var in ds.vars(d, full=True):
-		dims = ds.dims(d, var)
-		dirty = False
-		for i, dim in enumerate(dims):
-			if dim == old:
-				dims[i] = new
-				dirty = True
-		if dirty:
+	return rename_dim_m(d, {old: new})
+
+def rename_dim_m(d, mapping):
+	'''
+	title: rename_dim_m
+	caption: "Rename one or more dimensions."
+	usage: "`rename_dim_m`(*d*, *mapping*)"
+	arguments: {{
+		*d*: "Dataset (`dict`)."
+		*mapping*: "A dictionary where the key is an old dimension name (`str`) and the value is a new dimension name (`str`). Swapping of dimensions is also supported."
+	}}
+	returns: `None`
+	examples: {{
+		"Rename a dimension `time` to `new_time` in a dataset read from `dataset.nc`.":
+"$ d = ds.read('dataset.nc')
+$ ds.dims(d)
+['time']
+$ ds.rename_dim_m(d, {'time': 'new_time'})
+$ ds.dims(d)
+['new_time']"
+	}}
+	'''
+	check(d, 'd', dict)
+	check(mapping, 'mapping', dict, str, str)
+	tmp = {}
+	for old in mapping.keys():
+		for var in ds.vars(d, full=True):
+			dims = ds.dims(d, var)
+			if old not in dims:
+				continue
+			tmp[var] = dims
+	for old, new in mapping.items():
+		for var in ds.vars(d, full=True):
+			if var not in tmp:
+				continue
+			dims = ds.dims(d, var)
+			for i, dim in enumerate(tmp[var]):
+				if dim == old:
+					dims[i] = new
 			ds.dims(d, var, dims)
 
+def rename_m(d, mapping):
+	'''
+	title: rename_m
+	caption: "Rename one or more variables."
+	usage: "`rename_m`(*d*, *mapping*)"
+	desc: "Any dimension with the same name is also renamed."
+	arguments: {{
+		*d*: "Dataset (`dict`)."
+		*mapping*: "A dictionary where the key is an old variable name (`str`) and the value is a new variable name (`str`) or `None` to remove the variable. Swapping of variables is also supported."
+	}}
+	returns: `None`
+	examples: {{
+		"Rename a variable `time` to `new_time` and `temperature` to `new_temperature` in a dataset read from `dataset.nc`.":
+"$ d = ds.read('dataset.nc')
+$ ds.vars(d)
+['temperature', 'time']
+$ ds.rename(d, {'time': 'new_time', 'temperature': 'new_temperature'})
+$ ds.vars(d)
+['new_temperature', 'new_time']"
+	}}
+	'''
+	check(d, 'd', dict)
+	check(mapping, 'mapping', dict, str, [str, None])
+	tmp = {}
+	for old in mapping.keys():
+		if not require(d, 'var', old):
+			continue
+		var = ds.var(d, old)
+		meta = ds.meta(d, old)
+		tmp[old] = [var, meta]
+		ds.rm(d, old)
+	for old in tmp.keys():
+		new = mapping[old]
+		if new is None:
+			continue
+		var, meta = tmp[old]
+		ds.var(d, new, var)
+		ds.meta(d, new, meta)
+	ds.rename_dim_m(d, {k: v for k, v in mapping.items() if v is not None})
+
 def require(d, what, name, var=None, full=False):
 	'''
 	title: require
 	caption: "Require that a variable, dimension or attribute is defined in a dataset."
 	usage: "`require`(*d*, *what*, *name*, *var*=`None`, *full*=`False`)"
 	desc: "If the item is not found and the mode is \\"soft\\", returns `False`. If the mode is \\"strict\\", raises `NameError`. If the mode is \\"moderate\\", produces a warning and returns `False`."
 	arguments: {{
@@ -834,16 +929,20 @@
 $ ds.rm(d, 'temperature')
 $ ds.vars(d)
 ['time']"
 	}}
 	'''
 	check(d, 'd', dict)
 	check(var, 'var', str)
-	if require(d, 'var', var):
-		del d[ds.escape(var)]
+	var_e = ds.escape(var)
+	meta = ds.meta(d)
+	if var_e in d:
+		del d[var_e]
+	if var_e in meta:
+		del meta[var_e]
 
 def rm_attr(d, attr, var=None):
 	'''
 	title: rm_attr
 	caption: "Remove a dataset or variable attribute."
 	usage: "`rm_attr`(*d*, *attr*, *var*)"
 	arguments: {{
```

### Comparing `ds-format-3.6.1/ds_format/validate.py` & `ds-format-3.7.0/ds_format/validate.py`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/ds_format.egg-info/PKG-INFO` & `ds-format-3.7.0/ds_format.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ds-format
-Version: 3.6.1
+Version: 3.7.0
 Summary: ds-format is an open source program, a Python package and a storage format which provides an interface for reading and writing NetCDF files, as well as its own data file format.
 Home-page: https://ds-format.peterkuma.net
 Author: Peter Kuma
 Author-email: peter@peterkuma.net
 License: MIT
 Description: UNKNOWN
 Keywords: dataset,netcdf,hdf,json,numpy
```

### Comparing `ds-format-3.6.1/ds_format.egg-info/SOURCES.txt` & `ds-format-3.7.0/ds_format.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/man/ds-attrs.1` & `ds-format-3.7.0/man/ds-attrs.1`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/man/ds-cat.1` & `ds-format-3.7.0/man/ds-cat.1`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/man/ds-dims.1` & `ds-format-3.7.0/man/ds-dims.1`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/man/ds-ls.1` & `ds-format-3.7.0/man/ds-ls.1`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/man/ds-merge.1` & `ds-format-3.7.0/man/ds-merge.1`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/man/ds-meta.1` & `ds-format-3.7.0/man/ds-meta.1`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/man/ds-rename.1` & `ds-format-3.7.0/man/ds-rename.1`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 .br
 .SH "ARGUMENTS"
 .TP
 \fIvar\fR
 Variable name, or an array of variable names whose attributes to rename, or \fBnone\fR to rename dataset attributes\.
 .TP
 \fIvars\fR
-Pairs of old and new variable names as \fIoldvar\fR\fB:\fR \fInewvar\fR\. If \fInewattr\fR is \fBnone\fR, remove the attribute\.
+Pairs of old and new variable names as \fIoldvar\fR\fB:\fR \fInewvar\fR\. If \fInewvar\fR is \fBnone\fR, remove the variable\.
 .TP
 \fIattrs\fR
 Pairs of old and new attribute names as \fIoldattr\fR\fB:\fR \fInewattr\fR\. If \fInewattr\fR is \fBnone\fR, remove the attribute\.
 .TP
 \fIinput\fR
 Input file\.
 .TP
```

### Comparing `ds-format-3.6.1/man/ds-rename_attr.1` & `ds-format-3.7.0/man/ds-rename_attr.1`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/man/ds-rename_dim.1` & `ds-format-3.7.0/man/ds-rename_dim.1`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/man/ds-rm.1` & `ds-format-3.7.0/man/ds-rm.1`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/man/ds-rm_attr.1` & `ds-format-3.7.0/man/ds-rm_attr.1`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/man/ds-select.1` & `ds-format-3.7.0/man/ds-select.1`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/man/ds-set.1` & `ds-format-3.7.0/man/ds-set.1`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/man/ds-set_attrs.1` & `ds-format-3.7.0/man/ds-set_attrs.1`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/man/ds-set_dims.1` & `ds-format-3.7.0/man/ds-set_dims.1`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/man/ds-size.1` & `ds-format-3.7.0/man/ds-size.1`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/man/ds-stats.1` & `ds-format-3.7.0/man/ds-stats.1`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/man/ds-type.1` & `ds-format-3.7.0/man/ds-type.1`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/man/ds-write.1` & `ds-format-3.7.0/man/ds-write.1`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/man/ds.1` & `ds-format-3.7.0/man/ds.1`

 * *Files identical despite different names*

### Comparing `ds-format-3.6.1/setup.py` & `ds-format-3.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 from glob import glob
 
 setup(
 	name='ds-format',
-	version='3.6.1',
+	version='3.7.0',
 	scripts=['bin/ds'],
 	packages=find_packages(),
 	description='ds-format is an open source program, a Python package and a storage format which provides an interface for reading and writing NetCDF files, as well as its own data file format.',
 	author='Peter Kuma',
 	author_email='peter@peterkuma.net',
 	keywords=['dataset', 'netcdf', 'hdf', 'json', 'numpy'],
 	url='https://ds-format.peterkuma.net',
```

