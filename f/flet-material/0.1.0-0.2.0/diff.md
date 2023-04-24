# Comparing `tmp/flet-material-0.1.0.tar.gz` & `tmp/flet-material-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet-material-0.1.0.tar", last modified: Sun Apr 23 17:12:54 2023, max compression
+gzip compressed data, was "flet-material-0.2.0.tar", last modified: Mon Apr 24 13:04:25 2023, max compression
```

## Comparing `flet-material-0.1.0.tar` & `flet-material-0.2.0.tar`

### file list

```diff
@@ -1,73 +1,152 @@
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-23 17:12:54.530855 flet-material-0.1.0/
--rw-r--r--   0 ahmad      (501) staff       (20)       14 2023-04-23 11:39:25.000000 flet-material-0.1.0/.gitignore
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-23 17:12:54.517901 flet-material-0.1.0/.vscode/
--rw-r--r--   0 ahmad      (501) staff       (20)       64 2023-04-21 12:22:35.000000 flet-material-0.1.0/.vscode/settings.json
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-04-22 18:46:28.000000 flet-material-0.1.0/CHANGELOG.md
--rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-04-22 18:06:15.000000 flet-material-0.1.0/LICENSE
--rw-r--r--   0 ahmad      (501) staff       (20)      465 2023-04-23 17:12:54.530635 flet-material-0.1.0/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-04-20 15:07:43.000000 flet-material-0.1.0/README.md
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-23 17:12:54.518384 flet-material-0.1.0/command/
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-04-23 08:17:07.000000 flet-material-0.1.0/command/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)      682 2023-04-23 17:03:12.000000 flet-material-0.1.0/command/new_project.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-23 17:12:54.518576 flet-material-0.1.0/docs/
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-23 17:12:54.518777 flet-material-0.1.0/docs/docs/
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-23 17:12:54.520631 flet-material-0.1.0/docs/docs/controls/
--rw-r--r--   0 ahmad      (501) staff       (20)     1693 2023-04-23 15:29:21.000000 flet-material-0.1.0/docs/docs/controls/alerts.md
--rw-r--r--   0 ahmad      (501) staff       (20)     1060 2023-04-23 15:21:15.000000 flet-material-0.1.0/docs/docs/controls/annotations.md
--rw-r--r--   0 ahmad      (501) staff       (20)     2870 2023-04-23 15:54:57.000000 flet-material-0.1.0/docs/docs/controls/badges.md
--rw-r--r--   0 ahmad      (501) staff       (20)     1566 2023-04-23 16:04:13.000000 flet-material-0.1.0/docs/docs/controls/buttons.md
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-04-23 13:01:36.000000 flet-material-0.1.0/docs/docs/controls/checkboxes.md
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-04-23 13:01:48.000000 flet-material-0.1.0/docs/docs/controls/chips.md
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-04-23 13:01:55.000000 flet-material-0.1.0/docs/docs/controls/dropdowns.md
--rw-r--r--   0 ahmad      (501) staff       (20)     2811 2023-04-23 14:49:45.000000 flet-material-0.1.0/docs/docs/controls/index.md
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-04-23 13:02:07.000000 flet-material-0.1.0/docs/docs/controls/switches.md
--rw-r--r--   0 ahmad      (501) staff       (20)    11471 2023-04-23 13:02:15.000000 flet-material-0.1.0/docs/docs/index.md
--rw-r--r--   0 ahmad      (501) staff       (20)     2898 2023-04-23 17:02:36.000000 flet-material-0.1.0/docs/mkdocs.yml
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-23 17:12:54.523489 flet-material-0.1.0/flet_material/
--rw-r--r--   0 ahmad      (501) staff       (20)      421 2023-04-23 11:09:44.000000 flet-material-0.1.0/flet_material/__init__.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-23 17:12:54.527233 flet-material-0.1.0/flet_material/__pycache__/
--rw-r--r--   0 ahmad      (501) staff       (20)      706 2023-04-23 11:09:44.000000 flet-material-0.1.0/flet_material/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)     3911 2023-04-23 11:11:37.000000 flet-material-0.1.0/flet_material/__pycache__/admonition.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)     1892 2023-04-22 18:01:00.000000 flet-material-0.1.0/flet_material/__pycache__/alert.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)     1697 2023-04-21 17:58:50.000000 flet-material-0.1.0/flet_material/__pycache__/annotation.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)     1834 2023-04-21 16:25:55.000000 flet-material-0.1.0/flet_material/__pycache__/annotations.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)     3211 2023-04-23 15:51:31.000000 flet-material-0.1.0/flet_material/__pycache__/badge.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)      738 2023-04-23 14:56:58.000000 flet-material-0.1.0/flet_material/__pycache__/base.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)     1576 2023-04-22 11:58:50.000000 flet-material-0.1.0/flet_material/__pycache__/button.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)     1525 2023-04-23 11:36:01.000000 flet-material-0.1.0/flet_material/__pycache__/checkbox.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)     1646 2023-04-23 11:27:27.000000 flet-material-0.1.0/flet_material/__pycache__/chip.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)     1698 2023-04-22 14:16:22.000000 flet-material-0.1.0/flet_material/__pycache__/switch.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)     6416 2023-04-23 11:11:36.000000 flet-material-0.1.0/flet_material/admonition.py
--rw-r--r--   0 ahmad      (501) staff       (20)     2689 2023-04-22 18:01:00.000000 flet-material-0.1.0/flet_material/alert.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1503 2023-04-21 17:58:49.000000 flet-material-0.1.0/flet_material/annotation.py
--rw-r--r--   0 ahmad      (501) staff       (20)     4731 2023-04-23 15:51:31.000000 flet-material-0.1.0/flet_material/badge.py
--rw-r--r--   0 ahmad      (501) staff       (20)      358 2023-04-23 14:56:57.000000 flet-material-0.1.0/flet_material/base.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1383 2023-04-22 11:58:49.000000 flet-material-0.1.0/flet_material/button.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1038 2023-04-23 11:36:00.000000 flet-material-0.1.0/flet_material/checkbox.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1405 2023-04-23 11:27:26.000000 flet-material-0.1.0/flet_material/chip.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1399 2023-04-22 14:16:22.000000 flet-material-0.1.0/flet_material/switch.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-23 17:12:54.524905 flet-material-0.1.0/flet_material.egg-info/
--rw-r--r--   0 ahmad      (501) staff       (20)      465 2023-04-23 17:12:54.000000 flet-material-0.1.0/flet_material.egg-info/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)     1903 2023-04-23 17:12:54.000000 flet-material-0.1.0/flet_material.egg-info/SOURCES.txt
--rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-04-23 17:12:54.000000 flet-material-0.1.0/flet_material.egg-info/dependency_links.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       83 2023-04-23 17:12:54.000000 flet-material-0.1.0/flet_material.egg-info/entry_points.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       25 2023-04-23 17:12:54.000000 flet-material-0.1.0/flet_material.egg-info/requires.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       21 2023-04-23 17:12:54.000000 flet-material-0.1.0/flet_material.egg-info/top_level.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       24 2023-04-22 18:53:13.000000 flet-material-0.1.0/requirements.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-04-23 17:12:54.530910 flet-material-0.1.0/setup.cfg
--rw-r--r--   0 ahmad      (501) staff       (20)     1050 2023-04-23 17:11:40.000000 flet-material-0.1.0/setup.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-23 17:12:54.528972 flet-material-0.1.0/styles/
--rw-r--r--   0 ahmad      (501) staff       (20)      271 2023-04-22 17:17:29.000000 flet-material-0.1.0/styles/__init__.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-23 17:12:54.530344 flet-material-0.1.0/styles/__pycache__/
--rw-r--r--   0 ahmad      (501) staff       (20)      499 2023-04-22 17:17:29.000000 flet-material-0.1.0/styles/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)      708 2023-04-23 11:20:49.000000 flet-material-0.1.0/styles/__pycache__/admonition_style.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)      493 2023-04-22 17:30:06.000000 flet-material-0.1.0/styles/__pycache__/alert_style.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)      494 2023-04-22 17:08:25.000000 flet-material-0.1.0/styles/__pycache__/alert_styles.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)      487 2023-04-22 16:10:03.000000 flet-material-0.1.0/styles/__pycache__/badge_style.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)      287 2023-04-21 16:08:17.000000 flet-material-0.1.0/styles/__pycache__/fonts.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)     1040 2023-04-23 14:54:06.000000 flet-material-0.1.0/styles/__pycache__/theme.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)      908 2023-04-23 11:20:48.000000 flet-material-0.1.0/styles/admonition_style.py
--rw-r--r--   0 ahmad      (501) staff       (20)      378 2023-04-22 17:30:06.000000 flet-material-0.1.0/styles/alert_style.py
--rw-r--r--   0 ahmad      (501) staff       (20)      361 2023-04-22 16:10:02.000000 flet-material-0.1.0/styles/badge_style.py
--rw-r--r--   0 ahmad      (501) staff       (20)       90 2023-04-21 16:07:16.000000 flet-material-0.1.0/styles/fonts.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1421 2023-04-23 14:18:26.000000 flet-material-0.1.0/styles/theme.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.258348 flet-material-0.2.0/
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.205508 flet-material-0.2.0/.github/
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.210761 flet-material-0.2.0/.github/workflows/
+-rw-r--r--   0 ahmad      (501) staff       (20)      496 2023-04-23 18:54:25.000000 flet-material-0.2.0/.github/workflows/build.yml
+-rw-r--r--   0 ahmad      (501) staff       (20)       37 2023-04-24 09:59:38.000000 flet-material-0.2.0/.gitignore
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.211162 flet-material-0.2.0/.vscode/
+-rw-r--r--   0 ahmad      (501) staff       (20)       64 2023-04-21 12:22:35.000000 flet-material-0.2.0/.vscode/settings.json
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-04-24 11:04:16.000000 flet-material-0.2.0/CHANGELOG.md
+-rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-04-22 18:06:15.000000 flet-material-0.2.0/LICENSE
+-rw-r--r--   0 ahmad      (501) staff       (20)      465 2023-04-24 13:04:25.257946 flet-material-0.2.0/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)     3839 2023-04-24 12:56:14.000000 flet-material-0.2.0/README.md
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.211694 flet-material-0.2.0/command/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-04-23 08:17:07.000000 flet-material-0.2.0/command/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      682 2023-04-23 17:03:12.000000 flet-material-0.2.0/command/new_project.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.212032 flet-material-0.2.0/docs/
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.212757 flet-material-0.2.0/docs/docs/
+-rw-r--r--   0 ahmad      (501) staff       (20)     1819 2023-04-24 12:26:23.000000 flet-material-0.2.0/docs/docs/contribute.md
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.215803 flet-material-0.2.0/docs/docs/controls/
+-rw-r--r--   0 ahmad      (501) staff       (20)     1975 2023-04-24 12:09:58.000000 flet-material-0.2.0/docs/docs/controls/alerts.md
+-rw-r--r--   0 ahmad      (501) staff       (20)     1357 2023-04-24 12:10:06.000000 flet-material-0.2.0/docs/docs/controls/annotations.md
+-rw-r--r--   0 ahmad      (501) staff       (20)     3198 2023-04-24 11:12:12.000000 flet-material-0.2.0/docs/docs/controls/badges.md
+-rw-r--r--   0 ahmad      (501) staff       (20)     1566 2023-04-23 16:04:13.000000 flet-material-0.2.0/docs/docs/controls/buttons.md
+-rw-r--r--   0 ahmad      (501) staff       (20)     1605 2023-04-24 12:10:25.000000 flet-material-0.2.0/docs/docs/controls/checkboxes.md
+-rw-r--r--   0 ahmad      (501) staff       (20)     1434 2023-04-24 12:10:31.000000 flet-material-0.2.0/docs/docs/controls/chips.md
+-rw-r--r--   0 ahmad      (501) staff       (20)     3023 2023-04-24 12:10:54.000000 flet-material-0.2.0/docs/docs/controls/dropdowns.md
+-rw-r--r--   0 ahmad      (501) staff       (20)     2811 2023-04-23 14:49:45.000000 flet-material-0.2.0/docs/docs/controls/index.md
+-rw-r--r--   0 ahmad      (501) staff       (20)     1296 2023-04-24 12:10:56.000000 flet-material-0.2.0/docs/docs/controls/switches.md
+-rw-r--r--   0 ahmad      (501) staff       (20)     3038 2023-04-24 12:28:23.000000 flet-material-0.2.0/docs/docs/index.md
+-rw-r--r--   0 ahmad      (501) staff       (20)     3070 2023-04-24 12:35:43.000000 flet-material-0.2.0/docs/mkdocs.yml
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.217357 flet-material-0.2.0/docs/site/
+-rw-r--r--   0 ahmad      (501) staff       (20)        8 2023-04-24 12:45:17.000000 flet-material-0.2.0/docs/site/.gitignore
+-rw-r--r--   0 ahmad      (501) staff       (20)    28461 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/404.html
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.206826 flet-material-0.2.0/docs/site/assets/
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.217603 flet-material-0.2.0/docs/site/assets/images/
+-rw-r--r--   0 ahmad      (501) staff       (20)     1870 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/images/favicon.png
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.218731 flet-material-0.2.0/docs/site/assets/javascripts/
+-rw-r--r--   0 ahmad      (501) staff       (20)   113367 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/bundle.51198bba.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)   950772 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/bundle.51198bba.min.js.map
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.221249 flet-material-0.2.0/docs/site/assets/javascripts/lunr/
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.232393 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/
+-rw-r--r--   0 ahmad      (501) staff       (20)    17074 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.ar.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     4654 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.da.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     6119 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.de.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     6208 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.du.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)    11499 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.es.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     9342 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.fi.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)    10669 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.fr.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     3383 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.hi.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     9437 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.hu.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)    11232 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.it.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     2313 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.ja.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)       36 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.jp.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     7973 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.ko.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)      817 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.multi.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     6026 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.nl.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     4754 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.no.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)    10171 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.pt.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)    10958 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.ro.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)    10331 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.ru.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     3647 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     4523 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.sv.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     2406 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.ta.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     1031 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.th.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)    15009 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.tr.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)      784 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.vi.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     2062 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.zh.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)    22878 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/tinyseg.js
+-rw-r--r--   0 ahmad      (501) staff       (20)   677455 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/wordcut.js
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.233555 flet-material-0.2.0/docs/site/assets/javascripts/workers/
+-rw-r--r--   0 ahmad      (501) staff       (20)    38916 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/workers/search.208ed371.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)   209901 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/workers/search.208ed371.min.js.map
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.236568 flet-material-0.2.0/docs/site/assets/stylesheets/
+-rw-r--r--   0 ahmad      (501) staff       (20)   113417 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/stylesheets/main.ded33207.min.css
+-rw-r--r--   0 ahmad      (501) staff       (20)    38957 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/stylesheets/main.ded33207.min.css.map
+-rw-r--r--   0 ahmad      (501) staff       (20)    12355 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/stylesheets/palette.a0c5b2b5.min.css
+-rw-r--r--   0 ahmad      (501) staff       (20)     3646 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/stylesheets/palette.a0c5b2b5.min.css.map
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.237141 flet-material-0.2.0/docs/site/contribute/
+-rw-r--r--   0 ahmad      (501) staff       (20)    32427 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/contribute/index.html
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.237796 flet-material-0.2.0/docs/site/controls/
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.238199 flet-material-0.2.0/docs/site/controls/alerts/
+-rw-r--r--   0 ahmad      (501) staff       (20)    38198 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/controls/alerts/index.html
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.238610 flet-material-0.2.0/docs/site/controls/annotations/
+-rw-r--r--   0 ahmad      (501) staff       (20)    34841 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/controls/annotations/index.html
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.238997 flet-material-0.2.0/docs/site/controls/badges/
+-rw-r--r--   0 ahmad      (501) staff       (20)    48809 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/controls/badges/index.html
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.239460 flet-material-0.2.0/docs/site/controls/buttons/
+-rw-r--r--   0 ahmad      (501) staff       (20)    37505 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/controls/buttons/index.html
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.239843 flet-material-0.2.0/docs/site/controls/checkboxes/
+-rw-r--r--   0 ahmad      (501) staff       (20)    37319 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/controls/checkboxes/index.html
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.240208 flet-material-0.2.0/docs/site/controls/chips/
+-rw-r--r--   0 ahmad      (501) staff       (20)    36557 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/controls/chips/index.html
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.240601 flet-material-0.2.0/docs/site/controls/dropdowns/
+-rw-r--r--   0 ahmad      (501) staff       (20)    46447 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/controls/dropdowns/index.html
+-rw-r--r--   0 ahmad      (501) staff       (20)    32736 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/controls/index.html
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.240964 flet-material-0.2.0/docs/site/controls/switches/
+-rw-r--r--   0 ahmad      (501) staff       (20)    36069 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/controls/switches/index.html
+-rw-r--r--   0 ahmad      (501) staff       (20)    38036 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/index.html
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.241333 flet-material-0.2.0/docs/site/search/
+-rw-r--r--   0 ahmad      (501) staff       (20)    21578 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/search/search_index.json
+-rw-r--r--   0 ahmad      (501) staff       (20)     1484 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/sitemap.xml
+-rw-r--r--   0 ahmad      (501) staff       (20)      204 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/sitemap.xml.gz
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.245151 flet-material-0.2.0/flet_material/
+-rw-r--r--   0 ahmad      (501) staff       (20)      421 2023-04-23 11:09:44.000000 flet-material-0.2.0/flet_material/__init__.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.251647 flet-material-0.2.0/flet_material/__pycache__/
+-rw-r--r--   0 ahmad      (501) staff       (20)      706 2023-04-23 11:09:44.000000 flet-material-0.2.0/flet_material/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)     4049 2023-04-24 11:44:19.000000 flet-material-0.2.0/flet_material/__pycache__/admonition.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)     1892 2023-04-22 18:01:00.000000 flet-material-0.2.0/flet_material/__pycache__/alert.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)     1697 2023-04-21 17:58:50.000000 flet-material-0.2.0/flet_material/__pycache__/annotation.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)     1834 2023-04-21 16:25:55.000000 flet-material-0.2.0/flet_material/__pycache__/annotations.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)     3211 2023-04-23 15:51:31.000000 flet-material-0.2.0/flet_material/__pycache__/badge.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)      738 2023-04-23 14:56:58.000000 flet-material-0.2.0/flet_material/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)     1597 2023-04-23 18:10:10.000000 flet-material-0.2.0/flet_material/__pycache__/button.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)     1525 2023-04-23 11:36:01.000000 flet-material-0.2.0/flet_material/__pycache__/checkbox.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)     1698 2023-04-24 11:30:35.000000 flet-material-0.2.0/flet_material/__pycache__/chip.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)     1698 2023-04-22 14:16:22.000000 flet-material-0.2.0/flet_material/__pycache__/switch.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)     6919 2023-04-24 11:44:19.000000 flet-material-0.2.0/flet_material/admonition.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     2689 2023-04-22 18:01:00.000000 flet-material-0.2.0/flet_material/alert.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1503 2023-04-21 17:58:49.000000 flet-material-0.2.0/flet_material/annotation.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     4731 2023-04-23 15:51:31.000000 flet-material-0.2.0/flet_material/badge.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      358 2023-04-23 14:56:57.000000 flet-material-0.2.0/flet_material/base.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1425 2023-04-23 18:09:54.000000 flet-material-0.2.0/flet_material/button.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1038 2023-04-23 11:36:00.000000 flet-material-0.2.0/flet_material/checkbox.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1528 2023-04-24 11:30:35.000000 flet-material-0.2.0/flet_material/chip.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1399 2023-04-22 14:16:22.000000 flet-material-0.2.0/flet_material/switch.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.246825 flet-material-0.2.0/flet_material.egg-info/
+-rw-r--r--   0 ahmad      (501) staff       (20)      465 2023-04-24 13:04:25.000000 flet-material-0.2.0/flet_material.egg-info/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)     4488 2023-04-24 13:04:25.000000 flet-material-0.2.0/flet_material.egg-info/SOURCES.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-04-24 13:04:25.000000 flet-material-0.2.0/flet_material.egg-info/dependency_links.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       83 2023-04-24 13:04:25.000000 flet-material-0.2.0/flet_material.egg-info/entry_points.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       25 2023-04-24 13:04:25.000000 flet-material-0.2.0/flet_material.egg-info/requires.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       21 2023-04-24 13:04:25.000000 flet-material-0.2.0/flet_material.egg-info/top_level.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       24 2023-04-22 18:53:13.000000 flet-material-0.2.0/requirements.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-04-24 13:04:25.258414 flet-material-0.2.0/setup.cfg
+-rw-r--r--   0 ahmad      (501) staff       (20)      805 2023-04-24 13:04:08.000000 flet-material-0.2.0/setup.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.254038 flet-material-0.2.0/styles/
+-rw-r--r--   0 ahmad      (501) staff       (20)      271 2023-04-22 17:17:29.000000 flet-material-0.2.0/styles/__init__.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.256769 flet-material-0.2.0/styles/__pycache__/
+-rw-r--r--   0 ahmad      (501) staff       (20)      499 2023-04-22 17:17:29.000000 flet-material-0.2.0/styles/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)      708 2023-04-23 11:20:49.000000 flet-material-0.2.0/styles/__pycache__/admonition_style.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)      493 2023-04-22 17:30:06.000000 flet-material-0.2.0/styles/__pycache__/alert_style.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)      494 2023-04-22 17:08:25.000000 flet-material-0.2.0/styles/__pycache__/alert_styles.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)      487 2023-04-22 16:10:03.000000 flet-material-0.2.0/styles/__pycache__/badge_style.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)      287 2023-04-21 16:08:17.000000 flet-material-0.2.0/styles/__pycache__/fonts.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)     1040 2023-04-23 14:54:06.000000 flet-material-0.2.0/styles/__pycache__/theme.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)      908 2023-04-23 11:20:48.000000 flet-material-0.2.0/styles/admonition_style.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      378 2023-04-22 17:30:06.000000 flet-material-0.2.0/styles/alert_style.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      361 2023-04-22 16:10:02.000000 flet-material-0.2.0/styles/badge_style.py
+-rw-r--r--   0 ahmad      (501) staff       (20)       90 2023-04-21 16:07:16.000000 flet-material-0.2.0/styles/fonts.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1421 2023-04-23 14:18:26.000000 flet-material-0.2.0/styles/theme.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.257510 flet-material-0.2.0/tests/
+-rw-r--r--   0 ahmad      (501) staff       (20)      514 2023-04-23 19:11:47.000000 flet-material-0.2.0/tests/test_admonitions.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      392 2023-04-23 17:39:36.000000 flet-material-0.2.0/tests/test_buttons.py
```

### Comparing `flet-material-0.1.0/LICENSE` & `flet-material-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flet-material-0.1.0/command/new_project.py` & `flet-material-0.2.0/command/new_project.py`

 * *Files identical despite different names*

### Comparing `flet-material-0.1.0/docs/docs/controls/alerts.md` & `flet-material-0.2.0/docs/docs/controls/alerts.md`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,19 @@
 
 
 The ***alerts*** class is straightforward and easy to use. Choose where you want to place your annotation then create an instance of it, like this:
 
 
 <span style="font-size:1rem;">Basic Alerts Example</span>
 
-=== "*main()*"
+!!! tip "Flet Material Alerts"
+
+    The Flet Material Library classes inherit from the controls provided by Flet. In this case, the ```fm.Alerts()``` class inherits from Flet's ```ft.Container()``` class, this means all properties of the latter are accessable through the former. 
+
+=== "*Alerts*"
 
     ``` py linenums="1"
     import flet as ft
     import flet_material as fm
 
 
     fm.Theme.set_theme(theme="blue")
