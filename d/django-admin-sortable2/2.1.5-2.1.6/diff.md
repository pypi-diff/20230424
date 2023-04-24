# Comparing `tmp/django-admin-sortable2-2.1.5.tar.gz` & `tmp/django-admin-sortable2-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-admin-sortable2-2.1.5.tar", last modified: Thu Mar 23 22:02:32 2023, max compression
+gzip compressed data, was "django-admin-sortable2-2.1.6.tar", last modified: Mon Apr 24 15:29:14 2023, max compression
```

## Comparing `django-admin-sortable2-2.1.5.tar` & `django-admin-sortable2-2.1.6.tar`

### file list

```diff
@@ -1,78 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 22:02:32.030907 django-admin-sortable2-2.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-23 22:01:45.000000 django-admin-sortable2-2.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-03-23 22:01:45.000000 django-admin-sortable2-2.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-03-23 22:02:32.030907 django-admin-sortable2-2.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-03-23 22:01:45.000000 django-admin-sortable2-2.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 22:02:32.022907 django-admin-sortable2-2.1.5/adminsortable2/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-23 22:01:45.000000 django-admin-sortable2-2.1.5/adminsortable2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21816 2023-03-23 22:01:45.000000 django-admin-sortable2-2.1.5/adminsortable2/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 22:02:32.022907 django-admin-sortable2-2.1.5/adminsortable2/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 22:02:32.022907 django-admin-sortable2-2.1.5/adminsortable2/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 22:02:32.022907 django-admin-sortable2-2.1.5/adminsortable2/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-03-23 22:01:45.000000 django-admin-sortable2-2.1.5/adminsortable2/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-03-23 22:01:45.000000 django-admin-sortable2-2.1.5/adminsortable2/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 22:02:32.022907 django-admin-sortable2-2.1.5/adminsortable2/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 22:02:32.026907 django-admin-sortable2-2.1.5/adminsortable2/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-03-23 22:01:45.000000 django-admin-sortable2-2.1.5/adminsortable2/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-03-23 22:01:45.000000 django-admin-sortable2-2.1.5/adminsortable2/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 22:02:32.022907 django-admin-sortable2-2.1.5/adminsortable2/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 22:02:32.026907 django-admin-sortable2-2.1.5/adminsortable2/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-03-23 22:01:45.000000 django-admin-sortable2-2.1.5/adminsortable2/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-03-23 22:01:45.000000 django-admin-sortable2-2.1.5/adminsortable2/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 22:02:32.022907 django-admin-sortable2-2.1.5/adminsortable2/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 22:02:32.026907 django-admin-sortable2-2.1.5/adminsortable2/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-03-23 22:01:45.000000 django-admin-sortable2-2.1.5/adminsortable2/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-03-23 22:01:45.000000 django-admin-sortable2-2.1.5/adminsortable2/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 22:02:32.022907 django-admin-sortable2-2.1.5/adminsortable2/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 22:02:32.026907 django-admin-sortable2-2.1.5/adminsortable2/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-03-23 22:01:45.000000 django-admin-sortable2-2.1.5/adminsortable2/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-03-23 22:01:45.000000 django-admin-sortable2-2.1.5/adminsortable2/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 22:02:32.022907 django-admin-sortable2-2.1.5/adminsortable2/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 22:02:32.026907 django-admin-sortable2-2.1.5/adminsortable2/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-03-23 22:01:45.000000 django-admin-sortable2-2.1.5/adminsortable2/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-03-23 22:01:45.000000 django-admin-sortable2-2.1.5/adminsortable2/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 22:02:32.022907 django-admin-sortable2-2.1.5/adminsortable2/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 22:02:32.026907 django-admin-sortable2-2.1.5/adminsortable2/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-03-23 22:01:45.000000 django-admin-sortable2-2.1.5/adminsortable2/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-03-23 22:01:45.000000 django-admin-sortable2-2.1.5/adminsortable2/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 22:02:32.022907 django-admin-sortable2-2.1.5/adminsortable2/locale/uk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 22:02:32.026907 django-admin-sortable2-2.1.5/adminsortable2/locale/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-03-23 22:01:45.000000 django-admin-sortable2-2.1.5/adminsortable2/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-03-23 22:01:45.000000 django-admin-sortable2-2.1.5/adminsortable2/locale/uk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 22:02:32.026907 django-admin-sortable2-2.1.5/adminsortable2/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 22:01:45.000000 django-admin-sortable2-2.1.5/adminsortable2/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 22:02:32.026907 django-admin-sortable2-2.1.5/adminsortable2/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 22:01:45.000000 django-admin-sortable2-2.1.5/adminsortable2/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-03-23 22:01:45.000000 django-admin-sortable2-2.1.5/adminsortable2/management/commands/reorder.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-23 22:01:45.000000 django-admin-sortable2-2.1.5/adminsortable2/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 22:02:32.022907 django-admin-sortable2-2.1.5/adminsortable2/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 22:02:32.022907 django-admin-sortable2-2.1.5/adminsortable2/static/adminsortable2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 22:02:32.026907 django-admin-sortable2-2.1.5/adminsortable2/static/adminsortable2/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-03-23 22:01:45.000000 django-admin-sortable2-2.1.5/adminsortable2/static/adminsortable2/css/sortable.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 22:02:32.026907 django-admin-sortable2-2.1.5/adminsortable2/static/adminsortable2/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-03-23 22:01:45.000000 django-admin-sortable2-2.1.5/adminsortable2/static/adminsortable2/icons/drag.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 22:02:32.026907 django-admin-sortable2-2.1.5/adminsortable2/static/adminsortable2/js/
--rw-r--r--   0 runner    (1001) docker     (123)   113660 2023-03-23 22:02:21.000000 django-admin-sortable2-2.1.5/adminsortable2/static/adminsortable2/js/adminsortable2.js
--rw-r--r--   0 runner    (1001) docker     (123)   191513 2023-03-23 22:02:21.000000 django-admin-sortable2-2.1.5/adminsortable2/static/adminsortable2/js/adminsortable2.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    49197 2023-03-23 22:02:22.000000 django-admin-sortable2-2.1.5/adminsortable2/static/adminsortable2/js/adminsortable2.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 22:02:32.022907 django-admin-sortable2-2.1.5/adminsortable2/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 22:02:32.026907 django-admin-sortable2-2.1.5/adminsortable2/templates/adminsortable2/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-03-23 22:01:45.000000 django-admin-sortable2-2.1.5/adminsortable2/templates/adminsortable2/change_list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 22:02:32.026907 django-admin-sortable2-2.1.5/adminsortable2/templates/adminsortable2/edit_inline/
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-03-23 22:02:22.000000 django-admin-sortable2-2.1.5/adminsortable2/templates/adminsortable2/edit_inline/stacked-django-4.0.html
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-03-23 22:02:23.000000 django-admin-sortable2-2.1.5/adminsortable2/templates/adminsortable2/edit_inline/stacked-django-4.1.html
--rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-03-23 22:02:22.000000 django-admin-sortable2-2.1.5/adminsortable2/templates/adminsortable2/edit_inline/tabular-django-4.0.html
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-03-23 22:02:23.000000 django-admin-sortable2-2.1.5/adminsortable2/templates/adminsortable2/edit_inline/tabular-django-4.1.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 22:02:32.030907 django-admin-sortable2-2.1.5/django_admin_sortable2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-03-23 22:02:32.000000 django-admin-sortable2-2.1.5/django_admin_sortable2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-03-23 22:02:32.000000 django-admin-sortable2-2.1.5/django_admin_sortable2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 22:02:32.000000 django-admin-sortable2-2.1.5/django_admin_sortable2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 22:02:31.000000 django-admin-sortable2-2.1.5/django_admin_sortable2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-23 22:02:32.000000 django-admin-sortable2-2.1.5/django_admin_sortable2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-23 22:02:32.000000 django-admin-sortable2-2.1.5/django_admin_sortable2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 22:02:32.030907 django-admin-sortable2-2.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-03-23 22:01:45.000000 django-admin-sortable2-2.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 22:02:32.022907 django-admin-sortable2-2.1.5/testapp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 22:02:32.030907 django-admin-sortable2-2.1.5/testapp/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-03-23 22:01:45.000000 django-admin-sortable2-2.1.5/testapp/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 22:01:45.000000 django-admin-sortable2-2.1.5/testapp/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:29:14.179616 django-admin-sortable2-2.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-24 15:28:43.000000 django-admin-sortable2-2.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-24 15:28:43.000000 django-admin-sortable2-2.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-04-24 15:29:14.179616 django-admin-sortable2-2.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-04-24 15:28:43.000000 django-admin-sortable2-2.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:29:14.171616 django-admin-sortable2-2.1.6/adminsortable2/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-24 15:28:43.000000 django-admin-sortable2-2.1.6/adminsortable2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21816 2023-04-24 15:28:43.000000 django-admin-sortable2-2.1.6/adminsortable2/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:29:14.167616 django-admin-sortable2-2.1.6/adminsortable2/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:29:14.167616 django-admin-sortable2-2.1.6/adminsortable2/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:29:14.171616 django-admin-sortable2-2.1.6/adminsortable2/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-24 15:28:43.000000 django-admin-sortable2-2.1.6/adminsortable2/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-04-24 15:28:43.000000 django-admin-sortable2-2.1.6/adminsortable2/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:29:14.167616 django-admin-sortable2-2.1.6/adminsortable2/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:29:14.171616 django-admin-sortable2-2.1.6/adminsortable2/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-24 15:28:43.000000 django-admin-sortable2-2.1.6/adminsortable2/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-24 15:28:43.000000 django-admin-sortable2-2.1.6/adminsortable2/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:29:14.167616 django-admin-sortable2-2.1.6/adminsortable2/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:29:14.171616 django-admin-sortable2-2.1.6/adminsortable2/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-24 15:28:43.000000 django-admin-sortable2-2.1.6/adminsortable2/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-24 15:28:43.000000 django-admin-sortable2-2.1.6/adminsortable2/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:29:14.167616 django-admin-sortable2-2.1.6/adminsortable2/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:29:14.171616 django-admin-sortable2-2.1.6/adminsortable2/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-24 15:28:43.000000 django-admin-sortable2-2.1.6/adminsortable2/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-24 15:28:43.000000 django-admin-sortable2-2.1.6/adminsortable2/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:29:14.167616 django-admin-sortable2-2.1.6/adminsortable2/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:29:14.171616 django-admin-sortable2-2.1.6/adminsortable2/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-24 15:28:43.000000 django-admin-sortable2-2.1.6/adminsortable2/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-24 15:28:43.000000 django-admin-sortable2-2.1.6/adminsortable2/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:29:14.167616 django-admin-sortable2-2.1.6/adminsortable2/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:29:14.171616 django-admin-sortable2-2.1.6/adminsortable2/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-24 15:28:43.000000 django-admin-sortable2-2.1.6/adminsortable2/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-04-24 15:28:43.000000 django-admin-sortable2-2.1.6/adminsortable2/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:29:14.167616 django-admin-sortable2-2.1.6/adminsortable2/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:29:14.171616 django-admin-sortable2-2.1.6/adminsortable2/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-24 15:28:43.000000 django-admin-sortable2-2.1.6/adminsortable2/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-24 15:28:43.000000 django-admin-sortable2-2.1.6/adminsortable2/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:29:14.167616 django-admin-sortable2-2.1.6/adminsortable2/locale/uk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:29:14.171616 django-admin-sortable2-2.1.6/adminsortable2/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-24 15:28:43.000000 django-admin-sortable2-2.1.6/adminsortable2/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-04-24 15:28:43.000000 django-admin-sortable2-2.1.6/adminsortable2/locale/uk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:29:14.171616 django-admin-sortable2-2.1.6/adminsortable2/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:28:43.000000 django-admin-sortable2-2.1.6/adminsortable2/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:29:14.171616 django-admin-sortable2-2.1.6/adminsortable2/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:28:43.000000 django-admin-sortable2-2.1.6/adminsortable2/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-24 15:28:43.000000 django-admin-sortable2-2.1.6/adminsortable2/management/commands/reorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-24 15:28:43.000000 django-admin-sortable2-2.1.6/adminsortable2/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:29:14.167616 django-admin-sortable2-2.1.6/adminsortable2/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:29:14.171616 django-admin-sortable2-2.1.6/adminsortable2/static/adminsortable2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:29:14.171616 django-admin-sortable2-2.1.6/adminsortable2/static/adminsortable2/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-24 15:28:43.000000 django-admin-sortable2-2.1.6/adminsortable2/static/adminsortable2/css/sortable.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:29:14.171616 django-admin-sortable2-2.1.6/adminsortable2/static/adminsortable2/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-24 15:28:43.000000 django-admin-sortable2-2.1.6/adminsortable2/static/adminsortable2/icons/drag.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:29:14.175616 django-admin-sortable2-2.1.6/adminsortable2/static/adminsortable2/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   113660 2023-04-24 15:29:05.000000 django-admin-sortable2-2.1.6/adminsortable2/static/adminsortable2/js/adminsortable2.js
+-rw-r--r--   0 runner    (1001) docker     (123)   191513 2023-04-24 15:29:05.000000 django-admin-sortable2-2.1.6/adminsortable2/static/adminsortable2/js/adminsortable2.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    49197 2023-04-24 15:29:06.000000 django-admin-sortable2-2.1.6/adminsortable2/static/adminsortable2/js/adminsortable2.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:29:14.171616 django-admin-sortable2-2.1.6/adminsortable2/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:29:14.175616 django-admin-sortable2-2.1.6/adminsortable2/templates/adminsortable2/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-24 15:28:43.000000 django-admin-sortable2-2.1.6/adminsortable2/templates/adminsortable2/change_list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:29:14.175616 django-admin-sortable2-2.1.6/adminsortable2/templates/adminsortable2/edit_inline/
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-24 15:29:07.000000 django-admin-sortable2-2.1.6/adminsortable2/templates/adminsortable2/edit_inline/stacked-django-4.0.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-04-24 15:29:07.000000 django-admin-sortable2-2.1.6/adminsortable2/templates/adminsortable2/edit_inline/stacked-django-4.1.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-04-24 15:29:07.000000 django-admin-sortable2-2.1.6/adminsortable2/templates/adminsortable2/edit_inline/stacked-django-4.2.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-04-24 15:29:07.000000 django-admin-sortable2-2.1.6/adminsortable2/templates/adminsortable2/edit_inline/tabular-django-4.0.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-04-24 15:29:07.000000 django-admin-sortable2-2.1.6/adminsortable2/templates/adminsortable2/edit_inline/tabular-django-4.1.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-04-24 15:29:07.000000 django-admin-sortable2-2.1.6/adminsortable2/templates/adminsortable2/edit_inline/tabular-django-4.2.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-04-24 15:29:07.000000 django-admin-sortable2-2.1.6/adminsortable2/templates/adminsortable2/edit_inline/tabular-django-4.2.html.orig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:29:14.179616 django-admin-sortable2-2.1.6/django_admin_sortable2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-04-24 15:29:14.000000 django-admin-sortable2-2.1.6/django_admin_sortable2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-24 15:29:14.000000 django-admin-sortable2-2.1.6/django_admin_sortable2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 15:29:14.000000 django-admin-sortable2-2.1.6/django_admin_sortable2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 15:29:14.000000 django-admin-sortable2-2.1.6/django_admin_sortable2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-24 15:29:14.000000 django-admin-sortable2-2.1.6/django_admin_sortable2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-24 15:29:14.000000 django-admin-sortable2-2.1.6/django_admin_sortable2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 15:29:14.179616 django-admin-sortable2-2.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-24 15:28:43.000000 django-admin-sortable2-2.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:29:14.171616 django-admin-sortable2-2.1.6/testapp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:29:14.179616 django-admin-sortable2-2.1.6/testapp/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-04-24 15:28:43.000000 django-admin-sortable2-2.1.6/testapp/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:28:43.000000 django-admin-sortable2-2.1.6/testapp/migrations/__init__.py
```

### Comparing `django-admin-sortable2-2.1.5/LICENSE` & `django-admin-sortable2-2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.5/PKG-INFO` & `django-admin-sortable2-2.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-sortable2
-Version: 2.1.5
+Version: 2.1.6
 Summary: Generic drag-and-drop sorting for the List, the Stacked- and the Tabular-Inlines Views in the Django Admin
 Home-page: https://github.com/jrief/django-admin-sortable2
 Author: Jacob Rief
 Author-email: jacob.rief@gmail.com
 License: MIT
 Keywords: django
 Platform: OS Independent
