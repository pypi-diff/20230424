# Comparing `tmp/pursuitlib-django-0.2.8.tar.gz` & `tmp/pursuitlib-django-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pursuitlib-django-0.2.8.tar", last modified: Wed Dec 14 14:43:14 2022, max compression
+gzip compressed data, was "pursuitlib-django-0.2.9.tar", last modified: Sat Mar 18 20:00:28 2023, max compression
```

## Comparing `pursuitlib-django-0.2.8.tar` & `pursuitlib-django-0.2.9.tar`

### file list

```diff
@@ -1,75 +1,76 @@
-drwxrwxrwx   0        0        0        0 2022-12-14 14:43:14.492316 pursuitlib-django-0.2.8/
--rw-rw-rw-   0        0        0     1518 2022-12-14 14:43:14.491325 pursuitlib-django-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     1100 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/README.md
-drwxrwxrwx   0        0        0        0 2022-12-14 14:43:13.949128 pursuitlib-django-0.2.8/pursuitlib_django/
--rw-rw-rw-   0        0        0        0 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/__init__.py
--rw-rw-rw-   0        0        0       30 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/admin.py
--rw-rw-rw-   0        0        0      165 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/apps.py
--rw-rw-rw-   0        0        0      665 2022-12-06 23:37:10.000000 pursuitlib-django-0.2.8/pursuitlib_django/errors.py
--rw-rw-rw-   0        0        0     4161 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/forms.py
-drwxrwxrwx   0        0        0        0 2022-12-14 14:43:13.771129 pursuitlib-django-0.2.8/pursuitlib_django/locale/
-drwxrwxrwx   0        0        0        0 2022-12-14 14:43:13.773131 pursuitlib-django-0.2.8/pursuitlib_django/locale/fr/
-drwxrwxrwx   0        0        0        0 2022-12-14 14:43:13.996131 pursuitlib-django-0.2.8/pursuitlib_django/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0        0        0     5401 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/locale/fr/LC_MESSAGES/django.po
--rw-rw-rw-   0        0        0      487 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/mailto.py
-drwxrwxrwx   0        0        0        0 2022-12-14 14:43:13.999130 pursuitlib-django-0.2.8/pursuitlib_django/migrations/
--rw-rw-rw-   0        0        0        0 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/migrations/__init__.py
--rw-rw-rw-   0        0        0      993 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/models.py
--rw-rw-rw-   0        0        0      754 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/signals.py
-drwxrwxrwx   0        0        0        0 2022-12-14 14:43:13.781133 pursuitlib-django-0.2.8/pursuitlib_django/static/
-drwxrwxrwx   0        0        0        0 2022-12-14 14:43:14.102126 pursuitlib-django-0.2.8/pursuitlib_django/static/css/
--rw-rw-rw-   0        0        0    59309 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/static/css/fa.min.css
--rw-rw-rw-   0        0        0      247 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/static/css/pursuitlib-admin.css
--rw-rw-rw-   0        0        0     1424 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/static/css/pursuitlib.css
--rw-rw-rw-   0        0        0    22198 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/static/css/select2-bootstrap-5-theme.min.css
--rw-rw-rw-   0        0        0    16265 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/static/css/select2.min.css
-drwxrwxrwx   0        0        0        0 2022-12-14 14:43:14.251129 pursuitlib-django-0.2.8/pursuitlib_django/static/js/
--rw-rw-rw-   0        0        0    78135 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/static/js/bootstrap.bundle.min.js
--rw-rw-rw-   0        0        0   331017 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/static/js/bootstrap.bundle.min.js.map
-drwxrwxrwx   0        0        0        0 2022-12-14 14:43:13.779131 pursuitlib-django-0.2.8/pursuitlib_django/static/js/i18n/
-drwxrwxrwx   0        0        0        0 2022-12-14 14:43:14.262127 pursuitlib-django-0.2.8/pursuitlib_django/static/js/i18n/select2/
--rw-rw-rw-   0        0        0      983 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/static/js/i18n/select2/fr.js
--rw-rw-rw-   0        0        0    89503 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/static/js/jquery-3.6.0.min.js
--rw-rw-rw-   0        0        0      478 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/static/js/pursuitlib-collapseToggle.js
--rw-rw-rw-   0        0        0       85 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/static/js/pursuitlib-tooltips.js
--rw-rw-rw-   0        0        0    76776 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/static/js/select2.full.min.js
-drwxrwxrwx   0        0        0        0 2022-12-14 14:43:14.473317 pursuitlib-django-0.2.8/pursuitlib_django/static/webfonts/
--rw-rw-rw-   0        0        0   134294 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/static/webfonts/fa-brands-400.eot
--rw-rw-rw-   0        0        0   751644 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/static/webfonts/fa-brands-400.svg
--rw-rw-rw-   0        0        0   133988 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/static/webfonts/fa-brands-400.ttf
--rw-rw-rw-   0        0        0    89988 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/static/webfonts/fa-brands-400.woff
--rw-rw-rw-   0        0        0    76736 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/static/webfonts/fa-brands-400.woff2
--rw-rw-rw-   0        0        0    34034 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/static/webfonts/fa-regular-400.eot
--rw-rw-rw-   0        0        0   145515 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/static/webfonts/fa-regular-400.svg
--rw-rw-rw-   0        0        0    33736 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/static/webfonts/fa-regular-400.ttf
--rw-rw-rw-   0        0        0    16276 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/static/webfonts/fa-regular-400.woff
--rw-rw-rw-   0        0        0    13224 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/static/webfonts/fa-regular-400.woff2
--rw-rw-rw-   0        0        0   203030 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/static/webfonts/fa-solid-900.eot
--rw-rw-rw-   0        0        0   924025 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/static/webfonts/fa-solid-900.svg
--rw-rw-rw-   0        0        0   202744 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/static/webfonts/fa-solid-900.ttf
--rw-rw-rw-   0        0        0   101648 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/static/webfonts/fa-solid-900.woff
--rw-rw-rw-   0        0        0    78268 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/static/webfonts/fa-solid-900.woff2
-drwxrwxrwx   0        0        0        0 2022-12-14 14:43:13.784132 pursuitlib-django-0.2.8/pursuitlib_django/templates/
-drwxrwxrwx   0        0        0        0 2022-12-14 14:43:13.787129 pursuitlib-django-0.2.8/pursuitlib_django/templates/pursuitlib/
-drwxrwxrwx   0        0        0        0 2022-12-14 14:43:14.479318 pursuitlib-django-0.2.8/pursuitlib_django/templates/pursuitlib/component/
--rw-rw-rw-   0        0        0      688 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/templates/pursuitlib/component/form-field.html
--rw-rw-rw-   0        0        0      193 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/templates/pursuitlib/component/form-section.html
-drwxrwxrwx   0        0        0        0 2022-12-14 14:43:14.485319 pursuitlib-django-0.2.8/pursuitlib_django/templates/pursuitlib/modal/
--rw-rw-rw-   0        0        0      770 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/templates/pursuitlib/modal/base.html
--rw-rw-rw-   0        0        0     2258 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/templates/pursuitlib/modal/form.html
-drwxrwxrwx   0        0        0        0 2022-12-14 14:43:14.489316 pursuitlib-django-0.2.8/pursuitlib_django/templatetags/
--rw-rw-rw-   0        0        0        0 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/templatetags/__init__.py
--rw-rw-rw-   0        0        0     6432 2022-12-14 14:41:57.000000 pursuitlib-django-0.2.8/pursuitlib_django/templatetags/pursuitlib.py
--rw-rw-rw-   0        0        0       27 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/tests.py
--rw-rw-rw-   0        0        0     1242 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/utils.py
--rw-rw-rw-   0        0        0       27 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/views.py
--rw-rw-rw-   0        0        0     2669 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pursuitlib_django/widgets.py
-drwxrwxrwx   0        0        0        0 2022-12-14 14:43:13.985135 pursuitlib-django-0.2.8/pursuitlib_django.egg-info/
--rw-rw-rw-   0        0        0     1518 2022-12-14 14:43:13.000000 pursuitlib-django-0.2.8/pursuitlib_django.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2381 2022-12-14 14:43:13.000000 pursuitlib-django-0.2.8/pursuitlib_django.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-14 14:43:13.000000 pursuitlib-django-0.2.8/pursuitlib_django.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2022-12-14 14:43:13.000000 pursuitlib-django-0.2.8/pursuitlib_django.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2022-12-14 14:43:13.000000 pursuitlib-django-0.2.8/pursuitlib_django.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      177 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-12-14 14:43:14.492316 pursuitlib-django-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0     1100 2022-12-14 14:42:13.000000 pursuitlib-django-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-18 20:00:28.359223 pursuitlib-django-0.2.9/
+-rw-rw-rw-   0        0        0     1518 2023-03-18 20:00:28.358221 pursuitlib-django-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1100 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/README.md
+drwxrwxrwx   0        0        0        0 2023-03-18 20:00:27.655985 pursuitlib-django-0.2.9/pursuitlib_django/
+-rw-rw-rw-   0        0        0        0 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pursuitlib_django/__init__.py
+-rw-rw-rw-   0        0        0       30 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pursuitlib_django/admin.py
+-rw-rw-rw-   0        0        0      165 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pursuitlib_django/apps.py
+-rw-rw-rw-   0        0        0     1458 2023-03-18 19:17:41.000000 pursuitlib-django-0.2.9/pursuitlib_django/email.py
+-rw-rw-rw-   0        0        0      665 2022-12-06 23:37:10.000000 pursuitlib-django-0.2.9/pursuitlib_django/errors.py
+-rw-rw-rw-   0        0        0     4405 2023-03-18 19:57:23.000000 pursuitlib-django-0.2.9/pursuitlib_django/forms.py
+-rw-rw-rw-   0        0        0      228 2023-03-18 19:04:15.000000 pursuitlib-django-0.2.9/pursuitlib_django/gravatar.py
+drwxrwxrwx   0        0        0        0 2023-03-18 20:00:27.581639 pursuitlib-django-0.2.9/pursuitlib_django/locale/
+drwxrwxrwx   0        0        0        0 2023-03-18 20:00:27.581639 pursuitlib-django-0.2.9/pursuitlib_django/locale/fr/
+drwxrwxrwx   0        0        0        0 2023-03-18 20:00:27.713986 pursuitlib-django-0.2.9/pursuitlib_django/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     5401 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pursuitlib_django/locale/fr/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-03-18 20:00:27.715985 pursuitlib-django-0.2.9/pursuitlib_django/migrations/
+-rw-rw-rw-   0        0        0        0 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pursuitlib_django/migrations/__init__.py
+-rw-rw-rw-   0        0        0      993 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pursuitlib_django/models.py
+-rw-rw-rw-   0        0        0      754 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pursuitlib_django/signals.py
+drwxrwxrwx   0        0        0        0 2023-03-18 20:00:27.588639 pursuitlib-django-0.2.9/pursuitlib_django/static/
+drwxrwxrwx   0        0        0        0 2023-03-18 20:00:27.888028 pursuitlib-django-0.2.9/pursuitlib_django/static/css/
+-rw-rw-rw-   0        0        0    59309 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pursuitlib_django/static/css/fa.min.css
+-rw-rw-rw-   0        0        0      247 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pursuitlib_django/static/css/pursuitlib-admin.css
+-rw-rw-rw-   0        0        0     1424 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pursuitlib_django/static/css/pursuitlib.css
+-rw-rw-rw-   0        0        0    22198 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pursuitlib_django/static/css/select2-bootstrap-5-theme.min.css
+-rw-rw-rw-   0        0        0    16265 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pursuitlib_django/static/css/select2.min.css
+drwxrwxrwx   0        0        0        0 2023-03-18 20:00:28.074113 pursuitlib-django-0.2.9/pursuitlib_django/static/js/
+-rw-rw-rw-   0        0        0    78135 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pursuitlib_django/static/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0        0        0   331017 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pursuitlib_django/static/js/bootstrap.bundle.min.js.map
+drwxrwxrwx   0        0        0        0 2023-03-18 20:00:27.587642 pursuitlib-django-0.2.9/pursuitlib_django/static/js/i18n/
+drwxrwxrwx   0        0        0        0 2023-03-18 20:00:28.092112 pursuitlib-django-0.2.9/pursuitlib_django/static/js/i18n/select2/
+-rw-rw-rw-   0        0        0      983 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pursuitlib_django/static/js/i18n/select2/fr.js
+-rw-rw-rw-   0        0        0    89503 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pursuitlib_django/static/js/jquery-3.6.0.min.js
+-rw-rw-rw-   0        0        0      478 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pursuitlib_django/static/js/pursuitlib-collapseToggle.js
+-rw-rw-rw-   0        0        0       85 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pursuitlib_django/static/js/pursuitlib-tooltips.js
+-rw-rw-rw-   0        0        0    76776 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pursuitlib_django/static/js/select2.full.min.js
+drwxrwxrwx   0        0        0        0 2023-03-18 20:00:28.307217 pursuitlib-django-0.2.9/pursuitlib_django/static/webfonts/
+-rw-rw-rw-   0        0        0   134294 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pursuitlib_django/static/webfonts/fa-brands-400.eot
+-rw-rw-rw-   0        0        0   751644 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pursuitlib_django/static/webfonts/fa-brands-400.svg
+-rw-rw-rw-   0        0        0   133988 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pursuitlib_django/static/webfonts/fa-brands-400.ttf
+-rw-rw-rw-   0        0        0    89988 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pursuitlib_django/static/webfonts/fa-brands-400.woff
+-rw-rw-rw-   0        0        0    76736 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pursuitlib_django/static/webfonts/fa-brands-400.woff2
+-rw-rw-rw-   0        0        0    34034 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pursuitlib_django/static/webfonts/fa-regular-400.eot
+-rw-rw-rw-   0        0        0   145515 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pursuitlib_django/static/webfonts/fa-regular-400.svg
+-rw-rw-rw-   0        0        0    33736 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pursuitlib_django/static/webfonts/fa-regular-400.ttf
+-rw-rw-rw-   0        0        0    16276 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pursuitlib_django/static/webfonts/fa-regular-400.woff
+-rw-rw-rw-   0        0        0    13224 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pursuitlib_django/static/webfonts/fa-regular-400.woff2
+-rw-rw-rw-   0        0        0   203030 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pursuitlib_django/static/webfonts/fa-solid-900.eot
+-rw-rw-rw-   0        0        0   924025 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pursuitlib_django/static/webfonts/fa-solid-900.svg
+-rw-rw-rw-   0        0        0   202744 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pursuitlib_django/static/webfonts/fa-solid-900.ttf
+-rw-rw-rw-   0        0        0   101648 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pursuitlib_django/static/webfonts/fa-solid-900.woff
+-rw-rw-rw-   0        0        0    78268 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pursuitlib_django/static/webfonts/fa-solid-900.woff2
+drwxrwxrwx   0        0        0        0 2023-03-18 20:00:27.591638 pursuitlib-django-0.2.9/pursuitlib_django/templates/
+drwxrwxrwx   0        0        0        0 2023-03-18 20:00:27.593639 pursuitlib-django-0.2.9/pursuitlib_django/templates/pursuitlib/
+drwxrwxrwx   0        0        0        0 2023-03-18 20:00:28.324267 pursuitlib-django-0.2.9/pursuitlib_django/templates/pursuitlib/component/
+-rw-rw-rw-   0        0        0      688 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pursuitlib_django/templates/pursuitlib/component/form-field.html
+-rw-rw-rw-   0        0        0      193 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pursuitlib_django/templates/pursuitlib/component/form-section.html
+drwxrwxrwx   0        0        0        0 2023-03-18 20:00:28.343221 pursuitlib-django-0.2.9/pursuitlib_django/templates/pursuitlib/modal/
+-rw-rw-rw-   0        0        0      770 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pursuitlib_django/templates/pursuitlib/modal/base.html
+-rw-rw-rw-   0        0        0     2258 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pursuitlib_django/templates/pursuitlib/modal/form.html
+drwxrwxrwx   0        0        0        0 2023-03-18 20:00:28.356220 pursuitlib-django-0.2.9/pursuitlib_django/templatetags/
+-rw-rw-rw-   0        0        0        0 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pursuitlib_django/templatetags/__init__.py
+-rw-rw-rw-   0        0        0     6432 2022-12-14 14:41:57.000000 pursuitlib-django-0.2.9/pursuitlib_django/templatetags/pursuitlib.py
+-rw-rw-rw-   0        0        0       27 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pursuitlib_django/tests.py
+-rw-rw-rw-   0        0        0     1242 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pursuitlib_django/utils.py
+-rw-rw-rw-   0        0        0       27 2023-03-18 19:57:06.000000 pursuitlib-django-0.2.9/pursuitlib_django/views.py
+-rw-rw-rw-   0        0        0     2669 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pursuitlib_django/widgets.py
+drwxrwxrwx   0        0        0        0 2023-03-18 20:00:27.699986 pursuitlib-django-0.2.9/pursuitlib_django.egg-info/
+-rw-rw-rw-   0        0        0     1518 2023-03-18 20:00:27.000000 pursuitlib-django-0.2.9/pursuitlib_django.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2410 2023-03-18 20:00:27.000000 pursuitlib-django-0.2.9/pursuitlib_django.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-18 20:00:27.000000 pursuitlib-django-0.2.9/pursuitlib_django.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-03-18 20:00:27.000000 pursuitlib-django-0.2.9/pursuitlib_django.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-03-18 20:00:27.000000 pursuitlib-django-0.2.9/pursuitlib_django.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      177 2022-12-04 22:52:50.000000 pursuitlib-django-0.2.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-03-18 20:00:28.359223 pursuitlib-django-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1100 2023-03-18 19:58:22.000000 pursuitlib-django-0.2.9/setup.py
```

### Comparing `pursuitlib-django-0.2.8/PKG-INFO` & `pursuitlib-django-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pursuitlib-django
-Version: 0.2.8
+Version: 0.2.9
 Summary: Provides utility functions for Django
 Home-page: https://gitlab.com/frPursuit/pursuitlib-python
 Author: Pursuit
 Author-email: fr.pursuit@gmail.com
 License: All rights reserved
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `pursuitlib-django-0.2.8/README.md` & `pursuitlib-django-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.2.8/pursuitlib_django/errors.py` & `pursuitlib-django-0.2.9/pursuitlib_django/errors.py`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.2.8/pursuitlib_django/forms.py` & `pursuitlib-django-0.2.9/pursuitlib_django/forms.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import List, Optional, Dict
 
 import django.forms as dforms
 from django.contrib import messages
 from django.forms import BoundField