```

### Comparing `flet-material-0.1.0/docs/docs/controls/annotations.md` & `flet-material-0.2.0/docs/docs/controls/annotations.md`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,19 @@
 
 
 The ***annotations*** class is straightforward and easy to use. Choose where you want to place your annotation then create an instance of it, like this:
 
 
 <span style="font-size:1rem;">Basic Annotation Example</span>
 
-=== "*main()*"
+!!! tip "Flet Material Annotations"
+
+    The Flet Material Library classes inherit from the controls provided by Flet. In this case, the ```fm.Annotations()``` class inherits from Flet's ```ft.Container()``` class, this means all properties of the latter are accessable through the former. 
+
+=== "*Annotations*"
 
     ``` py linenums="1"
     import flet as ft
     import flet_material as fm
 
     def main(page: ft.Page):
```

### Comparing `flet-material-0.1.0/docs/docs/controls/badges.md` & `flet-material-0.2.0/docs/docs/controls/badges.md`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 
 
 The ***badges*** class is straightforward and easy to use. There are currently two types of badges, ***notifications*** and ***icon*** bagdes, each having its own unique material design. Choose where you want to place your annotation then create an instance of it, like this:
 
 
 <span style="font-size:1rem;">Basic Notifications Badge Example</span>
 
+!!! tip "Flet Material Badges"
+
+    The Flet Material Library classes inherit from the controls provided by Flet. In this case, both the ```fm.NotificationBadge()``` and the ```fm.IconBadge()``` classes inherit from Flet's ```ft.Container()``` class, this means all properties of the latter are accessable through the former. 
+
 === "*Notifications Badge*"
 
     ``` py linenums="1"
     import flet as ft
     import flet_material as fm
```

### Comparing `flet-material-0.1.0/docs/docs/controls/buttons.md` & `flet-material-0.2.0/docs/docs/controls/buttons.md`

 * *Files identical despite different names*

### Comparing `flet-material-0.1.0/docs/docs/controls/index.md` & `flet-material-0.2.0/docs/docs/controls/index.md`

 * *Files identical despite different names*

### Comparing `flet-material-0.1.0/docs/mkdocs.yml` & `flet-material-0.2.0/docs/mkdocs.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,38 @@
-site_name: Flet Material Design
-repo_name: LineIndent/material_design_flet
+# Project information
+site_name: Flet Material Library
+site_author: S. Ahmad P. Hakimi
+site_description: >-
+  UI component library built with Flet.
 
+# Repository
+repo_name: material_design_flet
 repo_url: https://github.com/LineIndent/material_design_flet
+
+# copyright
+copyright: Copyright &copy; 2023 S. Ahmad P. Hakimi
+
+# page tree
 nav:
   - Home: index.md
   - Controls:
       - controls/index.md
       - Annotations: controls/annotations.md
       - Alerts: controls/alerts.md
       - Badges: controls/badges.md
       - Buttons: controls/buttons.md
       - Checkboxes: controls/checkboxes.md
       - Chips: controls/chips.md
       - Dropdowns: controls/dropdowns.md
       - Switches: controls/switches.md
+  - Contribute: contribute.md
 
 theme:
   name: material
-  favicon: images/favicon.png
+  # favicon: images/favicon.png
   # logo:
   palette:
     scheme: slate
     primary: cyan
     accent: cyan
   font:
     text: Roboto
@@ -87,33 +98,26 @@
   - pymdownx.tasklist:
       custom_checkbox: true
   - pymdownx.emoji:
       emoji_index: !!python/name:materialx.emoji.twemoji
       emoji_generator: !!python/name:materialx.emoji.to_svg
 
 extra:
-  # made by Material MkDoc signature at footer
   generator: false
-
-  # social media icons and links
   social:
     - icon: fontawesome/brands/youtube
-      # link:
+      link: https://www.youtube.com/@lineindent
 
     - icon: fontawesome/brands/github
-      # link:
+      link: https://github.com/LineIndent
 
     - icon: fontawesome/brands/patreon
-      # link:
-
-  # form for cookies
+      link: https://www.patreon.com/user?u=87176956
   consent:
     title: Cookie consent
     description: >-
       We use cookies to recognize your repeated visits and preferences, as well
       as to measure the effectiveness of our documentation and whether users
       find what they're searching for. With your consent, you're helping us to
       make our documentation better.
 
-copyright: Copyright &copy; 2023 S. Ahmad P. Hakimi
-
 docs_dir: docs
```

### Comparing `flet-material-0.1.0/flet_material/__pycache__/__init__.cpython-310.pyc` & `flet-material-0.2.0/flet_material/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flet-material-0.1.0/flet_material/__pycache__/admonition.cpython-310.pyc` & `flet-material-0.2.0/flet_material/__pycache__/admonition.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 23 11:11:36 2023 UTC, .py size: 6416 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6812 4564 1019 0000  o.......h.Ed....
+00000000: 6f0d 0d0a 0000 0000 936b 4664 071b 0000  o........kFd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 6d04 5a04 0100 4700 6403 6404 8400 6404  m.Z...G.d.d...d.
 00000050: 6501 6a05 8303 5a06 4700 6405 6406 8400  e.j...Z.G.d.d...
 00000060: 6406 6501 6a05 8303 5a07 6401 5300 2907  d.e.j...Z.d.S.).
 00000070: e900 0000 004e 2902 da18 6164 6d6f 6e69  .....N)...admoni
@@ -11,235 +11,244 @@
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0800 0000 0000 0000 7336 0000 0065 005a  ........s6...e.Z
 000000c0: 0164 005a 0264 0165 0364 0265 0464 0365  .d.Z.d.e.d.e.d.e
 000000d0: 0564 0465 0666 0887 0066 0164 0564 0684  .d.e.f...f.d.d..
 000000e0: 0c5a 0764 0764 0884 005a 0887 0004 005a  .Z.d.d...Z.....Z
 000000f0: 0953 0029 09da 0b41 646d 6f6e 6974 696f  .S.)...Admonitio
 00000100: 6e73 da05 7479 7065 5fda 0f65 7870 616e  ns..type_..expan
