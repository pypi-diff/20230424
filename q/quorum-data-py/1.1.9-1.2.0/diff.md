# Comparing `tmp/quorum_data_py-1.1.9.tar.gz` & `tmp/quorum_data_py-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quorum_data_py-1.1.9.tar", last modified: Sat Apr 15 10:30:41 2023, max compression
+gzip compressed data, was "quorum_data_py-1.2.0.tar", last modified: Mon Apr 24 03:45:50 2023, max compression
```

## Comparing `quorum_data_py-1.1.9.tar` & `quorum_data_py-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 10:30:41.733122 quorum_data_py-1.1.9/
--rw-rw-rw-   0        0        0     1087 2023-04-03 04:08:10.000000 quorum_data_py-1.1.9/LICENSE
--rw-rw-rw-   0        0        0     2977 2023-04-15 10:30:41.702728 quorum_data_py-1.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     2018 2023-04-03 04:16:39.000000 quorum_data_py-1.1.9/README.md
--rw-rw-rw-   0        0        0      162 2023-02-24 07:11:51.000000 quorum_data_py-1.1.9/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-15 10:30:41.692767 quorum_data_py-1.1.9/quorum_data_py/
--rw-rw-rw-   0        0        0      349 2023-04-15 10:29:48.000000 quorum_data_py-1.1.9/quorum_data_py/__init__.py
--rw-rw-rw-   0        0        0     4161 2023-04-15 10:29:28.000000 quorum_data_py-1.1.9/quorum_data_py/_utils.py
--rw-rw-rw-   0        0        0     2980 2023-04-06 13:03:34.000000 quorum_data_py-1.1.9/quorum_data_py/converter.py
--rw-rw-rw-   0        0        0     5778 2023-04-06 12:27:52.000000 quorum_data_py-1.1.9/quorum_data_py/feed.py
--rw-rw-rw-   0        0        0     1357 2023-04-06 12:24:56.000000 quorum_data_py-1.1.9/quorum_data_py/trx_type.py
-drwxrwxrwx   0        0        0        0 2023-04-15 10:30:41.700734 quorum_data_py-1.1.9/quorum_data_py.egg-info/
--rw-rw-rw-   0        0        0     2977 2023-04-15 10:30:41.000000 quorum_data_py-1.1.9/quorum_data_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-04-15 10:30:41.000000 quorum_data_py-1.1.9/quorum_data_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 10:30:41.000000 quorum_data_py-1.1.9/quorum_data_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-15 10:30:41.000000 quorum_data_py-1.1.9/quorum_data_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-15 10:30:41.000000 quorum_data_py-1.1.9/quorum_data_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-15 10:30:41.733122 quorum_data_py-1.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1292 2023-04-15 10:29:48.000000 quorum_data_py-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 03:45:50.802922 quorum_data_py-1.2.0/
+-rw-rw-rw-   0        0        0     1087 2023-04-03 04:08:10.000000 quorum_data_py-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     2977 2023-04-24 03:45:50.781978 quorum_data_py-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2018 2023-04-03 04:16:39.000000 quorum_data_py-1.2.0/README.md
+-rw-rw-rw-   0        0        0      162 2023-02-24 07:11:51.000000 quorum_data_py-1.2.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-24 03:45:50.763028 quorum_data_py-1.2.0/quorum_data_py/
+-rw-rw-rw-   0        0        0      349 2023-04-24 03:44:48.000000 quorum_data_py-1.2.0/quorum_data_py/__init__.py
+-rw-rw-rw-   0        0        0     4161 2023-04-15 10:29:28.000000 quorum_data_py-1.2.0/quorum_data_py/_utils.py
+-rw-rw-rw-   0        0        0     2980 2023-04-06 13:03:34.000000 quorum_data_py-1.2.0/quorum_data_py/converter.py
+-rw-rw-rw-   0        0        0     5897 2023-04-24 03:44:25.000000 quorum_data_py-1.2.0/quorum_data_py/feed.py
+-rw-rw-rw-   0        0        0     1357 2023-04-06 12:24:56.000000 quorum_data_py-1.2.0/quorum_data_py/trx_type.py
+drwxrwxrwx   0        0        0        0 2023-04-24 03:45:50.778986 quorum_data_py-1.2.0/quorum_data_py.egg-info/
+-rw-rw-rw-   0        0        0     2977 2023-04-24 03:45:50.000000 quorum_data_py-1.2.0/quorum_data_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-04-24 03:45:50.000000 quorum_data_py-1.2.0/quorum_data_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 03:45:50.000000 quorum_data_py-1.2.0/quorum_data_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-24 03:45:50.000000 quorum_data_py-1.2.0/quorum_data_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-24 03:45:50.000000 quorum_data_py-1.2.0/quorum_data_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 03:45:50.803919 quorum_data_py-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1292 2023-04-24 03:44:48.000000 quorum_data_py-1.2.0/setup.py
```

### Comparing `quorum_data_py-1.1.9/LICENSE` & `quorum_data_py-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.1.9/PKG-INFO` & `quorum_data_py-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum_data_py
-Version: 1.1.9
+Version: 1.2.0
 Summary: Python Data for Apps of QuoRum
 Home-page: https://github.com/liujuanjuan1984/quorum_data_py
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_data_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_data_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_data_py-1.1.9/README.md` & `quorum_data_py-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.1.9/quorum_data_py/_utils.py` & `quorum_data_py-1.2.0/quorum_data_py/_utils.py`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.1.9/quorum_data_py/converter.py` & `quorum_data_py-1.2.0/quorum_data_py/converter.py`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.1.9/quorum_data_py/feed.py` & `quorum_data_py-1.2.0/quorum_data_py/feed.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 """Data structure recommendations in Quorum. For webapp Feed, Port and RumApp"""
 
 import datetime
 import logging
 
