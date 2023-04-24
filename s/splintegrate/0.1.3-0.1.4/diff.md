# Comparing `tmp/splintegrate-0.1.3.tar.gz` & `tmp/splintegrate-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splintegrate-0.1.3.tar", last modified: Sun Nov 27 22:10:45 2022, max compression
+gzip compressed data, was "splintegrate-0.1.4.tar", last modified: Mon Apr 24 16:18:37 2023, max compression
```

## Comparing `splintegrate-0.1.3.tar` & `splintegrate-0.1.4.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-11-27 22:10:45.483737 splintegrate-0.1.3/
--rw-r--r--   0 everettschlawin   (501) staff       (20)      292 2021-03-10 23:40:10.000000 splintegrate-0.1.3/.editorconfig
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-11-27 22:10:45.479885 splintegrate-0.1.3/.github/
--rw-r--r--   0 everettschlawin   (501) staff       (20)      323 2021-03-10 23:40:10.000000 splintegrate-0.1.3/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 everettschlawin   (501) staff       (20)     1196 2021-03-10 23:40:10.000000 splintegrate-0.1.3/.gitignore
--rw-r--r--   0 everettschlawin   (501) staff       (20)      298 2021-03-10 23:40:10.000000 splintegrate-0.1.3/.travis.yml
--rw-r--r--   0 everettschlawin   (501) staff       (20)      175 2021-03-10 23:40:10.000000 splintegrate-0.1.3/AUTHORS.rst
--rw-r--r--   0 everettschlawin   (501) staff       (20)     3578 2021-03-10 23:40:10.000000 splintegrate-0.1.3/CONTRIBUTING.rst
--rw-r--r--   0 everettschlawin   (501) staff       (20)       89 2021-03-10 23:40:10.000000 splintegrate-0.1.3/HISTORY.rst
--rw-r--r--   0 everettschlawin   (501) staff       (20)     1075 2021-03-10 23:40:10.000000 splintegrate-0.1.3/LICENSE
--rw-r--r--   0 everettschlawin   (501) staff       (20)      262 2021-03-10 23:40:10.000000 splintegrate-0.1.3/MANIFEST.in
--rw-r--r--   0 everettschlawin   (501) staff       (20)     2235 2021-03-10 23:40:10.000000 splintegrate-0.1.3/Makefile
--rw-r--r--   0 everettschlawin   (501) staff       (20)     1809 2022-11-27 22:10:45.483813 splintegrate-0.1.3/PKG-INFO
--rw-r--r--   0 everettschlawin   (501) staff       (20)      913 2021-03-10 23:40:10.000000 splintegrate-0.1.3/README.rst
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-11-27 22:10:45.479984 splintegrate-0.1.3/bin/
--rwxr-xr-x   0 everettschlawin   (501) staff       (20)     1762 2022-07-16 15:35:42.000000 splintegrate-0.1.3/bin/quick_split
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-11-27 22:10:45.481091 splintegrate-0.1.3/docs/
--rw-r--r--   0 everettschlawin   (501) staff       (20)      613 2021-03-10 23:40:10.000000 splintegrate-0.1.3/docs/Makefile
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-11-27 22:10:45.478190 splintegrate-0.1.3/docs/_build/
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-11-27 22:10:45.478228 splintegrate-0.1.3/docs/_build/html/
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-11-27 22:10:45.482560 splintegrate-0.1.3/docs/_build/html/_static/
--rw-r--r--   0 everettschlawin   (501) staff       (20)      673 2019-04-02 23:09:01.000000 splintegrate-0.1.3/docs/_build/html/_static/ajax-loader.gif
--rw-r--r--   0 everettschlawin   (501) staff       (20)      756 2019-04-02 23:09:01.000000 splintegrate-0.1.3/docs/_build/html/_static/comment-bright.png
--rw-r--r--   0 everettschlawin   (501) staff       (20)      829 2019-04-02 23:09:01.000000 splintegrate-0.1.3/docs/_build/html/_static/comment-close.png
--rw-r--r--   0 everettschlawin   (501) staff       (20)      641 2019-04-02 23:09:01.000000 splintegrate-0.1.3/docs/_build/html/_static/comment.png
--rw-r--r--   0 everettschlawin   (501) staff       (20)      222 2019-04-02 23:09:01.000000 splintegrate-0.1.3/docs/_build/html/_static/down-pressed.png
--rw-r--r--   0 everettschlawin   (501) staff       (20)      202 2019-04-02 23:09:01.000000 splintegrate-0.1.3/docs/_build/html/_static/down.png
--rw-r--r--   0 everettschlawin   (501) staff       (20)      286 2020-02-10 16:38:31.000000 splintegrate-0.1.3/docs/_build/html/_static/file.png
--rw-r--r--   0 everettschlawin   (501) staff       (20)       90 2020-02-10 16:38:31.000000 splintegrate-0.1.3/docs/_build/html/_static/minus.png
--rw-r--r--   0 everettschlawin   (501) staff       (20)       90 2020-02-10 16:38:31.000000 splintegrate-0.1.3/docs/_build/html/_static/plus.png
--rw-r--r--   0 everettschlawin   (501) staff       (20)      214 2019-04-02 23:09:01.000000 splintegrate-0.1.3/docs/_build/html/_static/up-pressed.png
--rw-r--r--   0 everettschlawin   (501) staff       (20)      203 2019-04-02 23:09:01.000000 splintegrate-0.1.3/docs/_build/html/_static/up.png
--rw-r--r--   0 everettschlawin   (501) staff       (20)       28 2021-03-10 23:40:10.000000 splintegrate-0.1.3/docs/authors.rst
--rwxr-xr-x   0 everettschlawin   (501) staff       (20)     4882 2021-11-01 05:44:27.000000 splintegrate-0.1.3/docs/conf.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)       33 2021-03-10 23:40:10.000000 splintegrate-0.1.3/docs/contributing.rst
--rw-r--r--   0 everettschlawin   (501) staff       (20)       28 2021-03-10 23:40:10.000000 splintegrate-0.1.3/docs/history.rst
--rw-r--r--   0 everettschlawin   (501) staff       (20)      311 2021-03-17 05:28:54.000000 splintegrate-0.1.3/docs/index.rst
--rw-r--r--   0 everettschlawin   (501) staff       (20)     1075 2021-09-21 19:13:11.000000 splintegrate-0.1.3/docs/installation.rst
--rw-r--r--   0 everettschlawin   (501) staff       (20)      774 2021-03-10 23:40:10.000000 splintegrate-0.1.3/docs/make.bat
--rw-r--r--   0 everettschlawin   (501) staff       (20)      198 2021-11-01 05:44:52.000000 splintegrate-0.1.3/docs/modules.rst
--rw-r--r--   0 everettschlawin   (501) staff       (20)       27 2021-03-10 23:40:10.000000 splintegrate-0.1.3/docs/readme.rst
--rw-r--r--   0 everettschlawin   (501) staff       (20)      620 2021-11-27 04:44:05.000000 splintegrate-0.1.3/docs/usage.rst
--rw-r--r--   0 everettschlawin   (501) staff       (20)      134 2021-03-10 23:40:10.000000 splintegrate-0.1.3/requirements_dev.txt
--rw-r--r--   0 everettschlawin   (501) staff       (20)      395 2022-11-27 22:10:45.484114 splintegrate-0.1.3/setup.cfg
--rwxr-xr-x   0 everettschlawin   (501) staff       (20)     1462 2022-06-29 23:25:44.000000 splintegrate-0.1.3/setup.py
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-11-27 22:10:45.482757 splintegrate-0.1.3/splintegrate/
--rw-r--r--   0 everettschlawin   (501) staff       (20)      149 2022-04-15 18:41:25.000000 splintegrate-0.1.3/splintegrate/__init__.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)     9632 2022-11-01 20:37:49.000000 splintegrate-0.1.3/splintegrate/splintegrate.py
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-11-27 22:10:45.483433 splintegrate-0.1.3/splintegrate.egg-info/
--rw-r--r--   0 everettschlawin   (501) staff       (20)     1809 2022-11-27 22:10:45.000000 splintegrate-0.1.3/splintegrate.egg-info/PKG-INFO
--rw-r--r--   0 everettschlawin   (501) staff       (20)     1118 2022-11-27 22:10:45.000000 splintegrate-0.1.3/splintegrate.egg-info/SOURCES.txt
--rw-r--r--   0 everettschlawin   (501) staff       (20)        1 2022-11-27 22:10:45.000000 splintegrate-0.1.3/splintegrate.egg-info/dependency_links.txt
--rw-r--r--   0 everettschlawin   (501) staff       (20)        1 2021-03-14 00:13:09.000000 splintegrate-0.1.3/splintegrate.egg-info/not-zip-safe
--rw-r--r--   0 everettschlawin   (501) staff       (20)       15 2022-11-27 22:10:45.000000 splintegrate-0.1.3/splintegrate.egg-info/requires.txt
--rw-r--r--   0 everettschlawin   (501) staff       (20)       13 2022-11-27 22:10:45.000000 splintegrate-0.1.3/splintegrate.egg-info/top_level.txt
-drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2022-11-27 22:10:45.483636 splintegrate-0.1.3/tests/
--rw-r--r--   0 everettschlawin   (501) staff       (20)       42 2021-03-10 23:40:10.000000 splintegrate-0.1.3/tests/__init__.py
--rwxr-xr-x   0 everettschlawin   (501) staff       (20)     1788 2021-03-14 22:56:54.000000 splintegrate-0.1.3/tests/test_splintegrate.py
--rw-r--r--   0 everettschlawin   (501) staff       (20)      293 2021-03-10 23:40:10.000000 splintegrate-0.1.3/tox.ini
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:18:37.430964 splintegrate-0.1.4/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      292 2021-03-10 23:40:10.000000 splintegrate-0.1.4/.editorconfig
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:18:37.424688 splintegrate-0.1.4/.github/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      323 2021-03-10 23:40:10.000000 splintegrate-0.1.4/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     1196 2021-03-10 23:40:10.000000 splintegrate-0.1.4/.gitignore
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      298 2021-03-10 23:40:10.000000 splintegrate-0.1.4/.travis.yml
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      175 2021-03-10 23:40:10.000000 splintegrate-0.1.4/AUTHORS.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     3578 2021-03-10 23:40:10.000000 splintegrate-0.1.4/CONTRIBUTING.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)       89 2021-03-10 23:40:10.000000 splintegrate-0.1.4/HISTORY.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     1075 2021-03-10 23:40:10.000000 splintegrate-0.1.4/LICENSE
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      262 2021-03-10 23:40:10.000000 splintegrate-0.1.4/MANIFEST.in
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     2235 2021-03-10 23:40:10.000000 splintegrate-0.1.4/Makefile
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     1789 2023-04-24 16:18:37.431028 splintegrate-0.1.4/PKG-INFO
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      913 2021-03-10 23:40:10.000000 splintegrate-0.1.4/README.rst
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:18:37.424831 splintegrate-0.1.4/bin/
+-rwxr-xr-x   0 everettschlawin   (501) staff       (20)     1762 2022-07-16 15:35:42.000000 splintegrate-0.1.4/bin/quick_split
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:18:37.426800 splintegrate-0.1.4/docs/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      613 2021-03-10 23:40:10.000000 splintegrate-0.1.4/docs/Makefile
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:18:37.422031 splintegrate-0.1.4/docs/_build/
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:18:37.422079 splintegrate-0.1.4/docs/_build/html/
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:18:37.429073 splintegrate-0.1.4/docs/_build/html/_static/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      673 2019-04-02 23:09:01.000000 splintegrate-0.1.4/docs/_build/html/_static/ajax-loader.gif
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      756 2019-04-02 23:09:01.000000 splintegrate-0.1.4/docs/_build/html/_static/comment-bright.png
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      829 2019-04-02 23:09:01.000000 splintegrate-0.1.4/docs/_build/html/_static/comment-close.png
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      641 2019-04-02 23:09:01.000000 splintegrate-0.1.4/docs/_build/html/_static/comment.png
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      222 2019-04-02 23:09:01.000000 splintegrate-0.1.4/docs/_build/html/_static/down-pressed.png
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      202 2019-04-02 23:09:01.000000 splintegrate-0.1.4/docs/_build/html/_static/down.png
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      286 2020-02-10 16:38:31.000000 splintegrate-0.1.4/docs/_build/html/_static/file.png
+-rw-r--r--   0 everettschlawin   (501) staff       (20)       90 2020-02-10 16:38:31.000000 splintegrate-0.1.4/docs/_build/html/_static/minus.png
+-rw-r--r--   0 everettschlawin   (501) staff       (20)       90 2020-02-10 16:38:31.000000 splintegrate-0.1.4/docs/_build/html/_static/plus.png
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      214 2019-04-02 23:09:01.000000 splintegrate-0.1.4/docs/_build/html/_static/up-pressed.png
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      203 2019-04-02 23:09:01.000000 splintegrate-0.1.4/docs/_build/html/_static/up.png
+-rw-r--r--   0 everettschlawin   (501) staff       (20)       28 2021-03-10 23:40:10.000000 splintegrate-0.1.4/docs/authors.rst
+-rwxr-xr-x   0 everettschlawin   (501) staff       (20)     4882 2021-11-01 05:44:27.000000 splintegrate-0.1.4/docs/conf.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)       33 2021-03-10 23:40:10.000000 splintegrate-0.1.4/docs/contributing.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)       28 2021-03-10 23:40:10.000000 splintegrate-0.1.4/docs/history.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      311 2021-03-17 05:28:54.000000 splintegrate-0.1.4/docs/index.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     1075 2021-09-21 19:13:11.000000 splintegrate-0.1.4/docs/installation.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      774 2021-03-10 23:40:10.000000 splintegrate-0.1.4/docs/make.bat
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      198 2021-11-01 05:44:52.000000 splintegrate-0.1.4/docs/modules.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)       27 2021-03-10 23:40:10.000000 splintegrate-0.1.4/docs/readme.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      620 2021-11-27 04:44:05.000000 splintegrate-0.1.4/docs/usage.rst
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      134 2021-03-10 23:40:10.000000 splintegrate-0.1.4/requirements_dev.txt
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      395 2023-04-24 16:18:37.431324 splintegrate-0.1.4/setup.cfg
+-rwxr-xr-x   0 everettschlawin   (501) staff       (20)     1462 2023-04-24 16:18:31.000000 splintegrate-0.1.4/setup.py
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:18:37.429639 splintegrate-0.1.4/splintegrate/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      149 2023-04-24 16:12:37.000000 splintegrate-0.1.4/splintegrate/__init__.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     9633 2023-04-24 16:11:46.000000 splintegrate-0.1.4/splintegrate/splintegrate.py
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:18:37.430594 splintegrate-0.1.4/splintegrate.egg-info/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     1789 2023-04-24 16:18:37.000000 splintegrate-0.1.4/splintegrate.egg-info/PKG-INFO
+-rw-r--r--   0 everettschlawin   (501) staff       (20)     1118 2023-04-24 16:18:37.000000 splintegrate-0.1.4/splintegrate.egg-info/SOURCES.txt
+-rw-r--r--   0 everettschlawin   (501) staff       (20)        1 2023-04-24 16:18:37.000000 splintegrate-0.1.4/splintegrate.egg-info/dependency_links.txt
+-rw-r--r--   0 everettschlawin   (501) staff       (20)        1 2021-03-14 00:13:09.000000 splintegrate-0.1.4/splintegrate.egg-info/not-zip-safe
+-rw-r--r--   0 everettschlawin   (501) staff       (20)       15 2023-04-24 16:18:37.000000 splintegrate-0.1.4/splintegrate.egg-info/requires.txt
+-rw-r--r--   0 everettschlawin   (501) staff       (20)       13 2023-04-24 16:18:37.000000 splintegrate-0.1.4/splintegrate.egg-info/top_level.txt
+drwxr-xr-x   0 everettschlawin   (501) staff       (20)        0 2023-04-24 16:18:37.430854 splintegrate-0.1.4/tests/
+-rw-r--r--   0 everettschlawin   (501) staff       (20)       42 2021-03-10 23:40:10.000000 splintegrate-0.1.4/tests/__init__.py
+-rwxr-xr-x   0 everettschlawin   (501) staff       (20)     1788 2021-03-14 22:56:54.000000 splintegrate-0.1.4/tests/test_splintegrate.py
+-rw-r--r--   0 everettschlawin   (501) staff       (20)      293 2021-03-10 23:40:10.000000 splintegrate-0.1.4/tox.ini
```

### Comparing `splintegrate-0.1.3/.gitignore` & `splintegrate-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `splintegrate-0.1.3/CONTRIBUTING.rst` & `splintegrate-0.1.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `splintegrate-0.1.3/LICENSE` & `splintegrate-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `splintegrate-0.1.3/Makefile` & `splintegrate-0.1.4/Makefile`

 * *Files identical despite different names*