-00000110: 6465 645f 6865 6967 6874 da06 6578 7061  ded_height..expa
-00000120: 6e64 da0d 636f 6e74 726f 6c73 5f6c 6973  nd..controls_lis
-00000130: 7463 0500 0000 0000 0000 0000 0000 0d00  tc..............
-00000140: 0000 1100 0000 0f00 0000 73ce 0100 007c  ..........s....|
-00000150: 0288 005f 0074 016a 027c 0464 018d 0188  ..._.t.j.|.d....
-00000160: 005f 0374 04a0 057c 0169 00a1 02a0 0564  ._.t...|.i.....d
-00000170: 0264 03a1 027d 0774 04a0 057c 0169 00a1  .d...}.t...|.i..
-00000180: 02a0 0564 0464 05a1 027d 0874 04a0 057c  ...d.d...}.t...|
-00000190: 0169 00a1 02a0 0564 0664 05a1 027d 0974  .i.....d.d...}.t
-000001a0: 06a0 0564 0769 00a1 027d 0a7c 0aa0 0564  ...d.i...}.|...d
-000001b0: 08a1 017d 0b7c 0aa0 0564 09a1 017d 0c74  ...}.|...d...}.t
-000001c0: 016a 0764 0a74 016a 08a0 0964 0b7c 07a1  .j.d.t.j...d.|..
-000001d0: 0264 0c64 0d74 016a 0a74 016a 0b6a 0c74  .d.d.t.j.t.j.j.t
-000001e0: 016a 0a64 0e64 0d74 016a 0d7c 097c 0864  .j.d.d.t.j.|.|.d
-000001f0: 0f64 108d 0374 016a 0e7c 01a0 0fa1 007c  .d...t.j.|.....|
-00000200: 0c7c 0b64 1164 128d 0467 0264 138d 0374  .|.d.d...g.d...t
-00000210: 016a 1074 016a 116a 1264 147c 0874 01a0  .j.t.j.j.d.|.t..
-00000220: 1364 1574 016a 146a 15a1 0274 01a0 1664  .d.t.j.j...t...d
-00000230: 1664 17a1 0287 0066 0164 1864 1984 0864  .d.....f.d.d...d
-00000240: 1a8d 0667 0264 1b8d 0264 1c8d 0588 005f  ...g.d...d....._
-00000250: 177c 06a0 1864 1d74 016a 1964 1e64 1474  .|...d.t.j.d.d.t
-00000260: 016a 08a0 0964 1f64 20a1 0274 01a0 1a64  .j...d.d ..t...d
-00000270: 2164 21a1 0264 228d 04a1 0201 007c 06a0  !d!..d"......|..
-00000280: 1864 2374 016a 1ba0 1c64 247c 08a1 02a1  .d#t.j...d$|....
-00000290: 0201 007c 06a0 1864 2574 016a 1d6a 1ea1  ...|...d%t.j.j..
-000002a0: 0201 007c 06a0 1864 2674 01a0 1664 2764  ...|...d&t...d'd
-000002b0: 28a1 02a1 0201 007c 06a0 1864 297c 03a1  (......|...d)|..
-000002c0: 0201 007c 06a0 1864 2a64 0ca1 0201 007c  ...|...d*d.....|
-000002d0: 06a0 1864 2b64 2ca1 0201 007c 06a0 1864  ...d+d,....|...d
-000002e0: 2d64 15a1 0201 007c 06a0 1864 2e74 016a  -d.....|...d.t.j
-000002f0: 0264 2f64 1588 006a 1788 006a 0367 0264  .d/d...j...j.g.d
-00000300: 308d 03a1 0201 0074 1f83 006a 207c 0569  0......t...j |.i
-00000310: 007c 06a4 018e 0101 0064 0053 0029 314e  .|.......d.S.)1N
-00000320: 2901 da08 636f 6e74 726f 6c73 da07 6267  )...controls..bg
-00000330: 636f 6c6f 72fa 0723 3230 3232 3263 da0c  color..#20222c..
-00000340: 626f 7264 6572 5f63 6f6c 6f72 da07 7768  border_color..wh
-00000350: 6974 6532 34da 0469 636f 6eda 1161 646d  ite24..icon..adm
-00000360: 6f6e 6974 696f 6e73 5f74 6974 6c65 da0b  onitions_title..
-00000370: 666f 6e74 5f66 616d 696c 79da 0473 697a  font_family..siz
-00000380: 65e9 3a00 0000 e766 6666 6666 66ee 3fe9  e.:....ffffff.?.
-00000390: 0600 0000 e90a 0000 00da 0663 656e 7465  ...........cente
-000003a0: 72e9 1200 0000 a903 da04 6e61 6d65 da05  r.........name..
-000003b0: 636f 6c6f 7272 1100 0000 da04 7737 3030  colorr......w700
-000003c0: a903 7211 0000 0072 1000 0000 da06 7765  ..r....r......we
-000003d0: 6967 6874 a903 da12 7665 7274 6963 616c  ight....vertical
-000003e0: 5f61 6c69 676e 6d65 6e74 da07 7370 6163  _alignment..spac
-000003f0: 696e 6772 0900 0000 e90f 0000 0072 0100  ingr.........r..
-00000400: 0000 6990 0100 00da 0b65 6173 654f 7574  ..i......easeOut
-00000410: 4261 636b 6301 0000 0000 0000 0000 0000  Backc...........
-00000420: 0001 0000 0003 0000 0013 0000 0073 0a00  .............s..
-00000430: 0000 8800 a000 7c00 a101 5300 2901 4e29  ......|...S.).N)
-00000440: 01da 1172 6573 697a 655f 6164 6d6f 6e69  ...resize_admoni
-00000450: 7469 6f6e 2901 da01 65a9 01da 0473 656c  tion)...e....sel
-00000460: 66a9 00fa 4d2f 5573 6572 732f 6168 6d61  f...M/Users/ahma
-00000470: 642f 436f 6465 7370 6163 652f 5079 7468  d/Codespace/Pyth
-00000480: 6f6e 2f66 6c65 742d 6d61 7465 7269 616c  on/flet-material
-00000490: 2d64 756d 6d79 2f66 6c65 745f 6d61 7465  -dummy/flet_mate
-000004a0: 7269 616c 2f61 646d 6f6e 6974 696f 6e2e  rial/admonition.
-000004b0: 7079 da08 3c6c 616d 6264 613e 3f00 0000  py..<lambda>?...
-000004c0: 7302 0000 000a 007a 2641 646d 6f6e 6974  s......z&Admonit
-000004d0: 696f 6e73 2e5f 5f69 6e69 745f 5f2e 3c6c  ions.__init__.<l
-000004e0: 6f63 616c 733e 2e3c 6c61 6d62 6461 3e29  ocals>.<lambda>)
-000004f0: 0672 0e00 0000 da09 6963 6f6e 5f73 697a  .r......icon_siz
-00000500: 65da 0a69 636f 6e5f 636f 6c6f 72da 0672  e..icon_color..r
-00000510: 6f74 6174 65da 1061 6e69 6d61 7465 5f72  otate..animate_r
-00000520: 6f74 6174 696f 6eda 086f 6e5f 636c 6963  otation..on_clic
-00000530: 6ba9 02da 0961 6c69 676e 6d65 6e74 7209  k....alignmentr.
-00000540: 0000 00a9 05da 0668 6569 6768 7472 0a00  .......heightr..
-00000550: 0000 da0d 626f 7264 6572 5f72 6164 6975  ....border_radiu
-00000560: 73da 0770 6164 6469 6e67 da07 636f 6e74  s..padding..cont
-00000570: 656e 74da 0673 6861 646f 77e9 0800 0000  ent..shadow.....
-00000580: e766 6666 6666 66d6 3fda 0562 6c61 636b  .ffffff.?..black
-00000590: e904 0000 00a9 04da 0d73 7072 6561 645f  .........spread_
-000005a0: 7261 6469 7573 da0b 626c 7572 5f72 6164  radius..blur_rad
-000005b0: 6975 7372 1a00 0000 da06 6f66 6673 6574  iusr......offset
-000005c0: da06 626f 7264 6572 e733 3333 3333 33eb  ..border.333333.
-000005d0: 3fda 0d63 6c69 705f 6265 6861 7669 6f72  ?..clip_behavior
-000005e0: da07 616e 696d 6174 65e9 2c01 0000 da0a  ..animate.,.....
-000005f0: 6465 6365 6c65 7261 7465 7207 0000 0072  decelerater....r
-00000600: 3300 0000 7232 0000 00e9 3c00 0000 7234  3...r2....<...r4
-00000610: 0000 0072 3500 0000 da05 7374 6172 74a9  ...r5.....start.
-00000620: 0372 3000 0000 7220 0000 0072 0900 0000  .r0...r ...r....
-00000630: 2921 7206 0000 00da 0266 74da 0643 6f6c  )!r......ft..Col
-00000640: 756d 6eda 0663 6f6c 756d 6e72 0200 0000  umn..columnr....
-00000650: da03 6765 7472 0300 0000 da09 436f 6e74  ..getr......Cont
-00000660: 6169 6e65 72da 0663 6f6c 6f72 73da 0c77  ainer..colors..w
-00000670: 6974 685f 6f70 6163 6974 79da 0352 6f77  ith_opacity..Row
-00000680: da11 4d61 696e 4178 6973 416c 6967 6e6d  ..MainAxisAlignm
-00000690: 656e 74da 0d53 5041 4345 5f42 4554 5745  ent..SPACE_BETWE
-000006a0: 454e da04 4963 6f6e da04 5465 7874 da0a  EN..Icon..Text..
-000006b0: 6361 7069 7461 6c69 7a65 da0a 4963 6f6e  capitalize..Icon
-000006c0: 4275 7474 6f6e da05 6963 6f6e 73da 0341  Button..icons..A
-000006d0: 4444 da06 526f 7461 7465 7230 0000 0072  DD..Rotater0...r
-000006e0: 1600 0000 da09 416e 696d 6174 696f 6eda  ......Animation.
-000006f0: 0963 6f6e 7461 696e 6572 da0a 7365 7464  .container..setd
-00000700: 6566 6175 6c74 da09 426f 7853 6861 646f  efault..BoxShado
-00000710: 77da 064f 6666 7365 7472 3f00 0000 da03  w..Offsetr?.....
-00000720: 616c 6cda 0c43 6c69 7042 6568 6176 696f  all..ClipBehavio
-00000730: 72da 0948 4152 445f 4544 4745 da05 7375  r..HARD_EDGE..su
-00000740: 7065 72da 085f 5f69 6e69 745f 5f29 0d72  per..__init__).r
-00000750: 2600 0000 7205 0000 0072 0600 0000 7207  &...r....r....r.
-00000760: 0000 0072 0800 0000 da04 6172 6773 da06  ...r......args..
-00000770: 6b77 6172 6773 720a 0000 0072 0c00 0000  kwargsr....r....
-00000780: 720e 0000 00da 0566 6f6e 7473 da0a 7469  r......fonts..ti
-00000790: 746c 655f 666f 6e74 da0a 7469 746c 655f  tle_font..title_
-000007a0: 7369 7a65 a901 da09 5f5f 636c 6173 735f  size....__class_
-000007b0: 5f72 2500 0000 7228 0000 0072 6200 0000  _r%...r(...rb...
-000007c0: 0600 0000 7392 0000 0006 0a04 0102 0108  ....s...........
-000007d0: ff14 050c 0104 0104 ff14 030c 020a 010a  ................
-000007e0: 0104 0202 010c 0102 0102 0104 0106 0104  ................
-000007f0: 0202 0102 0104 0202 0102 0102 0104 fd04  ................
-00000800: 0506 0102 0102 0102 0104 fc02 fa04 fd04  ................
-00000810: 1106 0102 0102 010e 010a 010a 0104 fa02  ................
-00000820: ee04 fe08 fb04 2602 0104 0102 0102 010c  ......&.........
-00000830: 010a 0104 fc04 fe16 0910 0114 010c 010c  ................
-00000840: 010c 010c 0104 0102 0104 0102 0102 0104  ................
-00000850: 0204 0102 fe04 fd04 fe16 0c7a 1441 646d  ...........z.Adm
-00000860: 6f6e 6974 696f 6e73 2e5f 5f69 6e69 745f  onitions.__init_
-00000870: 5f63 0200 0000 0000 0000 0000 0000 0200  _c..............
-00000880: 0000 0400 0000 4300 0000 736c 0000 007c  ......C...sl...|
-00000890: 006a 007c 006a 016b 0372 1f7c 006a 017c  .j.|.j.k.r.|.j.|
-000008a0: 005f 0074 026a 036a 0464 0164 0164 028d  ._.t.j.j.d.d.d..
-000008b0: 027c 006a 055f 0374 02a0 0664 0374 026a  .|.j._.t...d.t.j
-000008c0: 076a 08a1 027c 016a 095f 0a6e 1164 047c  .j...|.j._.n.d.|
-000008d0: 005f 0074 02a0 0664 0574 026a 076a 08a1  ._.t...d.t.j.j..
-000008e0: 027c 016a 095f 0a64 017c 006a 055f 037c  .|.j._.d.|.j._.|
-000008f0: 00a0 0ba1 0001 0064 0053 0029 064e 7214  .......d.S.).Nr.
-00000900: 0000 0029 02da 0774 6f70 4c65 6674 da08  ...)...topLeft..
-00000910: 746f 7052 6967 6874 6700 0000 0000 00e8  topRightg.......
-00000920: 3f72 4500 0000 7201 0000 0029 0c72 3200  ?rE...r....).r2.
-00000930: 0000 7206 0000 0072 4800 0000 7233 0000  ..r....rH...r3..
-00000940: 00da 046f 6e6c 7972 5a00 0000 7258 0000  ...onlyrZ...rX..
-00000950: 0072 3000 0000 7216 0000 00da 0763 6f6e  .r0...r......con
-00000960: 7472 6f6c 722c 0000 00da 0675 7064 6174  trolr,.....updat
-00000970: 6529 0272 2600 0000 7224 0000 0072 2700  e).r&...r$...r'.
-00000980: 0000 7227 0000 0072 2800 0000 7223 0000  ..r'...r(...r#..
-00000990: 0065 0000 0073 1000 0000 0c01 0801 1401  .e...s..........
-000009a0: 1601 0602 1401 0801 0c02 7a1d 4164 6d6f  ..........z.Admo
-000009b0: 6e69 7469 6f6e 732e 7265 7369 7a65 5f61  nitions.resize_a
-000009c0: 646d 6f6e 6974 696f 6e29 0ada 085f 5f6e  dmonition)...__n
-000009d0: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-000009e0: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
-000009f0: 0373 7472 da03 696e 74da 0462 6f6f 6cda  .str..int..bool.
-00000a00: 046c 6973 7472 6200 0000 7223 0000 00da  .listrb...r#....
-00000a10: 0d5f 5f63 6c61 7373 6365 6c6c 5f5f 7227  .__classcell__r'
-00000a20: 0000 0072 2700 0000 7268 0000 0072 2800  ...r'...rh...r(.
-00000a30: 0000 7204 0000 0005 0000 0073 1600 0000  ..r........s....
-00000a40: 0800 0201 0202 02fe 0203 02fd 0204 02fc  ................
-00000a50: 0205 0efb 105f 7204 0000 0063 0000 0000  ....._r....c....
-00000a60: 0000 0000 0000 0000 0000 0000 0400 0000  ................
-00000a70: 0000 0000 7326 0000 0065 005a 0164 005a  ....s&...e.Z.d.Z
-00000a80: 0264 0165 0364 0265 0466 0487 0066 0164  .d.e.d.e.f...f.d
-00000a90: 0364 0484 0c5a 0587 0004 005a 0653 0029  .d...Z.....Z.S.)
-00000aa0: 05da 1046 6978 6564 4164 6d6f 6e69 7469  ...FixedAdmoniti
-00000ab0: 6f6e 7372 0500 0000 7207 0000 0063 0300  onsr....r....c..
-00000ac0: 0000 0000 0000 0000 0000 0b00 0000 1100  ................
-00000ad0: 0000 0f00 0000 7382 0100 0074 00a0 017c  ......s....t...|
-00000ae0: 0169 00a1 02a0 0164 0164 02a1 027d 0574  .i.....d.d...}.t
-00000af0: 00a0 017c 0169 00a1 02a0 0164 0364 04a1  ...|.i.....d.d..
-00000b00: 027d 0674 00a0 017c 0169 00a1 02a0 0164  .}.t...|.i.....d
-00000b10: 0564 04a1 027d 0774 02a0 0164 0669 00a1  .d...}.t...d.i..
-00000b20: 027d 087c 08a0 0164 07a1 017d 097c 08a0  .}.|...d...}.|..
-00000b30: 0164 08a1 017d 0a74 036a 0464 0974 036a  .d...}.t.j.d.t.j
-00000b40: 05a0 0664 0a7c 05a1 0264 0b64 0c74 036a  ...d.|...d.d.t.j
-00000b50: 0774 036a 086a 0974 036a 0764 0d64 0c74  .t.j.j.t.j.d.d.t
-00000b60: 036a 0a7c 077c 0664 0e64 0f8d 0374 036a  .j.|.|.d.d...t.j
-00000b70: 0b7c 01a0 0ca1 007c 0a7c 0964 1064 118d  .|.....|.|.d.d..
-00000b80: 0467 0264 128d 0367 0164 138d 0264 148d  .g.d...g.d...d..
-00000b90: 057c 005f 0d7c 04a0 0e64 1574 036a 0f64  .|._.|...d.t.j.d
-00000ba0: 1664 1774 036a 05a0 0664 1864 19a1 0274  .d.t.j...d.d...t
-00000bb0: 03a0 1064 1a64 1aa1 0264 1b8d 04a1 0201  ...d.d...d......
-00000bc0: 007c 04a0 0e64 1c74 036a 11a0 1264 1d7c  .|...d.t.j...d.|
-00000bd0: 06a1 02a1 0201 007c 04a0 0e64 1e74 036a  .......|...d.t.j
-00000be0: 136a 14a1 0201 007c 04a0 0e64 1f74 03a0  .j.....|...d.t..
-00000bf0: 1564 2064 21a1 02a1 0201 007c 04a0 0e64  .d d!......|...d
-00000c00: 227c 02a1 0201 007c 04a0 0e64 2364 0ba1  "|.....|...d#d..
-00000c10: 0201 007c 04a0 0e64 2464 25a1 0201 007c  ...|...d$d%....|
-00000c20: 04a0 0e64 2664 27a1 0201 007c 04a0 0e64  ...d&d'....|...d
-00000c30: 2874 036a 1664 2964 277c 006a 0d67 0164  (t.j.d)d'|.j.g.d
-00000c40: 2a8d 03a1 0201 0074 1783 006a 187c 0369  *......t...j.|.i
-00000c50: 007c 04a4 018e 0101 0064 0053 0029 2b4e  .|.......d.S.)+N
-00000c60: 720a 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
-00000c70: 0d00 0000 720e 0000 0072 0f00 0000 7210  ....r....r....r.
-00000c80: 0000 0072 1100 0000 7212 0000 0072 1300  ...r....r....r..
-00000c90: 0000 7214 0000 0072 1500 0000 7216 0000  ..r....r....r...
-00000ca0: 0072 1700 0000 7218 0000 0072 1b00 0000  .r....r....r....
-00000cb0: 721c 0000 0072 1e00 0000 722f 0000 0072  r....r....r/...r
-00000cc0: 3100 0000 7236 0000 0072 3700 0000 7221  1...r6...r7...r!
-00000cd0: 0000 0072 3800 0000 7239 0000 0072 3a00  ...r8...r9...r:.
-00000ce0: 0000 723b 0000 0072 3f00 0000 7240 0000  ..r;...r?...r@..
-00000cf0: 0072 4100 0000 7242 0000 0072 4300 0000  .rA...rB...rC...
-00000d00: 7244 0000 0072 0700 0000 7233 0000 0072  rD...r....r3...r
-00000d10: 3200 0000 7245 0000 0072 3400 0000 7201  2...rE...r4...r.
-00000d20: 0000 0072 3500 0000 7246 0000 0072 4700  ...r5...rF...rG.
-00000d30: 0000 2919 7202 0000 0072 4b00 0000 7203  ..).r....rK...r.
-00000d40: 0000 0072 4800 0000 724c 0000 0072 4d00  ...rH...rL...rM.
-00000d50: 0000 724e 0000 0072 4f00 0000 7250 0000  ..rN...rO...rP..
-00000d60: 0072 5100 0000 7252 0000 0072 5300 0000  .rQ...rR...rS...
-00000d70: 7254 0000 0072 5a00 0000 725b 0000 0072  rT...rZ...r[...r
-00000d80: 5c00 0000 725d 0000 0072 3f00 0000 725e  \...r]...r?...r^
-00000d90: 0000 0072 5f00 0000 7260 0000 0072 5900  ...r_...r`...rY.
-00000da0: 0000 7249 0000 0072 6100 0000 7262 0000  ..rI...ra...rb..
-00000db0: 0029 0b72 2600 0000 7205 0000 0072 0700  .).r&...r....r..
-00000dc0: 0000 7263 0000 0072 6400 0000 720a 0000  ..rc...rd...r...
-00000dd0: 0072 0c00 0000 720e 0000 0072 6500 0000  .r....r....re...
-00000de0: 7266 0000 0072 6700 0000 7268 0000 0072  rf...rg...rh...r
-00000df0: 2700 0000 7228 0000 0072 6200 0000 7300  '...r(...rb...s.
-00000e00: 0000 7378 0000 0014 020c 0104 0104 ff14  ..sx............
-00000e10: 030c 020a 010a 0104 0202 010c 0102 0102  ................
-00000e20: 0104 0106 0104 0202 0102 0104 0202 0102  ................
-00000e30: 0102 0104 fd04 0506 0102 0102 0102 0104  ................
-00000e40: fc02 fa04 fd02 ff04 fe08 fb04 1e02 0104  ................
-00000e50: 0102 0102 010c 010a 0104 fc04 fe16 0910  ................
-00000e60: 0114 010c 010c 010c 010c 0104 0102 0104  ................
-00000e70: 0102 0102 0104 0202 ff04 fd04 fe16 0b7a  ...............z
-00000e80: 1946 6978 6564 4164 6d6f 6e69 7469 6f6e  .FixedAdmonition
-00000e90: 732e 5f5f 696e 6974 5f5f 2907 726f 0000  s.__init__).ro..
-00000ea0: 0072 7000 0000 7271 0000 0072 7200 0000  .rp...rq...rr...
-00000eb0: 7274 0000 0072 6200 0000 7276 0000 0072  rt...rb...rv...r
-00000ec0: 2700 0000 7227 0000 0072 6800 0000 7228  '...r'...rh...r(
-00000ed0: 0000 0072 7700 0000 7200 0000 7304 0000  ...rw...r...s...
-00000ee0: 0008 001e 0172 7700 0000 2908 da04 666c  .....rw...)...fl
-00000ef0: 6574 7248 0000 00da 0673 7479 6c65 7372  etrH.....stylesr
-00000f00: 0200 0000 7203 0000 0072 4c00 0000 7204  ....r....rL...r.
-00000f10: 0000 0072 7700 0000 7227 0000 0072 2700  ...rw...r'...r'.
-00000f20: 0000 7227 0000 0072 2800 0000 da08 3c6d  ..r'...r(.....<m
-00000f30: 6f64 756c 653e 0100 0000 7308 0000 0008  odule>....s.....
-00000f40: 0010 0112 0316 6d                        ......m
+00000110: 6465 645f 6865 6967 6874 da08 6578 7061  ded_height..expa
+00000120: 6e64 6564 da0d 636f 6e74 726f 6c73 5f6c  nded..controls_l
+00000130: 6973 7463 0500 0000 0000 0000 0000 0000  istc............
+00000140: 0d00 0000 1100 0000 0f00 0000 73ec 0100  ............s...
+00000150: 007c 0188 005f 007c 0288 005f 017c 0388  .|..._.|..._.|..
+00000160: 005f 027c 0488 005f 0374 046a 0588 006a  ._.|..._.t.j...j
+00000170: 0364 018d 0188 005f 0674 07a0 0888 006a  .d....._.t.....j
+00000180: 0069 00a1 02a0 0864 0264 03a1 027d 0774  .i.....d.d...}.t
+00000190: 07a0 0888 006a 0069 00a1 02a0 0864 0464  .....j.i.....d.d
+000001a0: 05a1 027d 0874 07a0 0888 006a 0069 00a1  ...}.t.....j.i..
+000001b0: 02a0 0864 0664 05a1 027d 0974 09a0 0864  ...d.d...}.t...d
+000001c0: 0769 00a1 027d 0a7c 0aa0 0864 08a1 017d  .i...}.|...d...}
+000001d0: 0b7c 0aa0 0864 09a1 017d 0c74 046a 0a64  .|...d...}.t.j.d
+000001e0: 0a74 046a 0ba0 0c64 0b7c 07a1 0264 0c64  .t.j...d.|...d.d
+000001f0: 0d74 046a 0d74 046a 0e6a 0f74 046a 0d64  .t.j.t.j.j.t.j.d
+00000200: 0e64 0d74 046a 107c 097c 0864 0f64 108d  .d.t.j.|.|.d.d..
+00000210: 0374 046a 1188 006a 00a0 12a1 007c 0c7c  .t.j...j.....|.|
+00000220: 0b64 1164 128d 0467 0264 138d 0374 046a  .d.d...g.d...t.j
+00000230: 1374 046a 146a 1564 147c 0874 04a0 1664  .t.j.j.d.|.t...d
+00000240: 1574 046a 176a 18a1 0274 04a0 1964 1664  .t.j.j...t...d.d
+00000250: 17a1 0287 0066 0164 1864 1984 0864 1a8d  .....f.d.d...d..
+00000260: 0667 0264 1b8d 0264 1c8d 0588 005f 1a7c  .g.d...d....._.|
+00000270: 06a0 1b64 1d74 046a 1c64 1e64 1474 046a  ...d.t.j.d.d.t.j
+00000280: 0ba0 0c64 1f64 20a1 0274 04a0 1d64 2164  ...d.d ..t...d!d
+00000290: 21a1 0264 228d 04a1 0201 007c 06a0 1b64  !..d"......|...d
+000002a0: 2374 046a 1ea0 1f64 247c 08a1 02a1 0201  #t.j...d$|......
+000002b0: 007c 06a0 1b64 2574 046a 206a 21a1 0201  .|...d%t.j j!...
+000002c0: 007c 06a0 1b64 2674 04a0 1964 2764 28a1  .|...d&t...d'd(.
+000002d0: 02a1 0201 007c 06a0 1b64 2988 006a 02a1  .....|...d)..j..
+000002e0: 0201 007c 06a0 1b64 2a64 0ca1 0201 007c  ...|...d*d.....|
+000002f0: 06a0 1b64 2b64 2ca1 0201 007c 06a0 1b64  ...d+d,....|...d
+00000300: 2d64 15a1 0201 007c 06a0 1b64 2e74 046a  -d.....|...d.t.j
+00000310: 0564 2f64 1588 006a 1a88 006a 0667 0264  .d/d...j...j.g.d
+00000320: 308d 03a1 0201 0074 2283 006a 237c 0569  0......t"..j#|.i
+00000330: 007c 06a4 018e 0101 0064 0053 0029 314e  .|.......d.S.)1N
+00000340: 2901 da08 636f 6e74 726f 6c73 da07 6267  )...controls..bg
+00000350: 636f 6c6f 72fa 0723 3230 3232 3263 da0c  color..#20222c..
+00000360: 626f 7264 6572 5f63 6f6c 6f72 da07 7768  border_color..wh
+00000370: 6974 6532 34da 0469 636f 6eda 1161 646d  ite24..icon..adm
+00000380: 6f6e 6974 696f 6e73 5f74 6974 6c65 da0b  onitions_title..
+00000390: 666f 6e74 5f66 616d 696c 79da 0473 697a  font_family..siz
+000003a0: 65e9 3a00 0000 e766 6666 6666 66ee 3fe9  e.:....ffffff.?.
+000003b0: 0600 0000 e90a 0000 00da 0663 656e 7465  ...........cente
+000003c0: 72e9 1200 0000 a903 da04 6e61 6d65 da05  r.........name..
+000003d0: 636f 6c6f 7272 1100 0000 da04 7737 3030  colorr......w700
+000003e0: a903 7211 0000 0072 1000 0000 da06 7765  ..r....r......we
+000003f0: 6967 6874 a903 da12 7665 7274 6963 616c  ight....vertical
+00000400: 5f61 6c69 676e 6d65 6e74 da07 7370 6163  _alignment..spac
+00000410: 696e 6772 0900 0000 e90f 0000 0072 0100  ingr.........r..
+00000420: 0000 6990 0100 00da 0b65 6173 654f 7574  ..i......easeOut
+00000430: 4261 636b 6301 0000 0000 0000 0000 0000  Backc...........
+00000440: 0001 0000 0003 0000 0013 0000 0073 0a00  .............s..
+00000450: 0000 8800 a000 7c00 a101 5300 2901 4e29  ......|...S.).N)
+00000460: 01da 1172 6573 697a 655f 6164 6d6f 6e69  ...resize_admoni
+00000470: 7469 6f6e 2901 da01 65a9 01da 0473 656c  tion)...e....sel
+00000480: 66a9 00fa 4d2f 5573 6572 732f 6168 6d61  f...M/Users/ahma
+00000490: 642f 436f 6465 7370 6163 652f 5079 7468  d/Codespace/Pyth
+000004a0: 6f6e 2f66 6c65 742d 6d61 7465 7269 616c  on/flet-material
+000004b0: 2d64 756d 6d79 2f66 6c65 745f 6d61 7465  -dummy/flet_mate
+000004c0: 7269 616c 2f61 646d 6f6e 6974 696f 6e2e  rial/admonition.
+000004d0: 7079 da08 3c6c 616d 6264 613e 4400 0000  py..<lambda>D...
+000004e0: 7302 0000 000a 007a 2641 646d 6f6e 6974  s......z&Admonit
+000004f0: 696f 6e73 2e5f 5f69 6e69 745f 5f2e 3c6c  ions.__init__.<l
+00000500: 6f63 616c 733e 2e3c 6c61 6d62 6461 3e29  ocals>.<lambda>)
+00000510: 0672 0e00 0000 da09 6963 6f6e 5f73 697a  .r......icon_siz
+00000520: 65da 0a69 636f 6e5f 636f 6c6f 72da 0672  e..icon_color..r
+00000530: 6f74 6174 65da 1061 6e69 6d61 7465 5f72  otate..animate_r
+00000540: 6f74 6174 696f 6eda 086f 6e5f 636c 6963  otation..on_clic
+00000550: 6ba9 02da 0961 6c69 676e 6d65 6e74 7209  k....alignmentr.
+00000560: 0000 00a9 05da 0668 6569 6768 7472 0a00  .......heightr..
+00000570: 0000 da0d 626f 7264 6572 5f72 6164 6975  ....border_radiu
+00000580: 73da 0770 6164 6469 6e67 da07 636f 6e74  s..padding..cont
+00000590: 656e 74da 0673 6861 646f 77e9 0800 0000  ent..shadow.....
+000005a0: e766 6666 6666 66d6 3fda 0562 6c61 636b  .ffffff.?..black
+000005b0: e904 0000 00a9 04da 0d73 7072 6561 645f  .........spread_
+000005c0: 7261 6469 7573 da0b 626c 7572 5f72 6164  radius..blur_rad
+000005d0: 6975 7372 1a00 0000 da06 6f66 6673 6574  iusr......offset
+000005e0: da06 626f 7264 6572 e733 3333 3333 33eb  ..border.333333.
+000005f0: 3fda 0d63 6c69 705f 6265 6861 7669 6f72  ?..clip_behavior
+00000600: da07 616e 696d 6174 65e9 2c01 0000 da0a  ..animate.,.....
+00000610: 6465 6365 6c65 7261 7465 da06 6578 7061  decelerate..expa
+00000620: 6e64 7233 0000 0072 3200 0000 e93c 0000  ndr3...r2....<..
+00000630: 0072 3400 0000 7235 0000 00da 0573 7461  .r4...r5.....sta
+00000640: 7274 a903 7230 0000 0072 2000 0000 7209  rt..r0...r ...r.
+00000650: 0000 0029 2472 0500 0000 7206 0000 0072  ...)$r....r....r
+00000660: 0700 0000 7208 0000 00da 0266 74da 0643  ....r......ft..C
+00000670: 6f6c 756d 6eda 0663 6f6c 756d 6e72 0200  olumn..columnr..
+00000680: 0000 da03 6765 7472 0300 0000 da09 436f  ....getr......Co
+00000690: 6e74 6169 6e65 72da 0663 6f6c 6f72 73da  ntainer..colors.
+000006a0: 0c77 6974 685f 6f70 6163 6974 79da 0352  .with_opacity..R
+000006b0: 6f77 da11 4d61 696e 4178 6973 416c 6967  ow..MainAxisAlig
+000006c0: 6e6d 656e 74da 0d53 5041 4345 5f42 4554  nment..SPACE_BET
+000006d0: 5745 454e da04 4963 6f6e da04 5465 7874  WEEN..Icon..Text
+000006e0: da0a 6361 7069 7461 6c69 7a65 da0a 4963  ..capitalize..Ic
+000006f0: 6f6e 4275 7474 6f6e da05 6963 6f6e 73da  onButton..icons.
+00000700: 0341 4444 da06 526f 7461 7465 7230 0000  .ADD..Rotater0..
+00000710: 0072 1600 0000 da09 416e 696d 6174 696f  .r......Animatio
+00000720: 6eda 0963 6f6e 7461 696e 6572 da0a 7365  n..container..se
+00000730: 7464 6566 6175 6c74 da09 426f 7853 6861  tdefault..BoxSha
+00000740: 646f 77da 064f 6666 7365 7472 3f00 0000  dow..Offsetr?...
+00000750: da03 616c 6cda 0c43 6c69 7042 6568 6176  ..all..ClipBehav
+00000760: 696f 72da 0948 4152 445f 4544 4745 da05  ior..HARD_EDGE..
+00000770: 7375 7065 72da 085f 5f69 6e69 745f 5f29  super..__init__)
+00000780: 0d72 2600 0000 7205 0000 0072 0600 0000  .r&...r....r....
+00000790: 7207 0000 0072 0800 0000 da04 6172 6773  r....r......args
+000007a0: da06 6b77 6172 6773 720a 0000 0072 0c00  ..kwargsr....r..
+000007b0: 0000 720e 0000 00da 0566 6f6e 7473 da0a  ..r......fonts..
+000007c0: 7469 746c 655f 666f 6e74 da0a 7469 746c  title_font..titl
+000007d0: 655f 7369 7a65 a901 da09 5f5f 636c 6173  e_size....__clas
+000007e0: 735f 5f72 2500 0000 7228 0000 0072 6300  s__r%...r(...rc.
+000007f0: 0000 0600 0000 7398 0000 0006 0a06 0106  ......s.........
+00000800: 0106 0104 0304 0108 ff16 050e 0104 0104  ................
+00000810: ff16 030c 020a 010a 0104 0202 010c 0102  ................
+00000820: 0102 0104 0106 0104 0202 0102 0104 0202  ................
+00000830: 0102 0102 0104 fd04 0508 0102 0102 0102  ................
+00000840: 0104 fc02 fa04 fd04 1106 0102 0102 010e  ................
+00000850: 010a 010a 0104 fa02 ee04 fe08 fb04 2602  ..............&.
+00000860: 0104 0102 0102 010c 010a 0104 fc04 fe16  ................
+00000870: 0910 0114 010e 010c 010c 010c 0104 0102  ................
+00000880: 0104 0102 0102 0104 0204 0102 fe04 fd04  ................
+00000890: fe16 0c7a 1441 646d 6f6e 6974 696f 6e73  ...z.Admonitions
+000008a0: 2e5f 5f69 6e69 745f 5f63 0200 0000 0000  .__init__c......
+000008b0: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
+000008c0: 0000 736c 0000 007c 006a 007c 006a 016b  ..sl...|.j.|.j.k
+000008d0: 0372 1f7c 006a 017c 005f 0074 026a 036a  .r.|.j.|._.t.j.j
+000008e0: 0464 0164 0164 028d 027c 006a 055f 0374  .d.d.d...|.j._.t
+000008f0: 02a0 0664 0374 026a 076a 08a1 027c 016a  ...d.t.j.j...|.j
+00000900: 095f 0a6e 1164 047c 005f 0074 02a0 0664  ._.n.d.|._.t...d
+00000910: 0574 026a 076a 08a1 027c 016a 095f 0a64  .t.j.j...|.j._.d
+00000920: 017c 006a 055f 037c 00a0 0ba1 0001 0064  .|.j._.|.......d
+00000930: 0053 0029 064e 7214 0000 0029 02da 0774  .S.).Nr....)...t
+00000940: 6f70 4c65 6674 da08 746f 7052 6967 6874  opLeft..topRight
+00000950: 6700 0000 0000 00e8 3f72 4600 0000 7201  g.......?rF...r.
+00000960: 0000 0029 0c72 3200 0000 7206 0000 0072  ...).r2...r....r
+00000970: 4900 0000 7233 0000 00da 046f 6e6c 7972  I...r3.....onlyr
+00000980: 5b00 0000 7259 0000 0072 3000 0000 7216  [...rY...r0...r.
+00000990: 0000 00da 0763 6f6e 7472 6f6c 722c 0000  .....controlr,..
+000009a0: 00da 0675 7064 6174 6529 0272 2600 0000  ...update).r&...
+000009b0: 7224 0000 0072 2700 0000 7227 0000 0072  r$...r'...r'...r
+000009c0: 2800 0000 7223 0000 006a 0000 0073 1000  (...r#...j...s..
+000009d0: 0000 0c01 0801 1401 1601 0602 1401 0801  ................
+000009e0: 0c02 7a1d 4164 6d6f 6e69 7469 6f6e 732e  ..z.Admonitions.
+000009f0: 7265 7369 7a65 5f61 646d 6f6e 6974 696f  resize_admonitio
+00000a00: 6e29 0ada 085f 5f6e 616d 655f 5fda 0a5f  n)...__name__.._
+00000a10: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00000a20: 6c6e 616d 655f 5fda 0373 7472 da03 696e  lname__..str..in
+00000a30: 74da 0462 6f6f 6cda 046c 6973 7472 6300  t..bool..listrc.
+00000a40: 0000 7223 0000 00da 0d5f 5f63 6c61 7373  ..r#.....__class
+00000a50: 6365 6c6c 5f5f 7227 0000 0072 2700 0000  cell__r'...r'...
+00000a60: 7269 0000 0072 2800 0000 7204 0000 0005  ri...r(...r.....
+00000a70: 0000 0073 1600 0000 0800 0201 0202 02fe  ...s............
+00000a80: 0203 02fd 0204 02fc 0205 0efb 1064 7204  .............dr.
+00000a90: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000aa0: 0000 0000 0600 0000 0000 0000 732a 0000  ............s*..
+00000ab0: 0065 005a 0164 005a 0264 0165 0364 0265  .e.Z.d.Z.d.e.d.e
+00000ac0: 0464 0365 0366 0687 0066 0164 0464 0584  .d.e.f...f.d.d..
+00000ad0: 0c5a 0587 0004 005a 0653 0029 06da 1046  .Z.....Z.S.)...F
+00000ae0: 6978 6564 4164 6d6f 6e69 7469 6f6e 7372  ixedAdmonitionsr
+00000af0: 0500 0000 7207 0000 00da 0574 6974 6c65  ....r......title
+00000b00: 6304 0000 0000 0000 0000 0000 000c 0000  c...............
+00000b10: 0012 0000 000f 0000 0073 9a01 0000 7c03  .........s....|.
+00000b20: 7c00 5f00 7401 a002 7c01 6900 a102 a002  |._.t...|.i.....
+00000b30: 6401 6402 a102 7d06 7401 a002 7c01 6900  d.d...}.t...|.i.
+00000b40: a102 a002 6403 6404 a102 7d07 7401 a002  ....d.d...}.t...
+00000b50: 7c01 6900 a102 a002 6405 6404 a102 7d08  |.i.....d.d...}.
+00000b60: 7403 a002 6406 6900 a102 7d09 7c09 a002  t...d.i...}.|...
+00000b70: 6407 a101 7d0a 7c09 a002 6408 a101 7d0b  d...}.|...d...}.
+00000b80: 7404 6a05 6409 7404 6a06 a007 640a 7c06  t.j.d.t.j...d.|.
+00000b90: a102 640b 640c 7404 6a08 7404 6a09 6a0a  ..d.d.t.j.t.j.j.
+00000ba0: 7404 6a08 640d 640c 7404 6a0b 7c08 7c07  t.j.d.d.t.j.|.|.
+00000bb0: 640e 640f 8d03 7404 6a0c 7c01 a00d a100  d.d...t.j.|.....
+00000bc0: 7c0b 7c0a 6410 6411 8d04 7404 6a0c 7c00  |.|.d.d...t.j.|.
+00000bd0: 6a00 6412 7c0a 6413 6411 8d04 6703 6414  j.d.|.d.d...g.d.
+00000be0: 8d03 6701 6415 8d02 6416 8d05 7c00 5f0e  ..g.d...d...|._.
+00000bf0: 7c05 a00f 6417 7404 6a10 6418 6419 7404  |...d.t.j.d.d.t.
+00000c00: 6a06 a007 641a 641b a102 7404 a011 641c  j...d.d...t...d.
+00000c10: 641c a102 641d 8d04 a102 0100 7c05 a00f  d...d.......|...
+00000c20: 641e 7404 6a12 a013 641f 7c07 a102 a102  d.t.j...d.|.....
+00000c30: 0100 7c05 a00f 6420 7404 6a14 6a15 a102  ..|...d t.j.j...
+00000c40: 0100 7c05 a00f 6421 7404 a016 6422 6423  ..|...d!t...d"d#
+00000c50: a102 a102 0100 7c05 a00f 6424 7c02 a102  ......|...d$|...
+00000c60: 0100 7c05 a00f 6425 640b a102 0100 7c05  ..|...d%d.....|.
+00000c70: a00f 6426 6427 a102 0100 7c05 a00f 6428  ..d&d'....|...d(
+00000c80: 6429 a102 0100 7c05 a00f 642a 7404 6a17  d)....|...d*t.j.
+00000c90: 642b 6429 7c00 6a0e 6701 642c 8d03 a102  d+d)|.j.g.d,....
+00000ca0: 0100 7418 8300 6a19 7c04 6900 7c05 a401  ..t...j.|.i.|...
+00000cb0: 8e01 0100 6400 5300 292d 4e72 0a00 0000  ....d.S.)-Nr....
+00000cc0: 720b 0000 0072 0c00 0000 720d 0000 0072  r....r....r....r
+00000cd0: 0e00 0000 720f 0000 0072 1000 0000 7211  ....r....r....r.
+00000ce0: 0000 0072 1200 0000 7213 0000 0072 1400  ...r....r....r..
+00000cf0: 0000 7215 0000 0072 1600 0000 7217 0000  ..r....r....r...
+00000d00: 0072 1800 0000 721b 0000 0072 1c00 0000  .r....r....r....
+00000d10: e90d 0000 00da 0477 3430 3072 1e00 0000  .......w400r....
+00000d20: 722f 0000 0072 3100 0000 7236 0000 0072  r/...r1...r6...r
+00000d30: 3700 0000 7221 0000 0072 3800 0000 7239  7...r!...r8...r9
+00000d40: 0000 0072 3a00 0000 723b 0000 0072 3f00  ...r:...r;...r?.
+00000d50: 0000 7240 0000 0072 4100 0000 7242 0000  ..r@...rA...rB..
+00000d60: 0072 4300 0000 7244 0000 0072 4500 0000  .rC...rD...rE...
+00000d70: 7233 0000 0072 3200 0000 7246 0000 0072  r3...r2...rF...r
+00000d80: 3400 0000 7201 0000 0072 3500 0000 7247  4...r....r5...rG
+00000d90: 0000 0072 4800 0000 291a 7279 0000 0072  ...rH...).ry...r
+00000da0: 0200 0000 724c 0000 0072 0300 0000 7249  ....rL...r....rI
+00000db0: 0000 0072 4d00 0000 724e 0000 0072 4f00  ...rM...rN...rO.
+00000dc0: 0000 7250 0000 0072 5100 0000 7252 0000  ..rP...rQ...rR..
+00000dd0: 0072 5300 0000 7254 0000 0072 5500 0000  .rS...rT...rU...
+00000de0: 725b 0000 0072 5c00 0000 725d 0000 0072  r[...r\...r]...r
+00000df0: 5e00 0000 723f 0000 0072 5f00 0000 7260  ^...r?...r_...r`
+00000e00: 0000 0072 6100 0000 725a 0000 0072 4a00  ...ra...rZ...rJ.
+00000e10: 0000 7262 0000 0072 6300 0000 290c 7226  ..rb...rc...).r&
+00000e20: 0000 0072 0500 0000 7207 0000 0072 7900  ...r....r....ry.
+00000e30: 0000 7264 0000 0072 6500 0000 720a 0000  ..rd...re...r...
+00000e40: 0072 0c00 0000 720e 0000 0072 6600 0000  .r....r....rf...
+00000e50: 7267 0000 0072 6800 0000 7269 0000 0072  rg...rh...ri...r
+00000e60: 2700 0000 7228 0000 0072 6300 0000 7800  '...r(...rc...x.
+00000e70: 0000 7386 0000 0006 0814 020c 0104 0104  ..s.............
+00000e80: ff14 030c 020a 010a 0104 0202 010c 0102  ................
+00000e90: 0102 0104 0106 0104 0202 0102 0104 0202  ................
+00000ea0: 0102 0102 0104 fd04 0506 0102 0102 0102  ................
+00000eb0: 0104 fc04 0604 0102 0102 0102 0104 fc02  ................
+00000ec0: f404 fd02 ff04 fe08 fb04 2402 0104 0102  ..........$.....
+00000ed0: 0102 010c 010a 0104 fc04 fe16 0910 0114  ................
+00000ee0: 010c 010c 010c 010c 0104 0102 0104 0102  ................
+00000ef0: 0102 0104 0202 ff04 fd04 fe16 0b7a 1946  .............z.F
+00000f00: 6978 6564 4164 6d6f 6e69 7469 6f6e 732e  ixedAdmonitions.
+00000f10: 5f5f 696e 6974 5f5f 2907 7270 0000 0072  __init__).rp...r
+00000f20: 7100 0000 7272 0000 0072 7300 0000 7275  q...rr...rs...ru
+00000f30: 0000 0072 6300 0000 7277 0000 0072 2700  ...rc...rw...r'.
+00000f40: 0000 7227 0000 0072 6900 0000 7228 0000  ..r'...ri...r(..
+00000f50: 0072 7800 0000 7700 0000 7310 0000 0008  .rx...w...s.....
+00000f60: 0002 0102 0202 fe02 0302 fd02 0416 fc72  ...............r
+00000f70: 7800 0000 2908 da04 666c 6574 7249 0000  x...)...fletrI..
+00000f80: 00da 0673 7479 6c65 7372 0200 0000 7203  ...stylesr....r.
+00000f90: 0000 0072 4d00 0000 7204 0000 0072 7800  ...rM...r....rx.
+00000fa0: 0000 7227 0000 0072 2700 0000 7227 0000  ..r'...r'...r'..
+00000fb0: 0072 2800 0000 da08 3c6d 6f64 756c 653e  .r(.....<module>
+00000fc0: 0100 0000 7308 0000 0008 0010 0112 0316  ....s...........
+00000fd0: 72                                       r
```

### Comparing `flet-material-0.1.0/flet_material/__pycache__/alert.cpython-310.pyc` & `flet-material-0.2.0/flet_material/__pycache__/alert.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flet-material-0.1.0/flet_material/__pycache__/annotation.cpython-310.pyc` & `flet-material-0.2.0/flet_material/__pycache__/annotation.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flet-material-0.1.0/flet_material/__pycache__/annotations.cpython-310.pyc` & `flet-material-0.2.0/flet_material/__pycache__/annotations.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flet-material-0.1.0/flet_material/__pycache__/badge.cpython-310.pyc` & `flet-material-0.2.0/flet_material/__pycache__/badge.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flet-material-0.1.0/flet_material/__pycache__/base.cpython-310.pyc` & `flet-material-0.2.0/flet_material/__pycache__/base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flet-material-0.1.0/flet_material/__pycache__/button.cpython-310.pyc` & `flet-material-0.2.0/flet_material/__pycache__/button.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 22 11:58:49 2023 UTC, .py size: 1383 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,99 +1,100 @@
-00000000: 6f0d 0d0a 0000 0000 f9cb 4364 6705 0000  o.........Cdg...
+00000000: 6f0d 0d0a 0000 0000 7274 4564 9105 0000  o.......rtEd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 0100 4700 6403 6404 8400 6404 6501 6a04  ..G.d.d...d.e.j.
 00000050: 6503 8304 5a05 6401 5300 2905 e900 0000  e...Z.d.S.).....
 00000060: 004e 2901 da05 5468 656d 6563 0000 0000  .N)...Themec....
 00000070: 0000 0000 0000 0000 0000 0000 0400 0000  ................
 00000080: 0000 0000 732a 0000 0065 005a 0164 005a  ....s*...e.Z.d.Z
 00000090: 0264 0165 0366 0287 0066 0164 0264 0384  .d.e.f...f.d.d..
 000000a0: 0c5a 0464 0464 0584 005a 0587 0004 005a  .Z.d.d...Z.....Z
 000000b0: 0653 0029 06da 0742 7574 746f 6e73 da05  .S.)...Buttons..
 000000c0: 7469 746c 6563 0400 0000 0000 0000 0000  titlec..........
