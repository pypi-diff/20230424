# Comparing `tmp/django-jwt-oidc-1.0.7.tar.gz` & `tmp/django-jwt-oidc-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-jwt-oidc-1.0.7.tar", last modified: Sun Apr 23 20:52:35 2023, max compression
+gzip compressed data, was "django-jwt-oidc-1.0.8.tar", last modified: Mon Apr 24 13:42:59 2023, max compression
```

## Comparing `django-jwt-oidc-1.0.7.tar` & `django-jwt-oidc-1.0.8.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:52:35.311243 django-jwt-oidc-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-23 20:52:22.000000 django-jwt-oidc-1.0.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-23 20:52:22.000000 django-jwt-oidc-1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-04-23 20:52:35.311243 django-jwt-oidc-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-04-23 20:52:22.000000 django-jwt-oidc-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:52:35.307243 django-jwt-oidc-1.0.7/django_jwt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 20:52:22.000000 django-jwt-oidc-1.0.7/django_jwt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-23 20:52:22.000000 django-jwt-oidc-1.0.7/django_jwt/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-04-23 20:52:22.000000 django-jwt-oidc-1.0.7/django_jwt/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-23 20:52:22.000000 django-jwt-oidc-1.0.7/django_jwt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-04-23 20:52:22.000000 django-jwt-oidc-1.0.7/django_jwt/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:52:35.307243 django-jwt-oidc-1.0.7/django_jwt/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 20:52:22.000000 django-jwt-oidc-1.0.7/django_jwt/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-23 20:52:22.000000 django-jwt-oidc-1.0.7/django_jwt/openid.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-23 20:52:22.000000 django-jwt-oidc-1.0.7/django_jwt/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-23 20:52:22.000000 django-jwt-oidc-1.0.7/django_jwt/rest_framework.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:52:35.311243 django-jwt-oidc-1.0.7/django_jwt/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 20:52:22.000000 django-jwt-oidc-1.0.7/django_jwt/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-23 20:52:22.000000 django-jwt-oidc-1.0.7/django_jwt/server/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-23 20:52:22.000000 django-jwt-oidc-1.0.7/django_jwt/server/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-23 20:52:22.000000 django-jwt-oidc-1.0.7/django_jwt/server/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:52:35.311243 django-jwt-oidc-1.0.7/django_jwt/server/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-04-23 20:52:22.000000 django-jwt-oidc-1.0.7/django_jwt/server/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-23 20:52:22.000000 django-jwt-oidc-1.0.7/django_jwt/server/migrations/0002_webpage_logout_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-04-23 20:52:22.000000 django-jwt-oidc-1.0.7/django_jwt/server/migrations/0003_nonceused_privateclaimswebpage_restrictuserstoweb_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 20:52:22.000000 django-jwt-oidc-1.0.7/django_jwt/server/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-04-23 20:52:22.000000 django-jwt-oidc-1.0.7/django_jwt/server/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-23 20:52:22.000000 django-jwt-oidc-1.0.7/django_jwt/server/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-23 20:52:22.000000 django-jwt-oidc-1.0.7/django_jwt/server/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:52:35.307243 django-jwt-oidc-1.0.7/django_jwt/server/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:52:35.311243 django-jwt-oidc-1.0.7/django_jwt/server/templates/django_jwt/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-23 20:52:22.000000 django-jwt-oidc-1.0.7/django_jwt/server/templates/django_jwt/oidc_confirmation.html
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-23 20:52:22.000000 django-jwt-oidc-1.0.7/django_jwt/server/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    17307 2023-04-23 20:52:22.000000 django-jwt-oidc-1.0.7/django_jwt/server/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-23 20:52:22.000000 django-jwt-oidc-1.0.7/django_jwt/server/views_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-23 20:52:22.000000 django-jwt-oidc-1.0.7/django_jwt/settings_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:52:35.307243 django-jwt-oidc-1.0.7/django_jwt/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:52:35.311243 django-jwt-oidc-1.0.7/django_jwt/templates/django_jwt/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-23 20:52:22.000000 django-jwt-oidc-1.0.7/django_jwt/templates/django_jwt/fake_login.html
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-23 20:52:22.000000 django-jwt-oidc-1.0.7/django_jwt/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-23 20:52:22.000000 django-jwt-oidc-1.0.7/django_jwt/view_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9316 2023-04-23 20:52:22.000000 django-jwt-oidc-1.0.7/django_jwt/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 20:52:35.311243 django-jwt-oidc-1.0.7/django_jwt_oidc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-04-23 20:52:35.000000 django-jwt-oidc-1.0.7/django_jwt_oidc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-23 20:52:35.000000 django-jwt-oidc-1.0.7/django_jwt_oidc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 20:52:35.000000 django-jwt-oidc-1.0.7/django_jwt_oidc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-23 20:52:35.000000 django-jwt-oidc-1.0.7/django_jwt_oidc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-23 20:52:35.000000 django-jwt-oidc-1.0.7/django_jwt_oidc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-23 20:52:22.000000 django-jwt-oidc-1.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 20:52:35.311243 django-jwt-oidc-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-23 20:52:22.000000 django-jwt-oidc-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:42:59.718811 django-jwt-oidc-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-24 13:42:46.000000 django-jwt-oidc-1.0.8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-24 13:42:46.000000 django-jwt-oidc-1.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-04-24 13:42:59.718811 django-jwt-oidc-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-04-24 13:42:46.000000 django-jwt-oidc-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:42:59.714811 django-jwt-oidc-1.0.8/django_jwt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:42:46.000000 django-jwt-oidc-1.0.8/django_jwt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-24 13:42:46.000000 django-jwt-oidc-1.0.8/django_jwt/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-04-24 13:42:46.000000 django-jwt-oidc-1.0.8/django_jwt/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-24 13:42:46.000000 django-jwt-oidc-1.0.8/django_jwt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-04-24 13:42:46.000000 django-jwt-oidc-1.0.8/django_jwt/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:42:59.714811 django-jwt-oidc-1.0.8/django_jwt/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:42:46.000000 django-jwt-oidc-1.0.8/django_jwt/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-24 13:42:46.000000 django-jwt-oidc-1.0.8/django_jwt/openid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-24 13:42:46.000000 django-jwt-oidc-1.0.8/django_jwt/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-24 13:42:46.000000 django-jwt-oidc-1.0.8/django_jwt/rest_framework.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:42:59.714811 django-jwt-oidc-1.0.8/django_jwt/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:42:46.000000 django-jwt-oidc-1.0.8/django_jwt/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-24 13:42:46.000000 django-jwt-oidc-1.0.8/django_jwt/server/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-24 13:42:46.000000 django-jwt-oidc-1.0.8/django_jwt/server/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-24 13:42:46.000000 django-jwt-oidc-1.0.8/django_jwt/server/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:42:59.714811 django-jwt-oidc-1.0.8/django_jwt/server/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-04-24 13:42:46.000000 django-jwt-oidc-1.0.8/django_jwt/server/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-24 13:42:46.000000 django-jwt-oidc-1.0.8/django_jwt/server/migrations/0002_webpage_logout_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-04-24 13:42:46.000000 django-jwt-oidc-1.0.8/django_jwt/server/migrations/0003_nonceused_privateclaimswebpage_restrictuserstoweb_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:42:46.000000 django-jwt-oidc-1.0.8/django_jwt/server/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-04-24 13:42:46.000000 django-jwt-oidc-1.0.8/django_jwt/server/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-24 13:42:46.000000 django-jwt-oidc-1.0.8/django_jwt/server/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-24 13:42:46.000000 django-jwt-oidc-1.0.8/django_jwt/server/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:42:59.710811 django-jwt-oidc-1.0.8/django_jwt/server/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:42:59.714811 django-jwt-oidc-1.0.8/django_jwt/server/templates/django_jwt/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-24 13:42:46.000000 django-jwt-oidc-1.0.8/django_jwt/server/templates/django_jwt/oidc_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-24 13:42:46.000000 django-jwt-oidc-1.0.8/django_jwt/server/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17526 2023-04-24 13:42:46.000000 django-jwt-oidc-1.0.8/django_jwt/server/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-24 13:42:46.000000 django-jwt-oidc-1.0.8/django_jwt/server/views_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-24 13:42:46.000000 django-jwt-oidc-1.0.8/django_jwt/settings_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:42:59.710811 django-jwt-oidc-1.0.8/django_jwt/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:42:59.718811 django-jwt-oidc-1.0.8/django_jwt/templates/django_jwt/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-24 13:42:46.000000 django-jwt-oidc-1.0.8/django_jwt/templates/django_jwt/fake_login.html
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-24 13:42:46.000000 django-jwt-oidc-1.0.8/django_jwt/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-24 13:42:46.000000 django-jwt-oidc-1.0.8/django_jwt/view_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9366 2023-04-24 13:42:46.000000 django-jwt-oidc-1.0.8/django_jwt/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:42:59.718811 django-jwt-oidc-1.0.8/django_jwt_oidc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-04-24 13:42:59.000000 django-jwt-oidc-1.0.8/django_jwt_oidc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-24 13:42:59.000000 django-jwt-oidc-1.0.8/django_jwt_oidc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:42:59.000000 django-jwt-oidc-1.0.8/django_jwt_oidc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-24 13:42:59.000000 django-jwt-oidc-1.0.8/django_jwt_oidc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-24 13:42:59.000000 django-jwt-oidc-1.0.8/django_jwt_oidc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-24 13:42:46.000000 django-jwt-oidc-1.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 13:42:59.718811 django-jwt-oidc-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-24 13:42:46.000000 django-jwt-oidc-1.0.8/setup.py
```

### Comparing `django-jwt-oidc-1.0.7/LICENSE.md` & `django-jwt-oidc-1.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0.7/PKG-INFO` & `django-jwt-oidc-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-jwt-oidc
-Version: 1.0.7
+Version: 1.0.8
 Summary: Django library that implements the authentification for OpenId SSO with JWT from oauth2.
 Home-page: https://github.com/Casassarnau/django-jwt
 Author: Arnau Casas Saez
 Author-email: casassarnau@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Casassarnau/django-jwt/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `django-jwt-oidc-1.0.7/README.md` & `django-jwt-oidc-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0.7/django_jwt/apps.py` & `django-jwt-oidc-1.0.8/django_jwt/apps.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0.7/django_jwt/auth.py` & `django-jwt-oidc-1.0.8/django_jwt/auth.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0.7/django_jwt/middleware.py` & `django-jwt-oidc-1.0.8/django_jwt/middleware.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0.7/django_jwt/openid.py` & `django-jwt-oidc-1.0.8/django_jwt/openid.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0.7/django_jwt/rest_framework.py` & `django-jwt-oidc-1.0.8/django_jwt/rest_framework.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0.7/django_jwt/server/admin.py` & `django-jwt-oidc-1.0.8/django_jwt/server/admin.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0.7/django_jwt/server/apps.py` & `django-jwt-oidc-1.0.8/django_jwt/server/apps.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0.7/django_jwt/server/forms.py` & `django-jwt-oidc-1.0.8/django_jwt/server/forms.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0.7/django_jwt/server/migrations/0001_initial.py` & `django-jwt-oidc-1.0.8/django_jwt/server/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0.7/django_jwt/server/migrations/0002_webpage_logout_all.py` & `django-jwt-oidc-1.0.8/django_jwt/server/migrations/0002_webpage_logout_all.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0.7/django_jwt/server/migrations/0003_nonceused_privateclaimswebpage_restrictuserstoweb_and_more.py` & `django-jwt-oidc-1.0.8/django_jwt/server/migrations/0003_nonceused_privateclaimswebpage_restrictuserstoweb_and_more.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0.7/django_jwt/server/models.py` & `django-jwt-oidc-1.0.8/django_jwt/server/models.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0.7/django_jwt/server/templates/django_jwt/oidc_confirmation.html` & `django-jwt-oidc-1.0.8/django_jwt/server/templates/django_jwt/oidc_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0.7/django_jwt/server/urls.py` & `django-jwt-oidc-1.0.8/django_jwt/server/urls.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0.7/django_jwt/server/views.py` & `django-jwt-oidc-1.0.8/django_jwt/server/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from django.shortcuts import redirect, render
 from django.urls import reverse
 from django.utils import timezone
 from django.utils.http import urlencode
 from django.utils.module_loading import import_string
 from django.views import View
 from django.views.generic import TemplateView
+from jwcrypto.jwt import JWTExpired
 from rest_framework import viewsets, mixins
 from rest_framework.permissions import IsAuthenticated
 
 from django_jwt.auth import JWTAuthentication
 from django_jwt.rest_framework import JWTTokenAuthentication
 
 from django_jwt.settings_utils import get_setting, get_domain_from_url
@@ -228,16 +229,20 @@
         return response_object
 
     def refresh_token_response(self, web: WebPage):
         try:
             sub_attr = web.privateclaimswebpage_set.get(claim='sub').attribute_from_user_model.replace('.', '__')
         except PrivateClaimsWebPage.DoesNotExist:
             sub_attr = 'pk'
-        user, claims = JWTAuthentication.validate_authorization_jwt(key=self.request.POST.get('refresh_token', None),
-                                                                    sub_attr=sub_attr)
+        try:
+            user, claims = JWTAuthentication.validate_authorization_jwt(key=self.request.POST.get('refresh_token',
+                                                                                                  None),
+                                                                        sub_attr=sub_attr)
+        except JWTExpired:
+            raise PermissionDenied()
         scopes = claims.get('scope', '').split(' ')
         try:
             external_session = UserExternalSession.objects.get(id=claims.get('sid', None))
         except UserExternalSession.DoesNotExist:
             raise PermissionDenied()
         if str(external_session.refresh_token) != str(claims.get('jti', 0)):
             external_session.delete()
```

