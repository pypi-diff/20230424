# Comparing `tmp/looper-1.3.2.tar.gz` & `tmp/looper-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "looper-1.3.2.tar", last modified: Wed Feb  9 21:36:41 2022, max compression
+gzip compressed data, was "looper-1.4.0.tar", last modified: Mon Apr 24 20:40:38 2023, max compression
```

## Comparing `looper-1.3.2.tar` & `looper-1.4.0.tar`

### file list

```diff
@@ -1,55 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-09 21:36:41.450755 looper-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1269 2022-02-09 21:36:30.000000 looper-1.3.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-02-09 21:36:30.000000 looper-1.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1198 2022-02-09 21:36:41.450755 looper-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      459 2022-02-09 21:36:30.000000 looper-1.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     5796 2022-02-09 21:36:30.000000 looper-1.3.2/logo_looper.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-09 21:36:41.446755 looper-1.3.2/looper/
--rw-r--r--   0 runner    (1001) docker     (121)    13332 2022-02-09 21:36:30.000000 looper-1.3.2/looper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-02-09 21:36:30.000000 looper-1.3.2/looper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      659 2022-02-09 21:36:30.000000 looper-1.3.2/looper/_devtools.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-02-09 21:36:30.000000 looper-1.3.2/looper/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    29805 2022-02-09 21:36:30.000000 looper-1.3.2/looper/conductor.py
--rw-r--r--   0 runner    (1001) docker     (121)     5215 2022-02-09 21:36:30.000000 looper-1.3.2/looper/const.py
--rw-r--r--   0 runner    (1001) docker     (121)     2801 2022-02-09 21:36:30.000000 looper-1.3.2/looper/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    42010 2022-02-09 21:36:30.000000 looper-1.3.2/looper/html_reports.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-09 21:36:41.450755 looper-1.3.2/looper/jinja_templates/
--rw-r--r--   0 runner    (1001) docker     (121)      206 2022-02-09 21:36:30.000000 looper-1.3.2/looper/jinja_templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (121)     2494 2022-02-09 21:36:30.000000 looper-1.3.2/looper/jinja_templates/footer_index.html
--rw-r--r--   0 runner    (1001) docker     (121)     3168 2022-02-09 21:36:30.000000 looper-1.3.2/looper/jinja_templates/head.html
--rw-r--r--   0 runner    (1001) docker     (121)     8960 2022-02-09 21:36:30.000000 looper-1.3.2/looper/jinja_templates/index.html
--rw-r--r--   0 runner    (1001) docker     (121)     7842 2022-02-09 21:36:30.000000 looper-1.3.2/looper/jinja_templates/logo.html
--rw-r--r--   0 runner    (1001) docker     (121)      850 2022-02-09 21:36:30.000000 looper-1.3.2/looper/jinja_templates/navbar.html
--rw-r--r--   0 runner    (1001) docker     (121)     3423 2022-02-09 21:36:30.000000 looper-1.3.2/looper/jinja_templates/navbar_links.html
--rw-r--r--   0 runner    (1001) docker     (121)      702 2022-02-09 21:36:30.000000 looper-1.3.2/looper/jinja_templates/navbar_list_parent.html
--rw-r--r--   0 runner    (1001) docker     (121)     1349 2022-02-09 21:36:30.000000 looper-1.3.2/looper/jinja_templates/object.html
--rw-r--r--   0 runner    (1001) docker     (121)     1404 2022-02-09 21:36:30.000000 looper-1.3.2/looper/jinja_templates/project_object.html
--rw-r--r--   0 runner    (1001) docker     (121)     4602 2022-02-09 21:36:30.000000 looper-1.3.2/looper/jinja_templates/sample.html
--rw-r--r--   0 runner    (1001) docker     (121)      398 2022-02-09 21:36:30.000000 looper-1.3.2/looper/jinja_templates/status.html
--rw-r--r--   0 runner    (1001) docker     (121)     3270 2022-02-09 21:36:30.000000 looper-1.3.2/looper/jinja_templates/status_table.html
--rw-r--r--   0 runner    (1001) docker     (121)     2395 2022-02-09 21:36:30.000000 looper-1.3.2/looper/jinja_templates/status_table_no_links.html
--rwxr-xr-x   0 runner    (1001) docker     (121)    30303 2022-02-09 21:36:30.000000 looper-1.3.2/looper/looper.py
--rw-r--r--   0 runner    (1001) docker     (121)     2139 2022-02-09 21:36:30.000000 looper-1.3.2/looper/looper_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     2217 2022-02-09 21:36:30.000000 looper-1.3.2/looper/parser_types.py
--rw-r--r--   0 runner    (1001) docker     (121)    14295 2022-02-09 21:36:30.000000 looper-1.3.2/looper/pipeline_interface.py
--rw-r--r--   0 runner    (1001) docker     (121)     5134 2022-02-09 21:36:30.000000 looper-1.3.2/looper/processed_project.py
--rw-r--r--   0 runner    (1001) docker     (121)    23394 2022-02-09 21:36:30.000000 looper-1.3.2/looper/project.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-09 21:36:41.450755 looper-1.3.2/looper/schemas/
--rw-r--r--   0 runner    (1001) docker     (121)     1580 2022-02-09 21:36:30.000000 looper-1.3.2/looper/schemas/pipeline_interface_schema_generic.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1566 2022-02-09 21:36:30.000000 looper-1.3.2/looper/schemas/pipeline_interface_schema_project.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1563 2022-02-09 21:36:30.000000 looper-1.3.2/looper/schemas/pipeline_interface_schema_sample.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    13268 2022-02-09 21:36:30.000000 looper-1.3.2/looper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-09 21:36:41.446755 looper-1.3.2/looper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1198 2022-02-09 21:36:41.000000 looper-1.3.2/looper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1398 2022-02-09 21:36:41.000000 looper-1.3.2/looper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-09 21:36:41.000000 looper-1.3.2/looper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-02-09 21:36:41.000000 looper-1.3.2/looper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-02-09 21:36:41.000000 looper-1.3.2/looper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-02-09 21:36:41.000000 looper-1.3.2/looper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-09 21:36:41.450755 looper-1.3.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-02-09 21:36:30.000000 looper-1.3.2/requirements/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-09 21:36:30.000000 looper-1.3.2/requirements/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-02-09 21:36:30.000000 looper-1.3.2/requirements/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-02-09 21:36:30.000000 looper-1.3.2/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-02-09 21:36:41.450755 looper-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2564 2022-02-09 21:36:30.000000 looper-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:40:38.388970 looper-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-24 20:40:25.000000 looper-1.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-24 20:40:25.000000 looper-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-24 20:40:38.388970 looper-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-24 20:40:25.000000 looper-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-24 20:40:25.000000 looper-1.4.0/logo_looper.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:40:38.384969 looper-1.4.0/looper/
+-rw-r--r--   0 runner    (1001) docker     (123)    15711 2023-04-24 20:40:25.000000 looper-1.4.0/looper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-24 20:40:25.000000 looper-1.4.0/looper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-24 20:40:25.000000 looper-1.4.0/looper/_devtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-24 20:40:25.000000 looper-1.4.0/looper/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35293 2023-04-24 20:40:25.000000 looper-1.4.0/looper/conductor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-04-24 20:40:25.000000 looper-1.4.0/looper/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-24 20:40:25.000000 looper-1.4.0/looper/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43820 2023-04-24 20:40:25.000000 looper-1.4.0/looper/html_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35130 2023-04-24 20:40:25.000000 looper-1.4.0/looper/html_reports_pipestat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-04-24 20:40:25.000000 looper-1.4.0/looper/html_reports_project_pipestat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:40:38.388970 looper-1.4.0/looper/jinja_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates/footer_index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates/head.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates/logo.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates/navbar.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates/navbar_links.html
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates/navbar_list_parent.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates/object.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates/project_object.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates/sample.html
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates/status.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates/status_table.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates/status_table_no_links.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:40:38.388970 looper-1.4.0/looper/jinja_templates_old/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates_old/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates_old/footer_index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates_old/head.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates_old/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates_old/logo.html
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates_old/navbar.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates_old/navbar_links.html
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates_old/navbar_list_parent.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates_old/object.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates_old/project_object.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates_old/sample.html
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates_old/status.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates_old/status_table.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-24 20:40:25.000000 looper-1.4.0/looper/jinja_templates_old/status_table_no_links.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45084 2023-04-24 20:40:25.000000 looper-1.4.0/looper/looper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-24 20:40:25.000000 looper-1.4.0/looper/parser_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14876 2023-04-24 20:40:25.000000 looper-1.4.0/looper/pipeline_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9867 2023-04-24 20:40:25.000000 looper-1.4.0/looper/processed_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30954 2023-04-24 20:40:25.000000 looper-1.4.0/looper/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:40:38.388970 looper-1.4.0/looper/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-24 20:40:25.000000 looper-1.4.0/looper/schemas/pipeline_interface_schema_generic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-24 20:40:25.000000 looper-1.4.0/looper/schemas/pipeline_interface_schema_project.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-24 20:40:25.000000 looper-1.4.0/looper/schemas/pipeline_interface_schema_sample.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20474 2023-04-24 20:40:25.000000 looper-1.4.0/looper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:40:38.384969 looper-1.4.0/looper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-24 20:40:38.000000 looper-1.4.0/looper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-24 20:40:38.000000 looper-1.4.0/looper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 20:40:38.000000 looper-1.4.0/looper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-24 20:40:38.000000 looper-1.4.0/looper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-24 20:40:38.000000 looper-1.4.0/looper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 20:40:38.000000 looper-1.4.0/looper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:40:38.388970 looper-1.4.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-24 20:40:25.000000 looper-1.4.0/requirements/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-24 20:40:25.000000 looper-1.4.0/requirements/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-24 20:40:25.000000 looper-1.4.0/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-24 20:40:38.388970 looper-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-04-24 20:40:25.000000 looper-1.4.0/setup.py
```

### Comparing `looper-1.3.2/LICENSE.txt` & `looper-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `looper-1.3.2/PKG-INFO` & `looper-1.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: looper
-Version: 1.3.2
+Version: 1.4.0
 Summary: A pipeline submission engine that parses sample inputs and submits pipelines for each sample.
 Home-page: https://github.com/pepkit/looper
 Author: Nathan Sheffield, Vince Reuter, Michal Stolarczyk, Johanna Klughammer, Andre Rendeiro
 License: BSD2
 Keywords: bioinformatics,sequencing,ngs
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # <img src="docs/img/looper_logo.svg" alt="looper logo" height="70">
- 
+
 ![Run pytests](https://github.com/pepkit/looper/workflows/Run%20pytests/badge.svg)
 [![PEP compatible](http://pepkit.github.io/img/PEP-compatible-green.svg)](http://pepkit.github.io)
-
-`Looper` is a pipeline submission engine. The typical use case is to run a bioinformatics pipeline across many different input samples. Instructions are in the [documentation](http://looper.databio.org/).
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 
+`Looper` is a pipeline submission engine. The typical use case is to run a bioinformatics pipeline across many different input samples. Instructions are in the [documentation](http://looper.databio.org/).
```

### Comparing `looper-1.3.2/logo_looper.svg` & `looper-1.4.0/logo_looper.svg`

 * *Files identical despite different names*

### Comparing `looper-1.3.2/looper/_devtools.py` & `looper-1.4.0/looper/_devtools.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """ Utility functions for internal, developmental use """
 
 import copy
+
 from logmuse import init_logger
 
 __author__ = "Vince Reuter"
 __email__ = "vreuter@virginia.edu"
 
 __all__ = ["est_log"]
 
@@ -14,12 +15,15 @@
     Establish logging, e.g. for an interactive session.
 
     :param dict kwargs: keyword arguments for logger setup.
     :return logging.Logger: looper logger
     """
     kwds = copy.copy(kwargs)
     if "name" in kwds:
-        print("Ignoring {} and setting fixed values for logging names".
-              format(kwds["name"]))
+        print(
+            "Ignoring {} and setting fixed values for logging names".format(
+                kwds["name"]
+            )
+        )
         del kwds["name"]
     init_logger(name="peppy", **kwds)
     return init_logger(name="looper", **kwds)
```

### Comparing `looper-1.3.2/looper/conductor.py` & `looper-1.4.0/looper/conductor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,86 @@
 """ Pipeline job submission orchestration """
 
+import importlib
 import logging
 import os
 import subprocess
 import time
-import importlib
-
-from jinja2.exceptions import UndefinedError
-from subprocess import check_output, CalledProcessError
+from copy import copy, deepcopy
 from json import loads
-from yaml import dump
+from subprocess import CalledProcessError, check_output
+from typing import *
 
-from attmap import AttMap
 from eido import read_schema, validate_inputs
-from eido.const import MISSING_KEY, INPUT_FILE_SIZE_KEY
+from eido.const import INPUT_FILE_SIZE_KEY, MISSING_KEY
+from jinja2.exceptions import UndefinedError
+
+from peppy.const import CONFIG_KEY, SAMPLE_NAME_ATTR, SAMPLE_YAML_EXT
+from peppy.exceptions import RemoteYAMLError
+from pipestat import PipestatError
 from ubiquerg import expandpath
-from peppy.const import CONFIG_KEY, SAMPLE_YAML_EXT, SAMPLE_NAME_ATTR
+from yaml import dump
+from yacman import YAMLConfigManager
 
-from .processed_project import populate_sample_paths
 from .const import *
 from .exceptions import JobSubmissionException
+from .processed_project import populate_sample_paths
 from .utils import fetch_sample_flags, jinja_render_template_strictly
 
 _LOGGER = logging.getLogger(__name__)
 
 
-def _get_yaml_path(namespaces, template_key, default_name_appendix="",
-                   filename=None):
+def _get_yaml_path(namespaces, template_key, default_name_appendix="", filename=None):
     """
-    Get a path to the a YAML file.
+    Get a path to a YAML file for the sample.
 
     :param dict[dict]] namespaces: namespaces mapping
     :param str template_key: the name of the key in 'var_templates' piface
         section that points to a template to render to get the
         user-provided target YAML path
     :param str default_name_appendix: a string to append to insert in target
         YAML file name: '{sample.sample_name}<>.yaml'
     :param str filename: A filename without folders. If not provided, a
         default name of sample_name.yaml will be used.
     :return str: sample YAML file path
     """
-    if VAR_TEMPL_KEY in namespaces["pipeline"] and \
-            template_key in namespaces["pipeline"][VAR_TEMPL_KEY]:
-        path = expandpath(jinja_render_template_strictly(
-            namespaces["pipeline"][template_key], namespaces))
+    if (
+        VAR_TEMPL_KEY in namespaces["pipeline"]
+        and template_key in namespaces["pipeline"][VAR_TEMPL_KEY]
+    ):
+        _LOGGER.debug(f"Sample namespace: {namespaces['sample']}")
+        x = jinja_render_template_strictly("{sample.sample_name}", namespaces)
+        _LOGGER.debug(f"x: {x}")
+        cpy = namespaces["pipeline"][VAR_TEMPL_KEY][template_key]
+        _LOGGER.debug(f"cpy: {cpy}")
+        path = expandpath(jinja_render_template_strictly(cpy, namespaces))
+        _LOGGER.debug(f"path: {path}")
+
         if not path.endswith(SAMPLE_YAML_EXT) and not filename:
             raise ValueError(
                 f"{template_key} is not a valid target YAML file path. "
-                f"It needs to end with: {' or '.join(SAMPLE_YAML_EXT)}")
+                f"It needs to end with: {' or '.join(SAMPLE_YAML_EXT)}"
+            )
         final_path = os.path.join(path, filename) if filename else path
         if not os.path.exists(os.path.dirname(final_path)):
             os.makedirs(os.path.dirname(final_path), exist_ok=True)
     else:
         # default YAML location
-        f = filename or f"{namespaces['sample'][SAMPLE_NAME_ATTR]}" \
-                        f"{default_name_appendix}" \
-                        f"{SAMPLE_YAML_EXT[0]}"
+        f = (
+            filename
+            or f"{namespaces['sample'][SAMPLE_NAME_ATTR]}"
+            f"{default_name_appendix}"
+            f"{SAMPLE_YAML_EXT[0]}"
+        )
         default = os.path.join(namespaces["looper"][OUTDIR_KEY], "submission")
         final_path = os.path.join(default, f)
         if not os.path.exists(default):
             os.makedirs(default, exist_ok=True)
+
+    _LOGGER.debug(f"Writing sample yaml: {final_path}")
     return final_path
 
 
 def write_sample_yaml(namespaces):
     """
     Plugin: saves sample representation to YAML.
 
@@ -72,16 +89,18 @@
     absolute path to the file where sample YAML representation is to be
     stored.
 
     :param dict namespaces: variable namespaces dict
     :return dict: sample namespace dict
     """
     sample = namespaces["sample"]
-    sample.to_yaml(_get_yaml_path(namespaces, SAMPLE_YAML_PATH_KEY, "_sample"),
-                   add_prj_ref=False)
+    sample["sample_yaml_path"] = _get_yaml_path(
+        namespaces, SAMPLE_YAML_PATH_KEY, "_sample"
+    )
+    sample.to_yaml(sample["sample_yaml_path"], add_prj_ref=False)
     return {"sample": sample}
 
 
 def write_sample_yaml_prj(namespaces):
     """
     Plugin: saves sample representation with project reference to YAML.
 
@@ -90,22 +109,61 @@
     absolute path to the file where sample YAML representation is to be
     stored.
 
     :param dict namespaces: variable namespaces dict
     :return dict: sample namespace dict
     """
     sample = namespaces["sample"]
-    sample.to_yaml(_get_yaml_path(
-        namespaces, SAMPLE_YAML_PRJ_PATH_KEY, "_sample_prj"), add_prj_ref=True)
+    sample.to_yaml(
+        _get_yaml_path(namespaces, SAMPLE_YAML_PRJ_PATH_KEY, "_sample_prj"),
+        add_prj_ref=True,
+    )
     return {"sample": sample}
 
 
+def write_custom_template(namespaces):
+    """
+    Plugin: Populates a user-provided jinja template
+
+    Parameterize by providing pipeline.var_templates.custom_template
+    """
+
+    def load_template(pipeline):
+        with open(namespaces["pipeline"]["var_templates"]["custom_template"], "r") as f:
+            x = f.read()
+        t = jinja2.Template(x)
+        return t
+
+    err_msg = (
+        "Custom template plugin requires a template in var_templates.custom_template"
+    )
+    if "var_templates" not in namespaces["pipeline"].keys():
+        _LOGGER.error(err_msg)
+        return None
+
+    if "custom_template" not in namespaces["pipeline"]["var_templates"].keys():
+        _LOGGER.error(err_msg)
+        return None
+
+    import jinja2
+
+    tpl = load_template(namespaces["pipeline"])
+    content = tpl.render(namespaces)
+    pth = _get_yaml_path(namespaces, "custom_template_output", "_config")
+    namespaces["sample"]["custom_template_output"] = pth
+    with open(pth, "wb") as fh:
+        # print(content)
+        fh.write(content.encode())
+
+    return {"sample": namespaces["sample"]}
+
+
 def write_sample_yaml_cwl(namespaces):
     """
-    Produce a cwl-compatible yaml representation of the sample
+    Plugin: Produce a cwl-compatible yaml representation of the sample
 
     Also adds the 'cwl_yaml' attribute to sample objects, which points
     to the file produced.
 
     This plugin can be parametrized by providing the path value/template in
     'pipeline.var_templates.sample_cwl_yaml_path'. This needs to be a complete and
     absolute path to the file where sample YAML representation is to be
@@ -113,27 +171,30 @@
 
     :param dict namespaces: variable namespaces dict
     :return dict: updated variable namespaces dict
     """
     from eido import read_schema
     from ubiquerg import is_url
 
-    def _get_schema_source(schema_source, piface_dir=namespaces["looper"]["piface_dir"]):
+    def _get_schema_source(
+        schema_source, piface_dir=namespaces["looper"]["piface_dir"]
+    ):
         # Stolen from piface object; should be a better way to do this...
         if is_url(schema_source):
             return schema_source
         elif not os.path.isabs(schema_source):
             schema_source = os.path.join(piface_dir, schema_source)
         return schema_source
 
     # To be compatible as a CWL job input, we need to handle the
     # File and Directory object types directly.
     sample = namespaces["sample"]
     sample.sample_yaml_cwl = _get_yaml_path(
-        namespaces, SAMPLE_CWL_YAML_PATH_KEY, "_sample_cwl")
+        namespaces, SAMPLE_CWL_YAML_PATH_KEY, "_sample_cwl"
+    )
 
     if "input_schema" in namespaces["pipeline"]:
         schema_path = _get_schema_source(namespaces["pipeline"]["input_schema"])
         file_list = []
         for ischema in read_schema(schema_path):
             if "files" in ischema["properties"]["samples"]["items"]:
                 file_list.extend(ischema["properties"]["samples"]["items"]["files"])
@@ -141,34 +202,37 @@
         for file_attr in file_list:
             _LOGGER.debug("CWL-ing file attribute: {}".format(file_attr))
             file_attr_value = sample[file_attr]
             # file paths are assumed relative to the sample table;
             # but CWL assumes they are relative to the yaml output file,
             # so we convert here.
             file_attr_rel = os.path.relpath(
-                file_attr_value, os.path.dirname(sample.sample_yaml_cwl))
-            sample[file_attr] = {"class": "File",
-                                 "path":  file_attr_rel}
+                file_attr_value, os.path.dirname(sample.sample_yaml_cwl)
+            )
+            sample[file_attr] = {"class": "File", "path": file_attr_rel}
 
         directory_list = []
         for ischema in read_schema(schema_path):
             if "directories" in ischema["properties"]["samples"]["items"]:
-                directory_list.extend(ischema["properties"]["samples"]["items"]["files"])
+                directory_list.extend(
+                    ischema["properties"]["samples"]["items"]["directories"]
+                )
 
         for dir_attr in directory_list:
             _LOGGER.debug("CWL-ing directory attribute: {}".format(dir_attr))
             dir_attr_value = sample[dir_attr]
             # file paths are assumed relative to the sample table;
             # but CWL assumes they are relative to the yaml output file,
             # so we convert here.
-            sample[dir_attr] = {"class": "Directory",
-                                "path":  dir_attr_value}
+            sample[dir_attr] = {"class": "Directory", "location": dir_attr_value}
     else:
-        _LOGGER.warning("No 'input_schema' defined, producing a regular "
-                        "sample YAML representation")
+        _LOGGER.warning(
+            "No 'input_schema' defined, producing a regular "
+            "sample YAML representation"
+        )
     _LOGGER.info("Writing sample yaml to {}".format(sample.sample_yaml_cwl))
     sample.to_yaml(sample.sample_yaml_cwl)
     return {"sample": sample}
 
 
 def write_submission_yaml(namespaces):
     """
@@ -177,15 +241,15 @@
     :param dict namespaces: variable namespaces dict
     :return dict: sample namespace dict
     """
     path = _get_yaml_path(namespaces, SAMPLE_CWL_YAML_PATH_KEY, "_submission")
     my_namespaces = {}
     for namespace, values in namespaces.items():
         my_namespaces.update({str(namespace): values.to_dict()})
-    with open(path, 'w') as yamlfile:
+    with open(path, "w") as yamlfile:
         dump(my_namespaces, yamlfile)
     return my_namespaces
 
 
 class SubmissionConductor(object):
     """
     Collects and then submits pipeline jobs.
@@ -193,18 +257,29 @@
     This class holds a 'pool' of commands to submit as a single cluster job.
     Eager to submit a job, each instance's collection of commands expands until
     it reaches the 'pool' has been filled, and it's therefore time to submit the
     job. The pool fills as soon as a fill criteria has been reached, which can
     be either total input file size or the number of individual commands.
 
     """
-    def __init__(self, pipeline_interface, prj, delay=0, extra_args=None,
-                 extra_args_override=None, ignore_flags=False,
-                 compute_variables=None, max_cmds=None, max_size=None,
-                 automatic=True, collate=False):
+
+    def __init__(
+        self,
+        pipeline_interface,
+        prj,
+        delay=0,
+        extra_args=None,
+        extra_args_override=None,
+        ignore_flags=False,
+        compute_variables=None,
+        max_cmds=None,
+        max_size=None,
+        automatic=True,
+        collate=False,
+    ):
         """
         Create a job submission manager.
 
         The most critical inputs are the pipeline interface and the pipeline
         key, which together determine which provide critical pipeline
         information like resource allocation packages and which pipeline will
         be overseen by this instance, respectively.
@@ -256,26 +331,30 @@
         self._num_good_job_submissions = 0
         self._num_total_job_submissions = 0
         self._num_cmds_submitted = 0
         self._curr_size = 0
         self._failed_sample_names = []
 
         if self.extra_pipe_args:
-            _LOGGER.debug("String appended to every pipeline command: "
-                          "{}".format(self.extra_pipe_args))
+            _LOGGER.debug(
+                "String appended to every pipeline command: "
+                "{}".format(self.extra_pipe_args)
+            )
 
         if not self.collate:
             self.automatic = automatic
             if max_cmds is None and max_size is None:
                 self.max_cmds = 1
-            elif (max_cmds is not None and max_cmds < 1) or \
-                    (max_size is not None and max_size < 0):
+            elif (max_cmds is not None and max_cmds < 1) or (
+                max_size is not None and max_size < 0
+            ):
                 raise ValueError(
                     "If specified, max per-job command count must positive, "
-                    "and max per-job total file size must be nonnegative")
+                    "and max per-job total file size must be nonnegative"
+                )
             else:
                 self.max_cmds = max_cmds
             self.max_size = max_size or float("inf")
 
             self._pool = []
             self._reset_curr_skips()
             self._skipped_sample_pools = []
@@ -284,156 +363,194 @@
     def failed_samples(self):
         return self._failed_sample_names
 
     @property
     def num_cmd_submissions(self):
         """
         Return the number of commands that this conductor has submitted.
-        
+
         :return int: Number of commands submitted so far.
         """
         return self._num_cmds_submitted
 
     @property
     def num_job_submissions(self):
         """
         Return the number of jobs that this conductor has submitted.
-        
+
         :return int: Number of jobs submitted so far.
         """
         return self._num_good_job_submissions
 
+    def is_project_submittable(self, force=False):
+        """
+        Check whether the current project has been already submitted
+
+        :param bool frorce: whether to force the project submission (ignore status/flags)
+        """
+        if self.prj.pipestat_configured_project:
+            psm = self.prj.get_pipestat_managers(project_level=True)[self.pl_name]
+            status = psm.get_status()
+            if not force and status is not None:
+                _LOGGER.info(f"> Skipping project. Determined status: {status}")
+                return False
+        return True
+
     def add_sample(self, sample, rerun=False):
         """
         Add a sample for submission to this conductor.
 
         :param peppy.Sample sample: sample to be included with this conductor's
             currently growing collection of command submissions
         :param bool rerun: whether the given sample is being rerun rather than
             run for the first time
         :return bool: Indication of whether the given sample was added to
             the current 'pool.'
         :raise TypeError: If sample subtype is provided but does not extend
             the base Sample class, raise a TypeError.
         """
-        _LOGGER.debug("Adding {} to conductor for {} to {}run".format(
-            sample.sample_name, self.pl_name, "re" if rerun else ""))
-        flag_files = fetch_sample_flags(self.prj, sample, self.pl_name)
+        _LOGGER.debug(
+            "Adding {} to conductor for {} to {}run".format(
+                sample.sample_name, self.pl_name, "re" if rerun else ""
+            )
+        )
+        if self.prj.pipestat_configured:
+            psms = self.prj.get_pipestat_managers(sample_name=sample.sample_name)
+            sample_statuses = psms[self.pl_name].get_status()
+            sample_statuses = [sample_statuses] if sample_statuses else []
+        else:
+            sample_statuses = fetch_sample_flags(self.prj, sample, self.pl_name)
         use_this_sample = not rerun
 
-        if flag_files or rerun:
+        if sample_statuses or rerun:
             if not self.ignore_flags:
                 use_this_sample = False
             # But rescue the sample in case rerun/failed passes
-            failed_flag = any("failed" in x for x in flag_files)
+            failed_flag = any("failed" in x for x in sample_statuses)
             if rerun:
                 if failed_flag:
                     _LOGGER.info("> Re-running failed sample")
                     use_this_sample = True
                 else:
                     use_this_sample = False
             if not use_this_sample:
-                msg = "> Skipping sample because flag found"
-                if flag_files:
-                    msg += ". Flags found: {}".format(flag_files)
+                msg = "> Skipping sample"
+                if sample_statuses:
+                    msg += f". Determined status: {', '.join(sample_statuses)}"
                 _LOGGER.info(msg)
 
-        if self.prj.toggle_key in sample \
-                and int(sample[self.prj.toggle_key]) == 0:
+        if self.prj.toggle_key in sample and int(sample[self.prj.toggle_key]) == 0:
             _LOGGER.warning(
-                "> Skipping sample ({}: {})".
-                    format(self.prj.toggle_key, sample[self.prj.toggle_key])
+                "> Skipping sample ({}: {})".format(
+                    self.prj.toggle_key, sample[self.prj.toggle_key]
+                )
             )
             use_this_sample = False
 
         skip_reasons = []
         validation = {}
         validation.setdefault(INPUT_FILE_SIZE_KEY, 0)
         # Check for any missing requirements before submitting.
         _LOGGER.debug("Determining missing requirements")
         schema_source = self.pl_iface.get_pipeline_schemas()
         if schema_source and self.prj.file_checks:
-            validation = validate_inputs(sample, read_schema(schema_source))
-            if validation[MISSING_KEY]:
-                missing_reqs_msg = f"Missing files: {validation[MISSING_KEY]}"
-                _LOGGER.warning(NOT_SUB_MSG.format(missing_reqs_msg))
-                use_this_sample and skip_reasons.append("Missing files")
+            try:
+                validation = validate_inputs(sample, read_schema(schema_source))
+            except RemoteYAMLError:
+                _LOGGER.warn(
+                    "Could not read remote schema. Skipping inputs validation."
+                )
+            else:
+                if validation[MISSING_KEY]:
+                    missing_reqs_msg = (
+                        f"Missing files: {', '.join(validation[MISSING_KEY])}"
+                    )
+                    _LOGGER.warning(NOT_SUB_MSG.format(missing_reqs_msg))
+                    use_this_sample and skip_reasons.append("Missing files")
 
         if _use_sample(use_this_sample, skip_reasons):
             self._pool.append(sample)
             self._curr_size += float(validation[INPUT_FILE_SIZE_KEY])
             if self.automatic and self._is_full(self._pool, self._curr_size):
                 self.submit()
         else:
             self._curr_skip_size += float(validation[INPUT_FILE_SIZE_KEY])
             self._curr_skip_pool.append(sample)
             if self._is_full(self._curr_skip_pool, self._curr_skip_size):
-                self._skipped_sample_pools.append((self._curr_skip_pool,
-                                                   self._curr_skip_size))
+                self._skipped_sample_pools.append(
+                    (self._curr_skip_pool, self._curr_skip_size)
+                )
                 self._reset_curr_skips()
 
         return skip_reasons
 
     def submit(self, force=False):
         """
         Submit one or more commands as a job.
-        
-        This call will submit the commands corresponding to the current pool 
-        of samples if and only if the argument to 'force' evaluates to a 
+
+        This call will submit the commands corresponding to the current pool
+        of samples if and only if the argument to 'force' evaluates to a
         true value, or the pool of samples is full.
-        
+
         :param bool force: Whether submission should be done/simulated even
             if this conductor's pool isn't full.
         :return bool: Whether a job was submitted (or would've been if
             not for dry run)
         """
         submitted = False
         if not self._pool:
             _LOGGER.debug("No submission (no pooled samples): %s", self.pl_name)
             # submitted = False
         elif self.collate or force or self._is_full(self._pool, self._curr_size):
             if not self.collate:
                 for s in self._pool:
