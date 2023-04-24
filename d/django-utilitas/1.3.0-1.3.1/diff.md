# Comparing `tmp/django-utilitas-1.3.0.tar.gz` & `tmp/django-utilitas-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-utilitas-1.3.0.tar", last modified: Sat Apr 22 06:45:48 2023, max compression
+gzip compressed data, was "django-utilitas-1.3.1.tar", last modified: Mon Apr 24 03:51:35 2023, max compression
```

## Comparing `django-utilitas-1.3.0.tar` & `django-utilitas-1.3.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 jamesthiha   (501) staff       (20)        0 2023-04-22 06:45:48.511867 django-utilitas-1.3.0/
--rw-r--r--   0 jamesthiha   (501) staff       (20)    35149 2022-12-05 07:45:37.000000 django-utilitas-1.3.0/LICENSE
--rw-r--r--   0 jamesthiha   (501) staff       (20)     4209 2023-04-22 06:45:48.512078 django-utilitas-1.3.0/PKG-INFO
--rw-r--r--   0 jamesthiha   (501) staff       (20)     3964 2023-04-22 06:44:50.000000 django-utilitas-1.3.0/README.md
-drwxr-xr-x   0 jamesthiha   (501) staff       (20)        0 2023-04-22 06:45:48.497208 django-utilitas-1.3.0/django_utilitas.egg-info/
--rw-r--r--   0 jamesthiha   (501) staff       (20)     4209 2023-04-22 06:45:48.000000 django-utilitas-1.3.0/django_utilitas.egg-info/PKG-INFO
--rw-r--r--   0 jamesthiha   (501) staff       (20)      642 2023-04-22 06:45:48.000000 django-utilitas-1.3.0/django_utilitas.egg-info/SOURCES.txt
--rw-r--r--   0 jamesthiha   (501) staff       (20)        1 2023-04-22 06:45:48.000000 django-utilitas-1.3.0/django_utilitas.egg-info/dependency_links.txt
--rw-r--r--   0 jamesthiha   (501) staff       (20)       80 2023-04-22 06:45:48.000000 django-utilitas-1.3.0/django_utilitas.egg-info/requires.txt
--rw-r--r--   0 jamesthiha   (501) staff       (20)        9 2023-04-22 06:45:48.000000 django-utilitas-1.3.0/django_utilitas.egg-info/top_level.txt
--rw-r--r--   0 jamesthiha   (501) staff       (20)      428 2023-04-22 06:45:48.513785 django-utilitas-1.3.0/setup.cfg
--rw-r--r--   0 jamesthiha   (501) staff       (20)      263 2022-12-05 08:04:03.000000 django-utilitas-1.3.0/setup.py
-drwxr-xr-x   0 jamesthiha   (501) staff       (20)        0 2023-04-22 06:45:48.510914 django-utilitas-1.3.0/utilitas/
--rw-r--r--   0 jamesthiha   (501) staff       (20)        0 2022-11-28 18:11:49.000000 django-utilitas-1.3.0/utilitas/__init__.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)       63 2022-11-28 18:11:49.000000 django-utilitas-1.3.0/utilitas/admin.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)      148 2022-11-28 18:11:50.000000 django-utilitas-1.3.0/utilitas/apps.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)      349 2022-12-05 07:27:09.000000 django-utilitas-1.3.0/utilitas/exception_handler.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)        0 2022-11-28 19:38:13.000000 django-utilitas-1.3.0/utilitas/exceptions.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)       76 2022-12-05 07:26:41.000000 django-utilitas-1.3.0/utilitas/managers.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)      778 2022-12-05 03:43:29.000000 django-utilitas-1.3.0/utilitas/metadata.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)      591 2023-01-25 15:05:12.000000 django-utilitas-1.3.0/utilitas/middlewares.py
-drwxr-xr-x   0 jamesthiha   (501) staff       (20)        0 2023-04-22 06:45:48.511430 django-utilitas-1.3.0/utilitas/migrations/
--rw-r--r--   0 jamesthiha   (501) staff       (20)        0 2022-11-28 18:11:49.000000 django-utilitas-1.3.0/utilitas/migrations/__init__.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)     1454 2022-12-05 07:25:03.000000 django-utilitas-1.3.0/utilitas/models.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)     1031 2023-02-22 06:50:16.000000 django-utilitas-1.3.0/utilitas/pagination.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)      366 2022-11-28 19:43:27.000000 django-utilitas-1.3.0/utilitas/renderer.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)     1450 2023-02-19 23:16:44.000000 django-utilitas-1.3.0/utilitas/serializers.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)      945 2022-12-05 08:14:19.000000 django-utilitas-1.3.0/utilitas/swagger_query_params.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)      347 2022-11-28 19:35:23.000000 django-utilitas-1.3.0/utilitas/swagger_serializers.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)       60 2022-11-28 18:11:49.000000 django-utilitas-1.3.0/utilitas/tests.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)       18 2022-11-28 18:28:32.000000 django-utilitas-1.3.0/utilitas/urls.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)    13433 2023-04-22 06:43:45.000000 django-utilitas-1.3.0/utilitas/views.py
+drwxr-xr-x   0 jamesthiha   (501) staff       (20)        0 2023-04-24 03:51:35.144939 django-utilitas-1.3.1/
+-rw-r--r--   0 jamesthiha   (501) staff       (20)    35149 2022-12-05 07:45:37.000000 django-utilitas-1.3.1/LICENSE
+-rw-r--r--   0 jamesthiha   (501) staff       (20)     4426 2023-04-24 03:51:35.145161 django-utilitas-1.3.1/PKG-INFO
+-rw-r--r--   0 jamesthiha   (501) staff       (20)     4181 2023-04-24 03:50:47.000000 django-utilitas-1.3.1/README.md
+drwxr-xr-x   0 jamesthiha   (501) staff       (20)        0 2023-04-24 03:51:35.131005 django-utilitas-1.3.1/django_utilitas.egg-info/
+-rw-r--r--   0 jamesthiha   (501) staff       (20)     4426 2023-04-24 03:51:35.000000 django-utilitas-1.3.1/django_utilitas.egg-info/PKG-INFO
+-rw-r--r--   0 jamesthiha   (501) staff       (20)      642 2023-04-24 03:51:35.000000 django-utilitas-1.3.1/django_utilitas.egg-info/SOURCES.txt
+-rw-r--r--   0 jamesthiha   (501) staff       (20)        1 2023-04-24 03:51:35.000000 django-utilitas-1.3.1/django_utilitas.egg-info/dependency_links.txt
+-rw-r--r--   0 jamesthiha   (501) staff       (20)       80 2023-04-24 03:51:35.000000 django-utilitas-1.3.1/django_utilitas.egg-info/requires.txt
+-rw-r--r--   0 jamesthiha   (501) staff       (20)        9 2023-04-24 03:51:35.000000 django-utilitas-1.3.1/django_utilitas.egg-info/top_level.txt
+-rw-r--r--   0 jamesthiha   (501) staff       (20)      428 2023-04-24 03:51:35.145887 django-utilitas-1.3.1/setup.cfg
+-rw-r--r--   0 jamesthiha   (501) staff       (20)      263 2022-12-05 08:04:03.000000 django-utilitas-1.3.1/setup.py
+drwxr-xr-x   0 jamesthiha   (501) staff       (20)        0 2023-04-24 03:51:35.143907 django-utilitas-1.3.1/utilitas/
+-rw-r--r--   0 jamesthiha   (501) staff       (20)        0 2022-11-28 18:11:49.000000 django-utilitas-1.3.1/utilitas/__init__.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)       63 2022-11-28 18:11:49.000000 django-utilitas-1.3.1/utilitas/admin.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)      148 2022-11-28 18:11:50.000000 django-utilitas-1.3.1/utilitas/apps.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)      349 2022-12-05 07:27:09.000000 django-utilitas-1.3.1/utilitas/exception_handler.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)        0 2022-11-28 19:38:13.000000 django-utilitas-1.3.1/utilitas/exceptions.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)       76 2022-12-05 07:26:41.000000 django-utilitas-1.3.1/utilitas/managers.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)      778 2022-12-05 03:43:29.000000 django-utilitas-1.3.1/utilitas/metadata.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)      591 2023-01-25 15:05:12.000000 django-utilitas-1.3.1/utilitas/middlewares.py
+drwxr-xr-x   0 jamesthiha   (501) staff       (20)        0 2023-04-24 03:51:35.144526 django-utilitas-1.3.1/utilitas/migrations/
+-rw-r--r--   0 jamesthiha   (501) staff       (20)        0 2022-11-28 18:11:49.000000 django-utilitas-1.3.1/utilitas/migrations/__init__.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)     1454 2022-12-05 07:25:03.000000 django-utilitas-1.3.1/utilitas/models.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)     1031 2023-02-22 06:50:16.000000 django-utilitas-1.3.1/utilitas/pagination.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)      366 2022-11-28 19:43:27.000000 django-utilitas-1.3.1/utilitas/renderer.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)     1450 2023-02-19 23:16:44.000000 django-utilitas-1.3.1/utilitas/serializers.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)      945 2022-12-05 08:14:19.000000 django-utilitas-1.3.1/utilitas/swagger_query_params.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)      347 2022-11-28 19:35:23.000000 django-utilitas-1.3.1/utilitas/swagger_serializers.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)       60 2022-11-28 18:11:49.000000 django-utilitas-1.3.1/utilitas/tests.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)       18 2022-11-28 18:28:32.000000 django-utilitas-1.3.1/utilitas/urls.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)    14571 2023-04-24 03:49:19.000000 django-utilitas-1.3.1/utilitas/views.py
```

### Comparing `django-utilitas-1.3.0/LICENSE` & `django-utilitas-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-utilitas-1.3.0/PKG-INFO` & `django-utilitas-1.3.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: django-utilitas
-Version: 1.3.0
-Summary: Django package with useful utility classes
-Home-page: https://github.com/ninnroot/utilitas
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Django Utilitas
 Django Utilitas is a library that contains many ready-to-use utility classes so that you can just focus on the business logic of your API.
 
 Utilitas itself is built upon many other great Django packages such as drf-ff, drf-yasg and the Django REST Framework itself.
 
 
 ## Feature summary
