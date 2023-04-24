# Comparing `tmp/axdd-person-client-1.1.2.tar.gz` & `tmp/axdd-person-client-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axdd-person-client-1.1.2.tar", last modified: Wed Apr 19 16:41:21 2023, max compression
+gzip compressed data, was "axdd-person-client-1.1.3.tar", last modified: Mon Apr 24 19:23:22 2023, max compression
```

## Comparing `axdd-person-client-1.1.2.tar` & `axdd-person-client-1.1.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 16:41:21.067101 axdd-person-client-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-04-19 16:41:11.000000 axdd-person-client-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-04-19 16:41:21.067101 axdd-person-client-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      615 2023-04-19 16:41:11.000000 axdd-person-client-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 16:41:21.063101 axdd-person-client-1.1.2/axdd_person_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-04-19 16:41:20.000000 axdd-person-client-1.1.2/axdd_person_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      779 2023-04-19 16:41:21.000000 axdd-person-client-1.1.2/axdd_person_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-19 16:41:20.000000 axdd-person-client-1.1.2/axdd_person_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-04-19 16:41:20.000000 axdd-person-client-1.1.2/axdd_person_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-04-19 16:41:20.000000 axdd-person-client-1.1.2/axdd_person_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 16:41:21.063101 axdd-person-client-1.1.2/conf/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 16:41:11.000000 axdd-person-client-1.1.2/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      869 2023-04-19 16:41:11.000000 axdd-person-client-1.1.2/conf/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-19 16:41:21.067101 axdd-person-client-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1509 2023-04-19 16:41:11.000000 axdd-person-client-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 16:41:21.063101 axdd-person-client-1.1.2/uw_person_client/
--rw-r--r--   0 runner    (1001) docker     (122)      470 2023-04-19 16:41:11.000000 axdd-person-client-1.1.2/uw_person_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 16:41:21.063101 axdd-person-client-1.1.2/uw_person_client/clients/
--rw-r--r--   0 runner    (1001) docker     (122)     1018 2023-04-19 16:41:11.000000 axdd-person-client-1.1.2/uw_person_client/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    24773 2023-04-19 16:41:11.000000 axdd-person-client-1.1.2/uw_person_client/clients/core_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     4733 2023-04-19 16:41:11.000000 axdd-person-client-1.1.2/uw_person_client/clients/mock_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     3309 2023-04-19 16:41:11.000000 axdd-person-client-1.1.2/uw_person_client/components.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 16:41:21.063101 axdd-person-client-1.1.2/uw_person_client/databases/
--rw-r--r--   0 runner    (1001) docker     (122)      828 2023-04-19 16:41:11.000000 axdd-person-client-1.1.2/uw_person_client/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      881 2023-04-19 16:41:11.000000 axdd-person-client-1.1.2/uw_person_client/databases/postgres.py
--rw-r--r--   0 runner    (1001) docker     (122)     5633 2023-04-19 16:41:11.000000 axdd-person-client-1.1.2/uw_person_client/databases/uwpds.py
--rw-r--r--   0 runner    (1001) docker     (122)      194 2023-04-19 16:41:11.000000 axdd-person-client-1.1.2/uw_person_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      349 2023-04-19 16:41:11.000000 axdd-person-client-1.1.2/uw_person_client/test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 16:41:21.067101 axdd-person-client-1.1.2/uw_person_client/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 16:41:11.000000 axdd-person-client-1.1.2/uw_person_client/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      501 2023-04-19 16:41:11.000000 axdd-person-client-1.1.2/uw_person_client/tests/test_components.py
--rw-r--r--   0 runner    (1001) docker     (122)    33750 2023-04-19 16:41:11.000000 axdd-person-client-1.1.2/uw_person_client/tests/test_core_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     3881 2023-04-19 16:41:11.000000 axdd-person-client-1.1.2/uw_person_client/tests/test_mock_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 19:23:22.856109 axdd-person-client-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-04-24 19:23:13.000000 axdd-person-client-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-04-24 19:23:22.856109 axdd-person-client-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      615 2023-04-24 19:23:13.000000 axdd-person-client-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 19:23:22.852108 axdd-person-client-1.1.3/axdd_person_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-04-24 19:23:22.000000 axdd-person-client-1.1.3/axdd_person_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      779 2023-04-24 19:23:22.000000 axdd-person-client-1.1.3/axdd_person_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-24 19:23:22.000000 axdd-person-client-1.1.3/axdd_person_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-04-24 19:23:22.000000 axdd-person-client-1.1.3/axdd_person_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-04-24 19:23:22.000000 axdd-person-client-1.1.3/axdd_person_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 19:23:22.852108 axdd-person-client-1.1.3/conf/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 19:23:13.000000 axdd-person-client-1.1.3/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      869 2023-04-24 19:23:13.000000 axdd-person-client-1.1.3/conf/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-24 19:23:22.856109 axdd-person-client-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1509 2023-04-24 19:23:13.000000 axdd-person-client-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 19:23:22.856109 axdd-person-client-1.1.3/uw_person_client/
+-rw-r--r--   0 runner    (1001) docker     (122)      470 2023-04-24 19:23:13.000000 axdd-person-client-1.1.3/uw_person_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 19:23:22.856109 axdd-person-client-1.1.3/uw_person_client/clients/
+-rw-r--r--   0 runner    (1001) docker     (122)     1018 2023-04-24 19:23:13.000000 axdd-person-client-1.1.3/uw_person_client/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25233 2023-04-24 19:23:13.000000 axdd-person-client-1.1.3/uw_person_client/clients/core_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4733 2023-04-24 19:23:13.000000 axdd-person-client-1.1.3/uw_person_client/clients/mock_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3309 2023-04-24 19:23:13.000000 axdd-person-client-1.1.3/uw_person_client/components.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 19:23:22.856109 axdd-person-client-1.1.3/uw_person_client/databases/
+-rw-r--r--   0 runner    (1001) docker     (122)      828 2023-04-24 19:23:13.000000 axdd-person-client-1.1.3/uw_person_client/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      881 2023-04-24 19:23:13.000000 axdd-person-client-1.1.3/uw_person_client/databases/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5633 2023-04-24 19:23:13.000000 axdd-person-client-1.1.3/uw_person_client/databases/uwpds.py
+-rw-r--r--   0 runner    (1001) docker     (122)      194 2023-04-24 19:23:13.000000 axdd-person-client-1.1.3/uw_person_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      349 2023-04-24 19:23:13.000000 axdd-person-client-1.1.3/uw_person_client/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 19:23:22.856109 axdd-person-client-1.1.3/uw_person_client/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 19:23:13.000000 axdd-person-client-1.1.3/uw_person_client/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      501 2023-04-24 19:23:13.000000 axdd-person-client-1.1.3/uw_person_client/tests/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33750 2023-04-24 19:23:13.000000 axdd-person-client-1.1.3/uw_person_client/tests/test_core_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3881 2023-04-24 19:23:13.000000 axdd-person-client-1.1.3/uw_person_client/tests/test_mock_client.py
```

### Comparing `axdd-person-client-1.1.2/LICENSE` & `axdd-person-client-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.2/PKG-INFO` & `axdd-person-client-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: axdd-person-client
-Version: 1.1.2
+Version: 1.1.3
 Summary: A library for connecting to and querying the uw-person-datastore
 Home-page: https://github.com/uw-it-aca/axdd-person-client
 Author: UW-IT AXDD
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Description: 
         See the README on `GitHub
```

