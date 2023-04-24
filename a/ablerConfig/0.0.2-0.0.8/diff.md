# Comparing `tmp/ablerConfig-0.0.2.tar.gz` & `tmp/ablerConfig-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ablerConfig-0.0.2.tar", last modified: Sun Apr 23 21:38:00 2023, max compression
+gzip compressed data, was "ablerConfig-0.0.8.tar", last modified: Mon Apr 24 10:13:03 2023, max compression
```

## Comparing `ablerConfig-0.0.2.tar` & `ablerConfig-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 21:38:00.915520 ablerConfig-0.0.2/
--rw-rw-rw-   0        0        0     1993 2023-04-23 21:38:00.914517 ablerConfig-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1225 2023-04-23 21:26:21.000000 ablerConfig-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 21:38:00.905518 ablerConfig-0.0.2/abler-config/
--rw-rw-rw-   0        0        0        0 2023-04-23 21:26:02.000000 ablerConfig-0.0.2/abler-config/__init__.py
--rw-rw-rw-   0        0        0    12706 2023-04-22 20:35:47.000000 ablerConfig-0.0.2/abler-config/config.py
-drwxrwxrwx   0        0        0        0 2023-04-23 21:38:00.912525 ablerConfig-0.0.2/ablerConfig.egg-info/
--rw-rw-rw-   0        0        0     1993 2023-04-23 21:38:00.000000 ablerConfig-0.0.2/ablerConfig.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-04-23 21:38:00.000000 ablerConfig-0.0.2/ablerConfig.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 21:38:00.000000 ablerConfig-0.0.2/ablerConfig.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-23 21:38:00.000000 ablerConfig-0.0.2/ablerConfig.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-23 21:38:00.000000 ablerConfig-0.0.2/ablerConfig.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 21:38:00.915520 ablerConfig-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1044 2023-04-23 21:02:47.000000 ablerConfig-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 10:13:03.215908 ablerConfig-0.0.8/
+-rw-rw-rw-   0        0        0     2004 2023-04-24 10:13:03.215908 ablerConfig-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1236 2023-04-23 22:28:12.000000 ablerConfig-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 10:13:03.207756 ablerConfig-0.0.8/ablerConfig/
+-rw-rw-rw-   0        0        0       15 2023-04-24 10:11:47.000000 ablerConfig-0.0.8/ablerConfig/__init__.py
+-rw-rw-rw-   0        0        0    12706 2023-04-22 20:35:47.000000 ablerConfig-0.0.8/ablerConfig/config.py
+drwxrwxrwx   0        0        0        0 2023-04-24 10:13:03.214908 ablerConfig-0.0.8/ablerConfig.egg-info/
+-rw-rw-rw-   0        0        0     2004 2023-04-24 10:13:03.000000 ablerConfig-0.0.8/ablerConfig.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-04-24 10:13:03.000000 ablerConfig-0.0.8/ablerConfig.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 10:13:03.000000 ablerConfig-0.0.8/ablerConfig.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-24 10:13:03.000000 ablerConfig-0.0.8/ablerConfig.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-24 10:13:03.000000 ablerConfig-0.0.8/ablerConfig.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 10:13:03.216908 ablerConfig-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1044 2023-04-24 10:12:46.000000 ablerConfig-0.0.8/setup.py
```

### Comparing `ablerConfig-0.0.2/PKG-INFO` & `ablerConfig-0.0.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ablerConfig
-Version: 0.0.2
+Version: 0.0.8
 Summary: 配置信息处理包
 Home-page: https://github.com/hanlaohan/abler-config
 Author: 憨老汉
 Author-email: hh28642257@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -19,24 +19,24 @@
 
 ablerConfig
 =============
 
 简介
 --
 
-这是一个用于处理配置信息的Python包。它可以帮助应用程序读取、写入和验证配置文件。该包主要是供彭彭自用的。
+这是一个用于处理配置信息的Python包。它可以帮助应用程序读取、写入和验证配置文件。该包暂时只供彭彭项目组自用。
 
 特点
 --
 
 *   支持JSON5格式的配置文件。
 *   可以验证配置文件的格式和内容。
 *   可以使用默认值填充缺失的配置项。
 *   可以将配置文件转换为Python对象，以便更方便地访问和修改。
-*   可以将Python对象转换为配置文件。
+*   支持内部配置文件和本地外部配置文件。
 
 依赖项
 ---
 
 *   pyjson5
 *   json5
 
@@ -50,25 +50,25 @@
 ```
 
 使用方法
 ----
 
 ### 加载配置文件
 
-您可以使用`abler_config.Config()`函数加载配置文件。例如：
+您可以使用`ablerConfig.Config()`函数加载配置文件。例如：
 
 ```python
 import ablerConfig as config
 config.Config(default='my-config', show_message=my_show_message)
 ```
 
 ### 引用配置项
 
-您可以使用`abler_config.Config.object_of()`函数引用配置文件中的配置对象，也可以使用`abler_config.Config.value_of()`函数将引用配置文件中的简单配置项。例如：
+您可以使用`ablerConfig.Config.object_of()`函数引用配置文件中的配置对象，也可以使用`ablerConfig.Config.value_of()`函数将引用配置文件中的简单配置项。例如：
 
 ```python
