# Comparing `tmp/django_htmx_ui-0.1.4.tar.gz` & `tmp/django_htmx_ui-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_htmx_ui-0.1.4.tar", last modified: Fri Mar 10 16:05:49 2023, max compression
+gzip compressed data, was "django_htmx_ui-0.1.5.tar", last modified: Mon Apr 24 09:31:21 2023, max compression
```

## Comparing `django_htmx_ui-0.1.4.tar` & `django_htmx_ui-0.1.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 nikalexis  (1000) nikalexis  (1000)        0 2023-03-10 16:05:49.527339 django_htmx_ui-0.1.4/
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)     1075 2023-02-28 15:45:04.000000 django_htmx_ui-0.1.4/LICENSE
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)    30677 2023-03-10 16:05:49.527339 django_htmx_ui-0.1.4/PKG-INFO
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)    30127 2023-03-02 09:30:30.000000 django_htmx_ui-0.1.4/README.md
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)      721 2023-03-10 16:04:05.000000 django_htmx_ui-0.1.4/pyproject.toml
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)       38 2023-03-10 16:05:49.527339 django_htmx_ui-0.1.4/setup.cfg
-drwxrwxr-x   0 nikalexis  (1000) nikalexis  (1000)        0 2023-03-10 16:05:49.519338 django_htmx_ui-0.1.4/src/
-drwxrwxr-x   0 nikalexis  (1000) nikalexis  (1000)        0 2023-03-10 16:05:49.523339 django_htmx_ui-0.1.4/src/django_htmx_ui/
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)        0 2023-02-28 15:45:04.000000 django_htmx_ui-0.1.4/src/django_htmx_ui/__init__.py
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)        0 2023-02-28 15:45:04.000000 django_htmx_ui-0.1.4/src/django_htmx_ui/admin.py
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)      158 2023-02-28 15:45:04.000000 django_htmx_ui-0.1.4/src/django_htmx_ui/apps.py
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)        0 2023-02-28 15:45:04.000000 django_htmx_ui-0.1.4/src/django_htmx_ui/forms.py
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)     1305 2023-03-08 10:26:03.000000 django_htmx_ui-0.1.4/src/django_htmx_ui/jinja.py
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)     1744 2023-02-28 15:45:04.000000 django_htmx_ui-0.1.4/src/django_htmx_ui/middleware.py
-drwxrwxr-x   0 nikalexis  (1000) nikalexis  (1000)        0 2023-03-10 16:05:49.523339 django_htmx_ui-0.1.4/src/django_htmx_ui/migrations/
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)        0 2023-02-28 15:45:04.000000 django_htmx_ui-0.1.4/src/django_htmx_ui/migrations/__init__.py
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)        0 2023-02-28 15:45:04.000000 django_htmx_ui-0.1.4/src/django_htmx_ui/models.py
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)       60 2023-02-28 15:45:04.000000 django_htmx_ui-0.1.4/src/django_htmx_ui/tests.py
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)        0 2023-02-28 15:45:04.000000 django_htmx_ui-0.1.4/src/django_htmx_ui/urls.py
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)     7203 2023-03-01 13:15:10.000000 django_htmx_ui-0.1.4/src/django_htmx_ui/utils.py
-drwxrwxr-x   0 nikalexis  (1000) nikalexis  (1000)        0 2023-03-10 16:05:49.523339 django_htmx_ui-0.1.4/src/django_htmx_ui/views/
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)     1929 2023-02-28 15:45:04.000000 django_htmx_ui-0.1.4/src/django_htmx_ui/views/crud.py
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)     6951 2023-03-01 12:40:50.000000 django_htmx_ui-0.1.4/src/django_htmx_ui/views/generic.py
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)     6363 2023-03-01 15:21:27.000000 django_htmx_ui-0.1.4/src/django_htmx_ui/views/mixins.py
-drwxrwxr-x   0 nikalexis  (1000) nikalexis  (1000)        0 2023-03-10 16:05:49.523339 django_htmx_ui-0.1.4/src/django_htmx_ui.egg-info/
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)    30677 2023-03-10 16:05:49.000000 django_htmx_ui-0.1.4/src/django_htmx_ui.egg-info/PKG-INFO
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)      674 2023-03-10 16:05:49.000000 django_htmx_ui-0.1.4/src/django_htmx_ui.egg-info/SOURCES.txt
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)        1 2023-03-10 16:05:49.000000 django_htmx_ui-0.1.4/src/django_htmx_ui.egg-info/dependency_links.txt
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)       50 2023-03-10 16:05:49.000000 django_htmx_ui-0.1.4/src/django_htmx_ui.egg-info/requires.txt
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)       15 2023-03-10 16:05:49.000000 django_htmx_ui-0.1.4/src/django_htmx_ui.egg-info/top_level.txt
+drwxr-xr-x   0 nikalexis  (1000) nikalexis  (1000)        0 2023-04-24 09:31:21.301876 django_htmx_ui-0.1.5/
+-rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)     1075 2023-02-27 22:03:36.000000 django_htmx_ui-0.1.5/LICENSE
+-rw-r--r--   0 nikalexis  (1000) nikalexis  (1000)    31177 2023-04-24 09:31:21.301876 django_htmx_ui-0.1.5/PKG-INFO
+-rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)    30627 2023-04-24 09:25:54.000000 django_htmx_ui-0.1.5/README.md
+-rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)      721 2023-04-24 09:25:30.000000 django_htmx_ui-0.1.5/pyproject.toml
+-rw-r--r--   0 nikalexis  (1000) nikalexis  (1000)       38 2023-04-24 09:31:21.301876 django_htmx_ui-0.1.5/setup.cfg
+drwxr-xr-x   0 nikalexis  (1000) nikalexis  (1000)        0 2023-04-24 09:31:21.301876 django_htmx_ui-0.1.5/src/
+drwxr-xr-x   0 nikalexis  (1000) nikalexis  (1000)        0 2023-04-24 09:31:21.301876 django_htmx_ui-0.1.5/src/django_htmx_ui/
+-rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)        0 2023-02-08 11:09:09.000000 django_htmx_ui-0.1.5/src/django_htmx_ui/__init__.py
+-rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)        0 2023-02-08 11:09:09.000000 django_htmx_ui-0.1.5/src/django_htmx_ui/admin.py
+-rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)      158 2023-02-08 11:09:09.000000 django_htmx_ui-0.1.5/src/django_htmx_ui/apps.py
+-rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)        0 2023-02-08 11:09:09.000000 django_htmx_ui-0.1.5/src/django_htmx_ui/forms.py
+-rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)     1305 2023-03-11 08:30:48.000000 django_htmx_ui-0.1.5/src/django_htmx_ui/jinja.py
+-rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)     1744 2023-02-08 11:09:09.000000 django_htmx_ui-0.1.5/src/django_htmx_ui/middleware.py
+drwxr-xr-x   0 nikalexis  (1000) nikalexis  (1000)        0 2023-04-24 09:31:21.301876 django_htmx_ui-0.1.5/src/django_htmx_ui/migrations/
+-rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)        0 2023-02-08 11:09:09.000000 django_htmx_ui-0.1.5/src/django_htmx_ui/migrations/__init__.py
+-rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)        0 2023-02-08 11:09:09.000000 django_htmx_ui-0.1.5/src/django_htmx_ui/models.py
+-rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)       60 2023-02-08 11:09:09.000000 django_htmx_ui-0.1.5/src/django_htmx_ui/tests.py
+-rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)        0 2023-02-08 11:09:09.000000 django_htmx_ui-0.1.5/src/django_htmx_ui/urls.py
+-rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)     7519 2023-04-20 08:28:01.000000 django_htmx_ui-0.1.5/src/django_htmx_ui/utils.py
+drwxr-xr-x   0 nikalexis  (1000) nikalexis  (1000)        0 2023-04-24 09:31:21.301876 django_htmx_ui-0.1.5/src/django_htmx_ui/views/
+-rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)     1929 2023-02-26 11:45:23.000000 django_htmx_ui-0.1.5/src/django_htmx_ui/views/crud.py
+-rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)     6947 2023-04-24 08:59:54.000000 django_htmx_ui-0.1.5/src/django_htmx_ui/views/generic.py
+-rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)     7441 2023-04-23 16:59:32.000000 django_htmx_ui-0.1.5/src/django_htmx_ui/views/mixins.py
+drwxr-xr-x   0 nikalexis  (1000) nikalexis  (1000)        0 2023-04-24 09:31:21.301876 django_htmx_ui-0.1.5/src/django_htmx_ui.egg-info/
+-rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)    31177 2023-04-24 09:31:21.000000 django_htmx_ui-0.1.5/src/django_htmx_ui.egg-info/PKG-INFO
+-rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)      674 2023-04-24 09:31:21.000000 django_htmx_ui-0.1.5/src/django_htmx_ui.egg-info/SOURCES.txt
+-rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)        1 2023-04-24 09:31:21.000000 django_htmx_ui-0.1.5/src/django_htmx_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 nikalexis  (1000) nikalexis  (1000)       50 2023-04-24 09:31:21.000000 django_htmx_ui-0.1.5/src/django_htmx_ui.egg-info/requires.txt
+-rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)       15 2023-04-24 09:31:21.000000 django_htmx_ui-0.1.5/src/django_htmx_ui.egg-info/top_level.txt
```

### Comparing `django_htmx_ui-0.1.4/LICENSE` & `django_htmx_ui-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django_htmx_ui-0.1.4/PKG-INFO` & `django_htmx_ui-0.1.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: django_htmx_ui
-Version: 0.1.4
-Summary: Django - HTMX - Jinja powerful combination library
-Author-email: Nikalexis Nikolaos <nikalexis@gmail.com>
-Project-URL: Homepage, https://github.com/nikalexis/django_htmx_ui
-Project-URL: Bug Tracker, https://github.com/nikalexis/django_htmx_ui/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Intro
 
 ## What is `django_htmx_ui` library
 
 This library is made to combine and help leveraging:
 * the full-stack [django](https://www.djangoproject.com/) framework
 * the frontend [htmx](https://htmx.org/) framework
@@ -196,16 +182,16 @@
 All sub-pages can extend these two basic classes like this:
 `Login(WelcomeOrigin)` or `Dashboard(DefaultPanelOrigin)`.
 These sub-pages will have their own templates, but will be served by a htmx lazy-load get.
 
 #### Creating a partial sub-page
 
 If you now want to create a Widget inside your user's dashboard page, you can define
-its view as `Widget(PartialMixin, DefaultPanelOrigin)`. Please, notice the usage of the
-`PartialMixin`. When you add this Mixin, it means that this view can only be requested
+its view as `Widget(PartialTemplateMixin, DefaultPanelOrigin)`. Please, notice the usage of the
+`PartialTemplateMixin`. When you add this Mixin, it means that this view can only be requested
 via a htmx request, therefore it can't be opened directly from the browser's address
 bar.
 
 #### Creating your first html with htmx usage
 
 This is a very simplified example to make you understand what this library does.
 
@@ -548,14 +534,32 @@
 `on_post_invalid_message` attributes.
 
 ### Mixins
 
 The following Mixins are available to automate some common scenarios.
 Feel free to extend them more or overwriting the attributes.
 
+#### *django_htmx_ui.views.mixins.*__OriginTemplateMixin__
+
+Add this Mixin in your `TemplateView` for the view to be accessible directly from
+a browser HTTP request and via a htmx request.
+You can also set the `push_url` attribute to `False`. In that case, the URL will be
+replaces in the browser's bar but no history will be creared (`HX-Replace` header).
+You can also set the `push_url` attribute to `None`. In that case, the URL will not
+be replaced in the browser's bar.
+
+#### *django_htmx_ui.views.mixins.*__PartialTemplateMixin__
+
+Add this Mixin in your `TemplateView` for the view to be only accessible via a htmx
+request.
+By default, if the url of view is called directly from the browser (outside htmx call),
+a redirection will happen to the `/` route path.
+You can overwrite the default redirection route path by defining the `redirect_partial`
+attribute of the view.
+
 #### *django_htmx_ui.views.mixins.*__FormMixin__
 
 Add this Mixin in your `TemplateView`, if the view contains a form.
 You can define a `Form` class inside the `TemplateView` class, which is recommended to
 be a subclass of django's `Form` or `ModelForm` or any other similar kind.
 
 For example:
@@ -630,23 +634,14 @@
 
 Sets a "'Instance' saved" message, when the form is successfully saved.
 
 `on_post_success_message` method
 
 Sets a "'Instance' not saved" message, when the form is not valid.
 
-#### *django_htmx_ui.views.mixins.*__PartialMixin__
-
-Add this Mixin in your `TemplateView` for the view to be only accessible via a htmx
-request.
-By default, if the url of view is called directly from the browser (outside htmx call),
-a redirection will happen to the `/` route path.
-You can overwrite the default redirection route path by defining the `redirect_partial`
-attribute of the view.
-
 #### *django_htmx_ui.views.mixins.*__ResponseNoContentMixin__
 
 Add this Mixin in your `TemplateView` to return `HTTP 204 No Content` as a response.
 No template rendering will happen.
 
 #### *django_htmx_ui.views.mixins.*__TabsMixin__
```

### Comparing `django_htmx_ui-0.1.4/README.md` & `django_htmx_ui-0.1.5/src/django_htmx_ui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: django-htmx-ui
+Version: 0.1.5
+Summary: Django - HTMX - Jinja powerful combination library
+Author-email: Nikalexis Nikolaos <nikalexis@gmail.com>
+Project-URL: Homepage, https://github.com/nikalexis/django_htmx_ui
+Project-URL: Bug Tracker, https://github.com/nikalexis/django_htmx_ui/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Intro
 
 ## What is `django_htmx_ui` library
 
 This library is made to combine and help leveraging:
 * the full-stack [django](https://www.djangoproject.com/) framework
 * the frontend [htmx](https://htmx.org/) framework
@@ -182,16 +196,16 @@
 All sub-pages can extend these two basic classes like this:
 `Login(WelcomeOrigin)` or `Dashboard(DefaultPanelOrigin)`.
 These sub-pages will have their own templates, but will be served by a htmx lazy-load get.
 
 #### Creating a partial sub-page
 
 If you now want to create a Widget inside your user's dashboard page, you can define
-its view as `Widget(PartialMixin, DefaultPanelOrigin)`. Please, notice the usage of the
-`PartialMixin`. When you add this Mixin, it means that this view can only be requested
+its view as `Widget(PartialTemplateMixin, DefaultPanelOrigin)`. Please, notice the usage of the
+`PartialTemplateMixin`. When you add this Mixin, it means that this view can only be requested
 via a htmx request, therefore it can't be opened directly from the browser's address
 bar.
 
 #### Creating your first html with htmx usage
 
 This is a very simplified example to make you understand what this library does.
 
@@ -534,14 +548,32 @@
 `on_post_invalid_message` attributes.
 
 ### Mixins
 
 The following Mixins are available to automate some common scenarios.
 Feel free to extend them more or overwriting the attributes.
 
+#### *django_htmx_ui.views.mixins.*__OriginTemplateMixin__
+
+Add this Mixin in your `TemplateView` for the view to be accessible directly from
+a browser HTTP request and via a htmx request.
+You can also set the `push_url` attribute to `False`. In that case, the URL will be
+replaces in the browser's bar but no history will be creared (`HX-Replace` header).
+You can also set the `push_url` attribute to `None`. In that case, the URL will not
+be replaced in the browser's bar.
+
+#### *django_htmx_ui.views.mixins.*__PartialTemplateMixin__
+
+Add this Mixin in your `TemplateView` for the view to be only accessible via a htmx
+request.
+By default, if the url of view is called directly from the browser (outside htmx call),
+a redirection will happen to the `/` route path.
+You can overwrite the default redirection route path by defining the `redirect_partial`
+attribute of the view.
+
 #### *django_htmx_ui.views.mixins.*__FormMixin__
 
 Add this Mixin in your `TemplateView`, if the view contains a form.
 You can define a `Form` class inside the `TemplateView` class, which is recommended to
 be a subclass of django's `Form` or `ModelForm` or any other similar kind.
 
 For example:
@@ -616,23 +648,14 @@
 
 Sets a "'Instance' saved" message, when the form is successfully saved.
 
 `on_post_success_message` method
 
 Sets a "'Instance' not saved" message, when the form is not valid.
 
-#### *django_htmx_ui.views.mixins.*__PartialMixin__
-
-Add this Mixin in your `TemplateView` for the view to be only accessible via a htmx
-request.
-By default, if the url of view is called directly from the browser (outside htmx call),
-a redirection will happen to the `/` route path.
-You can overwrite the default redirection route path by defining the `redirect_partial`
-attribute of the view.
-
 #### *django_htmx_ui.views.mixins.*__ResponseNoContentMixin__
 
 Add this Mixin in your `TemplateView` to return `HTTP 204 No Content` as a response.
 No template rendering will happen.
 
 #### *django_htmx_ui.views.mixins.*__TabsMixin__
```

### Comparing `django_htmx_ui-0.1.4/pyproject.toml` & `django_htmx_ui-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django_htmx_ui"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="Nikalexis Nikolaos", email="nikalexis@gmail.com" },
 ]
 description = "Django - HTMX - Jinja powerful combination library"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `django_htmx_ui-0.1.4/src/django_htmx_ui/jinja.py` & `django_htmx_ui-0.1.5/src/django_htmx_ui/jinja.py`

 * *Files identical despite different names*

### Comparing `django_htmx_ui-0.1.4/src/django_htmx_ui/middleware.py` & `django_htmx_ui-0.1.5/src/django_htmx_ui/middleware.py`

 * *Files identical despite different names*

### Comparing `django_htmx_ui-0.1.4/src/django_htmx_ui/utils.py` & `django_htmx_ui-0.1.5/src/django_htmx_ui/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,21 @@
             return self.url
 
         def update(self, **kwargs):
             for name, value in kwargs.items():
                 self.remove(name)
                 self.query_list.append((name, value))
             return self.url
+        
+        def get(self, key, single=False, single_index=-1):
+            values = [value for name, value in self.query_list if name == key]
+            if len(values) > 1:
+                return values if not single else values[single_index]
+            elif len(values) == 1:
+                return values[0]
 
     def __init__(self, path, query_list):
         self.path = str(path)
         self.query = Url.Query(query_list, self)
 
     def __call__(self, path=None, query_list=None):
         if path is not None:
@@ -148,15 +155,15 @@
 
 class Location(Url):
 
     def __init__(self, path, query_list, push=False):
         self.push = push
         super().__init__(path, query_list)
 
-    def __call__(self, path=None, query_list=None, push=False):
+    def __call__(self, path=None, query_list=None, push=None):
         if push is not None:
             self.push = push
         return super().__call__(path, query_list)
 
     @property
     def resolver_match(self):
         return resolve(self.path)
```

### Comparing `django_htmx_ui-0.1.4/src/django_htmx_ui/views/crud.py` & `django_htmx_ui-0.1.5/src/django_htmx_ui/views/crud.py`

 * *Files identical despite different names*

### Comparing `django_htmx_ui-0.1.4/src/django_htmx_ui/views/generic.py` & `django_htmx_ui-0.1.5/src/django_htmx_ui/views/generic.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     response = None
 
     def setup(self, request, *args, **kwargs):
         self.headers = {}
         self.triggers = []
         self.request = request
         self.location_bar = Location.create_from_url(self.bar_url())
-        self.location_req = Location.create_from_url(request.META['PATH_INFO'])
+        self.location_req = Location.create_from_url(request.get_full_path())
         self.add_context('request', request)
         return super().setup(request, *args, **kwargs)
 
     def get(self, request, *args, **kwargs):
         ret = self.on_get(request, *args, **kwargs)
         if ret:
             return ret
@@ -158,15 +158,15 @@
             return redirect(url)
 
     @ContextProperty
     def url(self):
         return UrlView(self)
 
     def bar_url(self):
-        return self.request.headers.get('HX-Current-URL', self.request.META['PATH_INFO'])
+        return self.request.headers.get('HX-Current-URL', self.request.get_full_path())
 
     @classmethod
     @property
     def templates_dir(cls):
         if hasattr(cls.module, 'TEMPLATES_DIR'):
             return cls.module.TEMPLATES_DIR
         else:
```

### Comparing `django_htmx_ui-0.1.4/src/django_htmx_ui/views/mixins.py` & `django_htmx_ui-0.1.5/src/django_htmx_ui/views/mixins.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 from django.core.exceptions import ViewDoesNotExist
 from django.shortcuts import redirect
+from django.utils.text import slugify
 
 from django_htmx_ui.utils import ContextProperty, ContextCachedProperty, UrlView, to_snake_case
 
 
 class OriginTemplateMixin:
+    push_url = True
 
     def get(self, request, *args, **kwargs):
         if request.htmx and OriginTemplateMixin in self.__class__.__bases__:
             raise ViewDoesNotExist("View '%s' is an 'OriginTemplateMixin'." % self.__class__.__name__)
         else:
+            if self.push_url is not None and self.location_bar.path != self.location_req.path:
+                self.location_bar(path=self.location_req.path, query_list=self.location_req.query.query_list, push=self.push_url)
             return super().get(request, *args, **kwargs)
 
 
 class PartialTemplateMixin:
     redirect_partial = '/'
 
     def get(self, request, *args, **kwargs):
@@ -124,23 +128,27 @@
             def __init__(self, title, url, slug=None):
                 self.title = title
                 self.url = url
                 self._slug = slug
 
             @property
             def slug(self):
-                return self._slug or self.index
+                return self._slug or str(self.index)
 
-        def __init__(self, *links, selected=0, remember=False):
+        def __init__(self, *links, selected=0, remember=False, titles_slugify=True):
             self.selected = selected
             self.remember = remember
             self.links = links
 
             for i, l in enumerate(self.links):
                 l.index = i
+                if titles_slugify and l._slug is None:
+                    l._slug = slugify(l.title) or None
+                    if l._slug in [ls.slug for ls in self.links if ls.index != l.index]:
+                        l._slug = None
 
         @property
         def active(self):
             return self.links[self.selected]
 
     def __init__(self, *args, **kwargs):
         class TabsView(TabsMixin.Tabs):
@@ -151,52 +159,65 @@
     @ContextProperty
     def tabs(self):
         raise NotImplementedError()
 
     @classmethod
     @property
     def slug_tab(cls):
-        return f'{cls.slug_module}_tab'
+        return f'{cls.slug_global}_tab'
 
     @property
     def tab_query_var(self):
         return self.slug_tab
+    
+    @property
+    def tab_session_key(self):
+        return f'tabs-remember-{self.slug_tab}'
+    
+    @property
+    def tab_selected_candidates(self):
+        return [
+            self.request.resolver_match.kwargs.get(self.slug_tab),
+            self.location_req.query.get(self.tab_query_var, True),
+            self.location_bar.query.get(self.tab_query_var, True),
+            self.request.session.get(self.tab_session_key),
+        ]
 
     @classmethod
     @property
     def path_route(cls):
         return super().path_route + f'(?:(?P<{cls.slug_tab}>\w+)/)?'
 
     def on_get(self, request, *args, **kwargs):
         super().on_get(request, *args, **kwargs)
 
-        session_key = f'tabs-remember-{self.slug_tab}'
-        if self.tabs.remember and session_key in request.session:
-            self.tabs.selected = int(request.session[session_key])
-
-        if self.tab_query_var in request.GET:
-            self.tabs.selected = int(request.GET[self.tab_query_var])
-
-        slug_tab_value = self.request.resolver_match.kwargs.get(self.slug_tab)
-        if slug_tab_value:
-            for link in self.tabs.links:
-                if link.slug == slug_tab_value:
-                    self.tabs.selected = int(link.index)
-                    break
-            else:
-                raise ValueError(f"Tab slug '{slug_tab_value}' not found.")
+        if self.request.session.get(self.tab_session_key) not in [None] + [l.slug for l in self.tabs.links]:
+            del self.request.session[self.tab_session_key]
+
+        for c in self.tab_selected_candidates:
+            if c is not None:
+                for link in self.tabs.links:
+                    if c in (link._slug, str(link.index)):
+                        self.tabs.selected = link.index
+                        break
+                else:
+                    raise ValueError(f"Tab slug '{c}' not found.")
+                break
 
-        if self.tabs.active.slug:
+        if self.location_bar.resolver_match.view_name == self.url.resolver_match.view_name:
             new_path = self.url(**{self.slug_tab: self.tabs.active.slug})
-            slug_location_bar = self.location_bar.resolver_match.kwargs.get(self.slug_tab)
-            push = slug_location_bar not in (None, slug_tab_value)
-            self.location_bar(path=new_path, push=push)
+            self.location_bar(path=new_path).query.remove(self.tab_query_var)
+        else:
+            current_slug = self.location_bar.query.get(self.tab_query_var)
+            if current_slug != self.tabs.active.slug:
+                push = current_slug is not None
+                self.location_bar(push=push).query(**{self.tab_query_var: self.tabs.active.slug})
 
         if self.tabs.remember:
-            request.session[session_key] = int(self.tabs.selected)
+            request.session[self.tab_session_key] = self.tabs.active.slug
 
 
 class ModalMixin:
 
     class Modal:
 
         def __init__(self, url, _id=None):
```

### Comparing `django_htmx_ui-0.1.4/src/django_htmx_ui.egg-info/PKG-INFO` & `django_htmx_ui-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: django-htmx-ui
-Version: 0.1.4
+Name: django_htmx_ui
+Version: 0.1.5
 Summary: Django - HTMX - Jinja powerful combination library
 Author-email: Nikalexis Nikolaos <nikalexis@gmail.com>
 Project-URL: Homepage, https://github.com/nikalexis/django_htmx_ui
 Project-URL: Bug Tracker, https://github.com/nikalexis/django_htmx_ui/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -196,16 +196,16 @@
 All sub-pages can extend these two basic classes like this:
 `Login(WelcomeOrigin)` or `Dashboard(DefaultPanelOrigin)`.
 These sub-pages will have their own templates, but will be served by a htmx lazy-load get.
 
 #### Creating a partial sub-page
 
 If you now want to create a Widget inside your user's dashboard page, you can define
-its view as `Widget(PartialMixin, DefaultPanelOrigin)`. Please, notice the usage of the
-`PartialMixin`. When you add this Mixin, it means that this view can only be requested
+its view as `Widget(PartialTemplateMixin, DefaultPanelOrigin)`. Please, notice the usage of the
+`PartialTemplateMixin`. When you add this Mixin, it means that this view can only be requested
 via a htmx request, therefore it can't be opened directly from the browser's address
 bar.
 
 #### Creating your first html with htmx usage
 
 This is a very simplified example to make you understand what this library does.
 
@@ -548,14 +548,32 @@
 `on_post_invalid_message` attributes.
 
 ### Mixins
 
 The following Mixins are available to automate some common scenarios.
 Feel free to extend them more or overwriting the attributes.
 
+#### *django_htmx_ui.views.mixins.*__OriginTemplateMixin__
+
+Add this Mixin in your `TemplateView` for the view to be accessible directly from
+a browser HTTP request and via a htmx request.
+You can also set the `push_url` attribute to `False`. In that case, the URL will be
+replaces in the browser's bar but no history will be creared (`HX-Replace` header).
+You can also set the `push_url` attribute to `None`. In that case, the URL will not
+be replaced in the browser's bar.
+
+#### *django_htmx_ui.views.mixins.*__PartialTemplateMixin__
+
+Add this Mixin in your `TemplateView` for the view to be only accessible via a htmx
+request.
+By default, if the url of view is called directly from the browser (outside htmx call),
+a redirection will happen to the `/` route path.
+You can overwrite the default redirection route path by defining the `redirect_partial`
+attribute of the view.
+
 #### *django_htmx_ui.views.mixins.*__FormMixin__
 
 Add this Mixin in your `TemplateView`, if the view contains a form.
 You can define a `Form` class inside the `TemplateView` class, which is recommended to
 be a subclass of django's `Form` or `ModelForm` or any other similar kind.
 
 For example:
@@ -630,23 +648,14 @@
 
 Sets a "'Instance' saved" message, when the form is successfully saved.
 
 `on_post_success_message` method
 
 Sets a "'Instance' not saved" message, when the form is not valid.
 
-#### *django_htmx_ui.views.mixins.*__PartialMixin__
-
-Add this Mixin in your `TemplateView` for the view to be only accessible via a htmx
-request.
-By default, if the url of view is called directly from the browser (outside htmx call),
-a redirection will happen to the `/` route path.
-You can overwrite the default redirection route path by defining the `redirect_partial`
-attribute of the view.
-
 #### *django_htmx_ui.views.mixins.*__ResponseNoContentMixin__
 
 Add this Mixin in your `TemplateView` to return `HTTP 204 No Content` as a response.
 No template rendering will happen.
 
 #### *django_htmx_ui.views.mixins.*__TabsMixin__
```

### Comparing `django_htmx_ui-0.1.4/src/django_htmx_ui.egg-info/SOURCES.txt` & `django_htmx_ui-0.1.5/src/django_htmx_ui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