### Comparing `axdd-person-client-1.1.2/README.md` & `axdd-person-client-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.2/axdd_person_client.egg-info/PKG-INFO` & `axdd-person-client-1.1.3/axdd_person_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: axdd-person-client
-Version: 1.1.2
+Version: 1.1.3
 Summary: A library for connecting to and querying the uw-person-datastore
 Home-page: https://github.com/uw-it-aca/axdd-person-client
 Author: UW-IT AXDD
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Description: 
         See the README on `GitHub
```

### Comparing `axdd-person-client-1.1.2/axdd_person_client.egg-info/SOURCES.txt` & `axdd-person-client-1.1.3/axdd_person_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.2/conf/settings.py` & `axdd-person-client-1.1.3/conf/settings.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.2/setup.py` & `axdd-person-client-1.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.2/uw_person_client/clients/__init__.py` & `axdd-person-client-1.1.3/uw_person_client/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.2/uw_person_client/clients/core_client.py` & `axdd-person-client-1.1.3/uw_person_client/clients/core_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -460,22 +460,29 @@
         transcript.over_qtr_grade_pt = sqla_transcript.over_qtr_grade_pt
         transcript.over_qtr_grade_at = sqla_transcript.over_qtr_grade_at
         transcript.over_qtr_nongrd = sqla_transcript.over_qtr_nongrd
         transcript.over_qtr_deduct = sqla_transcript.over_qtr_deduct
         transcript.qtr_comment = sqla_transcript.qtr_comment
         transcript.honors_program = sqla_transcript.honors_program
         transcript.special_program = sqla_transcript.special_program
+        transcript.special_program_desc = sqla_transcript.special_program_desc
         transcript.scholarship_type = sqla_transcript.scholarship_type
+        transcript.scholarship_abbr = sqla_transcript.scholarship_abbr
+        transcript.scholarship_desc = sqla_transcript.scholarship_desc
         transcript.yearly_honor_type = sqla_transcript.yearly_honor_type
         transcript.exemption_code = sqla_transcript.exemption_code
         transcript.num_ind_study = sqla_transcript.num_ind_study
         transcript.num_courses = sqla_transcript.num_courses
         transcript.enroll_status = sqla_transcript.enroll_status
+        transcript.enroll_status_request_code = \
+            sqla_transcript.enroll_status_request_code
+        transcript.enroll_status_desc = sqla_transcript.enroll_status_desc
         transcript.tenth_day_credits = float(sqla_transcript.tenth_day_credits)
         transcript.tr_en_stat_dt = sqla_transcript.tr_en_stat_dt
+        transcript.add_to_cum = sqla_transcript.add_to_cum
         return transcript
 
     def _map_transfer(self, sqla_transfer):
         transfer = Transfer()
         transfer.institution_code = sqla_transfer.institution_code
         transfer.year_ending = sqla_transfer.year_ending
         transfer.year_beginning = sqla_transfer.year_beginning
```

### Comparing `axdd-person-client-1.1.2/uw_person_client/clients/mock_client.py` & `axdd-person-client-1.1.3/uw_person_client/clients/mock_client.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.2/uw_person_client/components.py` & `axdd-person-client-1.1.3/uw_person_client/components.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.2/uw_person_client/databases/__init__.py` & `axdd-person-client-1.1.3/uw_person_client/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.2/uw_person_client/databases/postgres.py` & `axdd-person-client-1.1.3/uw_person_client/databases/postgres.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.2/uw_person_client/databases/uwpds.py` & `axdd-person-client-1.1.3/uw_person_client/databases/uwpds.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.2/uw_person_client/tests/test_core_client.py` & `axdd-person-client-1.1.3/uw_person_client/tests/test_core_client.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.2/uw_person_client/tests/test_mock_client.py` & `axdd-person-client-1.1.3/uw_person_client/tests/test_mock_client.py`

 * *Files identical despite different names*