-                    schemas = self.prj.get_schemas(self.prj.get_sample_piface(
-                        s[SAMPLE_NAME_ATTR]), OUTPUT_SCHEMA_KEY)
+                    schemas = self.prj.get_schemas(
+                        self.prj.get_sample_piface(s[self.prj.sample_table_index]),
+                        OUTPUT_SCHEMA_KEY,
+                    )
 
                     for schema in schemas:
-                        populate_sample_paths(s, read_schema(schema))
+                        populate_sample_paths(s, read_schema(schema)[0])
 
             script = self.write_script(self._pool, self._curr_size)
             # Determine whether to actually do the submission.
-            _LOGGER.info("Job script (n={0}; {1:.2f}Gb): {2}".
-                         format(len(self._pool), self._curr_size, script))
+            _LOGGER.info(
+                "Job script (n={0}; {1:.2f}Gb): {2}".format(
+                    len(self._pool), self._curr_size, script
+                )
+            )
             if self.dry_run:
                 _LOGGER.info("Dry run, not submitted")
             elif self._rendered_ok:
                 sub_cmd = self.prj.dcc.compute.submission_command
                 submission_command = "{} {}".format(sub_cmd, script)
                 # Capture submission command return value so that we can
                 # intercept and report basic submission failures; #167
                 try:
                     subprocess.check_call(submission_command, shell=True)
                 except subprocess.CalledProcessError:
-                    fails = "" if self.collate \
-                        else [s.sample_name for s in self._samples]
+                    fails = (
+                        "" if self.collate else [s.sample_name for s in self._samples]
+                    )
                     self._failed_sample_names.extend(fails)
                     self._reset_pool()
                     raise JobSubmissionException(sub_cmd, script)
                 time.sleep(self.delay)
 
             # Update the job and command submission tallies.
             _LOGGER.debug("SUBMITTED")
             if self._rendered_ok:
                 submitted = True
                 self._num_cmds_submitted += len(self._pool)
             self._reset_pool()
 
         else:
-            _LOGGER.debug("No submission (pool is not full and submission "
-                          "was not forced): %s", self.pl_name)
+            _LOGGER.debug(
+                f"No submission (pool is not full and submission was not forced): {self.pl_name}"
+            )
             # submitted = False
 
         return submitted
 
     def _is_full(self, pool, size):
         """
         Determine whether it's time to submit a job for the pool of commands.
@@ -454,155 +571,224 @@
 
         :return Iterable[str]: collection of samples currently in the active
             pool for this submission conductor
         """
         return [s for s in self._pool]
 
     def _sample_lump_name(self, pool):
-        """ Determine how to refer to the 'sample' for this submission. """
+        """Determine how to refer to the 'sample' for this submission."""
         if self.collate:
-            return "collate"
+            return self.prj.name
         if 1 == self.max_cmds:
-            assert 1 == len(pool), \
-                "If there's a single-command limit on job submission, jobname" \
-                " must be determined with exactly one sample in the pool," \
+            assert 1 == len(pool), (
+                "If there's a single-command limit on job submission, jobname"
+                " must be determined with exactly one sample in the pool,"
                 " but there is/are {}.".format(len(pool))
+            )
             sample = pool[0]
             return sample.sample_name
         else:
             # Note the order in which the increment of submission count and
             # the call to this function can influence naming. Make the jobname
             # generation call (this method) before incrementing the
             # submission counter, but add 1 to the index so that we get a
             # name concordant with 1-based, not 0-based indexing.
             return "lump{}".format(self._num_total_job_submissions + 1)
 
     def _jobname(self, pool):
-        """ Create the name for a job submission. """
-        return "{}_{}".format(self.pl_iface.pipeline_name,
-                              self._sample_lump_name(pool))
+        """Create the name for a job submission."""
+        return "{}_{}".format(self.pl_iface.pipeline_name, self._sample_lump_name(pool))
 
-    def _set_looper_namespace(self, pool, size):
+    def _build_looper_namespace(self, pool, size):
         """
-        Compile a dictionary of looper/submission related settings for use in
+        Compile a mapping of looper/submission related settings for use in
         the command templates and in submission script creation
-        in divvy (via adapters). Accessible via: {looper.attrname}
+        in divvy (via adapters).
 
         :param Iterable[peppy.Sample] pool: collection of sample instances
         :param float size: cumulative size of the given pool
-        :return dict: looper/submission related settings
+        :return yacman.YAMLConfigManager: looper/submission related settings
         """
-        settings = AttMap()
-        settings.pep_config = self.prj.config_file
-        settings.results_subdir = self.prj.results_folder
-        settings.submission_subdir = self.prj.submission_folder
-        settings.output_dir = self.prj.output_dir
-        settings.sample_output_folder = \
-            os.path.join(self.prj.results_folder, self._sample_lump_name(pool))
-        settings.job_name = self._jobname(pool)
-        settings.total_input_size = size
-        settings.log_file = \
-            os.path.join(self.prj.submission_folder, settings.job_name) + ".log"
-        settings.piface_dir = os.path.dirname(self.pl_iface.pipe_iface_file)
+        settings = YAMLConfigManager()
+        settings["pep_config"] = self.prj.config_file
+        settings[RESULTS_SUBDIR_KEY] = self.prj.results_folder
+        settings[SUBMISSION_SUBDIR_KEY] = self.prj.submission_folder
+        settings[OUTDIR_KEY] = self.prj.output_dir
+        # TODO: explore pulling additional constants from peppy and/or divvy.
+        settings["sample_output_folder"] = os.path.join(
+            self.prj.results_folder, self._sample_lump_name(pool)
+        )
+        settings[JOB_NAME_KEY] = self._jobname(pool)
+        settings["total_input_size"] = size
+        settings["log_file"] = (
+            os.path.join(self.prj.submission_folder, settings[JOB_NAME_KEY]) + ".log"
+        )
+        settings["piface_dir"] = os.path.dirname(self.pl_iface.pipe_iface_file)
         if hasattr(self.prj, "pipeline_config"):
             # Make sure it's a file (it could be provided as null.)
             pl_config_file = self.prj.pipeline_config
             if pl_config_file:
                 if not os.path.isfile(pl_config_file):
-                    _LOGGER.error("Pipeline config file specified "
-                                  "but not found: %s", pl_config_file)
+                    _LOGGER.error(
+                        "Pipeline config file specified " "but not found: %s",
+                        pl_config_file,
+                    )
                     raise IOError(pl_config_file)
                 _LOGGER.info("Found config file: %s", pl_config_file)
                 # Append arg for config file if found
-                settings.pipeline_config = pl_config_file
+                settings["pipeline_config"] = pl_config_file
         return settings
 
+    def _set_pipestat_namespace(
+        self, sample_name: Optional[str] = None
+    ) -> YAMLConfigManager:
+        """
+        Compile a mapping of pipestat-related settings for use in
+        the command templates. Accessible via: {pipestat.attrname}
+
+        :param str sample_name: name of the sample to get the pipestat
+            namespace for. If not provided the pipestat namespace will
+            be determined based on the Project
+        :return yacman.YAMLConfigManager: pipestat namespace
+        """
+        try:
+            psms = (
+                self.prj.get_pipestat_managers(sample_name)
+                if sample_name
+                else self.prj.get_pipestat_managers(project_level=True)
+            )
+            psm = psms[self.pl_iface.pipeline_name]
+        except (PipestatError, AttributeError) as e:
+            # pipestat section faulty or not found in project.looper or sample
+            # or project is missing required pipestat attributes
+            _LOGGER.debug(
+                f"Could not determine pipestat namespace. Caught exception: "
+                f"{getattr(e, 'message', repr(e))}"
+            )
+            # return an empty mapping
+            return YAMLConfigManager()
+        else:
+            full_namespace = {
+                "schema": psm.schema_path,
+                "results_file": psm.file,
+                "record_id": psm.record_identifier,
+                "namespace": psm.namespace,
+                "config": psm.config_path,
+            }
+            filtered_namespace = {k: v for k, v in full_namespace.items() if v}
+            return YAMLConfigManager(filtered_namespace)
+
     def write_script(self, pool, size):
         """
         Create the script for job submission.
 
         :param Iterable[peppy.Sample] pool: collection of sample instances
         :param float size: cumulative size of the given pool
         :return str: Path to the job submission script created.
         """
         # looper settings determination
         if self.collate:
             pool = [None]
-        looper = self._set_looper_namespace(pool, size)
+        looper = self._build_looper_namespace(pool, size)
         commands = []
-        namespaces = dict(project=self.prj[CONFIG_KEY],
-                          looper=looper,
-                          pipeline=self.pl_iface,
-                          compute=self.prj.dcc.compute)
+        namespaces = dict(
+            project=self.prj[CONFIG_KEY],
+            looper=looper,
+            pipeline=self.pl_iface,
+            compute=self.prj.dcc.compute,
+        )
         templ = self.pl_iface["command_template"]
         if not self.override_extra:
-            extras_template = EXTRA_PROJECT_CMD_TEMPLATE if self.collate \
+            extras_template = (
+                EXTRA_PROJECT_CMD_TEMPLATE
+                if self.collate
                 else EXTRA_SAMPLE_CMD_TEMPLATE
+            )
             templ += extras_template
         for sample in pool:
             # cascading compute settings determination:
             # divcfg < pipeline interface < config <  CLI
             cli = self.compute_variables or {}  # CLI
             if sample:
                 namespaces.update({"sample": sample})
             else:
                 namespaces.update({"samples": self.prj.samples})
-            res_pkg = self.pl_iface.choose_resource_package(namespaces, size or 0)  # config
+            pipestat_namespace = self._set_pipestat_namespace(
+                sample_name=sample.sample_name if sample else None
+            )
+            namespaces.update({"pipestat": pipestat_namespace})
+            res_pkg = self.pl_iface.choose_resource_package(
+                namespaces, size or 0
+            )  # config
             res_pkg.update(cli)
             self.prj.dcc.compute.update(res_pkg)  # divcfg
             namespaces["compute"].update(res_pkg)
-            self.pl_iface.render_var_templates(namespaces=namespaces)
-            namespaces["pipeline"] = self.pl_iface
+            # Here we make a copy of this so that each iteration gets its own template values
+            pl_iface = {}
+            pl_iface.update(self.pl_iface)
+            pl_iface[VAR_TEMPL_KEY] = self.pl_iface.render_var_templates(
+                namespaces=namespaces
+            )
+            _LOGGER.debug(f"namespace pipelines: { pl_iface }")
+            namespaces["pipeline"]["var_templates"] = pl_iface[VAR_TEMPL_KEY]
             # pre_submit hook namespace updates
-            namespaces = _exec_pre_submit(self.pl_iface, namespaces)
+            namespaces = _exec_pre_submit(pl_iface, namespaces)
             self._rendered_ok = False
             try:
-                argstring = jinja_render_template_strictly(template=templ,
-                                                           namespaces=namespaces)
+                argstring = jinja_render_template_strictly(
+                    template=templ, namespaces=namespaces
+                )
             except UndefinedError as jinja_exception:
                 _LOGGER.warning(NOT_SUB_MSG.format(str(jinja_exception)))
             except KeyError as e:
                 exc = "pipeline interface is missing {} section".format(str(e))
                 _LOGGER.warning(NOT_SUB_MSG.format(exc))
             else:
                 commands.append("{} {}".format(argstring, self.extra_pipe_args))
                 self._rendered_ok = True
                 self._num_good_job_submissions += 1
                 self._num_total_job_submissions += 1
-        looper.command = "\n".join(commands)
+        looper["command"] = "\n".join(commands)
         if self.collate:
             _LOGGER.debug("samples namespace:\n{}".format(self.prj.samples))
         else:
-            _LOGGER.debug("sample namespace:\n{}".format(
-                sample.__str__(max_attr=len(list(sample.keys())))))
+            _LOGGER.debug(
+                "sample namespace:\n{}".format(
+                    sample.__str__(max_attr=len(list(sample.keys())))
+                )
+            )
         _LOGGER.debug("project namespace:\n{}".format(self.prj[CONFIG_KEY]))
         _LOGGER.debug("pipeline namespace:\n{}".format(self.pl_iface))
         _LOGGER.debug("compute namespace:\n{}".format(self.prj.dcc.compute))
         _LOGGER.debug("looper namespace:\n{}".format(looper))
-        subm_base = os.path.join(self.prj.submission_folder, looper.job_name)
-        return self.prj.dcc.write_script(output_path=subm_base + ".sub",
-                                         extra_vars=[{"looper": looper}])
+        _LOGGER.debug("pipestat namespace:\n{}".format(pipestat_namespace))
+        subm_base = os.path.join(self.prj.submission_folder, looper[JOB_NAME_KEY])
+        return self.prj.dcc.write_script(
+            output_path=subm_base + ".sub", extra_vars=[{"looper": looper}]
+        )
 
     def write_skipped_sample_scripts(self):
         """
         For any sample skipped during initial processing write submission script
         """
         if self._curr_skip_pool:
             # move any hanging samples from current skip pool to the main pool
             self._skipped_sample_pools.append(
                 (self._curr_skip_pool, self._curr_skip_size)
             )
         if self._skipped_sample_pools:
-            _LOGGER.info("Writing {} submission scripts for skipped samples".
-                          format(len(self._skipped_sample_pools)))
-            [self.write_script(pool, size)
-             for pool, size in self._skipped_sample_pools]
+            _LOGGER.info(
+                "Writing {} submission scripts for skipped samples".format(
+                    len(self._skipped_sample_pools)
+                )
+            )
+            [self.write_script(pool, size) for pool, size in self._skipped_sample_pools]
 
     def _reset_pool(self):
-        """ Reset the state of the pool of samples """
+        """Reset the state of the pool of samples"""
         self._pool = []
         self._curr_size = 0
 
     def _reset_curr_skips(self):
         self._curr_skip_pool = []
         self._curr_skip_size = 0
 
@@ -616,63 +802,68 @@
     Execute pre submission hooks defined in the pipeline interface
 
     :param PipelineInterface piface: piface, a source of pre_submit hooks to execute
     :param dict[dict[]] namespaces: namspaces mapping
     :return dict[dict[]]: updated namspaces mapping
     """
 
-    def _log_raise_latest(cmd):
-        """ Log error info and raise latest handled exception """
-        _LOGGER.error("Could not retrieve JSON via command: '{}'".format(cmd))
-        raise
-
     def _update_namespaces(x, y, cmd=False):
         """
         Update namespaces mapping with a dictionary of the same structure,
         that includes just the values that need to be updated.
 
         :param dict[dict] x: namespaces mapping
         :param dict[dict] y: mapping to update namespaces with
-        :param bool cmd: whether the mapping to upodate with comes from the
+        :param bool cmd: whether the mapping to update with comes from the
             command template, used for messaging
         """
+        if not y:
+            return
         if not isinstance(y, dict):
             if cmd:
                 raise TypeError(
                     f"Object returned by {PRE_SUBMIT_HOOK_KEY}."
                     f"{PRE_SUBMIT_CMD_KEY} must return a dictionary when "
-                    f"processed with json.loads(), not {y.__class__.__name__}")
-            raise TypeError(f"Object returned by {PRE_SUBMIT_HOOK_KEY}."
-                            f"{PRE_SUBMIT_PY_FUN_KEY} must return a dictionary,"
-                            f" not {y.__class__.__name__}")
+                    f"processed with json.loads(), not {y.__class__.__name__}"
+                )
+            raise TypeError(
+                f"Object returned by {PRE_SUBMIT_HOOK_KEY}."
+                f"{PRE_SUBMIT_PY_FUN_KEY} must return a dictionary,"
+                f" not {y.__class__.__name__}"
+            )
         _LOGGER.debug("Updating namespaces with:\n{}".format(y))
         for namespace, mapping in y.items():
-            for attr, val in mapping.items():
-                setattr(x[namespace], attr, val)
+            for key, val in mapping.items():
+                x[namespace][key] = val
+
     if PRE_SUBMIT_HOOK_KEY in piface:
         pre_submit = piface[PRE_SUBMIT_HOOK_KEY]
         if PRE_SUBMIT_PY_FUN_KEY in pre_submit:
             for py_fun in pre_submit[PRE_SUBMIT_PY_FUN_KEY]:
                 pkgstr, funcstr = os.path.splitext(py_fun)
                 pkg = importlib.import_module(pkgstr)
                 func = getattr(pkg, funcstr[1:])
-                _LOGGER.info("Calling pre-submit function: {}.{}".format(
-                    pkgstr, func.__name__))
+                _LOGGER.info(
+                    "Calling pre-submit function: {}.{}".format(pkgstr, func.__name__)
+                )
                 _update_namespaces(namespaces, func(namespaces))
         if PRE_SUBMIT_CMD_KEY in pre_submit:
             for cmd_template in pre_submit[PRE_SUBMIT_CMD_KEY]:
                 _LOGGER.debug(
-                    "Rendering pre-submit command template: {}".format(
-                        cmd_template))
+                    "Rendering pre-submit command template: {}".format(cmd_template)
+                )
                 try:
-                    cmd = jinja_render_template_strictly(template=cmd_template,
-                                                         namespaces=namespaces)
+                    cmd = jinja_render_template_strictly(
+                        template=cmd_template, namespaces=namespaces
+                    )
                     _LOGGER.info("Executing pre-submit command: {}".format(cmd))
                     json = loads(check_output(cmd, shell=True))
-                except CalledProcessError as e:
-                    print(e.output)
-                    _log_raise_latest(cmd)
-                except Exception:
-                    _log_raise_latest(cmd_template)
+                except Exception as e:
+                    if hasattr(e, "output"):
+                        print(e.output)
+                    _LOGGER.error(
+                        "Could not retrieve JSON via command: '{}'".format(cmd)
+                    )
+                    raise
                 else:
                     _update_namespaces(namespaces, json, cmd=True)
     return namespaces
```

### Comparing `looper-1.3.2/looper/exceptions.py` & `looper-1.4.0/looper/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,76 +1,93 @@
 """ Exceptions for specific looper issues. """
 
 from abc import ABCMeta
-from collections import Iterable
+from collections.abc import Iterable
 
 __author__ = "Vince Reuter"
 __email__ = "vreuter@virginia.edu"
 
-_all__ = ["DuplicatePipelineKeyException",
-          "InvalidResourceSpecificationException",
-          "JobSubmissionException",
-          "LooperError",
-          "MissingPipelineConfigurationException",
-          "PipelineInterfaceConfigError",
-          "PipelineInterfaceRequirementsError",
-          "MisconfigurationException"]
+_all__ = [
+    "DuplicatePipelineKeyException",
+    "InvalidResourceSpecificationException",
+    "JobSubmissionException",
+    "LooperError",
+    "MissingPipelineConfigurationException",
+    "PipelineInterfaceConfigError",
+    "PipelineInterfaceRequirementsError",
+    "MisconfigurationException",
+]
 
 
 class LooperError(Exception):
-    """ Base type for custom package errors. """
+    """Base type for custom package errors."""
+
     __metaclass__ = ABCMeta
 
 
+class SampleFailedException(LooperError):
+    """An exception to be raised if any sample fails"""
+
+    pass
+
+
 class MisconfigurationException(LooperError):
-    """ Duplication of pipeline identifier precludes unique pipeline ref. """
+    """Duplication of pipeline identifier precludes unique pipeline ref."""
+
     def __init__(self, key):
         super(MisconfigurationException, self).__init__(key)
 
 
 class DuplicatePipelineKeyException(LooperError):
-    """ Duplication of pipeline identifier precludes unique pipeline ref. """
+    """Duplication of pipeline identifier precludes unique pipeline ref."""
+
     def __init__(self, key):
         super(DuplicatePipelineKeyException, self).__init__(key)
 
 
 class InvalidResourceSpecificationException(LooperError):
-    """ Pipeline interface resources--if present--needs default. """
+    """Pipeline interface resources--if present--needs default."""
+
     def __init__(self, reason):
         super(InvalidResourceSpecificationException, self).__init__(reason)
 
 
 class JobSubmissionException(LooperError):
-    """ Error type for when job submission fails. """
+    """Error type for when job submission fails."""
+
     def __init__(self, sub_cmd, script):
         self.script = script
-        reason = "Error for command {} and script '{}'".\
-            format(sub_cmd, self.script)
+        reason = "Error for command {} and script '{}'".format(sub_cmd, self.script)
         super(JobSubmissionException, self).__init__(reason)
 
 
 class MissingPipelineConfigurationException(LooperError):
-    """ A selected pipeline needs configuration data. """
+    """A selected pipeline needs configuration data."""
+
     def __init__(self, pipeline):
         super(MissingPipelineConfigurationException, self).__init__(pipeline)
 
 
 class PipelineInterfaceConfigError(LooperError):
-    """ Error with PipelineInterface config data during construction. """
+    """Error with PipelineInterface config data during construction."""
+
     def __init__(self, context):
         """
         For exception context, provide message or collection of missing sections.
 
         :param str | Iterable[str] context:
         """
         if not isinstance(context, str) and isinstance(context, Iterable):
             context = "Missing section(s): {}".format(", ".join(context))
         super(PipelineInterfaceConfigError, self).__init__(context)
 
 
 class PipelineInterfaceRequirementsError(LooperError):
-    """ Invalid specification of pipeline requirements in interface config. """
+    """Invalid specification of pipeline requirements in interface config."""
+
     def __init__(self, typename_by_requirement):
         super(PipelineInterfaceRequirementsError, self).__init__(
             "{} invalid requirements: {}".format(
-                len(typename_by_requirement), typename_by_requirement))
+                len(typename_by_requirement), typename_by_requirement
+            )
+        )
         self.error_specs = typename_by_requirement
```

### Comparing `looper-1.3.2/looper/html_reports.py` & `looper-1.4.0/looper/html_reports.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,60 +1,67 @@
 """ Generate HTML reports """
 
-import os
 import glob
-import pandas as _pd
 import logging
-import jinja2
+import os
 import re
 import sys
-from warnings import warn
+from copy import copy as cp
 from datetime import timedelta
+
+import jinja2
+import pandas as _pd
+from eido import read_schema
+from peppy.const import *
+
 from ._version import __version__ as v
 from .const import *
 from .processed_project import get_project_outputs
-from .utils import get_file_for_project
-from peppy.const import *
-from eido import read_schema
-from copy import copy as cp
+from .utils import get_file_for_project_old
+
 _LOGGER = logging.getLogger("looper")
 
 
-class HTMLReportBuilder(object):
-    """ Generate HTML summary report for project/samples """
+class HTMLReportBuilderOld(object):
+    """Generate HTML summary report for project/samples"""
 
     def __init__(self, prj):
         """
         The Project defines the instance.
 
         :param Project prj: Project with which to work/operate on
         """
-        super(HTMLReportBuilder, self).__init__()
+        super(HTMLReportBuilderOld, self).__init__()
         self.prj = prj
         self.j_env = get_jinja_env()
-        self.reports_dir = get_file_for_project(self.prj, "reports")
-        self.index_html_path = get_file_for_project(self.prj, "summary.html")
+        self.reports_dir = get_file_for_project_old(self.prj, "reports")
+        self.index_html_path = get_file_for_project_old(self.prj, "summary.html")
         self.index_html_filename = os.path.basename(self.index_html_path)
         self._outdir = self.prj.output_dir
         _LOGGER.debug("Reports dir: {}".format(self.reports_dir))
 
     def __call__(self, objs, stats, columns):
-        """ Do the work of the subcommand/program. """
+        """Do the work of the subcommand/program."""
         # Generate HTML report
-        navbar = self.create_navbar(self.create_navbar_links(
-            objs=objs, stats=stats,
-            wd=self._outdir),
-            self.index_html_filename)
+        navbar = self.create_navbar(
+            self.create_navbar_links(objs=objs, stats=stats, wd=self._outdir),
+            self.index_html_filename,
+        )
         navbar_reports = self.create_navbar(
-            self.create_navbar_links(
-                objs=objs, stats=stats, wd=self.reports_dir),
-            os.path.join("..", self.index_html_filename))
+            self.create_navbar_links(objs=objs, stats=stats, wd=self.reports_dir),
+            os.path.join(os.pardir, self.index_html_filename),
+        )
         index_html_path = self.create_index_html(
-            objs, stats, columns, footer=self.create_footer(),
-            navbar=navbar, navbar_reports=navbar_reports)
+            objs,
+            stats,
+            columns,
+            footer=self.create_footer(),
+            navbar=navbar,
+            navbar_reports=navbar_reports,
+        )
         return index_html_path
 
     def create_object_parent_html(self, objs, navbar, footer):
         """
         Generates a page listing all the project objects with links
         to individual object pages
 
@@ -66,23 +73,29 @@
         object_parent_path = os.path.join(self.reports_dir, "objects.html")
 
         if not os.path.exists(os.path.dirname(object_parent_path)):
             os.makedirs(os.path.dirname(object_parent_path))
         pages = list()
         labels = list()
         if not objs.empty:
-            for key in objs['key'].drop_duplicates().sort_values():
+            for key in objs["key"].drop_duplicates().sort_values():
                 page_name = key + ".html"
-                page_path = os.path.join(self.reports_dir, page_name.replace(' ', '_').lower())
+                page_path = os.path.join(
+                    self.reports_dir, page_name.replace(" ", "_").lower()
+                )
                 page_relpath = os.path.relpath(page_path, self.reports_dir)
                 pages.append(page_relpath)
                 labels.append(key)
 
-        template_vars = dict(navbar=navbar, footer=footer, labels=labels, pages=pages, header="Objects")
-        return render_jinja_template("navbar_list_parent.html", self.j_env, template_vars)
+        template_vars = dict(
+            navbar=navbar, footer=footer, labels=labels, pages=pages, header="Objects"
+        )
+        return render_jinja_template(
+            "navbar_list_parent.html", self.j_env, template_vars
+        )
 
     def create_sample_parent_html(self, navbar, footer):
         """
         Generates a page listing all the project samples with links
         to individual sample pages
         :param str navbar: HTML to be included as the navbar in the main summary page
         :param str footer: HTML to be included as the footer
@@ -92,27 +105,32 @@
 
         if not os.path.exists(os.path.dirname(sample_parent_path)):
             os.makedirs(os.path.dirname(sample_parent_path))
         pages = list()
         labels = list()
         for sample in self.prj.samples:
             sample_name = str(sample.sample_name)
-            sample_dir = os.path.join(
-                self.prj.results_folder, sample_name)
+            sample_dir = os.path.join(self.prj.results_folder, sample_name)
 
             # Confirm sample directory exists, then build page
             if os.path.exists(sample_dir):
                 page_name = sample_name + ".html"
-                page_path = os.path.join(self.reports_dir, page_name.replace(' ', '_').lower())
+                page_path = os.path.join(
+                    self.reports_dir, page_name.replace(" ", "_").lower()
+                )
                 page_relpath = os.path.relpath(page_path, self.reports_dir)
                 pages.append(page_relpath)
                 labels.append(sample_name)
 
-        template_vars = dict(navbar=navbar, footer=footer, labels=labels, pages=pages, header="Samples")
-        return render_jinja_template("navbar_list_parent.html", self.j_env, template_vars)
+        template_vars = dict(
+            navbar=navbar, footer=footer, labels=labels, pages=pages, header="Samples"
+        )
+        return render_jinja_template(
+            "navbar_list_parent.html", self.j_env, template_vars
+        )
 
     def create_navbar(self, navbar_links, index_html_relpath):
         """
         Creates the navbar using the privided links
 
         :param str navbar_links: HTML list of links to be inserted into a navbar
         :return str: navbar HTML
@@ -124,15 +142,17 @@
         """
         Renders the footer from the templates directory
 
         :return str: footer HTML
         """
         return render_jinja_template("footer.html", self.j_env, dict(version=v))
 
-    def create_navbar_links(self, objs, stats, wd=None, context=None, include_status=True):
+    def create_navbar_links(
+        self, objs, stats, wd=None, context=None, include_status=True
+    ):
         """
         Return a string containing the navbar prebuilt html.
 
         Generates links to each page relative to the directory of interest (wd arg) or uses the provided context to
         create the paths (context arg)
 
         :param pandas.DataFrame objs: project results dataframe containing
@@ -143,44 +163,74 @@
             relative to page
         :param list[str] context: the context the links will be used in.
             The sequence of directories to be prepended to the HTML file in the resulting navbar
         :param bool include_status: whether the status link should be included in the links set
         :return str: navbar links as HTML-formatted string
         """
         if wd is None and context is None:
-            raise ValueError("Either 'wd' (path the links should be relative to) or 'context'"
-                             " (the context for the links) has to be provided.")
-        status_relpath = _make_relpath(file_name=os.path.join(self.reports_dir, "status.html"), wd=wd, context=context)
-        objects_relpath = _make_relpath(file_name=os.path.join(self.reports_dir, "objects.html"), wd=wd, context=context)
-        samples_relpath = _make_relpath(file_name=os.path.join(self.reports_dir, "samples.html"), wd=wd, context=context)
+            raise ValueError(
+                "Either 'wd' (path the links should be relative to) or 'context'"
+                " (the context for the links) has to be provided."
+            )
+        status_relpath = _make_relpath(
+            file_name=os.path.join(self.reports_dir, "status.html"),
+            wd=wd,
+            context=context,
+        )
+        objects_relpath = _make_relpath(
+            file_name=os.path.join(self.reports_dir, "objects.html"),
+            wd=wd,
+            context=context,
+        )
+        samples_relpath = _make_relpath(
+            file_name=os.path.join(self.reports_dir, "samples.html"),
+            wd=wd,
+            context=context,
+        )
         dropdown_keys_objects = None
         dropdown_relpaths_objects = None
         dropdown_relpaths_samples = None
         sample_names = None
         if objs is not None and not objs.dropna().empty:
             # If the number of objects is 20 or less, use a drop-down menu
-            if len(objs['key'].drop_duplicates()) <= 20:
-                dropdown_relpaths_objects, dropdown_keys_objects = \
-                    _get_navbar_dropdown_data_objects(objs=objs, wd=wd, context=context, reports_dir=self.reports_dir)
+            if len(objs["key"].drop_duplicates()) <= 20:
+                (
+                    dropdown_relpaths_objects,
+                    dropdown_keys_objects,
+                ) = _get_navbar_dropdown_data_objects(
+                    objs=objs, wd=wd, context=context, reports_dir=self.reports_dir
+                )
             else:
                 dropdown_relpaths_objects = objects_relpath
         if stats:
             if len(stats) <= 20:
-                dropdown_relpaths_samples, sample_names = \
-                    _get_navbar_dropdown_data_samples(stats=stats, wd=wd, context=context, reports_dir=self.reports_dir)
+                (
+                    dropdown_relpaths_samples,
+                    sample_names,
+                ) = _get_navbar_dropdown_data_samples(
+                    stats=stats, wd=wd, context=context, reports_dir=self.reports_dir
+                )
             else:
                 # Create a menu link to the samples parent page
                 dropdown_relpaths_samples = samples_relpath
         status_page_name = "Status" if include_status else None