-000000d0: 0000 0600 0000 0a00 0000 0f00 0000 73ea  ..............s.
-000000e0: 0000 0074 006a 017c 0364 0174 006a 02a0  ...t.j.|.d.t.j..
-000000f0: 0364 0274 046a 05a1 0264 038d 0388 005f  .d.t.j...d....._
-00000100: 067c 05a0 0764 047c 01a1 0201 007c 05a0  .|...d.|.....|..
-00000110: 0764 057c 02a1 0201 007c 05a0 0764 0664  .d.|.....|...d.d
-00000120: 07a1 0201 007c 05a0 0764 0864 09a1 0201  .....|...d.d....
-00000130: 007c 05a0 0764 0a74 00a0 0864 0ba1 01a1  .|...d.t...d....
-00000140: 0201 007c 05a0 0764 0c74 006a 09a0 0a64  ...|...d.t.j...d
-00000150: 0d74 006a 02a0 0364 0274 046a 05a1 02a1  .t.j...d.t.j....
-00000160: 02a1 0201 007c 05a0 0764 0e64 0fa1 0201  .....|...d.d....
-00000170: 007c 05a0 0764 1087 0066 0164 1164 1284  .|...d...f.d.d..
-00000180: 08a1 0201 007c 05a0 0764 1374 006a 0b6a  .....|...d.t.j.j
-00000190: 0ca1 0201 007c 05a0 0764 1474 00a0 0d64  .....|...d.t...d
-000001a0: 1564 16a1 02a1 0201 007c 05a0 0764 1788  .d.......|...d..
-000001b0: 006a 06a1 0201 0074 0e83 006a 0f7c 0469  .j.....t...j.|.i
-000001c0: 007c 05a4 018e 0101 0064 0053 0029 184e  .|.......d.S.).N
-000001d0: da04 626f 6c64 e733 3333 3333 33eb 3f29  ..bold.333333.?)
-000001e0: 02da 0677 6569 6768 74da 0563 6f6c 6f72  ...weight..color
-000001f0: da05 7769 6474 68da 0668 6569 6768 74da  ..width..height.
-00000200: 0369 6e6b 54da 0762 6763 6f6c 6f72 fa07  .inkT..bgcolor..
-00000210: 2332 6532 6633 65da 0573 6861 7065 da09  #2e2f3e..shape..
-00000220: 7265 6374 616e 676c 65da 0662 6f72 6465  rectangle..borde
-00000230: 72e9 0200 0000 da0d 626f 7264 6572 5f72  r.......border_r
-00000240: 6164 6975 73e9 0400 0000 da08 6f6e 5f68  adius.......on_h
-00000250: 6f76 6572 6301 0000 0000 0000 0000 0000  overc...........
-00000260: 0001 0000 0003 0000 0013 0000 0073 0a00  .............s..
-00000270: 0000 8800 a000 7c00 a101 5300 2901 4e29  ......|...S.).N)
-00000280: 01da 0e61 6e69 6d61 7465 5f62 7574 746f  ...animate_butto
-00000290: 6e29 01da 0165 a901 da04 7365 6c66 a900  n)...e....self..
-000002a0: fa43 2f55 7365 7273 2f61 686d 6164 2f43  .C/Users/ahmad/C
-000002b0: 6f64 6573 7061 6365 2f50 7974 686f 6e2f  odespace/Python/
-000002c0: 666c 6574 2d6d 6174 6572 6961 6c2f 666c  flet-material/fl
-000002d0: 6574 5f6d 6174 6572 6961 6c2f 6275 7474  et_material/butt
-000002e0: 6f6e 2e70 79da 083c 6c61 6d62 6461 3e18  on.py..<lambda>.
-000002f0: 0000 0073 0200 0000 0a00 7a22 4275 7474  ...s......z"Butt
-00000300: 6f6e 732e 5f5f 696e 6974 5f5f 2e3c 6c6f  ons.__init__.<lo
-00000310: 6361 6c73 3e2e 3c6c 616d 6264 613e da09  cals>.<lambda>..
-00000320: 616c 6967 6e6d 656e 74da 0761 6e69 6d61  alignment..anima
-00000330: 7465 69f4 0100 00da 0465 6173 65da 0763  tei......ease..c
-00000340: 6f6e 7465 6e74 2910 da02 6674 da04 5465  ontent)...ft..Te
-00000350: 7874 da06 636f 6c6f 7273 da0c 7769 7468  xt..colors..with
-00000360: 5f6f 7061 6369 7479 7202 0000 00da 0d70  _opacityr......p
-00000370: 7269 6d61 7279 5f74 6865 6d65 da04 7465  rimary_theme..te
-00000380: 7874 da0a 7365 7464 6566 6175 6c74 da08  xt..setdefault..
-00000390: 426f 7853 6861 7065 7210 0000 00da 0361  BoxShaper......a
-000003a0: 6c6c 721c 0000 00da 0663 656e 7465 72da  llr......center.
-000003b0: 0941 6e69 6d61 7469 6f6e da05 7375 7065  .Animation..supe
-000003c0: 72da 085f 5f69 6e69 745f 5f29 0672 1800  r..__init__).r..
-000003d0: 0000 7209 0000 0072 0a00 0000 7204 0000  ..r....r....r...
-000003e0: 00da 0461 7267 73da 066b 7761 7267 73a9  ...args..kwargs.
-000003f0: 01da 095f 5f63 6c61 7373 5f5f 7217 0000  ...__class__r...
-00000400: 0072 1a00 0000 722c 0000 0006 0000 0073  .r....r,.......s
-00000410: 2800 0000 0402 0201 0201 0e01 08fd 0c06  (...............
-00000420: 0c01 0c01 0c01 1201 0401 0201 1801 04fe  ................
-00000430: 0c04 1401 1001 1401 0e01 1602 7a10 4275  ............z.Bu
-00000440: 7474 6f6e 732e 5f5f 696e 6974 5f5f 6302  ttons.__init__c.
-00000450: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00000460: 0000 0043 0000 0073 4c00 0000 7c00 6a00  ...C...sL...|.j.
-00000470: 6401 6b02 7213 7401 6a02 7c00 5f00 7403  d.k.r.t.j.|._.t.
-00000480: 6a04 a005 6402 6403 a102 7c00 6a06 5f07  j...d.d...|.j._.
-00000490: 6e0d 6401 7c00 5f00 7403 6a04 a005 6404  n.d.|._.t.j...d.
-000004a0: 7401 6a02 a102 7c00 6a06 5f07 7c00 a008  t.j...|.j._.|...
-000004b0: a100 0100 6400 5300 2905 4e72 0d00 0000  ....d.S.).Nr....
-000004c0: 6766 6666 6666 66ee 3fda 0577 6869 7465  gffffff.?..white
-000004d0: 7206 0000 0029 0972 0c00 0000 7202 0000  r....).r....r...
-000004e0: 0072 2400 0000 7220 0000 0072 2200 0000  .r$...r ...r"...
-000004f0: 7223 0000 0072 2500 0000 7208 0000 00da  r#...r%...r.....
-00000500: 0675 7064 6174 6529 0272 1800 0000 7216  .update).r....r.
-00000510: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
-00000520: 0000 7215 0000 001f 0000 0073 0c00 0000  ..r........s....
-00000530: 0a01 0801 1401 0602 1401 0c02 7a16 4275  ............z.Bu
-00000540: 7474 6f6e 732e 616e 696d 6174 655f 6275  ttons.animate_bu
-00000550: 7474 6f6e 2907 da08 5f5f 6e61 6d65 5f5f  tton)...__name__
-00000560: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00000570: 7175 616c 6e61 6d65 5f5f da03 7374 7272  qualname__..strr
-00000580: 2c00 0000 7215 0000 00da 0d5f 5f63 6c61  ,...r......__cla
-00000590: 7373 6365 6c6c 5f5f 7219 0000 0072 1900  sscell__r....r..
-000005a0: 0000 722f 0000 0072 1a00 0000 7203 0000  ..r/...r....r...
-000005b0: 0005 0000 0073 0600 0000 0800 1201 1019  .....s..........
-000005c0: 7203 0000 0029 06da 0466 6c65 7472 2000  r....)...fletr .
-000005d0: 0000 da12 666c 6574 5f6d 6174 6572 6961  ....flet_materia
-000005e0: 6c2e 6261 7365 7202 0000 00da 0943 6f6e  l.baser......Con
-000005f0: 7461 696e 6572 7203 0000 0072 1900 0000  tainerr....r....
-00000600: 7219 0000 0072 1900 0000 721a 0000 00da  r....r....r.....
-00000610: 083c 6d6f 6475 6c65 3e01 0000 0073 0600  .<module>....s..
-00000620: 0000 0800 0c01 1803                      ........
+000000d0: 0000 0600 0000 0a00 0000 0f00 0000 73f2  ..............s.
+000000e0: 0000 007c 0388 005f 0074 016a 0288 006a  ...|..._.t.j...j
+000000f0: 0064 0174 016a 03a0 0464 0274 056a 06a1  .d.t.j...d.t.j..
+00000100: 0264 038d 0388 005f 077c 05a0 0864 047c  .d....._.|...d.|
+00000110: 01a1 0201 007c 05a0 0864 057c 02a1 0201  .....|...d.|....
+00000120: 007c 05a0 0864 0664 07a1 0201 007c 05a0  .|...d.d.....|..
+00000130: 0864 0864 09a1 0201 007c 05a0 0864 0a74  .d.d.....|...d.t
+00000140: 01a0 0964 0ba1 01a1 0201 007c 05a0 0864  ...d.......|...d
+00000150: 0c74 016a 0aa0 0b64 0d74 016a 03a0 0464  .t.j...d.t.j...d
+00000160: 0274 056a 06a1 02a1 02a1 0201 007c 05a0  .t.j.........|..
+00000170: 0864 0e64 0fa1 0201 007c 05a0 0864 1087  .d.d.....|...d..
+00000180: 0066 0164 1164 1284 08a1 0201 007c 05a0  .f.d.d.......|..
+00000190: 0864 1374 016a 0c6a 0da1 0201 007c 05a0  .d.t.j.j.....|..
+000001a0: 0864 1474 01a0 0e64 1564 16a1 02a1 0201  .d.t...d.d......
+000001b0: 007c 05a0 0864 1788 006a 07a1 0201 0074  .|...d...j.....t
+000001c0: 0f83 006a 107c 0469 007c 05a4 018e 0101  ...j.|.i.|......
+000001d0: 0064 0053 0029 184e da04 626f 6c64 e733  .d.S.).N..bold.3
+000001e0: 3333 3333 33eb 3f29 02da 0677 6569 6768  33333.?)...weigh
+000001f0: 74da 0563 6f6c 6f72 da05 7769 6474 68da  t..color..width.
+00000200: 0668 6569 6768 74da 0369 6e6b 54da 0762  .height..inkT..b
+00000210: 6763 6f6c 6f72 fa07 2332 6532 6633 65da  gcolor..#2e2f3e.
+00000220: 0573 6861 7065 da09 7265 6374 616e 676c  .shape..rectangl
+00000230: 65da 0662 6f72 6465 72e9 0200 0000 da0d  e..border.......
+00000240: 626f 7264 6572 5f72 6164 6975 73e9 0400  border_radius...
+00000250: 0000 da08 6f6e 5f68 6f76 6572 6301 0000  ....on_hoverc...
+00000260: 0000 0000 0000 0000 0001 0000 0003 0000  ................
+00000270: 0013 0000 0073 0a00 0000 8800 a000 7c00  .....s........|.
+00000280: a101 5300 2901 4e29 01da 0e61 6e69 6d61  ..S.).N)...anima
+00000290: 7465 5f62 7574 746f 6e29 01da 0165 a901  te_button)...e..
+000002a0: da04 7365 6c66 a900 fa49 2f55 7365 7273  ..self...I/Users
+000002b0: 2f61 686d 6164 2f43 6f64 6573 7061 6365  /ahmad/Codespace
+000002c0: 2f50 7974 686f 6e2f 666c 6574 2d6d 6174  /Python/flet-mat
+000002d0: 6572 6961 6c2d 6475 6d6d 792f 666c 6574  erial-dummy/flet
+000002e0: 5f6d 6174 6572 6961 6c2f 6275 7474 6f6e  _material/button
+000002f0: 2e70 79da 083c 6c61 6d62 6461 3e1a 0000  .py..<lambda>...
+00000300: 0073 0200 0000 0a00 7a22 4275 7474 6f6e  .s......z"Button
+00000310: 732e 5f5f 696e 6974 5f5f 2e3c 6c6f 6361  s.__init__.<loca
+00000320: 6c73 3e2e 3c6c 616d 6264 613e da09 616c  ls>.<lambda>..al
+00000330: 6967 6e6d 656e 74da 0761 6e69 6d61 7465  ignment..animate
+00000340: 69f4 0100 00da 0465 6173 65da 0763 6f6e  i......ease..con
+00000350: 7465 6e74 2911 7204 0000 00da 0266 74da  tent).r......ft.
+00000360: 0454 6578 74da 0663 6f6c 6f72 73da 0c77  .Text..colors..w
+00000370: 6974 685f 6f70 6163 6974 7972 0200 0000  ith_opacityr....
+00000380: da0d 7072 696d 6172 795f 7468 656d 65da  ..primary_theme.
+00000390: 0474 6578 74da 0a73 6574 6465 6661 756c  .text..setdefaul
+000003a0: 74da 0842 6f78 5368 6170 6572 1000 0000  t..BoxShaper....
+000003b0: da03 616c 6c72 1c00 0000 da06 6365 6e74  ..allr......cent
+000003c0: 6572 da09 416e 696d 6174 696f 6eda 0573  er..Animation..s
+000003d0: 7570 6572 da08 5f5f 696e 6974 5f5f 2906  uper..__init__).
+000003e0: 7218 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
+000003f0: 0400 0000 da04 6172 6773 da06 6b77 6172  ......args..kwar
+00000400: 6773 a901 da09 5f5f 636c 6173 735f 5f72  gs....__class__r
+00000410: 1700 0000 721a 0000 0072 2c00 0000 0600  ....r....r,.....
+00000420: 0000 732a 0000 0006 0204 0204 0102 010e  ..s*............
+00000430: 0108 fd0c 060c 010c 010c 0112 0104 0102  ................
+00000440: 0118 0104 fe0c 0414 0110 0114 010e 0116  ................
+00000450: 027a 1042 7574 746f 6e73 2e5f 5f69 6e69  .z.Buttons.__ini
+00000460: 745f 5f63 0200 0000 0000 0000 0000 0000  t__c............
+00000470: 0200 0000 0400 0000 4300 0000 734c 0000  ........C...sL..
+00000480: 007c 006a 0064 016b 0272 1374 016a 027c  .|.j.d.k.r.t.j.|
+00000490: 005f 0074 036a 04a0 0564 0264 03a1 027c  ._.t.j...d.d...|
+000004a0: 006a 065f 076e 0d64 017c 005f 0074 036a  .j._.n.d.|._.t.j
+000004b0: 04a0 0564 0474 016a 02a1 027c 006a 065f  ...d.t.j...|.j._
+000004c0: 077c 00a0 08a1 0001 0064 0053 0029 054e  .|.......d.S.).N
+000004d0: 720d 0000 0067 6666 6666 6666 ee3f da05  r....gffffff.?..
+000004e0: 7768 6974 6572 0600 0000 2909 720c 0000  whiter....).r...
+000004f0: 0072 0200 0000 7224 0000 0072 2000 0000  .r....r$...r ...
+00000500: 7222 0000 0072 2300 0000 7225 0000 0072  r"...r#...r%...r
+00000510: 0800 0000 da06 7570 6461 7465 2902 7218  ......update).r.
+00000520: 0000 0072 1600 0000 7219 0000 0072 1900  ...r....r....r..
+00000530: 0000 721a 0000 0072 1500 0000 2100 0000  ..r....r....!...
+00000540: 730c 0000 000a 0108 0114 0106 0214 010c  s...............
+00000550: 027a 1642 7574 746f 6e73 2e61 6e69 6d61  .z.Buttons.anima
+00000560: 7465 5f62 7574 746f 6e29 07da 085f 5f6e  te_button)...__n
+00000570: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
+00000580: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
+00000590: 0373 7472 722c 0000 0072 1500 0000 da0d  .strr,...r......
+000005a0: 5f5f 636c 6173 7363 656c 6c5f 5f72 1900  __classcell__r..
+000005b0: 0000 7219 0000 0072 2f00 0000 721a 0000  ..r....r/...r...
+000005c0: 0072 0300 0000 0500 0000 7306 0000 0008  .r........s.....
+000005d0: 0012 0110 1b72 0300 0000 2906 da04 666c  .....r....)...fl
+000005e0: 6574 7220 0000 00da 1266 6c65 745f 6d61  etr .....flet_ma
+000005f0: 7465 7269 616c 2e62 6173 6572 0200 0000  terial.baser....
+00000600: da09 436f 6e74 6169 6e65 7272 0300 0000  ..Containerr....
+00000610: 7219 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
+00000620: 1a00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00000630: 0000 7306 0000 0008 000c 0118 03         ..s..........
```

### Comparing `flet-material-0.1.0/flet_material/__pycache__/checkbox.cpython-310.pyc` & `flet-material-0.2.0/flet_material/__pycache__/checkbox.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flet-material-0.1.0/flet_material/__pycache__/chip.cpython-310.pyc` & `flet-material-0.2.0/flet_material/__pycache__/chip.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 23 11:27:26 2023 UTC, .py size: 1405 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 21% similar despite different names*

