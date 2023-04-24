# Comparing `tmp/Turk_game-1.0.2.tar.gz` & `tmp/Turk_game-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Turk_game-1.0.2.tar", last modified: Fri Apr 21 10:30:15 2023, max compression
+gzip compressed data, was "Turk_game-1.0.3.tar", last modified: Sat Apr 22 09:26:57 2023, max compression
```

## Comparing `Turk_game-1.0.2.tar` & `Turk_game-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 10:30:14.000000 Turk_game-1.0.2/
--rw-rw-rw-   0        0        0     1066 2019-06-03 23:39:34.000000 Turk_game-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      278 2023-04-21 10:30:16.000000 Turk_game-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2033 2019-06-03 23:39:34.000000 Turk_game-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 10:30:14.000000 Turk_game-1.0.2/Turk_game.egg-info/
--rw-rw-rw-   0        0        0      278 2023-04-21 10:30:14.000000 Turk_game-1.0.2/Turk_game.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      183 2023-04-21 10:30:14.000000 Turk_game-1.0.2/Turk_game.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 10:30:14.000000 Turk_game-1.0.2/Turk_game.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 10:30:14.000000 Turk_game-1.0.2/Turk_game.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2698 2023-04-21 10:17:56.000000 Turk_game-1.0.2/Turk_game.py
--rw-rw-rw-   0        0        0       10 2023-04-11 06:37:16.000000 Turk_game-1.0.2/__init__.py
--rw-rw-rw-   0        0        0       42 2023-04-21 10:30:16.000000 Turk_game-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      425 2023-04-21 10:30:08.000000 Turk_game-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 09:26:56.000000 Turk_game-1.0.3/
+-rw-rw-rw-   0        0        0     1066 2019-06-03 23:39:34.000000 Turk_game-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0      298 2023-04-22 09:26:58.000000 Turk_game-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2033 2019-06-03 23:39:34.000000 Turk_game-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 09:26:56.000000 Turk_game-1.0.3/Turk_game.egg-info/
+-rw-rw-rw-   0        0        0      298 2023-04-22 09:26:54.000000 Turk_game-1.0.3/Turk_game.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      183 2023-04-22 09:26:56.000000 Turk_game-1.0.3/Turk_game.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 09:26:54.000000 Turk_game-1.0.3/Turk_game.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 09:26:54.000000 Turk_game-1.0.3/Turk_game.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2709 2023-04-22 09:25:14.000000 Turk_game-1.0.3/Turk_game.py
+-rw-rw-rw-   0        0        0       10 2023-04-11 06:37:16.000000 Turk_game-1.0.3/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-04-22 09:26:58.000000 Turk_game-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      468 2023-04-22 09:26:38.000000 Turk_game-1.0.3/setup.py
```

### Comparing `Turk_game-1.0.2/LICENSE` & `Turk_game-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Turk_game-1.0.2/README.md` & `Turk_game-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `Turk_game-1.0.2/Turk_game.py` & `Turk_game-1.0.3/Turk_game.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pygame as pg
 import threading as th
 import keyboard as ky
-import sys, os , time
+import sys, os , time , random
+
 
 def bekle(sure):
     time.sleep(sure)
 
 def basildi(tus:str):
     return ky.is_pressed(tus)
```

