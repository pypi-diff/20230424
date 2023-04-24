# Comparing `tmp/vue2img-0.0.1.tar.gz` & `tmp/vue2img-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vue2img-0.0.1.tar", last modified: Mon Apr 24 03:17:10 2023, max compression
+gzip compressed data, was "vue2img-0.0.2.tar", last modified: Mon Apr 24 03:30:55 2023, max compression
```

## Comparing `vue2img-0.0.1.tar` & `vue2img-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 03:17:10.383326 vue2img-0.0.1/
--rw-rw-rw-   0        0        0     1086 2023-03-31 15:06:16.000000 vue2img-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       24 2023-02-26 12:01:51.000000 vue2img-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      772 2023-04-24 03:17:10.383326 vue2img-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      108 2023-03-31 15:08:31.000000 vue2img-0.0.1/README.md
--rw-rw-rw-   0        0        0      523 2023-04-23 11:23:10.000000 vue2img-0.0.1/notice.txt
--rw-rw-rw-   0        0        0       55 2023-04-24 03:14:17.000000 vue2img-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 03:17:10.384324 vue2img-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      997 2023-04-24 03:12:48.000000 vue2img-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 03:17:10.367381 vue2img-0.0.1/vue2img/
--rw-rw-rw-   0        0        0      178 2023-04-24 02:43:47.000000 vue2img-0.0.1/vue2img/__init__.py
--rw-rw-rw-   0        0        0     1383 2023-04-22 10:16:30.000000 vue2img-0.0.1/vue2img/app.py
--rw-rw-rw-   0        0        0     9659 2023-04-24 03:04:14.000000 vue2img-0.0.1/vue2img/dom.py
--rw-rw-rw-   0        0        0      483 2023-04-24 03:04:58.000000 vue2img-0.0.1/vue2img/manager.py
--rw-rw-rw-   0        0        0     2311 2023-04-24 02:47:32.000000 vue2img-0.0.1/vue2img/operation.py
--rw-rw-rw-   0        0        0     4157 2023-04-24 03:14:14.000000 vue2img-0.0.1/vue2img/template.py
-drwxrwxrwx   0        0        0        0 2023-04-24 03:17:10.381342 vue2img-0.0.1/vue2img.egg-info/
--rw-rw-rw-   0        0        0      772 2023-04-24 03:17:10.000000 vue2img-0.0.1/vue2img.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      330 2023-04-24 03:17:10.000000 vue2img-0.0.1/vue2img.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 03:17:10.000000 vue2img-0.0.1/vue2img.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-04-24 03:17:10.000000 vue2img-0.0.1/vue2img.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-24 03:17:10.000000 vue2img-0.0.1/vue2img.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 03:30:55.020098 vue2img-0.0.2/
+-rw-rw-rw-   0        0        0     1086 2023-03-31 15:06:16.000000 vue2img-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       55 2023-04-24 03:29:08.000000 vue2img-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      746 2023-04-24 03:30:55.019109 vue2img-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      108 2023-03-31 15:08:31.000000 vue2img-0.0.2/README.md
+-rw-rw-rw-   0        0        0       55 2023-04-24 03:14:17.000000 vue2img-0.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 03:30:55.021094 vue2img-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      997 2023-04-24 03:30:23.000000 vue2img-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 03:30:55.005150 vue2img-0.0.2/vue2img/
+-rw-rw-rw-   0        0        0      178 2023-04-24 02:43:47.000000 vue2img-0.0.2/vue2img/__init__.py
+-rw-rw-rw-   0        0        0     1383 2023-04-22 10:16:30.000000 vue2img-0.0.2/vue2img/app.py
+-rw-rw-rw-   0        0        0     9659 2023-04-24 03:04:14.000000 vue2img-0.0.2/vue2img/dom.py
+-rw-rw-rw-   0        0        0      483 2023-04-24 03:04:58.000000 vue2img-0.0.2/vue2img/manager.py
+-rw-rw-rw-   0        0        0     2311 2023-04-24 02:47:32.000000 vue2img-0.0.2/vue2img/operation.py
+-rw-rw-rw-   0        0        0    13073 2023-04-12 17:11:53.000000 vue2img-0.0.2/vue2img/stopwords.txt
+-rw-rw-rw-   0        0        0     4157 2023-04-24 03:14:14.000000 vue2img-0.0.2/vue2img/template.py
+drwxrwxrwx   0        0        0        0 2023-04-24 03:30:55.017106 vue2img-0.0.2/vue2img.egg-info/
+-rw-rw-rw-   0        0        0      746 2023-04-24 03:30:54.000000 vue2img-0.0.2/vue2img.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2023-04-24 03:30:54.000000 vue2img-0.0.2/vue2img.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 03:30:54.000000 vue2img-0.0.2/vue2img.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-04-24 03:30:54.000000 vue2img-0.0.2/vue2img.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-24 03:30:54.000000 vue2img-0.0.2/vue2img.egg-info/top_level.txt
```

### Comparing `vue2img-0.0.1/LICENSE` & `vue2img-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vue2img-0.0.1/PKG-INFO` & `vue2img-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vue2img
-Version: 0.0.1
+Version: 0.0.2
 Summary: 通过 .vue 模板生成图片
 Home-page: https://github.com/Drelf2018/vue2img
 Author: Drelf2018
 Author-email: drelf2018@outlook.com
 License: MIT
 Keywords: python,vue
 Platform: UNKNOWN
@@ -13,15 +13,14 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-License-File: notice.txt
 
 # vue2img
  将 vue 文件编译为图片
 
 ```python
 createApp(1000).mount(config).export().canvas.show()
 ```
```

### Comparing `vue2img-0.0.1/setup.py` & `vue2img-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open("requirements.txt", "r", encoding="utf8") as f:
     requires = f.read()
 
 setup(
     name="vue2img",
-    version="0.0.1",
+    version="0.0.2",
     license="MIT",
     author="Drelf2018",
     author_email="drelf2018@outlook.com",
     description="通过 .vue 模板生成图片",
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
```

### Comparing `vue2img-0.0.1/vue2img/app.py` & `vue2img-0.0.2/vue2img/app.py`

 * *Files identical despite different names*

### Comparing `vue2img-0.0.1/vue2img/dom.py` & `vue2img-0.0.2/vue2img/dom.py`

 * *Files identical despite different names*

### Comparing `vue2img-0.0.1/vue2img/operation.py` & `vue2img-0.0.2/vue2img/operation.py`

 * *Files identical despite different names*

### Comparing `vue2img-0.0.1/vue2img/template.py` & `vue2img-0.0.2/vue2img/template.py`

 * *Files identical despite different names*

### Comparing `vue2img-0.0.1/vue2img.egg-info/PKG-INFO` & `vue2img-0.0.2/vue2img.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vue2img
-Version: 0.0.1
+Version: 0.0.2
 Summary: 通过 .vue 模板生成图片
 Home-page: https://github.com/Drelf2018/vue2img
 Author: Drelf2018
 Author-email: drelf2018@outlook.com
 License: MIT
 Keywords: python,vue
 Platform: UNKNOWN
@@ -13,15 +13,14 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-License-File: notice.txt
 
 # vue2img
  将 vue 文件编译为图片
 
 ```python
 createApp(1000).mount(config).export().canvas.show()
 ```
```

