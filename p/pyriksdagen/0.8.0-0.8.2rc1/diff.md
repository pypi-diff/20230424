# Comparing `tmp/pyriksdagen-0.8.0.tar.gz` & `tmp/pyriksdagen-0.8.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyriksdagen-0.8.0.tar", max compression
+gzip compressed data, was "pyriksdagen-0.8.2rc1.tar", max compression
```

## Comparing `pyriksdagen-0.8.0.tar` & `pyriksdagen-0.8.2rc1.tar`

### file list

```diff
@@ -1,40 +1,39 @@
--rw-r--r--   0        0        0     1249 2022-11-01 12:04:45.361073 pyriksdagen-0.8.0/LICENSE
--rw-r--r--   0        0        0     3519 2023-04-12 10:51:21.978195 pyriksdagen-0.8.0/README.md
--rw-r--r--   0        0        0      745 2023-04-12 11:07:15.247115 pyriksdagen-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1107 2022-11-01 12:05:01.901342 pyriksdagen-0.8.0/pyriksdagen/LICENSE
--rw-r--r--   0        0        0       84 2022-11-01 12:05:01.901407 pyriksdagen-0.8.0/pyriksdagen/__init__.py
--rw-r--r--   0        0        0      225 2022-11-01 12:05:01.901564 pyriksdagen-0.8.0/pyriksdagen/data/queries/alias.rq
--rw-r--r--   0        0        0      494 2023-02-07 15:52:31.495339 pyriksdagen-0.8.0/pyriksdagen/data/queries/government.rq
--rw-r--r--   0        0        0      729 2023-02-07 15:52:31.495749 pyriksdagen-0.8.0/pyriksdagen/data/queries/member_of_parliament.rq
--rw-r--r--   0        0        0      148 2022-11-01 12:05:01.901748 pyriksdagen-0.8.0/pyriksdagen/data/queries/member_of_parliament.txt
--rw-r--r--   0        0        0     1380 2022-11-01 12:05:01.901837 pyriksdagen-0.8.0/pyriksdagen/data/queries/minister.rq
--rw-r--r--   0        0        0      235 2022-11-01 12:05:01.901892 pyriksdagen-0.8.0/pyriksdagen/data/queries/minister.txt
--rw-r--r--   0        0        0      262 2022-11-01 12:05:01.901962 pyriksdagen-0.8.0/pyriksdagen/data/queries/name_location_specifier.rq
--rw-r--r--   0        0        0      484 2023-02-07 15:52:31.496167 pyriksdagen-0.8.0/pyriksdagen/data/queries/party_affiliation.rq
--rw-r--r--   0        0        0      549 2023-02-07 15:52:31.496580 pyriksdagen-0.8.0/pyriksdagen/data/queries/person.rq
--rw-r--r--   0        0        0      616 2022-11-01 12:05:01.902171 pyriksdagen-0.8.0/pyriksdagen/data/queries/speaker.rq
--rw-r--r--   0        0        0      253 2022-11-01 12:05:01.902229 pyriksdagen-0.8.0/pyriksdagen/data/queries/speaker.txt
--rw-r--r--   0        0        0      208 2022-11-01 12:05:01.902286 pyriksdagen-0.8.0/pyriksdagen/data/queries/twitter.rq
--rw-r--r--   0        0        0      225 2022-11-01 12:05:01.902412 pyriksdagen-0.8.0/pyriksdagen/data/queries_backup/alias.rq
--rw-r--r--   0        0        0      482 2022-11-01 12:05:01.902473 pyriksdagen-0.8.0/pyriksdagen/data/queries_backup/government.rq
--rw-r--r--   0        0        0      722 2022-11-01 12:05:01.902539 pyriksdagen-0.8.0/pyriksdagen/data/queries_backup/member_of_parliament.rq
--rw-r--r--   0        0        0     1380 2022-11-01 12:05:01.902591 pyriksdagen-0.8.0/pyriksdagen/data/queries_backup/minister.rq
--rw-r--r--   0        0        0     1013 2022-11-01 12:05:01.902681 pyriksdagen-0.8.0/pyriksdagen/data/queries_backup/name_location_specifier.rq
--rw-r--r--   0        0        0     1230 2022-11-01 12:05:01.902743 pyriksdagen-0.8.0/pyriksdagen/data/queries_backup/party_affiliation.rq
--rw-r--r--   0        0        0     1412 2022-11-01 12:05:01.902796 pyriksdagen-0.8.0/pyriksdagen/data/queries_backup/person.rq
--rw-r--r--   0        0        0      616 2022-11-01 12:05:01.902856 pyriksdagen-0.8.0/pyriksdagen/data/queries_backup/speaker.rq
--rw-r--r--   0        0        0      959 2022-11-01 12:05:01.902940 pyriksdagen-0.8.0/pyriksdagen/data/queries_backup/twitter.rq
--rw-r--r--   0        0        0     2195 2022-11-01 12:05:01.903003 pyriksdagen-0.8.0/pyriksdagen/dataset.py
--rw-r--r--   0        0        0     6193 2023-02-07 15:52:31.497165 pyriksdagen-0.8.0/pyriksdagen/db.py
--rw-r--r--   0        0        0     9747 2023-03-01 12:15:10.843910 pyriksdagen-0.8.0/pyriksdagen/download.py
--rw-r--r--   0        0        0     6813 2023-03-01 12:15:10.844248 pyriksdagen-0.8.0/pyriksdagen/export.py
--rw-r--r--   0        0        0     4532 2022-11-01 12:05:01.903384 pyriksdagen-0.8.0/pyriksdagen/match_mp.py
--rw-r--r--   0        0        0     6915 2023-02-07 15:52:31.497997 pyriksdagen-0.8.0/pyriksdagen/metadata.py
--rw-r--r--   0        0        0    11120 2022-11-01 12:05:01.903558 pyriksdagen-0.8.0/pyriksdagen/mp.py
--rw-r--r--   0        0        0    16044 2023-04-05 08:32:54.043579 pyriksdagen-0.8.0/pyriksdagen/refine.py
--rwxr-xr-x   0        0        0      237 2023-03-01 12:15:10.846196 pyriksdagen-0.8.0/pyriksdagen/requirements.txt
--rw-r--r--   0        0        0     7039 2023-04-05 08:32:54.044723 pyriksdagen-0.8.0/pyriksdagen/segmentation.py
--rw-r--r--   0        0        0     5497 2023-03-01 12:15:10.850360 pyriksdagen-0.8.0/pyriksdagen/utils.py
--rw-r--r--   0        0        0     5265 2023-03-01 12:14:56.389831 pyriksdagen-0.8.0/pyriksdagen/wikidata.py
--rw-r--r--   0        0        0     4545 2023-04-12 11:07:27.882668 pyriksdagen-0.8.0/setup.py
--rw-r--r--   0        0        0     4592 2023-04-12 11:07:27.882917 pyriksdagen-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1249 2023-04-24 12:55:27.543987 pyriksdagen-0.8.2rc1/LICENSE
+-rw-r--r--   0        0        0     3520 2023-04-24 12:55:27.543987 pyriksdagen-0.8.2rc1/README.md
+-rw-r--r--   0        0        0      748 2023-04-24 12:58:08.311789 pyriksdagen-0.8.2rc1/pyproject.toml
+-rw-r--r--   0        0        0     1107 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/LICENSE
+-rw-r--r--   0        0        0       84 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/__init__.py
+-rw-r--r--   0        0        0      225 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/data/queries/alias.rq
+-rw-r--r--   0        0        0      494 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/data/queries/government.rq
+-rw-r--r--   0        0        0      729 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/data/queries/member_of_parliament.rq
+-rw-r--r--   0        0        0      148 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/data/queries/member_of_parliament.txt
+-rw-r--r--   0        0        0     1380 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/data/queries/minister.rq
+-rw-r--r--   0        0        0      235 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/data/queries/minister.txt
+-rw-r--r--   0        0        0      262 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/data/queries/name_location_specifier.rq
+-rw-r--r--   0        0        0      484 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/data/queries/party_affiliation.rq
+-rw-r--r--   0        0        0      549 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/data/queries/person.rq
+-rw-r--r--   0        0        0      616 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/data/queries/speaker.rq
+-rw-r--r--   0        0        0      253 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/data/queries/speaker.txt
+-rw-r--r--   0        0        0      208 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/data/queries/twitter.rq
+-rw-r--r--   0        0        0      225 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/data/queries_backup/alias.rq
+-rw-r--r--   0        0        0      482 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/data/queries_backup/government.rq
+-rw-r--r--   0        0        0      722 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/data/queries_backup/member_of_parliament.rq
+-rw-r--r--   0        0        0     1380 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/data/queries_backup/minister.rq
+-rw-r--r--   0        0        0     1013 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/data/queries_backup/name_location_specifier.rq
+-rw-r--r--   0        0        0     1230 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/data/queries_backup/party_affiliation.rq
+-rw-r--r--   0        0        0     1412 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/data/queries_backup/person.rq
+-rw-r--r--   0        0        0      616 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/data/queries_backup/speaker.rq
+-rw-r--r--   0        0        0      959 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/data/queries_backup/twitter.rq
+-rw-r--r--   0        0        0     2195 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/dataset.py
+-rw-r--r--   0        0        0     6193 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/db.py
+-rw-r--r--   0        0        0     9747 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/download.py
+-rw-r--r--   0        0        0     6813 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/export.py
+-rw-r--r--   0        0        0     4532 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/match_mp.py
+-rw-r--r--   0        0        0     6915 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/metadata.py
+-rw-r--r--   0        0        0    11120 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/mp.py
+-rw-r--r--   0        0        0    16044 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/refine.py
+-rwxr-xr-x   0        0        0      237 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/requirements.txt
+-rw-r--r--   0        0        0     7053 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/segmentation.py
+-rw-r--r--   0        0        0     5497 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/utils.py
+-rw-r--r--   0        0        0     5265 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/wikidata.py
+-rw-r--r--   0        0        0     4647 1970-01-01 00:00:00.000000 pyriksdagen-0.8.2rc1/PKG-INFO
```

### Comparing `pyriksdagen-0.8.0/LICENSE` & `pyriksdagen-0.8.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.0/README.md` & `pyriksdagen-0.8.2rc1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [![Check unchanged](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/check_unchanged.yml/badge.svg)](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/check_unchanged.yml)
 [![Unit tests](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/push.yml/badge.svg)](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/push.yml)
 [![Validate Parla-Clarin XML](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/validate.yml/badge.svg)](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/validate.yml)
 
