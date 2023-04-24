# Comparing `tmp/drf-social-oauth2-2.0.0.tar.gz` & `tmp/drf-social-oauth2-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-social-oauth2-2.0.0.tar", last modified: Sun Apr 16 15:47:25 2023, max compression
+gzip compressed data, was "drf-social-oauth2-2.1.0.tar", last modified: Mon Apr 24 13:22:46 2023, max compression
```

## Comparing `drf-social-oauth2-2.0.0.tar` & `drf-social-oauth2-2.1.0.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-16 15:47:25.345432 drf-social-oauth2-2.0.0/
--rw-r--r--   0 wagner.delima   (502) staff       (20)     3561 2022-01-21 09:44:31.000000 drf-social-oauth2-2.0.0/CHANGELOG.rst
--rw-r--r--   0 wagner.delima   (502) staff       (20)     1080 2020-06-27 18:20:06.000000 drf-social-oauth2-2.0.0/LICENSE.txt
--rw-r--r--   0 wagner.delima   (502) staff       (20)       81 2020-06-27 18:20:06.000000 drf-social-oauth2-2.0.0/MANIFEST.in
--rw-r--r--   0 wagner.delima   (502) staff       (20)    20590 2023-04-16 15:47:25.344896 drf-social-oauth2-2.0.0/PKG-INFO
--rw-r--r--   0 wagner.delima   (502) staff       (20)    19790 2023-04-16 14:33:15.000000 drf-social-oauth2-2.0.0/README.rst
-drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-16 15:47:25.335068 drf-social-oauth2-2.0.0/drf_social_oauth2/
--rw-r--r--   0 wagner.delima   (502) staff       (20)     1379 2023-04-16 14:33:15.000000 drf-social-oauth2-2.0.0/drf_social_oauth2/__init__.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     2599 2022-01-13 22:12:11.000000 drf-social-oauth2-2.0.0/drf_social_oauth2/authentication.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     1253 2023-04-16 14:33:15.000000 drf-social-oauth2-2.0.0/drf_social_oauth2/backends.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     1166 2022-01-06 11:17:42.000000 drf-social-oauth2-2.0.0/drf_social_oauth2/oauth2_backends.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     5432 2022-01-21 09:44:31.000000 drf-social-oauth2-2.0.0/drf_social_oauth2/oauth2_endpoints.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     4630 2020-07-05 09:16:42.000000 drf-social-oauth2-2.0.0/drf_social_oauth2/oauth2_grants.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)      546 2023-04-02 20:09:06.000000 drf-social-oauth2-2.0.0/drf_social_oauth2/serializers.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)      558 2023-03-26 14:38:31.000000 drf-social-oauth2-2.0.0/drf_social_oauth2/settings.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     1766 2022-01-13 22:12:11.000000 drf-social-oauth2-2.0.0/drf_social_oauth2/test_settings.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     2221 2023-04-02 12:11:34.000000 drf-social-oauth2-2.0.0/drf_social_oauth2/urls.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     9117 2023-04-02 20:09:06.000000 drf-social-oauth2-2.0.0/drf_social_oauth2/views.py
-drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-16 15:47:25.339845 drf-social-oauth2-2.0.0/drf_social_oauth2.egg-info/
--rw-r--r--   0 wagner.delima   (502) staff       (20)    20590 2023-04-16 15:47:25.000000 drf-social-oauth2-2.0.0/drf_social_oauth2.egg-info/PKG-INFO
--rw-r--r--   0 wagner.delima   (502) staff       (20)      823 2023-04-16 15:47:25.000000 drf-social-oauth2-2.0.0/drf_social_oauth2.egg-info/SOURCES.txt
--rw-r--r--   0 wagner.delima   (502) staff       (20)        1 2023-04-16 15:47:25.000000 drf-social-oauth2-2.0.0/drf_social_oauth2.egg-info/dependency_links.txt
--rw-r--r--   0 wagner.delima   (502) staff       (20)        1 2023-04-16 14:29:16.000000 drf-social-oauth2-2.0.0/drf_social_oauth2.egg-info/not-zip-safe
--rw-r--r--   0 wagner.delima   (502) staff       (20)      120 2023-04-16 15:47:25.000000 drf-social-oauth2-2.0.0/drf_social_oauth2.egg-info/requires.txt
--rw-r--r--   0 wagner.delima   (502) staff       (20)       24 2023-04-16 15:47:25.000000 drf-social-oauth2-2.0.0/drf_social_oauth2.egg-info/top_level.txt
--rw-r--r--   0 wagner.delima   (502) staff       (20)      274 2023-03-26 14:58:52.000000 drf-social-oauth2-2.0.0/pyproject.toml
--rw-r--r--   0 wagner.delima   (502) staff       (20)       38 2023-04-16 15:47:25.346556 drf-social-oauth2-2.0.0/setup.cfg
--rw-r--r--   0 wagner.delima   (502) staff       (20)     1276 2023-04-02 20:09:06.000000 drf-social-oauth2-2.0.0/setup.py
-drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-16 15:47:25.340586 drf-social-oauth2-2.0.0/tests/
--rw-r--r--   0 wagner.delima   (502) staff       (20)        0 2020-08-30 10:08:43.000000 drf-social-oauth2-2.0.0/tests/__init__.py
-drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-16 15:47:25.342836 drf-social-oauth2-2.0.0/tests/drf_social_oauth2/
--rw-r--r--   0 wagner.delima   (502) staff       (20)        0 2023-04-16 13:51:16.000000 drf-social-oauth2-2.0.0/tests/drf_social_oauth2/__init__.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     2081 2021-12-29 16:09:48.000000 drf-social-oauth2-2.0.0/tests/drf_social_oauth2/test_authentication.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     5577 2023-04-16 14:20:37.000000 drf-social-oauth2-2.0.0/tests/drf_social_oauth2/test_oauth2_endpoints.py
+drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-24 13:22:46.647394 drf-social-oauth2-2.1.0/
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     6286 2023-04-24 13:22:06.000000 drf-social-oauth2-2.1.0/CHANGELOG.rst
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     1080 2020-06-27 18:20:06.000000 drf-social-oauth2-2.1.0/LICENSE.txt
+-rw-r--r--   0 wagner.delima   (502) staff       (20)       81 2020-06-27 18:20:06.000000 drf-social-oauth2-2.1.0/MANIFEST.in
+-rw-r--r--   0 wagner.delima   (502) staff       (20)    20761 2023-04-24 13:22:46.647057 drf-social-oauth2-2.1.0/PKG-INFO
+-rw-r--r--   0 wagner.delima   (502) staff       (20)    19961 2023-04-24 12:27:32.000000 drf-social-oauth2-2.1.0/README.rst
+drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-24 13:22:46.639953 drf-social-oauth2-2.1.0/drf_social_oauth2/
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     1379 2023-04-24 12:27:32.000000 drf-social-oauth2-2.1.0/drf_social_oauth2/__init__.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     2599 2022-01-13 22:12:11.000000 drf-social-oauth2-2.1.0/drf_social_oauth2/authentication.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     1253 2023-04-16 14:33:15.000000 drf-social-oauth2-2.1.0/drf_social_oauth2/backends.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     1166 2022-01-06 11:17:42.000000 drf-social-oauth2-2.1.0/drf_social_oauth2/oauth2_backends.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     5664 2023-04-22 18:56:44.000000 drf-social-oauth2-2.1.0/drf_social_oauth2/oauth2_endpoints.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     4630 2020-07-05 09:16:42.000000 drf-social-oauth2-2.1.0/drf_social_oauth2/oauth2_grants.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)      945 2023-04-22 18:56:44.000000 drf-social-oauth2-2.1.0/drf_social_oauth2/serializers.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)      558 2023-03-26 14:38:31.000000 drf-social-oauth2-2.1.0/drf_social_oauth2/settings.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     2036 2023-04-22 18:56:44.000000 drf-social-oauth2-2.1.0/drf_social_oauth2/test_settings.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     2288 2023-04-22 18:56:44.000000 drf-social-oauth2-2.1.0/drf_social_oauth2/urls.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     9065 2023-04-22 18:56:44.000000 drf-social-oauth2-2.1.0/drf_social_oauth2/views.py
+drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-24 13:22:46.643203 drf-social-oauth2-2.1.0/drf_social_oauth2.egg-info/
+-rw-r--r--   0 wagner.delima   (502) staff       (20)    20761 2023-04-24 13:22:46.000000 drf-social-oauth2-2.1.0/drf_social_oauth2.egg-info/PKG-INFO
+-rw-r--r--   0 wagner.delima   (502) staff       (20)      901 2023-04-24 13:22:46.000000 drf-social-oauth2-2.1.0/drf_social_oauth2.egg-info/SOURCES.txt
+-rw-r--r--   0 wagner.delima   (502) staff       (20)        1 2023-04-24 13:22:46.000000 drf-social-oauth2-2.1.0/drf_social_oauth2.egg-info/dependency_links.txt
+-rw-r--r--   0 wagner.delima   (502) staff       (20)        1 2023-04-24 13:22:46.000000 drf-social-oauth2-2.1.0/drf_social_oauth2.egg-info/not-zip-safe
+-rw-r--r--   0 wagner.delima   (502) staff       (20)      120 2023-04-24 13:22:46.000000 drf-social-oauth2-2.1.0/drf_social_oauth2.egg-info/requires.txt
+-rw-r--r--   0 wagner.delima   (502) staff       (20)       24 2023-04-24 13:22:46.000000 drf-social-oauth2-2.1.0/drf_social_oauth2.egg-info/top_level.txt
+-rw-r--r--   0 wagner.delima   (502) staff       (20)      274 2023-03-26 14:58:52.000000 drf-social-oauth2-2.1.0/pyproject.toml
+-rw-r--r--   0 wagner.delima   (502) staff       (20)       38 2023-04-24 13:22:46.647489 drf-social-oauth2-2.1.0/setup.cfg
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     1276 2023-04-02 20:09:06.000000 drf-social-oauth2-2.1.0/setup.py
+drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-24 13:22:46.643553 drf-social-oauth2-2.1.0/tests/
+-rw-r--r--   0 wagner.delima   (502) staff       (20)        0 2020-08-30 10:08:43.000000 drf-social-oauth2-2.1.0/tests/__init__.py
+drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-04-24 13:22:46.646287 drf-social-oauth2-2.1.0/tests/drf_social_oauth2/
+-rw-r--r--   0 wagner.delima   (502) staff       (20)        0 2023-04-22 11:25:22.000000 drf-social-oauth2-2.1.0/tests/drf_social_oauth2/__init__.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     1560 2023-04-22 18:56:44.000000 drf-social-oauth2-2.1.0/tests/drf_social_oauth2/drf_fixtures.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     2081 2021-12-29 16:09:48.000000 drf-social-oauth2-2.1.0/tests/drf_social_oauth2/test_authentication.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     4268 2023-04-22 18:56:44.000000 drf-social-oauth2-2.1.0/tests/drf_social_oauth2/test_oauth2_endpoints.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     7034 2023-04-22 18:56:44.000000 drf-social-oauth2-2.1.0/tests/drf_social_oauth2/test_views.py
```

### Comparing `drf-social-oauth2-2.0.0/LICENSE.txt` & `drf-social-oauth2-2.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.0.0/PKG-INFO` & `drf-social-oauth2-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-social-oauth2
-Version: 2.0.0
+Version: 2.1.0
 Summary: drf-social-oauth2 is a frameworks meant to be used with Django and Django Rest Framework.
 Home-page: https://github.com/wagnerdelima/drf-social-oauth2
 Author: Wagner de Lima
 Author-email: waglds@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -198,14 +198,18 @@
 
         curl -X POST -d "client_id=<client_id>&client_secret=<client_secret>&token=<your_token>" http://localhost:8000/auth/revoke-token
 
     Revoke all tokens for a user::
 
         curl -H "Authorization: Bearer <token>" -X POST -d "client_id=<client_id>" http://localhost:8000/auth/invalidate-sessions
 
