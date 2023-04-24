# Comparing `tmp/pyautosrt-0.1.7.tar.gz` & `tmp/pyautosrt-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyautosrt-0.1.7.tar", last modified: Sat Apr 15 02:11:55 2023, max compression
+gzip compressed data, was "pyautosrt-0.1.8.tar", last modified: Mon Apr 24 15:40:10 2023, max compression
```

## Comparing `pyautosrt-0.1.7.tar` & `pyautosrt-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 02:11:55.658001 pyautosrt-0.1.7/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 pyautosrt-0.1.7/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 pyautosrt-0.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0     2055 2023-04-15 02:11:55.658750 pyautosrt-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     3061 2023-02-10 19:35:06.000000 pyautosrt-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-15 02:11:55.635524 pyautosrt-0.1.7/pyautosrt/
--rw-rw-rw-   0        0        0    40142 2023-04-15 02:08:42.000000 pyautosrt-0.1.7/pyautosrt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 02:11:55.655753 pyautosrt-0.1.7/pyautosrt.egg-info/
--rw-rw-rw-   0        0        0     2055 2023-04-15 02:11:54.000000 pyautosrt-0.1.7/pyautosrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-04-15 02:11:55.000000 pyautosrt-0.1.7/pyautosrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 02:11:54.000000 pyautosrt-0.1.7/pyautosrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-04-15 02:11:54.000000 pyautosrt-0.1.7/pyautosrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      114 2023-04-15 02:11:54.000000 pyautosrt-0.1.7/pyautosrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-15 02:11:54.000000 pyautosrt-0.1.7/pyautosrt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-04-15 02:11:55.663245 pyautosrt-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1512 2023-04-15 02:08:56.000000 pyautosrt-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:40:10.932610 pyautosrt-0.1.8/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 pyautosrt-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 pyautosrt-0.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     2055 2023-04-24 15:40:10.933359 pyautosrt-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3061 2023-02-10 19:35:06.000000 pyautosrt-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 15:40:10.889905 pyautosrt-0.1.8/pyautosrt/
+-rw-rw-rw-   0        0        0    79215 2023-04-24 14:55:39.000000 pyautosrt-0.1.8/pyautosrt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:40:10.929613 pyautosrt-0.1.8/pyautosrt.egg-info/
+-rw-rw-rw-   0        0        0     2055 2023-04-24 15:40:10.000000 pyautosrt-0.1.8/pyautosrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-04-24 15:40:10.000000 pyautosrt-0.1.8/pyautosrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 15:40:10.000000 pyautosrt-0.1.8/pyautosrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-04-24 15:40:10.000000 pyautosrt-0.1.8/pyautosrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       75 2023-04-24 15:40:10.000000 pyautosrt-0.1.8/pyautosrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-24 15:40:10.000000 pyautosrt-0.1.8/pyautosrt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-04-24 15:40:10.939356 pyautosrt-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1449 2023-04-24 15:03:33.000000 pyautosrt-0.1.8/setup.py
```

### Comparing `pyautosrt-0.1.7/LICENSE` & `pyautosrt-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyautosrt-0.1.7/PKG-INFO` & `pyautosrt-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyautosrt
-Version: 0.1.7
+Version: 0.1.8
 Summary: pyautosrt is a python based desktop app to generate subtitle and translated subtitle file
 Home-page: https://github.com/botbahlul/pyautosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `pyautosrt-0.1.7/README.md` & `pyautosrt-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `pyautosrt-0.1.7/pyautosrt.egg-info/PKG-INFO` & `pyautosrt-0.1.8/pyautosrt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyautosrt
-Version: 0.1.7
+Version: 0.1.8
 Summary: pyautosrt is a python based desktop app to generate subtitle and translated subtitle file
 Home-page: https://github.com/botbahlul/pyautosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `pyautosrt-0.1.7/setup.py` & `pyautosrt-0.1.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     'them to a different language, and finally saves the resulting subtitles to disk.'
     'It supports  a variety of input and output languages  and can currently produce '
     'subtitles in SRT, VTT, JSON, and RAW format.'
 )
 
 setup(
     name="pyautosrt",
-    version="0.1.7",
+    version="0.1.8",
     description="pyautosrt is a python based desktop app to generate subtitle and translated subtitle file",
     long_description = long_description,
     author="Bot Bahlul",
     author_email="bot.bahlul@gmail.com",
     url="https://github.com/botbahlul/pyautosrt",
     packages=[str("pyautosrt")],
     entry_points={
@@ -30,14 +30,12 @@
             "pyautosrt = pyautosrt:main",
         ],
     },
     install_requires=[
         "requests>=2.3.0",
         "pysrt>=1.0.1",
         "six>=1.11.0",
-        "tk>=0.1.0",
         "pysimplegui>=4.60.1",
         "httpx>=0.13.3",
-        "ffmpeg_progress_yield>=0.7.2",
     ],
     license=open("LICENSE").read()
 )
```

