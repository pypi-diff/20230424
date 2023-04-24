# Comparing `tmp/django-rest-serializer-field-permissions-4.0.0rc2.tar.gz` & `tmp/django-rest-serializer-field-permissions-4.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\django-rest-serializer-field-permissions-4.0.0rc2.tar", last modified: Mon Feb 15 19:07:48 2021, max compression
+gzip compressed data, was "django-rest-serializer-field-permissions-4.1.0rc1.tar", last modified: Mon Apr 24 17:54:31 2023, max compression
```

## Comparing `django-rest-serializer-field-permissions-4.0.0rc2.tar` & `django-rest-serializer-field-permissions-4.1.0rc1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2021-02-15 19:07:48.000000 django-rest-serializer-field-permissions-4.0.0rc2/
-drwxrwxrwx   0        0        0        0 2021-02-15 19:07:48.000000 django-rest-serializer-field-permissions-4.0.0rc2/django_rest_serializer_field_permissions.egg-info/
--rw-rw-rw-   0        0        0        1 2021-02-15 19:07:47.000000 django-rest-serializer-field-permissions-4.0.0rc2/django_rest_serializer_field_permissions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     9641 2021-02-15 19:07:47.000000 django-rest-serializer-field-permissions-4.0.0rc2/django_rest_serializer_field_permissions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       37 2021-02-15 19:07:47.000000 django-rest-serializer-field-permissions-4.0.0rc2/django_rest_serializer_field_permissions.egg-info/requires.txt
--rw-rw-rw-   0        0        0      585 2021-02-15 19:07:48.000000 django-rest-serializer-field-permissions-4.0.0rc2/django_rest_serializer_field_permissions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       44 2021-02-15 19:07:47.000000 django-rest-serializer-field-permissions-4.0.0rc2/django_rest_serializer_field_permissions.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35797 2020-01-01 00:07:01.000000 django-rest-serializer-field-permissions-4.0.0rc2/LICENSE
--rw-rw-rw-   0        0        0       34 2020-01-01 00:07:01.000000 django-rest-serializer-field-permissions-4.0.0rc2/MANIFEST.in
--rw-rw-rw-   0        0        0     9641 2021-02-15 19:07:48.000000 django-rest-serializer-field-permissions-4.0.0rc2/PKG-INFO
--rw-rw-rw-   0        0        0     7342 2021-01-11 01:36:29.000000 django-rest-serializer-field-permissions-4.0.0rc2/README.md
-drwxrwxrwx   0        0        0        0 2021-02-15 19:07:48.000000 django-rest-serializer-field-permissions-4.0.0rc2/rest_framework_serializer_field_permissions/
--rw-rw-rw-   0        0        0     5225 2021-02-15 17:53:41.000000 django-rest-serializer-field-permissions-4.0.0rc2/rest_framework_serializer_field_permissions/fields.py
--rw-rw-rw-   0        0        0     1491 2020-01-01 00:07:01.000000 django-rest-serializer-field-permissions-4.0.0rc2/rest_framework_serializer_field_permissions/permissions.py
--rw-rw-rw-   0        0        0     1323 2021-01-11 01:36:29.000000 django-rest-serializer-field-permissions-4.0.0rc2/rest_framework_serializer_field_permissions/serializers.py
--rw-rw-rw-   0        0        0       83 2020-01-01 00:07:01.000000 django-rest-serializer-field-permissions-4.0.0rc2/rest_framework_serializer_field_permissions/__init__.py
--rw-rw-rw-   0        0        0       42 2021-02-15 19:07:48.000000 django-rest-serializer-field-permissions-4.0.0rc2/setup.cfg
--rw-rw-rw-   0        0        0     1397 2021-02-15 19:07:15.000000 django-rest-serializer-field-permissions-4.0.0rc2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 17:54:31.079532 django-rest-serializer-field-permissions-4.1.0rc1/
+-rw-rw-rw-   0        0        0    35797 2020-01-01 00:07:01.000000 django-rest-serializer-field-permissions-4.1.0rc1/LICENSE
+-rw-rw-rw-   0        0        0       34 2020-01-01 00:07:01.000000 django-rest-serializer-field-permissions-4.1.0rc1/MANIFEST.in
+-rw-rw-rw-   0        0        0     8393 2023-04-24 17:54:31.078387 django-rest-serializer-field-permissions-4.1.0rc1/PKG-INFO
+-rw-rw-rw-   0        0        0     7475 2023-04-24 17:33:33.000000 django-rest-serializer-field-permissions-4.1.0rc1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 17:54:31.072173 django-rest-serializer-field-permissions-4.1.0rc1/django_rest_serializer_field_permissions.egg-info/
+-rw-rw-rw-   0        0        0     8393 2023-04-24 17:54:31.000000 django-rest-serializer-field-permissions-4.1.0rc1/django_rest_serializer_field_permissions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      585 2023-04-24 17:54:31.000000 django-rest-serializer-field-permissions-4.1.0rc1/django_rest_serializer_field_permissions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 17:54:31.000000 django-rest-serializer-field-permissions-4.1.0rc1/django_rest_serializer_field_permissions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-04-24 17:54:31.000000 django-rest-serializer-field-permissions-4.1.0rc1/django_rest_serializer_field_permissions.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       44 2023-04-24 17:54:31.000000 django-rest-serializer-field-permissions-4.1.0rc1/django_rest_serializer_field_permissions.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 17:54:31.077388 django-rest-serializer-field-permissions-4.1.0rc1/rest_framework_serializer_field_permissions/
+-rw-rw-rw-   0        0        0       83 2020-01-01 00:07:01.000000 django-rest-serializer-field-permissions-4.1.0rc1/rest_framework_serializer_field_permissions/__init__.py
+-rw-rw-rw-   0        0        0     5277 2023-04-24 17:49:15.000000 django-rest-serializer-field-permissions-4.1.0rc1/rest_framework_serializer_field_permissions/fields.py
+-rw-rw-rw-   0        0        0     1491 2020-01-01 00:07:01.000000 django-rest-serializer-field-permissions-4.1.0rc1/rest_framework_serializer_field_permissions/permissions.py
+-rw-rw-rw-   0        0        0     1323 2021-01-11 01:36:29.000000 django-rest-serializer-field-permissions-4.1.0rc1/rest_framework_serializer_field_permissions/serializers.py
+-rw-rw-rw-   0        0        0       42 2023-04-24 17:54:31.079532 django-rest-serializer-field-permissions-4.1.0rc1/setup.cfg
+-rw-rw-rw-   0        0        0     1498 2023-04-24 17:54:24.000000 django-rest-serializer-field-permissions-4.1.0rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-rest-serializer-field-permissions-4.0.0rc2/django_rest_serializer_field_permissions.egg-info/PKG-INFO` & `django-rest-serializer-field-permissions-4.1.0rc1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,197 +1,196 @@
 Metadata-Version: 2.1
 Name: django-rest-serializer-field-permissions