### Comparing `splintegrate-0.1.3/PKG-INFO` & `splintegrate-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: splintegrate
-Version: 0.1.3
+Version: 0.1.4
 Summary: Splintegrate splits and combines integrations up.
 Home-page: https://github.com/eas342/splintegrate
 Author: Everett Schlawin
 Author-email: granfalloontoyballoon@hotmail.com
 License: MIT license
 Keywords: splintegrate
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
@@ -64,9 +63,7 @@
 History
 =======
 
 0.1.0 (2021-03-10)
 ------------------
 
 * First release on PyPI.
-
-
```

### Comparing `splintegrate-0.1.3/README.rst` & `splintegrate-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `splintegrate-0.1.3/bin/quick_split` & `splintegrate-0.1.4/bin/quick_split`

 * *Files identical despite different names*

### Comparing `splintegrate-0.1.3/docs/Makefile` & `splintegrate-0.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `splintegrate-0.1.3/docs/_build/html/_static/ajax-loader.gif` & `splintegrate-0.1.4/docs/_build/html/_static/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `splintegrate-0.1.3/docs/_build/html/_static/comment-bright.png` & `splintegrate-0.1.4/docs/_build/html/_static/comment-bright.png`

 * *Files identical despite different names*

### Comparing `splintegrate-0.1.3/docs/_build/html/_static/comment-close.png` & `splintegrate-0.1.4/docs/_build/html/_static/comment-close.png`

 * *Files identical despite different names*

