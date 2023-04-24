# Comparing `tmp/aa_discord_announcements-1.1.0.tar.gz` & `tmp/aa_discord_announcements-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa_discord_announcements-1.1.0.tar", last modified: Sun Apr 16 16:09:35 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `aa_discord_announcements-1.1.0.tar` & `aa_discord_announcements-1.2.0.tar`

### file list

```diff
@@ -1,98 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.037473 aa_discord_announcements-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-04-16 16:09:35.037473 aa_discord_announcements-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.033473 aa_discord_announcements-1.1.0/aa_discord_announcements/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/app_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/auth_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.033473 aa_discord_announcements-1.1.0/aa_discord_announcements/helper/
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/helper/announcement_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/helper/discord_webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.029473 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.029473 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.033473 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     6492 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.029473 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.033473 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.029473 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/fr_FR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.033473 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/fr_FR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/fr_FR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.029473 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/it_IT/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.033473 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/it_IT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.029473 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.033473 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.029473 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/ko_KR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.033473 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/ko_KR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/ko_KR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.029473 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.033473 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.029473 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.033473 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.033473 aa_discord_announcements-1.1.0/aa_discord_announcements/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.029473 aa_discord_announcements-1.1.0/aa_discord_announcements/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.029473 aa_discord_announcements-1.1.0/aa_discord_announcements/static/aa_discord_announcements/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.037473 aa_discord_announcements-1.1.0/aa_discord_announcements/static/aa_discord_announcements/css/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/static/aa_discord_announcements/css/aa-discord-announcements.css
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/static/aa_discord_announcements/css/aa-discord-announcements.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.037473 aa_discord_announcements-1.1.0/aa_discord_announcements/static/aa_discord_announcements/javascript/
--rw-r--r--   0 runner    (1001) docker     (123)     6636 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.js
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.029473 aa_discord_announcements-1.1.0/aa_discord_announcements/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.037473 aa_discord_announcements-1.1.0/aa_discord_announcements/templates/aa_discord_announcements/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/templates/aa_discord_announcements/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.037473 aa_discord_announcements-1.1.0/aa_discord_announcements/templates/aa_discord_announcements/bundles/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/templates/aa_discord_announcements/bundles/discord-announcements-css.html
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/templates/aa_discord_announcements/bundles/discord-announcements-js.html
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/templates/aa_discord_announcements/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.029473 aa_discord_announcements-1.1.0/aa_discord_announcements/templates/aa_discord_announcements/partials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.037473 aa_discord_announcements-1.1.0/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/copy-paste-text.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.037473 aa_discord_announcements-1.1.0/aa_discord_announcements/templates/aa_discord_announcements/partials/form/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.037473 aa_discord_announcements-1.1.0/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-channel.html
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-targets.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.037473 aa_discord_announcements-1.1.0/aa_discord_announcements/templates/aa_discord_announcements/partials/header/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/templates/aa_discord_announcements/partials/header/page-header.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.037473 aa_discord_announcements-1.1.0/aa_discord_announcements/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/templatetags/aa_discord_announcements_versioned_static.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.037473 aa_discord_announcements-1.1.0/aa_discord_announcements/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/tests/test_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/tests/test_ajax_calls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/tests/test_auth_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/tests/test_installed_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/tests/test_templatetags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.033473 aa_discord_announcements-1.1.0/aa_discord_announcements.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-04-16 16:09:35.000000 aa_discord_announcements-1.1.0/aa_discord_announcements.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-04-16 16:09:35.000000 aa_discord_announcements-1.1.0/aa_discord_announcements.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 16:09:35.000000 aa_discord_announcements-1.1.0/aa_discord_announcements.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 16:09:34.000000 aa_discord_announcements-1.1.0/aa_discord_announcements.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-16 16:09:35.000000 aa_discord_announcements-1.1.0/aa_discord_announcements.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-16 16:09:35.000000 aa_discord_announcements-1.1.0/aa_discord_announcements.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-16 16:09:35.037473 aa_discord_announcements-1.1.0/setup.cfg
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/__init__.py
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/admin.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/app_settings.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/apps.py
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/auth_hooks.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/constants.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/forms.py
+-rw-r--r--   0        0        0     5883 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/models.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/urls.py
+-rw-r--r--   0        0        0     4822 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/views.py
+-rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/helper/announcement_context.py
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/helper/discord_webhook.py
+-rw-r--r--   0        0        0     4428 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/locale/django.pot
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     6492 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4627 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4428 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6061 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7613 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     5383 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/migrations/0001_initial.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/migrations/__init__.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/static/aa_discord_announcements/css/aa-discord-announcements.css
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/static/aa_discord_announcements/css/aa-discord-announcements.min.css
+-rw-r--r--   0        0        0     6636 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.js
+-rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.min.js
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/templates/aa_discord_announcements/base.html
+-rw-r--r--   0        0        0     2385 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/templates/aa_discord_announcements/index.html
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/templates/aa_discord_announcements/bundles/discord-announcements-css.html
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/templates/aa_discord_announcements/bundles/discord-announcements-js.html
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/copy-paste-text.html
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-channel.html
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-targets.html
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/templates/aa_discord_announcements/partials/header/page-header.html
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/templatetags/__init__.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/templatetags/aa_discord_announcements_versioned_static.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/tests/__init__.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/tests/test_access.py
+-rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/tests/test_ajax_calls.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/tests/test_auth_hooks.py
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/tests/test_installed_modules.py
+-rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/tests/test_models.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/tests/test_templatetags.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/tests/utils.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/LICENSE
+-rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/README.md
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/PKG-INFO
```