+    Revoke only refresh tokens::
+
+        curl -H "Authorization: Bearer <token>" -X POST -d "client_id=<client_id>" http://localhost:8000/auth/invalidate-refresh-tokens
+
 
 Authenticating Requests
 -----------------------
 
 As you have probably noticed, we enabled a default authentication backend called ``SocialAuthentication``.
 This backend lets you register and authenticate your users seamlessly with your REST API.
```

### Comparing `drf-social-oauth2-2.0.0/README.rst` & `drf-social-oauth2-2.1.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -178,14 +178,18 @@
 
         curl -X POST -d "client_id=<client_id>&client_secret=<client_secret>&token=<your_token>" http://localhost:8000/auth/revoke-token
 
     Revoke all tokens for a user::
 
         curl -H "Authorization: Bearer <token>" -X POST -d "client_id=<client_id>" http://localhost:8000/auth/invalidate-sessions
 
+    Revoke only refresh tokens::
+
+        curl -H "Authorization: Bearer <token>" -X POST -d "client_id=<client_id>" http://localhost:8000/auth/invalidate-refresh-tokens
+
 
 Authenticating Requests
 -----------------------
 
 As you have probably noticed, we enabled a default authentication backend called ``SocialAuthentication``.
 This backend lets you register and authenticate your users seamlessly with your REST API.
