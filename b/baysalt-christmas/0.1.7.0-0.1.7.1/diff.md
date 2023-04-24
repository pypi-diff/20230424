# Comparing `tmp/baysalt_christmas-0.1.7.0.tar.gz` & `tmp/baysalt_christmas-0.1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baysalt_christmas-0.1.7.0.tar", last modified: Sat Apr 22 08:23:23 2023, max compression
+gzip compressed data, was "baysalt_christmas-0.1.7.1.tar", last modified: Mon Apr 24 06:23:05 2023, max compression
```

## Comparing `baysalt_christmas-0.1.7.0.tar` & `baysalt_christmas-0.1.7.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-04-22 08:23:23.793805 baysalt_christmas-0.1.7.0/
--rw-r--r--   0 christmas   (501) staff       (20)    10244 2023-04-19 08:43:20.000000 baysalt_christmas-0.1.7.0/.DS_Store
--rw-r--r--   0 christmas   (501) staff       (20)      117 2023-03-25 19:22:27.000000 baysalt_christmas-0.1.7.0/MANIFEST.in
--rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-04-22 08:23:23.793668 baysalt_christmas-0.1.7.0/PKG-INFO
--rw-r--r--   0 christmas   (501) staff       (20)     3732 2023-03-29 03:30:38.000000 baysalt_christmas-0.1.7.0/README.md
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-04-22 08:23:23.788643 baysalt_christmas-0.1.7.0/baysalt_christmas.egg-info/
--rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-04-22 08:23:23.000000 baysalt_christmas-0.1.7.0/baysalt_christmas.egg-info/PKG-INFO
--rw-r--r--   0 christmas   (501) staff       (20)      725 2023-04-22 08:23:23.000000 baysalt_christmas-0.1.7.0/baysalt_christmas.egg-info/SOURCES.txt
--rw-r--r--   0 christmas   (501) staff       (20)        1 2023-04-22 08:23:23.000000 baysalt_christmas-0.1.7.0/baysalt_christmas.egg-info/dependency_links.txt
--rw-r--r--   0 christmas   (501) staff       (20)       21 2023-04-22 08:23:23.000000 baysalt_christmas-0.1.7.0/baysalt_christmas.egg-info/requires.txt
--rw-r--r--   0 christmas   (501) staff       (20)       10 2023-04-22 08:23:23.000000 baysalt_christmas-0.1.7.0/baysalt_christmas.egg-info/top_level.txt
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-04-22 08:23:23.789921 baysalt_christmas-0.1.7.0/christmas/
--rw-r--r--   0 christmas   (501) staff       (20)    18741 2023-04-22 08:22:21.000000 baysalt_christmas-0.1.7.0/christmas/Blog.py
--rw-r--r--   0 christmas   (501) staff       (20)     1895 2023-03-25 02:55:02.000000 baysalt_christmas-0.1.7.0/christmas/S_DateTime.py
--rw-r--r--   0 christmas   (501) staff       (20)      441 2023-04-13 14:13:51.000000 baysalt_christmas-0.1.7.0/christmas/__init__.py
--rw-r--r--   0 christmas   (501) staff       (20)     4094 2023-04-20 13:28:55.000000 baysalt_christmas-0.1.7.0/christmas/commonCode.py
--rw-r--r--   0 christmas   (501) staff       (20)     1638 2023-04-12 07:23:55.000000 baysalt_christmas-0.1.7.0/christmas/cprintf.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-04-22 08:23:23.791300 baysalt_christmas-0.1.7.0/christmas/mncPy/
--rw-r--r--   0 christmas   (501) staff       (20)     1203 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.7.0/christmas/mncPy/.gitignore
--rw-r--r--   0 christmas   (501) staff       (20)    35149 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.7.0/christmas/mncPy/LICENSE
--rw-r--r--   0 christmas   (501) staff       (20)      239 2023-03-03 08:53:41.000000 baysalt_christmas-0.1.7.0/christmas/mncPy/__init__.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-04-22 08:23:23.793323 baysalt_christmas-0.1.7.0/christmas/mncPy/__pycache__/
--rw-r--r--   0 christmas   (501) staff       (20)      228 2023-03-26 18:28:05.000000 baysalt_christmas-0.1.7.0/christmas/mncPy/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)     8964 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.7.0/christmas/mncPy/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)     3411 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.7.0/christmas/mncPy/__pycache__/compress.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)    12920 2023-03-09 13:49:40.000000 baysalt_christmas-0.1.7.0/christmas/mncPy/common.py
--rw-r--r--   0 christmas   (501) staff       (20)     4347 2023-03-09 14:00:22.000000 baysalt_christmas-0.1.7.0/christmas/mncPy/compress.py
--rw-r--r--   0 christmas   (501) staff       (20)     3554 2023-03-29 02:58:20.000000 baysalt_christmas-0.1.7.0/christmas/processBar.py
--rw-r--r--   0 christmas   (501) staff       (20)     3473 2023-04-13 06:21:12.000000 baysalt_christmas-0.1.7.0/christmas/read_conf.py
--rw-r--r--   0 christmas   (501) staff       (20)     1506 2022-12-07 09:44:40.000000 baysalt_christmas-0.1.7.0/christmas/server_info.py
--rw-r--r--   0 christmas   (501) staff       (20)      456 2023-03-25 18:44:30.000000 baysalt_christmas-0.1.7.0/run_twine.py
--rw-r--r--   0 christmas   (501) staff       (20)       38 2023-04-22 08:23:23.793854 baysalt_christmas-0.1.7.0/setup.cfg
--rw-r--r--   0 christmas   (501) staff       (20)      796 2023-04-22 08:23:15.000000 baysalt_christmas-0.1.7.0/setup.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-04-24 06:23:05.209130 baysalt_christmas-0.1.7.1/
+-rw-r--r--   0 christmas   (501) staff       (20)    10244 2023-04-19 08:43:20.000000 baysalt_christmas-0.1.7.1/.DS_Store
+-rw-r--r--   0 christmas   (501) staff       (20)      117 2023-03-25 19:22:27.000000 baysalt_christmas-0.1.7.1/MANIFEST.in
+-rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-04-24 06:23:05.208877 baysalt_christmas-0.1.7.1/PKG-INFO
+-rw-r--r--   0 christmas   (501) staff       (20)     3732 2023-03-29 03:30:38.000000 baysalt_christmas-0.1.7.1/README.md
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-04-24 06:23:05.199684 baysalt_christmas-0.1.7.1/baysalt_christmas.egg-info/
+-rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-04-24 06:23:05.000000 baysalt_christmas-0.1.7.1/baysalt_christmas.egg-info/PKG-INFO
+-rw-r--r--   0 christmas   (501) staff       (20)      729 2023-04-24 06:23:05.000000 baysalt_christmas-0.1.7.1/baysalt_christmas.egg-info/SOURCES.txt
+-rw-r--r--   0 christmas   (501) staff       (20)        1 2023-04-24 06:23:05.000000 baysalt_christmas-0.1.7.1/baysalt_christmas.egg-info/dependency_links.txt
+-rw-r--r--   0 christmas   (501) staff       (20)       21 2023-04-24 06:23:05.000000 baysalt_christmas-0.1.7.1/baysalt_christmas.egg-info/requires.txt
+-rw-r--r--   0 christmas   (501) staff       (20)       10 2023-04-24 06:23:05.000000 baysalt_christmas-0.1.7.1/baysalt_christmas.egg-info/top_level.txt
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-04-24 06:23:05.202355 baysalt_christmas-0.1.7.1/christmas/
+-rw-r--r--   0 christmas   (501) staff       (20)    20394 2023-04-24 06:22:46.000000 baysalt_christmas-0.1.7.1/christmas/Blogging.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1895 2023-03-25 02:55:02.000000 baysalt_christmas-0.1.7.1/christmas/S_DateTime.py
+-rw-r--r--   0 christmas   (501) staff       (20)      445 2023-04-23 12:43:18.000000 baysalt_christmas-0.1.7.1/christmas/__init__.py
+-rw-r--r--   0 christmas   (501) staff       (20)     4526 2023-04-24 06:14:31.000000 baysalt_christmas-0.1.7.1/christmas/commonCode.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1638 2023-04-12 07:23:55.000000 baysalt_christmas-0.1.7.1/christmas/cprintf.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-04-24 06:23:05.206308 baysalt_christmas-0.1.7.1/christmas/mncPy/
+-rw-r--r--   0 christmas   (501) staff       (20)     1203 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.7.1/christmas/mncPy/.gitignore
+-rw-r--r--   0 christmas   (501) staff       (20)    35149 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.7.1/christmas/mncPy/LICENSE
+-rw-r--r--   0 christmas   (501) staff       (20)      239 2023-03-03 08:53:41.000000 baysalt_christmas-0.1.7.1/christmas/mncPy/__init__.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-04-24 06:23:05.208418 baysalt_christmas-0.1.7.1/christmas/mncPy/__pycache__/
+-rw-r--r--   0 christmas   (501) staff       (20)      228 2023-03-26 18:28:05.000000 baysalt_christmas-0.1.7.1/christmas/mncPy/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)     8964 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.7.1/christmas/mncPy/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)     3411 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.7.1/christmas/mncPy/__pycache__/compress.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)    12920 2023-03-09 13:49:40.000000 baysalt_christmas-0.1.7.1/christmas/mncPy/common.py
+-rw-r--r--   0 christmas   (501) staff       (20)     4347 2023-03-09 14:00:22.000000 baysalt_christmas-0.1.7.1/christmas/mncPy/compress.py
+-rw-r--r--   0 christmas   (501) staff       (20)     3554 2023-03-29 02:58:20.000000 baysalt_christmas-0.1.7.1/christmas/processBar.py
+-rw-r--r--   0 christmas   (501) staff       (20)     3473 2023-04-13 06:21:12.000000 baysalt_christmas-0.1.7.1/christmas/read_conf.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1506 2022-12-07 09:44:40.000000 baysalt_christmas-0.1.7.1/christmas/server_info.py
+-rw-r--r--   0 christmas   (501) staff       (20)      456 2023-03-25 18:44:30.000000 baysalt_christmas-0.1.7.1/run_twine.py
+-rw-r--r--   0 christmas   (501) staff       (20)       38 2023-04-24 06:23:05.209215 baysalt_christmas-0.1.7.1/setup.cfg
+-rw-r--r--   0 christmas   (501) staff       (20)      796 2023-04-24 06:23:01.000000 baysalt_christmas-0.1.7.1/setup.py
```

### Comparing `baysalt_christmas-0.1.7.0/.DS_Store` & `baysalt_christmas-0.1.7.1/.DS_Store`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.0/PKG-INFO` & `baysalt_christmas-0.1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baysalt_christmas
-Version: 0.1.7.0
+Version: 0.1.7.1
 Summary: Some simple tools for Christmas
 Author: Christmas
 Author-email: 273519355@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `baysalt_christmas-0.1.7.0/README.md` & `baysalt_christmas-0.1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.0/baysalt_christmas.egg-info/PKG-INFO` & `baysalt_christmas-0.1.7.1/baysalt_christmas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baysalt-christmas
