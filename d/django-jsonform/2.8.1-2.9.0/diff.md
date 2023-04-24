# Comparing `tmp/django-jsonform-2.8.1.tar.gz` & `tmp/django-jsonform-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/bharat/Projects/develop_python/django-jsonform/dist/tmpd5n532wc/django-jsonform-2.8.1.tar", last modified: Sun Mar 13 14:22:22 2022, max compression
+gzip compressed data, was "/home/bharat/Projects/develop_python/django-jsonform/dist/tmp4cmsrcg5/django-jsonform-2.9.0.tar", last modified: Fri Apr 22 16:35:00 2022, max compression
```

## Comparing `django-jsonform-2.8.1.tar` & `django-jsonform-2.9.0.tar`

### file list

```diff
@@ -1,55 +1,59 @@
-drwxrwxr-x   0 bharat    (1000) bharat    (1000)        0 2022-03-13 14:22:22.848504 django-jsonform-2.8.1/
--rw-rw-r--   0 bharat    (1000) bharat    (1000)     1478 2021-06-05 05:44:49.000000 django-jsonform-2.8.1/LICENSE.txt
--rw-rw-r--   0 bharat    (1000) bharat    (1000)      177 2021-09-15 10:40:20.000000 django-jsonform-2.8.1/MANIFEST.in
--rw-rw-r--   0 bharat    (1000) bharat    (1000)     3551 2022-03-13 14:22:22.848504 django-jsonform-2.8.1/PKG-INFO
--rw-rw-r--   0 bharat    (1000) bharat    (1000)     2369 2022-02-10 11:07:36.000000 django-jsonform-2.8.1/README.md
-drwxrwxr-x   0 bharat    (1000) bharat    (1000)        0 2022-03-13 14:22:22.840504 django-jsonform-2.8.1/django_jsonform/
--rw-rw-r--   0 bharat    (1000) bharat    (1000)       21 2022-03-13 14:20:34.000000 django-jsonform-2.8.1/django_jsonform/__init__.py
--rw-rw-r--   0 bharat    (1000) bharat    (1000)       63 2021-08-28 11:46:38.000000 django-jsonform-2.8.1/django_jsonform/admin.py
--rw-rw-r--   0 bharat    (1000) bharat    (1000)       97 2021-08-29 05:25:11.000000 django-jsonform-2.8.1/django_jsonform/apps.py
-drwxrwxr-x   0 bharat    (1000) bharat    (1000)        0 2022-03-13 14:22:22.840504 django-jsonform-2.8.1/django_jsonform/forms/
--rw-rw-r--   0 bharat    (1000) bharat    (1000)        0 2021-09-03 07:38:10.000000 django-jsonform-2.8.1/django_jsonform/forms/__init__.py
--rw-rw-r--   0 bharat    (1000) bharat    (1000)     3613 2021-09-05 03:41:20.000000 django-jsonform-2.8.1/django_jsonform/forms/compat.py
--rw-rw-r--   0 bharat    (1000) bharat    (1000)     2638 2022-02-09 20:04:58.000000 django-jsonform-2.8.1/django_jsonform/forms/fields.py
-drwxrwxr-x   0 bharat    (1000) bharat    (1000)        0 2022-03-13 14:22:22.844504 django-jsonform-2.8.1/django_jsonform/models/
--rw-rw-r--   0 bharat    (1000) bharat    (1000)        0 2021-09-03 07:38:10.000000 django-jsonform-2.8.1/django_jsonform/models/__init__.py
--rw-rw-r--   0 bharat    (1000) bharat    (1000)     3937 2021-09-05 03:41:22.000000 django-jsonform-2.8.1/django_jsonform/models/compat.py
--rw-rw-r--   0 bharat    (1000) bharat    (1000)     1666 2022-01-31 15:24:59.000000 django-jsonform-2.8.1/django_jsonform/models/fields.py
--rw-rw-r--   0 bharat    (1000) bharat    (1000)      531 2022-01-14 15:32:41.000000 django-jsonform-2.8.1/django_jsonform/parser.py
-drwxrwxr-x   0 bharat    (1000) bharat    (1000)        0 2022-03-13 14:22:22.836504 django-jsonform-2.8.1/django_jsonform/static/
-drwxrwxr-x   0 bharat    (1000) bharat    (1000)        0 2022-03-13 14:22:22.844504 django-jsonform-2.8.1/django_jsonform/static/django_jsonform/
-drwxrwxr-x   0 bharat    (1000) bharat    (1000)        0 2022-03-13 14:22:22.844504 django-jsonform-2.8.1/django_jsonform/static/django_jsonform/img/
--rw-rw-r--   0 bharat    (1000) bharat    (1000)     1374 2021-11-07 19:55:21.000000 django-jsonform-2.8.1/django_jsonform/static/django_jsonform/img/arrow-icons.svg
--rw-rw-r--   0 bharat    (1000) bharat    (1000)     2698 2021-11-07 20:06:15.000000 django-jsonform-2.8.1/django_jsonform/static/django_jsonform/img/control-icons.svg
--rw-rw-r--   0 bharat    (1000) bharat    (1000)      331 2021-08-15 05:02:59.000000 django-jsonform-2.8.1/django_jsonform/static/django_jsonform/img/icon-addlink.svg
--rw-rw-r--   0 bharat    (1000) bharat    (1000)      380 2021-08-18 12:15:08.000000 django-jsonform-2.8.1/django_jsonform/static/django_jsonform/img/icon-changelink.svg
--rw-rw-r--   0 bharat    (1000) bharat    (1000)      392 2021-08-15 05:09:43.000000 django-jsonform-2.8.1/django_jsonform/static/django_jsonform/img/icon-deletelink.svg
--rw-rw-r--   0 bharat    (1000) bharat    (1000)    30045 2022-03-11 05:37:06.000000 django-jsonform-2.8.1/django_jsonform/static/django_jsonform/react-json-form.min.js
--rw-rw-r--   0 bharat    (1000) bharat    (1000)    89489 2022-03-11 05:37:06.000000 django-jsonform-2.8.1/django_jsonform/static/django_jsonform/react-json-form.min.js.map
--rw-rw-r--   0 bharat    (1000) bharat    (1000)    11174 2022-03-08 04:31:01.000000 django-jsonform-2.8.1/django_jsonform/static/django_jsonform/style.css
-drwxrwxr-x   0 bharat    (1000) bharat    (1000)        0 2022-03-13 14:22:22.848504 django-jsonform-2.8.1/django_jsonform/static/django_jsonform/vendor/
--rw-rw-r--   0 bharat    (1000) bharat    (1000)   120585 2021-08-28 12:28:48.000000 django-jsonform-2.8.1/django_jsonform/static/django_jsonform/vendor/react-dom.production.min.js
--rw-rw-r--   0 bharat    (1000) bharat    (1000)    11440 2021-08-28 12:27:59.000000 django-jsonform-2.8.1/django_jsonform/static/django_jsonform/vendor/react.production.min.js
-drwxrwxr-x   0 bharat    (1000) bharat    (1000)        0 2022-03-13 14:22:22.836504 django-jsonform-2.8.1/django_jsonform/templates/
-drwxrwxr-x   0 bharat    (1000) bharat    (1000)        0 2022-03-13 14:22:22.848504 django-jsonform-2.8.1/django_jsonform/templates/django_jsonform/
--rw-rw-r--   0 bharat    (1000) bharat    (1000)     1565 2022-02-14 04:30:25.000000 django-jsonform-2.8.1/django_jsonform/templates/django_jsonform/editor.html
--rw-rw-r--   0 bharat    (1000) bharat    (1000)       60 2022-01-15 15:23:26.000000 django-jsonform-2.8.1/django_jsonform/tests.py
--rw-rw-r--   0 bharat    (1000) bharat    (1000)      156 2021-08-28 12:23:05.000000 django-jsonform-2.8.1/django_jsonform/urls.py
--rw-rw-r--   0 bharat    (1000) bharat    (1000)     1003 2022-01-14 18:07:58.000000 django-jsonform-2.8.1/django_jsonform/utils.py
--rw-rw-r--   0 bharat    (1000) bharat    (1000)      501 2021-08-29 04:43:25.000000 django-jsonform-2.8.1/django_jsonform/views.py
--rw-rw-r--   0 bharat    (1000) bharat    (1000)     1479 2022-02-13 05:19:35.000000 django-jsonform-2.8.1/django_jsonform/widgets.py
-drwxrwxr-x   0 bharat    (1000) bharat    (1000)        0 2022-03-13 14:22:22.840504 django-jsonform-2.8.1/django_jsonform.egg-info/
--rw-rw-r--   0 bharat    (1000) bharat    (1000)     3551 2022-03-13 14:22:22.000000 django-jsonform-2.8.1/django_jsonform.egg-info/PKG-INFO
--rw-rw-r--   0 bharat    (1000) bharat    (1000)     1496 2022-03-13 14:22:22.000000 django-jsonform-2.8.1/django_jsonform.egg-info/SOURCES.txt
--rw-rw-r--   0 bharat    (1000) bharat    (1000)        1 2022-03-13 14:22:22.000000 django-jsonform-2.8.1/django_jsonform.egg-info/dependency_links.txt
--rw-rw-r--   0 bharat    (1000) bharat    (1000)        1 2021-08-29 04:37:34.000000 django-jsonform-2.8.1/django_jsonform.egg-info/not-zip-safe
--rw-rw-r--   0 bharat    (1000) bharat    (1000)       12 2022-03-13 14:22:22.000000 django-jsonform-2.8.1/django_jsonform.egg-info/requires.txt
--rw-rw-r--   0 bharat    (1000) bharat    (1000)       22 2022-03-13 14:22:22.000000 django-jsonform-2.8.1/django_jsonform.egg-info/top_level.txt
--rw-rw-r--   0 bharat    (1000) bharat    (1000)     1173 2022-03-13 14:22:22.852504 django-jsonform-2.8.1/setup.cfg
--rw-rw-r--   0 bharat    (1000) bharat    (1000)       39 2020-02-12 10:38:35.000000 django-jsonform-2.8.1/setup.py
-drwxrwxr-x   0 bharat    (1000) bharat    (1000)        0 2022-03-13 14:22:22.848504 django-jsonform-2.8.1/tests/
--rw-rw-r--   0 bharat    (1000) bharat    (1000)        0 2022-01-17 14:06:07.000000 django-jsonform-2.8.1/tests/__init__.py
--rw-rw-r--   0 bharat    (1000) bharat    (1000)      362 2022-02-10 05:27:26.000000 django-jsonform-2.8.1/tests/__main__.py
--rw-rw-r--   0 bharat    (1000) bharat    (1000)      564 2022-02-10 05:26:01.000000 django-jsonform-2.8.1/tests/django_settings.py
--rw-rw-r--   0 bharat    (1000) bharat    (1000)      771 2022-01-17 14:17:31.000000 django-jsonform-2.8.1/tests/test_utils.py
--rw-rw-r--   0 bharat    (1000) bharat    (1000)     1275 2022-02-10 15:01:38.000000 django-jsonform-2.8.1/tests/test_widgets.py
+drwxrwxr-x   0 bharat    (1000) bharat    (1000)        0 2022-04-22 16:35:00.043818 django-jsonform-2.9.0/
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)     1478 2021-06-05 05:44:49.000000 django-jsonform-2.9.0/LICENSE.txt
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)      177 2021-09-15 10:40:20.000000 django-jsonform-2.9.0/MANIFEST.in
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)     3551 2022-04-22 16:35:00.043818 django-jsonform-2.9.0/PKG-INFO
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)     2369 2022-02-10 11:07:36.000000 django-jsonform-2.9.0/README.md
+drwxrwxr-x   0 bharat    (1000) bharat    (1000)        0 2022-04-22 16:35:00.035818 django-jsonform-2.9.0/django_jsonform/
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)       21 2022-04-22 15:17:11.000000 django-jsonform-2.9.0/django_jsonform/__init__.py
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)       63 2021-08-28 11:46:38.000000 django-jsonform-2.9.0/django_jsonform/admin.py
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)       97 2021-08-29 05:25:11.000000 django-jsonform-2.9.0/django_jsonform/apps.py
+drwxrwxr-x   0 bharat    (1000) bharat    (1000)        0 2022-04-22 16:35:00.035818 django-jsonform-2.9.0/django_jsonform/forms/
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)        0 2021-09-03 07:38:10.000000 django-jsonform-2.9.0/django_jsonform/forms/__init__.py
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)     3613 2021-09-05 03:41:20.000000 django-jsonform-2.9.0/django_jsonform/forms/compat.py
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)     2638 2022-02-09 20:04:58.000000 django-jsonform-2.9.0/django_jsonform/forms/fields.py
+drwxrwxr-x   0 bharat    (1000) bharat    (1000)        0 2022-04-22 16:35:00.035818 django-jsonform-2.9.0/django_jsonform/models/
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)        0 2021-09-03 07:38:10.000000 django-jsonform-2.9.0/django_jsonform/models/__init__.py
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)     3937 2021-09-05 03:41:22.000000 django-jsonform-2.9.0/django_jsonform/models/compat.py
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)     1666 2022-01-31 15:24:59.000000 django-jsonform-2.9.0/django_jsonform/models/fields.py
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)      531 2022-01-14 15:32:41.000000 django-jsonform-2.9.0/django_jsonform/parser.py
+drwxrwxr-x   0 bharat    (1000) bharat    (1000)        0 2022-04-22 16:35:00.031818 django-jsonform-2.9.0/django_jsonform/static/
+drwxrwxr-x   0 bharat    (1000) bharat    (1000)        0 2022-04-22 16:35:00.035818 django-jsonform-2.9.0/django_jsonform/static/django_jsonform/
+drwxrwxr-x   0 bharat    (1000) bharat    (1000)        0 2022-04-22 16:35:00.039818 django-jsonform-2.9.0/django_jsonform/static/django_jsonform/img/
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)     1374 2021-11-07 19:55:21.000000 django-jsonform-2.9.0/django_jsonform/static/django_jsonform/img/arrow-icons.svg
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)     2698 2021-11-07 20:06:15.000000 django-jsonform-2.9.0/django_jsonform/static/django_jsonform/img/control-icons.svg
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)      331 2021-08-15 05:02:59.000000 django-jsonform-2.9.0/django_jsonform/static/django_jsonform/img/icon-addlink.svg
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)      380 2021-08-18 12:15:08.000000 django-jsonform-2.9.0/django_jsonform/static/django_jsonform/img/icon-changelink.svg
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)      392 2021-08-15 05:09:43.000000 django-jsonform-2.9.0/django_jsonform/static/django_jsonform/img/icon-deletelink.svg
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)    30967 2022-04-22 14:52:30.000000 django-jsonform-2.9.0/django_jsonform/static/django_jsonform/react-json-form.min.js
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)    91573 2022-04-22 14:52:30.000000 django-jsonform-2.9.0/django_jsonform/static/django_jsonform/react-json-form.min.js.map
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)    13889 2022-04-22 15:03:33.000000 django-jsonform-2.9.0/django_jsonform/static/django_jsonform/style.css
+drwxrwxr-x   0 bharat    (1000) bharat    (1000)        0 2022-04-22 16:35:00.039818 django-jsonform-2.9.0/django_jsonform/static/django_jsonform/vendor/
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)   120585 2021-08-28 12:28:48.000000 django-jsonform-2.9.0/django_jsonform/static/django_jsonform/vendor/react-dom.production.min.js
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)    11440 2021-08-28 12:27:59.000000 django-jsonform-2.9.0/django_jsonform/static/django_jsonform/vendor/react.production.min.js
+drwxrwxr-x   0 bharat    (1000) bharat    (1000)        0 2022-04-22 16:35:00.031818 django-jsonform-2.9.0/django_jsonform/templates/
+drwxrwxr-x   0 bharat    (1000) bharat    (1000)        0 2022-04-22 16:35:00.039818 django-jsonform-2.9.0/django_jsonform/templates/django_jsonform/
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)     1565 2022-02-14 04:30:25.000000 django-jsonform-2.9.0/django_jsonform/templates/django_jsonform/editor.html
+drwxrwxr-x   0 bharat    (1000) bharat    (1000)        0 2022-04-22 16:35:00.039818 django-jsonform-2.9.0/django_jsonform/templatetags/
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)        0 2022-04-21 07:28:58.000000 django-jsonform-2.9.0/django_jsonform/templatetags/__init__.py
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)      539 2022-04-21 07:55:23.000000 django-jsonform-2.9.0/django_jsonform/templatetags/django_jsonform.py
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)       60 2022-01-15 15:23:26.000000 django-jsonform-2.9.0/django_jsonform/tests.py
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)      156 2021-08-28 12:23:05.000000 django-jsonform-2.9.0/django_jsonform/urls.py
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)     1003 2022-01-14 18:07:58.000000 django-jsonform-2.9.0/django_jsonform/utils.py
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)      501 2021-08-29 04:43:25.000000 django-jsonform-2.9.0/django_jsonform/views.py
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)     1479 2022-04-22 14:58:42.000000 django-jsonform-2.9.0/django_jsonform/widgets.py
+drwxrwxr-x   0 bharat    (1000) bharat    (1000)        0 2022-04-22 16:35:00.035818 django-jsonform-2.9.0/django_jsonform.egg-info/
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)     3551 2022-04-22 16:34:59.000000 django-jsonform-2.9.0/django_jsonform.egg-info/PKG-INFO
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)     1612 2022-04-22 16:35:00.000000 django-jsonform-2.9.0/django_jsonform.egg-info/SOURCES.txt
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)        1 2022-04-22 16:34:59.000000 django-jsonform-2.9.0/django_jsonform.egg-info/dependency_links.txt
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)        1 2021-08-29 04:37:34.000000 django-jsonform-2.9.0/django_jsonform.egg-info/not-zip-safe
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)       12 2022-04-22 16:34:59.000000 django-jsonform-2.9.0/django_jsonform.egg-info/requires.txt
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)       22 2022-04-22 16:34:59.000000 django-jsonform-2.9.0/django_jsonform.egg-info/top_level.txt
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)     1173 2022-04-22 16:35:00.043818 django-jsonform-2.9.0/setup.cfg
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)       39 2020-02-12 10:38:35.000000 django-jsonform-2.9.0/setup.py
+drwxrwxr-x   0 bharat    (1000) bharat    (1000)        0 2022-04-22 16:35:00.043818 django-jsonform-2.9.0/tests/
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)        0 2022-01-17 14:06:07.000000 django-jsonform-2.9.0/tests/__init__.py
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)      362 2022-02-10 05:27:26.000000 django-jsonform-2.9.0/tests/__main__.py
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)      564 2022-02-10 05:26:01.000000 django-jsonform-2.9.0/tests/django_settings.py
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)      774 2022-04-21 07:43:19.000000 django-jsonform-2.9.0/tests/test_templatetags.py
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)      771 2022-01-17 14:17:31.000000 django-jsonform-2.9.0/tests/test_utils.py
+-rw-rw-r--   0 bharat    (1000) bharat    (1000)     1275 2022-02-10 15:01:38.000000 django-jsonform-2.9.0/tests/test_widgets.py
```

### Comparing `django-jsonform-2.8.1/LICENSE.txt` & `django-jsonform-2.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-jsonform-2.8.1/PKG-INFO` & `django-jsonform-2.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-jsonform
-Version: 2.8.1
+Version: 2.9.0
 Summary: A user-friendly JSON editing form for Django admin.
 Home-page: https://www.github.com/bhch/django-jsonform
 Author: Bharat Chauhan
 Author-email: tell.bhch@gmail.com
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-jsonform Version: 2.8.1 Summary: A user-
+Metadata-Version: 2.1 Name: django-jsonform Version: 2.9.0 Summary: A user-
 friendly JSON editing form for Django admin. Home-page: https://www.github.com/
 bhch/django-jsonform Author: Bharat Chauhan Author-email: tell.bhch@gmail.com
 License: BSD-3-Clause Platform: UNKNOWN Classifier: Environment :: Web
 Environment Classifier: Framework :: Django Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: BSD License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

