# Comparing `tmp/unravel-python-1.2.2.tar.gz` & `tmp/unravel-python-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unravel-python-1.2.2.tar", last modified: Mon Apr 24 11:41:24 2023, max compression
+gzip compressed data, was "unravel-python-1.2.3.tar", last modified: Mon Apr 24 14:12:09 2023, max compression
```

## Comparing `unravel-python-1.2.2.tar` & `unravel-python-1.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 11:41:24.120000 unravel-python-1.2.2/
--rw-rw-rw-   0        0        0    35823 2023-03-09 15:58:46.000000 unravel-python-1.2.2/LICENSE
--rw-rw-rw-   0        0        0     3897 2023-04-24 11:41:26.000000 unravel-python-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     3439 2023-04-05 09:30:36.000000 unravel-python-1.2.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-24 11:41:26.000000 unravel-python-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1057 2023-03-10 13:34:14.000000 unravel-python-1.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 11:41:24.140000 unravel-python-1.2.2/unravel/
--rw-rw-rw-   0        0        0      358 2023-04-24 11:41:10.000000 unravel-python-1.2.2/unravel/__init__.py
--rw-rw-rw-   0        0        0    48173 2023-04-05 16:32:30.000000 unravel-python-1.2.2/unravel/core.py
--rw-rw-rw-   0        0        0     4558 2023-04-05 16:37:44.000000 unravel-python-1.2.2/unravel/example.py
--rw-rw-rw-   0        0        0    14562 2023-04-24 11:36:50.000000 unravel-python-1.2.2/unravel/utils.py
--rw-rw-rw-   0        0        0     3746 2023-04-20 07:59:10.000000 unravel-python-1.2.2/unravel/viz.py
-drwxrwxrwx   0        0        0        0 2023-04-24 11:41:24.140000 unravel-python-1.2.2/unravel_python.egg-info/
--rw-rw-rw-   0        0        0     3897 2023-04-24 11:41:24.000000 unravel-python-1.2.2/unravel_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-04-24 11:41:26.000000 unravel-python-1.2.2/unravel_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 11:41:24.000000 unravel-python-1.2.2/unravel_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-04-24 11:41:24.000000 unravel-python-1.2.2/unravel_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-24 11:41:24.000000 unravel-python-1.2.2/unravel_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 14:12:09.550000 unravel-python-1.2.3/
+-rw-rw-rw-   0        0        0    35823 2023-03-09 15:58:46.000000 unravel-python-1.2.3/LICENSE
+-rw-rw-rw-   0        0        0     3897 2023-04-24 14:12:10.000000 unravel-python-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3439 2023-04-05 09:30:36.000000 unravel-python-1.2.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-24 14:12:10.000000 unravel-python-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1057 2023-03-10 13:34:14.000000 unravel-python-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:12:09.550000 unravel-python-1.2.3/unravel/
+-rw-rw-rw-   0        0        0      358 2023-04-24 14:11:56.000000 unravel-python-1.2.3/unravel/__init__.py
+-rw-rw-rw-   0        0        0    48173 2023-04-05 16:32:30.000000 unravel-python-1.2.3/unravel/core.py
+-rw-rw-rw-   0        0        0     4558 2023-04-05 16:37:44.000000 unravel-python-1.2.3/unravel/example.py
+-rw-rw-rw-   0        0        0    14624 2023-04-24 14:10:10.000000 unravel-python-1.2.3/unravel/utils.py
+-rw-rw-rw-   0        0        0     3746 2023-04-20 07:59:10.000000 unravel-python-1.2.3/unravel/viz.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:12:09.550000 unravel-python-1.2.3/unravel_python.egg-info/
+-rw-rw-rw-   0        0        0     3897 2023-04-24 14:12:10.000000 unravel-python-1.2.3/unravel_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-04-24 14:12:10.000000 unravel-python-1.2.3/unravel_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 14:12:10.000000 unravel-python-1.2.3/unravel_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-04-24 14:12:10.000000 unravel-python-1.2.3/unravel_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-24 14:12:10.000000 unravel-python-1.2.3/unravel_python.egg-info/top_level.txt
```

### Comparing `unravel-python-1.2.2/LICENSE` & `unravel-python-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `unravel-python-1.2.2/PKG-INFO` & `unravel-python-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unravel-python
-Version: 1.2.2
+Version: 1.2.3
 Summary: Implementation of UNRAVEL
 Home-page: https://github.com/DelinteNicolas/UNRAVEL
 Author: Nicolas Delinte
 Author-email: nicolas.delinte@uclouvain.be
 License: GNU General Public License v3.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
```

### Comparing `unravel-python-1.2.2/README.md` & `unravel-python-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `unravel-python-1.2.2/setup.py` & `unravel-python-1.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `unravel-python-1.2.2/unravel/core.py` & `unravel-python-1.2.3/unravel/core.py`

 * *Files identical despite different names*

### Comparing `unravel-python-1.2.2/unravel/example.py` & `unravel-python-1.2.3/unravel/example.py`

 * *Files identical despite different names*

### Comparing `unravel-python-1.2.2/unravel/utils.py` & `unravel-python-1.2.3/unravel/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,18 +102,19 @@
     rgb = np.zeros(peaksList[0].shape)
 
     for xyz in np.ndindex(peaksList[0].shape[:-1]):
         for k in range(K):
             rgb[xyz] += abs(peaksList[k][xyz])*fracList[k][xyz]*fvfList[k][xyz]
 
     # Normalize between [0,1] and by number of peaks per voxel
-    p = peak_count[(slice(None),) * dim + (np.newaxis,)]
-    warnings.filterwarnings("ignore")
-    rgb *= np.repeat(1+(K-p)/p, 3, axis=dim)
-    warnings.filterwarnings("default")
+    if fracList is None and fvfList is None:
+        p = peak_count[(slice(None),) * dim + (np.newaxis,)]
+        warnings.filterwarnings("ignore")
+        rgb *= np.repeat(1+(K-p)/p, 3, axis=dim)
+        warnings.filterwarnings("default")
     rgb[np.isnan(rgb)] = 0
     rgb /= np.max(rgb)
 
     # Color order
     if order == 'brg':
         rgb = rgb[(slice(None),) * 3 + ([2, 0, 1],)]
     elif order == 'gbr':
```

### Comparing `unravel-python-1.2.2/unravel/viz.py` & `unravel-python-1.2.3/unravel/viz.py`

 * *Files identical despite different names*

### Comparing `unravel-python-1.2.2/unravel_python.egg-info/PKG-INFO` & `unravel-python-1.2.3/unravel_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unravel-python
-Version: 1.2.2
+Version: 1.2.3
 Summary: Implementation of UNRAVEL
 Home-page: https://github.com/DelinteNicolas/UNRAVEL
 Author: Nicolas Delinte
 Author-email: nicolas.delinte@uclouvain.be
 License: GNU General Public License v3.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
```

