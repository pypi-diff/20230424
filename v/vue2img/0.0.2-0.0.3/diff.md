# Comparing `tmp/vue2img-0.0.2.tar.gz` & `tmp/vue2img-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vue2img-0.0.2.tar", last modified: Mon Apr 24 03:30:55 2023, max compression
+gzip compressed data, was "vue2img-0.0.3.tar", last modified: Mon Apr 24 03:36:23 2023, max compression
```

## Comparing `vue2img-0.0.2.tar` & `vue2img-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 03:30:55.020098 vue2img-0.0.2/
--rw-rw-rw-   0        0        0     1086 2023-03-31 15:06:16.000000 vue2img-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       55 2023-04-24 03:29:08.000000 vue2img-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      746 2023-04-24 03:30:55.019109 vue2img-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      108 2023-03-31 15:08:31.000000 vue2img-0.0.2/README.md
--rw-rw-rw-   0        0        0       55 2023-04-24 03:14:17.000000 vue2img-0.0.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 03:30:55.021094 vue2img-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      997 2023-04-24 03:30:23.000000 vue2img-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 03:30:55.005150 vue2img-0.0.2/vue2img/
--rw-rw-rw-   0        0        0      178 2023-04-24 02:43:47.000000 vue2img-0.0.2/vue2img/__init__.py
--rw-rw-rw-   0        0        0     1383 2023-04-22 10:16:30.000000 vue2img-0.0.2/vue2img/app.py
--rw-rw-rw-   0        0        0     9659 2023-04-24 03:04:14.000000 vue2img-0.0.2/vue2img/dom.py
--rw-rw-rw-   0        0        0      483 2023-04-24 03:04:58.000000 vue2img-0.0.2/vue2img/manager.py
--rw-rw-rw-   0        0        0     2311 2023-04-24 02:47:32.000000 vue2img-0.0.2/vue2img/operation.py
--rw-rw-rw-   0        0        0    13073 2023-04-12 17:11:53.000000 vue2img-0.0.2/vue2img/stopwords.txt
--rw-rw-rw-   0        0        0     4157 2023-04-24 03:14:14.000000 vue2img-0.0.2/vue2img/template.py
-drwxrwxrwx   0        0        0        0 2023-04-24 03:30:55.017106 vue2img-0.0.2/vue2img.egg-info/
--rw-rw-rw-   0        0        0      746 2023-04-24 03:30:54.000000 vue2img-0.0.2/vue2img.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      341 2023-04-24 03:30:54.000000 vue2img-0.0.2/vue2img.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 03:30:54.000000 vue2img-0.0.2/vue2img.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-04-24 03:30:54.000000 vue2img-0.0.2/vue2img.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-24 03:30:54.000000 vue2img-0.0.2/vue2img.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 03:36:23.378361 vue2img-0.0.3/
+-rw-rw-rw-   0        0        0     1086 2023-03-31 15:06:16.000000 vue2img-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       55 2023-04-24 03:29:08.000000 vue2img-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      746 2023-04-24 03:36:23.378361 vue2img-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      108 2023-03-31 15:08:31.000000 vue2img-0.0.3/README.md
+-rw-rw-rw-   0        0        0       55 2023-04-24 03:14:17.000000 vue2img-0.0.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 03:36:23.379358 vue2img-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      997 2023-04-24 03:36:20.000000 vue2img-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 03:36:23.355439 vue2img-0.0.3/vue2img/
+-rw-rw-rw-   0        0        0      178 2023-04-24 02:43:47.000000 vue2img-0.0.3/vue2img/__init__.py
+-rw-rw-rw-   0        0        0     1383 2023-04-22 10:16:30.000000 vue2img-0.0.3/vue2img/app.py
+-rw-rw-rw-   0        0        0     9659 2023-04-24 03:04:14.000000 vue2img-0.0.3/vue2img/dom.py
+-rw-rw-rw-   0        0        0      483 2023-04-24 03:04:58.000000 vue2img-0.0.3/vue2img/manager.py
+-rw-rw-rw-   0        0        0     2098 2023-04-24 03:35:55.000000 vue2img-0.0.3/vue2img/operation.py
+-rw-rw-rw-   0        0        0    24517 2023-04-24 03:36:10.000000 vue2img-0.0.3/vue2img/stopwords.py
+-rw-rw-rw-   0        0        0     4157 2023-04-24 03:14:14.000000 vue2img-0.0.3/vue2img/template.py
+drwxrwxrwx   0        0        0        0 2023-04-24 03:36:23.376369 vue2img-0.0.3/vue2img.egg-info/
+-rw-rw-rw-   0        0        0      746 2023-04-24 03:36:23.000000 vue2img-0.0.3/vue2img.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-04-24 03:36:23.000000 vue2img-0.0.3/vue2img.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 03:36:23.000000 vue2img-0.0.3/vue2img.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-04-24 03:36:23.000000 vue2img-0.0.3/vue2img.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-24 03:36:23.000000 vue2img-0.0.3/vue2img.egg-info/top_level.txt
```

### Comparing `vue2img-0.0.2/LICENSE` & `vue2img-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vue2img-0.0.2/PKG-INFO` & `vue2img-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vue2img
-Version: 0.0.2
+Version: 0.0.3
 Summary: 通过 .vue 模板生成图片
 Home-page: https://github.com/Drelf2018/vue2img
 Author: Drelf2018
 Author-email: drelf2018@outlook.com
 License: MIT
 Keywords: python,vue
 Platform: UNKNOWN