@@ -19,14 +19,15 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # django-admin-sortable2
 
 This Django package adds functionality for generic drag-and-drop ordering of items in the List, the Stacked- and the
 Tabular-Inlines Views of the Django Admin interface.
```

### Comparing `django-admin-sortable2-2.1.5/README.md` & `django-admin-sortable2-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.5/adminsortable2/admin.py` & `django-admin-sortable2-2.1.6/adminsortable2/admin.py`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.5/adminsortable2/locale/de/LC_MESSAGES/django.mo` & `django-admin-sortable2-2.1.6/adminsortable2/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.5/adminsortable2/locale/de/LC_MESSAGES/django.po` & `django-admin-sortable2-2.1.6/adminsortable2/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.5/adminsortable2/locale/en/LC_MESSAGES/django.po` & `django-admin-sortable2-2.1.6/adminsortable2/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.5/adminsortable2/locale/es/LC_MESSAGES/django.mo` & `django-admin-sortable2-2.1.6/adminsortable2/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.5/adminsortable2/locale/es/LC_MESSAGES/django.po` & `django-admin-sortable2-2.1.6/adminsortable2/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.5/adminsortable2/locale/fr/LC_MESSAGES/django.mo` & `django-admin-sortable2-2.1.6/adminsortable2/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.5/adminsortable2/locale/fr/LC_MESSAGES/django.po` & `django-admin-sortable2-2.1.6/adminsortable2/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.5/adminsortable2/locale/it/LC_MESSAGES/django.mo` & `django-admin-sortable2-2.1.6/adminsortable2/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.5/adminsortable2/locale/it/LC_MESSAGES/django.po` & `django-admin-sortable2-2.1.6/adminsortable2/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.5/adminsortable2/locale/pl/LC_MESSAGES/django.mo` & `django-admin-sortable2-2.1.6/adminsortable2/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.5/adminsortable2/locale/pl/LC_MESSAGES/django.po` & `django-admin-sortable2-2.1.6/adminsortable2/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.5/adminsortable2/locale/ru/LC_MESSAGES/django.mo` & `django-admin-sortable2-2.1.6/adminsortable2/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.5/adminsortable2/locale/ru/LC_MESSAGES/django.po` & `django-admin-sortable2-2.1.6/adminsortable2/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.5/adminsortable2/locale/uk/LC_MESSAGES/django.mo` & `django-admin-sortable2-2.1.6/adminsortable2/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.5/adminsortable2/locale/uk/LC_MESSAGES/django.po` & `django-admin-sortable2-2.1.6/adminsortable2/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.5/adminsortable2/management/commands/reorder.py` & `django-admin-sortable2-2.1.6/adminsortable2/management/commands/reorder.py`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.5/adminsortable2/static/adminsortable2/css/sortable.css` & `django-admin-sortable2-2.1.6/adminsortable2/static/adminsortable2/css/sortable.css`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.5/adminsortable2/static/adminsortable2/icons/drag.png` & `django-admin-sortable2-2.1.6/adminsortable2/static/adminsortable2/icons/drag.png`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.5/adminsortable2/static/adminsortable2/js/adminsortable2.js` & `django-admin-sortable2-2.1.6/adminsortable2/static/adminsortable2/js/adminsortable2.js`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.5/adminsortable2/static/adminsortable2/js/adminsortable2.js.map` & `django-admin-sortable2-2.1.6/adminsortable2/static/adminsortable2/js/adminsortable2.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.5/adminsortable2/static/adminsortable2/js/adminsortable2.min.js` & `django-admin-sortable2-2.1.6/adminsortable2/static/adminsortable2/js/adminsortable2.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.5/adminsortable2/templates/adminsortable2/edit_inline/stacked-django-4.0.html` & `django-admin-sortable2-2.1.6/adminsortable2/templates/adminsortable2/edit_inline/stacked-django-4.0.html`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.5/adminsortable2/templates/adminsortable2/edit_inline/stacked-django-4.1.html` & `django-admin-sortable2-2.1.6/adminsortable2/templates/adminsortable2/edit_inline/stacked-django-4.1.html`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.5/adminsortable2/templates/adminsortable2/edit_inline/tabular-django-4.0.html` & `django-admin-sortable2-2.1.6/adminsortable2/templates/adminsortable2/edit_inline/tabular-django-4.0.html`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.5/adminsortable2/templates/adminsortable2/edit_inline/tabular-django-4.1.html` & `django-admin-sortable2-2.1.6/adminsortable2/templates/adminsortable2/edit_inline/tabular-django-4.1.html`

 * *Files identical despite different names*

### Comparing `django-admin-sortable2-2.1.5/django_admin_sortable2.egg-info/PKG-INFO` & `django-admin-sortable2-2.1.6/django_admin_sortable2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-sortable2
-Version: 2.1.5
+Version: 2.1.6
 Summary: Generic drag-and-drop sorting for the List, the Stacked- and the Tabular-Inlines Views in the Django Admin
 Home-page: https://github.com/jrief/django-admin-sortable2
 Author: Jacob Rief
 Author-email: jacob.rief@gmail.com
 License: MIT
 Keywords: django
 Platform: OS Independent