```diff
@@ -1,103 +1,107 @@
-00000000: 6f0d 0d0a 0000 0000 1e16 4564 7d05 0000  o.........Ed}...
+00000000: 6f0d 0d0a 0000 0000 5b68 4664 f805 0000  o.......[hFd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 0100 4700 6403 6404 8400 6404 6501 6a04  ..G.d.d...d.e.j.
 00000050: 6503 8304 5a05 6401 5300 2905 e900 0000  e...Z.d.S.).....
 00000060: 004e 2901 da05 5468 656d 6563 0000 0000  .N)...Themec....
 00000070: 0000 0000 0000 0000 0000 0000 0400 0000  ................
-00000080: 0000 0000 732a 0000 0065 005a 0164 005a  ....s*...e.Z.d.Z
-00000090: 0264 0165 0366 0287 0066 0164 0264 0384  .d.e.f...f.d.d..
-000000a0: 0c5a 0464 0464 0584 005a 0587 0004 005a  .Z.d.d...Z.....Z
-000000b0: 0653 0029 06da 0a46 696c 7465 7243 6869  .S.)...FilterChi
-000000c0: 70da 0574 6974 6c65 6302 0000 0000 0000  p..titlec.......
-000000d0: 0000 0000 0004 0000 000e 0000 000f 0000  ................
-000000e0: 0073 e600 0000 7400 6a01 6401 6401 7400  .s....t.j.d.d.t.
-000000f0: a002 6402 a101 6403 6404 6405 6406 6407  ..d...d.d.d.d.d.
-00000100: 8d07 0400 8800 5f03 7400 5f04 7c03 a005  ......_.t._.|...
-00000110: 6408 6403 a102 0100 7c03 a005 6409 6406  d.d.....|...d.d.
-00000120: a102 0100 7c03 a005 640a 7400 6a06 a007  ....|...d.t.j...
-00000130: 640b 7408 6a09 a102 a102 0100 7c03 a005  d.t.j.......|...
-00000140: 640c 640d a102 0100 7c03 a005 640e 6405  d.d.....|...d.d.
-00000150: a102 0100 7c03 a005 640f 6410 a102 0100  ....|...d.d.....
-00000160: 7c03 a005 6411 7400 6a0a 6a0b a102 0100  |...d.t.j.j.....
-00000170: 7c03 a005 6412 8700 6601 6413 6414 8408  |...d...f.d.d...
-00000180: a102 0100 7c03 a005 6415 7400 6a0c 6406  ....|...d.t.j.d.
-00000190: 6416 7400 6a0d 6a0e 6417 8800 6a03 7400  d.t.j.j.d...j.t.
-000001a0: 6a0f 7c01 6418 6419 641a 8d03 6702 641b  j.|.d.d.d...g.d.
-000001b0: 8d05 a102 0100 7410 8300 6a11 7c02 6900  ......t...j.|.i.
-000001c0: 7c03 a401 8e01 0100 6400 5300 291c 4ee9  |.......d.S.).N.
-000001d0: 0200 0000 6766 6666 6666 66e6 3f7a 0723  ....gffffff.?z.#
-000001e0: 3265 3266 3365 da05 7768 6974 6554 4629  2e2f3e..whiteTF)
-000001f0: 07da 0577 6964 7468 da06 6865 6967 6874  ...width..height
-00000200: da05 7363 616c 65da 0a66 696c 6c5f 636f  ..scale..fill_co
-00000210: 6c6f 72da 0b63 6865 636b 5f63 6f6c 6f72  lor..check_color
-00000220: da08 6469 7361 626c 6564 da05 7661 6c75  ..disabled..valu
-00000230: 65da 0762 6763 6f6c 6f72 da06 6578 7061  e..bgcolor..expa
-00000240: 6e64 da06 626f 7264 6572 e901 0000 00da  nd..border......
-00000250: 0770 6164 6469 6e67 e908 0000 00da 0369  .padding.......i
-00000260: 6e6b da0d 626f 7264 6572 5f72 6164 6975  nk..border_radiu
-00000270: 73e9 0600 0000 da09 616c 6967 6e6d 656e  s.......alignmen
-00000280: 74da 086f 6e5f 636c 6963 6b63 0100 0000  t..on_clickc....
-00000290: 0000 0000 0000 0000 0100 0000 0300 0000  ................
-000002a0: 1300 0000 730a 0000 0088 00a0 007c 00a1  ....s........|..
-000002b0: 0153 0029 014e 2901 da12 746f 6767 6c65  .S.).N)...toggle
-000002c0: 5f66 696c 7465 725f 6368 6970 2901 da01  _filter_chip)...
-000002d0: 65a9 01da 0473 656c 66a9 00fa 472f 5573  e....self...G/Us
-000002e0: 6572 732f 6168 6d61 642f 436f 6465 7370  ers/ahmad/Codesp
-000002f0: 6163 652f 5079 7468 6f6e 2f66 6c65 742d  ace/Python/flet-
-00000300: 6d61 7465 7269 616c 2d64 756d 6d79 2f66  material-dummy/f
-00000310: 6c65 745f 6d61 7465 7269 616c 2f63 6869  let_material/chi
-00000320: 702e 7079 da08 3c6c 616d 6264 613e 1900  p.py..<lambda>..
-00000330: 0000 7302 0000 000a 007a 2546 696c 7465  ..s......z%Filte
-00000340: 7243 6869 702e 5f5f 696e 6974 5f5f 2e3c  rChip.__init__.<
-00000350: 6c6f 6361 6c73 3e2e 3c6c 616d 6264 613e  locals>.<lambda>
-00000360: da07 636f 6e74 656e 7472 0100 0000 da06  ..contentr......
-00000370: 6365 6e74 6572 e90b 0000 00da 0462 6f6c  center.......bol
-00000380: 6429 02da 0473 697a 65da 0677 6569 6768  d)...size..weigh
-00000390: 7429 0572 0f00 0000 da07 7370 6163 696e  t).r......spacin
-000003a0: 6772 1700 0000 da12 7665 7274 6963 616c  gr......vertical
-000003b0: 5f61 6c69 676e 6d65 6e74 da08 636f 6e74  _alignment..cont
-000003c0: 726f 6c73 2912 da02 6674 da08 4368 6563  rols)...ft..Chec
-000003d0: 6b62 6f78 da05 5363 616c 65da 0474 6963  kbox..Scale..tic
-000003e0: 6bda 0743 6f6e 7472 6f6c da0a 7365 7464  k..Control..setd
-000003f0: 6566 6175 6c74 7210 0000 00da 0361 6c6c  efaultr......all
-00000400: 7202 0000 00da 0d70 7269 6d61 7279 5f74  r......primary_t
-00000410: 6865 6d65 7217 0000 0072 2100 0000 da03  hemer....r!.....
-00000420: 526f 77da 114d 6169 6e41 7869 7341 6c69  Row..MainAxisAli
-00000430: 676e 6d65 6e74 da0c 5350 4143 455f 4152  gnment..SPACE_AR
-00000440: 4f55 4e44 da04 5465 7874 da05 7375 7065  OUND..Text..supe
-00000450: 72da 085f 5f69 6e69 745f 5f29 0472 1c00  r..__init__).r..
-00000460: 0000 7204 0000 00da 0461 7267 73da 066b  ..r......args..k
-00000470: 7761 7267 73a9 01da 095f 5f63 6c61 7373  wargs....__class
-00000480: 5f5f 721b 0000 0072 1e00 0000 7236 0000  __r....r....r6..
-00000490: 0006 0000 0073 3800 0000 0402 0201 0201  .....s8.........
-000004a0: 0801 0201 0201 0201 0201 0ef9 0c0a 0c01  ................
-000004b0: 1801 0c01 0c01 0c01 1001 1401 0401 0201  ................
-000004c0: 0401 0201 0201 0601 0201 1401 04fb 04fe  ................
-000004d0: 160b 7a13 4669 6c74 6572 4368 6970 2e5f  ..z.FilterChip._
-000004e0: 5f69 6e69 745f 5f63 0200 0000 0000 0000  _init__c........
-000004f0: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
-00000500: 732c 0000 007c 006a 006a 0164 016b 0272  s,...|.j.j.d.k.r
-00000510: 0b64 027c 006a 005f 016e 0464 017c 006a  .d.|.j._.n.d.|.j
-00000520: 005f 017c 006a 00a0 02a1 0001 0064 0053  ._.|.j.......d.S
-00000530: 0029 034e 4654 2903 722c 0000 0072 0d00  .).NFT).r,...r..
-00000540: 0000 da06 7570 6461 7465 2902 721c 0000  ....update).r...
-00000550: 0072 1a00 0000 721d 0000 0072 1d00 0000  .r....r....r....
-00000560: 721e 0000 0072 1900 0000 2700 0000 7308  r....r....'...s.
-00000570: 0000 000c 010a 0108 020e 027a 1d46 696c  ...........z.Fil
-00000580: 7465 7243 6869 702e 746f 6767 6c65 5f66  terChip.toggle_f
-00000590: 696c 7465 725f 6368 6970 2907 da08 5f5f  ilter_chip)...__
-000005a0: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-000005b0: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-000005c0: da03 7374 7272 3600 0000 7219 0000 00da  ..strr6...r.....
-000005d0: 0d5f 5f63 6c61 7373 6365 6c6c 5f5f 721d  .__classcell__r.
-000005e0: 0000 0072 1d00 0000 7239 0000 0072 1e00  ...r....r9...r..
-000005f0: 0000 7203 0000 0005 0000 0073 0600 0000  ..r........s....
-00000600: 0800 1201 1021 7203 0000 0029 06da 0466  .....!r....)...f
-00000610: 6c65 7472 2900 0000 da12 666c 6574 5f6d  letr).....flet_m
-00000620: 6174 6572 6961 6c2e 6261 7365 7202 0000  aterial.baser...
-00000630: 00da 0943 6f6e 7461 696e 6572 7203 0000  ...Containerr...
-00000640: 0072 1d00 0000 721d 0000 0072 1d00 0000  .r....r....r....
-00000650: 721e 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-00000660: 0000 0073 0600 0000 0800 0c01 1803       ...s..........
+00000080: 0000 0000 732e 0000 0065 005a 0164 005a  ....s....e.Z.d.Z
+00000090: 0264 0165 0364 0265 0466 0487 0066 0164  .d.e.d.e.f...f.d
+000000a0: 0364 0484 0c5a 0564 0564 0684 005a 0687  .d...Z.d.d...Z..
+000000b0: 0004 005a 0753 0029 07da 0a46 696c 7465  ...Z.S.)...Filte
+000000c0: 7243 6869 70da 0574 6974 6c65 da0a 6368  rChip..title..ch
+000000d0: 6970 5f77 6964 7468 6303 0000 0000 0000  ip_widthc.......
+000000e0: 0000 0000 0005 0000 000d 0000 000f 0000  ................
+000000f0: 0073 f400 0000 7c01 8800 5f00 7c02 8800  .s....|..._.|...
+00000100: 5f01 7402 6a03 6401 6401 7402 a004 6402  _.t.j.d.d.t...d.
+00000110: a101 6403 6404 6405 6406 6407 8d07 0400  ..d.d.d.d.d.....
+00000120: 8800 5f05 7402 5f06 7c04 a007 6408 8800  .._.t._.|...d...
+00000130: 6a01 a102 0100 7c04 a007 6409 6403 a102  j.....|...d.d...
+00000140: 0100 7c04 a007 640a 7402 6a08 a009 640b  ..|...d.t.j...d.
+00000150: 740a 6a0b a102 a102 0100 7c04 a007 640c  t.j.......|...d.
+00000160: 640d a102 0100 7c04 a007 640e 6405 a102  d.....|...d.d...
+00000170: 0100 7c04 a007 640f 6410 a102 0100 7c04  ..|...d.d.....|.
+00000180: a007 6411 7402 6a0c 6a0d a102 0100 7c04  ..d.t.j.j.....|.
+00000190: a007 6412 8700 6601 6413 6414 8408 a102  ..d...f.d.d.....
+000001a0: 0100 7c04 a007 6415 7402 6a0e 6416 7402  ..|...d.t.j.d.t.
+000001b0: 6a0f 6a10 6417 8800 6a05 7402 6a11 8800  j.j.d...j.t.j...
+000001c0: 6a00 6418 6419 641a 8d03 6702 641b 8d04  j.d.d.d...g.d...
+000001d0: a102 0100 7412 8300 6a13 7c03 6900 7c04  ....t...j.|.i.|.
+000001e0: a401 8e01 0100 6400 5300 291c 4ee9 0200  ......d.S.).N...
+000001f0: 0000 6766 6666 6666 66e6 3f7a 0723 3265  ..gffffff.?z.#2e
+00000200: 3266 3365 da05 7768 6974 6554 4629 07da  2f3e..whiteTF)..
+00000210: 0577 6964 7468 da06 6865 6967 6874 da05  .width..height..
+00000220: 7363 616c 65da 0a66 696c 6c5f 636f 6c6f  scale..fill_colo
+00000230: 72da 0b63 6865 636b 5f63 6f6c 6f72 da08  r..check_color..
+00000240: 6469 7361 626c 6564 da05 7661 6c75 6572  disabled..valuer
+00000250: 0800 0000 da07 6267 636f 6c6f 72da 0662  ......bgcolor..b
+00000260: 6f72 6465 72e9 0100 0000 da07 7061 6464  order.......padd
+00000270: 696e 67e9 0800 0000 da03 696e 6bda 0d62  ing.......ink..b
+00000280: 6f72 6465 725f 7261 6469 7573 e906 0000  order_radius....
+00000290: 00da 0961 6c69 676e 6d65 6e74 da08 6f6e  ...alignment..on
+000002a0: 5f63 6c69 636b 6301 0000 0000 0000 0000  _clickc.........
+000002b0: 0000 0001 0000 0003 0000 0013 0000 0073  ...............s
+000002c0: 0a00 0000 8800 a000 7c00 a101 5300 2901  ........|...S.).
+000002d0: 4e29 01da 1274 6f67 676c 655f 6669 6c74  N)...toggle_filt
+000002e0: 6572 5f63 6869 7029 01da 0165 a901 da04  er_chip)...e....
+000002f0: 7365 6c66 a900 fa47 2f55 7365 7273 2f61  self...G/Users/a
+00000300: 686d 6164 2f43 6f64 6573 7061 6365 2f50  hmad/Codespace/P
+00000310: 7974 686f 6e2f 666c 6574 2d6d 6174 6572  ython/flet-mater
+00000320: 6961 6c2d 6475 6d6d 792f 666c 6574 5f6d  ial-dummy/flet_m
+00000330: 6174 6572 6961 6c2f 6368 6970 2e70 79da  aterial/chip.py.
+00000340: 083c 6c61 6d62 6461 3e23 0000 0073 0200  .<lambda>#...s..
+00000350: 0000 0a00 7a25 4669 6c74 6572 4368 6970  ....z%FilterChip
+00000360: 2e5f 5f69 6e69 745f 5f2e 3c6c 6f63 616c  .__init__.<local
+00000370: 733e 2e3c 6c61 6d62 6461 3eda 0763 6f6e  s>.<lambda>..con
+00000380: 7465 6e74 7201 0000 00da 0663 656e 7465  tentr......cente
+00000390: 72e9 0b00 0000 da04 626f 6c64 2902 da04  r.......bold)...
+000003a0: 7369 7a65 da06 7765 6967 6874 2904 da07  size..weight)...
+000003b0: 7370 6163 696e 6772 1700 0000 da12 7665  spacingr......ve
+000003c0: 7274 6963 616c 5f61 6c69 676e 6d65 6e74  rtical_alignment
+000003d0: da08 636f 6e74 726f 6c73 2914 7204 0000  ..controls).r...
+000003e0: 0072 0500 0000 da02 6674 da08 4368 6563  .r......ft..Chec
+000003f0: 6b62 6f78 da05 5363 616c 65da 0474 6963  kbox..Scale..tic
+00000400: 6bda 0743 6f6e 7472 6f6c da0a 7365 7464  k..Control..setd
+00000410: 6566 6175 6c74 7210 0000 00da 0361 6c6c  efaultr......all
+00000420: 7202 0000 00da 0d70 7269 6d61 7279 5f74  r......primary_t
+00000430: 6865 6d65 7217 0000 0072 2100 0000 da03  hemer....r!.....
+00000440: 526f 77da 114d 6169 6e41 7869 7341 6c69  Row..MainAxisAli
+00000450: 676e 6d65 6e74 da0c 5350 4143 455f 4152  gnment..SPACE_AR
+00000460: 4f55 4e44 da04 5465 7874 da05 7375 7065  OUND..Text..supe
+00000470: 72da 085f 5f69 6e69 745f 5f29 0572 1c00  r..__init__).r..
+00000480: 0000 7204 0000 0072 0500 0000 da04 6172  ..r....r......ar
+00000490: 6773 da06 6b77 6172 6773 a901 da09 5f5f  gs..kwargs....__
+000004a0: 636c 6173 735f 5f72 1b00 0000 721e 0000  class__r....r...
+000004b0: 0072 3600 0000 0600 0000 733a 0000 0006  .r6.......s:....
+000004c0: 0806 0104 0302 0102 0108 0102 0102 0102  ................
+000004d0: 0102 010e f90e 0a0c 0118 010c 010c 010c  ................
+000004e0: 0110 0114 0104 0102 0104 0102 0106 0102  ................
+000004f0: 0116 0104 fc04 fe16 0a7a 1346 696c 7465  .........z.Filte
+00000500: 7243 6869 702e 5f5f 696e 6974 5f5f 6302  rChip.__init__c.
+00000510: 0000 0000 0000 0000 0000 0002 0000 0002  ................
+00000520: 0000 0043 0000 0073 2c00 0000 7c00 6a00  ...C...s,...|.j.
+00000530: 6a01 6401 6b02 720b 6402 7c00 6a00 5f01  j.d.k.r.d.|.j._.
+00000540: 6e04 6401 7c00 6a00 5f01 7c00 6a00 a002  n.d.|.j._.|.j...
+00000550: a100 0100 6400 5300 2903 4e46 5429 0372  ....d.S.).NFT).r
+00000560: 2c00 0000 720e 0000 00da 0675 7064 6174  ,...r......updat
+00000570: 6529 0272 1c00 0000 721a 0000 0072 1d00  e).r....r....r..
+00000580: 0000 721d 0000 0072 1e00 0000 7219 0000  ..r....r....r...
+00000590: 0030 0000 0073 0800 0000 0c01 0a01 0802  .0...s..........
+000005a0: 0e02 7a1d 4669 6c74 6572 4368 6970 2e74  ..z.FilterChip.t
+000005b0: 6f67 676c 655f 6669 6c74 6572 5f63 6869  oggle_filter_chi
+000005c0: 7029 08da 085f 5f6e 616d 655f 5fda 0a5f  p)...__name__.._
+000005d0: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+000005e0: 6c6e 616d 655f 5fda 0373 7472 da03 696e  lname__..str..in
+000005f0: 7472 3600 0000 7219 0000 00da 0d5f 5f63  tr6...r......__c
+00000600: 6c61 7373 6365 6c6c 5f5f 721d 0000 0072  lasscell__r....r
+00000610: 1d00 0000 7239 0000 0072 1e00 0000 7203  ....r9...r....r.
+00000620: 0000 0005 0000 0073 0e00 0000 0800 0201  .......s........
+00000630: 0202 02fe 0203 0efd 102a 7203 0000 0029  .........*r....)
+00000640: 06da 0466 6c65 7472 2900 0000 da12 666c  ...fletr).....fl
+00000650: 6574 5f6d 6174 6572 6961 6c2e 6261 7365  et_material.base
+00000660: 7202 0000 00da 0943 6f6e 7461 696e 6572  r......Container
+00000670: 7203 0000 0072 1d00 0000 721d 0000 0072  r....r....r....r
+00000680: 1d00 0000 721e 0000 00da 083c 6d6f 6475  ....r......<modu
+00000690: 6c65 3e01 0000 0073 0600 0000 0800 0c01  le>....s........
+000006a0: 1803                                     ..
```