@@ -101,16 +92,20 @@
 class BookSerializer(BaseModelSerializer):
     class Meta:
         model = Book
         fields = "__all__"
         list_serializer_class = BaseListSerializer
 ```
 
+For more information about django-utilitas, please read the architecture document [here](./architecture.md)
+
 ## Changelog
 
+- 1.3.1
+    - now, the API won't return 500 if missing foreign keys are provided in the `expand` parameter.
 - 1.3.0
     - removed the need for `related_fields` parameter. Prefetching related fields is now done automatically using the `expand` parameter provided by the client.
 - 1.2.9
     - renamed file from `migrations.py` to `middlewares.py` (my stupid mistake in the first place)
 - 1.2.8
     - bug fixes
 - 1.2.7
```

### Comparing `django-utilitas-1.3.0/README.md` & `django-utilitas-1.3.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: django-utilitas
+Version: 1.3.1
+Summary: Django package with useful utility classes
+Home-page: https://github.com/ninnroot/utilitas
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Django Utilitas
 Django Utilitas is a library that contains many ready-to-use utility classes so that you can just focus on the business logic of your API.
 
 Utilitas itself is built upon many other great Django packages such as drf-ff, drf-yasg and the Django REST Framework itself.
 
 
 ## Feature summary
@@ -92,16 +101,20 @@
 class BookSerializer(BaseModelSerializer):
     class Meta:
         model = Book
         fields = "__all__"
         list_serializer_class = BaseListSerializer
 ```
 
+For more information about django-utilitas, please read the architecture document [here](./architecture.md)
+
 ## Changelog
 
+- 1.3.1
+    - now, the API won't return 500 if missing foreign keys are provided in the `expand` parameter.
 - 1.3.0
     - removed the need for `related_fields` parameter. Prefetching related fields is now done automatically using the `expand` parameter provided by the client.
 - 1.2.9
     - renamed file from `migrations.py` to `middlewares.py` (my stupid mistake in the first place)
 - 1.2.8
     - bug fixes
 - 1.2.7
```

