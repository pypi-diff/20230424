# Comparing `tmp/Subsearch-2.33.4.tar.gz` & `tmp/Subsearch-2.33.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Subsearch-2.33.4.tar", last modified: Tue Apr 11 17:14:02 2023, max compression
+gzip compressed data, was "Subsearch-2.33.5.tar", last modified: Mon Apr 24 21:54:43 2023, max compression
```

## Comparing `Subsearch-2.33.4.tar` & `Subsearch-2.33.5.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:14:02.893850 Subsearch-2.33.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-11 17:13:46.000000 Subsearch-2.33.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-11 17:13:46.000000 Subsearch-2.33.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-04-11 17:14:02.893850 Subsearch-2.33.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-04-11 17:13:46.000000 Subsearch-2.33.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-11 17:13:46.000000 Subsearch-2.33.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 17:14:02.893850 Subsearch-2.33.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-04-11 17:13:46.000000 Subsearch-2.33.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:14:02.881850 Subsearch-2.33.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:14:02.885850 Subsearch-2.33.4/src/Subsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-04-11 17:14:02.000000 Subsearch-2.33.4/src/Subsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-11 17:14:02.000000 Subsearch-2.33.4/src/Subsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 17:14:02.000000 Subsearch-2.33.4/src/Subsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-11 17:14:02.000000 Subsearch-2.33.4/src/Subsearch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 17:14:02.000000 Subsearch-2.33.4/src/Subsearch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-11 17:14:02.000000 Subsearch-2.33.4/src/Subsearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 17:14:02.000000 Subsearch-2.33.4/src/Subsearch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:14:02.885850 Subsearch-2.33.4/src/subsearch/
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9512 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:14:02.885850 Subsearch-2.33.4/src/subsearch/data/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/data/application_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     9106 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/data/data_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/data/languages.json
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/data/set_data.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:14:02.885850 Subsearch-2.33.4/src/subsearch/gui/
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:14:02.885850 Subsearch-2.33.4/src/subsearch/gui/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:14:02.885850 Subsearch-2.33.4/src/subsearch/gui/assets/btn/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/btn/btn_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/btn/btn_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/btn/btn_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/btn/btn_rest.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:14:02.889850 Subsearch-2.33.4/src/subsearch/gui/assets/checkbox/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/checkbox/check_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/checkbox/check_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/checkbox/check_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/checkbox/check_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/checkbox/check_tri_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/checkbox/check_tri_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/checkbox/check_tri_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/checkbox/check_tri_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/checkbox/check_unsel_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/checkbox/check_unsel_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/checkbox/check_unsel_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/checkbox/check_unsel_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/dark.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:14:02.889850 Subsearch-2.33.4/src/subsearch/gui/assets/icon/
--rw-r--r--   0 runner    (1001) docker     (123)   105808 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/icon/subsearch.ico
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/icon/subsearch.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:14:02.889850 Subsearch-2.33.4/src/subsearch/gui/assets/scale/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/scale/scale_thumb_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/scale/scale_thumb_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/scale/scale_thumb_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/scale/scale_thumb_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/scale/scale_trough_hor.png
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/scale/scale_trough_vert.png
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/scale/separator.png
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/scale/sizegrip.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:14:02.889850 Subsearch-2.33.4/src/subsearch/gui/assets/scrollbar/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/scrollbar/scroll_down.png
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/scrollbar/scroll_hor_thumb.png
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/scrollbar/scroll_hor_trough.png
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/scrollbar/scroll_left.png
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/scrollbar/scroll_right.png
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/scrollbar/scroll_up.png
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/scrollbar/scroll_vert_thumb.png
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/scrollbar/scroll_vert_trough.png
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/scrollbar/separator.png
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/scrollbar/sizegrip.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:14:02.893850 Subsearch-2.33.4/src/subsearch/gui/assets/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/tabs/download_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/tabs/download_press.png
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/tabs/download_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/tabs/language_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/tabs/language_press.png
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/tabs/language_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/tabs/search_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/tabs/search_press.png
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/tabs/search_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/tabs/settings_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/tabs/settings_press.png
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/tabs/settings_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/assets/ttk_style.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     9035 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/tab_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:14:02.893850 Subsearch-2.33.4/src/subsearch/gui/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/tabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/tabs/dowload_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/tabs/language_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/tabs/search_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/tabs/settings_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)    13667 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/gui/tkinter_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:14:02.893850 Subsearch-2.33.4/src/subsearch/providers/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/providers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/providers/opensubtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/providers/subscene.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/providers/yifysubtitles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:14:02.893850 Subsearch-2.33.4/src/subsearch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/utils/file_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/utils/imdb_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/utils/io_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/utils/io_winreg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    11259 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/utils/string_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-11 17:13:46.000000 Subsearch-2.33.4/src/subsearch/utils/updates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:54:43.453870 Subsearch-2.33.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-24 21:54:26.000000 Subsearch-2.33.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-24 21:54:26.000000 Subsearch-2.33.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-04-24 21:54:43.453870 Subsearch-2.33.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-04-24 21:54:26.000000 Subsearch-2.33.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-24 21:54:26.000000 Subsearch-2.33.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 21:54:43.453870 Subsearch-2.33.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-04-24 21:54:26.000000 Subsearch-2.33.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:54:43.441870 Subsearch-2.33.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:54:43.445870 Subsearch-2.33.5/src/Subsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-04-24 21:54:43.000000 Subsearch-2.33.5/src/Subsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-24 21:54:43.000000 Subsearch-2.33.5/src/Subsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 21:54:43.000000 Subsearch-2.33.5/src/Subsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-24 21:54:43.000000 Subsearch-2.33.5/src/Subsearch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 21:54:43.000000 Subsearch-2.33.5/src/Subsearch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-24 21:54:43.000000 Subsearch-2.33.5/src/Subsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-24 21:54:43.000000 Subsearch-2.33.5/src/Subsearch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:54:43.445870 Subsearch-2.33.5/src/subsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9512 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:54:43.445870 Subsearch-2.33.5/src/subsearch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/data/application_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9106 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/data/data_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/data/languages.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/data/set_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:54:43.445870 Subsearch-2.33.5/src/subsearch/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:54:43.445870 Subsearch-2.33.5/src/subsearch/gui/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:54:43.445870 Subsearch-2.33.5/src/subsearch/gui/assets/btn/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/btn/btn_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/btn/btn_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/btn/btn_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/btn/btn_rest.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:54:43.449870 Subsearch-2.33.5/src/subsearch/gui/assets/checkbox/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/checkbox/check_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/checkbox/check_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/checkbox/check_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/checkbox/check_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/checkbox/check_tri_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/checkbox/check_tri_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/checkbox/check_tri_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/checkbox/check_tri_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/checkbox/check_unsel_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/checkbox/check_unsel_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/checkbox/check_unsel_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/checkbox/check_unsel_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/dark.tcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:54:43.449870 Subsearch-2.33.5/src/subsearch/gui/assets/icon/
+-rw-r--r--   0 runner    (1001) docker     (123)   105808 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/icon/subsearch.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/icon/subsearch.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:54:43.449870 Subsearch-2.33.5/src/subsearch/gui/assets/scale/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/scale/scale_thumb_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/scale/scale_thumb_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/scale/scale_thumb_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/scale/scale_thumb_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/scale/scale_trough_hor.png
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/scale/scale_trough_vert.png
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/scale/separator.png
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/scale/sizegrip.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:54:43.449870 Subsearch-2.33.5/src/subsearch/gui/assets/scrollbar/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/scrollbar/scroll_down.png
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/scrollbar/scroll_hor_thumb.png
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/scrollbar/scroll_hor_trough.png
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/scrollbar/scroll_left.png
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/scrollbar/scroll_right.png
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/scrollbar/scroll_up.png
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/scrollbar/scroll_vert_thumb.png
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/scrollbar/scroll_vert_trough.png
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/scrollbar/separator.png
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/scrollbar/sizegrip.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:54:43.449870 Subsearch-2.33.5/src/subsearch/gui/assets/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/tabs/download_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/tabs/download_press.png
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/tabs/download_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/tabs/language_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/tabs/language_press.png
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/tabs/language_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/tabs/search_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/tabs/search_press.png
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/tabs/search_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/tabs/settings_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/tabs/settings_press.png
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/tabs/settings_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/assets/ttk_style.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     9035 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/tab_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:54:43.453870 Subsearch-2.33.5/src/subsearch/gui/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/tabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/tabs/dowload_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/tabs/language_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/tabs/search_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/tabs/settings_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13667 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/gui/tkinter_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:54:43.453870 Subsearch-2.33.5/src/subsearch/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/providers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/providers/opensubtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/providers/subscene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/providers/yifysubtitles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:54:43.453870 Subsearch-2.33.5/src/subsearch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/utils/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/utils/imdb_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/utils/io_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/utils/io_winreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11259 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/utils/string_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-24 21:54:26.000000 Subsearch-2.33.5/src/subsearch/utils/updates.py
```

### Comparing `Subsearch-2.33.4/LICENSE` & `Subsearch-2.33.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/PKG-INFO` & `Subsearch-2.33.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Subsearch
-Version: 2.33.4
+Version: 2.33.5
 Summary: Download subtitles for movies and shows, automatically with one easy mouse click.
 Author: vagabondHustler
 Author-email: vagabondHustler.github@gmail.com
 License: MIT license
 Project-URL: repository, https://github.com/vagabondHustler/subsearch
 Keywords: subsearch,subscene,opensubtitles,yifysubtitles,download,subtitles,movies,shows,automatically,scrape
 Platform: win32