### Comparing `flet-material-0.1.0/flet_material/__pycache__/switch.cpython-310.pyc` & `flet-material-0.2.0/flet_material/__pycache__/switch.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flet-material-0.1.0/flet_material/admonition.py` & `flet-material-0.2.0/flet_material/admonition.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,31 +3,36 @@
 
 
 class Admonitions(ft.Container):
     def __init__(
         self,
         type_: str,
         expanded_height: int,
-        expand: bool,
+        expanded: bool,
         controls_list: list,
         *args,
-        **kwargs
+        **kwargs,
     ):
-        # define: control
+        #
+        self.type_ = type_
         self.expanded_height = expanded_height
+        self.expanded = expanded
+        self.controls_list = controls_list
+
+        # define: control
         self.column = ft.Column(
-            controls=controls_list,
+            controls=self.controls_list,
         )
 
         # define admonition title properties
-        bgcolor = admonitions_color_scheme.get(type_, {}).get("bgcolor", "#20222c")
-        border_color = admonitions_color_scheme.get(type_, {}).get(
+        bgcolor = admonitions_color_scheme.get(self.type_, {}).get("bgcolor", "#20222c")
+        border_color = admonitions_color_scheme.get(self.type_, {}).get(
             "border_color", "white24"
         )
-        icon = admonitions_color_scheme.get(type_, {}).get("icon", "white24")
+        icon = admonitions_color_scheme.get(self.type_, {}).get("icon", "white24")
 
         fonts = font_scheme.get("admonitions_title", {})
         title_font = fonts.get("font_family")
         title_size = fonts.get("size")
 
         self.container = ft.Container(
             height=58,
@@ -43,15 +48,15 @@
                         controls=[
                             ft.Icon(
                                 name=icon,
                                 color=border_color,
                                 size=18,
                             ),
                             ft.Text(
-                                type_.capitalize(),
+                                self.type_.capitalize(),
                                 size=title_size,
                                 font_family=title_font,
                                 weight="w700",
                             ),
                         ],
                     ),
                     ft.IconButton(
@@ -75,15 +80,15 @@
                 color=ft.colors.with_opacity(0.35, "black"),
                 offset=ft.Offset(4, 4),
             ),
         )
         kwargs.setdefault("border", ft.border.all(0.85, border_color))
         kwargs.setdefault("clip_behavior", ft.ClipBehavior.HARD_EDGE)
         kwargs.setdefault("animate", ft.Animation(300, "decelerate"))
