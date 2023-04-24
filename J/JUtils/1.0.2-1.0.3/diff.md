# Comparing `tmp/JUtils-1.0.2.tar.gz` & `tmp/JUtils-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JUtils-1.0.2.tar", last modified: Mon Apr 24 19:25:14 2023, max compression
+gzip compressed data, was "JUtils-1.0.3.tar", last modified: Mon Apr 24 19:38:35 2023, max compression
```

## Comparing `JUtils-1.0.2.tar` & `JUtils-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 19:25:14.685768 JUtils-1.0.2/
--rw-rw-rw-   0        0        0     1072 2022-12-25 18:22:55.000000 JUtils-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     8894 2023-04-24 19:25:14.684769 JUtils-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     8448 2023-04-24 19:24:15.000000 JUtils-1.0.2/README.md
--rw-rw-rw-   0        0        0      522 2023-04-24 19:24:44.000000 JUtils-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-24 19:25:14.685768 JUtils-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-24 19:25:14.661541 JUtils-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-24 19:25:14.672258 JUtils-1.0.2/src/JUtils/
--rw-rw-rw-   0        0        0     1723 2023-04-24 19:24:12.000000 JUtils-1.0.2/src/JUtils/AutoDoc.py
--rw-rw-rw-   0        0        0     2188 2023-04-24 18:55:53.000000 JUtils-1.0.2/src/JUtils/JArr.py
--rw-rw-rw-   0        0        0     8610 2023-04-24 18:55:59.000000 JUtils-1.0.2/src/JUtils/JColors.py
--rw-rw-rw-   0        0        0      110 2023-04-24 18:56:06.000000 JUtils-1.0.2/src/JUtils/JConst.py
--rw-rw-rw-   0        0        0     3307 2023-04-24 18:56:14.000000 JUtils-1.0.2/src/JUtils/JConv.py
--rw-rw-rw-   0        0        0     1153 2023-04-24 18:56:22.000000 JUtils-1.0.2/src/JUtils/JNum.py
--rw-rw-rw-   0        0        0      650 2023-04-24 18:56:27.000000 JUtils-1.0.2/src/JUtils/JOut.py
--rw-rw-rw-   0        0        0     2128 2023-04-24 18:56:32.000000 JUtils-1.0.2/src/JUtils/JStr.py
--rw-rw-rw-   0        0        0        0 2023-01-05 20:19:20.000000 JUtils-1.0.2/src/JUtils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 19:25:14.683768 JUtils-1.0.2/src/JUtils.egg-info/
--rw-rw-rw-   0        0        0     8894 2023-04-24 19:25:14.000000 JUtils-1.0.2/src/JUtils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2023-04-24 19:25:14.000000 JUtils-1.0.2/src/JUtils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 19:25:14.000000 JUtils-1.0.2/src/JUtils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-24 19:25:14.000000 JUtils-1.0.2/src/JUtils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 19:38:35.291995 JUtils-1.0.3/
+-rw-rw-rw-   0        0        0     1072 2022-12-25 18:22:55.000000 JUtils-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     8894 2023-04-24 19:38:35.291995 JUtils-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     8448 2023-04-24 19:24:15.000000 JUtils-1.0.3/README.md
+-rw-rw-rw-   0        0        0      522 2023-04-24 19:37:48.000000 JUtils-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-24 19:38:35.291995 JUtils-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-24 19:38:35.258751 JUtils-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-24 19:38:35.277485 JUtils-1.0.3/src/JUtils/
+-rw-rw-rw-   0        0        0     1915 2023-04-24 19:37:30.000000 JUtils-1.0.3/src/JUtils/AutoDoc.py
+-rw-rw-rw-   0        0        0     2188 2023-04-24 18:55:53.000000 JUtils-1.0.3/src/JUtils/JArr.py
+-rw-rw-rw-   0        0        0     8610 2023-04-24 18:55:59.000000 JUtils-1.0.3/src/JUtils/JColors.py
+-rw-rw-rw-   0        0        0      110 2023-04-24 18:56:06.000000 JUtils-1.0.3/src/JUtils/JConst.py
+-rw-rw-rw-   0        0        0     3307 2023-04-24 18:56:14.000000 JUtils-1.0.3/src/JUtils/JConv.py
+-rw-rw-rw-   0        0        0     1153 2023-04-24 18:56:22.000000 JUtils-1.0.3/src/JUtils/JNum.py
+-rw-rw-rw-   0        0        0      650 2023-04-24 18:56:27.000000 JUtils-1.0.3/src/JUtils/JOut.py
+-rw-rw-rw-   0        0        0     2128 2023-04-24 18:56:32.000000 JUtils-1.0.3/src/JUtils/JStr.py
+-rw-rw-rw-   0        0        0        0 2023-01-05 20:19:20.000000 JUtils-1.0.3/src/JUtils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 19:38:35.290994 JUtils-1.0.3/src/JUtils.egg-info/
+-rw-rw-rw-   0        0        0     8894 2023-04-24 19:38:35.000000 JUtils-1.0.3/src/JUtils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2023-04-24 19:38:35.000000 JUtils-1.0.3/src/JUtils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 19:38:35.000000 JUtils-1.0.3/src/JUtils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-24 19:38:35.000000 JUtils-1.0.3/src/JUtils.egg-info/top_level.txt
```

### Comparing `JUtils-1.0.2/LICENSE` & `JUtils-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `JUtils-1.0.2/PKG-INFO` & `JUtils-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JUtils
-Version: 1.0.2
+Version: 1.0.3
 Summary: Package containing various utility functions i needed now and then, that i wanted to share
 Author-email: Jan Seifert <jan@seifert-online.de>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `JUtils-1.0.2/README.md` & `JUtils-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `JUtils-1.0.2/pyproject.toml` & `JUtils-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "JUtils"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Jan Seifert", email="jan@seifert-online.de" },
 ]
 description = "Package containing various utility functions i needed now and then, that i wanted to share"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `JUtils-1.0.2/src/JUtils/AutoDoc.py` & `JUtils-1.0.3/src/JUtils/AutoDoc.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,54 @@