-        template_vars = dict(status_html_page=status_relpath, status_page_name=status_page_name,
-                             dropdown_keys_objects=dropdown_keys_objects, objects_page_name="Objects",
-                             samples_page_name="Samples", objects_html_page=dropdown_relpaths_objects,
-                             samples_html_page=dropdown_relpaths_samples, menu_name_objects="Objects",
-                             menu_name_samples="Samples", sample_names=sample_names, all_samples=samples_relpath,
-                             all_objects=objects_relpath)
+        template_vars = dict(
+            status_html_page=status_relpath,
+            status_page_name=status_page_name,
+            dropdown_keys_objects=dropdown_keys_objects,
+            objects_page_name="Objects",
+            samples_page_name="Samples",
+            objects_html_page=dropdown_relpaths_objects,
+            samples_html_page=dropdown_relpaths_samples,
+            menu_name_objects="Objects",
+            menu_name_samples="Samples",
+            sample_names=sample_names,
+            all_samples=samples_relpath,
+            all_objects=objects_relpath,
+        )
         return render_jinja_template("navbar_links.html", self.j_env, template_vars)
 
     def create_object_html(self, single_object, navbar, footer):
         """
         Generates a page for an individual object type with all of its
         plots from each sample
 
@@ -189,78 +239,103 @@
         :param pandas.DataFrame objs: project level dataframe
             containing any reported objects for all samples
         :param str navbar: HTML to be included as the navbar in the main summary page
         :param str footer: HTML to be included as the footer
         """
 
         # Generate object filename
-        for key in single_object['key'].drop_duplicates().sort_values():
+        for key in single_object["key"].drop_duplicates().sort_values():
             # even though it's always one element, loop to extract the data
             current_name = str(key)
             filename = current_name + ".html"
-        html_page_path = os.path.join(self.reports_dir, filename.replace(' ', '_').lower())
+        html_page_path = os.path.join(
+            self.reports_dir, filename.replace(" ", "_").lower()
+        )
 
         if not os.path.exists(os.path.dirname(html_page_path)):
             os.makedirs(os.path.dirname(html_page_path))
 
         links = []
         figures = []
         warnings = []
         for i, row in single_object.iterrows():
             # Set the PATH to a page for the sample. Catch any errors.
             try:
-                object_path = os.path.join(self.prj.results_folder, row['sample_name'], row['filename'])
+                object_path = os.path.join(
+                    self.prj.results_folder, row["sample_name"], row["filename"]
+                )
                 object_relpath = os.path.relpath(object_path, self.reports_dir)
             except AttributeError:
-                err_msg = ("Sample: {} | " + "Missing valid object path for: {}")
+                err_msg = "Sample: {} | " + "Missing valid object path for: {}"
                 # Report the sample that fails, if that information exists
-                if str(row['sample_name']) and str(row['filename']):
-                    _LOGGER.warning(err_msg.format(row['sample_name'], row['filename']))
+                if str(row["sample_name"]) and str(row["filename"]):
+                    _LOGGER.warning(err_msg.format(row["sample_name"], row["filename"]))
                 else:
                     _LOGGER.warning(err_msg.format("Unknown sample"))
                 object_relpath = ""
 
             # Set the PATH to the image/file. Catch any errors.
             # Check if the object is an HTML document
 
-            if not str(row['anchor_image']).lower().endswith(IMAGE_EXTS):
+            if not str(row["anchor_image"]).lower().endswith(IMAGE_EXTS):
                 image_path = object_path
             else:
                 try:
-                    image_path = os.path.join(self.prj.results_folder, row['sample_name'], row['anchor_image'])
+                    image_path = os.path.join(
+                        self.prj.results_folder, row["sample_name"], row["anchor_image"]
+                    )
                 except AttributeError:
                     _LOGGER.warning(str(row))
-                    err_msg = ("Sample: {} | " + "Missing valid image path for: {}")
+                    err_msg = "Sample: {} | " + "Missing valid image path for: {}"
                     # Report the sample that fails, if that information exists
-                    if str(row['sample_name']) and str(row['filename']):
-                        _LOGGER.warning(err_msg.format(row['sample_name'], row['filename']))
+                    if str(row["sample_name"]) and str(row["filename"]):
+                        _LOGGER.warning(
+                            err_msg.format(row["sample_name"], row["filename"])
+                        )
                     else:
                         _LOGGER.warning(err_msg.format("Unknown", "Unknown"))
                     image_path = ""
             # Check for the presence of both the file and thumbnail
             if os.path.isfile(image_path) and os.path.isfile(object_path):
                 image_relpath = os.path.relpath(image_path, self.reports_dir)
                 # If the object has a valid image, use it!
                 _LOGGER.debug("Checking image path: {}".format(image_path))
                 if str(image_path).lower().endswith(IMAGE_EXTS):
-                    figures.append([object_relpath, str(row['sample_name']), image_relpath])
+                    figures.append(
+                        [object_relpath, str(row["sample_name"]), image_relpath]
+                    )
                 # Or if that "image" is not an image, treat it as a link
                 elif not str(image_path).lower().endswith(IMAGE_EXTS):
                     _LOGGER.debug("Got link")
-                    links.append([str(row['sample_name']), image_relpath])
+                    links.append([str(row["sample_name"]), image_relpath])
             else:
-                warnings.append(str(row['filename']))
+                warnings.append(str(row["filename"]))
 
         if warnings:
-            _LOGGER.warning("create_object_html: " +
-                            filename.replace(' ', '_').lower() + " references nonexistent object files")
-            _LOGGER.debug(filename.replace(' ', '_').lower() +
-                          " nonexistent files: " + ','.join(str(x) for x in warnings))
-        template_vars = dict(navbar=navbar, footer=footer, name=current_name, figures=figures, links=links)
-        save_html(html_page_path, render_jinja_template("object.html", self.j_env, args=template_vars))
+            _LOGGER.warning(
+                "create_object_html: "
+                + filename.replace(" ", "_").lower()
+                + " references nonexistent object files"
+            )
+            _LOGGER.debug(
+                filename.replace(" ", "_").lower()
+                + " nonexistent files: "
+                + ",".join(str(x) for x in warnings)
+            )
+        template_vars = dict(
+            navbar=navbar,
+            footer=footer,
+            name=current_name,
+            figures=figures,
+            links=links,
+        )
+        save_html(
+            html_page_path,
+            render_jinja_template("object.html", self.j_env, args=template_vars),
+        )
 
     def create_sample_html(self, objs, sample_name, sample_stats, navbar, footer):
         """
         Produce an HTML page containing all of a sample's objects
         and the sample summary statistics
 
         :param pandas.DataFrame objs: project level dataframe containing
@@ -268,42 +343,56 @@
         :param str sample_name: the name of the current sample
         :param dict sample_stats: pipeline run statistics for the current sample
         :param str navbar: HTML to be included as the navbar in the main summary page
         :param str footer: HTML to be included as the footer
         :return str: path to the produced HTML page
         """
         html_filename = sample_name + ".html"
-        html_page = os.path.join(self.reports_dir, html_filename.replace(' ', '_').lower())
+        html_page = os.path.join(
+            self.reports_dir, html_filename.replace(" ", "_").lower()
+        )
         sample_page_relpath = os.path.relpath(html_page, self._outdir)
-        single_sample = _pd.DataFrame() if objs.empty else objs[objs['sample_name'] == sample_name]
+        single_sample = (
+            _pd.DataFrame() if objs.empty else objs[objs["sample_name"] == sample_name]
+        )
         if not os.path.exists(os.path.dirname(html_page)):
             os.makedirs(os.path.dirname(html_page))
         sample_dir = os.path.join(self.prj.results_folder, sample_name)
         if os.path.exists(sample_dir):
             if single_sample.empty:
                 # When there is no objects.tsv file, search for the
                 # presence of log, profile, and command files
-                log_name = _match_file_for_sample(sample_name, 'log.md', self.prj.results_folder)
-                profile_name = _match_file_for_sample(sample_name, 'profile.tsv', self.prj.results_folder)
-                command_name = _match_file_for_sample(sample_name, 'commands.sh', self.prj.results_folder)
+                log_name = _match_file_for_sample(
+                    sample_name, "log.md", self.prj.results_folder
+                )
+                profile_name = _match_file_for_sample(
+                    sample_name, "profile.tsv", self.prj.results_folder
+                )
+                command_name = _match_file_for_sample(
+                    sample_name, "commands.sh", self.prj.results_folder
+                )
             else:
-                log_name = str(single_sample.iloc[0]['annotation']) + "_log.md"
-                profile_name = str(single_sample.iloc[0]['annotation']) + "_profile.tsv"
-                command_name = str(single_sample.iloc[0]['annotation']) + "_commands.sh"
+                log_name = str(single_sample.iloc[0]["annotation"]) + "_log.md"
+                profile_name = str(single_sample.iloc[0]["annotation"]) + "_profile.tsv"
+                command_name = str(single_sample.iloc[0]["annotation"]) + "_commands.sh"
             stats_name = "stats.tsv"
             flag = _get_flags(sample_dir)
             # get links to the files
             stats_file_path = _get_relpath_to_file(
-                stats_name, sample_name, self.prj.results_folder, self.reports_dir)
+                stats_name, sample_name, self.prj.results_folder, self.reports_dir
+            )
             profile_file_path = _get_relpath_to_file(
-                profile_name, sample_name, self.prj.results_folder, self.reports_dir)
+                profile_name, sample_name, self.prj.results_folder, self.reports_dir
+            )
             commands_file_path = _get_relpath_to_file(
-                command_name, sample_name, self.prj.results_folder, self.reports_dir)
+                command_name, sample_name, self.prj.results_folder, self.reports_dir
+            )
             log_file_path = _get_relpath_to_file(
-                log_name, sample_name, self.prj.results_folder, self.reports_dir)
+                log_name, sample_name, self.prj.results_folder, self.reports_dir
+            )
             if not flag:
                 button_class = "btn btn-secondary"
                 flag = "Missing"
             elif len(flag) > 1:
                 button_class = "btn btn-secondary"
                 flag = "Multiple"
             else:
@@ -316,77 +405,97 @@
                 else:
                     button_class = flag_dict["button_class"]
                     flag = flag_dict["flag"]
         links = []
         figures = []
         warnings = []
         if not single_sample.empty:
-            for sample_name in single_sample['sample_name'].drop_duplicates().sort_values():
-                o = single_sample[single_sample['sample_name'] == sample_name]
+            for sample_name in (
+                single_sample["sample_name"].drop_duplicates().sort_values()
+            ):
+                o = single_sample[single_sample["sample_name"] == sample_name]
                 for i, row in o.iterrows():
                     try:
                         # Image thumbnails are optional
                         # This references to "image" should really
                         # be "thumbnail"
                         image_path = os.path.join(
-                            self.prj.results_folder,
-                            sample_name, row['anchor_image'])
+                            self.prj.results_folder, sample_name, row["anchor_image"]
+                        )
                         image_relpath = os.path.relpath(image_path, self.reports_dir)
                     except (AttributeError, TypeError):
                         image_path = ""
                         image_relpath = ""
 
                     # These references to "page" should really be
                     # "object", because they can be anything.
                     page_path = os.path.join(
-                        self.prj.results_folder,
-                        sample_name, row['filename'])
+                        self.prj.results_folder, sample_name, row["filename"]
+                    )
                     page_relpath = os.path.relpath(page_path, self.reports_dir)
                     # If the object has a thumbnail image, add as a figure
                     if os.path.isfile(image_path) and os.path.isfile(page_path):
                         # If the object has a valid image, add as a figure
-                        if str(image_path).lower().endswith(('.png', '.jpg', '.jpeg', '.svg', '.gif')):
-                            figures.append([page_relpath, str(row['key']), image_relpath])
+                        if (
+                            str(image_path)
+                            .lower()
+                            .endswith((".png", ".jpg", ".jpeg", ".svg", ".gif"))
+                        ):
+                            figures.append(
+                                [page_relpath, str(row["key"]), image_relpath]
+                            )
                         # Otherwise treat as a link
                         elif os.path.isfile(page_path):
-                            links.append([str(row['key']), page_relpath])
+                            links.append([str(row["key"]), page_relpath])
                         # If neither, there is no object by that name
                         else:
-                            warnings.append(str(row['filename']))
+                            warnings.append(str(row["filename"]))
                     # If no thumbnail image, it's just a link
                     elif os.path.isfile(page_path):
-                        links.append([str(row['key']), page_relpath])
+                        links.append([str(row["key"]), page_relpath])
                     # If no file present, there is no object by that name
                     else:
-                        warnings.append(str(row['filename']))
+                        warnings.append(str(row["filename"]))
         else:
             # Sample was not run through the pipeline
-            _LOGGER.warning("{} is not present in {}".format(
-                sample_name, self.prj.results_folder))
-
-        template_vars = dict(navbar=navbar, footer=footer, sample_name=sample_name, stats_file_path=stats_file_path,
-                             profile_file_path=profile_file_path, commands_file_path=commands_file_path,
-                             log_file_path=log_file_path, button_class=button_class, sample_stats=sample_stats,
-                             flag=flag, links=links, figures=figures)
-        save_html(html_page, render_jinja_template("sample.html", self.j_env, template_vars))
+            _LOGGER.warning(
+                "{} is not present in {}".format(sample_name, self.prj.results_folder)
+            )
+
+        template_vars = dict(
+            navbar=navbar,
+            footer=footer,
+            sample_name=sample_name,
+            stats_file_path=stats_file_path,
+            profile_file_path=profile_file_path,
+            commands_file_path=commands_file_path,
+            log_file_path=log_file_path,
+            button_class=button_class,
+            sample_stats=sample_stats,
+            flag=flag,
+            links=links,
+            figures=figures,
+        )
+        save_html(
+            html_page, render_jinja_template("sample.html", self.j_env, template_vars)
+        )
         return sample_page_relpath
 
     def create_status_html(self, status_table, navbar, footer):
         """
         Generates a page listing all the samples, their run status, their
         log file, and the total runtime if completed.
 
         :param pandas.DataFrame objs: project level dataframe containing any reported objects for all samples
         :param str navbar: HTML to be included as the navbar in the main summary page
         :param str footer: HTML to be included as the footer
         :return str: rendered status HTML file
         """
         _LOGGER.debug("Building status page...")
-        template_vars = dict(status_table=status_table, navbar=navbar,
-                             footer=footer)
+        template_vars = dict(status_table=status_table, navbar=navbar, footer=footer)
         return render_jinja_template("status.html", self.j_env, template_vars)
 
     def create_project_objects(self):
         """
         Render available project level outputs defined in the
         pipeline output schemas
         """
@@ -395,153 +504,175 @@
         links = []
         warnings = []
         # For each protocol report the project summarizers' results
         self.prj.populate_pipeline_outputs()
         ifaces = self.prj.project_pipeline_interfaces
         # Check the interface files for summarizers
         for iface in ifaces:
-            schema_paths = \
-                iface.get_pipeline_schemas(OUTPUT_SCHEMA_KEY)
+            schema_paths = iface.get_pipeline_schemas(OUTPUT_SCHEMA_KEY)
             if schema_paths is not None:
                 if isinstance(schema_paths, str):
                     schema_paths = [schema_paths]
                 for output_schema_path in schema_paths:
                     results = get_project_outputs(
-                        self.prj, read_schema(output_schema_path))
+                        self.prj, read_schema(output_schema_path)
+                    )
                     for name, result in results.items():
-                        title = str(result.setdefault('title', "No caption"))
-                        result_type = str(result['type'])
-                        result_file = str(result['path'])
-                        result_img = \
-                            str(result.setdefault('thumbnail_path', None))
+                        title = str(result.setdefault("title", "No caption"))
+                        result_type = str(result["type"])
+                        result_file = str(result["path"])
+                        result_img = str(result.setdefault("thumbnail_path", None))
                         if result_img and not os.path.isabs(result_file):
-                            result_img = os.path.join(
-                                self._outdir, result_img)
+                            result_img = os.path.join(self._outdir, result_img)
                         if not os.path.isabs(result_file):
-                            result_file = os.path.join(
-                                self._outdir, result_file)
-                        _LOGGER.debug("Looking for project file: {}".
-                                      format(result_file))
+                            result_file = os.path.join(self._outdir, result_file)
+                        _LOGGER.debug(
+                            "Looking for project file: {}".format(result_file)
+                        )
                         # Confirm the file itself was produced
                         if glob.glob(result_file):
                             file_path = str(glob.glob(result_file)[0])
-                            file_relpath = \
-                                os.path.relpath(file_path, self._outdir)
+                            file_relpath = os.path.relpath(file_path, self._outdir)
                             if result_type == "image":
                                 # Add as a figure, find thumbnail
                                 search = os.path.join(self._outdir, result_img)
                                 if glob.glob(search):
                                     img_path = str(glob.glob(search)[0])
-                                    img_relpath = \
-                                        os.path.relpath(img_path, self._outdir)
-                                    figures.append(
-                                        [file_relpath, title, img_relpath])
+                                    img_relpath = os.path.relpath(
+                                        img_path, self._outdir
+                                    )
+                                    figures.append([file_relpath, title, img_relpath])
                             # add as a link otherwise
                             # TODO: add more fine-grained type support?
                             #  not just image and link
                             else:
                                 links.append([title, file_relpath])
                         else:
-                            warnings.append("{} ({})".format(title,
-                                                             result_file))
+                            warnings.append("{} ({})".format(title, result_file))
             else:
-                _LOGGER.debug("No project-level outputs defined in "
-                              "schema: {}".format(schema_paths))
+                _LOGGER.debug(
+                    "No project-level outputs defined in "
+                    "schema: {}".format(schema_paths)
+                )
         if warnings:
-            _LOGGER.warning("Not found: {}".
-                            format([str(x) for x in warnings]))
+            _LOGGER.warning("Not found: {}".format([str(x) for x in warnings]))
         _LOGGER.debug("collected project-level figures: {}".format(figures))
         _LOGGER.debug("collected project-level links: {}".format(links))
         template_vars = dict(figures=figures, links=links)
-        return render_jinja_template("project_object.html", self.j_env,
-                                     template_vars)
+        return render_jinja_template("project_object.html", self.j_env, template_vars)
 
-    def create_index_html(self, objs, stats, col_names, navbar, footer, navbar_reports=None):
+    def create_index_html(
+        self, objs, stats, col_names, navbar, footer, navbar_reports=None
+    ):
         """
         Generate an index.html style project home page w/ sample summary
         statistics
 
         :param pandas.DataFrame objs: project level dataframe containing
             any reported objects for all samples
         :param list[dict] stats: a summary file of pipeline statistics for each
             analyzed sample
         :param list col_names: all unique column names used in the stats file
         :param str navbar: HTML to be included as the navbar in the main summary page
         :param str footer: HTML to be included as the footer
         :param str navbar_reports: HTML to be included as the navbar for pages in the reports directory
         """
         # set default encoding when running in python2
-        if sys.version[0] == '2':
+        if sys.version[0] == "2":
             from importlib import reload
+
             reload(sys)
             sys.setdefaultencoding("utf-8")
         _LOGGER.debug("Building index page...")
         # copy the columns names and remove the sample_name one, since it will be processed differently
         cols = cp(col_names)
         cols.remove("sample_name")
         if navbar_reports is None:
             navbar_reports = navbar
         if not objs.dropna().empty:
-            objs.drop_duplicates(keep='last', inplace=True)
+            objs.drop_duplicates(keep="last", inplace=True)
         # Generate parent index.html page path
-        index_html_path = get_file_for_project(self.prj, "summary.html")
+        index_html_path = get_file_for_project_old(self.prj, "summary.html")
 
         # Add stats_summary.tsv button link
         stats_file_name = os.path.join(self._outdir, self.prj.name)
         if hasattr(self.prj, "subproject") and self.prj.subproject:
-            stats_file_name += '_' + self.prj.subproject
-        stats_file_name += '_stats_summary.tsv'
+            stats_file_name += "_" + self.prj.subproject
+        stats_file_name += "_stats_summary.tsv"
         stats_file_path = os.path.relpath(stats_file_name, self._outdir)
         # Add stats summary table to index page and produce individual
         # sample pages
         if os.path.isfile(stats_file_name):
             # Produce table rows
             table_row_data = []
             samples_cols_missing = []
             _LOGGER.debug(" * Creating sample pages...")
             for row in stats:
                 table_cell_data = []
                 sample_name = row["sample_name"]
-                sample_page = self.create_sample_html(objs, sample_name, row, navbar_reports, footer)
+                sample_page = self.create_sample_html(
+                    objs, sample_name, row, navbar_reports, footer
+                )
                 # treat sample_name column differently - provide a link to the sample page
                 table_cell_data.append([sample_page, sample_name])
                 # for each column read the data from the stats
                 for c in cols:
                     try:
                         table_cell_data.append(str(row[c]))
                     except KeyError:
                         table_cell_data.append("NA")
                         samples_cols_missing.append(sample_name)
                 table_row_data.append(table_cell_data)
-            _LOGGER.debug("Samples with missing columns: {}".format(set(samples_cols_missing)))
+            _LOGGER.debug(
+                "Samples with missing columns: {}".format(set(samples_cols_missing))
+            )
         else:
             _LOGGER.warning("No stats file '%s'", stats_file_name)
 
         # Create parent samples page with links to each sample
-        save_html(os.path.join(self.reports_dir, "samples.html"), self.create_sample_parent_html(navbar_reports, footer))
+        save_html(
+            os.path.join(self.reports_dir, "samples.html"),
+            self.create_sample_parent_html(navbar_reports, footer),
+        )
         _LOGGER.debug(" * Creating object pages...")
         # Create objects pages
         if not objs.dropna().empty:
-            for key in objs['key'].drop_duplicates().sort_values():
-                single_object = objs[objs['key'] == key]
+            for key in objs["key"].drop_duplicates().sort_values():
+                single_object = objs[objs["key"] == key]
                 self.create_object_html(single_object, navbar_reports, footer)
 
         # Create parent objects page with links to each object type
-        save_html(os.path.join(self.reports_dir, "objects.html"),
-                  self.create_object_parent_html(objs, navbar_reports, footer))
+        save_html(
+            os.path.join(self.reports_dir, "objects.html"),
+            self.create_object_parent_html(objs, navbar_reports, footer),
+        )
         # Create status page with each sample's status listed
-        save_html(os.path.join(self.reports_dir, "status.html"),
-                  self.create_status_html(create_status_table(self.prj), navbar_reports, footer))
+        save_html(
+            os.path.join(self.reports_dir, "status.html"),
+            self.create_status_html(
+                create_status_table(self.prj), navbar_reports, footer
+            ),
+        )
         # Add project level objects
         project_objects = self.create_project_objects()
         # Complete and close HTML file
-        template_vars = dict(project_name=self.prj.name, stats_json=_read_tsv_to_json(stats_file_name),
-                             navbar=navbar, footer=footer, stats_file_path=stats_file_path,
-                             project_objects=project_objects, columns=col_names, table_row_data=table_row_data)
-        save_html(index_html_path, render_jinja_template("index.html", self.j_env, template_vars))
+        template_vars = dict(
+            project_name=self.prj.name,
+            stats_json=_read_tsv_to_json(stats_file_name),
+            navbar=navbar,
+            footer=footer,
+            stats_file_path=stats_file_path,
+            project_objects=project_objects,
+            columns=col_names,
+            table_row_data=table_row_data,
+        )
+        save_html(
+            index_html_path,
+            render_jinja_template("index.html", self.j_env, template_vars),
+        )
         return index_html_path
 
 
 def render_jinja_template(name, jinja_env, args=dict()):
     """
     Render template in the specified jinja environment using the provided args
 
@@ -561,49 +692,61 @@
 
     :param str path: the desired location for the file to be produced
     :param str template: the template or just string
     """
     if not os.path.exists(os.path.dirname(path)):
         os.makedirs(os.path.dirname(path))
     try:
-        with open(path, 'w') as f:
+        with open(path, "w") as f:
             f.write(template)
     except IOError:
         _LOGGER.error("Could not write the HTML file: {}".format(path))
 
 
 def get_jinja_env(templates_dirname=None):
     """
     Create jinja environment with the provided path to the templates directory
 
     :param str templates_dirname: path to the templates directory
     :return jinja2.Environment: jinja environment
     """
     if templates_dirname is None:
         file_dir = os.path.dirname(os.path.realpath(__file__))
-        templates_dirname = os.path.join(file_dir, TEMPLATES_DIRNAME)
+        templates_dirname = os.path.join(file_dir, f"{TEMPLATES_DIRNAME}_old")
     _LOGGER.debug("Using templates dir: " + templates_dirname)
     return jinja2.Environment(loader=jinja2.FileSystemLoader(templates_dirname))
 
 
 def _get_flags(sample_dir):
     """
     Get the flag(s) present in the directory
 
     :param str sample_dir: path to the directory to be searched for flags
     :return list: flags found in the dir
     """
-    assert os.path.exists(sample_dir), "The provided path ('{}') does not exist".format(sample_dir)
-    flag_files = glob.glob(os.path.join(sample_dir, '*.flag'))
+    assert os.path.exists(sample_dir), "The provided path ('{}') does not exist".format(
+        sample_dir
+    )
+    flag_files = glob.glob(os.path.join(sample_dir, "*.flag"))
     if len(flag_files) > 1:
-        _LOGGER.warning("Multiple flag files ({files_count}) found in sample dir '{sample_dir}'".
-                        format(files_count=len(flag_files), sample_dir=sample_dir))
+        _LOGGER.warning(
+            "Multiple flag files ({files_count}) found in sample dir '{sample_dir}'".format(
+                files_count=len(flag_files), sample_dir=sample_dir
+            )
+        )
     if len(flag_files) == 0:
-        _LOGGER.warning("No flag files found in sample dir '{sample_dir}'".format(sample_dir=sample_dir))
-    return [re.search(r'\_([a-z]+)\.flag$', os.path.basename(f)).groups()[0] for f in flag_files]
+        _LOGGER.warning(
+            "No flag files found in sample dir '{sample_dir}'".format(
+                sample_dir=sample_dir
+            )
+        )
+    return [
+        re.search(r"\_([a-z]+)\.flag$", os.path.basename(f)).groups()[0]
+        for f in flag_files
+    ]
 
 
 def _match_file_for_sample(sample_name, appendix, location, full_path=False):
     """
     Safely looks for files matching the appendix in the specified location for the sample
 
     :param str sample_name: name of the sample that the file name should be found for
@@ -614,15 +757,19 @@
     """
     regex = "*" + appendix
     search_pattern = os.path.join(location, sample_name, regex)
     matches = glob.glob(search_pattern)
     if len(matches) < 1:
         return None
     elif len(matches) > 1:
-        _LOGGER.warning("matched mutiple files for '{}'. Returning the first one".format(search_pattern))
+        _LOGGER.warning(
+            "matched mutiple files for '{}'. Returning the first one".format(
+                search_pattern
+            )
+        )
     return matches[0] if full_path else os.path.basename(matches[0])
 
 
 def _get_relpath_to_file(file_name, sample_name, location, relative_to):
     """
     Safely gets the relative path for the file for the specified sample
 
@@ -654,31 +801,33 @@
     return relpath if not context else os.path.join(os.path.join(*context), relpath)
 
 
 def _get_navbar_dropdown_data_objects(objs, wd, context, reports_dir):
     if objs is None:
         return None, None
     relpaths = []
-    df_keys = objs['key'].drop_duplicates().sort_values()
+    df_keys = objs["key"].drop_duplicates().sort_values()
     for key in df_keys:
-        page_name = os.path.join(reports_dir, (key + ".html").replace(' ', '_').lower())
+        page_name = os.path.join(reports_dir, (key + ".html").replace(" ", "_").lower())
         relpaths.append(_make_relpath(page_name, wd, context))
     return relpaths, df_keys
 
 
 def _get_navbar_dropdown_data_samples(stats, wd, context, reports_dir):
     if stats is None:
         return None, None
     relpaths = []
     sample_names = []
     for sample in stats:
         for entry, val in sample.items():
             if entry == "sample_name":
                 sample_name = str(val)
-                page_name = os.path.join(reports_dir, (sample_name + ".html").replace(' ', '_').lower())
+                page_name = os.path.join(
+                    reports_dir, (sample_name + ".html").replace(" ", "_").lower()
+                )
                 relpaths.append(_make_relpath(page_name, wd, context))
                 sample_names.append(sample_name)
                 break
             else:
                 _LOGGER.warning("Could not determine sample name in stats.tsv")
     return relpaths, sample_names
 
@@ -695,39 +844,47 @@
         e = encodings[idx]
         try:
             t = _pd.read_csv(path, encoding=e, **kwargs)
             return t
         except UnicodeDecodeError:
             pass
         idx = idx + 1
-    _LOGGER.warning("Could not read the log file '{p}' with encodings '{enc}'".format(p=path, enc=encodings))
+    _LOGGER.warning(
+        "Could not read the log file '{p}' with encodings '{enc}'".format(
+            p=path, enc=encodings
+        )
+    )
 
 
 def _get_from_log(log_path, regex):
     """
     Get the value for the matched key from log file
 
     :param str log_path: path to the log file
     :param str regex: matching str. Should be formatted as follows: r'(phrase to match)'
     :return str: matched and striped string
     :raises IOError: when the file is not found in the provided path
     """
     if not os.path.exists(log_path):
         raise IOError("Can't read the log file '{}'. Not found".format(log_path))
-    log = _read_csv_encodings(log_path, header=None, names=['data'])
+    log = _read_csv_encodings(log_path, header=None, names=["data"])
     if log is None:
         _LOGGER.warning("'{r}' was not read from log".format(r=regex))
         return None
     # match regex, get row(s) that matched the regex
     log_row = log.iloc[:, 0].str.extractall(regex)
     # not matches? return None
     if log_row.empty:
         return None
     if log_row.size > 1:
-        _LOGGER.warning("When parsing '{lp}', more than one values matched with: {r}. Returning first.".format(lp=log_path, r=regex))
+        _LOGGER.warning(
+            "When parsing '{lp}', more than one values matched with: {r}. Returning first.".format(
+                lp=log_path, r=regex
+            )
+        )
     # split the matched line by first colon return stripped data.
     # This way both mem values (e.g 1.1GB) and time values (e.g 1:10:10) will work.
     val = log.iloc[log_row.index[0][0]].str.split(":", 1, expand=True)[1][0].strip()
     return val
 
 
 def _read_tsv_to_json(path):
@@ -740,15 +897,15 @@
     assert os.path.exists(path), "The file '{}' does not exist".format(path)
     _LOGGER.debug("Reading TSV from '{}'".format(path))
     df = _pd.read_csv(path, sep="\t", index_col=False, header=None)
     return df.to_json()
 
 
 def uniqify(seq):
-    """ Fast way to uniqify while preserving input order. """
+    """Fast way to uniqify while preserving input order."""
     # http://stackoverflow.com/questions/480214/
     seen = set()
     seen_add = seen.add
     return [x for x in seq if not (x in seen or seen_add(x))]
 
 
 def create_status_table(prj, final=True):
@@ -772,16 +929,15 @@
     sample_link_names = []
     flags = []
     row_classes = []
     times = []
     mems = []
     for sample in prj.samples:
         sample_name = str(sample.sample_name)
-        sample_dir = os.path.join(
-            prj.results_folder, sample_name)
+        sample_dir = os.path.join(prj.results_folder, sample_name)
 
         # Confirm sample directory exists, then build page
         if os.path.exists(sample_dir):
             # Grab the status flag for the current sample
             flag = _get_flags(sample_dir)
             if not flag:
                 button_class = "table-secondary"
@@ -798,81 +954,104 @@
                     flag = "Unknown"
                 else:
                     button_class = flag_dict["button_class"]
                     flag = flag_dict["flag"]
             row_classes.append(button_class)
             # get first column data (sample name/link)
             page_name = sample_name + ".html"
-            page_path = os.path.join(get_file_for_project(prj, "reports"),
-                                     page_name.replace(' ', '_').lower())
-            page_relpath = os.path.relpath(page_path,
-                                           get_file_for_project(prj, "reports"))
+            page_path = os.path.join(
+                get_file_for_project_old(prj, "reports"),
+                page_name.replace(" ", "_").lower(),
+            )
+            page_relpath = os.path.relpath(
+                page_path, get_file_for_project_old(prj, "reports")
+            )
             sample_paths.append(page_relpath)
             sample_link_names.append(sample_name)
             # get second column data (status/flag)
             flags.append(flag)
             # get third column data (log file/link)
-            log_name = _match_file_for_sample(sample_name, "log.md",
-                                              prj.results_folder)
-            log_file_link = \
-                _get_relpath_to_file(log_name, sample_name, prj.results_folder,
-                                     get_file_for_project(prj, "reports"))
+            log_name = _match_file_for_sample(sample_name, "log.md", prj.results_folder)
+            log_file_link = _get_relpath_to_file(
+                log_name,
+                sample_name,
+                prj.results_folder,
+                get_file_for_project_old(prj, "reports"),
+            )
             log_link_names.append(log_name)
             log_paths.append(log_file_link)
             # get fourth column data (runtime) and fifth column data (memory)
-            profile_file_path = \
-                _match_file_for_sample(sample.sample_name, 'profile.tsv',
-                                       prj.results_folder, full_path=True)
+            profile_file_path = _match_file_for_sample(
+                sample.sample_name, "profile.tsv", prj.results_folder, full_path=True
+            )
             if os.path.exists(profile_file_path):
-                df = _pd.read_csv(profile_file_path, sep="\t", comment="#",
-                                  names=PROFILE_COLNAMES)
-                df['runtime'] = _pd.to_timedelta(df['runtime'])
+                df = _pd.read_csv(
+                    profile_file_path, sep="\t", comment="#", names=PROFILE_COLNAMES
+                )
+                df["runtime"] = _pd.to_timedelta(df["runtime"])
                 times.append(_get_runtime(df))
                 mems.append(_get_maxmem(df))
             else:
                 _LOGGER.warning("'{}' does not exist".format(profile_file_path))
                 times.append(NO_DATA_PLACEHOLDER)
                 mems.append(NO_DATA_PLACEHOLDER)
         else:
             # Sample was not run through the pipeline
             sample_warning.append(sample_name)
 
     # Alert the user to any warnings generated
     if status_warning:
-        _LOGGER.warning("The stats table is incomplete, likely because one or "
-                        "more jobs either failed or is still running.")
+        _LOGGER.warning(
+            "The stats table is incomplete, likely because one or "
+            "more jobs either failed or is still running."
+        )
     if sample_warning:
-        _LOGGER.warning("{} samples not present in {}: {}".format(
-            len(sample_warning), prj.results_folder,
-            str([sample for sample in sample_warning])))
-    template_vars = dict(sample_link_names=sample_link_names,
-                         row_classes=row_classes, flags=flags, times=times,
-                         mems=mems)
+        _LOGGER.warning(
+            "{} samples not present in {}: {}".format(
+                len(sample_warning),
+                prj.results_folder,
+                str([sample for sample in sample_warning]),
+            )
+        )
+    template_vars = dict(
+        sample_link_names=sample_link_names,
+        row_classes=row_classes,
+        flags=flags,
+        times=times,
+        mems=mems,
+    )
     template_name = "status_table_no_links.html"
     if final:
         template_name = "status_table.html"
-        template_vars.update(dict(sample_paths=sample_paths,
-                                  log_link_names=log_link_names,
-                                  log_paths=log_paths))
+        template_vars.update(
+            dict(
+                sample_paths=sample_paths,
+                log_link_names=log_link_names,
+                log_paths=log_paths,
+            )
+        )
     return render_jinja_template(template_name, get_jinja_env(), template_vars)
 
 
 def _get_maxmem(profile_df):
     """
     Get current peak memory
 
     :param pandas.core.frame.DataFrame profile_df: a data frame representing the current profile.tsv for a sample
     :return str: max memory
     """
-    return "{} GB".format(str(max(profile_df['mem']) if not profile_df['mem'].empty else 0))
+    return "{} GB".format(
+        str(max(profile_df["mem"]) if not profile_df["mem"].empty else 0)
+    )
 
 
 def _get_runtime(profile_df):
     """
     Collect the unique and last duplicated runtimes, sum them and then return in str format
 
     :param pandas.core.frame.DataFrame profile_df: a data frame representing the current profile.tsv for a sample
     :return str: sum of runtimes
     """
-    unique_df = profile_df[~profile_df.duplicated('cid', keep='last').values]
-    return str(timedelta(seconds=sum(unique_df['runtime'].apply(lambda x: x.total_seconds())))).split(".")[0]
-
+    unique_df = profile_df[~profile_df.duplicated("cid", keep="last").values]
+    return str(
+        timedelta(seconds=sum(unique_df["runtime"].apply(lambda x: x.total_seconds())))
+    ).split(".")[0]
```

### Comparing `looper-1.3.2/looper/jinja_templates/footer_index.html` & `looper-1.4.0/looper/jinja_templates_old/footer_index.html`

 * *Files 7% similar despite different names*

```diff
@@ -48,17 +48,17 @@
       }];
       var layout = {
         title: colname
       };
       chart = document.getElementById('charts');
       Plotly.newPlot(chart, data, layout);
     }
-    
+
     function displayPlottableColumns(){
         for(var col in plotDict){
             $("#plot-cols").append("<li class='list-group-item'><a href='#' title='Click to visualize this column' onclick='graphCol(\"" + col +
                 "\");return false;'>" + col+ "</a></li>");
         }
     }
 
     displayPlottableColumns();
-</script>
+</script>
```

### Comparing `looper-1.3.2/looper/jinja_templates/head.html` & `looper-1.4.0/looper/jinja_templates_old/head.html`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -130,8 +130,8 @@
         overflow:scroll;
         -webkit-overflow-scrolling: touch;
     }
 
     div#navbar_links {
       display: flex;
     }
-</style>
+</style>
```

#### html2text {}

```diff
@@ -1,4 +1,5 @@
 
 
 
 
+
```

### Comparing `looper-1.3.2/looper/jinja_templates/index.html` & `looper-1.4.0/looper/jinja_templates_old/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -212,15 +212,15 @@
 				padding: 0.3rem !important;
 			}
 			.popover {
 				max-width: none;
 			}
 		</style>
     </head>
-    {{ navbar }} 
+    {{ navbar }}
     <body>
     	<div class="container">
   			<div class="row" style="margin-top: 20px; margin-bottom: 25px;">
 				<div class="col-10">
   					<h3 style="margin-bottom: 0px;">Looper <code>{{ project_name }}</code> summary</h3>
 				</div>
 				<div class="col-2">
```

### Comparing `looper-1.3.2/looper/jinja_templates/logo.html` & `looper-1.4.0/looper/jinja_templates/logo.html`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1 +1 @@
-<img src="data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiIHN0YW5kYWxvbmU9Im5vIj8+CjwhLS0gQ3JlYXRlZCB3aXRoIElua3NjYXBlIChodHRwOi8vd3d3Lmlua3NjYXBlLm9yZy8pIC0tPgoKPHN2ZwogICB4bWxuczpkYz0iaHR0cDovL3B1cmwub3JnL2RjL2VsZW1lbnRzLzEuMS8iCiAgIHhtbG5zOmNjPSJodHRwOi8vY3JlYXRpdmVjb21tb25zLm9yZy9ucyMiCiAgIHhtbG5zOnJkZj0iaHR0cDovL3d3dy53My5vcmcvMTk5OS8wMi8yMi1yZGYtc3ludGF4LW5zIyIKICAgeG1sbnM6c3ZnPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyIKICAgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIgogICB4bWxuczpzb2RpcG9kaT0iaHR0cDovL3NvZGlwb2RpLnNvdXJjZWZvcmdlLm5ldC9EVEQvc29kaXBvZGktMC5kdGQiCiAgIHhtbG5zOmlua3NjYXBlPSJodHRwOi8vd3d3Lmlua3NjYXBlLm9yZy9uYW1lc3BhY2VzL2lua3NjYXBlIgogICB3aWR0aD0iNjMuODg1MTM2bW0iCiAgIGhlaWdodD0iNTguNTA0NzA3bW0iCiAgIHZpZXdCb3g9IjAgMCAyMjYuMzY0NjUgMjA3LjMwMDEzIgogICBpZD0ic3ZnNDE5OCIKICAgdmVyc2lvbj0iMS4xIgogICBpbmtzY2FwZTp2ZXJzaW9uPSIwLjkxIHIxMzcyNSIKICAgc29kaXBvZGk6ZG9jbmFtZT0ibG9nb19sb29wZXIuc3ZnIj4KICA8ZGVmcwogICAgIGlkPSJkZWZzNDIwMCIgLz4KICA8c29kaXBvZGk6bmFtZWR2aWV3CiAgICAgaWQ9ImJhc2UiCiAgICAgcGFnZWNvbG9yPSIjZmZmZmZmIgogICAgIGJvcmRlcmNvbG9yPSIjNjY2NjY2IgogICAgIGJvcmRlcm9wYWNpdHk9IjEuMCIKICAgICBpbmtzY2FwZTpwYWdlb3BhY2l0eT0iMC4wIgogICAgIGlua3NjYXBlOnBhZ2VzaGFkb3c9IjIiCiAgICAgaW5rc2NhcGU6em9vbT0iMi44Mjg0MjcxIgogICAgIGlua3NjYXBlOmN4PSI4MC45NTQ1MzIiCiAgICAgaW5rc2NhcGU6Y3k9IjIyOS42MjgxOCIKICAgICBpbmtzY2FwZTpkb2N1bWVudC11bml0cz0icHgiCiAgICAgaW5rc2NhcGU6Y3VycmVudC1sYXllcj0ibGF5ZXIxIgogICAgIHNob3dncmlkPSJmYWxzZSIKICAgICBmaXQtbWFyZ2luLXRvcD0iMiIKICAgICBmaXQtbWFyZ2luLWxlZnQ9IjMiCiAgICAgZml0LW1hcmdpbi1yaWdodD0iMyIKICAgICBmaXQtbWFyZ2luLWJvdHRvbT0iMiIgLz4KICA8bWV0YWRhdGEKICAgICBpZD0ibWV0YWRhdGE0MjAzIj4KICAgIDxyZGY6UkRGPgogICAgICA8Y2M6V29yawogICAgICAgICByZGY6YWJvdXQ9IiI+CiAgICAgICAgPGRjOmZvcm1hdD5pbWFnZS9zdmcreG1sPC9kYzpmb3JtYXQ+CiAgICAgICAgPGRjOnR5cGUKICAgICAgICAgICByZGY6cmVzb3VyY2U9Imh0dHA6Ly9wdXJsLm9yZy9kYy9kY21pdHlwZS9TdGlsbEltYWdlIiAvPgogICAgICAgIDxkYzp0aXRsZT48L2RjOnRpdGxlPgogICAgICA8L2NjOldvcms+CiAgICA8L3JkZjpSREY+CiAgPC9tZXRhZGF0YT4KICA8ZwogICAgIGlua3NjYXBlOmxhYmVsPSJMYXllciAxIgogICAgIGlua3NjYXBlOmdyb3VwbW9kZT0ibGF5ZXIiCiAgICAgaWQ9ImxheWVyMSIKICAgICB0cmFuc2Zvcm09InRyYW5zbGF0ZSgtMjc4LjI0NjI0LC04NTQuNDI2NDIpIj4KICAgIDxwYXRoCiAgICAgICBzdHlsZT0iZmlsbDojNWY4ZGQzO3N0cm9rZTojZmZmZmZmO3N0cm9rZS13aWR0aDoxLjU7c3Ryb2tlLW1pdGVybGltaXQ6NDtzdHJva2UtZGFzaGFycmF5Om5vbmUiCiAgICAgICBpZD0icGF0aDQxNDYiCiAgICAgICBkPSJtIDM0NS40MjUyNCw5OTMuMDc5MDQgYyA2LjE1MSwwIDEyLjQwOCwtMS4wMTQgMTguNTM2LC0zLjE0NyBsIC00LjYwOCwtMTMuMjIxIGMgLTIyLjEyNiw3LjcwMyAtNDYuMzk5LC00LjAyMSAtNTQuMTA1LC0yNi4xNCAtNy43MTEsLTIyLjEyMDAxIDQuMDE1LC00Ni4zOTEwMSAyNi4xMzcsLTU0LjEwMzAxIDguMzI3LC0yLjkwMiAxNy4xNzcsLTMuMTM1IDI1LjUxMywtMC43NyBsIC0xNS4yNiw4LjA4MyA2LjU1NCwxMi4zNzIgMzYuNTQ4MDEsLTE5LjM2IC0yMi4yMDMwMSwtMzUuMjggLTExLjg0OSw3LjQ1NiA4LjAwMywxMi43MTkgYyAtMTAuNDg3LC0yLjU2MyAtMjEuNTA5LC0yLjA2NCAtMzEuOTE1LDEuNTYyIC0yOS40MTIsMTAuMjUzIC00NS4wMDAwMSw0Mi41MjEgLTM0Ljc0OTAxLDcxLjkzMDAxIDguMTEyMDEsMjMuMjggMzAuMDIyMDEsMzcuODk5IDUzLjM5ODAxLDM3Ljg5OSB6IgogICAgICAgaW5rc2NhcGU6Y29ubmVjdG9yLWN1cnZhdHVyZT0iMCIKICAgICAgIHNvZGlwb2RpOm5vZGV0eXBlcz0ic2NjY2NjY2NjY2NjY2NzIiAvPgogICAgPHJlY3QKICAgICAgIHN0eWxlPSJjb2xvcjojMDAwMDAwO2NsaXAtcnVsZTpub256ZXJvO2Rpc3BsYXk6aW5saW5lO292ZXJmbG93OnZpc2libGU7dmlzaWJpbGl0eTp2aXNpYmxlO29wYWNpdHk6MTtpc29sYXRpb246YXV0bzttaXgtYmxlbmQtbW9kZTpub3JtYWw7Y29sb3ItaW50ZXJwb2xhdGlvbjpzUkdCO2NvbG9yLWludGVycG9sYXRpb24tZmlsdGVyczpsaW5lYXJSR0I7c29saWQtY29sb3I6IzAwMDAwMDtzb2xpZC1vcGFjaXR5OjE7ZmlsbDojNWY4ZGQzO2ZpbGwtb3BhY2l0eToxO2ZpbGwtcnVsZTpub256ZXJvO3N0cm9rZTojZmZmZmZmO3N0cm9rZS13aWR0aDoxLjU7c3Ryb2tlLWxpbmVjYXA6YnV0dDtzdHJva2UtbGluZWpvaW46bWl0ZXI7c3Ryb2tlLW1pdGVybGltaXQ6NDtzdHJva2UtZGFzaGFycmF5Om5vbmU7c3Ryb2tlLWRhc2hvZmZzZXQ6MDtzdHJva2Utb3BhY2l0eToxO21hcmtlcjpub25lO2NvbG9yLXJlbmRlcmluZzphdXRvO2ltYWdlLXJlbmRlcmluZzphdXRvO3NoYXBlLXJlbmRlcmluZzphdXRvO3RleHQtcmVuZGVyaW5nOmF1dG87ZW5hYmxlLWJhY2tncm91bmQ6YWNjdW11bGF0ZSIKICAgICAgIGlkPSJyZWN0NDE1NyIKICAgICAgIHdpZHRoPSI0NC4wMzc0NDkiCiAgICAgICBoZWlnaHQ9IjExLjAwOTgxMiIKICAgICAgIHg9IjMyNC4xMTgxIgogICAgICAgeT0iOTIyLjc4NjMyIiAvPgogICAgPHJlY3QKICAgICAgIHk9IjkzOS41NTQyNiIKICAgICAgIHg9IjMyNC4xMTgxIgogICAgICAgaGVpZ2h0PSIxMS4wMDk4MTIiCiAgICAgICB3aWR0aD0iNDQuMDM3NDQ5IgogICAgICAgaWQ9InJlY3Q0MTU5IgogICAgICAgc3R5bGU9ImNvbG9yOiMwMDAwMDA7Y2xpcC1ydWxlOm5vbnplcm87ZGlzcGxheTppbmxpbmU7b3ZlcmZsb3c6dmlzaWJsZTt2aXNpYmlsaXR5OnZpc2libGU7b3BhY2l0eToxO2lzb2xhdGlvbjphdXRvO21peC1ibGVuZC1tb2RlOm5vcm1hbDtjb2xvci1pbnRlcnBvbGF0aW9uOnNSR0I7Y29sb3ItaW50ZXJwb2xhdGlvbi1maWx0ZXJzOmxpbmVhclJHQjtzb2xpZC1jb2xvcjojMDAwMDAwO3NvbGlkLW9wYWNpdHk6MTtmaWxsOiM1ZjhkZDM7ZmlsbC1vcGFjaXR5OjE7ZmlsbC1ydWxlOm5vbnplcm87c3Ryb2tlOiNmZmZmZmY7c3Ryb2tlLXdpZHRoOjEuNTtzdHJva2UtbGluZWNhcDpidXR0O3N0cm9rZS1saW5lam9pbjptaXRlcjtzdHJva2UtbWl0ZXJsaW1pdDo0O3N0cm9rZS1kYXNoYXJyYXk6bm9uZTtzdHJva2UtZGFzaG9mZnNldDowO3N0cm9rZS1vcGFjaXR5OjE7bWFya2VyOm5vbmU7Y29sb3ItcmVuZGVyaW5nOmF1dG87aW1hZ2UtcmVuZGVyaW5nOmF1dG87c2hhcGUtcmVuZGVyaW5nOmF1dG87dGV4dC1yZW5kZXJpbmc6YXV0bztlbmFibGUtYmFja2dyb3VuZDphY2N1bXVsYXRlIiAvPgogICAgPHJlY3QKICAgICAgIHN0eWxlPSJjb2xvcjojMDAwMDAwO2NsaXAtcnVsZTpub256ZXJvO2Rpc3BsYXk6aW5saW5lO292ZXJmbG93OnZpc2libGU7dmlzaWJpbGl0eTp2aXNpYmxlO29wYWNpdHk6MTtpc29sYXRpb246YXV0bzttaXgtYmxlbmQtbW9kZTpub3JtYWw7Y29sb3ItaW50ZXJwb2xhdGlvbjpzUkdCO2NvbG9yLWludGVycG9sYXRpb24tZmlsdGVyczpsaW5lYXJSR0I7c29saWQtY29sb3I6IzAwMDAwMDtzb2xpZC1vcGFjaXR5OjE7ZmlsbDojNWY4ZGQzO2ZpbGwtb3BhY2l0eToxO2ZpbGwtcnVsZTpub256ZXJvO3N0cm9rZTojZmZmZmZmO3N0cm9rZS13aWR0aDoxLjU7c3Ryb2tlLWxpbmVjYXA6YnV0dDtzdHJva2UtbGluZWpvaW46bWl0ZXI7c3Ryb2tlLW1pdGVybGltaXQ6NDtzdHJva2UtZGFzaGFycmF5Om5vbmU7c3Ryb2tlLWRhc2hvZmZzZXQ6MDtzdHJva2Utb3BhY2l0eToxO21hcmtlcjpub25lO2NvbG9yLXJlbmRlcmluZzphdXRvO2ltYWdlLXJlbmRlcmluZzphdXRvO3NoYXBlLXJlbmRlcmluZzphdXRvO3RleHQtcmVuZGVyaW5nOmF1dG87ZW5hYmxlLWJhY2tncm91bmQ6YWNjdW11bGF0ZSIKICAgICAgIGlkPSJyZWN0NDE2MSIKICAgICAgIHdpZHRoPSI0NC4wMzc0NDkiCiAgICAgICBoZWlnaHQ9IjExLjAwOTgxMiIKICAgICAgIHg9IjMyNC4xMTgxIgogICAgICAgeT0iOTU2LjMyMjIiIC8+CiAgICA8cGF0aAogICAgICAgc3R5bGU9ImZpbGw6IzVmOGRkMztzdHJva2U6I2ZmZmZmZjtzdHJva2Utd2lkdGg6MS41O3N0cm9rZS1taXRlcmxpbWl0OjQ7c3Ryb2tlLWRhc2hhcnJheTpub25lIgogICAgICAgaWQ9InBhdGg0MTY3IgogICAgICAgZD0ibSA0OTIuMDAzODQsMTAzMi41MjM2IGMgLTQuMDAwMjYsLTguNjkwMiAtOC45MjAxMSwtMjIuODA2MSAtOS43MDE3NywtMzMuOTMzMjMgbCAtMC41MDU3OCwtNy4wODA5MSAtNy44NjI1OCwxNi43ODI2NCAtMTcuMTA0NTQsLTE3LjEwNDUgOS4wODA5MSwwIGMgNi41NzUxNCwwIDExLjk1NDc5LC01LjM3OTY2IDExLjk1NDc5LC0xMS45NTQ3OSBsIDAsLTU5LjYxNDQ0IGMgMCwtNi41NzUxMyAtNS4zNzk2NSwtMTEuOTU0NzkgLTExLjk1NDc5LC0xMS45NTQ3OSBsIC03Ni45Mjg4NCwwIGMgLTYuNTc1MTMsMCAtMTEuOTU0NzksNS4zNzk2NiAtMTEuOTU0NzksMTEuOTU0NzkgbCAwLDU5LjYxNDQ0IGMgMCw2LjU3NTEzIDUuMzc5NjYsMTEuOTU0NzkgMTEuOTU0NzksMTEuOTU0NzkgbCAzLjMxMDU2LDAgLTE3LjEwNDU0LDE3LjEwNDUgLTcuODYyNTgsLTE2Ljc4MjY0IC0wLjUwNTc4LDcuMDgwOTEgYyAtMC43ODE2NiwxMS4xMjcxMyAtNS43MDE1MiwyNS4yNDMwMyAtOS43MDE3NywzMy45MzMyMyBsIC0yLjA2OTEsNC41MDYgNC41MDYwNCwtMi4wNjkxIGMgOC42OTAyMSwtNC4wMDAyIDIyLjgwNjA2LC04LjkyMDEgMzMuOTMzMjEsLTkuNzAxNyBsIDcuMDgwOTEsLTAuNTA1OCAtMTYuNzgyNjgsLTcuODYyNiAyNS4yNDMsLTI1LjI0MyBjIDAuMTM3OTQsLTAuMTM3OTQgMC4yNzU4OCwtMC4zMjE4NiAwLjQxMzgyLC0wLjUwNTc4IGwgOS4xNTIzMiwwIDAsMjguOTY3MzggLTE3LjQyNjQsLTYuMjk5MyA0LjY4OTk1LDUuMzMzNyBjIDcuMzEwODIsOC40MTQzIDEzLjc5Mzk5LDIxLjg0MDUgMTcuMTUwNTMsMzAuODUyNiBsIDEuNzQ3MjQsNC42NDM5IDEuNzAxMjYsLTQuNjQzOSBjIDMuMzEwNTUsLTguOTY2MSA5Ljc5MzczLC0yMi40MzgzIDE3LjE1MDUyLC0zMC44NTI2IGwgNC42ODk5NiwtNS4zMzM3IC0xNy40MjY0MSw2LjI5OTMgMCwtMjguOTY3MzggOC43MTUzOCwwIGMgMC4xMzc5NCwwLjE4MzkyIDAuMjc1ODgsMC4zMjE4NiAwLjQxMzgyLDAuNTA1NzggbCAyNS4yNDMsMjUuMjQzIC0xNi43ODI2OSw3Ljg2MjYgNy4wODA5MiwwLjUwNTggYyAxMS4xMjcxNSwwLjc4MTYgMjUuMjQzLDUuNzAxNSAzMy45MzMyMSw5LjcwMTcgbCA0LjUwNjA0LDIuMDY5MSB6IG0gLTEwMi4xMDMsLTExMS45ODU2MyA3NS4xMzU2MiwwIDAsNTcuNzc1MjQgLTc1LjEzNTYyLDAgeiIKICAgICAgIGlua3NjYXBlOmNvbm5lY3Rvci1jdXJ2YXR1cmU9IjAiCiAgICAgICBzb2RpcG9kaTpub2RldHlwZXM9ImNjY2Njc3Nzc3Nzc3NjY2NjY2NjY2Njc2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2MiIC8+CiAgPC9nPgo8L3N2Zz4K" class="d-inline-block align-middle img-responsive" alt="LOOPER" height="60">
+<img src="data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiIHN0YW5kYWxvbmU9Im5vIj8+CjwhLS0gQ3JlYXRlZCB3aXRoIElua3NjYXBlIChodHRwOi8vd3d3Lmlua3NjYXBlLm9yZy8pIC0tPgoKPHN2ZwogICB4bWxuczpkYz0iaHR0cDovL3B1cmwub3JnL2RjL2VsZW1lbnRzLzEuMS8iCiAgIHhtbG5zOmNjPSJodHRwOi8vY3JlYXRpdmVjb21tb25zLm9yZy9ucyMiCiAgIHhtbG5zOnJkZj0iaHR0cDovL3d3dy53My5vcmcvMTk5OS8wMi8yMi1yZGYtc3ludGF4LW5zIyIKICAgeG1sbnM6c3ZnPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyIKICAgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIgogICB4bWxuczpzb2RpcG9kaT0iaHR0cDovL3NvZGlwb2RpLnNvdXJjZWZvcmdlLm5ldC9EVEQvc29kaXBvZGktMC5kdGQiCiAgIHhtbG5zOmlua3NjYXBlPSJodHRwOi8vd3d3Lmlua3NjYXBlLm9yZy9uYW1lc3BhY2VzL2lua3NjYXBlIgogICB3aWR0aD0iNjMuODg1MTM2bW0iCiAgIGhlaWdodD0iNTguNTA0NzA3bW0iCiAgIHZpZXdCb3g9IjAgMCAyMjYuMzY0NjUgMjA3LjMwMDEzIgogICBpZD0ic3ZnNDE5OCIKICAgdmVyc2lvbj0iMS4xIgogICBpbmtzY2FwZTp2ZXJzaW9uPSIwLjkxIHIxMzcyNSIKICAgc29kaXBvZGk6ZG9jbmFtZT0ibG9nb19sb29wZXIuc3ZnIj4KICA8ZGVmcwogICAgIGlkPSJkZWZzNDIwMCIgLz4KICA8c29kaXBvZGk6bmFtZWR2aWV3CiAgICAgaWQ9ImJhc2UiCiAgICAgcGFnZWNvbG9yPSIjZmZmZmZmIgogICAgIGJvcmRlcmNvbG9yPSIjNjY2NjY2IgogICAgIGJvcmRlcm9wYWNpdHk9IjEuMCIKICAgICBpbmtzY2FwZTpwYWdlb3BhY2l0eT0iMC4wIgogICAgIGlua3NjYXBlOnBhZ2VzaGFkb3c9IjIiCiAgICAgaW5rc2NhcGU6em9vbT0iMi44Mjg0MjcxIgogICAgIGlua3NjYXBlOmN4PSI4MC45NTQ1MzIiCiAgICAgaW5rc2NhcGU6Y3k9IjIyOS42MjgxOCIKICAgICBpbmtzY2FwZTpkb2N1bWVudC11bml0cz0icHgiCiAgICAgaW5rc2NhcGU6Y3VycmVudC1sYXllcj0ibGF5ZXIxIgogICAgIHNob3dncmlkPSJmYWxzZSIKICAgICBmaXQtbWFyZ2luLXRvcD0iMiIKICAgICBmaXQtbWFyZ2luLWxlZnQ9IjMiCiAgICAgZml0LW1hcmdpbi1yaWdodD0iMyIKICAgICBmaXQtbWFyZ2luLWJvdHRvbT0iMiIgLz4KICA8bWV0YWRhdGEKICAgICBpZD0ibWV0YWRhdGE0MjAzIj4KICAgIDxyZGY6UkRGPgogICAgICA8Y2M6V29yawogICAgICAgICByZGY6YWJvdXQ9IiI+CiAgICAgICAgPGRjOmZvcm1hdD5pbWFnZS9zdmcreG1sPC9kYzpmb3JtYXQ+CiAgICAgICAgPGRjOnR5cGUKICAgICAgICAgICByZGY6cmVzb3VyY2U9Imh0dHA6Ly9wdXJsLm9yZy9kYy9kY21pdHlwZS9TdGlsbEltYWdlIiAvPgogICAgICAgIDxkYzp0aXRsZT48L2RjOnRpdGxlPgogICAgICA8L2NjOldvcms+CiAgICA8L3JkZjpSREY+CiAgPC9tZXRhZGF0YT4KICA8ZwogICAgIGlua3NjYXBlOmxhYmVsPSJMYXllciAxIgogICAgIGlua3NjYXBlOmdyb3VwbW9kZT0ibGF5ZXIiCiAgICAgaWQ9ImxheWVyMSIKICAgICB0cmFuc2Zvcm09InRyYW5zbGF0ZSgtMjc4LjI0NjI0LC04NTQuNDI2NDIpIj4KICAgIDxwYXRoCiAgICAgICBzdHlsZT0iZmlsbDojNWY4ZGQzO3N0cm9rZTojZmZmZmZmO3N0cm9rZS13aWR0aDoxLjU7c3Ryb2tlLW1pdGVybGltaXQ6NDtzdHJva2UtZGFzaGFycmF5Om5vbmUiCiAgICAgICBpZD0icGF0aDQxNDYiCiAgICAgICBkPSJtIDM0NS40MjUyNCw5OTMuMDc5MDQgYyA2LjE1MSwwIDEyLjQwOCwtMS4wMTQgMTguNTM2LC0zLjE0NyBsIC00LjYwOCwtMTMuMjIxIGMgLTIyLjEyNiw3LjcwMyAtNDYuMzk5LC00LjAyMSAtNTQuMTA1LC0yNi4xNCAtNy43MTEsLTIyLjEyMDAxIDQuMDE1LC00Ni4zOTEwMSAyNi4xMzcsLTU0LjEwMzAxIDguMzI3LC0yLjkwMiAxNy4xNzcsLTMuMTM1IDI1LjUxMywtMC43NyBsIC0xNS4yNiw4LjA4MyA2LjU1NCwxMi4zNzIgMzYuNTQ4MDEsLTE5LjM2IC0yMi4yMDMwMSwtMzUuMjggLTExLjg0OSw3LjQ1NiA4LjAwMywxMi43MTkgYyAtMTAuNDg3LC0yLjU2MyAtMjEuNTA5LC0yLjA2NCAtMzEuOTE1LDEuNTYyIC0yOS40MTIsMTAuMjUzIC00NS4wMDAwMSw0Mi41MjEgLTM0Ljc0OTAxLDcxLjkzMDAxIDguMTEyMDEsMjMuMjggMzAuMDIyMDEsMzcuODk5IDUzLjM5ODAxLDM3Ljg5OSB6IgogICAgICAgaW5rc2NhcGU6Y29ubmVjdG9yLWN1cnZhdHVyZT0iMCIKICAgICAgIHNvZGlwb2RpOm5vZGV0eXBlcz0ic2NjY2NjY2NjY2NjY2NzIiAvPgogICAgPHJlY3QKICAgICAgIHN0eWxlPSJjb2xvcjojMDAwMDAwO2NsaXAtcnVsZTpub256ZXJvO2Rpc3BsYXk6aW5saW5lO292ZXJmbG93OnZpc2libGU7dmlzaWJpbGl0eTp2aXNpYmxlO29wYWNpdHk6MTtpc29sYXRpb246YXV0bzttaXgtYmxlbmQtbW9kZTpub3JtYWw7Y29sb3ItaW50ZXJwb2xhdGlvbjpzUkdCO2NvbG9yLWludGVycG9sYXRpb24tZmlsdGVyczpsaW5lYXJSR0I7c29saWQtY29sb3I6IzAwMDAwMDtzb2xpZC1vcGFjaXR5OjE7ZmlsbDojNWY4ZGQzO2ZpbGwtb3BhY2l0eToxO2ZpbGwtcnVsZTpub256ZXJvO3N0cm9rZTojZmZmZmZmO3N0cm9rZS13aWR0aDoxLjU7c3Ryb2tlLWxpbmVjYXA6YnV0dDtzdHJva2UtbGluZWpvaW46bWl0ZXI7c3Ryb2tlLW1pdGVybGltaXQ6NDtzdHJva2UtZGFzaGFycmF5Om5vbmU7c3Ryb2tlLWRhc2hvZmZzZXQ6MDtzdHJva2Utb3BhY2l0eToxO21hcmtlcjpub25lO2NvbG9yLXJlbmRlcmluZzphdXRvO2ltYWdlLXJlbmRlcmluZzphdXRvO3NoYXBlLXJlbmRlcmluZzphdXRvO3RleHQtcmVuZGVyaW5nOmF1dG87ZW5hYmxlLWJhY2tncm91bmQ6YWNjdW11bGF0ZSIKICAgICAgIGlkPSJyZWN0NDE1NyIKICAgICAgIHdpZHRoPSI0NC4wMzc0NDkiCiAgICAgICBoZWlnaHQ9IjExLjAwOTgxMiIKICAgICAgIHg9IjMyNC4xMTgxIgogICAgICAgeT0iOTIyLjc4NjMyIiAvPgogICAgPHJlY3QKICAgICAgIHk9IjkzOS41NTQyNiIKICAgICAgIHg9IjMyNC4xMTgxIgogICAgICAgaGVpZ2h0PSIxMS4wMDk4MTIiCiAgICAgICB3aWR0aD0iNDQuMDM3NDQ5IgogICAgICAgaWQ9InJlY3Q0MTU5IgogICAgICAgc3R5bGU9ImNvbG9yOiMwMDAwMDA7Y2xpcC1ydWxlOm5vbnplcm87ZGlzcGxheTppbmxpbmU7b3ZlcmZsb3c6dmlzaWJsZTt2aXNpYmlsaXR5OnZpc2libGU7b3BhY2l0eToxO2lzb2xhdGlvbjphdXRvO21peC1ibGVuZC1tb2RlOm5vcm1hbDtjb2xvci1pbnRlcnBvbGF0aW9uOnNSR0I7Y29sb3ItaW50ZXJwb2xhdGlvbi1maWx0ZXJzOmxpbmVhclJHQjtzb2xpZC1jb2xvcjojMDAwMDAwO3NvbGlkLW9wYWNpdHk6MTtmaWxsOiM1ZjhkZDM7ZmlsbC1vcGFjaXR5OjE7ZmlsbC1ydWxlOm5vbnplcm87c3Ryb2tlOiNmZmZmZmY7c3Ryb2tlLXdpZHRoOjEuNTtzdHJva2UtbGluZWNhcDpidXR0O3N0cm9rZS1saW5lam9pbjptaXRlcjtzdHJva2UtbWl0ZXJsaW1pdDo0O3N0cm9rZS1kYXNoYXJyYXk6bm9uZTtzdHJva2UtZGFzaG9mZnNldDowO3N0cm9rZS1vcGFjaXR5OjE7bWFya2VyOm5vbmU7Y29sb3ItcmVuZGVyaW5nOmF1dG87aW1hZ2UtcmVuZGVyaW5nOmF1dG87c2hhcGUtcmVuZGVyaW5nOmF1dG87dGV4dC1yZW5kZXJpbmc6YXV0bztlbmFibGUtYmFja2dyb3VuZDphY2N1bXVsYXRlIiAvPgogICAgPHJlY3QKICAgICAgIHN0eWxlPSJjb2xvcjojMDAwMDAwO2NsaXAtcnVsZTpub256ZXJvO2Rpc3BsYXk6aW5saW5lO292ZXJmbG93OnZpc2libGU7dmlzaWJpbGl0eTp2aXNpYmxlO29wYWNpdHk6MTtpc29sYXRpb246YXV0bzttaXgtYmxlbmQtbW9kZTpub3JtYWw7Y29sb3ItaW50ZXJwb2xhdGlvbjpzUkdCO2NvbG9yLWludGVycG9sYXRpb24tZmlsdGVyczpsaW5lYXJSR0I7c29saWQtY29sb3I6IzAwMDAwMDtzb2xpZC1vcGFjaXR5OjE7ZmlsbDojNWY4ZGQzO2ZpbGwtb3BhY2l0eToxO2ZpbGwtcnVsZTpub256ZXJvO3N0cm9rZTojZmZmZmZmO3N0cm9rZS13aWR0aDoxLjU7c3Ryb2tlLWxpbmVjYXA6YnV0dDtzdHJva2UtbGluZWpvaW46bWl0ZXI7c3Ryb2tlLW1pdGVybGltaXQ6NDtzdHJva2UtZGFzaGFycmF5Om5vbmU7c3Ryb2tlLWRhc2hvZmZzZXQ6MDtzdHJva2Utb3BhY2l0eToxO21hcmtlcjpub25lO2NvbG9yLXJlbmRlcmluZzphdXRvO2ltYWdlLXJlbmRlcmluZzphdXRvO3NoYXBlLXJlbmRlcmluZzphdXRvO3RleHQtcmVuZGVyaW5nOmF1dG87ZW5hYmxlLWJhY2tncm91bmQ6YWNjdW11bGF0ZSIKICAgICAgIGlkPSJyZWN0NDE2MSIKICAgICAgIHdpZHRoPSI0NC4wMzc0NDkiCiAgICAgICBoZWlnaHQ9IjExLjAwOTgxMiIKICAgICAgIHg9IjMyNC4xMTgxIgogICAgICAgeT0iOTU2LjMyMjIiIC8+CiAgICA8cGF0aAogICAgICAgc3R5bGU9ImZpbGw6IzVmOGRkMztzdHJva2U6I2ZmZmZmZjtzdHJva2Utd2lkdGg6MS41O3N0cm9rZS1taXRlcmxpbWl0OjQ7c3Ryb2tlLWRhc2hhcnJheTpub25lIgogICAgICAgaWQ9InBhdGg0MTY3IgogICAgICAgZD0ibSA0OTIuMDAzODQsMTAzMi41MjM2IGMgLTQuMDAwMjYsLTguNjkwMiAtOC45MjAxMSwtMjIuODA2MSAtOS43MDE3NywtMzMuOTMzMjMgbCAtMC41MDU3OCwtNy4wODA5MSAtNy44NjI1OCwxNi43ODI2NCAtMTcuMTA0NTQsLTE3LjEwNDUgOS4wODA5MSwwIGMgNi41NzUxNCwwIDExLjk1NDc5LC01LjM3OTY2IDExLjk1NDc5LC0xMS45NTQ3OSBsIDAsLTU5LjYxNDQ0IGMgMCwtNi41NzUxMyAtNS4zNzk2NSwtMTEuOTU0NzkgLTExLjk1NDc5LC0xMS45NTQ3OSBsIC03Ni45Mjg4NCwwIGMgLTYuNTc1MTMsMCAtMTEuOTU0NzksNS4zNzk2NiAtMTEuOTU0NzksMTEuOTU0NzkgbCAwLDU5LjYxNDQ0IGMgMCw2LjU3NTEzIDUuMzc5NjYsMTEuOTU0NzkgMTEuOTU0NzksMTEuOTU0NzkgbCAzLjMxMDU2LDAgLTE3LjEwNDU0LDE3LjEwNDUgLTcuODYyNTgsLTE2Ljc4MjY0IC0wLjUwNTc4LDcuMDgwOTEgYyAtMC43ODE2NiwxMS4xMjcxMyAtNS43MDE1MiwyNS4yNDMwMyAtOS43MDE3NywzMy45MzMyMyBsIC0yLjA2OTEsNC41MDYgNC41MDYwNCwtMi4wNjkxIGMgOC42OTAyMSwtNC4wMDAyIDIyLjgwNjA2LC04LjkyMDEgMzMuOTMzMjEsLTkuNzAxNyBsIDcuMDgwOTEsLTAuNTA1OCAtMTYuNzgyNjgsLTcuODYyNiAyNS4yNDMsLTI1LjI0MyBjIDAuMTM3OTQsLTAuMTM3OTQgMC4yNzU4OCwtMC4zMjE4NiAwLjQxMzgyLC0wLjUwNTc4IGwgOS4xNTIzMiwwIDAsMjguOTY3MzggLTE3LjQyNjQsLTYuMjk5MyA0LjY4OTk1LDUuMzMzNyBjIDcuMzEwODIsOC40MTQzIDEzLjc5Mzk5LDIxLjg0MDUgMTcuMTUwNTMsMzAuODUyNiBsIDEuNzQ3MjQsNC42NDM5IDEuNzAxMjYsLTQuNjQzOSBjIDMuMzEwNTUsLTguOTY2MSA5Ljc5MzczLC0yMi40MzgzIDE3LjE1MDUyLC0zMC44NTI2IGwgNC42ODk5NiwtNS4zMzM3IC0xNy40MjY0MSw2LjI5OTMgMCwtMjguOTY3MzggOC43MTUzOCwwIGMgMC4xMzc5NCwwLjE4MzkyIDAuMjc1ODgsMC4zMjE4NiAwLjQxMzgyLDAuNTA1NzggbCAyNS4yNDMsMjUuMjQzIC0xNi43ODI2OSw3Ljg2MjYgNy4wODA5MiwwLjUwNTggYyAxMS4xMjcxNSwwLjc4MTYgMjUuMjQzLDUuNzAxNSAzMy45MzMyMSw5LjcwMTcgbCA0LjUwNjA0LDIuMDY5MSB6IG0gLTEwMi4xMDMsLTExMS45ODU2MyA3NS4xMzU2MiwwIDAsNTcuNzc1MjQgLTc1LjEzNTYyLDAgeiIKICAgICAgIGlua3NjYXBlOmNvbm5lY3Rvci1jdXJ2YXR1cmU9IjAiCiAgICAgICBzb2RpcG9kaTpub2RldHlwZXM9ImNjY2Njc3Nzc3Nzc3NjY2NjY2NjY2Njc2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2MiIC8+CiAgPC9nPgo8L3N2Zz4K" class="d-inline-block align-middle img-responsive" alt="LOOPER" height="60">
```

### Comparing `looper-1.3.2/looper/jinja_templates/navbar.html` & `looper-1.4.0/looper/jinja_templates_old/navbar.html`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,7 @@
               <li class="nav-item active">
                 <a class="nav-link" href="{{index_html}}">Summary<span class="sr-only">(current)</span></a>
               </li>
               {{ navbar_links }}
             </ul>
           </div>
         </nav>
-
```

### Comparing `looper-1.3.2/looper/jinja_templates/navbar_links.html` & `looper-1.4.0/looper/jinja_templates_old/navbar_links.html`

 * *Files 0% similar despite different names*

```diff
@@ -7,19 +7,19 @@
               {% if dropdown_keys_objects is none %}
               <!-- there is more than 20 objects or 0 -->
                 {% if objects_html_page is none %}
                 <!-- no objects at all -->
                   <li class="nav-item">
                     <!-- intentionally no href attribute, inactive link -->
                     <a class="nav-link disabled">{{objects_page_name}}</a>
-                  </li> 
+                  </li>
                 {% else %}
                   <li class="nav-item active">
                     <a class="nav-link" href="{{objects_html_page}}">{{objects_page_name}}</a>
-                  </li>  
+                  </li>
                 {% endif %}
               {% else %}
                <!-- there is less than 20 objects -->
                 <li class="nav-item dropdown active">
                   <a class="nav-link dropdown-toggle active" href="#" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                     {{ menu_name_objects }}
                   </a>
@@ -41,15 +41,15 @@
                     <!-- intentionally no href attribute, inactive link -->
                     <a class="nav-link disabled">{{samples_page_name}}</a>
                   </li>
                 {% else %}
                   <li class="nav-item active">
                     <a class="nav-link" href="{{samples_html_page}}">{{samples_page_name}}</a>
                   </li>
-                {% endif %}  
+                {% endif %}
               {% else %}
                 <!-- there is less than 20 samples -->
                 <li class="nav-item dropdown active">
                   <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                   {{menu_name_samples}}
                   </a>
                   <div class="dropdown-menu" aria-labelledby="navbarDropdown">
@@ -57,8 +57,8 @@
                     <div class="dropdown-divider"></div>
                     {% for sample_name in sample_names %}
                       {% set i = loop.index - 1 %}
                       <a class="dropdown-item" href="{{ samples_html_page[i] }}">{{ sample_name }}</a>
                     {% endfor %}
                   </div>
                 </li>
-              {% endif %}
+              {% endif %}
```

### Comparing `looper-1.3.2/looper/jinja_templates/navbar_list_parent.html` & `looper-1.4.0/looper/jinja_templates_old/navbar_list_parent.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html lang="en">
     <head>
       {% include "head.html" %}
       <title>Looper: {{ header }}</title>
     </head>
-    {{ navbar }}    
+    {{ navbar }}
     <body>
       <div id="top"></div>
       <div class="container" style="margin-top:20px">
             <h4>{{ header }}</h4>
             <div class="list-group" style="display:inline-block">
                 {% for label in labels %}
                     {% set i = loop.index - 1 %}
@@ -17,8 +17,8 @@
             </div>
       </div>
     </body>
     <hr class="featurette-divider">
     <footer class="text-muted">
         {{ footer }}
     </footer>
-</html>
+</html>
```

### Comparing `looper-1.3.2/looper/jinja_templates/object.html` & `looper-1.4.0/looper/jinja_templates_old/object.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html lang="en">
     <head>
       {% include "head.html" %}
       <title>Looper: {{ name }} objects</title>
     </head>
-    {{ navbar }} 
+    {{ navbar }}
     <body>
     	<div id="top"></div>
     	<div class="container">
 			{% if links[0] is defined or figures[0] is defined %}
 				<h3>{{ name }}</h3>
 			{% else %}
 				<p><b>No objects to display for: <code>{{ name }}</code></b><p>
@@ -40,8 +40,8 @@
 			{% endif %}
     	</div>
     </body>
     <hr class="featurette-divider">
     <footer class="text-muted">
         {{ footer }}
     </footer>
-</html>
+</html>
```

### Comparing `looper-1.3.2/looper/jinja_templates/project_object.html` & `looper-1.4.0/looper/jinja_templates_old/project_object.html`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -42,8 +42,8 @@
 						<div class="list-group" style="display:inline-block">
 							{% for link in links %}
 								<a href='{{ link[1] }}' class="list-group-item">{{ link[0] }}</a>
 							{% endfor %}
 						</div>
 					</div>
 				</div>
-        	{% endif %}
+        	{% endif %}
```

### Comparing `looper-1.3.2/looper/jinja_templates/sample.html` & `looper-1.4.0/looper/jinja_templates_old/sample.html`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
             $.noConflict();
             jQuery(function ($) {
                 $('[data-toggle="popover"]').popover();
             });
         </script>
         <title>Looper: {{ sample_name }}</title>
     </head>
-    {{ navbar }} 
+    {{ navbar }}
     <body>
     	<div class="container">
             <div class="container-fluid">
         	   <h3>Sample name: <code>{{ sample_name }}</code></h3>
             </div>
             <div class="container-fluid">
                 <p class="text-left">
@@ -41,15 +41,15 @@
                 {% endif %}
                 </p>
             </div>
             <hr>
             <div class='container-fluid'>
     	      	<h3>Looper stats summary</h3>
     	        <div class="table-responsive-sm">
-    				<table class="table table-sm table-hover table-bordered table-condensed" style="white-space: nowrap; width: 1%;">             
+    				<table class="table table-sm table-hover table-bordered table-condensed" style="white-space: nowrap; width: 1%;">
     					<tbody>
     						{% for row_name, row_value in sample_stats.items() %}
     							<tr>
     								<th>{{ row_name }}</th>
                                     {% if row_value|length > 60 %}
     								    <td class="text">{{ row_value|truncate(60,True) }} <a data-html="true" data-toggle="popover" data-placement="top" data-trigger="click" data-content="{{ row_value }}" href="javascript:void(0)"><i class="fa fa-caret-square-o-right" aria-hidden="true"></i></a></td>
                                     {% else %}
@@ -92,8 +92,8 @@
         	</div>
         </div>
     </body>
     <hr class="featurette-divider">
     <footer class="text-muted">
         {{ footer }}
     </footer>
-</html>
+</html>
```

### Comparing `looper-1.3.2/looper/jinja_templates/status_table.html` & `looper-1.4.0/looper/jinja_templates_old/status_table.html`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -46,8 +46,8 @@
         </div>
     </div>
     <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.6/umd/popper.min.js" integrity="sha384-wHAiFfRlMFy6i5SRaxvfOCifBUQy1xHdJ/yoi7FRNXMRBu5WHdZYu1hA6ZOblgut" crossorigin="anonymous"></script>
     <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/js/bootstrap.min.js" integrity="sha384-ChfqqxuZUCnJSK3+MXmPNIyE6ZbWh2IMqE241rYiqJxyMiZ6OW/JmZQ5stwEULTy" crossorigin="anonymous"></script>
     <link href="https://unpkg.com/bootstrap-table@1.15.3/dist/bootstrap-table.min.css" rel="stylesheet">
     <link href="https://unpkg.com/bootstrap-table@1.15.3/dist/extensions/fixed-columns/bootstrap-table-fixed-columns.css" rel="stylesheet">
     <script src="https://unpkg.com/bootstrap-table@1.15.3/dist/bootstrap-table.min.js"></script>
-    <script src="https://unpkg.com/bootstrap-table@1.15.3/dist/extensions/fixed-columns/bootstrap-table-fixed-columns.js"></script>
+    <script src="https://unpkg.com/bootstrap-table@1.15.3/dist/extensions/fixed-columns/bootstrap-table-fixed-columns.js"></script>
```

#### html2text {}

```diff
@@ -2,7 +2,8 @@
                                                       use
 {                                      {
 {                 {{ flags[i] NA       {              {{ times[i] {{ mems[i] }}
 sample_link_names }}                   log_link_names }}
 [i]_}}                                 [i]_}}
 
 
+
```

### Comparing `looper-1.3.2/looper/jinja_templates/status_table_no_links.html` & `looper-1.4.0/looper/jinja_templates/status_table_no_links.html`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -51,8 +51,8 @@
         padding-right: 10px !important;
     }
 </style>
 <script src="http://code.jquery.com/jquery-latest.min.js" type="text/javascript"></script>
 <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.6/umd/popper.min.js" integrity="sha384-wHAiFfRlMFy6i5SRaxvfOCifBUQy1xHdJ/yoi7FRNXMRBu5WHdZYu1hA6ZOblgut" crossorigin="anonymous"></script>
 <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/js/bootstrap.min.js" integrity="sha384-ChfqqxuZUCnJSK3+MXmPNIyE6ZbWh2IMqE241rYiqJxyMiZ6OW/JmZQ5stwEULTy" crossorigin="anonymous"></script>
 <link href="https://unpkg.com/bootstrap-table@1.15.3/dist/bootstrap-table.min.css" rel="stylesheet">
-<script src="https://unpkg.com/bootstrap-table@1.15.3/dist/bootstrap-table.min.js"></script>
+<script src="https://unpkg.com/bootstrap-table@1.15.3/dist/bootstrap-table.min.js"></script>
```

#### html2text {}

```diff
@@ -1,3 +1,4 @@
 Sample name                Status         Runtime        Peak memory use
 {{ sample_link_names[i] }} {{ flags[i] }} {{ times[i] }} {{ mems[i] }}
 
+
```

### Comparing `looper-1.3.2/looper/looper.py` & `looper-1.4.0/looper/project.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,773 +1,786 @@
-#!/usr/bin/env python
-"""
-Looper: a pipeline submission engine. https://github.com/pepkit/looper
-"""
-
-import abc
-import csv
-import glob
-import logging
+""" Looper version of NGS project model. """
+
+import itertools
 import os
-import subprocess
-import sys
-if sys.version_info < (3, 3):
-    from collections import Mapping
-else:
-    from collections.abc import Mapping
-import yaml
-import pandas as _pd
-
-from collections import defaultdict
-# Need specific sequence of actions for colorama imports?
-from colorama import init
-init()
-from colorama import Fore, Style
-from shutil import rmtree
+
+try:
+    from functools import cached_property
+except ImportError:
+    # cached_property was introduced in python 3.8
+    cached_property = property
+from logging import getLogger
+
+from divvy import ComputingConfiguration
+from eido import PathAttrNotFoundError, read_schema
 from jsonschema import ValidationError
-from copy import copy
+from pandas.core.common import flatten
+from peppy import CONFIG_KEY, OUTDIR_KEY
+from peppy import Project as peppyProject
+from peppy.utils import make_abs_via_cfg
+from pipestat import PipestatError, PipestatManager
+from ubiquerg import expandpath, is_command_callable
 
-from . import __version__, build_parser, _LEVEL_BY_VERBOSITY
-from .conductor import SubmissionConductor
 from .const import *
-from .exceptions import JobSubmissionException, MisconfigurationException
-from .html_reports import HTMLReportBuilder
-from .project import Project, ProjectContext
+from .exceptions import *
+from .pipeline_interface import PipelineInterface
+from .processed_project import populate_project_paths, populate_sample_paths
 from .utils import *
-from .looper_config import *
-
-from divvy import DEFAULT_COMPUTE_RESOURCES_NAME, select_divvy_config
-from logmuse import init_logger
-from peppy.const import *
-from eido import validate_sample, validate_config, inspect_project
-from ubiquerg.cli_tools import query_yes_no
-from ubiquerg.collection import uniqify
 
+__all__ = ["Project"]
 
-_PKGNAME = "looper"
-_LOGGER = logging.getLogger(_PKGNAME)
+_LOGGER = getLogger(__name__)
 
-class Executor(object):
-    """ Base class that ensures the program's Sample counter starts.
 