+from django.forms.utils import ErrorDict, ErrorList
 from django.forms.widgets import CheckboxInput, TextInput, Select
 from django.http import HttpRequest
 from django.utils.safestring import SafeText
 from django_select2.forms import Select2Mixin
 from pursuitlib.utils import is_null_or_empty, get_oneline_string
 
 DEFAULT_LIST_HTML = "<ul><li>&nbsp;</li></ul>"
@@ -66,14 +67,15 @@
                 widget.attrs["class"] = "form-control"
 
             if isinstance(widget, Select2Mixin):
                 # noinspection PyUnresolvedReferences
                 widget.attrs["data-placeholder"] = self.get_field_placeholder(field)
             else: widget.attrs["placeholder"] = self.get_field_placeholder(field)
 
+    # noinspection PyUnresolvedReferences
     def full_clean(self):
         super().full_clean()
         for field in self.get_text_list_fields():
             if get_oneline_string(self.cleaned_data[field]) == DEFAULT_LIST_HTML:
                 self.cleaned_data[field] = ""
                 if hasattr(self.instance, field):
                     setattr(self.instance, field, "")
@@ -114,10 +116,13 @@
 
 
 class ModelForm(Form, dforms.ModelForm):
     pass
 
 
 def display_form_errors(request: HttpRequest, form: Form):