```

### Comparing `drf-social-oauth2-2.0.0/drf_social_oauth2/__init__.py` & `drf-social-oauth2-2.1.0/drf_social_oauth2/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 drf-social-oauth2 is a frameworks meant to be used with Django and Django Rest Framework.
 drf-social-oauth2 offers support to oauth2 authentication and authorization.
 It's one of the easiest frameworks to integrate Oauth2 to your Django Rest Framework application.
 By using drf-social-oauth2 you can authenticate with major vendors such as Google, Facebook, Instagram, Github, Twitter
 and a ton more!
 """
 
-__version__ = '2.0.0'
+__version__ = '2.1.0'
 
 try:
     from secrets import SystemRandom
 except ImportError:
     from random import SystemRandom
```

### Comparing `drf-social-oauth2-2.0.0/drf_social_oauth2/authentication.py` & `drf-social-oauth2-2.1.0/drf_social_oauth2/authentication.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.0.0/drf_social_oauth2/backends.py` & `drf-social-oauth2-2.1.0/drf_social_oauth2/backends.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.0.0/drf_social_oauth2/oauth2_backends.py` & `drf-social-oauth2-2.1.0/drf_social_oauth2/oauth2_backends.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.0.0/drf_social_oauth2/oauth2_endpoints.py` & `drf-social-oauth2-2.1.0/drf_social_oauth2/oauth2_endpoints.py`

 * *Files 8% similar despite different names*

```diff
@@ -92,41 +92,46 @@
         )
 
         # validates request and assigns user to request object.
         SocialTokenGrant(self.request_validator).validate_token_request(request)
 
         access_token = self.__check_for_no_existing_tokens(request)
         # Checks if the last token created exists, and if so, if token is still valid.
-        if access_token is None or (access_token and access_token.is_expired()):
+        # also check if an access token has a refresh token associated. Otherwise, create both
+        # access token and refresh token.
+        if (
+            access_token is None
+            or (access_token and access_token.is_expired())
+            or (access_token and not hasattr(access_token, 'refresh_token'))
+        ):
             # create the request again, as a convert_token grant type.
             request = self.__create_django_request(
                 uri, http_method, body, headers, credentials
             )
             return grant_type_handler.create_token_response(
                 request, self.default_token_type
             )
 
         # if token is valid, do not create a new token, just return the token.
         token = {
             'access_token': access_token.token,
-            'expires_in': (
-                access_token.expires - timezone.now()
-            ).total_seconds(),
+            'expires_in': (access_token.expires - timezone.now()).total_seconds(),
             'scope': access_token.scope,
             'refresh_token': access_token.refresh_token.token,
             'token_type': 'Bearer',
         }
         return headers, dumps(token), 200
 
     def __check_for_no_existing_tokens(self, request: Request):
         """
         Checks if the last token created.
         """
         return AccessToken.objects.filter(
-            user=request.user, application=request.client,
+            user=request.user,
+            application=request.client,
         ).last()
 
     def __create_django_request(
         self, uri, http_method='GET', body=None, headers=None, credentials=None
     ):
         """
         Assembles a request and assigns django_request to Request object.
