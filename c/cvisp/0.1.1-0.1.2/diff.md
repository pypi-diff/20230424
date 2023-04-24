# Comparing `tmp/cvisp-0.1.1.tar.gz` & `tmp/cvisp-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvisp-0.1.1.tar", last modified: Mon Apr 24 07:38:33 2023, max compression
+gzip compressed data, was "cvisp-0.1.2.tar", last modified: Mon Apr 24 08:04:19 2023, max compression
```

## Comparing `cvisp-0.1.1.tar` & `cvisp-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 07:38:33.824722 cvisp-0.1.1/
--rw-rw-rw-   0        0        0     1096 2023-04-24 03:44:04.000000 cvisp-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0      454 2023-04-24 07:38:33.822728 cvisp-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-24 03:13:53.000000 cvisp-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 07:38:33.773580 cvisp-0.1.1/cvisp/
--rw-rw-rw-   0        0        0        0 2023-04-24 03:39:59.000000 cvisp-0.1.1/cvisp/__init__.py
--rw-rw-rw-   0        0        0    17014 2023-04-24 03:38:22.000000 cvisp-0.1.1/cvisp/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-24 07:38:33.814253 cvisp-0.1.1/cvisp.egg-info/
--rw-rw-rw-   0        0        0      454 2023-04-24 07:38:32.000000 cvisp-0.1.1/cvisp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-04-24 07:38:33.000000 cvisp-0.1.1/cvisp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 07:38:32.000000 cvisp-0.1.1/cvisp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-04-24 07:38:32.000000 cvisp-0.1.1/cvisp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-24 07:38:32.000000 cvisp-0.1.1/cvisp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 07:38:33.825718 cvisp-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1229 2023-04-24 07:38:29.000000 cvisp-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:04:19.916174 cvisp-0.1.2/
+-rw-rw-rw-   0        0        0     1096 2023-04-24 03:44:04.000000 cvisp-0.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      454 2023-04-24 08:04:19.913182 cvisp-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-24 03:13:53.000000 cvisp-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 08:04:19.826993 cvisp-0.1.2/cvisp/
+-rw-rw-rw-   0        0        0        0 2023-04-24 03:39:59.000000 cvisp-0.1.2/cvisp/__init__.py
+-rw-rw-rw-   0        0        0    17014 2023-04-24 03:38:22.000000 cvisp-0.1.2/cvisp/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:04:19.899923 cvisp-0.1.2/cvisp.egg-info/
+-rw-rw-rw-   0        0        0      454 2023-04-24 08:04:19.000000 cvisp-0.1.2/cvisp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2023-04-24 08:04:19.000000 cvisp-0.1.2/cvisp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 08:04:19.000000 cvisp-0.1.2/cvisp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-04-24 08:04:19.000000 cvisp-0.1.2/cvisp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-24 08:04:19.000000 cvisp-0.1.2/cvisp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 08:04:19.918170 cvisp-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1229 2023-04-24 08:04:00.000000 cvisp-0.1.2/setup.py
```

### Comparing `cvisp-0.1.1/LICENSE.txt` & `cvisp-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cvisp-0.1.1/cvisp/utils.py` & `cvisp-0.1.2/cvisp/utils.py`

 * *Files identical despite different names*

### Comparing `cvisp-0.1.1/setup.py` & `cvisp-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools  # 导入setuptools打包工具
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cvisp",  # 用自己的名替换其中的YOUR_USERNAME_
-    version="0.1.1",  # 包版本号，便于pip维护版本
+    version="0.1.2",  # 包版本号，便于pip维护版本
     author="Huii Ji",  # 作者，可以写自己的姓名
     author_email="752413464@qq.com",  # 作者联系方式，可写自己的邮箱地址
     description="A small example package of demosaic-raw and cvisp, for our team",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://github.com/HuiiJi",  # 自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
@@ -22,9 +22,9 @@
         # add any other dependencies here
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.9',  # 对python的最低版本要求
+    python_requires='>=3.6',  # 对python的最低版本要求
 )
```