-    errors = form.errors
-    for field in errors:
-        messages.add_message(request, messages.ERROR, errors[field].as_text()[2:].replace("* ", ""))
+    errors: ErrorDict = form.errors
+    for key, value in errors.items():
+        field_name = form[key].label
+        elist: ErrorList = value
+        elist_txt = "<br />".join([str(e) for e in elist])
+        messages.error(request, SafeText(f"<strong>{field_name}</strong><br />{elist_txt}"))
```

### Comparing `pursuitlib-django-0.2.8/pursuitlib_django/locale/fr/LC_MESSAGES/django.po` & `pursuitlib-django-0.2.9/pursuitlib_django/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.2.8/pursuitlib_django/models.py` & `pursuitlib-django-0.2.9/pursuitlib_django/models.py`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.2.8/pursuitlib_django/signals.py` & `pursuitlib-django-0.2.9/pursuitlib_django/signals.py`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.2.8/pursuitlib_django/static/css/fa.min.css` & `pursuitlib-django-0.2.9/pursuitlib_django/static/css/fa.min.css`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.2.8/pursuitlib_django/static/css/pursuitlib.css` & `pursuitlib-django-0.2.9/pursuitlib_django/static/css/pursuitlib.css`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.2.8/pursuitlib_django/static/css/select2-bootstrap-5-theme.min.css` & `pursuitlib-django-0.2.9/pursuitlib_django/static/css/select2-bootstrap-5-theme.min.css`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.2.8/pursuitlib_django/static/css/select2.min.css` & `pursuitlib-django-0.2.9/pursuitlib_django/static/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.2.8/pursuitlib_django/static/js/bootstrap.bundle.min.js` & `pursuitlib-django-0.2.9/pursuitlib_django/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.2.8/pursuitlib_django/static/js/bootstrap.bundle.min.js.map` & `pursuitlib-django-0.2.9/pursuitlib_django/static/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.2.8/pursuitlib_django/static/js/i18n/select2/fr.js` & `pursuitlib-django-0.2.9/pursuitlib_django/static/js/i18n/select2/fr.js`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.2.8/pursuitlib_django/static/js/jquery-3.6.0.min.js` & `pursuitlib-django-0.2.9/pursuitlib_django/static/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.2.8/pursuitlib_django/static/js/select2.full.min.js` & `pursuitlib-django-0.2.9/pursuitlib_django/static/js/select2.full.min.js`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.2.8/pursuitlib_django/static/webfonts/fa-brands-400.eot` & `pursuitlib-django-0.2.9/pursuitlib_django/static/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.2.8/pursuitlib_django/static/webfonts/fa-brands-400.svg` & `pursuitlib-django-0.2.9/pursuitlib_django/static/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.2.8/pursuitlib_django/static/webfonts/fa-brands-400.ttf` & `pursuitlib-django-0.2.9/pursuitlib_django/static/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.2.8/pursuitlib_django/static/webfonts/fa-brands-400.woff` & `pursuitlib-django-0.2.9/pursuitlib_django/static/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.2.8/pursuitlib_django/static/webfonts/fa-brands-400.woff2` & `pursuitlib-django-0.2.9/pursuitlib_django/static/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.2.8/pursuitlib_django/static/webfonts/fa-regular-400.eot` & `pursuitlib-django-0.2.9/pursuitlib_django/static/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.2.8/pursuitlib_django/static/webfonts/fa-regular-400.svg` & `pursuitlib-django-0.2.9/pursuitlib_django/static/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.2.8/pursuitlib_django/static/webfonts/fa-regular-400.ttf` & `pursuitlib-django-0.2.9/pursuitlib_django/static/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.2.8/pursuitlib_django/static/webfonts/fa-regular-400.woff` & `pursuitlib-django-0.2.9/pursuitlib_django/static/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.2.8/pursuitlib_django/static/webfonts/fa-regular-400.woff2` & `pursuitlib-django-0.2.9/pursuitlib_django/static/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.2.8/pursuitlib_django/static/webfonts/fa-solid-900.eot` & `pursuitlib-django-0.2.9/pursuitlib_django/static/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.2.8/pursuitlib_django/static/webfonts/fa-solid-900.svg` & `pursuitlib-django-0.2.9/pursuitlib_django/static/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.2.8/pursuitlib_django/static/webfonts/fa-solid-900.ttf` & `pursuitlib-django-0.2.9/pursuitlib_django/static/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.2.8/pursuitlib_django/static/webfonts/fa-solid-900.woff` & `pursuitlib-django-0.2.9/pursuitlib_django/static/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.2.8/pursuitlib_django/static/webfonts/fa-solid-900.woff2` & `pursuitlib-django-0.2.9/pursuitlib_django/static/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.2.8/pursuitlib_django/templates/pursuitlib/component/form-field.html` & `pursuitlib-django-0.2.9/pursuitlib_django/templates/pursuitlib/component/form-field.html`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.2.8/pursuitlib_django/templates/pursuitlib/modal/base.html` & `pursuitlib-django-0.2.9/pursuitlib_django/templates/pursuitlib/modal/base.html`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.2.8/pursuitlib_django/templates/pursuitlib/modal/form.html` & `pursuitlib-django-0.2.9/pursuitlib_django/templates/pursuitlib/modal/form.html`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.2.8/pursuitlib_django/templatetags/pursuitlib.py` & `pursuitlib-django-0.2.9/pursuitlib_django/templatetags/pursuitlib.py`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.2.8/pursuitlib_django/utils.py` & `pursuitlib-django-0.2.9/pursuitlib_django/utils.py`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.2.8/pursuitlib_django/widgets.py` & `pursuitlib-django-0.2.9/pursuitlib_django/widgets.py`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.2.8/pursuitlib_django.egg-info/PKG-INFO` & `pursuitlib-django-0.2.9/pursuitlib_django.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pursuitlib-django
-Version: 0.2.8
+Version: 0.2.9
 Summary: Provides utility functions for Django
 Home-page: https://gitlab.com/frPursuit/pursuitlib-python
 Author: Pursuit
 Author-email: fr.pursuit@gmail.com
 License: All rights reserved
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `pursuitlib-django-0.2.8/pursuitlib_django.egg-info/SOURCES.txt` & `pursuitlib-django-0.2.9/pursuitlib_django.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 README.md
 pyproject.toml
 setup.py
 pursuitlib_django/__init__.py
 pursuitlib_django/admin.py
 pursuitlib_django/apps.py
+pursuitlib_django/email.py
 pursuitlib_django/errors.py
 pursuitlib_django/forms.py
-pursuitlib_django/mailto.py
+pursuitlib_django/gravatar.py
 pursuitlib_django/models.py
 pursuitlib_django/signals.py
 pursuitlib_django/tests.py
 pursuitlib_django/utils.py
 pursuitlib_django/views.py
 pursuitlib_django/widgets.py
 pursuitlib_django.egg-info/PKG-INFO
```

### Comparing `pursuitlib-django-0.2.8/setup.py` & `pursuitlib-django-0.2.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 directory = Path(__file__).parent
 
 setup(
     name='pursuitlib-django',
-    version='0.2.8',
+    version='0.2.9',
     packages=find_packages(),
     include_package_data=True,
     package_data={'pursuitlib_django': ['locale/*/*/*',
                                         'static/*/*', 'static/*/*/*', 'static/*/*/*/*',
                                         'templates/pursuitlib/*', 'templates/pursuitlib/*/*']},
     install_requires=[
         'pursuitlib',
```