-Version: 0.1.7.0
+Version: 0.1.7.1
 Summary: Some simple tools for Christmas
 Author: Christmas
 Author-email: 273519355@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `baysalt_christmas-0.1.7.0/baysalt_christmas.egg-info/SOURCES.txt` & `baysalt_christmas-0.1.7.1/baysalt_christmas.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 run_twine.py
 setup.py
 baysalt_christmas.egg-info/PKG-INFO
 baysalt_christmas.egg-info/SOURCES.txt
 baysalt_christmas.egg-info/dependency_links.txt
 baysalt_christmas.egg-info/requires.txt
 baysalt_christmas.egg-info/top_level.txt
-christmas/Blog.py
+christmas/Blogging.py
 christmas/S_DateTime.py
 christmas/__init__.py
 christmas/commonCode.py
 christmas/cprintf.py
 christmas/processBar.py
 christmas/read_conf.py
 christmas/server_info.py
```

### Comparing `baysalt_christmas-0.1.7.0/christmas/Blog.py` & `baysalt_christmas-0.1.7.1/christmas/Blogging.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 """
 
 """
 
 import logging
 import colorlog
 import datetime
-from christmas import rmfiles
+from christmas import rmfiles, whether_instanced
 from logging.handlers import RotatingFileHandler, TimedRotatingFileHandler
 
 
 class Blog:
     """
     先创建日志记录器（logging.getLogger），然后再设置日志级别（logger.setLevel），
     接着再创建日志文件，也就是日志保存的地方（logging.FileHandler），然后再设置日志格式（logging.Formatter），