-from abler_config import Config, ConfigNode
+from ablerConfig import Config, ConfigNode
 
 conf = Config.object_of('alarm_control.state_send')
 addr = tuple(Config.value_of('net_gate.tt_addr'))
 ```
```

### Comparing `ablerConfig-0.0.2/README.md` & `ablerConfig-0.0.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 ablerConfig
 =============
 
 简介
 --
 
-这是一个用于处理配置信息的Python包。它可以帮助应用程序读取、写入和验证配置文件。该包主要是供彭彭自用的。
+这是一个用于处理配置信息的Python包。它可以帮助应用程序读取、写入和验证配置文件。该包暂时只供彭彭项目组自用。
 
 特点
 --
 
 *   支持JSON5格式的配置文件。
 *   可以验证配置文件的格式和内容。
 *   可以使用默认值填充缺失的配置项。
 *   可以将配置文件转换为Python对象，以便更方便地访问和修改。
-*   可以将Python对象转换为配置文件。
+*   支持内部配置文件和本地外部配置文件。
 
 依赖项
 ---
 
 *   pyjson5
 *   json5
 
@@ -31,25 +31,25 @@
 ```
 
 使用方法
 ----
 
 ### 加载配置文件
 
-您可以使用`abler_config.Config()`函数加载配置文件。例如：
+您可以使用`ablerConfig.Config()`函数加载配置文件。例如：
 
 ```python
 import ablerConfig as config
 config.Config(default='my-config', show_message=my_show_message)
 ```
 
 ### 引用配置项
 
-您可以使用`abler_config.Config.object_of()`函数引用配置文件中的配置对象，也可以使用`abler_config.Config.value_of()`函数将引用配置文件中的简单配置项。例如：
+您可以使用`ablerConfig.Config.object_of()`函数引用配置文件中的配置对象，也可以使用`ablerConfig.Config.value_of()`函数将引用配置文件中的简单配置项。例如：
 
 ```python
-from abler_config import Config, ConfigNode
+from ablerConfig import Config, ConfigNode
 
 conf = Config.object_of('alarm_control.state_send')
 addr = tuple(Config.value_of('net_gate.tt_addr'))
 ```
```

### Comparing `ablerConfig-0.0.2/abler-config/config.py` & `ablerConfig-0.0.8/ablerConfig/config.py`

 * *Files identical despite different names*

### Comparing `ablerConfig-0.0.2/ablerConfig.egg-info/PKG-INFO` & `ablerConfig-0.0.8/ablerConfig.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ablerConfig
-Version: 0.0.2
+Version: 0.0.8
 Summary: 配置信息处理包
 Home-page: https://github.com/hanlaohan/abler-config
 Author: 憨老汉
 Author-email: hh28642257@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -19,24 +19,24 @@
 
 ablerConfig
 =============
 
 简介
 --
 
-这是一个用于处理配置信息的Python包。它可以帮助应用程序读取、写入和验证配置文件。该包主要是供彭彭自用的。
+这是一个用于处理配置信息的Python包。它可以帮助应用程序读取、写入和验证配置文件。该包暂时只供彭彭项目组自用。
 
 特点
 --
 
 *   支持JSON5格式的配置文件。
 *   可以验证配置文件的格式和内容。
 *   可以使用默认值填充缺失的配置项。
 *   可以将配置文件转换为Python对象，以便更方便地访问和修改。
-*   可以将Python对象转换为配置文件。
+*   支持内部配置文件和本地外部配置文件。
 
 依赖项
 ---
 
 *   pyjson5
 *   json5
 
@@ -50,25 +50,25 @@
 ```
 
 使用方法
 ----
 
 ### 加载配置文件
 
-您可以使用`abler_config.Config()`函数加载配置文件。例如：
+您可以使用`ablerConfig.Config()`函数加载配置文件。例如：
 
 ```python
 import ablerConfig as config
 config.Config(default='my-config', show_message=my_show_message)
 ```
 
 ### 引用配置项
 
-您可以使用`abler_config.Config.object_of()`函数引用配置文件中的配置对象，也可以使用`abler_config.Config.value_of()`函数将引用配置文件中的简单配置项。例如：
+您可以使用`ablerConfig.Config.object_of()`函数引用配置文件中的配置对象，也可以使用`ablerConfig.Config.value_of()`函数将引用配置文件中的简单配置项。例如：
 
 ```python
-from abler_config import Config, ConfigNode
+from ablerConfig import Config, ConfigNode
 
 conf = Config.object_of('alarm_control.state_send')
 addr = tuple(Config.value_of('net_gate.tt_addr'))
 ```
```

### Comparing `ablerConfig-0.0.2/setup.py` & `ablerConfig-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="ablerConfig",
-    version="0.0.2",
+    version="0.0.8",
     author="憨老汉",
     author_email="hh28642257@gmail.com",
     description="配置信息处理包",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hanlaohan/abler-config",
     packages=find_packages(),
```

