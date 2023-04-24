# Comparing `tmp/DA4RDM-RecSys-UserBased-1.0.8.tar.gz` & `tmp/DA4RDM-RecSys-UserBased-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DA4RDM-RecSys-UserBased-1.0.8.tar", last modified: Tue Feb  7 17:37:13 2023, max compression
+gzip compressed data, was "DA4RDM-RecSys-UserBased-1.0.9.tar", last modified: Thu Feb 16 12:39:15 2023, max compression
```

## Comparing `DA4RDM-RecSys-UserBased-1.0.8.tar` & `DA4RDM-RecSys-UserBased-1.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-02-07 17:37:13.036358 DA4RDM-RecSys-UserBased-1.0.8/
--rw-rw-rw-   0        0        0     1089 2022-07-12 10:21:29.000000 DA4RDM-RecSys-UserBased-1.0.8/LICENSE
--rw-rw-rw-   0        0        0      650 2023-02-07 17:37:13.036358 DA4RDM-RecSys-UserBased-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      219 2023-02-07 15:07:46.000000 DA4RDM-RecSys-UserBased-1.0.8/README.md
--rw-rw-rw-   0        0        0      575 2023-02-07 17:36:48.000000 DA4RDM-RecSys-UserBased-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-07 17:37:13.036358 DA4RDM-RecSys-UserBased-1.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-02-07 17:37:12.926578 DA4RDM-RecSys-UserBased-1.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-02-07 17:37:13.005136 DA4RDM-RecSys-UserBased-1.0.8/src/DA4RDM_RecSys_UserBased/
--rw-rw-rw-   0        0        0        0 2023-02-01 11:55:52.000000 DA4RDM-RecSys-UserBased-1.0.8/src/DA4RDM_RecSys_UserBased/__init__.py
--rw-rw-rw-   0        0        0     3230 2023-02-07 17:36:16.000000 DA4RDM-RecSys-UserBased-1.0.8/src/DA4RDM_RecSys_UserBased/create_matrix.py
--rw-rw-rw-   0        0        0     2909 2022-10-25 06:29:41.000000 DA4RDM-RecSys-UserBased-1.0.8/src/DA4RDM_RecSys_UserBased/evaluate_interest_rating.py
--rw-rw-rw-   0        0        0     4243 2023-02-07 17:27:58.000000 DA4RDM-RecSys-UserBased-1.0.8/src/DA4RDM_RecSys_UserBased/evaluate_weight.py
--rw-rw-rw-   0        0        0      278 2022-10-20 06:46:08.000000 DA4RDM-RecSys-UserBased-1.0.8/src/DA4RDM_RecSys_UserBased/extract_data.py
--rw-rw-rw-   0        0        0     1745 2023-02-07 17:28:18.000000 DA4RDM-RecSys-UserBased-1.0.8/src/DA4RDM_RecSys_UserBased/get_recommendation.py
--rw-rw-rw-   0        0        0      641 2022-10-20 08:07:15.000000 DA4RDM-RecSys-UserBased-1.0.8/src/DA4RDM_RecSys_UserBased/get_roles.py
--rw-rw-rw-   0        0        0     3306 2023-02-07 13:57:41.000000 DA4RDM-RecSys-UserBased-1.0.8/src/DA4RDM_RecSys_UserBased/recommendation.py
--rw-rw-rw-   0        0        0     1724 2023-02-07 13:34:12.000000 DA4RDM-RecSys-UserBased-1.0.8/src/DA4RDM_RecSys_UserBased/remove_outliers.py
-drwxrwxrwx   0        0        0        0 2023-02-07 17:37:13.020741 DA4RDM-RecSys-UserBased-1.0.8/src/DA4RDM_RecSys_UserBased.egg-info/
--rw-rw-rw-   0        0        0      650 2023-02-07 17:37:12.000000 DA4RDM-RecSys-UserBased-1.0.8/src/DA4RDM_RecSys_UserBased.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      702 2023-02-07 17:37:12.000000 DA4RDM-RecSys-UserBased-1.0.8/src/DA4RDM_RecSys_UserBased.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-07 17:37:12.000000 DA4RDM-RecSys-UserBased-1.0.8/src/DA4RDM_RecSys_UserBased.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-02-07 17:37:12.000000 DA4RDM-RecSys-UserBased-1.0.8/src/DA4RDM_RecSys_UserBased.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-02-07 17:37:12.000000 DA4RDM-RecSys-UserBased-1.0.8/src/DA4RDM_RecSys_UserBased.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-02-16 12:39:15.865031 DA4RDM-RecSys-UserBased-1.0.9/
+-rw-rw-rw-   0        0        0     1089 2022-07-12 10:21:29.000000 DA4RDM-RecSys-UserBased-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0      650 2023-02-16 12:39:15.864032 DA4RDM-RecSys-UserBased-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2023-02-07 15:07:46.000000 DA4RDM-RecSys-UserBased-1.0.9/README.md
+-rw-rw-rw-   0        0        0      575 2023-02-16 12:37:18.000000 DA4RDM-RecSys-UserBased-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-02-16 12:39:15.865031 DA4RDM-RecSys-UserBased-1.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-02-16 12:39:15.726834 DA4RDM-RecSys-UserBased-1.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-02-16 12:39:15.825841 DA4RDM-RecSys-UserBased-1.0.9/src/DA4RDM_RecSys_UserBased/
+-rw-rw-rw-   0        0        0        0 2023-02-01 11:55:52.000000 DA4RDM-RecSys-UserBased-1.0.9/src/DA4RDM_RecSys_UserBased/__init__.py
+-rw-rw-rw-   0        0        0     3230 2023-02-07 17:36:16.000000 DA4RDM-RecSys-UserBased-1.0.9/src/DA4RDM_RecSys_UserBased/create_matrix.py
+-rw-rw-rw-   0        0        0     2909 2022-10-25 06:29:41.000000 DA4RDM-RecSys-UserBased-1.0.9/src/DA4RDM_RecSys_UserBased/evaluate_interest_rating.py
+-rw-rw-rw-   0        0        0     4243 2023-02-07 17:27:58.000000 DA4RDM-RecSys-UserBased-1.0.9/src/DA4RDM_RecSys_UserBased/evaluate_weight.py
+-rw-rw-rw-   0        0        0      278 2022-10-20 06:46:08.000000 DA4RDM-RecSys-UserBased-1.0.9/src/DA4RDM_RecSys_UserBased/extract_data.py
+-rw-rw-rw-   0        0        0     1745 2023-02-07 17:28:18.000000 DA4RDM-RecSys-UserBased-1.0.9/src/DA4RDM_RecSys_UserBased/get_recommendation.py
+-rw-rw-rw-   0        0        0      641 2022-10-20 08:07:15.000000 DA4RDM-RecSys-UserBased-1.0.9/src/DA4RDM_RecSys_UserBased/get_roles.py
+-rw-rw-rw-   0        0        0     3306 2023-02-07 13:57:41.000000 DA4RDM-RecSys-UserBased-1.0.9/src/DA4RDM_RecSys_UserBased/recommendation.py
+-rw-rw-rw-   0        0        0     1724 2023-02-07 13:34:12.000000 DA4RDM-RecSys-UserBased-1.0.9/src/DA4RDM_RecSys_UserBased/remove_outliers.py
+drwxrwxrwx   0        0        0        0 2023-02-16 12:39:15.861035 DA4RDM-RecSys-UserBased-1.0.9/src/DA4RDM_RecSys_UserBased.egg-info/
+-rw-rw-rw-   0        0        0      650 2023-02-16 12:39:15.000000 DA4RDM-RecSys-UserBased-1.0.9/src/DA4RDM_RecSys_UserBased.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      702 2023-02-16 12:39:15.000000 DA4RDM-RecSys-UserBased-1.0.9/src/DA4RDM_RecSys_UserBased.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-16 12:39:15.000000 DA4RDM-RecSys-UserBased-1.0.9/src/DA4RDM_RecSys_UserBased.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-02-16 12:39:15.000000 DA4RDM-RecSys-UserBased-1.0.9/src/DA4RDM_RecSys_UserBased.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-02-16 12:39:15.000000 DA4RDM-RecSys-UserBased-1.0.9/src/DA4RDM_RecSys_UserBased.egg-info/top_level.txt
```

### Comparing `DA4RDM-RecSys-UserBased-1.0.8/LICENSE` & `DA4RDM-RecSys-UserBased-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `DA4RDM-RecSys-UserBased-1.0.8/PKG-INFO` & `DA4RDM-RecSys-UserBased-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DA4RDM-RecSys-UserBased
-Version: 1.0.8
+Version: 1.0.9
 Summary: A package that recommends similar data collections based on the analysis of user-resource interaction patterns.
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `DA4RDM-RecSys-UserBased-1.0.8/pyproject.toml` & `DA4RDM-RecSys-UserBased-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "DA4RDM-RecSys-UserBased"
-version = "1.0.8"
+version = "1.0.9"
 description = "A package that recommends similar data collections based on the analysis of user-resource interaction patterns."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `DA4RDM-RecSys-UserBased-1.0.8/src/DA4RDM_RecSys_UserBased/create_matrix.py` & `DA4RDM-RecSys-UserBased-1.0.9/src/DA4RDM_RecSys_UserBased/create_matrix.py`

 * *Files identical despite different names*

