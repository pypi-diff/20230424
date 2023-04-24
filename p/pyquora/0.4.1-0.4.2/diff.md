# Comparing `tmp/pyquora-0.4.1.tar.gz` & `tmp/pyquora-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyquora-0.4.1.tar", last modified: Sun Apr 16 09:25:40 2023, max compression
+gzip compressed data, was "pyquora-0.4.2.tar", last modified: Mon Apr 24 06:45:13 2023, max compression
```

## Comparing `pyquora-0.4.1.tar` & `pyquora-0.4.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:25:40.021825 pyquora-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-16 09:25:27.000000 pyquora-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-16 09:25:27.000000 pyquora-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-16 09:25:40.021825 pyquora-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-16 09:25:27.000000 pyquora-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:25:40.021825 pyquora-0.4.1/pyquora.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-16 09:25:39.000000 pyquora-0.4.1/pyquora.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-16 09:25:39.000000 pyquora-0.4.1/pyquora.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 09:25:39.000000 pyquora-0.4.1/pyquora.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-16 09:25:39.000000 pyquora-0.4.1/pyquora.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-16 09:25:39.000000 pyquora-0.4.1/pyquora.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:25:40.021825 pyquora-0.4.1/quora/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-16 09:25:27.000000 pyquora-0.4.1/quora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 09:25:27.000000 pyquora-0.4.1/quora/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-16 09:25:27.000000 pyquora-0.4.1/quora/_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-16 09:25:27.000000 pyquora-0.4.1/quora/answer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-16 09:25:27.000000 pyquora-0.4.1/quora/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-16 09:25:27.000000 pyquora-0.4.1/quora/content.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-16 09:25:27.000000 pyquora-0.4.1/quora/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-16 09:25:27.000000 pyquora-0.4.1/quora/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-16 09:25:27.000000 pyquora-0.4.1/quora/question.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-16 09:25:27.000000 pyquora-0.4.1/quora/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-16 09:25:27.000000 pyquora-0.4.1/quora/topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-04-16 09:25:27.000000 pyquora-0.4.1/quora/user.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 09:25:40.021825 pyquora-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-16 09:25:27.000000 pyquora-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:45:13.144856 pyquora-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-24 06:45:03.000000 pyquora-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-24 06:45:03.000000 pyquora-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-24 06:45:13.144856 pyquora-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-24 06:45:03.000000 pyquora-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:45:13.144856 pyquora-0.4.2/pyquora.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-24 06:45:13.000000 pyquora-0.4.2/pyquora.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-24 06:45:13.000000 pyquora-0.4.2/pyquora.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 06:45:13.000000 pyquora-0.4.2/pyquora.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-24 06:45:13.000000 pyquora-0.4.2/pyquora.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 06:45:13.000000 pyquora-0.4.2/pyquora.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:45:13.144856 pyquora-0.4.2/quora/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-24 06:45:03.000000 pyquora-0.4.2/quora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:45:03.000000 pyquora-0.4.2/quora/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-24 06:45:03.000000 pyquora-0.4.2/quora/_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-24 06:45:03.000000 pyquora-0.4.2/quora/answer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-24 06:45:03.000000 pyquora-0.4.2/quora/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-24 06:45:03.000000 pyquora-0.4.2/quora/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-24 06:45:03.000000 pyquora-0.4.2/quora/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-04-24 06:45:03.000000 pyquora-0.4.2/quora/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-24 06:45:03.000000 pyquora-0.4.2/quora/question.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-24 06:45:03.000000 pyquora-0.4.2/quora/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-24 06:45:03.000000 pyquora-0.4.2/quora/topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-04-24 06:45:03.000000 pyquora-0.4.2/quora/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 06:45:13.144856 pyquora-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-24 06:45:03.000000 pyquora-0.4.2/setup.py
```

### Comparing `pyquora-0.4.1/LICENSE` & `pyquora-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyquora-0.4.1/PKG-INFO` & `pyquora-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyquora
-Version: 0.4.1
+Version: 0.4.2
 Summary: Fetch profiles and data from Quora.
 Home-page: https://github.com/TheShubhendra/pyquora
 Author: Shubhendra Kushwaha
 Author-email: shubhendrakushwaha94@gmail.com
 License: MIT
 Keywords: scraper,quora
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyquora-0.4.1/README.md` & `pyquora-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pyquora-0.4.1/pyquora.egg-info/PKG-INFO` & `pyquora-0.4.2/pyquora.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyquora
-Version: 0.4.1
+Version: 0.4.2
 Summary: Fetch profiles and data from Quora.
 Home-page: https://github.com/TheShubhendra/pyquora
 Author: Shubhendra Kushwaha
 Author-email: shubhendrakushwaha94@gmail.com
 License: MIT
 Keywords: scraper,quora
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyquora-0.4.1/quora/_parsers.py` & `pyquora-0.4.2/quora/_parsers.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,27 +2,26 @@
 import json
 import re
 
 from quora.answer import Answer
 from quora.topic import Topic
 from .exceptions import ProfileNotFoundError
 