-Version: 4.0.0rc2
+Version: 4.1.0rc1
 Summary: Field-by-field serializer permissions for Django Rest Framework.
 Home-page: https://github.com/InterSIS/django-rest-serializer-field-permissions/
 Author: The Intersis Foundation
 Author-email: dev@intersis.org
 License: GNU General Public License v3 (GPLv3)
-Description: [![Build Status](https://travis-ci.org/InterSIS/django-rest-serializer-field-permissions.svg?branch=master)](https://travis-ci.org/InterSIS/django-rest-serializer-field-permissions)
-        [![Code Climate](https://codeclimate.com/github/InterSIS/django-rest-serializer-field-permissions/badges/gpa.svg)](https://codeclimate.com/github/InterSIS/django-rest-serializer-field-permissions)
-        [![Coverage Status](https://coveralls.io/repos/InterSIS/django-rest-serializer-field-permissions/badge.svg?branch=master&service=github)](https://coveralls.io/github/InterSIS/django-rest-serializer-field-permissions?branch=master)
-        [![PyPI version](https://badge.fury.io/py/django-rest-serializer-field-permissions.svg)](http://badge.fury.io/py/django-rest-serializer-field-permissions)
-        
-        django-rest-serializer-field-permissions
-        =============
-        
-        Add field-by-field permission classes to your serializer fields that look like this:
-        
-        ```python
-          class PersonSerializer(FieldPermissionSerializerMixin, LookupModelSerializer):
-        
-              # Only allow authenticated users to retrieve family and given names
-              family_names = serializers.CharField(permission_classes=(IsAuthenticated(), ))
-              given_names = serializers.CharField(permission_classes=(IsAuthenticated(), ))
-              
-              # Allow all users to retrieve nick name
-              nick_name = serializers.CharField(permission_classes=(AllowAll(), ))
-        
-        ```
-        
-        Complete Tutorial
-        ----------------
-        
-        This example builds on the example Django REST Framework API in the [DRF 3.9 documentation](https://github.com/encode/django-rest-framework/tree/3.9.x#example). Please make sure that you have completed that tutorial before beginning this one.
-        
-        Install this module into your environment:
-        
-        ```
-          $ pip install django-rest-serializer-field-permissions~=3.0
-        ```
-        
-        Install this module into Django by adding it to your `INSTALLED_APPS`.
-        ```python
-          INSTALLED_APPS = (
-          # ...
-              'rest_framework_serializer_field_permissions',
-          # ...
-          )
-        ```
-        
-        
-        Now you can add retrieve permissions to individual fields. You must import the modules and classes shown below, mix `FieldPermissionSerializerMixin` as the **leftmost** parent to your serializers, and then define your fields using the provided drop-in field classes.
-        
-        For example, modify the root `urls.py` you created in the DRF tutorial with the following code:
-        
-        ```python
-        from django.conf.urls import url, include
-        from django.contrib.auth.models import User
-        from rest_framework import routers, serializers, viewsets
-        
-        from rest_framework_serializer_field_permissions import fields                                      # <--
-        from rest_framework_serializer_field_permissions.serializers import FieldPermissionSerializerMixin  # <--
-        from rest_framework_serializer_field_permissions.permissions import IsAuthenticated                 # <--
-        
-        # Serializers define the API representation.
-        class UserSerializer(FieldPermissionSerializerMixin, serializers.HyperlinkedModelSerializer):       # <--
-            class Meta:
-                model = User
-                fields = ('url', 'username', 'email', 'is_staff')
-        
-            email = fields.EmailField(permission_classes=(IsAuthenticated(), ))                             # <--
-        
-        # ViewSets define the view behavior.
-        class UserViewSet(viewsets.ModelViewSet):
-            queryset = User.objects.all()
-            serializer_class = UserSerializer
-        
-        # Routers provide an easy way of automatically determining the URL conf.
-        router = routers.DefaultRouter()
-        router.register(r'users', UserViewSet)
-        
-        # Wire up our API using automatic URL routing.
-        # Additionally, we include login URLs for the browsable API.
-        urlpatterns = [
-            url(r'^', include(router.urls)),
-            url(r'^api-auth/', include('rest_framework.urls', namespace='rest_framework'))
-        ]
-        
-        ```
-        
-        Now, only authenticated users will be able to retrieve your users' emails. You can confirm this by creating a superuser account, if you haven't already, and visiting [http://localhost:8000/users/](http://localhost:8000/users) as both an authenticated user and an unauthenticated visitor.
-        
-        Alternately, you could have restricted retrieve access to the `username` field with the code:
-        
-        ```python
-            username = fields.CharField(permission_classes=(IsAuthenticated(), ))
-        ```
-        
-        You can define your own permissions classes that operate on any aspect of the incoming `request`, and you can specify multiple r`permission_classes` on a field: all provided permissions must be satisfied for the visitor to retrieve the given field.
-        
-        Use
-        ---
-        
-        ### Installation
-        
-        Install the module in your Python distribution or virtualenv:
-        
-            $ pip install django-rest-serializer-field-permissions
-        
-        Add the application to your `INSTALLED_APPS`:
-        
-        ```python
-          INSTALLED_APPS = (
-          ...
-          'rest_framework_serializer_field_permissions',
-          ...
-          )
-        ```
-        
-        ### Adding Permissions
-        
-        In your serializers, mix `FieldPermissionSerializerMixin` into your serializer classes, as the left-most parent. The fields
-        provided by `rest_framework_serializer_field_permissions.fields` accept `permission_classes` which operate in typical
-        DRF fashion:
-        
-        ```python
-          from rest_framework import serializers
-          
-          from rest_framework_serializer_field_permissions import fields
-          from rest_framework_serializer_field_permissions.serializers import FieldPermissionSerializerMixin
-          from rest_framework_serializer_field_permissions.permissions import IsAuthenticated
-        
-          class UserSerializer(FieldPermissionSerializerMixin, serializers.HyperlinkedModelSerializer):
-            class Meta:
-                model = User
-                fields = ('url', 'username', 'email', 'is_staff')
-        
-            email = fields.EmailField(permission_classes=(IsAuthenticated(), ))
-        
-        ```
-        
-        The `FieldPermissionSerializerMixin` may be mixed with any DRF serializer class, not just `ModelSerializer`.
-        
-        You can write your own permission classes by sub-classing `BaseFieldPermission` in `permissions.py`.
-        
-        How it Works
-        ------------
-        
-        The `FieldPermissionSerializerMixin` provides its own `fields` property, which DRF serializers call to get a list
-        of their own fields. The amended `fields` property checks for permission-bearing fields, forces them to check their
-        permissions against the request, and scrubs from the return any fields which fail their permission checks.
-        
-        Compatibility
-        -------------
-        
-        This package is tested for compatibility against the following software versions:
-        
-        * Django Rest Framework 3.11
-        * Django 2.2, 3.0
-        * Python 3.7
-        
-        This package may incidentally be compatible with other similar versions of the above software. See tox.ini for specific minor versions tested.
-        
-        Additional Requirements
-        -----------------------
-        
-        None
-        
-        Todo
-        ----
-        
-        * Integration tests
-        
-        Getting Involved
-        ----------------
-        
-        Feel free to open pull requests or issues. [GitHub](https://github.com/InterSIS/django-rest-serializer-field-permissions) is the canonical location of this project.
-        
-        Here's the general sequence of events for contribution:
-        
-        1. Open an issue in the [issue tracker](https://github.com/InterSIS/django-rest-serializer-field-permissions/issues/).
-        2. In any order:
-          * Submit a pull request with a **failing** test that demonstrates the issue/feature.
-          * Get acknowledgement/concurrence.
-        3. Submit pull request that passes your test in (2). Include documentation, if appropriate.
-        
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+[![Code Climate](https://codeclimate.com/github/InterSIS/django-rest-serializer-field-permissions/badges/gpa.svg)](https://codeclimate.com/github/InterSIS/django-rest-serializer-field-permissions)
+[![Coverage Status](https://coveralls.io/repos/InterSIS/django-rest-serializer-field-permissions/badge.svg?branch=master&service=github)](https://coveralls.io/github/InterSIS/django-rest-serializer-field-permissions?branch=master)
+[![PyPI version](https://badge.fury.io/py/django-rest-serializer-field-permissions.svg)](http://badge.fury.io/py/django-rest-serializer-field-permissions)
+
+django-rest-serializer-field-permissions
+=============
+
+Add field-by-field permission classes to your serializer fields that look like this:
+
+```python
+  class PersonSerializer(FieldPermissionSerializerMixin, LookupModelSerializer):
+
+      # Only allow authenticated users to retrieve family and given names
+      family_names = serializers.CharField(permission_classes=(IsAuthenticated(), ))
+      given_names = serializers.CharField(permission_classes=(IsAuthenticated(), ))
+      
+      # Allow all users to retrieve nick name
+      nick_name = serializers.CharField(permission_classes=(AllowAll(), ))
+
+```
+
+Getting Involved, New Features, Etc.
+------------------------------------
+
+This project is in *maintenance mode*. I can offer the following support/upgrades:
+  * Ongoing compatibility with DRF version 3.
+  * Ongoing compatibility with Django version 3.
+  * If future major versions of Django and DRF are roughly compatible with this plugin, then I hope to offer ongoing support for those as well.
+  * Adding new fields to the library's drop-in replacements as Django adds new fields.
+
+Several people have offered really great ideas for how to improve this library. Unfortunately, I don't use this library regularly myself and it takes me a day or two to spin myself back up on it to the point where I can safely and responsibly consider the impacts of proposed changes. And at this time, I'm unable to fulfill that responsibility.
+
+If you have a change/issue that falls under one of the bullet points above, please feel free to raise it in the issue tracker!
+
+Complete Tutorial
+----------------
+
+This example builds on the example Django REST Framework API in the [DRF 3.9 documentation](https://github.com/encode/django-rest-framework/tree/3.9.x#example). Please make sure that you have completed that tutorial before beginning this one.
+
+Install this module into your environment:
+
+```
+  $ pip install django-rest-serializer-field-permissions~=3.0
+```
+
+Install this module into Django by adding it to your `INSTALLED_APPS`.
+```python
+  INSTALLED_APPS = (
+  # ...
+      'rest_framework_serializer_field_permissions',
+  # ...
+  )
+```
+
+
+Now you can add retrieve permissions to individual fields. You must import the modules and classes shown below, mix `FieldPermissionSerializerMixin` as the **leftmost** parent to your serializers, and then define your fields using the provided drop-in field classes.
+
+For example, modify the root `urls.py` you created in the DRF tutorial with the following code:
+
+```python
+from django.conf.urls import url, include
+from django.contrib.auth.models import User
+from rest_framework import routers, serializers, viewsets
+
+from rest_framework_serializer_field_permissions import fields                                      # <--
+from rest_framework_serializer_field_permissions.serializers import FieldPermissionSerializerMixin  # <--
+from rest_framework_serializer_field_permissions.permissions import IsAuthenticated                 # <--
+
+# Serializers define the API representation.
+class UserSerializer(FieldPermissionSerializerMixin, serializers.HyperlinkedModelSerializer):       # <--
+    class Meta:
+        model = User
+        fields = ('url', 'username', 'email', 'is_staff')
+
+    email = fields.EmailField(permission_classes=(IsAuthenticated(), ))                             # <--
+
+# ViewSets define the view behavior.
+class UserViewSet(viewsets.ModelViewSet):
+    queryset = User.objects.all()
+    serializer_class = UserSerializer
+
+# Routers provide an easy way of automatically determining the URL conf.
+router = routers.DefaultRouter()
+router.register(r'users', UserViewSet)
+
+# Wire up our API using automatic URL routing.
+# Additionally, we include login URLs for the browsable API.
+urlpatterns = [
+    url(r'^', include(router.urls)),
+    url(r'^api-auth/', include('rest_framework.urls', namespace='rest_framework'))
+]
+
+```
+
+Now, only authenticated users will be able to retrieve your users' emails. You can confirm this by creating a superuser account, if you haven't already, and visiting [http://localhost:8000/users/](http://localhost:8000/users) as both an authenticated user and an unauthenticated visitor.
+
+Alternately, you could have restricted retrieve access to the `username` field with the code:
+
+```python
+    username = fields.CharField(permission_classes=(IsAuthenticated(), ))
+```
+
+You can define your own permissions classes that operate on any aspect of the incoming `request`, and you can specify multiple r`permission_classes` on a field: all provided permissions must be satisfied for the visitor to retrieve the given field.
+
+Use
+---
+
+### Installation
+
+Install the module in your Python distribution or virtualenv:
+
+    $ pip install django-rest-serializer-field-permissions
+
+Add the application to your `INSTALLED_APPS`:
+
+```python
+  INSTALLED_APPS = (
+  ...
+  'rest_framework_serializer_field_permissions',
+  ...
+  )
+```
+
+### Adding Permissions
+
+In your serializers, mix `FieldPermissionSerializerMixin` into your serializer classes, as the left-most parent. The fields
+provided by `rest_framework_serializer_field_permissions.fields` accept `permission_classes` which operate in typical
+DRF fashion:
+
+```python
+  from rest_framework import serializers
+  
+  from rest_framework_serializer_field_permissions import fields
+  from rest_framework_serializer_field_permissions.serializers import FieldPermissionSerializerMixin
+  from rest_framework_serializer_field_permissions.permissions import IsAuthenticated
+
+  class UserSerializer(FieldPermissionSerializerMixin, serializers.HyperlinkedModelSerializer):
+    class Meta:
+        model = User
+        fields = ('url', 'username', 'email', 'is_staff')
+
+    email = fields.EmailField(permission_classes=(IsAuthenticated(), ))
+
+```
+
+The `FieldPermissionSerializerMixin` may be mixed with any DRF serializer class, not just `ModelSerializer`.
+
+You can write your own permission classes by sub-classing `BaseFieldPermission` in `permissions.py`.
+
+How it Works
+------------
+
+The `FieldPermissionSerializerMixin` provides its own `fields` property, which DRF serializers call to get a list
+of their own fields. The amended `fields` property checks for permission-bearing fields, forces them to check their
+permissions against the request, and scrubs from the return any fields which fail their permission checks.
+
+Compatibility
+-------------
+
+This package is tested for compatibility against the following software versions:
+
+* Django Rest Framework 3.14.0
+* Django 3.2, 4.2
+* Python 3.7
+
+This package may incidentally be compatible with other similar versions of the above software. See tox.ini for specific minor versions tested.
+
+Additional Requirements
+-----------------------
+
+None
+
+
+
```

### Comparing `django-rest-serializer-field-permissions-4.0.0rc2/django_rest_serializer_field_permissions.egg-info/SOURCES.txt` & `django-rest-serializer-field-permissions-4.1.0rc1/django_rest_serializer_field_permissions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-rest-serializer-field-permissions-4.0.0rc2/LICENSE` & `django-rest-serializer-field-permissions-4.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-rest-serializer-field-permissions-4.0.0rc2/PKG-INFO` & `django-rest-serializer-field-permissions-4.1.0rc1/django_rest_serializer_field_permissions.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,197 +1,196 @@
 Metadata-Version: 2.1
 Name: django-rest-serializer-field-permissions
-Version: 4.0.0rc2
+Version: 4.1.0rc1
 Summary: Field-by-field serializer permissions for Django Rest Framework.
 Home-page: https://github.com/InterSIS/django-rest-serializer-field-permissions/
 Author: The Intersis Foundation
 Author-email: dev@intersis.org
 License: GNU General Public License v3 (GPLv3)
-Description: [![Build Status](https://travis-ci.org/InterSIS/django-rest-serializer-field-permissions.svg?branch=master)](https://travis-ci.org/InterSIS/django-rest-serializer-field-permissions)
-        [![Code Climate](https://codeclimate.com/github/InterSIS/django-rest-serializer-field-permissions/badges/gpa.svg)](https://codeclimate.com/github/InterSIS/django-rest-serializer-field-permissions)
-        [![Coverage Status](https://coveralls.io/repos/InterSIS/django-rest-serializer-field-permissions/badge.svg?branch=master&service=github)](https://coveralls.io/github/InterSIS/django-rest-serializer-field-permissions?branch=master)
-        [![PyPI version](https://badge.fury.io/py/django-rest-serializer-field-permissions.svg)](http://badge.fury.io/py/django-rest-serializer-field-permissions)
-        
-        django-rest-serializer-field-permissions
-        =============
-        
-        Add field-by-field permission classes to your serializer fields that look like this:
-        
-        ```python
-          class PersonSerializer(FieldPermissionSerializerMixin, LookupModelSerializer):
-        
-              # Only allow authenticated users to retrieve family and given names
-              family_names = serializers.CharField(permission_classes=(IsAuthenticated(), ))
-              given_names = serializers.CharField(permission_classes=(IsAuthenticated(), ))
-              
-              # Allow all users to retrieve nick name
-              nick_name = serializers.CharField(permission_classes=(AllowAll(), ))
-        
-        ```
-        
-        Complete Tutorial
-        ----------------
-        
-        This example builds on the example Django REST Framework API in the [DRF 3.9 documentation](https://github.com/encode/django-rest-framework/tree/3.9.x#example). Please make sure that you have completed that tutorial before beginning this one.
-        
-        Install this module into your environment:
-        
-        ```
-          $ pip install django-rest-serializer-field-permissions~=3.0
-        ```
-        
-        Install this module into Django by adding it to your `INSTALLED_APPS`.
-        ```python
-          INSTALLED_APPS = (
-          # ...
-              'rest_framework_serializer_field_permissions',
-          # ...
-          )
-        ```
-        
-        
-        Now you can add retrieve permissions to individual fields. You must import the modules and classes shown below, mix `FieldPermissionSerializerMixin` as the **leftmost** parent to your serializers, and then define your fields using the provided drop-in field classes.
-        
-        For example, modify the root `urls.py` you created in the DRF tutorial with the following code:
-        
-        ```python
-        from django.conf.urls import url, include
-        from django.contrib.auth.models import User
-        from rest_framework import routers, serializers, viewsets
-        
-        from rest_framework_serializer_field_permissions import fields                                      # <--
-        from rest_framework_serializer_field_permissions.serializers import FieldPermissionSerializerMixin  # <--
-        from rest_framework_serializer_field_permissions.permissions import IsAuthenticated                 # <--
-        
-        # Serializers define the API representation.
-        class UserSerializer(FieldPermissionSerializerMixin, serializers.HyperlinkedModelSerializer):       # <--
-            class Meta:
-                model = User
-                fields = ('url', 'username', 'email', 'is_staff')
-        
-            email = fields.EmailField(permission_classes=(IsAuthenticated(), ))                             # <--
-        
-        # ViewSets define the view behavior.
-        class UserViewSet(viewsets.ModelViewSet):
-            queryset = User.objects.all()
-            serializer_class = UserSerializer
-        
-        # Routers provide an easy way of automatically determining the URL conf.
-        router = routers.DefaultRouter()
-        router.register(r'users', UserViewSet)
-        
-        # Wire up our API using automatic URL routing.
-        # Additionally, we include login URLs for the browsable API.
-        urlpatterns = [
-            url(r'^', include(router.urls)),
-            url(r'^api-auth/', include('rest_framework.urls', namespace='rest_framework'))
-        ]
-        
-        ```
-        
-        Now, only authenticated users will be able to retrieve your users' emails. You can confirm this by creating a superuser account, if you haven't already, and visiting [http://localhost:8000/users/](http://localhost:8000/users) as both an authenticated user and an unauthenticated visitor.
-        
-        Alternately, you could have restricted retrieve access to the `username` field with the code:
-        
-        ```python
-            username = fields.CharField(permission_classes=(IsAuthenticated(), ))
-        ```
-        
-        You can define your own permissions classes that operate on any aspect of the incoming `request`, and you can specify multiple r`permission_classes` on a field: all provided permissions must be satisfied for the visitor to retrieve the given field.
-        
-        Use
-        ---
-        
-        ### Installation
-        
-        Install the module in your Python distribution or virtualenv:
-        
-            $ pip install django-rest-serializer-field-permissions
-        
-        Add the application to your `INSTALLED_APPS`:
-        
-        ```python
-          INSTALLED_APPS = (
-          ...
-          'rest_framework_serializer_field_permissions',
-          ...
-          )
-        ```
-        
-        ### Adding Permissions
-        
-        In your serializers, mix `FieldPermissionSerializerMixin` into your serializer classes, as the left-most parent. The fields
-        provided by `rest_framework_serializer_field_permissions.fields` accept `permission_classes` which operate in typical
-        DRF fashion:
-        
-        ```python
-          from rest_framework import serializers
-          
-          from rest_framework_serializer_field_permissions import fields
-          from rest_framework_serializer_field_permissions.serializers import FieldPermissionSerializerMixin
-          from rest_framework_serializer_field_permissions.permissions import IsAuthenticated
-        
-          class UserSerializer(FieldPermissionSerializerMixin, serializers.HyperlinkedModelSerializer):
-            class Meta:
-                model = User
-                fields = ('url', 'username', 'email', 'is_staff')
-        
-            email = fields.EmailField(permission_classes=(IsAuthenticated(), ))
-        
-        ```
-        
-        The `FieldPermissionSerializerMixin` may be mixed with any DRF serializer class, not just `ModelSerializer`.
-        
-        You can write your own permission classes by sub-classing `BaseFieldPermission` in `permissions.py`.
-        
-        How it Works
-        ------------
-        
-        The `FieldPermissionSerializerMixin` provides its own `fields` property, which DRF serializers call to get a list
-        of their own fields. The amended `fields` property checks for permission-bearing fields, forces them to check their
-        permissions against the request, and scrubs from the return any fields which fail their permission checks.
-        
-        Compatibility
-        -------------
-        
-        This package is tested for compatibility against the following software versions:
-        
-        * Django Rest Framework 3.11
-        * Django 2.2, 3.0
-        * Python 3.7
-        
-        This package may incidentally be compatible with other similar versions of the above software. See tox.ini for specific minor versions tested.
-        
-        Additional Requirements
-        -----------------------
-        
-        None
-        
-        Todo
-        ----
-        
-        * Integration tests
-        
-        Getting Involved
-        ----------------
-        
-        Feel free to open pull requests or issues. [GitHub](https://github.com/InterSIS/django-rest-serializer-field-permissions) is the canonical location of this project.
-        
-        Here's the general sequence of events for contribution:
-        
-        1. Open an issue in the [issue tracker](https://github.com/InterSIS/django-rest-serializer-field-permissions/issues/).
-        2. In any order:
-          * Submit a pull request with a **failing** test that demonstrates the issue/feature.
-          * Get acknowledgement/concurrence.
-        3. Submit pull request that passes your test in (2). Include documentation, if appropriate.
-        
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+[![Code Climate](https://codeclimate.com/github/InterSIS/django-rest-serializer-field-permissions/badges/gpa.svg)](https://codeclimate.com/github/InterSIS/django-rest-serializer-field-permissions)
+[![Coverage Status](https://coveralls.io/repos/InterSIS/django-rest-serializer-field-permissions/badge.svg?branch=master&service=github)](https://coveralls.io/github/InterSIS/django-rest-serializer-field-permissions?branch=master)
+[![PyPI version](https://badge.fury.io/py/django-rest-serializer-field-permissions.svg)](http://badge.fury.io/py/django-rest-serializer-field-permissions)
+
+django-rest-serializer-field-permissions
+=============
+
+Add field-by-field permission classes to your serializer fields that look like this:
+
+```python
+  class PersonSerializer(FieldPermissionSerializerMixin, LookupModelSerializer):
+
+      # Only allow authenticated users to retrieve family and given names
+      family_names = serializers.CharField(permission_classes=(IsAuthenticated(), ))
+      given_names = serializers.CharField(permission_classes=(IsAuthenticated(), ))
+      
+      # Allow all users to retrieve nick name
+      nick_name = serializers.CharField(permission_classes=(AllowAll(), ))
+
+```
+
+Getting Involved, New Features, Etc.
+------------------------------------
+
+This project is in *maintenance mode*. I can offer the following support/upgrades:
+  * Ongoing compatibility with DRF version 3.
+  * Ongoing compatibility with Django version 3.
+  * If future major versions of Django and DRF are roughly compatible with this plugin, then I hope to offer ongoing support for those as well.
+  * Adding new fields to the library's drop-in replacements as Django adds new fields.
+
+Several people have offered really great ideas for how to improve this library. Unfortunately, I don't use this library regularly myself and it takes me a day or two to spin myself back up on it to the point where I can safely and responsibly consider the impacts of proposed changes. And at this time, I'm unable to fulfill that responsibility.
+
+If you have a change/issue that falls under one of the bullet points above, please feel free to raise it in the issue tracker!
+
+Complete Tutorial
+----------------
+
+This example builds on the example Django REST Framework API in the [DRF 3.9 documentation](https://github.com/encode/django-rest-framework/tree/3.9.x#example). Please make sure that you have completed that tutorial before beginning this one.
+
+Install this module into your environment:
+
+```
+  $ pip install django-rest-serializer-field-permissions~=3.0
+```
+
+Install this module into Django by adding it to your `INSTALLED_APPS`.
+```python
+  INSTALLED_APPS = (
+  # ...
+      'rest_framework_serializer_field_permissions',
+  # ...
+  )
+```
+
+
+Now you can add retrieve permissions to individual fields. You must import the modules and classes shown below, mix `FieldPermissionSerializerMixin` as the **leftmost** parent to your serializers, and then define your fields using the provided drop-in field classes.
+
+For example, modify the root `urls.py` you created in the DRF tutorial with the following code:
+
+```python
+from django.conf.urls import url, include
+from django.contrib.auth.models import User
+from rest_framework import routers, serializers, viewsets
+
+from rest_framework_serializer_field_permissions import fields                                      # <--
+from rest_framework_serializer_field_permissions.serializers import FieldPermissionSerializerMixin  # <--
+from rest_framework_serializer_field_permissions.permissions import IsAuthenticated                 # <--
+
+# Serializers define the API representation.
+class UserSerializer(FieldPermissionSerializerMixin, serializers.HyperlinkedModelSerializer):       # <--
+    class Meta:
+        model = User
+        fields = ('url', 'username', 'email', 'is_staff')
+
+    email = fields.EmailField(permission_classes=(IsAuthenticated(), ))                             # <--
+
+# ViewSets define the view behavior.
+class UserViewSet(viewsets.ModelViewSet):
+    queryset = User.objects.all()
+    serializer_class = UserSerializer
+
+# Routers provide an easy way of automatically determining the URL conf.
+router = routers.DefaultRouter()
+router.register(r'users', UserViewSet)
+
+# Wire up our API using automatic URL routing.
+# Additionally, we include login URLs for the browsable API.
+urlpatterns = [
+    url(r'^', include(router.urls)),
+    url(r'^api-auth/', include('rest_framework.urls', namespace='rest_framework'))
+]
+
+```
+
+Now, only authenticated users will be able to retrieve your users' emails. You can confirm this by creating a superuser account, if you haven't already, and visiting [http://localhost:8000/users/](http://localhost:8000/users) as both an authenticated user and an unauthenticated visitor.
+
+Alternately, you could have restricted retrieve access to the `username` field with the code:
+
+```python
+    username = fields.CharField(permission_classes=(IsAuthenticated(), ))
+```
+
+You can define your own permissions classes that operate on any aspect of the incoming `request`, and you can specify multiple r`permission_classes` on a field: all provided permissions must be satisfied for the visitor to retrieve the given field.
+
+Use
+---
+
+### Installation
+
+Install the module in your Python distribution or virtualenv:
+
+    $ pip install django-rest-serializer-field-permissions
+
+Add the application to your `INSTALLED_APPS`:
+
+```python
+  INSTALLED_APPS = (
+  ...
+  'rest_framework_serializer_field_permissions',
+  ...
+  )
+```
+
+### Adding Permissions
+
+In your serializers, mix `FieldPermissionSerializerMixin` into your serializer classes, as the left-most parent. The fields
+provided by `rest_framework_serializer_field_permissions.fields` accept `permission_classes` which operate in typical
+DRF fashion:
+
+```python
+  from rest_framework import serializers
+  
+  from rest_framework_serializer_field_permissions import fields
+  from rest_framework_serializer_field_permissions.serializers import FieldPermissionSerializerMixin
+  from rest_framework_serializer_field_permissions.permissions import IsAuthenticated
+
+  class UserSerializer(FieldPermissionSerializerMixin, serializers.HyperlinkedModelSerializer):
+    class Meta:
+        model = User
+        fields = ('url', 'username', 'email', 'is_staff')
+
+    email = fields.EmailField(permission_classes=(IsAuthenticated(), ))
+
+```
+
+The `FieldPermissionSerializerMixin` may be mixed with any DRF serializer class, not just `ModelSerializer`.
+
+You can write your own permission classes by sub-classing `BaseFieldPermission` in `permissions.py`.
+
+How it Works
+------------
+
+The `FieldPermissionSerializerMixin` provides its own `fields` property, which DRF serializers call to get a list
+of their own fields. The amended `fields` property checks for permission-bearing fields, forces them to check their
+permissions against the request, and scrubs from the return any fields which fail their permission checks.
+
+Compatibility
+-------------
+
+This package is tested for compatibility against the following software versions:
+
+* Django Rest Framework 3.14.0
+* Django 3.2, 4.2
+* Python 3.7
+
+This package may incidentally be compatible with other similar versions of the above software. See tox.ini for specific minor versions tested.
+
+Additional Requirements
+-----------------------
+
+None
+
+
+
```

### Comparing `django-rest-serializer-field-permissions-4.0.0rc2/README.md` & `django-rest-serializer-field-permissions-4.1.0rc1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-[![Build Status](https://travis-ci.org/InterSIS/django-rest-serializer-field-permissions.svg?branch=master)](https://travis-ci.org/InterSIS/django-rest-serializer-field-permissions)
 [![Code Climate](https://codeclimate.com/github/InterSIS/django-rest-serializer-field-permissions/badges/gpa.svg)](https://codeclimate.com/github/InterSIS/django-rest-serializer-field-permissions)
 [![Coverage Status](https://coveralls.io/repos/InterSIS/django-rest-serializer-field-permissions/badge.svg?branch=master&service=github)](https://coveralls.io/github/InterSIS/django-rest-serializer-field-permissions?branch=master)
 [![PyPI version](https://badge.fury.io/py/django-rest-serializer-field-permissions.svg)](http://badge.fury.io/py/django-rest-serializer-field-permissions)
 
 django-rest-serializer-field-permissions
 =============
 
@@ -16,14 +15,27 @@
       given_names = serializers.CharField(permission_classes=(IsAuthenticated(), ))
       
       # Allow all users to retrieve nick name
       nick_name = serializers.CharField(permission_classes=(AllowAll(), ))
 
 ```
 
+Getting Involved, New Features, Etc.
+------------------------------------
+
+This project is in *maintenance mode*. I can offer the following support/upgrades:
+  * Ongoing compatibility with DRF version 3.
+  * Ongoing compatibility with Django version 3.
+  * If future major versions of Django and DRF are roughly compatible with this plugin, then I hope to offer ongoing support for those as well.
+  * Adding new fields to the library's drop-in replacements as Django adds new fields.
+
+Several people have offered really great ideas for how to improve this library. Unfortunately, I don't use this library regularly myself and it takes me a day or two to spin myself back up on it to the point where I can safely and responsibly consider the impacts of proposed changes. And at this time, I'm unable to fulfill that responsibility.
+
+If you have a change/issue that falls under one of the bullet points above, please feel free to raise it in the issue tracker!
+
 Complete Tutorial
 ----------------
 
 This example builds on the example Django REST Framework API in the [DRF 3.9 documentation](https://github.com/encode/django-rest-framework/tree/3.9.x#example). Please make sure that you have completed that tutorial before beginning this one.
 
 Install this module into your environment:
 
@@ -143,35 +155,18 @@
 permissions against the request, and scrubs from the return any fields which fail their permission checks.
 
 Compatibility
 -------------
 
 This package is tested for compatibility against the following software versions:
 
-* Django Rest Framework 3.11
-* Django 2.2, 3.0
+* Django Rest Framework 3.14.0
+* Django 3.2, 4.2
 * Python 3.7
 
 This package may incidentally be compatible with other similar versions of the above software. See tox.ini for specific minor versions tested.
 
 Additional Requirements
 -----------------------
 
 None
 
-Todo
-----
-
-* Integration tests
-
-Getting Involved
-----------------
-
-Feel free to open pull requests or issues. [GitHub](https://github.com/InterSIS/django-rest-serializer-field-permissions) is the canonical location of this project.
-
-Here's the general sequence of events for contribution:
-
-1. Open an issue in the [issue tracker](https://github.com/InterSIS/django-rest-serializer-field-permissions/issues/).
-2. In any order:
-  * Submit a pull request with a **failing** test that demonstrates the issue/feature.
-  * Get acknowledgement/concurrence.
-3. Submit pull request that passes your test in (2). Include documentation, if appropriate.
```

### Comparing `django-rest-serializer-field-permissions-4.0.0rc2/rest_framework_serializer_field_permissions/fields.py` & `django-rest-serializer-field-permissions-4.1.0rc1/rest_framework_serializer_field_permissions/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,16 +72,19 @@
 
 
 # pylint: disable=missing-docstring
 class BooleanField(PermissionMixin, fields.BooleanField):
     pass
 
 
-# pylint: disable=missing-docstring
-class NullBooleanField(PermissionMixin, fields.NullBooleanField):
+try:
+    # pylint: disable=missing-docstring
+    class NullBooleanField(PermissionMixin, fields.NullBooleanField):
+        pass
+except AttributeError:
     pass
 
 
 # pylint: disable=missing-docstring
 class CharField(PermissionMixin, fields.CharField):
     pass
```

### Comparing `django-rest-serializer-field-permissions-4.0.0rc2/rest_framework_serializer_field_permissions/permissions.py` & `django-rest-serializer-field-permissions-4.1.0rc1/rest_framework_serializer_field_permissions/permissions.py`

 * *Files identical despite different names*

### Comparing `django-rest-serializer-field-permissions-4.0.0rc2/rest_framework_serializer_field_permissions/serializers.py` & `django-rest-serializer-field-permissions-4.1.0rc1/rest_framework_serializer_field_permissions/serializers.py`

 * *Files identical despite different names*

### Comparing `django-rest-serializer-field-permissions-4.0.0rc2/setup.py` & `django-rest-serializer-field-permissions-4.1.0rc1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,28 +5,34 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-rest-serializer-field-permissions',
-    version='4.0.0rc2',
+    version='4.1.0rc1',
     packages=['rest_framework_serializer_field_permissions'],
     include_package_data=True,
     license='GNU General Public License v3 (GPLv3)',
     description='Field-by-field serializer permissions for Django Rest Framework.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/InterSIS/django-rest-serializer-field-permissions/',
     author='The Intersis Foundation',
     author_email='dev@intersis.org',
     install_requires=[
-        'django>=2.1',
+        'django>=3.0',
         'djangorestframework~=3.0',
     ],
+    extras_require={
+        'dev': [
+            'tox',
+            'twine',
+        ]
+    },
     classifiers=[
         'Environment :: Web Environment',
         'Framework :: Django',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
```

