# Comparing `tmp/EOmaps-6.3.tar.gz` & `tmp/EOmaps-6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/EOmaps-6.3.tar", last modified: Thu Mar 23 19:22:28 2023, max compression
+gzip compressed data, was "dist/EOmaps-6.4.tar", last modified: Mon Apr 24 13:10:45 2023, max compression
```

## Comparing `EOmaps-6.3.tar` & `EOmaps-6.4.tar`

### file list

```diff
@@ -1,75 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:22:28.000000 EOmaps-6.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:22:28.000000 EOmaps-6.3/EOmaps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13042 2023-03-23 19:22:28.000000 EOmaps-6.3/EOmaps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-03-23 19:22:28.000000 EOmaps-6.3/EOmaps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 19:22:28.000000 EOmaps-6.3/EOmaps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-23 19:22:28.000000 EOmaps-6.3/EOmaps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-23 19:22:28.000000 EOmaps-6.3/EOmaps.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-23 19:22:20.000000 EOmaps-6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13042 2023-03-23 19:22:28.000000 EOmaps-6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10507 2023-03-23 19:22:20.000000 EOmaps-6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:22:28.000000 EOmaps-6.3/eomaps/
--rw-r--r--   0 runner    (1001) docker     (123)    17356 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/NE_features.json
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68730 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/_cb_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)    26918 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/_data_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    62757 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/_shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    46419 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/_webmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    81704 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/_webmap_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)    40549 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    43344 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/colorbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    27961 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/draw.py
--rw-r--r--   0 runner    (1001) docker     (123)   175272 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/eomaps.py
--rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    82877 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    86617 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    16949 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/mapsgrid.py
--rw-r--r--   0 runner    (1001) docker     (123)    20044 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/ne_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/projections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:22:28.000000 EOmaps-6.3/eomaps/qtcompanion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/qtcompanion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/qtcompanion/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/qtcompanion/base.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/qtcompanion/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:22:28.000000 EOmaps-6.3/eomaps/qtcompanion/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/qtcompanion/icons/close.png
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/qtcompanion/icons/eye_closed.png
--rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/qtcompanion/icons/eye_open.png
--rw-r--r--   0 runner    (1001) docker     (123)    86617 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/qtcompanion/icons/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/qtcompanion/icons/maximize.png
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/qtcompanion/icons/peek_bottom.png
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/qtcompanion/icons/peek_bottom_active.png
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/qtcompanion/icons/peek_circle.png
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/qtcompanion/icons/peek_circle_active.png
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/qtcompanion/icons/peek_ellipse.png
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/qtcompanion/icons/peek_ellipse_active.png
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/qtcompanion/icons/peek_left.png
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/qtcompanion/icons/peek_left_active.png
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/qtcompanion/icons/peek_rectangle.png
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/qtcompanion/icons/peek_rectangle_active.png
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/qtcompanion/icons/peek_right.png
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/qtcompanion/icons/peek_right_active.png
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/qtcompanion/icons/peek_square.png
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/qtcompanion/icons/peek_square_active.png
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/qtcompanion/icons/peek_top.png
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/qtcompanion/icons/peek_top_active.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:22:28.000000 EOmaps-6.3/eomaps/qtcompanion/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/qtcompanion/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/qtcompanion/widgets/annotate.py
--rw-r--r--   0 runner    (1001) docker     (123)    18878 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/qtcompanion/widgets/click_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/qtcompanion/widgets/draw.py
--rw-r--r--   0 runner    (1001) docker     (123)    44722 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/qtcompanion/widgets/editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/qtcompanion/widgets/extent.py
--rw-r--r--   0 runner    (1001) docker     (123)    36930 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/qtcompanion/widgets/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    11162 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/qtcompanion/widgets/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18529 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/qtcompanion/widgets/peek.py
--rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/qtcompanion/widgets/save.py
--rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/qtcompanion/widgets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    28994 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/qtcompanion/widgets/wms.py
--rw-r--r--   0 runner    (1001) docker     (123)    46756 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    55784 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/scalebar.py
--rw-r--r--   0 runner    (1001) docker     (123)    20486 2023-03-23 19:22:20.000000 EOmaps-6.3/eomaps/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 19:22:28.000000 EOmaps-6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-03-23 19:22:20.000000 EOmaps-6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:10:45.000000 EOmaps-6.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:10:45.000000 EOmaps-6.4/EOmaps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13042 2023-04-24 13:10:44.000000 EOmaps-6.4/EOmaps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-04-24 13:10:45.000000 EOmaps-6.4/EOmaps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:10:44.000000 EOmaps-6.4/EOmaps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-24 13:10:44.000000 EOmaps-6.4/EOmaps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 13:10:44.000000 EOmaps-6.4/EOmaps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-24 13:10:33.000000 EOmaps-6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13042 2023-04-24 13:10:45.000000 EOmaps-6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10507 2023-04-24 13:10:33.000000 EOmaps-6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:10:45.000000 EOmaps-6.4/eomaps/
+-rw-r--r--   0 runner    (1001) docker     (123)    17356 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/NE_features.json
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68730 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/_cb_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27548 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/_data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62949 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46463 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/_webmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81704 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/_webmap_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40682 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44442 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/colorbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19138 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/compass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27961 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)   176295 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/eomaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82397 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86617 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16949 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/mapsgrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20044 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/ne_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/projections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:10:45.000000 EOmaps-6.4/eomaps/qtcompanion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:10:45.000000 EOmaps-6.4/eomaps/qtcompanion/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/icons/close.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/icons/eye_closed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/icons/eye_open.png
+-rw-r--r--   0 runner    (1001) docker     (123)    86617 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/icons/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/icons/maximize.png
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/icons/peek_bottom.png
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/icons/peek_bottom_active.png
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/icons/peek_circle.png
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/icons/peek_circle_active.png
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/icons/peek_ellipse.png
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/icons/peek_ellipse_active.png
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/icons/peek_left.png
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/icons/peek_left_active.png
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/icons/peek_rectangle.png
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/icons/peek_rectangle_active.png
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/icons/peek_right.png
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/icons/peek_right_active.png
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/icons/peek_square.png
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/icons/peek_square_active.png
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/icons/peek_top.png
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/icons/peek_top_active.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:10:45.000000 EOmaps-6.4/eomaps/qtcompanion/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/widgets/annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18878 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/widgets/click_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/widgets/draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47567 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/widgets/editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/widgets/extent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36930 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/widgets/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11221 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/widgets/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18529 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/widgets/peek.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/widgets/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/widgets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28994 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/qtcompanion/widgets/wms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46756 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56021 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/scalebar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20486 2023-04-24 13:10:34.000000 EOmaps-6.4/eomaps/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 13:10:45.000000 EOmaps-6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-24 13:10:34.000000 EOmaps-6.4/setup.py
```

### Comparing `EOmaps-6.3/EOmaps.egg-info/PKG-INFO` & `EOmaps-6.4/EOmaps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EOmaps
-Version: 6.3
+Version: 6.4
 Summary: A library to create interactive maps of geographical datasets.
 Home-page: https://github.com/raphaelquast/maps
 Author: Raphael Quast
 Author-email: raphael.quast@geo.tuwien.ac.at
 Maintainer: Raphael Quast
 Maintainer-email: raphael.quast@geo.tuwien.ac.at
 License: GNU General Public License v3 or later (GPLv3+)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EOmaps Version: 6.3 Summary: A library to create
