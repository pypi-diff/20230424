# Comparing `tmp/ablerConfig-0.0.9.tar.gz` & `tmp/ablerConfig-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ablerConfig-0.0.9.tar", last modified: Mon Apr 24 10:32:14 2023, max compression
+gzip compressed data, was "ablerConfig-0.1.0.tar", last modified: Mon Apr 24 15:12:57 2023, max compression
```

## Comparing `ablerConfig-0.0.9.tar` & `ablerConfig-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 10:32:14.586812 ablerConfig-0.0.9/
--rw-rw-rw-   0        0        0     2004 2023-04-24 10:32:14.585821 ablerConfig-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     1236 2023-04-23 22:28:12.000000 ablerConfig-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 10:32:14.576673 ablerConfig-0.0.9/ablerConfig/
--rw-rw-rw-   0        0        0      131 2023-04-24 10:30:59.000000 ablerConfig-0.0.9/ablerConfig/__init__.py
--rw-rw-rw-   0        0        0    12706 2023-04-22 20:35:47.000000 ablerConfig-0.0.9/ablerConfig/config.py
-drwxrwxrwx   0        0        0        0 2023-04-24 10:32:14.583810 ablerConfig-0.0.9/ablerConfig.egg-info/
--rw-rw-rw-   0        0        0     2004 2023-04-24 10:32:14.000000 ablerConfig-0.0.9/ablerConfig.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-04-24 10:32:14.000000 ablerConfig-0.0.9/ablerConfig.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 10:32:14.000000 ablerConfig-0.0.9/ablerConfig.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-24 10:32:14.000000 ablerConfig-0.0.9/ablerConfig.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-24 10:32:14.000000 ablerConfig-0.0.9/ablerConfig.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 10:32:14.587828 ablerConfig-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1044 2023-04-24 10:31:23.000000 ablerConfig-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:12:57.606714 ablerConfig-0.1.0/
+-rw-rw-rw-   0        0        0     2004 2023-04-24 15:12:57.605714 ablerConfig-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1236 2023-04-23 22:28:12.000000 ablerConfig-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 15:12:57.597604 ablerConfig-0.1.0/ablerConfig/
+-rw-rw-rw-   0        0        0      131 2023-04-24 15:11:44.000000 ablerConfig-0.1.0/ablerConfig/__init__.py
+-rw-rw-rw-   0        0        0    12751 2023-04-24 15:06:14.000000 ablerConfig-0.1.0/ablerConfig/config.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:12:57.604710 ablerConfig-0.1.0/ablerConfig.egg-info/
+-rw-rw-rw-   0        0        0     2004 2023-04-24 15:12:57.000000 ablerConfig-0.1.0/ablerConfig.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-04-24 15:12:57.000000 ablerConfig-0.1.0/ablerConfig.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 15:12:57.000000 ablerConfig-0.1.0/ablerConfig.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-24 15:12:57.000000 ablerConfig-0.1.0/ablerConfig.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-24 15:12:57.000000 ablerConfig-0.1.0/ablerConfig.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 15:12:57.606714 ablerConfig-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1044 2023-04-24 15:11:29.000000 ablerConfig-0.1.0/setup.py
```

### Comparing `ablerConfig-0.0.9/PKG-INFO` & `ablerConfig-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ablerConfig
-Version: 0.0.9
+Version: 0.1.0
 Summary: 配置信息处理包
 Home-page: https://github.com/hanlaohan/abler-config
 Author: 憨老汉
 Author-email: hh28642257@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ablerConfig-0.0.9/README.md` & `ablerConfig-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ablerConfig-0.0.9/ablerConfig/config.py` & `ablerConfig-0.1.0/ablerConfig/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 (TOML不支持异质数组， 如 [1, '井眼井深', 0, 'm'])
 """
 from __future__ import annotations
 import os
 import pyjson5 as qjson  # 非常奇怪，不知道怎么格式化输出
 import json5 as json  # 要输出的时候改成这个，比较慢的
 
-# DEF_CFG_NAME = 'dsw-config'
-DEF_CFG_NAME = ''   # 主程序首次调用 Config() 时设置
+DEF_CFG_NAME = ''       # 主程序首次调用 Config() 时设置
+LOCAL_CONF_DIR = ''     # 本地外部配置文件目录名
 CONF_EXT = '.json5'
 
 
 class ConfigError(Exception):
     def __init__(self, conf_name):
         filenames = [Config.conf_file_path(conf_name)]
         if conf_name != DEF_CFG_NAME:
@@ -136,24 +136,29 @@
 class Config:
     main: Config = None
     root: ConfigNode = None
     """
     第一个创建的实例将作为系统的主配置对象
     """
 
-    def __init__(self, conf_name=None, default=None, show_message=print):
+    def __init__(self, conf_name=None, default='', local_dir='', show_message=print):
         if Config.main is None:
             Config.main = self
         self.root: ConfigNode = None
-        global DEF_CFG_NAME
+        global DEF_CFG_NAME, LOCAL_CONF_DIR
         self.conf_name = conf_name or default or DEF_CFG_NAME
         if default != '' and DEF_CFG_NAME == '':
             DEF_CFG_NAME = default
         if DEF_CFG_NAME == '':
-            raise Exception('编码错误：使用Config()之前必须设置DEF_CFG_NAME')
+            raise Exception('编码错误：首次调用Config()必须指定default=?')
+        if local_dir != '' and LOCAL_CONF_DIR == '':
+            LOCAL_CONF_DIR = local_dir
+        if LOCAL_CONF_DIR == '':
+            raise Exception('编码错误：首次调用Config()必须指定local_dir=?')
+
         # self.default = self.open_conf_file(default, local=False)
         # self.root = self.open_conf_file(self.conf_name, local=True)
         # self._root = ConfigNode({'local': self.root, 'default': self.default})
         # self.root = self._root.local
         # self.default = self._root.default
 
         inner = self.open_conf_file(default, local=False)
@@ -192,27 +197,26 @@
 
     def get_object(self, path):
         result = self.get_value(path)
         # return ConfigNode(result)
         return result
 
     @staticmethod
-    def conf_dir_path(sub_name, local=False):
+    def conf_path(sub_name=None, local=False):
         if local:
-            return os.path.join(os.path.dirname(os.path.abspath(__file__)), '..', 'dsw-conf', sub_name)
-        return os.path.join(os.path.dirname(os.path.abspath(__file__)), 'config', sub_name)
+            cfg_dir = os.path.abspath(os.path.join(os.getcwd(), '..', LOCAL_CONF_DIR))
+        else:
+            cfg_dir = os.path.join(os.getcwd(), 'config')
+        if sub_name is not None:
+            cfg_dir = os.path.join(cfg_dir, sub_name)
+        return cfg_dir
 
     @staticmethod
     def conf_file_path(conf_name, local=False):
-        if local:
-            cfg_dir = os.path.abspath(os.path.join(os.path.dirname(os.path.abspath(__file__)), '..', 'dsw-conf'))
-            if not os.path.exists(cfg_dir):
-                os.makedirs(cfg_dir)
-            return os.path.join(cfg_dir, f"{conf_name}{CONF_EXT}")
-        return os.path.join(os.path.dirname(os.path.abspath(__file__)), 'config', f"{conf_name}{CONF_EXT}")
+        return Config.conf_path(sub_name=f"{conf_name}{CONF_EXT}", local=local)
 
     @classmethod
     def open_conf_file(cls, conf_name, local=False, show_message=print):
         conf_file = cls.conf_file_path(conf_name, local)
         if local and (conf_name == DEF_CFG_NAME):
             # 检查本地配置文件
             return cls.check_local_config(cls.root, show_message=show_message)
```

### Comparing `ablerConfig-0.0.9/ablerConfig.egg-info/PKG-INFO` & `ablerConfig-0.1.0/ablerConfig.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ablerConfig
-Version: 0.0.9
+Version: 0.1.0
 Summary: 配置信息处理包
 Home-page: https://github.com/hanlaohan/abler-config
 Author: 憨老汉
 Author-email: hh28642257@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ablerConfig-0.0.9/setup.py` & `ablerConfig-0.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="ablerConfig",
-    version="0.0.9",
+    version="0.1.0",
     author="憨老汉",
     author_email="hh28642257@gmail.com",
     description="配置信息处理包",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hanlaohan/abler-config",
     packages=find_packages(),
```