```

### Comparing `drf-social-oauth2-2.0.0/drf_social_oauth2/oauth2_grants.py` & `drf-social-oauth2-2.1.0/drf_social_oauth2/oauth2_grants.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.0.0/drf_social_oauth2/serializers.py` & `drf-social-oauth2-2.1.0/drf_social_oauth2/serializers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,33 @@
 from rest_framework.serializers import Serializer
-from rest_framework.serializers import CharField
+from rest_framework.serializers import CharField, IntegerField
 
 
 class InvalidateRefreshTokenSerializer(Serializer):
     """
     Validate the client_id required and length 100 characters for refresh tokens.
     """
 
     client_id = CharField(max_length=100)
 
 
+class InvalidateSessionsSerializer(Serializer):
+    client_id = CharField(max_length=100)
+
+
 class ConvertTokenSerializer(Serializer):
     grant_type = CharField(max_length=32)
     backend = CharField(max_length=100)
     client_id = CharField(max_length=100)
     client_secret = CharField(max_length=255)
     token = CharField(max_length=500)
+
+
+class RevokeTokenSerializer(Serializer):
+    client_id = CharField(max_length=100)
+    client_secret = CharField(max_length=255)
+    token = CharField(max_length=500)
+
+
+class DisconnectBackendSerializer(Serializer):
+    backend = CharField(max_length=50)
+    association_id = IntegerField()
```

### Comparing `drf-social-oauth2-2.0.0/drf_social_oauth2/settings.py` & `drf-social-oauth2-2.1.0/drf_social_oauth2/settings.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.0.0/drf_social_oauth2/test_settings.py` & `drf-social-oauth2-2.1.0/drf_social_oauth2/test_settings.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 
 BASE_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 
 SECRET_KEY = 'secret_key'
 
 DEBUG = True
 
