# Comparing `tmp/hearthstone-6.5.1.tar.gz` & `tmp/hearthstone-6.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hearthstone-6.5.1.tar", last modified: Mon Apr 17 18:43:07 2023, max compression
+gzip compressed data, was "hearthstone-6.5.2.tar", last modified: Mon Apr 24 10:53:45 2023, max compression
```

## Comparing `hearthstone-6.5.1.tar` & `hearthstone-6.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:07.991585 hearthstone-6.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-17 18:43:02.000000 hearthstone-6.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-17 18:43:07.991585 hearthstone-6.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-17 18:43:02.000000 hearthstone-6.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:07.991585 hearthstone-6.5.1/hearthstone/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-17 18:43:02.000000 hearthstone-6.5.1/hearthstone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-04-17 18:43:02.000000 hearthstone-6.5.1/hearthstone/bountyxml.py
--rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-04-17 18:43:02.000000 hearthstone-6.5.1/hearthstone/cardxml.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-04-17 18:43:02.000000 hearthstone-6.5.1/hearthstone/dbf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-04-17 18:43:02.000000 hearthstone-6.5.1/hearthstone/deckstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-04-17 18:43:02.000000 hearthstone-6.5.1/hearthstone/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)    58839 2023-04-17 18:43:02.000000 hearthstone-6.5.1/hearthstone/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-04-17 18:43:02.000000 hearthstone-6.5.1/hearthstone/mercenaryxml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-17 18:43:02.000000 hearthstone-6.5.1/hearthstone/stringsfile.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-17 18:43:02.000000 hearthstone-6.5.1/hearthstone/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:07.991585 hearthstone-6.5.1/hearthstone/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    11663 2023-04-17 18:43:02.000000 hearthstone-6.5.1/hearthstone/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-17 18:43:02.000000 hearthstone-6.5.1/hearthstone/xmlutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:43:07.991585 hearthstone-6.5.1/hearthstone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-17 18:43:07.000000 hearthstone-6.5.1/hearthstone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-17 18:43:07.000000 hearthstone-6.5.1/hearthstone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 18:43:07.000000 hearthstone-6.5.1/hearthstone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-17 18:43:07.000000 hearthstone-6.5.1/hearthstone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-17 18:43:07.000000 hearthstone-6.5.1/hearthstone.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 18:43:07.000000 hearthstone-6.5.1/hearthstone.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-17 18:43:07.995585 hearthstone-6.5.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-04-17 18:43:02.000000 hearthstone-6.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:53:45.425326 hearthstone-6.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-24 10:53:31.000000 hearthstone-6.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-24 10:53:45.425326 hearthstone-6.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-24 10:53:31.000000 hearthstone-6.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:53:45.425326 hearthstone-6.5.2/hearthstone/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-24 10:53:31.000000 hearthstone-6.5.2/hearthstone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-04-24 10:53:31.000000 hearthstone-6.5.2/hearthstone/bountyxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-04-24 10:53:31.000000 hearthstone-6.5.2/hearthstone/cardxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-04-24 10:53:31.000000 hearthstone-6.5.2/hearthstone/dbf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-04-24 10:53:31.000000 hearthstone-6.5.2/hearthstone/deckstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-04-24 10:53:31.000000 hearthstone-6.5.2/hearthstone/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58839 2023-04-24 10:53:31.000000 hearthstone-6.5.2/hearthstone/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-04-24 10:53:31.000000 hearthstone-6.5.2/hearthstone/mercenaryxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-24 10:53:31.000000 hearthstone-6.5.2/hearthstone/stringsfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-24 10:53:31.000000 hearthstone-6.5.2/hearthstone/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:53:45.425326 hearthstone-6.5.2/hearthstone/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    11663 2023-04-24 10:53:31.000000 hearthstone-6.5.2/hearthstone/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-24 10:53:31.000000 hearthstone-6.5.2/hearthstone/xmlutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:53:45.425326 hearthstone-6.5.2/hearthstone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-24 10:53:45.000000 hearthstone-6.5.2/hearthstone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-24 10:53:45.000000 hearthstone-6.5.2/hearthstone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 10:53:45.000000 hearthstone-6.5.2/hearthstone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-24 10:53:45.000000 hearthstone-6.5.2/hearthstone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-24 10:53:45.000000 hearthstone-6.5.2/hearthstone.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 10:53:45.000000 hearthstone-6.5.2/hearthstone.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-24 10:53:45.429326 hearthstone-6.5.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-04-24 10:53:31.000000 hearthstone-6.5.2/setup.py
```

### Comparing `hearthstone-6.5.1/LICENSE` & `hearthstone-6.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hearthstone-6.5.1/PKG-INFO` & `hearthstone-6.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hearthstone
-Version: 6.5.1
+Version: 6.5.2
 Summary: CardDefs.xml parser and Hearthstone enums for Python
 Home-page: https://github.com/HearthSim/python-hearthstone/
 Download-URL: https://github.com/HearthSim/python-hearthstone/tarball/master
 Author: Jerome Leclanche
 Author-email: jerome@leclan.ch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `hearthstone-6.5.1/README.md` & `hearthstone-6.5.2/README.md`

 * *Files identical despite different names*

