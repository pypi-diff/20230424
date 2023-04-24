# Comparing `tmp/spacetool-0.2.2.tar.gz` & `tmp/spacetool-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacetool-0.2.2.tar", last modified: Fri Dec 30 04:00:07 2022, max compression
+gzip compressed data, was "spacetool-1.0.1.tar", last modified: Mon Apr 24 06:25:09 2023, max compression
```

## Comparing `spacetool-0.2.2.tar` & `spacetool-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 leo        (501) staff       (20)        0 2022-12-30 04:00:07.421496 spacetool-0.2.2/
--rw-r--r--   0 leo        (501) staff       (20)     1068 2022-11-03 01:53:28.000000 spacetool-0.2.2/LICENSE
--rw-r--r--   0 leo        (501) staff       (20)      422 2022-12-30 04:00:07.421397 spacetool-0.2.2/PKG-INFO
--rw-r--r--   0 leo        (501) staff       (20)       28 2022-11-03 01:53:28.000000 spacetool-0.2.2/README.md
--rw-r--r--   0 leo        (501) staff       (20)       38 2022-12-30 04:00:07.421544 spacetool-0.2.2/setup.cfg
--rw-r--r--   0 leo        (501) staff       (20)     2459 2022-12-30 03:48:43.000000 spacetool-0.2.2/setup.py
-drwxr-xr-x   0 leo        (501) staff       (20)        0 2022-12-30 04:00:07.420681 spacetool-0.2.2/spacetool/
--rw-r--r--   0 leo        (501) staff       (20)        0 2022-11-03 01:53:28.000000 spacetool-0.2.2/spacetool/__init__.py
--rw-r--r--   0 leo        (501) staff       (20)        7 2022-11-08 03:02:34.000000 spacetool-0.2.2/spacetool/__version__.py
--rw-r--r--   0 leo        (501) staff       (20)     6994 2022-12-29 12:08:19.000000 spacetool-0.2.2/spacetool/main_tool.py
-drwxr-xr-x   0 leo        (501) staff       (20)        0 2022-12-30 04:00:07.421265 spacetool-0.2.2/spacetool.egg-info/
--rw-r--r--   0 leo        (501) staff       (20)      422 2022-12-30 04:00:07.000000 spacetool-0.2.2/spacetool.egg-info/PKG-INFO
--rw-r--r--   0 leo        (501) staff       (20)      260 2022-12-30 04:00:07.000000 spacetool-0.2.2/spacetool.egg-info/SOURCES.txt
--rw-r--r--   0 leo        (501) staff       (20)        1 2022-12-30 04:00:07.000000 spacetool-0.2.2/spacetool.egg-info/dependency_links.txt
--rw-r--r--   0 leo        (501) staff       (20)       17 2022-12-30 04:00:07.000000 spacetool-0.2.2/spacetool.egg-info/requires.txt
--rw-r--r--   0 leo        (501) staff       (20)       10 2022-12-30 04:00:07.000000 spacetool-0.2.2/spacetool.egg-info/top_level.txt
+drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-04-24 06:25:09.610072 spacetool-1.0.1/
+-rw-r--r--   0 leo        (501) staff       (20)     1068 2022-11-03 01:53:28.000000 spacetool-1.0.1/LICENSE
+-rw-r--r--   0 leo        (501) staff       (20)      432 2023-04-24 06:25:09.609947 spacetool-1.0.1/PKG-INFO
+-rw-r--r--   0 leo        (501) staff       (20)      135 2023-04-10 02:45:30.000000 spacetool-1.0.1/README.md
+-rw-r--r--   0 leo        (501) staff       (20)       38 2023-04-24 06:25:09.610121 spacetool-1.0.1/setup.cfg
+-rw-r--r--   0 leo        (501) staff       (20)     2527 2023-04-24 06:14:48.000000 spacetool-1.0.1/setup.py
+drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-04-24 06:25:09.608683 spacetool-1.0.1/spacetool/
+-rw-r--r--   0 leo        (501) staff       (20)        0 2022-11-03 01:53:28.000000 spacetool-1.0.1/spacetool/__init__.py
+-rw-r--r--   0 leo        (501) staff       (20)        7 2022-11-08 03:02:34.000000 spacetool-1.0.1/spacetool/__version__.py
+-rw-r--r--   0 leo        (501) staff       (20)    41089 2023-04-24 06:23:47.000000 spacetool-1.0.1/spacetool/main_tool.py
+drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-04-24 06:25:09.609752 spacetool-1.0.1/spacetool.egg-info/
+-rw-r--r--   0 leo        (501) staff       (20)      432 2023-04-24 06:25:09.000000 spacetool-1.0.1/spacetool.egg-info/PKG-INFO
+-rw-r--r--   0 leo        (501) staff       (20)      260 2023-04-24 06:25:09.000000 spacetool-1.0.1/spacetool.egg-info/SOURCES.txt
+-rw-r--r--   0 leo        (501) staff       (20)        1 2023-04-24 06:25:09.000000 spacetool-1.0.1/spacetool.egg-info/dependency_links.txt
+-rw-r--r--   0 leo        (501) staff       (20)       68 2023-04-24 06:25:09.000000 spacetool-1.0.1/spacetool.egg-info/requires.txt
+-rw-r--r--   0 leo        (501) staff       (20)       10 2023-04-24 06:25:09.000000 spacetool-1.0.1/spacetool.egg-info/top_level.txt
```

### Comparing `spacetool-0.2.2/LICENSE` & `spacetool-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spacetool-0.2.2/setup.py` & `spacetool-1.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,32 +3,33 @@
 from setuptools import find_packages
 
 
 from setuptools import setup, find_packages
 
 setup(
     name="spacetool",
-    version="0.2.2",
+    version="1.0.1",
     description='space.top的数据管理工具',
     author="Leo Ni",
     author_email="nij6173@gmail.com",
     url='http://space.top/',
     packages=find_packages(),
-    install_requires=["requests==2.28.1", ],
+    install_requires=["requests==2.28.1", "cos-python-sdk-v5==1.9.23", "qcloud-python-sts==3.1.3"],
     python_requires=">=3.6,<3.11",
-    keywords=['data',],
+    keywords=['data', "spacedata"],
     license='MIT',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
 
 
+
 # setup(name='spacetool',
 #         version='0.1',
 #         packages=find_packages(where='src\\'),  # 查找包的路径
 #         package_dir={'': 'src'},  # 包的root路径映射到的实际路径
 #         include_package_data=False,
 #         package_data={'data': []},
 #         description='A python lib for xxxxx',
```

