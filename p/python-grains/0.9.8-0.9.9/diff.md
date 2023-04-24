# Comparing `tmp/python_grains-0.9.8.tar.gz` & `tmp/python_grains-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_grains-0.9.8.tar", last modified: Wed Mar 15 14:29:56 2023, max compression
+gzip compressed data, was "python_grains-0.9.9.tar", last modified: Wed Mar 15 14:50:51 2023, max compression
```

## Comparing `python_grains-0.9.8.tar` & `python_grains-0.9.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-03-15 14:29:56.245399 python_grains-0.9.8/
--rw-rw-rw-   0        0        0       80 2022-02-16 11:59:00.000000 python_grains-0.9.8/MANIFEST.in
--rw-rw-rw-   0        0        0      275 2023-03-15 14:29:56.245399 python_grains-0.9.8/PKG-INFO
--rw-rw-rw-   0        0        0       71 2022-02-15 10:07:24.000000 python_grains-0.9.8/README.md
--rw-rw-rw-   0        0        0     1083 2022-02-15 10:36:51.000000 python_grains-0.9.8/license.txt
-drwxrwxrwx   0        0        0        0 2023-03-15 14:29:56.212930 python_grains-0.9.8/python_grains/
--rw-rw-rw-   0        0        0       56 2022-08-12 13:06:28.000000 python_grains-0.9.8/python_grains/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-15 14:29:56.212930 python_grains-0.9.8/python_grains/aliassing/
--rw-rw-rw-   0        0        0       61 2022-08-12 13:06:28.000000 python_grains-0.9.8/python_grains/aliassing/__init__.py
--rw-rw-rw-   0        0        0     4837 2022-08-12 13:06:28.000000 python_grains-0.9.8/python_grains/aliassing/aliassing.py
-drwxrwxrwx   0        0        0        0 2023-03-15 14:29:56.227525 python_grains-0.9.8/python_grains/dynamic_settings/
--rw-rw-rw-   0        0        0       74 2022-08-12 13:06:28.000000 python_grains-0.9.8/python_grains/dynamic_settings/__init__.py
--rw-rw-rw-   0        0        0    19935 2022-11-11 12:47:15.000000 python_grains-0.9.8/python_grains/dynamic_settings/dynamic_settings.py
--rw-rw-rw-   0        0        0     2050 2022-08-12 13:06:28.000000 python_grains-0.9.8/python_grains/dynamic_settings/lua.py
-drwxrwxrwx   0        0        0        0 2023-03-15 14:29:56.227525 python_grains-0.9.8/python_grains/experiments/
--rw-rw-rw-   0        0        0       69 2022-08-12 13:06:28.000000 python_grains-0.9.8/python_grains/experiments/__init__.py
--rw-rw-rw-   0        0        0     5913 2022-08-12 13:06:28.000000 python_grains-0.9.8/python_grains/experiments/experiments.py
-drwxrwxrwx   0        0        0        0 2023-03-15 14:29:56.227525 python_grains-0.9.8/python_grains/locks/
--rw-rw-rw-   0        0        0       91 2022-08-12 13:06:28.000000 python_grains-0.9.8/python_grains/locks/__init__.py
--rw-rw-rw-   0        0        0     3842 2022-08-12 13:06:28.000000 python_grains-0.9.8/python_grains/locks/locks.py
-drwxrwxrwx   0        0        0        0 2023-03-15 14:29:56.245399 python_grains-0.9.8/python_grains/profiles/
--rw-rw-rw-   0        0        0      165 2023-02-22 09:23:08.000000 python_grains-0.9.8/python_grains/profiles/__init__.py
--rw-rw-rw-   0        0        0    12822 2023-03-15 14:29:32.000000 python_grains-0.9.8/python_grains/profiles/audiences.py
--rw-rw-rw-   0        0        0      137 2023-02-09 08:44:37.000000 python_grains-0.9.8/python_grains/profiles/exceptions.py
--rw-rw-rw-   0        0        0     9471 2023-03-08 12:13:58.000000 python_grains-0.9.8/python_grains/profiles/getter.py
--rw-rw-rw-   0        0        0    29615 2022-11-11 12:34:26.000000 python_grains-0.9.8/python_grains/profiles/lua.py
--rw-rw-rw-   0        0        0    14190 2022-09-14 17:45:44.000000 python_grains-0.9.8/python_grains/profiles/profile_properties.py
--rw-rw-rw-   0        0        0    33325 2022-11-30 07:18:26.000000 python_grains-0.9.8/python_grains/profiles/profiles.py
--rw-rw-rw-   0        0        0    18955 2023-01-17 14:37:39.000000 python_grains-0.9.8/python_grains/profiles/stitches.py
--rw-rw-rw-   0        0        0     1293 2022-09-08 08:01:31.000000 python_grains-0.9.8/python_grains/profiles/stitching.py
-drwxrwxrwx   0        0        0        0 2023-03-15 14:29:56.245399 python_grains-0.9.8/python_grains/queues/
--rw-rw-rw-   0        0        0       45 2022-08-12 13:06:28.000000 python_grains-0.9.8/python_grains/queues/__init__.py
--rw-rw-rw-   0        0        0     2828 2022-08-12 13:06:28.000000 python_grains-0.9.8/python_grains/queues/lua.py
--rw-rw-rw-   0        0        0    23567 2022-08-12 13:06:28.000000 python_grains-0.9.8/python_grains/queues/queues.py
-drwxrwxrwx   0        0        0        0 2023-03-15 14:29:56.245399 python_grains-0.9.8/python_grains/splunk/
--rw-rw-rw-   0        0        0       52 2022-08-12 13:06:28.000000 python_grains-0.9.8/python_grains/splunk/__init__.py
--rw-rw-rw-   0        0        0     4742 2022-08-12 13:06:28.000000 python_grains-0.9.8/python_grains/splunk/splunk.py
-drwxrwxrwx   0        0        0        0 2023-03-15 14:29:56.245399 python_grains-0.9.8/python_grains/utils/
--rw-rw-rw-   0        0        0      211 2022-08-12 13:06:28.000000 python_grains-0.9.8/python_grains/utils/__init__.py
--rw-rw-rw-   0        0        0     3389 2022-08-12 13:06:28.000000 python_grains-0.9.8/python_grains/utils/utils.py
--rw-rw-rw-   0        0        0       21 2023-03-15 14:29:41.000000 python_grains-0.9.8/python_grains/version.py
-drwxrwxrwx   0        0        0        0 2023-03-15 14:29:56.212930 python_grains-0.9.8/python_grains.egg-info/
--rw-rw-rw-   0        0        0      275 2023-03-15 14:29:56.000000 python_grains-0.9.8/python_grains.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1161 2023-03-15 14:29:56.000000 python_grains-0.9.8/python_grains.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-15 14:29:56.000000 python_grains-0.9.8/python_grains.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-03-15 14:29:56.000000 python_grains-0.9.8/python_grains.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-03-15 14:29:56.000000 python_grains-0.9.8/python_grains.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-15 14:29:56.245399 python_grains-0.9.8/setup.cfg
--rw-rw-rw-   0        0        0      979 2022-02-16 08:39:53.000000 python_grains-0.9.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-15 14:50:51.615199 python_grains-0.9.9/
+-rw-rw-rw-   0        0        0       80 2022-02-16 11:59:00.000000 python_grains-0.9.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      275 2023-03-15 14:50:51.615199 python_grains-0.9.9/PKG-INFO
+-rw-rw-rw-   0        0        0       71 2022-02-15 10:07:24.000000 python_grains-0.9.9/README.md
+-rw-rw-rw-   0        0        0     1083 2022-02-15 10:36:51.000000 python_grains-0.9.9/license.txt
+drwxrwxrwx   0        0        0        0 2023-03-15 14:50:51.574630 python_grains-0.9.9/python_grains/
+-rw-rw-rw-   0        0        0       56 2022-08-12 13:06:28.000000 python_grains-0.9.9/python_grains/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-15 14:50:51.584640 python_grains-0.9.9/python_grains/aliassing/
+-rw-rw-rw-   0        0        0       61 2022-08-12 13:06:28.000000 python_grains-0.9.9/python_grains/aliassing/__init__.py
+-rw-rw-rw-   0        0        0     4837 2022-08-12 13:06:28.000000 python_grains-0.9.9/python_grains/aliassing/aliassing.py
+drwxrwxrwx   0        0        0        0 2023-03-15 14:50:51.594638 python_grains-0.9.9/python_grains/dynamic_settings/
+-rw-rw-rw-   0        0        0       74 2022-08-12 13:06:28.000000 python_grains-0.9.9/python_grains/dynamic_settings/__init__.py
+-rw-rw-rw-   0        0        0    19935 2022-11-11 12:47:15.000000 python_grains-0.9.9/python_grains/dynamic_settings/dynamic_settings.py
+-rw-rw-rw-   0        0        0     2050 2022-08-12 13:06:28.000000 python_grains-0.9.9/python_grains/dynamic_settings/lua.py
+drwxrwxrwx   0        0        0        0 2023-03-15 14:50:51.595634 python_grains-0.9.9/python_grains/experiments/
+-rw-rw-rw-   0        0        0       69 2022-08-12 13:06:28.000000 python_grains-0.9.9/python_grains/experiments/__init__.py
+-rw-rw-rw-   0        0        0     5913 2022-08-12 13:06:28.000000 python_grains-0.9.9/python_grains/experiments/experiments.py
+drwxrwxrwx   0        0        0        0 2023-03-15 14:50:51.595634 python_grains-0.9.9/python_grains/locks/
+-rw-rw-rw-   0        0        0       91 2022-08-12 13:06:28.000000 python_grains-0.9.9/python_grains/locks/__init__.py
+-rw-rw-rw-   0        0        0     3842 2022-08-12 13:06:28.000000 python_grains-0.9.9/python_grains/locks/locks.py
+drwxrwxrwx   0        0        0        0 2023-03-15 14:50:51.608190 python_grains-0.9.9/python_grains/profiles/
+-rw-rw-rw-   0        0        0      165 2023-02-22 09:23:08.000000 python_grains-0.9.9/python_grains/profiles/__init__.py
+-rw-rw-rw-   0        0        0    12822 2023-03-15 14:50:33.000000 python_grains-0.9.9/python_grains/profiles/audiences.py
+-rw-rw-rw-   0        0        0      137 2023-02-09 08:44:37.000000 python_grains-0.9.9/python_grains/profiles/exceptions.py
+-rw-rw-rw-   0        0        0     9471 2023-03-08 12:13:58.000000 python_grains-0.9.9/python_grains/profiles/getter.py
+-rw-rw-rw-   0        0        0    29615 2022-11-11 12:34:26.000000 python_grains-0.9.9/python_grains/profiles/lua.py
+-rw-rw-rw-   0        0        0    14190 2022-09-14 17:45:44.000000 python_grains-0.9.9/python_grains/profiles/profile_properties.py
+-rw-rw-rw-   0        0        0    33325 2022-11-30 07:18:26.000000 python_grains-0.9.9/python_grains/profiles/profiles.py
+-rw-rw-rw-   0        0        0    18955 2023-01-17 14:37:39.000000 python_grains-0.9.9/python_grains/profiles/stitches.py
+-rw-rw-rw-   0        0        0     1293 2022-09-08 08:01:31.000000 python_grains-0.9.9/python_grains/profiles/stitching.py
+drwxrwxrwx   0        0        0        0 2023-03-15 14:50:51.615199 python_grains-0.9.9/python_grains/queues/
+-rw-rw-rw-   0        0        0       45 2022-08-12 13:06:28.000000 python_grains-0.9.9/python_grains/queues/__init__.py
+-rw-rw-rw-   0        0        0     2828 2022-08-12 13:06:28.000000 python_grains-0.9.9/python_grains/queues/lua.py
+-rw-rw-rw-   0        0        0    23567 2022-08-12 13:06:28.000000 python_grains-0.9.9/python_grains/queues/queues.py
+drwxrwxrwx   0        0        0        0 2023-03-15 14:50:51.615199 python_grains-0.9.9/python_grains/splunk/
+-rw-rw-rw-   0        0        0       52 2022-08-12 13:06:28.000000 python_grains-0.9.9/python_grains/splunk/__init__.py
+-rw-rw-rw-   0        0        0     4742 2022-08-12 13:06:28.000000 python_grains-0.9.9/python_grains/splunk/splunk.py
+drwxrwxrwx   0        0        0        0 2023-03-15 14:50:51.615199 python_grains-0.9.9/python_grains/utils/
+-rw-rw-rw-   0        0        0      211 2022-08-12 13:06:28.000000 python_grains-0.9.9/python_grains/utils/__init__.py
+-rw-rw-rw-   0        0        0     3389 2022-08-12 13:06:28.000000 python_grains-0.9.9/python_grains/utils/utils.py
+-rw-rw-rw-   0        0        0       21 2023-03-15 14:50:33.000000 python_grains-0.9.9/python_grains/version.py
+drwxrwxrwx   0        0        0        0 2023-03-15 14:50:51.584640 python_grains-0.9.9/python_grains.egg-info/
+-rw-rw-rw-   0        0        0      275 2023-03-15 14:50:51.000000 python_grains-0.9.9/python_grains.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1161 2023-03-15 14:50:51.000000 python_grains-0.9.9/python_grains.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-15 14:50:51.000000 python_grains-0.9.9/python_grains.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-03-15 14:50:51.000000 python_grains-0.9.9/python_grains.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-03-15 14:50:51.000000 python_grains-0.9.9/python_grains.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-03-15 14:50:51.615199 python_grains-0.9.9/setup.cfg
+-rw-rw-rw-   0        0        0      979 2022-02-16 08:39:53.000000 python_grains-0.9.9/setup.py
```

### Comparing `python_grains-0.9.8/license.txt` & `python_grains-0.9.9/license.txt`

 * *Files identical despite different names*

### Comparing `python_grains-0.9.8/python_grains/aliassing/aliassing.py` & `python_grains-0.9.9/python_grains/aliassing/aliassing.py`

 * *Files identical despite different names*

### Comparing `python_grains-0.9.8/python_grains/dynamic_settings/dynamic_settings.py` & `python_grains-0.9.9/python_grains/dynamic_settings/dynamic_settings.py`

 * *Files identical despite different names*

### Comparing `python_grains-0.9.8/python_grains/dynamic_settings/lua.py` & `python_grains-0.9.9/python_grains/dynamic_settings/lua.py`

 * *Files identical despite different names*

### Comparing `python_grains-0.9.8/python_grains/experiments/experiments.py` & `python_grains-0.9.9/python_grains/experiments/experiments.py`

 * *Files identical despite different names*

### Comparing `python_grains-0.9.8/python_grains/locks/locks.py` & `python_grains-0.9.9/python_grains/locks/locks.py`

 * *Files identical despite different names*

### Comparing `python_grains-0.9.8/python_grains/profiles/audiences.py` & `python_grains-0.9.9/python_grains/profiles/audiences.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
                 else:
 
                     parts.append(cls.parse_query_atom(field_name=kw, value=v, allowed_fields=allowed_fields))
 
         elif isinstance(raw_data, list):
 
             for el in raw_data:
