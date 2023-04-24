# Comparing `tmp/gkligo-0.0.4.tar.gz` & `tmp/gkligo-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gkligo-0.0.4.tar", last modified: Mon Apr 24 13:32:09 2023, max compression
+gzip compressed data, was "gkligo-0.0.5.tar", last modified: Mon Apr 24 14:33:11 2023, max compression
```

## Comparing `gkligo-0.0.4.tar` & `gkligo-0.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-24 13:32:09.395295 gkligo-0.0.4/
--rwxr-xr-x   0 kws        (502) staff       (20)     1055 2020-06-10 15:35:24.000000 gkligo-0.0.4/LICENSE
--rw-r--r--   0 kws        (502) staff       (20)       74 2023-03-08 21:39:07.000000 gkligo-0.0.4/MANIFEST.in
--rw-r--r--   0 kws        (502) staff       (20)     1436 2023-04-24 13:32:09.394739 gkligo-0.0.4/PKG-INFO
--rw-r--r--   0 kws        (502) staff       (20)      980 2023-04-24 12:55:14.000000 gkligo-0.0.4/README.md
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-24 13:32:09.382921 gkligo-0.0.4/gkligo/
--rw-r--r--   0 kws        (502) staff       (20)       22 2023-03-08 21:32:16.000000 gkligo-0.0.4/gkligo/__init__.py
--rw-r--r--   0 kws        (502) staff       (20)       22 2023-04-24 13:28:47.000000 gkligo-0.0.4/gkligo/__version__.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-24 13:32:09.386959 gkligo-0.0.4/gkligo/scripts/
--rw-r--r--   0 kws        (502) staff       (20)       21 2023-03-08 21:34:47.000000 gkligo-0.0.4/gkligo/scripts/__init__.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-24 13:32:09.393466 gkligo-0.0.4/gkligo/scripts/python/
--rw-r--r--   0 kws        (502) staff       (20)       31 2023-03-08 21:35:35.000000 gkligo-0.0.4/gkligo/scripts/python/__init__.py
--rw-r--r--   0 kws        (502) staff       (20)       89 2023-04-20 16:53:23.000000 gkligo-0.0.4/gkligo/scripts/python/config_download_example.yaml
--rw-r--r--   0 kws        (502) staff       (20)      426 2023-04-24 12:50:06.000000 gkligo-0.0.4/gkligo/scripts/python/config_reports.yaml
--rw-r--r--   0 kws        (502) staff       (20)      520 2023-04-24 12:50:32.000000 gkligo-0.0.4/gkligo/scripts/python/config_reports_example.yaml
--rwxr-xr-x   0 kws        (502) staff       (20)     8993 2023-04-24 09:27:27.000000 gkligo-0.0.4/gkligo/scripts/python/downloadGWAlerts.py
--rwxr-xr-x   0 kws        (502) staff       (20)     4927 2023-04-24 13:29:46.000000 gkligo-0.0.4/gkligo/scripts/python/generateGWReports.py
--rwxr-xr-x   0 kws        (502) staff       (20)     2538 2023-04-20 14:57:17.000000 gkligo-0.0.4/gkligo/scripts/python/testDaemon.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-24 13:32:09.386349 gkligo-0.0.4/gkligo.egg-info/
--rw-r--r--   0 kws        (502) staff       (20)     1436 2023-04-24 13:32:09.000000 gkligo-0.0.4/gkligo.egg-info/PKG-INFO
--rw-r--r--   0 kws        (502) staff       (20)      586 2023-04-24 13:32:09.000000 gkligo-0.0.4/gkligo.egg-info/SOURCES.txt
--rw-r--r--   0 kws        (502) staff       (20)        1 2023-04-24 13:32:09.000000 gkligo-0.0.4/gkligo.egg-info/dependency_links.txt
--rw-r--r--   0 kws        (502) staff       (20)      146 2023-04-24 13:32:09.000000 gkligo-0.0.4/gkligo.egg-info/entry_points.txt
--rw-r--r--   0 kws        (502) staff       (20)       85 2023-04-24 13:32:09.000000 gkligo-0.0.4/gkligo.egg-info/requires.txt
--rw-r--r--   0 kws        (502) staff       (20)        7 2023-04-24 13:32:09.000000 gkligo-0.0.4/gkligo.egg-info/top_level.txt
--rw-r--r--   0 kws        (502) staff       (20)       38 2023-04-24 13:32:09.395529 gkligo-0.0.4/setup.cfg
--rwxr-xr-x   0 kws        (502) staff       (20)     1308 2023-04-24 13:23:15.000000 gkligo-0.0.4/setup.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-24 14:33:11.019288 gkligo-0.0.5/
+-rwxr-xr-x   0 kws        (502) staff       (20)     1055 2020-06-10 15:35:24.000000 gkligo-0.0.5/LICENSE
+-rw-r--r--   0 kws        (502) staff       (20)       74 2023-03-08 21:39:07.000000 gkligo-0.0.5/MANIFEST.in
+-rw-r--r--   0 kws        (502) staff       (20)     1436 2023-04-24 14:33:11.018361 gkligo-0.0.5/PKG-INFO
+-rw-r--r--   0 kws        (502) staff       (20)      980 2023-04-24 12:55:14.000000 gkligo-0.0.5/README.md
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-24 14:33:11.006914 gkligo-0.0.5/gkligo/
+-rw-r--r--   0 kws        (502) staff       (20)       22 2023-03-08 21:32:16.000000 gkligo-0.0.5/gkligo/__init__.py
+-rw-r--r--   0 kws        (502) staff       (20)       22 2023-04-24 14:31:10.000000 gkligo-0.0.5/gkligo/__version__.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-24 14:33:11.010168 gkligo-0.0.5/gkligo/scripts/
+-rw-r--r--   0 kws        (502) staff       (20)       21 2023-03-08 21:34:47.000000 gkligo-0.0.5/gkligo/scripts/__init__.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-24 14:33:11.017033 gkligo-0.0.5/gkligo/scripts/python/
+-rw-r--r--   0 kws        (502) staff       (20)       31 2023-03-08 21:35:35.000000 gkligo-0.0.5/gkligo/scripts/python/__init__.py
+-rw-r--r--   0 kws        (502) staff       (20)       89 2023-04-20 16:53:23.000000 gkligo-0.0.5/gkligo/scripts/python/config_download_example.yaml
+-rw-r--r--   0 kws        (502) staff       (20)      426 2023-04-24 12:50:06.000000 gkligo-0.0.5/gkligo/scripts/python/config_reports.yaml
+-rw-r--r--   0 kws        (502) staff       (20)      498 2023-04-24 13:37:26.000000 gkligo-0.0.5/gkligo/scripts/python/config_reports_example.yaml
+-rwxr-xr-x   0 kws        (502) staff       (20)     8993 2023-04-24 09:27:27.000000 gkligo-0.0.5/gkligo/scripts/python/downloadGWAlerts.py
+-rwxr-xr-x   0 kws        (502) staff       (20)     5522 2023-04-24 14:30:22.000000 gkligo-0.0.5/gkligo/scripts/python/generateGWReports.py
+-rwxr-xr-x   0 kws        (502) staff       (20)     2538 2023-04-20 14:57:17.000000 gkligo-0.0.5/gkligo/scripts/python/testDaemon.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-04-24 14:33:11.009573 gkligo-0.0.5/gkligo.egg-info/
+-rw-r--r--   0 kws        (502) staff       (20)     1436 2023-04-24 14:33:10.000000 gkligo-0.0.5/gkligo.egg-info/PKG-INFO
+-rw-r--r--   0 kws        (502) staff       (20)      586 2023-04-24 14:33:10.000000 gkligo-0.0.5/gkligo.egg-info/SOURCES.txt
+-rw-r--r--   0 kws        (502) staff       (20)        1 2023-04-24 14:33:10.000000 gkligo-0.0.5/gkligo.egg-info/dependency_links.txt
+-rw-r--r--   0 kws        (502) staff       (20)      146 2023-04-24 14:33:10.000000 gkligo-0.0.5/gkligo.egg-info/entry_points.txt
+-rw-r--r--   0 kws        (502) staff       (20)       85 2023-04-24 14:33:10.000000 gkligo-0.0.5/gkligo.egg-info/requires.txt
+-rw-r--r--   0 kws        (502) staff       (20)        7 2023-04-24 14:33:10.000000 gkligo-0.0.5/gkligo.egg-info/top_level.txt
+-rw-r--r--   0 kws        (502) staff       (20)       38 2023-04-24 14:33:11.019498 gkligo-0.0.5/setup.cfg
+-rwxr-xr-x   0 kws        (502) staff       (20)     1308 2023-04-24 13:23:15.000000 gkligo-0.0.5/setup.py
```

### Comparing `gkligo-0.0.4/LICENSE` & `gkligo-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gkligo-0.0.4/PKG-INFO` & `gkligo-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gkligo
-Version: 0.0.4
+Version: 0.0.5
 Summary: GW (LIGO) utilities
 Home-page: https://github.com/genghisken/gkligo
 Author: genghisken
 Author-email: ken.w.smith@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gkligo-0.0.4/README.md` & `gkligo-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `gkligo-0.0.4/gkligo/scripts/python/downloadGWAlerts.py` & `gkligo-0.0.5/gkligo/scripts/python/downloadGWAlerts.py`

 * *Files identical despite different names*