### Comparing `django-jwt-oidc-1.0.7/django_jwt/server/views_utils.py` & `django-jwt-oidc-1.0.8/django_jwt/server/views_utils.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0.7/django_jwt/settings_utils.py` & `django-jwt-oidc-1.0.8/django_jwt/settings_utils.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0.7/django_jwt/templates/django_jwt/fake_login.html` & `django-jwt-oidc-1.0.8/django_jwt/templates/django_jwt/fake_login.html`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0.7/django_jwt/urls.py` & `django-jwt-oidc-1.0.8/django_jwt/urls.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0.7/django_jwt/view_utils.py` & `django-jwt-oidc-1.0.8/django_jwt/view_utils.py`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0.7/django_jwt/views.py` & `django-jwt-oidc-1.0.8/django_jwt/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from django.http import JsonResponse, HttpResponseBadRequest
 from django.shortcuts import render, redirect
 from django.urls import reverse
 from django.utils import timezone
 from django.utils.crypto import get_random_string
 from django.utils.http import urlencode
 from django.views import View
+from jwcrypto.jwt import JWTExpired
 
 from django_jwt.auth import JWTAuthentication
 from django_jwt.openid import OpenId2Info
 from django_jwt.settings_utils import get_setting
 from django_jwt.view_utils import crear_url_amb_jwt, get_jwks, get_sub_jwt
 
 