+ALLOWED_HOSTS = [
+    'testserver',
+]
+
 INSTALLED_APPS = [
     'django.contrib.admin',
     'django.contrib.auth',
     'django.contrib.contenttypes',
     'django.contrib.sessions',
     'django.contrib.messages',
     'django.contrib.staticfiles',
@@ -51,14 +55,25 @@
         'HOST': 'db',
         'PORT': 5432,
         'USER': 'user',
         'PASSWORD': 'password',
     }
 }
 
+TEST_LOCAL_DATABASES = {
+    'default': {
+        'ENGINE': 'django.db.backends.postgresql',
+        'NAME': 'db',
+        'HOST': '127.0.0.1',
+        'PORT': 3333,
+        'USER': 'postgres',
+        'PASSWORD': '0119',
+    }
+}
+
 
 DRFSO2_PROPRIETARY_BACKEND_NAME = 'Django'
 
 DRFSO2_URL_NAMESPACE = 'drf'
 
 ROOT_URLCONF = 'drf_social_oauth2.urls'
```

### Comparing `drf-social-oauth2-2.0.0/drf_social_oauth2/urls.py` & `drf-social-oauth2-2.1.0/drf_social_oauth2/urls.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from oauth2_provider.views import AuthorizationView
 from social_django.views import complete
 
 from drf_social_oauth2.views import (
     ConvertTokenView,
     TokenView,
     RevokeTokenView,
-    invalidate_sessions,
+    InvalidateSessions,
     DisconnectBackendView,
     InvalidateRefreshTokens,
 )
 
 app_name = 'drfso2'
 
 