```

### Comparing `Subsearch-2.33.4/README.md` & `Subsearch-2.33.5/README.md`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/pyproject.toml` & `Subsearch-2.33.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "Programming Language :: Python :: 3.11",
     "Operating System :: Microsoft :: Windows",
     "Topic :: Multimedia :: Video",
     "Topic :: Utilities",
     "Intended Audience :: Developers",
     "Intended Audience :: End Users/Desktop"
 ]
-dependencies = ["selectolax==0.3.12", "cloudscraper==1.2.69", "num2words==0.5.12", "packaging==23.0", "requests==2.28.2"]
+dependencies = ["selectolax==0.3.12", "cloudscraper==1.2.69", "num2words==0.5.12", "packaging==23.1", "requests==2.28.2"]
 dynamic = ["version"]
 
 [project.urls]
 repository = "https://github.com/vagabondHustler/subsearch"
 
 [project.scripts]
 subsearch = "subsearch:main"
@@ -40,16 +40,16 @@
 include = ["subsearch*"]
 exclude = ["examples*", "tools*", "subsearch.test*"]
 
 [tool.setuptools.dynamic]
 version = {attr = "subsearch.data.__version__"}
 
 [project.optional-dependencies]
-optional = ["black==23.3.0", "isort==5.12.0", "twine==4.0.2", "build==0.10.0", "cx_Freeze==6.14.9", "mypy==1.2.0", "pipreqs==0.4.11"]
-dev = ["pytest==7.3.0", "pytest-cov==4.0.0", "tox==4.4.11"]
+optional = ["black==23.3.0", "isort==5.12.0", "twine==4.0.2", "build==0.10.0", "cx_Freeze==6.14.9", "mypy==1.2.0", "pipreqs==0.4.13"]
+dev = ["pytest==7.3.1", "pytest-cov==4.0.0", "tox==4.4.12"]
 
 
 [tool.pytest.ini_options]
 filterwarnings =[
     'ignore::DeprecationWarning'
 ]
 log_cli = true
```

