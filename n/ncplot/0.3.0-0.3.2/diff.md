# Comparing `tmp/ncplot-0.3.0.tar.gz` & `tmp/ncplot-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncplot-0.3.0.tar", last modified: Wed Mar  1 14:09:01 2023, max compression
+gzip compressed data, was "ncplot-0.3.2.tar", last modified: Mon Apr 24 13:23:58 2023, max compression
```

## Comparing `ncplot-0.3.0.tar` & `ncplot-0.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:09:01.297282 ncplot-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-01 14:08:48.000000 ncplot-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-03-01 14:08:48.000000 ncplot-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-03-01 14:09:01.297282 ncplot-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-03-01 14:08:48.000000 ncplot-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:09:01.297282 ncplot-0.3.0/ncplot/
--rwxr-xr-x   0 runner    (1001) docker     (123)       29 2023-03-01 14:08:48.000000 ncplot-0.3.0/ncplot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-03-01 14:08:48.000000 ncplot-0.3.0/ncplot/command_line.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:08:48.000000 ncplot-0.3.0/ncplot/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)    34266 2023-03-01 14:08:48.000000 ncplot-0.3.0/ncplot/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-03-01 14:08:48.000000 ncplot-0.3.0/ncplot/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-03-01 14:08:48.000000 ncplot-0.3.0/ncplot/xarray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 14:09:01.297282 ncplot-0.3.0/ncplot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-03-01 14:09:01.000000 ncplot-0.3.0/ncplot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-01 14:08:48.000000 ncplot-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-01 14:09:01.297282 ncplot-0.3.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1840 2023-03-01 14:08:48.000000 ncplot-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:23:58.791739 ncplot-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-24 13:23:41.000000 ncplot-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-24 13:23:41.000000 ncplot-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-04-24 13:23:58.791739 ncplot-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-24 13:23:41.000000 ncplot-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:23:58.787739 ncplot-0.3.2/ncplot/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       29 2023-04-24 13:23:41.000000 ncplot-0.3.2/ncplot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-24 13:23:41.000000 ncplot-0.3.2/ncplot/command_line.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:23:41.000000 ncplot-0.3.2/ncplot/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34266 2023-04-24 13:23:41.000000 ncplot-0.3.2/ncplot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-04-24 13:23:41.000000 ncplot-0.3.2/ncplot/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-24 13:23:41.000000 ncplot-0.3.2/ncplot/xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:23:58.791739 ncplot-0.3.2/ncplot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-24 13:23:58.000000 ncplot-0.3.2/ncplot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-24 13:23:41.000000 ncplot-0.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 13:23:58.791739 ncplot-0.3.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1952 2023-04-24 13:23:41.000000 ncplot-0.3.2/setup.py
```

### Comparing `ncplot-0.3.0/LICENSE` & `ncplot-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ncplot-0.3.0/MANIFEST.in` & `ncplot-0.3.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `ncplot-0.3.0/PKG-INFO` & `ncplot-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncplot
-Version: 0.3.0
+Version: 0.3.2
 Summary: Interactive viewing of NetCDF data
 Home-page: https://github.com/pmlmodelling/ncplot
 Author: Robert Wilson
 Author-email: rwi@pml.ac.uk
 Maintainer: Robert Wilson
 Project-URL: Bug Tracker, https://github.com/pmlmodelling/ncplot/issues
 Project-URL: Documentation, https://ncplot.readthedocs.io/en/stable
```

### Comparing `ncplot-0.3.0/README.md` & `ncplot-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `ncplot-0.3.0/ncplot/command_line.py` & `ncplot-0.3.2/ncplot/command_line.py`

 * *Files identical despite different names*

### Comparing `ncplot-0.3.0/ncplot/plot.py` & `ncplot-0.3.2/ncplot/plot.py`

 * *Files identical despite different names*

### Comparing `ncplot-0.3.0/ncplot/utils.py` & `ncplot-0.3.2/ncplot/utils.py`

 * *Files identical despite different names*

### Comparing `ncplot-0.3.0/setup.py` & `ncplot-0.3.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,24 +17,31 @@
 # Use the README file as the description
 try:
     with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
         long_description = '\n' + f.read()
 except IOError:
     long_description = DESCRIPTION
 
-extras_require: dict[str, list[str]] = {
+#extras_require: dict[str, list[str]] = {
+#        ':python_version <= "3.10"': [
+#            'datashader',
+#        ],
+#}
+
+extras_require: dict() = {
         ':python_version <= "3.10"': [
             'datashader',
         ],
 }
 
+
 extras_require["complete"] = ["geoviews"]
 
 setup(name='ncplot',
-      version='0.3.0',
+      version='0.3.2',
       description=DESCRIPTION,
       long_description=long_description,
       long_description_content_type='text/markdown',
 
       python_requires='>=3.6.1',
 
       entry_points={
```

