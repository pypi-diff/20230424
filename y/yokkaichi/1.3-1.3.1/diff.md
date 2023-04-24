# Comparing `tmp/yokkaichi-1.3.tar.gz` & `tmp/yokkaichi-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yokkaichi-1.3.tar", last modified: Mon Apr 24 16:57:56 2023, max compression
+gzip compressed data, was "yokkaichi-1.3.1.tar", last modified: Mon Apr 24 19:14:03 2023, max compression
```

## Comparing `yokkaichi-1.3.tar` & `yokkaichi-1.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-04-24 16:57:56.282512 yokkaichi-1.3/
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1063 2023-04-09 23:36:24.000000 yokkaichi-1.3/LICENSE.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)     2710 2023-04-24 16:57:56.282512 yokkaichi-1.3/PKG-INFO
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1954 2023-03-10 22:19:25.000000 yokkaichi-1.3/README.md
--rw-r--r--   0 krystian  (1000) krystian  (1000)       38 2023-04-24 16:57:56.282512 yokkaichi-1.3/setup.cfg
--rw-r--r--   0 krystian  (1000) krystian  (1000)     1389 2023-04-09 23:36:24.000000 yokkaichi-1.3/setup.py
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-04-24 16:57:56.282512 yokkaichi-1.3/yokkaichi/
--rw-r--r--   0 krystian  (1000) krystian  (1000)     2967 2023-04-09 23:36:24.000000 yokkaichi-1.3/yokkaichi/MasscanScan.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)     6489 2023-04-09 23:36:24.000000 yokkaichi-1.3/yokkaichi/ServerScan.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)        0 2023-01-14 23:17:48.000000 yokkaichi-1.3/yokkaichi/__init__.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)     7971 2023-04-09 23:36:24.000000 yokkaichi-1.3/yokkaichi/__main__.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)       20 2023-04-24 16:56:31.000000 yokkaichi-1.3/yokkaichi/_version.py
--rw-r--r--   0 krystian  (1000) krystian  (1000)       54 2023-04-09 23:36:24.000000 yokkaichi-1.3/yokkaichi/rich_console.py
-drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-04-24 16:57:56.282512 yokkaichi-1.3/yokkaichi.egg-info/
--rw-r--r--   0 krystian  (1000) krystian  (1000)     2710 2023-04-24 16:57:56.000000 yokkaichi-1.3/yokkaichi.egg-info/PKG-INFO
--rw-r--r--   0 krystian  (1000) krystian  (1000)      335 2023-04-24 16:57:56.000000 yokkaichi-1.3/yokkaichi.egg-info/SOURCES.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)        1 2023-04-24 16:57:56.000000 yokkaichi-1.3/yokkaichi.egg-info/dependency_links.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)       50 2023-04-24 16:57:56.000000 yokkaichi-1.3/yokkaichi.egg-info/requires.txt
--rw-r--r--   0 krystian  (1000) krystian  (1000)       10 2023-04-24 16:57:56.000000 yokkaichi-1.3/yokkaichi.egg-info/top_level.txt
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-04-24 19:14:03.005697 yokkaichi-1.3.1/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1063 2023-04-09 23:36:24.000000 yokkaichi-1.3.1/LICENSE.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     2712 2023-04-24 19:14:03.005697 yokkaichi-1.3.1/PKG-INFO
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1954 2023-03-10 22:19:25.000000 yokkaichi-1.3.1/README.md
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       38 2023-04-24 19:14:03.005697 yokkaichi-1.3.1/setup.cfg
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     1389 2023-04-09 23:36:24.000000 yokkaichi-1.3.1/setup.py
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-04-24 19:14:03.005697 yokkaichi-1.3.1/yokkaichi/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     2967 2023-04-09 23:36:24.000000 yokkaichi-1.3.1/yokkaichi/MasscanScan.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     6520 2023-04-24 19:13:21.000000 yokkaichi-1.3.1/yokkaichi/ServerScan.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)        0 2023-01-14 23:17:48.000000 yokkaichi-1.3.1/yokkaichi/__init__.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     7971 2023-04-09 23:36:24.000000 yokkaichi-1.3.1/yokkaichi/__main__.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       22 2023-04-24 19:13:21.000000 yokkaichi-1.3.1/yokkaichi/_version.py
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       54 2023-04-09 23:36:24.000000 yokkaichi-1.3.1/yokkaichi/rich_console.py
+drwxr-xr-x   0 krystian  (1000) krystian  (1000)        0 2023-04-24 19:14:03.005697 yokkaichi-1.3.1/yokkaichi.egg-info/
+-rw-r--r--   0 krystian  (1000) krystian  (1000)     2712 2023-04-24 19:14:02.000000 yokkaichi-1.3.1/yokkaichi.egg-info/PKG-INFO
+-rw-r--r--   0 krystian  (1000) krystian  (1000)      335 2023-04-24 19:14:02.000000 yokkaichi-1.3.1/yokkaichi.egg-info/SOURCES.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)        1 2023-04-24 19:14:02.000000 yokkaichi-1.3.1/yokkaichi.egg-info/dependency_links.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       50 2023-04-24 19:14:02.000000 yokkaichi-1.3.1/yokkaichi.egg-info/requires.txt
+-rw-r--r--   0 krystian  (1000) krystian  (1000)       10 2023-04-24 19:14:02.000000 yokkaichi-1.3.1/yokkaichi.egg-info/top_level.txt
```

### Comparing `yokkaichi-1.3/LICENSE.txt` & `yokkaichi-1.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.3/PKG-INFO` & `yokkaichi-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yokkaichi
-Version: 1.3
+Version: 1.3.1
 Summary: Shodan-like server scanner for Minecraft (formely mcserverscanner)
 Home-page: https://github.com/Oreeeee/yokkaichi
 Author: Oreeeee
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `yokkaichi-1.3/README.md` & `yokkaichi-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.3/setup.py` & `yokkaichi-1.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.3/yokkaichi/MasscanScan.py` & `yokkaichi-1.3.1/yokkaichi/MasscanScan.py`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.3/yokkaichi/ServerScan.py` & `yokkaichi-1.3.1/yokkaichi/ServerScan.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,9 +177,9 @@
         # Convert the data to dict
         ip2location_data_dict = ast.literal_eval(ip2location_data_str)
 
         return ip2location_data_dict
 
     def add_to_file(self, server_info):
         self.results["server_list"].append(server_info)
-        with open(self.output_file, "w") as f:
-            f.write(json.dumps(self.results, indent=4))
+        with open(self.output_file, "w", encoding="utf-8") as f:
+            json.dump(self.results, f, indent=4, ensure_ascii=False)
```

### Comparing `yokkaichi-1.3/yokkaichi/__main__.py` & `yokkaichi-1.3.1/yokkaichi/__main__.py`

 * *Files identical despite different names*

### Comparing `yokkaichi-1.3/yokkaichi.egg-info/PKG-INFO` & `yokkaichi-1.3.1/yokkaichi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yokkaichi
-Version: 1.3
+Version: 1.3.1
 Summary: Shodan-like server scanner for Minecraft (formely mcserverscanner)
 Home-page: https://github.com/Oreeeee/yokkaichi
 Author: Oreeeee
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

