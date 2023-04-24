# Comparing `tmp/pyfbsdk-stub-generator-0.0.4.tar.gz` & `tmp/pyfbsdk-stub-generator-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfbsdk-stub-generator-0.0.4.tar", last modified: Sat Apr 15 19:56:13 2023, max compression
+gzip compressed data, was "pyfbsdk-stub-generator-1.0.0.tar", last modified: Mon Apr 24 04:58:06 2023, max compression
```

## Comparing `pyfbsdk-stub-generator-0.0.4.tar` & `pyfbsdk-stub-generator-1.0.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 19:56:13.829535 pyfbsdk-stub-generator-0.0.4/
--rw-rw-rw-   0        0        0     1235 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/LICENSE
--rw-rw-rw-   0        0        0       46 2023-04-15 19:55:38.000000 pyfbsdk-stub-generator-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2051 2023-04-15 19:56:13.829535 pyfbsdk-stub-generator-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1561 2023-04-15 19:07:58.000000 pyfbsdk-stub-generator-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-15 19:56:13.727218 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/
--rw-rw-rw-   0        0        0      932 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 19:56:13.763292 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/base_content/
--rw-rw-rw-   0        0        0      330 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/base_content/pyfbsdk.pyi
--rw-rw-rw-   0        0        0     7750 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/module_types.py
--rw-rw-rw-   0        0        0     9182 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/native_generator.py
-drwxrwxrwx   0        0        0        0 2023-04-15 19:56:13.769515 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/
--rw-rw-rw-   0        0        0      568 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 19:56:13.776239 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/fb_property/
--rw-rw-rw-   0        0        0        0 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/fb_property/__init__.py
--rw-rw-rw-   0        0        0     1847 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/fb_property/fb_property_plugin.py
-drwxrwxrwx   0        0        0        0 2023-04-15 19:56:13.787889 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/manual_documentation/
--rw-rw-rw-   0        0        0       57 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/manual_documentation/__init__.py
--rw-rw-rw-   0        0        0     1033 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/manual_documentation/doc_bases.py
-drwxrwxrwx   0        0        0        0 2023-04-15 19:56:13.793253 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/manual_documentation/modules/
--rw-rw-rw-   0        0        0        0 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/manual_documentation/modules/__init__.py
--rw-rw-rw-   0        0        0     4036 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/manual_documentation/modules/pyfbsdk.py
--rw-rw-rw-   0        0        0     2978 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/manual_documentation/plugin_manual_docs.py
-drwxrwxrwx   0        0        0        0 2023-04-15 19:56:13.799613 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/online_documentation/
--rw-rw-rw-   0        0        0       66 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/online_documentation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 19:56:13.824315 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/
--rw-rw-rw-   0        0        0        0 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/__init__.py
--rw-rw-rw-   0        0        0     1251 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/documentation_cache.py
--rw-rw-rw-   0        0        0      492 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/documentation_urls.py
--rw-rw-rw-   0        0        0    11801 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/page_parser.py
--rw-rw-rw-   0        0        0     2557 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/table_of_contents.py
--rw-rw-rw-   0        0        0    16475 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/online_documentation/plugin_online_documentation.py
--rw-rw-rw-   0        0        0     2666 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/plugin.py
--rw-rw-rw-   0        0        0     6559 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/stub_generator.py
-drwxrwxrwx   0        0        0        0 2023-04-15 19:56:13.758281 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator.egg-info/
--rw-rw-rw-   0        0        0     2051 2023-04-15 19:56:13.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1649 2023-04-15 19:56:13.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 19:56:13.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-04-15 19:56:13.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-04-15 19:56:13.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2022-06-24 08:36:30.000000 pyfbsdk-stub-generator-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      724 2023-04-15 19:56:13.834870 pyfbsdk-stub-generator-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-24 04:58:06.897504 pyfbsdk-stub-generator-1.0.0/
+-rw-rw-rw-   0        0        0     1235 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0       46 2023-04-15 19:55:38.000000 pyfbsdk-stub-generator-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2051 2023-04-24 04:58:06.898516 pyfbsdk-stub-generator-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1561 2023-04-15 19:07:58.000000 pyfbsdk-stub-generator-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 04:58:06.838839 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/
+-rw-rw-rw-   0        0        0      932 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 04:58:06.867663 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/base_content/
+-rw-rw-rw-   0        0        0      330 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/base_content/pyfbsdk.pyi
+-rw-rw-rw-   0        0        0     7750 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/module_types.py
+-rw-rw-rw-   0        0        0     9220 2023-04-23 15:58:00.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/native_generator.py
+drwxrwxrwx   0        0        0        0 2023-04-24 04:58:06.871672 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/
+-rw-rw-rw-   0        0        0      568 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 04:58:06.874671 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/fb_property/
+-rw-rw-rw-   0        0        0        0 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/fb_property/__init__.py
+-rw-rw-rw-   0        0        0     1847 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/fb_property/fb_property_plugin.py
+drwxrwxrwx   0        0        0        0 2023-04-24 04:58:06.880675 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/manual_documentation/
+-rw-rw-rw-   0        0        0       57 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/manual_documentation/__init__.py
+-rw-rw-rw-   0        0        0     1033 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/manual_documentation/doc_bases.py
+drwxrwxrwx   0        0        0        0 2023-04-24 04:58:06.883813 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/manual_documentation/modules/
+-rw-rw-rw-   0        0        0        0 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/manual_documentation/modules/__init__.py
+-rw-rw-rw-   0        0        0     4035 2023-04-24 04:50:45.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/manual_documentation/modules/pyfbsdk.py
+-rw-rw-rw-   0        0        0     2978 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/manual_documentation/plugin_manual_docs.py
+drwxrwxrwx   0        0        0        0 2023-04-24 04:58:06.887170 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/online_documentation/
+-rw-rw-rw-   0        0        0       66 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/online_documentation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 04:58:06.896489 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/
+-rw-rw-rw-   0        0        0        0 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/__init__.py
+-rw-rw-rw-   0        0        0     1251 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/documentation_cache.py
+-rw-rw-rw-   0        0        0      492 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/documentation_urls.py
+-rw-rw-rw-   0        0        0    12628 2023-04-22 08:47:04.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/page_parser.py
+-rw-rw-rw-   0        0        0     2593 2023-04-23 15:16:47.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/table_of_contents.py
+-rw-rw-rw-   0        0        0    17079 2023-04-24 04:54:07.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/online_documentation/plugin_online_documentation.py
+-rw-rw-rw-   0        0        0     2704 2023-04-23 15:57:38.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/plugin.py
+-rw-rw-rw-   0        0        0     6626 2023-04-24 04:47:13.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/stub_generator.py
+drwxrwxrwx   0        0        0        0 2023-04-24 04:58:06.865340 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator.egg-info/
+-rw-rw-rw-   0        0        0     2051 2023-04-24 04:58:06.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1649 2023-04-24 04:58:06.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 04:58:06.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 04:58:06.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-04-24 04:58:06.000000 pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2022-06-24 08:36:30.000000 pyfbsdk-stub-generator-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0      724 2023-04-24 04:58:06.900525 pyfbsdk-stub-generator-1.0.0/setup.cfg
```

### Comparing `pyfbsdk-stub-generator-0.0.4/LICENSE` & `pyfbsdk-stub-generator-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfbsdk-stub-generator-0.0.4/PKG-INFO` & `pyfbsdk-stub-generator-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfbsdk-stub-generator
-Version: 0.0.4
+Version: 1.0.0
 Summary: Generate pyfbsdk stub files for better intellisense when working with MotionBuilder
 Home-page: https://github.com/nils-soderman/pyfbsdk-stub-generator
 Author: Nils Soderman
 License: UNLICENSE
 Keywords: pyfbsdk,motionbuilder,mobu,autodesk,stub,stubfile,generator,gen
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `pyfbsdk-stub-generator-0.0.4/README.md` & `pyfbsdk-stub-generator-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/__init__.py` & `pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/module_types.py` & `pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/module_types.py`

 * *Files identical despite different names*

