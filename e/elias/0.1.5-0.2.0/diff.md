# Comparing `tmp/elias-0.1.5.tar.gz` & `tmp/elias-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/d/Projects/elias/dist/.tmp-zx71rpyy/elias-0.1.5.tar", last modified: Sat Jan 14 17:01:42 2023, max compression
+gzip compressed data, was "/mnt/d/Projects/elias/dist/.tmp-46s1rhv8/elias-0.2.0.tar", last modified: Mon Apr 24 08:35:40 2023, max compression
```

## Comparing `elias-0.1.5.tar` & `elias-0.2.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-01-14 17:01:42.000000 elias-0.1.5/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2022-04-27 09:37:39.000000 elias-0.1.5/LICENSE
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2138 2023-01-14 17:01:42.000000 elias-0.1.5/PKG-INFO
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1736 2022-04-27 09:37:39.000000 elias-0.1.5/README.md
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      110 2022-04-27 09:37:39.000000 elias-0.1.5/pyproject.toml
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      707 2023-01-14 17:01:42.000000 elias-0.1.5/setup.cfg
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)       98 2022-04-27 09:37:39.000000 elias-0.1.5/setup.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-01-14 17:01:41.000000 elias-0.1.5/src/
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-01-14 17:01:41.000000 elias-0.1.5/src/elias/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2022-04-27 09:37:39.000000 elias-0.1.5/src/elias/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    21906 2023-01-13 14:05:47.000000 elias-0.1.5/src/elias/config.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-01-14 17:01:41.000000 elias-0.1.5/src/elias/data/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2022-04-27 09:37:39.000000 elias-0.1.5/src/elias/data/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     8439 2022-04-27 09:37:39.000000 elias-0.1.5/src/elias/data/combined.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4507 2022-04-27 09:37:39.000000 elias-0.1.5/src/elias/data/loader.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4987 2022-04-27 09:37:39.000000 elias-0.1.5/src/elias/data/sampling.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1047 2022-04-27 09:37:39.000000 elias-0.1.5/src/elias/data/stop_criterion.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-01-14 17:01:42.000000 elias-0.1.5/src/elias/folder/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      156 2022-04-27 09:37:39.000000 elias-0.1.5/src/elias/folder/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1355 2022-04-27 09:37:39.000000 elias-0.1.5/src/elias/folder/analysis.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     8126 2022-05-13 11:41:20.000000 elias-0.1.5/src/elias/folder/data.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13271 2022-12-23 10:38:59.000000 elias-0.1.5/src/elias/folder/folder.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1491 2022-12-23 10:15:28.000000 elias-0.1.5/src/elias/folder/model.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4564 2023-01-14 17:00:38.000000 elias-0.1.5/src/elias/folder/run.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-01-14 17:01:42.000000 elias-0.1.5/src/elias/manager/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      294 2022-04-27 09:37:39.000000 elias-0.1.5/src/elias/manager/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2705 2022-04-27 09:37:39.000000 elias-0.1.5/src/elias/manager/analysis.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1594 2022-04-27 09:37:39.000000 elias-0.1.5/src/elias/manager/artifact.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    12045 2022-04-27 09:37:39.000000 elias-0.1.5/src/elias/manager/buffered.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13104 2022-10-23 15:43:10.000000 elias-0.1.5/src/elias/manager/data.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    22291 2022-12-23 10:55:00.000000 elias-0.1.5/src/elias/manager/model.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2914 2022-05-10 13:31:36.000000 elias-0.1.5/src/elias/manager/run.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-01-14 17:01:42.000000 elias-0.1.5/src/elias/util/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      361 2022-06-24 14:37:22.000000 elias-0.1.5/src/elias/util/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1629 2022-10-23 15:45:04.000000 elias-0.1.5/src/elias/util/fs.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     7919 2022-06-24 13:43:08.000000 elias-0.1.5/src/elias/util/io.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3860 2022-12-26 22:15:43.000000 elias-0.1.5/src/elias/util/range.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1248 2022-10-24 10:11:39.000000 elias-0.1.5/src/elias/util/timing.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5512 2022-05-11 08:27:09.000000 elias-0.1.5/src/elias/util/version.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-01-14 17:01:41.000000 elias-0.1.5/src/elias.egg-info/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2138 2023-01-14 17:01:40.000000 elias-0.1.5/src/elias.egg-info/PKG-INFO
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      898 2023-01-14 17:01:41.000000 elias-0.1.5/src/elias.egg-info/SOURCES.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        1 2023-01-14 17:01:40.000000 elias-0.1.5/src/elias.egg-info/dependency_links.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      100 2023-01-14 17:01:40.000000 elias-0.1.5/src/elias.egg-info/requires.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        6 2023-01-14 17:01:40.000000 elias-0.1.5/src/elias.egg-info/top_level.txt
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-24 08:35:40.000000 elias-0.2.0/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2022-04-27 09:37:39.000000 elias-0.2.0/LICENSE
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2138 2023-04-24 08:35:40.000000 elias-0.2.0/PKG-INFO
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1736 2022-04-27 09:37:39.000000 elias-0.2.0/README.md
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      110 2022-04-27 09:37:39.000000 elias-0.2.0/pyproject.toml
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      707 2023-04-24 08:35:40.000000 elias-0.2.0/setup.cfg
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)       98 2022-04-27 09:37:39.000000 elias-0.2.0/setup.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-24 08:35:38.000000 elias-0.2.0/src/
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-24 08:35:38.000000 elias-0.2.0/src/elias/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2022-04-27 09:37:39.000000 elias-0.2.0/src/elias/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    22222 2023-04-24 08:29:27.000000 elias-0.2.0/src/elias/config.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-24 08:35:39.000000 elias-0.2.0/src/elias/data/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2022-04-27 09:37:39.000000 elias-0.2.0/src/elias/data/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     8439 2022-04-27 09:37:39.000000 elias-0.2.0/src/elias/data/combined.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4507 2022-04-27 09:37:39.000000 elias-0.2.0/src/elias/data/loader.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4987 2022-04-27 09:37:39.000000 elias-0.2.0/src/elias/data/sampling.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1047 2022-04-27 09:37:39.000000 elias-0.2.0/src/elias/data/stop_criterion.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-24 08:35:39.000000 elias-0.2.0/src/elias/folder/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      156 2022-04-27 09:37:39.000000 elias-0.2.0/src/elias/folder/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1355 2022-04-27 09:37:39.000000 elias-0.2.0/src/elias/folder/analysis.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     8126 2022-05-13 11:41:20.000000 elias-0.2.0/src/elias/folder/data.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13271 2022-12-23 10:38:59.000000 elias-0.2.0/src/elias/folder/folder.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1491 2022-12-23 10:15:28.000000 elias-0.2.0/src/elias/folder/model.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4564 2023-01-14 17:00:38.000000 elias-0.2.0/src/elias/folder/run.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-24 08:35:39.000000 elias-0.2.0/src/elias/manager/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      294 2022-04-27 09:37:39.000000 elias-0.2.0/src/elias/manager/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2705 2022-04-27 09:37:39.000000 elias-0.2.0/src/elias/manager/analysis.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1594 2022-04-27 09:37:39.000000 elias-0.2.0/src/elias/manager/artifact.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    12045 2022-04-27 09:37:39.000000 elias-0.2.0/src/elias/manager/buffered.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13104 2022-10-23 15:43:10.000000 elias-0.2.0/src/elias/manager/data.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    22291 2022-12-23 10:55:00.000000 elias-0.2.0/src/elias/manager/model.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2914 2022-05-10 13:31:36.000000 elias-0.2.0/src/elias/manager/run.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-24 08:35:40.000000 elias-0.2.0/src/elias/util/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      361 2022-06-24 14:37:22.000000 elias-0.2.0/src/elias/util/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     6824 2023-03-21 10:22:24.000000 elias-0.2.0/src/elias/util/fs.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     7919 2022-06-24 13:43:08.000000 elias-0.2.0/src/elias/util/io.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     4690 2023-03-21 10:20:42.000000 elias-0.2.0/src/elias/util/range.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1248 2022-10-24 10:11:39.000000 elias-0.2.0/src/elias/util/timing.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5512 2022-05-11 08:27:09.000000 elias-0.2.0/src/elias/util/version.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-24 08:35:39.000000 elias-0.2.0/src/elias.egg-info/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2138 2023-04-24 08:35:38.000000 elias-0.2.0/src/elias.egg-info/PKG-INFO
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      898 2023-04-24 08:35:38.000000 elias-0.2.0/src/elias.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        1 2023-04-24 08:35:38.000000 elias-0.2.0/src/elias.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      100 2023-04-24 08:35:38.000000 elias-0.2.0/src/elias.egg-info/requires.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        6 2023-04-24 08:35:38.000000 elias-0.2.0/src/elias.egg-info/top_level.txt
```

### Comparing `elias-0.1.5/PKG-INFO` & `elias-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elias
-Version: 0.1.5
+Version: 0.2.0
 Summary: ELIAS experiment library for facilitating machine learning projects
 Home-page: https://github.com/tobias-kirschstein/elias
 Author: Tobias Kirschstein
 Author-email: tobias.kirschstein@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `elias-0.1.5/README.md` & `elias-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `elias-0.1.5/setup.cfg` & `elias-0.2.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = elias