### Comparing `django-jsonform-2.8.1/README.md` & `django-jsonform-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `django-jsonform-2.8.1/django_jsonform/forms/compat.py` & `django-jsonform-2.9.0/django_jsonform/forms/compat.py`

 * *Files identical despite different names*

### Comparing `django-jsonform-2.8.1/django_jsonform/forms/fields.py` & `django-jsonform-2.9.0/django_jsonform/forms/fields.py`

 * *Files identical despite different names*

### Comparing `django-jsonform-2.8.1/django_jsonform/models/compat.py` & `django-jsonform-2.9.0/django_jsonform/models/compat.py`

 * *Files identical despite different names*

### Comparing `django-jsonform-2.8.1/django_jsonform/models/fields.py` & `django-jsonform-2.9.0/django_jsonform/models/fields.py`

 * *Files identical despite different names*

### Comparing `django-jsonform-2.8.1/django_jsonform/parser.py` & `django-jsonform-2.9.0/django_jsonform/parser.py`

 * *Files identical despite different names*

### Comparing `django-jsonform-2.8.1/django_jsonform/static/django_jsonform/img/arrow-icons.svg` & `django-jsonform-2.9.0/django_jsonform/static/django_jsonform/img/arrow-icons.svg`

 * *Files identical despite different names*

### Comparing `django-jsonform-2.8.1/django_jsonform/static/django_jsonform/img/control-icons.svg` & `django-jsonform-2.9.0/django_jsonform/static/django_jsonform/img/control-icons.svg`

 * *Files identical despite different names*

### Comparing `django-jsonform-2.8.1/django_jsonform/static/django_jsonform/react-json-form.min.js` & `django-jsonform-2.9.0/django_jsonform/static/django_jsonform/react-json-form.min.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -20,71 +20,71 @@
             return e.__proto__ = t, e
         })(e, t)
     }
 
     function n(e, t) {
         if (null == e) return {};
         var a, n, r = {},
-            i = Object.keys(e);
-        for (n = 0; n < i.length; n++) t.indexOf(a = i[n]) >= 0 || (r[a] = e[a]);
+            l = Object.keys(e);
+        for (n = 0; n < l.length; n++) t.indexOf(a = l[n]) >= 0 || (r[a] = e[a]);
         return r
     }
 
     function r(e) {
         var t = {},
             a = e.keys || e.properties;
         for (var n in a) {
-            var l = a[n],
-                o = l.type;
-            "list" === o ? o = "array" : "dict" === o && (o = "object"), t[n] = "array" === o ? i(l) : "object" === o ? r(l) : "boolean" === o ? l.default || !1 : "integer" === o || "number" === o ? l.default || null : l.default || ""
+            var i = a[n],
+                c = i.type;
+            "list" === c ? c = "array" : "dict" === c && (c = "object"), t[n] = "array" === c ? l(i) : "object" === c ? r(i) : "boolean" === c ? i.default || !1 : "integer" === c || "number" === c ? i.default || null : i.default || ""
         }
         return t
     }
 
