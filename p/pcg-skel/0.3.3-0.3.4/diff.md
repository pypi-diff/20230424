# Comparing `tmp/pcg_skel-0.3.3.tar.gz` & `tmp/pcg_skel-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcg_skel-0.3.3.tar", last modified: Fri Apr 21 20:17:47 2023, max compression
+gzip compressed data, was "pcg_skel-0.3.4.tar", last modified: Mon Apr 24 20:05:00 2023, max compression
```

## Comparing `pcg_skel-0.3.3.tar` & `pcg_skel-0.3.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-04-21 20:17:47.782776 pcg_skel-0.3.3/
--rw-r--r--   0 caseysm    (501) staff       (20)     1842 2022-11-15 01:01:33.000000 pcg_skel-0.3.3/LICENSE.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       24 2022-11-15 01:01:33.000000 pcg_skel-0.3.3/MANIFEST.in
--rw-r--r--   0 caseysm    (501) staff       (20)    10165 2023-04-21 20:17:47.782168 pcg_skel-0.3.3/PKG-INFO
--rw-r--r--   0 caseysm    (501) staff       (20)     9871 2023-03-08 00:43:18.000000 pcg_skel-0.3.3/README.md
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-04-21 20:17:47.781076 pcg_skel-0.3.3/pcg_skel/
--rw-r--r--   0 caseysm    (501) staff       (20)      117 2023-04-21 20:17:35.000000 pcg_skel-0.3.3/pcg_skel/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)     1926 2022-11-15 01:01:33.000000 pcg_skel-0.3.3/pcg_skel/chunk_cache.py
--rw-r--r--   0 caseysm    (501) staff       (20)    15449 2023-03-07 01:08:41.000000 pcg_skel-0.3.3/pcg_skel/chunk_tools.py
--rw-r--r--   0 caseysm    (501) staff       (20)    11760 2023-04-21 18:23:20.000000 pcg_skel-0.3.3/pcg_skel/features.py
--rw-r--r--   0 caseysm    (501) staff       (20)    25012 2023-03-07 01:08:41.000000 pcg_skel-0.3.3/pcg_skel/nocache.py
--rw-r--r--   0 caseysm    (501) staff       (20)     6211 2023-04-21 18:54:26.000000 pcg_skel-0.3.3/pcg_skel/pcg_anno.py
--rw-r--r--   0 caseysm    (501) staff       (20)    36782 2023-04-21 20:14:20.000000 pcg_skel-0.3.3/pcg_skel/pcg_skel.py
--rw-r--r--   0 caseysm    (501) staff       (20)     3216 2022-11-15 01:01:33.000000 pcg_skel-0.3.3/pcg_skel/skel_utils.py
--rw-r--r--   0 caseysm    (501) staff       (20)     2866 2023-03-07 01:08:41.000000 pcg_skel-0.3.3/pcg_skel/utils.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-04-21 20:17:47.781924 pcg_skel-0.3.3/pcg_skel.egg-info/
--rw-r--r--   0 caseysm    (501) staff       (20)    10165 2023-04-21 20:17:47.000000 pcg_skel-0.3.3/pcg_skel.egg-info/PKG-INFO
--rw-r--r--   0 caseysm    (501) staff       (20)      411 2023-04-21 20:17:47.000000 pcg_skel-0.3.3/pcg_skel.egg-info/SOURCES.txt
--rw-r--r--   0 caseysm    (501) staff       (20)        1 2023-04-21 20:17:47.000000 pcg_skel-0.3.3/pcg_skel.egg-info/dependency_links.txt
--rw-r--r--   0 caseysm    (501) staff       (20)      112 2023-04-21 20:17:47.000000 pcg_skel-0.3.3/pcg_skel.egg-info/requires.txt
--rw-r--r--   0 caseysm    (501) staff       (20)        9 2023-04-21 20:17:47.000000 pcg_skel-0.3.3/pcg_skel.egg-info/top_level.txt
--rw-r--r--   0 caseysm    (501) staff       (20)      112 2022-11-15 01:01:33.000000 pcg_skel-0.3.3/requirements.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       38 2023-04-21 20:17:47.782872 pcg_skel-0.3.3/setup.cfg
--rw-r--r--   0 caseysm    (501) staff       (20)     1467 2022-11-15 01:01:33.000000 pcg_skel-0.3.3/setup.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-04-24 20:05:00.391821 pcg_skel-0.3.4/
+-rw-r--r--   0 caseysm    (501) staff       (20)     1842 2022-11-15 01:01:33.000000 pcg_skel-0.3.4/LICENSE.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       24 2022-11-15 01:01:33.000000 pcg_skel-0.3.4/MANIFEST.in
+-rw-r--r--   0 caseysm    (501) staff       (20)    10165 2023-04-24 20:05:00.391572 pcg_skel-0.3.4/PKG-INFO
+-rw-r--r--   0 caseysm    (501) staff       (20)     9871 2023-03-08 00:43:18.000000 pcg_skel-0.3.4/README.md
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-04-24 20:05:00.390197 pcg_skel-0.3.4/pcg_skel/
+-rw-r--r--   0 caseysm    (501) staff       (20)      117 2023-04-24 20:04:52.000000 pcg_skel-0.3.4/pcg_skel/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     1926 2022-11-15 01:01:33.000000 pcg_skel-0.3.4/pcg_skel/chunk_cache.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    15449 2023-03-07 01:08:41.000000 pcg_skel-0.3.4/pcg_skel/chunk_tools.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    11760 2023-04-21 18:23:20.000000 pcg_skel-0.3.4/pcg_skel/features.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    25012 2023-03-07 01:08:41.000000 pcg_skel-0.3.4/pcg_skel/nocache.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     6228 2023-04-24 19:45:23.000000 pcg_skel-0.3.4/pcg_skel/pcg_anno.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    36782 2023-04-21 20:14:20.000000 pcg_skel-0.3.4/pcg_skel/pcg_skel.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     3216 2022-11-15 01:01:33.000000 pcg_skel-0.3.4/pcg_skel/skel_utils.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     2866 2023-03-07 01:08:41.000000 pcg_skel-0.3.4/pcg_skel/utils.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-04-24 20:05:00.391240 pcg_skel-0.3.4/pcg_skel.egg-info/
+-rw-r--r--   0 caseysm    (501) staff       (20)    10165 2023-04-24 20:05:00.000000 pcg_skel-0.3.4/pcg_skel.egg-info/PKG-INFO
+-rw-r--r--   0 caseysm    (501) staff       (20)      411 2023-04-24 20:05:00.000000 pcg_skel-0.3.4/pcg_skel.egg-info/SOURCES.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)        1 2023-04-24 20:05:00.000000 pcg_skel-0.3.4/pcg_skel.egg-info/dependency_links.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)      112 2023-04-24 20:05:00.000000 pcg_skel-0.3.4/pcg_skel.egg-info/requires.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)        9 2023-04-24 20:05:00.000000 pcg_skel-0.3.4/pcg_skel.egg-info/top_level.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)      112 2022-11-15 01:01:33.000000 pcg_skel-0.3.4/requirements.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       38 2023-04-24 20:05:00.391884 pcg_skel-0.3.4/setup.cfg
+-rw-r--r--   0 caseysm    (501) staff       (20)     1467 2022-11-15 01:01:33.000000 pcg_skel-0.3.4/setup.py
```

### Comparing `pcg_skel-0.3.3/LICENSE.txt` & `pcg_skel-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pcg_skel-0.3.3/PKG-INFO` & `pcg_skel-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcg_skel
-Version: 0.3.3
+Version: 0.3.4
 Summary: Skeletonization using the pychunkedgraph
 Home-page: https://github.com/AllenInstitute/pcg_skel
 Author: Casey Schneider-mizell
 Author-email: caseys@alleninstitute.org
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `pcg_skel-0.3.3/README.md` & `pcg_skel-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `pcg_skel-0.3.3/pcg_skel/chunk_cache.py` & `pcg_skel-0.3.4/pcg_skel/chunk_cache.py`

 * *Files identical despite different names*

### Comparing `pcg_skel-0.3.3/pcg_skel/chunk_tools.py` & `pcg_skel-0.3.4/pcg_skel/chunk_tools.py`

 * *Files identical despite different names*

### Comparing `pcg_skel-0.3.3/pcg_skel/features.py` & `pcg_skel-0.3.4/pcg_skel/features.py`

 * *Files identical despite different names*

### Comparing `pcg_skel-0.3.3/pcg_skel/nocache.py` & `pcg_skel-0.3.4/pcg_skel/nocache.py`

 * *Files identical despite different names*

### Comparing `pcg_skel-0.3.3/pcg_skel/pcg_anno.py` & `pcg_skel-0.3.4/pcg_skel/pcg_anno.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,15 +147,15 @@
     else:
         syn_df = client.materialize.query_table(
             synapse_table,
             filter_equal_dict={f"{side}_pt_root_id": root_id},
             metadata=metadata,
         )
     if remove_crud:
