# Comparing `tmp/sloth-framework-0.1.2.tar.gz` & `tmp/sloth-framework-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sloth-framework-0.1.2.tar", last modified: Tue Apr 18 21:58:27 2023, max compression
+gzip compressed data, was "sloth-framework-0.1.3.tar", last modified: Mon Apr 24 10:11:30 2023, max compression
```

## Comparing `sloth-framework-0.1.2.tar` & `sloth-framework-0.1.3.tar`

### file list

```diff
@@ -1,292 +1,295 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.935845 sloth-framework-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-18 21:58:27.935845 sloth-framework-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 21:58:27.935845 sloth-framework-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.891843 sloth-framework-0.1.2/sloth/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.895843 sloth-framework-0.1.2/sloth/actions/
--rw-r--r--   0 runner    (1001) docker     (123)    36880 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/actions/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/actions/inputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.895843 sloth-framework-0.1.2/sloth/api/
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18644 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/actions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.895843 sloth-framework-0.1.2/sloth/api/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.895843 sloth-framework-0.1.2/sloth/api/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.895843 sloth-framework-0.1.2/sloth/api/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.895843 sloth-framework-0.1.2/sloth/api/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/management/commands/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/management/commands/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/management/commands/reset_passwords.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/management/commands/selenium.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/management/commands/send_web_push_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/management/commands/startserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/management/commands/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/management/commands/sync_roles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.899843 sloth-framework-0.1.2/sloth/api/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/migrations/0002_role_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/migrations/0003_alter_application_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/migrations/0004_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/migrations/0005_task_stopped_alter_task_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/migrations/0006_role_active_alter_role_name_alter_role_scope_key_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/migrations/0007_alter_scope_description_alter_task_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/migrations/0008_alter_application_available_scopes_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/migrations/0009_pushnotification.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/migrations/0010_alter_pushnotification_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/migrations/0011_alter_application_client_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/migrations/0012_authcode.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/migrations/0013_task_partial_task_total.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/migrations/0014_email.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.887843 sloth-framework-0.1.2/sloth/api/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.899843 sloth-framework-0.1.2/sloth/api/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)    58578 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/css/all.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    67289 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/css/bootstrap-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)   155845 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/css/colorpick.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.903843 sloth-framework-0.1.2/sloth/api/static/css/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   107280 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/css/fonts/Eina02-Bold.f8011405.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   116316 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/css/fonts/Eina02-Regular.2e682693.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   112880 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   111976 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/css/fonts/bootstrap-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)    83304 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/css/fonts/bootstrap-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    30702 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/css/icons.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.903843 sloth-framework-0.1.2/sloth/api/static/css/images/
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/css/images/ui-icons_444444_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/css/images/ui-icons_555555_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)    35973 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/css/jquery-ui.css
--rw-r--r--   0 runner    (1001) docker     (123)    14670 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/css/leaflet.css
--rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/css/select2.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/css/sloth.css
--rw-r--r--   0 runner    (1001) docker     (123)    17867 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/css/trumbowyg.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.887843 sloth-framework-0.1.2/sloth/api/static/icons/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.903843 sloth-framework-0.1.2/sloth/api/static/icons/fontawesome/
--rw-r--r--   0 runner    (1001) docker     (123)   100170 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/icons/fontawesome/fontawesome.min.css
--rw-r--r--   0 runner    (1001) docker     (123)  1726692 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/icons/fontawesome/fontawesome.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.907844 sloth-framework-0.1.2/sloth/api/static/icons/fontawesome/webfonts/
--rw-r--r--   0 runner    (1001) docker     (123)   181852 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   105536 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    60520 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    23940 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    10556 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.907844 sloth-framework-0.1.2/sloth/api/static/icons/materialicons/
--rw-r--r--   0 runner    (1001) docker     (123)   174176 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/icons/materialicons/LDItaoyNOAY6Uewc665JcIzCKsKc_M9flwmPq_HTTw.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   127220 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/icons/materialicons/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   155604 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/icons/materialicons/gok-H7zzDkdnRel8-DQ6KAXJ69wP1tGnf4ZGhUcel5euIg.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/icons/materialicons/materialicons.css
--rw-r--r--   0 runner    (1001) docker     (123)   135988 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/icons/materialicons/oPWQ_lt5nv4pWNJpghLP75WiFR4kLh3kvmvRImcycg.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.911844 sloth-framework-0.1.2/sloth/api/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    57420 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/images/click.png
--rw-r--r--   0 runner    (1001) docker     (123)    55448 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/images/hand.png
--rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/images/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/images/icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.911844 sloth-framework-0.1.2/sloth/api/static/images/images/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/images/images/badge.png
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/images/images/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    45136 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/images/login.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)    22817 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    21495 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/images/no-image.png
--rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/images/sloth.png
--rw-r--r--   0 runner    (1001) docker     (123)    13670 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/images/user.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.915844 sloth-framework-0.1.2/sloth/api/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/js/api.js
--rw-r--r--   0 runner    (1001) docker     (123)    78743 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/js/bootstrap.bundle.min.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     4098 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/js/colorpick.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.915844 sloth-framework-0.1.2/sloth/api/static/js/i18n/
--rwxr-xr-x   0 runner    (1001) docker     (123)      853 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/js/i18n/pt-BR.js
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/js/jquery-3.6.0.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   520714 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/js/jquery-ui.js
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/js/jquery.binarytransport.js
--rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/js/jquery.mask.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    80794 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/js/jquery.timepicker.js
--rw-r--r--   0 runner    (1001) docker     (123)   147555 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/js/leaflet.js
--rw-r--r--   0 runner    (1001) docker     (123)    24103 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/js/masonry.pkgd.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/js/popper.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    43994 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/js/qr-scanner-worker.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    15538 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/js/qr-scanner.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    19927 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/js/qrcode.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    73163 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/js/select2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    15700 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/js/sloth.js
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/js/sw.js
--rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/js/tests.js
--rw-r--r--   0 runner    (1001) docker     (123)    28280 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/js/trumbowyg.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/static/js/wpn.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.915844 sloth-framework-0.1.2/sloth/api/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.891843 sloth-framework-0.1.2/sloth/api/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.915844 sloth-framework-0.1.2/sloth/api/templates/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/actions/execute_query.html
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/actions/execute_script.html
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/actions/show_icons.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.915844 sloth-framework-0.1.2/sloth/api/templates/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/api/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.915844 sloth-framework-0.1.2/sloth/api/templates/charts/
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/charts/bar.html
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/charts/column.html
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/charts/donut.html
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/charts/legend.html
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/charts/pie.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.919844 sloth-framework-0.1.2/sloth/api/templates/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/actions.html
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/apps.html
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/bottom.html
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/cards.html
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/dashboards.html
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/default.html
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/form.html
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/grids.html
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/header.html
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/links.html
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/menu.html
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/messages.html
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/modal.html
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/plus.html
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/report.html
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/search.html
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/settings.html
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/shortcuts.html
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/tasks.html
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/dashboard/tools.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.919844 sloth-framework-0.1.2/sloth/api/templates/inputs/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/inputs/picker.html
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/inputs/qrcode.html
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/inputs/select.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.923844 sloth-framework-0.1.2/sloth/api/templates/queryset/
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/queryset/accordion.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.923844 sloth-framework-0.1.2/sloth/api/templates/queryset/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/queryset/actions/actions.html
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/queryset/actions/batch.html
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/queryset/actions/global.html
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/queryset/calendar.html
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/queryset/cards.html
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/queryset/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/queryset/datatable.html
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/queryset/filter.html
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/queryset/filters.html
--rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/queryset/queryset.html
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/queryset/rows.html
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/queryset/scroll.html
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/queryset/statistics.html
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/queryset/timeline.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.891843 sloth-framework-0.1.2/sloth/api/templates/renderers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.923844 sloth-framework-0.1.2/sloth/api/templates/renderers/badges/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/badges/badge.html
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/badges/boolean.html
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/badges/primary.html
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/badges/status.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.923844 sloth-framework-0.1.2/sloth/api/templates/renderers/boolean/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/boolean/thumb.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.923844 sloth-framework-0.1.2/sloth/api/templates/renderers/calendar/
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/calendar/calendar.html
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/calendar/events.html
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/calendar/legend.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.923844 sloth-framework-0.1.2/sloth/api/templates/renderers/documents/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/documents/document.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.923844 sloth-framework-0.1.2/sloth/api/templates/renderers/images/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/images/banner.html
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/images/image.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.923844 sloth-framework-0.1.2/sloth/api/templates/renderers/links/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/links/file.html
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/links/url.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.923844 sloth-framework-0.1.2/sloth/api/templates/renderers/maps/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/maps/geolocation.html
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/maps/map.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.927844 sloth-framework-0.1.2/sloth/api/templates/renderers/messages/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/messages/custom.html
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/messages/danger.html
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/messages/message.html
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/messages/primary.html
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/messages/success.html
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/messages/warning.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.927844 sloth-framework-0.1.2/sloth/api/templates/renderers/photos/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/photos/photo.html
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/photos/round.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.927844 sloth-framework-0.1.2/sloth/api/templates/renderers/programing/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/programing/strtable.html
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/programing/terminal.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.927844 sloth-framework-0.1.2/sloth/api/templates/renderers/tags/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/tags/primary.html
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/tags/tags.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.927844 sloth-framework-0.1.2/sloth/api/templates/renderers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/utils/formatted.html
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/utils/progress.html
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/utils/qrcode.html
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/utils/steps.html
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/renderers/utils/table.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.927844 sloth-framework-0.1.2/sloth/api/templates/themes/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/themes/dark.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.931844 sloth-framework-0.1.2/sloth/api/templates/valueset/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/valueset/2-column.html
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/valueset/field.html
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/valueset/fieldset-group.html
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/valueset/fieldset-list.html
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/valueset/fieldset-tab.html
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/valueset/fieldset.html
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/valueset/primitive.html
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/valueset/value.html
--rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templates/valueset/valueset.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.931844 sloth-framework-0.1.2/sloth/api/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9110 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/templatetags/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    11104 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/api/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.931844 sloth-framework-0.1.2/sloth/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/cloud/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      688 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/cloud/printer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6116 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/cloud/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.931844 sloth-framework-0.1.2/sloth/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/conf/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.931844 sloth-framework-0.1.2/sloth/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21312 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    37888 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/core/queryset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/core/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/core/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    20111 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/core/valueset.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/core/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.931844 sloth-framework-0.1.2/sloth/db/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.931844 sloth-framework-0.1.2/sloth/db/models/
--rw-r--r--   0 runner    (1001) docker     (123)     9656 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/db/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.931844 sloth-framework-0.1.2/sloth/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.931844 sloth-framework-0.1.2/sloth/test/selenium/
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/test/selenium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/test/selenium/browser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.931844 sloth-framework-0.1.2/sloth/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.931844 sloth-framework-0.1.2/sloth/utils/formatter/
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/utils/formatter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.931844 sloth-framework-0.1.2/sloth/utils/http/
--rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/utils/http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.935845 sloth-framework-0.1.2/sloth/utils/icons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/utils/icons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28753 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/utils/icons/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)    53105 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/utils/icons/fontawesome.py
--rw-r--r--   0 runner    (1001) docker     (123)    20959 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/utils/icons/materialicons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.935845 sloth-framework-0.1.2/sloth/utils/log/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/utils/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-18 21:58:22.000000 sloth-framework-0.1.2/sloth/utils/log/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:27.935845 sloth-framework-0.1.2/sloth_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-18 21:58:27.000000 sloth-framework-0.1.2/sloth_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9416 2023-04-18 21:58:27.000000 sloth-framework-0.1.2/sloth_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 21:58:27.000000 sloth-framework-0.1.2/sloth_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 21:58:27.000000 sloth-framework-0.1.2/sloth_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-18 21:58:27.000000 sloth-framework-0.1.2/sloth_framework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.989580 sloth-framework-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-24 10:11:30.989580 sloth-framework-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 10:11:30.989580 sloth-framework-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.965579 sloth-framework-0.1.3/sloth/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.965579 sloth-framework-0.1.3/sloth/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)    37193 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/actions/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/actions/inputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.965579 sloth-framework-0.1.3/sloth/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18644 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/actions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.965579 sloth-framework-0.1.3/sloth/api/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.965579 sloth-framework-0.1.3/sloth/api/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.965579 sloth-framework-0.1.3/sloth/api/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.965579 sloth-framework-0.1.3/sloth/api/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/management/commands/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/management/commands/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/management/commands/reset_passwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/management/commands/selenium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/management/commands/send_web_push_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/management/commands/startserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/management/commands/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/management/commands/sync_roles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.965579 sloth-framework-0.1.3/sloth/api/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/migrations/0002_role_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/migrations/0003_alter_application_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/migrations/0004_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/migrations/0005_task_stopped_alter_task_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/migrations/0006_role_active_alter_role_name_alter_role_scope_key_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/migrations/0007_alter_scope_description_alter_task_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/migrations/0008_alter_application_available_scopes_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/migrations/0009_pushnotification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/migrations/0010_alter_pushnotification_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/migrations/0011_alter_application_client_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/migrations/0012_authcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/migrations/0013_task_partial_task_total.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/migrations/0014_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.961579 sloth-framework-0.1.3/sloth/api/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.969580 sloth-framework-0.1.3/sloth/api/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    58578 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/css/all.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    67289 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/css/bootstrap-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)   155845 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/css/colorpick.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.969580 sloth-framework-0.1.3/sloth/api/static/css/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   107280 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/css/fonts/Eina02-Bold.f8011405.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   116316 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/css/fonts/Eina02-Regular.2e682693.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   112880 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   111976 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/css/fonts/bootstrap-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    83304 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/css/fonts/bootstrap-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    30702 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/css/icons.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.969580 sloth-framework-0.1.3/sloth/api/static/css/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/css/images/ui-icons_444444_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/css/images/ui-icons_555555_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)    35973 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/css/jquery-ui.css
+-rw-r--r--   0 runner    (1001) docker     (123)    14670 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/css/leaflet.css
+-rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/css/select2.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/css/sloth.css
+-rw-r--r--   0 runner    (1001) docker     (123)    17867 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/css/trumbowyg.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.961579 sloth-framework-0.1.3/sloth/api/static/icons/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.969580 sloth-framework-0.1.3/sloth/api/static/icons/fontawesome/
+-rw-r--r--   0 runner    (1001) docker     (123)   100170 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/icons/fontawesome/fontawesome.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)  1726692 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/icons/fontawesome/fontawesome.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.973580 sloth-framework-0.1.3/sloth/api/static/icons/fontawesome/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   181852 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   105536 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    60520 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    23940 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    10556 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.973580 sloth-framework-0.1.3/sloth/api/static/icons/materialicons/
+-rw-r--r--   0 runner    (1001) docker     (123)   174176 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/icons/materialicons/LDItaoyNOAY6Uewc665JcIzCKsKc_M9flwmPq_HTTw.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   127220 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/icons/materialicons/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   155604 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/icons/materialicons/gok-H7zzDkdnRel8-DQ6KAXJ69wP1tGnf4ZGhUcel5euIg.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/icons/materialicons/materialicons.css
+-rw-r--r--   0 runner    (1001) docker     (123)   135988 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/icons/materialicons/oPWQ_lt5nv4pWNJpghLP75WiFR4kLh3kvmvRImcycg.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.973580 sloth-framework-0.1.3/sloth/api/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    57420 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/images/click.png
+-rw-r--r--   0 runner    (1001) docker     (123)    55448 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/images/hand.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/images/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/images/icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.973580 sloth-framework-0.1.3/sloth/api/static/images/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/images/images/badge.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/images/images/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    45136 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/images/login.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)    22817 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    21495 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/images/no-image.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/images/sloth.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13670 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/images/user.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.977580 sloth-framework-0.1.3/sloth/api/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/js/api.js
+-rw-r--r--   0 runner    (1001) docker     (123)    78743 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/js/bootstrap.bundle.min.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4098 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/js/colorpick.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.977580 sloth-framework-0.1.3/sloth/api/static/js/i18n/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      853 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/js/i18n/pt-BR.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/js/jquery-3.6.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   520714 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/js/jquery-ui.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/js/jquery.binarytransport.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/js/jquery.mask.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    80794 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/js/jquery.timepicker.js
+-rw-r--r--   0 runner    (1001) docker     (123)   147555 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/js/leaflet.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24103 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/js/masonry.pkgd.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/js/popper.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    43994 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/js/qr-scanner-worker.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15538 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/js/qr-scanner.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19927 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/js/qrcode.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    73163 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/js/select2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15684 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/js/sloth.js
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/js/sw.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/js/tests.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28280 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/js/trumbowyg.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/js/wpn.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.977580 sloth-framework-0.1.3/sloth/api/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.961579 sloth-framework-0.1.3/sloth/api/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.977580 sloth-framework-0.1.3/sloth/api/templates/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/actions/execute_query.html
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/actions/execute_script.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/actions/show_icons.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.977580 sloth-framework-0.1.3/sloth/api/templates/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/api/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.977580 sloth-framework-0.1.3/sloth/api/templates/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/charts/bar.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/charts/column.html
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/charts/donut.html
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/charts/legend.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/charts/pie.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.981580 sloth-framework-0.1.3/sloth/api/templates/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/actions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/apps.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/bottom.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/cards.html
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/dashboards.html
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/default.html
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7132 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/grids.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/header.html
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/links.html
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/messages.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/plus.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/report.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/settings.html
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/shortcuts.html
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/tasks.html
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/tools.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.981580 sloth-framework-0.1.3/sloth/api/templates/inputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/inputs/picker.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/inputs/qrcode.html
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/inputs/select.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.981580 sloth-framework-0.1.3/sloth/api/templates/queryset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/queryset/accordion.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.981580 sloth-framework-0.1.3/sloth/api/templates/queryset/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/queryset/actions/actions.html
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/queryset/actions/batch.html
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/queryset/actions/global.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/queryset/calendar.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/queryset/cards.html
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/queryset/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/queryset/datatable.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/queryset/filter.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/queryset/filters.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/queryset/queryset.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/queryset/rows.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/queryset/scroll.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/queryset/statistics.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/queryset/timeline.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.961579 sloth-framework-0.1.3/sloth/api/templates/renderers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.981580 sloth-framework-0.1.3/sloth/api/templates/renderers/badges/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/badges/badge.html
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/badges/boolean.html
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/badges/danger.html
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/badges/primary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/badges/status.html
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/badges/warning.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.981580 sloth-framework-0.1.3/sloth/api/templates/renderers/boolean/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/boolean/thumb.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.985580 sloth-framework-0.1.3/sloth/api/templates/renderers/calendar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/calendar/calendar.html
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/calendar/events.html
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/calendar/legend.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.985580 sloth-framework-0.1.3/sloth/api/templates/renderers/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/documents/document.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.985580 sloth-framework-0.1.3/sloth/api/templates/renderers/images/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/images/banner.html
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/images/image.html
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/images/round.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.985580 sloth-framework-0.1.3/sloth/api/templates/renderers/links/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/links/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/links/url.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.985580 sloth-framework-0.1.3/sloth/api/templates/renderers/maps/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/maps/geolocation.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/maps/map.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.985580 sloth-framework-0.1.3/sloth/api/templates/renderers/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/messages/custom.html
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/messages/danger.html
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/messages/message.html
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/messages/primary.html
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/messages/success.html
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/messages/warning.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.985580 sloth-framework-0.1.3/sloth/api/templates/renderers/photos/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/photos/photo.html
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/photos/round.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.985580 sloth-framework-0.1.3/sloth/api/templates/renderers/programing/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/programing/strtable.html
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/programing/terminal.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.985580 sloth-framework-0.1.3/sloth/api/templates/renderers/tags/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/tags/primary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/tags/tags.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.985580 sloth-framework-0.1.3/sloth/api/templates/renderers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/utils/formatted.html
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/utils/progress.html
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/utils/qrcode.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/utils/steps.html
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/utils/table.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.985580 sloth-framework-0.1.3/sloth/api/templates/themes/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/themes/dark.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.985580 sloth-framework-0.1.3/sloth/api/templates/valueset/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/valueset/2-column.html
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/valueset/field.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/valueset/fieldset-group.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/valueset/fieldset-list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/valueset/fieldset-tab.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/valueset/fieldset.html
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/valueset/primitive.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/valueset/value.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/valueset/valueset.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.985580 sloth-framework-0.1.3/sloth/api/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templatetags/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11104 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.985580 sloth-framework-0.1.3/sloth/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/cloud/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      688 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/cloud/printer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6116 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/cloud/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.989580 sloth-framework-0.1.3/sloth/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/conf/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.989580 sloth-framework-0.1.3/sloth/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21329 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38221 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/core/queryset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11250 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/core/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/core/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20156 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/core/valueset.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/core/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.989580 sloth-framework-0.1.3/sloth/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.989580 sloth-framework-0.1.3/sloth/db/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     9656 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/db/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.989580 sloth-framework-0.1.3/sloth/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.989580 sloth-framework-0.1.3/sloth/test/selenium/
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/test/selenium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/test/selenium/browser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.989580 sloth-framework-0.1.3/sloth/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.989580 sloth-framework-0.1.3/sloth/utils/formatter/
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/utils/formatter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.989580 sloth-framework-0.1.3/sloth/utils/http/
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/utils/http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.989580 sloth-framework-0.1.3/sloth/utils/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/utils/icons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28753 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/utils/icons/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53105 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/utils/icons/fontawesome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20959 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/utils/icons/materialicons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.989580 sloth-framework-0.1.3/sloth/utils/log/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/utils/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/utils/log/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.989580 sloth-framework-0.1.3/sloth_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-24 10:11:30.000000 sloth-framework-0.1.3/sloth_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-04-24 10:11:30.000000 sloth-framework-0.1.3/sloth_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 10:11:30.000000 sloth-framework-0.1.3/sloth_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-24 10:11:30.000000 sloth-framework-0.1.3/sloth_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 10:11:30.000000 sloth-framework-0.1.3/sloth_framework.egg-info/top_level.txt
```

### Comparing `sloth-framework-0.1.2/PKG-INFO` & `sloth-framework-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sloth-framework
-Version: 0.1.2
+Version: 0.1.3
 Summary: Metadata-based web framework for the development of management information systems
 Home-page: http://sloth.aplicativo.click/
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `sloth-framework-0.1.2/setup.py` & `sloth-framework-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open(os.path.join(root_dir, 'sloth/requirements.txt')) as file:
     requirements = file.read().strip().splitlines()
 
 os.chdir(root_dir)
 
 setup(
     name='sloth-framework',
-    version='0.1.2',
+    version='0.1.3',
     packages=find_packages(),
     install_requires=requirements,
     extras_require={
         'dev': [],
         'production': [],
     },
     include_package_data=True,
```