@@ -308,57 +308,112 @@
         logging.addLevelName(level, levelName)
     
     @staticmethod
     def getLevelName(level):
         return logging.getLevelName(level)
 
 
+def debug(msg, *args, **kwargs):
+    TF, instanced = whether_instanced(Blog)
+    if TF:
+        instanced[instanced.keys()[0]].logger.debug(msg, *args, **kwargs)
+    else:
+        Blog().logger.debug(msg, *args, **kwargs)
+
+
+def info(msg, *args, **kwargs):
+    TF, instanced = whether_instanced(Blog)
+    if TF:
+        instanced[instanced.keys()[0]].logger.info(msg, *args, **kwargs)
+    else:
+        Blog().logger.info(msg, *args, **kwargs)
+
+
+def warning(msg, *args, **kwargs):
+    TF, instanced = whether_instanced(Blog)
+    if TF:
+        instanced[instanced.keys()[0]].logger.warning(msg, *args, **kwargs)
+    else:
+        Blog().logger.warning(msg, *args, **kwargs)
+
+
+def error(msg, *args, **kwargs):
+    TF, instanced = whether_instanced(Blog)
+    if TF:
+        instanced[instanced.keys()[0]].logger.error(msg, *args, **kwargs)
+    else:
+        Blog().logger.error(msg, *args, **kwargs)
+
+
+def critical(msg, *args, **kwargs):
+    TF, instanced = whether_instanced(Blog)
+    if TF:
+        instanced[instanced.keys()[0]].logger.critical(msg, *args, **kwargs)
+    else:
+        Blog().logger.critical(msg, *args, **kwargs)
+
+
+def exception(msg, *args, **kwargs):
+    TF, instanced = whether_instanced(Blog)
+    if TF:
+        instanced[instanced.keys()[0]].logger.exception(msg, *args, **kwargs)
+    else:
+        Blog().logger.exception(msg, *args, **kwargs)
+
+
+def log(level, msg, *args, **kwargs):
+    TF, instanced = whether_instanced(Blog)
+    if TF:
+        instanced[instanced.keys()[0]].logger.log(level, msg, *args, **kwargs)
+    else:
+        Blog().logger.log(level, msg, *args, **kwargs)
+
+
 def example_Blog():