@@ -19,14 +19,15 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # django-admin-sortable2
 
 This Django package adds functionality for generic drag-and-drop ordering of items in the List, the Stacked- and the
 Tabular-Inlines Views of the Django Admin interface.
```

### Comparing `django-admin-sortable2-2.1.5/django_admin_sortable2.egg-info/SOURCES.txt` & `django-admin-sortable2-2.1.6/django_admin_sortable2.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -28,16 +28,19 @@
 adminsortable2/static/adminsortable2/icons/drag.png
 adminsortable2/static/adminsortable2/js/adminsortable2.js
 adminsortable2/static/adminsortable2/js/adminsortable2.js.map
 adminsortable2/static/adminsortable2/js/adminsortable2.min.js
 adminsortable2/templates/adminsortable2/change_list.html
 adminsortable2/templates/adminsortable2/edit_inline/stacked-django-4.0.html
 adminsortable2/templates/adminsortable2/edit_inline/stacked-django-4.1.html
+adminsortable2/templates/adminsortable2/edit_inline/stacked-django-4.2.html
 adminsortable2/templates/adminsortable2/edit_inline/tabular-django-4.0.html
 adminsortable2/templates/adminsortable2/edit_inline/tabular-django-4.1.html
+adminsortable2/templates/adminsortable2/edit_inline/tabular-django-4.2.html
+adminsortable2/templates/adminsortable2/edit_inline/tabular-django-4.2.html.orig
 django_admin_sortable2.egg-info/PKG-INFO
 django_admin_sortable2.egg-info/SOURCES.txt
 django_admin_sortable2.egg-info/dependency_links.txt
 django_admin_sortable2.egg-info/not-zip-safe
 django_admin_sortable2.egg-info/requires.txt
 django_admin_sortable2.egg-info/top_level.txt
 testapp/migrations/0001_initial.py
```

### Comparing `django-admin-sortable2-2.1.5/setup.py` & `django-admin-sortable2-2.1.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     'Development Status :: 5 - Production/Stable',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Framework :: Django',
     'Framework :: Django :: 4.0',
     'Framework :: Django :: 4.1',
+    'Framework :: Django :: 4.2',
 ]
 
 
 setup(
     name='django-admin-sortable2',
     version=__version__,
     author='Jacob Rief',
```

### Comparing `django-admin-sortable2-2.1.5/testapp/migrations/0001_initial.py` & `django-admin-sortable2-2.1.6/testapp/migrations/0001_initial.py`

 * *Files identical despite different names*

