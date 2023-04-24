# Comparing `tmp/neapolitan-23.7.tar.gz` & `tmp/neapolitan-23.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neapolitan-23.7.tar", last modified: Wed Apr 12 10:09:11 2023, max compression
+gzip compressed data, was "neapolitan-23.8.tar", last modified: Mon Apr 24 09:55:40 2023, max compression
```

## Comparing `neapolitan-23.7.tar` & `neapolitan-23.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0       59 2023-04-08 15:53:57.994299 neapolitan-23.7/.gitignore
--rw-r--r--   0        0        0     1081 2023-04-08 09:37:37.437304 neapolitan-23.7/LICENSE
--rw-r--r--   0        0        0     1128 2023-04-11 13:44:05.034404 neapolitan-23.7/Notes.txt
--rw-r--r--   0        0        0     1621 2023-04-10 13:12:58.659109 neapolitan-23.7/README.rst
--rw-r--r--   0        0        0      638 2023-04-08 10:32:21.337055 neapolitan-23.7/docs/Makefile
--rw-r--r--   0        0        0      804 2023-04-08 10:32:21.337901 neapolitan-23.7/docs/make.bat
--rw-r--r--   0        0        0      943 2023-04-08 13:11:08.113103 neapolitan-23.7/docs/source/conf.py
--rw-r--r--   0        0        0      160 2023-04-11 14:07:29.272376 neapolitan-23.7/docs/source/crud-view.rst
--rw-r--r--   0        0        0     1232 2023-04-12 10:05:03.102830 neapolitan-23.7/docs/source/index.rst
--rw-r--r--   0        0        0      562 2023-04-12 10:04:35.742277 neapolitan-23.7/docs/source/templates.rst
--rw-r--r--   0        0        0      213 2023-04-08 15:52:45.220880 neapolitan-23.7/justfile
--rw-r--r--   0        0        0      653 2023-04-10 09:35:41.106347 neapolitan-23.7/pyproject.toml
--rw-r--r--   0        0        0      978 2023-04-12 10:08:36.880467 neapolitan-23.7/src/neapolitan/__init__.py
--rw-r--r--   0        0        0      273 2023-01-30 10:02:57.766415 neapolitan-23.7/src/neapolitan/templates/neapolitan/object_confirm_delete.html
--rw-r--r--   0        0        0      149 2023-02-03 20:19:46.419308 neapolitan-23.7/src/neapolitan/templates/neapolitan/object_detail.html
--rw-r--r--   0        0        0      427 2023-04-12 09:54:30.457200 neapolitan-23.7/src/neapolitan/templates/neapolitan/object_form.html
--rw-r--r--   0        0        0      381 2023-04-12 07:36:22.945023 neapolitan-23.7/src/neapolitan/templates/neapolitan/object_list.html
--rw-r--r--   0        0        0      131 2023-01-30 15:27:46.386717 neapolitan-23.7/src/neapolitan/templates/neapolitan/partial/detail.html
--rw-r--r--   0        0        0      313 2023-01-30 19:42:10.115831 neapolitan-23.7/src/neapolitan/templates/neapolitan/partial/list.html
--rw-r--r--   0        0        0        0 2023-01-30 15:19:09.531163 neapolitan-23.7/src/neapolitan/templatetags/__init__.py
--rw-r--r--   0        0        0     1263 2023-04-08 14:11:26.730590 neapolitan-23.7/src/neapolitan/templatetags/neapolitan.py
--rw-r--r--   0        0        0    17002 2023-04-11 14:10:32.822513 neapolitan-23.7/src/neapolitan/views.py
--rw-r--r--   0        0        0        0 2023-04-08 09:49:24.396767 neapolitan-23.7/tests/__init__.py
--rw-r--r--   0        0        0      840 2023-04-10 09:00:23.657242 neapolitan-23.7/tests/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-04-08 09:49:24.398351 neapolitan-23.7/tests/migrations/__init__.py
--rw-r--r--   0        0        0      236 2023-04-10 08:59:09.860534 neapolitan-23.7/tests/models.py
--rw-r--r--   0        0        0     1411 2023-04-08 16:03:51.880684 neapolitan-23.7/tests/settings.py
--rw-r--r--   0        0        0      181 2023-04-08 16:13:55.492481 neapolitan-23.7/tests/templates/base.html
--rw-r--r--   0        0        0     4434 2023-04-12 09:58:49.359041 neapolitan-23.7/tests/tests.py
--rw-r--r--   0        0        0     2226 1970-01-01 00:00:00.000000 neapolitan-23.7/PKG-INFO
+-rw-r--r--   0        0        0       59 2023-04-08 15:53:57.994299 neapolitan-23.8/.gitignore
+-rw-r--r--   0        0        0      653 2023-04-24 09:42:29.532121 neapolitan-23.8/CHANGELOG.rst
+-rw-r--r--   0        0        0     1081 2023-04-08 09:37:37.437304 neapolitan-23.8/LICENSE
+-rw-r--r--   0        0        0     1933 2023-04-21 14:19:08.925095 neapolitan-23.8/README.rst
+-rw-r--r--   0        0        0      638 2023-04-08 10:32:21.337055 neapolitan-23.8/docs/Makefile
+-rw-r--r--   0        0        0      804 2023-04-08 10:32:21.337901 neapolitan-23.8/docs/make.bat
+-rw-r--r--   0        0        0      943 2023-04-08 13:11:08.113103 neapolitan-23.8/docs/source/conf.py
+-rw-r--r--   0        0        0      160 2023-04-11 14:07:29.272376 neapolitan-23.8/docs/source/crud-view.rst
+-rw-r--r--   0        0        0     2016 2023-04-21 16:00:29.106838 neapolitan-23.8/docs/source/index.rst
+-rw-r--r--   0        0        0     1028 2023-04-24 09:51:45.493372 neapolitan-23.8/docs/source/templates.rst
+-rw-r--r--   0        0        0      213 2023-04-08 15:52:45.220880 neapolitan-23.8/justfile
+-rw-r--r--   0        0        0      653 2023-04-10 09:35:41.106347 neapolitan-23.8/pyproject.toml
+-rw-r--r--   0        0        0      978 2023-04-24 09:54:57.892476 neapolitan-23.8/src/neapolitan/__init__.py
+-rw-r--r--   0        0        0      273 2023-01-30 10:02:57.766415 neapolitan-23.8/src/neapolitan/templates/neapolitan/object_confirm_delete.html
+-rw-r--r--   0        0        0      149 2023-02-03 20:19:46.419308 neapolitan-23.8/src/neapolitan/templates/neapolitan/object_detail.html
+-rw-r--r--   0        0        0      427 2023-04-12 09:54:30.457200 neapolitan-23.8/src/neapolitan/templates/neapolitan/object_form.html
+-rw-r--r--   0        0        0      381 2023-04-12 07:36:22.945023 neapolitan-23.8/src/neapolitan/templates/neapolitan/object_list.html
+-rw-r--r--   0        0        0      131 2023-01-30 15:27:46.386717 neapolitan-23.8/src/neapolitan/templates/neapolitan/partial/detail.html
+-rw-r--r--   0        0        0      313 2023-01-30 19:42:10.115831 neapolitan-23.8/src/neapolitan/templates/neapolitan/partial/list.html
+-rw-r--r--   0        0        0        0 2023-01-30 15:19:09.531163 neapolitan-23.8/src/neapolitan/templatetags/__init__.py
+-rw-r--r--   0        0        0     1899 2023-04-24 09:52:53.326834 neapolitan-23.8/src/neapolitan/templatetags/neapolitan.py
+-rw-r--r--   0        0        0    17002 2023-04-11 14:10:32.822513 neapolitan-23.8/src/neapolitan/views.py
+-rw-r--r--   0        0        0        0 2023-04-08 09:49:24.396767 neapolitan-23.8/tests/__init__.py
+-rw-r--r--   0        0        0      840 2023-04-10 09:00:23.657242 neapolitan-23.8/tests/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-04-08 09:49:24.398351 neapolitan-23.8/tests/migrations/__init__.py
+-rw-r--r--   0        0        0      236 2023-04-10 08:59:09.860534 neapolitan-23.8/tests/models.py
+-rw-r--r--   0        0        0     1411 2023-04-08 16:03:51.880684 neapolitan-23.8/tests/settings.py
+-rw-r--r--   0        0        0      181 2023-04-08 16:13:55.492481 neapolitan-23.8/tests/templates/base.html
+-rw-r--r--   0        0        0     4434 2023-04-12 09:58:49.359041 neapolitan-23.8/tests/tests.py
+-rw-r--r--   0        0        0     2538 1970-01-01 00:00:00.000000 neapolitan-23.8/PKG-INFO
```

### Comparing `neapolitan-23.7/LICENSE` & `neapolitan-23.8/LICENSE`

 * *Files identical despite different names*

### Comparing `neapolitan-23.7/README.rst` & `neapolitan-23.8/src/neapolitan/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,65 +1,38 @@
-==========
-Neapolitan
-==========
+"""
+Neapolitan: quick CRUD views for Django.
 
 I have a Django model::
 
     from django.db import models
 
     class Bookmark(models.Model):
         url = models.URLField(unique=True)
         title = models.CharField(max_length=255)
         note = models.TextField(blank=True)
-        favourite = models.BooleanField(default=False)
 
 I want easy CRUD views for it, without it taking all day::
 
     # urls.py
     from neapolitan.views import CRUDView
 
     class BookmarkView(CRUDView):
         model = Bookmark
         fields = ["url", "title", "note"]
-        filterset_fields = [
-            "favourite",
-        ]
+
 
     urlpatterns = [ ... ] + BookmarkView.get_urls()
 
-Neapolitan's ``CRUDView`` provides the standard list, detail,
+Neapolitan's `CRUDView` provides the standard list, detail,
 create, edit, and delete views for a model, as well as the hooks you need to
 be able to customise any part of that.
 
 Neapolitan provides base templates and re-usable template tags to make getting
 your model on the page as easy as possible.
 
 Where you take your app after that is up to you. But Neapolitan will get you
 started.
 
 Let's go! 🚀
+"""
 
