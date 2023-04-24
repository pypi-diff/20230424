# Comparing `tmp/ats_case-0.5.9.tar.gz` & `tmp/ats_case-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ats_case-0.5.9.tar", last modified: Sun Apr 23 09:03:53 2023, max compression
+gzip compressed data, was "ats_case-0.6.0.tar", last modified: Mon Apr 24 01:15:06 2023, max compression
```

## Comparing `ats_case-0.5.9.tar` & `ats_case-0.6.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 09:03:53.312601 ats_case-0.5.9/
--rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.5.9/LICENSE
--rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.5.9/MANIFEST.in
--rw-rw-rw-   0        0        0     1042 2023-04-23 09:03:53.310778 ats_case-0.5.9/PKG-INFO
--rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.5.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 09:03:52.763199 ats_case-0.5.9/ats_case/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.5.9/ats_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 09:03:53.009391 ats_case-0.5.9/ats_case/case/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.5.9/ats_case/case/__init__.py
--rw-rw-rw-   0        0        0    17449 2023-04-23 09:01:08.000000 ats_case-0.5.9/ats_case/case/command.py
--rw-rw-rw-   0        0        0     9976 2023-04-23 06:01:24.000000 ats_case-0.5.9/ats_case/case/context.py
--rw-rw-rw-   0        0        0     7383 2023-04-23 03:03:58.000000 ats_case-0.5.9/ats_case/case/executor.py
--rw-rw-rw-   0        0        0     5549 2023-04-23 08:37:16.000000 ats_case-0.5.9/ats_case/case/translator.py
-drwxrwxrwx   0        0        0        0 2023-04-23 09:03:53.159988 ats_case-0.5.9/ats_case/common/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.5.9/ats_case/common/__init__.py
--rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.5.9/ats_case/common/enum.py
--rw-rw-rw-   0        0        0      640 2023-04-20 02:04:10.000000 ats_case-0.5.9/ats_case/common/error.py
-drwxrwxrwx   0        0        0        0 2023-04-23 09:03:53.229802 ats_case-0.5.9/ats_case/manage/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.5.9/ats_case/manage/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-03-03 01:15:16.000000 ats_case-0.5.9/ats_case/manage/core.py
--rw-rw-rw-   0        0        0     2953 2023-04-20 07:40:35.000000 ats_case-0.5.9/ats_case/manage/start.py
-drwxrwxrwx   0        0        0        0 2023-04-23 09:03:53.295631 ats_case-0.5.9/ats_case/template/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.5.9/ats_case/template/__init__.py
--rw-rw-rw-   0        0        0     2067 2023-04-20 00:58:29.000000 ats_case-0.5.9/ats_case/template/testcase_v1.tmp
-drwxrwxrwx   0        0        0        0 2023-04-23 09:03:52.861781 ats_case-0.5.9/ats_case.egg-info/
--rw-rw-rw-   0        0        0     1042 2023-04-23 09:03:52.000000 ats_case-0.5.9/ats_case.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-04-23 09:03:52.000000 ats_case-0.5.9/ats_case.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 09:03:52.000000 ats_case-0.5.9/ats_case.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-04-23 09:03:52.000000 ats_case-0.5.9/ats_case.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-23 09:03:52.000000 ats_case-0.5.9/ats_case.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 09:03:53.312601 ats_case-0.5.9/setup.cfg
--rw-rw-rw-   0        0        0      935 2023-04-23 09:03:46.000000 ats_case-0.5.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:15:06.025209 ats_case-0.6.0/
+-rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.6.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1042 2023-04-24 01:15:06.022249 ats_case-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 01:15:05.635723 ats_case-0.6.0/ats_case/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.6.0/ats_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:15:05.851400 ats_case-0.6.0/ats_case/case/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.6.0/ats_case/case/__init__.py
+-rw-rw-rw-   0        0        0    17449 2023-04-23 09:01:08.000000 ats_case-0.6.0/ats_case/case/command.py
+-rw-rw-rw-   0        0        0     9976 2023-04-23 06:01:24.000000 ats_case-0.6.0/ats_case/case/context.py
+-rw-rw-rw-   0        0        0     7383 2023-04-23 03:03:58.000000 ats_case-0.6.0/ats_case/case/executor.py
+-rw-rw-rw-   0        0        0     5549 2023-04-24 01:14:40.000000 ats_case-0.6.0/ats_case/case/translator.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:15:05.924205 ats_case-0.6.0/ats_case/common/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.6.0/ats_case/common/__init__.py
+-rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.6.0/ats_case/common/enum.py
+-rw-rw-rw-   0        0        0      640 2023-04-20 02:04:10.000000 ats_case-0.6.0/ats_case/common/error.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:15:05.982349 ats_case-0.6.0/ats_case/manage/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.6.0/ats_case/manage/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-03-03 01:15:16.000000 ats_case-0.6.0/ats_case/manage/core.py
+-rw-rw-rw-   0        0        0     2953 2023-04-20 07:40:35.000000 ats_case-0.6.0/ats_case/manage/start.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:15:06.014238 ats_case-0.6.0/ats_case/template/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.6.0/ats_case/template/__init__.py
+-rw-rw-rw-   0        0        0     2067 2023-04-20 00:58:29.000000 ats_case-0.6.0/ats_case/template/testcase_v1.tmp
+drwxrwxrwx   0        0        0        0 2023-04-24 01:15:05.725484 ats_case-0.6.0/ats_case.egg-info/
+-rw-rw-rw-   0        0        0     1042 2023-04-24 01:15:04.000000 ats_case-0.6.0/ats_case.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-04-24 01:15:04.000000 ats_case-0.6.0/ats_case.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 01:15:04.000000 ats_case-0.6.0/ats_case.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-04-24 01:15:04.000000 ats_case-0.6.0/ats_case.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-24 01:15:04.000000 ats_case-0.6.0/ats_case.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 01:15:06.025209 ats_case-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0      935 2023-04-24 01:14:56.000000 ats_case-0.6.0/setup.py
```

### Comparing `ats_case-0.5.9/PKG-INFO` & `ats_case-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats_case
-Version: 0.5.9
+Version: 0.6.0
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.5.9/README.md` & `ats_case-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.9/ats_case/case/command.py` & `ats_case-0.6.0/ats_case/case/command.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.9/ats_case/case/context.py` & `ats_case-0.6.0/ats_case/case/context.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.9/ats_case/case/executor.py` & `ats_case-0.6.0/ats_case/case/executor.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.9/ats_case/case/translator.py` & `ats_case-0.6.0/ats_case/case/translator.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
         return script_file
 
     def _gen_import(self):
         return 'from ats_case.case import command' + self.LINE + 'from ats_case.case.context import Context' + self.LINE
 
     def _gen_step(self, step: int, op: dict):