-    log = Blog(_loger_name='Christmas',  # 日志收集器名称
-               _log_filename='ChristmasWRITING',  # 日志文件名前缀
-               _switch_write_all_log=True,  # 是否写入全部日志 ALL.log
-               _switch_write_error_plus_log=True,  # 是否写入错误日志 BUG.log
-               _switch_print_log=True,  # 是否打印日志到控制台
-               _switch_write_debug_log=True,  # 是否写入debug日志
-               _switch_write_info_log=True,  # 是否写入info日志
-               _switch_write_warning_log=True,  # 是否写入warning日志
-               _switch_write_error_log=True,  # 是否写入error日志
-               _switch_write_critical_log=True,  # 是否写入critical日志
-               )
-    log.addLevelName(15, "CUSTOM")  # 自定义日志级别 15 --> CUSTOM
-    log.setup_Blog(write_mode='w')  # 日志写入模式
-    log.setup_Blog(maxBytes=1024 * 1024 * 5)  # 日志文件大小
-    log.setup_Blog(backupCount=5)  # 日志文件数量
-    log.setup_Blog(log_level=1)  # 日志级别
-    log.setup_Blog(log_ddt_fmt='%Y-%m-%d %H:%M:%S')  # 日志时间格式
-    log.setup_Blog(colors_config={
+    log2 = Blog(_loger_name='Christmas',  # 日志收集器名称
+                _log_filename='ChristmasWRITING',  # 日志文件名前缀
+                _switch_write_all_log=True,  # 是否写入全部日志 ALL.log
+                _switch_write_error_plus_log=True,  # 是否写入错误日志 BUG.log
+                _switch_print_log=True,  # 是否打印日志到控制台
+                _switch_write_debug_log=True,  # 是否写入debug日志
+                _switch_write_info_log=True,  # 是否写入info日志
+                _switch_write_warning_log=True,  # 是否写入warning日志
+                _switch_write_error_log=True,  # 是否写入error日志
+                _switch_write_critical_log=True,  # 是否写入critical日志
+                )
+    log2.addLevelName(15, "CUSTOM")  # 自定义日志级别 15 --> CUSTOM
+    log2.setup_Blog(write_mode='w')  # 日志写入模式
+    log2.setup_Blog(maxBytes=1024 * 1024 * 5)  # 日志文件大小
+    log2.setup_Blog(backupCount=5)  # 日志文件数量
+    log2.setup_Blog(log_level=1)  # 日志级别
+    log2.setup_Blog(log_ddt_fmt='%Y-%m-%d %H:%M:%S')  # 日志时间格式
+    log2.setup_Blog(colors_config={
         "CUSTOM": "yellow",
         'DEBUG': 'cyan',
         'INFO': 'blue',
         'WARNING': 'yellow',
         'ERROR': 'red',
         'CRITICAL': 'purple',
         'EXCEPTION': 'red'})  # 日志颜色配置
-    log.setup_Blog(Rotating='time')  # 日志切割模式
-    log.setup_Blog(when='D')  # 日志切割时间
-    log.setup_Blog(interval=1)  # 日志切割间隔
-    x = log.console()  # 日志收集器
+    log2.setup_Blog(Rotating='time')  # 日志切割模式
+    log2.setup_Blog(when='D')  # 日志切割时间
+    log2.setup_Blog(interval=1)  # 日志切割间隔
+    x = log2.console()  # 日志收集器
     x.debug("这是debug信息")  # 日志输出
     x.log(15, "CUSTOM")  # 自定义日志级别
     x.info("这是日志信息")  # 日志输出
     x.warning("这是警告信息")  # 日志输出
     x.error("这是错误日志信息")  # 日志输出
     x.critical("这是严重级别信息")  # 日志输出
 
 
 def example_Blog_simple():
-    log = Blog()
-    log.logger.debug("这是debug信息")
-    log.logger.info("这是日志信息")
-    log.logger.warning("这是警告信息")
-    log.logger.error("这是错误日志信息")
-    log.logger.critical("这是严重级别信息")
+    log1 = Blog()
+    log1.logger.debug("这是debug信息")
+    log1.logger.info("这是日志信息")
+    log1.logger.warning("这是警告信息")
+    log1.logger.error("这是错误日志信息")
+    log1.logger.critical("这是严重级别信息")
 
 
 if __name__ == '__main__':
     example_Blog_simple()
-
```

### Comparing `baysalt_christmas-0.1.7.0/christmas/S_DateTime.py` & `baysalt_christmas-0.1.7.1/christmas/S_DateTime.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.0/christmas/commonCode.py` & `baysalt_christmas-0.1.7.1/christmas/commonCode.py`

 * *Files 10% similar despite different names*

```diff
@@ -151,7 +151,25 @@
     def inside(self):
         t1 = time.time()
         func(self)
         t2 = time.time()
         print('task time:{:.2f}s'.format(t2 - t1))
 
     return inside
+
+
+def whether_instanced(_class):
+    """
+    判断是否被实例化
+    :param _class: 类名
+    """
+    has_instance = False
+    instanced = {}
+    instances = globals().copy()
+    for var_name, var_value in instances.items():
+        if isinstance(var_value, _class):
+            has_instance = True
+            instanced[var_name] = var_value
+        else:
+            has_instance = False
+
+    return has_instance, instanced
```

### Comparing `baysalt_christmas-0.1.7.0/christmas/cprintf.py` & `baysalt_christmas-0.1.7.1/christmas/cprintf.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.0/christmas/mncPy/.gitignore` & `baysalt_christmas-0.1.7.1/christmas/mncPy/.gitignore`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.0/christmas/mncPy/LICENSE` & `baysalt_christmas-0.1.7.1/christmas/mncPy/LICENSE`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.0/christmas/mncPy/__pycache__/common.cpython-39.pyc` & `baysalt_christmas-0.1.7.1/christmas/mncPy/__pycache__/common.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.0/christmas/mncPy/__pycache__/compress.cpython-39.pyc` & `baysalt_christmas-0.1.7.1/christmas/mncPy/__pycache__/compress.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.0/christmas/mncPy/common.py` & `baysalt_christmas-0.1.7.1/christmas/mncPy/common.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.0/christmas/mncPy/compress.py` & `baysalt_christmas-0.1.7.1/christmas/mncPy/compress.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.0/christmas/processBar.py` & `baysalt_christmas-0.1.7.1/christmas/processBar.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.0/christmas/read_conf.py` & `baysalt_christmas-0.1.7.1/christmas/read_conf.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.0/christmas/server_info.py` & `baysalt_christmas-0.1.7.1/christmas/server_info.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.0/setup.py` & `baysalt_christmas-0.1.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="baysalt_christmas",
-    version="0.1.7.0",
+    version="0.1.7.1",
     author="Christmas",
     author_email="273519355@qq.com",
     description="Some simple tools for Christmas",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     include_package_data=True,
```