```

### Comparing `vue2img-0.0.2/setup.py` & `vue2img-0.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open("requirements.txt", "r", encoding="utf8") as f:
     requires = f.read()
 
 setup(
     name="vue2img",
-    version="0.0.2",
+    version="0.0.3",
     license="MIT",
     author="Drelf2018",
     author_email="drelf2018@outlook.com",
     description="通过 .vue 模板生成图片",
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
```

### Comparing `vue2img-0.0.2/vue2img/app.py` & `vue2img-0.0.3/vue2img/app.py`

 * *Files identical despite different names*

### Comparing `vue2img-0.0.2/vue2img/dom.py` & `vue2img-0.0.3/vue2img/dom.py`

 * *Files identical despite different names*

### Comparing `vue2img-0.0.2/vue2img/operation.py` & `vue2img-0.0.3/vue2img/operation.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,15 @@
 from typing import Set, Tuple
 
 import jieba
 import numpy as np
 from PIL import Image, ImageDraw
 from wordcloud import STOPWORDS, WordCloud
 
-stopwords = os.path.abspath(
-    os.path.join(
-        os.path.dirname(__file__), "stopwords.txt"
-    )
-)
+from .stopwords import stopwords
 
 
 def radiusMask(alpha: Image.Image, radius: Tuple[float], beta: float = 10):
     "给遮罩层加圆角"
 
     w, h = alpha.size
     # 圆角的位置
@@ -30,24 +26,20 @@
         draw = ImageDraw.Draw(circle)
         draw.pieslice(((0, 0), (int(2 * beta * r), int(2 * beta * r))), 180, 270, fill=255)  # 绘制白色扇形
         circle = circle.rotate(-90 * i).resize((int(r), int(r)), Image.LANCZOS)  # 旋转以及缩小
         alpha.paste(circle, position[i])
     return alpha
 
 
-def word2cloud(danmakus: str, mask: Image.Image, font_path: str = None, content: Set[str] = set()) -> Image.Image:
+def word2cloud(danmakus: str, mask: Image.Image, font_path: str = None, content: Set[str] = stopwords) -> Image.Image:
     # jieba 分词
     jieba.add_word('睡啄')
     sentence = "/".join(jieba.cut(danmakus))
     graph = np.array(mask)
 
-    # 停用词
-    if not content:
-        content = set(line.strip() for line in open(stopwords, "r", encoding="utf-8").readlines())
-
     # 词云
     return WordCloud(
         font_path=font_path,
         prefer_horizontal=1,
         collocations=False,
         background_color=None,
         mask=graph,
```

### Comparing `vue2img-0.0.2/vue2img/template.py` & `vue2img-0.0.3/vue2img/template.py`

 * *Files identical despite different names*

### Comparing `vue2img-0.0.2/vue2img.egg-info/PKG-INFO` & `vue2img-0.0.3/vue2img.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vue2img
-Version: 0.0.2
+Version: 0.0.3
 Summary: 通过 .vue 模板生成图片
 Home-page: https://github.com/Drelf2018/vue2img
 Author: Drelf2018
 Author-email: drelf2018@outlook.com
 License: MIT
 Keywords: python,vue
 Platform: UNKNOWN
```