-    function i(e) {
+    function l(e) {
         if (e.default) return e.default;
         var t = [],
             a = e.items.type;
-        return "list" === a ? a = "array" : "dict" === a && (a = "object"), "array" === a ? (t.push(i(e.items)), t) : "object" === a ? (t.push(r(e.items)), t) : ("multiselect" === e.items.widget || t.push("boolean" === a ? e.items.default || !1 : "integer" === a || "number" === a ? e.items.default || null : e.items.default || ""), t)
+        return "list" === a ? a = "array" : "dict" === a && (a = "object"), "array" === a ? (t.push(l(e.items)), t) : "object" === a ? (t.push(r(e.items)), t) : ("multiselect" === e.items.widget || t.push("boolean" === a ? e.items.default || !1 : "integer" === a || "number" === a ? e.items.default || null : e.items.default || ""), t)
     }
 
-    function l(e) {
+    function i(e) {
         var t = e.type;
-        return "list" === t ? t = "array" : "dict" === t && (t = "object"), "array" === t ? i(e) : "object" === t ? r(e) : "boolean" === t ? e.default || !1 : "integer" === t || "number" === t ? e.default || null : e.default || ""
+        return "list" === t ? t = "array" : "dict" === t && (t = "object"), "array" === t ? l(e) : "object" === t ? r(e) : "boolean" === t ? e.default || !1 : "integer" === t || "number" === t ? e.default || null : e.default || ""
     }
 
-    function o(e, t) {
+    function c(e, t) {
         var a = JSON.parse(JSON.stringify(e)),
             n = t.items.type;
         "list" === n ? n = "array" : "dict" === n && (n = "object");
         for (var r = 0; r < e.length; r++) {
-            var i = e[r];
-            "array" === n ? a[r] = o(i, t.items) : "object" === n ? a[r] = c(i, t.items) : "integer" !== n && "number" !== n || "" !== i || (a[r] = null)
+            var l = e[r];
+            "array" === n ? a[r] = c(l, t.items) : "object" === n ? a[r] = o(l, t.items) : "integer" !== n && "number" !== n || "" !== l || (a[r] = null)
         }
         return a
     }
 
-    function c(e, t) {
-        for (var a = JSON.parse(JSON.stringify(e)), n = t.keys || t.properties, r = [].concat(Object.keys(n)), i = 0; i < r.length; i++) {
-            var l = r[i],
-                s = n[l],
+    function o(e, t) {
+        for (var a = JSON.parse(JSON.stringify(e)), n = t.keys || t.properties, r = [].concat(Object.keys(n)), l = 0; l < r.length; l++) {
+            var i = r[l],
+                s = n[i],
                 m = s.type;
-            "list" === m ? m = "array" : "dict" === m && (m = "object"), a[l] = e.hasOwnProperty(l) ? "array" === m ? o(e[l], s) : "object" === m ? c(e[l], s) : "integer" !== m && "number" !== m || "" !== e[l] ? e[l] : null : "array" === m ? o([], s) : "object" === m ? c({}, s) : "boolean" !== m && ("integer" === m || "number" === m ? null : "")
+            "list" === m ? m = "array" : "dict" === m && (m = "object"), a[i] = e.hasOwnProperty(i) ? "array" === m ? c(e[i], s) : "object" === m ? o(e[i], s) : "integer" !== m && "number" !== m || "" !== e[i] ? e[i] : null : "array" === m ? c([], s) : "object" === m ? o({}, s) : "boolean" !== m && ("integer" === m || "number" === m ? null : "")
         }
         return a
     }
     var s = ["className"];
 
     function m(t) {
         var a = t.className,
             r = n(t, s);
         a || (a = "");
-        var i = a.split(" ");
+        var l = a.split(" ");
         a = "";
-        for (var l = 0; l < i.length; l++) a = a + "rjf-" + i[l] + "-button ";
+        for (var i = 0; i < l.length; i++) a = a + "rjf-" + l[i] + "-button ";
         return React.createElement("button", e({
             className: a.trim(),
             type: "button"
         }, r), r.children)
     }
 
     function p(e) {
@@ -132,16 +132,16 @@
                     t.props.onChange(e)
                 }, t.validateValue = function(e, t) {
                     return "hh" === e && t < 1 ? 1 : "hh" !== e && t < 0 ? 0 : "hh" === e && t > 12 ? 12 : "hh" !== e && t > 59 ? 59 : t
                 }, t.handleChange = function(e) {
                     var a, n = e.target.dataset.name,
                         r = e.target.value;
                     if (!isNaN(r)) {
-                        var i = t.validateValue(n, parseInt(r) || 0);
-                        "hh" !== n || "0" !== r && "" !== r && "00" !== r || 1 !== i || (i = 0), r.startsWith("0") && i < 10 && 0 !== i && (i = i.toString().padStart(2, "0")), t.sendValue(((a = {})[n] = "" !== r ? i.toString() : "", a))
+                        var l = t.validateValue(n, parseInt(r) || 0);
+                        "hh" !== n || "0" !== r && "" !== r && "00" !== r || 1 !== l || (l = 0), r.startsWith("0") && l < 10 && 0 !== l && (l = l.toString().padStart(2, "0")), t.sendValue(((a = {})[n] = "" !== r ? l.toString() : "", a))
                     }
                 }, t.handleKeyDown = function(e) {
                     var a;
                     if (38 === e.keyCode || 40 === e.keyCode) {
                         var n = e.target.dataset.name,
                             r = parseInt(e.target.value) || 0;
                         38 === e.keyCode ? r++ : 40 === e.keyCode && r--, t.sendValue(((a = {})[n] = t.validateValue(n, r).toString().padStart(2, "0"), a))
@@ -313,62 +313,82 @@
         E = ["label", "help_text", "error", "value", "options"],
         b = ["label", "help_text", "error", "value", "options"],
         k = ["label", "value"],
         N = ["label", "help_text", "error", "inputRef"];
 
     function j(e) {
         var t = e.label,
-            a = e.inputRef,
-            r = n(e, R);
-        return "string" === r.type && (r.type = "text"), a && (r.ref = a), null === r.value && (r.value = ""), React.createElement("div", null, t && React.createElement("label", null, t), React.createElement("input", r))
+            a = e.help_text,
+            r = e.inputRef,
+            l = n(e, R);
+        return "string" === l.type && (l.type = "text"), r && (l.ref = r), null === l.value && (l.value = ""), React.createElement("div", null, t && React.createElement("label", null, t), React.createElement("div", {
+            className: "rjf-input-group"
+        }, React.createElement("input", l), a && React.createElement("span", {
+            class: "rjf-help-text"
+        }, a)))
     }
 
     function w(e) {
         var t = e.label,
-            a = e.value,
-            r = n(e, y);
-        return t || (t = r.name.toUpperCase()), "bool" === r.type && (r.type = "checkbox"), void 0 === r.checked && (r.checked = a), "" !== r.checked && null != r.checked || (r.checked = !1), r.readOnly && (r.disabled = !0), React.createElement("div", null, React.createElement("label", null, React.createElement("input", r), " ", t))
+            a = e.help_text,
+            r = e.value,
+            l = n(e, y);
+        return t || (t = l.name.toUpperCase()), "bool" === l.type && (l.type = "checkbox"), void 0 === l.checked && (l.checked = r), "" !== l.checked && null != l.checked || (l.checked = !1), l.readOnly && (l.disabled = !0), React.createElement("div", {
+            className: "rjf-check-input"
+        }, React.createElement("label", null, React.createElement("input", l), " ", t), a && React.createElement("span", {
+            class: "rjf-help-text"
+        }, a))
     }
 
     function C(t) {
         var a = t.label,
-            r = t.value,
+            r = t.help_text,
+            l = t.value,
             i = t.options,
-            l = n(t, E);
-        return l.readOnly && (l.disabled = !0), React.createElement("div", null, React.createElement("label", null, a), i.map(function(t, a) {
-            var n, i;
-            return "object" == typeof t ? (n = t.label, i = t.value) : ("boolean" == typeof(n = t) && (n = g(n.toString())), i = t), React.createElement("label", {
-                key: n + "_" + i + "_" + a
-            }, React.createElement("input", e({}, l, {
-                value: i,
-                checked: i === r
+            c = n(t, E);
+        return c.readOnly && (c.disabled = !0), React.createElement("div", {
+            className: "rjf-check-input"
+        }, React.createElement("label", null, a), i.map(function(t, a) {
+            var n, r;
+            return "object" == typeof t ? (n = t.label, r = t.value) : ("boolean" == typeof(n = t) && (n = g(n.toString())), r = t), React.createElement("label", {
+                key: n + "_" + r + "_" + a
+            }, React.createElement("input", e({}, c, {
+                value: r,
+                checked: r === l
             })), " ", n)
-        }))
+        }), r && React.createElement("span", {
+            class: "rjf-help-text"
+        }, r))
     }
 
     function S(t) {
         var a = t.label,
-            r = t.value,
+            r = t.help_text,
+            l = t.value,
             i = t.options,
-            l = n(t, b);
-        return l.readOnly && (l.disabled = !0), React.createElement("div", null, a && React.createElement("label", null, a), React.createElement("select", e({
-            value: r || ""
-        }, l), React.createElement("option", {
+            c = n(t, b);
+        return c.readOnly && (c.disabled = !0), React.createElement("div", null, a && React.createElement("label", null, a), React.createElement("div", {
+            class: "rjf-input-group"
+        }, React.createElement("select", e({
+            value: l || ""
+        }, c), React.createElement("option", {
             disabled: !0,
             value: "",
             key: "__placehlder"
         }, "Select..."), i.map(function(e, t) {
             var a, n;
             return "object" == typeof e ? (a = e.label, n = e.value) : ("boolean" == typeof(a = e) && (a = g(a.toString())), n = e), React.createElement("option", {
                 value: n,
                 key: a + "_" + n + "_" + t
             }, a)
-        })))
+        })), r && React.createElement("span", {
+            class: "rjf-help-text"
+        }, r)))
     }
-    var O = function(e) {
+    var x = function(e) {
             function a(t) {
                 var a;
                 return (a = e.call(this, t) || this).handleChange = function(e) {
                     var t = [].concat(a.props.value);
                     e.target.checked ? t.push(e.target.value) : t = t.filter(function(t) {
                         return t !== e.target.value
                     }), a.props.onChange({
@@ -405,26 +425,27 @@
                     value: this.props.value.length ? this.props.value.length + " selected" : "Select...",
                     help_text: this.props.help_text,
                     error: this.props.error,
                     onClick: this.toggleOptions,
                     readOnly: !0,
                     inputRef: this.input,
                     className: "rjf-multiselect-field-input"
-                }), this.state.showOptions && React.createElement(x, {
+                }), this.state.showOptions && React.createElement(O, {
                     options: this.props.options,
                     value: this.props.value,
                     hideOptions: this.hideOptions,
                     onChange: this.handleChange,
                     containerRef: this.optionsContainer,
                     inputRef: this.input,
-                    disabled: this.props.readOnly
+                    disabled: this.props.readOnly,
+                    hasHelpText: this.props.help_text && 1
                 }))
             }, a
         }(React.Component),
-        x = function(e) {
+        O = function(e) {
             function a() {
                 for (var t, a = arguments.length, n = new Array(a), r = 0; r < a; r++) n[r] = arguments[r];
                 return (t = e.call.apply(e, [this].concat(n)) || this).handleClickOutside = function(e) {
                     !t.props.containerRef.current || t.props.containerRef.current.contains(e.target) || t.props.inputRef.current.contains(e.target) || t.props.hideOptions()
                 }, t
             }
             t(a, e);
@@ -434,50 +455,53 @@
             }, n.componentWillUnmount = function() {
                 document.removeEventListener("mousedown", this.handleClickOutside)
             }, n.render = function() {
                 var e = this;
                 return React.createElement("div", {
                     ref: this.props.containerRef
                 }, React.createElement("div", {
-                    className: "rjf-multiselect-field-options-container"
+                    className: "rjf-multiselect-field-options-container",
+                    style: this.props.hasHelpText ? {
+                        marginTop: "-15px"
+                    } : {}
                 }, this.props.options.map(function(t, a) {
                     var n, r;
                     "object" == typeof t ? (n = t.label, r = t.value) : ("boolean" == typeof(n = t) && (n = g(n.toString())), r = t);
-                    var i = e.props.value.indexOf(r) > -1,
-                        l = "rjf-multiselect-field-option";
-                    return i && (l += " selected"), e.props.disabled && (l += " disabled"), React.createElement("div", {
+                    var l = e.props.value.indexOf(r) > -1,
+                        i = "rjf-multiselect-field-option";
+                    return l && (i += " selected"), e.props.disabled && (i += " disabled"), React.createElement("div", {
                         key: n + "_" + r + "_" + a,
-                        className: l
+                        className: i
                     }, React.createElement("label", null, React.createElement("input", {
                         type: "checkbox",
                         onChange: e.props.onChange,
                         value: r,
-                        checked: i,
+                        checked: l,
                         disabled: e.props.disabled
                     }), " ", n))
                 })))
             }, a
         }(React.Component),
-        D = function(a) {
+        _ = function(a) {
             function r(e) {
                 var t;
                 return (t = a.call(this, e) || this).getFileName = function() {
                     return t.props.value ? "data-url" === t.props.type ? t.extractFileInfo(t.props.value).name : "file-url" === t.props.type ? t.props.value : "Unknown file" : ""
                 }, t.extractFileInfo = function(e) {
                     var t = function(e) {
                             var t, a = e.split(","),
                                 n = a[0].split(";"),
                                 r = n[0].replace("data:", ""),
-                                i = n.filter(function(e) {
+                                l = n.filter(function(e) {
                                     return "name" === e.split("=")[0]
                                 });
-                            t = 1 !== i.length ? "unknown" : i[0].split("=")[1];
-                            for (var l = atob(a[1]), o = [], c = 0; c < l.length; c++) o.push(l.charCodeAt(c));
+                            t = 1 !== l.length ? "unknown" : l[0].split("=")[1];
+                            for (var i = atob(a[1]), c = [], o = 0; o < i.length; o++) c.push(i.charCodeAt(o));
                             return {
-                                blob: new window.Blob([new Uint8Array(o)], {
+                                blob: new window.Blob([new Uint8Array(c)], {
                                     type: r
                                 }),
                                 name: t
                             }
                         }(e),
                         a = t.blob;
                     return {
@@ -499,30 +523,30 @@
                                     value: t.addNameToDataURL(r.result, n),
                                     name: t.props.name
                                 }
                             };
                             t.props.onChange(e)
                         }, r.readAsDataURL(a)
                     } else if ("file-url" === t.props.type) {
-                        var i = t.context.fileUploadEndpoint;
-                        if (!i) return console.error("Error: fileUploadEndpoint option need to be passed while initializing editor for enabling file uploads."), void alert("Files can't be uploaded.");
+                        var l = t.context.fileUploadEndpoint;
+                        if (!l) return console.error("Error: fileUploadEndpoint option need to be passed while initializing editor for enabling file uploads."), void alert("Files can't be uploaded.");
                         t.setState({
                             loading: !0
                         });
-                        var l = new FormData;
-                        l.append("field_name", t.context.fieldName), l.append("model_name", t.context.modelName), l.append("coordinates", JSON.stringify(t.props.name.split("-").slice(1))), l.append("file", e.target.files[0]), fetch(i, {
+                        var i = new FormData;
+                        i.append("field_name", t.context.fieldName), i.append("model_name", t.context.modelName), i.append("coordinates", JSON.stringify(t.props.name.split("-").slice(1))), i.append("file", e.target.files[0]), fetch(l, {
                             method: "POST",
                             headers: {
                                 "X-CSRFToken": document.cookie.split(";").filter(function(e) {
                                     return 0 === e.trim().indexOf("csrftoken=")
                                 }).length ? document.cookie.split(";").filter(function(e) {
                                     return 0 === e.trim().indexOf("csrftoken=")
                                 })[0].split("=")[1] : null
                             },
-                            body: l
+                            body: i
                         }).then(function(e) {
                             return e.json()
                         }).then(function(e) {
                             t.props.onChange({
                                 target: {
                                     type: "text",
                                     value: e.file_path,
@@ -536,59 +560,59 @@
                                 loading: !1
                             })
                         })
                     }
                 }, t.showFileBrowser = function() {
                     t.inputRef.current.click()
                 }, t.clearFile = function() {
-                    window.confirm("Do you want to remove this file?") && t.props.onChange({
+                    window.confirm("Do you want to remove this file?") && (t.props.onChange({
                         target: {
                             type: "text",
                             value: "",
                             name: t.props.name
                         }
-                    })
+                    }), t.inputRef.current && (t.inputRef.current.value = ""))
                 }, t.state = {
                     value: e.value,
                     fileName: t.getFileName(),
                     loading: !1
                 }, t.inputRef = React.createRef(), t
             }
             t(r, a);
-            var i = r.prototype;
-            return i.componentDidUpdate = function(e, t) {
+            var l = r.prototype;
+            return l.componentDidUpdate = function(e, t) {
                 this.props.value !== e.value && this.setState({
                     value: this.props.value,
                     fileName: this.getFileName()
                 })
-            }, i.render = function() {
+            }, l.render = function() {
                 var t = e({
                         value: r
                     }, this.props),
                     a = t.label,
                     r = t.value,
-                    i = n(t, k);
-                return i.type = "file", i.onChange = this.handleChange, i.readOnly && (i.disabled = !0), React.createElement("div", null, a && React.createElement("label", null, a), React.createElement("div", {
+                    l = n(t, k);
+                return l.type = "file", l.onChange = this.handleChange, l.readOnly && (l.disabled = !0), React.createElement("div", null, a && React.createElement("label", null, a), React.createElement("div", {
                     className: "rjf-file-field"
                 }, this.state.value && React.createElement("div", {
                     className: "rjf-current-file-name"
                 }, "Current file: ", React.createElement("span", null, this.state.fileName), " ", " ", React.createElement(m, {
                     className: "remove-file",
                     onClick: this.clearFile
                 }, "Clear")), this.state.value && !this.state.loading && "Change:", this.state.loading ? React.createElement("div", {
                     className: "rjf-file-field-loading"
                 }, React.createElement(p, null), " Uploading...") : React.createElement("div", {
                     className: "rjf-file-field-input"
-                }, React.createElement(j, e({}, i, {
+                }, React.createElement(j, e({}, l, {
                     inputRef: this.inputRef
                 })))))
             }, r
         }(React.Component);
-    D.contextType = v;
-    var I = function(e) {
+    _.contextType = v;
+    var D = function(e) {
             function a(t) {
                 var a;
                 return (a = e.call(this, t) || this).handleChange = function(e) {
                     a.updateHeight(e.target), a.props.onChange && a.props.onChange(e)
                 }, a.updateHeight = function(e) {
                     var t = e.offsetHeight - e.clientHeight;
                     e.style.height = "auto", e.style.height = e.scrollHeight + t + "px"
@@ -597,40 +621,45 @@
             t(a, e);
             var r = a.prototype;
             return r.componentDidMount = function() {
                 this.updateHeight(this.props.inputRef ? this.props.inputRef.current : this.inputRef.current)
             }, r.render = function() {
                 var e = this.props,
                     t = e.label,
-                    a = e.inputRef,
-                    r = n(e, N);
-                return delete r.type, r.ref = a || this.inputRef, r.onChange = this.handleChange, React.createElement("div", null, t && React.createElement("label", null, t), React.createElement("textarea", r))
+                    a = e.help_text,
+                    r = e.inputRef,
+                    l = n(e, N);
+                return delete l.type, l.ref = r || this.inputRef, l.onChange = this.handleChange, React.createElement("div", null, t && React.createElement("label", null, t), React.createElement("div", {
+                    className: "rjf-input-group"
+                }, React.createElement("textarea", l), a && React.createElement("span", {
+                    class: "rjf-help-text"
+                }, a)))
             }, a
         }(React.Component),
-        M = function(a) {
+        I = function(a) {
             function n(t) {
                 var n;
                 return (n = a.call(this, t) || this).getStateFromProps = function() {
                     var e = "",
                         t = "12",
                         a = "00",
                         r = "00",
-                        i = "000",
-                        l = "am";
+                        l = "000",
+                        i = "am";
                     if (n.props.value) {
-                        var o = new Date(n.props.value);
-                        e = o.getFullYear().toString().padStart(2, "0") + "-" + (o.getMonth() + 1).toString().padStart(2, "0") + "-" + o.getDate().toString().padStart(2, "0"), 0 === (t = o.getHours()) ? t = 12 : 12 === t ? l = "pm" : t > 12 && (t -= 12, l = "pm"), a = o.getMinutes(), r = o.getSeconds(), i = o.getMilliseconds(), t = t.toString().padStart(2, "0"), a = a.toString().padStart(2, "0"), r = r.toString().padStart(2, "0")
+                        var c = new Date(n.props.value);
+                        e = c.getFullYear().toString().padStart(2, "0") + "-" + (c.getMonth() + 1).toString().padStart(2, "0") + "-" + c.getDate().toString().padStart(2, "0"), 0 === (t = c.getHours()) ? t = 12 : 12 === t ? i = "pm" : t > 12 && (t -= 12, i = "pm"), a = c.getMinutes(), r = c.getSeconds(), l = c.getMilliseconds(), t = t.toString().padStart(2, "0"), a = a.toString().padStart(2, "0"), r = r.toString().padStart(2, "0")
                     }
                     return {
                         date: e,
                         hh: t,
                         mm: a,
                         ss: r,
-                        ms: i,
-                        ampm: l
+                        ms: l,
+                        ampm: i
                     }
                 }, n.handleClickOutside = function(e) {
                     n.state.showTimePicker && (!n.timePickerContainer.current || n.timePickerContainer.current.contains(e.target) || n.timeInput.current.contains(e.target) || n.setState({
                         showTimePicker: !1
                     }))
                 }, n.sendValue = function() {
                     var e = {
@@ -642,16 +671,16 @@
                     };
                     if ("" === n.state.date || null === n.state.date) return n.props.onChange(e);
                     var t = parseInt(n.state.hh);
                     0 === t && (t = NaN), "am" === n.state.ampm ? 12 === t && (t = 0) : "pm" === n.state.ampm && 12 !== t && (t += 12), t = t.toString().padStart(2, "0");
                     var a = n.state.mm.padStart(2, "0"),
                         r = n.state.ss.padStart(2, "0");
                     try {
-                        var i = new Date(n.state.date + "T" + t + ":" + a + ":" + r + "." + n.state.ms);
-                        e.target.value = i.toISOString().replace("Z", "+00:00")
+                        var l = new Date(n.state.date + "T" + t + ":" + a + ":" + r + "." + n.state.ms);
+                        e.target.value = l.toISOString().replace("Z", "+00:00")
                     } catch (t) {
                         return n.props.onChange(e)
                     }
                     n.props.onChange(e)
                 }, n.handleDateChange = function(e) {
                     n.setState({
                         date: e.target.value
@@ -668,30 +697,32 @@
             }
             t(n, a);
             var r = n.prototype;
             return r.componentDidUpdate = function(t, a) {
                 if (t.value !== this.props.value && "" !== this.state.hh && "0" !== this.state.hh && "00" !== this.state.hh) {
                     var n = !1,
                         r = this.getStateFromProps();
-                    for (var i in r)
-                        if (r[i] !== this.state[i]) {
+                    for (var l in r)
+                        if (r[l] !== this.state[l]) {
                             n = !0;
                             break
                         } n && this.setState(e({}, r))
                 }
             }, r.componentDidMount = function() {
                 document.addEventListener("mousedown", this.handleClickOutside)
             }, r.componentWillUnmount = function() {
                 document.removeEventListener("mousedown", this.handleClickOutside)
             }, r.render = function() {
                 return React.createElement("div", {
                     className: "rjf-datetime-field"
                 }, this.props.label && React.createElement("label", null, this.props.label), React.createElement("div", {
                     className: "rjf-datetime-field-inner"
                 }, React.createElement("div", {
+                    className: "rjf-datetime-field-inputs"
+                }, React.createElement("div", {
                     className: "rjf-datetime-field-date"
                 }, React.createElement(j, {
                     label: "Date",
                     type: "date",
                     value: this.state.date,
                     onChange: this.handleDateChange
                 })), React.createElement("div", {
@@ -707,103 +738,106 @@
                     ref: this.timePickerContainer
                 }, this.state.showTimePicker && React.createElement(f, {
                     onChange: this.handleTimeChange,
                     hh: this.state.hh,
                     mm: this.state.mm,
                     ss: this.state.ss,
                     ampm: this.state.ampm
-                })))))
+                })))), this.props.help_text && React.createElement("span", {
+                    class: "rjf-help-text"
+                }, this.props.help_text)))
             }, n
         }(React.Component);
 
-    function _(e) {
+    function M(e) {
         return e.children ? React.createElement("div", {
             className: "rjf-form-group-title"
         }, e.children) : null
     }
 
-    function U(e, t, a) {
+    function T(e, t, a) {
         var n = e.target.parentElement.parentElement,
             r = n.previousElementSibling,
-            i = n.nextElementSibling;
+            l = n.nextElementSibling;
         if (n.classList.add("rjf-animate", "rjf-" + t), "move-up" === t) {
-            var l = r.getBoundingClientRect().y,
-                o = l,
-                c = l = n.getBoundingClientRect().y;
-            r.classList.add("rjf-animate"), r.style.opacity = 0, r.style.transform = "translateY(" + (c - o) + "px)", n.style.opacity = 0, n.style.transform = "translateY(-" + (c - o) + "px)"
+            var i = r.getBoundingClientRect().y,
+                c = i,
+                o = i = n.getBoundingClientRect().y;
+            r.classList.add("rjf-animate"), r.style.opacity = 0, r.style.transform = "translateY(" + (o - c) + "px)", n.style.opacity = 0, n.style.transform = "translateY(-" + (o - c) + "px)"
         } else if ("move-down" === t) {
             var s = n.getBoundingClientRect().y,
                 m = s,
-                p = s = i.getBoundingClientRect().y;
-            i.classList.add("rjf-animate"), i.style.opacity = 0, i.style.transform = "translateY(-" + (p - m) + "px)", n.style.opacity = 0, n.style.transform = "translateY(" + (p - m) + "px)"
+                p = s = l.getBoundingClientRect().y;
+            l.classList.add("rjf-animate"), l.style.opacity = 0, l.style.transform = "translateY(-" + (p - m) + "px)", n.style.opacity = 0, n.style.transform = "translateY(" + (p - m) + "px)"
         }
         setTimeout(function() {
-            a(), n.classList.remove("rjf-animate", "rjf-" + t), n.style = null, "move-up" === t ? (r.classList.remove("rjf-animate"), r.style = null) : "move-down" === t && (i.classList.remove("rjf-animate"), i.style = null)
+            a(), n.classList.remove("rjf-animate", "rjf-" + t), n.style = null, "move-up" === t ? (r.classList.remove("rjf-animate"), r.style = null) : "move-down" === t && (l.classList.remove("rjf-animate"), l.style = null)
         }, 200)
     }
 
-    function A(e) {
+    function U(e) {
         return React.createElement("div", {
             className: "rjf-form-row-controls"
         }, e.onMoveUp && React.createElement(m, {
             className: "move-up",
             onClick: function(t) {
-                return U(t, "move-up", e.onMoveUp)
+                return T(t, "move-up", e.onMoveUp)
             },
             title: "Move up"
         }, React.createElement("span", null, "↑")), e.onMoveDown && React.createElement(m, {
             className: "move-down",
             onClick: function(t) {
-                return U(t, "move-down", e.onMoveDown)
+                return T(t, "move-down", e.onMoveDown)
             },
             title: "Move down"
         }, React.createElement("span", null, "↓")), e.onRemove && React.createElement(m, {
             className: "remove",
             onClick: function(t) {
-                return U(t, "remove", e.onRemove)
+                return T(t, "remove", e.onRemove)
             },
             title: "Remove"
         }, React.createElement("span", null, "×")))
     }
 
-    function F(e) {
+    function A(e) {
         return React.createElement("div", {
             className: "rjf-form-row"
-        }, React.createElement(A, e), React.createElement("div", {
+        }, React.createElement(U, e), React.createElement("div", {
             className: "rjf-form-row-inner"
         }, e.children))
     }
 
-    function T(e) {
+    function F(e) {
         var t = React.Children.count(e.children),
             a = 0 !== e.level || t ? "rjf-form-group-inner" : "";
         return React.createElement("div", {
             className: "rjf-form-group"
-        }, 0 === e.level && React.createElement(_, null, e.schema.title), React.createElement("div", {
+        }, 0 === e.level && React.createElement(M, null, e.schema.title), React.createElement("div", {
             className: a
-        }, e.level > 0 && React.createElement(_, null, e.schema.title), e.children, e.addable && React.createElement(m, {
+        }, e.level > 0 && React.createElement(M, null, e.schema.title), e.children, e.addable && React.createElement(m, {
             className: "add",
             onClick: function(t) {
                 return e.onAdd()
             },
             title: "Add new"
         }, t ? "Add more" : "Add")))
     }
     var P = ["data", "schema", "name", "onChange", "onRemove", "removable", "onEdit", "editable", "onMoveUp", "onMoveDown", "parentType"];
 
     function V(t) {
         var a, n = {
                 name: t.name,
                 value: t.data,
-                readOnly: t.schema.readOnly || t.schema.readonly
+                readOnly: t.schema.readOnly || t.schema.readonly,
+                help_text: t.schema.help_text || t.schema.helpText
             },
             r = t.schema.type;
         switch (t.schema.choices && (n.options = t.schema.choices, r = "select"), t.schema.widget && ("multiselect" === t.schema.widget && "array" !== t.parentType || (r = t.schema.widget)), r) {
             case "string":
-                a = j, t.schema.format ? ("data-url" === t.schema.format || "file-url" === t.schema.format ? a = D : "datetime" === t.schema.format && (a = M), n.type = t.schema.format) : n.type = "text";
+                a = j, t.schema.format ? ("data-url" === t.schema.format || "file-url" === t.schema.format ? a = _ : "datetime" === t.schema.format && (a = I), n.type = t.schema.format) : n.type = "text";
                 break;
             case "number":
                 n.type = "number", a = j;
                 break;
             case "integer":
                 n.type = "number", n.step = "1", a = j;
                 break;
@@ -814,18 +848,18 @@
             case "radio":
                 n.type = "radio", a = C;
                 break;
             case "select":
                 a = S;
                 break;
             case "multiselect":
-                a = O;
+                a = x;
                 break;
             case "textarea":
-                a = I;
+                a = D;
                 break;
             default:
                 n.type = "text", a = j
         }
         return React.createElement(a, e({}, n, {
             label: t.editable ? React.createElement("span", null, t.schema.title, " ", React.createElement(m, {
                 className: "edit",
@@ -840,123 +874,123 @@
             }
         }))
     }
 
     function B(t) {
         var a = t.data,
             r = t.schema,
-            i = t.name,
-            l = t.onChange,
-            o = t.onRemove,
-            c = t.removable,
+            l = t.name,
+            i = t.onChange,
+            c = t.onRemove,
+            o = t.removable,
             s = t.onEdit,
             m = t.editable,
             p = t.onMoveUp,
             u = t.onMoveDown,
             d = t.parentType,
             h = n(t, P);
-        return React.createElement(F, {
-            key: i,
-            onRemove: c ? function(e) {
-                return o(i)
+        return React.createElement(A, {
+            key: l,
+            onRemove: o ? function(e) {
+                return c(l)
             } : null,
             onMoveUp: p,
             onMoveDown: u
         }, React.createElement(V, e({
             data: a,
             schema: r,
-            name: i,
-            onChange: l,
+            name: l,
+            onChange: i,
             onEdit: s,
             editable: m,
             parentType: d
         }, h)))
     }
 
     function J(e) {
         var t = e.data,
             a = e.schema,
             n = e.name,
             r = e.onAdd,
-            i = e.onRemove,
-            o = e.onMove,
-            c = e.level,
+            l = e.onRemove,
+            c = e.onMove,
+            o = e.level,
             s = [],
             p = [],
             u = !0;
         t.length <= (a.min_items || a.minItems || 0) && (u = !1);
         var d = !0;
         t.length >= (a.max_items || a.maxItems || 100) && (d = !1);
         var h = a.items.type;
         "list" === h ? h = "array" : "dict" === h && (h = "object");
         var f = {
             schema: a.items,
             onChange: e.onChange,
             onAdd: r,
-            onRemove: i,
-            level: c + 1,
+            onRemove: l,
+            level: o + 1,
             removable: u,
-            onMove: o,
+            onMove: c,
             parentType: "array"
         };
         if ("multiselect" === f.schema.widget) f.data = t, f.name = n, f.removable = !1, f.onMoveUp = null, f.onMoveDown = null, d = !1, s.push(B(f));
         else
             for (var v = function(e) {
                     f.data = t[e], f.name = n + "-" + e, f.onMoveUp = 0 === e ? null : function(t) {
-                        return o(n + "-" + e, n + "-" + (e - 1))
+                        return c(n + "-" + e, n + "-" + (e - 1))
                     }, f.onMoveDown = e === t.length - 1 ? null : function(t) {
-                        return o(n + "-" + e, n + "-" + (e + 1))
+                        return c(n + "-" + e, n + "-" + (e + 1))
                     }, "array" === h ? p.push(J(f)) : "object" === h ? p.push(L(f)) : s.push(B(f))
                 }, g = 0; g < t.length; g++) v(g);
         var R = n;
-        return (s.length || !s.length && !p.length) && (s = React.createElement(T, {
-            level: c,
+        return (s.length || !s.length && !p.length) && (s = React.createElement(F, {
+            level: o,
             schema: a,
             addable: d,
             onAdd: function() {
-                return r(l(a.items), R)
+                return r(i(a.items), R)
             },
             key: "row_group_" + n
         }, s)), p.length && (p = React.createElement("div", {
             key: "group_" + n
         }, a.title ? React.createElement("div", {
             className: "rjf-form-group-title"
         }, a.title) : null, p.map(function(e, t) {
             return React.createElement("div", {
                 className: "rjf-form-group-wrapper",
                 key: "group_wrapper_" + n + "_" + t
-            }, React.createElement(A, {
+            }, React.createElement(U, {
                 onRemove: u ? function(e) {
-                    return i(n + "-" + t)
+                    return l(n + "-" + t)
                 } : null,
                 onMoveUp: t > 0 ? function(e) {
-                    return o(n + "-" + t, n + "-" + (t - 1))
+                    return c(n + "-" + t, n + "-" + (t - 1))
                 } : null,
                 onMoveDown: t < p.length - 1 ? function(e) {
-                    return o(n + "-" + t, n + "-" + (t + 1))
+                    return c(n + "-" + t, n + "-" + (t + 1))
                 } : null
             }), e)
         }), d && React.createElement(m, {
             className: "add",
             onClick: function(e) {
-                return r(l(a.items), R)
+                return r(i(a.items), R)
             },
             title: "Add new"
         }, "Add item"))), [].concat(s, p)
     }
 
     function L(e) {
         var t = e.data,
             a = e.schema,
             n = e.name,
             r = e.onChange,
-            i = e.onAdd,
-            l = e.onRemove,
-            o = e.level,
-            c = e.onMove,
+            l = e.onAdd,
+            i = e.onRemove,
+            c = e.level,
+            o = e.onMove,
             s = [],
             m = a.keys || a.properties,
             p = [].concat(Object.keys(m));
         a.additionalProperties && (p = [].concat(p, Object.keys(t).filter(function(e) {
             return -1 === p.indexOf(e)
         })));
         for (var u = function(e) {
@@ -973,44 +1007,44 @@
                 var v = !1;
                 void 0 === m[a] && (v = !0);
                 var R = {
                     data: u,
                     schema: h,
                     name: d,
                     onChange: r,
-                    onAdd: i,
-                    onRemove: l,
-                    level: o + 1,
+                    onAdd: l,
+                    onRemove: i,
+                    level: c + 1,
                     removable: v,
-                    onMove: c,
+                    onMove: o,
                     parentType: "object"
                 };
                 "array" === f ? s.push(J(R)) : "object" === f ? s.push(L(R)) : (R.onEdit = function() {
-                    return function(e, t, a, n, r, i) {
-                        var l = prompt("Rename key", t);
-                        if (null !== l && (l = l.trim()) !== t) {
-                            if (!l) return alert("(!) Key name can't be empty.\r\n\r\n‎");
-                            if (e.hasOwnProperty(l)) return alert("(!) Duplicate keys not allowed. This key already exists.\r\n\r\n‎");
-                            var o = n.split("-");
-                            o.pop(), o.push(l), r(a, o = o.join("-")), i(n)
+                    return function(e, t, a, n, r, l) {
+                        var i = prompt("Rename key", t);
+                        if (null !== i && (i = i.trim()) !== t) {
+                            if (!i) return alert("(!) Key name can't be empty.\r\n\r\n‎");
+                            if (e.hasOwnProperty(i)) return alert("(!) Duplicate keys not allowed. This key already exists.\r\n\r\n‎");
+                            var c = n.split("-");
+                            c.pop(), c.push(i), r(a, c = c.join("-")), l(n)
                         }
-                    }(t, a, u, d, i, l)
+                    }(t, a, u, d, l, i)
                 }, R.editable = v, s.push(B(R)))
             }, d = 0; d < p.length; d++) u(d);
         if (s.length || a.additionalProperties) {
             var h = n;
-            s = React.createElement(T, {
-                level: o,
+            s = React.createElement(F, {
+                level: c,
                 schema: a,
                 addable: a.additionalProperties,
                 onAdd: function() {
                     return function(e, t, a) {
                         var n = prompt("Add new key");
                         null !== n && ((n = n.trim()) ? e.hasOwnProperty(n) ? alert("(!) Duplicate keys not allowed. This key already exists.\r\n\r\n‎") : a("", t + "-" + n) : alert("(!) Can't add empty key.\r\n\r\n‎"))
-                    }(t, h, i)
+                    }(t, h, l)
                 },
                 key: "row_group_" + n
             }, s)
         }
         return s
     }
     var H = function(e) {
@@ -1071,20 +1105,20 @@
                 (e = e.split("-")).shift(), (t = t.split("-")).shift(), a.setState(function(a) {
                     var n = JSON.parse(JSON.stringify(a.data));
                     return Y(e, t, n), {
                         data: n
                     }
                 })
             }, a.dataInput = document.getElementById(a.props.dataInputId), a.schema = t.schema;
-            var n, r, i, s = t.data;
+            var n, r, l, s = t.data;
             if (s) try {
-                n = s, "list" === (i = (r = a.schema).type) ? i = "array" : "dict" === i && (i = "object"), s = "array" === i ? o(n, r) : "object" === i ? c(n, r) : n
+                n = s, "list" === (l = (r = a.schema).type) ? l = "array" : "dict" === l && (l = "object"), s = "array" === l ? c(n, r) : "object" === l ? o(n, r) : n
             } catch (e) {
                 console.error("Error: Schema and data structure don't match"), console.error(e)
-            } else s = l(a.schema);
+            } else s = i(a.schema);
             return a.state = {
                 value: "",
                 data: s
             }, a.populateDataInput(), a
         }
         t(a, e);
         var n = a.prototype;
@@ -1116,16 +1150,16 @@
     }
 
     function Y(e, t, a) {
         var n = e.shift();
         if (isNaN(Number(n)) || (n = Number(n)), e.length) Y(e, t, a[n]);
         else if (Array.isArray(a)) {
             var r = t[t.length - 1],
-                i = a[n];
-            a.splice(n, 1), a.splice(r, 0, i)
+                l = a[n];
+            a.splice(n, 1), a.splice(r, 0, l)
         }
     }
     return {
         JSONForm: function(e) {
             this.containerId = e.containerId, this.dataInputId = e.dataInputId, this.schema = e.schema, this.data = e.data, this.fileUploadEndpoint = e.fileUploadEndpoint, this.fieldName = e.fieldName, this.modelName = e.modelName, this.render = function() {
                 ReactDOM.render(React.createElement(H, {
                     schema: this.schema,
```

### Comparing `django-jsonform-2.8.1/django_jsonform/static/django_jsonform/react-json-form.min.js.map` & `django-jsonform-2.9.0/django_jsonform/static/django_jsonform/react-json-form.min.js.map`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8908184068734527%*

 * *Differences: {"'mappings'": "'gvBAAgBA,EAAeC,GAC3B,IAAIC,EAAO,GAEPC,EAAcF,EAAOC,MAAQD,EAAOG,WAExC,IAAK,IAAIC,KAAOF,EAAa,CACzB,IAAIG,EAAQH,EAAYE,GACpBE,EAAOD,EAAMC,KAEJ,SAATA,EACAA,EAAO,QACO,SAATA,IACLA,EAAO,UAGPL,EAAKG,GADI,UAATE,EACYC,EAAcF,GACZ,WAATC,EACOP,EAAeM,GACb,YAATC,EACOD,YAAiB,EACf,YAATC,GAA+B,WAATA,EACfD,WAAiB,KAEjBA,WAAiB,GAGrC,OAAOJ,WAIKM,EAAcP,GAC1B,GAAIA,UACA,OAAOA,UAEX,IAAIQ,EAAQ,GACRF,EAAON,EAAOQ,MAAMF,KAOxB,MALa,SAATA,EACAA,EAAO,QACO,SAATA,IACLA,EAAO,UAEE,UAATA,GACAE,EAAMC,KAAKF,EAAcP,EAAOQ,QACzBA,GAEO […]*

```diff
@@ -1,10 +1,10 @@
 {
     "file": "react-json-form.min.js",
-    "mappings": "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",
+    "mappings": "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",
     "names": [
         "getBlankObject",
         "schema",
         "keys",
         "schema_keys",
         "properties",
         "key",
@@ -86,16 +86,18 @@
         "string",
         "charAt",
         "toUpperCase",
         "substr",
         "toLowerCase",
         "FormInput",
         "label",
+        "help_text",
         "inputRef",
         "ref",
+        "class",
         "FormCheckInput",
         "undefined",
         "checked",
         "readOnly",
         "disabled",
         "FormRadioInput",
         "options",
@@ -109,25 +111,27 @@
         "state",
         "setState",
         "hideOptions",
         "toggleOptions",
         "optionsContainer",
         "createRef",
         "input",
-        "help_text",
         "error",
         "FormMultiSelectInputOptions",
         "containerRef",
+        "hasHelpText",
         "handleClickOutside",
         "current",
         "contains",
         "componentDidMount",
         "document",
         "addEventListener",
         "removeEventListener",
+        "style",
+        "marginTop",
         "selected",
         "_this3",
         "indexOf",
         "optionClassName",
         "FormFileInput",
         "_this4",
         "getFileName",
@@ -191,15 +195,14 @@
         "FormTextareaInput",
         "_this5",
         "updateHeight",
         "el",
         "offset",
         "offsetHeight",
         "clientHeight",
-        "style",
         "scrollHeight",
         "FormDateTimeInput",
         "_this6",
         "getStateFromProps",
         "date",
         "ms",
         "Date",
@@ -254,14 +257,15 @@
         "level",
         "addable",
         "onAdd",
         "FormField",
         "InputField",
         "inputProps",
         "readonly",
+        "helpText",
         "choices",
         "parentType",
         "format",
         "step",
         "editable",
         "onEdit",
         "fieldType",
@@ -341,16 +345,16 @@
     "sourcesContent": [
         "export function getBlankObject(schema) {\n    let keys = {};\n\n    let schema_keys = schema.keys || schema.properties;\n\n    for (let key in schema_keys) {\n        let value = schema_keys[key];\n        let type = value.type;\n\n        if (type === 'list')\n            type = 'array';\n        else if (type === 'dict')\n            type = 'object';\n\n        if (type === 'array')\n            keys[key] = getBlankArray(value);\n        else if (type === 'object')\n            keys[key] = getBlankObject(value);\n        else if (type === 'boolean')\n            keys[key] = value.default || false;\n        else if (type === 'integer' || type === 'number')\n            keys[key] = value.default || null;\n        else // string etc.\n            keys[key] = value.default || '';\n    }\n\n    return keys;\n}\n\n\nexport function getBlankArray(schema) {\n    if (schema.default)\n        return schema.default;\n\n    let items = [];\n    let type = schema.items.type;\n\n    if (type === 'list')\n        type = 'array';\n    else if (type === 'dict')\n        type = 'object';\n\n    if (type === 'array') {\n        items.push(getBlankArray(schema.items))\n        return items;\n    }\n    else if (type === 'object') {\n        items.push(getBlankObject(schema.items));\n        return items;\n    }\n\n    if (schema.items.widget === 'multiselect')\n        return items;\n\n    if (type === 'boolean')\n        items.push(schema.items.default || false);\n    else if (type === 'integer' || type === 'number')\n        items.push(schema.items.default || null);\n    else // string, etc.\n        items.push(schema.items.default || '');\n\n    return items;\n}\n\n\nexport function getBlankData(schema) {\n    let type = schema.type;\n\n    if (type === 'list')\n        type = 'array';\n    else if (type === 'dict')\n        type = 'object';\n\n    if (type === 'array')\n        return getBlankArray(schema);\n    else if (type === 'object')\n        return getBlankObject(schema);\n    else if (type === 'boolean')\n        return schema.default || false;\n    else if (type === 'integer' || type === 'number')\n        return schema.default || null;\n    else // string, etc.\n        return schema.default || '';\n}\n\n\n\nfunction getSyncedArray(data, schema) {\n    let newData = JSON.parse(JSON.stringify(data));\n\n    let type = schema.items.type;\n    \n    if (type === 'list')\n        type = 'array';\n    else if (type === 'dict')\n        type = 'object';\n\n    for (let i = 0; i < data.length; i++) {\n        let item = data[i];\n\n        if (type === 'array') {\n            newData[i] = getSyncedArray(item, schema.items);\n        } else if (type === 'object') {\n            newData[i] = getSyncedObject(item, schema.items);\n        }\n        else {\n            if ((type === 'integer' || type === 'number') && item === '')\n                newData[i] = null;\n        }\n    }\n\n    return newData;\n}\n\n\nfunction getSyncedObject(data, schema) {\n    let newData = JSON.parse(JSON.stringify(data));\n\n    let schema_keys = schema.keys || schema.properties;\n\n    let keys = [...Object.keys(schema_keys)];\n\n    for (let i = 0; i < keys.length; i++) {\n        let key = keys[i];\n        let schemaValue = schema_keys[key];\n        let type = schemaValue.type;\n    \n        if (type === 'list')\n            type = 'array';\n        else if (type === 'dict')\n            type = 'object';\n      \n        if (!data.hasOwnProperty(key)) {\n            if (type === 'array')\n                newData[key] = getSyncedArray([], schemaValue);\n            else if (type === 'object')\n                newData[key] = getSyncedObject({}, schemaValue);\n            else if (type === 'boolean')\n                newData[key] = false;\n            else if (type === 'integer' || type === 'number')\n                newData[key] = null;\n            else\n                newData[key] = '';\n        } else {\n            if (type === 'array')\n                newData[key] = getSyncedArray(data[key], schemaValue);\n            else if (type === 'object')\n                newData[key] = getSyncedObject(data[key], schemaValue);\n            else {\n                if ((type === 'integer' || type === 'number') && data[key] === '')\n                    newData[key] = null;\n                else\n                    newData[key] = data[key];\n            }\n        }\n        \n    }\n\n    return newData;\n}\n\n\nexport function getSyncedData(data, schema) {\n    // adds those keys to data which are in schema but not in data\n\n    let type = schema.type;\n    \n    if (type === 'list')\n        type = 'array';\n    else if (type === 'dict')\n        type = 'object';\n\n    if (type === 'array') {\n        return getSyncedArray(data, schema);\n    } else if (type === 'object') {\n        return getSyncedObject(data, schema);\n    }\n\n    return data;\n}\n",
         "export default function Button({className, ...props}) {\n    if (!className)\n        className = '';\n\n    let classes = className.split(' ');\n\n    className = '';\n    for (let i = 0; i < classes.length; i++) {\n        className = className + 'rjf-' + classes[i] + '-button ';\n    }\n\n    return (\n        <button \n            className={className.trim()}\n            type=\"button\"\n            {...props}\n        >\n            {props.children}\n        </button>\n    );\n}",
         "export default function Loader (props) {\n    return <div className=\"rjf-loader\"></div>;\n}\n",
         "export default function Icon(props) {\n    let icon;\n\n    switch (props.name) {\n        case 'chevron-up':\n            icon = <ChevronUp />;\n            break;\n        case 'chevron-down':\n            icon = <ChevronDown />;\n            break;\n    }\n\n    return (\n        <svg xmlns=\"http://www.w3.org/2000/svg\" width=\"16\" height=\"16\" fill=\"currentColor\" className={\"rjf-icon rjf-icon-\" + props.name} viewBox=\"0 0 16 16\">\n            {icon}\n        </svg>\n    );\n}\n\nfunction ChevronUp(props) {\n    return (\n        <path fillRule=\"evenodd\" d=\"M7.646 4.646a.5.5 0 0 1 .708 0l6 6a.5.5 0 0 1-.708.708L8 5.707l-5.646 5.647a.5.5 0 0 1-.708-.708l6-6z\"/>\n    );\n}\n\nfunction ChevronDown(props) {\n    return (\n        <path fillRule=\"evenodd\" d=\"M1.646 4.646a.5.5 0 0 1 .708 0L8 10.293l5.646-5.647a.5.5 0 0 1 .708.708l-6 6a.5.5 0 0 1-.708 0l-6-6a.5.5 0 0 1 0-.708z\"/>\n    );\n}\n",
         "import Button from './buttons';\nimport Icon from './icons';\n\n\nexport class TimePicker extends React.Component {\n    componentWillUnmount() {\n        let data = {\n            hh: this.validateValue('hh', this.props.hh).toString().padStart(2, '0'),\n            mm: this.validateValue('mm', this.props.mm).toString().padStart(2, '0'),\n            ss: this.validateValue('ss', this.props.ss).toString().padStart(2, '0')\n        }\n        this.sendValue(data);\n    }\n\n    sendValue = (data) => {\n        this.props.onChange(data);\n    }\n\n    validateValue = (name, value) => {\n        if (name === 'hh' && value < 1)\n            return 1;\n        else if (name !== 'hh' && value < 0)\n            return 0;\n        else if (name === 'hh' && value > 12)\n            return 12;\n        else if (name !== 'hh' && value > 59)\n            return 59;\n\n        return value;\n    }\n\n    handleChange = (e) => {\n        let name = e.target.dataset.name;\n        let value = e.target.value;\n\n        if (isNaN(value))\n            return;\n\n        let validValue = this.validateValue(name, parseInt(value) || 0);\n\n        if (name === 'hh' && (value === '0' || value === '' || value === '00') && validValue === 1)\n            validValue = 0;\n\n        if (value.startsWith('0') && validValue < 10 && validValue !== 0) {\n            validValue = validValue.toString().padStart(2, '0');\n        }\n\n        this.sendValue({[name]: value !== '' ? validValue.toString() : ''});\n    }\n\n    handleKeyDown = (e) => {\n        if (e.keyCode !== 38 && e.keyCode !== 40)\n            return;\n\n        let name = e.target.dataset.name;\n        let value = parseInt(e.target.value) || 0;\n\n        if (e.keyCode === 38) {\n            value++;\n        } else if (e.keyCode === 40) {\n            value--;\n        }\n\n        this.sendValue({[name]: this.validateValue(name, value).toString().padStart(2, '0')});\n    }\n\n    handleSpin = (name, type) => {\n        let value = this.props[name];\n\n        if (name === 'ampm') {\n            value = value === 'am' ? 'pm': 'am';\n        } else {\n            value = parseInt(value) || 0;\n            if (type === 'up') {\n                value++;\n            } else {\n                value--;\n            }\n            value = this.validateValue(name, value).toString().padStart(2, '0');\n        }\n\n        this.sendValue({[name]: value});\n    }\n\n    handleBlur = (e) => {\n        let value = this.validateValue(e.target.dataset.name, parseInt(e.target.value) || 0);\n\n        if (value < 10) {\n            this.sendValue({[e.target.dataset.name]: value.toString().padStart(2, '0')});\n        }\n    }\n\n    render() {\n        return (\n            <div className=\"rjf-time-picker\">\n                <div className=\"rjf-time-picker-row rjf-time-picker-labels\">\n                    <div className=\"rjf-time-picker-col\">Hrs</div>\n                    <div className=\"rjf-time-picker-col rjf-time-picker-col-sm\"></div>\n                    <div className=\"rjf-time-picker-col\">Min</div>\n                    <div className=\"rjf-time-picker-col rjf-time-picker-col-sm\"></div>\n                    <div className=\"rjf-time-picker-col\">Sec</div>\n                    <div className=\"rjf-time-picker-col rjf-time-picker-col-sm\"></div>\n                    <div className=\"rjf-time-picker-col\">am/pm</div>\n                </div>\n\n                <div className=\"rjf-time-picker-row\">\n                    <div className=\"rjf-time-picker-col\"><Button onClick={() => this.handleSpin('hh', 'up')}><Icon name=\"chevron-up\"/></Button></div>\n                    <div className=\"rjf-time-picker-col rjf-time-picker-col-sm\"></div>\n                    <div className=\"rjf-time-picker-col\"><Button onClick={() => this.handleSpin('mm', 'up')}><Icon name=\"chevron-up\"/></Button></div>\n                    <div className=\"rjf-time-picker-col rjf-time-picker-col-sm\"></div>\n                    <div className=\"rjf-time-picker-col\"><Button onClick={() => this.handleSpin('ss', 'up')}><Icon name=\"chevron-up\"/></Button></div>\n                    <div className=\"rjf-time-picker-col rjf-time-picker-col-sm\"></div>\n                    <div className=\"rjf-time-picker-col\"><Button onClick={() => this.handleSpin('ampm', 'up')}><Icon name=\"chevron-up\"/></Button></div> \n                </div>\n\n                <div className=\"rjf-time-picker-row rjf-time-picker-values\">\n                    <div className=\"rjf-time-picker-col\"><input type=\"text\" data-name=\"hh\" value={this.props.hh} onChange={this.handleChange} onBlur={this.handleBlur} onKeyDown={this.handleKeyDown} /></div>\n                    <div className=\"rjf-time-picker-col rjf-time-picker-col-sm\">:</div>\n                    <div className=\"rjf-time-picker-col\"><input type=\"text\" data-name=\"mm\" value={this.props.mm} onChange={this.handleChange} onBlur={this.handleBlur} onKeyDown={this.handleKeyDown} /></div>\n                    <div className=\"rjf-time-picker-col rjf-time-picker-col-sm\">:</div>\n                    <div className=\"rjf-time-picker-col\"><input type=\"text\" data-name=\"ss\" value={this.props.ss} onChange={this.handleChange} onBlur={this.handleBlur} onKeyDown={this.handleKeyDown} /></div>\n                    <div className=\"rjf-time-picker-col rjf-time-picker-col-sm\"></div>\n                    <div className=\"rjf-time-picker-col\">{this.props.ampm}</div>\n                </div>\n\n                <div className=\"rjf-time-picker-row\">\n                    <div className=\"rjf-time-picker-col\"><Button onClick={() => this.handleSpin('hh', 'down')}><Icon name=\"chevron-down\"/></Button></div>\n                    <div className=\"rjf-time-picker-col rjf-time-picker-col-sm\"></div>\n                    <div className=\"rjf-time-picker-col\"><Button onClick={() => this.handleSpin('mm', 'down')}><Icon name=\"chevron-down\"/></Button></div>\n                    <div className=\"rjf-time-picker-col rjf-time-picker-col-sm\"></div>\n                    <div className=\"rjf-time-picker-col\"><Button onClick={() => this.handleSpin('ss', 'down')}><Icon name=\"chevron-down\"/></Button></div>\n                    <div className=\"rjf-time-picker-col rjf-time-picker-col-sm\"></div>\n                    <div className=\"rjf-time-picker-col\"><Button onClick={() => this.handleSpin('ampm', 'down')}><Icon name=\"chevron-down\"/></Button></div> \n                </div>\n            </div>\n        );\n    }\n}\n",
         "export const EditorContext = React.createContext();\n\n\nexport function capitalize(string) {\n    if (!string)\n        return '';\n    \n    return string.charAt(0).toUpperCase() + string.substr(1).toLowerCase();\n}\n\n\nexport function getVerboseName(name) {\n    if (name === undefined || name === null)\n        return '';\n\n    name = name.replace(/_/g, ' ');\n    return capitalize(name);\n}\n\n\nexport function getCsrfCookie() {\n    if ((document.cookie.split(';').filter((item) => item.trim().indexOf('csrftoken=') === 0)).length) {\n        return document.cookie.split(';').filter((item) => item.trim().indexOf('csrftoken=') === 0)[0].split('=')[1];\n    }\n    return null;\n}\n",
-        "import Button from './buttons';\nimport Loader from './loaders';\nimport {TimePicker} from './widgets';\nimport {EditorContext, getCsrfCookie, capitalize} from '../util';\n\n\nexport function FormInput({label, help_text, error, inputRef, ...props}) {\n\n    if (props.type === 'string')\n        props.type = 'text'\n\n    if (inputRef)\n        props.ref = inputRef;\n\n    if (props.value === null)\n        props.value = '';\n\n    return (\n        <div>\n            {label && <label>{label}</label>}\n            <input {...props} />\n        </div>\n    );\n}\n\n\nexport function FormCheckInput({label, help_text, error, value, ...props}) {\n\n    if (!label)\n        label = props.name.toUpperCase();\n\n    if (props.type === 'bool')\n        props.type = 'checkbox';\n\n    if (props.checked === undefined)\n        props.checked = value;\n\n    if (props.checked === '' || props.checked === null || props.checked === undefined)\n        props.checked = false\n\n    if (props.readOnly)\n        props.disabled = true;\n\n    return (\n        <div>\n            <label><input {...props} /> {label}</label>\n        </div>\n    );\n}\n\n\nexport function FormRadioInput({label, help_text, error, value, options, ...props}) {\n    if (props.readOnly)\n        props.disabled = true;\n\n    return (\n        <div>\n            <label>{label}</label>\n            {options.map((option, i) => {\n                let label, inputValue;\n                if (typeof option === 'object') {\n                    label = option.label;\n                    inputValue = option.value;\n                } else {\n                    label = option;\n                    if (typeof label === 'boolean')\n                        label = capitalize(label.toString());\n                    inputValue = option;\n                }\n\n                return (\n                    <label key={label + '_' + inputValue + '_' + i}>\n                        <input {...props} value={inputValue} checked={inputValue === value} /> {label}\n                    </label>\n                );\n            })}\n        </div>\n    );\n}\n\n\nexport function FormSelectInput({label, help_text, error, value, options, ...props}) {\n    if (props.readOnly)\n        props.disabled = true;\n\n    return (\n        <div>\n            {label && <label>{label}</label>}\n            <select value={value || ''} {...props}>\n                <option disabled value=\"\" key={'__placehlder'}>Select...</option>\n                {options.map((option, i) => {\n                    let label, inputValue;\n                    if (typeof option === 'object') {\n                        label = option.label;\n                        inputValue = option.value;\n                    } else {\n                        label = option;\n                        if (typeof label === 'boolean')\n                            label = capitalize(label.toString());\n                        inputValue = option;\n                    }\n\n                    return (\n                        <option value={inputValue} key={label + '_' + inputValue + '_' + i}>\n                            {label}\n                        </option>\n                    );\n                })}\n            </select>\n        </div>\n    );\n}\n\nexport class FormMultiSelectInput extends React.Component {\n    constructor(props) {\n        super(props);\n\n        this.state = {\n            showOptions: false\n        };\n\n        this.optionsContainer = React.createRef();\n        this.input = React.createRef();\n    }\n\n    handleChange = (e) => {\n        let value = [...this.props.value];\n\n        if (e.target.checked) {\n            value.push(e.target.value);\n        } else {\n            value = value.filter((item) => item !== e.target.value);\n        }\n\n        let event = {\n            target: {\n                type: this.props.type,\n                value: value,\n                name: this.props.name\n            }\n        };\n\n        this.props.onChange(event);\n    }\n\n    showOptions = (e) => {\n        if (!this.state.showOptions)\n            this.setState({showOptions: true});\n    }\n\n    hideOptions = (e) => {\n        this.setState({showOptions: false});\n    }\n\n    toggleOptions = (e) => {\n        this.setState((state) => ({showOptions: !state.showOptions}))\n    }\n\n    render() {\n        return (\n            <div className=\"rjf-multiselect-field\">\n                <FormInput\n                    label={this.props.label}\n                    type=\"text\"\n                    value={this.props.value.length ? this.props.value.length + ' selected' : 'Select...'}\n                    help_text={this.props.help_text}\n                    error={this.props.error}\n                    onClick={this.toggleOptions}\n                    readOnly={true}\n                    inputRef={this.input}\n                    className=\"rjf-multiselect-field-input\"\n                />\n                {this.state.showOptions &&\n                    <FormMultiSelectInputOptions\n                        options={this.props.options}\n                        value={this.props.value}\n                        hideOptions={this.hideOptions}\n                        onChange={this.handleChange}\n                        containerRef={this.optionsContainer}\n                        inputRef={this.input}\n                        disabled={this.props.readOnly}\n                    />\n                }\n            </div>\n        )\n    }\n}\n\nclass FormMultiSelectInputOptions extends React.Component {\n    componentDidMount() {\n        document.addEventListener('mousedown', this.handleClickOutside);\n    }\n\n    componentWillUnmount() {\n      document.removeEventListener('mousedown', this.handleClickOutside);\n    }\n\n    handleClickOutside = (e) => {\n        if (this.props.containerRef.current &&\n            !this.props.containerRef.current.contains(e.target) &&\n            !this.props.inputRef.current.contains(e.target)\n        )\n            this.props.hideOptions();\n    };\n\n    render() {\n        return (\n            <div ref={this.props.containerRef}>\n                <div className=\"rjf-multiselect-field-options-container\">\n                    {this.props.options.map((option, i) => {\n                        let label, inputValue;\n                        if (typeof option === 'object') {\n                            label = option.label;\n                            inputValue = option.value;\n                        } else {\n                            label = option;\n                            if (typeof label === 'boolean')\n                                label = capitalize(label.toString());\n                            inputValue = option;\n                        }\n\n                        let selected = this.props.value.indexOf(inputValue) > -1;\n\n                        let optionClassName = 'rjf-multiselect-field-option';\n                        if (selected)\n                            optionClassName += ' selected';\n                        if (this.props.disabled)\n                            optionClassName += ' disabled';\n\n                        return (\n                            <div key={label + '_' + inputValue + '_' + i} className={optionClassName}>\n                                <label>\n                                    <input\n                                        type=\"checkbox\"\n                                        onChange={this.props.onChange}\n                                        value={inputValue}\n                                        checked={selected}\n                                        disabled={this.props.disabled}\n                                    /> {label}\n                                </label>\n                            </div>\n                        );\n                    })}\n                </div>\n            </div>\n        );\n    }\n\n}\n\nexport function dataURItoBlob(dataURI) {\n      // Split metadata from data\n      const splitted = dataURI.split(\",\");\n      // Split params\n      const params = splitted[0].split(\";\");\n      // Get mime-type from params\n      const type = params[0].replace(\"data:\", \"\");\n      // Filter the name property from params\n      const properties = params.filter(param => {\n            return param.split(\"=\")[0] === \"name\";\n      });\n      // Look for the name and use unknown if no name property.\n      let name;\n      if (properties.length !== 1) {\n            name = \"unknown\";\n      } else {\n            // Because we filtered out the other property,\n            // we only have the name case here.\n            name = properties[0].split(\"=\")[1];\n      }\n\n      // Built the Uint8Array Blob parameter from the base64 string.\n      const binary = atob(splitted[1]);\n      const array = [];\n      for (let i = 0; i < binary.length; i++) {\n            array.push(binary.charCodeAt(i));\n      }\n      // Create the blob object\n      const blob = new window.Blob([new Uint8Array(array)], { type });\n\n      return {blob, name};\n}\n\n\n\nexport class FormFileInput extends React.Component {\n    static contextType = EditorContext;\n\n    constructor(props) {\n        super(props);\n\n        this.state = {\n            value: props.value,\n            fileName: this.getFileName(),\n            loading: false\n        };\n\n        this.inputRef = React.createRef();\n    }\n\n    componentDidUpdate(prevProps, prevState) {\n        if (this.props.value !== prevProps.value) {\n            this.setState({\n                value: this.props.value, \n                fileName: this.getFileName()\n            });\n        }\n    }\n\n    getFileName = () => {\n        if (!this.props.value)\n            return '';\n\n        if (this.props.type === 'data-url') {\n            return this.extractFileInfo(this.props.value).name;\n        } else if (this.props.type === 'file-url') {\n            return this.props.value;\n        } else {\n            return 'Unknown file';\n        }\n    }\n\n    extractFileInfo = (dataURL) => {\n        const {blob, name} = dataURItoBlob(dataURL);\n        return {\n            name: name,\n            size: blob.size,\n            type: blob.type\n        }\n    }\n\n    addNameToDataURL = (dataURL, name) => {\n        return dataURL.replace(';base64', ';name=' + encodeURIComponent(name) + ';base64');\n    }\n\n    handleChange = (e) => {\n        if (this.props.type === 'data-url') {\n            let file = e.target.files[0];\n            let fileName = file.name\n\n            let reader = new FileReader();\n\n            reader.onload = () => {\n\n                // this.setState({src: reader.result});\n\n                // we create a fake event object\n                let event = {\n                    target: {\n                        type: 'text',\n                        value: this.addNameToDataURL(reader.result, fileName),\n                        name: this.props.name\n                    }\n                };\n\n                this.props.onChange(event);\n\n            }\n            reader.readAsDataURL(file);\n        } else if (this.props.type === 'file-url') {\n            let endpoint = this.context.fileUploadEndpoint;\n            if (!endpoint) {\n                console.error(\n                    \"Error: fileUploadEndpoint option need to be passed \"\n                    + \"while initializing editor for enabling file uploads.\");\n                alert(\"Files can't be uploaded.\");\n                return;\n            }\n\n            this.setState({loading: true});\n\n            let formData = new FormData();\n            formData.append('field_name', this.context.fieldName);\n            formData.append('model_name', this.context.modelName);\n            formData.append('coordinates', JSON.stringify(this.props.name.split('-').slice(1)));\n            formData.append('file', e.target.files[0]);\n\n            fetch(endpoint, {\n                method: 'POST',\n                headers: {\n                    'X-CSRFToken': getCsrfCookie(),\n                },\n                body: formData\n            })\n            .then((response) => response.json())\n            .then((result) => {\n                // we create a fake event object\n                let event = {\n                    target: {\n                        type: 'text',\n                        value: result.file_path,\n                        name: this.props.name\n                    }\n                };\n\n                this.props.onChange(event);\n                this.setState({loading: false});\n            })\n            .catch((error) => {\n                alert('Something went wrong while uploading file');\n                console.error('Error:', error);\n                this.setState({loading: false});\n            });\n\n        }\n\n    }\n\n    showFileBrowser = () => {\n        this.inputRef.current.click();\n    }\n\n    clearFile = () => {\n        if (window.confirm('Do you want to remove this file?')) {\n            let event = {\n                target: {\n                    type: 'text',\n                    value: '',\n                    name: this.props.name\n                }\n            };\n\n            this.props.onChange(event);\n        }\n    }\n\n    render() {\n        let {label, value, ...props} = {value, ...this.props};\n        props.type = 'file';\n        props.onChange = this.handleChange;\n\n        if (props.readOnly)\n            props.disabled = true;\n\n        return (\n            <div> \n                {label && <label>{label}</label>}\n                <div className=\"rjf-file-field\">\n                    {this.state.value && \n                        <div className=\"rjf-current-file-name\">\n                            Current file: <span>{this.state.fileName}</span> {' '}\n                            <Button className=\"remove-file\" onClick={this.clearFile}>Clear</Button>\n                        </div>\n                    }\n                    {this.state.value && !this.state.loading && 'Change:'}\n                    {this.state.loading ?\n                        <div className=\"rjf-file-field-loading\"><Loader/> Uploading...</div>\n                    : \n                    <div className=\"rjf-file-field-input\">\n                        <FormInput {...props} inputRef={this.inputRef} />\n                    </div>\n                    }\n                    </div>\n            </div>\n        );\n    }\n}\n\n\nexport class FormTextareaInput extends React.Component {\n    constructor(props) {\n        super(props);\n\n        if (!props.inputRef)\n            this.inputRef = React.createRef();\n    }\n\n    handleChange = (e) => {\n        this.updateHeight(e.target);\n\n        if (this.props.onChange)\n            this.props.onChange(e);\n    }\n\n    updateHeight = (el) => {\n        let offset = el.offsetHeight - el.clientHeight;\n        el.style.height = 'auto';\n        el.style.height = (el.scrollHeight + offset) + 'px';\n    }\n\n    componentDidMount() {\n        if (this.props.inputRef)\n            this.updateHeight(this.props.inputRef.current);\n        else \n            this.updateHeight(this.inputRef.current);\n    }\n\n    render() {\n        let {label, help_text, error, inputRef, ...props} = this.props;\n\n        delete props.type;\n\n        props.ref = inputRef || this.inputRef;\n        props.onChange = this.handleChange;\n\n        return (\n            <div>\n                {label && <label>{label}</label>}\n                <textarea {...props} />\n            </div>\n        );\n    }\n}\n\n\nexport class FormDateTimeInput extends React.Component {\n    constructor(props) {\n        super(props);\n        // we maintain this input's state in itself\n        // so that we can only pass valid values\n        // otherwise keep the value empty if invalid\n\n        this.state = {\n            ...this.getStateFromProps(),\n            showTimePicker: false,\n        };\n\n        this.timeInput = React.createRef();\n        this.timePickerContainer = React.createRef();\n    }\n\n    getStateFromProps = () => {\n        let date = '';\n        let hh = '12';\n        let mm = '00';\n        let ss = '00';\n        let ms = '000';\n        let ampm = 'am';\n\n        if (this.props.value) {\n            let d = new Date(this.props.value);\n            let year = d.getFullYear().toString().padStart(2, '0');\n            let month = (d.getMonth() + 1).toString().padStart(2, '0');\n            let day = d.getDate().toString().padStart(2, '0');\n            date = year + '-' + month + '-' + day;\n\n            hh = d.getHours();\n            if (hh === 0) {\n                hh = 12;\n            } else if (hh === 12) {\n                ampm = 'pm';\n            } else if (hh > 12) {\n                hh = hh - 12;\n                ampm = 'pm';\n            }\n\n            mm = d.getMinutes();\n            ss = d.getSeconds();\n            ms = d.getMilliseconds();\n\n            hh = hh.toString().padStart(2, '0');\n            mm = mm.toString().padStart(2, '0');\n            ss = ss.toString().padStart(2, '0');\n        }\n\n        return {\n            date: date, hh: hh, mm: mm, ss: ss, ms: ms, ampm: ampm\n        }\n    }\n\n    componentDidUpdate(prevProps, prevState) {\n        if (prevProps.value !== this.props.value) {\n            if (this.state.hh !== '' && this.state.hh !== '0' && this.state.hh !== '00') {\n\n                let changed = false;\n                let newState = this.getStateFromProps();\n                \n                for (let key in newState) {\n                    if (newState[key] !== this.state[key]) {\n                        changed = true;\n                        break;\n                    }\n                }\n\n                if (changed)\n                    this.setState({...newState});\n            }\n        }\n    }\n\n    componentDidMount() {\n        document.addEventListener('mousedown', this.handleClickOutside);\n    }\n\n    componentWillUnmount() {\n      document.removeEventListener('mousedown', this.handleClickOutside);\n    }\n\n    handleClickOutside = (e) => {\n        if (this.state.showTimePicker) {\n            if (this.timePickerContainer.current &&\n                !this.timePickerContainer.current.contains(e.target) &&\n                !this.timeInput.current.contains(e.target)\n            )\n                this.setState({showTimePicker: false});\n        }\n    };\n\n    sendValue = () => {\n        // we create a fake event object\n        // to send a combined value from two inputs\n        let event = {\n            target: {\n                type: 'text',\n                value: '',\n                name: this.props.name\n            }\n        };\n\n        if (this.state.date === '' || this.state.date === null)\n            return this.props.onChange(event);\n\n        let hh = parseInt(this.state.hh);\n\n        if (hh === 0)\n            hh = NaN; // zero value is invalid for 12 hour clock, but will be valid for 24 hour clock\n                      // so we set it to NaN to prevent creating a date object\n        \n        if (this.state.ampm === 'am') {\n            if (hh === 12)\n                hh = 0;\n        } else if (this.state.ampm === 'pm') {\n            if (hh !== 12)\n                hh = hh + 12;\n        }\n\n        hh = hh.toString().padStart(2, '0');\n        let mm = this.state.mm.padStart(2, '0');\n        let ss = this.state.ss.padStart(2, '0');\n\n        try {\n            let date = new Date(this.state.date + 'T' + hh + ':' + mm + ':' + ss + '.' + this.state.ms);\n            event['target']['value'] = date.toISOString().replace('Z', '+00:00') // make compatible to python\n        } catch (err) {\n            // invalid date\n            return this.props.onChange(event);\n        }\n\n        this.props.onChange(event);\n    }\n\n    handleDateChange = (e) => {\n        this.setState({date: e.target.value}, this.sendValue);\n    }\n\n    handleTimeChange = (value) => {\n        this.setState({...value}, this.sendValue);\n    }\n\n    showTimePicker = () => {\n        this.setState({showTimePicker: true});\n    }\n\n    render() {\n        return (\n            <div className=\"rjf-datetime-field\">\n                {this.props.label && <label>{this.props.label}</label>}\n                <div className=\"rjf-datetime-field-inner\">\n                    <div className=\"rjf-datetime-field-date\">\n                        <FormInput\n                            label='Date'\n                            type='date'\n                            value={this.state.date}\n                            onChange={this.handleDateChange}\n                        />\n                    </div>\n                    <div className=\"rjf-datetime-field-time\">\n                        <FormInput\n                            label='Time'\n                            type='text'\n                            value={this.state.hh + ':' + this.state.mm + ':' + this.state.ss + ' ' + this.state.ampm}\n                            onFocus={this.showTimePicker}\n                            readOnly={true}\n                            inputRef={this.timeInput}\n                        />\n                        <div ref={this.timePickerContainer}>\n                            {this.state.showTimePicker &&\n                                <TimePicker\n                                    onChange={this.handleTimeChange}\n                                    hh={this.state.hh}\n                                    mm={this.state.mm}\n                                    ss={this.state.ss}\n                                    ampm={this.state.ampm}\n                                />\n                            }\n                        </div>\n                    </div>\n                </div>\n            </div>\n        );\n    }\n}\n",
+        "import Button from './buttons';\nimport Loader from './loaders';\nimport {TimePicker} from './widgets';\nimport {EditorContext, getCsrfCookie, capitalize} from '../util';\n\n\nexport function FormInput({label, help_text, error, inputRef, ...props}) {\n\n    if (props.type === 'string')\n        props.type = 'text'\n\n    if (inputRef)\n        props.ref = inputRef;\n\n    if (props.value === null)\n        props.value = '';\n\n    return (\n        <div>\n            {label && <label>{label}</label>}\n            <div className=\"rjf-input-group\">\n                <input {...props} />\n                {help_text && <span class=\"rjf-help-text\">{help_text}</span>}\n            </div>\n        </div>\n    );\n}\n\n\nexport function FormCheckInput({label, help_text, error, value, ...props}) {\n\n    if (!label)\n        label = props.name.toUpperCase();\n\n    if (props.type === 'bool')\n        props.type = 'checkbox';\n\n    if (props.checked === undefined)\n        props.checked = value;\n\n    if (props.checked === '' || props.checked === null || props.checked === undefined)\n        props.checked = false\n\n    if (props.readOnly)\n        props.disabled = true;\n\n    return (\n        <div className=\"rjf-check-input\">\n            <label><input {...props} /> {label}</label>\n            {help_text && <span class=\"rjf-help-text\">{help_text}</span>}\n        </div>\n    );\n}\n\n\nexport function FormRadioInput({label, help_text, error, value, options, ...props}) {\n    if (props.readOnly)\n        props.disabled = true;\n\n    return (\n        <div className=\"rjf-check-input\">\n            <label>{label}</label>\n            {options.map((option, i) => {\n                let label, inputValue;\n                if (typeof option === 'object') {\n                    label = option.label;\n                    inputValue = option.value;\n                } else {\n                    label = option;\n                    if (typeof label === 'boolean')\n                        label = capitalize(label.toString());\n                    inputValue = option;\n                }\n\n                return (\n                    <label key={label + '_' + inputValue + '_' + i}>\n                        <input {...props} value={inputValue} checked={inputValue === value} /> {label}\n                    </label>\n                );\n            })}\n            {help_text && <span class=\"rjf-help-text\">{help_text}</span>}\n        </div>\n    );\n}\n\n\nexport function FormSelectInput({label, help_text, error, value, options, ...props}) {\n    if (props.readOnly)\n        props.disabled = true;\n\n    return (\n        <div>\n            {label && <label>{label}</label>}\n            <div class=\"rjf-input-group\">\n                <select value={value || ''} {...props}>\n                    <option disabled value=\"\" key={'__placehlder'}>Select...</option>\n                    {options.map((option, i) => {\n                        let label, inputValue;\n                        if (typeof option === 'object') {\n                            label = option.label;\n                            inputValue = option.value;\n                        } else {\n                            label = option;\n                            if (typeof label === 'boolean')\n                                label = capitalize(label.toString());\n                            inputValue = option;\n                        }\n\n                        return (\n                            <option value={inputValue} key={label + '_' + inputValue + '_' + i}>\n                                {label}\n                            </option>\n                        );\n                    })}\n                </select>\n                {help_text && <span class=\"rjf-help-text\">{help_text}</span>}\n            </div>\n        </div>\n    );\n}\n\nexport class FormMultiSelectInput extends React.Component {\n    constructor(props) {\n        super(props);\n\n        this.state = {\n            showOptions: false\n        };\n\n        this.optionsContainer = React.createRef();\n        this.input = React.createRef();\n    }\n\n    handleChange = (e) => {\n        let value = [...this.props.value];\n\n        if (e.target.checked) {\n            value.push(e.target.value);\n        } else {\n            value = value.filter((item) => item !== e.target.value);\n        }\n\n        let event = {\n            target: {\n                type: this.props.type,\n                value: value,\n                name: this.props.name\n            }\n        };\n\n        this.props.onChange(event);\n    }\n\n    showOptions = (e) => {\n        if (!this.state.showOptions)\n            this.setState({showOptions: true});\n    }\n\n    hideOptions = (e) => {\n        this.setState({showOptions: false});\n    }\n\n    toggleOptions = (e) => {\n        this.setState((state) => ({showOptions: !state.showOptions}))\n    }\n\n    render() {\n        return (\n            <div className=\"rjf-multiselect-field\">\n                <FormInput\n                    label={this.props.label}\n                    type=\"text\"\n                    value={this.props.value.length ? this.props.value.length + ' selected' : 'Select...'}\n                    help_text={this.props.help_text}\n                    error={this.props.error}\n                    onClick={this.toggleOptions}\n                    readOnly={true}\n                    inputRef={this.input}\n                    className=\"rjf-multiselect-field-input\"\n                />\n                {this.state.showOptions &&\n                    <FormMultiSelectInputOptions\n                        options={this.props.options}\n                        value={this.props.value}\n                        hideOptions={this.hideOptions}\n                        onChange={this.handleChange}\n                        containerRef={this.optionsContainer}\n                        inputRef={this.input}\n                        disabled={this.props.readOnly}\n                        hasHelpText={this.props.help_text && 1}\n                    />\n                }\n            </div>\n        )\n    }\n}\n\nclass FormMultiSelectInputOptions extends React.Component {\n    componentDidMount() {\n        document.addEventListener('mousedown', this.handleClickOutside);\n    }\n\n    componentWillUnmount() {\n      document.removeEventListener('mousedown', this.handleClickOutside);\n    }\n\n    handleClickOutside = (e) => {\n        if (this.props.containerRef.current &&\n            !this.props.containerRef.current.contains(e.target) &&\n            !this.props.inputRef.current.contains(e.target)\n        )\n            this.props.hideOptions();\n    };\n\n    render() {\n        return (\n            <div ref={this.props.containerRef}>\n                <div\n                    className=\"rjf-multiselect-field-options-container\"\n                    style={this.props.hasHelpText ? {marginTop: '-15px'} : {}}\n                >\n                    {this.props.options.map((option, i) => {\n                        let label, inputValue;\n                        if (typeof option === 'object') {\n                            label = option.label;\n                            inputValue = option.value;\n                        } else {\n                            label = option;\n                            if (typeof label === 'boolean')\n                                label = capitalize(label.toString());\n                            inputValue = option;\n                        }\n\n                        let selected = this.props.value.indexOf(inputValue) > -1;\n\n                        let optionClassName = 'rjf-multiselect-field-option';\n                        if (selected)\n                            optionClassName += ' selected';\n                        if (this.props.disabled)\n                            optionClassName += ' disabled';\n\n                        return (\n                            <div key={label + '_' + inputValue + '_' + i} className={optionClassName}>\n                                <label>\n                                    <input\n                                        type=\"checkbox\"\n                                        onChange={this.props.onChange}\n                                        value={inputValue}\n                                        checked={selected}\n                                        disabled={this.props.disabled}\n                                    /> {label}\n                                </label>\n                            </div>\n                        );\n                    })}\n                </div>\n            </div>\n        );\n    }\n\n}\n\nexport function dataURItoBlob(dataURI) {\n      // Split metadata from data\n      const splitted = dataURI.split(\",\");\n      // Split params\n      const params = splitted[0].split(\";\");\n      // Get mime-type from params\n      const type = params[0].replace(\"data:\", \"\");\n      // Filter the name property from params\n      const properties = params.filter(param => {\n            return param.split(\"=\")[0] === \"name\";\n      });\n      // Look for the name and use unknown if no name property.\n      let name;\n      if (properties.length !== 1) {\n            name = \"unknown\";\n      } else {\n            // Because we filtered out the other property,\n            // we only have the name case here.\n            name = properties[0].split(\"=\")[1];\n      }\n\n      // Built the Uint8Array Blob parameter from the base64 string.\n      const binary = atob(splitted[1]);\n      const array = [];\n      for (let i = 0; i < binary.length; i++) {\n            array.push(binary.charCodeAt(i));\n      }\n      // Create the blob object\n      const blob = new window.Blob([new Uint8Array(array)], { type });\n\n      return {blob, name};\n}\n\n\n\nexport class FormFileInput extends React.Component {\n    static contextType = EditorContext;\n\n    constructor(props) {\n        super(props);\n\n        this.state = {\n            value: props.value,\n            fileName: this.getFileName(),\n            loading: false\n        };\n\n        this.inputRef = React.createRef();\n    }\n\n    componentDidUpdate(prevProps, prevState) {\n        if (this.props.value !== prevProps.value) {\n            this.setState({\n                value: this.props.value, \n                fileName: this.getFileName()\n            });\n        }\n    }\n\n    getFileName = () => {\n        if (!this.props.value)\n            return '';\n\n        if (this.props.type === 'data-url') {\n            return this.extractFileInfo(this.props.value).name;\n        } else if (this.props.type === 'file-url') {\n            return this.props.value;\n        } else {\n            return 'Unknown file';\n        }\n    }\n\n    extractFileInfo = (dataURL) => {\n        const {blob, name} = dataURItoBlob(dataURL);\n        return {\n            name: name,\n            size: blob.size,\n            type: blob.type\n        }\n    }\n\n    addNameToDataURL = (dataURL, name) => {\n        return dataURL.replace(';base64', ';name=' + encodeURIComponent(name) + ';base64');\n    }\n\n    handleChange = (e) => {\n        if (this.props.type === 'data-url') {\n            let file = e.target.files[0];\n            let fileName = file.name\n\n            let reader = new FileReader();\n\n            reader.onload = () => {\n\n                // this.setState({src: reader.result});\n\n                // we create a fake event object\n                let event = {\n                    target: {\n                        type: 'text',\n                        value: this.addNameToDataURL(reader.result, fileName),\n                        name: this.props.name\n                    }\n                };\n\n                this.props.onChange(event);\n\n            }\n            reader.readAsDataURL(file);\n        } else if (this.props.type === 'file-url') {\n            let endpoint = this.context.fileUploadEndpoint;\n            if (!endpoint) {\n                console.error(\n                    \"Error: fileUploadEndpoint option need to be passed \"\n                    + \"while initializing editor for enabling file uploads.\");\n                alert(\"Files can't be uploaded.\");\n                return;\n            }\n\n            this.setState({loading: true});\n\n            let formData = new FormData();\n            formData.append('field_name', this.context.fieldName);\n            formData.append('model_name', this.context.modelName);\n            formData.append('coordinates', JSON.stringify(this.props.name.split('-').slice(1)));\n            formData.append('file', e.target.files[0]);\n\n            fetch(endpoint, {\n                method: 'POST',\n                headers: {\n                    'X-CSRFToken': getCsrfCookie(),\n                },\n                body: formData\n            })\n            .then((response) => response.json())\n            .then((result) => {\n                // we create a fake event object\n                let event = {\n                    target: {\n                        type: 'text',\n                        value: result.file_path,\n                        name: this.props.name\n                    }\n                };\n\n                this.props.onChange(event);\n                this.setState({loading: false});\n            })\n            .catch((error) => {\n                alert('Something went wrong while uploading file');\n                console.error('Error:', error);\n                this.setState({loading: false});\n            });\n\n        }\n\n    }\n\n    showFileBrowser = () => {\n        this.inputRef.current.click();\n    }\n\n    clearFile = () => {\n        if (window.confirm('Do you want to remove this file?')) {\n            let event = {\n                target: {\n                    type: 'text',\n                    value: '',\n                    name: this.props.name\n                }\n            };\n\n            this.props.onChange(event);\n            \n            if (this.inputRef.current)\n                this.inputRef.current.value = '';\n        }\n    }\n\n    render() {\n        let {label, value, ...props} = {value, ...this.props};\n        props.type = 'file';\n        props.onChange = this.handleChange;\n\n        if (props.readOnly)\n            props.disabled = true;\n\n        return (\n            <div> \n                {label && <label>{label}</label>}\n                <div className=\"rjf-file-field\">\n                    {this.state.value && \n                        <div className=\"rjf-current-file-name\">\n                            Current file: <span>{this.state.fileName}</span> {' '}\n                            <Button className=\"remove-file\" onClick={this.clearFile}>Clear</Button>\n                        </div>\n                    }\n                    {this.state.value && !this.state.loading && 'Change:'}\n                    {this.state.loading ?\n                        <div className=\"rjf-file-field-loading\"><Loader/> Uploading...</div>\n                    : \n                    <div className=\"rjf-file-field-input\">\n                        <FormInput {...props} inputRef={this.inputRef} />\n                    </div>\n                    }\n                    </div>\n            </div>\n        );\n    }\n}\n\n\nexport class FormTextareaInput extends React.Component {\n    constructor(props) {\n        super(props);\n\n        if (!props.inputRef)\n            this.inputRef = React.createRef();\n    }\n\n    handleChange = (e) => {\n        this.updateHeight(e.target);\n\n        if (this.props.onChange)\n            this.props.onChange(e);\n    }\n\n    updateHeight = (el) => {\n        let offset = el.offsetHeight - el.clientHeight;\n        el.style.height = 'auto';\n        el.style.height = (el.scrollHeight + offset) + 'px';\n    }\n\n    componentDidMount() {\n        if (this.props.inputRef)\n            this.updateHeight(this.props.inputRef.current);\n        else \n            this.updateHeight(this.inputRef.current);\n    }\n\n    render() {\n        let {label, help_text, error, inputRef, ...props} = this.props;\n\n        delete props.type;\n\n        props.ref = inputRef || this.inputRef;\n        props.onChange = this.handleChange;\n\n        return (\n            <div>\n                {label && <label>{label}</label>}\n                <div className=\"rjf-input-group\">\n                    <textarea {...props} />\n                    {help_text && <span class=\"rjf-help-text\">{help_text}</span>}\n                </div>\n            </div>\n        );\n    }\n}\n\n\nexport class FormDateTimeInput extends React.Component {\n    constructor(props) {\n        super(props);\n        // we maintain this input's state in itself\n        // so that we can only pass valid values\n        // otherwise keep the value empty if invalid\n\n        this.state = {\n            ...this.getStateFromProps(),\n            showTimePicker: false,\n        };\n\n        this.timeInput = React.createRef();\n        this.timePickerContainer = React.createRef();\n    }\n\n    getStateFromProps = () => {\n        let date = '';\n        let hh = '12';\n        let mm = '00';\n        let ss = '00';\n        let ms = '000';\n        let ampm = 'am';\n\n        if (this.props.value) {\n            let d = new Date(this.props.value);\n            let year = d.getFullYear().toString().padStart(2, '0');\n            let month = (d.getMonth() + 1).toString().padStart(2, '0');\n            let day = d.getDate().toString().padStart(2, '0');\n            date = year + '-' + month + '-' + day;\n\n            hh = d.getHours();\n            if (hh === 0) {\n                hh = 12;\n            } else if (hh === 12) {\n                ampm = 'pm';\n            } else if (hh > 12) {\n                hh = hh - 12;\n                ampm = 'pm';\n            }\n\n            mm = d.getMinutes();\n            ss = d.getSeconds();\n            ms = d.getMilliseconds();\n\n            hh = hh.toString().padStart(2, '0');\n            mm = mm.toString().padStart(2, '0');\n            ss = ss.toString().padStart(2, '0');\n        }\n\n        return {\n            date: date, hh: hh, mm: mm, ss: ss, ms: ms, ampm: ampm\n        }\n    }\n\n    componentDidUpdate(prevProps, prevState) {\n        if (prevProps.value !== this.props.value) {\n            if (this.state.hh !== '' && this.state.hh !== '0' && this.state.hh !== '00') {\n\n                let changed = false;\n                let newState = this.getStateFromProps();\n                \n                for (let key in newState) {\n                    if (newState[key] !== this.state[key]) {\n                        changed = true;\n                        break;\n                    }\n                }\n\n                if (changed)\n                    this.setState({...newState});\n            }\n        }\n    }\n\n    componentDidMount() {\n        document.addEventListener('mousedown', this.handleClickOutside);\n    }\n\n    componentWillUnmount() {\n      document.removeEventListener('mousedown', this.handleClickOutside);\n    }\n\n    handleClickOutside = (e) => {\n        if (this.state.showTimePicker) {\n            if (this.timePickerContainer.current &&\n                !this.timePickerContainer.current.contains(e.target) &&\n                !this.timeInput.current.contains(e.target)\n            )\n                this.setState({showTimePicker: false});\n        }\n    };\n\n    sendValue = () => {\n        // we create a fake event object\n        // to send a combined value from two inputs\n        let event = {\n            target: {\n                type: 'text',\n                value: '',\n                name: this.props.name\n            }\n        };\n\n        if (this.state.date === '' || this.state.date === null)\n            return this.props.onChange(event);\n\n        let hh = parseInt(this.state.hh);\n\n        if (hh === 0)\n            hh = NaN; // zero value is invalid for 12 hour clock, but will be valid for 24 hour clock\n                      // so we set it to NaN to prevent creating a date object\n        \n        if (this.state.ampm === 'am') {\n            if (hh === 12)\n                hh = 0;\n        } else if (this.state.ampm === 'pm') {\n            if (hh !== 12)\n                hh = hh + 12;\n        }\n\n        hh = hh.toString().padStart(2, '0');\n        let mm = this.state.mm.padStart(2, '0');\n        let ss = this.state.ss.padStart(2, '0');\n\n        try {\n            let date = new Date(this.state.date + 'T' + hh + ':' + mm + ':' + ss + '.' + this.state.ms);\n            event['target']['value'] = date.toISOString().replace('Z', '+00:00') // make compatible to python\n        } catch (err) {\n            // invalid date\n            return this.props.onChange(event);\n        }\n\n        this.props.onChange(event);\n    }\n\n    handleDateChange = (e) => {\n        this.setState({date: e.target.value}, this.sendValue);\n    }\n\n    handleTimeChange = (value) => {\n        this.setState({...value}, this.sendValue);\n    }\n\n    showTimePicker = () => {\n        this.setState({showTimePicker: true});\n    }\n\n    render() {\n        return (\n            <div className=\"rjf-datetime-field\">\n                {this.props.label && <label>{this.props.label}</label>}\n                <div className=\"rjf-datetime-field-inner\">\n                    <div className=\"rjf-datetime-field-inputs\">\n                        <div className=\"rjf-datetime-field-date\">\n                            <FormInput\n                                label='Date'\n                                type='date'\n                                value={this.state.date}\n                                onChange={this.handleDateChange}\n                            />\n                        </div>\n                        <div className=\"rjf-datetime-field-time\">\n                            <FormInput\n                                label='Time'\n                                type='text'\n                                value={this.state.hh + ':' + this.state.mm + ':' + this.state.ss + ' ' + this.state.ampm}\n                                onFocus={this.showTimePicker}\n                                readOnly={true}\n                                inputRef={this.timeInput}\n                            />\n                            <div ref={this.timePickerContainer}>\n                                {this.state.showTimePicker &&\n                                    <TimePicker\n                                        onChange={this.handleTimeChange}\n                                        hh={this.state.hh}\n                                        mm={this.state.mm}\n                                        ss={this.state.ss}\n                                        ampm={this.state.ampm}\n                                    />\n                                }\n                            </div>\n                        </div>\n                    </div>\n                    {this.props.help_text && <span class=\"rjf-help-text\">{this.props.help_text}</span>}\n                </div>\n            </div>\n        );\n    }\n}\n",
         "import Button from './buttons';\n\n\nexport function GroupTitle(props) {\n    if (!props.children)\n        return null;\n\n    return (\n        <div className=\"rjf-form-group-title\">{props.children}</div>\n    );\n}\n\n\nfunction animate(e, animation, callback) {\n    let el = e.target.parentElement.parentElement;\n    let prevEl = el.previousElementSibling;\n    let nextEl = el.nextElementSibling;\n\n    el.classList.add('rjf-animate', 'rjf-' + animation);\n\n    if (animation === 'move-up') {\n        let {y, height} = prevEl.getBoundingClientRect();\n        let y1 = y, h1 = height;\n        \n        ({y, height} = el.getBoundingClientRect());\n        let y2 = y, h2 = height;\n        \n        prevEl.classList.add('rjf-animate');\n\n        prevEl.style.opacity = 0;\n        prevEl.style.transform = 'translateY(' + (y2 - y1)  + 'px)';\n\n        el.style.opacity = 0;\n        el.style.transform = 'translateY(-' + (y2 - y1)  + 'px)';\n\n    } else if (animation === 'move-down') {\n        let {y, height} = el.getBoundingClientRect();\n        let y1 = y, h1 = height;\n        \n        ({y, height} = nextEl.getBoundingClientRect());\n        let y2 = y, h2 = height;\n        \n        nextEl.classList.add('rjf-animate');\n\n        nextEl.style.opacity = 0;\n        nextEl.style.transform = 'translateY(-' + (y2 - y1)  + 'px)';\n\n        el.style.opacity = 0;\n        el.style.transform = 'translateY(' + (y2 - y1)  + 'px)';\n    }\n\n    setTimeout(function() {\n        callback();\n        \n        el.classList.remove('rjf-animate', 'rjf-' + animation);\n        el.style = null;\n\n        if (animation === 'move-up') {\n            prevEl.classList.remove('rjf-animate');\n            prevEl.style = null;\n        }\n        else if (animation === 'move-down') {\n            nextEl.classList.remove('rjf-animate');\n            nextEl.style = null;\n        }\n    }, 200);\n}\n\nexport function FormRowControls(props) {\n    return (\n        <div className=\"rjf-form-row-controls\">\n            {props.onMoveUp &&\n                <Button \n                    className=\"move-up\"\n                    onClick={(e) => animate(e, 'move-up', props.onMoveUp)}\n                    title=\"Move up\"\n                >\n                    <span>&uarr;</span>\n                </Button>\n            }\n            {props.onMoveDown &&\n                <Button \n                    className=\"move-down\"\n                    onClick={(e) => animate(e, 'move-down', props.onMoveDown)}\n                    title=\"Move down\"\n                >\n                    <span>&darr;</span>\n                </Button>\n            }\n            {props.onRemove &&\n                <Button \n                    className=\"remove\"\n                    onClick={(e) => animate(e, 'remove', props.onRemove)}\n                    title=\"Remove\"\n                >\n                    <span>&times;</span>\n                </Button>\n            }\n        </div>\n    );\n}\n\nexport function FormRow(props) {\n    return (\n        <div className=\"rjf-form-row\">\n            <FormRowControls {...props} />\n            <div className=\"rjf-form-row-inner\">\n                {props.children}\n            </div>\n        </div>\n    );\n}\n\n\nexport function FormGroup(props) {\n    let hasChildren = React.Children.count(props.children);\n\n    let innerClassName = props.level === 0 && !hasChildren\n        ? \"\" \n        : \"rjf-form-group-inner\";\n\n    return (\n        <div className=\"rjf-form-group\">\n            {props.level === 0 && <GroupTitle>{props.schema.title}</GroupTitle>}\n            <div className={innerClassName}>\n                {props.level > 0 && <GroupTitle>{props.schema.title}</GroupTitle>}\n                {props.children}\n                {props.addable && \n                <Button\n                    className=\"add\"\n                    onClick={(e) => props.onAdd()}\n                    title=\"Add new\"\n                >\n                    {hasChildren ? 'Add more' : 'Add'}\n                </Button>\n                }\n            </div>\n        </div>\n    );\n}\n",
-        "import {getBlankData} from './data';\nimport {Button, FormInput, FormCheckInput, FormRadioInput, FormSelectInput,\n    FormFileInput, FormRow, FormGroup, FormRowControls, FormTextareaInput,\n    FormDateTimeInput, FormMultiSelectInput} from './components';\nimport {getVerboseName} from './util';\n\n\nfunction handleChange(e, fieldType, callback) {\n    let type = e.target.type\n    let value;\n\n    if (type === 'checkbox') {\n        value = e.target.checked;\n    } else {\n        value = e.target.value;\n    }\n\n    if (fieldType === 'number' || fieldType === 'integer') {\n        value = value.trim();\n        if (value === '')\n            value = null;\n        else if (!isNaN(Number(value)))\n            value = Number(value);\n    } else if (fieldType === 'boolean') {\n        if (value === 'false' || value === false)\n            value = false;\n        else\n            value = true;\n    }\n\n    callback(e.target.name, value);\n}\n\n\nfunction FormField(props) {\n    let inputProps = {\n        name: props.name,\n        value: props.data,\n        readOnly: props.schema.readOnly || props.schema.readonly,\n    };\n\n    let type = props.schema.type;\n    if (props.schema.choices) {\n        inputProps.options = props.schema.choices;\n        type = 'select';\n    }\n    if (props.schema.widget) {\n         if (props.schema.widget === 'multiselect' && props.parentType !== 'array') {\n            // pass\n         } else {\n            type = props.schema.widget;\n         }\n    }\n\n\n    let InputField;\n\n    switch (type) {\n        case 'string':\n            InputField = FormInput;\n\n            if (props.schema.format) {\n                if (props.schema.format === 'data-url' || props.schema.format === 'file-url') {\n                    InputField = FormFileInput;\n                } else if (props.schema.format === 'datetime') {\n                    InputField = FormDateTimeInput;\n                }\n                inputProps.type = props.schema.format;\n            }\n            else {\n                inputProps.type = 'text';\n            }\n            break;\n        case 'number':\n            inputProps.type = 'number';\n            InputField = FormInput;\n            break;\n        case 'integer':\n            inputProps.type = 'number';\n            inputProps.step = '1';\n            InputField = FormInput;\n            break;\n        case 'boolean':\n            inputProps.type = 'checkbox';\n            InputField = FormCheckInput;\n            break;\n        case 'checkbox':\n            inputProps.type = 'checkbox';\n            InputField = FormCheckInput;\n            break;\n        case 'radio':\n            inputProps.type = 'radio';\n            InputField = FormRadioInput;\n            break;\n        case 'select':\n            InputField = FormSelectInput;\n            break;\n        case 'multiselect':\n            InputField = FormMultiSelectInput;\n            break;\n        case 'textarea':\n            InputField = FormTextareaInput;\n            break;\n        default:\n            inputProps.type = 'text';\n            InputField = FormInput;\n    }\n\n   return (\n        <InputField \n            {...inputProps}\n            label={\n                props.editable ? <span>{props.schema.title} <Button className=\"edit\" onClick={props.onEdit} title=\"Edit\">Edit</Button></span>\n                :\n                props.schema.title\n            }\n            onChange={(e) => handleChange(e, props.schema.type, props.onChange)}\n        />\n    );\n}\n\n\nexport function getStringFormRow(args) {\n    let {\n        data, schema, name, onChange, onRemove, removable, onEdit, editable, \n        onMoveUp, onMoveDown, parentType, ...fieldProps\n    } = args;\n\n    return (\n        <FormRow \n            key={name}\n            onRemove={removable ? (e) => onRemove(name) : null}\n            onMoveUp={onMoveUp}\n            onMoveDown={onMoveDown}\n        >\n            <FormField \n                data={data}\n                schema={schema}\n                name={name}\n                onChange={onChange}\n                onEdit={onEdit}\n                editable={editable}\n                parentType={parentType}\n                {...fieldProps}\n            />\n        </FormRow>\n    );\n}\n\nexport function getArrayFormRow(args) {\n    let {data, schema, name, onChange, onAdd, onRemove, onMove, level} = args;\n\n    let rows = [];\n    let groups = [];\n\n    let removable = true;\n    let min_items = schema.min_items || schema.minItems || 0;\n    if (data.length <= min_items)\n        removable = false;\n\n    let addable = true;\n    let max_items = schema.max_items || schema.maxItems || 100;\n    if (data.length >= max_items)\n        addable = false;\n\n    let type = schema.items.type;\n    \n    if (type === 'list')\n        type = 'array';\n    else if (type === 'dict')\n        type = 'object';\n\n    let nextArgs = {\n        schema: schema.items,\n        onChange: onChange,\n        onAdd: onAdd,\n        onRemove: onRemove,\n        level: level + 1,\n        removable: removable,\n        onMove: onMove,\n        parentType: 'array',\n    };\n\n    if (nextArgs.schema.widget === 'multiselect') {\n        nextArgs.data = data;\n        nextArgs.name = name;\n        nextArgs.removable = false;\n        nextArgs.onMoveUp = null;\n        nextArgs.onMoveDown = null;\n        addable = false;\n        rows.push(getStringFormRow(nextArgs));\n    } else {\n\n        for (let i = 0; i < data.length; i++) {\n            nextArgs.data = data[i];\n            nextArgs.name = name + '-' + i;\n\n            if (i === 0)\n                nextArgs.onMoveUp = null;\n            else\n                nextArgs.onMoveUp = (e) => onMove(name + '-' + i, name + '-' + (i - 1));\n\n            if (i === data.length - 1)\n                nextArgs.onMoveDown = null;\n            else\n                nextArgs.onMoveDown = (e) => onMove(name + '-' + i, name + '-' + (i + 1));\n\n            if (type === 'array') {\n                groups.push(getArrayFormRow(nextArgs));\n            } else if (type === 'object') {\n                groups.push(getObjectFormRow(nextArgs));\n            } else {\n                rows.push(getStringFormRow(nextArgs));\n            } \n        }\n    }\n\n    let coords = name; // coordinates for insertion and deletion\n\n    if (rows.length || (!rows.length && !groups.length)) {\n        rows = (\n            <FormGroup\n                level={level}\n                schema={schema}\n                addable={addable}\n                onAdd={() => onAdd(getBlankData(schema.items), coords)}\n                key={'row_group_' + name}\n            >\n                {rows}\n            </FormGroup>\n        );\n    }\n\n    if (groups.length) {\n        let groupTitle = schema.title ? <div className=\"rjf-form-group-title\">{schema.title}</div> : null;\n\n        groups = (\n            <div key={'group_' + name}>\n                {groupTitle}\n                {groups.map((i, index) => (\n                    <div className=\"rjf-form-group-wrapper\" key={'group_wrapper_' + name + '_' + index}>\n                        <FormRowControls\n                            onRemove={removable ? (e) => onRemove(name + '-' + index) : null}\n                            onMoveUp={index > 0 ? (e) => onMove(name + '-' + index, name + '-' + (index - 1)) : null}\n                            onMoveDown={index < groups.length - 1 ? (e) => onMove(name + '-' + index, name + '-' + (index + 1)) : null}\n                        />\n                        {i}\n                    </div>\n                    )\n                )}\n                {addable && \n                    <Button\n                        className=\"add\"\n                        onClick={(e) => onAdd(getBlankData(schema.items), coords)}\n                        title=\"Add new\"\n                    >\n                        Add item\n                    </Button>\n                }\n            </div>\n        )\n    }\n\n    return [...rows, ...groups];\n}\n\n\nexport function getObjectFormRow(args) {\n    let {data, schema, name, onChange, onAdd, onRemove, level, onMove} = args;\n\n    let rows = [];\n\n    let schema_keys = schema.keys || schema.properties;\n\n    let keys = [...Object.keys(schema_keys)];\n\n    if (schema.additionalProperties)\n        keys = [...keys, ...Object.keys(data).filter((k) => keys.indexOf(k) === -1)];\n\n    for (let i = 0; i < keys.length; i++) {\n        let key = keys[i];\n        let value = data[key];\n        let childName = name + '-' + key;\n        let schemaValue = schema_keys[key] || {type: 'string'};\n\n        let type = schemaValue.type;\n    \n        if (type === 'list')\n            type = 'array';\n        else if (type === 'dict')\n            type = 'object';\n\n        if (!schemaValue.title)\n            schemaValue.title = getVerboseName(key);\n\n        let removable = false;\n        if (schema_keys[key] === undefined)\n            removable = true;\n\n        let nextArgs = {\n            data: value,\n            schema: schemaValue,\n            name: childName,\n            onChange: onChange,\n            onAdd: onAdd,\n            onRemove: onRemove,\n            level: level + 1,\n            removable: removable,\n            onMove: onMove,\n            parentType: 'object',\n        };\n\n         if (type === 'array') {\n            rows.push(getArrayFormRow(nextArgs));\n        } else if (type === 'object') {\n            rows.push(getObjectFormRow(nextArgs));\n        } else {\n            nextArgs.onEdit = () => handleKeyEdit(data, key, value, childName, onAdd, onRemove);\n            nextArgs.editable = removable;\n            rows.push(getStringFormRow(nextArgs));\n        }\n    }\n\n    if (rows.length || schema.additionalProperties) {\n        let className = \"rjf-form-group-inner\";\n        if (level === 0 && !rows.length)\n            className = \"\";\n        \n        let coords = name;\n\n        rows = (\n            <FormGroup\n                level={level}\n                schema={schema}\n                addable={schema.additionalProperties}\n                onAdd={() => handleKeyValueAdd(data, coords, onAdd)}\n                key={'row_group_' + name}\n            >\n                {rows}\n            </FormGroup>\n        );\n    }\n\n    return rows;\n}\n\n\nfunction handleKeyValueAdd(data, coords, onAdd) {\n    let key = prompt(\"Add new key\");\n    if (key === null) // clicked cancel\n        return;\n\n    key = key.trim();\n    if (!key)\n        alert(\"(!) Can't add empty key.\\r\\n\\r\\n\u200e\");\n    else if (data.hasOwnProperty(key))\n        alert(\"(!) Duplicate keys not allowed. This key already exists.\\r\\n\\r\\n\u200e\");\n    else\n        onAdd(\"\", coords + '-' + key);   \n}\n\n\nfunction handleKeyEdit(data, key, value, coords, onAdd, onRemove) {\n    let newKey = prompt(\"Rename key\", key);\n    if (newKey === null) // clicked cancel\n        return;\n\n    newKey = newKey.trim();\n\n    if (newKey === key) // same keys\n        return;\n\n    if (!newKey)\n        return alert(\"(!) Key name can't be empty.\\r\\n\\r\\n\u200e\");\n    else if (data.hasOwnProperty(newKey))\n        return alert(\"(!) Duplicate keys not allowed. This key already exists.\\r\\n\\r\\n\u200e\");\n\n    let newCoords = coords.split('-');\n    newCoords.pop();\n    newCoords.push(newKey);\n    newCoords = newCoords.join('-');\n\n    onAdd(value, newCoords);\n    onRemove(coords);\n}\n",
+        "import {getBlankData} from './data';\nimport {Button, FormInput, FormCheckInput, FormRadioInput, FormSelectInput,\n    FormFileInput, FormRow, FormGroup, FormRowControls, FormTextareaInput,\n    FormDateTimeInput, FormMultiSelectInput} from './components';\nimport {getVerboseName} from './util';\n\n\nfunction handleChange(e, fieldType, callback) {\n    let type = e.target.type\n    let value;\n\n    if (type === 'checkbox') {\n        value = e.target.checked;\n    } else {\n        value = e.target.value;\n    }\n\n    if (fieldType === 'number' || fieldType === 'integer') {\n        value = value.trim();\n        if (value === '')\n            value = null;\n        else if (!isNaN(Number(value)))\n            value = Number(value);\n    } else if (fieldType === 'boolean') {\n        if (value === 'false' || value === false)\n            value = false;\n        else\n            value = true;\n    }\n\n    callback(e.target.name, value);\n}\n\n\nfunction FormField(props) {\n    let inputProps = {\n        name: props.name,\n        value: props.data,\n        readOnly: props.schema.readOnly || props.schema.readonly,\n        help_text: props.schema.help_text || props.schema.helpText,\n    };\n\n    let type = props.schema.type;\n    if (props.schema.choices) {\n        inputProps.options = props.schema.choices;\n        type = 'select';\n    }\n    if (props.schema.widget) {\n         if (props.schema.widget === 'multiselect' && props.parentType !== 'array') {\n            // pass\n         } else {\n            type = props.schema.widget;\n         }\n    }\n\n\n    let InputField;\n\n    switch (type) {\n        case 'string':\n            InputField = FormInput;\n\n            if (props.schema.format) {\n                if (props.schema.format === 'data-url' || props.schema.format === 'file-url') {\n                    InputField = FormFileInput;\n                } else if (props.schema.format === 'datetime') {\n                    InputField = FormDateTimeInput;\n                }\n                inputProps.type = props.schema.format;\n            }\n            else {\n                inputProps.type = 'text';\n            }\n            break;\n        case 'number':\n            inputProps.type = 'number';\n            InputField = FormInput;\n            break;\n        case 'integer':\n            inputProps.type = 'number';\n            inputProps.step = '1';\n            InputField = FormInput;\n            break;\n        case 'boolean':\n            inputProps.type = 'checkbox';\n            InputField = FormCheckInput;\n            break;\n        case 'checkbox':\n            inputProps.type = 'checkbox';\n            InputField = FormCheckInput;\n            break;\n        case 'radio':\n            inputProps.type = 'radio';\n            InputField = FormRadioInput;\n            break;\n        case 'select':\n            InputField = FormSelectInput;\n            break;\n        case 'multiselect':\n            InputField = FormMultiSelectInput;\n            break;\n        case 'textarea':\n            InputField = FormTextareaInput;\n            break;\n        default:\n            inputProps.type = 'text';\n            InputField = FormInput;\n    }\n\n   return (\n        <InputField \n            {...inputProps}\n            label={\n                props.editable ? <span>{props.schema.title} <Button className=\"edit\" onClick={props.onEdit} title=\"Edit\">Edit</Button></span>\n                :\n                props.schema.title\n            }\n            onChange={(e) => handleChange(e, props.schema.type, props.onChange)}\n        />\n    );\n}\n\n\nexport function getStringFormRow(args) {\n    let {\n        data, schema, name, onChange, onRemove, removable, onEdit, editable, \n        onMoveUp, onMoveDown, parentType, ...fieldProps\n    } = args;\n\n    return (\n        <FormRow \n            key={name}\n            onRemove={removable ? (e) => onRemove(name) : null}\n            onMoveUp={onMoveUp}\n            onMoveDown={onMoveDown}\n        >\n            <FormField \n                data={data}\n                schema={schema}\n                name={name}\n                onChange={onChange}\n                onEdit={onEdit}\n                editable={editable}\n                parentType={parentType}\n                {...fieldProps}\n            />\n        </FormRow>\n    );\n}\n\nexport function getArrayFormRow(args) {\n    let {data, schema, name, onChange, onAdd, onRemove, onMove, level} = args;\n\n    let rows = [];\n    let groups = [];\n\n    let removable = true;\n    let min_items = schema.min_items || schema.minItems || 0;\n    if (data.length <= min_items)\n        removable = false;\n\n    let addable = true;\n    let max_items = schema.max_items || schema.maxItems || 100;\n    if (data.length >= max_items)\n        addable = false;\n\n    let type = schema.items.type;\n    \n    if (type === 'list')\n        type = 'array';\n    else if (type === 'dict')\n        type = 'object';\n\n    let nextArgs = {\n        schema: schema.items,\n        onChange: onChange,\n        onAdd: onAdd,\n        onRemove: onRemove,\n        level: level + 1,\n        removable: removable,\n        onMove: onMove,\n        parentType: 'array',\n    };\n\n    if (nextArgs.schema.widget === 'multiselect') {\n        nextArgs.data = data;\n        nextArgs.name = name;\n        nextArgs.removable = false;\n        nextArgs.onMoveUp = null;\n        nextArgs.onMoveDown = null;\n        addable = false;\n        rows.push(getStringFormRow(nextArgs));\n    } else {\n\n        for (let i = 0; i < data.length; i++) {\n            nextArgs.data = data[i];\n            nextArgs.name = name + '-' + i;\n\n            if (i === 0)\n                nextArgs.onMoveUp = null;\n            else\n                nextArgs.onMoveUp = (e) => onMove(name + '-' + i, name + '-' + (i - 1));\n\n            if (i === data.length - 1)\n                nextArgs.onMoveDown = null;\n            else\n                nextArgs.onMoveDown = (e) => onMove(name + '-' + i, name + '-' + (i + 1));\n\n            if (type === 'array') {\n                groups.push(getArrayFormRow(nextArgs));\n            } else if (type === 'object') {\n                groups.push(getObjectFormRow(nextArgs));\n            } else {\n                rows.push(getStringFormRow(nextArgs));\n            } \n        }\n    }\n\n    let coords = name; // coordinates for insertion and deletion\n\n    if (rows.length || (!rows.length && !groups.length)) {\n        rows = (\n            <FormGroup\n                level={level}\n                schema={schema}\n                addable={addable}\n                onAdd={() => onAdd(getBlankData(schema.items), coords)}\n                key={'row_group_' + name}\n            >\n                {rows}\n            </FormGroup>\n        );\n    }\n\n    if (groups.length) {\n        let groupTitle = schema.title ? <div className=\"rjf-form-group-title\">{schema.title}</div> : null;\n\n        groups = (\n            <div key={'group_' + name}>\n                {groupTitle}\n                {groups.map((i, index) => (\n                    <div className=\"rjf-form-group-wrapper\" key={'group_wrapper_' + name + '_' + index}>\n                        <FormRowControls\n                            onRemove={removable ? (e) => onRemove(name + '-' + index) : null}\n                            onMoveUp={index > 0 ? (e) => onMove(name + '-' + index, name + '-' + (index - 1)) : null}\n                            onMoveDown={index < groups.length - 1 ? (e) => onMove(name + '-' + index, name + '-' + (index + 1)) : null}\n                        />\n                        {i}\n                    </div>\n                    )\n                )}\n                {addable && \n                    <Button\n                        className=\"add\"\n                        onClick={(e) => onAdd(getBlankData(schema.items), coords)}\n                        title=\"Add new\"\n                    >\n                        Add item\n                    </Button>\n                }\n            </div>\n        )\n    }\n\n    return [...rows, ...groups];\n}\n\n\nexport function getObjectFormRow(args) {\n    let {data, schema, name, onChange, onAdd, onRemove, level, onMove} = args;\n\n    let rows = [];\n\n    let schema_keys = schema.keys || schema.properties;\n\n    let keys = [...Object.keys(schema_keys)];\n\n    if (schema.additionalProperties)\n        keys = [...keys, ...Object.keys(data).filter((k) => keys.indexOf(k) === -1)];\n\n    for (let i = 0; i < keys.length; i++) {\n        let key = keys[i];\n        let value = data[key];\n        let childName = name + '-' + key;\n        let schemaValue = schema_keys[key] || {type: 'string'};\n\n        let type = schemaValue.type;\n    \n        if (type === 'list')\n            type = 'array';\n        else if (type === 'dict')\n            type = 'object';\n\n        if (!schemaValue.title)\n            schemaValue.title = getVerboseName(key);\n\n        let removable = false;\n        if (schema_keys[key] === undefined)\n            removable = true;\n\n        let nextArgs = {\n            data: value,\n            schema: schemaValue,\n            name: childName,\n            onChange: onChange,\n            onAdd: onAdd,\n            onRemove: onRemove,\n            level: level + 1,\n            removable: removable,\n            onMove: onMove,\n            parentType: 'object',\n        };\n\n         if (type === 'array') {\n            rows.push(getArrayFormRow(nextArgs));\n        } else if (type === 'object') {\n            rows.push(getObjectFormRow(nextArgs));\n        } else {\n            nextArgs.onEdit = () => handleKeyEdit(data, key, value, childName, onAdd, onRemove);\n            nextArgs.editable = removable;\n            rows.push(getStringFormRow(nextArgs));\n        }\n    }\n\n    if (rows.length || schema.additionalProperties) {\n        let className = \"rjf-form-group-inner\";\n        if (level === 0 && !rows.length)\n            className = \"\";\n        \n        let coords = name;\n\n        rows = (\n            <FormGroup\n                level={level}\n                schema={schema}\n                addable={schema.additionalProperties}\n                onAdd={() => handleKeyValueAdd(data, coords, onAdd)}\n                key={'row_group_' + name}\n            >\n                {rows}\n            </FormGroup>\n        );\n    }\n\n    return rows;\n}\n\n\nfunction handleKeyValueAdd(data, coords, onAdd) {\n    let key = prompt(\"Add new key\");\n    if (key === null) // clicked cancel\n        return;\n\n    key = key.trim();\n    if (!key)\n        alert(\"(!) Can't add empty key.\\r\\n\\r\\n\u200e\");\n    else if (data.hasOwnProperty(key))\n        alert(\"(!) Duplicate keys not allowed. This key already exists.\\r\\n\\r\\n\u200e\");\n    else\n        onAdd(\"\", coords + '-' + key);   \n}\n\n\nfunction handleKeyEdit(data, key, value, coords, onAdd, onRemove) {\n    let newKey = prompt(\"Rename key\", key);\n    if (newKey === null) // clicked cancel\n        return;\n\n    newKey = newKey.trim();\n\n    if (newKey === key) // same keys\n        return;\n\n    if (!newKey)\n        return alert(\"(!) Key name can't be empty.\\r\\n\\r\\n\u200e\");\n    else if (data.hasOwnProperty(newKey))\n        return alert(\"(!) Duplicate keys not allowed. This key already exists.\\r\\n\\r\\n\u200e\");\n\n    let newCoords = coords.split('-');\n    newCoords.pop();\n    newCoords.push(newKey);\n    newCoords = newCoords.join('-');\n\n    onAdd(value, newCoords);\n    onRemove(coords);\n}\n",
         "import {getBlankData, getSyncedData} from './data';\nimport {getArrayFormRow, getObjectFormRow} from './ui';\nimport {EditorContext} from './util';\n\n\nexport default class Form extends React.Component {\n    constructor(props) {\n        super(props);\n\n        this.dataInput = document.getElementById(this.props.dataInputId);\n        this.schema = props.schema;\n\n        let data = props.data;\n\n        if (!data) {\n            // create empty data from schema\n            data = getBlankData(this.schema);\n        } else {\n            // data might be stale if schema has new keys, so add them to data\n            try {\n                data = getSyncedData(data, this.schema);\n            } catch (error) {\n                console.error(\"Error: Schema and data structure don't match\");\n                console.error(error);\n            }\n        }\n\n        this.state = {\n            value: '',\n            data: data\n        };\n        \n        // update data in the input\n        this.populateDataInput();\n    }\n\n    componentDidUpdate(prevProps, prevState) {\n        if (this.state.data !== prevState.data) {\n            this.populateDataInput();\n        }\n    }\n\n    populateDataInput = () => {\n        this.dataInput.value = JSON.stringify(this.state.data);\n    }\n\n    handleChange = (coords, value) => {\n        /*\n            e.target.name is a chain of indices and keys:\n            xxx-0-key-1-key2 and so on.\n            These can be used as coordinates to locate \n            a particular deeply nested item.\n\n            This first coordinate is not important and should be removed.\n        */\n        coords = coords.split('-');\n\n        coords.shift(); // remove first coord\n\n        function setDataUsingCoords(coords, data, value) {\n            let coord = coords.shift();\n            if (!isNaN(Number(coord)))\n                coord = Number(coord);\n\n            if (coords.length) {\n                setDataUsingCoords(coords, data[coord], value);\n            } else {\n                data[coord] = value;\n            }\n        }\n\n        let _data = JSON.parse(JSON.stringify(this.state.data));\n\n        setDataUsingCoords(coords, _data, value);\n\n        this.setState({data: _data});\n    }\n\n    getFields = () => {\n        let data = this.state.data;\n        let formGroups = [];\n\n        try {\n            let type = this.schema.type;\n    \n            if (type === 'list')\n                type = 'array';\n            else if (type === 'dict')\n                type = 'object';\n\n            let args = {\n                data: data,\n                schema: this.schema,\n                name: 'rjf',\n                onChange: this.handleChange,\n                onAdd: this.addFieldset,\n                onRemove: this.removeFieldset,\n                onMove: this.moveFieldset,\n                level: 0\n            };\n\n            if (type === 'array') {\n                return getArrayFormRow(args);\n            } else if (type === 'object') {\n                return getObjectFormRow(args);\n            }\n        } catch (error) {\n            formGroups = (\n                <p style={{color: '#f00'}}>\n                    <strong>(!) Error:</strong> Schema and data structure do not match.\n                </p>\n            );\n        }\n\n        return formGroups;\n    }\n\n    addFieldset = (blankData, coords) => {\n        coords = coords.split('-');\n        coords.shift();\n\n        this.setState((state) => {\n            let _data = JSON.parse(JSON.stringify(state.data));\n\n            addDataUsingCoords(coords, _data, blankData);\n\n            return {data: _data};\n        });\n    }\n\n    removeFieldset = (coords) => {\n        coords = coords.split('-');\n        coords.shift();\n\n        this.setState((state) => {\n            let _data = JSON.parse(JSON.stringify(state.data));\n\n            removeDataUsingCoords(coords, _data);\n\n            return {data: _data};\n        });\n    }\n\n    moveFieldset = (oldCoords, newCoords) => {\n        oldCoords = oldCoords.split(\"-\");\n        oldCoords.shift();\n\n        newCoords = newCoords.split(\"-\");\n        newCoords.shift();\n\n        this.setState((state) => {\n            let _data = JSON.parse(JSON.stringify(state.data));\n\n            moveDataUsingCoords(oldCoords, newCoords, _data);\n\n            return {data: _data};\n        });\n    }\n\n    render() {\n        return (\n            <div className=\"rjf-form-wrapper\">\n                <fieldset className=\"module aligned\">\n                    <EditorContext.Provider \n                        value={{\n                            fileUploadEndpoint: this.props.fileUploadEndpoint,\n                            fieldName: this.props.fieldName,\n                            modelName: this.props.modelName,\n                        }}\n                    >\n                    {this.getFields()}\n                    </EditorContext.Provider>\n                </fieldset>\n            </div>\n        );\n    }\n}\n\n\nfunction addDataUsingCoords(coords, data, value) {\n    let coord = coords.shift();\n    if (!isNaN(Number(coord)))\n        coord = Number(coord);\n\n    if (coords.length) {\n        addDataUsingCoords(coords, data[coord], value);\n    } else {\n        if (Array.isArray(data[coord])) {\n            data[coord].push(value);\n        }\n        else {\n            if (Array.isArray(data)) {\n                data.push(value);\n            } else {\n                data[coord] = value;\n            }\n        }\n    }\n}\n\nfunction removeDataUsingCoords(coords, data) {\n    let coord = coords.shift();\n    if (!isNaN(Number(coord)))\n        coord = Number(coord);\n\n    if (coords.length) {\n        removeDataUsingCoords(coords, data[coord]);\n    } else {\n        if (Array.isArray(data))\n            data.splice(coord, 1); // in-place mutation\n        else\n            delete data[coord];\n    }\n}\n\n\nfunction moveDataUsingCoords(oldCoords, newCoords, data) {\n    let oldCoord = oldCoords.shift();\n\n    if (!isNaN(Number(oldCoord)))\n        oldCoord = Number(oldCoord);\n\n    if (oldCoords.length) {\n        moveDataUsingCoords(oldCoords, newCoords, data[oldCoord]);\n    } else {\n        if (Array.isArray(data)) {\n            /* Using newCoords allows us to move items from \n            one array to another. \n            However, for now, we're only moving items in a \n            single array.\n            */\n            let newCoord = newCoords[newCoords.length - 1];\n            \n            let item = data[oldCoord];\n\n            data.splice(oldCoord, 1);\n            data.splice(newCoord, 0, item);\n        }\n    }\n}\n",
         "import JSONForm from './renderer';\n\n\nexport default {\n  JSONForm,\n};",
         "import Form from './form';\n\n\nexport default function JSONForm(config) {\n    this.containerId = config.containerId;\n    this.dataInputId = config.dataInputId;\n    this.schema = config.schema;\n    this.data = config.data;\n    this.fileUploadEndpoint = config.fileUploadEndpoint;\n    this.fieldName = config.fieldName;\n    this.modelName = config.modelName;\n\n    this.render = function() {\n        ReactDOM.render(\n            <Form\n                schema={this.schema}\n                dataInputId={this.dataInputId}\n                data={this.data}\n                fileUploadEndpoint={this.fileUploadEndpoint}\n                fieldName={this.fieldName}\n                modelName={this.modelName}\n            />,\n            document.getElementById(this.containerId)\n        );\n    }\n}"
     ],
     "version": 3
 }
```

### Comparing `django-jsonform-2.8.1/django_jsonform/static/django_jsonform/style.css` & `django-jsonform-2.9.0/django_jsonform/static/django_jsonform/style.css`

 * *Files 18% similar despite different names*

```diff
@@ -68,29 +68,43 @@
     font-size: 13px;
 }
 .rjf-form-group input[readonly] {
     background-color: #eee;
     outline: 0;
 }
 
-.rjf-form-row label + div {
-    margin-left: 170px;
+.rjf-input-group {
     display: table;
-    width: 19.4em;
+    width: 19.4em
 }
 
-.rjf-file-field {
-    color: #666;
+.rjf-check-input > label {
+    display: table;
+    float: none;
+    width: auto;
+}
+
+.rjf-help-text {
+    font-size: 11px;
+    color: var(--body-quiet-color);
+    display: block;
+    margin-top: 4px;
 }
 
-.rjf-file-field .rjf-file-field-input {
+.rjf-check-input > .rjf-help-text {
+    margin-top: 0;
+}
+
+.rjf-file-field {
+    color: #666;
     display: inline-block;
 }
+
 .rjf-file-field .rjf-file-field-input input {
-    max-width: 18em;
+    width: 18em;
 }
 
 .rjf-current-file-name {
     color: #666;
     max-width: 18em;
     margin-bottom: 0.5em;
 }
@@ -199,27 +213,34 @@
 .rjf-move-down-button:hover {
     background-position: 0px -60px;
 }
 
 .rjf-edit-button {
     text-indent: -9999px;
     background: url(./img/icon-changelink.svg) 0 1px no-repeat;
-    width: 3px;
+    width: 16px;
     height: 16px;
     border: 0px none;
     cursor: pointer;
+    margin-left: 2px;
+}
+.rjf-edit-button:hover {
+    border: 0;
 }
 
 .rjf-icon {
     width: 1.2em;
     height: 1.2em;
     display: inline-block;
 }
 
-.rjf-datetime-field-inner::after {
+.rjf-datetime-field-inner {
+    display: inline-block;
+}
+.rjf-datetime-field-inputs::after {
     display: table;
     content: " ";
     clear: both;
 }
 .rjf-datetime-field-date,
 .rjf-datetime-field-time {
     float: left;
@@ -228,16 +249,20 @@
     box-sizing: border-box;
     position: relative;
 }
 .rjf-datetime-field-date > div > label,
 .rjf-datetime-field-time > div > label {
     display: none;
 }
-.rjf-datetime-field-date > div > input,
-.rjf-datetime-field-time > div > input {
+.rjf-datetime-field-date .rjf-input-group,
+.rjf-datetime-field-time .rjf-input-group {
+    width: 100%;
+}
+.rjf-datetime-field-date .rjf-input-group > input,
+.rjf-datetime-field-time .rjf-input-group > input {
     width: 100%;
     margin-left: 0;
     box-sizing: border-box;
 }
 .rjf-time-picker {
     width: 18em;
     position: absolute;
@@ -447,15 +472,15 @@
         width: 100%;
     }
 
     .rjf-form-row label input[type="checkbox"] {
         width: auto;
     }
 
-    .rjf-form-row label + div {
+    .rjf-input-group {
         width: 100%;
     }
 
     .rjf-form-row > .rjf-form-row-controls {
         right: -0.4rem;
     }
 
@@ -487,15 +512,15 @@
 
     .rjf-multiselect-field-options-container {
         width: calc(100% + 60px);
     }
 }
 
 @media(max-width: 1024px) {
-    .rjf-form-row label + div {
+    .rjf-input-group {
         margin-left: 0;
     }
 
     .form-row input[type="date"],
     .form-row input[type="time"] {
         box-sizing: border-box;
         margin: 0;
@@ -505,7 +530,94 @@
     }
 
     .rjf-multiselect-field-input {
         padding-right: 32px !important;
         background-position: right 8px center;
     }
 }
+
+
+/* Styles for Grappelli admin */
+
+.grp-module .rjf-add-button {
+    padding: 0 2px 0 16px;
+    margin-top: 8px;
+    margin-left: 0;
+    width: auto;
+    height: auto;
+    border: 0;
+    border-radius: 2px;
+}
+.grp-module .rjf-remove-file-button {
+    padding: 0 1px;
+    margin-left: 0;
+    width: auto;
+    height: auto;
+    display: inline-block;
+    vertical-align: middle;
+    border-radius: 2px;
+    border: 0;
+}
+.grp-module .rjf-add-button:hover,
+.grp-module .rjf-remove-file-button:hover {
+    border: 0;
+}
+.grp-module .rjf-form-row-inner label {
+    display: block;
+    padding: 4px 10px 0 0;
+    float: left;
+    width: 140px;
+    word-wrap: break-word;
+    line-height: 1;
+}
+.grp-module .rjf-multiselect-field-option label {
+    width: 100%;
+    float: none;
+    margin: 0 !important;
+}
+.grp-module input[readonly] {
+    border: 1px solid #ccc !important;
+    box-shadow: inset 0 1px 3px 0 #eee !important;
+    cursor: default;    
+}
+.grp-module .rjf-multiselect-field-input {
+    cursor: pointer;
+    padding-right: 28px !important;
+    background-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16'%3e%3cpath fill='none' stroke='%23777777' stroke-linecap='round' stroke-linejoin='round' stroke-width='2' d='M2 5l6 6 6-6'/%3e%3c/svg%3e") !important;
+    background-repeat: no-repeat !important;
+    background-position: right 6px center !important;
+    background-size: 16px 12px !important;
+}
+.grp-module .rjf-form-row input[type="date"],
+.grp-module .rjf-form-row input[type="time"] {
+    border: 1px solid #ccc !important;
+    margin-top: 0;
+    color: #333;
+    background-color: #fdfdfd !important;
+    box-shadow: inset 0 1px 3px 0 #eee !important;
+    padding: 2px 6px;
+    border-radius: 3px;
+}
+.grp-module .rjf-datetime-field-date,
+.grp-module .rjf-datetime-field-time {
+    width: 9.2em;
+}
+.grp-module .rjf-datetime-field-date > div > label,
+.grp-module .rjf-datetime-field-time > div > label {
+    display: none;
+}
+.grp-module .rjf-time-picker button {
+    margin-left: 0;
+}
+.grp-module .rjf-multiselect-field-input {
+    background-color: #fdfdfd !important;
+    cursor: pointer !important;
+}
+.grp-module .rjf-check-input > label {
+    display: table;
+    float: none;
+    width: auto;
+}
+.grp-module .rjf-help-text {
+    color: #888;
+}
+
```

### Comparing `django-jsonform-2.8.1/django_jsonform/static/django_jsonform/vendor/react-dom.production.min.js` & `django-jsonform-2.9.0/django_jsonform/static/django_jsonform/vendor/react-dom.production.min.js`

 * *Files identical despite different names*

### Comparing `django-jsonform-2.8.1/django_jsonform/static/django_jsonform/vendor/react.production.min.js` & `django-jsonform-2.9.0/django_jsonform/static/django_jsonform/vendor/react.production.min.js`

 * *Files identical despite different names*

### Comparing `django-jsonform-2.8.1/django_jsonform/templates/django_jsonform/editor.html` & `django-jsonform-2.9.0/django_jsonform/templates/django_jsonform/editor.html`

 * *Files identical despite different names*

### Comparing `django-jsonform-2.8.1/django_jsonform/utils.py` & `django-jsonform-2.9.0/django_jsonform/utils.py`

 * *Files identical despite different names*

### Comparing `django-jsonform-2.8.1/django_jsonform/widgets.py` & `django-jsonform-2.9.0/django_jsonform/widgets.py`

 * *Files identical despite different names*

### Comparing `django-jsonform-2.8.1/django_jsonform.egg-info/PKG-INFO` & `django-jsonform-2.9.0/django_jsonform.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-jsonform
-Version: 2.8.1
+Version: 2.9.0
 Summary: A user-friendly JSON editing form for Django admin.
 Home-page: https://www.github.com/bhch/django-jsonform
 Author: Bharat Chauhan
 Author-email: tell.bhch@gmail.com
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-jsonform Version: 2.8.1 Summary: A user-
+Metadata-Version: 2.1 Name: django-jsonform Version: 2.9.0 Summary: A user-
 friendly JSON editing form for Django admin. Home-page: https://www.github.com/
 bhch/django-jsonform Author: Bharat Chauhan Author-email: tell.bhch@gmail.com
 License: BSD-3-Clause Platform: UNKNOWN Classifier: Environment :: Web
 Environment Classifier: Framework :: Django Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: BSD License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

### Comparing `django-jsonform-2.8.1/django_jsonform.egg-info/SOURCES.txt` & `django-jsonform-2.9.0/django_jsonform.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -31,12 +31,15 @@
 django_jsonform/static/django_jsonform/img/control-icons.svg
 django_jsonform/static/django_jsonform/img/icon-addlink.svg
 django_jsonform/static/django_jsonform/img/icon-changelink.svg
 django_jsonform/static/django_jsonform/img/icon-deletelink.svg
 django_jsonform/static/django_jsonform/vendor/react-dom.production.min.js
 django_jsonform/static/django_jsonform/vendor/react.production.min.js
 django_jsonform/templates/django_jsonform/editor.html
+django_jsonform/templatetags/__init__.py
+django_jsonform/templatetags/django_jsonform.py
 tests/__init__.py
 tests/__main__.py
 tests/django_settings.py
+tests/test_templatetags.py
 tests/test_utils.py
 tests/test_widgets.py
```

### Comparing `django-jsonform-2.8.1/setup.cfg` & `django-jsonform-2.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-jsonform-2.8.1/tests/django_settings.py` & `django-jsonform-2.9.0/tests/django_settings.py`

 * *Files identical despite different names*

### Comparing `django-jsonform-2.8.1/tests/test_utils.py` & `django-jsonform-2.9.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-jsonform-2.8.1/tests/test_widgets.py` & `django-jsonform-2.9.0/tests/test_widgets.py`

 * *Files identical despite different names*