### Comparing `DA4RDM-RecSys-UserBased-1.0.8/src/DA4RDM_RecSys_UserBased/evaluate_interest_rating.py` & `DA4RDM-RecSys-UserBased-1.0.9/src/DA4RDM_RecSys_UserBased/evaluate_interest_rating.py`

 * *Files identical despite different names*

### Comparing `DA4RDM-RecSys-UserBased-1.0.8/src/DA4RDM_RecSys_UserBased/evaluate_weight.py` & `DA4RDM-RecSys-UserBased-1.0.9/src/DA4RDM_RecSys_UserBased/evaluate_weight.py`

 * *Files identical despite different names*

### Comparing `DA4RDM-RecSys-UserBased-1.0.8/src/DA4RDM_RecSys_UserBased/get_recommendation.py` & `DA4RDM-RecSys-UserBased-1.0.9/src/DA4RDM_RecSys_UserBased/get_recommendation.py`

 * *Files identical despite different names*

### Comparing `DA4RDM-RecSys-UserBased-1.0.8/src/DA4RDM_RecSys_UserBased/get_roles.py` & `DA4RDM-RecSys-UserBased-1.0.9/src/DA4RDM_RecSys_UserBased/get_roles.py`

 * *Files identical despite different names*

### Comparing `DA4RDM-RecSys-UserBased-1.0.8/src/DA4RDM_RecSys_UserBased/recommendation.py` & `DA4RDM-RecSys-UserBased-1.0.9/src/DA4RDM_RecSys_UserBased/recommendation.py`

 * *Files identical despite different names*

### Comparing `DA4RDM-RecSys-UserBased-1.0.8/src/DA4RDM_RecSys_UserBased/remove_outliers.py` & `DA4RDM-RecSys-UserBased-1.0.9/src/DA4RDM_RecSys_UserBased/remove_outliers.py`

 * *Files identical despite different names*

### Comparing `DA4RDM-RecSys-UserBased-1.0.8/src/DA4RDM_RecSys_UserBased.egg-info/PKG-INFO` & `DA4RDM-RecSys-UserBased-1.0.9/src/DA4RDM_RecSys_UserBased.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DA4RDM-RecSys-UserBased
-Version: 1.0.8
+Version: 1.0.9
 Summary: A package that recommends similar data collections based on the analysis of user-resource interaction patterns.
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `DA4RDM-RecSys-UserBased-1.0.8/src/DA4RDM_RecSys_UserBased.egg-info/SOURCES.txt` & `DA4RDM-RecSys-UserBased-1.0.9/src/DA4RDM_RecSys_UserBased.egg-info/SOURCES.txt`

 * *Files identical despite different names*