### Comparing `pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/native_generator.py` & `pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/native_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import inspect
 
 from types import ModuleType
 
 from .module_types import StubClass, StubFunction, StubParameter, StubProperty
 
 ENUMERATION_NAME = "Enumeration"
```

### Comparing `pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/__init__.py` & `pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/fb_property/fb_property_plugin.py` & `pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/fb_property/fb_property_plugin.py`

 * *Files identical despite different names*

### Comparing `pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/manual_documentation/doc_bases.py` & `pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/manual_documentation/doc_bases.py`

 * *Files identical despite different names*

### Comparing `pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/manual_documentation/modules/pyfbsdk.py` & `pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/manual_documentation/modules/pyfbsdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,11 +97,11 @@
         - bResizeWnd: Adjust the size of the tool window if needed (if started too close to the end of the screen for example).
 
     ### Returns:
     A pointer to the FBTool object, `None` otherwise."""
 
     Parameters = (
         ParameterBase("ToolName", str),
-        ParameterBase("ResizeWnd", bool, False),
+        ParameterBase("ResizeWnd", bool, True),
     )
 
     ReturnType = pyfbsdk.FBTool
```

### Comparing `pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/manual_documentation/plugin_manual_docs.py` & `pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/manual_documentation/plugin_manual_docs.py`

 * *Files identical despite different names*

### Comparing `pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/documentation_cache.py` & `pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/documentation_cache.py`

 * *Files identical despite different names*

### Comparing `pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/page_parser.py` & `pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/page_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 from . import documentation_cache as cache
 
 reload(cache)
 reload(urls)
 
 PY2_TO_PY3_PRINT_PATTERN = re.compile(r"(?<!\w)print\s+(.*)\s*(?<!\\)(?:\n|$)")
 
-
 class ClassNames:
     Items = "memitem"
+    ItemTitles = "memtitle"
     Doc = "memdoc"
     ItemName = "memname"
     ParameterName = "paramname"
     ParameterType = "paramtype"
     TextBlockDescription = "textblock"
     ParameterTalble = "params"
     CodeBlock = "fragment"
@@ -39,14 +39,15 @@
 
 @dataclass
 class MemberItem:
     Name: str
     Type: str
     DocString: str
     Parameters: list[Parameter]
+    RelativeUrl: str
 
 
 class DocumentationParsedPage():
     def __init__(self, Name: str, DocString: str, Members: list[MemberItem]):
         self.Name = Name
         self.DocString = DocString
         self.Members = Members
@@ -88,33 +89,51 @@
     Parser = BeautifulSoup(PageHtmlContent, "html.parser")
 
     DescriptionHtml = Parser.find("div", class_ = ClassNames.TextBlockDescription)
     Description = DocStringMdConverter.ConvertDocString(DescriptionHtml) if DescriptionHtml else ""
 
     MemberItems = []
     Item: Tag | NavigableString
-    for Item in Parser.find_all("div", class_ = ClassNames.Items):
+    Items = Parser.find_all("div", class_ = ClassNames.Items)
+    ItemTitles = Parser.find_all("h2", class_ = ClassNames.ItemTitles)
+
+    # If the titles doesn't match, fallback to not using titles
+    if len(Items) != len(ItemTitles):
+        print(f"Warning: The number of items ({len(Items)}) and item titles ({len(ItemTitles)}) doesn't match for page '{PageName}'.")
+        ItemTitles = [None] * len(Items)
+    
+    for Item, Title in zip(Items, ItemTitles):
         ItemName = ""
         ItemType = ""
         ItemDocumentation = ""
+        Url = ""
+
+        if Title:
+            LinkElemt = Title.find("a")
+            if LinkElemt:
+                Url = LinkElemt.get("href")
 
         DocumentationHtml = Item.find("div", class_ = ClassNames.Doc)
         if DocumentationHtml:
             ItemDocumentation: str = DocStringMdConverter.ConvertDocString(DocumentationHtml)
 
         NameTable = Item.find("table", class_ = ClassNames.ItemName)
         if NameTable:
             NameHtml = NameTable.find("td", class_ = ClassNames.ItemName)
             if NameHtml:
                 ItemName: str = GetSafeText(NameHtml.get_text())
                 if " " in ItemName:
-                    ItemType, _, ItemName = ItemName.partition(" ")
+                    ItemType, _, ItemName = ItemName.rpartition(" ")
                     ItemName = ItemName.strip()
                     ItemType = ItemType.strip()
 
+                    # In 2024 `FBSystem::DesktopSize` type is broken and contains html code 
+                    if "</a>" in ItemType:
+                        ItemType = ItemType.rpartition("</a>")[2].strip()
+
             # Find all parameters
             Parameters = []
             for Row in NameTable.find_all("tr"):
                 ParameterNameHtml = Row.find("td", class_ = ClassNames.ParameterName)
                 ParameterTypeHtml = Row.find("td", class_ = ClassNames.ParameterType)
                 if ParameterNameHtml and ParameterTypeHtml:
                     ParameterName: str = GetSafeText(ParameterNameHtml.get_text())
@@ -131,15 +150,15 @@
                             ParameterName = ParameterType
                             ParameterType = ""
                         else:
                             ParameterName = None
 
                     Parameters.append(Parameter(ParameterName, ParameterType, ParamDefaultValue))
 
-        MemberItems.append(MemberItem(ItemName, ItemType, ItemDocumentation, Parameters))
+        MemberItems.append(MemberItem(ItemName, ItemType, ItemDocumentation, Parameters, Url))
 
     return DocumentationParsedPage(PageName, Description.strip(), MemberItems)
 
 
 def GetSafeText(Text: str):
     # Remove any non-breaking spaces and strip the text of whitespace and commas
     return Text.replace('\xa0', ' ').strip(string.whitespace + ",").replace("\\", "\\\\")
```

### Comparing `pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/table_of_contents.py` & `pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/table_of_contents.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """ 
 Web Documentation scraper for the pyfbsdk SDK.
 """
+from __future__ import annotations
 
 from importlib import reload
 
 import requests
 import js2py
 
 from . import documentation_cache as cache
```

### Comparing `pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/online_documentation/plugin_online_documentation.py` & `pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/online_documentation/plugin_online_documentation.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,24 +11,31 @@
 from ..plugin import PluginBaseClass
 from ...module_types import StubClass, StubFunction, StubParameter, StubProperty
 
 reload(table_of_contents)
 
 EVENT_SOURCE_TYPE = "callbackframework.FBEventSource"
 
+TYPE_IGNORE_PREFIXES = (
+    "unsigned",
+    "K_DEPRECATED"
+)
+
 TRANSLATION_TYPE = {
     "double": "float",
     "long": "int",
     "kInt64": "int",
     "kULong": "int",
+    "char": "str",
 
     "kReference": "int",
     "FBkReference": "int",
 
     "FBAudioFmt": "int",
+    "FBBool": "bool",
 
     "FBArrayDouble": "list[float]",
     "FBArrayUInt": "list[int]",
 
     "FBVector4[float]": "FBVector4d",
     "FBTVector": "FBVector4d",
     "FBQuaternion": "FBVector4d",
@@ -214,15 +221,16 @@
             # Remove them from the lists so we don't try to match them again
             FunctionsCopy.remove(Function)
             MembersCopy.remove(Member)
 
     def PatchFunctionWithDocumentation(self, Function: StubFunction, DocMember: MemberItem, ParentClass: StubClass | None = None):
         Function.DocString = DocMember.DocString
         if Function.Name == "__init__":
-            Function.DocString = Function.DocString.removeprefix("Constructor.")
+            if Function.DocString.startswith("Constructor."):
+                Function.DocString = Function.DocString.replace("Constructor.", "", 1)
 
         if self.ShouldPatchType(Function.ReturnType, DocMember.Type):
             NewType = self.EnsureValidType(DocMember.Type)
             if NewType:
                 Function.ReturnType = NewType
 
         FunctionParameters = Function.GetParameters(bExcludeSelf = True)
@@ -327,39 +335,50 @@
 
         ValidatedType = self.EnsureValidType(NewType)
         if not ValidatedType:
             return False
 
         if CurrentType == "list" and ValidatedType.startswith("list"):
             return True
+        if CurrentType == "tuple" and ValidatedType.startswith("tuple"):
+            return True
 
         # TODO: Must check if type is valid as well
         if CurrentType.startswith(("E", "FB")) and CurrentType not in self.AllClassesMap:
             return True
 
         return False
 
     def EnsureValidType(self, Type: str) -> str | None:
         if "<" in Type:
             Type = Type.replace("<", "[").replace(">", "]").replace(" ", "")
             Type = Type.replace("FBArrayTemplate", "list")
 
             # Get content between brackets
-            ListTypes = Type[Type.find("[") + 1:Type.find("]")]
-            if ListTypes:
+            ListTypesStr = Type[Type.find("[") + 1:Type.find("]")]
+            if ListTypesStr:
                 ValidatedTypes = []
-                for ListType in ListTypes.split(","):
+                ListTypes = ListTypesStr.split(",")
+                for ListType in ListTypes:
                     ListType = self.EnsureValidType(ListType)
                     if ListType:
                         ValidatedTypes.append(ListType)
-                TypeBefore = Type
-                Type = Type.replace(ListTypes, ",".join(ValidatedTypes))
+                
+                if len(ListTypes) != len(ValidatedTypes):
+                    return None
+                
+                Type = Type.replace(ListTypesStr, ",".join(ValidatedTypes))
                 if Type.endswith("[]"):
                     Type = Type[:-2]
 
+        if " " in Type:
+            for Prefix in TYPE_IGNORE_PREFIXES:
+                if Type.startswith(Prefix):
+                    Type = Type.rpartition(" ")[2]
+        
         Type = TRANSLATION_TYPE.get(Type, Type)
 
         # Replace namespace C++ syntax with Python
         if "::" in Type:
             Type = Type.replace("::", ".")
 
         if Type.startswith("FB"):
```

### Comparing `pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/plugin.py` & `pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/plugins/plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import threading
 import logging
 import os
 
 from types import ModuleType, FunctionType
 
 from ..module_types import StubClass, StubFunction, StubParameter, StubProperty
```

### Comparing `pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/stub_generator.py` & `pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator/stub_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 
 import pyfbsdk
 
 bTest = "builtin" in __name__
 if bTest:
     for Path in (
         os.path.dirname(os.path.dirname(__file__)),
-        f"C:/Python{sys.version_info.major}{sys.version_info.minor}/lib/site-packages"
+        f"C:/Python{sys.version_info.major}{sys.version_info.minor}/lib/site-packages",
+        f"{os.getenv('APPDATA')}/Python/Python310/site-packages"
     ):
         if Path not in sys.path:
             sys.path.append(Path)
     __name__ = "pyfbsdk_stub_generator.stub_generator"  # pylint: disable=redefined-builtin
     os.environ["PYFBSDK_DEVMODE"] = "True"
 
 from . import plugins
```

### Comparing `pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator.egg-info/PKG-INFO` & `pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfbsdk-stub-generator
-Version: 0.0.4
+Version: 1.0.0
 Summary: Generate pyfbsdk stub files for better intellisense when working with MotionBuilder
 Home-page: https://github.com/nils-soderman/pyfbsdk-stub-generator
 Author: Nils Soderman
 License: UNLICENSE
 Keywords: pyfbsdk,motionbuilder,mobu,autodesk,stub,stubfile,generator,gen
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator.egg-info/SOURCES.txt` & `pyfbsdk-stub-generator-1.0.0/pyfbsdk_stub_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyfbsdk-stub-generator-0.0.4/setup.cfg` & `pyfbsdk-stub-generator-1.0.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7966 6273 646b 2d73 7475 622d   = pyfbsdk-stub-
 00000020: 6765 6e65 7261 746f 720d 0a76 6572 7369  generator..versi
-00000030: 6f6e 203d 2030 2e30 2e34 0d0a 6175 7468  on = 0.0.4..auth
+00000030: 6f6e 203d 2031 2e30 2e30 0d0a 6175 7468  on = 1.0.0..auth
 00000040: 6f72 203d 204e 696c 7320 536f 6465 726d  or = Nils Soderm
 00000050: 616e 0d0a 6465 7363 7269 7074 696f 6e20  an..description 
 00000060: 3d20 4765 6e65 7261 7465 2070 7966 6273  = Generate pyfbs
 00000070: 646b 2073 7475 6220 6669 6c65 7320 666f  dk stub files fo
 00000080: 7220 6265 7474 6572 2069 6e74 656c 6c69  r better intelli
 00000090: 7365 6e73 6520 7768 656e 2077 6f72 6b69  sense when worki
 000000a0: 6e67 2077 6974 6820 4d6f 7469 6f6e 4275  ng with MotionBu
```

