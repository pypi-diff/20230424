# Comparing `tmp/yourtools-0.5.7.tar.gz` & `tmp/yourtools-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yourtools-0.5.7.tar", last modified: Tue Apr 18 06:11:04 2023, max compression
+gzip compressed data, was "dist/yourtools-0.5.8.tar", last modified: Mon Apr 24 02:37:11 2023, max compression
```

## Comparing `yourtools-0.5.7.tar` & `yourtools-0.5.8.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-18 06:11:04.000000 yourtools-0.5.7/
-drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-18 06:11:04.000000 yourtools-0.5.7/yourtools/
-drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-18 06:11:04.000000 yourtools-0.5.7/yourtools/db/
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      347 2023-04-07 10:28:09.000000 yourtools-0.5.7/yourtools/db/__init__.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      739 2023-04-07 10:28:09.000000 yourtools-0.5.7/yourtools/db/dbutils.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     2122 2023-04-07 10:28:09.000000 yourtools-0.5.7/yourtools/db/hive.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     2399 2023-04-13 10:15:47.000000 yourtools-0.5.7/yourtools/db/mysql.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     3842 2023-04-07 10:28:09.000000 yourtools-0.5.7/yourtools/Azkaban.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     1025 2023-04-18 01:51:31.000000 yourtools-0.5.7/yourtools/Time.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     6292 2023-04-14 11:05:56.000000 yourtools-0.5.7/yourtools/WeChat.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      474 2023-04-14 10:42:59.000000 yourtools-0.5.7/yourtools/__init__.py
-drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-18 06:11:04.000000 yourtools-0.5.7/yourtools.egg-info/
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     2658 2023-04-18 06:11:04.000000 yourtools-0.5.7/yourtools.egg-info/PKG-INFO
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      372 2023-04-18 06:11:04.000000 yourtools-0.5.7/yourtools.egg-info/SOURCES.txt
--rw-rw-r--   0 zfang     (3307) zfang     (3307)        1 2023-04-18 06:11:04.000000 yourtools-0.5.7/yourtools.egg-info/dependency_links.txt
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      190 2023-04-18 06:11:04.000000 yourtools-0.5.7/yourtools.egg-info/requires.txt
--rw-rw-r--   0 zfang     (3307) zfang     (3307)       10 2023-04-18 06:11:04.000000 yourtools-0.5.7/yourtools.egg-info/top_level.txt
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     2232 2023-04-07 10:28:09.000000 yourtools-0.5.7/README.md
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      189 2023-04-13 08:31:32.000000 yourtools-0.5.7/requirements.txt
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     2364 2023-04-18 06:07:38.000000 yourtools-0.5.7/setup.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     2658 2023-04-18 06:11:04.000000 yourtools-0.5.7/PKG-INFO
--rw-rw-r--   0 zfang     (3307) zfang     (3307)       38 2023-04-18 06:11:04.000000 yourtools-0.5.7/setup.cfg
+drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-24 02:37:11.000000 yourtools-0.5.8/
+drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-24 02:37:11.000000 yourtools-0.5.8/yourtools/
+drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-24 02:37:11.000000 yourtools-0.5.8/yourtools/db/
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      347 2023-04-07 10:28:09.000000 yourtools-0.5.8/yourtools/db/__init__.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      739 2023-04-07 10:28:09.000000 yourtools-0.5.8/yourtools/db/dbutils.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2122 2023-04-07 10:28:09.000000 yourtools-0.5.8/yourtools/db/hive.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2399 2023-04-13 10:15:47.000000 yourtools-0.5.8/yourtools/db/mysql.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     3842 2023-04-07 10:28:09.000000 yourtools-0.5.8/yourtools/Azkaban.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2469 2023-04-23 02:29:16.000000 yourtools-0.5.8/yourtools/COS.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     1025 2023-04-18 01:51:31.000000 yourtools-0.5.8/yourtools/Time.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     6292 2023-04-14 11:05:56.000000 yourtools-0.5.8/yourtools/WeChat.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      474 2023-04-14 10:42:59.000000 yourtools-0.5.8/yourtools/__init__.py
+drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-24 02:37:11.000000 yourtools-0.5.8/yourtools.egg-info/
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2658 2023-04-24 02:37:11.000000 yourtools-0.5.8/yourtools.egg-info/PKG-INFO
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      389 2023-04-24 02:37:11.000000 yourtools-0.5.8/yourtools.egg-info/SOURCES.txt
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)        1 2023-04-24 02:37:11.000000 yourtools-0.5.8/yourtools.egg-info/dependency_links.txt
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      190 2023-04-24 02:37:11.000000 yourtools-0.5.8/yourtools.egg-info/requires.txt
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)       10 2023-04-24 02:37:11.000000 yourtools-0.5.8/yourtools.egg-info/top_level.txt
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2232 2023-04-07 10:28:09.000000 yourtools-0.5.8/README.md
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      189 2023-04-13 08:31:32.000000 yourtools-0.5.8/requirements.txt
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2367 2023-04-18 06:12:45.000000 yourtools-0.5.8/setup.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2658 2023-04-24 02:37:11.000000 yourtools-0.5.8/PKG-INFO
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)       38 2023-04-24 02:37:11.000000 yourtools-0.5.8/setup.cfg
```

### Comparing `yourtools-0.5.7/yourtools/db/dbutils.py` & `yourtools-0.5.8/yourtools/db/dbutils.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.5.7/yourtools/db/hive.py` & `yourtools-0.5.8/yourtools/db/hive.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.5.7/yourtools/db/mysql.py` & `yourtools-0.5.8/yourtools/db/mysql.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.5.7/yourtools/Azkaban.py` & `yourtools-0.5.8/yourtools/Azkaban.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.5.7/yourtools/Time.py` & `yourtools-0.5.8/yourtools/Time.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.5.7/yourtools/WeChat.py` & `yourtools-0.5.8/yourtools/WeChat.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.5.7/yourtools.egg-info/PKG-INFO` & `yourtools-0.5.8/yourtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yourtools
-Version: 0.5.7
+Version: 0.5.8
 Summary: Python helper tools
 Home-page: https://pypi.org/project/yourtools/
 Author: zfang
 Author-email: founder517518@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yourtools-0.5.7/README.md` & `yourtools-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `yourtools-0.5.7/setup.py` & `yourtools-0.5.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,18 +70,17 @@
     with open("VERSION", "w") as version_f:
         version_f.write(get_version())
 
 
 def main():
     try:
         upload()
+        print("Upload success , Current VERSION:", curr_version())
     except Exception as e:
         raise Exception("Upload package error", e)
 
     # 将新的版本号字符串回写入文件中
     # write_now_version()
 
-    print("Upload success , Current VERSION:", curr_version())
-
 
 if __name__ == '__main__':
     main()
```

### Comparing `yourtools-0.5.7/PKG-INFO` & `yourtools-0.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yourtools
-Version: 0.5.7
+Version: 0.5.8
 Summary: Python helper tools
 Home-page: https://pypi.org/project/yourtools/
 Author: zfang
 Author-email: founder517518@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

