# Comparing `tmp/pursuitlib-django-0.3.0.tar.gz` & `tmp/pursuitlib-django-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pursuitlib-django-0.3.0.tar", last modified: Sat Mar 25 20:14:03 2023, max compression
+gzip compressed data, was "pursuitlib-django-0.3.1.tar", last modified: Mon Apr 24 17:59:08 2023, max compression
```

## Comparing `pursuitlib-django-0.3.0.tar` & `pursuitlib-django-0.3.1.tar`

### file list

```diff
@@ -1,77 +1,81 @@
-drwxrwxrwx   0        0        0        0 2023-03-25 20:14:03.501021 pursuitlib-django-0.3.0/
--rw-rw-rw-   0        0        0     1518 2023-03-25 20:14:03.500021 pursuitlib-django-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1100 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-25 20:14:02.948755 pursuitlib-django-0.3.0/pursuitlib_django/
--rw-rw-rw-   0        0        0        0 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pursuitlib_django/__init__.py
--rw-rw-rw-   0        0        0       30 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pursuitlib_django/admin.py
--rw-rw-rw-   0        0        0      165 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pursuitlib_django/apps.py
--rw-rw-rw-   0        0        0      808 2023-03-25 20:03:53.000000 pursuitlib-django-0.3.0/pursuitlib_django/decorators.py
--rw-rw-rw-   0        0        0     1458 2023-03-18 19:17:41.000000 pursuitlib-django-0.3.0/pursuitlib_django/email.py
--rw-rw-rw-   0        0        0      665 2022-12-06 23:37:10.000000 pursuitlib-django-0.3.0/pursuitlib_django/errors.py
--rw-rw-rw-   0        0        0     5415 2023-03-25 20:05:12.000000 pursuitlib-django-0.3.0/pursuitlib_django/forms.py
--rw-rw-rw-   0        0        0      228 2023-03-18 19:04:15.000000 pursuitlib-django-0.3.0/pursuitlib_django/gravatar.py
-drwxrwxrwx   0        0        0        0 2023-03-25 20:14:02.903714 pursuitlib-django-0.3.0/pursuitlib_django/locale/
-drwxrwxrwx   0        0        0        0 2023-03-25 20:14:02.905753 pursuitlib-django-0.3.0/pursuitlib_django/locale/fr/
-drwxrwxrwx   0        0        0        0 2023-03-25 20:14:02.987760 pursuitlib-django-0.3.0/pursuitlib_django/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0        0        0     5401 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pursuitlib_django/locale/fr/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-03-25 20:14:02.989774 pursuitlib-django-0.3.0/pursuitlib_django/migrations/
--rw-rw-rw-   0        0        0        0 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pursuitlib_django/migrations/__init__.py
--rw-rw-rw-   0        0        0      993 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pursuitlib_django/models.py
--rw-rw-rw-   0        0        0      754 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pursuitlib_django/signals.py
-drwxrwxrwx   0        0        0        0 2023-03-25 20:14:02.910756 pursuitlib-django-0.3.0/pursuitlib_django/static/
-drwxrwxrwx   0        0        0        0 2023-03-25 20:14:03.080430 pursuitlib-django-0.3.0/pursuitlib_django/static/css/
--rw-rw-rw-   0        0        0    59309 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pursuitlib_django/static/css/fa.min.css
--rw-rw-rw-   0        0        0      247 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pursuitlib_django/static/css/pursuitlib-admin.css
--rw-rw-rw-   0        0        0     1424 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pursuitlib_django/static/css/pursuitlib.css
--rw-rw-rw-   0        0        0    22198 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pursuitlib_django/static/css/select2-bootstrap-5-theme.min.css
--rw-rw-rw-   0        0        0    16265 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pursuitlib_django/static/css/select2.min.css
-drwxrwxrwx   0        0        0        0 2023-03-25 20:14:03.221460 pursuitlib-django-0.3.0/pursuitlib_django/static/js/
--rw-rw-rw-   0        0        0    78135 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pursuitlib_django/static/js/bootstrap.bundle.min.js
--rw-rw-rw-   0        0        0   331017 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pursuitlib_django/static/js/bootstrap.bundle.min.js.map
-drwxrwxrwx   0        0        0        0 2023-03-25 20:14:02.910756 pursuitlib-django-0.3.0/pursuitlib_django/static/js/i18n/
-drwxrwxrwx   0        0        0        0 2023-03-25 20:14:03.233439 pursuitlib-django-0.3.0/pursuitlib_django/static/js/i18n/select2/
--rw-rw-rw-   0        0        0      983 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pursuitlib_django/static/js/i18n/select2/fr.js
--rw-rw-rw-   0        0        0    89503 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pursuitlib_django/static/js/jquery-3.6.0.min.js
--rw-rw-rw-   0        0        0      478 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pursuitlib_django/static/js/pursuitlib-collapseToggle.js
--rw-rw-rw-   0        0        0       85 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pursuitlib_django/static/js/pursuitlib-tooltips.js
--rw-rw-rw-   0        0        0    76776 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pursuitlib_django/static/js/select2.full.min.js
-drwxrwxrwx   0        0        0        0 2023-03-25 20:14:03.449027 pursuitlib-django-0.3.0/pursuitlib_django/static/webfonts/
--rw-rw-rw-   0        0        0   134294 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pursuitlib_django/static/webfonts/fa-brands-400.eot
--rw-rw-rw-   0        0        0   751644 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pursuitlib_django/static/webfonts/fa-brands-400.svg
--rw-rw-rw-   0        0        0   133988 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pursuitlib_django/static/webfonts/fa-brands-400.ttf
--rw-rw-rw-   0        0        0    89988 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pursuitlib_django/static/webfonts/fa-brands-400.woff
--rw-rw-rw-   0        0        0    76736 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pursuitlib_django/static/webfonts/fa-brands-400.woff2
--rw-rw-rw-   0        0        0    34034 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pursuitlib_django/static/webfonts/fa-regular-400.eot
--rw-rw-rw-   0        0        0   145515 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pursuitlib_django/static/webfonts/fa-regular-400.svg
--rw-rw-rw-   0        0        0    33736 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pursuitlib_django/static/webfonts/fa-regular-400.ttf
--rw-rw-rw-   0        0        0    16276 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pursuitlib_django/static/webfonts/fa-regular-400.woff
--rw-rw-rw-   0        0        0    13224 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pursuitlib_django/static/webfonts/fa-regular-400.woff2
--rw-rw-rw-   0        0        0   203030 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pursuitlib_django/static/webfonts/fa-solid-900.eot
--rw-rw-rw-   0        0        0   924025 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pursuitlib_django/static/webfonts/fa-solid-900.svg
--rw-rw-rw-   0        0        0   202744 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pursuitlib_django/static/webfonts/fa-solid-900.ttf
--rw-rw-rw-   0        0        0   101648 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pursuitlib_django/static/webfonts/fa-solid-900.woff
--rw-rw-rw-   0        0        0    78268 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pursuitlib_django/static/webfonts/fa-solid-900.woff2
-drwxrwxrwx   0        0        0        0 2023-03-25 20:14:02.912754 pursuitlib-django-0.3.0/pursuitlib_django/templates/
-drwxrwxrwx   0        0        0        0 2023-03-25 20:14:02.913762 pursuitlib-django-0.3.0/pursuitlib_django/templates/pursuitlib/
-drwxrwxrwx   0        0        0        0 2023-03-25 20:14:03.466018 pursuitlib-django-0.3.0/pursuitlib_django/templates/pursuitlib/component/
--rw-rw-rw-   0        0        0      688 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pursuitlib_django/templates/pursuitlib/component/form-field.html
--rw-rw-rw-   0        0        0      193 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pursuitlib_django/templates/pursuitlib/component/form-section.html
-drwxrwxrwx   0        0        0        0 2023-03-25 20:14:03.483019 pursuitlib-django-0.3.0/pursuitlib_django/templates/pursuitlib/modal/
--rw-rw-rw-   0        0        0      770 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pursuitlib_django/templates/pursuitlib/modal/base.html
--rw-rw-rw-   0        0        0     2258 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pursuitlib_django/templates/pursuitlib/modal/form.html
-drwxrwxrwx   0        0        0        0 2023-03-25 20:14:03.497018 pursuitlib-django-0.3.0/pursuitlib_django/templatetags/
--rw-rw-rw-   0        0        0        0 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pursuitlib_django/templatetags/__init__.py
--rw-rw-rw-   0        0        0     6432 2022-12-14 14:41:57.000000 pursuitlib-django-0.3.0/pursuitlib_django/templatetags/pursuitlib.py
--rw-rw-rw-   0        0        0       27 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pursuitlib_django/tests.py
--rw-rw-rw-   0        0        0     1242 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pursuitlib_django/utils.py
--rw-rw-rw-   0        0        0      205 2023-03-25 20:04:20.000000 pursuitlib-django-0.3.0/pursuitlib_django/views.py
--rw-rw-rw-   0        0        0     2669 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pursuitlib_django/widgets.py
-drwxrwxrwx   0        0        0        0 2023-03-25 20:14:02.977756 pursuitlib-django-0.3.0/pursuitlib_django.egg-info/
--rw-rw-rw-   0        0        0     1518 2023-03-25 20:14:02.000000 pursuitlib-django-0.3.0/pursuitlib_django.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2442 2023-03-25 20:14:02.000000 pursuitlib-django-0.3.0/pursuitlib_django.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-25 20:14:02.000000 pursuitlib-django-0.3.0/pursuitlib_django.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-03-25 20:14:02.000000 pursuitlib-django-0.3.0/pursuitlib_django.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-03-25 20:14:02.000000 pursuitlib-django-0.3.0/pursuitlib_django.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      177 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-25 20:14:03.501021 pursuitlib-django-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1100 2023-03-25 20:09:53.000000 pursuitlib-django-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 17:59:08.692482 pursuitlib-django-0.3.1/
+-rw-rw-rw-   0        0        0     1558 2023-04-24 17:59:08.691498 pursuitlib-django-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1140 2023-04-24 17:56:57.000000 pursuitlib-django-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 17:59:08.276528 pursuitlib-django-0.3.1/pursuitlib_django/
+-rw-rw-rw-   0        0        0        0 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.1/pursuitlib_django/__init__.py
+-rw-rw-rw-   0        0        0      877 2023-04-08 12:22:20.000000 pursuitlib-django-0.3.1/pursuitlib_django/admin.py
+drwxrwxrwx   0        0        0        0 2023-04-24 17:59:08.314481 pursuitlib-django-0.3.1/pursuitlib_django/api/
+-rw-rw-rw-   0        0        0        0 2023-04-14 18:21:55.000000 pursuitlib-django-0.3.1/pursuitlib_django/api/__init__.py
+-rw-rw-rw-   0        0        0     1236 2023-04-14 18:50:53.000000 pursuitlib-django-0.3.1/pursuitlib_django/api/decorators.py
+-rw-rw-rw-   0        0        0      479 2023-04-09 20:14:16.000000 pursuitlib-django-0.3.1/pursuitlib_django/api/utils.py
+-rw-rw-rw-   0        0        0      165 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.1/pursuitlib_django/apps.py
+-rw-rw-rw-   0        0        0     2667 2023-04-14 18:40:04.000000 pursuitlib-django-0.3.1/pursuitlib_django/decorators.py
+-rw-rw-rw-   0        0        0     1458 2023-03-18 19:17:41.000000 pursuitlib-django-0.3.1/pursuitlib_django/email.py
+-rw-rw-rw-   0        0        0     1129 2023-04-14 18:22:36.000000 pursuitlib-django-0.3.1/pursuitlib_django/errors.py
+-rw-rw-rw-   0        0        0     9808 2023-04-23 11:58:32.000000 pursuitlib-django-0.3.1/pursuitlib_django/forms.py
+-rw-rw-rw-   0        0        0      228 2023-03-18 19:04:15.000000 pursuitlib-django-0.3.1/pursuitlib_django/gravatar.py
+drwxrwxrwx   0        0        0        0 2023-04-24 17:59:08.162484 pursuitlib-django-0.3.1/pursuitlib_django/locale/
+drwxrwxrwx   0        0        0        0 2023-04-24 17:59:08.162484 pursuitlib-django-0.3.1/pursuitlib_django/locale/fr/
+drwxrwxrwx   0        0        0        0 2023-04-24 17:59:08.322483 pursuitlib-django-0.3.1/pursuitlib_django/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     5401 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.1/pursuitlib_django/locale/fr/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-24 17:59:08.325525 pursuitlib-django-0.3.1/pursuitlib_django/migrations/
+-rw-rw-rw-   0        0        0        0 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.1/pursuitlib_django/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2938 2023-04-24 17:56:57.000000 pursuitlib-django-0.3.1/pursuitlib_django/models.py
+-rw-rw-rw-   0        0        0     1417 2023-04-02 20:08:27.000000 pursuitlib-django-0.3.1/pursuitlib_django/pagination.py
+-rw-rw-rw-   0        0        0      754 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.1/pursuitlib_django/signals.py
+drwxrwxrwx   0        0        0        0 2023-04-24 17:59:08.169483 pursuitlib-django-0.3.1/pursuitlib_django/static/
+drwxrwxrwx   0        0        0        0 2023-04-24 17:59:08.353483 pursuitlib-django-0.3.1/pursuitlib_django/static/css/
+-rw-rw-rw-   0        0        0    59309 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.1/pursuitlib_django/static/css/fa.min.css
+-rw-rw-rw-   0        0        0      247 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.1/pursuitlib_django/static/css/pursuitlib-admin.css
+-rw-rw-rw-   0        0        0     1426 2023-04-15 16:36:54.000000 pursuitlib-django-0.3.1/pursuitlib_django/static/css/pursuitlib.css
+-rw-rw-rw-   0        0        0    16265 2023-04-15 16:45:53.000000 pursuitlib-django-0.3.1/pursuitlib_django/static/css/select2.min.css
+drwxrwxrwx   0        0        0        0 2023-04-24 17:59:08.443483 pursuitlib-django-0.3.1/pursuitlib_django/static/js/
+-rw-rw-rw-   0        0        0    78135 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.1/pursuitlib_django/static/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0        0        0   331017 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.1/pursuitlib_django/static/js/bootstrap.bundle.min.js.map
+drwxrwxrwx   0        0        0        0 2023-04-24 17:59:08.169483 pursuitlib-django-0.3.1/pursuitlib_django/static/js/i18n/
+drwxrwxrwx   0        0        0        0 2023-04-24 17:59:08.456482 pursuitlib-django-0.3.1/pursuitlib_django/static/js/i18n/select2/
+-rw-rw-rw-   0        0        0      981 2021-01-23 04:36:25.000000 pursuitlib-django-0.3.1/pursuitlib_django/static/js/i18n/select2/fr.js
+-rw-rw-rw-   0        0        0    89503 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.1/pursuitlib_django/static/js/jquery-3.6.0.min.js
+-rw-rw-rw-   0        0        0     4056 2023-04-15 22:40:42.000000 pursuitlib-django-0.3.1/pursuitlib_django/static/js/pursuitlib.js
+-rw-rw-rw-   0        0        0    76776 2023-04-15 16:46:58.000000 pursuitlib-django-0.3.1/pursuitlib_django/static/js/select2.full.min.js
+drwxrwxrwx   0        0        0        0 2023-04-24 17:59:08.626480 pursuitlib-django-0.3.1/pursuitlib_django/static/webfonts/
+-rw-rw-rw-   0        0        0   134294 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.1/pursuitlib_django/static/webfonts/fa-brands-400.eot
+-rw-rw-rw-   0        0        0   751644 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.1/pursuitlib_django/static/webfonts/fa-brands-400.svg
+-rw-rw-rw-   0        0        0   133988 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.1/pursuitlib_django/static/webfonts/fa-brands-400.ttf
+-rw-rw-rw-   0        0        0    89988 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.1/pursuitlib_django/static/webfonts/fa-brands-400.woff
+-rw-rw-rw-   0        0        0    76736 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.1/pursuitlib_django/static/webfonts/fa-brands-400.woff2
+-rw-rw-rw-   0        0        0    34034 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.1/pursuitlib_django/static/webfonts/fa-regular-400.eot
+-rw-rw-rw-   0        0        0   145515 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.1/pursuitlib_django/static/webfonts/fa-regular-400.svg
+-rw-rw-rw-   0        0        0    33736 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.1/pursuitlib_django/static/webfonts/fa-regular-400.ttf
+-rw-rw-rw-   0        0        0    16276 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.1/pursuitlib_django/static/webfonts/fa-regular-400.woff
+-rw-rw-rw-   0        0        0    13224 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.1/pursuitlib_django/static/webfonts/fa-regular-400.woff2
+-rw-rw-rw-   0        0        0   203030 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.1/pursuitlib_django/static/webfonts/fa-solid-900.eot
+-rw-rw-rw-   0        0        0   924025 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.1/pursuitlib_django/static/webfonts/fa-solid-900.svg
+-rw-rw-rw-   0        0        0   202744 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.1/pursuitlib_django/static/webfonts/fa-solid-900.ttf
+-rw-rw-rw-   0        0        0   101648 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.1/pursuitlib_django/static/webfonts/fa-solid-900.woff
+-rw-rw-rw-   0        0        0    78268 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.1/pursuitlib_django/static/webfonts/fa-solid-900.woff2
+drwxrwxrwx   0        0        0        0 2023-04-24 17:59:08.171496 pursuitlib-django-0.3.1/pursuitlib_django/templates/
+drwxrwxrwx   0        0        0        0 2023-04-24 17:59:08.173515 pursuitlib-django-0.3.1/pursuitlib_django/templates/pursuitlib/
+drwxrwxrwx   0        0        0        0 2023-04-24 17:59:08.652482 pursuitlib-django-0.3.1/pursuitlib_django/templates/pursuitlib/component/
+-rw-rw-rw-   0        0        0      688 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.1/pursuitlib_django/templates/pursuitlib/component/form-field.html
+-rw-rw-rw-   0        0        0      193 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.1/pursuitlib_django/templates/pursuitlib/component/form-section.html
+-rw-rw-rw-   0        0        0     2122 2023-04-02 20:08:27.000000 pursuitlib-django-0.3.1/pursuitlib_django/templates/pursuitlib/component/pagination.html
+drwxrwxrwx   0        0        0        0 2023-04-24 17:59:08.675499 pursuitlib-django-0.3.1/pursuitlib_django/templates/pursuitlib/modal/
+-rw-rw-rw-   0        0        0      770 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.1/pursuitlib_django/templates/pursuitlib/modal/base.html
+-rw-rw-rw-   0        0        0     2715 2023-04-16 15:34:58.000000 pursuitlib-django-0.3.1/pursuitlib_django/templates/pursuitlib/modal/form.html
+drwxrwxrwx   0        0        0        0 2023-04-24 17:59:08.689482 pursuitlib-django-0.3.1/pursuitlib_django/templatetags/
+-rw-rw-rw-   0        0        0        0 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.1/pursuitlib_django/templatetags/__init__.py
+-rw-rw-rw-   0        0        0     7075 2023-04-15 22:33:38.000000 pursuitlib-django-0.3.1/pursuitlib_django/templatetags/pursuitlib.py
+-rw-rw-rw-   0        0        0       27 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.1/pursuitlib_django/tests.py
+-rw-rw-rw-   0        0        0     1479 2023-04-08 13:24:03.000000 pursuitlib-django-0.3.1/pursuitlib_django/utils.py
+-rw-rw-rw-   0        0        0      983 2023-04-23 11:05:13.000000 pursuitlib-django-0.3.1/pursuitlib_django/views.py
+-rw-rw-rw-   0        0        0     2724 2023-04-15 16:44:07.000000 pursuitlib-django-0.3.1/pursuitlib_django/widgets.py
+drwxrwxrwx   0        0        0        0 2023-04-24 17:59:08.299484 pursuitlib-django-0.3.1/pursuitlib_django.egg-info/
+-rw-rw-rw-   0        0        0     1558 2023-04-24 17:59:08.000000 pursuitlib-django-0.3.1/pursuitlib_django.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2511 2023-04-24 17:59:08.000000 pursuitlib-django-0.3.1/pursuitlib_django.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 17:59:08.000000 pursuitlib-django-0.3.1/pursuitlib_django.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-04-24 17:59:08.000000 pursuitlib-django-0.3.1/pursuitlib_django.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-24 17:59:08.000000 pursuitlib-django-0.3.1/pursuitlib_django.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      177 2022-12-04 22:52:50.000000 pursuitlib-django-0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-24 17:59:08.693493 pursuitlib-django-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1100 2023-04-24 17:56:57.000000 pursuitlib-django-0.3.1/setup.py
```

### Comparing `pursuitlib-django-0.3.0/PKG-INFO` & `pursuitlib-django-0.3.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pursuitlib-django
-Version: 0.3.0
+Version: 0.3.1
 Summary: Provides utility functions for Django
 Home-page: https://gitlab.com/frPursuit/pursuitlib-python
 Author: Pursuit
 Author-email: fr.pursuit@gmail.com
 License: All rights reserved
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Pursuit Library - Django
 
 This package provides utility functions and classes for Django (and Select2).
 
 It also contains static files for:
@@ -23,14 +23,16 @@
 - [FontAwesome](https://fontawesome.com/) 5.15.4
 
 ## Configuration
 
 The following values should be added to the Django configuration:
 
 ```python
+from pursuitlib.utils import get_env
+
 VERSION = "PROJECT_VERSION"
 DEV_STAGE = "PROJECT_DEV_STAGE"
 DISPLAY_VERSION = VERSION if DEV_STAGE is None else VERSION + " " + DEV_STAGE
 
 DOMAIN = get_env('PROJECTNAME_DOMAIN')
 USE_HTTPS = get_env('PROJECTNAME_USE_HTTPS').lower() == 'true'
 BASE_URL = ("https://" if USE_HTTPS else "http://") + DOMAIN
```

### Comparing `pursuitlib-django-0.3.0/README.md` & `pursuitlib-django-0.3.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 - [FontAwesome](https://fontawesome.com/) 5.15.4
 
 ## Configuration
 
 The following values should be added to the Django configuration:
 
 ```python
+from pursuitlib.utils import get_env
+
 VERSION = "PROJECT_VERSION"
 DEV_STAGE = "PROJECT_DEV_STAGE"
 DISPLAY_VERSION = VERSION if DEV_STAGE is None else VERSION + " " + DEV_STAGE
 
 DOMAIN = get_env('PROJECTNAME_DOMAIN')
 USE_HTTPS = get_env('PROJECTNAME_USE_HTTPS').lower() == 'true'
 BASE_URL = ("https://" if USE_HTTPS else "http://") + DOMAIN
```

### Comparing `pursuitlib-django-0.3.0/pursuitlib_django/email.py` & `pursuitlib-django-0.3.1/pursuitlib_django/email.py`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.3.0/pursuitlib_django/locale/fr/LC_MESSAGES/django.po` & `pursuitlib-django-0.3.1/pursuitlib_django/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.3.0/pursuitlib_django/signals.py` & `pursuitlib-django-0.3.1/pursuitlib_django/signals.py`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.3.0/pursuitlib_django/static/css/fa.min.css` & `pursuitlib-django-0.3.1/pursuitlib_django/static/css/fa.min.css`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.3.0/pursuitlib_django/static/css/pursuitlib.css` & `pursuitlib-django-0.3.1/pursuitlib_django/static/css/pursuitlib.css`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -91,8 +91,8 @@
 
 .select2-search--hide {
     display: none !important;
 }
 
 .select2-container--bootstrap-5 .select2-selection--multiple .select2-search .select2-search__field {
     height: 1.75rem;
-}
+}
```

### Comparing `pursuitlib-django-0.3.0/pursuitlib_django/static/css/select2.min.css` & `pursuitlib-django-0.3.1/pursuitlib_django/static/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.3.0/pursuitlib_django/static/js/bootstrap.bundle.min.js` & `pursuitlib-django-0.3.1/pursuitlib_django/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.3.0/pursuitlib_django/static/js/bootstrap.bundle.min.js.map` & `pursuitlib-django-0.3.1/pursuitlib_django/static/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.3.0/pursuitlib_django/static/js/i18n/select2/fr.js` & `pursuitlib-django-0.3.1/pursuitlib_django/static/js/i18n/select2/fr.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,38 +1,38 @@
-/*! Select2 4.1.0-rc.0 | https://github.com/select2/select2/blob/master/LICENSE.md */
-
-! function() {
-    if (jQuery && jQuery.fn && jQuery.fn.select2 && jQuery.fn.select2.amd) var e = jQuery.fn.select2.amd;
-    e.define("select2/i18n/fr", [], function() {
-        return {
-            errorLoading: function() {
-                return "Les résultats ne peuvent pas être chargés."
-            },
-            inputTooLong: function(e) {
-                var n = e.input.length - e.maximum;
-                return "Supprimez " + n + " caractère" + (n > 1 ? "s" : "")
-            },
-            inputTooShort: function(e) {
-                var n = e.minimum - e.input.length;
-                return "Saisissez au moins " + n + " caractère" + (n > 1 ? "s" : "")
-            },
-            loadingMore: function() {
-                return "Chargement de résultats supplémentaires…"
-            },
-            maximumSelected: function(e) {
-                return "Vous pouvez seulement sélectionner " + e.maximum + " élément" + (e.maximum > 1 ? "s" : "")
-            },
-            noResults: function() {
-                return "Aucun résultat trouvé"
-            },
-            searching: function() {
-                return "Recherche en cours…"
-            },
-            removeAllItems: function() {
-                return "Supprimer tous les éléments"
-            },
-            removeItem: function() {
-                return "Supprimer l'élément"
-            }
-        }
-    }), e.define, e.require
+/*! Select2 4.1.0-rc.0 | https://github.com/select2/select2/blob/master/LICENSE.md */
+
+! function() {
+    if (jQuery && jQuery.fn && jQuery.fn.select2 && jQuery.fn.select2.amd) var e = jQuery.fn.select2.amd;
+    e.define("select2/i18n/fr", [], function() {
+        return {
+            errorLoading: function() {
+                return "Les résultats ne peuvent pas être chargés."
+            },
+            inputTooLong: function(e) {
+                var n = e.input.length - e.maximum;
+                return "Supprimez " + n + " caractère" + (n > 1 ? "s" : "")
+            },
+            inputTooShort: function(e) {
+                var n = e.minimum - e.input.length;
+                return "Saisissez au moins " + n + " caractère" + (n > 1 ? "s" : "")
+            },
+            loadingMore: function() {
+                return "Chargement de résultats supplémentaires…"
+            },
+            maximumSelected: function(e) {
+                return "Vous pouvez seulement sélectionner " + e.maximum + " élément" + (e.maximum > 1 ? "s" : "")
+            },
+            noResults: function() {
+                return "Aucun résultat trouvé"
+            },
+            searching: function() {
+                return "Recherche en cours…"
+            },
+            removeAllItems: function() {
+                return "Supprimer tous les éléments"
+            },
+            removeItem: function() {
+                return "Supprimer l'élément"
+            }
+        }
+    }), e.define, e.require
 }();
```

### Comparing `pursuitlib-django-0.3.0/pursuitlib_django/static/js/jquery-3.6.0.min.js` & `pursuitlib-django-0.3.1/pursuitlib_django/static/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.3.0/pursuitlib_django/static/js/select2.full.min.js` & `pursuitlib-django-0.3.1/pursuitlib_django/static/js/select2.full.min.js`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.3.0/pursuitlib_django/static/webfonts/fa-brands-400.eot` & `pursuitlib-django-0.3.1/pursuitlib_django/static/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.3.0/pursuitlib_django/static/webfonts/fa-brands-400.svg` & `pursuitlib-django-0.3.1/pursuitlib_django/static/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.3.0/pursuitlib_django/static/webfonts/fa-brands-400.ttf` & `pursuitlib-django-0.3.1/pursuitlib_django/static/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.3.0/pursuitlib_django/static/webfonts/fa-brands-400.woff` & `pursuitlib-django-0.3.1/pursuitlib_django/static/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.3.0/pursuitlib_django/static/webfonts/fa-brands-400.woff2` & `pursuitlib-django-0.3.1/pursuitlib_django/static/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.3.0/pursuitlib_django/static/webfonts/fa-regular-400.eot` & `pursuitlib-django-0.3.1/pursuitlib_django/static/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.3.0/pursuitlib_django/static/webfonts/fa-regular-400.svg` & `pursuitlib-django-0.3.1/pursuitlib_django/static/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.3.0/pursuitlib_django/static/webfonts/fa-regular-400.ttf` & `pursuitlib-django-0.3.1/pursuitlib_django/static/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.3.0/pursuitlib_django/static/webfonts/fa-regular-400.woff` & `pursuitlib-django-0.3.1/pursuitlib_django/static/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.3.0/pursuitlib_django/static/webfonts/fa-regular-400.woff2` & `pursuitlib-django-0.3.1/pursuitlib_django/static/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.3.0/pursuitlib_django/static/webfonts/fa-solid-900.eot` & `pursuitlib-django-0.3.1/pursuitlib_django/static/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.3.0/pursuitlib_django/static/webfonts/fa-solid-900.svg` & `pursuitlib-django-0.3.1/pursuitlib_django/static/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.3.0/pursuitlib_django/static/webfonts/fa-solid-900.ttf` & `pursuitlib-django-0.3.1/pursuitlib_django/static/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.3.0/pursuitlib_django/static/webfonts/fa-solid-900.woff` & `pursuitlib-django-0.3.1/pursuitlib_django/static/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.3.0/pursuitlib_django/static/webfonts/fa-solid-900.woff2` & `pursuitlib-django-0.3.1/pursuitlib_django/static/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.3.0/pursuitlib_django/templates/pursuitlib/component/form-field.html` & `pursuitlib-django-0.3.1/pursuitlib_django/templates/pursuitlib/component/form-field.html`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.3.0/pursuitlib_django/templates/pursuitlib/modal/base.html` & `pursuitlib-django-0.3.1/pursuitlib_django/templates/pursuitlib/modal/base.html`

 * *Files identical despite different names*

### Comparing `pursuitlib-django-0.3.0/pursuitlib_django/templatetags/pursuitlib.py` & `pursuitlib-django-0.3.1/pursuitlib_django/templatetags/pursuitlib.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import os
-from typing import Type, List, Dict
+from typing import Type, List
 
 from django import template
 from django.conf import settings
 from django.db.models import QuerySet
 from django.db.models.fields.files import FieldFile
 from django.db.models.functions import Lower
 from django.forms.boundfield import BoundField
 from django.forms.fields import FileField
 from django.template import loader
 from django.templatetags.static import static as dstatic
 from django.utils.html import escape
 from django.utils.safestring import SafeText
-
 from pursuitlib import utils
 from pursuitlib.color import is_dark
 from pursuitlib.utils import is_null_or_empty
 
 from pursuitlib_django.forms import Form, DEFAULT_FORM_SECTION
-from pursuitlib_django.utils import get_verbose_name, get_verbose_name_plural
+from pursuitlib_django import utils
 
 # Read the Django configuration
 
 VERSION = getattr(settings, "VERSION")
 DISPLAY_VERSION = getattr(settings, "DISPLAY_VERSION", VERSION)
 BASE_URL = getattr(settings, "BASE_URL")
 MEDIA_URL = getattr(settings, "MEDIA_URL")
@@ -167,28 +166,25 @@
 @register.filter
 def typeof(obj) -> Type:
     return type(obj)
 
 
 @register.filter
 def verbose_name(obj) -> str:
-    return get_verbose_name(obj)
+    return utils.get_verbose_name(obj)
 
 
 @register.filter
 def verbose_name_plural(obj) -> str:
-    return get_verbose_name_plural(obj)
+    return utils.get_verbose_name_plural(obj)
 
 
 @register.filter
 def is_feminine(obj) -> bool:
-    try:
-        return type(obj).Gender.feminine
-    except AttributeError:
-        return False
+    return utils.is_feminine(obj)
 
 
 @register.filter
 def genderize(obj, suffix: str = "e") -> str:
     return suffix if is_feminine(obj) else ""
 
 
@@ -207,14 +203,22 @@
     return "#FFFFFF" if is_dark(color) else "#000000"
 
 
 @register.filter
 def section_fields(form: Form, section: str) -> List[BoundField]:
     return form.get_section(section)
 
+@register.simple_tag(takes_context=True)
+def global_csrf_token(context) -> SafeText:
+    csrf_token = context.get("csrf_token")
+    if not csrf_token or csrf_token == "NOTPROVIDED":
+        return SafeText("")
+    else:
+        return SafeText(f'<meta data-post data-post-csrfmiddlewaretoken="{csrf_token}">')
+
 
 # Components
 
 @register.simple_tag
 def form_section(form: Form, section: str = DEFAULT_FORM_SECTION, padding: bool = True, label: bool = True):
     return loader.get_template("pursuitlib/component/form-section.html").render({"form": form,
                                                                                  "section": section,
@@ -223,7 +227,16 @@
 
 
 @register.simple_tag
 def field(form_field: BoundField, padding: bool = True, label: bool = True):
     return loader.get_template("pursuitlib/component/form-field.html").render({"field": form_field,
                                                                                "padding": padding,
                                                                                "display_label": label})
+
+
+@register.simple_tag(takes_context=True)
+def pagination(context, pages: dict = None, page_var: str = "page"):
+    if pages is None:
+        # Using the "pages" context variable by default
+        pages = context["pages"]
+    return loader.get_template("pursuitlib/component/pagination.html").render({"pages": pages,
+                                                                               "page_var": page_var})
```

### Comparing `pursuitlib-django-0.3.0/pursuitlib_django/utils.py` & `pursuitlib-django-0.3.1/pursuitlib_django/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,12 +30,22 @@
 def get_verbose_name_plural(obj) -> str:
     try:
         return obj._meta.verbose_name_plural
     except AttributeError:
         return get_verbose_name(obj) + "s"
 
 
+def is_feminine(obj) -> bool:
+    try:
+        # noinspection PyTypeChecker
+        if not isinstance(obj, Type):
+            obj = type(obj)
+        return obj.Gender.feminine
+    except AttributeError:
+        return False
+
+
 def safemap(function, input_set) -> map:  # Used to create maps without throwing an error when the database has not been yet initialized
     try:
         return map(function, input_set)
     except ProgrammingError:  # If the database has not been yet initialized, return an empty list, this souldn't matter anyway
         return map(lambda x: x, [])
```

### Comparing `pursuitlib-django-0.3.0/pursuitlib_django/widgets.py` & `pursuitlib-django-0.3.1/pursuitlib_django/widgets.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,14 +65,15 @@
         vtype = self.get_value_type()
         values = super().value_from_datadict(data, files, name)
 
         for i in range(len(values)):
             if not values[i].isdigit():  # If this is a newly created object
                 if self.use_lowercase_names():
                     values[i] = values[i].lower()
+                # noinspection PyUnresolvedReferences
                 try:
                     values[i] = self.queryset.get(name__iexact=values[i]).pk  # If the object already exists, don't create a new one
                 except vtype.DoesNotExist:
                     values[i] = self.queryset.create(name=values[i]).pk
 
         return values
```

### Comparing `pursuitlib-django-0.3.0/pursuitlib_django.egg-info/PKG-INFO` & `pursuitlib-django-0.3.1/pursuitlib_django.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pursuitlib-django
-Version: 0.3.0
+Version: 0.3.1
 Summary: Provides utility functions for Django
 Home-page: https://gitlab.com/frPursuit/pursuitlib-python
 Author: Pursuit
 Author-email: fr.pursuit@gmail.com
 License: All rights reserved
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Pursuit Library - Django
 
 This package provides utility functions and classes for Django (and Select2).
 
 It also contains static files for:
@@ -23,14 +23,16 @@
 - [FontAwesome](https://fontawesome.com/) 5.15.4
 
 ## Configuration
 
 The following values should be added to the Django configuration:
 
 ```python
+from pursuitlib.utils import get_env
+
 VERSION = "PROJECT_VERSION"
 DEV_STAGE = "PROJECT_DEV_STAGE"
 DISPLAY_VERSION = VERSION if DEV_STAGE is None else VERSION + " " + DEV_STAGE
 
 DOMAIN = get_env('PROJECTNAME_DOMAIN')
 USE_HTTPS = get_env('PROJECTNAME_USE_HTTPS').lower() == 'true'
 BASE_URL = ("https://" if USE_HTTPS else "http://") + DOMAIN
```

### Comparing `pursuitlib-django-0.3.0/pursuitlib_django.egg-info/SOURCES.txt` & `pursuitlib-django-0.3.1/pursuitlib_django.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -6,36 +6,38 @@
 pursuitlib_django/apps.py
 pursuitlib_django/decorators.py
 pursuitlib_django/email.py
 pursuitlib_django/errors.py
 pursuitlib_django/forms.py
 pursuitlib_django/gravatar.py
 pursuitlib_django/models.py
+pursuitlib_django/pagination.py
 pursuitlib_django/signals.py
 pursuitlib_django/tests.py
 pursuitlib_django/utils.py
 pursuitlib_django/views.py
 pursuitlib_django/widgets.py
 pursuitlib_django.egg-info/PKG-INFO
 pursuitlib_django.egg-info/SOURCES.txt
 pursuitlib_django.egg-info/dependency_links.txt
 pursuitlib_django.egg-info/requires.txt
 pursuitlib_django.egg-info/top_level.txt
+pursuitlib_django/api/__init__.py
+pursuitlib_django/api/decorators.py
+pursuitlib_django/api/utils.py
 pursuitlib_django/locale/fr/LC_MESSAGES/django.po
 pursuitlib_django/migrations/__init__.py
 pursuitlib_django/static/css/fa.min.css
 pursuitlib_django/static/css/pursuitlib-admin.css
 pursuitlib_django/static/css/pursuitlib.css
-pursuitlib_django/static/css/select2-bootstrap-5-theme.min.css
 pursuitlib_django/static/css/select2.min.css
 pursuitlib_django/static/js/bootstrap.bundle.min.js
 pursuitlib_django/static/js/bootstrap.bundle.min.js.map
 pursuitlib_django/static/js/jquery-3.6.0.min.js
-pursuitlib_django/static/js/pursuitlib-collapseToggle.js
-pursuitlib_django/static/js/pursuitlib-tooltips.js
+pursuitlib_django/static/js/pursuitlib.js
 pursuitlib_django/static/js/select2.full.min.js
 pursuitlib_django/static/js/i18n/select2/fr.js
 pursuitlib_django/static/webfonts/fa-brands-400.eot
 pursuitlib_django/static/webfonts/fa-brands-400.svg
 pursuitlib_django/static/webfonts/fa-brands-400.ttf
 pursuitlib_django/static/webfonts/fa-brands-400.woff
 pursuitlib_django/static/webfonts/fa-brands-400.woff2
@@ -47,11 +49,12 @@
 pursuitlib_django/static/webfonts/fa-solid-900.eot
 pursuitlib_django/static/webfonts/fa-solid-900.svg
 pursuitlib_django/static/webfonts/fa-solid-900.ttf
 pursuitlib_django/static/webfonts/fa-solid-900.woff
 pursuitlib_django/static/webfonts/fa-solid-900.woff2
 pursuitlib_django/templates/pursuitlib/component/form-field.html
 pursuitlib_django/templates/pursuitlib/component/form-section.html
+pursuitlib_django/templates/pursuitlib/component/pagination.html
 pursuitlib_django/templates/pursuitlib/modal/base.html
 pursuitlib_django/templates/pursuitlib/modal/form.html
 pursuitlib_django/templatetags/__init__.py
 pursuitlib_django/templatetags/pursuitlib.py
```

### Comparing `pursuitlib-django-0.3.0/setup.py` & `pursuitlib-django-0.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 directory = Path(__file__).parent
 
 setup(
     name='pursuitlib-django',
-    version='0.3.0',
+    version='0.3.1',
     packages=find_packages(),
     include_package_data=True,
     package_data={'pursuitlib_django': ['locale/*/*/*',
                                         'static/*/*', 'static/*/*/*', 'static/*/*/*/*',
                                         'templates/pursuitlib/*', 'templates/pursuitlib/*/*']},
     install_requires=[
         'pursuitlib',
@@ -24,9 +24,9 @@
     long_description_content_type='text/markdown',
     url='https://gitlab.com/frPursuit/pursuitlib-python',
     license='All rights reserved',
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
-    python_requires=">=3.7"
+    python_requires=">=3.8"
 )
```

