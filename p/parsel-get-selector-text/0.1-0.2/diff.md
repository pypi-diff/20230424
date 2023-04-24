# Comparing `tmp/parsel_get_selector_text-0.1.tar.gz` & `tmp/parsel_get_selector_text-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsel_get_selector_text-0.1.tar", last modified: Mon Apr 24 01:02:49 2023, max compression
+gzip compressed data, was "parsel_get_selector_text-0.2.tar", last modified: Mon Apr 24 01:20:48 2023, max compression
```

## Comparing `parsel_get_selector_text-0.1.tar` & `parsel_get_selector_text-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2023-04-24 01:02:49.009094 parsel_get_selector_text-0.1/
--rw-r--r--   0 andrei    (1000) andrei    (1000)     1089 2023-04-23 23:41:13.000000 parsel_get_selector_text-0.1/LICENSE
--rw-r--r--   0 andrei    (1000) andrei    (1000)      783 2023-04-24 01:02:49.009094 parsel_get_selector_text-0.1/PKG-INFO
--rw-r--r--   0 andrei    (1000) andrei    (1000)       85 2023-04-23 22:53:37.000000 parsel_get_selector_text-0.1/README.md
-drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2023-04-24 01:02:49.009094 parsel_get_selector_text-0.1/parsel_get_selector_text/
--rw-r--r--   0 andrei    (1000) andrei    (1000)     2218 2023-04-23 22:49:03.000000 parsel_get_selector_text-0.1/parsel_get_selector_text/__init__.py
-drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2023-04-24 01:02:49.009094 parsel_get_selector_text-0.1/parsel_get_selector_text.egg-info/
--rw-r--r--   0 andrei    (1000) andrei    (1000)      783 2023-04-24 01:02:48.000000 parsel_get_selector_text-0.1/parsel_get_selector_text.egg-info/PKG-INFO
--rw-r--r--   0 andrei    (1000) andrei    (1000)      270 2023-04-24 01:02:49.000000 parsel_get_selector_text-0.1/parsel_get_selector_text.egg-info/SOURCES.txt
--rw-r--r--   0 andrei    (1000) andrei    (1000)        1 2023-04-24 01:02:48.000000 parsel_get_selector_text-0.1/parsel_get_selector_text.egg-info/dependency_links.txt
--rw-r--r--   0 andrei    (1000) andrei    (1000)       25 2023-04-24 01:02:48.000000 parsel_get_selector_text-0.1/parsel_get_selector_text.egg-info/top_level.txt
--rw-r--r--   0 andrei    (1000) andrei    (1000)       85 2023-04-24 01:01:58.000000 parsel_get_selector_text-0.1/pyproject.toml
--rw-r--r--   0 andrei    (1000) andrei    (1000)       38 2023-04-24 01:02:49.009094 parsel_get_selector_text-0.1/setup.cfg
--rw-r--r--   0 andrei    (1000) andrei    (1000)      957 2023-04-24 00:59:52.000000 parsel_get_selector_text-0.1/setup.py
+drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2023-04-24 01:20:48.556095 parsel_get_selector_text-0.2/
+-rw-r--r--   0 andrei    (1000) andrei    (1000)     1089 2023-04-23 23:41:13.000000 parsel_get_selector_text-0.2/LICENSE
+-rw-r--r--   0 andrei    (1000) andrei    (1000)      783 2023-04-24 01:20:48.556095 parsel_get_selector_text-0.2/PKG-INFO
+-rw-r--r--   0 andrei    (1000) andrei    (1000)       85 2023-04-23 22:53:37.000000 parsel_get_selector_text-0.2/README.md
+drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2023-04-24 01:20:48.549429 parsel_get_selector_text-0.2/parsel_get_selector_text/
+-rw-r--r--   0 andrei    (1000) andrei    (1000)     2225 2023-04-24 01:19:56.000000 parsel_get_selector_text-0.2/parsel_get_selector_text/__init__.py
+drwxr-xr-x   0 andrei    (1000) andrei    (1000)        0 2023-04-24 01:20:48.556095 parsel_get_selector_text-0.2/parsel_get_selector_text.egg-info/
+-rw-r--r--   0 andrei    (1000) andrei    (1000)      783 2023-04-24 01:20:48.000000 parsel_get_selector_text-0.2/parsel_get_selector_text.egg-info/PKG-INFO
+-rw-r--r--   0 andrei    (1000) andrei    (1000)      270 2023-04-24 01:20:48.000000 parsel_get_selector_text-0.2/parsel_get_selector_text.egg-info/SOURCES.txt
+-rw-r--r--   0 andrei    (1000) andrei    (1000)        1 2023-04-24 01:20:48.000000 parsel_get_selector_text-0.2/parsel_get_selector_text.egg-info/dependency_links.txt
+-rw-r--r--   0 andrei    (1000) andrei    (1000)       25 2023-04-24 01:20:48.000000 parsel_get_selector_text-0.2/parsel_get_selector_text.egg-info/top_level.txt
+-rw-r--r--   0 andrei    (1000) andrei    (1000)       85 2023-04-24 01:01:58.000000 parsel_get_selector_text-0.2/pyproject.toml
+-rw-r--r--   0 andrei    (1000) andrei    (1000)       38 2023-04-24 01:20:48.556095 parsel_get_selector_text-0.2/setup.cfg
+-rw-r--r--   0 andrei    (1000) andrei    (1000)      957 2023-04-24 01:19:33.000000 parsel_get_selector_text-0.2/setup.py
```

### Comparing `parsel_get_selector_text-0.1/LICENSE` & `parsel_get_selector_text-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `parsel_get_selector_text-0.1/PKG-INFO` & `parsel_get_selector_text-0.2/parsel_get_selector_text.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: parsel_get_selector_text
-Version: 0.1
+Name: parsel-get-selector-text
+Version: 0.2
 Summary: Extracts all text results from an XPath query on a parsel Selector object.
 Home-page: https://github.com/carlosplanchon/parsel_get_selector_text
-Download-URL: https://github.com/carlosplanchon/parsel_get_selector_text/archive/v0.1.tar.gz
+Download-URL: https://github.com/carlosplanchon/parsel_get_selector_text/archive/v0.2.tar.gz
 Author: Carlos A. Planchón
 Author-email: carlosandresplanchonprestes@gmail.com
 License: MIT
 Keywords: comment,remover
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `parsel_get_selector_text-0.1/parsel_get_selector_text/__init__.py` & `parsel_get_selector_text-0.2/parsel_get_selector_text/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         children_list = list(root.children)
         for child in children_list:
             if isinstance(child, bs4.element.NavigableString):
                 text: str = child.get_text(separator=" ")
                 text = remove_trailing_chars(text=text)
                 if text != "":
                     text = ftfy.fix_text(text=text)
-                    self.total_text += text
+                    self.total_text += text + "\n"
             else:
                 self.traverse_soup(root=child)
         return None
 
     def get_sel_results(self, sel_results: parsel.SelectorList) -> None:
         """
         Takes a list of Selector objects and extracts
```

### Comparing `parsel_get_selector_text-0.1/setup.py` & `parsel_get_selector_text-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setup(
     name="parsel_get_selector_text",
     packages=["parsel_get_selector_text"],
-    version="0.1",
+    version="0.2",
     license="MIT",
     description="Extracts all text results from an XPath "\
         "query on a parsel Selector object.",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Carlos A. Planchón",
     author_email="carlosandresplanchonprestes@gmail.com",
     url="https://github.com/carlosplanchon/parsel_get_selector_text",
     download_url="https://github.com/carlosplanchon/"
-        "parsel_get_selector_text/archive/v0.1.tar.gz",
+        "parsel_get_selector_text/archive/v0.2.tar.gz",
     keywords=["comment", "remover"],
     classifiers=[
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.11",
     ],
```