-# noqa: E501
+
 def parse_page(html_data, user):
     """Parse HTML and return JSON."""
     try:
         data = re.search(
             r'window\.ansFrontendGlobals\.data\.inlineQueryResults\.results\[".*\]\.push\((?P<extracted_data>\".*\")\);',
             html_data,
-        )
+        )  # noqa: E501
         data = data.group('extracted_data')
         data = json.loads(json.loads(data))
         return data["data"]["user"]
     except Exception as e:
-        # user.logger.warn("Unable to Parse the profile")
         raise ProfileNotFoundError(
             f"No profile\
 found with the username {user.username}."
         )
 
 
 def parse_answers(json_data, user, language):
```

### Comparing `pyquora-0.4.1/quora/answer.py` & `pyquora-0.4.2/quora/answer.py`

 * *Files identical despite different names*

### Comparing `pyquora-0.4.1/quora/cache.py` & `pyquora-0.4.2/quora/cache.py`

 * *Files identical despite different names*

### Comparing `pyquora-0.4.1/quora/content.py` & `pyquora-0.4.2/quora/content.py`

 * *Files identical despite different names*

### Comparing `pyquora-0.4.1/quora/profile.py` & `pyquora-0.4.2/quora/profile.py`

 * *Files 25% similar despite different names*

```diff
@@ -22,21 +22,23 @@
         except Exception:
             self.lastName = None
         try:
             self.profileCrendential = data["profileCredential"]["experience"]
         except Exception:
             self.profileCrendential = None
         try:
-            text = ""
-            description = json.loads(data.get("description"))
-            for section in description["sections"]:
-                for span in section["spans"]:
-                    text += span["text"]
-                text += "\n"
-            self.profileBio = text
+            description = json.loads(
+                data['descriptionQtextDocument']['legacyJson'])
+            description = description['sections']
+            bio = ''
+            for i in range(len(description)):
+                for key in description[i]['spans']:
+                    bio += key['text'] + '\n'
+            self.profileBio = bio
+
         except Exception:
             self.profileBio = "Not Available"
         self.contributingSpaceCount = data.get("numCanContributeTribes")
         self.twitterProfileUrl = data.get("twitterProfileUrl")
         self.answerViewsCount = data.get("allTimePublicAnswerViews")
         self.contentViewsCount = data.get("allTimePublicContentViews")
         self.lastMonthContentView = data.get("lastMonthPublicContentViews")
```

### Comparing `pyquora-0.4.1/quora/sync.py` & `pyquora-0.4.2/quora/sync.py`

 * *Files identical despite different names*

### Comparing `pyquora-0.4.1/quora/topic.py` & `pyquora-0.4.2/quora/topic.py`

 * *Files identical despite different names*

### Comparing `pyquora-0.4.1/quora/user.py` & `pyquora-0.4.2/quora/user.py`

 * *Files identical despite different names*

### Comparing `pyquora-0.4.1/setup.py` & `pyquora-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         requirements = f.read()
     return requirements
 
 
 setup(
     name="pyquora",
     packages=find_packages(),
-    version="0.4.1",
+    version="0.4.2",
     license="MIT",
     description="""Fetch profiles and data from Quora.""",
     author="Shubhendra Kushwaha",
     author_email="shubhendrakushwaha94@gmail.com",
     url="https://github.com/TheShubhendra/pyquora",
     keywords=[
         "scraper",
```