-    Looper is made up of a series of child classes that each extend the base
-    Executor class. Each child class does a particular task (such as run the
-    project, summarize the project, destroy the project, etc). The parent
-    Executor class simply holds the code that is common to all child classes,
-    such as counting samples as the class does its thing."""
+class ProjectContext(object):
+    """Wrap a Project to provide protocol-specific Sample selection."""
 
-    __metaclass__ = abc.ABCMeta
+    def __init__(
+        self, prj, selector_attribute=None, selector_include=None, selector_exclude=None
+    ):
+        """Project and what to include/exclude defines the context."""
+        if not isinstance(selector_attribute, str):
+            raise TypeError(
+                "Name of attribute for sample selection isn't a string: {} "
+                "({})".format(selector_attribute, type(selector_attribute))
+            )
+        self.prj = prj
+        self.include = selector_include
+        self.exclude = selector_exclude
+        self.attribute = selector_attribute
+
+    def __getattr__(self, item):
+        """Samples are context-specific; other requests are handled
+        locally or dispatched to Project."""
+        if item == "samples":
+            return fetch_samples(
+                prj=self.prj,
+                selector_attribute=self.attribute,
+                selector_include=self.include,
+                selector_exclude=self.exclude,
+            )
+        if item in ["prj", "include", "exclude"]:
+            # Attributes requests that this context/wrapper handles
+            return self.__dict__[item]
+        else:
+            # Dispatch attribute request to Project.
+            return getattr(self.prj, item)
 
-    def __init__(self, prj):
-        """
-        The Project defines the instance; establish an iteration counter.
+    def __getitem__(self, item):
+        """Provide the Mapping-like item access to the instance's Project."""
+        return self.prj[item]
+
+    def __enter__(self):
+        """References pass through this instance as needed, so the context
+        provided is the instance itself."""
+        return self
 
-        :param Project prj: Project with which to work/operate on
-        """
-        super(Executor, self).__init__()
-        self.prj = prj
-        self.counter = LooperCounter(len(prj.samples))
+    def __repr__(self):
+        return self.prj.__repr__()
 
-    @abc.abstractmethod
-    def __call__(self, *args, **kwargs):
-        """ Do the work of the subcommand/program. """
+    def __exit__(self, *args):
+        """Context teardown."""
         pass
 
 
-class Checker(Executor):
+class Project(peppyProject):
+    """
+    Looper-specific Project.
+
+    :param str cfg: path to configuration file with data from
+        which Project is to be built
+    :param Iterable[str] amendments: name indicating amendment to use, optional
+    :param str divcfg_path: path to an environment configuration YAML file
+        specifying compute settings.
+    :param bool permissive: Whether a error should be thrown if
+        a sample input file(s) do not exist or cannot be open.
+    :param str compute_env_file: Environment configuration YAML file specifying
+        compute settings.
+    """
+
+    def __init__(self, cfg, amendments=None, divcfg_path=None, runp=False, **kwargs):
+        super(Project, self).__init__(cfg=cfg, amendments=amendments)
+        setattr(self, EXTRA_KEY, dict())
+        for attr_name in CLI_PROJ_ATTRS:
+            if attr_name in kwargs:
+                setattr(self[EXTRA_KEY], attr_name, kwargs[attr_name])
+        self._samples_by_interface = self._samples_by_piface(self.piface_key)
+        self._interfaces_by_sample = self._piface_by_samples()
+        self.linked_sample_interfaces = self._get_linked_pifaces()
+        if FILE_CHECKS_KEY in self[EXTRA_KEY]:
+            setattr(self, "file_checks", not self[EXTRA_KEY][FILE_CHECKS_KEY])
+        if DRY_RUN_KEY in self[EXTRA_KEY]:
+            setattr(self, DRY_RUN_KEY, self[EXTRA_KEY][DRY_RUN_KEY])
+        self.dcc = (
+            None
+            if divcfg_path is None
+            else ComputingConfiguration(filepath=divcfg_path)
+        )
+        if hasattr(self, DRY_RUN_KEY) and not self[DRY_RUN_KEY]:
+            _LOGGER.debug("Ensuring project directories exist")
+            self.make_project_dirs()
 
-    def __call__(self, flags=None, all_folders=False, max_file_count=30):
+    @property
+    def piface_key(self):
         """
-        Check Project status, based on flag files.
+        Name of the pipeline interface attribute for this project
 
-        :param Iterable[str] | str flags: Names of flags to check, optional;
-            if unspecified, all known flags will be checked.
-        :param bool all_folders: Whether to check flags in all folders, not
-            just those for samples in the config file from which the Project
-            was created.
-        :param int max_file_count: Maximum number of filepaths to display for a
-            given flag.
-        """
-
-        # Handle single or multiple flags, and alphabetize.
-        flags = sorted([flags] if isinstance(flags, str)
-                       else list(flags or FLAGS))
-        flag_text = ", ".join(flags)
-
-        # Collect the files by flag and sort by flag name.
-        _LOGGER.debug("Checking project folders for flags: %s", flag_text)
-        if all_folders:
-            files_by_flag = fetch_flag_files(
-                results_folder=self.prj.results_folder, flags=flags)
-        else:
-            files_by_flag = fetch_flag_files(prj=self.prj, flags=flags)
+        :return str: name of the pipeline interface attribute
+        """
+        return self._extra_cli_or_cfg(PIFACE_KEY_SELECTOR) or PIPELINE_INTERFACES_KEY
 
-        # For each flag, output occurrence count.
-        for flag in flags:
-            _LOGGER.info("%s: %d", flag.upper(), len(files_by_flag[flag]))
+    @property
+    def toggle_key(self):
+        """
+        Name of the toggle attribute for this project
 
-        # For each flag, output filepath(s) if not overly verbose.
-        for flag in flags:
-            try:
-                files = files_by_flag[flag]
-            except Exception as e:
-                _LOGGER.debug("No files for {} flag. Caught exception: {}".
-                              format(flags, getattr(e, 'message', repr(e))))
-                continue
-            # If checking on a specific flag, do not limit the number of
-            # reported filepaths, but do not report empty file lists
-            if len(flags) == 1 and len(files) > 0:
-                _LOGGER.info("%s (%d):\n%s", flag.upper(),
-                             len(files), "\n".join(files))
-            # Regardless of whether 0-count flags are previously reported,
-            # don't report an empty file list for a flag that's absent.
-            # If the flag-to-files mapping is defaultdict, absent flag (key)
-            # will fetch an empty collection, so check for length of 0.
-            if 0 < len(files) <= max_file_count:
-                _LOGGER.info("%s (%d):\n%s", flag.upper(),
-                             len(files), "\n".join(files))
-
-
-class Cleaner(Executor):
-    """ Remove all intermediate files (defined by pypiper clean scripts). """
-
-    def __call__(self, args, preview_flag=True):
-        """
-        Execute the file cleaning process.
-
-        :param argparse.Namespace args: command-line options and arguments
-        :param bool preview_flag: whether to halt before actually removing files
-        """
-        for sample in self.prj.samples:
-            _LOGGER.info(self.counter.show(sample.sample_name))
-            sample_output_folder = sample_folder(self.prj, sample)
-            cleanup_files = glob.glob(os.path.join(sample_output_folder,
-                                                   "*_cleanup.sh"))
-            if not cleanup_files:
-                _LOGGER.info("Nothing to clean.")
-                continue
-            if preview_flag:
-                # Preview: Don't actually clean, just show what will be cleaned.
-                _LOGGER.info("Files to clean: %s", ", ".join(cleanup_files))
-            else:
-                for f in cleanup_files:
-                    _LOGGER.info(f)
-                    subprocess.call(["sh", f])
-        if not preview_flag:
-            _LOGGER.info("Clean complete.")
-            return 0
-        if args.dry_run:
-            _LOGGER.info("Dry run. No files cleaned.")
-            return 0
-        if not args.force_yes and not \
-                query_yes_no("Are you sure you want to permanently delete all "
-                             "intermediate pipeline results for this project?"):
-            _LOGGER.info("Clean action aborted by user.")
-            return 1
-        self.counter.reset()
-        return self(args, preview_flag=False)
-
-
-class Destroyer(Executor):
-    """ Destroyer of files and folders associated with Project's Samples """
-
-    def __call__(self, args, preview_flag=True):
-        """
-        Completely remove all output produced by any pipelines.
-
-        :param argparse.Namespace args: command-line options and arguments
-        :param bool preview_flag: whether to halt before actually removing files
-        """
-
-        _LOGGER.info("Removing results:")
-        for sample in self.prj.samples:
-            _LOGGER.info(self.counter.show(sample.sample_name))
-            sample_output_folder = sample_folder(self.prj, sample)
-            if preview_flag:
-                # Preview: Don't actually delete, just show files.
-                _LOGGER.info(str(sample_output_folder))
-            else:
-                _remove_or_dry_run(sample_output_folder, args.dry_run)
+        :return str: name of the toggle attribute
+        """
+        return self._extra_cli_or_cfg(TOGGLE_KEY_SELECTOR) or SAMPLE_TOGGLE_ATTR
+
+    @property
+    def selected_compute_package(self):
+        """
+        Compute package name specified in object constructor
+
+        :return str: compute package name
+        """
+        return self._extra_cli_or_cfg(COMPUTE_PACKAGE_KEY)
+
+    @property
+    def cli_pifaces(self):
+        """
+        Collection of pipeline interface sources specified in object constructor
 
-        _LOGGER.info("Removing summary:")
-        destroy_summary(self.prj, args.dry_run)
+        :return list[str]: collection of pipeline interface sources
+        """
+        x = self._extra_cli_or_cfg(self.piface_key)
+        return (
+            list(flatten([x] if not isinstance(x, list) else x))
+            if x is not None
+            else None
+        )
 
-        if not preview_flag:
-            _LOGGER.info("Destroy complete.")
-            return 0
+    @property
+    def output_dir(self):
+        """
+        Output directory for the project, specified in object constructor
 
-        if args.dry_run:
-            _LOGGER.info("Dry run. No files destroyed.")
-            return 0
+        :return str: path to the output directory
+        """
+        return self._extra_cli_or_cfg(OUTDIR_KEY, strict=True)
 
-        if not args.force_yes and not query_yes_no(
-                "Are you sure you want to permanently delete all pipeline "
-                "results for this project?"):
-            _LOGGER.info("Destroy action aborted by user.")
-            return 1
+    def _extra_cli_or_cfg(self, attr_name, strict=False):
+        """
+        Get attribute value provided in kwargs in object constructor of from
+        looper section in the configuration file
 