### Comparing `Subsearch-2.33.4/setup.py` & `Subsearch-2.33.5/setup.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/src/Subsearch.egg-info/PKG-INFO` & `Subsearch-2.33.5/src/Subsearch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Subsearch
-Version: 2.33.4
+Version: 2.33.5
 Summary: Download subtitles for movies and shows, automatically with one easy mouse click.
 Author: vagabondHustler
 Author-email: vagabondHustler.github@gmail.com
 License: MIT license
 Project-URL: repository, https://github.com/vagabondHustler/subsearch
 Keywords: subsearch,subscene,opensubtitles,yifysubtitles,download,subtitles,movies,shows,automatically,scrape
 Platform: win32
```

### Comparing `Subsearch-2.33.4/src/Subsearch.egg-info/SOURCES.txt` & `Subsearch-2.33.5/src/Subsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/src/subsearch/__init__.py` & `Subsearch-2.33.5/src/subsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/src/subsearch/core.py` & `Subsearch-2.33.5/src/subsearch/core.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/src/subsearch/data/application_config.json` & `Subsearch-2.33.5/src/subsearch/data/application_config.json`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/src/subsearch/data/data_objects.py` & `Subsearch-2.33.5/src/subsearch/data/data_objects.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/src/subsearch/data/languages.json` & `Subsearch-2.33.5/src/subsearch/data/languages.json`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/src/subsearch/data/set_data.py` & `Subsearch-2.33.5/src/subsearch/data/set_data.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/src/subsearch/gui/__init__.py` & `Subsearch-2.33.5/src/subsearch/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/src/subsearch/gui/assets/dark.tcl` & `Subsearch-2.33.5/src/subsearch/gui/assets/dark.tcl`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/src/subsearch/gui/assets/icon/subsearch.ico` & `Subsearch-2.33.5/src/subsearch/gui/assets/icon/subsearch.ico`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/src/subsearch/gui/assets/scale/scale_thumb_disabled.png` & `Subsearch-2.33.5/src/subsearch/gui/assets/scale/scale_thumb_disabled.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/src/subsearch/gui/assets/scale/scale_thumb_hover.png` & `Subsearch-2.33.5/src/subsearch/gui/assets/scale/scale_thumb_hover.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/src/subsearch/gui/assets/scale/scale_thumb_pressed.png` & `Subsearch-2.33.5/src/subsearch/gui/assets/scale/scale_thumb_pressed.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/src/subsearch/gui/assets/scale/scale_thumb_rest.png` & `Subsearch-2.33.5/src/subsearch/gui/assets/scale/scale_thumb_rest.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/src/subsearch/gui/assets/tabs/download_hover.png` & `Subsearch-2.33.5/src/subsearch/gui/assets/tabs/download_hover.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/src/subsearch/gui/assets/tabs/download_press.png` & `Subsearch-2.33.5/src/subsearch/gui/assets/tabs/download_press.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/src/subsearch/gui/assets/tabs/download_rest.png` & `Subsearch-2.33.5/src/subsearch/gui/assets/tabs/download_rest.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/src/subsearch/gui/assets/tabs/search_hover.png` & `Subsearch-2.33.5/src/subsearch/gui/assets/tabs/search_hover.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/src/subsearch/gui/assets/tabs/search_press.png` & `Subsearch-2.33.5/src/subsearch/gui/assets/tabs/search_press.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/src/subsearch/gui/assets/tabs/search_rest.png` & `Subsearch-2.33.5/src/subsearch/gui/assets/tabs/search_rest.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/src/subsearch/gui/assets/tabs/settings_hover.png` & `Subsearch-2.33.5/src/subsearch/gui/assets/tabs/settings_hover.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/src/subsearch/gui/assets/tabs/settings_press.png` & `Subsearch-2.33.5/src/subsearch/gui/assets/tabs/settings_press.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/src/subsearch/gui/assets/tabs/settings_rest.png` & `Subsearch-2.33.5/src/subsearch/gui/assets/tabs/settings_rest.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/src/subsearch/gui/assets/ttk_style.tcl` & `Subsearch-2.33.5/src/subsearch/gui/assets/ttk_style.tcl`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/src/subsearch/gui/tab_manager.py` & `Subsearch-2.33.5/src/subsearch/gui/tab_manager.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/src/subsearch/gui/tabs/dowload_tab.py` & `Subsearch-2.33.5/src/subsearch/gui/tabs/dowload_tab.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/src/subsearch/gui/tabs/language_tab.py` & `Subsearch-2.33.5/src/subsearch/gui/tabs/language_tab.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,9 +62,9 @@
         btn.bind("<ButtonRelease-1>", self.set_current_language)
 
     def set_current_language(self, event) -> None:
         btn = event.widget
         self.checkbox_values[self.active_btn].set(0)  # type: ignore
         self.active_btn.state(["!alternate"])  # type: ignore
         self.active_btn = btn
-
-        io_json.set_config_key_value("current_language", btn["text"])
+        json_key = self.name_find_key[btn["text"]]
+        io_json.set_config_key_value("current_language", json_key)
```