-        kwargs.setdefault("expand", expand)
+        kwargs.setdefault("expand", self.expanded)
         kwargs.setdefault("border_radius", 6)
         kwargs.setdefault("height", 60)
         kwargs.setdefault("padding", 0)
         kwargs.setdefault(
             "content",
             ft.Column(
                 alignment="start",
@@ -108,15 +113,23 @@
             e.control.rotate = ft.Rotate(0, ft.alignment.center)
             self.container.border_radius = 6
 
         self.update()
 
 
 class FixedAdmonitions(ft.Container):
-    def __init__(self, type_: str, expand: bool, *args, **kwargs):
+    def __init__(
+        self,
+        type_: str,
+        expanded: bool,
+        title: str,
+        *args,
+        **kwargs,
+    ):
+        self.title = title
         # define admonition title properties
         bgcolor = admonitions_color_scheme.get(type_, {}).get("bgcolor", "#20222c")
         border_color = admonitions_color_scheme.get(type_, {}).get(
             "border_color", "white24"
         )
         icon = admonitions_color_scheme.get(type_, {}).get("icon", "white24")
 
@@ -143,14 +156,20 @@
                             ),
                             ft.Text(
                                 type_.capitalize(),
                                 size=title_size,
                                 font_family=title_font,
                                 weight="w700",
                             ),
+                            ft.Text(
+                                self.title,
+                                size=13,
+                                font_family=title_font,
+                                weight="w400",
+                            ),
                         ],
                     ),
                 ],
             ),
         )
 
         # define self instance properties