### Comparing `splintegrate-0.1.3/docs/_build/html/_static/comment.png` & `splintegrate-0.1.4/docs/_build/html/_static/comment.png`

 * *Files identical despite different names*

### Comparing `splintegrate-0.1.3/docs/conf.py` & `splintegrate-0.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `splintegrate-0.1.3/docs/installation.rst` & `splintegrate-0.1.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `splintegrate-0.1.3/docs/make.bat` & `splintegrate-0.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `splintegrate-0.1.3/docs/usage.rst` & `splintegrate-0.1.4/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `splintegrate-0.1.3/setup.py` & `splintegrate-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,10 +40,10 @@
     name='splintegrate',
     scripts=['bin/quick_split'],
     packages=find_packages(include=['splintegrate', 'splintegrate.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/eas342/splintegrate',
-    version='0.1.3',
+    version='0.1.4',
     zip_safe=False,
 )
```

### Comparing `splintegrate-0.1.3/splintegrate/splintegrate.py` & `splintegrate-0.1.4/splintegrate/splintegrate.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
             thisHeader=deepcopy(self.head)
             
             if self.flipToDet == True:
                 outDat = flip_data(_thisint,self.head,detectorName=self.detectorName)
                 thisHeader['FLIP2DET'] = (True,'Flipped to detector coordinates?')
             else:
                 outDat = _thisint
-                thisHeader['FLIP2DET'] = (True,'Flipped to detector coordinates?')
+                thisHeader['FLIP2DET'] = (False,'Flipped to detector coordinates?')
             
             tmpStr="{:05d}".format(i+self.int_start_num-1)
             outFile = "{}_I{}.fits".format(self.baseName,tmpStr)
             
             ## since we have split the ints, set nints to 1
             thisHeader['NINTS'] = 1
             thisHeader.insert("NINTS",("ON_NINT",i+self.int_start_num,"This is INT of TOT_NINT"),after=True)
```

### Comparing `splintegrate-0.1.3/splintegrate.egg-info/PKG-INFO` & `splintegrate-0.1.4/splintegrate.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: splintegrate
-Version: 0.1.3
+Version: 0.1.4
 Summary: Splintegrate splits and combines integrations up.
 Home-page: https://github.com/eas342/splintegrate
 Author: Everett Schlawin
 Author-email: granfalloontoyballoon@hotmail.com
 License: MIT license
 Keywords: splintegrate
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
@@ -64,9 +63,7 @@
 History
 =======
 
 0.1.0 (2021-03-10)
 ------------------
 
 * First release on PyPI.
-
-
```

### Comparing `splintegrate-0.1.3/splintegrate.egg-info/SOURCES.txt` & `splintegrate-0.1.4/splintegrate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `splintegrate-0.1.3/tests/test_splintegrate.py` & `splintegrate-0.1.4/tests/test_splintegrate.py`

 * *Files identical despite different names*