-# Swedish parliamentary proceedings - Riksdagens protokoll 1867-2023
+# Swedish parliamentary proceedings - Riksdagens protokoll 1867-today
 
 _Westac Project, 2020-2023_
 
 The full data set consists of multiple parts:
 
 - Riksdagens protokoll between from 1867 until today in the [Parla-clarin](https://github.com/clarin-eric/parla-clarin) format
 - Comprehensive list of MPs and cabinet members during this period
```

### Comparing `pyriksdagen-0.8.0/pyproject.toml` & `pyriksdagen-0.8.2rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyriksdagen"
-version = "0.8.0"
+version = "0.8.2rc1"
 description = "Access the Riksdagen corpus"
 authors = ["ninpnin <vainoyrjanainen@icloud.com>"]
 repository = "https://github.com/welfare-state-analytics/riksdagen-corpus"
 readme = "README.md"
 license = "MIT"
 packages = [
     { include = "pyriksdagen", from = "" }
```

### Comparing `pyriksdagen-0.8.0/pyriksdagen/LICENSE` & `pyriksdagen-0.8.2rc1/pyriksdagen/LICENSE`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.0/pyriksdagen/data/queries/member_of_parliament.rq` & `pyriksdagen-0.8.2rc1/pyriksdagen/data/queries/member_of_parliament.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.0/pyriksdagen/data/queries/minister.rq` & `pyriksdagen-0.8.2rc1/pyriksdagen/data/queries/minister.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.0/pyriksdagen/data/queries/person.rq` & `pyriksdagen-0.8.2rc1/pyriksdagen/data/queries/person.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.0/pyriksdagen/data/queries/speaker.rq` & `pyriksdagen-0.8.2rc1/pyriksdagen/data/queries/speaker.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.0/pyriksdagen/data/queries_backup/member_of_parliament.rq` & `pyriksdagen-0.8.2rc1/pyriksdagen/data/queries_backup/member_of_parliament.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.0/pyriksdagen/data/queries_backup/minister.rq` & `pyriksdagen-0.8.2rc1/pyriksdagen/data/queries_backup/minister.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.0/pyriksdagen/data/queries_backup/name_location_specifier.rq` & `pyriksdagen-0.8.2rc1/pyriksdagen/data/queries_backup/name_location_specifier.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.0/pyriksdagen/data/queries_backup/party_affiliation.rq` & `pyriksdagen-0.8.2rc1/pyriksdagen/data/queries_backup/party_affiliation.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.0/pyriksdagen/data/queries_backup/person.rq` & `pyriksdagen-0.8.2rc1/pyriksdagen/data/queries_backup/person.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.0/pyriksdagen/data/queries_backup/speaker.rq` & `pyriksdagen-0.8.2rc1/pyriksdagen/data/queries_backup/speaker.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.0/pyriksdagen/data/queries_backup/twitter.rq` & `pyriksdagen-0.8.2rc1/pyriksdagen/data/queries_backup/twitter.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.0/pyriksdagen/dataset.py` & `pyriksdagen-0.8.2rc1/pyriksdagen/dataset.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.0/pyriksdagen/db.py` & `pyriksdagen-0.8.2rc1/pyriksdagen/db.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.0/pyriksdagen/download.py` & `pyriksdagen-0.8.2rc1/pyriksdagen/download.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.0/pyriksdagen/export.py` & `pyriksdagen-0.8.2rc1/pyriksdagen/export.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.0/pyriksdagen/match_mp.py` & `pyriksdagen-0.8.2rc1/pyriksdagen/match_mp.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.0/pyriksdagen/metadata.py` & `pyriksdagen-0.8.2rc1/pyriksdagen/metadata.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.0/pyriksdagen/mp.py` & `pyriksdagen-0.8.2rc1/pyriksdagen/mp.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.0/pyriksdagen/refine.py` & `pyriksdagen-0.8.2rc1/pyriksdagen/refine.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.0/pyriksdagen/segmentation.py` & `pyriksdagen-0.8.2rc1/pyriksdagen/segmentation.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
         if ", " in s:
             s = s.split(", ")
             s = s[1] + " " + s[0]
         d["name"] = s
 
     if "gender" in d:
         d["gender"] = d["gender"].lower()
-        if d["gender"] == "herr":
+        if d["gender"] in ["herr", "friherre"]:
             d["gender"] = "man"
         if d["gender"] in ["fru", "fröken"]:
             d["gender"] = "woman"
 
     if "specifier" in d:
         d["specifier"] = d["specifier"].replace("i ", "")
```

### Comparing `pyriksdagen-0.8.0/pyriksdagen/utils.py` & `pyriksdagen-0.8.2rc1/pyriksdagen/utils.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.0/pyriksdagen/wikidata.py` & `pyriksdagen-0.8.2rc1/pyriksdagen/wikidata.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.0/PKG-INFO` & `pyriksdagen-0.8.2rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pyriksdagen
-Version: 0.8.0
+Version: 0.8.2rc1
 Summary: Access the Riksdagen corpus
 Home-page: https://github.com/welfare-state-analytics/riksdagen-corpus
 License: MIT
 Author: ninpnin
 Author-email: vainoyrjanainen@icloud.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: SPARQLWrapper
 Requires-Dist: base58
 Requires-Dist: beautifulsoup4
 Requires-Dist: dateparser
 Requires-Dist: importlib_resources
 Requires-Dist: kblab-client
 Requires-Dist: lxml
@@ -31,15 +32,15 @@
 Project-URL: Repository, https://github.com/welfare-state-analytics/riksdagen-corpus
 Description-Content-Type: text/markdown
 
 [![Check unchanged](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/check_unchanged.yml/badge.svg)](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/check_unchanged.yml)
 [![Unit tests](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/push.yml/badge.svg)](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/push.yml)
 [![Validate Parla-Clarin XML](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/validate.yml/badge.svg)](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/validate.yml)
 
-# Swedish parliamentary proceedings - Riksdagens protokoll 1867-2023
+# Swedish parliamentary proceedings - Riksdagens protokoll 1867-today
 
 _Westac Project, 2020-2023_
 
 The full data set consists of multiple parts:
 
 - Riksdagens protokoll between from 1867 until today in the [Parla-clarin](https://github.com/clarin-eric/parla-clarin) format
 - Comprehensive list of MPs and cabinet members during this period
```

