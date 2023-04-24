# Comparing `tmp/grun_js-0.0.2.tar.gz` & `tmp/grun_js-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grun_js-0.0.2.tar", last modified: Mon Apr 24 06:37:14 2023, max compression
+gzip compressed data, was "grun_js-0.0.3.tar", last modified: Mon Apr 24 06:39:09 2023, max compression
```

## Comparing `grun_js-0.0.2.tar` & `grun_js-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 06:37:14.583035 grun_js-0.0.2/
--rw-rw-rw-   0        0        0      666 2023-04-24 06:37:14.581026 grun_js-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-24 06:37:14.560007 grun_js-0.0.2/grun_js/
--rw-rw-rw-   0        0        0       33 2023-04-24 06:32:44.000000 grun_js-0.0.2/grun_js/__init__.py
--rw-rw-rw-   0        0        0     2765 2023-04-24 06:14:28.000000 grun_js-0.0.2/grun_js/runjs.py
-drwxrwxrwx   0        0        0        0 2023-04-24 06:37:14.576009 grun_js-0.0.2/grun_js.egg-info/
--rw-rw-rw-   0        0        0      666 2023-04-24 06:37:14.000000 grun_js-0.0.2/grun_js.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      169 2023-04-24 06:37:14.000000 grun_js-0.0.2/grun_js.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 06:37:14.000000 grun_js-0.0.2/grun_js.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-24 06:37:14.000000 grun_js-0.0.2/grun_js.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 06:37:14.583035 grun_js-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      825 2023-04-24 06:37:10.000000 grun_js-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 06:39:09.432819 grun_js-0.0.3/
+-rw-rw-rw-   0        0        0       25 2023-04-24 06:39:01.000000 grun_js-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      666 2023-04-24 06:39:09.431819 grun_js-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-24 06:39:09.408836 grun_js-0.0.3/grun_js/
+-rw-rw-rw-   0        0        0      345 2023-04-24 06:32:44.000000 grun_js-0.0.3/grun_js/README.md
+-rw-rw-rw-   0        0        0       33 2023-04-24 06:32:44.000000 grun_js-0.0.3/grun_js/__init__.py
+-rw-rw-rw-   0        0        0     2765 2023-04-24 06:14:28.000000 grun_js-0.0.3/grun_js/runjs.py
+drwxrwxrwx   0        0        0        0 2023-04-24 06:39:09.426843 grun_js-0.0.3/grun_js.egg-info/
+-rw-rw-rw-   0        0        0      666 2023-04-24 06:39:09.000000 grun_js-0.0.3/grun_js.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      199 2023-04-24 06:39:09.000000 grun_js-0.0.3/grun_js.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 06:39:09.000000 grun_js-0.0.3/grun_js.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-24 06:39:09.000000 grun_js-0.0.3/grun_js.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 06:39:09.433823 grun_js-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      825 2023-04-24 06:39:05.000000 grun_js-0.0.3/setup.py
```

### Comparing `grun_js-0.0.2/PKG-INFO` & `grun_js-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grun_js
-Version: 0.0.2
+Version: 0.0.3
 Summary: 调用 node 执行 js，可指定编码
 Home-page: https://github.com/Leviathangk/runjs
 Author: 郭一会儿
 Author-email: 1015295213@qq.com
 License: MIT Licence
 Keywords: js,grun_js,pyexecjs
 Platform: any
```

### Comparing `grun_js-0.0.2/grun_js/runjs.py` & `grun_js-0.0.3/grun_js/runjs.py`

 * *Files identical despite different names*

### Comparing `grun_js-0.0.2/grun_js.egg-info/PKG-INFO` & `grun_js-0.0.3/grun_js.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grun-js
-Version: 0.0.2
+Version: 0.0.3
 Summary: 调用 node 执行 js，可指定编码
 Home-page: https://github.com/Leviathangk/runjs
 Author: 郭一会儿
 Author-email: 1015295213@qq.com
 License: MIT Licence
 Keywords: js,grun_js,pyexecjs
 Platform: any
```

### Comparing `grun_js-0.0.2/setup.py` & `grun_js-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages  # 这个包没有的可以pip一下
 
 file_path = './grun_js/README.md'
 
 setup(
     name="grun_js",  # 这里是pip项目发布的名称
-    version="0.0.2",  # 版本号，数值大的会优先被 pip
+    version="0.0.3",  # 版本号，数值大的会优先被 pip
     keywords=["js", "grun_js", "pyexecjs"],  # 关键字
     description="调用 node 执行 js，可指定编码",  # 描述
     long_description=open(file_path, 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     license="MIT Licence",  # 许可证
 
     url="https://github.com/Leviathangk/runjs",  # 项目相关文件地址，一般是github项目地址即可
```

