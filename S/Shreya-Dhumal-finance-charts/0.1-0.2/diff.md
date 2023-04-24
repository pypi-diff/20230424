# Comparing `tmp/Shreya-Dhumal-finance-charts-0.1.tar.gz` & `tmp/Shreya-Dhumal-finance-charts-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Shreya-Dhumal-finance-charts-0.1.tar", last modified: Sun Apr 23 20:43:28 2023, max compression
+gzip compressed data, was "Shreya-Dhumal-finance-charts-0.2.tar", last modified: Mon Apr 24 13:18:40 2023, max compression
```

## Comparing `Shreya-Dhumal-finance-charts-0.1.tar` & `Shreya-Dhumal-finance-charts-0.2.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxrwxr-x   0 murali    (1000) murali    (1000)        0 2023-04-23 20:43:28.504900 Shreya-Dhumal-finance-charts-0.1/
--rw-rw-r--   0 murali    (1000) murali    (1000)     1073 2023-04-23 20:40:34.000000 Shreya-Dhumal-finance-charts-0.1/LICENSE
--rw-rw-r--   0 murali    (1000) murali    (1000)      471 2023-04-23 20:43:28.504900 Shreya-Dhumal-finance-charts-0.1/PKG-INFO
--rw-rw-r--   0 murali    (1000) murali    (1000)      614 2023-04-23 19:15:21.000000 Shreya-Dhumal-finance-charts-0.1/README.rst
-drwxrwxr-x   0 murali    (1000) murali    (1000)        0 2023-04-23 20:43:28.500900 Shreya-Dhumal-finance-charts-0.1/Shreya_Dhumal_finance_charts.egg-info/
--rw-rw-r--   0 murali    (1000) murali    (1000)      471 2023-04-23 20:43:28.000000 Shreya-Dhumal-finance-charts-0.1/Shreya_Dhumal_finance_charts.egg-info/PKG-INFO
--rw-rw-r--   0 murali    (1000) murali    (1000)      455 2023-04-23 20:43:28.000000 Shreya-Dhumal-finance-charts-0.1/Shreya_Dhumal_finance_charts.egg-info/SOURCES.txt
--rw-rw-r--   0 murali    (1000) murali    (1000)        1 2023-04-23 20:43:28.000000 Shreya-Dhumal-finance-charts-0.1/Shreya_Dhumal_finance_charts.egg-info/dependency_links.txt
--rw-rw-r--   0 murali    (1000) murali    (1000)       12 2023-04-23 20:43:28.000000 Shreya-Dhumal-finance-charts-0.1/Shreya_Dhumal_finance_charts.egg-info/requires.txt
--rw-rw-r--   0 murali    (1000) murali    (1000)        7 2023-04-23 20:43:28.000000 Shreya-Dhumal-finance-charts-0.1/Shreya_Dhumal_finance_charts.egg-info/top_level.txt
-drwxrwxr-x   0 murali    (1000) murali    (1000)        0 2023-04-23 20:43:28.500900 Shreya-Dhumal-finance-charts-0.1/charts/
--rw-r--r--   0 murali    (1000) murali    (1000)        0 2023-04-21 11:38:31.000000 Shreya-Dhumal-finance-charts-0.1/charts/__init__.py
--rw-r--r--   0 murali    (1000) murali    (1000)       63 2023-04-21 11:38:31.000000 Shreya-Dhumal-finance-charts-0.1/charts/admin.py
--rw-r--r--   0 murali    (1000) murali    (1000)      144 2023-04-21 11:38:31.000000 Shreya-Dhumal-finance-charts-0.1/charts/apps.py
-drwxrwxr-x   0 murali    (1000) murali    (1000)        0 2023-04-23 20:43:28.504900 Shreya-Dhumal-finance-charts-0.1/charts/migrations/
--rw-r--r--   0 murali    (1000) murali    (1000)        0 2023-04-21 11:38:31.000000 Shreya-Dhumal-finance-charts-0.1/charts/migrations/__init__.py
--rw-r--r--   0 murali    (1000) murali    (1000)       57 2023-04-21 11:38:31.000000 Shreya-Dhumal-finance-charts-0.1/charts/models.py
--rw-r--r--   0 murali    (1000) murali    (1000)       60 2023-04-21 11:38:31.000000 Shreya-Dhumal-finance-charts-0.1/charts/tests.py
--rw-rw-r--   0 murali    (1000) murali    (1000)      442 2023-04-22 19:34:39.000000 Shreya-Dhumal-finance-charts-0.1/charts/urls.py
--rw-r--r--   0 murali    (1000) murali    (1000)     6234 2023-04-22 19:36:06.000000 Shreya-Dhumal-finance-charts-0.1/charts/views.py
--rw-rw-r--   0 murali    (1000) murali    (1000)      426 2023-04-23 20:37:40.000000 Shreya-Dhumal-finance-charts-0.1/pyproject.toml
--rw-rw-r--   0 murali    (1000) murali    (1000)     1002 2023-04-23 20:43:28.504900 Shreya-Dhumal-finance-charts-0.1/setup.cfg
--rw-rw-r--   0 murali    (1000) murali    (1000)       37 2023-04-23 19:20:31.000000 Shreya-Dhumal-finance-charts-0.1/setup.py
+drwxrwxr-x   0 murali    (1000) murali    (1000)        0 2023-04-24 13:18:40.244126 Shreya-Dhumal-finance-charts-0.2/
+-rw-rw-r--   0 murali    (1000) murali    (1000)     1073 2023-04-23 20:40:34.000000 Shreya-Dhumal-finance-charts-0.2/LICENSE
+-rw-rw-r--   0 murali    (1000) murali    (1000)      448 2023-04-24 13:18:40.244126 Shreya-Dhumal-finance-charts-0.2/PKG-INFO
+-rw-rw-r--   0 murali    (1000) murali    (1000)      614 2023-04-23 19:15:21.000000 Shreya-Dhumal-finance-charts-0.2/README.rst
+drwxrwxr-x   0 murali    (1000) murali    (1000)        0 2023-04-24 13:18:40.244126 Shreya-Dhumal-finance-charts-0.2/Shreya_Dhumal_finance_charts.egg-info/
+-rw-rw-r--   0 murali    (1000) murali    (1000)      448 2023-04-24 13:18:40.000000 Shreya-Dhumal-finance-charts-0.2/Shreya_Dhumal_finance_charts.egg-info/PKG-INFO
+-rw-rw-r--   0 murali    (1000) murali    (1000)      404 2023-04-24 13:18:40.000000 Shreya-Dhumal-finance-charts-0.2/Shreya_Dhumal_finance_charts.egg-info/SOURCES.txt
+-rw-rw-r--   0 murali    (1000) murali    (1000)        1 2023-04-24 13:18:40.000000 Shreya-Dhumal-finance-charts-0.2/Shreya_Dhumal_finance_charts.egg-info/dependency_links.txt
+-rw-rw-r--   0 murali    (1000) murali    (1000)        7 2023-04-24 13:18:40.000000 Shreya-Dhumal-finance-charts-0.2/Shreya_Dhumal_finance_charts.egg-info/top_level.txt
+drwxrwxr-x   0 murali    (1000) murali    (1000)        0 2023-04-24 13:18:40.244126 Shreya-Dhumal-finance-charts-0.2/charts/
+-rw-r--r--   0 murali    (1000) murali    (1000)        0 2023-04-21 11:38:31.000000 Shreya-Dhumal-finance-charts-0.2/charts/__init__.py
+-rw-r--r--   0 murali    (1000) murali    (1000)       63 2023-04-21 11:38:31.000000 Shreya-Dhumal-finance-charts-0.2/charts/admin.py
+-rw-r--r--   0 murali    (1000) murali    (1000)      144 2023-04-21 11:38:31.000000 Shreya-Dhumal-finance-charts-0.2/charts/apps.py
+drwxrwxr-x   0 murali    (1000) murali    (1000)        0 2023-04-24 13:18:40.244126 Shreya-Dhumal-finance-charts-0.2/charts/migrations/
+-rw-r--r--   0 murali    (1000) murali    (1000)        0 2023-04-21 11:38:31.000000 Shreya-Dhumal-finance-charts-0.2/charts/migrations/__init__.py
+-rw-r--r--   0 murali    (1000) murali    (1000)       57 2023-04-21 11:38:31.000000 Shreya-Dhumal-finance-charts-0.2/charts/models.py
+-rw-r--r--   0 murali    (1000) murali    (1000)       60 2023-04-21 11:38:31.000000 Shreya-Dhumal-finance-charts-0.2/charts/tests.py
+-rw-rw-r--   0 murali    (1000) murali    (1000)      442 2023-04-22 19:34:39.000000 Shreya-Dhumal-finance-charts-0.2/charts/urls.py
+-rw-r--r--   0 murali    (1000) murali    (1000)     6234 2023-04-22 19:36:06.000000 Shreya-Dhumal-finance-charts-0.2/charts/views.py
+-rw-rw-r--   0 murali    (1000) murali    (1000)      426 2023-04-24 13:17:50.000000 Shreya-Dhumal-finance-charts-0.2/pyproject.toml
+-rw-rw-r--   0 murali    (1000) murali    (1000)      720 2023-04-24 13:18:40.244126 Shreya-Dhumal-finance-charts-0.2/setup.cfg
+-rw-rw-r--   0 murali    (1000) murali    (1000)       37 2023-04-23 19:20:31.000000 Shreya-Dhumal-finance-charts-0.2/setup.py
```

### Comparing `Shreya-Dhumal-finance-charts-0.1/LICENSE` & `Shreya-Dhumal-finance-charts-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Shreya-Dhumal-finance-charts-0.1/README.rst` & `Shreya-Dhumal-finance-charts-0.2/README.rst`

 * *Files identical despite different names*

### Comparing `Shreya-Dhumal-finance-charts-0.1/charts/views.py` & `Shreya-Dhumal-finance-charts-0.2/charts/views.py`

 * *Files identical despite different names*