### Comparing `sloth-framework-0.1.2/sloth/Dockerfile` & `sloth-framework-0.1.3/sloth/Dockerfile`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/__init__.py` & `sloth-framework-0.1.3/sloth/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/__main__.py` & `sloth-framework-0.1.3/sloth/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 
 MODELS_FILE_CONTENT = '''from sloth.db import models, role, meta
 '''
 
 ACTIONS_FILE_CONTENT = '''from sloth import actions
 '''
 
+TASKS_FILE_CONTENT = '''from sloth.api.tasks import Task
+'''
+
 DASHBOARD_FILE_CONTENT = '''from sloth.api.dashboard import Dashboard
 from .models import *
 
 
 class AppDashboard(Dashboard):
 
     def __init__(self, request):
@@ -144,14 +147,17 @@
         file.write(URLS_FILE_CONTENT)
     models_path = os.path.join(name, 'models.py')
     with open(models_path, 'w') as file:
         file.write(MODELS_FILE_CONTENT)
     actions_path = os.path.join(name, 'actions.py')
     with open(actions_path, 'w') as file:
         file.write(ACTIONS_FILE_CONTENT)
+    tasks_path = os.path.join(name, 'tasks.py')
+    with open(tasks_path, 'w') as file:
+        file.write(TASKS_FILE_CONTENT)
     dashboard_path = os.path.join(name, 'dashboard.py')
     with open(dashboard_path, 'w') as file:
         file.write(DASHBOARD_FILE_CONTENT)
     workflows_path = os.path.join('.github', 'workflows')
     os.makedirs(workflows_path, exist_ok=True)
     deploy_workflow_path = os.path.join(workflows_path, 'deploy.yml')
     with open(deploy_workflow_path, 'w') as file:
```

### Comparing `sloth-framework-0.1.2/sloth/actions/__init__.py` & `sloth-framework-0.1.3/sloth/actions/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         self.queryset = kwargs.pop('queryset', None)
         self.instances = kwargs.pop('instances', None)
         self.metaclass = getattr(self, 'Meta')
 
         self.show_form = True
         self.can_be_closed = False
         self.can_be_reloaded = False
-        self.content = dict(top=[], left=[], center=[], right=[], bottom=[], info=[], alert=[])
+        self.content = dict(top=[], left=[], center=[], right=[], bottom=[], info=[], alert=[], danger=[])
         self.on_change_data = dict(show=[], hide=[], set=[], show_fieldset=[], hide_fieldset=[])
 
         if forms.ModelForm in self.__class__.__bases__:
             self.instance = kwargs.get('instance', None)
         else:
             self.instance = kwargs.pop('instance', None)
 
@@ -148,15 +148,16 @@
         super().__init__(*args, **kwargs)
         if self.instance is not None and hasattr(self.instance, 'autouser') and not self.instance.autouser_id:
             self.instance.autouser = self.request.user
             if 'autouser' in self.fields:
                 del self.fields['autouser']
 
         for name in self.fields:
-            setattr(self, name, self.initial.get(name, None))
+            if name != 'data':
+                setattr(self, name, self.initial.get(name, None))
         self.asynchronous = getattr(self.metaclass, 'asynchronous', None) and self.request.GET.get('synchronous') is None
 
         related_field_name = getattr(self.metaclass, 'related_field', None)
         if related_field_name:
             setattr(self.instance, related_field_name, self.instantiator)
             if related_field_name in self.fields:
                 del self.fields[related_field_name]
@@ -211,14 +212,18 @@
         if text:
             self.content['info'].append(text)
 
     def alert(self, text):
         if text:
             self.content['alert'].append(text)
 
+    def danger(self, text):
+        if text:
+            self.content['danger'].append(text)
+
     def parameters(self, index):
         values = None
         for token in self.request.path.split('/'):
             if values is not None:
                 values.append((token))
             if token.lower() == self.get_api_name():
                 values = []
@@ -519,16 +524,22 @@
             auto_reload=auto_reload, image=image
         )
         return metadata
 
     def get_method(self):
         return getattr(self.metaclass, 'method', 'post') if hasattr(self, 'Meta') else 'post'
 
-    def get_instructions(self):
-        return None
+    def get_instances(self):
+        if self.instance:
+            return [self.instance]
+        elif self.instances is not None:
+            return self.instances
+        elif self.queryset is not None:
+            return self.queryset
+        return []
 
     def is_modal(self):
         return getattr(self.metaclass, 'modal', True) if hasattr(self, 'Meta') else True
 
     def has_permission(self, user):
         return user.is_superuser
 
@@ -774,15 +785,15 @@
         if self.instances:
             for instance in self.instances:
                 self.instance = instance
                 self._post_clean()
                 self.save()
         else:
             self.save()
-        self.message('Ação realizada com sucesso.')
+        self.message()
         self.redirect()
 
     def process(self):
         try:
             return self.check_ouput(self.submit(), True)
         except forms.ValidationError as e:
             if self.request.path.startswith('/app/'):
```

### Comparing `sloth-framework-0.1.2/sloth/actions/fields.py` & `sloth-framework-0.1.3/sloth/actions/fields.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/actions/inputs.py` & `sloth-framework-0.1.3/sloth/actions/inputs.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/__init__.py` & `sloth-framework-0.1.3/sloth/api/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/actions.py` & `sloth-framework-0.1.3/sloth/api/actions.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/backends/__init__.py` & `sloth-framework-0.1.3/sloth/api/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/dashboard.py` & `sloth-framework-0.1.3/sloth/api/dashboard.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -201,23 +201,23 @@
         self._load('tools', items, modal=modal, app=app)
 
     def plus_menu(self, *items, modal=True, app=None):
         self._load('plus', items, modal=modal, app=app)
 
     def navigation(self, *items, app=None):
         if mobile(self.request):
-            self._load('floating', items, app=app)
-        else:
             self._load('navigation', items, app=app)
+        else:
+            self._load('floating', items, app=app)
 
     def add_navigation(self, url, label, icon, app=None):
         if mobile(self.request):
-            self._item('floating', url, label, icon, app=app)
-        else:
             self._item('navigation', url, label, icon, app=app)
+        else:
+            self._item('floating', url, label, icon, app=app)
 
     def settings_menu(self, *items, modal=True, app=None):
         self._load('settings', items, modal=modal, app=app)
 
     def append(self, data, aside=False, grid=1):
         if inspect.isclass(data) and issubclass(data, Action):
             action = data(request=self.request)
```

### Comparing `sloth-framework-0.1.2/sloth/api/management/commands/cloud.py` & `sloth-framework-0.1.3/sloth/api/management/commands/cloud.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/management/commands/query.py` & `sloth-framework-0.1.3/sloth/api/management/commands/query.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/management/commands/send_web_push_notification.py` & `sloth-framework-0.1.3/sloth/api/management/commands/send_web_push_notification.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/management/commands/startserver.py` & `sloth-framework-0.1.3/sloth/api/management/commands/startserver.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/management/commands/sync.py` & `sloth-framework-0.1.3/sloth/api/management/commands/sync.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/migrations/0001_initial.py` & `sloth-framework-0.1.3/sloth/api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/migrations/0002_role_user.py` & `sloth-framework-0.1.3/sloth/api/migrations/0002_role_user.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/migrations/0003_alter_application_user.py` & `sloth-framework-0.1.3/sloth/api/migrations/0003_alter_application_user.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/migrations/0004_task.py` & `sloth-framework-0.1.3/sloth/api/migrations/0004_task.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/migrations/0005_task_stopped_alter_task_message.py` & `sloth-framework-0.1.3/sloth/api/migrations/0005_task_stopped_alter_task_message.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/migrations/0006_role_active_alter_role_name_alter_role_scope_key_and_more.py` & `sloth-framework-0.1.3/sloth/api/migrations/0006_role_active_alter_role_name_alter_role_scope_key_and_more.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/migrations/0007_alter_scope_description_alter_task_error.py` & `sloth-framework-0.1.3/sloth/api/migrations/0007_alter_scope_description_alter_task_error.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/migrations/0008_alter_application_available_scopes_and_more.py` & `sloth-framework-0.1.3/sloth/api/migrations/0008_alter_application_available_scopes_and_more.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/migrations/0009_pushnotification.py` & `sloth-framework-0.1.3/sloth/api/migrations/0009_pushnotification.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/migrations/0010_alter_pushnotification_user.py` & `sloth-framework-0.1.3/sloth/api/migrations/0010_alter_pushnotification_user.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/migrations/0011_alter_application_client_secret.py` & `sloth-framework-0.1.3/sloth/api/migrations/0011_alter_application_client_secret.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/migrations/0012_authcode.py` & `sloth-framework-0.1.3/sloth/api/migrations/0012_authcode.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/migrations/0013_task_partial_task_total.py` & `sloth-framework-0.1.3/sloth/api/migrations/0013_task_partial_task_total.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/migrations/0014_email.py` & `sloth-framework-0.1.3/sloth/api/migrations/0014_email.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/models.py` & `sloth-framework-0.1.3/sloth/api/models.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/css/all.min.css` & `sloth-framework-0.1.3/sloth/api/static/css/all.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/css/bootstrap-icons.css` & `sloth-framework-0.1.3/sloth/api/static/css/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/css/bootstrap.min.css` & `sloth-framework-0.1.3/sloth/api/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/css/colorpick.min.css` & `sloth-framework-0.1.3/sloth/api/static/css/colorpick.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/css/fonts/Eina02-Bold.f8011405.ttf` & `sloth-framework-0.1.3/sloth/api/static/css/fonts/Eina02-Bold.f8011405.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/css/fonts/Eina02-Regular.2e682693.ttf` & `sloth-framework-0.1.3/sloth/api/static/css/fonts/Eina02-Regular.2e682693.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf` & `sloth-framework-0.1.3/sloth/api/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/css/fonts/bootstrap-icons.woff` & `sloth-framework-0.1.3/sloth/api/static/css/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/css/fonts/bootstrap-icons.woff2` & `sloth-framework-0.1.3/sloth/api/static/css/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/css/icons.svg` & `sloth-framework-0.1.3/sloth/api/static/css/icons.svg`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/css/images/ui-icons_444444_256x240.png` & `sloth-framework-0.1.3/sloth/api/static/css/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/css/images/ui-icons_555555_256x240.png` & `sloth-framework-0.1.3/sloth/api/static/css/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/css/jquery-ui.css` & `sloth-framework-0.1.3/sloth/api/static/css/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/css/leaflet.css` & `sloth-framework-0.1.3/sloth/api/static/css/leaflet.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/css/select2.min.css` & `sloth-framework-0.1.3/sloth/api/static/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/css/sloth.css` & `sloth-framework-0.1.3/sloth/api/static/css/sloth.css`

 * *Files 2% similar despite different names*

```diff
@@ -173,14 +173,17 @@
     height: 38px;
     border: 1px solid #ced4da;
     border-radius: 4px;
 }
 .search-and-filters form>div {
     display: inline;
 }
+.search-and-filters .filter.mobile, .search-and-filters .filter.mobile .btn{
+    width: 100%;
+}
 .search-and-filters .filter {
     display: inline-block;
     margin-right: 10px;
     padding: 0;
     margin-bottom: 5px;
 }
 .search-and-filters .filter .fa-calendar{
@@ -257,18 +260,20 @@
     margin: 5px;
 }
 
 .select2-selection__clear{
     margin-top: 8px;
     padding-right: 12px !important;
 }
-
+#search, .search-menu{
+    border-radius: 0;
+}
 .search-results{
     position: absolute;
-    top: 50;
+    top: 57;
     z-index: 1;
     max-height: 300px;
     overflow-y: scroll;
     border-bottom: solid 1px #ced4da;
 }
 .search-results a{
     text-decoration: none;
@@ -277,14 +282,17 @@
 dl dl {
     margin-left: 10px;
 }
 
 textarea{
     width: 100%;
 }
+.form-display{
+    margin-bottom: 10;
+}
 .form-display .valueset-header{
     display: none;
 }
 .form-display .valueset .col{
     padding-right: 0;
     padding-left: 0;
 }
@@ -428,15 +436,15 @@
 
 .fieldset-inline-action .action-wrapper fieldset, .fieldset-tab .box,
 #login-wrapper fieldset{
     box-shadow: none;
     padding: 0;
 }
 
-.admin-queryset .queryset-data, .admin-queryset .search-and-filters form,
+.admin-queryset .queryset-data, .admin-queryset .search-and-filters form.with-filter,
 .fieldset-inline-action, .action-wrapper fieldset, .cards-wrapper,
 .shortcut-wrapper, .fieldset-list, .fieldset-group, .box,
 .valueset-fieldsets > reloadable-fieldset:not(.box){
 	background-color: white;
 	box-shadow: 0px 16px 32px 0px #001E3C0A;
 	border-radius: 8px;
 	padding: 20px;
@@ -467,8 +475,14 @@
 
 #login-wrapper .btn{
     width: 100%;
 }
 
 #login-wrapper h2{
     text-align: center;
+}
+
+.accordion-button:not(.collapsed), .accordion-button:focus{
+	border-color: white;
+	background-color: white;
+	box-shadow: none;
 }
```

### Comparing `sloth-framework-0.1.2/sloth/api/static/css/trumbowyg.min.css` & `sloth-framework-0.1.3/sloth/api/static/css/trumbowyg.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/icons/fontawesome/fontawesome.min.css` & `sloth-framework-0.1.3/sloth/api/static/icons/fontawesome/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/icons/fontawesome/fontawesome.min.js` & `sloth-framework-0.1.3/sloth/api/static/icons/fontawesome/fontawesome.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.ttf` & `sloth-framework-0.1.3/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.woff2` & `sloth-framework-0.1.3/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.ttf` & `sloth-framework-0.1.3/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.woff2` & `sloth-framework-0.1.3/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.ttf` & `sloth-framework-0.1.3/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.woff2` & `sloth-framework-0.1.3/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/icons/materialicons/LDItaoyNOAY6Uewc665JcIzCKsKc_M9flwmPq_HTTw.woff2` & `sloth-framework-0.1.3/sloth/api/static/icons/materialicons/LDItaoyNOAY6Uewc665JcIzCKsKc_M9flwmPq_HTTw.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/icons/materialicons/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2` & `sloth-framework-0.1.3/sloth/api/static/icons/materialicons/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/icons/materialicons/gok-H7zzDkdnRel8-DQ6KAXJ69wP1tGnf4ZGhUcel5euIg.woff2` & `sloth-framework-0.1.3/sloth/api/static/icons/materialicons/gok-H7zzDkdnRel8-DQ6KAXJ69wP1tGnf4ZGhUcel5euIg.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/icons/materialicons/materialicons.css` & `sloth-framework-0.1.3/sloth/api/static/icons/materialicons/materialicons.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/icons/materialicons/oPWQ_lt5nv4pWNJpghLP75WiFR4kLh3kvmvRImcycg.woff2` & `sloth-framework-0.1.3/sloth/api/static/icons/materialicons/oPWQ_lt5nv4pWNJpghLP75WiFR4kLh3kvmvRImcycg.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/images/click.png` & `sloth-framework-0.1.3/sloth/api/static/images/click.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/images/hand.png` & `sloth-framework-0.1.3/sloth/api/static/images/hand.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/images/icon.png` & `sloth-framework-0.1.3/sloth/api/static/images/icon.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/images/icon.svg` & `sloth-framework-0.1.3/sloth/api/static/images/icon.svg`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/images/images/badge.png` & `sloth-framework-0.1.3/sloth/api/static/images/images/badge.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/images/images/icon.png` & `sloth-framework-0.1.3/sloth/api/static/images/images/icon.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/images/login.jpeg` & `sloth-framework-0.1.3/sloth/api/static/images/login.jpeg`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/images/logo.png` & `sloth-framework-0.1.3/sloth/api/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/images/logo.svg` & `sloth-framework-0.1.3/sloth/api/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/images/no-image.png` & `sloth-framework-0.1.3/sloth/api/static/images/no-image.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/images/sloth.png` & `sloth-framework-0.1.3/sloth/api/static/images/sloth.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/images/user.png` & `sloth-framework-0.1.3/sloth/api/static/images/user.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/js/api.js` & `sloth-framework-0.1.3/sloth/api/static/js/api.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/js/bootstrap.bundle.min.js` & `sloth-framework-0.1.3/sloth/api/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/js/colorpick.min.js` & `sloth-framework-0.1.3/sloth/api/static/js/colorpick.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/js/i18n/pt-BR.js` & `sloth-framework-0.1.3/sloth/api/static/js/i18n/pt-BR.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/js/jquery-3.6.0.min.js` & `sloth-framework-0.1.3/sloth/api/static/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/js/jquery-ui.js` & `sloth-framework-0.1.3/sloth/api/static/js/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/js/jquery.binarytransport.js` & `sloth-framework-0.1.3/sloth/api/static/js/jquery.binarytransport.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/js/jquery.mask.min.js` & `sloth-framework-0.1.3/sloth/api/static/js/jquery.mask.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/js/jquery.timepicker.js` & `sloth-framework-0.1.3/sloth/api/static/js/jquery.timepicker.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/js/leaflet.js` & `sloth-framework-0.1.3/sloth/api/static/js/leaflet.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/js/masonry.pkgd.min.js` & `sloth-framework-0.1.3/sloth/api/static/js/masonry.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/js/popper.min.js` & `sloth-framework-0.1.3/sloth/api/static/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/js/qr-scanner-worker.min.js` & `sloth-framework-0.1.3/sloth/api/static/js/qr-scanner-worker.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/js/qr-scanner.min.js` & `sloth-framework-0.1.3/sloth/api/static/js/qr-scanner.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/js/qrcode.min.js` & `sloth-framework-0.1.3/sloth/api/static/js/qrcode.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/js/select2.min.js` & `sloth-framework-0.1.3/sloth/api/static/js/select2.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/js/sloth.js` & `sloth-framework-0.1.3/sloth/api/static/js/sloth.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -67,16 +67,18 @@
         $(this).request(url, method || 'GET', data || {}, function(html) {
             $('#modal').find('.modal-body').html(html).initialize();
             if ($('.modal-body input[type=text]:first').length > 0) {
                 window.setTimeout(function() {
                     //$('.modal-body').find('input[type=text], input[type=number]').first().focus();
                 }, 200);
             }
+            $('#modal').on('shown.bs.modal', function(e) {
+                $('#modal').responsive()
+            });
             $('#modal').modal('show');
-            document.getElementById('modal').addEventListener('hidden.bs.modal', function(event) {});
         });
     },
     reloadAreas(areas) {
         if (areas != null) {
             $('.reloadable-fieldset').map(function(i, item) {
                 if (areas.indexOf(item.id) >= 0 || areas.length == 0) {
                     $.get($(item).data('path'), function(html) {
```

### Comparing `sloth-framework-0.1.2/sloth/api/static/js/sw.js` & `sloth-framework-0.1.3/sloth/api/static/js/sw.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/js/tests.js` & `sloth-framework-0.1.3/sloth/api/static/js/tests.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/js/trumbowyg.min.js` & `sloth-framework-0.1.3/sloth/api/static/js/trumbowyg.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/static/js/wpn.js` & `sloth-framework-0.1.3/sloth/api/static/js/wpn.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/tasks/__init__.py` & `sloth-framework-0.1.3/sloth/api/tasks/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 class Task(Thread):
 
     def __init__(self, *args, **kwargs):
         self.total = 0
         self.partial = 0
         self.previous = 0
         self.task_id = None
+        self._message = None
         super().__init__(*args, **kwargs)
 
     def start(self, request):
         task = TaskModel.objects.create(name=self.get_name(), user=request.user)
         self.task_id = task.id
         super().start()
 
@@ -32,15 +33,18 @@
         if cache.get('task_{}_stopped'.format(self.task_id)) is None:
             if self.partial == 0:
                 TaskModel.objects.filter(pk=self.task_id).update(total=self.total)
             self.partial += 1
             progress = 100 if self.total == 0 else int(self.partial / self.total * 100)
             if (self.previous == 0 and progress) or (progress - self.previous) >= self.get_update_progress_interval() or self.partial % 1000 == 0 or progress == 100:
                 self.previous = progress
-                TaskModel.objects.filter(pk=self.task_id).update(progress=progress, partial=self.partial)
+                kwargs = dict(progress=progress, partial=self.partial)
+                if self._message:
+                    kwargs.update(message=self._message)
+                TaskModel.objects.filter(pk=self.task_id).update(**kwargs)
             return True
         return False
 
     def iterate(self, iterable):
         if hasattr(iterable, 'model') and hasattr(iterable, 'count'):
             self.total = iterable.count()
         else:
@@ -48,15 +52,15 @@
         for obj in iterable:
             if self.running():
                 yield obj
             else:
                 break
 
     def message(self, text):
-        TaskModel.objects.filter(pk=self.task_id).update(message=text)
+        self._message = text
 
     def finalize(self, text='Ação realizada com sucesso'):
         TaskModel.objects.filter(pk=self.task_id).update(message=text, end=datetime.datetime.now(), partial=self.partial)
 
     def error(self, text, exception=None):
         if exception:
             traceback.print_exc()
```

### Comparing `sloth-framework-0.1.2/sloth/api/templates/actions/execute_query.html` & `sloth-framework-0.1.3/sloth/api/templates/actions/execute_query.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/templates/actions/show_icons.html` & `sloth-framework-0.1.3/sloth/api/templates/actions/show_icons.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/templates/api/index.html` & `sloth-framework-0.1.3/sloth/api/templates/api/index.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/templates/charts/bar.html` & `sloth-framework-0.1.3/sloth/api/templates/charts/bar.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/templates/charts/column.html` & `sloth-framework-0.1.3/sloth/api/templates/charts/column.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/templates/charts/pie.html` & `sloth-framework-0.1.3/sloth/api/templates/charts/pie.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {% load tags %}
 {% for key, series in data.normalized.items %}
 <style>
-    #container-{{ forloop.counter }} .pie-chart {
+    #container{{ data.key }}-{{ forloop.counter }} .pie-chart {
       background:
         conic-gradient(
           {% for serie in series %}
             {% if forloop.first %}
               {{ serie.color }} {{ serie.end }}%,
             {% endif %}
             {% if not forloop.first and not forloop.last  %}
@@ -18,28 +18,28 @@
         );
       margin: auto;
       border-radius: 50%;
       width: 150;
       height: 150;
       margin-top: -62px;
     }
-    #container-{{ forloop.counter }} .pie-center{
+    #container{{ data.key }}-{{ forloop.counter }} .pie-center{
 
       top: 50px;
       width: 75px;
       height: 75px;
 
       position: relative;
       background: #FFF;
       border-radius: 50%;
       margin: auto;
       {% if donut is None %}visibility: hidden;{% endif %}
     }
 </style>
-<div style="width:100%" id="container-{{ forloop.counter }}">
+<div style="width:100%" id="container{{ data.key }}-{{ forloop.counter }}">
     {% if key != 'default' %}
     <h5>{{ key }}</h5>
     {% endif %}
     <div class="pie-center"></div>
     <div class="pie-chart"></div>
     {% include "charts/legend.html" %}
 </div>
```

### Comparing `sloth-framework-0.1.2/sloth/api/templates/dashboard/actions.html` & `sloth-framework-0.1.3/sloth/api/templates/dashboard/actions.html`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     $('#{{ target }}-{{ uuid }}-{{id}}').find('.action-button').on('mouseenter', function(){
         if($(this).hasClass('instance')){
             this.href = actionURL($(this).data('url').replace('{id}', $(this).data('id')));
         }
         if($(this).hasClass('queryset')){
             var ids = $('#queryset-{{ uuid }}').find('.action-checkbox:checked').map(function(){
               return $(this).val();
-            }).get().filter(function (id) { return id!='on' }).join('-');
+            }).get().filter(function (id) { return id!='' }).join('-');
             this.href = actionURL($(this).data('url').replace('{id}', '0-'+ids));
         }
         if($(this).hasClass('model')){
             this.href = actionURL($(this).data('url'));
         }
     });
 </script>
```

### Comparing `sloth-framework-0.1.2/sloth/api/templates/dashboard/apps.html` & `sloth-framework-0.1.3/sloth/api/templates/dashboard/apps.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/templates/dashboard/base.html` & `sloth-framework-0.1.3/sloth/api/templates/dashboard/base.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/templates/dashboard/bottom.html` & `sloth-framework-0.1.3/sloth/api/templates/dashboard/bottom.html`

 * *Files 4% similar despite different names*

```diff
@@ -46,48 +46,45 @@
 }
 
 .bottom-navbar {
   overflow: hidden;
   position: fixed;
   bottom: 0;
   width: 100%;
-  background-color: #cfe2ff;
-  border-top: 1px solid #dee2e6;
   z-index: 101;
 }
 
 .bottom-navbar a {
   float: left;
   display: block;
   text-align: center;
   text-decoration: none;
   width: {% widthratio 100 dashboard.data.navigation|length 1 %}%;
-  height: 100;
   font-size: 12px;
 }
 
 .bottom-navbar a.active {
-  color: #333;
+  color: white;
 }
 
 .bottom-navbar a:hover {
-  color: #0d6efd;
+  color: white;
 }
 
 .bottom-navbar a i{
   font-size: 2rem;
 }
 
 .bottom-navbar div{
   padding: 10px;
 }
 
 </style>
 
-<div class="bottom-navbar">
+<div class="bottom-navbar bg-primary">
   {% for item in dashboard.data.navigation %}
   <a href="{{ item.url }}" class="active">
     <div>
       {{ item.icon|icontag }}
       <p>{{ item.label }}</p>
     </div>
   </a>
```

### Comparing `sloth-framework-0.1.2/sloth/api/templates/dashboard/cards.html` & `sloth-framework-0.1.3/sloth/api/templates/dashboard/cards.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/templates/dashboard/footer.html` & `sloth-framework-0.1.3/sloth/api/templates/dashboard/footer.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/templates/dashboard/form.html` & `sloth-framework-0.1.3/sloth/api/templates/dashboard/form.html`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     <div class="alert alert-primary" role="alert">{{ text|breaklines|safe }}</div>
 {% endfor %}
 
 {% for text in self.content.alert %}
     <div class="alert alert-warning" role="alert">{{ text|breaklines|safe }}</div>
 {% endfor %}
 
+{% for text in self.content.danger %}
+    <div class="alert alert-danger" role="alert">{{ text|breaklines|safe }}</div>
+{% endfor %}
+
 <div class="form-display">
 {% for item in self.content.center %}{{ item }}{% endfor %}
 </div>
 
 {% if self.show_form %}
 <form id="{{ self.get_metadata.key|slugify }}" action="{{ self.get_full_path }}" method="{{ self.get_method }}" novalidate="novalidate" class="{% if self.get_metadata.ajax %}form{% endif %} form-{{ self.get_metadata.name|slugify }}" enctype="multipart/form-data">
     <input type="hidden" name="{{ self.get_metadata.key }}" value="{{ self.dumps }}">
```

#### html2text {}

```diff
@@ -9,14 +9,16 @@
 ***** {{ self.get_metadata.icon|icontag }} {{ title }} *****
 {% endif %} {% endwith %} {% if self.get_image %}
                             [{{ self.get_image }}]
 {% endif %} {% for text in self.content.info %}
 {{ text|breaklines|safe }}
 {% endfor %} {% for text in self.content.alert %}
 {{ text|breaklines|safe }}
+{% endfor %} {% for text in self.content.danger %}
+{{ text|breaklines|safe }}
 {% endfor %}
 {% for item in self.content.center %}{{ item }}{% endfor %}
 {% if self.show_form %}
  {% if self.get_metadata.method == "post" %} {% csrf_token %} {% endif %} {% if
 self.non_field_errors %}
 {{ self.non_field_errors }}
 {% endif %} {% for hidden_field in self.hidden_fields %} {{ hidden_field.errors
```

### Comparing `sloth-framework-0.1.2/sloth/api/templates/dashboard/grids.html` & `sloth-framework-0.1.3/sloth/api/templates/dashboard/grids.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/templates/dashboard/header.html` & `sloth-framework-0.1.3/sloth/api/templates/dashboard/header.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/templates/dashboard/links.html` & `sloth-framework-0.1.3/sloth/api/templates/dashboard/links.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/templates/dashboard/messages.html` & `sloth-framework-0.1.3/sloth/api/templates/dashboard/messages.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/templates/dashboard/modal.html` & `sloth-framework-0.1.3/sloth/api/templates/dashboard/modal.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/templates/dashboard/plus.html` & `sloth-framework-0.1.3/sloth/api/templates/dashboard/plus.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/templates/dashboard/report.html` & `sloth-framework-0.1.3/sloth/api/templates/dashboard/report.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/templates/dashboard/search.html` & `sloth-framework-0.1.3/sloth/api/templates/dashboard/search.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/templates/dashboard/settings.html` & `sloth-framework-0.1.3/sloth/api/templates/dashboard/settings.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/templates/dashboard/shortcuts.html` & `sloth-framework-0.1.3/sloth/api/templates/dashboard/shortcuts.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/templates/dashboard/tasks.html` & `sloth-framework-0.1.3/sloth/api/templates/dashboard/tasks.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/templates/dashboard/tools.html` & `sloth-framework-0.1.3/sloth/api/templates/dashboard/tools.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/templates/inputs/picker.html` & `sloth-framework-0.1.3/sloth/api/templates/inputs/picker.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/templates/inputs/qrcode.html` & `sloth-framework-0.1.3/sloth/api/templates/inputs/qrcode.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/templates/inputs/select.html` & `sloth-framework-0.1.3/sloth/api/templates/inputs/select.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/templates/queryset/accordion.html` & `sloth-framework-0.1.3/sloth/api/templates/queryset/accordion.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/templates/queryset/calendar.html` & `sloth-framework-0.1.3/sloth/api/templates/queryset/calendar.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/templates/queryset/cards.html` & `sloth-framework-0.1.3/sloth/api/templates/queryset/cards.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/templates/queryset/datatable.html` & `sloth-framework-0.1.3/sloth/api/templates/queryset/datatable.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/templates/queryset/filter.html` & `sloth-framework-0.1.3/sloth/api/templates/queryset/filter.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {% load tags %}
-<div class="filter {% if metadata.hidden %}d-none{% endif %}">
+<div class="filter {% if metadata.hidden %}d-none{% endif %} {% if request|mobile %}mobile{% endif %}">
     <label>{{ metadata.name|truncatechars:25 }}</label>
     {% if metadata.type == "choices" %}
     <select name="{{ metadata.key }}" class="{{ metadata.key }}-{{ data.uuid }}">
         {% if metadata.choices %}
             <option value=""></option>
             {% for choice in metadata.choices %}
                 <option {% if metadata.value.1 == choice.id %}selected{% endif %} value="{{ choice.id|stringformat:'s' }}">{{ choice.text }}</option>
```

### Comparing `sloth-framework-0.1.2/sloth/api/templates/queryset/filters.html` & `sloth-framework-0.1.3/sloth/api/templates/queryset/filters.html`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <style>
 {% if data.metadata.collapsed  %}
     #search-and-filters-{{ data.uuid }}.search-and-filters form{display: none}
 {% endif %}
 </style>
 
         <div class="search-and-filters" id="search-and-filters-{{ data.uuid }}">
-            <form method="get" id="form-{{ data.uuid }}" action="{{ data.path }}" style="{% if data.metadata.collapsed %}display:none{% endif %}">
+            <form method="get" id="form-{{ data.uuid }}" action="{{ data.path }}" style="{% if data.metadata.collapsed %}display:none{% endif %}" class="{% if data.metadata.search or data.metadata.filters %}with-filter{% endif %}">
                 <input type="hidden" name="uuid" value="{{ data.uuid }}">
                 <input type="hidden" name="is_admin" value="{% if data.metadata.is_admin %}1{% endif %}">
                 <input type="hidden" name="collapsed" value="{% if data.metadata.collapsed %}1{% endif %}" id="collapsed-{{ data.uuid }}">
                 <input type="hidden" name="page" value="{{ data.page }}" id="pagination-{{ data.uuid }}">
                 <input type="hidden" name="compact" value="{% if compact or request.GET.compact or request|mobile %}1{%endif%}">
                 <input type="hidden" name="subset" value="{{ data.metadata.subset }}" id="subset-{{ data.uuid }}">
                 <input type="hidden" name="selected-date" value="" id="selected-date-{{ data.uuid }}">
@@ -18,23 +18,23 @@
                     {% if k != 'csrfmiddlewaretoken' %}
                         <input type="hidden" name="post__{{ k }}" value="{{ v }}">
                     {% endif %}
                 {% endfor %}-->
                 {% if data.metadata.search or data.metadata.filters %}
                     <div class="filters" id="filters-{{ data.uuid }}">
                         {% if data.metadata.search %}
-                            <div class="filter">
+                            <div class="filter {% if request|mobile %}mobile{% endif %}">
                                 <label>Busca</label>
                                 <input type="text" class="form-control" pattern=".{3,}" name="q" value="{{ request.GET.q|default:'' }}" id="searchbar" title="3 ou mais caracteres" onkeypress="if(event.which==13){reload{{ data.uuid }}();return false;}" placeholder="">
                             </div>
                         {% endif %}
                         {% for metadata in data.metadata.filters.values %}
                             {% include "queryset/filter.html" %}
                         {% endfor %}
-                        <div class="filter">
+                        <div class="filter {% if request|mobile %}mobile{% endif %}">
                             <button type="button" class="btn btn-primary filter-button" onclick="$(this).find('.spinner-border').removeClass('d-none');$(this).find('i').addClass('d-none');$('#pagination-{{ data.uuid }}').val(1);reload{{ data.uuid }}()">
                                 <div class="spinner-border spinner-border-sm d-none" role="status">
                                   <span class="visually-hidden">Loading...</span>
                                 </div>
                                 <i class="bi bi-funnel"></i>
                                 Filtrar
                             </button>
```

### Comparing `sloth-framework-0.1.2/sloth/api/templates/queryset/queryset.html` & `sloth-framework-0.1.3/sloth/api/templates/queryset/queryset.html`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
                         success:function( html ) {
                             $('#{{ data.key }}').html($(html).find('#{{ data.key }}').html()).initialize();
                             $(document.body).removeClass('page-loading');
                         }
                     });
                 }
                 function toggleActions{{ data.uuid }}(input){
-                    if(input.value=='on') $('#queryset-{{ data.uuid }}').find('.action-checkbox').prop('checked', input.checked);
+                    if(input.value=='') $('#queryset-{{ data.uuid }}').find('.action-checkbox').prop('checked', input.checked);
                     if($('#queryset-{{ data.uuid }}').find('.action-checkbox:checked').length>0){
                         $('#queryset-{{ data.uuid }}').find('.dropdown-toggle.queryset').removeClass('disabled');
                         $('#queryset-{{ data.uuid }}').find('.dropdown-toggle.instance, .dropdown-toggle.model').addClass('disabled');
                         $('#queryset-{{ data.uuid }}').find('.btn.instance, .btn.model').addClass('disabled');
                         $('#queryset-{{ data.uuid }}').find('.btn.queryset').removeClass('disabled');
                     } else {
                         $('#queryset-{{ data.uuid }}').find('.dropdown-toggle.queryset').addClass('disabled');
@@ -127,20 +127,21 @@
         {% endfor %}
         <div class="clear-fix">&nbsp;</div>
     {% endif %}
 
     {% endif %}
 
     {% if data.template %}
+        <div class="clear-fix">&nbsp;</div>
         {% include data.template with data=data %}
     {% else %}
         {% include "queryset/datatable.html" with data=data %}
     {% endif %}
     {% include "queryset/actions/batch.html" %}
-    {% if data.metadata.pagination.pages|length > 1 and data.metadata.scrollable %}
+    {% if data.metadata.pagination.pages|length > 1 and not data.metadata.scrollable %}
 
         <nav aria-label="Paginação">
       <ul class="pagination" style="overflow-x:hidden">
         {% for page in data.metadata.pagination.pages %}
            {% if forloop.counter|add:3 == data.metadata.pagination.pages|length and not forloop.counter == 5 %}
             <li class="page-item disabled">
               <a class="page-link" href="#" tabindex="-1" aria-disabled="true">...</a>
```

#### html2text {}

```diff
@@ -24,18 +24,20 @@
    {% if data.metadata.search or data.metadata.filters %}  {% endif %}
 {% if data.metadata.calendar %} {% include "queryset/calendar.html" with
 data=data %} {% endif %} {% if data.metadata.aggregations %} {% for aggregation
 in data.metadata.aggregations.values %}
 **** {{ aggregation.name }}: {{ aggregation.value|format }} ****
 {% endfor %}
  
-{% endif %} {% endif %} {% if data.template %} {% include data.template with
-data=data %} {% else %} {% include "queryset/datatable.html" with data=data %}
-{% endif %} {% include "queryset/actions/batch.html" %} {% if
-data.metadata.pagination.pages|length > 1 and data.metadata.scrollable %}
+{% endif %} {% endif %} {% if data.template %}
+ 
+{% include data.template with data=data %} {% else %} {% include "queryset/
+datatable.html" with data=data %} {% endif %} {% include "queryset/actions/
+batch.html" %} {% if data.metadata.pagination.pages|length > 1 and not
+data.metadata.scrollable %}
     * {% for page in data.metadata.pagination.pages %} {% if
       forloop.counter|add:3 == data.metadata.pagination.pages|length and not
       forloop.counter == 5 %}
     * ...
     * {% endif %}
     * {{_page_}}
     * {% if forloop.counter == 4 %}
```

### Comparing `sloth-framework-0.1.2/sloth/api/templates/queryset/rows.html` & `sloth-framework-0.1.3/sloth/api/templates/queryset/rows.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/templates/queryset/scroll.html` & `sloth-framework-0.1.3/sloth/api/templates/queryset/scroll.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/templates/queryset/statistics.html` & `sloth-framework-0.1.3/sloth/api/templates/queryset/statistics.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% load tags %}
 <div class="reloadable-fieldset box" id="{{ data.key }}" data-path="{{ data.path }}">
 <div id="statistics-{{ data.uuid }}">
 {% if uuid is None or request.GET.uuid is None %}
     {% if data.name %}
         <div class="fieldset-title" onclick="$(this).parent().find('.toogle-data').slideToggle();$(this).find('i').toggleClass('bi-chevron-down').toggleClass('bi-chevron-right');">
-          <h5><i class="bi bi-chevron-down"></i>{{ data.name }}</h5>
+          <h5><i class="bi bi-chevron-down"></i> {{ data.name }}</h5>
         </div>
     {% endif %}
     <div class="card-text fieldset-data toogle-data" id="{{ fieldset.name|slugify }}-statistics">
 {% endif %}
         {% if data.series %}
             {% if data.template %}
                 {% include data.template with data=data %}
@@ -60,33 +60,54 @@
                         </thead>
                         {% for name, value, color in data.series.default %}
                         <tr>
                             <th scope="col">{{ name }}</th>
                             <td scope="col" class="align-middle" align="center">{{ value|format }}</td>
                         </tr>
                         {% endfor %}
+                        <tr>
+                            <th scope="col"></th>
+                            <th scope="col" class="align-middle" style="text-align:center">{{ data.tx.0|format }}</th>
+
+                        </tr>
                     {% else %}
                             {% for name, series in data.series.items %}
                                 {% if forloop.first %}
                                     <thead>
                                     <tr>
                                         <td scope="col"></td>
                                         {% for name, value, color in series %}
                                             <th scope="col" class="align-middle" style="text-align:center">{{ name }}</th>
                                         {% endfor %}
+                                        {% if data.ty %}
+                                            <td scope="col"></td>
+                                        {% endif %}
                                     </tr>
                                     </thead>
                                 {% endif %}
                                 <tr>
                                     <th scope="col">{{ name }}</th>
                                     {% for name, value, color in series %}
-                                        <td scope="col" class="align-middle" align="center">{{ value|format }}</td>
+                                        <td scope="col" class="align-middle" align="center">
+                                            {{ value|format }}
+                                        </td>
+                                    {% endfor %}
+                                    {% for total in data.ty %}
+                                        {% if forloop.parentloop.counter0 == forloop.counter0 %}
+                                        <th scope="col" class="align-middle" style="text-align:center">
+                                            {{ total|format }}
+                                        </th>
+                                        {% endif %}
                                     {% endfor %}
                                 </tr>
                             {% endfor %}
+                            {% for total in data.tx %}
+                                {% if forloop.first %}<td scope="col"></td>{% endif %}
+                                <th scope="col" class="align-middle" style="text-align:center">{{ total|format }}</th>
+                            {% endfor %}
                     {% endif %}
                 </table>
             {% endif %}
         {% else %}
             <div class="alert alert-primary" role="alert">Nenhum registro encontrado.</div>
         {% endif %}
     </div>
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
 {% load tags %}
 {% if uuid is None or request.GET.uuid is None %} {% if data.name %}
-{{ data.name }}
+ {{ data.name }}
 {% endif %}
 {% endif %} {% if data.series %} {% if data.template %} {% include
 data.template with data=data %} {% else %} {% if 0 %}
 {% for name, metadata in data.filters.items %} {% include "queryset/
 filter.html" %} {% endfor %}
 Loading...
  Filtrar
  {% endif %}
            Total
-{{ name }} {{ value|format }}
+{{ name }}    {{ value|format }}
+           {{ data.tx.0|format }}
            {{ name }}
-{{ name }} {{ value|format }}
+{{ name }}    {{ value|format }}  {{ total|format }}
 {% endif %} {% else %}
 Nenhum registro encontrado.
 {% endif %}
 {% if uuid is None or request.GET.uuid is None %} {% endif %}
```

### Comparing `sloth-framework-0.1.2/sloth/api/templates/queryset/timeline.html` & `sloth-framework-0.1.3/sloth/api/templates/queryset/timeline.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/templates/renderers/calendar/calendar.html` & `sloth-framework-0.1.3/sloth/api/templates/renderers/calendar/calendar.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/templates/renderers/maps/map.html` & `sloth-framework-0.1.3/sloth/api/templates/renderers/maps/map.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/templates/renderers/programing/strtable.html` & `sloth-framework-0.1.3/sloth/api/templates/renderers/programing/strtable.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/templates/renderers/utils/steps.html` & `sloth-framework-0.1.3/sloth/api/templates/renderers/utils/steps.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/templates/renderers/utils/table.html` & `sloth-framework-0.1.3/sloth/api/templates/renderers/utils/table.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/templates/themes/dark.html` & `sloth-framework-0.1.3/sloth/api/templates/themes/dark.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/templates/valueset/fieldset-group.html` & `sloth-framework-0.1.3/sloth/api/templates/valueset/fieldset-group.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/templates/valueset/fieldset-list.html` & `sloth-framework-0.1.3/sloth/api/templates/valueset/fieldset-list.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/templates/valueset/fieldset.html` & `sloth-framework-0.1.3/sloth/api/templates/valueset/fieldset.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/templates/valueset/value.html` & `sloth-framework-0.1.3/sloth/api/templates/valueset/value.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 {% load tags %}
 
 {% if v|is_valueset %}
     <dl>
-    {% for v2 in v.values %}
-        {% if v2.metadata.icon %}
-            <dt></dt>
-            <dd>
-            {{ v2.metadata.icon|icontag }}
-            {% if v2.template %}
-                {% include v2.template with value=v2.value metadata=v2.metadata %}
-            {% else %}
-                {{ v2.value|format|linebreaksbr }}
-            {% endif %}
-            </dd>
-        {% else %}
-            <dt>{{ v2.name }}</dt>
-            <dd>
+    {% for k2, v2 in v.items %}
+        {% if k2 != 'instance' %}
+            {% if v2.metadata.icon %}
+                <dt></dt>
+                <dd>
+                {{ v2.metadata.icon|icontag }}
                 {% if v2.template %}
                     {% include v2.template with value=v2.value metadata=v2.metadata %}
                 {% else %}
                     {{ v2.value|format|linebreaksbr }}
                 {% endif %}
-            </dd>
+                </dd>
+            {% else %}
+                <dt>{{ v2.name }}</dt>
+                <dd>
+                    {% if v2.template %}
+                        {% include v2.template with value=v2.value metadata=v2.metadata %}
+                    {% else %}
+                        {{ v2.value|format|linebreaksbr }}
+                    {% endif %}
+                </dd>
+            {% endif %}
         {% endif %}
     {% endfor %}
     </dl>
 {% else %}
     {% if v.template %}
         {% include v.template with value=v.value metadata=v.metadata %}
     {% else %}
```

### Comparing `sloth-framework-0.1.2/sloth/api/templates/valueset/valueset.html` & `sloth-framework-0.1.3/sloth/api/templates/valueset/valueset.html`

 * *Files 1% similar despite different names*

```diff
@@ -15,24 +15,24 @@
                             <h2>{{ data.title.value }}</h2>
                         {% endif %}
                     </div>
                 {% else %}
                     <h2>{{ data.icon|icontag }} {{ data.name }}</h2>
                 {% endif %}
                 {% if data.subtitle.value %}
-                    <div class="valueset-subtitle pb-1">
+                    <div class="valueset-subtitle pb-2">
                         {% if data.subtitle.template %}
                             {% include data.subtitle.template with value=data.subtitle.value metadata=data.subtitle.metadata %}
                         {% else %}
                             <div class="valueset-subtitle-text">{{ data.subtitle.value }}</div>
                         {% endif %}
                     </div>
                 {% endif %}
                 {% if data.status.value %}
-                    <div class="valueset-status pb-1">
+                    <div class="valueset-status pb-2">
                         {% if data.status.template %}
                             {% include data.status.template with value=data.status.value metadata=data.status.metadata %}
                         {% else %}
                             <div class="valueset-status-text">{{ data.status.value }}</div>
                         {% endif %}
                     </div>
                 {% endif %}
@@ -64,15 +64,15 @@
         </div>
         {% if data.template %}
             {% include data.template with data=data.data %}
         {% else %}
             {% if data.data %}
             <div class="valueset-fieldsets">
                 {% if data.data|has_only_primitive_fields %}
-                    <div class="box">
+                    <div class="box responsive-container">
                         {% for name, item in data.data.items %}
                             {% if item.template %}
                                 {% include item.template with value=item.value metadata=item.metadata %}
                             {% else %}
                                 {% include 'valueset/field.html' with v=item %}
                             {% endif %}
                         {% endfor %}
@@ -91,21 +91,21 @@
                         {% if item.type == 'queryset' %}
                             {% include 'valueset/fieldset.html' with data=item %}
                         {% endif %}
                         {% if item.type == 'statistics' %}
                             {% include 'valueset/fieldset.html' with data=item %}
                         {% endif %}
                         {% if item.type == 'primitive' %}
-                            <div class="reloadable-fieldset box" id="{{ item.key }}" data-path="{{ item.path }}">
                             {% if item.template %}
                                 {% include item.template with value=item.value metadata=item.metadata %}
                             {% else %}
-                                {% include 'valueset/field.html' with v=item %}
+                                <div class="reloadable-fieldset box responsive-container" id="{{ item.key }}" data-path="{{ item.path }}">
+                                    {% include 'valueset/field.html' with v=item %}
+                                </div>
                             {% endif %}
-                            </div>
                         {% endif %}
                     {% endfor %}
                 {% endif %}
             </div>
             {% endif %}
         {% endif %}
     </div>
```

### Comparing `sloth-framework-0.1.2/sloth/api/templatetags/tags.py` & `sloth-framework-0.1.3/sloth/api/templatetags/tags.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     return indexable[i]
 
 
 @register.filter
 def mobile(request):
     if request:
         width = int(request.COOKIES.get('width', 0))
-        return width if width < 600 else False
+        return width < 600
     return False
 
 
 @register.filter
 def tablet(request):
     if request:
         width = int(request.COOKIES.get('width', 0))
```

### Comparing `sloth-framework-0.1.2/sloth/api/urls.py` & `sloth-framework-0.1.3/sloth/api/urls.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/api/views.py` & `sloth-framework-0.1.3/sloth/api/views.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/cloud/printer.py` & `sloth-framework-0.1.3/sloth/cloud/printer.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/cloud/server.py` & `sloth-framework-0.1.3/sloth/cloud/server.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/conf/settings.py` & `sloth-framework-0.1.3/sloth/conf/settings.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/core/base.py` & `sloth-framework-0.1.3/sloth/core/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,16 +96,16 @@
         return getattr(self, 'autouser', None) == user
 
     ### VISUALIZATION ###
 
     def value_set(self, *names):
         return ValueSet(self, names)
 
-    def view(self):
-        names = [field.name for field in self.metaclass().fields]
+    def view(self, *names):
+        names = names or [field.name for field in self.metaclass().fields]
         return self.value_set(*names)
 
     def serialize(self, wrap=True):
         return self.view().serialize(wrap=wrap)
 
     def get_select_display(self):
         select_fields = getattr(type(self).metaclass(), 'select_fields', None)
```

### Comparing `sloth-framework-0.1.2/sloth/core/queryset.py` & `sloth-framework-0.1.3/sloth/core/queryset.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         if self.model and getattr(self.model.metaclass(), 'autouser', False):
             self.lookups(autouser='pk')
             self.ignore('autouser')
 
     def _clone(self):
         clone = super()._clone()
         clone.request = self.request
-        self.instantiator = self.instantiator
+        clone.instantiator = self.instantiator
         clone.metadata = dict(self.metadata)
         return clone
 
     def first(self):
         obj = super().first()
         if self.metadata['related_field'] and isinstance(obj, self.model):
             obj.related_field = self.metadata['related_field']
@@ -66,23 +66,28 @@
             self.metadata['lookups'].append((name, scopes))
         return self
 
     def lookups(self, name='Usuário', *names, **scopes):
         self.role_lookups(*((name,) + names), **scopes)
         return self
 
+    def readonly(self):
+        for key in ('actions', 'inline_actions', 'batch_actions'):
+            self.metadata[key].clear()
+        return self
+
     def has_permission(self, user):
         if user.is_authenticated:
             return user.is_superuser or user.roles.contains(*(t[0] for t in self.metadata['lookups']))
         return False
 
     def has_attr_permission(self, user, name):
         if user.is_superuser:
             return True
-        qs = self.model.objects.all()
+        qs = self.model.objects
         if name == 'all' or name in qs.metadata['attach']:
             return qs.has_permission(user)
         return getattr(self._clone(), name)().has_permission(user)
 
     def get_allowed_attrs(self, recursive=True):
         allowed = []
         for key in ('global_actions', 'actions', 'batch_actions', 'inline_actions'):
@@ -365,15 +370,15 @@
                 for view in self.metadata['view']:
                     if view['name'] == 'self':
                         has_view_permission = obj.has_view_permission(self.request.user)
                     else:
                         has_view_permission = obj.has_view_attr_permission(self.request.user, view['name'])
                     if self.request.user.is_superuser or has_view_permission or obj.has_permission(self.request.user):
                         actions.append(view['name'])
-            item = obj.value_set(*self.get_list_display(add_id=add_id)).load(wrap=False, detail=detail)
+            item = obj.value_set(*self.get_list_display(add_id=add_id)).contextualize(self.request).load(wrap=False, detail=detail)
             data.append(dict(id=obj.id, description=str(obj), data=item, actions=actions) if wrap else item)
         return data
 
     def export(self, limit=100):
         data = []
         header = []
         for i, obj in enumerate(self[0:limit]):
@@ -512,15 +517,15 @@
 
                 template = self.metadata['template']
                 if template is None:
                     template = getattr(self.model.metaclass(), 'list_template', None)
                 if template:
                     template = template if template.endswith('.html') else '{}.html'.format(template)
                     data.update(template=template)
-            # pprint(data)
+            # from pprint import pprint; pprint(data)
             return data
         return self.to_list(detail=False)
 
     def debug(self):
         print(json.dumps(self.serialize(wrap=True), indent=4, ensure_ascii=False))
 
     # metadata functions
@@ -537,14 +542,15 @@
         # self.metadata['uuid'] = slugify(name).replace('-', '_')
         self.metadata['verbose_name'] = pretty(name)
         return self
 
     def preview(self, *names, modal=True, icon=None):
         for name in names:
             if name:
+                self.metadata['view'] = list(self.metadata['view'])
                 self.metadata['view'].append(dict(name=name, modal=modal, icon=icon))
             else:
                 self.metadata['view'].clear()
         return self
 
     def view(self):
         return self.all()
@@ -587,15 +593,15 @@
 
     def attach(self, *names):
         qs = self._clone()
         qs.metadata['attach'] = list(names)
         return qs
 
     def ignore(self, *names):
-        self.metadata['ignore'].extend(names)
+        self.metadata['ignore'] = list(names)
         return self
 
     def only(self, *names, **kwargs):
         if kwargs:
             for name, role in kwargs.items():
                 if name not in self.metadata['only']:
                     self.metadata['only'][name] = []
@@ -770,24 +776,25 @@
             else:
                 meta = request.path.startswith('/meta/')
                 raise JsonReadyResponseException(component.serialize(wrap=meta))
             return self.apply_role_lookups(request.user)
         return self
 
     def process_request(self, request):
-        self.get_attach()
         from sloth.core.valueset import ValueSet
         page = 1
         attr_name = request.GET.get('subset', 'all')
         self.metadata['uuid'] = request.GET.get('uuid')
         if attr_name == 'all':
             attach = self
         else:
+            attaches = self.get_attach()
             self.metadata['subset'] = attr_name
             attach = getattr(self._clone(), attr_name)()
+            attach.metadata['attach'] = attaches
         if isinstance(attach, QuerySet):
             qs = attach
             if self.metadata['ignore']:
                 qs.metadata['ignore'] = self.metadata['ignore']
         elif isinstance(attach, QuerySetStatistics):
             qs = attach.qs
         elif isinstance(attach, ValueSet):
```

### Comparing `sloth-framework-0.1.2/sloth/core/statistics.py` & `sloth-framework-0.1.3/sloth/core/statistics.py`

 * *Files 4% similar despite different names*

```diff
@@ -150,14 +150,16 @@
         self.qs = self.qs.apply_role_lookups(user)
         return self
 
     def debug(self):
         print(json.dumps(self.serialize(wrap=True), indent=4, ensure_ascii=False))
 
     def serialize(self, wrap=True, path=None, lazy=False):
+        tx = []
+        ty = []
         series = dict()
         if not lazy:
             self._calc()
 
             formatter = {True: 'Sim', False: 'Não', None: ''}
 
             def format_value(value):
@@ -166,33 +168,60 @@
             if self._ydict:
                 for i, (yk, yv) in enumerate(self._ydict.items()):
                     data = []
                     self.cursor = 0
                     for j, (xk, xv) in enumerate(self._xdict.items()):
                         data.append([formatter.get(xv, str(self._xfield_display_value(xv))), format_value(self._values_dict.get((xk, yk), 0)), self.nex_color()])
                     series.update(**{formatter.get(yv, str(self._yfield_display_value(yv))): data})
+                ty = []
+                for k, serie in series.items():
+                    sy = 0
+                    ly = len(serie)
+                    for i, item in enumerate(serie):
+                        sy += item[1]
+                    ty.append(sy)
+                tx = [0 for i in range(0, ly)]
+                # breakpoint()
+                for i in range(0, len(tx)):
+                    for kj in series:
+                        tx[i] += series[kj][i][1]
+                if len(tx) == len(ty) == 1:
+                    tx = ty = []
+                elif len(tx) > 1 and len(ty) > 1:
+                    ty.append(sum(ty))
+                    tx.append(sum(tx))
+                elif len(ty) > 1:
+                    if len(ty) > 2: tx.append(sum(tx))
+                    ty = []
+                elif len(tx) > 1:
+                    if len(tx) > 2: ty.append(sum(ty))
+                    tx = []
             else:
+                sx = 0
                 data = list()
                 for j, (xk, xv) in enumerate(self._xdict.items()):
                     data.append([formatter.get(xv, str(self._xfield_display_value(xv))), format_value(self._values_dict.get((xk, None), 0)), self.nex_color()])
+                    sx+=data[-1][1]
                 if data:
                     series['default'] = data
+                tx = [sx]
         if self.request and path is None:
             prefix = self.request.path.split('/')[1]
             path = self.request.path.replace('/{}'.format(prefix), '')
         if wrap:
             return dict(
                 type='statistics',
                 uuid=self.qs.metadata['uuid'],
                 name=self.qs.metadata['verbose_name'],
                 key=self.qs.metadata['attr'],
                 path=path,
                 series=series,
                 template=self.metadata['template'],
                 normalized=self.normalize(series),
+                tx=tx, ty=ty
             )
         else:
             return series['default'] if 'default' in series else series
 
     def process_request(self, request):
         for item in self.qs.get_filters().values():
             value = request.GET.get(item['key'])
```

### Comparing `sloth-framework-0.1.2/sloth/core/validation.py` & `sloth-framework-0.1.3/sloth/core/validation.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,19 @@
 
 
 def warning(message):
     print(termcolors.colorize('WARNING', fg='yellow', opts=('bold',)), message)
 
 
 def validate_model(model):
-    validate_valueset(model(pk=0).view())
+    valueset = model(pk=0).view()
+    if valueset is None:
+        warning('The method "view" of class {} must return a ValueSet intance. It returned "None".'.format(model))
+    else:
+        validate_valueset(valueset)
     validate_queryset(model.objects.all())
 
 
 def validate_valueset(valueset, method='view'):
     for name in valueset.metadata['names'].keys():
         try:
             try:
```

### Comparing `sloth-framework-0.1.2/sloth/core/valueset.py` & `sloth-framework-0.1.3/sloth/core/valueset.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,24 +203,23 @@
             else:
                 schema[attr_name] = self.instance.get_attr_api_type(attr_name)
         if recursive:
             return schema
         return dict(type='object', properties=schema)
 
     def load(self, wrap=True, detail=False, deep=0):
-        is_meta_api = False
         if self.request:
-            is_meta_api = self.request.path.startswith('/meta/')
             if 'only' in self.request.GET:
                 self.metadata['names'] = {k: 100 for k in self.request.GET['only'].split(',') if hasattr(self.instance, k)}
                 self.request.GET._mutable = True
                 self.request.GET.pop('only')
                 self.request.GET._mutable = False
 
         if self.metadata['names']:
+            is_app = self.request and self.request.path.startswith('/app/')
             for i, (attr_name, width) in enumerate(self.metadata['names'].items()):
                 if self.request and not self.request.user.is_superuser:
                     if self.metadata['only'] and attr_name in self.metadata['only']:
                         if not self.request.user.roles.contains(*self.metadata['only'][attr_name]):
                             continue
                 if self.request is None or self.instance.has_attr_permission(self.request.user, attr_name):
                     lazy = (wrap and (deep > 1 or (deep > 0 and i > 0)) and self.metadata['template'] is None) and not self.metadata['printing']
@@ -295,15 +294,15 @@
                             if valueset.metadata['template']:
                                 data.update(template='{}.html'.format(valueset.metadata['template']))
                     else:
                         path = '{}{}/'.format(self.path, attr_name)
                         data = value
                         verbose_name = pretty(self.metadata['model'].get_attr_metadata(attr_name)[0])
                         self.metadata['primitive'] = True
-                        if not wrap or is_meta_api:
+                        if not is_app:
                             data = serialize(data)
                         if wrap or detail:
                             template = getattr(attr, '__template__', None)
                             metadata = getattr(attr, '__metadata__', None)
                             if template:
                                 template = 'renderers/{}.html'.format(template)
                             data = dict(key=attr_name, name=verbose_name, value=data, width=width, template=template, metadata=metadata, type='primitive', path=path)
@@ -347,15 +346,15 @@
                 if self.metadata[key]:
                     value = getattr(self.instance, self.metadata[key])
                     value = value() if callable(value) else value
                     verbose_name, ordering, template, metadata = self.instance.get_attr_metadata(self.metadata[key])
                     if isinstance(value, QuerySet):
                         value = [str(obj) for obj in value]
                     output[key] = dict(value=value, template=template, metadata=metadata)
-
+            is_app = self.request and self.request.path.startswith('/app/')
             output.update(icon=icon, data=self, actions=[], inline_actions=[], attach=[], append={})
             for action_type in ('actions', 'inline_actions'):
                 for form_name in self.metadata[action_type]:
                     form_cls = self.instance.action_form_cls(form_name)
                     if self.request is None or form_cls.check_fake_permission(
                             request=self.request, instance=self.instance, instantiator=self.instance,
                     ):
```

### Comparing `sloth-framework-0.1.2/sloth/db/models/__init__.py` & `sloth-framework-0.1.3/sloth/db/models/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/test/__init__.py` & `sloth-framework-0.1.3/sloth/test/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/test/selenium/__init__.py` & `sloth-framework-0.1.3/sloth/test/selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/test/selenium/browser.py` & `sloth-framework-0.1.3/sloth/test/selenium/browser.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/utils/__init__.py` & `sloth-framework-0.1.3/sloth/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/utils/formatter/__init__.py` & `sloth-framework-0.1.3/sloth/utils/formatter/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,16 @@
             return mark_safe(obj)
         elif isinstance(obj, bool):
             return 'Sim' if obj else 'Não'
         elif isinstance(obj, datetime.datetime):
             return obj.strftime('%d/%m/%Y %H:%M')
         elif isinstance(obj, datetime.date):
             return obj.strftime('%d/%m/%Y')
+        elif isinstance(obj, int):
+            return format_decimal(obj, 0)
         elif isinstance(obj, float):
             return format_decimal(obj)
         elif isinstance(obj, Decimal):
             return format_decimal(obj)
         elif isinstance(obj, list):
             return mark_safe(
                 '<ul>{}</ul>'.format(''.join(['<li>{}</li>'.format(o) for o in obj]))
```

### Comparing `sloth-framework-0.1.2/sloth/utils/http/__init__.py` & `sloth-framework-0.1.3/sloth/utils/http/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/utils/icons/bootstrap.py` & `sloth-framework-0.1.3/sloth/utils/icons/bootstrap.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/utils/icons/fontawesome.py` & `sloth-framework-0.1.3/sloth/utils/icons/fontawesome.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/utils/icons/materialicons.py` & `sloth-framework-0.1.3/sloth/utils/icons/materialicons.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth/utils/log/sql.py` & `sloth-framework-0.1.3/sloth/utils/log/sql.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.2/sloth_framework.egg-info/PKG-INFO` & `sloth-framework-0.1.3/sloth_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sloth-framework
-Version: 0.1.2
+Version: 0.1.3
 Summary: Metadata-based web framework for the development of management information systems
 Home-page: http://sloth.aplicativo.click/
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `sloth-framework-0.1.2/sloth_framework.egg-info/SOURCES.txt` & `sloth-framework-0.1.3/sloth_framework.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -152,23 +152,26 @@
 sloth/api/templates/queryset/statistics.html
 sloth/api/templates/queryset/timeline.html
 sloth/api/templates/queryset/actions/actions.html
 sloth/api/templates/queryset/actions/batch.html
 sloth/api/templates/queryset/actions/global.html
 sloth/api/templates/renderers/badges/badge.html
 sloth/api/templates/renderers/badges/boolean.html
+sloth/api/templates/renderers/badges/danger.html
 sloth/api/templates/renderers/badges/primary.html
 sloth/api/templates/renderers/badges/status.html
+sloth/api/templates/renderers/badges/warning.html
 sloth/api/templates/renderers/boolean/thumb.html
 sloth/api/templates/renderers/calendar/calendar.html
 sloth/api/templates/renderers/calendar/events.html
 sloth/api/templates/renderers/calendar/legend.html
 sloth/api/templates/renderers/documents/document.html
 sloth/api/templates/renderers/images/banner.html
 sloth/api/templates/renderers/images/image.html
+sloth/api/templates/renderers/images/round.html
 sloth/api/templates/renderers/links/file.html
 sloth/api/templates/renderers/links/url.html
 sloth/api/templates/renderers/maps/geolocation.html
 sloth/api/templates/renderers/maps/map.html
 sloth/api/templates/renderers/messages/custom.html
 sloth/api/templates/renderers/messages/danger.html
 sloth/api/templates/renderers/messages/message.html
```