-        return '@command.step_annotation(desc={}){}'.format(op.get('desc', '""'), self.LINE) + \
+        return '@command.step_annotation(desc="{}"){}'.format(op.get('desc', ''), self.LINE) + \
                'def step_{}(context: Context):{}'.format(step, self.LINE)
 
     def _gen_tab(self, count: int):
         ts = ''
         for i in range(count):
             ts += self.TAB
```

### Comparing `ats_case-0.5.9/ats_case/common/error.py` & `ats_case-0.6.0/ats_case/common/error.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.9/ats_case/manage/core.py` & `ats_case-0.6.0/ats_case/manage/core.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.9/ats_case/manage/start.py` & `ats_case-0.6.0/ats_case/manage/start.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.9/ats_case/template/testcase_v1.tmp` & `ats_case-0.6.0/ats_case/template/testcase_v1.tmp`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.9/ats_case.egg-info/PKG-INFO` & `ats_case-0.6.0/ats_case.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats-case
-Version: 0.5.9
+Version: 0.6.0
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.5.9/ats_case.egg-info/SOURCES.txt` & `ats_case-0.6.0/ats_case.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.9/setup.py` & `ats_case-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ats_case",
-    version="0.5.9",
+    version="0.6.0",
     py_modules=['ats_case'],
     author="zhangyue",
     author_email="zhangyue@techen.cn",
     description="Test Script Development Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/henry9000/ats_case",
```