-import os
-from inspect import getmembers, isfunction
-from json import dumps
-
-#######################################################
-
-foldername = __file__.split("\\")[-2]
-
-dataStruct = {foldername : {}}
-
-for file in os.listdir():
-    if file.endswith(".py"):
-        if file not in ["__init__.py", __file__.split("\\")[-1]]:
-            dataStruct[foldername][file.replace(".py", "")] = {}
-
-for package in dataStruct[foldername].keys():
-    exec(f"import {package}")
-    exec(f"dataStruct[foldername][package]['doc'] = {package}.__doc__")
-
-    dataStruct[foldername][package]["funcs"] = {}
-    funclist = []
-    exec(f"funclist = getmembers({package}, isfunction)")
-    for name, func in funclist:
-        dataStruct[foldername][package]["funcs"][name] = func.__doc__
-
-#print(dumps(dataStruct, indent=4))
-#######################################################
-
-readme = f"# {foldername}\n"
-with open("ModuleStart.txt", "r") as f2:
-        readme += f2.read() + "\n\n"
-
-readme += "# Table of Contents\n"
-count = 1
-for package in dataStruct[foldername].keys():
-    readme += f"## {str(count)}. [{package}](#{foldername}.{package})\n"
-    count += 1
-readme += "\n"
-
-for package, info in dataStruct[foldername].items():
-    readme += f"# {package}\n{info['doc']}.\n```py\nfrom {foldername}.{package} import *\n```\n\n"
-    for func, funcINFO in info["funcs"].items():
-        readme += f"- **{func}**\n```{funcINFO}.\n```\n"
-with open("ModuleEnd.txt", "r") as f3:
-    readme += f3.read()
-
-#print(readme)
-#######################################################
-
-if os.path.exists("README.md"):
-    os.remove("README.md")
-with open("README.md", "x") as f:
-    f.write(readme)
+if __name__ == "__main__":
+    import os
+    from inspect import getmembers, isfunction
+    from json import dumps
+
+    #######################################################
+
+    foldername = __file__.split("\\")[-2]
+
+    dataStruct = {foldername : {}}
+
+    for file in os.listdir():
+        if file.endswith(".py"):
+            if file not in ["__init__.py", __file__.split("\\")[-1]]:
+                dataStruct[foldername][file.replace(".py", "")] = {}
+
+    for package in dataStruct[foldername].keys():
+        exec(f"import {package}")
+        exec(f"dataStruct[foldername][package]['doc'] = {package}.__doc__")
+
+        dataStruct[foldername][package]["funcs"] = {}
+        funclist = []
+        exec(f"funclist = getmembers({package}, isfunction)")
+        for name, func in funclist:
+            dataStruct[foldername][package]["funcs"][name] = func.__doc__
+
+    #print(dumps(dataStruct, indent=4))
+    #######################################################
+
+    readme = f"# {foldername}\n"
+    with open("ModuleStart.txt", "r") as f2:
+            readme += f2.read() + "\n\n"
+
+    readme += "# Table of Contents\n"
+    count = 1
+    for package in dataStruct[foldername].keys():
+        readme += f"## {str(count)}. [{package}](#{foldername}.{package})\n"
+        count += 1
+    readme += "\n"
+
+    for package, info in dataStruct[foldername].items():
+        readme += f"# {package}\n{info['doc']}.\n```py\nfrom {foldername}.{package} import *\n```\n\n"
+        for func, funcINFO in info["funcs"].items():
+            readme += f"- **{func}**\n```{funcINFO}.\n```\n"
+    with open("ModuleEnd.txt", "r") as f3:
+        readme += f3.read()
+
+    #print(readme)
+    #######################################################
+
+    if os.path.exists("README.md"):
+        os.remove("README.md")
+    with open("README.md", "x") as f:
+        f.write(readme)
```

### Comparing `JUtils-1.0.2/src/JUtils/JArr.py` & `JUtils-1.0.3/src/JUtils/JArr.py`

 * *Files identical despite different names*

### Comparing `JUtils-1.0.2/src/JUtils/JColors.py` & `JUtils-1.0.3/src/JUtils/JColors.py`

 * *Files identical despite different names*

### Comparing `JUtils-1.0.2/src/JUtils/JConv.py` & `JUtils-1.0.3/src/JUtils/JConv.py`

 * *Files identical despite different names*

### Comparing `JUtils-1.0.2/src/JUtils/JNum.py` & `JUtils-1.0.3/src/JUtils/JNum.py`

 * *Files identical despite different names*

### Comparing `JUtils-1.0.2/src/JUtils/JOut.py` & `JUtils-1.0.3/src/JUtils/JOut.py`

 * *Files identical despite different names*

### Comparing `JUtils-1.0.2/src/JUtils/JStr.py` & `JUtils-1.0.3/src/JUtils/JStr.py`

 * *Files identical despite different names*

### Comparing `JUtils-1.0.2/src/JUtils.egg-info/PKG-INFO` & `JUtils-1.0.3/src/JUtils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JUtils
-Version: 1.0.2
+Version: 1.0.3
 Summary: Package containing various utility functions i needed now and then, that i wanted to share
 Author-email: Jan Seifert <jan@seifert-online.de>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

