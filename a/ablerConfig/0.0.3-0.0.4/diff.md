# Comparing `tmp/ablerConfig-0.0.3-py3-none-any.whl.zip` & `tmp/ablerConfig-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,7 @@
-Zip file size: 5458 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-23 21:26 ablerConfig/__init__.py
--rw-rw-rw-  2.0 fat    12706 b- defN 23-Apr-22 20:35 ablerConfig/config.py
--rw-rw-rw-  2.0 fat     2039 b- defN 23-Apr-23 22:11 ablerConfig-0.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-23 22:11 ablerConfig-0.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-Apr-23 22:11 ablerConfig-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      470 b- defN 23-Apr-23 22:11 ablerConfig-0.0.3.dist-info/RECORD
-6 files, 15319 bytes uncompressed, 4604 bytes compressed:  69.9%
+Zip file size: 2105 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat       13 b- defN 23-Apr-23 23:22 ablerConfig/__init__.py
+-rw-rw-rw-  2.0 fat     2050 b- defN 23-Apr-23 23:31 ablerConfig-0.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-23 23:31 ablerConfig-0.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Apr-23 23:31 ablerConfig-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      392 b- defN 23-Apr-23 23:31 ablerConfig-0.0.4.dist-info/RECORD
+5 files, 2559 bytes uncompressed, 1369 bytes compressed:  46.5%
```

## zipnote {}

```diff
@@ -1,19 +1,16 @@
 Filename: ablerConfig/__init__.py
 Comment: 
 
-Filename: ablerConfig/config.py
+Filename: ablerConfig-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: ablerConfig-0.0.3.dist-info/METADATA
+Filename: ablerConfig-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: ablerConfig-0.0.3.dist-info/WHEEL
+Filename: ablerConfig-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: ablerConfig-0.0.3.dist-info/top_level.txt
-Comment: 
-
-Filename: ablerConfig-0.0.3.dist-info/RECORD
+Filename: ablerConfig-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ablerConfig/__init__.py

```diff
@@ -0,0 +1 @@
+00000000: 696d 706f 7274 2063 6f6e 6669 67         import config
```

## Comparing `ablerConfig-0.0.3.dist-info/METADATA` & `ablerConfig-0.0.4.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ablerConfig
-Version: 0.0.3
+Version: 0.0.4
 Summary: 配置信息处理包
 Home-page: https://github.com/hanlaohan/abler-config
 Author: 憨老汉
 Author-email: hh28642257@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -21,24 +21,24 @@
 
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
 
@@ -52,25 +52,25 @@
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