@@ -27,15 +27,17 @@
     urlpatterns += [
         url(r'^authorize/?$', AuthorizationView.as_view(), name='authorize'),
         url(r'^token/?$', TokenView.as_view(), name='token'),
         url('', include('social_django.urls', namespace='social')),
         url(r'^convert-token/?$', ConvertTokenView.as_view(), name='convert_token'),
         url(r'^revoke-token/?$', RevokeTokenView.as_view(), name='revoke_token'),
         url(
-            r'^invalidate-sessions/?$', invalidate_sessions, name='invalidate_sessions'
+            r'^invalidate-sessions/?$',
+            InvalidateSessions.as_view(),
+            name='invalidate_sessions',
         ),
         url(
             r'invalidate-refresh-tokens/?$',
             InvalidateRefreshTokens.as_view(),
             name='invalidate_refresh_tokens',
         ),
         url(
@@ -48,15 +50,17 @@
     urlpatterns += [
         re_path(r'^authorize/?$', AuthorizationView.as_view(), name='authorize'),
         re_path(r'^token/?$', TokenView.as_view(), name='token'),
         re_path('', include('social_django.urls', namespace='social')),
         re_path(r'^convert-token/?$', ConvertTokenView.as_view(), name='convert_token'),
         re_path(r'^revoke-token/?$', RevokeTokenView.as_view(), name='revoke_token'),
         re_path(
-            r'^invalidate-sessions/?$', invalidate_sessions, name='invalidate_sessions'
+            r'^invalidate-sessions/?$',
+            InvalidateSessions.as_view(),
+            name='invalidate_sessions',
         ),
         re_path(
             r'invalidate-refresh-tokens/?$',
             InvalidateRefreshTokens.as_view(),
             name='invalidate_refresh_tokens',
         ),
         re_path(
```

### Comparing `drf-social-oauth2-2.0.0/drf_social_oauth2/views.py` & `drf-social-oauth2-2.1.0/drf_social_oauth2/views.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,38 +3,38 @@
 from django.urls import reverse
 from django.utils.decorators import method_decorator
 from django.views.decorators.csrf import csrf_exempt
 
 from social_core.exceptions import MissingBackend
 from social_django.utils import load_strategy, load_backend
 
-from oauth2_provider.contrib.rest_framework import OAuth2Authentication
 from oauth2_provider.models import Application, AccessToken, RefreshToken
 from oauth2_provider.settings import oauth2_settings
 from oauth2_provider.views.mixins import OAuthLibMixin
 from oauthlib.oauth2.rfc6749.errors import (
     InvalidClientError,
     UnsupportedGrantTypeError,
     AccessDeniedError,
     MissingClientIdError,
     InvalidRequestError,
 )
 
 from rest_framework.permissions import AllowAny, IsAuthenticated
 from rest_framework.status import HTTP_204_NO_CONTENT, HTTP_400_BAD_REQUEST
-from rest_framework.decorators import (
-    api_view,
-    authentication_classes,
-    permission_classes,
-)
 from rest_framework.response import Response
 from rest_framework.request import Request
 from rest_framework.views import APIView
 
-from drf_social_oauth2.serializers import InvalidateRefreshTokenSerializer
+from drf_social_oauth2.serializers import (
+    InvalidateRefreshTokenSerializer,
+    ConvertTokenSerializer,
+    RevokeTokenSerializer,
+    DisconnectBackendSerializer,
+    InvalidateSessionsSerializer,
+)
 from drf_social_oauth2.oauth2_backends import KeepRequestCore
 from drf_social_oauth2.oauth2_endpoints import SocialTokenServer
 
 
 class CsrfExemptMixin:
     """
     Exempts the view from CSRF requirements.
@@ -98,18 +98,19 @@
 
     server_class = SocialTokenServer
     validator_class = oauth2_settings.OAUTH2_VALIDATOR_CLASS
     oauthlib_backend_class = KeepRequestCore
     permission_classes = (AllowAny,)
 
     def post(self, request: Request, *args, **kwargs):
+        serializer = ConvertTokenSerializer(data=request.data)
+        serializer.is_valid(raise_exception=True)
         # Use the rest framework `.data` to fake the post body of the django request.
-        mutable_data = request.data.copy()
         request._request.POST = request._request.POST.copy()
-        for key, value in mutable_data.items():
+        for key, value in serializer.validated_data.items():
             request._request.POST[key] = value
 
         try:
             url, headers, body, status = self.create_token_response(request._request)
         except InvalidClientError:
             return Response(
                 data={'invalid_client': 'Missing client type.'},
@@ -150,57 +151,58 @@
 
     server_class = oauth2_settings.OAUTH2_SERVER_CLASS
     validator_class = oauth2_settings.OAUTH2_VALIDATOR_CLASS
     oauthlib_backend_class = oauth2_settings.OAUTH2_BACKEND_CLASS
     permission_classes = (AllowAny,)
 
     def post(self, request: Request, *args, **kwargs):
+        serializer = RevokeTokenSerializer(data=request.data)
+        serializer.is_valid(raise_exception=True)
         # Use the rest framework `.data` to fake the post body of the django request.
-        mutable_data = request.data.copy()
         request._request.POST = request._request.POST.copy()
-        for key, value in mutable_data.items():
+        for key, value in serializer.validated_data.items():
             request._request.POST[key] = value
 
         url, headers, body, status = self.create_revocation_response(request._request)
         response = Response(
             data=json_loads(body) if body else '', status=status if body else 204
         )
 
         for k, v in headers.items():
             response[k] = v
         return response
 
 
-@api_view(['POST'])
-@authentication_classes([OAuth2Authentication])
-@permission_classes([IsAuthenticated])
-def invalidate_sessions(request):
+class InvalidateSessions(APIView):
     """
     Delete all access tokens associated with a client id.
     """
 
-    client_id = request.data.get("client_id", None)
-    if client_id is None:
-        return Response(
-            {"client_id": ["This field is required."]},
-            status=HTTP_400_BAD_REQUEST,
-        )
+    permission_classes = (IsAuthenticated,)
 
-    try:
-        app = Application.objects.get(client_id=client_id)
-        AccessToken.objects.filter(user=request.user, application=app).delete()
-    except Application.DoesNotExist:
-        return Response(
-            {
-                "detail": "The application linked to the provided client_id could not be found."
-            },
-            status=HTTP_400_BAD_REQUEST,
-        )
+    def get_object(self):
+        return self.request.user
 
-    return Response({}, status=HTTP_204_NO_CONTENT)
+    def post(self, request: Request, *args, **kwargs):
+        serializer = InvalidateSessionsSerializer(data=request.data)
+        serializer.is_valid(raise_exception=True)
+        client_id = serializer.validated_data['client_id']
+
+        try:
+            app = Application.objects.get(client_id=client_id)
+            AccessToken.objects.filter(user=self.get_object(), application=app).delete()
+        except Application.DoesNotExist:
+            return Response(
+                {
+                    "detail": "The application linked to the provided client_id could not be found."
+                },
+                status=HTTP_400_BAD_REQUEST,
+            )
+
+        return Response({}, status=HTTP_204_NO_CONTENT)
 
 
 class InvalidateRefreshTokens(APIView):
     """
     Invalidate all refresh tokens associated with a client id.
     """
 
@@ -236,28 +238,19 @@
 
     permission_classes = (IsAuthenticated,)
 
     def get_object(self):
         return self.request.user
 
     def post(self, request: Request, *args, **kwargs):
-        backend = request.data.get("backend", None)
-        if backend is None:
-            return Response(
-                {"backend": ["This field is required."]},
-                status=HTTP_400_BAD_REQUEST,
-            )
-
-        association_id = request.data.get("association_id", None)
-        if association_id is None:
-            return Response(
-                {"association_id": ["This field is required."]},
-                status=HTTP_400_BAD_REQUEST,
-            )
+        serializer = DisconnectBackendSerializer(data=request.data)
+        serializer.is_valid(raise_exception=True)
 
+        backend = serializer.validated_data['backend']
+        association_id = serializer.validated_data['association_id']
         strategy = load_strategy(request=request)
         try:
             namespace = 'drf'
             backend = load_backend(
                 strategy, backend, reverse(namespace + ":complete", args=(backend,))
             )
         except MissingBackend:
```

### Comparing `drf-social-oauth2-2.0.0/drf_social_oauth2.egg-info/PKG-INFO` & `drf-social-oauth2-2.1.0/drf_social_oauth2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-social-oauth2
-Version: 2.0.0
+Version: 2.1.0
 Summary: drf-social-oauth2 is a frameworks meant to be used with Django and Django Rest Framework.
 Home-page: https://github.com/wagnerdelima/drf-social-oauth2
 Author: Wagner de Lima
 Author-email: waglds@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -198,14 +198,18 @@
 
         curl -X POST -d "client_id=<client_id>&client_secret=<client_secret>&token=<your_token>" http://localhost:8000/auth/revoke-token
 
     Revoke all tokens for a user::
 
         curl -H "Authorization: Bearer <token>" -X POST -d "client_id=<client_id>" http://localhost:8000/auth/invalidate-sessions
 
+    Revoke only refresh tokens::
+
+        curl -H "Authorization: Bearer <token>" -X POST -d "client_id=<client_id>" http://localhost:8000/auth/invalidate-refresh-tokens
+
 
 Authenticating Requests
 -----------------------
 
 As you have probably noticed, we enabled a default authentication backend called ``SocialAuthentication``.
 This backend lets you register and authenticate your users seamlessly with your REST API.
```

### Comparing `drf-social-oauth2-2.0.0/setup.py` & `drf-social-oauth2-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.0.0/tests/drf_social_oauth2/test_authentication.py` & `drf-social-oauth2-2.1.0/tests/drf_social_oauth2/test_authentication.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.0.0/tests/drf_social_oauth2/test_oauth2_endpoints.py` & `drf-social-oauth2-2.1.0/tests/drf_social_oauth2/test_oauth2_endpoints.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,80 +5,25 @@
 os.environ.setdefault('DJANGO_SETTINGS_MODULE', 'drf_social_oauth2.test_settings')
 
 from django import setup
 
 setup()
 
 from django.contrib.auth.models import User
-from django.db import IntegrityError
 
 from oauth2_provider.models import Application, AccessToken, RefreshToken
-from pytest import fixture
 
 from drf_social_oauth2.oauth2_endpoints import SocialTokenServer
 from drf_social_oauth2 import generate_token
-
-
-@fixture(scope='function')
-def user():
-    """
-    Creates a user in database. this is a mock user, it's deletes after test runs.
-    """
-    try:
-        user = User.objects.create_user(
-            username='user', email='test@email.com', password='password'
-        )
-    except IntegrityError:
-        user = User.objects.get(
-            username='user',
-            email='test@email.com',
-        )
-
-    yield user
-    del user
-
-
-@fixture(scope='function')
-def application(user):
-    app, _ = Application.objects.get_or_create(
-        user=user,
-        client_type='confidential',
-        authorization_grant_type='Resource owner password-based',
-        name='app',
-    )
-
-    yield app
-    del app
-
-
-def save(token, request):
-    u = User.objects.get(email='test@email.com')
-    app = Application.objects.get(user=u.id)
-    re_token = RefreshToken.objects.create(
-        user=u,
-        token=token['refresh_token'],
-        application=app,
-    )
-    ac_token = AccessToken.objects.create(
-        user=u,
-        token=token['access_token'],
-        scope=token['scope'],
-        application=app,
-        source_refresh_token=re_token,
-        expires=datetime.now(tz=timezone.utc) + timedelta(seconds=token['expires_in']),
-    )
-    re_token.access_token = ac_token
-    re_token.save()
-
-    return ac_token
+from tests.drf_social_oauth2.drf_fixtures import application, user, save
 
 
 def assign_request_application(request):
-    u = User.objects.get(email='test@email.com')
-    app = Application.objects.get(user=u.id)
+    user = User.objects.get(email='test@email.com')
+    app = Application.objects.get(user=user.id)
     request.client = app
 
 
 def test_create_social_token(mocker, user, application):
     """
     Creates a social token.
     """
```