### Comparing `aa_discord_announcements-1.1.0/LICENSE` & `aa_discord_announcements-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.1.0/PKG-INFO` & `aa_discord_announcements-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: aa_discord_announcements
-Version: 1.1.0
+Name: aa-discord-announcements
+Version: 1.2.0
 Summary: Discord Announcements via Alliance Auth. Write announcements and manage who can write announcements on your corporation or alliance Discord through Alliance Auth.
-Home-page: https://github.com/ppfeufer/aa-discord-announcements
-Author: Peter Pfeufer
-Author-email: develop@ppfeufer.de
-Maintainer: Peter Pfeufer
-Maintainer-email: develop@ppfeufer.de
-License: GPL-3.0
-Project-URL: Issue / Bug Reports, https://github.com/ppfeufer/aa-discord-announcements/issues
+Project-URL: Homepage, https://github.com/ppfeufer/aa-discord-announcements
+Project-URL: Documentation, https://github.com/ppfeufer/aa-discord-announcements/blob/master/README.md
+Project-URL: Source, https://github.com/ppfeufer/aa-discord-announcements.git
 Project-URL: Changelog, https://github.com/ppfeufer/aa-discord-announcements/blob/master/CHANGELOG.md
-Keywords: allianceauth,eveonline,discord,announcements
+Project-URL: Tracker, https://github.com/ppfeufer/aa-discord-announcements/issues
+Author-email: Peter Pfeufer <develop@ppfeufer.de>
+License-Expression: GPL-3.0
+License-File: LICENSE
+Keywords: allianceauth,announcements,discord,eveonline
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -22,16 +22,18 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: ~=3.8
+Requires-Dist: allianceauth-app-utils>=1.13.0
+Requires-Dist: allianceauth>=3.0.0
+Requires-Dist: dhooks-lite>=0.6.1
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # AA Discord Announcements
 
 [![Version](https://img.shields.io/pypi/v/aa-discord-announcements?label=release)](https://pypi.org/project/aa-discord-announcements/)
 [![License](https://img.shields.io/github/license/ppfeufer/aa-discord-announcements)](https://github.com/ppfeufer/aa-discord-announcements/blob/master/LICENSE)
 [![Python](https://img.shields.io/pypi/pyversions/aa-discord-announcements)](https://pypi.org/project/aa-discord-announcements/)
 [![Django](https://img.shields.io/pypi/djversions/aa-discord-announcements?label=django)](https://pypi.org/project/aa-discord-announcements/)
@@ -45,26 +47,29 @@
 [![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/N4N8CL1BY)
 
 Discord Announcements via [Alliance Auth](https://gitlab.com/allianceauth/allianceauth)
 
 Write announcements and manage who can write announcements on your corporation or
 alliance Discord through Alliance Auth.
 
+---
 
 <!-- TOC -->
 * [AA Discord Announcements](#aa-discord-announcements)
   * [Installation](#installation)
     * [⚠️ Important ⚠️](#-important-)
     * [Step 1: Install the App](#step-1-install-the-app)
     * [Step 2: Update Your AA Settings](#step-2-update-your-aa-settings)
     * [Step 3: Finalizing the Installation](#step-3-finalizing-the-installation)
     * [Step 4: Setting up Permission](#step-4-setting-up-permission)
     * [Step 5: Setting up the App](#step-5-setting-up-the-app)
 <!-- TOC -->
 
+---
+
 
 ## Installation
 
 ### ⚠️ Important ⚠️
 
 This app is a plugin for Alliance Auth. If you don't have Alliance Auth running already,
 please install it first before proceeding.
```

### Comparing `aa_discord_announcements-1.1.0/README.md` & `aa_discord_announcements-1.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,26 +14,29 @@
 [![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/N4N8CL1BY)
 
 Discord Announcements via [Alliance Auth](https://gitlab.com/allianceauth/allianceauth)
 
 Write announcements and manage who can write announcements on your corporation or
 alliance Discord through Alliance Auth.
 
+---
 
 <!-- TOC -->
 * [AA Discord Announcements](#aa-discord-announcements)
   * [Installation](#installation)
     * [⚠️ Important ⚠️](#-important-)
     * [Step 1: Install the App](#step-1-install-the-app)
     * [Step 2: Update Your AA Settings](#step-2-update-your-aa-settings)
     * [Step 3: Finalizing the Installation](#step-3-finalizing-the-installation)
     * [Step 4: Setting up Permission](#step-4-setting-up-permission)
     * [Step 5: Setting up the App](#step-5-setting-up-the-app)
 <!-- TOC -->
 
+---
+
 
 ## Installation
 
 ### ⚠️ Important ⚠️
 
 This app is a plugin for Alliance Auth. If you don't have Alliance Auth running already,
 please install it first before proceeding.
```

### Comparing `aa_discord_announcements-1.1.0/aa_discord_announcements/admin.py` & `aa_discord_announcements-1.2.0/aa_discord_announcements/admin.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.1.0/aa_discord_announcements/auth_hooks.py` & `aa_discord_announcements-1.2.0/aa_discord_announcements/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.1.0/aa_discord_announcements/forms.py` & `aa_discord_announcements-1.2.0/aa_discord_announcements/forms.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.1.0/aa_discord_announcements/helper/announcement_context.py` & `aa_discord_announcements-1.2.0/aa_discord_announcements/helper/announcement_context.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.1.0/aa_discord_announcements/helper/discord_webhook.py` & `aa_discord_announcements-1.2.0/aa_discord_announcements/helper/discord_webhook.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.1.0/aa_discord_announcements/locale/de/LC_MESSAGES/django.mo` & `aa_discord_announcements-1.2.0/aa_discord_announcements/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.1.0/aa_discord_announcements/locale/de/LC_MESSAGES/django.po` & `aa_discord_announcements-1.2.0/aa_discord_announcements/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.1.0/aa_discord_announcements/locale/es/LC_MESSAGES/django.po` & `aa_discord_announcements-1.2.0/aa_discord_announcements/locale/django.pot`

 * *Files 1% similar despite different names*

```diff
@@ -4,23 +4,22 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-11 23:21+0200\n"
+"POT-Creation-Date: 2023-04-19 01:15+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: forms.py:20
 msgid "This field is mandatory"
 msgstr ""
 
 #: forms.py:41
 msgid "Discord Markdown"
```

### Comparing `aa_discord_announcements-1.1.0/aa_discord_announcements/locale/fr_FR/LC_MESSAGES/django.po` & `aa_discord_announcements-1.2.0/aa_discord_announcements/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.1.0/aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.po` & `aa_discord_announcements-1.2.0/aa_discord_announcements/locale/ja/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
 #: forms.py:20
 msgid "This field is mandatory"
 msgstr ""
 
 #: forms.py:41
 msgid "Discord Markdown"
```

### Comparing `aa_discord_announcements-1.1.0/aa_discord_announcements/locale/ja/LC_MESSAGES/django.po` & `aa_discord_announcements-1.2.0/aa_discord_announcements/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.1.0/aa_discord_announcements/locale/ko_KR/LC_MESSAGES/django.po` & `aa_discord_announcements-1.2.0/aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-#
-#, fuzzy
+# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-04-11 23:21+0200\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"PO-Revision-Date: 2023-04-18 23:17+0000\n"
+"Last-Translator: \"H. Peter Pfeufer\" <info@ppfeufer.de>\n"
+"Language-Team: Italian <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-discord-announcements/it/>\n"
+"Language: it_IT\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 4.16.4\n"
 
 #: forms.py:20
 msgid "This field is mandatory"
-msgstr ""
+msgstr "Questo campo è obbligatorio"
 
 #: forms.py:41
 msgid "Discord Markdown"
 msgstr ""
 
 #: forms.py:48
 #, python-brace-format
```

### Comparing `aa_discord_announcements-1.1.0/aa_discord_announcements/locale/ru/LC_MESSAGES/django.mo` & `aa_discord_announcements-1.2.0/aa_discord_announcements/locale/ru/LC_MESSAGES/django.mo`

 * *Files 13% similar despite different names*

#### msgunfmt {}

```diff
@@ -6,17 +6,16 @@
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: Russian <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-discord-announcements/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
-"n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
-"(n%100>=11 && n%100<=14)? 2 : 3);\n"
+"Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
+"n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "X-Generator: Weblate 4.16.4\n"
 
 msgid "Additionally configured announcement targets"
 msgstr "Дополнительно сконфигурированные цели объявлений"
 
 msgid "Announcement Channel"
 msgstr "Канал объявления"
@@ -27,15 +26,15 @@
 msgid "Announcement Target"
 msgstr "Цель объявления"
 
 msgid "Announcement Text"
 msgstr "Текст объявления"
 
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
-msgstr "Вы уверены, что Discord связан с Allaince Auth?"
+msgstr "Вы уверены, что Ваш Discord связан с Вашим Alliance Auth?"
 
 msgid "Copy Announcement Text"
 msgstr "Скопировать текст объявления"
 
 msgid "Create Announcement"
 msgstr "Создать объявление"
 
@@ -75,16 +74,16 @@
 msgid "ID of the Discord role to ping"
 msgstr "ID роли Discord для пинга"
 
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
-"Некорректный URL для webhook. Введенный URL не совпадает с известными "
-"форматами Discord webhook. Пожалуйста, проверьте URL."
+"Некорректный URL вебхука. Введенный URL не совпадает с известными форматами "
+"вебхуков Discord. Пожалуйста, проверьте URL."
 
 msgid ""
 "Mandatory information is missing.<br>To create an announcement, you need to "
 "fill out the following fields:<br>» Announcement Text"
 msgstr ""
 "Отсутствует необходимая информация. <br>Для создания объявления необходимо "
 "заполнить следующие поля:<br>» Текст объявления"
@@ -93,15 +92,15 @@
 "Name of the Discord role to ping. (Note: This must be an Auth group that is "
 "synced to Discord.)"
 msgstr ""
 "Имя роли Discord для пинга. (Примечание: Это должна быть синхронизированная "
 "с Discord группа Auth.)"
 
 msgid "Name of the channel this webhook posts to"
-msgstr "Название канала, в который webhook отправляет сообщения"
+msgstr "Название канала, в который вебхук отправляет сообщения"
 
 msgid "No announcement created yet ..."
 msgstr "Объявлений нет..."
 
 msgid "No form data submitted."
 msgstr "Данные формы не отправлены."
 
@@ -122,35 +121,35 @@
 
 msgid "This group has not been synced to Discord yet."
 msgstr "Эта группа не была синхронизирована с Discord."
 
 msgid ""
 "URL of this webhook, e.g. https://discord.com/api/webhooks/123456/abcdef"
 msgstr ""
-"URL этого webhook, например https://discord.com/api/webhooks/123456/abcdef"
+"URL этого вебхука, например https://discord.com/api/webhooks/123456/abcdef"
 
 msgid "Webhook"
-msgstr "Webhook"
+msgstr "Вебхук"
 
 msgid "Webhooks"
-msgstr "Webhook'и"
+msgstr "Вебхуки"
 
 msgid "Whether this ping target is enabled or not"
 msgstr "Разрешена или нет цель пинга"
 
 msgid "Whether this webhook is active or not"
-msgstr "Активен или нет webhook"
+msgstr "Активен или нет вебхук"
 
 msgid "Who do you want to ping?"
 msgstr "Кого Вы хотите пинговать?"
 
 msgid "You can add notes about this configuration here if you want"
 msgstr "Здесь Вы можете добавить примечания для этой конфигурации"
 
 msgid "You can add notes about this webhook here if you want"
-msgstr "Здесь Вы можете добавить примечания для этого webhook"
+msgstr "Здесь Вы можете добавить примечания для этого вебхука"
 
 msgid "You might want to install the Discord service first ..."
-msgstr "Возможно Вам следует сначала установить сервис Discord..."
+msgstr "Возможно, Вам следует сначала установить сервис Discord..."
 
 msgid "Your announcement…"
 msgstr "Ваше объявление…"
```

### Comparing `aa_discord_announcements-1.1.0/aa_discord_announcements/locale/ru/LC_MESSAGES/django.po` & `aa_discord_announcements-1.2.0/aa_discord_announcements/locale/ru/LC_MESSAGES/django.po`

 * *Files 10% similar despite different names*

```diff
@@ -4,25 +4,24 @@
 # "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
 # Nikolay <nick.postnikov@gmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-04-11 23:21+0200\n"
-"PO-Revision-Date: 2023-04-16 15:33+0000\n"
+"PO-Revision-Date: 2023-04-20 21:50+0000\n"
 "Last-Translator: Nikolay <nick.postnikov@gmail.com>\n"
 "Language-Team: Russian <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-discord-announcements/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
-"n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || ("
-"n%100>=11 && n%100<=14)? 2 : 3);\n"
+"Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
+"n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "X-Generator: Weblate 4.16.4\n"
 
 #: forms.py:20
 msgid "This field is mandatory"
 msgstr "Обязательное поле"
 
 #: forms.py:41
@@ -58,19 +57,19 @@
 
 #: forms.py:76
 msgid "Your announcement…"
 msgstr "Ваше объявление…"
 
 #: models.py:37
 msgid "You might want to install the Discord service first ..."
-msgstr "Возможно Вам следует сначала установить сервис Discord..."
+msgstr "Возможно, Вам следует сначала установить сервис Discord..."
 
 #: models.py:44
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
-msgstr "Вы уверены, что Discord связан с Allaince Auth?"
+msgstr "Вы уверены, что Ваш Discord связан с Вашим Alliance Auth?"
 
 #: models.py:48
 msgid "This group has not been synced to Discord yet."
 msgstr "Эта группа не была синхронизирована с Discord."
 
 #: models.py:81
 msgid ""
@@ -102,45 +101,45 @@
 
 #: models.py:123
 msgid "Discord Ping Targets"
 msgstr "Цели пинга Discord"
 
 #: models.py:163
 msgid "Name of the channel this webhook posts to"
-msgstr "Название канала, в который webhook отправляет сообщения"
+msgstr "Название канала, в который вебхук отправляет сообщения"
 
 #: models.py:172
 msgid ""
 "URL of this webhook, e.g. https://discord.com/api/webhooks/123456/abcdef"
 msgstr ""
-"URL этого webhook, например https://discord.com/api/webhooks/123456/abcdef"
+"URL этого вебхука, например https://discord.com/api/webhooks/123456/abcdef"
 
 #: models.py:190
 msgid "You can add notes about this webhook here if you want"
-msgstr "Здесь Вы можете добавить примечания для этого webhook"
+msgstr "Здесь Вы можете добавить примечания для этого вебхука"
 
 #: models.py:197
 msgid "Whether this webhook is active or not"
-msgstr "Активен или нет webhook"
+msgstr "Активен или нет вебхук"
 
 #: models.py:205
 msgid "Webhook"
-msgstr "Webhook"
+msgstr "Вебхук"
 
 #: models.py:206
 msgid "Webhooks"
-msgstr "Webhook'и"
+msgstr "Вебхуки"
 
 #: models.py:222
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
-"Некорректный URL для webhook. Введенный URL не совпадает с известными "
-"форматами Discord webhook. Пожалуйста, проверьте URL."
+"Некорректный URL вебхука. Введенный URL не совпадает с известными форматами "
+"вебхуков Discord. Пожалуйста, проверьте URL."
 
 #: templates/aa_discord_announcements/base.html:5
 #: templates/aa_discord_announcements/base.html:8
 msgid "Discord Announcements"
 msgstr "Объявления Discord"
 
 #: templates/aa_discord_announcements/index.html:10
```

### Comparing `aa_discord_announcements-1.1.0/aa_discord_announcements/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_discord_announcements-1.2.0/aa_discord_announcements/locale/es/LC_MESSAGES/django.po`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-#
-#, fuzzy
+# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-04-11 23:21+0200\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"PO-Revision-Date: 2023-04-18 23:17+0000\n"
+"Last-Translator: \"H. Peter Pfeufer\" <info@ppfeufer.de>\n"
+"Language-Team: Spanish <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-discord-announcements/es/>\n"
+"Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 4.16.4\n"
 
 #: forms.py:20
 msgid "This field is mandatory"
-msgstr ""
+msgstr "Este campo es obligatorio"
 
 #: forms.py:41
 msgid "Discord Markdown"
 msgstr ""
 
 #: forms.py:48
 #, python-brace-format
```

### Comparing `aa_discord_announcements-1.1.0/aa_discord_announcements/migrations/0001_initial.py` & `aa_discord_announcements-1.2.0/aa_discord_announcements/migrations/0001_initial.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 # Django
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = [
         ("auth", "0012_alter_user_first_name_max_length"),
     ]
 
     operations = [
```

### Comparing `aa_discord_announcements-1.1.0/aa_discord_announcements/models.py` & `aa_discord_announcements-1.2.0/aa_discord_announcements/models.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.1.0/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.js` & `aa_discord_announcements-1.2.0/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.js`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.1.0/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.min.js` & `aa_discord_announcements-1.2.0/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.min.js`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.1.0/aa_discord_announcements/templates/aa_discord_announcements/index.html` & `aa_discord_announcements-1.2.0/aa_discord_announcements/templates/aa_discord_announcements/index.html`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.1.0/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html` & `aa_discord_announcements-1.2.0/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.1.0/aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html` & `aa_discord_announcements-1.2.0/aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.1.0/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-targets.html` & `aa_discord_announcements-1.2.0/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-targets.html`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.1.0/aa_discord_announcements/templatetags/aa_discord_announcements_versioned_static.py` & `aa_discord_announcements-1.2.0/aa_discord_announcements/templatetags/aa_discord_announcements_versioned_static.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.1.0/aa_discord_announcements/tests/test_access.py` & `aa_discord_announcements-1.2.0/aa_discord_announcements/tests/test_access.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.1.0/aa_discord_announcements/tests/test_ajax_calls.py` & `aa_discord_announcements-1.2.0/aa_discord_announcements/tests/test_ajax_calls.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.1.0/aa_discord_announcements/tests/test_auth_hooks.py` & `aa_discord_announcements-1.2.0/aa_discord_announcements/tests/test_auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.1.0/aa_discord_announcements/tests/test_installed_modules.py` & `aa_discord_announcements-1.2.0/aa_discord_announcements/tests/test_installed_modules.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.1.0/aa_discord_announcements/tests/test_models.py` & `aa_discord_announcements-1.2.0/aa_discord_announcements/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.1.0/aa_discord_announcements/tests/test_templatetags.py` & `aa_discord_announcements-1.2.0/aa_discord_announcements/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.1.0/aa_discord_announcements/tests/utils.py` & `aa_discord_announcements-1.2.0/aa_discord_announcements/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.1.0/aa_discord_announcements/urls.py` & `aa_discord_announcements-1.2.0/aa_discord_announcements/urls.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.1.0/aa_discord_announcements/views.py` & `aa_discord_announcements-1.2.0/aa_discord_announcements/views.py`

 * *Files identical despite different names*