-        syn_df.drop(columns=['created', 'superceded_id', 'valid'], inplace=True)
+        syn_df.drop(columns=['created', 'superceded_id', 'valid'], inplace=True, errors='ignore')
 
     if remove_self:
         syn_df = syn_df.query("pre_pt_root_id != post_pt_root_id").reset_index(
             drop=True
         )
     syn_df = annotation_to_level2_id(
         syn_df,
```

### Comparing `pcg_skel-0.3.3/pcg_skel/pcg_skel.py` & `pcg_skel-0.3.4/pcg_skel/pcg_skel.py`

 * *Files identical despite different names*

### Comparing `pcg_skel-0.3.3/pcg_skel/skel_utils.py` & `pcg_skel-0.3.4/pcg_skel/skel_utils.py`

 * *Files identical despite different names*

### Comparing `pcg_skel-0.3.3/pcg_skel/utils.py` & `pcg_skel-0.3.4/pcg_skel/utils.py`

 * *Files identical despite different names*

### Comparing `pcg_skel-0.3.3/pcg_skel.egg-info/PKG-INFO` & `pcg_skel-0.3.4/pcg_skel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcg-skel
-Version: 0.3.3
+Version: 0.3.4
 Summary: Skeletonization using the pychunkedgraph
 Home-page: https://github.com/AllenInstitute/pcg_skel
 Author: Casey Schneider-mizell
 Author-email: caseys@alleninstitute.org
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `pcg_skel-0.3.3/setup.py` & `pcg_skel-0.3.4/setup.py`

 * *Files identical despite different names*

