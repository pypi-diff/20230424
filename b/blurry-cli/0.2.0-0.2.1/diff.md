# Comparing `tmp/blurry_cli-0.2.0.tar.gz` & `tmp/blurry_cli-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blurry_cli-0.2.0.tar", max compression
+gzip compressed data, was "blurry_cli-0.2.1.tar", max compression
```

## Comparing `blurry_cli-0.2.0.tar` & `blurry_cli-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1068 2022-12-23 03:32:02.242743 blurry_cli-0.2.0/LICENSE
--rw-r--r--   0        0        0     1784 2023-04-16 22:37:50.018954 blurry_cli-0.2.0/README.md
--rw-r--r--   0        0        0     8177 2023-04-16 23:06:33.073434 blurry_cli-0.2.0/blurry/__init__.py
--rw-r--r--   0        0        0       72 2022-12-23 03:32:02.242743 blurry_cli-0.2.0/blurry/__main__.py
--rw-r--r--   0        0        0      527 2022-12-23 03:32:02.242743 blurry_cli-0.2.0/blurry/async_typer.py
--rw-r--r--   0        0        0       76 2022-12-23 03:32:02.242743 blurry_cli-0.2.0/blurry/constants.py
--rw-r--r--   0        0        0     3414 2023-04-05 22:11:18.719201 blurry_cli-0.2.0/blurry/images.py
--rw-r--r--   0        0        0     6514 2023-04-16 22:37:50.018954 blurry_cli-0.2.0/blurry/markdown/__init__.py
--rw-r--r--   0        0        0     1633 2023-04-15 17:13:08.997639 blurry_cli-0.2.0/blurry/markdown/front_matter.py
--rw-r--r--   0        0        0     2261 2022-12-23 03:32:02.242743 blurry_cli-0.2.0/blurry/open_graph.py
--rw-r--r--   0        0        0      189 2023-04-16 22:37:50.025621 blurry_cli-0.2.0/blurry/plugins/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 22:37:50.025621 blurry_cli-0.2.0/blurry/plugins/html_plugins/__init__.py
--rw-r--r--   0        0        0      334 2023-04-16 22:37:50.025621 blurry_cli-0.2.0/blurry/plugins/html_plugins/minify_html_plugin.py
--rw-r--r--   0        0        0        0 2023-04-16 22:37:50.025621 blurry_cli-0.2.0/blurry/plugins/markdown_plugins/__init__.py
--rw-r--r--   0        0        0     1119 2023-04-16 22:37:50.025621 blurry_cli-0.2.0/blurry/plugins/markdown_plugins/container_plugin.py
--rw-r--r--   0        0        0      644 2023-04-16 22:37:50.025621 blurry_cli-0.2.0/blurry/plugins/markdown_plugins/punctuation_plugin.py
--rw-r--r--   0        0        0     1471 2023-04-16 22:37:50.025621 blurry_cli-0.2.0/blurry/plugins/markdown_plugins/python_code_plugin.py
--rw-r--r--   0        0        0        0 2022-12-23 03:32:02.242743 blurry_cli-0.2.0/blurry/py.typed
--rw-r--r--   0        0        0     2042 2023-04-09 23:10:30.264113 blurry_cli-0.2.0/blurry/settings.py
--rw-r--r--   0        0        0     1538 2023-03-28 22:11:29.443893 blurry_cli-0.2.0/blurry/sitemap.py
--rw-r--r--   0        0        0      636 2023-04-16 22:37:50.025621 blurry_cli-0.2.0/blurry/types.py
--rw-r--r--   0        0        0     4535 2023-04-22 14:16:05.282134 blurry_cli-0.2.0/blurry/utils.py
--rw-r--r--   0        0        0     1988 2023-04-22 15:07:18.954697 blurry_cli-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3311 1970-01-01 00:00:00.000000 blurry_cli-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2022-12-23 03:32:02.242743 blurry_cli-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1784 2023-04-16 22:37:50.018954 blurry_cli-0.2.1/README.md
+-rw-r--r--   0        0        0     8177 2023-04-16 23:06:33.073434 blurry_cli-0.2.1/blurry/__init__.py
+-rw-r--r--   0        0        0       72 2022-12-23 03:32:02.242743 blurry_cli-0.2.1/blurry/__main__.py
+-rw-r--r--   0        0        0      527 2022-12-23 03:32:02.242743 blurry_cli-0.2.1/blurry/async_typer.py
+-rw-r--r--   0        0        0       76 2022-12-23 03:32:02.242743 blurry_cli-0.2.1/blurry/constants.py
+-rw-r--r--   0        0        0     3414 2023-04-05 22:11:18.719201 blurry_cli-0.2.1/blurry/images.py
+-rw-r--r--   0        0        0     6514 2023-04-16 22:37:50.018954 blurry_cli-0.2.1/blurry/markdown/__init__.py
+-rw-r--r--   0        0        0     1633 2023-04-15 17:13:08.997639 blurry_cli-0.2.1/blurry/markdown/front_matter.py
+-rw-r--r--   0        0        0     1995 2023-04-23 22:31:36.524446 blurry_cli-0.2.1/blurry/open_graph.py
+-rw-r--r--   0        0        0      189 2023-04-16 22:37:50.025621 blurry_cli-0.2.1/blurry/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 22:37:50.025621 blurry_cli-0.2.1/blurry/plugins/html_plugins/__init__.py
+-rw-r--r--   0        0        0     1145 2023-04-23 21:40:44.156168 blurry_cli-0.2.1/blurry/plugins/html_plugins/minify_html_plugin.py
+-rw-r--r--   0        0        0        0 2023-04-16 22:37:50.025621 blurry_cli-0.2.1/blurry/plugins/markdown_plugins/__init__.py
+-rw-r--r--   0        0        0     1119 2023-04-16 22:37:50.025621 blurry_cli-0.2.1/blurry/plugins/markdown_plugins/container_plugin.py
+-rw-r--r--   0        0        0      644 2023-04-16 22:37:50.025621 blurry_cli-0.2.1/blurry/plugins/markdown_plugins/punctuation_plugin.py
+-rw-r--r--   0        0        0     1471 2023-04-16 22:37:50.025621 blurry_cli-0.2.1/blurry/plugins/markdown_plugins/python_code_plugin.py
+-rw-r--r--   0        0        0        0 2022-12-23 03:32:02.242743 blurry_cli-0.2.1/blurry/py.typed
+-rw-r--r--   0        0        0     2042 2023-04-09 23:10:30.264113 blurry_cli-0.2.1/blurry/settings.py
+-rw-r--r--   0        0        0     1546 2023-04-23 21:51:14.275747 blurry_cli-0.2.1/blurry/sitemap.py
+-rw-r--r--   0        0        0      636 2023-04-16 22:37:50.025621 blurry_cli-0.2.1/blurry/types.py
+-rw-r--r--   0        0        0     3722 2023-04-23 21:40:44.156168 blurry_cli-0.2.1/blurry/utils.py
+-rw-r--r--   0        0        0     1988 2023-04-23 22:52:11.247417 blurry_cli-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3311 1970-01-01 00:00:00.000000 blurry_cli-0.2.1/PKG-INFO
```

### Comparing `blurry_cli-0.2.0/LICENSE` & `blurry_cli-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.2.0/README.md` & `blurry_cli-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.2.0/blurry/__init__.py` & `blurry_cli-0.2.1/blurry/__init__.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.2.0/blurry/async_typer.py` & `blurry_cli-0.2.1/blurry/async_typer.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.2.0/blurry/images.py` & `blurry_cli-0.2.1/blurry/images.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.2.0/blurry/markdown/__init__.py` & `blurry_cli-0.2.1/blurry/markdown/__init__.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.2.0/blurry/markdown/front_matter.py` & `blurry_cli-0.2.1/blurry/markdown/front_matter.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.2.0/blurry/open_graph.py` & `blurry_cli-0.2.1/blurry/open_graph.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,13 @@
 from typing import Any
 from typing import Literal
 
 from blurry.types import SchemaType
 
 