### Comparing `Subsearch-2.33.4/src/subsearch/gui/tabs/search_tab.py` & `Subsearch-2.33.5/src/subsearch/gui/tabs/search_tab.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/src/subsearch/gui/tabs/settings_tab.py` & `Subsearch-2.33.5/src/subsearch/gui/tabs/settings_tab.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/src/subsearch/gui/tkinter_utils.py` & `Subsearch-2.33.5/src/subsearch/gui/tkinter_utils.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/src/subsearch/providers/generic.py` & `Subsearch-2.33.5/src/subsearch/providers/generic.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/src/subsearch/providers/opensubtitles.py` & `Subsearch-2.33.5/src/subsearch/providers/opensubtitles.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/src/subsearch/providers/subscene.py` & `Subsearch-2.33.5/src/subsearch/providers/subscene.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/src/subsearch/providers/yifysubtitles.py` & `Subsearch-2.33.5/src/subsearch/providers/yifysubtitles.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/src/subsearch/utils/exceptions.py` & `Subsearch-2.33.5/src/subsearch/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/src/subsearch/utils/file_manager.py` & `Subsearch-2.33.5/src/subsearch/utils/file_manager.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/src/subsearch/utils/imdb_lookup.py` & `Subsearch-2.33.5/src/subsearch/utils/imdb_lookup.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/src/subsearch/utils/io_json.py` & `Subsearch-2.33.5/src/subsearch/utils/io_json.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/src/subsearch/utils/io_winreg.py` & `Subsearch-2.33.5/src/subsearch/utils/io_winreg.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/src/subsearch/utils/log.py` & `Subsearch-2.33.5/src/subsearch/utils/log.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/src/subsearch/utils/string_parser.py` & `Subsearch-2.33.5/src/subsearch/utils/string_parser.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.33.4/src/subsearch/utils/updates.py` & `Subsearch-2.33.5/src/subsearch/utils/updates.py`

 * *Files identical despite different names*