-        self.counter.reset()
+        :param str attr_name: name of the attribute to get value for
+        :param bool strict: whether a non-existent attribute is exceptional
+        :raise MisconfigurationException: in strict mode, when no attribute
+         found
+        """
+        try:
+            result = getattr(self[EXTRA_KEY], attr_name)
+        except (AttributeError, KeyError):
+            pass
+        else:
+            if result is not None:
+                return result
+        if (
+            CONFIG_KEY in self
+            and LOOPER_KEY in self[CONFIG_KEY]
+            and attr_name in self[CONFIG_KEY][LOOPER_KEY]
+        ):
+            return self[CONFIG_KEY][LOOPER_KEY][attr_name]
+        else:
+            if strict:
+                raise MisconfigurationException(
+                    "'{}' is missing. Provide it in the '{}' section of the "
+                    "project configuration file".format(attr_name, LOOPER_KEY)
+                )
+            return
 
-        # Finally, run the true destroy:
-        return self(args, preview_flag=False)
+    @property
+    def results_folder(self):
+        """
+        Path to the results folder for the project
 
+        :return str: path to the results folder in the output folder
+        """
+        return self._out_subdir_path(RESULTS_SUBDIR_KEY, default="results_pipeline")
 
-class Collator(Executor):
-    """" Submitter for project-level pipelines """
-    def __init__(self, prj):
+    @property
+    def submission_folder(self):
         """
-        Initializes an instance
+        Path to the submission folder for the project
 
-        :param Project prj: Project with which to work/operate on
+        :return str: path to the submission in the output folder
         """
-        super(Executor, self).__init__()
-        self.prj = prj
+        return self._out_subdir_path(SUBMISSION_SUBDIR_KEY, default="submission")
 
-    def __call__(self, args, **compute_kwargs):
+    def _out_subdir_path(self, key: str, default: str) -> str:
         """
-        Matches collators by protocols, creates submission scripts
-        and submits them
+        Create a system path relative to the project output directory.
+        The values for the names of the subdirectories are sourced from
+        kwargs passed to the object constructor.
 
-        :param argparse.Namespace args: parsed command-line options and
-            arguments, recognized by looper
+        :param str key: name of the attribute mapped to the value of interest
+        :param str default: if key not specified, a default to use
+        :return str: path to the folder
         """
-        jobs = 0
-        project_pifaces = self.prj.project_pipeline_interface_sources
-        if not project_pifaces:
-            raise MisconfigurationException(
-                "Looper requires a pointer to at least one project pipeline. "
-                "Please refer to the documentation on linking project to a "
-                "pipeline: "
-                "http://looper.databio.org/en/latest/defining-a-project")
-        self.counter = LooperCounter(len(project_pifaces))
-        for project_piface in project_pifaces:
-            try:
-                project_piface_object = \
-                    PipelineInterface(project_piface, pipeline_type="project")
-            except (IOError, ValidationError) as e:
-                _LOGGER.warning(
-                    "Ignoring invalid pipeline interface source: {}. "
-                    "Caught exception: {}".
-                        format(project_piface, getattr(e, 'message', repr(e))))
-                continue
-            _LOGGER.info(self.counter.show(
-                name=self.prj.name, type="project",
-                pipeline_name=project_piface_object.pipeline_name))
-            conductor = SubmissionConductor(
-                pipeline_interface=project_piface_object,
-                prj=self.prj,
-                compute_variables=compute_kwargs,
-                delay=args.time_delay,
-                extra_args=args.command_extra,
-                extra_args_override=args.command_extra_override,
-                ignore_flags=args.ignore_flags,
-                collate=True
-            )
-            conductor._pool = [None]
-            conductor.submit()
-            jobs += conductor.num_job_submissions
-        _LOGGER.info("\nLooper finished")
-        _LOGGER.info("Jobs submitted: {}".format(jobs))
-
-
-class Runner(Executor):
-    """ The true submitter of pipelines """
-
-    def __call__(self, args, rerun=False, **compute_kwargs):
-        """
-        Do the Sample submission.
-
-        :param argparse.Namespace args: parsed command-line options and
-            arguments, recognized by looper
-        :param list remaining_args: command-line options and arguments not
-            recognized by looper, germane to samples/pipelines
-        :param bool rerun: whether the given sample is being rerun rather than
-            run for the first time
-        """
-        max_cmds = sum(list(map(len, self.prj._samples_by_interface.values())))
-        self.counter.total = max_cmds
-        failures = defaultdict(list)  # Collect problems by sample.
-        processed_samples = set()  # Enforce one-time processing.
-        submission_conductors = {}
-        comp_vars = compute_kwargs or {}
-
-        # Determine number of samples eligible for processing.
-        num_samples = len(self.prj.samples)
-        if args.limit is None:
-            upper_sample_bound = num_samples
-        elif args.limit < 0:
-            raise ValueError("Invalid number of samples to run: {}".format(args.limit))
-        else:
-            upper_sample_bound = min(args.limit, num_samples)
-        _LOGGER.debug("Limiting to {} of {} samples".
-                      format(upper_sample_bound, num_samples))
-
-        num_commands_possible = 0
-        failed_submission_scripts = []
-
-        # config validation (samples excluded) against all schemas defined
-        # for every pipeline matched for this project
-        [validate_config(self.prj, schema_file, True)
-         for schema_file in self.prj.get_schemas(self.prj.pipeline_interfaces)]
-
-        for piface in self.prj.pipeline_interfaces:
-            conductor = SubmissionConductor(
-                pipeline_interface=piface,
-                prj=self.prj,
-                compute_variables=comp_vars,
-                delay=args.time_delay,
-                extra_args=args.command_extra,
-                extra_args_override=args.command_extra_override,
-                ignore_flags=args.ignore_flags,
-                max_cmds=args.lumpn,
-                max_size=args.lump
-            )
-            submission_conductors[piface.pipe_iface_file] = conductor
-
-        for sample in self.prj.samples[:upper_sample_bound]:
-            pl_fails = []
-            skip_reasons = []
-            sample_pifaces = self.prj.get_sample_piface(sample[SAMPLE_NAME_ATTR])
-            if not sample_pifaces:
-                skip_reasons.append("No pipeline interfaces defined")
-
-            if skip_reasons:
-                _LOGGER.warning(NOT_SUB_MSG.format(", ".join(skip_reasons)))
-                failures[sample.sample_name] = skip_reasons
-                continue
+        parent = getattr(self, OUTDIR_KEY)
+        child = getattr(self[EXTRA_KEY], key, default) or default
+        return os.path.join(parent, child)
 
-            # single sample validation against a single schema
-            # (from sample's piface)
-            [validate_sample(self.prj, sample.sample_name, schema_file, True)
-             for schema_file in self.prj.get_schemas(sample_pifaces)]
-
-            processed_samples.add(sample[SAMPLE_NAME_ATTR])
-
-            for sample_piface in sample_pifaces:
-                _LOGGER.info(
-                    self.counter.show(name=sample.sample_name,
-                                      pipeline_name=sample_piface.pipeline_name)
+    def make_project_dirs(self):
+        """
+        Create project directory structure if it doesn't exist.
+        """
+        for folder_key in ["results_folder", "submission_folder"]:
+            folder_path = getattr(self, folder_key)
+            _LOGGER.debug("Ensuring project dir exists: '{}'".format(folder_path))
+            if not os.path.exists(folder_path):
+                _LOGGER.debug(
+                    "Attempting to create project folder: '{}'".format(folder_path)
                 )
-                num_commands_possible += 1
-                cndtr = submission_conductors[sample_piface.pipe_iface_file]
                 try:
-                    curr_pl_fails = cndtr.add_sample(sample, rerun=rerun)
-                except JobSubmissionException as e:
-                    failed_submission_scripts.append(e.script)
-                else:
-                    pl_fails.extend(curr_pl_fails)
-            if pl_fails:
-                failures[sample.sample_name].extend(pl_fails)
-
-        job_sub_total = 0
-        cmd_sub_total = 0
-
-        for piface, conductor in submission_conductors.items():
-            conductor.submit(force=True)
-            job_sub_total += conductor.num_job_submissions
-            cmd_sub_total += conductor.num_cmd_submissions
-            conductor.write_skipped_sample_scripts()
-
-        # Report what went down.
-        _LOGGER.info("\nLooper finished")
-        _LOGGER.info("Samples valid for job generation: {} of {}".
-                     format(len(processed_samples), num_samples))
-        _LOGGER.info("Commands submitted: {} of {}".
-                     format(cmd_sub_total, max_cmds))
-        _LOGGER.info("Jobs submitted: {}".format(job_sub_total))
-        if args.dry_run:
-            _LOGGER.info("Dry run. No jobs were actually submitted.")
-
-        # Restructure sample/failure data for display.
-        samples_by_reason = defaultdict(set)
-        # Collect names of failed sample(s) by failure reason.
-        for sample, failures in failures.items():
-            for f in failures:
-                samples_by_reason[f].add(sample)
-        # Collect samples by pipeline with submission failure.
-        for piface, conductor in submission_conductors.items():
-            # Don't add failure key if there are no samples that failed for
-            # that reason.
-            if conductor.failed_samples:
-                fails = set(conductor.failed_samples)
-                samples_by_reason[SUBMISSION_FAILURE_MESSAGE] |= fails
-
-        failed_sub_samples = samples_by_reason.get(SUBMISSION_FAILURE_MESSAGE)
-        if failed_sub_samples:
-            _LOGGER.info("\n{} samples with at least one failed job submission:"
-                         " {}".format(len(failed_sub_samples),
-                                      ", ".join(failed_sub_samples)))
-
-        # If failure keys are only added when there's at least one sample that
-        # failed for that reason, we can display information conditionally,
-        # depending on whether there's actually failure(s).
-        if samples_by_reason:
-            _LOGGER.info("\n{} unique reasons for submission failure: {}".format(
-                len(samples_by_reason), ", ".join(samples_by_reason.keys())))
-            full_fail_msgs = [_create_failure_message(reason, samples)
-                              for reason, samples in samples_by_reason.items()]
-            _LOGGER.info("\nSummary of failures:\n{}".
-                         format("\n".join(full_fail_msgs)))
-
-
-class Report(Executor):
-    """ Combine project outputs into a browsable HTML report """
-    def __call__(self, args):
-        # initialize the report builder
-        report_builder = HTMLReportBuilder(self.prj)
-
-        # Do the stats and object summarization.
-        table = Table(self.prj)()
-        # run the report builder. a set of HTML pages is produced
-        report_path = report_builder(table.objs, table.stats,
-                                     uniqify(table.columns))
-
-        _LOGGER.info("HTML Report (n=" + str(len(table.stats)) + "): "
-                     + report_path)
-
-
-class Table(Executor):
-    """ Project/Sample statistics and table output generator """
-    def __init__(self, prj):
-        # call the inherited initialization
-        super(Table, self).__init__(prj)
-        self.prj = prj
+                    os.makedirs(folder_path)
+                except OSError as e:
+                    _LOGGER.warning(
+                        "Could not create project folder: '{}'".format(str(e))
+                    )
+
+    @cached_property
+    def project_pipeline_interface_sources(self):
+        """
+        Get a list of all valid project-level pipeline interface sources
+        associated with this project. Sources that are file paths are expanded
+
+        :return list[str]: collection of valid pipeline interface sources:
+        """
+        return (
+            [self._resolve_path_with_cfg(src) for src in self.cli_pifaces]
+            if self.cli_pifaces is not None
+            else []
+        )
 
-    def __call__(self):
-        # pull together all the fits and stats from each sample into
-        # project-combined spreadsheets.
-        self.stats, self.columns = _create_stats_summary(self.prj, self.counter)
-        self.objs = _create_obj_summary(self.prj, self.counter)
-        return self
+    @cached_property
+    def project_pipeline_interfaces(self):
+        """
+        Flat list of all valid project-level interface objects associated
+        with this Project
 
+        Note that only valid pipeline interfaces will show up in the
+        result (ones that exist on disk/remotely and validate successfully
+        against the schema)
 
-def _create_stats_summary(project, counter):
-    """
-    Create stats spreadsheet and columns to be considered in the report, save
-    the spreadsheet to file
+        :return list[looper.PipelineInterface]: list of pipeline interfaces
+        """
+        return [
+            PipelineInterface(pi, pipeline_type="project")
+            for pi in self.project_pipeline_interface_sources
+        ]
 
-    :param looper.Project project: the project to be summarized
-    :param looper.LooperCounter counter: a counter object
-    """
-    # Create stats_summary file
-    columns = []
-    stats = []
-    project_samples = project.samples
-    missing_files = []
-    _LOGGER.info("Creating stats summary...")
-    for sample in project_samples:
-        _LOGGER.info(counter.show(sample.sample_name, sample.protocol))
-        sample_output_folder = sample_folder(project, sample)
-        # Grab the basic info from the annotation sheet for this sample.
-        # This will correspond to a row in the output.
-        sample_stats = sample.get_sheet_dict()
-        columns.extend(sample_stats.keys())
-        # Version 0.3 standardized all stats into a single file
-        stats_file = os.path.join(sample_output_folder, "stats.tsv")
-        if not os.path.isfile(stats_file):
-            missing_files.append(stats_file)
-            continue
-        t = _pd.read_csv(stats_file, sep="\t", header=None,
-                         names=['key', 'value', 'pl'])
-        t.drop_duplicates(subset=['key', 'pl'], keep='last', inplace=True)
-        t.loc[:, 'plkey'] = t['pl'] + ":" + t['key']
-        dupes = t.duplicated(subset=['key'], keep=False)
-        t.loc[dupes, 'key'] = t.loc[dupes, 'plkey']
-        sample_stats.update(t.set_index('key')['value'].to_dict())
-        stats.append(sample_stats)
-        columns.extend(t.key.tolist())
-    if missing_files:
-        _LOGGER.warning("Stats files missing for {} samples: {}".
-                        format(len(missing_files),missing_files))
-    tsv_outfile_path = get_file_for_project(project, 'stats_summary.tsv')
-    tsv_outfile = open(tsv_outfile_path, 'w')
-    tsv_writer = csv.DictWriter(tsv_outfile, fieldnames=uniqify(columns),
-                                delimiter='\t', extrasaction='ignore')
-    tsv_writer.writeheader()
-    for row in stats:
-        tsv_writer.writerow(row)
-    tsv_outfile.close()
-    _LOGGER.info("Statistics summary (n=" + str(len(stats)) + "): " +
-                 tsv_outfile_path)
-    counter.reset()
-    return stats, uniqify(columns)
+    @cached_property
+    def pipeline_interfaces(self):
+        """
+        Flat list of all valid interface objects associated with this Project
 
+        Note that only valid pipeline interfaces will show up in the
+        result (ones that exist on disk/remotely and validate successfully
+        against the schema)
 
-def _create_obj_summary(project, counter):
-    """
-    Read sample specific objects files and save to a data frame
+        :return list[looper.PipelineInterface]: list of pipeline interfaces
+        """
+        return [pi for ifaces in self._interfaces_by_sample.values() for pi in ifaces]
 
-    :param looper.Project project: the project to be summarized
-    :param looper.LooperCounter counter: a counter object
-    :return pandas.DataFrame: objects spreadsheet
-    """
-    _LOGGER.info("Creating objects summary...")
-    objs = _pd.DataFrame()
-    # Create objects summary file
-    missing_files = []
-    for sample in project.samples:
-        # Process any reported objects
-        _LOGGER.info(counter.show(sample.sample_name, sample.protocol))
-        sample_output_folder = sample_folder(project, sample)
-        objs_file = os.path.join(sample_output_folder, "objects.tsv")
-        if not os.path.isfile(objs_file):
-            missing_files.append(objs_file)
-            continue
-        t = _pd.read_csv(objs_file, sep="\t", header=None,
-                         names=['key', 'filename', 'anchor_text',
-                                'anchor_image', 'annotation'])
-        t['sample_name'] = sample.sample_name
-        objs = objs.append(t, ignore_index=True)
-    if missing_files:
-        _LOGGER.warning("Object files missing for {} samples: {}".
-                        format(len(missing_files), missing_files))
-    # create the path to save the objects file in
-    objs_file = get_file_for_project(project, 'objs_summary.tsv')
-    objs.to_csv(objs_file, sep="\t")
-    _LOGGER.info("Objects summary (n=" +
-                 str(len(project.samples) - len(missing_files)) + "): " +
-                 objs_file)
-    return objs
-
-
-def _create_failure_message(reason, samples):
-    """ Explain lack of submission for a single reason, 1 or more samples. """
-    color = Fore.LIGHTRED_EX
-    reason_text = color + reason + Style.RESET_ALL
-    samples_text = ", ".join(samples)
-    return "{}: {}".format(reason_text, samples_text)
+    @cached_property
+    def pipeline_interface_sources(self):
+        """
+        Get a list of all valid pipeline interface sources associated
+        with this project. Sources that are file paths are expanded
 
+        :return list[str]: collection of valid pipeline interface sources
+        """
+        return self._samples_by_interface.keys()
 
-def _remove_or_dry_run(paths, dry_run=False):
-    """
-    Remove file or directory or just inform what would be removed in
-    case of dry run
+    @cached_property
+    def pipestat_configured(self):
+        """
+        Whether pipestat configuration is complete for all sample pipelines
 
-    :param list|str paths: list of paths to files/dirs to be removed
-    :param bool dry_run: logical indicating whether the files should remain
-        untouched and massage printed
-    """
-    paths = paths if isinstance(paths, list) else [paths]
-    for path in paths:
-        if os.path.exists(path):
-            if dry_run:
-                _LOGGER.info("DRY RUN. I would have removed: " + path)
-            else:
-                _LOGGER.info("Removing: " + path)
-                if os.path.isfile(path):
-                    os.remove(path)
-                else:
-                    rmtree(path, ignore_errors=True)
-        else:
-            _LOGGER.info(path + " does not exist.")
+        :return bool: whether pipestat configuration is complete
+        """
+        return self._check_if_pipestat_configured()
 
+    @cached_property
+    def pipestat_configured_project(self):
+        """
+        Whether pipestat configuration is complete for all project pipelines
 
-def destroy_summary(prj, dry_run=False):
-    """
-    Delete the summary files if not in dry run mode
-    """
-    _remove_or_dry_run([get_file_for_project(prj, "summary.html"),
-                        get_file_for_project(prj, 'stats_summary.tsv'),
-                        get_file_for_project(prj, 'objs_summary.tsv'),
-                        get_file_for_project(prj, "reports")], dry_run)
+        :return bool: whether pipestat configuration is complete
+        """
+        return self._check_if_pipestat_configured(project_level=True)
 
+    def get_sample_piface(self, sample_name):
+        """
+        Get a list of pipeline interfaces associated with the specified sample.
 
-class LooperCounter(object):
-    """
-    Count samples as you loop through them, and create text for the
-    subcommand logging status messages.
+        Note that only valid pipeline interfaces will show up in the
+        result (ones that exist on disk/remotely and validate successfully
+        against the schema)
 
-    :param int total: number of jobs to process
-    """
+        :param str sample_name: name of the sample to retrieve list of
+            pipeline interfaces for
+        :return list[looper.PipelineInterface]: collection of valid
+            pipeline interfaces associated with selected sample
+        """
+        try:
+            return self._interfaces_by_sample[sample_name]
+        except KeyError:
+            return None
+
+    def build_submission_bundles(self, protocol, priority=True):
+        """
+        Create pipelines to submit for each sample of a particular protocol.
+
+        With the argument (flag) to the priority parameter, there's control
+        over whether to submit pipeline(s) from only one of the project's
+        known pipeline locations with a match for the protocol, or whether to
+        submit pipelines created from all locations with a match for the
+        protocol.
+
+        :param str protocol: name of the protocol/library for which to
+            create pipeline(s)
+        :param bool priority: to only submit pipeline(s) from the first of the
+            pipelines location(s) (indicated in the project config file) that
+            has a match for the given protocol; optional, default True
+        :return Iterable[(PipelineInterface, type, str, str)]:
+        :raises AssertionError: if there's a failure in the attempt to
+            partition an interface's pipeline scripts into disjoint subsets of
+            those already mapped and those not yet mapped
+        """
+
+        if not priority:
+            raise NotImplementedError(
+                "Currently, only prioritized protocol mapping is supported "
+                "(i.e., pipeline interfaces collection is a prioritized list, "
+                "so only the first interface with a protocol match is used.)"
+            )
+
+        # Pull out the collection of interfaces (potentially one from each of
+        # the locations indicated in the project configuration file) as a
+        # sort of pool of information about possible ways in which to submit
+        # pipeline(s) for sample(s) of the indicated protocol.
+        pifaces = self.interfaces.get_pipeline_interface(protocol)
+        if not pifaces:
+            raise PipelineInterfaceConfigError(
+                "No interfaces for protocol: {}".format(protocol)
+            )
 
-    def __init__(self, total):
-        self.count = 0
-        self.total = total
+        # coonvert to a list, in the future we might allow to match multiple
+        pifaces = pifaces if isinstance(pifaces, str) else [pifaces]
 
-    def show(self, name, type="sample", pipeline_name=None):
-        """
-        Display sample counts status for a particular protocol type.
+        job_submission_bundles = []
+        new_jobs = []
 
-        The counts are running vs. total for the protocol within the Project,
-        and as a side-effect of the call, the running count is incremented.
+        _LOGGER.debug("Building pipelines matched by protocol: {}".format(protocol))
+
+        for pipe_iface in pifaces:
+            # Determine how to reference the pipeline and where it is.
+            path = pipe_iface["path"]
+            if not (os.path.exists(path) or is_command_callable(path)):
+                _LOGGER.warning("Missing pipeline script: {}".format(path))
+                continue
 
-        :param str name: name of the sample
-        :param str pipeline_name: name of the pipeline
-        :return str: message suitable for logging a status update
+            # Add this bundle to the collection of ones relevant for the
+            # current PipelineInterface.
+            new_jobs.append(pipe_iface)
+            job_submission_bundles.append(new_jobs)
+        return list(itertools.chain(*job_submission_bundles))
+
+    @staticmethod
+    def get_schemas(pifaces, schema_key=INPUT_SCHEMA_KEY):
+        """
+        Get the list of unique schema paths for a list of pipeline interfaces
+
+        :param str | Iterable[str] pifaces: pipeline interfaces to search
+            schemas for
+        :param str schema_key: where to look for schemas in the piface
+        :return Iterable[str]: unique list of schema file paths
+        """
+        if isinstance(pifaces, str):
+            pifaces = [pifaces]
+        schema_set = set()
+        for piface in pifaces:
+            schema_file = piface.get_pipeline_schemas(schema_key)
+            if schema_file:
+                schema_set.update([schema_file])
+        return list(schema_set)
+
+    def get_pipestat_managers(self, sample_name=None, project_level=False):
+        """
+        Get a collection of pipestat managers for the selected sample or project.
+
+        The number of pipestat managers corresponds to the number of unique
+        output schemas in the pipeline interfaces specified by the sample or project.
+
+        :param str sample_name: sample name to get pipestat managers for
+        :param bool project_level: whether the project PipestatManagers
+            should be returned
+        :return dict[str, pipestat.PipestatManager]: a mapping of pipestat
+            managers by pipeline interface name
         """
-        self.count += 1
-        return _submission_status_text(type=type,
-            curr=self.count, total=self.total, name=name,
-            pipeline_name=pipeline_name, color=Fore.CYAN
+        pipestat_configs = self._get_pipestat_configuration(
+            sample_name=sample_name, project_level=project_level
         )
+        return {
+            pipeline_name: PipestatManager(**pipestat_vars)
+            for pipeline_name, pipestat_vars in pipestat_configs.items()
+        }
 
-    def reset(self):
-        self.count = 0
+    def _check_if_pipestat_configured(self, project_level=False):
+        """
+        A helper method determining whether pipestat configuration is complete
 
-    def __str__(self):
-        return "LooperCounter of size {}".format(self.total)
+        :param bool project_level: whether the project pipestat config should be checked
+        :return bool: whether pipestat configuration is complete
+        """
+        try:
+            if project_level:
+                self._get_pipestat_configuration(
+                    sample_name=None, project_level=project_level
+                )
+            else:
+                for s in self.samples:
+                    self._get_pipestat_configuration(sample_name=s.sample_name)
+        except Exception as e:
+            context = (
+                f"Project '{self.name}'"
+                if project_level
+                else f"Sample '{s.sample_name}'"
+            )
+            _LOGGER.debug(
+                f"Pipestat configuration incomplete for {context}; "
+                f"caught exception: {getattr(e, 'message', repr(e))}"
+            )
+            return False
+        return True
 
+    def _get_pipestat_configuration(self, sample_name=None, project_level=False):
+        """
+        Get all required pipestat configuration variables
+        """
 
-def _submission_status_text(curr, total, name, pipeline_name=None,
-                            type="sample", color=Fore.CYAN):
-    """ Generate submission sample text for run or collate """
-    txt = color + "## [{n} of {t}] {type}: {name}".\
-        format(n=curr, t=total, type=type, name=name)
-    if pipeline_name:
-        txt += "; pipeline: {}".format(pipeline_name)
-    return txt + Style.RESET_ALL
+        def _get_val_from_attr(pipestat_sect, object, attr_name, default, no_err=False):
+            """
+            Get configuration value from an object's attribute or return default
+
+            :param dict pipestat_sect: pipestat section for sample or project
+            :param peppy.Sample | peppy.Project object: object to get the
+                configuration values for
+            :param str attr_name: attribute name with the value to retrieve
+            :param str default: default attribute name
+            :param bool no_err: do not raise error in case the attribute is missing,
+                in order to use the values specified in a different way, e.g. in pipestat config
+            :return str: retrieved configuration value
+            """
+            if pipestat_sect is not None and attr_name in pipestat_sect:
+                return getattr(object, pipestat_sect[attr_name])
+            try:
+                return getattr(object, default)
+            except AttributeError:
+                if no_err:
+                    return None
+                raise AttributeError(f"'{default}' attribute is missing")
+
+        ret = {}
+        if not project_level and sample_name is None:
+            raise ValueError(
+                "Must provide the sample_name to determine the "
+                "sample to get the PipestatManagers for"
+            )
+        key = "project" if project_level else "sample"
+        if (
+            CONFIG_KEY in self
+            and LOOPER_KEY in self[CONFIG_KEY]
+            and PIPESTAT_KEY in self[CONFIG_KEY][LOOPER_KEY]
+            and key in self[CONFIG_KEY][LOOPER_KEY][PIPESTAT_KEY]
+        ):
+            pipestat_section = self[CONFIG_KEY][LOOPER_KEY][PIPESTAT_KEY][key]
+        else:
+            _LOGGER.debug(
+                f"'{PIPESTAT_KEY}' not found in '{LOOPER_KEY}' section of the "
+                f"project configuration file. Using defaults."
+            )
+            pipestat_section = None
+        pipestat_config = _get_val_from_attr(
+            pipestat_section,
+            self.config if project_level else self.get_sample(sample_name),
+            PIPESTAT_CONFIG_ATTR_KEY,
+            DEFAULT_PIPESTAT_CONFIG_ATTR,
+            True,  # allow for missing pipestat cfg attr, the settings may be provided as Project/Sample attrs
+        )
 
+        pipestat_config = self._resolve_path_with_cfg(pth=pipestat_config)
+        namespace = _get_val_from_attr(
+            pipestat_section,
+            self.config if project_level else self.get_sample(sample_name),
+            PIPESTAT_NAMESPACE_ATTR_KEY,
+            "name" if project_level else self.sample_table_index,
+            pipestat_config and os.path.exists(pipestat_config),
+        )
+        results_file_path = _get_val_from_attr(
+            pipestat_section,
+            self.config if project_level else self.get_sample(sample_name),
+            PIPESTAT_RESULTS_FILE_ATTR_KEY,
+            DEFAULT_PIPESTAT_RESULTS_FILE_ATTR,
+            pipestat_config and os.path.exists(pipestat_config),
+        )
+        if results_file_path is not None:
+            results_file_path = expandpath(results_file_path)
+            if not os.path.isabs(results_file_path):
+                results_file_path = os.path.join(self.output_dir, results_file_path)
+        pifaces = (
+            self.project_pipeline_interfaces
+            if project_level
+            else self._interfaces_by_sample[sample_name]
+        )
+        for piface in pifaces:
+            rec_id = (
+                piface.pipeline_name
+                if self.amendments is None
+                else f"{piface.pipeline_name}_{'_'.join(self.amendments)}"
+            )
+            ret[piface.pipeline_name] = {
+                "namespace": namespace,
+                "config": pipestat_config,
+                "results_file_path": results_file_path,
+                "record_identifier": rec_id,
+                "schema_path": piface.get_pipeline_schemas(OUTPUT_SCHEMA_KEY),
+            }
+        return ret
+
+    def populate_pipeline_outputs(self):
+        """
+        Populate project and sample output attributes based on output schemas
+        that pipeline interfaces point to.
+        """
+        # eido.read_schema always returns a list of schemas since it supports
+        # imports in schemas. The output schemas can't have the import section,
+        # hence it's safe to select the fist element after read_schema() call.
+        for sample in self.samples:
+            sample_piface = self.get_sample_piface(sample[self.sample_table_index])
+            if sample_piface:
+                paths = self.get_schemas(sample_piface, OUTPUT_SCHEMA_KEY)
+                for path in paths:
+                    populate_sample_paths(sample, read_schema(path)[0])
+        schemas = self.get_schemas(self.project_pipeline_interfaces, OUTPUT_SCHEMA_KEY)
+        for schema in schemas:
+            populate_project_paths(self, read_schema(schema)[0])
+
+    def _get_linked_pifaces(self):
+        """
+        Get linked sample pipeline interfaces by project pipeline interface.
+
+        These are indicated in project pipeline interface by
+        'linked_pipeline_interfaces' key. If a project pipeline interface
+         does not have such key defined, an empty list is returned for that
+         pipeline interface.
+
+        :return dict[list[str]]: mapping of sample pipeline interfaces
+            by project pipeline interfaces
+        """
+
+        def _process_linked_piface(p, piface, prj_piface):
+            piface = make_abs_via_cfg(piface, prj_piface)
+            if piface not in p.pipeline_interface_sources:
+                raise PipelineInterfaceConfigError(
+                    "Linked sample pipeline interface was not assigned "
+                    f"to any sample in this project: {piface}"
+                )
+            return piface
 
-def _proc_resources_spec(args):
-    """
-    Process CLI-sources compute setting specification. There are two sources
-    of compute settings in the CLI alone:
-        * YAML file (--settings argument)
-        * itemized compute settings (--compute argument)
-
-    The itemized compute specification is given priority
-
-    :param argparse.Namespace: arguments namespace
-    :return Mapping[str, str]: binding between resource setting name and value
-    :raise ValueError: if interpretation of the given specification as encoding
-        of key-value pairs fails
-    """
-    spec = getattr(args, "compute", None)
-    try:
-        settings_data = read_yaml_file(args.settings) or {}
-    except yaml.YAMLError:
-        _LOGGER.warning("Settings file ({}) does not follow YAML format,"
-                        " disregarding".format(args.settings))
-        settings_data = {}
-    if not spec:
-        return settings_data
-    pairs = [(kv, kv.split("=")) for kv in spec]
-    bads = []
-    for orig, pair in pairs:
-        try:
-            k, v = pair
-        except ValueError:
-            bads.append(orig)
-        else:
-            settings_data[k] = v
-    if bads:
-        raise ValueError(
-            "Could not correctly parse itemized compute specification. "
-            "Correct format: " + EXAMPLE_COMPUTE_SPEC_FMT)
-    return settings_data
-
-
-def main():
-    """ Primary workflow """
-    global _LOGGER
-    parsers = build_parser()
-    parser = parsers[0]
-    aux_parser = parsers[1]
-    aux_parser.suppress_defaults()
-    args, remaining_args = parser.parse_known_args()
-    if args.command is None:
-        parser.print_help(sys.stderr)
-        sys.exit(1)
-    if args.config_file is None:
-        m = "No project config defined"
-        try:
-            setattr(args, "config_file", read_cfg_from_dotfile())
-        except OSError:
-            print(m + " and dotfile does not exist: {}".format(dotfile_path()))
-            parser.print_help(sys.stderr)
-            sys.exit(1)
-        else:
-            print(m + ", using: {}. Read from dotfile ({}).".
-                  format(read_cfg_from_dotfile(), dotfile_path()))
-    if args.command == "init":
-        sys.exit(int(not init_dotfile(dotfile_path(), args.config_file, args.force)))
-    args = enrich_args_via_cfg(args, aux_parser)
-
-    # Set the logging level.
-    if args.dbg:
-        # Debug mode takes precedence and will listen for all messages.
-        level = args.logging_level or logging.DEBUG
-    elif args.verbosity is not None:
-        # Verbosity-framed specification trumps logging_level.
-        level = _LEVEL_BY_VERBOSITY[args.verbosity]
-    else:
-        # Normally, we're not in debug mode, and there's not verbosity.
-        level = LOGGING_LEVEL
+        linked_pifaces = {}
+        for prj_piface in self.project_pipeline_interfaces:
+            pifaces = (
+                prj_piface.linked_pipeline_interfaces
+                if hasattr(prj_piface, "linked_pipeline_interfaces")
+                else []
+            )
+            linked_pifaces[prj_piface.source] = list(
+                {
+                    _process_linked_piface(self, piface, prj_piface.source)
+                    for piface in pifaces
+                }
+            )
+        return linked_pifaces
 
-    # Establish the project-root logger and attach one for this module.
-    logger_kwargs = {"level": level,
-                     "logfile": args.logfile,
-                     "devmode": args.dbg}
-    init_logger(name="peppy", **logger_kwargs)
-    init_logger(name="divvy", **logger_kwargs)
-    init_logger(name="eido", **logger_kwargs)
-    _LOGGER = init_logger(name=_PKGNAME, **logger_kwargs)
-
-    # lc = LooperConfig(select_looper_config(filename=args.looper_config))
-    # _LOGGER.debug("Determined genome config: {}".format(lc))
-
-    _LOGGER.info("Looper version: {}\nCommand: {}".
-                 format(__version__, args.command))
-
-    if len(remaining_args) > 0:
-        _LOGGER.warning("Unrecognized arguments: {}".
-                      format(" ".join([str(x) for x in remaining_args])))
-
-    divcfg = select_divvy_config(filepath=args.divvy) \
-        if hasattr(args, "divvy") else None
-
-    # Initialize project
-    _LOGGER.debug("Building Project")
-    try:
-        p = Project(config_file=args.config_file,
-                    amendments=args.amend,
-                    divcfg_path=divcfg,
-                    runp=args.command == "runp",
-                    **{attr: getattr(args, attr) for attr in CLI_PROJ_ATTRS if attr in args})
-    except yaml.parser.ParserError as e:
-        _LOGGER.error("Project config parse failed -- {}".format(e))
-        sys.exit(1)
-
-    selected_compute_pkg = p.selected_compute_package \
-                           or DEFAULT_COMPUTE_RESOURCES_NAME
-    if p.dcc is not None and not p.dcc.activate_package(selected_compute_pkg):
-        _LOGGER.info("Failed to activate '{}' computing package. "
-                     "Using the default one".format(selected_compute_pkg))
-
-    with ProjectContext(prj=p,
-                        selector_attribute=args.sel_attr,
-                        selector_include=args.sel_incl,
-                        selector_exclude=args.sel_excl) as prj:
+    def _piface_by_samples(self):
+        """
+        Create a mapping of all defined interfaces in this Project by samples.
 
-        if args.command in ["run", "rerun"]:
-            run = Runner(prj)
+        :return dict[str, list[PipelineInterface]]: a collection of pipeline
+            interfaces keyed by sample name
+        """
+        pifaces_by_sample = {}
+        for source, sample_names in self._samples_by_interface.items():
             try:
-                compute_kwargs = _proc_resources_spec(args)
-                run(args, rerun=(args.command == "rerun"), **compute_kwargs)
-            except IOError:
-                _LOGGER.error("{} pipeline_interfaces: '{}'".
-                              format(prj.__class__.__name__,
-                                     prj.pipeline_interface_sources))
-                raise
-
-        if args.command == "runp":
-            compute_kwargs = _proc_resources_spec(args)
-            collate = Collator(prj)
-            collate(args, **compute_kwargs)
-
-        if args.command == "destroy":
-            return Destroyer(prj)(args)
-
-        if args.command == "table":
-            Table(prj)()
-        
-        if args.command == "report":
-            Report(prj)(args)
+                pi = PipelineInterface(source, pipeline_type="sample")
+            except PipelineInterfaceConfigError as e:
+                _LOGGER.debug(f"Skipping pipeline interface creation: {e}")
+            else:
+                for sample_name in sample_names:
+                    pifaces_by_sample.setdefault(sample_name, []).append(pi)
+        return pifaces_by_sample
+
+    def _omit_from_repr(self, k, cls):
+        """
+        Exclude the interfaces from representation.
+
+        :param str k: key of item to consider for omission
+        :param type cls: placeholder to comply with superclass signature
+        """
+        return super(Project, self)._omit_from_repr(k, cls) or k == "interfaces"
+
+    def _resolve_path_with_cfg(self, pth):
+        """
+        Expand provided path and make it absolute using project config path
+
+        :param str pth: path, possibly including env vars and/or relative
+        :return str: absolute path
+        """
+        if pth is None:
+            return
+        pth = expandpath(pth)
+        if not os.path.isabs(pth):
+            pth = os.path.realpath(os.path.join(os.path.dirname(self.config_file), pth))
+            _LOGGER.debug("Relative path made absolute: {}".format(pth))
+        return pth
+
+    def _samples_by_piface(self, piface_key):
+        """
+        Create a collection of all samples with valid pipeline interfaces
+
+        :param str piface_key: name of the attribute that holds pipeline
+         interfaces
+        :return list[str]: a collection of samples keyed by pipeline interface
+            source
+        """
+        samples_by_piface = {}
+        msgs = set()
+        for sample in self.samples:
+            if piface_key in sample and sample[piface_key]:
+                piface_srcs = sample[piface_key]
+                if isinstance(piface_srcs, str):
+                    piface_srcs = [piface_srcs]
+                for source in piface_srcs:
+                    source = self._resolve_path_with_cfg(source)
+                    try:
+                        PipelineInterface(source, pipeline_type="sample")
+                    except (
+                        ValidationError,
+                        IOError,
+                        PipelineInterfaceConfigError,
+                    ) as e:
+                        msg = (
+                            "Ignoring invalid pipeline interface source: "
+                            "{}. Caught exception: {}".format(
+                                source, getattr(e, "message", repr(e))
+                            )
+                        )
+                        msgs.add(msg)
+                        continue
+                    else:
+                        samples_by_piface.setdefault(source, set())
+                        samples_by_piface[source].add(sample[self.sample_table_index])
+        for msg in msgs:
+            _LOGGER.warning(msg)
+        return samples_by_piface
+
+
+def fetch_samples(
+    prj, selector_attribute=None, selector_include=None, selector_exclude=None
+):
+    """
+    Collect samples of particular protocol(s).
+
+    Protocols can't be both positively selected for and negatively
+    selected against. That is, it makes no sense and is not allowed to
+    specify both selector_include and selector_exclude protocols. On the
+    other hand, if
+    neither is provided, all of the Project's Samples are returned.
+    If selector_include is specified, Samples without a protocol will be
+    excluded,
+    but if selector_exclude is specified, protocol-less Samples will be
+    included.
+
+    :param Project prj: the Project with Samples to fetch
+    :param str selector_attribute: name of attribute on which to base the
+    fetch
+    :param Iterable[str] | str selector_include: protocol(s) of interest;
+        if specified, a Sample must
+    :param Iterable[str] | str selector_exclude: protocol(s) to include
+    :return list[Sample]: Collection of this Project's samples with
+        protocol that either matches one of those in selector_include,
+        or either
+        lacks a protocol or does not match one of those in selector_exclude
+    :raise TypeError: if both selector_include and selector_exclude
+    protocols are
+        specified; TypeError since it's basically providing two arguments
+        when only one is accepted, so remain consistent with vanilla
+        Python2;
+        also possible if name of attribute for selection isn't a string
+    """
+    if selector_attribute is None or (not selector_include and not selector_exclude):
+        # Simple; keep all samples.  In this case, this function simply
+        # offers a list rather than an iterator.
+        return list(prj.samples)
+
+    if not isinstance(selector_attribute, str):
+        raise TypeError(
+            "Name for attribute on which to base selection isn't string: "
+            "{} "
+            "({})".format(selector_attribute, type(selector_attribute))
+        )
 
-        if args.command == "check":
-            Checker(prj)(flags=args.flags)
+    # At least one of the samples has to have the specified attribute
+    if prj.samples and not any([hasattr(s, selector_attribute) for s in prj.samples]):
+        raise AttributeError(
+            "The Project samples do not have the attribute '{attr}'".format(
+                attr=selector_attribute
+            )
+        )
 
-        if args.command == "clean":
-            return Cleaner(prj)(args)
+    # Intersection between selector_include and selector_exclude is
+    # nonsense user error.
+    if selector_include and selector_exclude:
+        raise TypeError(
+            "Specify only selector_include or selector_exclude parameter, " "not both."
+        )
+
+    # Ensure that we're working with sets.
+    def make_set(items):
+        if isinstance(items, str):
+            items = [items]
+        return items
+
+    # Use the attr check here rather than exception block in case the
+    # hypothetical AttributeError would occur; we want such
+    # an exception to arise, not to catch it as if the Sample lacks
+    # "protocol"
+    if not selector_include:
+        # Loose; keep all samples not in the selector_exclude.
+        def keep(s):
+            return not hasattr(s, selector_attribute) or getattr(
+                s, selector_attribute
+            ) not in make_set(selector_exclude)
+
+    else:
+        # Strict; keep only samples in the selector_include.
+        def keep(s):
+            return hasattr(s, selector_attribute) and getattr(
+                s, selector_attribute
+            ) in make_set(selector_include)
 
-        if args.command == "inspect":
-            inspect_project(p, args.snames, args.attr_limit)
+    return list(filter(keep, prj.samples))
```

### Comparing `looper-1.3.2/looper/parser_types.py` & `looper-1.4.0/looper/parser_types.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,72 @@
 """ Definitions of the parser argument types """
 
-from attmap import PathExAttMap
+from yacman import YAMLConfigManager
 
 
 def html_range(caravel=False, min_val=0, max_val=10, step=1, value=0):
-    caravel_data = PathExAttMap({
-        "element_type": "range",
-        "element_args": {
-            "min": min_val, "max": max_val, "step": step, "value": value}})
+    caravel_data = YAMLConfigManager(
+        {
+            "element_type": "range",
+            "element_args": {
+                "min": min_val,
+                "max": max_val,
+                "step": step,
+                "value": value,
+            },
+        }
+    )
     if step < 1:
+
         def fun(x=None, caravel_data=caravel_data, caravel=caravel):
             return caravel_data if caravel else float(x)
+
     else:
+
         def fun(x=None, caravel_data=caravel_data, caravel=caravel):
-            return caravel_data if caravel else int(x)
+            return caravel_data if caravel else str(x)
+
     return fun
 
 
 def html_checkbox(caravel=False, checked=False):
     """
     Create argument for type parameter on argparse.ArgumentParser.add_argument.
 
     :param bool caravel: whether this is being used in the caravel context
     :param bool checked: whether to add a particular key-value entry to a
         collection used by caravel
     :return callable: argument to the type parameter of an
         argparse.ArgumentParser's add_argument method.
     """
-    caravel_data = \
-        PathExAttMap({"element_type": "checkbox", "element_args": {}})
+    caravel_data = YAMLConfigManager({"element_type": "checkbox", "element_args": {}})
     if checked:
         caravel_data.add_entries({"element_args": {"checked": True}})
 
     def fun(x=None, caravel_data=caravel_data, caravel=caravel):
         return caravel_data if caravel else eval(x)
+
     return fun
 
 
 def html_select(choices, caravel=False):
     """
     Create argument for type parameter on argparse.ArgumentParser.add_argument.
 
-    :param list[object] choices: collection of valid argument provisions via 
+    :param list[object] choices: collection of valid argument provisions via
         to a particular CLI option
     :param bool caravel: whether this is being used in the caravel context
     :return callable: argument to the type parameter of an
         argparse.ArgumentParser's add_argument method.
     """
     if not isinstance(choices, list):
         raise TypeError(
-            "Argument to choices parameter must be list, got {}.".
-                format(type(choices)))
-    caravel_data = PathExAttMap(
-        {"element_type": "select", "element_args": {"option": choices}})
+            "Argument to choices parameter must be list, got {}.".format(type(choices))
+        )
+    caravel_data = YAMLConfigManager(
+        {"element_type": "select", "element_args": {"option": choices}}
+    )
 
     def fun(x=None, caravel_data=caravel_data, caravel=caravel):
         return caravel_data if caravel else x
+
     return fun
```

### Comparing `looper-1.3.2/looper/pipeline_interface.py` & `looper-1.4.0/looper/pipeline_interface.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,81 +1,97 @@
 """ Model the connection between a pipeline and a project or executor. """
 
 import os
-import jsonschema
-import pandas as pd
-
-from collections import Mapping
+from collections.abc import Mapping
 from logging import getLogger
 from warnings import warn
 
-from attmap import PathExAttMap as PXAM
+import jsonschema
+import pandas as pd
 from eido import read_schema
 from peppy import utils as peputil
 from ubiquerg import expandpath, is_url
-from yacman import load_yaml
+from yacman import load_yaml, YAMLConfigManager
 
 from .const import *
+from .exceptions import (
+    InvalidResourceSpecificationException,
+    PipelineInterfaceConfigError,
+)
 from .utils import jinja_render_template_strictly
-from .exceptions import InvalidResourceSpecificationException
 
 __author__ = "Michal Stolarczyk"
 __email__ = "michal@virginia.edu"
 
 _LOGGER = getLogger(__name__)
 
 
 @peputil.copy
-class PipelineInterface(PXAM):
+class PipelineInterface(YAMLConfigManager):
     """
     This class parses, holds, and returns information for a yaml file that
     specifies how to interact with each individual pipeline. This
     includes both resources to request for cluster job submission, as well as
     arguments to be passed from the sample annotation metadata to the pipeline
 
     :param str | Mapping config: path to file from which to parse
         configuration data, or pre-parsed configuration data.
     :param str pipeline_type: type of the pipeline,
         must be either 'sample' or 'project'.
     """
+
     def __init__(self, config, pipeline_type=None):
         super(PipelineInterface, self).__init__()
 
         if isinstance(config, Mapping):
             self.pipe_iface_file = None
             self.source = None
         else:
-            _LOGGER.debug("Reading {} from: {}".
-                          format(self.__class__.__name__, config))
+            _LOGGER.debug("Reading {} from: {}".format(self.__class__.__name__, config))
             self.pipe_iface_file = config
             self.source = config
             config = load_yaml(config)
+        if PIPELINE_INTERFACE_PIPELINE_NAME_KEY not in config:
+            raise PipelineInterfaceConfigError(
+                f"'{PIPELINE_INTERFACE_PIPELINE_NAME_KEY}' is required in pipeline interface config data."
+            )
         self.update(config)
-        self._validate(PIFACE_SCHEMA_SRC, flavor=pipeline_type)
+        self._validate(schema_src=PIFACE_SCHEMA_SRC)
         if "path" in self:
-            warn(message="'path' specification as a top-level pipeline "
-                         "interface key is deprecated and will be removed with "
-                         "the next release. Please use 'paths' section "
-                         "from now on.", category=DeprecationWarning)
+            warn(
+                message="'path' specification as a top-level pipeline "
+                "interface key is deprecated and will be removed with "
+                "the next release. Please use 'paths' section "
+                "from now on.",
+                category=DeprecationWarning,
+            )
             self._expand_paths(["path"])
         self._expand_paths(["compute", "dynamic_variables_script_path"])
 
+    @property
+    def pipeline_name(self):
+        return self[PIPELINE_INTERFACE_PIPELINE_NAME_KEY]
+
     def render_var_templates(self, namespaces):
         """
         Render path templates under 'var_templates' in this pipeline interface.
 
         :param dict namespaces: namespaces to use for rendering
         """
         if VAR_TEMPL_KEY in self:
-            for k, v in self[VAR_TEMPL_KEY].items():
-                setattr(self[VAR_TEMPL_KEY], k,
-                        jinja_render_template_strictly(v, namespaces))
+            var_templates = {}
+            var_templates.update(self[VAR_TEMPL_KEY])
+            for k, v in var_templates.items():
+                var_templates[k] = jinja_render_template_strictly(v, namespaces)
+            return var_templates
         else:
-            _LOGGER.debug(f"'{VAR_TEMPL_KEY}' section not found in the "
-                          f"{self.__class__.__name__} object.")
+            _LOGGER.debug(
+                f"'{VAR_TEMPL_KEY}' section not found in the "
+                f"{self.__class__.__name__} object."
+            )
 
     def get_pipeline_schemas(self, schema_key=INPUT_SCHEMA_KEY):
         """
         Get path to the pipeline schema.
 
         :param str schema_key: where to look for schemas in the pipeline iface
         :return str: absolute path to the pipeline schema file
@@ -85,15 +101,16 @@
             schema_source = self[schema_key]
         if schema_source:
             _LOGGER.debug("Got schema source: {}".format(schema_source))
             if is_url(schema_source):
                 return schema_source
             elif not os.path.isabs(schema_source):
                 schema_source = os.path.join(
-                    os.path.dirname(self.pipe_iface_file), schema_source)
+                    os.path.dirname(self.pipe_iface_file), schema_source
+                )
         return schema_source
 
     def choose_resource_package(self, namespaces, file_size):
         """
         Select resource bundle for given input file size to given pipeline.
 
         :param float file_size: Size of input data (in gigabytes).
@@ -102,28 +119,31 @@
         :return MutableMapping: resource bundle appropriate for given pipeline,
             for given input file size
         :raises ValueError: if indicated file size is negative, or if the
             file size value specified for any resource package is negative
         :raises InvalidResourceSpecificationException: if no default
             resource package specification is provided
         """