-version = 0.1.5
+version = 0.2.0
 author = Tobias Kirschstein
 author_email = tobias.kirschstein@gmail.com
 description = ELIAS experiment library for facilitating machine learning projects
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tobias-kirschstein/elias
 project_urls =
```

### Comparing `elias-0.1.5/src/elias/config.py` & `elias-0.2.0/src/elias/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,15 +211,21 @@
                 t = t if inspect.isclass(t) else type(t)
                 if issubclass(t, Config) and f.name in loaded_config:
                     # If a field is a Config Type, apply its backward compatibility method
                     # TODO: How do we want to handle cases like List[SomeConfig]?
                     #   Currently, the loaded_config[f.name] will be the list of items and the config class will
                     #   have to deal with unpacking itself.
                     #   This can be super complex like Tuple[SomeConfig, List[Union[SomeConfig2, SomeConfig3]]]...
-                    t._backward_compatibility(loaded_config[f.name])
+                    sub_dict = loaded_config[f.name]
+
+                    # Only traverse further if dictionary is not None.
+                    # After all, what should a dataclass do in its backward_compatibility() method if the passed dict
+                    # is None?
+                    if sub_dict is not None:
+                        t._backward_compatibility(sub_dict)
 
     @classmethod
     def _define_casts(cls) -> List[Type]:
         """
         Lists all the types of dataclass attributes that are enums and thus should be casted to their proper types
         if they not yet belong to it.
```

### Comparing `elias-0.1.5/src/elias/data/combined.py` & `elias-0.2.0/src/elias/data/combined.py`

 * *Files identical despite different names*

### Comparing `elias-0.1.5/src/elias/data/loader.py` & `elias-0.2.0/src/elias/data/loader.py`

 * *Files identical despite different names*

### Comparing `elias-0.1.5/src/elias/data/sampling.py` & `elias-0.2.0/src/elias/data/sampling.py`

 * *Files identical despite different names*

### Comparing `elias-0.1.5/src/elias/data/stop_criterion.py` & `elias-0.2.0/src/elias/data/stop_criterion.py`

 * *Files identical despite different names*

### Comparing `elias-0.1.5/src/elias/folder/analysis.py` & `elias-0.2.0/src/elias/folder/analysis.py`

 * *Files identical despite different names*

### Comparing `elias-0.1.5/src/elias/folder/data.py` & `elias-0.2.0/src/elias/folder/data.py`

 * *Files identical despite different names*

### Comparing `elias-0.1.5/src/elias/folder/folder.py` & `elias-0.2.0/src/elias/folder/folder.py`

 * *Files identical despite different names*

### Comparing `elias-0.1.5/src/elias/folder/model.py` & `elias-0.2.0/src/elias/folder/model.py`

 * *Files identical despite different names*

### Comparing `elias-0.1.5/src/elias/folder/run.py` & `elias-0.2.0/src/elias/folder/run.py`

 * *Files identical despite different names*

### Comparing `elias-0.1.5/src/elias/manager/analysis.py` & `elias-0.2.0/src/elias/manager/analysis.py`

 * *Files identical despite different names*

### Comparing `elias-0.1.5/src/elias/manager/artifact.py` & `elias-0.2.0/src/elias/manager/artifact.py`

 * *Files identical despite different names*

### Comparing `elias-0.1.5/src/elias/manager/buffered.py` & `elias-0.2.0/src/elias/manager/buffered.py`

 * *Files identical despite different names*

### Comparing `elias-0.1.5/src/elias/manager/data.py` & `elias-0.2.0/src/elias/manager/data.py`

 * *Files identical despite different names*

### Comparing `elias-0.1.5/src/elias/manager/model.py` & `elias-0.2.0/src/elias/manager/model.py`

 * *Files identical despite different names*

### Comparing `elias-0.1.5/src/elias/manager/run.py` & `elias-0.2.0/src/elias/manager/run.py`

 * *Files identical despite different names*

### Comparing `elias-0.1.5/src/elias/util/io.py` & `elias-0.2.0/src/elias/util/io.py`

 * *Files identical despite different names*

### Comparing `elias-0.1.5/src/elias/util/timing.py` & `elias-0.2.0/src/elias/util/timing.py`

 * *Files identical despite different names*

### Comparing `elias-0.1.5/src/elias/util/version.py` & `elias-0.2.0/src/elias/util/version.py`

 * *Files identical despite different names*

### Comparing `elias-0.1.5/src/elias.egg-info/PKG-INFO` & `elias-0.2.0/src/elias.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elias
-Version: 0.1.5
+Version: 0.2.0
 Summary: ELIAS experiment library for facilitating machine learning projects
 Home-page: https://github.com/tobias-kirschstein/elias
 Author: Tobias Kirschstein
 Author-email: tobias.kirschstein@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `elias-0.1.5/src/elias.egg-info/SOURCES.txt` & `elias-0.2.0/src/elias.egg-info/SOURCES.txt`

 * *Files identical despite different names*