@@ -162,15 +181,15 @@
                 color=ft.colors.with_opacity(0.35, "black"),
                 offset=ft.Offset(4, 4),
             ),
         )
         kwargs.setdefault("border", ft.border.all(0.85, border_color))
         kwargs.setdefault("clip_behavior", ft.ClipBehavior.HARD_EDGE)
         kwargs.setdefault("animate", ft.Animation(300, "decelerate"))
-        kwargs.setdefault("expand", expand)
+        kwargs.setdefault("expand", expanded)
         kwargs.setdefault("border_radius", 6)
         kwargs.setdefault("height", 60)
         kwargs.setdefault("padding", 0)
         kwargs.setdefault(
             "content",
             ft.Column(
                 alignment="start",
```

### Comparing `flet-material-0.1.0/flet_material/alert.py` & `flet-material-0.2.0/flet_material/alert.py`

 * *Files identical despite different names*

### Comparing `flet-material-0.1.0/flet_material/annotation.py` & `flet-material-0.2.0/flet_material/annotation.py`

 * *Files identical despite different names*

### Comparing `flet-material-0.1.0/flet_material/badge.py` & `flet-material-0.2.0/flet_material/badge.py`

 * *Files identical despite different names*

### Comparing `flet-material-0.1.0/flet_material/button.py` & `flet-material-0.2.0/flet_material/button.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import flet as ft
 from flet_material.base import Theme
 
 
 class Buttons(ft.Container, Theme):
     def __init__(self, width, height, title: str, *args, **kwargs):
         #
+        self.title = title
+        #
         self.text = ft.Text(
-            title,
+            self.title,
             weight="bold",
             color=ft.colors.with_opacity(0.85, Theme.primary_theme),
         )
         #
         kwargs.setdefault("width", width)
         kwargs.setdefault("height", height)
         kwargs.setdefault("ink", True)
```

### Comparing `flet-material-0.1.0/flet_material/checkbox.py` & `flet-material-0.2.0/flet_material/checkbox.py`

 * *Files identical despite different names*

### Comparing `flet-material-0.1.0/flet_material/switch.py` & `flet-material-0.2.0/flet_material/switch.py`

 * *Files identical despite different names*

### Comparing `flet-material-0.1.0/setup.py` & `flet-material-0.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="flet-material",
-    version="0.1.0",
+    version="0.2.0",
     author="S. Ahmad P. Hakimi",
     author_email="pourhakimi@pm.me",
     description="Material UI Library for Flet",
     long_description="",
     long_description_content_type="text/markdown",
     url="https://github.com/LineIndent/material_design_flet",
     packages=["flet_material", "styles"],
@@ -19,14 +19,7 @@
     entry_points={
         "console_scripts": [
             "flet_material_init=flet_material.command.new_project:init_code"
         ],
     },
     keywords=["material design", "UI library", "Flet"],
 )
-
-
-# Update the version number in your setup.py file. Change the version argument to a new version number, following the semantic versioning scheme (e.g., 1.0.1).
-
-# python3 setup.py sdist bdist_wheel
-
-# [inside dist direcotry] => twine upload *
```

### Comparing `flet-material-0.1.0/styles/__pycache__/admonition_style.cpython-310.pyc` & `flet-material-0.2.0/styles/__pycache__/admonition_style.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flet-material-0.1.0/styles/__pycache__/theme.cpython-310.pyc` & `flet-material-0.2.0/styles/__pycache__/theme.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flet-material-0.1.0/styles/admonition_style.py` & `flet-material-0.2.0/styles/admonition_style.py`

 * *Files identical despite different names*

### Comparing `flet-material-0.1.0/styles/theme.py` & `flet-material-0.2.0/styles/theme.py`

 * *Files identical despite different names*