+
         def _file_size_ante(name, data):
             # Retrieve this package's minimum file size.
             # Retain backwards compatibility while enforcing key presence.
             try:
                 fsize = float(data[FILE_SIZE_COLNAME])
             except KeyError:
                 raise InvalidResourceSpecificationException(
                     "Required column '{}' does not exist in resource "
-                    "specification TSV.".format(FILE_SIZE_COLNAME))
+                    "specification TSV.".format(FILE_SIZE_COLNAME)
+                )
             # Negative file size is illogical and problematic for comparison.
             if fsize < 0:
                 raise InvalidResourceSpecificationException(
-                    "Found negative value () in '{}' column; package '{}'".
-                        format(fsize, FILE_SIZE_COLNAME, name)
+                    "Found negative value () in '{}' column; package '{}'".format(
+                        fsize, FILE_SIZE_COLNAME, name
+                    )
                 )
             return fsize
 
         def _notify(msg):
             msg += " for pipeline"
             if self.pipe_iface_file is not None:
                 msg += " in interface {}".format(self.pipe_iface_file)
@@ -134,129 +154,147 @@
             Render command string (jinja2 template), execute it in a subprocess
             and return its result (JSON object) as a dict
 
             :param Mapping pipeline: pipeline dict
             :return Mapping: a dict with attributes returned in the JSON
                 by called command
             """
+
             def _log_raise_latest():
-                """ Log error info and raise latest handled exception """
+                """Log error info and raise latest handled exception"""
                 _LOGGER.error(
                     "Could not retrieve JSON via command: '{}'".format(
-                        pipeline[COMPUTE_KEY][DYN_VARS_KEY]))
+                        pipeline[COMPUTE_KEY][DYN_VARS_KEY]
+                    )
+                )
                 raise
+
             json = None
-            if COMPUTE_KEY in pipeline \
-                    and DYN_VARS_KEY in pipeline[COMPUTE_KEY]:
-                from warnings import warn
-                from subprocess import check_output, CalledProcessError
+            if COMPUTE_KEY in pipeline and DYN_VARS_KEY in pipeline[COMPUTE_KEY]:
                 from json import loads
+                from subprocess import CalledProcessError, check_output
+                from warnings import warn
+
                 from .utils import jinja_render_template_strictly
-                warn(message="'dynamic_variables_command_template' feature is "
-                             "deprecated and will be removed with the next "
-                             "release. Please use 'pre_submit' feature from "
-                             "now on.",
-                     category=DeprecationWarning)
+
+                warn(
+                    message="'dynamic_variables_command_template' feature is "
+                    "deprecated and will be removed with the next "
+                    "release. Please use 'pre_submit' feature from "
+                    "now on.",
+                    category=DeprecationWarning,
+                )
                 try:
                     cmd = jinja_render_template_strictly(
                         template=pipeline[COMPUTE_KEY][DYN_VARS_KEY],
-                        namespaces=namespaces
+                        namespaces=namespaces,
                     )
                     json = loads(check_output(cmd, shell=True))
                 except CalledProcessError as e:
                     print(e.output)
                     _log_raise_latest()
                 except Exception:
                     _log_raise_latest()
                 else:
                     _LOGGER.debug(
                         "Loaded resources from JSON returned by a command for"
-                        " pipeline '{}':\n{}".format(self.pipeline_name, json))
+                        " pipeline '{}':\n{}".format(self.pipeline_name, json)
+                    )
             return json
 
         def _load_size_dep_vars(piface):
             """
             Read the resources from a TSV provided in the pipeline interface
 
             :param looper.PipelineInterface piface: currently processed piface
             :param str section: section of pipeline interface to process
             :return pandas.DataFrame: resources
             """
             df = None
-            if COMPUTE_KEY in piface \
-                    and SIZE_DEP_VARS_KEY in piface[COMPUTE_KEY]:
+            if COMPUTE_KEY in piface and SIZE_DEP_VARS_KEY in piface[COMPUTE_KEY]:
                 resources_tsv_path = piface[COMPUTE_KEY][SIZE_DEP_VARS_KEY]
                 if not os.path.isabs(resources_tsv_path):
                     resources_tsv_path = os.path.join(
-                        os.path.dirname(piface.pipe_iface_file),
-                        resources_tsv_path)
-                df = pd.read_csv(resources_tsv_path, sep='\t', header=0).\
-                    fillna(float("inf"))
+                        os.path.dirname(piface.pipe_iface_file), resources_tsv_path
+                    )
+                df = pd.read_csv(resources_tsv_path, sep="\t", header=0).fillna(
+                    float("inf")
+                )
                 df[ID_COLNAME] = df.index
                 df.set_index(ID_COLNAME)
-                _LOGGER.debug("Loaded resources ({}) for pipeline '{}':\n{}".
-                              format(resources_tsv_path, piface.pipeline_name, df))
+                _LOGGER.debug(
+                    "Loaded resources ({}) for pipeline '{}':\n{}".format(
+                        resources_tsv_path, piface.pipeline_name, df
+                    )
+                )
             else:
                 _notify("No '{}' defined".format(SIZE_DEP_VARS_KEY))
             return df
 
         # Ensure that we have a numeric value before attempting comparison.
         file_size = float(file_size)
-        assert file_size >= 0, ValueError("Attempted selection of resource "
-                                         "package for negative file size: {}".
-                                         format(file_size))
+        assert file_size >= 0, ValueError(
+            "Attempted selection of resource "
+            "package for negative file size: {}".format(file_size)
+        )
 
         fluid_resources = _load_dynamic_vars(self)
         if fluid_resources is not None:
             return fluid_resources
         resources_df = _load_size_dep_vars(self)
         resources_data = {}
         if resources_df is not None:
-            resources = resources_df.to_dict('index')
+            resources = resources_df.to_dict("index")
             try:
                 # Sort packages by descending file size minimum to return first
                 # package for which given file size satisfies the minimum.
                 resource_packages = sorted(
                     resources.items(),
                     key=lambda name_and_data: _file_size_ante(*name_and_data),
-                    reverse=False)
+                    reverse=False,
+                )
             except ValueError:
-                _LOGGER.error("Unable to use file size to prioritize "
-                              "resource packages: {}".format(resources))
+                _LOGGER.error(
+                    "Unable to use file size to prioritize "
+                    "resource packages: {}".format(resources)
+                )
                 raise
 
             # choose minimally-sufficient package
             for rp_name, rp_data in resource_packages:
                 size_ante = _file_size_ante(rp_name, rp_data)
                 if file_size <= size_ante:
                     _LOGGER.debug(
                         "Selected '{}' package with file size {}Gb for file "
-                        "of size {}Gb.".format(rp_name, size_ante, file_size))
-                    _LOGGER.debug("Selected resource package data:\n{}".
-                                  format(rp_data))
+                        "of size {}Gb.".format(rp_name, size_ante, file_size)
+                    )
+                    _LOGGER.debug("Selected resource package data:\n{}".format(rp_data))
                     resources_data = rp_data
                     break
 
         if COMPUTE_KEY in self:
             resources_data.update(self[COMPUTE_KEY])
         project = namespaces["project"]
-        if LOOPER_KEY in project and COMPUTE_KEY in project[LOOPER_KEY] \
-                and RESOURCES_KEY in project[LOOPER_KEY][COMPUTE_KEY]:
+        if (
+            LOOPER_KEY in project
+            and COMPUTE_KEY in project[LOOPER_KEY]
+            and RESOURCES_KEY in project[LOOPER_KEY][COMPUTE_KEY]
+        ):
             # overwrite with values from project.looper.compute.resources
-            resources_data.\
-                update(project[LOOPER_KEY][COMPUTE_KEY][RESOURCES_KEY])
+            resources_data.update(project[LOOPER_KEY][COMPUTE_KEY][RESOURCES_KEY])
         return resources_data
 
     def _expand_paths(self, keys):
         """
         Expand paths defined in the pipeline interface file
 
         :param list keys: list of keys resembling the nested structure to get
             to the pipeline interface attributre to expand
         """
+
         def _get_from_dict(map, attrs):
             """
             Get value from a possibly nested mapping using a list of its attributes
 
             :param collections.Mapping map: mapping to retrieve values from
             :param Iterable[str] attrs: a list of attributes
             :return: value found in the the requested attribute or
@@ -288,43 +326,45 @@
 
         raw_path = _get_from_dict(self, keys)
         if not raw_path:
             return
         split_path = raw_path.split(" ")
         if len(split_path) > 1:
             _LOGGER.warning(
-                "Path ({}) contains spaces. Using the first part as path: {}".
-                    format(raw_path, split_path[0]))
+                "Path ({}) contains spaces. Using the first part as path: {}".format(
+                    raw_path, split_path[0]
+                )
+            )
         path = split_path[0]
         pipe_path = expandpath(path)
         if not os.path.isabs(pipe_path) and self.pipe_iface_file:
-            abs = os.path.join(os.path.dirname(
-                self.pipe_iface_file), pipe_path)
+            abs = os.path.join(os.path.dirname(self.pipe_iface_file), pipe_path)
             if os.path.exists(abs):
                 _LOGGER.debug(
-                    "Path relative to pipeline interface made absolute: {}".
-                        format(abs))
+                    "Path relative to pipeline interface made absolute: {}".format(abs)
+                )
                 _set_in_dict(self, keys, abs)
                 return
             _LOGGER.debug("Expanded path: {}".format(pipe_path))
             _set_in_dict(self, keys, pipe_path)
 
-    def _validate(self, schema_src, exclude_case=False, flavor=None):
+    def _validate(self, schema_src, exclude_case=False, flavor="generic"):
         """
-        Generic function to validate object against a schema
+        Generic function to validate the object against a schema
 
         :param str schema_src: schema source to validate against, URL or path
         :param bool exclude_case: whether to exclude validated objects
             from the error. Useful when used ith large projects
         :param str flavor: type of the pipeline schema to use
         """
-        schema_source = schema_src.format(flavor if flavor else "generic")
-        schemas = read_schema(schema_source)
-        for schema in schemas:
+        schema_source = schema_src.format(flavor)
+        for schema in read_schema(schema_source):
             try:
                 jsonschema.validate(self, schema)
-                _LOGGER.debug("Successfully validated {} against schema: {}".
-                              format(self.__class__.__name__, schema_source))
+                _LOGGER.debug(
+                    f"Successfully validated {self.__class__.__name__} "
+                    f"against schema: {schema_source}"
+                )
             except jsonschema.exceptions.ValidationError as e:
                 if not exclude_case:
                     raise e
-                raise jsonschema.exceptions.ValidationError(e.message)
+                raise jsonschema.exceptions.ValidationError(e.message)
```

### Comparing `looper-1.3.2/looper/processed_project.py` & `looper-1.4.0/looper/processed_project.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,141 @@
 """
 Processed Project manipulation functions.
-Will be moved to a separate package
+These functions are used to process pipestat-compatible schema,
+but the report generation approach has changed.
+"""
+
+__author__ = "Michal Stolarczyk"
+__email__ = "michal@virginia.edu"
+
+# import os
+# from collections.abc import Mapping
+# from copy import copy
+# from logging import getLogger
+
+# from eido.const import *
+# from eido.exceptions import *
+# from peppy.project import Project
+# from peppy.sample import Sample
+# from pipestat import SCHEMA_TYPE_KEY, SchemaError
+# from ubiquerg import expandpath
+
+# _LOGGER = getLogger(__name__)
+# PATH_KEY = "path"
+# THUMB_PATH_KEY = "thumbnail_path"
+# PATH_LIKE = [PATH_KEY, THUMB_PATH_KEY]
+
+
+# def _populate_paths_in_schema(object, schema):
+#     """
+#     Populate path-like object attributes with other object attributes
+#     based on a defined template, e.g. '/Users/x/test_{name}/{genome}_file.txt'
+
+#     :param Mapping object: object with attributes to populate path template with
+#     :param dict schema: schema with path attributes defined, e.g.
+#         output of read_schema function
+#     :return Mapping: object with path templates populated
+#     """
+
+#     def _recurse_and_populate(mapping, object):
+#         """
+#         Recursively populate paths and thumbnail_paths templates in a mapping
+
+#         :param any mapping: a potential mapping with paths to populate
+#         :param Mapping object: object with attributes to populate path
+#             template with
+#         :return any: potentially populated object
+#         """
+#         if isinstance(mapping, Mapping):
+#             for k, v in mapping.items():
+#                 if isinstance(v, Mapping):
+#                     _recurse_and_populate(v, object)
+#                 elif k in PATH_LIKE:
+#                     try:
+#                         mapping[k] = expandpath(v.format(**dict(object.items())))
+#                     except Exception as e:
+#                         _LOGGER.warning(
+#                             f"Caught exception: {getattr(e, 'message', repr(e))}."
+#                             f"\nCould not populate template in schema: {v}"
+#                         )
+#                     else:
+#                         _LOGGER.debug(f"Populated: {mapping[k]}")
+#         return mapping
+
+#     for k, v in schema.items():
+#         if "value" not in v:
+#             continue
+#         if SCHEMA_TYPE_KEY not in v:
+#             raise SchemaError(
+#                 f"'{SCHEMA_TYPE_KEY}' not found in '{k}' section "
+#                 f"of the output schema"
+#             )
+#         schema[k] = _recurse_and_populate(v, object)
+#     return schema
+
+
+# def populate_sample_paths(sample, schema):
+#     """
+#     Populate path-like Sample attributes with other object attributes
+#     based on a defined template, e.g. '/Users/x/test_{name}/{genome}_file.txt'
+
+#     :param peppy.Sample sample: sample to populate paths in
+#     :param Iterable[dict] schema: schema with path attributes defined, e.g.
+#         output of read_schema function
+#     :return Mapping: Sample with path templates populated
+#     """
+#     # TODO: merge this and 'populate_project_paths' into one?
+#     if not isinstance(sample, Sample):
+#         raise TypeError("Can only populate paths in peppy.Sample objects")
+#     for k, v in _populate_paths_in_schema(sample, copy(schema)).items():
+#         if "value" in v:
+#             setattr(sample, k, v["value"])
+#     return sample
+
+
+# def populate_project_paths(project, schema):
+#     """
+#     Populate path-like Project attributes with other object attributes
+#     based on a defined template, e.g. '/Users/x/test_{name}/{genome}_file.txt'
+
+#     :param peppy.Project project: project to populate paths in
+#     :param dict schema: schema with path attributes defined, e.g.
+#         output of read_schema function
+#     :return Mapping: Project with path templates populated
+#     """
+#     for k, v in _populate_paths_in_schema(project.config, copy(schema)).items():
+#         if "value" in v:
+#             setattr(project, k, v["value"])
+#     return project
+
+
+# def get_project_outputs(project, schema):
+#     """
+#     Get project level outputs, where the path-like attributes are populated with
+#     project attributes
+
+#     :param peppy.Project project: project o get the set of outputs for
+#     :param Iterable[dict] schema: pipestat schema to source the outputs for
+#     :return attmap.PathExAttMap: mapping with populated path-like attributes
+#     """
+#     from attmap import PathExAttMap
+
+#     schema = schema[-1]  # use only first schema, in case there are imports
+#     populated = populate_project_paths(project, schema)
+#     return PathExAttMap({k: getattr(populated, k) for k in schema.keys()})
+"""
+Processed Project manipulation functions, required pipelines with no pipestat support (old schema)
 """
 import os
 from logging import getLogger
 
 from eido.const import *
 from eido.exceptions import *
