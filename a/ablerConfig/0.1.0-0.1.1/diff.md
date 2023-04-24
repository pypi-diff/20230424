# Comparing `tmp/ablerConfig-0.1.0.tar.gz` & `tmp/ablerConfig-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ablerConfig-0.1.0.tar", last modified: Mon Apr 24 15:12:57 2023, max compression
+gzip compressed data, was "ablerConfig-0.1.1.tar", last modified: Mon Apr 24 18:12:21 2023, max compression
```

## Comparing `ablerConfig-0.1.0.tar` & `ablerConfig-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 15:12:57.606714 ablerConfig-0.1.0/
--rw-rw-rw-   0        0        0     2004 2023-04-24 15:12:57.605714 ablerConfig-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1236 2023-04-23 22:28:12.000000 ablerConfig-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 15:12:57.597604 ablerConfig-0.1.0/ablerConfig/
--rw-rw-rw-   0        0        0      131 2023-04-24 15:11:44.000000 ablerConfig-0.1.0/ablerConfig/__init__.py
--rw-rw-rw-   0        0        0    12751 2023-04-24 15:06:14.000000 ablerConfig-0.1.0/ablerConfig/config.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:12:57.604710 ablerConfig-0.1.0/ablerConfig.egg-info/
--rw-rw-rw-   0        0        0     2004 2023-04-24 15:12:57.000000 ablerConfig-0.1.0/ablerConfig.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-04-24 15:12:57.000000 ablerConfig-0.1.0/ablerConfig.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 15:12:57.000000 ablerConfig-0.1.0/ablerConfig.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-24 15:12:57.000000 ablerConfig-0.1.0/ablerConfig.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-24 15:12:57.000000 ablerConfig-0.1.0/ablerConfig.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 15:12:57.606714 ablerConfig-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1044 2023-04-24 15:11:29.000000 ablerConfig-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 18:12:21.935610 ablerConfig-0.1.1/
+-rw-rw-rw-   0        0        0     2025 2023-04-24 18:12:21.934599 ablerConfig-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1257 2023-04-24 18:09:32.000000 ablerConfig-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 18:12:21.923426 ablerConfig-0.1.1/ablerConfig/
+-rw-rw-rw-   0        0        0      131 2023-04-24 18:06:40.000000 ablerConfig-0.1.1/ablerConfig/__init__.py
+-rw-rw-rw-   0        0        0    12847 2023-04-24 18:06:26.000000 ablerConfig-0.1.1/ablerConfig/config.py
+drwxrwxrwx   0        0        0        0 2023-04-24 18:12:21.932597 ablerConfig-0.1.1/ablerConfig.egg-info/
+-rw-rw-rw-   0        0        0     2025 2023-04-24 18:12:21.000000 ablerConfig-0.1.1/ablerConfig.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-04-24 18:12:21.000000 ablerConfig-0.1.1/ablerConfig.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 18:12:21.000000 ablerConfig-0.1.1/ablerConfig.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-24 18:12:21.000000 ablerConfig-0.1.1/ablerConfig.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-24 18:12:21.000000 ablerConfig-0.1.1/ablerConfig.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 18:12:21.935610 ablerConfig-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1044 2023-04-24 18:06:50.000000 ablerConfig-0.1.1/setup.py
```

### Comparing `ablerConfig-0.1.0/PKG-INFO` & `ablerConfig-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ablerConfig
-Version: 0.1.0
+Version: 0.1.1
 Summary: 配置信息处理包
 Home-page: https://github.com/hanlaohan/abler-config
 Author: 憨老汉
 Author-email: hh28642257@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -54,20 +54,20 @@
 
 ### 加载配置文件
 
 您可以使用`ablerConfig.Config()`函数加载配置文件。例如：
 
 ```python
 import ablerConfig as config
-config.Config(default='my-config', show_message=my_show_message)
+config.Config(default='my-config', local_dir='ex-conf', show_message=my_show_message)
 ```
 
 ### 引用配置项
 
-您可以使用`ablerConfig.Config.object_of()`函数引用配置文件中的配置对象，也可以使用`ablerConfig.Config.value_of()`函数将引用配置文件中的简单配置项。例如：
+您可以使用`ablerConfig.Config.object_of()`方法引用配置文件中的配置对象，也可以使用`ablerConfig.Config.value_of()`方法将引用配置文件中的简单配置项。例如：
 
 ```python
 from ablerConfig import Config, ConfigNode
 
 conf = Config.object_of('alarm_control.state_send')
 addr = tuple(Config.value_of('net_gate.tt_addr'))
 ```