-OPEN_GRAPH_TEMPLATE = """
-<meta property="og:title" content="{title}" />
-<meta property="og:type" content="{type}" />
-<meta property="og:url" content="{url}" />
-<meta property="og:image" content="{image}" />
-<meta property="og:site_name" content="{site_name}" />
-"""
-
 META_TAG_TEMPLATE = '<meta property="og:{property}" content="{content}" />'
 
 OpenGraphType = Literal["article", "book", "profile", "website"]
 
 
 schema_type_to_open_graph_type: dict[SchemaType, OpenGraphType] = {
     SchemaType.ARTICLE: "article",
@@ -29,16 +21,16 @@
     SchemaType.ORGANIZATION: "profile",
     SchemaType.PERSON: "profile",
 }
 
 
 def open_graph_type_from_schema_type(schema_type_str: str) -> OpenGraphType:
     try:
-        return schema_type_to_open_graph_type[SchemaType[schema_type_str]]
-    except KeyError:
+        return schema_type_to_open_graph_type[SchemaType(schema_type_str)]
+    except ValueError:
         return "website"
 
 
 def open_graph_meta_tags(schema_data: dict[str, Any]) -> str:
     open_graph_properties = {}
     if type := schema_data.get("@type"):
         open_graph_properties["type"] = open_graph_type_from_schema_type(type)