-Status
-------
-
-This is alpha software. I'm still working out the details of the API, and I've
-not written the docs.
-
-**But**: You could just read `neapolitan.views.CRUDView` and see what it does.
-Up to you. 😜
-
-Installation
-------------
-
-Install with pip::
-
-    pip install neapolitan
-
-Add ``neapolitan`` to your ``INSTALLED_APPS``::
-
-    INSTALLED_APPS = [
-        ...
-        "neapolitan",
-    ]
-
-Templates expect a ``base.html`` template to exist and for that to defined a
-``content`` block. (Refs <https://github.com/carltongibson/neapolitan/issues/6>.)
+__version__ = "23.8"
```

### Comparing `neapolitan-23.7/docs/Makefile` & `neapolitan-23.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `neapolitan-23.7/docs/make.bat` & `neapolitan-23.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `neapolitan-23.7/docs/source/conf.py` & `neapolitan-23.8/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `neapolitan-23.7/docs/source/index.rst` & `neapolitan-23.8/README.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,36 @@
-Welcome to Neapolitan's documentation!
-======================================
+==========
+Neapolitan
+==========
 
-Neapolitan provides quick CRUD views for Django.
+I have a Django model:
 
-I have a Django model::
+.. code:: python
 
     from django.db import models
 
     class Bookmark(models.Model):
         url = models.URLField(unique=True)
         title = models.CharField(max_length=255)
         note = models.TextField(blank=True)
+        favourite = models.BooleanField(default=False)
 
-I want easy CRUD views for it, without it taking all day::
+I want easy CRUD views for it, without it taking all day:
+
+.. code:: python
 
     # urls.py
     from neapolitan.views import CRUDView
 
     class BookmarkView(CRUDView):
         model = Bookmark
         fields = ["url", "title", "note"]
-
+        filterset_fields = [
+            "favourite",
+        ]
 
     urlpatterns = [ ... ] + BookmarkView.get_urls()
 
 Neapolitan's ``CRUDView`` provides the standard list, detail,
 create, edit, and delete views for a model, as well as the hooks you need to
 be able to customise any part of that.
 
@@ -32,22 +38,41 @@
 your model on the page as easy as possible.
 
 Where you take your app after that is up to you. But Neapolitan will get you
 started.
 
 Let's go! 🚀
 
+Next stop `the docs <https://noumenal.es/neapolitan/>`_ 🚂
+
+Versioning and Status
+---------------------
+
+Neapolitan uses a two-part CalVer versioning scheme, such as ``23.7``. The first
+number is the year. The second is the release number within that year.
+
+This is alpha software. I'm still working out the details of the API, and I've
+only begun the docs.
+
+**But**: You could just read ``neapolitan.views.CRUDView`` and see what it does.
+Up to you. 😜
+
+Installation
+------------
+
+Install with pip:
+
+.. code:: bash
+
+    pip install neapolitan
+
+Add ``neapolitan`` to your ``INSTALLED_APPS``:
+
+.. code:: python
+
+    INSTALLED_APPS = [
+        ...
+        "neapolitan",
+    ]
 
-.. toctree::
-    :maxdepth: 1
-    :caption: Contents:
-
-    crud-view
-    templates
-
-..
-   Indices and tables
-   ==================
-
-   * :ref:`genindex`
-   * :ref:`modindex`
-   * :ref:`search`
+Templates expect a ``base.html`` template to exist and for that to defined a
+``content`` block. (Refs <https://github.com/carltongibson/neapolitan/issues/6>.)
```

### Comparing `neapolitan-23.7/pyproject.toml` & `neapolitan-23.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `neapolitan-23.7/src/neapolitan/views.py` & `neapolitan-23.8/src/neapolitan/views.py`

 * *Files identical despite different names*

### Comparing `neapolitan-23.7/tests/migrations/0001_initial.py` & `neapolitan-23.8/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `neapolitan-23.7/tests/settings.py` & `neapolitan-23.8/tests/settings.py`

 * *Files identical despite different names*

### Comparing `neapolitan-23.7/tests/tests.py` & `neapolitan-23.8/tests/tests.py`

 * *Files identical despite different names*

### Comparing `neapolitan-23.7/PKG-INFO` & `neapolitan-23.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neapolitan
-Version: 23.7
+Version: 23.8
 Summary: Neapolitan: quick CRUD views for Django.
 Author-email: Carlton Gibson <carlton.gibson@noumenal.es>
 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: Django
 Requires-Dist: django-filter
 Requires-Dist: Sphinx ; extra == "docs"
@@ -15,25 +15,29 @@
 Provides-Extra: docs
 Provides-Extra: tests
 
 ==========
 Neapolitan
 ==========
 
-I have a Django model::
+I have a Django model:
+
+.. code:: python
 
     from django.db import models
 
     class Bookmark(models.Model):
         url = models.URLField(unique=True)
         title = models.CharField(max_length=255)
         note = models.TextField(blank=True)
         favourite = models.BooleanField(default=False)
 
-I want easy CRUD views for it, without it taking all day::
+I want easy CRUD views for it, without it taking all day:
+
+.. code:: python
 
     # urls.py
     from neapolitan.views import CRUDView
 
     class BookmarkView(CRUDView):
         model = Bookmark
         fields = ["url", "title", "note"]
@@ -51,31 +55,40 @@
 your model on the page as easy as possible.
 
 Where you take your app after that is up to you. But Neapolitan will get you
 started.
 
 Let's go! 🚀
 
-Status
-------
+Next stop `the docs <https://noumenal.es/neapolitan/>`_ 🚂
+
+Versioning and Status
+---------------------
+
+Neapolitan uses a two-part CalVer versioning scheme, such as ``23.7``. The first
+number is the year. The second is the release number within that year.
 
 This is alpha software. I'm still working out the details of the API, and I've
-not written the docs.
+only begun the docs.
 
-**But**: You could just read `neapolitan.views.CRUDView` and see what it does.
+**But**: You could just read ``neapolitan.views.CRUDView`` and see what it does.
 Up to you. 😜
 
 Installation
 ------------
 
-Install with pip::
+Install with pip:
+
+.. code:: bash
 
     pip install neapolitan
 
-Add ``neapolitan`` to your ``INSTALLED_APPS``::
+Add ``neapolitan`` to your ``INSTALLED_APPS``:
+
+.. code:: python
 
     INSTALLED_APPS = [
         ...
         "neapolitan",
     ]
 
 Templates expect a ``base.html`` template to exist and for that to defined a
```