+Metadata-Version: 2.1 Name: EOmaps Version: 6.4 Summary: A library to create
 interactive maps of geographical datasets. Home-page: https://github.com/
 raphaelquast/maps Author: Raphael Quast Author-email:
 raphael.quast@geo.tuwien.ac.at Maintainer: Raphael Quast Maintainer-email:
 raphael.quast@geo.tuwien.ac.at License: GNU General Public License v3 or later
 (GPLv3+) Description:
                                  [EOmaps_logo]
 [![tests](https://github.com/raphaelquast/EOmaps/actions/workflows/
```

### Comparing `EOmaps-6.3/EOmaps.egg-info/SOURCES.txt` & `EOmaps-6.4/EOmaps.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 eomaps/_data_manager.py
 eomaps/_shapes.py
 eomaps/_version.py
 eomaps/_webmap.py
 eomaps/_webmap_containers.py
 eomaps/callbacks.py
 eomaps/colorbar.py
+eomaps/compass.py
 eomaps/draw.py
 eomaps/eomaps.py
 eomaps/grid.py
 eomaps/helpers.py
 eomaps/logo.png
 eomaps/mapsgrid.py
 eomaps/ne_features.py
```

### Comparing `EOmaps-6.3/LICENSE` & `EOmaps-6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `EOmaps-6.3/PKG-INFO` & `EOmaps-6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EOmaps
-Version: 6.3
+Version: 6.4
 Summary: A library to create interactive maps of geographical datasets.
 Home-page: https://github.com/raphaelquast/maps
 Author: Raphael Quast
 Author-email: raphael.quast@geo.tuwien.ac.at
 Maintainer: Raphael Quast
 Maintainer-email: raphael.quast@geo.tuwien.ac.at
 License: GNU General Public License v3 or later (GPLv3+)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EOmaps Version: 6.3 Summary: A library to create
+Metadata-Version: 2.1 Name: EOmaps Version: 6.4 Summary: A library to create
 interactive maps of geographical datasets. Home-page: https://github.com/
 raphaelquast/maps Author: Raphael Quast Author-email:
 raphael.quast@geo.tuwien.ac.at Maintainer: Raphael Quast Maintainer-email:
 raphael.quast@geo.tuwien.ac.at License: GNU General Public License v3 or later
 (GPLv3+) Description:
                                  [EOmaps_logo]
 [![tests](https://github.com/raphaelquast/EOmaps/actions/workflows/
```

### Comparing `EOmaps-6.3/README.md` & `EOmaps-6.4/README.md`

 * *Files identical despite different names*

### Comparing `EOmaps-6.3/eomaps/NE_features.json` & `EOmaps-6.4/eomaps/NE_features.json`

 * *Files identical despite different names*

### Comparing `EOmaps-6.3/eomaps/__init__.py` & `EOmaps-6.4/eomaps/__init__.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.3/eomaps/_cb_container.py` & `EOmaps-6.4/eomaps/_cb_container.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.3/eomaps/_containers.py` & `EOmaps-6.4/eomaps/_containers.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.3/eomaps/_data_manager.py` & `EOmaps-6.4/eomaps/_data_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -414,14 +414,20 @@
                 # if the collection is still attached to the axes, remove it
                 if self.m.coll.axes is not None:
                     self.m.coll.remove()
                 self.m._coll = None
             except Exception as ex:
                 print(ex)
 
+    def _get_current_datasize(self):
+        if self._current_data:
+            return self._get_datasize(**self._current_data)
+        else:
+            return 99
+
     def on_fetch_bg(self, layer=None, bbox=None, check_redraw=True):
         # TODO support providing a bbox as extent?
         if layer is None:
             layer = self.layer
         try:
             if check_redraw and not self.redraw_required(layer):
                 return
@@ -432,15 +438,15 @@
                 return False
 
             props = self.get_props()
             if props is None:
                 # fail-fast in case the data is completely outside the extent
                 return
 
-            s = self._get_datasize(props)
+            s = self._get_datasize(**props)
             self._print_datasize_warnings(s)
 
             # stop here in case we are dealing with a pick-only dataset
             if self._only_pick:
                 return
 
             if props["x0"].size < 1 or props["y0"].size < 1:
@@ -628,16 +634,34 @@
             z_data=self._select_vals(self.z_data),
             ids=self._select_ids(),
         )
         self.last_extent = self.current_extent
 
         return self._current_data
 
-    def _get_datasize(self, props):
-        return np.size(props["z_data"])
+    def _get_datasize(self, z_data, x0, y0, **kwargs):
+        # if a dataset is provided, use it to identify the data-size
+        if z_data is not None:
+            return np.size(z_data)
+
+        sx = np.size(x0)
+
+        if len(x0.shape) == 2:
+            return sx
+
+        sy = np.size(y0)
+
+        # TODO add better treatment for 1D2D datasets with data=None
+        if len(x0.shape) == 1 and len(y0.shape) == 1:
+            if sx == sy:
+                return sx
+            else:
+                return sx * sy
+
+        return 99
 
     def _print_datasize_warnings(self, s):
         if s < 1e5:
             return
 
         name = self.m.shape.name
```

### Comparing `EOmaps-6.3/eomaps/_shapes.py` & `EOmaps-6.4/eomaps/_shapes.py`

 * *Files 0% similar despite different names*

```diff
@@ -275,42 +275,38 @@
         name = "none"
 
         def __init__(self, m):
             self._m = m
             self._n = None
 
         def _get_auto_n(self):
-            if self._m.data is not None:
-                data = self._m._data_manager._current_data.get("z_data", self._m.data)
-                s = np.size(data)
-
-                if self.name == "rectangles":
-                    # mesh currently only supports n=1
-                    if self.mesh is True:
-                        return 1
-
-                    # if plot crs is same as input-crs there is no need for
-                    # intermediate points since the rectangles are not curved!
-                    if self._m._crs_plot == self._m.data_specs.crs:
-                        return 1
-
-                if s < 10:
-                    n = 100
-                elif s < 100:
-                    n = 75
-                elif s < 1000:
-                    n = 50
-                elif s < 10000:
-                    n = 20
-                else:
-                    n = 12
+            s = self._m._data_manager._get_current_datasize()
 
-                return n
+            if self.name == "rectangles":
+                # mesh currently only supports n=1
+                if self.mesh is True:
+                    return 1
+
+                # if plot crs is same as input-crs there is no need for
+                # intermediate points since the rectangles are not curved!
+                if self._m._crs_plot == self._m.data_specs.crs:
+                    return 1
+
+            if s < 10:
+                n = 100
+            elif s < 100:
+                n = 75
+            elif s < 1000:
+                n = 50
+            elif s < 10000:
+                n = 20
             else:
-                return 12
+                n = 12
+
+            return n
 
         @property
         def n(self):
             if self._n is None:
                 return self._get_auto_n()
             else:
                 return self._n
@@ -1334,15 +1330,16 @@
             tri, datamask = self._get_delaunay_triangulation(
                 x, y, crs, self.mask_radius, self.mask_radius_crs, self.masked
             )
             maskedTris = tri.get_masked_triangles()
 
             # find the masked points that are not masked by the datamask
             mask = ~datamask.copy()
-            mask[np.where(datamask)[0][list(set(maskedTris.flat))]] = True
+            if self.masked:
+                mask[np.where(datamask)[0][list(set(maskedTris.flat))]] = True
 
             # remember the mask
             self._m._data_mask = mask
 
             color_and_array = shapes._get_colors_and_array(kwargs, datamask)
 
             if self.flat == False:
@@ -1364,15 +1361,21 @@
                 for key, val in color_and_array.items():
                     if val is None:
                         continue
 
                     if key == "array":
                         color_and_array[key] = val[maskedTris].mean(axis=1)
                     else:
-                        color_and_array[key] = val[maskedTris[:, 0]]
+                        # explicitly handle single-color entries
+                        # (e.g. int, float, str rgb-tuples etc.)
+                        if isinstance(val, (int, float, str, tuple)):
+                            pass
+                        elif isinstance(val, np.ndarray):
+                            # if arrays of colors have been provided, broadcast them
+                            color_and_array[key] = val[maskedTris[:, 0]]
 
                 # Vertices of triangles.
                 verts = np.stack((tri.x[maskedTris], tri.y[maskedTris]), axis=-1)
 
                 coll = PolyCollection(
                     verts=verts,
                     # transOffset=self._m.ax.transData,
```

### Comparing `EOmaps-6.3/eomaps/_webmap.py` & `EOmaps-6.4/eomaps/_webmap.py`

 * *Files 0% similar despite different names*

```diff
@@ -1275,14 +1275,15 @@
     _refetch_on_size_change = True
 
     def __init__(self, ax, raster_source, **kwargs):
         self.raster_source = raster_source
         # This artist fills the Axes, so should not influence layout.
         kwargs.setdefault("in_layout", False)
         kwargs.setdefault("zorder", -5)
+        kwargs.setdefault("animated", True)
 
         super().__init__(ax, **kwargs)
 
         self.cache = []
 
         ax.callbacks.connect("xlim_changed", self.on_xlim)
         self._prev_extent = (0, 0)
```

### Comparing `EOmaps-6.3/eomaps/_webmap_containers.py` & `EOmaps-6.4/eomaps/_webmap_containers.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.3/eomaps/callbacks.py` & `EOmaps-6.4/eomaps/callbacks.py`

 * *Files 1% similar despite different names*

```diff
@@ -730,14 +730,17 @@
 
         """
         shape = "ellipses" if shape == "round" else "rectangles"
 
         if not isinstance(layer, str):
             layer = self.m._get_combined_layer_name(*layer)
 
+        # add spines and relevant inset-map layers to the specified peek-layer
+        layer = self.m.BM._get_showlayer_name(layer)
+
         ID, pos, val, ind, picker_name, val_color = self._popargs(kwargs)
 
         ax = self.m.ax
 
         # default boundary args
         args = dict(fc="none", ec="k", lw=1.1)
         args.update(kwargs)
```

### Comparing `EOmaps-6.3/eomaps/colorbar.py` & `EOmaps-6.4/eomaps/colorbar.py`

 * *Files 2% similar despite different names*

```diff
@@ -266,22 +266,28 @@
             if not self._m.colorbar:
                 inherit_position = True
             else:
                 inherit_position = False
 
         self._inherit_position = inherit_position
 
-        self._hist_size = hist_size
+        if hist_size is None:
+            self._hist_size = 0
+        else:
+            self._hist_size = hist_size
+
         self._hist_bins = hist_bins
 
         if hist_kwargs is None:
             self._hist_kwargs = dict()
         else:
             self._hist_kwargs = copy.deepcopy(hist_kwargs)
 
+        self._histogram_plotted = False  # indicator if histogram has been plotted
+
         self._orientation = orientation
         self._dynamic_shade_indicator = dynamic_shade_indicator
         self._show_outline = show_outline
         self._tick_precision = tick_precision
         self._tick_formatter = tick_formatter
         self._log = log
         self._out_of_range_vals = out_of_range_vals
@@ -297,20 +303,19 @@
 
         if self._hist_bins == "bins" and not self._classified:
             raise AssertionError(
                 "EOmaps: Using hist_bins='bins' is only possible "
                 "for classified datasets!"
             )
 
-        self._redraw = False
         self._ax = None
         self.ax_cb = None
         self.ax_cb_plot = None
 
-        self._cid_redraw = None
+        self._cid_redraw = False
 
         self._set_data()
         self._setup_axes()
 
         if ylabel is not None:
             self.ax_cb_plot.set_ylabel(ylabel)
 
@@ -321,16 +326,23 @@
         Parameters
         ----------
         vis : bool
             - True: colorbar visible
             - False: colorbar not visible
         """
         for ax in self._axes:
+            if ax is self.ax_cb_plot:
+                pass
             ax.set_visible(vis)
 
+        if self._hist_size <= 0.0001:
+            self.ax_cb_plot.set_visible(False)
+        else:
+            self.ax_cb_plot.set_visible(vis)
+
     def _default_cb_tick_formatter(self, x, pos, precision=None):
         """
         A formatter to format the tick-labels of the colorbar for encoded datasets.
         (used in xaxis.set_major_formatter() )
         """
         # if precision=None the shortest representation of the number is used
         return np.format_float_positional(self._m._decode_values(x), precision)
@@ -393,31 +405,34 @@
             self.ax_cb_plot.set_axes_locator(
                 _TransformedBoundsLocator(histpos, self._ax.transAxes)
             )
             self.ax_cb.set_axes_locator(
                 _TransformedBoundsLocator(cbpos, self._ax.transAxes)
             )
 
-        # only show histogram if it is larger than 1 pixel
-        if self.ax_cb_plot.bbox.width > 1 and self.ax_cb_plot.bbox.height > 1:
+        if self._hist_size > 0.0001:
             self.ax_cb_plot.set_visible(True)
+
+            # in case the histogram has not yet been plotted, plot it!
+            if not self._histogram_plotted:
+                self._plot_histogram()
         else:
             self.ax_cb_plot.set_visible(False)  # to avoid singular matrix errors
 
         if self.ax_cb.bbox.width > 1 and self.ax_cb.bbox.height > 1:
             self.ax_cb.set_visible(True)
             [i.set_visible(True) for i in self.ax_cb.patches]
             [i.set_visible(True) for i in self.ax_cb.collections]
         else:
             self.ax_cb.set_visible(False)  # to avoid singular matrix errors
             [i.set_visible(False) for i in self.ax_cb.patches]
             [i.set_visible(False) for i in self.ax_cb.collections]
 
         # tag layer for refetch
-        self._m.BM._refetch_layer(self._m.layer)
+        self._m.redraw(self._m.layer)
 
     def _identify_parent_cb(self):
         parent_cb = None
         # check if there is already an existing colorbar for a Maps-object that shares
         # the same plot-axis.
         # If yes, use the position of this colorbar to creat a new one
 
@@ -443,15 +458,15 @@
             while parent._parent_cb is not None:
                 parent = parent._parent_cb
 
             return parent
 
     def _setup_axes(self):
         horizontal = self._orientation == "horizontal"
-        add_hist = self._hist_size > 0
+        add_hist = self._hist_size > 0.0001
 
         # check if one of the parent colorbars has a colorbar, and if so,
         # use it to set the position of the colorbar.
         if self._inherit_position:
             if self._parent_cb is not None:
 
                 try:
@@ -617,15 +632,19 @@
         if not add_hist:
             self.ax_cb_plot.set_visible(False)
 
         # add all axes as artists
         for a in self._axes:
             a.set_navigate(False)
             if a is not None:
-                self._m.BM.add_bg_artist(a, self._m.layer)
+                if self._dynamic_shade_indicator is True:
+                    self._m.BM.add_artist(a, self._m.layer)
+                else:
+                    self._m.BM.add_bg_artist(a, self._m.layer)
+
         # we need to re-draw since the background axis size has changed!
         self._m.BM._refetch_layer(self._m.layer)
         self._m.BM._refetch_layer("__SPINES__")
         self._m.redraw("__SPINES__")
 
     @property
     def _axes(self):
@@ -688,15 +707,15 @@
                 #     + "...creating a 'dynamic_shade_indicator' colorbar instead."
                 # )
                 # self._dynamic_shade_indicator = True
 
             try:
                 z_data = self._coll.get_ds_data().values
             except:
-                self._m.redraw(self.layer)
+                self._m.redraw(self._m.layer)
                 z_data = self._coll.get_ds_data().values
 
             if "count" in aggname:
                 # make sure we don't count empty pixels
                 z_data = z_data[~(z_data == 0)]
 
             # datashader sets None to 0 by default!
@@ -712,17 +731,38 @@
                 # (only clip if either vmin or vmax is not None)
                 # if vmin or vmax:
                 #     z_data = z_data.clip(vmin, vmax)
                 cmap = self._coll.get_cmap()
             else:
                 norm = self._m.classify_specs._norm
 
-            # TODO remove cid on figure close
-            if self._cid_redraw is None:
-                self._cid_redraw = self._coll.add_callback(self._redraw_colorbar)
+            if self._cid_redraw is False:
+                # TODO check why this no longer triggers on data-updates...
+                # self._m.coll.add_callback(self._redraw_colorbar)
+
+                def check_data_updated(*args, **kwargs):
+                    # make sure the artist is drawn before checking for new data
+                    self._m.f.draw_artist(self._m.coll)
+                    dsdata = self._m.coll.get_ds_data()
+                    if getattr(self, "_last_ds_data", None) is not None:
+                        if not self._last_ds_data.equals(dsdata):
+                            # if the data has changed, redraw the colorbar
+                            self._redraw_colorbar()
+                    self._last_ds_data = dsdata
+
+                self._m.BM._before_fetch_bg_actions.append(check_data_updated)
+
+                self._m.BM.on_layer(
+                    lambda *args, **kwargs: self._redraw_colorbar,
+                    layer=self._m.layer,
+                    persistent=True,
+                )
+
+                self._cid_redraw = True
+
                 # TODO colorbar not properly updated on layer change after zoom?
                 self._m.BM.on_layer(
                     self._redraw_colorbar,
                     layer=self._m.layer,
                     persistent=True,
                     m=self._m,
                 )
@@ -762,26 +802,14 @@
         # to avoid issues with vmin/vmax in-between colorbar-boundaries
 
         if hasattr(self._norm, "boundaries"):
             self._norm.boundaries = np.clip(
                 self._norm.boundaries, self._vmin, self._vmax
             )
 
-        if self._dynamic_shade_indicator:
-            if not hasattr(self, "_ds_data"):
-                self._ds_data = self._z_data
-                self._redraw = True
-                return
-            if self._ds_data.shape == self._z_data.shape:
-                if np.allclose(self._ds_data, self._z_data, equal_nan=True):
-                    self._redraw = False
-                    return
-            self._ds_data = self._z_data
-            self._redraw = True
-
     def _plot_colorbar(self):
         # plot the colorbar
         horizontal = self._orientation == "horizontal"
         n_cmap = plt.cm.ScalarMappable(cmap=self._cmap, norm=self._norm)
 
         self.cb = plt.colorbar(
             n_cmap,
@@ -841,20 +869,20 @@
         # set the axis_locator to set relative axis positions
         # TODO check why colorbar axis size changes after plot!
         # (e.g. this needs to be called AFTER plotting the colorbar to make sure
         # the extension-arrows are properly aligned)
         self.set_hist_size()
 
     def _plot_histogram(self):
-        horizontal = self._orientation == "horizontal"
-        n_cmap = plt.cm.ScalarMappable(cmap=self._cmap, norm=self._norm)
-
         if self._hist_size <= 0.0001:
             return
 
+        horizontal = self._orientation == "horizontal"
+        n_cmap = plt.cm.ScalarMappable(cmap=self._cmap, norm=self._norm)
+
         # plot the histogram
         h = self.ax_cb_plot.hist(
             self._z_data,
             orientation="vertical" if horizontal else "horizontal",
             bins=self._bins
             if (self._classified and self._hist_bins == "bins")
             else self._hist_bins,
@@ -976,18 +1004,22 @@
                 transform=self.ax_cb_plot.transAxes,
             )
             # make sure lower x-limit is 0
             if self._log is False:
                 # self.ax_cb_plot.xaxis.set_major_locator(plt.MaxNLocator(5))
                 self.ax_cb_plot.set_xlim(None, 0)
 
+        self._histogram_plotted = True
+
     def _redraw_colorbar(self, *args, **kwargs):
-        self._set_data()
-        if not self._redraw:
+        # only re-draw if the corresponding layer is visible
+        if self._m.layer not in self._m.BM.bg_layer.split("|"):
             return
+
+        self._set_data()
         self.ax_cb_plot.clear()
         self._plot_histogram()
 
     def set_bin_labels(self, bins, names, tick_lines="center", show_values=False):
         """
         Set the tick-labels of the colorbar to custom names with respect to a given
         set of bins.
@@ -1164,15 +1196,15 @@
     def tick_params(self, what="colorbar", **kwargs):
         """Set the appearance of the colorbar (or histogram) ticks."""
         if what == "colorbar":
             self.ax_cb.tick_params(**kwargs)
         elif what == "histogram":
             self.ax_cb_plot.tick_params(**kwargs)
 
-        self._m.BM._refetch_layer(self._m.layer)
+        self._m.redraw(self._m.layer)
 
     tick_params.__doc__ = (
         "NOTE\n"
         "----\n"
         "This is a wrapper for `m.colorbar.ax_cb.tick_params` or "
         "`m.colorbar.ax_cb_plot.tick_params` to set the appearance of the ticks for "
         "the colorbar or the histogram."
```

### Comparing `EOmaps-6.3/eomaps/draw.py` & `EOmaps-6.4/eomaps/draw.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.3/eomaps/eomaps.py` & `EOmaps-6.4/eomaps/eomaps.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,16 @@
     refetch_wms_on_size_change = None
     _cx_refetch_wms_on_size_change = None
     wms_container = None
 
 from .ne_features import NaturalEarth_features
 
 from ._cb_container import cb_container, _gpd_picker
-from .scalebar import ScaleBar, Compass
+from .scalebar import ScaleBar
+from .compass import Compass
 from .projections import Equi7Grid_projection  # import to supercharge cartopy.ccrs
 from .reader import read_file, from_file, new_layer_from_file
 from .grid import GridFactory
 
 from .utilities import utilities
 from .draw import ShapeDrawer
 
@@ -334,18 +335,25 @@
     __version__ = __version__
 
     from_file = from_file
     read_file = read_file
 
     CRS = ccrs
 
+    # the keybord shortcut to activate the companion-widget
     _companion_widget_key = "w"
+    # max. number of layers to show all layers as tabs in the widget
+    # (otherwise only recently active layers are shown as tabs)
+    _companion_widget_n_layer_tabs = 50
 
     CLASSIFIERS = SimpleNamespace(**dict(zip(_CLASSIFIERS, _CLASSIFIERS)))
 
+    _crs_cache = dict()
+    _transformer_cache = dict()
+
     def __init__(
         self,
         crs=None,
         layer="base",
         f=None,
         ax=None,
         preferred_wms_service="wms",
@@ -441,38 +449,23 @@
 
         self._shapes = shapes(weakref.proxy(self))
         self._shape = None
 
         # the radius is estimated when plot_map is called
         self._estimated_radius = None
 
-        # cache commonly used transformers
-        self._transf_plot_to_lonlat = Transformer.from_crs(
-            self.crs_plot,
-            self.get_crs(Maps.CRS.PlateCarree(globe=self.crs_plot.globe)),
-            always_xy=True,
-        )
-        self._transf_lonlat_to_plot = Transformer.from_crs(
-            self.get_crs(Maps.CRS.PlateCarree(globe=self.crs_plot.globe)),
-            self.crs_plot,
-            always_xy=True,
-        )
-
         # a set to hold references to the compass objects
         self._compass = set()
 
         if not hasattr(self.parent, "_wms_legend"):
             self.parent._wms_legend = dict()
 
         if not hasattr(self.parent, "_execute_callbacks"):
             self.parent._execute_callbacks = True
 
-        # initialize the shape-drawer
-        self._shape_drawer = ShapeDrawer(weakref.proxy(self))
-
         # initialize the data-manager
         self._data_manager = DataManager(self._proxy(self))
         self._data_plotted = False
         self._set_extent_on_plot = True
 
         # Make sure the figure-background patch is on an explicit layer
         # This is used to avoid having the background patch on each fetched
@@ -1326,17 +1319,14 @@
 
         Returns
         -------
         crs : pyproj.CRS
             the pyproj CRS instance
 
         """
-        if not hasattr(self, "_crs_cache"):
-            self._crs_cache = dict()
-
         # check for strings first to avoid expensive equality checking for CRS objects!
         if isinstance(crs, str):
             if crs == "in":
                 crs = self.data_specs.crs
             elif crs == "out" or crs == "plot":
                 crs = self.crs_plot
 
@@ -1747,18 +1737,17 @@
             if isinstance(radius, str) and radius != "pixel":
                 raise TypeError(f"I don't know what to do with radius='{radius}'")
 
         if xy is not None:
             ID = None
             if xy_crs is not None:
                 # get coordinate transformation
-                transformer = Transformer.from_crs(
+                transformer = self._get_transformer(
                     self.get_crs(xy_crs),
                     self.crs_plot,
-                    always_xy=True,
                 )
                 # transform coordinates
                 xy = transformer.transform(*xy)
 
         if layer is None:
             layer = self.layer
 
@@ -1893,18 +1882,17 @@
             xy is not None
         ), "EOmaps: you must provide either ID or xy to position the annotation!"
 
         xy = (np.atleast_1d(xy[0]), np.atleast_1d(xy[1]))
 
         if xy_crs is not None:
             # get coordinate transformation
-            transformer = Transformer.from_crs(
+            transformer = self._get_transformer(
                 CRS.from_user_input(xy_crs),
                 self.crs_plot,
-                always_xy=True,
             )
             # transform coordinates
             xy = transformer.transform(*xy)
 
         kwargs.setdefault("permanent", None)
 
         if isinstance(text, str) or callable(text):
@@ -1936,48 +1924,47 @@
         # store a reference to the object (required for callbacks)!
         self._compass.add(c)
         return c
 
     @wraps(ScaleBar.__init__)
     def add_scalebar(
         self,
-        lon=None,
-        lat=None,
-        azim=0,
-        preset=None,
+        pos=None,
+        rotation=0,
         scale=None,
+        n=10,
+        preset=None,
         autoscale_fraction=0.25,
-        auto_position=(0.75, 0.25),
+        auto_position=(0.8, 0.25),
         scale_props=None,
         patch_props=None,
         label_props=None,
+        line_props=None,
         layer=None,
+        size_factor=1,
+        pickable=True,
     ):
         """Add a scalebar to the map."""
         s = ScaleBar(
             m=self,
             preset=preset,
             scale=scale,
+            n=n,
             autoscale_fraction=autoscale_fraction,
             auto_position=auto_position,
             scale_props=scale_props,
             patch_props=patch_props,
             label_props=label_props,
+            line_props=line_props,
             layer=layer,
+            size_factor=size_factor,
         )
 
-        if lon is None or lat is None:
-            s._auto_position = auto_position
-            lon, lat = s._get_autopos(auto_position)
-        else:
-            # don't auto-reposition if lon/lat has been provided
-            s._auto_position = None
-
-        s._add_scalebar(lon, lat, azim)
-        s._make_pickable()
+        # add the scalebar to the map at the desired position
+        s._add_scalebar(pos=pos, azim=rotation, pickable=pickable)
 
         return s
 
     if wms_container is not None:
 
         @property
         @wraps(wms_container)
@@ -2114,24 +2101,26 @@
                     + "(`del_s`) must be 1 less than the number of points!"
                 )
         else:
             # use 100 subdivisions by default
             n = 100
             del_s = 0
 
-        t_xy_plot = Transformer.from_crs(
-            self.get_crs(xy_crs), self.crs_plot, always_xy=True
+        t_xy_plot = self._get_transformer(
+            self.get_crs(xy_crs),
+            self.crs_plot,
         )
         xplot, yplot = t_xy_plot.transform(*zip(*xy))
 
         if connect == "geod":
             # connect points via geodesic lines
             if xy_crs != 4326:
-                t = Transformer.from_crs(
-                    self.get_crs(xy_crs), self.get_crs(4326), always_xy=True
+                t = self._get_transformer(
+                    self.get_crs(xy_crs),
+                    self.get_crs(4326),
                 )
                 x, y = t.transform(*zip(*xy))
             else:
                 x, y = zip(*xy)
 
             geod = self.crs_plot.get_geod()
 
@@ -2365,14 +2354,67 @@
         if crs is not None:
             crs = self._get_cartopy_crs(crs)
         else:
             crs = Maps.CRS.PlateCarree()
 
         return self.ax.get_extent(crs=crs)
 
+    def _set_vmin_vmax(self, vmin=None, vmax=None):
+        self._vmin = vmin
+        self._vmax = vmax
+
+        if self._inherit_classification is not None:
+            if not (vmin is None and vmax is None):
+                raise TypeError(
+                    "EOmaps: 'vmin' and 'vmax' cannot be set explicitly "
+                    "if the classification is inherited!"
+                )
+
+            if self._vmin is None:
+                print("EOmaps: Warning, inherited value for 'vmin' is None!")
+            if self._vmax is None:
+                print("EOmaps: Warning, inherited value for 'vmax' is None!")
+
+            self._vmin = self._inherit_classification._vmin
+            self._vmax = self._inherit_classification._vmax
+            return
+
+        if not self.shape.name.startswith("shade_"):
+            if vmin is None and self.data is not None:
+                self._vmin = self._encode_values(np.nanmin(self._data_manager.z_data))
+            if vmax is None and self.data is not None:
+                self._vmax = self._encode_values(np.nanmax(self._data_manager.z_data))
+        else:
+            # get the name of the used aggretation reduction
+            aggname = self.shape.aggregator.__class__.__name__
+            if aggname in ["first", "last", "max", "min", "mean", "mode"]:
+                # set vmin/vmax in case the aggregation still represents data-values
+                if vmin is None:
+                    self._vmin = self._encode_values(
+                        np.nanmin(self._data_manager.z_data)
+                    )
+                if vmax is None:
+                    self._vmax = self._encode_values(
+                        np.nanmax(self._data_manager.z_data)
+                    )
+            else:
+                # set vmin/vmax for aggregations that do NOT represent data values
+
+                # allow vmin/vmax = None (e.g. autoscaling)
+                if "count" in aggname:
+                    # if the reduction represents a count, don't count empty pixels
+                    if vmin and vmin <= 0:
+                        print(
+                            "EOmaps: setting vmin=1 to avoid counting empty pixels..."
+                        )
+                        self._vmin = 1
+
+                    if vmax and vmax > 0:
+                        self._vmax = vmax
+
     def plot_map(
         self,
         layer=None,
         dynamic=False,
         set_extent=True,
         assume_sorted=True,
         indicate_masked_points=False,
@@ -2454,110 +2496,129 @@
             (dependent on the plot-shape) [linewidth, edgecolor, facecolor, ...]
 
             For "shade_points" or "shade_raster" shapes, kwargs are passed to
             `datashader.mpl_ext.dsshow`
 
         """
         verbose = kwargs.pop("verbose", 1)
+
+        # make sure zorder is set to 1 by default
+        # (by default shading would use 0 while ordinary collections use 1)
+        kwargs.setdefault("zorder", 1)
+
         if verbose >= 1:
-            if getattr(self, "coll", None) is not None:
+            if (
+                getattr(self, "coll", None) is not None
+                and len(self.cb.pick.get.cbs) > 0
+            ):
                 print(
                     "EOmaps-warning: Calling `m.plot_map()` or "
                     "`m.make_dataset_pickable()` more than once on the "
-                    "same Maps-object will override the assigned PICK-dataset!"
+                    "same Maps-object overrides the assigned PICK-dataset!"
                 )
 
-        # convert vmin/vmax values to respect the encoding of the data
-        vmin = kwargs.get("vmin", None)
-        if vmin is not None:
-            kwargs["vmin"] = self._encode_values(vmin)
-        vmax = kwargs.get("vmax", None)
-        if vmax is not None:
-            kwargs["vmax"] = self._encode_values(vmax)
-
         if layer is None:
             layer = self.layer
         else:
             if (verbose > 0) and not isinstance(layer, str):
                 print("EOmaps: The layer-name has been converted to a string!")
                 layer = str(layer)
 
         useshape = self.shape  # invoke the setter to set the default shape
+        shade_q = useshape.name.startswith("shade_")  # indicator if shading is used
 
         # make sure the colormap is properly set and transparencies are assigned
-        cmap = kwargs.setdefault("cmap", "viridis")
+        cmap = kwargs.pop("cmap", "viridis")
+
         if "alpha" in kwargs and kwargs["alpha"] < 1:
             # get a unique name for the colormap
             cmapname = self._get_alpha_cmap_name(kwargs["alpha"])
 
-            kwargs["cmap"] = cmap_alpha(
+            cmap = cmap_alpha(
                 cmap=cmap,
                 alpha=kwargs["alpha"],
                 name=cmapname,
             )
 
-            plt.colormaps.register(name=cmapname, cmap=kwargs["cmap"])
+            plt.colormaps.register(name=cmapname, cmap=cmap)
             if self._companion_widget is not None:
                 self._companion_widget.cmapsChanged.emit()
             # remember registered colormaps (to de-register on close)
             self._registered_cmaps.append(cmapname)
 
-        # make sure zorder is set to 1 by default
-        # (by default shading would use 0 while ordinary collections use 1)
-        kwargs.setdefault("zorder", 1)
-
         # ---------------------- prepare the data
         if verbose >= 10:
             print("EOmaps: Preparing the data")
 
-        if useshape.name.startswith("shade"):
-            # shade shapes use datashader to update the data of the collections!
-            self._data_manager.set_props(
-                layer=layer,
-                assume_sorted=assume_sorted,
-                update_coll_on_fetch=False,
-                indicate_masked_points=indicate_masked_points,
-                dynamic=dynamic,
-            )
+        # ---------------------- assign the data to the data_manager
+
+        # shade shapes use datashader to update the data of the collections!
+        update_coll_on_fetch = False if shade_q else True
+
+        self._data_manager.set_props(
+            layer=layer,
+            assume_sorted=assume_sorted,
+            update_coll_on_fetch=update_coll_on_fetch,
+            indicate_masked_points=indicate_masked_points,
+            dynamic=dynamic,
+        )
+
+        # ---------------------- classify the data
+        if verbose > 0 and not self._inherit_classification:
+            if self.classify_specs.scheme is not None:
+                print("EOmaps: Classifying...")
+
+        self._set_vmin_vmax(
+            vmin=kwargs.pop("vmin", None), vmax=kwargs.pop("vmax", None)
+        )
+
+        cbcmap, norm, bins, classified = self._classify_data(
+            vmin=self._vmin,
+            vmax=self._vmax,
+            cmap=cmap,
+            classify_specs=self.classify_specs,
+        )
+
+        # todo remove duplicate attributes
+        self.classify_specs._cbcmap = cbcmap
+        self.classify_specs._norm = norm
+        self.classify_specs._bins = bins
+        self.classify_specs._classified = classified
+
+        self._cbcmap = cbcmap
+        self._norm = norm
+        self._bins = bins
+        self._classified = classified
+
+        # ---------------------- plot the data
 
+        if shade_q:
             self._shade_map(
                 layer=layer,
                 dynamic=dynamic,
                 set_extent=set_extent,
                 assume_sorted=assume_sorted,
                 **kwargs,
             )
-            self.BM._refetch_layer(layer)
-
         else:
-            self._data_manager.set_props(
-                layer=layer,
-                assume_sorted=assume_sorted,
-                update_coll_on_fetch=True,
-                indicate_masked_points=indicate_masked_points,
-                dynamic=dynamic,
-            )
-
             # dont set extent if "m.set_extent" was called explicitly
             if set_extent and self._set_extent_on_plot:
                 # note bg-layers are automatically triggered for re-draw
                 # if the extent changes!
                 self._data_manager._set_lims()
 
             self._plot_map(
                 layer=layer,
                 dynamic=dynamic,
                 set_extent=set_extent,
                 assume_sorted=assume_sorted,
                 **kwargs,
             )
-            self.BM._refetch_layer(layer)
 
-            # if dynamic is False:
-            #     self.BM._refetch_layer(layer)
+        self.BM._refetch_layer(layer)
 
         if verbose >= 1:
             if getattr(self, "_data_mask", None) is not None and not np.all(
                 self._data_mask
             ):
                 print("EOmaps: Warning: some datapoints could not be drawn!")
 
@@ -2821,22 +2882,25 @@
                     self.show_layer(initial_layer)
                 else:
                     sn = self._get_snapshot()
 
         display(Image.fromarray(sn, "RGBA"), display_id=True, clear=clear)
 
     @wraps(plt.Figure.text)
-    def text(self, *args, **kwargs):
+    def text(self, *args, layer=None, **kwargs):
         """Add text to the map."""
         kwargs.setdefault("animated", True)
         kwargs.setdefault("horizontalalignment", "center")
         kwargs.setdefault("verticalalignment", "center")
 
         a = self.f.text(*args, **kwargs)
-        self.BM.add_artist(a)
+
+        if layer is None:
+            layer = self.layer
+        self.BM.add_artist(a, layer=layer)
 
         return a
 
     @_add_to_docstring(
         insert={
             "Other Parameters": (
                 "refetch_wms : bool\n"
@@ -3273,14 +3337,19 @@
                 self.parent.f._EOmaps_parent = self.parent._real_self
             self.parent._add_child(self)
 
         if isinstance(ax, plt.Axes):
             # check if the axis is already used by another maps-object
             if ax not in (i.ax for i in (self.parent, *self.parent._children)):
                 newax = True
+                ax.set_animated(True)
+                # make sure axes are drawn once to properly set transforms etc.
+                # (otherwise pan/zoom, ax.contains_point etc. will not work)
+                ax.draw(self.f.canvas.get_renderer())
+
             else:
                 newax = False
         else:
             newax = True
             # create a new axis
             if ax is None:
                 gs = GridSpec(
@@ -3308,15 +3377,19 @@
 
             ax = self.f.add_subplot(
                 *gsspec,
                 projection=projection,
                 aspect="equal",
                 adjustable="box",
                 label=self._get_ax_label(),
+                animated=True,
             )
+            # make sure axes are drawn once to properly set transforms etc.
+            # (otherwise pan/zoom, ax.contains_point etc. will not work)
+            ax.draw(self.f.canvas.get_renderer())
 
         self._ax = ax
         self._gridspec = ax.get_gridspec()
 
         # add support for "frameon" kwarg
         if kwargs.get("frameon", True) is False:
             self.ax.spines["geo"].set_edgecolor("none")
@@ -3922,55 +3995,20 @@
         layer=None,
         dynamic=False,
         set_extent=True,
         assume_sorted=True,
         **kwargs,
     ):
 
-        cmap = kwargs.pop("cmap", "viridis")
-        vmin = kwargs.pop("vmin", None)
-        vmax = kwargs.pop("vmax", None)
-
         for key in ("array", "norm"):
             assert (
                 key not in kwargs
             ), f"The key '{key}' is assigned internally by EOmaps!"
 
         try:
-            if vmin is None and self.data is not None:
-                vmin = np.nanmin(self._data_manager.z_data)
-            if vmax is None and self.data is not None:
-                vmax = np.nanmax(self._data_manager.z_data)
-
-            # clip the data to properly account for vmin and vmax
-            # (do this only if we don't intend to use the full dataset!)
-            # if vmin or vmax:
-            #     props["z_data"] = props["z_data"].clip(vmin, vmax)
-
-            # ---------------------- classify the data
-            cbcmap, norm, bins, classified = self._classify_data(
-                vmin=vmin,
-                vmax=vmax,
-                cmap=cmap,
-                classify_specs=self.classify_specs,
-            )
-
-            # TODO remove duplicated attributes!!
-            self.classify_specs._cbcmap = cbcmap
-            self.classify_specs._norm = norm
-            self.classify_specs._bins = bins
-            self.classify_specs._classified = classified
-
-            self._cbcmap = cbcmap
-            self._norm = norm
-            self._bins = bins
-            self._classified = classified
-
-            self._vmin = vmin
-            self._vmax = vmax
             self._set_extent = set_extent
 
             # ------------- plot the data
             self._coll_kwargs = kwargs
             self._coll_dynamic = dynamic
 
             # NOTE: the actual plot is performed by the data-manager
@@ -4110,73 +4148,30 @@
         """
         assert _register_datashader(), (
             "EOmaps: Missing dependency: 'datashader' \n ... please install"
             + " (conda install -c conda-forge datashader) to use the plot-shapes "
             + "'shade_points' and 'shade_raster'"
         )
 
-        cmap = kwargs.pop("cmap", "viridis")
-        vmin = kwargs.pop("vmin", None)
-        vmax = kwargs.pop("vmin", None)
-
         # remove previously fetched backgrounds for the used layer
         if dynamic is False:
             self.BM._refetch_layer(layer)
             # del self.BM._bg_layers[layer]
             # self.BM._refetch_bg = True
 
+        # in case the aggregation does not represent data-values
+        # (e.g. count, std, var ... ) use an automatic "linear" normalization
+
         # get the name of the used aggretation reduction
         aggname = self.shape.aggregator.__class__.__name__
-        if aggname in ["first", "last", "max", "min", "mean", "mode"]:
-            # set vmin/vmax in case the aggregation still represents data-values
-            if vmin is None:
-                vmin = np.nanmin(self._data_manager.z_data)
-            if vmax is None:
-                vmax = np.nanmax(self._data_manager.z_data)
-        else:
-            # set vmin/vmax for aggregations that do NOT represent data values
-
-            # allow vmin/vmax = None (e.g. autoscaling)
-            if "count" in aggname:
-                # if the reduction represents a count, don't count empty pixels
-                if vmin and vmin <= 0:
-                    print("EOmaps: setting vmin=1 to avoid counting empty pixels...")
-                    vmin = 1
-
-        if verbose > 0:
-            print("EOmaps: Classifying...")
 
-        # ---------------------- classify the data
-        cbcmap, norm, bins, classified = self._classify_data(
-            vmin=vmin,
-            vmax=vmax,
-            cmap=cmap,
-            classify_specs=self.classify_specs,
-        )
-
-        self.classify_specs._cbcmap = cbcmap
-        self.classify_specs._norm = norm
-        self.classify_specs._bins = bins
-        self.classify_specs._classified = classified
-
-        # in case the aggregation does not represent data-values
-        # (e.g. count, std, var ... ) use an automatic "linear" normalization
         if aggname in ["first", "last", "max", "min", "mean", "mode"]:
             kwargs.setdefault("norm", self.classify_specs._norm)
-            kwargs.setdefault("vmin", vmin)
-            kwargs.setdefault("vmax", vmax)
-
-            # clip the data to properly account for vmin and vmax
-            # (do this only if we don't intend to use the full dataset!)
-            # if vmin or vmax:
-            #     props["z_data"] = props["z_data"].clip(vmin, vmax)
         else:
             kwargs.setdefault("norm", "linear")
-            kwargs.setdefault("vmin", vmin)
-            kwargs.setdefault("vmax", vmax)
 
         if verbose > 0:
             print("EOmaps: Plotting...")
 
         zdata = self._data_manager.z_data
         if len(zdata) == 0:
             print("EOmaps: there was no data to plot")
@@ -4284,18 +4279,17 @@
                 )
                 xg, yg = np.meshgrid(df.x, df.y)
 
                 # transform the grid from input-coordinates to the plot-coordinates
                 crs1 = CRS.from_user_input(self.data_specs.crs)
                 crs2 = CRS.from_user_input(self._crs_plot)
                 if crs1 != crs2:
-                    transformer = Transformer.from_crs(
+                    transformer = self._get_transformer(
                         crs1,
                         crs2,
-                        always_xy=True,
                     )
                     xg, yg = transformer.transform(xg, yg)
 
                 # use a curvilinear QuadMesh
                 if self.shape.name == "shade_raster":
                     self.shape.glyph = ds.glyphs.QuadMeshCurvilinear("x", "y", "val")
 
@@ -4324,24 +4318,26 @@
             df,
             glyph=self.shape.glyph,
             aggregator=self.shape.aggregator,
             shade_hook=self.shape.shade_hook,
             agg_hook=self.shape.agg_hook,
             # norm="eq_hist",
             # norm=plt.Normalize(vmin, vmax),
-            cmap=cbcmap,
+            cmap=self._cbcmap,
             ax=self.ax,
             plot_width=plot_width,
             plot_height=plot_height,
             # x_range=(x0, x1),
             # y_range=(y0, y1),
             # x_range=(df.x.min(), df.x.max()),
             # y_range=(df.y.min(), df.y.max()),
             x_range=x_range,
             y_range=y_range,
+            vmin=self._vmin,
+            vmax=self._vmax,
             **kwargs,
         )
 
         self._coll = coll
         if verbose > 0:
             print("EOmaps: Indexing for pick-callbacks...")
 
@@ -4643,14 +4639,46 @@
                     cartopy_proj = Maps.CRS.Equi7Grid_projection(subgrid)
                     break
         else:
             raise AssertionError(f"EOmaps: cannot identify the CRS for: {crs}")
         return cartopy_proj
 
     @staticmethod
+    def _get_transformer(crs_from, crs_to):
+        # create a pyproj Transformer object or return a cached version of it
+        # if it has already been created.
+        c_from = Maps._transformer_cache.setdefault(hash(crs_from), dict())
+        return c_from.setdefault(
+            hash(crs_to), Transformer.from_crs(crs_from, crs_to, always_xy=True)
+        )
+
+    @property
+    @lru_cache()
+    def _transf_plot_to_lonlat(self):
+        # cache commonly used transformers
+        return self._get_transformer(
+            self.crs_plot,
+            self.get_crs(self.crs_plot.as_geodetic()),
+        )
+
+    @property
+    @lru_cache()
+    def _transf_lonlat_to_plot(self):
+        return self._get_transformer(
+            self.get_crs(self.crs_plot.as_geodetic()),
+            self.crs_plot,
+        )
+
+    @property
+    @lru_cache()
+    def _shape_drawer(self):
+        # initialize the shape-drawer
+        return ShapeDrawer(weakref.proxy(self))
+
+    @staticmethod
     def _make_rect_poly(x0, y0, x1, y1, crs=None, npts=100):
         """
         Return a geopandas.GeoDataFrame with a rectangle in the given crs.
 
         Parameters
         ----------
         x0, y0, y1, y1 : float
@@ -4814,26 +4842,31 @@
         if indicate_extent is not False:
             self.indicate_inset_extent(
                 parent, layer=parent.layer, permanent=True, **extent_kwargs
             )
 
         # add a background patch to the "all" layer
         if background_color is not None:
-            self._add_background_patch(color=background_color, layer="all")
+            self._bg_patch = self._add_background_patch(
+                color=background_color, layer="all"
+            )
+        else:
+            self._bg_patch = None
 
     def _add_background_patch(self, color, layer="all"):
         (art,) = self.ax.fill(
             [0, 0, 1, 1],
             [0, 1, 1, 0],
             fc=color,
             ec="none",
             zorder=-np.inf,
             transform=self.ax.transAxes,
         )
         self.BM.add_bg_artist(art, layer=layer)
+        return art
 
     def _handle_spines(self):
         spine = self.ax.spines["geo"]
         if spine not in self.BM._bg_artists.get("__inset___SPINES__", []):
             self.BM.add_bg_artist(spine, layer="__inset___SPINES__")
 
     def _get_ax_label(self):
@@ -4864,14 +4897,17 @@
         if not any((i in kwargs for i in ["fc", "facecolor"])):
             kwargs["fc"] = "none"
         if not any((i in kwargs for i in ["ec", "edgecolor"])):
             kwargs["ec"] = "r"
         if not any((i in kwargs for i in ["lw", "linewidth"])):
             kwargs["lw"] = 1
 
+        kwargs.setdefault("permanent", True)
+        kwargs.setdefault("zorder", 9999)
+
         m.add_marker(
             shape=self._inset_props["shape"],
             xy=self._inset_props["xy"],
             xy_crs=self._inset_props["xy_crs"],
             radius=self._inset_props["radius"],
             radius_crs=self._inset_props["radius_crs"],
             n=n,
```

### Comparing `EOmaps-6.3/eomaps/grid.py` & `EOmaps-6.4/eomaps/grid.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.3/eomaps/helpers.py` & `EOmaps-6.4/eomaps/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1680,35 +1680,39 @@
         if a != 1:
             rgba = rgba.copy()
             rgba[..., -1] = (rgba[..., -1] * a).astype(rgba.dtype)
         return rgba
 
     def _do_fetch_bg(self, layer, bbox=None):
         cv = self.canvas
+        renderer = cv.get_renderer()
 
         if bbox is None:
             bbox = self.figure.bbox
 
         if "|" in layer:
             if layer not in self._bg_layers:
                 self._combine_bgs(layer)
             return
 
+        # update axes spines and patches since they are used to clip artists!
+        for ax in self._get_all_map_axes():
+            ax.spines["geo"]._adjust_location()
+            ax.patch._adjust_location()
+
         # use contextmanagers to make sure the background patches are not stored
         # in the buffer regions!
         with ExitStack() as stack:
             # get rid of the axes background patches
             # (the figure background patch is on the "__BG__" layer)
             for ax_i in self._get_all_map_axes():
                 stack.enter_context(
                     ax_i.patch._cm_set(facecolor="none", edgecolor="none")
                 )
 
-            stack.enter_context(self._make_layer_artists_visible(layer=layer))
-
             # execute actions before fetching new artists
             # (e.g. update data based on extent etc.)
             for action in self._before_fetch_bg_actions:
                 action(layer=layer, bbox=bbox)
 
             # get all relevant artists to plot and remember zorders
             # self.get_bg_artists() already returns artists sorted by zorder!
@@ -1729,45 +1733,18 @@
                 return
 
             self.canvas.restore_region(self._blank_bg)
 
             if not self._m.parent._layout_editor._modifier_pressed:
                 for art in allartists:
                     if art not in self._hidden_artists:
-                        art.draw(cv.get_renderer())
+                        art.draw(renderer)
                         art.stale = False
-
                 self._bg_layers[layer] = cv.copy_from_bbox(bbox)
 
-    @contextmanager
-    def _make_layer_artists_visible(self, layer):
-        layers = [layer]
-        if layer.startswith("__inset_"):
-            layers.append("__inset_all")
-        else:
-            layers.append("all")
-
-        try:
-            for l, artists in self._bg_artists.items():
-                if l not in layers:
-                    # artists on "all" are always visible!
-                    # make all artists of other layers invisible
-                    for a in artists:
-                        a.set_visible(False)
-                else:
-                    for a in artists:
-                        a.set_visible(True)
-            yield
-
-        finally:
-            # hide all artists (to avoid triggering re-draws of webmaps etc.)
-            for a in chain(*self._m.BM._bg_artists.values()):
-                a.set_visible(False)
-            pass
-
     def _do_fetch_blank(self):
         # fetch a blank background
         if self._refetch_blank is False and self._blank_bg is not None:
             # don't re-fetch the background if it is not necessary
             return
         try:
             self._m.f.set_visible(False)
@@ -1812,15 +1789,15 @@
             if self.cid is None:
                 self.cid = self.canvas.mpl_connect("draw_event", self.on_draw)
 
     def on_draw(self, event):
         """Callback to register with 'draw_event'."""
         cv = self.canvas
 
-        if "RendererBase._draw_disabled" in cv.renderer.draw_image.__qualname__:
+        if "RendererBase._draw_disabled" in cv.get_renderer().draw_image.__qualname__:
             # TODO this fixes issues when saving figues with a "tight" bbox, e.g.:
             # m.savefig(bbox_inches='tight', pad_inches=0.1)
 
             # This workaround is necessary but the implementation is suboptimal since
             # it relies on the __qualname__ to identify if the
             # `matplotlib.backend_bases.RendererBase._draw_disabled()` context is active
             # The reason why the "_draw_disabled" context has to be handled explicitly
@@ -1892,29 +1869,32 @@
 
             - If "all": the corresponding feature will be added to ALL layers
 
             The default is None in which case the layer of the base-Maps object is used.
         """
 
         if art.figure != self.figure:
-            raise RuntimeError
+            raise RuntimeError(
+                "EOmaps: The artist does not belong to the figure"
+                "of this Maps-object!"
+            )
 
         if layer is None:
             layer = self._m.layer
 
         # make sure all layers are converted to string
         layer = str(layer)
 
-        self._artists.setdefault(layer, set())
+        self._artists.setdefault(layer, list())
 
         if art in self._artists[layer]:
             return
         else:
             art.set_animated(True)
-            self._artists[layer].add(art)
+            self._artists[layer].append(art)
 
             if isinstance(art, plt.Axes):
                 self._managed_axes.add(art)
 
     def add_bg_artist(self, art, layer=None):
         """
         Add a background-artist to be managed.
@@ -2334,14 +2314,16 @@
         def action():
             if self.bg_layer == layer:
                 return
 
             # make sure the background is fetched
             if layer not in self._bg_layers:
                 self.fetch_bg(layer)
+                # update to make sure spines etc. are properly displayed
+                self.update()
 
             x0, y0, w, h = bbox.bounds
 
             # convert the buffer to rgba so that we can add transparency
             buffer = self._bg_layers[layer]
 
             x = buffer.get_extents()
```

### Comparing `EOmaps-6.3/eomaps/logo.png` & `EOmaps-6.4/eomaps/logo.png`

 * *Files identical despite different names*

### Comparing `EOmaps-6.3/eomaps/mapsgrid.py` & `EOmaps-6.4/eomaps/mapsgrid.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.3/eomaps/ne_features.py` & `EOmaps-6.4/eomaps/ne_features.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.3/eomaps/projections.py` & `EOmaps-6.4/eomaps/projections.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,18 +31,16 @@
 # fmt: on
 
 
 class Equi7Grid_projection(ccrs.Projection):
     """
     Equi7Grid projection for cartopy.
 
-    >>> m = Maps(Equi7Grid_projection("EU"))
+    >>> m = Maps(Equi7Grid_EU)
     >>> m.add_feature.preset.coastline()
-    >>> m.ax.add_geometries([m.ax.projection.equi7_zone_polygon],
-    >>>                     m.ax.projection, fc="none", ec="r")
 
     possible subgrid's are:
         - "EU": Europe
         - "AF": Africa
         - "AS": Asia
         - "NA": North-America
         - "SA": South-America
```

### Comparing `EOmaps-6.3/eomaps/qtcompanion/app.py` & `EOmaps-6.4/eomaps/qtcompanion/app.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.3/eomaps/qtcompanion/base.py` & `EOmaps-6.4/eomaps/qtcompanion/base.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.3/eomaps/qtcompanion/icons/eye_closed.png` & `EOmaps-6.4/eomaps/qtcompanion/icons/eye_closed.png`

 * *Files identical despite different names*

### Comparing `EOmaps-6.3/eomaps/qtcompanion/icons/eye_open.png` & `EOmaps-6.4/eomaps/qtcompanion/icons/eye_open.png`

 * *Files identical despite different names*

### Comparing `EOmaps-6.3/eomaps/qtcompanion/icons/logo.png` & `EOmaps-6.4/eomaps/qtcompanion/icons/logo.png`

 * *Files identical despite different names*

### Comparing `EOmaps-6.3/eomaps/qtcompanion/icons/peek_circle.png` & `EOmaps-6.4/eomaps/qtcompanion/icons/peek_circle.png`

 * *Files identical despite different names*

### Comparing `EOmaps-6.3/eomaps/qtcompanion/icons/peek_circle_active.png` & `EOmaps-6.4/eomaps/qtcompanion/icons/peek_circle_active.png`

 * *Files identical despite different names*

### Comparing `EOmaps-6.3/eomaps/qtcompanion/icons/peek_ellipse.png` & `EOmaps-6.4/eomaps/qtcompanion/icons/peek_ellipse.png`

 * *Files identical despite different names*

### Comparing `EOmaps-6.3/eomaps/qtcompanion/icons/peek_ellipse_active.png` & `EOmaps-6.4/eomaps/qtcompanion/icons/peek_ellipse_active.png`

 * *Files identical despite different names*

### Comparing `EOmaps-6.3/eomaps/qtcompanion/widgets/annotate.py` & `EOmaps-6.4/eomaps/qtcompanion/widgets/annotate.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.3/eomaps/qtcompanion/widgets/click_callbacks.py` & `EOmaps-6.4/eomaps/qtcompanion/widgets/click_callbacks.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.3/eomaps/qtcompanion/widgets/draw.py` & `EOmaps-6.4/eomaps/qtcompanion/widgets/draw.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.3/eomaps/qtcompanion/widgets/editor.py` & `EOmaps-6.4/eomaps/qtcompanion/widgets/editor.py`

 * *Files 3% similar despite different names*

```diff
@@ -493,14 +493,15 @@
                 "save the shapes as geo-coded shapefiles.</li>"
                 "</ul>",
             )
 
 
 class LayerTabBar(QtWidgets.QTabBar):
     _number_of_min_tabs_for_size = 8
+    _n_layer_msg_shown = False
 
     def __init__(self, m=None, populate=False, *args, **kwargs):
         """
         Parameters
         ----------
         m : eomaps.Maps
             the Maps object to use
@@ -531,23 +532,23 @@
         self.setUsesScrollButtons(True)
 
         self.tabBarClicked.connect(self.tabchanged)
 
         self.setTabsClosable(True)
         self.tabCloseRequested.connect(self.close_handler)
 
-        self.m.BM.on_layer(self.color_active_tab, persistent=True)
         self.tabMoved.connect(self.tab_moved)
 
         if populate:
             # re-populate tabs if a new layer is created
             # NOTE this is done by the TabWidget if tabs have content!!
             self.populate()
-            self.m._after_add_child.append(self.populate)
             # re-populate on show to make sure currently active layers are shown
+            self.m.BM.on_layer(self.populate_on_layer, persistent=True)
+            self.m._after_add_child.append(self.populate)
             self.m._on_show_companion_widget.append(self.populate)
 
     def sizeHint(self):
         # make sure the TabBar does not expand the window width
 
         hint = super().sizeHint()
         width = self.window().width()
@@ -741,35 +742,61 @@
                 layer = self.tabText(i)
                 if layer == cl:
                     self.moveTab(i, 0)
         # re-connect tab_moved callback
         self.tabMoved.connect(self.tab_moved)
 
     @pyqtSlot()
-    def populate(self):
+    def populate_on_layer(self, *args, **kwargs):
+        lastlayer = getattr(self, "_last_populated_layer", "")
+        currlayer = self.m.BM.bg_layer
+        # only populate if the current layer is not part of the last set of layers
+        # (e.g. to allow show/hide of selected layers without removing the tabs)
+        if not set(lastlayer.split("|")).issuperset(set(currlayer.split("|"))):
+            self.populate(*args, **kwargs)
+            self._last_populated_layer = currlayer
+
+    @pyqtSlot()
+    def populate(self, *args, **kwargs):
         if not self.isVisible():
             return
 
         self._current_tab_idx = self.currentIndex()
         self._current_tab_name = self.tabText(self._current_tab_idx)
 
         alllayers = set(self.m._get_layers())
+        nlayers = len(alllayers)
+        max_n_layers = self.m._companion_widget_n_layer_tabs
+        if nlayers > max_n_layers:
+            if not LayerTabBar._n_layer_msg_shown:
+                print(
+                    "EOmaps-companion: The map has more than "
+                    f"{max_n_layers} layers... only last active layers "
+                    "are shown in the layer-tabs!"
+                )
+                LayerTabBar._n_layer_msg_shown = True
 
-        # go through the layers in reverse and remove any no longer existing layers
-        existing_layers = set()
-        for i in range(self.count(), -1, -1):
-            layer = self.tabText(i)
-            # remove all tabs that do not represent existing layers of the map
-            if layer not in alllayers:
+            # if more than 200 layers are available, show only active tabs to
+            # avoid performance issues when too many tabs are created
+            alllayers = [i for i in self.m.BM._bg_layer.split("|") if i in alllayers]
+            for i in range(self.count(), -1, -1):
                 self.removeTab(i)
-            else:
-                existing_layers.add(layer)
+        else:
+            # go through the layers in reverse and remove any no longer existing layers
+            existing_layers = set()
+            for i in range(self.count(), -1, -1):
+                layer = self.tabText(i)
+                # remove all tabs that do not represent existing layers of the map
+                if layer not in alllayers:
+                    self.removeTab(i)
+                else:
+                    existing_layers.add(layer)
 
-        # pop all existing layers from the alllayers set (no need to re-create them)
-        alllayers.difference_update(existing_layers)
+            # pop all existing layers from the alllayers set (no need to re-create them)
+            alllayers.difference_update(existing_layers)
 
         for i, layer in enumerate(sorted(alllayers)):
 
             layout = QtWidgets.QGridLayout()
             layout.setAlignment(Qt.AlignTop | Qt.AlignLeft)
 
             if layer.startswith("_"):  # or "|" in layer:
@@ -868,14 +895,15 @@
         self.m = m
 
         self.setTabBar(LayerTabBar(m=self.m))
 
         # re-populate tabs if a new layer is created
         self.populate()
         self.m._after_add_child.append(self.populate)
+        self.m.BM.on_layer(self.populate_on_layer, persistent=True)
 
         self.currentChanged.connect(self.populate_layer)
         self.m.BM._on_add_bg_artist.append(self.populate)
         self.m.BM._on_remove_bg_artist.append(self.populate)
 
         self.m._on_show_companion_widget.append(self.populate)
         self.m._on_show_companion_widget.append(self.populate_layer)
@@ -1049,40 +1077,70 @@
         #     layout.append((b_cmap, 6))  # cmap
 
         layout.append((b_r, 7))  # remove
 
         return layout
 
     @pyqtSlot()
-    def populate(self):
+    def populate_on_layer(self, *args, **kwargs):
+        lastlayer = getattr(self, "_last_populated_layer", "")
+        currlayer = self.m.BM.bg_layer
+        # only populate if the current layer is not part of the last set of layers
+        # (e.g. to allow show/hide of selected layers without removing the tabs)
+        if not set(lastlayer.split("|")).issuperset(set(currlayer.split("|"))):
+            self.populate(*args, **kwargs)
+            self._last_populated_layer = currlayer
+
+    @pyqtSlot()
+    def populate(self, *args, **kwargs):
         if not self.isVisible():
             return
 
+        tabbar = self.tabBar()
         self._current_tab_idx = self.currentIndex()
         self._current_tab_name = self.tabText(self._current_tab_idx)
 
         alllayers = sorted(list(self.m._get_layers()))
 
         self._current_tab_idx = self.currentIndex()
         self._current_tab_name = self.tabText(self._current_tab_idx)
 
         alllayers = set(self.m._get_layers())
 
         # go through the layers in reverse and remove any no longer existing layers
-        existing_layers = set()
-        for i in range(self.count(), -1, -1):
-            layer = self.tabText(i)
-            # remove all tabs that do not represent existing layers of the map
-            if layer not in alllayers:
+
+        alllayers = set(self.m._get_layers())
+        nlayers = len(alllayers)
+        max_n_layers = self.m._companion_widget_n_layer_tabs
+        if nlayers > max_n_layers:
+            if not LayerTabBar._n_layer_msg_shown:
+                print(
+                    "EOmaps-companion: The map has more than "
+                    f"{max_n_layers} layers... only last active layers "
+                    "are shown in the layer-tabs!"
+                )
+                LayerTabBar._n_layer_msg_shown = True
+
+            # if more than max_n_layers layers are available, show only active tabs to
+            # avoid performance issues when too many tabs are created
+            alllayers = [i for i in self.m.BM._bg_layer.split("|") if i in alllayers]
+            for i in range(self.count(), -1, -1):
                 self.removeTab(i)
-            else:
-                existing_layers.add(layer)
+        else:
+            existing_layers = set()
+            for i in range(self.count(), -1, -1):
+                layer = self.tabText(i)
+                # remove all tabs that do not represent existing layers of the map
+                if layer not in alllayers:
+                    self.removeTab(i)
+                else:
+                    existing_layers.add(layer)
 
-        # pop all existing layers from the alllayers set (no need to re-create them)
-        alllayers.difference_update(existing_layers)
+            # pop all existing layers from the alllayers set (no need to re-create them)
+            alllayers.difference_update(existing_layers)
 
         for i, layer in enumerate(sorted(alllayers)):
 
             layout = QtWidgets.QGridLayout()
             layout.setAlignment(Qt.AlignTop | Qt.AlignLeft)
 
             if layer.startswith("_"):  # or "|" in layer:
@@ -1095,22 +1153,19 @@
             scroll.setWidgetResizable(True)
 
             self.addTab(scroll, layer)
             self.setTabToolTip(i, layer)
 
             if layer == "all" or layer == self.m.layer:
                 # don't show the close button for this tab
-                self.tabBar().setTabButton(
-                    self.count() - 1, self.tabBar().RightSide, None
-                )
+                tabbar.setTabButton(self.count() - 1, tabbar.RightSide, None)
 
         # try to restore the previously opened tab
-        self.tabBar().set_current_tab_by_name(self._current_tab_name)
-
-        self.tabBar().color_active_tab()
+        tabbar.set_current_tab_by_name(self._current_tab_name)
+        tabbar.color_active_tab()
 
     @pyqtSlot()
     def populate_layer(self, layer=None):
         if not self.isVisible():
             return
 
         if layer is None:
```

### Comparing `EOmaps-6.3/eomaps/qtcompanion/widgets/extent.py` & `EOmaps-6.4/eomaps/qtcompanion/widgets/extent.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.3/eomaps/qtcompanion/widgets/files.py` & `EOmaps-6.4/eomaps/qtcompanion/widgets/files.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.3/eomaps/qtcompanion/widgets/layer.py` & `EOmaps-6.4/eomaps/qtcompanion/widgets/layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,14 +104,15 @@
         self.m = m
         self._layers = layers
         self._exclude = exclude
 
         self._last_layers = []
 
         menu = QtWidgets.QMenu()
+        menu.setStyleSheet("QMenu { menu-scrollable: 1;}")
         menu.aboutToShow.connect(self.update_layers)
         self.setMenu(menu)
 
         # update layers on every change of the Maps-object background layer
         self.m.BM.on_layer(self.update_visible_layer, persistent=True)
         # update layers before the widget is shown to make sure they always
         # represent the currently visible layers on startup of the widget
```

### Comparing `EOmaps-6.3/eomaps/qtcompanion/widgets/peek.py` & `EOmaps-6.4/eomaps/qtcompanion/widgets/peek.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.3/eomaps/qtcompanion/widgets/save.py` & `EOmaps-6.4/eomaps/qtcompanion/widgets/save.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.3/eomaps/qtcompanion/widgets/utils.py` & `EOmaps-6.4/eomaps/qtcompanion/widgets/utils.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.3/eomaps/qtcompanion/widgets/wms.py` & `EOmaps-6.4/eomaps/qtcompanion/widgets/wms.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.3/eomaps/reader.py` & `EOmaps-6.4/eomaps/reader.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.3/eomaps/scalebar.py` & `EOmaps-6.4/eomaps/scalebar.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,92 +1,117 @@
 from .helpers import pairwise
 from collections import OrderedDict
+from functools import lru_cache
+import warnings
 
 import numpy as np
-from pyproj import Transformer, CRS
 
-from matplotlib.collections import PolyCollection, LineCollection
+from matplotlib.collections import LineCollection
 from matplotlib.textpath import TextPath
-from matplotlib.patches import PathPatch, CirclePolygon
+from matplotlib.patches import Polygon, PathPatch
 from matplotlib.transforms import Affine2D
 from matplotlib.font_manager import FontProperties
-from matplotlib.offsetbox import AuxTransformBox
-import matplotlib.transforms as transforms
+from matplotlib.colors import to_hex
+
+_picked_scalebars = set()
 
 
 class ScaleBar:
     """Base class for EOmaps scalebars."""
 
     def __init__(
         self,
         m,
         preset=None,
         scale=None,
-        autoscale_fraction=0.25,
+        n=10,
+        autoscale_fraction=0.1,
         auto_position=(0.75, 0.25),
+        size_factor=1,
         scale_props=None,
         patch_props=None,
         label_props=None,
+        line_props=None,
         layer=None,
     ):
         """
         Add a scalebar to the map.
 
         The scalebar represents a ruler in units of meters whose direction
         follows geodesic lines.
 
         Note
         ----
         You can click on the scalebar to dynamically adjust its position,
-        orientation and size! (hold down the left mouse-button to use the keys)
+        orientation and size!
+
+        Use ` .print_code()` to print the command that will reproduce the current
+        appearance of the scalebar to the console.
+
+        - **LEFT-CLICK** on the scalebar to make the scalebar interactive
+        - drag the scalebar with the <LEFT MOUSE BUTTON>
+        - use the **SCROLL WHEEL** to adjust the (auto-)scale of the scalebar
+          (hold < shift > to make bigger steps)
+        - use < control > + **SCROLL WHEEL** to adjust the size of the labels
+
+        Keyboard-shortcuts (only active if a scalebar is selected):
+
+        - use < + > and < - > to rotate the scalebar
+        - use the < arrow-keys > to increase the frame size
+        - use < alt > + < arrow-keys > to decrease the frame size
+        - use < control > + < left > and < right > keys to adjust the label-offset
+        - use < control > + < up > and < down > keys to rotate the labels
 
-            - < LEFT-click> on the scalebar to make the scalebar interactive
-            - you can move and interact with the scalebar as long as you hold down the
-              < LEFT > mouse-button
-            - use < + > and < - > keys on your keyboard to rotate the scalebar
-            - use <alt> + < + > and < - > keys to set the text-offset
-            - use the < arrow-keys > to increase the size of the frame
-            - use < alt > + < arrow-keys > to decrease the size of the frame
-            - use the < DELETE-key > to remove the scalebar from the plot
+        - use < delete > to remove the scalebar from the plot
+        - use the < escape > to exit editing the scalebar
 
         Parameters
         ----------
         lon, lat : float
             The longitude and latitude of the starting point for the scalebar
             (If None, the center of the axis is used )
         azim : float
             The azimuth-direction (in degrees) in which the scalebar points.
             The default is 90.
         preset : str
             The name of the style preset to use.
 
-            - "bw" : a simple black-and white ruler without a background patch
+            - "bw" : a black and white scalebar with no background color
+            - "bw_2" : a black and white scalebar with white background
+            - "kr" : a black and red scalebar with semi-transparent white background
 
         scale : float or None, optional
-            The distance of the individual segments of the scalebar.
+            The distance of the segments of the scalebar.
 
             - If None: the scale is automatically updated based on the current
               zoom level and the provided "autoscale_fraction".
             - If float: A fixed length of the segments (in meters).
-              (e.g. the total length of the scalebar will be `scale_props["n"] * scale`
+              (e.g. the total length of the scalebar will be `n * scale`
 
             The default is None.
+        n : int, optional
+            The number of segments to use.
+            The default is 10.
         autoscale_fraction : float, optional
             The (approximate) fraction of the axis width to use as size for the scalebar
             in the autoscale procedure. Note that this is number is not exact since
             (depending on the crs) the final scalebar might be curved.
             The default is 0.25.
         auto_position : tuple or False, optional
             Re-position the scalebar automatically on pan/zoom events.
 
             - If False: the position of the scalebar remains fixed.
             - If a tuple is provided, it is identified as relative (x, y) position
               on the axes (e.g. (0,0)=lower left, (1,1)=upper right )
 
             The default is (0.75, 0.25).
+        size_factor : float, optional
+            A factor that is used to adjust the relative size of the labels.
+            The default is 1
+
         scale_props : dict, optional
             A dictionary that is used to set the properties of the scale.
 
             - "n": (int) The number of scales (e.g. line-segments) to draw.
             - "width": (float) The width of the scalebar
             - "colors" (tuple): A sequence of colors that will be repeated to
               color the individual line-fragments of the scalebar.
@@ -114,159 +139,335 @@
 
             - "scale": A scaling factor for the fontsize
             - "offset" : A scaling factor to adjust the offset of the labels
               relative to the scalebar
             - "rotation" : the rotation angle of the labels (in degrees)
               relative to the curvature of the scalebar
             - "color" : The color of the text
-            - "every" : indicator which scales should be labelled (e.g. every nth)
+            - "every" : indicator which sections should be labelled
+              If an integer is provided, every nth section is labelled,
+              If a list or tuple is provided, it is used to label the selected sections.
             - ... additional kwargs are passed to `matplotlib.font_manager.FontProperties`
               to set the used font-properties. Possible values are:
 
               - "family", "style", "variant", "stretch", and "weight"
 
               for example: `{family="Helvetica", style="italic"}`
 
             The default is:
                 >>> dict(scale=1, offset=1, rotation=0, every=2)
+        line_props : dict, optional
+            A dictionary that is used to set the properties of the text-indicator lines.
+            (e.g. the lines between the scale and the labels)
+
+            All arguments are passed to the LineCollection used to draw the lines.
+            Possible values are:
+
+             - "edgecolor" (or "ec"), "linewidth" (or "lw"), "linestyle" (or "ls") ...
+
         layer : str, optional
             The layer at which the scalebar should be visible.
             If None, the layer of the Maps-object used to create the scalebar is used.
             The default is None.
-
+        pickable : bool, optional
+            If True, the scalebar can be interactively adjusted using the mouse
+            and keyboard-shortcuts. If False, the scalebar is non-interactive.
+            The default is True
         """
         self._m = m
 
         if layer is None:
             layer = self._m.layer
-        self.layer = layer
+        self._layer = layer
+
+        # number of intermediate points for evaluating the curvature
+        self._interm_pts = 20
+        # size-factor to adjust the size of the labels
+        self._size_factor = size_factor
+
+        # ----- Interactivity parameters
+        self._pickable = False
+        # click offset relative to the start-position of the scale
+        self._pick_start_offset = (0.0, 0.0)
+        # multiplier for changing the scale of the scalebar
+        self._scale_factor_base = 1000
+        # multipliers for changing the label size
+        self._size_factor_base = 50
+        # inverval for adjusting the text-offset
+        self._cb_offset_interval = 0.05
+        # interval for rotating the scalebar
+        self._cb_rotate_interval = 1
+
+        self._scale = scale
+        self._n = n
+        self._estimated_scale = None
 
-        self._scale_props = dict(scale=None)
+        self._artists = OrderedDict(patch=None, scale=None)
+        self._texts = dict()
+        self._scale_props = dict()
         self._label_props = dict()
+        self._line_props = dict()
         self._patch_props = dict()
         self._patch_offsets = (1, 1, 1, 1)
 
         self._font_kwargs = dict()
         self._fontkeys = ("family", "style", "variant", "stretch", "weight")
 
-        # apply preset styling (so that any additional properties are applied on top
-        # of the preset)
+        # apply preset styling (so that additional properties are applied on top)
+        self._preset = None
         self._apply_preset(preset)
 
-        if scale is None:
-            self._autoscale = autoscale_fraction
-        else:
-            self._autoscale = None
+        self._autoscale = autoscale_fraction
+
+        assert (
+            isinstance(auto_position, tuple) or auto_position is False
+        ), "EOmaps: Scalebar 'auto_position' must be either a tuple (x, y) or False!"
 
         self._auto_position = auto_position
 
-        self.set_scale_props(scale=scale, **(scale_props if scale_props else {}))
+        self._set_scale_props(**(scale_props if scale_props else {}))
         # set the label properties
-        self.set_label_props(**(label_props if label_props else {}))
+        self._set_label_props(**(label_props if label_props else {}))
         # set the patch properties
-        self.set_patch_props(**(patch_props if patch_props else {}))
+        self._set_patch_props(**(patch_props if patch_props else {}))
+        # set the line properties
+        self._set_line_props(**(line_props if line_props else {}))
 
-        # number of intermediate points for evaluating the curvature
-        self._interm_pts = 20
+        # cache geod from plot_crs
+        self._geod = self._m.crs_plot.get_geod()
+        # cache renderer
+        self._renderer = None
 
-        self._cb_offset_interval = 0.05
-        self._cb_rotate_inverval = 1
+    @property
+    def _current_scale(self):
+        """The currently used scale of the scalebar."""
+        if self._scale is None:
+            if self._estimated_scale is None:
+                self._estimated_scale()
+            return self._estimated_scale
+        else:
+            return self._scale
 
-        # geod from plot_crs
-        self._geod = self._m.crs_plot.get_geod()
+    def get_scale(self):
+        """Get the currently used scale of the scalebar."""
+        return self._current_scale
 
-        self._artists = OrderedDict(patch=None, scale=None)
-        self._picker_name = None
+    def print_code(self, fixed=True, return_str=False):
+        """
+        Print the command that will reproduce the scalebar in its current state.
+
+        Parameters
+        ----------
+        fixed : bool, optional
+            - If True, the returned command will produce a scalebar that is fixed
+              with respect to its scale, and position.
+            - If False, the command will produce a scalebar that autoscales itself
+              with respect to the currently set autoscale parameters.
+
+            The default is True.
+        return_str: bool, optional
+            If True, the string is returned.
+            If False, the string is only printed and None is returned.
+            The default is False.
+
+        Returns
+        -------
+        code : str
+            A string of the command that will reproduce the scalebar.
+
+        """
+        s = self._get_code(fixed=fixed)
+        try:
+            import black
+
+            code = black.format_str(s, mode=black.Mode())
+            print(code)
+            if return_str:
+                return s
+        except ImportError:
+            print(s)
+            if return_str:
+                return s
+
+    def _get_code(self, fixed=True, precision=10):
+        """
+        Return a string that can be used to reproduce the scalebar in its current state.
+
+        Parameters
+        ----------
+        fixed : bool, optional
+            - If True, the returned command will produce a scalebar that is fixed
+              with respect to its scale, position and properties.
+            - If False, the command will produce a scalebar that autoscales itself
+              with respect to the currently set autoscale parameters.
+
+            The default is True.
+        precision : int, optional
+            The float precision used for lon/lat/azim values.
+            The default is 10.
+
+        Returns
+        -------
+        s : str
+            A command that will add the scalebar to the map when executed.
+
+        """
+        patch_offsets = [round(i, 3) for i in self._patch_offsets]
+        patchprops = {"offsets": patch_offsets, **self._patch_props}
+
+        labelprops = {**self._label_props, **self._font_kwargs}
+
+        layer = f"'{self._layer}'" if self._layer else "None"
+
+        if fixed:
+            s = (
+                "m.add_scalebar("
+                f"pos=({np.format_float_positional(self._lon, precision)}, "
+                f"{np.format_float_positional(self._lat, precision)}), "
+                f"rotation={np.format_float_positional(self._azim, precision=10)}, "
+                f"scale={self._scale if self._scale else 'None'}, "
+                f"n={self._n}, "
+                f"preset={self._preset if self._preset else 'None'}, "
+                f"scale_props={self._scale_props}, "
+                f"patch_props={patchprops}, "
+                f"label_props={labelprops}, "
+                f"line_props={self._line_props}, "
+                f"layer={layer}, "
+                f"size_factor={self._size_factor}"
+                ")"
+            )
+        else:
+            autopos = [
+                np.format_float_positional(i, 3)
+                for i in self._get_pos_as_autopos(self._lon, self._lat)
+            ]
+
+            s = (
+                "m.add_scalebar("
+                f"autoscale_fraction={self._autoscale}, "
+                f"auto_position=({autopos[0]}, {autopos[1]}), "
+                f"n={self._n}, "
+                f"preset={self._preset if self._preset else 'None'}, "
+                f"scale_props={self._scale_props}, "
+                f"patch_props={patchprops}, "
+                f"label_props={labelprops}, "
+                f"line_props={self._line_props}, "
+                f"layer={layer}, "
+                f"size_factor={self._size_factor}"
+                ")"
+            )
+
+        return s
 
     def _get_preset_props(self, preset):
-        scale_props = dict(n=10, width=5, colors=("k", "w"))
+        scale_props = dict(width=5, colors=("k", "w"))
         patch_props = dict(fc=".75", ec="k", lw=1, ls="-")
         label_props = dict(scale=2, offset=1, every=2, rotation=0, color="k")
+        line_props = dict(ec="k", lw=0.5, linestyle=(0, (5, 5)))
 
-        if preset == "bw":
-            scale_props.update(dict(n=10, width=4, colors=("k", "w")))
+        if preset is None:
+            pass
+        elif preset == "bw":
+            scale_props.update(dict(width=4, colors=("k", "w")))
             patch_props.update(dict(fc="none", ec="none"))
             label_props.update(
                 dict(
                     scale=1.5,
                     offset=0.5,
                     every=2,
                     weight="bold",
                     family="Courier New",
                 )
             )
-        return scale_props, patch_props, label_props
+        elif preset == "bw_2":
+            scale_props.update(dict(width=3, colors=("k", ".25", ".5", ".75", ".95")))
+            patch_props.update(dict(fc="w"))
+            label_props.update(dict(every=5, weight="bold", family="Calibri"))
+        elif preset == "kr":
+            scale_props.update(dict(width=3, colors=("k", "r")))
+            patch_props.update(dict(fc=(1, 1, 1, 0.25), ec="r", lw=0.25))
+            label_props.update(dict(weight="bold", family="Impact"))
+        else:
+            raise TypeError(f"EOmaps: The scalebar preset '{preset}' is not available.")
+
+        return scale_props, patch_props, label_props, line_props
 
     def _apply_preset(self, preset):
-        self.preset = preset
+        self._preset = preset
 
-        scale_props, patch_props, label_props = self._get_preset_props(preset)
-        self.set_scale_props(**scale_props)
-        self.set_patch_props(**patch_props)
-        self.set_label_props(**label_props)
+        scale_props, patch_props, label_props, line_props = self._get_preset_props(
+            preset
+        )
+        self._set_scale_props(**scale_props)
+        self._set_patch_props(**patch_props)
+        self._set_label_props(**label_props)
+        self._set_line_props(**line_props)
 
     def apply_preset(self, preset):
         """
         Apply a style-preset to the Scalebar.
 
+        Currently available presets are:
+
+            - "bw" : a black and white scalebar with no background color
+            - "bw_2" : a black and white scalebar with white background
+            - "kr" : a black and red scalebar with semi-transparent white background
+
+
         Parameters
         ----------
         preset : str
             The name of the preset.
 
         """
         self._apply_preset(preset)
         self._estimate_scale()
-        self.set_position()
+        self._update(BM_update=True)
 
     @staticmethod
     def _round_to_n(x, n=0):
         # round to n significant digits
         # 1234 -> 1000
         # 0.01234 -> 0.1
         res = round(x, n - int(np.floor(np.log10(abs(x)))))
         if res.is_integer():
             return int(res)
         else:
             return res
 
     def _estimate_scale(self):
         try:
-            ax2data = self._m.ax.transAxes + self._m.ax.transData.inverted()
-            ang = np.deg2rad(self._azim)
-
-            x0, y0 = ax2data.inverted().transform((self._lon, self._lat))
-
-            aspect = self._m.ax.bbox.height / self._m.ax.bbox.width
-            d = self._autoscale * aspect
-
-            dx = abs(d * np.cos(ang))
-            dy = abs(d * np.sin(ang))
+            x0, x1, y0, y1 = self._m.get_extent(4326)
 
-            p0 = ax2data.transform((x0, y0))
-            p1 = ax2data.transform((x0 + dx, y0 + dy))
+            x0, x1 = np.clip((x0, x1), -180, 180)
+            y0, y1 = np.clip((y0, y1), -90, 90)
 
-            l0 = self._m._transf_plot_to_lonlat.transform(*p0)
-            l1 = self._m._transf_plot_to_lonlat.transform(*p1)
+            n = 100
 
-            geod = self._m.ax.projection.get_geod()
+            lons, lats = np.meshgrid(np.linspace(x0, x1, n), np.linspace(y0, y1, n))
 
-            faz, baz, dist = geod.inv(*l0, *l1)
+            geod = self._geod
+            ls = geod.line_lengths(lons, lats)
+            scale = np.nanmedian(ls) * self._autoscale * 100
 
-            scale = dist / self._scale_props["n"]
-            # round to 1 significant digit
-            scale = self._round_to_n(scale)
-
-            self._scale_props["scale"] = scale
-            return scale
+            # estimate the scale so that the actually drawn labels are properly rounded
+            if isinstance(self._label_props["every"], int):
+                scale = (
+                    self._round_to_n(scale / self._n * self._label_props["every"], 1)
+                    / self._label_props["every"]
+                )
+            else:
+                scale = self._round_to_n(scale, 1) / self._n
 
+            self._estimated_scale = scale
         except Exception:
             raise AssertionError(
-                "EOmaps: Unable to determine a suitable 'scale' for the scalebar...\n"
-                + "Please provide the scale explicitly via `m.add_scalebar(scale=10000)`"
+                "EOmaps: Unable to automatically determine an "
+                "appropriate scale for the scalebar... is the "
+                "currently visible map extent heavily distorted?"
             )
 
     def _get_autopos(self, pos):
         # try to position the colorbar at the lower right corner of the axis
         x0, y0 = (self._m.ax.transAxes + self._m.ax.transData.inverted()).transform(pos)
         lon, lat = self._m._transf_plot_to_lonlat.transform(x0, y0)
 
@@ -275,79 +476,130 @@
             extent = self._m.get_extent()
             lon, lat = self._m._transf_plot_to_lonlat.transform(
                 np.mean(extent[:2]),
                 np.mean(extent[2:]),
             )
         return lon, lat
 
-    def auto_position(self, pos):
+    def _get_pos_as_autopos(self, lon, lat):
+        pos = self._m._transf_lonlat_to_plot.transform(lon, lat)
+        pos = (self._m.ax.transData + self._m.ax.transAxes.inverted()).transform(pos)
+        return pos
+
+    def _set_auto_position(self, pos):
         """Move the scalebar to the desired position and apply auto-scaling."""
         lon, lat = self._get_autopos(pos)
-        self.set_position(lon, lat, self._azim)
+        self._set_position(lon, lat, self._azim)
 
-    @property
-    def cb_rotate_interval(self):
-        """Get/set the rotation interval when rotating the scalebar with +/- keys."""
-        return self._cb_rotate_inverval
-
-    @cb_rotate_interval.setter
-    def cb_rotate_interval(self, val):
-        self._cb_rotate_inverval = val
+    def set_scale(self, scale=None):
+        """
+        Set the length of a segment of the scalebar in meters.
+
+        Parameters
+        ----------
+        scale  : float, optional
+            The length (in meters) of the individual line-segments.
+            If None, the scale will be determined automatically based on the currently
+            visible plot-extent. The default is None.
+
+        See Also
+        --------
+        set_n : Set the number of segments to use.
 
-    @property
-    def cb_offset_interval(self):
         """
-        Get/set the interval for changing the text-offset with keyboard-shortcuts.
+        self._scale = scale
+        self._update(BM_update=True)
+
+    def set_n(self, n=None):
+        """
+        Set number of segments to use for the scalebar.
+
+        Parameters
+        ----------
+        n  : int, optional
+            The number of segments. The default is None.
+
+        See Also
+        --------
+        set_scale : Set the length of the scalebar segments.
 
-        e.g.: when using the <alt> + <+>/<-> keyboard-shortcut to set the offset for
-        the scalebar-labels.
         """
-        return self._cb_offset_interval
+        self._n = n
 
-    @cb_offset_interval.setter
-    def cb_offset_interval(self, val):
-        self._cb_offset_interval = val
+        # if the number of segments changed, re-draw labels completely!
+        self._redraw_minitxt()
+        self._update(BM_update=True)
 
-    def set_scale_props(self, scale=None, n=None, width=None, colors=None):
+    def set_scale_props(self, width=None, colors=None, **kwargs):
         """
-        Set the properties of the scalebar (and update the plot accordingly).
+        Set the style properties of the scale.
 
         Parameters
         ----------
-        scale  : float, optional
-            The length (in meters) of the individual line-segments.
-            The default is 10000.
-        n : int, optional
-            The number of scales (e.g. line-segments) to draw.
-            The default is 10.
         width : float, optional
             The width of the scalebar (in ordinary matplotlib linewidth units).
             The default is 5.
         colors : tuple, optional
             A sequence of colors that will be repeated to color the individual
             line-fragments of the scalebar. (you can provide more than 2 colors!)
             The default is ("k", "w").
+
+        See Also
+        --------
+        set_scale : Set a fixed length of the scalebar segments.
+
+        set_n : Set the number of segments to use.
+
+        set_patch_props : Set style properties of the scalebar frame.
+
+        set_label_props : Set style properties of the labels.
+
+        set_line_props : Set style properties of the lines between scalebar and labels.
+
         """
-        if scale is not None:
-            self._scale_props["scale"] = scale
-        if n is not None:
-            self._scale_props["n"] = n
-            self._redraw_minitxt()
+        self._set_scale_props(width=width, colors=colors, **kwargs)
+
+        self._update(BM_update=True)
+
+    def _set_scale_props(self, width=None, colors=None, **kwargs):
+        if "n" in kwargs:
+            warnings.warn(
+                "EOmaps: Setting the number of scalebar segments ('n') via the "
+                "`scale_props` is depreciated and will raise an error in the next "
+                "major release! \n"
+                "Use `s = m.add_scalebar(n=...)` or `s.set_n(...)` instead! ",
+                FutureWarning,
+                stacklevel=4,
+            )
+            self._n = kwargs.pop("n")
+            if hasattr(self, "_lon"):
+                self._redraw_minitxt()
+
+        if "scale" in kwargs:
+            warnings.warn(
+                "EOmaps: Setting the length of the scalebar segments ('scale') via the "
+                "`scale_props` is depreciated and will raise an error in the next major "
+                " release! \n"
+                "Use `s = m.add_scalebar(scale=...)` or `s.set_scale(...)` instead! ",
+                FutureWarning,
+                stacklevel=4,
+            )
+            self._scale = kwargs.pop("scale")
+
+        if len(kwargs) > 0:
+            raise TypeError(f"{list(kwargs)} are not allowed as 'scale_props' kwargs.")
+
         if width is not None:
             self._scale_props["width"] = width
         if colors is not None:
             self._scale_props["colors"] = colors
 
-        if hasattr(self, "_lon") and hasattr(self, "_lat"):
-            self.set_position()
-            self._m.BM.update(artists=self._artists.values())
-
     def set_patch_props(self, offsets=None, **kwargs):
         """
-        Set the properties of the frame (and update the plot accordingly).
+        Set the style properties of the background patch.
 
         Parameters
         ----------
         offsets : tuple, optional
             A tuple that is used to adjust the offset of the frame-patch.
             Individual values represent `(top, bottom, left, right)` on a
             horizontally oriented scalebar. The default is (1, 1, 1, 1).
@@ -355,50 +607,121 @@
             Additional kwargs are passed to the `matpltlotlib.Patches.PolygonPatch`
             that is used to draw the frame.
             The default is `{"fc": ".75", "ec": "k", "lw": 1, "ls": "-"}`
 
             Possible values are:
 
             - "facecolor", "edgecolor", "linewidth", "linestyle", "alpha" ...
+
+        See Also
+        --------
+        set_scale_props : Set style properties of the scale.
+
+        set_label_props : Set style properties of the labels.
+
+        set_line_props : Set style properties of the lines between scalebar and labels.
+
         """
-        if offsets is not None:
-            self._patch_offsets = offsets
+        for key in kwargs:
+            if not hasattr(self._artists["patch"], f"set_{key}"):
+                raise AttributeError(f"EOmaps: '{key}' is not a valid patch property!")
 
+        self._set_patch_props(offsets=offsets, **kwargs)
+        self._update(BM_update=True)
+
+    def _set_patch_props(self, offsets=None, **kwargs):
         for key, synonym in [
             ["fc", "facecolor"],
             ["ec", "edgecolor"],
             ["lw", "linewidth"],
             ["ls", "linestyle"],
         ]:
             if key in self._patch_props:
                 self._patch_props[key] = kwargs.pop(
                     key, kwargs.pop(synonym, self._patch_props[key])
                 )
 
+        if offsets is not None:
+            self._patch_offsets = offsets
+
         self._patch_props.update(kwargs)
 
-        if hasattr(self, "_lon") and hasattr(self, "_lat"):
-            self.set_position()
-            self._m.BM.update(artists=self._artists.values())
+    def set_line_props(self, update=True, **kwargs):
+        """
+        Set the style properties of the lines connecting the scale and the labels.
+
+        Parameters
+        ----------
+        kwargs :
+            All kwargs are passed to the `matpltlotlib.Collections.LineCollection`
+            that is used to draw the frame.
+            The default is `{"ec": "k", "lw": 1, "ls": "--"}`
+
+            Possible values are:
+
+            - "edgecolor" (or "ec"), "linewidth" (or "lw"), "linestyle" (or "ls") ...
+
+        See Also
+        --------
+        set_scale_props : Set style properties of the scale.
+
+        set_patch_props : Set style properties of the scalebar frame.
+
+        set_label_props : Set style properties of the labels.
+
+        """
+        for key in kwargs:
+            if not hasattr(self._artists["patch_lines"], f"set_{key}"):
+                raise AttributeError(f"EOmaps: '{key}' is not a valid line property!")
+
+        self._set_line_props(**kwargs)
+        self._update(BM_update=True)
+
+    def _set_line_props(self, **kwargs):
+
+        for key, synonym in [
+            ["fc", "facecolor"],
+            ["ec", "edgecolor"],
+            ["lw", "linewidth"],
+            ["ls", "linestyle"],
+        ]:
+            if key in self._line_props:
+                self._line_props[key] = kwargs.pop(
+                    key, kwargs.pop(synonym, self._line_props[key])
+                )
+
+        self._line_props.update(kwargs)
 
     def set_label_props(
-        self, scale=None, rotation=None, every=None, offset=None, color=None, **kwargs
+        self,
+        scale=None,
+        rotation=None,
+        every=None,
+        offset=None,
+        color=None,
+        update=True,
+        **kwargs,
     ):
         """
-        Set the properties of the labels (and update the plot accordingly).
+        Set the style properties of the labels.
 
         Parameters
         ----------
         scale : int, optional
             A scaling factor for the fontsize of the labels. The default is 1.
         rotation : float, optional
-            the rotation angle of the labels (in degrees) relative to the
+            The rotation angle of the labels (in degrees) relative to the
             curvature of the scalebar. The default is 0.
-        every : int, optional
-            DESCRIPTION. The default is 2.
+        every : int, list or tuple of ints, optional
+            Indicator which sections of the scalebar should be labelled.
+
+            - if int: every nth section is labelled
+            - if a list/tuple is provided, only the selected sections are labelled.
+
+            The default is 2.
         offset : float, optional
             A scaling factor to adjust the offset of the labels relative to the
             scalebar. The default is 1.
         color : str or tuple
             The color of the text.
             The default is "k" (e.g. black)
         kwargs :
@@ -406,63 +729,279 @@
             to set the font specifications of the labels. Possible values are:
 
               - "family", "style", "variant", "stretch", and "weight"
 
             For example:
                 >>> dict(family="Helvetica", style="italic").
 
-        """
+        See Also
+        --------
+        set_scale_props : Set style properties of the scale.
+
+        set_patch_props : Set style properties of the scalebar frame.
+
+        set_line_props : Set style properties of the lines between scalebar and labels.
+
+        """
+        for key in kwargs:
+            if not hasattr(FontProperties, f"set_{key}"):
+                raise AttributeError(f"EOmaps: '{key}' is not a valid font property!")
+
+        self._set_label_props(
+            scale=scale,
+            rotation=rotation,
+            every=every,
+            offset=offset,
+            color=color,
+            **kwargs,
+        )
+
+        # in case the number of labels changed, re-draw labels completely
+        if every is not None:
+            self._redraw_minitxt()
+
+        self._update(BM_update=True)
+
+    def _set_label_props(
+        self,
+        scale=None,
+        rotation=None,
+        every=None,
+        offset=None,
+        color=None,
+        **kwargs,
+    ):
+
         if scale is not None:
             self._label_props["scale"] = scale
         if rotation is not None:
             self._label_props["rotation"] = rotation
         if every is not None:
             self._label_props["every"] = every
-            self._redraw_minitxt()
         if offset is not None:
             self._label_props["offset"] = offset
         if color is not None:
             self._label_props["color"] = color
 
         self._font_kwargs.update(
             **{key: kwargs.pop(key) for key in self._fontkeys if key in kwargs}
         )
         self._font_props = FontProperties(**self._font_kwargs)
 
         self._label_props.update(kwargs)
 
-        if hasattr(self, "_lon") and hasattr(self, "_lat"):
-            self.set_position()
-            self._m.BM.update(artists=self._artists.values())
+    def set_position(self, pos=None, auto_pos=None, azim=None):
+        """
+        Set the position of the colorbar.
+
+        The position hereby represents the starting-point of the scalebar!
+
+        Note
+        ----
+        If you set the position explicitly via the "pos" kwarg, the scalebar will no
+        longer automatically update its position on pan/zoom events.
+        (it can still be dragged to another position)
+
+        Parameters
+        ----------
+        pos : (float, float) or None, optional
+            (longitude, latitude) of the starting-point of the scalebar.
+
+            The default is None.
+        auto_pos : (float, float) or None, optional
+            (x, y) of the starting-point of the scalebar in relative axis-coordinates.
+            (e.g. (0, 0) = lower left corner and (1, 1) = upper right corner).
+
+            Note: If you specify a point outside the map the scalebar will not be
+            visible!
+
+            The default is None.
+        azim : float, optional
+            The azimuth-direction in which to calculate the intermediate
+            points for the scalebar. The default is None.
+
+        """
+        if pos is not None and auto_pos is not None:
+            raise TypeError(
+                "EOmaps: You can only provide either pos or auto_pos, "
+                "to set the position of the scalebar, not both!"
+            )
+
+        if pos is not None:
+            self._auto_position = False
+            self._set_position(*pos, azim=azim)
+
+        if auto_pos is not None:
+            self._auto_position = auto_pos
+
+        self._update(BM_update=True)
+
+    def _set_position(self, lon=None, lat=None, azim=None, update=False):
+        if lon is None:
+            lon = self._lon
+        if lat is None:
+            lat = self._lat
+        if azim is None:
+            azim = self._azim
+
+        self._lon = lon
+        self._lat = lat
+        self._azim = azim
+        pts = self._get_pts(lon, lat, azim)
+        d = self._get_d()
+        ang = self._get_ang(pts[0][0], pts[0][1])
+
+        # do this after setting _lon, _lat and _azim !
+        # and BEFORE all other changes since we need the size of the text-patches!
+        self._update_minitxt(d, pts)
+
+        # update scale properties
+        self._artists["scale"].set_verts(pts)
+        # don't use first and last scale (they are just used as placeholders)
+        color_names = self._get_scale_color_names()
+        colors = np.tile(
+            color_names,
+            int(np.ceil(len(pts) / len(color_names))),
+        )[: len(pts)]
+        self._artists["scale"].set_colors(colors)
+        self._artists["scale"].set_linewidth(self._scale_props["width"])
+
+        verts = self._get_patch_verts(pts, lon, lat, ang, d)
+        # TODO check how to deal with invalid vertices!!
+        # print(np.all(np.isfinite(self._m._transf_plot_to_lonlat.transform(*verts.T))))
+        # verts = np.ma.masked_invalid(verts)
+
+        self._artists["patch"].set_xy(verts)
+        self._artists["patch"].update(self._patch_props)
+
+        # update indicator lines
+        line_verts = self._get_line_verts(pts, lon, lat, self._azim, d)
+        self._artists["patch_lines"].set_segments(line_verts)
+        self._artists["patch_lines"].update(self._line_props)
+
+        if getattr(self, "_picked", False):
+            self._artists["patch"].set_edgecolor("r")
+            self._artists["patch"].set_linewidth(2)
+            self._artists["patch"].set_linestyle("-")
+
+    def set_size_factor(self, s):
+        """
+        Set the size_factor that is used to adjust the size of the labels.
+
+        Parameters
+        ----------
+        s : float
+            The size factor. The default is 1.
+        """
+        self._size_factor = s
+        self._update(BM_update=True)
+
+    def get_size_factor(self):
+        """
+        Get the current size-factor of the scalebar.
+
+        Returns
+        -------
+        size_factor
+            The size factor.
+
+        """
+        return self._size_factor
+
+    def get_position(self):
+        """
+        Return the current position (and orientation) of the scalebar.
+
+        Returns
+        -------
+        list
+            a list corresponding to [longitude, latitude, azimuth].
+        """
+        return [self._lon, self._lat, self._azim]
+
+    def set_auto_scale(self, autoscale_fraction=0.25):
+        """
+        Automatically evaluate an appropriate scale for the scalebar.
+
+        (and dynamically update the scale on pan/zoom events.)
+
+
+        Parameters
+        ----------
+        autoscale_fraction : float, or None, optional
+            The (approximate) fraction of the axis width to use as size for the scalebar
+            in the autoscale procedure. Note that this is number is not exact since
+            (depending on the crs) the final scalebar might be curved.
+
+            If None, the current scale is maintained.
+            The default is 0.25.
+        """
+        self._autoscale = autoscale_fraction
+        self._update(BM_update=True)
+
+    def set_pickable(self, q):
+        """
+        Set if the scalebar is interactive (True) or not (False).
+
+        If True, the following interactions can be performed:
+
+        - **LEFT-CLICK** on the scalebar to make the scalebar interactive
+        - drag the scalebar with the <LEFT MOUSE BUTTON>
+        - use the **SCROLL WHEEL** to adjust the (auto-)scale of the scalebar
+        - use < control > + **SCROLL WHEEL** to adjust the size of the labels
+
+        Keyboard-shortcuts (only active if a scalebar is selected):
+
+        - use < + > and < - > to rotate the scalebar
+        - use the < arrow-keys > to increase the frame size
+        - use < alt > + < arrow-keys > to decrease the frame size
+        - use < control > + < left > and < right > keys to adjust the label-offset
+        - use < control > + < up > and < down > keys to rotate the labels
+
+        - use < delete > to remove the scalebar from the plot
+        - use the < escape > to exit editing the scalebar
+
+        Parameters
+        ----------
+        q : bool
+            Indicator if the scalebar is interactive (True) or not (False).
+
+        """
+        if q is True:
+            self._make_pickable()
+        else:
+            self._undo_pickable()
 
     def _get_base_pts(self, lon, lat, azim, npts=None):
         if npts is None:
-            npts = self._scale_props["n"] + 1
+            npts = self._n + 1
 
         pts = self._geod.fwd_intermediate(
             lon1=lon,
             lat1=lat,
             azi1=azim,
             npts=npts,
-            del_s=self._scale_props["scale"],
+            del_s=self._current_scale,
             initial_idx=0,
             terminus_idx=0,
         )
+
+        if isinstance(self._label_props["every"], int):
+            self._every = [
+                i for i in range(pts.npts) if i % self._label_props["every"] == 0
+            ]
+        else:
+            self._every = [i for i in self._label_props["every"] if i <= pts.npts]
         return pts
 
     def _get_pts(self, lon, lat, azim):
         pts = self._get_base_pts(lon, lat, azim)
 
         lons, lats = [], []
         for [lon1, lon2], [lat1, lat2] in zip(pairwise(pts.lons), pairwise(pts.lats)):
-            if abs(lon1 - lon2) > 180:
-                continue
-            if abs(lat1 - lat2) > 90:
-                continue
-
             # get intermediate points
             p = self._geod.inv_intermediate(
                 lon1=lon1,
                 lat1=lat1,
                 lon2=lon2,
                 lat2=lat2,
                 npts=self._interm_pts,
@@ -475,57 +1014,54 @@
         # transform points to plot-crs
         pts_t = self._m._transf_lonlat_to_plot.transform(np.array(lons), np.array(lats))
         pts_t = np.stack(pts_t, axis=2)
 
         return pts_t
 
     def _get_txt(self, n):
-        scale = self._scale_props["scale"]
+        scale = self._current_scale
         # the text displayed above the scalebar
         units = {" mm": 0.001, " m": 1, " km": 1000, "k km": 1000000}
         for key, val in units.items():
             x = scale * n / val
             if scale * n / val < 1000:
                 return np.format_float_positional(x, trim="-", precision=3) + key
 
         return f"{scale} m"
 
     def _txt(self):
-        return self._get_txt(self._scale_props["n"])
+        return self._get_txt(self._n)
 
     def _get_d(self):
         # the base length used to define the size of the scalebar
+        x0, x1, y0, y1 = self._m.get_extent(self._m.crs_plot)
 
-        # get the position in figure coordinates
-        x, y = self._m.ax.transData.transform(
-            self._m._transf_lonlat_to_plot.transform(self._lon, self._lat)
+        return (
+            np.max(np.abs([x0 - x1, y0 - y1]))
+            / self._size_factor_base
+            * self._size_factor
         )
 
-        d_fig = max(self._m.ax.bbox.height, self._m.ax.bbox.width) / 100
-        # translate d_fig to data-coordinates
-        xb, yb = self._m.ax.transData.inverted().transform(
-            ([x, y + d_fig], [x, y - d_fig])
-        )
-        return np.abs(xb[1] - yb[1])
-
     def _get_patch_verts(self, pts, lon, lat, ang, d):
-        # top bottom left right referrs to a horizontally oriented colorbar!
-        ot = d * self._patch_offsets[0]
-        ob = self._maxw + d * (self._label_props["offset"] + self._patch_offsets[1])
-        o_l = d * self._patch_offsets[2]
-        o_r = d * self._patch_offsets[3]
+        offsets = self._patch_offsets
 
-        # in case the top scale has a label, add a margin to encompass the text!
-        if len(pts) % self._label_props["every"] == 0:
-            o_r += self._top_h * 1.5
+        # top bottom left right referrs to a horizontally oriented colorbar!
+        ot = d * offsets[0]
+        ob = self._maxw + d * (self._label_props["offset"] + offsets[1])
+        o_l = d * offsets[2]
+        o_r = d * offsets[3]
 
         dxy = np.gradient(pts.reshape((-1, 2)), axis=0)
         alpha = np.arctan2(dxy[:, 1], -dxy[:, 0])
         t = np.column_stack([np.sin(alpha), np.cos(alpha)])
 
+        # in case the top scale has a label, add a margin to encompass the text!
+        if len(pts) in self._every:
+            o_r += self._top_h / 2
+
         ptop = pts.reshape((-1, 2)) - ot * t
         pbottom = pts.reshape((-1, 2)) + ob * t
 
         ptop[0] += (o_l * np.cos(alpha[0]), -o_l * np.sin(alpha[0]))
         pbottom[0] += (o_l * np.cos(alpha[0]), -o_l * np.sin(alpha[0]))
 
         ptop[-1] -= (o_r * np.cos(alpha[-1]), -o_r * np.sin(alpha[-1]))
@@ -549,90 +1085,122 @@
     def _get_txt_coords(self, lon, lat, d, ang):
         # get the base point for the text
         xt, yt = self._m._transf_lonlat_to_plot.transform(lon, lat)
         xt = xt - d * self._label_props["offset"] * np.sin(ang)
         yt = yt + d * self._label_props["offset"] * np.cos(ang)
         return xt, yt
 
-    from functools import lru_cache
+    def _get_line_pts(self, lon, lat, d, ang):
+        # get the base point for the text
+        x0, y0 = self._m._transf_lonlat_to_plot.transform(lon, lat)
+
+        offset = d / 3
+
+        ox = offset * self._label_props["offset"] * np.sin(ang)
+        oy = offset * self._label_props["offset"] * np.cos(ang)
+
+        x0 -= ox
+        y0 += oy
+
+        x1 = x0 - d * self._label_props["offset"] * np.sin(ang) + ox * 1.2
+        y1 = y0 + d * self._label_props["offset"] * np.cos(ang) - oy * 1.2
+        return (x0, y0), (x1, y1)
+
+    def _get_line_verts(self, pts, lon, lat, ang, d):
+        line_pts = self._get_base_pts(lon, lat, ang)
+        line_lons, line_lats = line_pts.lons, line_pts.lats
+
+        angs = np.arctan2(*np.array([p[0] - p[-1] for p in pts]).T[::-1])
+        angs = [*angs, angs[-1]]
+
+        lines = []
+        for i, (lon, lat, ang) in enumerate(zip(line_lons, line_lats, angs)):
+            if i not in self._every:
+                continue
+
+            lines.append(self._get_line_pts(lon, lat, d, ang))
+
+        return lines
 
     # cache this to avoid re-evaluating the text-size when dragging the scalebar
     @lru_cache(1)
     def _get_maxw(self, sscale, sn, lscale, lrotation, levery):
         # arguments are only used for caching!
 
-        # update here to make sure axis-transformations etc. are properly set
-        self._m.BM.update(blit=False)
-
         # the max. width of the texts
         _maxw = 0
-        for key, val in self._artists.items():
-            if not key.startswith("text_"):
-                continue
+        _top_h = 0
 
-            # use try-except here since the renderer can only estimate the size
-            # if the object is within the canvas!
-            try:
-                # get the widths of the text patches in data-coordinates
-                bbox = val.get_window_extent(self._m.f.canvas.get_renderer())
-                bbox = bbox.transformed(self._m.ax.transData.inverted())
-                # use the max to account for rotated text objects
-                w = max(bbox.width, bbox.height)
-                if w > _maxw:
-                    _maxw = w
-            except Exception:
-                pass
+        _transf_data_inverted = self._m.ax.transData.inverted()
 
-        _top_h = 0
+        # make sure to cache the renderer instance to avoid performance issues!
+        if self._renderer is None:
+            self._renderer = self._m.f.canvas.get_renderer()
+
+        # use the longest label to evaluate the max. width of the texts
+        try:
+            txtartist = self._artists[
+                max(self._texts, key=lambda x: len(self._texts[x]))
+            ]
+            bbox = txtartist.get_window_extent(self._renderer).transformed(
+                _transf_data_inverted
+            )
+            _maxw = max(bbox.width, bbox.height)
+        except Exception:
+            pass
+
+        # evaluate the size of the "top" label
         try:
-            _top_label = next(i for i in sorted(self._artists) if i.startswith("text_"))
+            _top_label = next(i for i in sorted(self._texts))
             val = self._artists[_top_label]
-            bbox = val.get_window_extent(self._m.f.canvas.get_renderer())
-            bbox = bbox.transformed(self._m.ax.transData.inverted())
-            _top_h = min(bbox.width, bbox.height)
+            bbox = val.get_window_extent(self._renderer).transformed(
+                _transf_data_inverted
+            )
+            _top_h = np.sqrt(bbox.width**2 + bbox.height**2)
         except Exception:
             pass
 
         self._maxw = _maxw
         self._top_h = _top_h
 
     def _set_minitxt(self, d, pts):
         angs = np.arctan2(*np.array([p[0] - p[-1] for p in pts]).T[::-1])
         angs = [*angs, angs[-1]]
-        pts = self._get_base_pts(
-            self._lon, self._lat, self._azim, npts=self._scale_props["n"] + 2
-        )
+        pts = self._get_base_pts(self._lon, self._lat, self._azim, npts=self._n + 2)
 
+        self._texts.clear()
         for i, (lon, lat, ang) in enumerate(zip(pts.lons, pts.lats, angs)):
-            if i % self._label_props["every"] != 0:
+            if i not in self._every:
                 continue
+
             if i == 0:
                 txt = "0"
             else:
                 txt = self._get_txt(i)
 
             xy = self._get_txt_coords(lon, lat, d, ang)
             tp = TextPath(
                 xy, txt, size=self._label_props["scale"] * d / 2, prop=self._font_props
             )
 
-            self._artists[f"text_{i}"] = self._m.ax.add_artist(
-                PathPatch(tp, color=self._label_props["color"], lw=0)
-            )
-            self._artists[f"text_{i}"].set_transform(
+            patch = PathPatch(tp, color=self._label_props["color"], lw=0, zorder=1)
+            patch.set_transform(
                 Affine2D().rotate_around(
                     *xy, ang + np.pi / 2 + np.deg2rad(self._label_props["rotation"])
                 )
                 + self._m.ax.transData
             )
 
-            self._artists[f"text_{i}"].set_zorder(1)
-            self._m.BM.add_artist(self._artists[f"text_{i}"], layer=self.layer)
+            self._artists[f"text_{i}"] = self._m.ax.add_artist(patch)
+            self._texts[f"text_{i}"] = txt
+            self._m.BM.add_artist(self._artists[f"text_{i}"], layer=self._layer)
 
     def _redraw_minitxt(self):
+        # re-draw the text patches in case the number of texts changed
+
         # don't redraw if we haven't drawn anything yet
         if not hasattr(self, "_artists"):
             return
 
         for key in list(self._artists):
             if key.startswith("text_"):
                 self._artists[key].remove()
@@ -642,20 +1210,18 @@
         pts = self._get_pts(self._lon, self._lat, self._azim)
         d = self._get_d()
         self._set_minitxt(d, pts)
 
     def _update_minitxt(self, d, pts):
         angs = np.arctan2(*np.array([p[0] - p[-1] for p in pts]).T[::-1])
         angs = [*angs, angs[-1]]
-        pts = self._get_base_pts(
-            self._lon, self._lat, self._azim, npts=self._scale_props["n"] + 2
-        )
+        pts = self._get_base_pts(self._lon, self._lat, self._azim, npts=self._n + 2)
 
         for i, (lon, lat, ang) in enumerate(zip(pts.lons, pts.lats, angs)):
-            if i % self._label_props["every"] != 0:
+            if i not in self._every:
                 continue
 
             if i == 0:
                 txt = "0"
             else:
                 txt = self._get_txt(i)
 
@@ -666,912 +1232,379 @@
                     xy,
                     txt,
                     size=self._label_props["scale"] * d / 2,
                     prop=self._font_props,
                 ),
                 lw=0,
             )
+
+            self._texts[f"text_{i}"] = txt
             self._artists[f"text_{i}"].set_path(tp.get_path())
             self._artists[f"text_{i}"].set_transform(
                 Affine2D().rotate_around(
                     *xy, ang + np.pi / 2 + np.deg2rad(self._label_props["rotation"])
                 )
                 + self._m.ax.transData
             )
+
+        # do this to allow using every as key for the lru_cache
+        if isinstance(self._label_props["every"], int):
+            hashable_every = self._label_props["every"]
+        else:
+            hashable_every = frozenset(self._label_props["every"])
+
         self._get_maxw(
-            self._scale_props["scale"],
-            self._scale_props["n"],
+            self._current_scale,
+            self._n,
             self._label_props["scale"],
             self._label_props["rotation"],
-            self._label_props["every"],
+            hashable_every,
         )
 
-    def _add_scalebar(self, lon, lat, azim):
+    def _add_scalebar(self, pos, azim, pickable=True):
 
         assert (
             self._artists["scale"] is None
         ), "EOmaps: there is already a scalebar present!"
 
-        # do this to make sure that the ax-transformations work as expected
-        self._m.BM.update(blit=False)
+        # we need to make sure that the figure has been drawn to ensure that the
+        # ax-transformations work as expected
+        # TODO is there a way to omit this?
+        self._m.f.canvas.draw()
+
+        if pos is None:
+            lon, lat = self._get_autopos(self._auto_position)
+        else:
+            # don't auto-reposition if lon/lat has been provided
+            lon, lat = pos
+            self._auto_position = False
 
         self._lon = lon
         self._lat = lat
         self._azim = azim
 
-        if self._scale_props["scale"] is None:
+        if self._scale is None:
             self._estimate_scale()
 
         pts = self._get_pts(lon, lat, azim)
         d = self._get_d()
         ang = self._get_ang(pts[0][0], pts[0][1])
 
         # -------------- add the labels
         self._set_minitxt(d, pts)
 
         # -------------- add the patch
         self._get_maxw(
-            self._scale_props["scale"],
-            self._scale_props["n"],
+            self._current_scale,
+            self._n,
             self._label_props["scale"],
             self._label_props["rotation"],
             self._label_props["every"],
         )
 
         verts = self._get_patch_verts(pts, lon, lat, ang, d)
-        p = PolyCollection([verts], **self._patch_props)
+        p = Polygon(verts, **self._patch_props)
         self._artists["patch"] = self._m.ax.add_artist(p)
 
+        # -------------- add lines between text and scale
+        line_verts = self._get_line_verts(pts, lon, lat, self._azim, d)
+        lc = LineCollection(line_verts, **self._line_props)
+        self._artists["patch_lines"] = self._m.ax.add_artist(lc)
+        self._m.BM.add_artist(self._artists["patch_lines"], layer=self._layer)
+
         # -------------- add the scalebar
         coll = LineCollection(pts)
+
+        color_names = self._get_scale_color_names()
         colors = np.tile(
-            self._scale_props["colors"],
-            int(np.ceil(len(pts) / len(self._scale_props["colors"]))),
+            color_names,
+            int(np.ceil(len(pts) / len(color_names))),
         )[: len(pts)]
         coll.set_colors(colors)
         coll.set_linewidth(self._scale_props["width"])
         self._artists["scale"] = self._m.ax.add_collection(coll, autolim=False)
 
         # -------------- make all artists animated
         self._artists["scale"].set_zorder(1)
         self._artists["patch"].set_zorder(0)
 
-        self._m.BM.add_artist(self._artists["scale"], layer=self.layer)
-        # self._m.BM.add_artist(self._artists["text"])
-        self._m.BM.add_artist(self._artists["patch"], layer=self.layer)
-
-        self._m.BM.update(artists=self._artists.values())
-        # make sure to update the artists on zoom
-        self._decorate_zooms()
-
-    def set_position(self, lon=None, lat=None, azim=None, update=False):
-        """
-        Set the position of the colorbar.
-
-        Parameters
-        ----------
-        lon : float, optional
-            The longitude of the starting-point. The default is None.
-        lat : float, optional
-            The latitude of the starting point. The default is None.
-        azim : float, optional
-            The azimuth-direction in which to calculate the intermediate
-            points for the scalebar. The default is None.
-        update : bool
-            Indicator if the plot should be immediately updated (True) or at the next
-            event (False). The default is False.
-
-        """
-        if lon is None:
-            lon = self._lon
-        if lat is None:
-            lat = self._lat
-        if azim is None:
-            azim = self._azim
-
-        self._lon = lon
-        self._lat = lat
-        self._azim = azim
-        pts = self._get_pts(lon, lat, azim)
-        d = self._get_d()
-        ang = self._get_ang(pts[0][0], pts[0][1])
-
-        # do this after setting _lon, _lat and _azim !
-        # and BEFORE all other changes since we need the size of the text-patches!
-        self._update_minitxt(d, pts)
-
-        # don't use first and last scale (they are just used as placeholders)
-        self._artists["scale"].set_verts(pts)
-        colors = np.tile(
-            self._scale_props["colors"],
-            int(np.ceil(len(pts) / len(self._scale_props["colors"]))),
-        )[: len(pts)]
-        self._artists["scale"].set_colors(colors)
-
-        verts = self._get_patch_verts(pts, lon, lat, ang, d)
-
-        # TODO check how to deal with invalid vertices!!
-        # print(np.all(np.isfinite(self._m._transf_plot_to_lonlat.transform(*verts.T))))
-
-        # verts = np.ma.masked_invalid(verts)
+        self._m.BM.add_artist(self._artists["scale"], layer=self._layer)
+        self._m.BM.add_artist(self._artists["patch"], layer=self._layer)
 
-        self._artists["patch"].set_verts([verts])
-        self._artists["patch"].update(self._patch_props)
-
-        if self._picker_name:
-            if self._m.cb.pick[self._picker_name].is_picked:
-                self._artists["patch"].set_edgecolor("r")
-                self._artists["patch"].set_linewidth(2)
-                self._artists["patch"].set_linestyle("-")
-
-        if update:
-            self._m.BM.update()
+        # update scalebar props whenever new backgrounds are fetched
+        # (e.g. to take care of updates on pan/zoom/resize)
+        self._m.BM._before_fetch_bg_actions.append(self._update)
+
+        if pickable is True:
+            self._make_pickable()
+
+    def _get_scale_color_names(self):
+        colors = []
+        for i in self._scale_props["colors"]:
+            if isinstance(i, tuple):
+                colors.append(to_hex(i, keep_alpha=True))
+            else:
+                colors.append(i)
+        return colors
 
     def _make_pickable(self):
-        """
-        Add callbacks to adjust the scalebar position manually.
-
-            - <LEFT>-click on the scalebar with the mouse to pick it up
-                - hold down <LEFT> to drag the scalebar
-            - use "+" and "-" keys to rotate the colorbar
-            - <RIGHT>-click on the scalebar to detach the callbacks again
-              (e.g. make it non-interactive)
-            - use <ARROW-keys> to set the size of the patch
-
-        """
-
-        def scb_move(s, pos, **kwargs):
-            # scb_remove(self, s)
-            # s._artists["patch"].set_pickradius(150)
-            # if not s._artists["patch"].contains(self.cb.click._event)[0]:
-            #     return
-            lon, lat = self._m._transf_plot_to_lonlat.transform(*pos)
-            # don't update here... the click callback updates itself!
-            s.set_position(lon, lat, update=False)
-
-        def scb_remove(s, **kwargs):
-            if not s._m.cb.pick[s._picker_name].is_picked:
-                return
-            s.remove()
-
-        def scb_az_ud(s, up=True, **kwargs):
-            if not s._m.cb.pick[s._picker_name].is_picked:
-                return
-            s._azim += s.cb_rotate_interval if up else -s.cb_rotate_interval
-            s.set_position(update=True)
-
-        # ------------ callbacks to change frame with arrow-keys
-        def scb_patch_dim(s, udlr, add=True, **kwargs):
-            if not s._m.cb.pick[s._picker_name].is_picked:
-                return
-            o = [*s._patch_offsets]
-            o[udlr] += 0.1 if add else -0.1
-            s.set_patch_props(offsets=o)
-
-        # ------------ callbacks to change the text offset with alt +-
-        def scb_txt_offset(s, add=True, **kwargs):
-            if not s._m.cb.pick[s._picker_name].is_picked:
-                return
-
-            o = s._label_props["offset"]
-            o += s._cb_offset_interval if add else -s._cb_offset_interval
-            s.set_label_props(offset=o)
-
-        def addcbs(s, **kwargs):
-            m = s._m
-            # make sure we pick always only one scalebar
-            for i in s._existing_pickers:
-                p = getattr(m.cb, i)
-                if p.is_picked is True and p.scalebar is not s:
-                    p.scalebar._remove_callbacks()
-
-            m.cb.pick[s._picker_name].is_picked = True
-
-            if not hasattr(s, "_cid_move"):
-                s._cid_move = m.cb.click.attach(scb_move, s=s)
-
-            if not hasattr(s, "_cid_up"):
-                s._cid_up = m.cb.keypress.attach(scb_az_ud, key="+", up=True, s=s)
-            if not hasattr(s, "_cid_down"):
-                s._cid_down = m.cb.keypress.attach(scb_az_ud, key="-", up=False, s=s)
-
-            if not hasattr(s, "_cid_txt_offset_up"):
-                s._cid_txt_offset_up = m.cb.keypress.attach(
-                    scb_txt_offset, key="alt++", add=True, s=s
-                )
-            if not hasattr(s, "_cid_txt_offset_down"):
-                s._cid_txt_offset_down = m.cb.keypress.attach(
-                    scb_txt_offset, key="alt+-", add=False, s=s
-                )
-
-            for key, udlr in zip(["up", "down", "left", "right"], range(4)):
-                if not hasattr(s, f"_cid_patch_dim_{key}_0"):
-                    setattr(
-                        s,
-                        f"_cid_patch_dim_{key}_0",
-                        m.cb.keypress.attach(
-                            scb_patch_dim, key=key, udlr=udlr, add=True, s=s
-                        ),
-                    )
-                if not hasattr(s, f"_cid_patch_dim_{key}_1"):
-                    setattr(
-                        s,
-                        f"_cid_patch_dim_{key}_1",
-                        m.cb.keypress.attach(
-                            scb_patch_dim, key="alt+" + key, udlr=udlr, add=False, s=s
-                        ),
-                    )
-
-            if not hasattr(s, "_cid_remove"):
-                s._cid_remove = m.cb.keypress.attach(scb_remove, key="delete", s=s)
-
-        def scb_unpick(s, **kwargs):
-            s._remove_callbacks()
-
-        self._picker_name = f"_scalebar{len(self._existing_pickers)}"
-
-        self._m.cb.add_picker(self._picker_name, self._artists["patch"], True)
-        self._cid_pick = self._m.cb.pick[self._picker_name].attach(addcbs, s=self)
-        # remove all callbacks (except the pick-callback) on right-click
-        self._cid_remove_cbs = self._m.cb.click.attach(
-            scb_unpick, s=self, button=1, double_click="release"
-        )
-
-        self._m.cb.pick[self._picker_name].scalebar = self
-        self._m.cb.pick[self._picker_name].is_picked = False
-
-    @property
-    def _existing_pickers(self):
-        return [i for i in self._m.cb.__dict__ if i.startswith("_pick__scalebar")]
-
-    def _remove_callbacks(self, **kwargs):
-        if hasattr(self, "_cid_move"):
-            self._m.cb.click.remove(self._cid_move)
-            del self._cid_move
-
-        if hasattr(self, "_cid_up"):
-            self._m.cb.keypress.remove(self._cid_up)
-            del self._cid_up
-        if hasattr(self, "_cid_down"):
-            self._m.cb.keypress.remove(self._cid_down)
-            del self._cid_down
-
-        if hasattr(self, "_cid_txt_up"):
-            self._m.cb.keypress.remove(self._cid_txt_up)
-            del self._cid_down
-        if hasattr(self, "_cid_txt_down"):
-            self._m.cb.keypress.remove(self._cid_txt_down)
-            del self._cid_down
-
-        self._m.cb.pick[self._picker_name].is_picked = False
-
-        self.set_position()
-
-    def _decorate_zooms(self):
-        toolbar = self._m.f.canvas.toolbar
-
-        if toolbar is not None:
-            toolbar.release_zoom = self._zoom_decorator(toolbar.release_zoom)
-            toolbar.release_pan = self._zoom_decorator(toolbar.release_pan)
-            toolbar._update_view = self._update_decorator(toolbar._update_view)
-
-    def _zoom_decorator(self, f):
-        def newzoom(event):
-            ret = f(event)
-
-            # clear the cache to re-evaluate the text-width
-            self.__class__._get_maxw.cache_clear()
-            if self._autoscale is not None:
-                prev_scale = self._scale_props["scale"]
-                try:
-                    self._estimate_scale()
-                except Exception:
-                    self._scale_props["scale"] = prev_scale
-            if self._auto_position:
-                self.auto_position(self._auto_position)
-
-            self.set_position()
-            self._m.BM.update()
-            return ret
-
-        return newzoom
-
-    def _update_decorator(self, f):
-        def newupdate():
-            # clear the cache to re-evaluate the text-width
-            ret = f()
-            self.__class__._get_maxw.cache_clear()
-            if self._autoscale is not None:
-                prev_scale = self._scale_props["scale"]
-                try:
-                    self._estimate_scale()
-                except Exception:
-                    self._scale_props["scale"] = prev_scale
-
-            if self._auto_position:
-                self.auto_position(self._auto_position)
-
-            self.set_position()
-            self._m.BM.update()
-
-            return ret
-
-        return newupdate
-
-    def get_position(self):
-        """
-        Return the current position (and orientation) of the scalebar.
-
-        Returns
-        -------
-        list
-            a list corresponding to [longitude, latitude, azimuth].
-        """
-        return [self._lon, self._lat, self._azim]
-
-    def remove(self):
-        """Remove the scalebar from the map."""
-        self._remove_callbacks()
-        for a in self._artists.values():
-            self._m.BM.remove_artist(a)
-            a.remove()
-
-        self._m.BM.update()
-
-
-class Compass:
-    """Base class for EOmaps compass objects."""
-
-    def __init__(self, m):
-        self._m = m
-
-        self._scale = 10
-        self._style = "north arrow"
-        self._patch = False
-        self._txt = "N"
-
-    def __call__(
-        self,
-        pos=None,
-        pos_transform="axes",
-        scale=10,
-        style="compass",
-        patch=None,
-        txt="N",
-        pickable=True,
-        layer=None,
-        ignore_invalid_angles=False,
-    ):
-        """
-        Add a "compass" or "north-arrow" to the map.
-
-        Note
-        ----
-        You can use the mouse to pick the compass and move it anywhere on the map.
-        (the directions are dynamically updated if you pan/zoom or pick the compass)
-
-        - If you press the "delete" key while clicking on the compass, it is removed.
-          (same as calling `compass.remove()`)
-        - If you press the "d" key while clicking on the compass, it will be
-          disconnected from pick-events (same as calling `compass.set_pickable(False)`)
-
-
-        Parameters
-        ----------
-        pos : tuple or None, optional
-            The initial position of the compass with respect to the transformation
-            defined as "pos_transform".
-            Note that you can also move the compass with the mouse!
-        pos_transform : string, optional
-            Indicator in what coordinate-system the initial position is provided.
-
-            - "axes": relative axis-coordinates in the range (0-1)
-            - "lonlat": coordinates provided as (longitude, latitude)
-            - "plot_crs": coordinates provided in the crs used for plotting.
-
-            The default is "axes".
-        scale : float, optional
-            A scale-factor for the size of the compass. The default is 10.
-        style : str, optional
-
-            - "north arrow" : draw only a north-arrow
-            - "compass": draw a compass with arrows in all 4 directions
-
-            The default is "compass".
-        patch : False, str or tuple, optional
-            The color of the background-patch.
-            (can be any color specification supported by matplotlib)
-            The default is "w".
-        txt : str, optional
-            Indicator which directions should be indicated.
-            - "NESW" : add letters for all 4 directions
-            - "NE" : add only letters for North and East (same for other combinations)
-            - None : don't add any letters
-            The default is "N".
-        pickable : bool, optional
-            Indicator if the compass should be static (False) or if it can be dragged
-            with the mouse (True). The default is True
-        layer : str, optional
-            The layer to put the compass on. The default is "all".
-        ignore_invalid_angles : bool, optional
-            - If True the compass will always (silently) use the last valid rotation-angle
-              in case the correct angle could not be determined.
-            - If False, a warning will be issued in case the angle could
-              not be determined, and a red border will be drawn around the compass to
-              indicate that it might not point in the right direction.
-
-            The default is False
-
-        Returns
-        -------
-        compass : eomaps.Compass
-            A compass-object that can be used to manually adjust the style and position
-            of the compass or remove it from the map.
-
-        """
-        if layer is None:
-            layer = self._m.layer
-        self.layer = layer
-
-        self._ignore_invalid_angles = ignore_invalid_angles
-        # self._m.BM.update()
+        if self._pickable is True:
+            return
 
-        ax2data = self._m.ax.transAxes + self._m.ax.transData.inverted()
+        self._picked = False
+        self._pick_drag = False
 
-        if pos is None:
-            pos = ax2data.transform((0.5, 0.5))
-        else:
-            if pos_transform == "axes":
-                pos = ax2data.transform(pos)
-            elif pos_transform == "lonlat":
-                pos = self._m._transf_lonlat_to_plot.transform(*pos)
-            elif pos_transform == "plot_crs":
-                pass
-            else:
-                raise TypeError(
-                    f"EOmaps: {pos_transform} is not a valid 'pos_transform'."
-                    "Use one of ('axes', 'lonlat', 'plot_crs')"
-                )
+        self._artists["patch"].set_picker(True)
 
-        self._style = style
-        self._patch = patch
-        self._txt = txt
-        self._scale = scale
-        # remember the dpi at the time the compass was initialized
-        self._init_dpi = self._m.f.dpi
+        # if not hasattr(self, "_cid_PICK"):
+        if getattr(self, "_cid_PICK", None) is None:
+            self._cid_PICK = self._m.f.canvas.mpl_connect("pick_event", self._cb_pick)
 
-        self._ang = 0
-        # remember last used rotation angle for out-of-axes compass
-        self._last_ang = 999
-
-        self._artist = self._get_artist(pos)
-        self._m.ax.add_artist(self._artist)
-        self._m.BM.add_artist(self._artist, layer=self.layer)
-
-        self._set_position(pos)
-
-        if pickable:
-            if not self._artist.pickable():
-                self._artist.set_picker(True)
-
-        self._got_artist = True
-        self._canvas = self._artist.figure.canvas
-        self._cids = [
-            self._canvas.mpl_connect("pick_event", self._on_pick),
-            self._canvas.mpl_connect("button_release_event", self._on_release),
-            self._canvas.mpl_connect("scroll_event", self._on_scroll),
-        ]
-
-        if self._update_offset not in self._m.BM._before_fetch_bg_actions:
-            self._m.BM._before_fetch_bg_actions.append(self._update_offset)
-
-    def _get_artist(self, pos):
-        if self._style == "north arrow":
-            bg_patch = PolyCollection(
-                [[[-1.5, -0.5], [-1.5, 5], [1.5, 5], [1.5, -0.5]]],
-                facecolors=[self._patch] if self._patch else ["none"],
-                edgecolors=["k"] if self._patch else ["none"],
-            )
+        self._pickable = True
 
-            verts = [
-                [[1, 0], [0, 3], [0, 0.5]],  # N w
-                [[-1, 0], [0, 3], [0, 0.5]],  # N b
-            ]
-            arrow = PolyCollection(
-                verts,
-                facecolors=["w", "k"],
-                edgecolors=["k"],
-            )
-        elif self._style == "compass":
-            c = CirclePolygon((0, 0)).get_path().vertices
+    def _undo_pickable(self):
+        if not self._pickable:
+            return
 
-            bg_patch = PolyCollection(
-                [[[-3.5, -3.5], [-3.5, 5], [3.5, 5], [3.5, -3.5]]],
-                facecolors=[self._patch] if self._patch else ["none"],
-                edgecolors=["k"] if self._patch else ["none"],
-            )
+        self._unpick()
+        self._artists["patch"].set_picker(None)
 
-            verts = [
-                [[-1, 0], [0, 3], [0, 1]],  # N b
-                [[0, 1], [3, 0], [1, 0]],  # E b
-                [[0, -3], [0, -1], [1, 0]],  # S b
-                [[-3, 0], [-1, 0], [0, -1]],  # W b
-                [[-3, 0], [0, 1], [-1, 0]],  # W w
-                [[0, 1], [0, 3], [1, 0]],  # N w
-                [[3, 0], [0, -1], [1, 0]],  # E w
-                [[0, -3], [-1, 0], [0, -1]],  # S w
-                c / 4,
-                c / 8,
-            ]
+        if getattr(self, "_cid_PICK", None) is not None:
+            self._m.f.canvas.mpl_disconnect(self._cb_pick)
+            self._cid_PICK = None
+
+        self._pickable = False
+
+    def _unpick(self):
+        global _picked_scalebars
+
+        if self._picked:
+            self._picked = False
+            self._pick_drag = False
+            self._remove_cbs()
+            if self in _picked_scalebars:
+                _picked_scalebars.remove(self)
+
+    def _cb_pick(self, event):
+        global _picked_scalebars
+
+        if event.mouseevent.button == 1:
+            if event.artist is self._artists["patch"]:
+                # unpick all other scalebars to make sure overlapping scalebars
+                # are not picked together
+                while len(_picked_scalebars) > 0:
+                    s = _picked_scalebars.pop()
+                    s._unpick()
+                    s._update()
+
+                self._picked = True
+                self._add_cbs()
+                # forward mouseevent to start dragging if button remains pressed
+                self._cb_click(event.mouseevent)
+                _picked_scalebars.add(self)
+                self._update(BM_update=True)
+
+    def _cb_click(self, event):
+        if (
+            self._picked
+            and event.button == 1
+            and self._artists["patch"].contains(event)[0]
+        ):
+            # TODO
+            # if self._auto_position is False:
+            #     print("The position of this scalebar is fixed!")
+            #     return
 
-            arrow = PolyCollection(
-                verts,
-                facecolors=["k"] * 4 + ["w"] * 4 + [".5", "w"],
-                edgecolors=["k"],
+            self._pick_drag = True
+            # get the offset_position of the click with respect to the
+            # reference point of the scalebar
+            lon0, lat0 = self._m._transf_plot_to_lonlat.transform(
+                event.xdata, event.ydata
             )
-        else:
-            raise AssertionError("EOmaps: {style} is not a valid compass-style.")
-
-        art = AuxTransformBox(self._get_transform(pos))
-        art.add_artist(bg_patch)
-        art.add_artist(arrow)
-
-        for t in self._txt:
-            if t == "N":
-                txt = PathPatch(TextPath((-0.75, 3.2), "N", size=2), fc="k", ec="none")
-                art.add_artist(txt)
-            elif self._style == "compass":
-                if t == "E":
-                    txt = PathPatch(
-                        TextPath((3.3, -0.75), "E", size=2), fc="k", ec="none"
-                    )
-                    art.add_artist(txt)
-                elif t == "S":
-                    txt = PathPatch(
-                        TextPath((-0.75, -4.7), "S", size=2), fc="k", ec="none"
-                    )
-                    art.add_artist(txt)
-                elif t == "W":
-                    txt = PathPatch(
-                        TextPath((-5.2, -0.75), "W", size=2), fc="k", ec="none"
-                    )
-                    art.add_artist(txt)
+            self._pick_start_offset = self._lon - lon0, self._lat - lat0
 
-        return art
-
-    def _update_offset(self, x=None, y=None, *args, **kwargs):
-        # reset to the center of the axis if both are None
-        try:
-            if x is None or y is None:
-                try:
-                    self._set_position(self._pos)
-                    return
-                except Exception:
-                    x, y = 0.9, 0.1
-                    self._set_position((x, y), "axis")
-                    return
-
-            self._set_position((x, y), "data")
-        except Exception:
+        elif event.button in ["up", "down"]:
+            # pass scroll events that happen on top of the scalebar
+            # (they are handled explicitly in "cb_scroll" )
             pass
+        elif self._picked:
+            self._unpick()
+            self._update(BM_update=True)
 
-    def _get_transform(self, pos):
+    def _cb_move(self, event):
+        if not self._picked or not self._pick_drag:
+            return
 
-        lon, lat = self._m._transf_plot_to_lonlat.transform(*pos)
-        x, y = self._m._transf_lonlat_to_plot.transform([lon, lon], [lat, lat + 0.01])
+        if event.button != 1:
+            return
 
+        ox, oy = self._pick_start_offset
         try:
-            ang = -np.arctan2(x[1] - x[0], y[1] - y[0])
+            lon, lat = self._m._transf_plot_to_lonlat.transform(
+                event.xdata, event.ydata
+            )
         except Exception:
-            print("EOmaps: could not add scalebar at the desired location")
+            print("EOmaps: Unable to position scalebar.")
             return
 
-        if np.isnan(ang):
-            if not self._ignore_invalid_angles:
-                if self._last_ang != self._ang:
-                    print(
-                        "EOmaps: Compass rotation-angle could not be determined! "
-                        f"... using last found angle: {np.rad2deg(self._ang):.2f}"
-                    )
-                    patch = self._artist.get_children()[0]
-                    self._patch_ec = patch.get_edgecolor()
-                    patch.set_edgecolor("r")
+        self._update(lon=lon + ox, lat=lat + oy, BM_update=True)
 
-                self._last_ang = self._ang
-            else:
-                if hasattr(self, "_patch_ec"):
-                    self._artist.get_children()[0].set_edgecolor(self._patch_ec)
-                    del self._patch_ec
-                self._last_ang = 9999
-
-            ang = self._ang
-        else:
-            if hasattr(self, "_patch_ec"):
-                self._artist.get_children()[0].set_edgecolor(self._patch_ec)
-                del self._patch_ec
-
-            self._last_ang = 9999
-
-        self._ang = ang
-        r = transforms.Affine2D().rotate(ang)
-        # apply the scale-factor with respect to the current figure dpi to keep the
-        # relative size of the north-arrow on dpi-changes!
-        s = transforms.Affine2D().scale(self._scale * self._m.f.dpi / self._init_dpi)
-        t = transforms.Affine2D().translate(*self._m.ax.transData.transform(pos))
-        trans = r + s + t
-        return trans
-
-    def _on_motion(self, evt):
-        if not self._layer_visible:
+    def _cb_scroll(self, event):
+        if not self._picked:
             return
 
-        if self._check_still_parented() and self._got_artist:
-            x, y = evt.xdata, evt.ydata
-
-            # transform values if axes is put outside the figure
-            if evt.inaxes is None:
-                x, y = self._m.ax.transData.inverted().transform((evt.x, evt.y))
-            elif evt.inaxes != self._m.ax:
-                # don't allow moving the compass on top of another axes
-                # (somehow pick-events do not fire if compass is in another axes)
-                # TODO check this!
-                return
-
-            # continue values outside of the crs-domain
-            if x is None or y is None:
-                x, y = self._m.ax.transData.inverted().transform((evt.x, evt.y))
-
-            self._update_offset(x, y)
-            self._m.BM.update(artists=[self._artist])
+        if event.key == "control":
+            self._size_factor = max(
+                0.01, self._size_factor + event.step / self._size_factor_base
+            )
+        elif event.key == "r":
+            self._azim += event.step * self._cb_rotate_interval
+        else:
 
-    def _on_scroll(self, event):
-        if not self._layer_visible:
-            return
+            if event.key == "shift":
+                multip = 5
+            else:
+                multip = 1
 
-        if self._check_still_parented() and self._got_artist:
-            self.set_scale(max(1, self._scale + event.step))
+            if self._scale is None:
+                self._autoscale = np.clip(
+                    self._autoscale + multip * event.step / self._scale_factor_base,
+                    0.01,
+                    0.99,
+                )
+            else:
+                print(
+                    "EOmaps: The scale of the scalebar is fixed! "
+                    "Use s.set_scale(None) to use autoscaling!"
+                )
 
-    def _on_pick(self, evt):
-        if not self._layer_visible:
-            return
+        self._update(BM_update=True)
 
-        if evt.mouseevent.button != 1:
+    def _cb_keypress(self, event):
+        if not self._picked:
             return
 
-        if self._check_still_parented() and evt.artist == self._artist:
-            self._got_artist = True
-            self._c1 = self._canvas.mpl_connect("motion_notify_event", self._on_motion)
-            self._c2 = self._canvas.mpl_connect("key_press_event", self._on_keypress)
-
-    def _on_keypress(self, event):
-        if not self._layer_visible:
-            return
+        key = event.key
+        udlr = ["left", "right", "down", "up"]
 
         if event.key == "delete":
             self.remove()
-        if event.key == "d":
-            self._on_release(None)
-            self.set_pickable(False)
-
-    def _on_release(self, event):
-        if not self._layer_visible:
             return
 
-        if self._check_still_parented() and self._got_artist:
-            self._finalize_offset()
-            self._got_artist = False
-            try:
-                c1 = self._c1
-            except AttributeError:
-                pass
-            else:
-                self._canvas.mpl_disconnect(c1)
+        # rotate
+        if key == "+":
+            self._azim += self._cb_rotate_interval
+        elif key == "-":
+            self._azim -= self._cb_rotate_interval
+        # set text offset
+        elif key == "ctrl+right":
+            o = self._label_props["offset"]
+            o += self._cb_offset_interval
+            self._set_label_props(offset=o)
+        elif key == "ctrl+left":
+            o = self._label_props["offset"]
+            o -= self._cb_offset_interval
+            self._set_label_props(offset=o)
+        # set text rotation
+        elif key == "ctrl+up":
+            o = self._label_props["rotation"]
+            o += self._cb_rotate_interval
+            self._set_label_props(rotation=o)
+        elif key == "ctrl+down":
+            o = self._label_props["rotation"]
+            o -= self._cb_rotate_interval
+            self._set_label_props(rotation=o)
+        # set patch offsets
+        elif key in udlr:
+            patch_offsets = [*self._patch_offsets]
+            patch_offsets[udlr.index(key)] += 0.1
+            self._set_patch_props(offsets=patch_offsets)
+        elif key in ("alt+" + i for i in udlr):
+            patch_offsets = [*self._patch_offsets]
+            patch_offsets[udlr.index(key[4:])] -= 0.1
+            self._set_patch_props(offsets=patch_offsets)
+        # unpick scalebar
+        elif event.key == "escape":
+            self._unpick()
 
-            try:
-                c2 = self._c2
-            except AttributeError:
-                pass
-            else:
-                self._canvas.mpl_disconnect(c2)
-            self._m.BM.update()
+        self._update(BM_update=True)
 
-    def _check_still_parented(self):
-        if self._artist.figure is None:
-            self._disconnect()
-            return False
-        else:
-            return True
+    def _add_cbs(self):
+        self._remove_cbs()
 
-    @property
-    def _layer_visible(self):
-        return self.layer == "all" or (
-            self.layer in (*self._m.BM.bg_layer.split("|"), self._m.BM.bg_layer)
+        self._cid_MOVE = self._m.f.canvas.mpl_connect(
+            "motion_notify_event", self._cb_move
+        )
+        self._cid_SCROLL = self._m.f.canvas.mpl_connect("scroll_event", self._cb_scroll)
+        self._cid_CLICK = self._m.f.canvas.mpl_connect(
+            "button_press_event", self._cb_click
+        )
+        self._cid_KEYPRESS = self._m.f.canvas.mpl_connect(
+            "key_press_event", self._cb_keypress
         )
 
-    def _disconnect(self):
-        """Disconnect the callbacks."""
-        for cid in self._cids:
-            self._canvas.mpl_disconnect(cid)
+    def _remove_cbs(self):
+        for cidname in (
+            "_cid_MOVE",
+            "_cid_SCROLL",
+            "_cid_CLICK",
+            "_cid_KEYPRESS",
+        ):
+            cid = getattr(self, cidname, None)
+            if cid is not None:
+                self._m.f.canvas.mpl_disconnect(cid)
+                setattr(self, cidname, None)
+
+    def _update(self, lon=None, lat=None, azim=None, BM_update=False, **kwargs):
+        # check if the scalebar is in the current field-of-view
+        # if not, avoid updating it and make it invisible
+        if self._auto_position is False:
+            bbox = self._artists["patch"].get_extents()
+            if not self._m.ax.bbox.overlaps(bbox):
+                for a in self._artists.values():
+                    a.set_visible(False)
+                return
+            else:
+                for a in self._artists.values():
+                    a.set_visible(True)
 
-        if self._update_offset in self._m.BM._before_fetch_bg_actions:
-            self._m.BM._before_fetch_bg_actions.append(self._update_offset)
+        # clear the cache to re-evaluate the text-width if label props have changed
+        self.__class__._get_maxw.cache_clear()
 
-        try:
-            c1 = self._c1
-        except AttributeError:
-            pass
-        else:
-            self._canvas.mpl_disconnect(c1)
+        if self._scale is None:
+            prev_scale = self._scale
+            try:
+                self._estimate_scale()
+            except Exception:
+                self._scale = prev_scale
 
-        try:
-            c2 = self._c2
-        except AttributeError:
-            pass
+        # make sure scalebars are not positioned out of bounds
+        if lon is not None and lat is not None:
+            lon = np.clip(lon, -179, 179)
+            lat = np.clip(lat, -89, 89)
+
+        if self._auto_position is not False:
+            if lon is not None and lat is not None:
+                self._auto_position = self._get_pos_as_autopos(lon, lat)
+            self._set_auto_position(self._auto_position)
         else:
-            self._canvas.mpl_disconnect(c2)
+            self._set_position(lon=lon, lat=lat, azim=azim)
 
-    def _finalize_offset(self):
-        pass
+        if BM_update:
+            # note: when using this function as before_fetch_bg action, updates
+            # would cause a recursion!
+            self._m.BM.update()
 
     def remove(self):
-        """
-        Remove the compass from the map.
-
-        Note
-        ----
-        You can also remove a compass by clicking on it and pressing the "delete"
-        button on the keyboard (while holding down the mouse-button)
-
-        """
-        self._disconnect()
-        self._m.BM.remove_artist(self._artist)
-        self._artist.remove()
-        self._m.BM.update()
-
-    def set_patch(self, facecolor=None, edgecolor=None, linewidth=None):
-        """
-        Set the style of the background patch.
-
-        Parameters
-        ----------
-        facecolor, edgecolor : str, tuple, None or False
-            - str or tuple: Set the color of the background patch.
-            - False or "none": Make the background-patch invisible.
-        linewidth: float
-            The linewidth of the patch.
-
-        """
-        if facecolor is False:
-            facecolor = "none"
-        if edgecolor is False:
-            edgecolor = "none"
-
-        if facecolor is not None:
-            self._artist.get_children()[0].set_facecolor(facecolor)
-        if edgecolor is not None:
-            self._artist.get_children()[0].set_edgecolor(edgecolor)
-        if linewidth is not None:
-            assert isinstance(
-                linewidth, (int, float, np.number)
-            ), "EOmaps: linewidth must be int or float!"
-            self._artist.get_children()[0].set_linewidth(linewidth)
-
-    def set_scale(self, scale):
-        """
-        Set the size scale-factor of the compass. (The default is 10).
-
-        Parameters
-        ----------
-        s : float
-            The size of the compass.
-
-        """
-        self._scale = scale
-        self._update_offset(*self._pos)
-
-    def set_pickable(self, b):
-        """
-        Set if the compass can be picked with the mouse or not.
-
-        Parameters
-        ----------
-        b : bool
-            True : enable picking
-            False : disable picking
-        """
-        if b is False:
-            b = None
-        self._artist.set_picker(b)
-
-    def _set_position(self, pos, coords="data"):
-        # Avoid calling BM.update() in here! It results in infinite
-        # recursions on zoom events because the position of the scalebar is
-        # dynamically updated on each re-fetch of the background!
-
-        if coords == "axis":
-            self._ax2data = self._m.ax.transAxes + self._m.ax.transData.inverted()
-            pos = self._ax2data.transform(pos)
-
-        trans = self._get_transform(pos)
-        for c in self._artist.get_children():
-            c.set_transform(trans)
-        self._pos = pos
-
-    def set_position(self, pos, coords="data"):
-        """
-        Set the position of the compass.
-
-        Parameters
-        ----------
-        pos : tuple
-            The (x, y) coordinates.
-        coords : str, optional
-            Indicator how the coordinates are provided
-
-            - "data" : pos represents coordinates in the plot-crs
-            - "axis" : pos represents relative [0-1] coordinates with respect to the
-              axis (e.g. (0, 0) = lower left corner, (1, 1) = upper right corner).
-
-            The default is "data".
-        """
-        self._set_position(pos, coords="data")
-        self._m.BM.update(artists=[self._artist])
-
-    def get_position(self, coords="data"):
-        """
-        Return the current position of the compass.
-
-        Parameters
-        ----------
-        coords : str, optional
-            Define what coordinates are returned
-
-            - "data" : coordinates in the plot-crs
-            - "axis": relative [0-1] coordinates with respect to the
-              axis (e.g. (0, 0) = lower left corner, (1, 1) = upper right corner)
-
-            The default is "data".
-
-        Returns
-        -------
-        pos
-            a tuple (x, y) representing the current location of the compass.
-
-        """
-        self._ax2data = self._m.ax.transAxes + self._m.ax.transData.inverted()
-
-        if coords == "axis":
-            return self._ax2data.inverted().transform(self._pos)
-        elif coords == "data":
-            return self._pos
-        else:
-            raise TypeError("EOmaps: 'coords' must be one of ['data', 'axis']!")
-
-    def get_scale(self):
-        """
-        Return the current size scale-factor of the compass.
-
-        Returns
-        -------
-        s : float
-            The size of the compass.
-
-        """
-        return self._scale
+        """Remove the scalebar from the map."""
+        self._unpick()
+        for a in self._artists.values():
+            self._m.BM.remove_artist(a)
+            a.remove()
 
-    def set_ignore_invalid_angles(self, val):
-        """
-        Set how to deal with invalid rotation-angles.
+        # remove trigger to update scalebar properties on fetch_bg
+        if self._update in self._m.BM._before_fetch_bg_actions:
+            self._m.BM._before_fetch_bg_actions.remove(self._update)
 
-        - If True the compass will always (silently) use the last valid rotation-angle
-          in case the correct angle could not be determined.
-        - If False (the default), a warning will be issued in case the angle could
-          not be determined, and a red border will be drawn around the compass to
-          indicate that it might not point in the right direction.
+        self._renderer = None
 
-        Parameters
-        ----------
-        val : bool
-            ignore invalid rotation angles.
-        """
-        self._ignore_invalid_angles = val
-        self.set_position(self._pos)
+        self._m.BM.update()
```

### Comparing `EOmaps-6.3/eomaps/utilities.py` & `EOmaps-6.4/eomaps/utilities.py`

 * *Files identical despite different names*

### Comparing `EOmaps-6.3/setup.py` & `EOmaps-6.4/setup.py`

 * *Files identical despite different names*