### Comparing `django-utilitas-1.3.0/django_utilitas.egg-info/PKG-INFO` & `django-utilitas-1.3.1/django_utilitas.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-utilitas
-Version: 1.3.0
+Version: 1.3.1
 Summary: Django package with useful utility classes
 Home-page: https://github.com/ninnroot/utilitas
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django Utilitas
@@ -101,16 +101,20 @@
 class BookSerializer(BaseModelSerializer):
     class Meta:
         model = Book
         fields = "__all__"
         list_serializer_class = BaseListSerializer
 ```
 
+For more information about django-utilitas, please read the architecture document [here](./architecture.md)
+
 ## Changelog
 
+- 1.3.1
+    - now, the API won't return 500 if missing foreign keys are provided in the `expand` parameter.
 - 1.3.0
     - removed the need for `related_fields` parameter. Prefetching related fields is now done automatically using the `expand` parameter provided by the client.
 - 1.2.9
     - renamed file from `migrations.py` to `middlewares.py` (my stupid mistake in the first place)
 - 1.2.8
     - bug fixes
 - 1.2.7
```

### Comparing `django-utilitas-1.3.0/django_utilitas.egg-info/SOURCES.txt` & `django-utilitas-1.3.1/django_utilitas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-utilitas-1.3.0/utilitas/metadata.py` & `django-utilitas-1.3.1/utilitas/metadata.py`

 * *Files identical despite different names*

