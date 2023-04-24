# Comparing `tmp/Zeraora-0.2.3.tar.gz` & `tmp/Zeraora-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Zeraora-0.2.3.tar", last modified: Fri Apr 21 10:09:37 2023, max compression
+gzip compressed data, was "dist/Zeraora-0.2.4.tar", last modified: Mon Apr 24 09:14:35 2023, max compression
```

## Comparing `Zeraora-0.2.3.tar` & `Zeraora-0.2.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:09:37.000000 Zeraora-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-21 10:09:37.000000 Zeraora-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-21 10:09:26.000000 Zeraora-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:09:37.000000 Zeraora-0.2.3/Zeraora.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-21 10:09:36.000000 Zeraora-0.2.3/Zeraora.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-21 10:09:37.000000 Zeraora-0.2.3/Zeraora.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 10:09:36.000000 Zeraora-0.2.3/Zeraora.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-21 10:09:36.000000 Zeraora-0.2.3/Zeraora.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 10:09:37.000000 Zeraora-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-21 10:09:26.000000 Zeraora-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:09:37.000000 Zeraora-0.2.3/zeraora/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-21 10:09:26.000000 Zeraora-0.2.3/zeraora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-21 10:09:26.000000 Zeraora-0.2.3/zeraora/charsets.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-21 10:09:26.000000 Zeraora-0.2.3/zeraora/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:09:37.000000 Zeraora-0.2.3/zeraora/djangobase/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-21 10:09:26.000000 Zeraora-0.2.3/zeraora/djangobase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-04-21 10:09:26.000000 Zeraora-0.2.3/zeraora/djangobase/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-04-21 10:09:26.000000 Zeraora-0.2.3/zeraora/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-21 10:09:26.000000 Zeraora-0.2.3/zeraora/math.py
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-04-21 10:09:26.000000 Zeraora-0.2.3/zeraora/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-04-21 10:09:26.000000 Zeraora-0.2.3/zeraora/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:35.000000 Zeraora-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-24 09:14:35.000000 Zeraora-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-24 09:14:10.000000 Zeraora-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:35.000000 Zeraora-0.2.4/Zeraora.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-24 09:14:34.000000 Zeraora-0.2.4/Zeraora.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-24 09:14:35.000000 Zeraora-0.2.4/Zeraora.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 09:14:34.000000 Zeraora-0.2.4/Zeraora.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-24 09:14:34.000000 Zeraora-0.2.4/Zeraora.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 09:14:35.000000 Zeraora-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-24 09:14:10.000000 Zeraora-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:35.000000 Zeraora-0.2.4/zeraora/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-24 09:14:10.000000 Zeraora-0.2.4/zeraora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-24 09:14:10.000000 Zeraora-0.2.4/zeraora/charsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-24 09:14:10.000000 Zeraora-0.2.4/zeraora/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:35.000000 Zeraora-0.2.4/zeraora/djangobase/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-24 09:14:10.000000 Zeraora-0.2.4/zeraora/djangobase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-04-24 09:14:10.000000 Zeraora-0.2.4/zeraora/djangobase/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-04-24 09:14:10.000000 Zeraora-0.2.4/zeraora/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-24 09:14:10.000000 Zeraora-0.2.4/zeraora/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-04-24 09:14:10.000000 Zeraora-0.2.4/zeraora/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10314 2023-04-24 09:14:10.000000 Zeraora-0.2.4/zeraora/typing.py
```

### Comparing `Zeraora-0.2.3/PKG-INFO` & `Zeraora-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Zeraora
-Version: 0.2.3
+Version: 0.2.4
 Summary: 一个包含原创工具类及快捷函数的工具库。A original utility Python package.
 Home-page: https://github.com/aixcyi/zeraora
 Author: aixcyi
 Author-email: 75880483+aixcyi@users.noreply.github.com
 License: MIT
 Project-URL: Source, https://github.com/aixcyi/zeraora
 Project-URL: Tracker, https://github.com/aixcyi/zeraora/issues
```

### Comparing `Zeraora-0.2.3/README.md` & `Zeraora-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.3/Zeraora.egg-info/PKG-INFO` & `Zeraora-0.2.4/Zeraora.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Zeraora
-Version: 0.2.3
+Version: 0.2.4
 Summary: 一个包含原创工具类及快捷函数的工具库。A original utility Python package.
 Home-page: https://github.com/aixcyi/zeraora
 Author: aixcyi
 Author-email: 75880483+aixcyi@users.noreply.github.com
 License: MIT
 Project-URL: Source, https://github.com/aixcyi/zeraora
 Project-URL: Tracker, https://github.com/aixcyi/zeraora/issues
```

### Comparing `Zeraora-0.2.3/setup.py` & `Zeraora-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.3/zeraora/charsets.py` & `Zeraora-0.2.4/zeraora/charsets.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.3/zeraora/decorators.py` & `Zeraora-0.2.4/zeraora/decorators.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.3/zeraora/djangobase/mixins.py` & `Zeraora-0.2.4/zeraora/djangobase/mixins.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.3/zeraora/generators.py` & `Zeraora-0.2.4/zeraora/generators.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.3/zeraora/time.py` & `Zeraora-0.2.4/zeraora/time.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.3/zeraora/typing.py` & `Zeraora-0.2.4/zeraora/typing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 类型相关。
 """
 
 import datetime
 import json
+import re
 from typing import Callable, Type, Union
 from uuid import UUID
 
 
 class OnionObject(object):
 
     def __translate_list(self, items: list) -> list:
@@ -257,7 +258,45 @@
             pk = self.id
         else:
             return ''
         return pk if isinstance(pk, str) else represent(pk)
 
     def _obtain_kls(self) -> str:
         return self.__class__.__name__
+
+
+def datasize(literal: str) -> Union[int, float]:
+    """
+    将一个字面量转换为字节数目。
+
+    支持的单位包括：
+      - B、b
+      - KB、KiB、Kb、Kib
+      - MB、MiB、Mb、Mib
+      - GB、GiB、Gb、Gib
+      - TB、TiB、Tb、Tib
+      - 以此类推……
+
+    - 1 B == 8 b
+    - 1 MB == 1000 KB
+    - 1 MiB == 1024 KiB
+
+    :param literal: 一个整数后缀数据大小的单位。
+    :return:
+    """
+    if not isinstance(literal, str):
+        raise TypeError(
+            '不支持解析一个非字符串类型的值。'
+        )
+
+    pattern = re.compile(r'^([0-9]+)\s*([KMGTPEZY]?)(i?[Bb])$')
+    result = re.fullmatch(pattern, literal)
+
+    if result is None:
+        return 0
+
+    base = int(result.group(1))
+    shift = 'BKMGTPEZY'.index(result.group(2))
+    power = (1024 if 'i' in result.group(3) else 1000) ** shift
+    power = (power / 8) if 'b' in result.group(3) else power
+
+    return base * power
```