-                parts.append(cls.parse(el, allowed_fields=allowed_fields))
+                parts.extend(cls.parse(el, allowed_fields=allowed_fields))
 
         else:
             raise InvalidQuery('Query needs to be a list or a dictionary.')
 
         return parts
 
     def run(self, data):
```

### Comparing `python_grains-0.9.8/python_grains/profiles/getter.py` & `python_grains-0.9.9/python_grains/profiles/getter.py`

 * *Files identical despite different names*

### Comparing `python_grains-0.9.8/python_grains/profiles/lua.py` & `python_grains-0.9.9/python_grains/profiles/lua.py`

 * *Files identical despite different names*

### Comparing `python_grains-0.9.8/python_grains/profiles/profile_properties.py` & `python_grains-0.9.9/python_grains/profiles/profile_properties.py`

 * *Files identical despite different names*

### Comparing `python_grains-0.9.8/python_grains/profiles/profiles.py` & `python_grains-0.9.9/python_grains/profiles/profiles.py`

 * *Files identical despite different names*

### Comparing `python_grains-0.9.8/python_grains/profiles/stitches.py` & `python_grains-0.9.9/python_grains/profiles/stitches.py`

 * *Files identical despite different names*

### Comparing `python_grains-0.9.8/python_grains/profiles/stitching.py` & `python_grains-0.9.9/python_grains/profiles/stitching.py`

 * *Files identical despite different names*

### Comparing `python_grains-0.9.8/python_grains/queues/lua.py` & `python_grains-0.9.9/python_grains/queues/lua.py`

 * *Files identical despite different names*

### Comparing `python_grains-0.9.8/python_grains/queues/queues.py` & `python_grains-0.9.9/python_grains/queues/queues.py`

 * *Files identical despite different names*

### Comparing `python_grains-0.9.8/python_grains/splunk/splunk.py` & `python_grains-0.9.9/python_grains/splunk/splunk.py`

 * *Files identical despite different names*

### Comparing `python_grains-0.9.8/python_grains/utils/utils.py` & `python_grains-0.9.9/python_grains/utils/utils.py`

 * *Files identical despite different names*

### Comparing `python_grains-0.9.8/python_grains.egg-info/SOURCES.txt` & `python_grains-0.9.9/python_grains.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python_grains-0.9.8/setup.py` & `python_grains-0.9.9/setup.py`

 * *Files identical despite different names*