### Comparing `django-utilitas-1.3.0/utilitas/middlewares.py` & `django-utilitas-1.3.1/utilitas/middlewares.py`

 * *Files identical despite different names*

### Comparing `django-utilitas-1.3.0/utilitas/models.py` & `django-utilitas-1.3.1/utilitas/models.py`

 * *Files identical despite different names*

### Comparing `django-utilitas-1.3.0/utilitas/pagination.py` & `django-utilitas-1.3.1/utilitas/pagination.py`

 * *Files identical despite different names*

### Comparing `django-utilitas-1.3.0/utilitas/serializers.py` & `django-utilitas-1.3.1/utilitas/serializers.py`

 * *Files identical despite different names*

### Comparing `django-utilitas-1.3.0/utilitas/swagger_query_params.py` & `django-utilitas-1.3.1/utilitas/swagger_query_params.py`

 * *Files identical despite different names*

### Comparing `django-utilitas-1.3.0/utilitas/views.py` & `django-utilitas-1.3.1/utilitas/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,32 @@
 from utilitas.serializers import FilterParamSerializer
 from utilitas.swagger_serializers import FilterParamsSerializer
 from utilitas.swagger_query_params import *
 
 from utilitas.models import BaseModel
 from utilitas.serializers import BaseSerializer, BaseModelSerializer
 
+from django.db.models.base import ModelBase
+
+def get_prefetchable_fields(instance):
+    opts = instance._meta
+    ret = []
+    for field in opts.get_fields():
+        if not isinstance(instance, ModelBase):
+            rel_obj_descriptor = getattr(instance.__class__, field.name, None)
+        else:
+            rel_obj_descriptor = getattr(instance, field.name, None)
+        if rel_obj_descriptor:
+            if hasattr(rel_obj_descriptor, 'get_prefetch_queryset'):
+                ret.append(field.name)
+            else:
+                rel_obj = getattr(instance, field.name)
+                if hasattr(rel_obj, 'get_prefetch_queryset'):
+                    ret.append(field.name)
+    return ret
 
 class BaseView(APIView, CustomPagination):
     name: str = "Base view (not cringe view)"
     description: str = ""
 
     authentication_classes = []
     permission_classes = []
@@ -31,14 +49,22 @@
     # query_params' names
     fields_param = "fields"
     sorts_param = "sorts"
     expand_param = "expand"
     # customizing the response format
     renderer_classes = [CustomRenderer, BrowsableAPIRenderer]
 
+    # Some `expand` parameters cannot be present in the model's foreign keys (client's mistakes). 
+    # To avoid being a chatty API, we will just quietly ignore thier mistakes.
+    def _translate_expand_params(self, expand):
+        translated_expand = []
+        # Replacing dots with Django ORM's format.
+        for i in expand:
+            translated_expand.append(i.replace(".", "__"))
+        return set(translated_expand).intersection(set(get_prefetchable_fields(self.model)))
 
     @classmethod
     def _validate_attributes(cls, **kwargs):
         for i in [{"var": "model", "parent_class": BaseModel},
                   {"var": "serializer", "parent_class": (BaseSerializer, BaseModelSerializer)}]:
 
             # making sure certain class variables are implemented.
@@ -87,17 +113,15 @@
         if fields is None:
             fields = []
 
         if expand is None:
             expand = []
         # query from the database
 
-        translated_expand = []
-        for i in expand:
-            translated_expand.append(i.replace(".", "__"))
+        translated_expand = self._translate_expand_params(expand)
 
         queryset = (
             self.model.objects.filter(**filter_params).exclude(**exclude_params)
             .prefetch_related(*translated_expand)
             .all()
             .order_by(*sorts)
         )
```

