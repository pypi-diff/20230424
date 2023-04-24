# Comparing `tmp/huscy.project_consents-0.4.0a6.tar.gz` & `tmp/huscy.project_consents-0.4.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huscy.project_consents-0.4.0a6.tar", last modified: Fri Apr 21 14:34:44 2023, max compression
+gzip compressed data, was "huscy.project_consents-0.4.0a7.tar", last modified: Mon Apr 24 10:37:45 2023, max compression
```

## Comparing `huscy.project_consents-0.4.0a6.tar` & `huscy.project_consents-0.4.0a7.tar`

### file list

```diff
@@ -1,32 +1,36 @@
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-21 14:34:44.033269 huscy.project_consents-0.4.0a6/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)    34523 2022-12-05 12:04:00.000000 huscy.project_consents-0.4.0a6/LICENSE
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1101 2023-04-21 14:34:44.033269 huscy.project_consents-0.4.0a6/PKG-INFO
--rw-rw-r--   0 lotus     (1000) lotus     (1000)       19 2022-09-12 13:32:12.000000 huscy.project_consents-0.4.0a6/README.md
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-21 14:34:44.033269 huscy.project_consents-0.4.0a6/huscy/
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-21 14:34:44.033269 huscy.project_consents-0.4.0a6/huscy/project_consents/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)       81 2023-04-21 14:34:31.000000 huscy.project_consents-0.4.0a6/huscy/project_consents/__init__.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      435 2023-04-21 12:57:46.000000 huscy.project_consents-0.4.0a6/huscy/project_consents/admin.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      479 2023-04-21 13:33:05.000000 huscy.project_consents-0.4.0a6/huscy/project_consents/api_urls.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      194 2022-12-05 12:04:00.000000 huscy.project_consents-0.4.0a6/huscy/project_consents/apps.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      684 2023-04-21 08:48:37.000000 huscy.project_consents-0.4.0a6/huscy/project_consents/forms.py
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-21 14:34:44.033269 huscy.project_consents-0.4.0a6/huscy/project_consents/migrations/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     2492 2023-04-21 14:34:41.000000 huscy.project_consents-0.4.0a6/huscy/project_consents/migrations/0001_initial.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)        0 2022-12-08 10:36:34.000000 huscy.project_consents-0.4.0a6/huscy/project_consents/migrations/__init__.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1495 2023-04-20 11:49:39.000000 huscy.project_consents-0.4.0a6/huscy/project_consents/models.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1304 2023-01-30 14:04:08.000000 huscy.project_consents-0.4.0a6/huscy/project_consents/serializer.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1171 2023-01-24 10:55:08.000000 huscy.project_consents-0.4.0a6/huscy/project_consents/services.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      430 2023-04-21 09:36:45.000000 huscy.project_consents-0.4.0a6/huscy/project_consents/urls.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     2919 2023-04-21 12:54:19.000000 huscy.project_consents-0.4.0a6/huscy/project_consents/views.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1527 2023-01-13 21:29:30.000000 huscy.project_consents-0.4.0a6/huscy/project_consents/viewsets.py
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-21 14:34:44.033269 huscy.project_consents-0.4.0a6/huscy.project_consents.egg-info/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1101 2023-04-21 14:34:44.000000 huscy.project_consents-0.4.0a6/huscy.project_consents.egg-info/PKG-INFO
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      833 2023-04-21 14:34:44.000000 huscy.project_consents-0.4.0a6/huscy.project_consents.egg-info/SOURCES.txt
--rw-rw-r--   0 lotus     (1000) lotus     (1000)        1 2023-04-21 14:34:44.000000 huscy.project_consents-0.4.0a6/huscy.project_consents.egg-info/dependency_links.txt
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      115 2023-04-21 14:34:44.000000 huscy.project_consents-0.4.0a6/huscy.project_consents.egg-info/requires.txt
--rw-rw-r--   0 lotus     (1000) lotus     (1000)        6 2023-04-21 14:34:44.000000 huscy.project_consents-0.4.0a6/huscy.project_consents.egg-info/top_level.txt
--rw-rw-r--   0 lotus     (1000) lotus     (1000)       38 2023-04-21 14:34:44.033269 huscy.project_consents-0.4.0a6/setup.cfg
--rwxrwxr-x   0 lotus     (1000) lotus     (1000)     1642 2023-04-20 09:24:18.000000 huscy.project_consents-0.4.0a6/setup.py
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-21 14:34:44.033269 huscy.project_consents-0.4.0a6/tests/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      760 2023-01-30 14:04:08.000000 huscy.project_consents-0.4.0a6/tests/test_project_consent_category_serializer.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      684 2023-01-30 14:04:08.000000 huscy.project_consents-0.4.0a6/tests/test_project_consent_serializer.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     5532 2023-01-24 10:55:08.000000 huscy.project_consents-0.4.0a6/tests/test_viewsets.py
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-24 10:37:45.153574 huscy.project_consents-0.4.0a7/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)    34523 2022-12-05 12:04:00.000000 huscy.project_consents-0.4.0a7/LICENSE
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)       39 2023-04-24 10:37:15.000000 huscy.project_consents-0.4.0a7/MANIFEST.in
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     1101 2023-04-24 10:37:45.153574 huscy.project_consents-0.4.0a7/PKG-INFO
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)       19 2022-09-12 13:32:12.000000 huscy.project_consents-0.4.0a7/README.md
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-24 10:37:45.149574 huscy.project_consents-0.4.0a7/huscy/
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-24 10:37:45.153574 huscy.project_consents-0.4.0a7/huscy/project_consents/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)       81 2023-04-24 10:37:32.000000 huscy.project_consents-0.4.0a7/huscy/project_consents/__init__.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      435 2023-04-21 12:57:46.000000 huscy.project_consents-0.4.0a7/huscy/project_consents/admin.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      479 2023-04-21 13:33:05.000000 huscy.project_consents-0.4.0a7/huscy/project_consents/api_urls.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      194 2022-12-05 12:04:00.000000 huscy.project_consents-0.4.0a7/huscy/project_consents/apps.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      684 2023-04-21 08:48:37.000000 huscy.project_consents-0.4.0a7/huscy/project_consents/forms.py
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-24 10:37:45.153574 huscy.project_consents-0.4.0a7/huscy/project_consents/migrations/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     2492 2023-04-24 10:37:42.000000 huscy.project_consents-0.4.0a7/huscy/project_consents/migrations/0001_initial.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)        0 2022-12-08 10:36:34.000000 huscy.project_consents-0.4.0a7/huscy/project_consents/migrations/__init__.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     1495 2023-04-20 11:49:39.000000 huscy.project_consents-0.4.0a7/huscy/project_consents/models.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     1304 2023-01-30 14:04:08.000000 huscy.project_consents-0.4.0a7/huscy/project_consents/serializer.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     1171 2023-01-24 10:55:08.000000 huscy.project_consents-0.4.0a7/huscy/project_consents/services.py
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-24 10:37:45.149574 huscy.project_consents-0.4.0a7/huscy/project_consents/templates/
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-24 10:37:45.153574 huscy.project_consents-0.4.0a7/huscy/project_consents/templates/project_consents/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      731 2023-04-21 09:45:41.000000 huscy.project_consents-0.4.0a7/huscy/project_consents/templates/project_consents/projectconsenttoken.html
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      430 2023-04-21 09:36:45.000000 huscy.project_consents-0.4.0a7/huscy/project_consents/urls.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     2919 2023-04-21 12:54:19.000000 huscy.project_consents-0.4.0a7/huscy/project_consents/views.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     1527 2023-01-13 21:29:30.000000 huscy.project_consents-0.4.0a7/huscy/project_consents/viewsets.py
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-24 10:37:45.149574 huscy.project_consents-0.4.0a7/huscy.project_consents.egg-info/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     1101 2023-04-24 10:37:45.000000 huscy.project_consents-0.4.0a7/huscy.project_consents.egg-info/PKG-INFO
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      920 2023-04-24 10:37:45.000000 huscy.project_consents-0.4.0a7/huscy.project_consents.egg-info/SOURCES.txt
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)        1 2023-04-24 10:37:45.000000 huscy.project_consents-0.4.0a7/huscy.project_consents.egg-info/dependency_links.txt
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      115 2023-04-24 10:37:45.000000 huscy.project_consents-0.4.0a7/huscy.project_consents.egg-info/requires.txt
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)        6 2023-04-24 10:37:45.000000 huscy.project_consents-0.4.0a7/huscy.project_consents.egg-info/top_level.txt
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)       38 2023-04-24 10:37:45.153574 huscy.project_consents-0.4.0a7/setup.cfg
+-rwxrwxr-x   0 lotus     (1000) lotus     (1000)     1673 2023-04-24 10:36:29.000000 huscy.project_consents-0.4.0a7/setup.py
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-24 10:37:45.153574 huscy.project_consents-0.4.0a7/tests/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      760 2023-01-30 14:04:08.000000 huscy.project_consents-0.4.0a7/tests/test_project_consent_category_serializer.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      684 2023-01-30 14:04:08.000000 huscy.project_consents-0.4.0a7/tests/test_project_consent_serializer.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     5532 2023-01-24 10:55:08.000000 huscy.project_consents-0.4.0a7/tests/test_viewsets.py
```

### Comparing `huscy.project_consents-0.4.0a6/LICENSE` & `huscy.project_consents-0.4.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.4.0a6/PKG-INFO` & `huscy.project_consents-0.4.0a7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huscy.project_consents
-Version: 0.4.0a6
+Version: 0.4.0a7
 Summary: projects_consents
 Home-page: https://bitbucket.org/huscy/project_consents
 Author: Gefan Qian, Stefan Bunde
 Author-email: gefan.qian@gmail.com, stefanbunde+git@posteo.de
 License: AGPLv3+
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `huscy.project_consents-0.4.0a6/huscy/project_consents/forms.py` & `huscy.project_consents-0.4.0a7/huscy/project_consents/forms.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.4.0a6/huscy/project_consents/migrations/0001_initial.py` & `huscy.project_consents-0.4.0a7/huscy/project_consents/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# Generated by Django 4.2 on 2023-04-21 14:34
+# Generated by Django 4.2 on 2023-04-24 10:37
 
 from django.db import migrations, models
 import django.db.models.deletion
 import uuid
 
 
 class Migration(migrations.Migration):
 
     initial = True
 
     dependencies = [
-        ('consents', '0001_initial'),
         ('projects', '0002_alter_membership_options'),
         ('subjects', '0001_squashed_0009_delete_contactold'),
+        ('consents', '0001_initial'),
     ]
 
     operations = [
         migrations.CreateModel(
             name='ProjectConsent',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
```