-
-from peppy.sample import Sample
 from peppy.project import Project
-
-__author__ = "Michal Stolarczyk"
-__email__ = "michal@virginia.edu"
+from peppy.sample import Sample
 
 _LOGGER = getLogger(__name__)
 PATH_KEY = "path"
 THUMB_PATH_KEY = "thumbnail_path"
 PATH_LIKE = [PATH_KEY, THUMB_PATH_KEY]
 
 
@@ -48,25 +167,29 @@
     s = schema[PROP_KEY]
     path_sects = _get_path_sect_keys(s)
     for ps in path_sects:
         templ = s[ps][PATH_KEY]
         try:
             populated = templ.format(**dict(object.items()))
         except Exception as e:
-            _LOGGER.warning("Caught exception: {}.\n"
-                            "Could not populate path: {}".
-                            format(getattr(e, 'message', repr(e)), templ))
+            _LOGGER.warning(
+                "Caught exception: {}.\n"
+                "Could not populate path: {}".format(
+                    getattr(e, "message", repr(e)), templ
+                )
+            )
         else:
             setattr(object, ps, populated)
             _LOGGER.debug("Path set to: {}".format(object[ps]))
             if check_exist and not os.path.exists(object[ps]):
                 missing.append(object[ps])
     if missing:
-        raise PathAttrNotFoundError("Path attributes not found:\n- {}".
-                                    format("\n- ".join(missing)))
+        raise PathAttrNotFoundError(
+            "Path attributes not found:\n- {}".format("\n- ".join(missing))
+        )
 
 
 def populate_sample_paths(sample, schema, check_exist=False):
     """
     Populate path-like Sample attributes with other object attributes
     based on a defined template, e.g. '/Users/x/test_{name}/{genome}_file.txt'
 
@@ -76,16 +199,15 @@
     :param bool check_exist: whether the paths should be check for existence
     :return Mapping: Sample with path templates populated
     """
     if not isinstance(sample, Sample):
         raise TypeError("Can only populate paths in peppy.Sample objects")
     # schema = schema[-1]  # use only first schema, in case there are imports
     if PROP_KEY in schema and "samples" in schema[PROP_KEY]:
-        _populate_paths(sample, schema[PROP_KEY]["samples"]["items"],
-                        check_exist)
+        _populate_paths(sample, schema[PROP_KEY]["samples"]["items"], check_exist)
 
 
 def populate_project_paths(project, schema, check_exist=False):
     """
     Populate path-like Project attributes with other object attributes
     based on a defined template, e.g. '/Users/x/test_{name}/{genome}_file.txt'
 
@@ -103,17 +225,18 @@
 def get_project_outputs(project, schema):
     """
     Get project level outputs with path-like attributes populated with
     project attributes
 
     :param peppy.Project project:
     :param Iterable[dict] schema:
-    :return attmap.PathExAttMap: mapping with populated path-like attributes
+    :return yacman.YAMLConfigManager: mapping with populated path-like attributes
     """
-    from attmap import PathExAttMap
+    from yacman import YAMLConfigManager
+
     # if not any([isinstance(project, Project),
     #             issubclass(type(project), Project)]):
     #     raise TypeError("Can only populate paths in peppy.Project "
     #                     "objects or it subclasses")
     schema = schema[-1]  # use only first schema, in case there are imports
     if PROP_KEY not in schema:
         raise EidoSchemaInvalidError("Schema is missing properties section.")
@@ -122,10 +245,12 @@
     path_sects = _get_path_sect_keys(s, keys=PATH_LIKE)
     for ps in path_sects:
         res[ps] = s[ps]
         for p in PATH_LIKE:
             try:
                 res[ps][p] = s[ps][p].format(**dict(project.items()))
             except Exception as e:
-                _LOGGER.debug("Caught exception: {}.\n Could not populate {} "
-                              "path".format(p, str(e)))
-    return PathExAttMap(res)
+                _LOGGER.debug(
+                    "Caught exception: {}.\n Could not populate {} "
+                    "path".format(p, str(e))
+                )
+    return YAMLConfigManager(res)
```

### Comparing `looper-1.3.2/looper/schemas/pipeline_interface_schema_generic.yaml` & `looper-1.4.0/looper/schemas/pipeline_interface_schema_sample.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-description: pipeline interface schema
+description: sample pipeline interface schema
 
 properties:
   pipeline_name:
     type: string
     pattern: "^\\S*$"
     description: "name of the pipeline with no whitespaces"
   pipeline_type:
     type: string
-    enum: ["project", "sample"]
-    description: "type of the pipeline, either 'project' or 'sample'"
+    const: "sample"
+    description: "type of the pipeline, must be 'sample'"
   command_template:
     type: string
     description: "Jinja2-like template to construct the command to run"
   var_templates:
     type: object
     description: "Jinja2-like templates to construct submission variables"
   pre_submit:
@@ -41,8 +41,8 @@
         description: "Bulker registry path identifying the crate to use"
       docker_image:
         type: string
         description: "Docker image identifier"
       singularity_image:
         type: string
         description: "Singularity image identifier"
-required: [pipeline_name, pipeline_type, command_template]
+required: [pipeline_name, pipeline_type, command_template]
```

### Comparing `looper-1.3.2/looper/schemas/pipeline_interface_schema_project.yaml` & `looper-1.4.0/looper/schemas/pipeline_interface_schema_project.yaml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -41,8 +41,8 @@
         description: "Bulker registry path identifying the crate to use"
       docker_image:
         type: string
         description: "Docker image identifier"
       singularity_image:
         type: string
         description: "Singularity image identifier"
-required: [pipeline_name, pipeline_type, command_template]
+required: [pipeline_name, pipeline_type, command_template]
```

### Comparing `looper-1.3.2/looper/utils.py` & `looper-1.4.0/looper/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 """ Helpers without an obvious logical home. """
 
-from collections import defaultdict, Iterable
-from logging import getLogger
+import argparse
+from collections import defaultdict, namedtuple
 import glob
+import itertools
+from logging import getLogger
 import os
-from .const import *
-from .exceptions import MisconfigurationException
-from peppy.const import *
-from peppy import Project as peppyProject
+import sys
+from typing import *
+
 import jinja2
 import yaml
-import argparse
+from peppy import Project as peppyProject
+from peppy.const import *
 from ubiquerg import convert_value, expandpath
 
+from .const import *
+from .exceptions import MisconfigurationException
+
 _LOGGER = getLogger(__name__)
 
 
 def fetch_flag_files(prj=None, results_folder="", flags=FLAGS):
     """
     Find all flag file paths for the given project.
 
@@ -72,20 +77,26 @@
     :param peppy.Sample sample: sample object of interest
     :param str pl_name: name of the pipeline for which flag(s) should be found
     :return Iterable[str]: collection of flag file path(s) associated with the
         given sample for the given project
     """
     sfolder = sample_folder(prj=prj, sample=sample)
     if not os.path.isdir(sfolder):
-        _LOGGER.debug("Results folder ({}) doesn't exist for sample {}".
-                      format(sfolder, str(sample)))
+        _LOGGER.debug(
+            "Results folder ({}) doesn't exist for sample {}".format(
+                sfolder, str(sample)
+            )
+        )
         return []
     folder_contents = [os.path.join(sfolder, f) for f in os.listdir(sfolder)]
-    return [x for x in folder_contents if os.path.splitext(x)[1] == ".flag"
-            and os.path.basename(x).startswith(pl_name)]
+    return [
+        x
+        for x in folder_contents
+        if os.path.splitext(x)[1] == ".flag" and os.path.basename(x).startswith(pl_name)
+    ]
 
 
 def grab_project_data(prj):
     """
     From the given Project, grab Sample-independent data.
 
     There are some aspects of a Project of which it's beneficial for a Sample
@@ -98,47 +109,68 @@
     :param Project prj: Project from which to grab data
     :return Mapping: Sample-independent data sections from given Project
     """
     if not prj:
         return {}
 
     try:
-        data = prj[CONFIG_KEY]
+        return prj[CONFIG_KEY]
     except KeyError:
         _LOGGER.debug("Project lacks section '%s', skipping", CONFIG_KEY)
-    return data
 
 
 def sample_folder(prj, sample):
     """
     Get the path to this Project's root folder for the given Sample.
 
     :param AttributeDict | Project prj: project with which sample is associated
     :param Mapping sample: Sample or sample data for which to get root output
         folder path.
     :return str: this Project's root folder for the given Sample
     """
-    return os.path.join(prj.results_folder,
-                        sample[SAMPLE_NAME_ATTR])
+    return os.path.join(prj.results_folder, sample[prj.sample_table_index])
 
 
-def get_file_for_project(prj, appendix):
+def get_file_for_project(prj, pipeline_name, appendix=None, directory=None):
+    """
+    Create a path to the file for the current project.
+    Takes the possibility of amendment being activated at the time
+
+    Format of the output path:
+    {output_dir}/{directory}/{p.name}_{pipeline_name}_{active_amendments}_{appendix}
+
+    :param looper.Project prj: project object
+    :param str pipeline_name: name of the pipeline to get the file for
+    :param str appendix: the appendix of the file to create the path for,
+        like 'objs_summary.tsv' for objects summary file
+    :return str: path to the file
+    """
+    fp = os.path.join(
+        prj.output_dir, directory or "", f"{prj[NAME_KEY]}_{pipeline_name}"
+    )
+    if hasattr(prj, "amendments") and getattr(prj, "amendments"):
+        fp += f"_{'_'.join(prj.amendments)}"
+    fp += f"_{appendix}"
+    return fp
+
+
+def get_file_for_project_old(prj, appendix):
     """
     Create a path to the file for the current project.
     Takes the possibility of amendment being activated at the time
 
     :param looper.Project prj: project object
     :param str appendix: the appendix of the file to create the path for,
         like 'objs_summary.tsv' for objects summary file
     :return str: path to the file
     """
     fp = os.path.join(prj.output_dir, prj[NAME_KEY])
     if hasattr(prj, AMENDMENTS_KEY) and getattr(prj, AMENDMENTS_KEY):
-        fp += '_' + '_'.join(getattr(prj, AMENDMENTS_KEY))
-    fp += '_' + appendix
+        fp += "_" + "_".join(getattr(prj, AMENDMENTS_KEY))
+    fp += "_" + appendix
     return fp
 
 
 def jinja_render_template_strictly(template, namespaces):
     """
     Render a command string in the provided namespaces context.
 
@@ -148,47 +180,50 @@
     :param str template: command template do be filled in with the
         variables in the provided namespaces. For example:
         "prog.py --name {project.name} --len {sample.len}"
     :param Mapping[Mapping[str] namespaces: context for command rendering.
         Possible namespaces are: looper, project, sample, pipeline
     :return str: rendered command
     """
+
     def _finfun(x):
         """
         A callable that can be used to process the result of a variable
         expression before it is output. Joins list elements
         """
         return " ".join(x) if isinstance(x, list) else x
 
-    env = jinja2.Environment(undefined=jinja2.StrictUndefined,
-                             variable_start_string="{",
-                             variable_end_string="}",
-                             finalize=_finfun)
+    env = jinja2.Environment(
+        undefined=jinja2.StrictUndefined,
+        variable_start_string="{",
+        variable_end_string="}",
+        finalize=_finfun,
+    )
     templ_obj = env.from_string(template)
     try:
         rendered = templ_obj.render(**namespaces)
-    except jinja2.exceptions.UndefinedError:
-        _LOGGER.error(f"Attributes in namespaces "
-                      f"({', '.join(list(namespaces.keys()))}) missing for "
-                      f"the following template: '{template}'")
-        raise
+    except jinja2.exceptions.UndefinedError as e:
+        _LOGGER.error("Error populating command template: " + str(e))
+        _LOGGER.debug(f"({', '.join(list(namespaces.keys()))}) missing for ")
+        _LOGGER.debug(f"Template: '{template}'")
+        raise e
     _LOGGER.debug("rendered arg str: {}".format(rendered))
     return rendered
 
 
 def read_yaml_file(filepath):
     """
     Read a YAML file
 
     :param str filepath: path to the file to read
     :return dict: read data
     """
     data = None
     if os.path.exists(filepath):
-        with open(filepath, 'r') as f:
+        with open(filepath, "r") as f:
             data = yaml.safe_load(f)
     return data
 
 
 def enrich_args_via_cfg(parser_args, aux_parser):
     """
     Read in a looper dotfile and set arguments.
@@ -196,17 +231,19 @@
     Priority order: CLI > dotfile/config > parser default
 
     :param argparse.Namespace parser_args: parsed args by the original parser
     :param argparse.Namespace aux_parser: parsed args by the a parser
         with defaults suppressed
     :return argparse.Namespace: selected argument values
     """
-    cfg_args_all = \
-        _get_subcommand_args(parser_args) \
-            if os.path.exists(parser_args.config_file) else dict()
+    cfg_args_all = (
+        _get_subcommand_args(parser_args)
+        if os.path.exists(parser_args.config_file)
+        else dict()
+    )
     result = argparse.Namespace()
     cli_args, _ = aux_parser.parse_known_args()
     for dest in vars(parser_args):
         if dest not in POSITIONAL or not hasattr(result, dest):
             if dest in cli_args:
                 x = getattr(cli_args, dest)
                 r = convert_value(x) if isinstance(x, str) else x
@@ -231,42 +268,89 @@
     with '_'), which strongly relies on argument parser using default
     destinations.
 
     :param argparser.Namespace parser_args: argument namespace
     :return dict: mapping of argument destinations to their values
     """
     args = dict()
-    cfg = peppyProject(parser_args.config_file,
-                       defer_samples_creation=True,
-                       amendments=parser_args.amend)
-    if CONFIG_KEY in cfg and LOOPER_KEY in cfg[CONFIG_KEY] \
-            and CLI_KEY in cfg[CONFIG_KEY][LOOPER_KEY]:
+    cfg = peppyProject(
+        parser_args.config_file,
+        defer_samples_creation=True,
+        amendments=parser_args.amend,
+    )
+    if (
+        CONFIG_KEY in cfg
+        and LOOPER_KEY in cfg[CONFIG_KEY]
+        and CLI_KEY in cfg[CONFIG_KEY][LOOPER_KEY]
+    ):
         try:
             cfg_args = cfg[CONFIG_KEY][LOOPER_KEY][CLI_KEY] or dict()
-            args = cfg_args[ALL_SUBCMD_KEY] or dict() \
-                if ALL_SUBCMD_KEY in cfg_args else dict()
-            args.update(cfg_args[parser_args.command] or dict()
-                        if parser_args.command in cfg_args else dict())
+            args = (
+                cfg_args[ALL_SUBCMD_KEY] or dict()
+                if ALL_SUBCMD_KEY in cfg_args
+                else dict()
+            )
+            args.update(
+                cfg_args[parser_args.command] or dict()
+                if parser_args.command in cfg_args
+                else dict()
+            )
         except (TypeError, KeyError, AttributeError, ValueError) as e:
             raise MisconfigurationException(
-                "Invalid '{}.{}' section in the config. Caught exception: {}".
-                    format(LOOPER_KEY, CLI_KEY, getattr(e, 'message', repr(e))))
+                "Invalid '{}.{}' section in the config. Caught exception: {}".format(
+                    LOOPER_KEY, CLI_KEY, getattr(e, "message", repr(e))
+                )
+            )
     if CONFIG_KEY in cfg and LOOPER_KEY in cfg[CONFIG_KEY]:
         try:
             if CLI_KEY in cfg[CONFIG_KEY][LOOPER_KEY]:
                 del cfg[CONFIG_KEY][LOOPER_KEY][CLI_KEY]
             args.update(cfg[CONFIG_KEY][LOOPER_KEY])
         except (TypeError, KeyError, AttributeError, ValueError) as e:
             raise MisconfigurationException(
-                "Invalid '{}' section in the config. Caught exception: {}".
-                    format(LOOPER_KEY, getattr(e, 'message', repr(e))))
+                "Invalid '{}' section in the config. Caught exception: {}".format(
+                    LOOPER_KEY, getattr(e, "message", repr(e))
+                )
+            )
     args = {k.replace("-", "_"): v for k, v in args.items()} if args else None
     return args
 
 
+def init_generic_pipeline():
+    # check for pipeline folder
+    try:
+        os.makedirs("pipeline")
+    except FileExistsError:
+        print("Pipeline folder already exists.")
+        pass
+
+    # Destination one level down from CWD in pipeline folder
+    dest_file = os.path.join(os.getcwd(), "pipeline", LOOPER_GENERIC_PIPELINE)
+
+    # Determine Lines for Generic Pipeline Interface
+    line1 = "pipeline_name: count_lines\n"
+    line2 = "pipeline_type: sample\n"
+    line3 = "output_schema: output_schema.yaml\n"
+    line4 = "var_templates:\n"
+    line5 = "  pipeline: '{looper.piface_dir}/count_lines.sh'\n"
+    line6 = "command_template: >\n"
+    line7 = "  {pipeline.var_templates.pipeline} {sample.file} --output-parent {looper.sample_output_folder}\n"
+    yaml_body = line1 + line2 + line3 + line4 + line5 + line6 + line7
+
+    # Write file
+    if not os.path.exists(dest_file):
+        with open(dest_file, mode="w") as file:
+            file.write(str(yaml_body))
+        print(f"Generic pipeline interface successfully created at: {dest_file}")
+    else:
+        print("Generic pipeline interface file already exists. Skipping creation.")
+
+    return True
+
+
 def init_dotfile(path, cfg_path, force=False):
     """
     Initialize looper dotfile
 
     :param str path: absolute path to the file to initialize
     :param str cfg_path: path to the config file. Absolute or relative to 'path'
     :param bool force: whether the existing file should be overwritten
@@ -274,43 +358,44 @@
     """
     if os.path.exists(path) and not force:
         print("Can't initialize, file exists: {}".format(path))
         return False
     cfg_path = expandpath(cfg_path)
     if not os.path.isabs(cfg_path):
         cfg_path = os.path.join(os.path.dirname(path), cfg_path)
-    assert os.path.exists(cfg_path), \
-        OSError("Provided config path is invalid. You must provide path "
-                "that is either absolute or relative to: {}".
-                format(os.path.dirname(path)))
+    assert os.path.exists(cfg_path), OSError(
+        "Provided config path is invalid. You must provide path "
+        "that is either absolute or relative to: {}".format(os.path.dirname(path))
+    )
     relpath = os.path.relpath(cfg_path, os.path.dirname(path))
-    with open(path, 'w') as dotfile:
+    with open(path, "w") as dotfile:
         yaml.dump({DOTFILE_CFG_PTH_KEY: relpath}, dotfile)
     print("Initialized looper dotfile: {}".format(path))
     return True
 
 
 def read_cfg_from_dotfile():
     """
     Read file path to the config file from the dotfile
 
     :return str: path to the config file read from the dotfile
     :raise MisconfigurationException: if the dotfile does not consist of the
         required key pointing to the PEP
     """
     dp = dotfile_path(must_exist=True)
-    with open(dp, 'r') as dotfile:
+    with open(dp, "r") as dotfile:
         dp_data = yaml.safe_load(dotfile)
     if DOTFILE_CFG_PTH_KEY in dp_data:
-        return os.path.join(os.path.dirname(dp),
-                            str(os.path.join(dp_data[DOTFILE_CFG_PTH_KEY])))
+        return os.path.join(
+            os.path.dirname(dp), str(os.path.join(dp_data[DOTFILE_CFG_PTH_KEY]))
+        )
     else:
         raise MisconfigurationException(
-            "Looper dotfile ({}) is missing '{}' key".
-                format(dp, DOTFILE_CFG_PTH_KEY))
+            "Looper dotfile ({}) is missing '{}' key".format(dp, DOTFILE_CFG_PTH_KEY)
+        )
 
 
 def dotfile_path(directory=os.getcwd(), must_exist=False):
     """
     Get the path to the looper dotfile
 
     If file existence is forced this function will look for it in
@@ -326,10 +411,151 @@
         return os.path.join(cur_dir, LOOPER_DOTFILE_NAME)
     while True:
         parent_dir = os.path.dirname(cur_dir)
         if LOOPER_DOTFILE_NAME in os.listdir(cur_dir):
             return os.path.join(cur_dir, LOOPER_DOTFILE_NAME)
         if cur_dir == parent_dir:
             # root, file does not exist
-            raise OSError("Looper dotfile ({}) not found in '{}' and all "
-                          "its parents".format(LOOPER_DOTFILE_NAME, directory))
+            raise OSError(
+                "Looper dotfile ({}) not found in '{}' and all "
+                "its parents".format(LOOPER_DOTFILE_NAME, directory)
+            )
         cur_dir = parent_dir
+
+
+class NatIntervalException(Exception):
+    """Subtype for errors specifically related to natural number interval"""
+
+    pass
+
+
+class NatIntervalInclusive(object):
+    def __init__(self, lo: int, hi: int):
+        super().__init__()
+        self._lo = lo
+        self._hi = hi
+        problems = self._invalidations()
+        if problems:
+            raise NatIntervalException(
+                f"{len(problems)} issues with interval on natural numbers: {', '.join(problems)}"
+            )
+
+    def __eq__(self, other) -> bool:
+        return type(other) == type(self) and self.to_tuple() == other.to_tuple()
+
+    def __hash__(self) -> int:
+        return hash(self.to_tuple())
+
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}: {self.to_tuple()}"
+
+    def __str__(self) -> str:
+        return f"{self.__class__.__name__}: {self.to_tuple()}"
+
+    def to_tuple(self) -> Tuple[int, int]:
+        return self.lo, self.hi
+
+    @property
+    def lo(self) -> int:
+        return self._lo
+
+    @property
+    def hi(self) -> int:
+        return self._hi
+
+    def _invalidations(self) -> Iterable[str]:
+        problems = []
+        if self.lo < 1:
+            problems.append(f"Interval must be on natural numbers: {self.lo}")
+        if self.hi < self.lo:
+            problems.append(
+                f"Upper bound must not be less than lower bound: {self.hi} < {self.lo}"
+            )
+        return problems
+
+    def to_range(self) -> Iterable[int]:
+        return range(self.lo, self.hi + 1)
+
+    @classmethod
+    def from_string(cls, s: str, upper_bound: int) -> "IntRange":
+        """
+        Create an instance from a string, e.g. command-line argument.
+
+        :param str s: The string to parse as an interval
+        :param int upper_bound: the default upper bound
+        """
+        if upper_bound < 1:
+            raise NatIntervalException(f"Upper bound must be positive: {upper_bound}")
+
+        # Determine delimiter, invalidating presence of multiple occurrences.
+        delim_histo = defaultdict(int)
+        candidates = [":", "-"]
+        for c in s:
+            if c in candidates:
+                delim_histo[c] += 1
+        seps = [sep for sep, num_occ in delim_histo.items() if num_occ == 1]
+        if len(seps) != 1:
+            raise NatIntervalException(
+                f"Did not find exactly one candidate delimiter with occurrence count of 1: {delim_histo}"
+            )
+        sep = seps[0]
+
+        # Use the determined delimiter.
+        lo, hi = s.split(sep)
+        if lo == "" and hi == "":
+            # We could do an interval like [1, upper_bound], but this is nonsensical as input.
+            raise NatIntervalException(
+                f"Parsed both lower and upper limit as empty from given arg: {s}"
+            )
+        try:
+            lo = 1 if lo == "" else int(lo)
+            hi = upper_bound if hi == "" else min(int(hi), upper_bound)
+        except ValueError as e:
+            raise NatIntervalException(str(e))
+        return cls(lo, hi)
+
+
+def desired_samples_range_limited(arg: str, num_samples: int) -> Iterable[int]:
+    """
+    Create a contiguous interval of natural numbers. Used for _positive_ selection of samples.
+
+    Interpret given arg as upper bound (1-based) if it's a single value, but take the
+    minimum of that and the given number of samples. If arg is parseable as a range,
+    use that.
+
+    :param str arg: CLI specification of a range of samples to use, or as the greatest
+        1-based index of a sample to include
+    :param int num_samples: what to use as the upper bound on the 1-based index interval
+        if the given arg isn't a range but rather a single value.
+    :return: an iterable of 1-based indices into samples to select
+    """
+    try:
+        upper_bound = min(int(arg), num_samples)
+    except ValueError:
+        intv = NatIntervalInclusive.from_string(arg, upper_bound=num_samples)
+    else:
+        _LOGGER.debug("Limiting to {} of {} samples".format(upper_bound, num_samples))
+        intv = NatIntervalInclusive(1, upper_bound)
+    return intv.to_range()
+
+
+def desired_samples_range_skipped(arg: str, num_samples: int) -> Iterable[int]:
+    """
+    Create a contiguous interval of natural numbers. Used for _negative_ selection of samples.
+
+    :param str arg: CLI specification of a range of samples to use, or as the lowest
+        1-based index of a sample to skip
+    :param int num_samples: highest 1-based index of samples to include
+    :return: an iterable of 1-based indices into samples to select
+    """
+    try:
+        lower_bound = int(arg)
+    except ValueError:
+        intv = NatIntervalInclusive.from_string(arg, upper_bound=num_samples)
+        lower = range(1, intv.lo)
+        upper = range(intv.hi + 1, num_samples + 1)
+        return itertools.chain(lower, upper)
+    else:
+        if num_samples <= lower_bound:
+            return []
+        intv = NatIntervalInclusive(lower_bound + 1, num_samples)
+        return intv.to_range()
```

### Comparing `looper-1.3.2/looper.egg-info/PKG-INFO` & `looper-1.4.0/looper.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: looper
-Version: 1.3.2
+Version: 1.4.0
 Summary: A pipeline submission engine that parses sample inputs and submits pipelines for each sample.
 Home-page: https://github.com/pepkit/looper
 Author: Nathan Sheffield, Vince Reuter, Michal Stolarczyk, Johanna Klughammer, Andre Rendeiro
 License: BSD2
 Keywords: bioinformatics,sequencing,ngs
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # <img src="docs/img/looper_logo.svg" alt="looper logo" height="70">
- 
+
 ![Run pytests](https://github.com/pepkit/looper/workflows/Run%20pytests/badge.svg)
 [![PEP compatible](http://pepkit.github.io/img/PEP-compatible-green.svg)](http://pepkit.github.io)
-
-`Looper` is a pipeline submission engine. The typical use case is to run a bioinformatics pipeline across many different input samples. Instructions are in the [documentation](http://looper.databio.org/).
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 
+`Looper` is a pipeline submission engine. The typical use case is to run a bioinformatics pipeline across many different input samples. Instructions are in the [documentation](http://looper.databio.org/).
```

### Comparing `looper-1.3.2/setup.py` & `looper-1.4.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,86 +1,92 @@
 #! /usr/bin/env python
 
 import os
-from setuptools import setup
 import sys
 
+from setuptools import setup
 
 # Additional keyword arguments for setup().
 extra = {}
 
 
 # Ordinary dependencies
 DEPENDENCIES = []
 with open("requirements/requirements-all.txt", "r") as reqs_file:
     for line in reqs_file:
         if not line.strip():
             continue
-        #DEPENDENCIES.append(line.split("=")[0].rstrip("<>"))
+        # DEPENDENCIES.append(line.split("=")[0].rstrip("<>"))
         DEPENDENCIES.append(line)
 
 
 # numexpr for pandas
 try:
     import numexpr
 except ImportError:
     # No numexpr is OK for pandas.
     pass
 else:
     # pandas 0.20.2 needs updated numexpr; the claim is 2.4.6, but that failed.
     DEPENDENCIES.append("numexpr>=2.6.2")
 extra["install_requires"] = DEPENDENCIES
 
+
 # Additional files to include with package
 def get_static(name, condition=None):
-    static = [os.path.join(name, f) for f in os.listdir(
-            os.path.join(os.path.dirname(os.path.realpath(__file__)), name))]
+    static = [
+        os.path.join(name, f)
+        for f in os.listdir(
+            os.path.join(os.path.dirname(os.path.realpath(__file__)), name)
+        )
+    ]
     if condition is None:
         return static
     else:
         return [i for i in filter(lambda x: eval(condition), static)]
 
 
 # scripts to be added to the $PATH
 # scripts = get_static("scripts", condition="'.' in x")
 # scripts removed (TO remove this)
 scripts = None
 
 
-with open("looper/_version.py", 'r') as versionfile:
+with open("looper/_version.py", "r") as versionfile:
     version = versionfile.readline().split()[-1].strip("\"'\n")
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="looper",
     packages=["looper"],
     version=version,
     description="A pipeline submission engine that parses sample inputs and submits pipelines for each sample.",
     long_description=long_description,
-    long_description_content_type='text/markdown', 
+    long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: BSD License",
-        "Programming Language :: Python :: 2.7",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
-        "Topic :: Scientific/Engineering :: Bio-Informatics"
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Topic :: Scientific/Engineering :: Bio-Informatics",
     ],
     keywords="bioinformatics, sequencing, ngs",
     url="https://github.com/pepkit/looper",
-    author=u"Nathan Sheffield, Vince Reuter, Michal Stolarczyk, Johanna Klughammer, Andre Rendeiro",
+    author="Nathan Sheffield, Vince Reuter, Michal Stolarczyk, Johanna Klughammer, Andre Rendeiro",
     license="BSD2",
     entry_points={
-        "console_scripts": [
-            'looper = looper.__main__:main'
-        ],
+        "console_scripts": ["looper = looper.__main__:main"],
     },
     scripts=scripts,
-    package_data={'looper': ['submit_templates/*']},
+    package_data={"looper": ["submit_templates/*"]},
     include_package_data=True,
     test_suite="tests",
     tests_require=(["mock", "pytest"]),
-    setup_requires=(["pytest-runner"] if {"test", "pytest", "ptr"} & set(sys.argv) else []),
+    setup_requires=(
+        ["pytest-runner"] if {"test", "pytest", "ptr"} & set(sys.argv) else []
+    ),
     **extra
 )
```