@@ -73,15 +74,15 @@
             for key, value in JWTAuthentication.get_defaults_from_claims(json.loads(jwt.claims))[0].items():
                 if getattr(user, key, None) != value:
                     setattr(user, key, value)
                     changed = True
             if changed:
                 user.save()
             self.request.session[token_name] = jwt.serialize()
-        except JWTAuthentication.JWTException:
+        except (JWTAuthentication.JWTException, JWTExpired):
             logger.error('JWT authentication error.')
             return HttpResponseBadRequest('JWT authentication error.')
         return user
 
     def capture_authorization_flow_response(self, id_token=None, access_token=None):
         data = {
             'grant_type': 'authorization_code',
```

### Comparing `django-jwt-oidc-1.0.7/django_jwt_oidc.egg-info/PKG-INFO` & `django-jwt-oidc-1.0.8/django_jwt_oidc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-jwt-oidc
-Version: 1.0.7
+Version: 1.0.8
 Summary: Django library that implements the authentification for OpenId SSO with JWT from oauth2.
 Home-page: https://github.com/Casassarnau/django-jwt
 Author: Arnau Casas Saez
 Author-email: casassarnau@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Casassarnau/django-jwt/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `django-jwt-oidc-1.0.7/django_jwt_oidc.egg-info/SOURCES.txt` & `django-jwt-oidc-1.0.8/django_jwt_oidc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-jwt-oidc-1.0.7/setup.py` & `django-jwt-oidc-1.0.8/setup.py`

 * *Files identical despite different names*