```

### Comparing `ablerConfig-0.1.0/README.md` & `ablerConfig-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -35,20 +35,20 @@
 
 ### 加载配置文件
 
 您可以使用`ablerConfig.Config()`函数加载配置文件。例如：
 
 ```python
 import ablerConfig as config
-config.Config(default='my-config', show_message=my_show_message)
+config.Config(default='my-config', local_dir='ex-conf', show_message=my_show_message)
 ```
 
 ### 引用配置项
 
-您可以使用`ablerConfig.Config.object_of()`函数引用配置文件中的配置对象，也可以使用`ablerConfig.Config.value_of()`函数将引用配置文件中的简单配置项。例如：
+您可以使用`ablerConfig.Config.object_of()`方法引用配置文件中的配置对象，也可以使用`ablerConfig.Config.value_of()`方法将引用配置文件中的简单配置项。例如：
 
 ```python
 from ablerConfig import Config, ConfigNode
 
 conf = Config.object_of('alarm_control.state_send')
 addr = tuple(Config.value_of('net_gate.tt_addr'))
 ```
```

### Comparing `ablerConfig-0.1.0/ablerConfig/config.py` & `ablerConfig-0.1.1/ablerConfig/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,20 +199,20 @@
         result = self.get_value(path)
         # return ConfigNode(result)
         return result
 
     @staticmethod
     def conf_path(sub_name=None, local=False):
         if local:
-            cfg_dir = os.path.abspath(os.path.join(os.getcwd(), '..', LOCAL_CONF_DIR))
+            path = os.path.abspath(os.path.join(os.getcwd(), '..', LOCAL_CONF_DIR))
         else:
-            cfg_dir = os.path.join(os.getcwd(), 'config')
+            path = os.path.join(os.getcwd(), 'config')
         if sub_name is not None:
-            cfg_dir = os.path.join(cfg_dir, sub_name)
-        return cfg_dir
+            path = os.path.join(path, sub_name)
+        return path
 
     @staticmethod
     def conf_file_path(conf_name, local=False):
         return Config.conf_path(sub_name=f"{conf_name}{CONF_EXT}", local=local)
 
     @classmethod
     def open_conf_file(cls, conf_name, local=False, show_message=print):
@@ -224,15 +224,17 @@
 
     @classmethod
     def check_local_config(cls, root: ConfigNode, show_message=print):
         # default = cls.main.default
         # default_ver = default.get('cfg_version')
         # default_file = cls.conf_file_path(DEF_CFG_NAME, local=False)
         local_file = cls.conf_file_path(DEF_CFG_NAME, local=True)
-
+        _dir = os.path.dirname(local_file)
+        if not os.path.exists(_dir):
+            os.makedirs(_dir)
         # if not os.path.exists(local_file):
         #     _dir = os.path.dirname(local_file)
         #     if not os.path.exists(_dir):
         #         os.makedirs(_dir)
         #     # 第一次，不改版本号，以便能够直接运行，增强用户信心
         #     copyfile(default_file, local_file)
         local = None
```

### Comparing `ablerConfig-0.1.0/ablerConfig.egg-info/PKG-INFO` & `ablerConfig-0.1.1/ablerConfig.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ablerConfig
-Version: 0.1.0
+Version: 0.1.1
 Summary: 配置信息处理包
 Home-page: https://github.com/hanlaohan/abler-config
 Author: 憨老汉
 Author-email: hh28642257@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -54,20 +54,20 @@
 
 ### 加载配置文件
 
 您可以使用`ablerConfig.Config()`函数加载配置文件。例如：
 
 ```python
 import ablerConfig as config
-config.Config(default='my-config', show_message=my_show_message)
+config.Config(default='my-config', local_dir='ex-conf', show_message=my_show_message)
 ```
 
 ### 引用配置项
 
-您可以使用`ablerConfig.Config.object_of()`函数引用配置文件中的配置对象，也可以使用`ablerConfig.Config.value_of()`函数将引用配置文件中的简单配置项。例如：
+您可以使用`ablerConfig.Config.object_of()`方法引用配置文件中的配置对象，也可以使用`ablerConfig.Config.value_of()`方法将引用配置文件中的简单配置项。例如：
 
 ```python
 from ablerConfig import Config, ConfigNode
 
 conf = Config.object_of('alarm_control.state_send')
 addr = tuple(Config.value_of('net_gate.tt_addr'))
 ```
```

### Comparing `ablerConfig-0.1.0/setup.py` & `ablerConfig-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="ablerConfig",
-    version="0.1.0",
+    version="0.1.1",
     author="憨老汉",
     author_email="hh28642257@gmail.com",
     description="配置信息处理包",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hanlaohan/abler-config",
     packages=find_packages(),
```