```

### Comparing `blurry_cli-0.2.0/blurry/plugins/markdown_plugins/container_plugin.py` & `blurry_cli-0.2.1/blurry/plugins/markdown_plugins/container_plugin.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.2.0/blurry/plugins/markdown_plugins/punctuation_plugin.py` & `blurry_cli-0.2.1/blurry/plugins/markdown_plugins/punctuation_plugin.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.2.0/blurry/plugins/markdown_plugins/python_code_plugin.py` & `blurry_cli-0.2.1/blurry/plugins/markdown_plugins/python_code_plugin.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.2.0/blurry/settings.py` & `blurry_cli-0.2.1/blurry/settings.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.2.0/blurry/sitemap.py` & `blurry_cli-0.2.1/blurry/sitemap.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
     xsi:schemaLocation="http://www.sitemaps.org/schemas/sitemap/0.9
     http://www.sitemaps.org/schemas/sitemap/0.9/sitemap.xsd"
     xmlns="http://www.sitemaps.org/schemas/sitemap/0.9"
 >
 {urls}
 </urlset>
-"""
+""".strip()
 URL_TEMPLATE = "    <url><loc>{url}</loc><lastmod>{lastmod}</lastmod></url>"
 
 
 def generate_sitemap_for_file_data_list(file_data_list: list[MarkdownFileData]) -> str:
     sitemap_url_data = []
     for file_data in file_data_list:
         lastmod = file_data.front_matter.get(
```

### Comparing `blurry_cli-0.2.0/blurry/types.py` & `blurry_cli-0.2.1/blurry/types.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.2.0/pyproject.toml` & `blurry_cli-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blurry-cli"
-version = "0.2.0"
+version = "0.2.1"
 description = "A Mistune-based static site generator for Python"
 authors = ["John Franey <franey@duck.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/blurry-dev/blurry"
 keywords = ["static-site-generator", "seo", "pagespeed"]
 classifiers = [
```

### Comparing `blurry_cli-0.2.0/PKG-INFO` & `blurry_cli-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blurry-cli
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Mistune-based static site generator for Python
 Home-page: https://github.com/blurry-dev/blurry
 License: MIT
 Keywords: static-site-generator,seo,pagespeed
 Author: John Franey
 Author-email: franey@duck.com
 Requires-Python: >=3.10,<4.0
```