### Comparing `hearthstone-6.5.1/hearthstone/bountyxml.py` & `hearthstone-6.5.2/hearthstone/bountyxml.py`

 * *Files identical despite different names*

### Comparing `hearthstone-6.5.1/hearthstone/cardxml.py` & `hearthstone-6.5.2/hearthstone/cardxml.py`

 * *Files identical despite different names*

### Comparing `hearthstone-6.5.1/hearthstone/dbf.py` & `hearthstone-6.5.2/hearthstone/dbf.py`

 * *Files identical despite different names*

### Comparing `hearthstone-6.5.1/hearthstone/deckstrings.py` & `hearthstone-6.5.2/hearthstone/deckstrings.py`

 * *Files identical despite different names*

### Comparing `hearthstone-6.5.1/hearthstone/entities.py` & `hearthstone-6.5.2/hearthstone/entities.py`

 * *Files identical despite different names*

### Comparing `hearthstone-6.5.1/hearthstone/enums.py` & `hearthstone-6.5.2/hearthstone/enums.py`

 * *Files identical despite different names*

### Comparing `hearthstone-6.5.1/hearthstone/mercenaryxml.py` & `hearthstone-6.5.2/hearthstone/mercenaryxml.py`

 * *Files identical despite different names*

### Comparing `hearthstone-6.5.1/hearthstone/stringsfile.py` & `hearthstone-6.5.2/hearthstone/stringsfile.py`

 * *Files identical despite different names*

### Comparing `hearthstone-6.5.1/hearthstone/utils/__init__.py` & `hearthstone-6.5.2/hearthstone/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hearthstone-6.5.1/hearthstone/xmlutils.py` & `hearthstone-6.5.2/hearthstone/xmlutils.py`

 * *Files identical despite different names*

### Comparing `hearthstone-6.5.1/hearthstone.egg-info/PKG-INFO` & `hearthstone-6.5.2/hearthstone.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hearthstone
-Version: 6.5.1
+Version: 6.5.2
 Summary: CardDefs.xml parser and Hearthstone enums for Python
 Home-page: https://github.com/HearthSim/python-hearthstone/
 Download-URL: https://github.com/HearthSim/python-hearthstone/tarball/master
 Author: Jerome Leclanche
 Author-email: jerome@leclan.ch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `hearthstone-6.5.1/hearthstone.egg-info/SOURCES.txt` & `hearthstone-6.5.2/hearthstone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hearthstone-6.5.1/setup.cfg` & `hearthstone-6.5.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hearthstone
-version = 6.5.1
+version = 6.5.2
 description = CardDefs.xml parser and Hearthstone enums for Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Jerome Leclanche
 author_email = jerome@leclan.ch
 url = https://github.com/HearthSim/python-hearthstone/
 download_url = https://github.com/HearthSim/python-hearthstone/tarball/master
```