### Comparing `gkligo-0.0.4/gkligo/scripts/python/generateGWReports.py` & `gkligo-0.0.5/gkligo/scripts/python/generateGWReports.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 Usage:
   %s <configfile> <numberOfDays> [--outputlocation=<outputlocation>]
   %s (-h | --help)
   %s --version
 
 Options:
-  -h --help                         Show this screen.
-  --version                         Show version.
-  --outputlocaton=<outputlocaton>   Location to store the results [default: /tmp].
+  -h --help                           Show this screen.
+  --version                           Show version.
+  --outputlocation=<outputlocation>   Location to store the results [default: /tmp].
 
 E.g.:
   %s config.yaml 21
 """
 
 import sys
 __doc__ = __doc__ % (sys.argv[0], sys.argv[0], sys.argv[0], sys.argv[0])
@@ -119,41 +119,53 @@
     hostnamepso4 = config['databases']['pso4']['hostname']
 
     connatlas = dbConnect(hostnameatlas, usernameatlas, passwordatlas, databaseatlas)
     connps = dbConnect(hostnameps, usernameps, passwordps, databaseps)
     connpso4 = dbConnect(hostnamepso4, usernamepso4, passwordpso4, databasepso4)
 
     atlasExps = getATLASExposures(connatlas, options)
-    panstarrsExps = getPanSTARRSExposures(connps, options)
+    panstarrsExpsWS = getPanSTARRSExposures(connps, options, warpstack = 'W')
+    panstarrsExpsSS = getPanSTARRSExposures(connps, options, warpstack = 'S')
     pso4ExpsWS = getPanSTARRSExposures(connpso4, options, warpstack = 'W')
     pso4ExpsSS = getPanSTARRSExposures(connpso4, options, warpstack = 'S')
 
-    with open(options.outputlocation + '/atlasExps.csv', 'w') as f:
-        w = csv.DictWriter(f, atlasExps[0].keys(), delimiter = ',')
-        w.writeheader()
-        for row in atlasExps:
-            w.writerow(row)
-
-    with open(options.outputlocation + '/panstarrsExps.csv', 'w') as f:
-        w = csv.DictWriter(f, panstarrsExps[0].keys(), delimiter = ',')
-        w.writeheader()
-        for row in panstarrsExps:
-            w.writerow(row)
-
-    with open(options.outputlocation + '/pso4ExpsWS.csv', 'w') as f:
-        w = csv.DictWriter(f, pso4ExpsWS[0].keys(), delimiter = ',')
-        w.writeheader()
-        for row in pso4ExpsWS:
-            w.writerow(row)
-
-    with open(options.outputlocation + '/pso4ExpsSS.csv', 'w') as f:
-        w = csv.DictWriter(f, pso4ExpsSS[0].keys(), delimiter = ',')
-        w.writeheader()
-        for row in pso4ExpsSS:
-            w.writerow(row)
+    if len(atlasExps) > 0:
+        with open(options.outputlocation + '/atlasExps.csv', 'w') as f:
+            w = csv.DictWriter(f, atlasExps[0].keys(), delimiter = ',')
+            w.writeheader()
+            for row in atlasExps:
+                w.writerow(row)
+
+    if len(panstarrsExpsWS) > 0:
+        with open(options.outputlocation + '/panstarrsExpsWS.csv', 'w') as f:
+            w = csv.DictWriter(f, panstarrsExpsWS[0].keys(), delimiter = ',')
+            w.writeheader()
+            for row in panstarrsExpsWS:
+                w.writerow(row)
+
+    if len(panstarrsExpsSS) > 0:
+        with open(options.outputlocation + '/panstarrsExpsSS.csv', 'w') as f:
+            w = csv.DictWriter(f, panstarrsExpsSS[0].keys(), delimiter = ',')
+            w.writeheader()
+            for row in panstarrsExpsSS:
+                w.writerow(row)
+
+    if len(pso4ExpsWS) > 0:
+        with open(options.outputlocation + '/pso4ExpsWS.csv', 'w') as f:
+            w = csv.DictWriter(f, pso4ExpsWS[0].keys(), delimiter = ',')
+            w.writeheader()
+            for row in pso4ExpsWS:
+                w.writerow(row)
+
+    if len(pso4ExpsSS) > 0:
+        with open(options.outputlocation + '/pso4ExpsSS.csv', 'w') as f:
+            w = csv.DictWriter(f, pso4ExpsSS[0].keys(), delimiter = ',')
+            w.writeheader()
+            for row in pso4ExpsSS:
+                w.writerow(row)
 
     connatlas.close()
     connps.close()
     connpso4.close()
 
 
 if __name__ == '__main__':
```

### Comparing `gkligo-0.0.4/gkligo/scripts/python/testDaemon.py` & `gkligo-0.0.5/gkligo/scripts/python/testDaemon.py`

 * *Files identical despite different names*

### Comparing `gkligo-0.0.4/gkligo.egg-info/PKG-INFO` & `gkligo-0.0.5/gkligo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gkligo
-Version: 0.0.4
+Version: 0.0.5
 Summary: GW (LIGO) utilities
 Home-page: https://github.com/genghisken/gkligo
 Author: genghisken
 Author-email: ken.w.smith@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gkligo-0.0.4/gkligo.egg-info/SOURCES.txt` & `gkligo-0.0.5/gkligo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gkligo-0.0.4/setup.py` & `gkligo-0.0.5/setup.py`

 * *Files identical despite different names*