### Comparing `huscy.project_consents-0.4.0a6/huscy/project_consents/models.py` & `huscy.project_consents-0.4.0a7/huscy/project_consents/models.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.4.0a6/huscy/project_consents/serializer.py` & `huscy.project_consents-0.4.0a7/huscy/project_consents/serializer.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.4.0a6/huscy/project_consents/services.py` & `huscy.project_consents-0.4.0a7/huscy/project_consents/services.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.4.0a6/huscy/project_consents/views.py` & `huscy.project_consents-0.4.0a7/huscy/project_consents/views.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.4.0a6/huscy/project_consents/viewsets.py` & `huscy.project_consents-0.4.0a7/huscy/project_consents/viewsets.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.4.0a6/huscy.project_consents.egg-info/PKG-INFO` & `huscy.project_consents-0.4.0a7/huscy.project_consents.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huscy.project-consents
-Version: 0.4.0a6
+Version: 0.4.0a7
 Summary: projects_consents
 Home-page: https://bitbucket.org/huscy/project_consents
 Author: Gefan Qian, Stefan Bunde
 Author-email: gefan.qian@gmail.com, stefanbunde+git@posteo.de
 License: AGPLv3+
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `huscy.project_consents-0.4.0a6/huscy.project_consents.egg-info/SOURCES.txt` & `huscy.project_consents-0.4.0a7/huscy.project_consents.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE
+MANIFEST.in
 README.md
 setup.py
 huscy.project_consents.egg-info/PKG-INFO
 huscy.project_consents.egg-info/SOURCES.txt
 huscy.project_consents.egg-info/dependency_links.txt
 huscy.project_consents.egg-info/requires.txt
 huscy.project_consents.egg-info/top_level.txt
@@ -15,10 +16,11 @@
 huscy/project_consents/serializer.py
 huscy/project_consents/services.py
 huscy/project_consents/urls.py
 huscy/project_consents/views.py
 huscy/project_consents/viewsets.py
 huscy/project_consents/migrations/0001_initial.py
 huscy/project_consents/migrations/__init__.py
+huscy/project_consents/templates/project_consents/projectconsenttoken.html
 tests/test_project_consent_category_serializer.py
 tests/test_project_consent_serializer.py
 tests/test_viewsets.py
```

### Comparing `huscy.project_consents-0.4.0a6/setup.py` & `huscy.project_consents-0.4.0a7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
     author='Gefan Qian, Stefan Bunde',
     author_email='gefan.qian@gmail.com, stefanbunde+git@posteo.de',
 
     url='https://bitbucket.org/huscy/project_consents',
 
     packages=find_namespace_packages(include=['huscy.*']),
+    include_package_data=True,
 
     install_requires=[
         'django-qr-code',
         'huscy.consents',
         'huscy.projects',
         'huscy.subjects',
     ],
```

### Comparing `huscy.project_consents-0.4.0a6/tests/test_project_consent_category_serializer.py` & `huscy.project_consents-0.4.0a7/tests/test_project_consent_category_serializer.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.4.0a6/tests/test_project_consent_serializer.py` & `huscy.project_consents-0.4.0a7/tests/test_project_consent_serializer.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.4.0a6/tests/test_viewsets.py` & `huscy.project_consents-0.4.0a7/tests/test_viewsets.py`

 * *Files identical despite different names*