-from dateutil import parser
-
 from quorum_data_py._utils import pack_icon, pack_imgs, pack_obj
 
 logger = logging.getLogger(__name__)
 
 
-def add_published(data: dict, published):
-    """
-    published: timestamp int or ISO format string
-    e.g. 2020-01-01T00:00:00Z, 2023-04-04T10:31:45+08:00
-    """
+def check_publiched(published):
     if isinstance(published, (float, int)):
         published = int(str(published)[:10])
         dt = datetime.datetime.fromtimestamp(published, datetime.timezone.utc)
         published = dt.isoformat(timespec="seconds")
     else:
         try:
-            dt = parser.parse(published)
+            dt = datetime.datetime.fromisoformat(
+                published.replace("Z", "+00:00")
+            )
             published = dt.isoformat(timespec="seconds")
         except Exception as e:
             raise ValueError(f"published format error: {published}") from e
-    data["published"] = published
+    return published
+
+
+def add_published(data: dict, published):
+    """
+    published: timestamp int or ISO format string
+    e.g. 2020-01-01T00:00:00Z, 2023-04-04T10:31:45+08:00
+    """
+    data["published"] = check_publiched(published)
     return data
 
 
 def add_origin(data: dict, origin_name, origin_type=None):
     origin_type = origin_type or "Application"
     if origin_type not in ["Application", "Service"]:
         logger.warning("origin_type should be 'Application' or 'Service'")
```

### Comparing `quorum_data_py-1.1.9/quorum_data_py/trx_type.py` & `quorum_data_py-1.2.0/quorum_data_py/trx_type.py`

 * *Files identical despite different names*

### Comparing `quorum_data_py-1.1.9/quorum_data_py.egg-info/PKG-INFO` & `quorum_data_py-1.2.0/quorum_data_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum-data-py
-Version: 1.1.9
+Version: 1.2.0
 Summary: Python Data for Apps of QuoRum
 Home-page: https://github.com/liujuanjuan1984/quorum_data_py
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_data_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_data_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_data_py-1.1.9/setup.py` & `quorum_data_py-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="quorum_data_py",
-    version="1.1.9",
+    version="1.2.0",
     author="liujuanjuan1984",
     author_email="qiaoanlu@163.com",
     description="Python Data for Apps of QuoRum",
     keywords=["quorum_data_py", "rumsystem", "quorum"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/quorum_data_py",
```

