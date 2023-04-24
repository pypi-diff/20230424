# Comparing `tmp/html2notion-0.1.3.tar.gz` & `tmp/html2notion-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html2notion-0.1.3.tar", last modified: Sun Apr 23 04:45:05 2023, max compression
+gzip compressed data, was "html2notion-0.1.4.tar", last modified: Mon Apr 24 05:22:51 2023, max compression
```

## Comparing `html2notion-0.1.3.tar` & `html2notion-0.1.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-23 04:45:05.060841 html2notion-0.1.3/
--rw-r--r--   0 daemonzhao   (501) staff       (20)     1064 2023-03-22 08:52:55.000000 html2notion-0.1.3/LICENSE
--rw-r--r--   0 daemonzhao   (501) staff       (20)     4600 2023-04-23 04:45:05.061036 html2notion-0.1.3/PKG-INFO
--rw-r--r--   0 daemonzhao   (501) staff       (20)     4111 2023-04-23 03:24:11.000000 html2notion-0.1.3/README.md
-drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-23 04:45:05.040993 html2notion-0.1.3/html2notion/
--rw-r--r--   0 daemonzhao   (501) staff       (20)        0 2023-03-20 01:38:35.000000 html2notion-0.1.3/html2notion/__init__.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     3955 2023-04-23 03:47:45.000000 html2notion-0.1.3/html2notion/main.py
-drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-23 04:45:05.053144 html2notion-0.1.3/html2notion/translate/
--rw-r--r--   0 daemonzhao   (501) staff       (20)        0 2023-03-20 01:38:35.000000 html2notion-0.1.3/html2notion/translate/__init__.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     4176 2023-04-23 03:24:11.000000 html2notion-0.1.3/html2notion/translate/batch_import.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     2724 2023-04-19 01:44:49.000000 html2notion-0.1.3/html2notion/translate/cos_uploader.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     2481 2023-04-20 11:03:46.000000 html2notion-0.1.3/html2notion/translate/html2json.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     7894 2023-04-21 09:57:38.000000 html2notion-0.1.3/html2notion/translate/html2json_base.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)      430 2023-04-20 02:17:23.000000 html2notion-0.1.3/html2notion/translate/html2json_default.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     8804 2023-04-21 02:35:36.000000 html2notion-0.1.3/html2notion/translate/html2json_yinxiang.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     7030 2023-04-12 04:47:53.000000 html2notion-0.1.3/html2notion/translate/notion_export.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     2387 2023-04-21 02:20:28.000000 html2notion-0.1.3/html2notion/translate/notion_import.py
-drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-23 04:45:05.056801 html2notion-0.1.3/html2notion/utils/
--rw-r--r--   0 daemonzhao   (501) staff       (20)      427 2023-03-24 02:23:25.000000 html2notion-0.1.3/html2notion/utils/__init__.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)      828 2023-03-22 03:05:54.000000 html2notion-0.1.3/html2notion/utils/load_config.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     1579 2023-04-20 06:50:27.000000 html2notion-0.1.3/html2notion/utils/log.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)      437 2023-04-21 02:46:15.000000 html2notion-0.1.3/html2notion/utils/timeutil.py
-drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-23 04:45:05.044729 html2notion-0.1.3/html2notion.egg-info/
--rw-r--r--   0 daemonzhao   (501) staff       (20)     4600 2023-04-23 04:45:04.000000 html2notion-0.1.3/html2notion.egg-info/PKG-INFO
--rw-r--r--   0 daemonzhao   (501) staff       (20)      875 2023-04-23 04:45:04.000000 html2notion-0.1.3/html2notion.egg-info/SOURCES.txt
--rw-r--r--   0 daemonzhao   (501) staff       (20)        1 2023-04-23 04:45:04.000000 html2notion-0.1.3/html2notion.egg-info/dependency_links.txt
--rw-r--r--   0 daemonzhao   (501) staff       (20)       54 2023-04-23 04:45:04.000000 html2notion-0.1.3/html2notion.egg-info/entry_points.txt
--rw-r--r--   0 daemonzhao   (501) staff       (20)      170 2023-04-23 04:45:04.000000 html2notion-0.1.3/html2notion.egg-info/requires.txt
--rw-r--r--   0 daemonzhao   (501) staff       (20)       12 2023-04-23 04:45:04.000000 html2notion-0.1.3/html2notion.egg-info/top_level.txt
--rw-r--r--   0 daemonzhao   (501) staff       (20)      103 2023-03-20 01:38:35.000000 html2notion-0.1.3/pyproject.toml
--rw-r--r--   0 daemonzhao   (501) staff       (20)      852 2023-04-23 04:45:05.061683 html2notion-0.1.3/setup.cfg
--rw-r--r--   0 daemonzhao   (501) staff       (20)       38 2023-03-17 05:39:04.000000 html2notion-0.1.3/setup.py
-drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-23 04:45:05.059908 html2notion-0.1.3/tests/
--rw-r--r--   0 daemonzhao   (501) staff       (20)     2892 2023-04-20 03:22:55.000000 html2notion-0.1.3/tests/test_batchimport.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     3038 2023-04-20 03:22:52.000000 html2notion-0.1.3/tests/test_cosupload.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     2698 2023-04-13 05:01:24.000000 html2notion-0.1.3/tests/test_notionexport.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)    15597 2023-04-20 11:59:35.000000 html2notion-0.1.3/tests/test_yinxiang.py
+drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-24 05:22:51.113231 html2notion-0.1.4/
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     1064 2023-03-22 08:52:55.000000 html2notion-0.1.4/LICENSE
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     4600 2023-04-24 05:22:51.113409 html2notion-0.1.4/PKG-INFO
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     4111 2023-04-23 03:24:11.000000 html2notion-0.1.4/README.md
+drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-24 05:22:51.097775 html2notion-0.1.4/html2notion/
+-rw-r--r--   0 daemonzhao   (501) staff       (20)        0 2023-03-20 01:38:35.000000 html2notion-0.1.4/html2notion/__init__.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     3955 2023-04-23 03:47:45.000000 html2notion-0.1.4/html2notion/main.py
+drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-24 05:22:51.106635 html2notion-0.1.4/html2notion/translate/
+-rw-r--r--   0 daemonzhao   (501) staff       (20)        0 2023-03-20 01:38:35.000000 html2notion-0.1.4/html2notion/translate/__init__.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     4176 2023-04-23 03:24:11.000000 html2notion-0.1.4/html2notion/translate/batch_import.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     2724 2023-04-19 01:44:49.000000 html2notion-0.1.4/html2notion/translate/cos_uploader.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     2689 2023-04-23 06:05:09.000000 html2notion-0.1.4/html2notion/translate/html2json.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     7936 2023-04-24 05:22:27.000000 html2notion-0.1.4/html2notion/translate/html2json_base.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      430 2023-04-20 02:17:23.000000 html2notion-0.1.4/html2notion/translate/html2json_default.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)    10540 2023-04-24 05:22:27.000000 html2notion-0.1.4/html2notion/translate/html2json_yinxiang.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     7168 2023-04-23 11:21:17.000000 html2notion-0.1.4/html2notion/translate/notion_export.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     2389 2023-04-23 05:23:44.000000 html2notion-0.1.4/html2notion/translate/notion_import.py
+drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-24 05:22:51.109650 html2notion-0.1.4/html2notion/utils/
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      427 2023-03-24 02:23:25.000000 html2notion-0.1.4/html2notion/utils/__init__.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      828 2023-03-22 03:05:54.000000 html2notion-0.1.4/html2notion/utils/load_config.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     1579 2023-04-20 06:50:27.000000 html2notion-0.1.4/html2notion/utils/log.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      437 2023-04-21 02:46:15.000000 html2notion-0.1.4/html2notion/utils/timeutil.py
+drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-24 05:22:51.100459 html2notion-0.1.4/html2notion.egg-info/
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     4600 2023-04-24 05:22:51.000000 html2notion-0.1.4/html2notion.egg-info/PKG-INFO
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      875 2023-04-24 05:22:51.000000 html2notion-0.1.4/html2notion.egg-info/SOURCES.txt
+-rw-r--r--   0 daemonzhao   (501) staff       (20)        1 2023-04-24 05:22:51.000000 html2notion-0.1.4/html2notion.egg-info/dependency_links.txt
+-rw-r--r--   0 daemonzhao   (501) staff       (20)       54 2023-04-24 05:22:51.000000 html2notion-0.1.4/html2notion.egg-info/entry_points.txt
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      170 2023-04-24 05:22:51.000000 html2notion-0.1.4/html2notion.egg-info/requires.txt
+-rw-r--r--   0 daemonzhao   (501) staff       (20)       12 2023-04-24 05:22:51.000000 html2notion-0.1.4/html2notion.egg-info/top_level.txt
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      103 2023-03-20 01:38:35.000000 html2notion-0.1.4/pyproject.toml
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      852 2023-04-24 05:22:51.114083 html2notion-0.1.4/setup.cfg
+-rw-r--r--   0 daemonzhao   (501) staff       (20)       38 2023-03-17 05:39:04.000000 html2notion-0.1.4/setup.py
+drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-24 05:22:51.112729 html2notion-0.1.4/tests/
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     2892 2023-04-20 03:22:55.000000 html2notion-0.1.4/tests/test_batchimport.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     3038 2023-04-20 03:22:52.000000 html2notion-0.1.4/tests/test_cosupload.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     2698 2023-04-13 05:01:24.000000 html2notion-0.1.4/tests/test_notionexport.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)    17438 2023-04-24 05:22:27.000000 html2notion-0.1.4/tests/test_yinxiang.py
```

### Comparing `html2notion-0.1.3/LICENSE` & `html2notion-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.3/PKG-INFO` & `html2notion-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html2notion
-Version: 0.1.3
+Version: 0.1.4
 Summary: This tool can accurately convert HTML to Notion notes and is also useful for exporting Evernote notes to Notion.
 Home-page: https://github.com/selfboot/html2notion
 Author: selfboot
 Author-email: xuezaigds@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `html2notion-0.1.3/README.md` & `html2notion-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.3/html2notion/main.py` & `html2notion-0.1.4/html2notion/main.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.3/html2notion/translate/batch_import.py` & `html2notion-0.1.4/html2notion/translate/batch_import.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.3/html2notion/translate/cos_uploader.py` & `html2notion-0.1.4/html2notion/translate/cos_uploader.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.3/html2notion/translate/html2json.py` & `html2notion-0.1.4/html2notion/translate/html2json.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,31 +5,37 @@
 from bs4 import BeautifulSoup, Tag
 from ..utils import logger, test_prepare_conf
 from ..translate.html2json_base import Html2JsonBase
 from ..translate.html2json_default import Default_Type
 from ..translate.html2json_yinxiang import YinXiang_Type
 
 
+"""
+<meta name="source" content="yinxiang.superNote"/>
+<meta name="source" content="desktop.mac"/>
+"""
+def _is_yinxiang_export_html(html_soup):
+    exporter_version_meta = html_soup.select_one('html > head > meta[name="exporter-version"]')
+    meta_source = html_soup.select_one('html > head > meta[name="source"]')
+    exporter_version_content = exporter_version_meta.get( 'content', "") if isinstance(exporter_version_meta, Tag) else ""
+
+    meta_source_content = meta_source.get('content', "") if isinstance(meta_source, Tag) else ""
+    if isinstance(exporter_version_content, str) and not exporter_version_content.startswith("Evernote"):
+        return False
+
+    yinxiang_source_content = ["yinxiang", "desktop"]
+    for prefix in yinxiang_source_content:
+        if isinstance(meta_source_content, str) and meta_source_content.startswith(prefix):
+            return True
+    return False
+
+
 def _infer_input_type(html_content):
     soup = BeautifulSoup(html_content, 'html.parser')
-    exporter_version_meta = soup.select_one(
-        'html > head > meta[name="exporter-version"]')
-    meta_source = soup.select_one('html > head > meta[name="source"]')
-
-    exporter_version_content = ""
-    if exporter_version_meta and isinstance(exporter_version_meta, Tag):
-        exporter_version_content = exporter_version_meta.get('content', "")
-    meta_source_content = ""
-    if meta_source and isinstance(meta_source, Tag):
-        meta_source_content = meta_source.get('content', "")
-
-    if isinstance(exporter_version_content, str) \
-            and exporter_version_content.startswith("Evernote") \
-            and isinstance(meta_source_content, str) \
-            and meta_source_content.startswith("desktop"):
+    if _is_yinxiang_export_html(soup):
         return YinXiang_Type
 
     return Default_Type
 
 
 def _get_converter(html_content):
     html_type = _infer_input_type(html_content)
@@ -62,15 +68,15 @@
     converter = _get_converter(html_content)
     result = converter.process()
     return converter.get_notion_data(), result
 
 
 if __name__ == "__main__":
     test_prepare_conf()
-    html_file = Path("./demos/TestCaseA.html")
+    html_file = Path("./demos/Test Case C.html")
     result, html_type = html2json_process(html_file)
     print(html_type)
     print(json.dumps(result, indent=4, ensure_ascii=False))
     result2, html_type2 = html2json_process(
         "<html><body><div>test</div></body></html>")
     print(html_type2)
     print(json.dumps(result2, indent=4, ensure_ascii=False))
```

### Comparing `html2notion-0.1.3/html2notion/translate/html2json_base.py` & `html2notion-0.1.4/html2notion/translate/html2json_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 class Block(Enum):
     FAIL = "fail"
     PARAGRAPH = "paragraph"
     QUOTE = "quote"
     NUMBERED_LIST = "numbered_list_item"
     BULLETED_LIST = "bulleted_list_item"
+    HEADING = "heading"
+    CODE = "code"
 
 class Html2JsonBase:
     _registry = {}
     _text_annotations = {
         "bold": bool,
         "italic": bool,
         "strikethrough": bool,
```

### Comparing `html2notion-0.1.3/html2notion/translate/html2json_yinxiang.py` & `html2notion-0.1.4/html2notion/translate/html2json_yinxiang.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,50 +15,43 @@
     def process(self):
         soup = BeautifulSoup(self.html_content, 'html.parser')
         self.convert_children(soup)
         self.convert_properties(soup)
         return YinXiang_Type
 
     def convert_properties(self, soup):
+        properties = {"title": "Unknown"}
         title_tag = soup.select_one('head > title')
-        title_text = "Unknow"
         if title_tag:
-            title_text = title_tag.text
-        properties = {"title": title_text}
+            properties["title"] = title_tag.text
 
-        meta_url_tag = soup.select_one('head > meta[name="source-url"]')
-        if meta_url_tag:
-            source_url = meta_url_tag['content']
-            if source_url:
-                properties["url"] = source_url
-
-        # <meta name="keywords" content="openai"/>
-        meta_keywords_tag = soup.select_one('head > meta[name="keywords"]')
-        if meta_keywords_tag:
-            keywords = meta_keywords_tag['content']
-            if keywords:
-                properties["tags"] = keywords.split(",")
-        
-        created_time_tag = soup.select_one('head > meta[name="created"]')
-        if created_time_tag:
-            created_time = created_time_tag['content']
-            if created_time:
-                properties["created_time"] = DateStrToISO8601(created_time)
+        meta_tags = [
+            ('head > meta[name="source-url"]', "url"),
+            ('head > meta[name="keywords"]', "tags", lambda x: x.split(",")),
+            ('head > meta[name="created"]', "created_time", DateStrToISO8601),
+        ]
+
+        for selector, key, *converter in meta_tags:
+            tag = soup.select_one(selector)
+            if tag and tag.get('content', None):
+                content = tag['content']
+                properties[key] = converter[0](content) if converter else content
 
         self.properties = self.generate_properties(**properties)
         return
 
     def convert_children(self, soup):
         content_tags = soup.find_all('body', recursive=True)
         if not content_tags:
             logger.warning("No content found")
             return
 
         for child in content_tags[0].children:
             block_type = self.get_block_type(child)
+            logger.debug(f'Support tag {child} with style {block_type}')
             converter = getattr(self, f"convert_{block_type}")
             if converter:
                 block = converter(child)
                 if block:
                     self.children.extend([block] if not isinstance(block, list) else block)
             else:
                 logger.warning(f"Unknown block type: {block_type}")
@@ -69,19 +62,67 @@
             "type": "paragraph",
             "paragraph": {
                 "rich_text": []
             }
         }
         rich_text = json_obj["paragraph"]["rich_text"]
         tag_text = soup.text if soup.text else ""
-        text_obj = self.parse_inline_block(soup, tag_text)
+        text_obj = self.parse_inline_block(soup)
         if text_obj:
             rich_text.extend(text_obj)
         return json_obj
 
+    def convert_heading(self, soup):
+        heading_map = {"h1": "heading_1", "h2": "heading_2", "h3": "heading_3",
+                       "h4": "heading_3", "h5": "heading_3", "h6": "heading_3"}
+
+        heading_level = heading_map.get(soup.name, "heading_3")
+        json_obj = {
+            "object": "block",
+            "type": heading_level,
+            heading_level: {
+                "rich_text": []
+            }
+        }
+        rich_text = json_obj[heading_level]["rich_text"]
+        text_obj = self.parse_inline_block(soup)
+        if text_obj:
+            rich_text.extend(text_obj)
+        return json_obj
+    
+    def convert_code(self, soup):
+        json_obj = {
+            "object": "block",
+            "type": "code",
+            "code": {
+                "rich_text": [],
+                "language": "plain text",
+            },
+        }
+        rich_text = json_obj["code"]["rich_text"]
+        children_list = list(soup.children) if isinstance(soup, Tag) else [soup]
+        for index, child in enumerate(children_list):
+            is_last_child = index == len(children_list) - 1
+            text_obj = self.parse_inline_block(child)
+            if text_obj:
+                rich_text.extend(text_obj)
+            if not is_last_child:
+                rich_text.append(self.generate_text(plain_text='\n'))
+        json_obj["code"]["rich_text"] = self.merge_rich_text(rich_text)
+
+        style = soup.get('style') if soup.name else ""
+        css_dict = {}
+        if style:
+            style = ''.join(style.split())
+            css_dict = {rule.split(':')[0].strip(): rule.split(':')[1].strip() for rule in style.split(';') if rule}
+            language = css_dict.get('--en-codeblockLanguage', 'plain text')
+            json_obj["code"]["language"] = language
+        
+        return json_obj
+    
     def convert_fail(self, soup):
         return {
             "object": "block",
             "type": "paragraph",
             "paragraph": {
                 "rich_text": []
             }
@@ -95,16 +136,15 @@
                 "rich_text": []
             }
         }
         rich_text = json_obj["quote"]["rich_text"]
         children_list = list(soup.children)
         for index, child in enumerate(children_list):
             is_last_child = index == len(children_list) - 1
-            tag_text = child.text if child.text else ""
-            text_obj = self.parse_inline_block(child, tag_text)
+            text_obj = self.parse_inline_block(child)
             if text_obj:
                 rich_text.extend(text_obj)
             if not is_last_child:
                 rich_text.append(self.generate_text(plain_text='\n'))
 
         # Merge tags has same anotions
         logger.debug(f'before merge: {rich_text}')
@@ -142,18 +182,15 @@
             list_type: {
                 "rich_text": []
             },
             "type": list_type,
         }
         rich_text = json_obj[list_type]["rich_text"]
         for child in soup.children:
-            tag_text = child.text if child.text else ""
-            if not tag_text:
-                continue
-            text_obj = self.parse_inline_block(child, tag_text)
+            text_obj = self.parse_inline_block(child)
             if text_obj:
                 rich_text.extend(text_obj)
 
         return json_obj
 
     def _recursive_parse_style(self, tag_soup, tag_text, text_params):
         tag_name = tag_soup.name.lower() if tag_soup.name else ""
@@ -179,28 +216,29 @@
             text_params["color"] = color
 
         if not tag_soup or isinstance(tag_soup, NavigableString):
             return
 
         for child in tag_soup.children:
             logger.debug(f'Recursive, child: {child}, {child.name}')
-            if child.name:
+            if isinstance(child, Tag):
                 self._recursive_parse_style(child, child.text, text_params)
         return
 
     # <b><u>unlineline and bold</u></b>
     # <div><font color="#ff2600">Red color4</font></div>
-    def parse_inline_block(self, tag_soup, tag_text):
+    # <div> Code in super note</div>
+    def parse_inline_block(self, tag_soup):
         block_objs = []
-        for child in tag_soup.children:
+        all_tags = tag_soup.children if isinstance(tag_soup, Tag) else [tag_soup]
+        for child in all_tags:
             text_params = {}
             tag_name = child.name.lower() if child.name else ""
             child_text = child.text if child.text else ""
-            # if tag_name == 'br':
-            #     child_text = ''
+ 
             text_params["plain_text"] = child_text
             if not isinstance(child, NavigableString):
                 self._recursive_parse_style(child, child_text, text_params)
 
             text_obj = {}
             if not isinstance(child, NavigableString) and tag_name == 'a':
                 href = child.get('href', "")
@@ -218,29 +256,33 @@
 
     def get_block_type(self, single_tag):
         tag_name = single_tag.name
         style = single_tag.get('style') if tag_name else ""
 
         if tag_name == 'ol':
             return Block.NUMBERED_LIST.value
-        if tag_name == 'ul':
+        elif tag_name == 'ul':
             return Block.BULLETED_LIST.value
-
+        elif tag_name == 'p':
+            return Block.PARAGRAPH.value
+        elif tag_name in ('h1', 'h2', 'h3', 'h4', 'h5', 'h6'):
+            return Block.HEADING.value
         if not style and tag_name == 'div':
             return Block.PARAGRAPH.value
 
-        # Remove all space such as \t \n in style
-        style = ''.join(style.split())
-        logger.info(f'Support tag {tag_name} with style {style}')
-
         css_dict = {}
         if style:
+            # Remove all space such as \t \n in style
+            style = ''.join(style.split())
             css_dict = {rule.split(':')[0].strip(): rule.split(
                 ':')[1].strip() for rule in style.split(';') if rule}
-        en_codeblock = css_dict.get('-en-codeblock', None)
-        if en_codeblock == 'true':
+        if css_dict.get('--en-blockquote', None) == 'true':
             return Block.QUOTE.value
-
+        if css_dict.get('--en-codeblock', None) == 'true':
+            return Block.CODE.value
+        if css_dict.get('-en-codeblock', None) == 'true':
+            return Block.CODE.value
+        
         return Block.FAIL.value
 
 
 Html2JsonBase.register(YinXiang_Type, Html2JsonYinXiang)
```

### Comparing `html2notion-0.1.3/html2notion/translate/notion_export.py` & `html2notion-0.1.4/html2notion/translate/notion_export.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,16 @@
                     "code": False,
                     "color": "default"
                 },
                 # "plain_text": "测试第一行",
                 "href": None
             }
         ],
-        "color": "default"
+        "color": "default",
+        "is_toggleable": False
     }
 
     delete_conf = {
         # "object": "block",
         "id": "__any__",
         "parent": "__any__",
         "created_time": "__any__",
@@ -38,15 +39,18 @@
         "last_edited_by": "__any__",
         "has_children": False,
         "archived": False,
         # "type": "paragraph",
         "paragraph": delete_block,
         "quote": delete_block,
         "numbered_list_item": delete_block,
-        "bulleted_list_item": delete_block
+        "bulleted_list_item": delete_block,
+        "heading_1": delete_block,
+        "heading_2": delete_block,
+        "heading_3": delete_block,
     }
 
     def __init__(self, api_key, page_id, page_size=2):
         self.notion = Client(auth=api_key, logger=logger)
         self.page_id = page_id
         self.page_size = page_size
         self.all_blocks = []
```

### Comparing `html2notion-0.1.3/html2notion/translate/notion_import.py` & `html2notion-0.1.4/html2notion/translate/notion_import.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,14 @@
             importer = NotionImporter(session, notion_client)
             result = await importer.process_file(file_path)
             logger.info(f"Import result: {result}")
 
 
 if __name__ == "__main__":
     test_prepare_conf()
-    file = Path("./demos/TestCaseB.html")
+    file = Path("./demos/Test Case C.html")
     notion_api_key = ""
     if 'GITHUB_ACTIONS' in os.environ:
         notion_api_key = os.environ['notion_api_key']
     else:
         notion_api_key = config['notion']['api_key']
     asyncio.run(main(file, notion_api_key))
```

### Comparing `html2notion-0.1.3/html2notion/utils/load_config.py` & `html2notion-0.1.4/html2notion/utils/load_config.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.3/html2notion/utils/log.py` & `html2notion-0.1.4/html2notion/utils/log.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.3/html2notion.egg-info/PKG-INFO` & `html2notion-0.1.4/html2notion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html2notion
-Version: 0.1.3
+Version: 0.1.4
 Summary: This tool can accurately convert HTML to Notion notes and is also useful for exporting Evernote notes to Notion.
 Home-page: https://github.com/selfboot/html2notion
 Author: selfboot
 Author-email: xuezaigds@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `html2notion-0.1.3/html2notion.egg-info/SOURCES.txt` & `html2notion-0.1.4/html2notion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.3/setup.cfg` & `html2notion-0.1.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = html2notion
-version = 0.1.3
+version = 0.1.4
 author = selfboot
 author_email = xuezaigds@gmail.com
 description = This tool can accurately convert HTML to Notion notes and is also useful for exporting Evernote notes to Notion.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/selfboot/html2notion
 license_files = LICENSE
```

### Comparing `html2notion-0.1.3/tests/test_batchimport.py` & `html2notion-0.1.4/tests/test_batchimport.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.3/tests/test_cosupload.py` & `html2notion-0.1.4/tests/test_cosupload.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.3/tests/test_notionexport.py` & `html2notion-0.1.4/tests/test_notionexport.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.3/tests/test_yinxiang.py` & `html2notion-0.1.4/tests/test_yinxiang.py`

 * *Files 27% similar despite different names*

```diff
@@ -93,108 +93,15 @@
                     "type": "text"
                 }
             ]
         }
     }
 ]
 
-quote_content = '<div style="box-sizing: border-box; padding: 8px; font-family: Monaco, Menlo, Consolas, &quot;Courier New&quot;, monospace; font-size: 12px; color: rgb(51, 51, 51); border-radius: 4px; background-color: rgb(251, 250, 248); border: 1px solid rgba(0, 0, 0, 0.15);-en-codeblock:true;"><div>Quote 1</div><div>Quote 2</div><div>Quote 3</div><div><font color="#ff2600">Quote 4(red)</font></div></div>'
-quote_block = [
-    {
-        "object": "block",
-        "type": "quote",
-        "quote": {
-            "rich_text": [
-                {
-                    "plain_text": "Quote 1\nQuote 2\nQuote 3\n",
-                    "text": {
-                        "content": "Quote 1\nQuote 2\nQuote 3\n"
-                    },
-                    "type": "text"
-                },
-                {
-                    "plain_text": "Quote 4(red)",
-                    "text": {
-                        "content": "Quote 4(red)"
-                    },
-                    "annotations": {
-                        "color": "red"
-                    },
-                    "type": "text"
-                }
-            ]
-        }
-    }
-]
-
-quote_multi_paragram = """
-<div style="box-sizing: border-box; padding: 8px; font-family: Monaco, Menlo, Consolas, &quot;Courier New&quot;, monospace; font-size: 12px; color: rgb(51, 51, 51); border-radius: 4px; background-color: rgb(251, 250, 248); border: 1px solid rgba(0, 0, 0, 0.15);-en-codeblock:true;"><div>Our models understand and process text by breaking it down into tokens. <font color="#ff9300">Tokens can be words or just chunks of characters.</font> For example, the word “hamburger” gets broken up into the tokens “ham”, “bur” and “ger”, while a short and common word like “pear” is a single token. Many tokens start with a whitespace, for example “ hello” and “ bye”.</div><div><br/></div><div>The number of tokens processed in a given API request depends on the length of both your inputs and outputs. As a rough rule of thumb, 1 token is approximately 4 characters or 0.75 words for English text. One limitation to keep in mind is that your text prompt and generated completion combined must be no more than the model's maximum context length (for most models this is 2048 tokens, or about 1500 words). Check out our <a href="https://platform.openai.com/tokenizer">tokenizer tool</a> to learn more about how text translates to tokens.</div></div>"""
-
-quote_multi_paragram_block = [
-    {
-        "object": "block",
-        "type": "paragraph",
-        "paragraph": {
-            "rich_text": []
-        }
-    },
-    {
-        "object": "block",
-        "type": "quote",
-        "quote": {
-            "rich_text": [
-                {
-                    "plain_text": "Our models understand and process text by breaking it down into tokens. ",
-                    "text": {
-                        "content": "Our models understand and process text by breaking it down into tokens. "
-                    },
-                    "type": "text"
-                },
-                {
-                    "plain_text": "Tokens can be words or just chunks of characters.",
-                    "text": {
-                        "content": "Tokens can be words or just chunks of characters."
-                    },
-                    "annotations": {
-                        "color": "orange"
-                    },
-                    "type": "text"
-                },
-                {
-                    "plain_text": " For example, the word \u201chamburger\u201d gets broken up into the tokens \u201cham\u201d, \u201cbur\u201d and \u201cger\u201d, while a short and common word like \u201cpear\u201d is a single token. Many tokens start with a whitespace, for example \u201c hello\u201d and \u201c bye\u201d.\n\nThe number of tokens processed in a given API request depends on the length of both your inputs and outputs. As a rough rule of thumb, 1 token is approximately 4 characters or 0.75 words for English text. One limitation to keep in mind is that your text prompt and generated completion combined must be no more than the model's maximum context length (for most models this is 2048 tokens, or about 1500 words). Check out our ",
-                    "text": {
-                        "content": " For example, the word \u201chamburger\u201d gets broken up into the tokens \u201cham\u201d, \u201cbur\u201d and \u201cger\u201d, while a short and common word like \u201cpear\u201d is a single token. Many tokens start with a whitespace, for example \u201c hello\u201d and \u201c bye\u201d.\n\nThe number of tokens processed in a given API request depends on the length of both your inputs and outputs. As a rough rule of thumb, 1 token is approximately 4 characters or 0.75 words for English text. One limitation to keep in mind is that your text prompt and generated completion combined must be no more than the model's maximum context length (for most models this is 2048 tokens, or about 1500 words). Check out our "
-                    },
-                    "type": "text"
-                },
-                {
-                    "href": "https://platform.openai.com/tokenizer",
-                    "plain_text": "tokenizer tool",
-                    "text": {
-                        "link": {
-                            "url": "https://platform.openai.com/tokenizer"
-                        },
-                        "content": "tokenizer tool"
-                    },
-                    "type": "text"
-                },
-                {
-                    "plain_text": " to learn more about how text translates to tokens.",
-                    "text": {
-                        "content": " to learn more about how text translates to tokens."
-                    },
-                    "type": "text"
-                }
-            ]
-        }
-    }
-]
-    
 paragram_rich_content = '<div>Normal text<span style="color: rgb(255, 38, 0);">Red text</span>, <span style="color: rgb(0, 249, 0);">Green text</span>, <span style="color: rgb(170, 121, 66);">Gray text</span><span style="color: rgb(148, 33, 146);">Purple text</span>, <span style="color: rgb(255, 147, 0);">Orange text</span>, <span style="color: rgb(255, 251, 0);">Yellow text</span><a href="http://www.baidu.com/">Link</a>, <span style="text-decoration: underline;">Underline text</span>,<span style="font-weight: bold;">Bold text</span>,<span style="text-decoration: line-through;">Strikethrough text</span>,<span style="font-style: italic;">Italic text</span></div>'
-
 paragram_rich_block = [
     {
         "object": "block",
         "type": "paragraph",
         "paragraph": {
             "rich_text": [
                 {
@@ -372,28 +279,264 @@
                     "type": "text"
                 }
             ]
         }
     }
 ]
 
+heading_content = '<h1>Heading 1</h1><h2>Heading 2</h2><h3>Heading 3</h3><h4>Heading 4</h4><h5>Heading 5</h5><h6>Heading 6</h6>'
+heading_block = [
+    {
+        "object": "block",
+        "type": "heading_1",
+        "heading_1": {
+            "rich_text": [
+                {
+                    "plain_text": "Heading 1",
+                    "text": {
+                        "content": "Heading 1"
+                    },
+                    "type": "text"
+                }
+            ]
+        }
+    },
+    {
+        "object": "block",
+        "type": "heading_2",
+        "heading_2": {
+            "rich_text": [
+                {
+                    "plain_text": "Heading 2",
+                    "text": {
+                        "content": "Heading 2"
+                    },
+                    "type": "text"
+                }
+            ]
+        }
+    },
+    {
+        "object": "block",
+        "type": "heading_3",
+        "heading_3": {
+            "rich_text": [
+                {
+                    "plain_text": "Heading 3",
+                    "text": {
+                        "content": "Heading 3"
+                    },
+                    "type": "text"
+                }
+            ]
+        }
+    },
+    {
+        "object": "block",
+        "type": "heading_3",
+        "heading_3": {
+            "rich_text": [
+                {
+                    "plain_text": "Heading 4",
+                    "text": {
+                        "content": "Heading 4"
+                    },
+                    "type": "text"
+                }
+            ]
+        }
+    },
+    {
+        "object": "block",
+        "type": "heading_3",
+        "heading_3": {
+            "rich_text": [
+                {
+                    "plain_text": "Heading 5",
+                    "text": {
+                        "content": "Heading 5"
+                    },
+                    "type": "text"
+                }
+            ]
+        }
+    },
+    {
+        "object": "block",
+        "type": "heading_3",
+        "heading_3": {
+            "rich_text": [
+                {
+                    "plain_text": "Heading 6",
+                    "text": {
+                        "content": "Heading 6"
+                    },
+                    "type": "text"
+                }
+            ]
+        }
+    }
+]
+
+
+code_content = '<div style="-en-codeblock:true;"><div>Code Line 1</div><div>Code Line 2</div><div>Code Line 3</div><div><font color="#ff2600">Code Line 4(red)</font></div></div>'
+code_block = [
+    {
+        "object": "block",
+        "type": "code",
+        "code": {
+            "rich_text": [
+                {
+                    "plain_text": "Code Line 1\nCode Line 2\nCode Line 3\n",
+                    "text": {
+                        "content": "Code Line 1\nCode Line 2\nCode Line 3\n"
+                    },
+                    "type": "text"
+                },
+                {
+                    "plain_text": "Code Line 4(red)",
+                    "text": {
+                        "content": "Code Line 4(red)"
+                    },
+                    "type": "text",
+                    "annotations": {
+                        "color": "red"
+                    }
+                }
+            ],
+            "language": "plain text"
+        }
+    }
+]
 
+code_paragraph_content = '<div style="-en-codeblock:true;"><div>Quote 1</div><div>2</div><div>3</div><div><span style="color: rgb(255, 38, 0);">Read 4</span></div><div><span style="color: rgb(255, 38, 0);">5</span></div><div>6. <a href="https://openai.com/">OpenAI</a>’s mission is to create artificial intelligence systems that benefit everyone. To that end, we invest heavily in research and engineering to ensure our AI systems are safe and secure. However, as with any <font color="#942192"><b>complex technology</b></font>, we understand that vulnerabilities and flaws can emerge.</div></div>'
+code_paragraph_block = [
+    {
+        "object": "block",
+        "type": "code",
+        "code": {
+            "rich_text": [
+                {
+                    "plain_text": "Quote 1\n2\n3\n",
+                    "text": {
+                        "content": "Quote 1\n2\n3\n"
+                    },
+                    "type": "text"
+                },
+                {
+                    "plain_text": "Read 4",
+                    "text": {
+                        "content": "Read 4"
+                    },
+                    "type": "text",
+                    "annotations": {
+                        "color": "red"
+                    }
+                },
+                {
+                    "plain_text": "\n",
+                    "text": {
+                        "content": "\n"
+                    },
+                    "type": "text"
+                },
+                {
+                    "plain_text": "5",
+                    "text": {
+                        "content": "5"
+                    },
+                    "type": "text",
+                    "annotations": {
+                        "color": "red"
+                    }
+                },
+                {
+                    "plain_text": "\n6. ",
+                    "text": {
+                        "content": "\n6. "
+                    },
+                    "type": "text"
+                },
+                {
+                    "href": "https://openai.com/",
+                    "plain_text": "OpenAI",
+                    "text": {
+                        "link": {
+                            "url": "https://openai.com/"
+                        },
+                        "content": "OpenAI"
+                    },
+                    "type": "text"
+                },
+                {
+                    "plain_text": "\u2019s mission is to create artificial intelligence systems that benefit everyone. To that end, we invest heavily in research and engineering to ensure our AI systems are safe and secure. However, as with any ",
+                    "text": {
+                        "content": "\u2019s mission is to create artificial intelligence systems that benefit everyone. To that end, we invest heavily in research and engineering to ensure our AI systems are safe and secure. However, as with any "
+                    },
+                    "type": "text"
+                },
+                {
+                    "plain_text": "complex technology",
+                    "text": {
+                        "content": "complex technology"
+                    },
+                    "type": "text",
+                    "annotations": {
+                        "color": "purple",
+                        "bold": True
+                    }
+                },
+                {
+                    "plain_text": ", we understand that vulnerabilities and flaws can emerge.",
+                    "text": {
+                        "content": ", we understand that vulnerabilities and flaws can emerge."
+                    },
+                    "type": "text"
+                }
+            ],
+            "language": "plain text"
+        }
+    }
+]
+
+language_code_content = '<div style="--en-codeblock:true;--en-codeblockLanguage:python;">import os\nprint("hello")</div>'
+language_code_block = [
+    {
+        "object": "block",
+        "type": "code",
+        "code": {
+            "rich_text": [
+                {
+                    "plain_text": "import os\nprint(\"hello\")",
+                    "text": {
+                        "content": "import os\nprint(\"hello\")"
+                    },
+                    "type": "text"
+                }
+            ],
+            "language": "python"
+        }
+    }
+]
+    
 def test_convert():
     if 'GITHUB_ACTIONS' not in os.environ:
         from html2notion.utils import test_prepare_conf, logger
         test_prepare_conf()
         logger.info("prepare_conf_fixture")
 
     html_jsons = {
         link_content: link_block,
         order_list_content: ordered_list_block,
         nested_bold_content: nested_bold_block,
-        quote_content: quote_block,
-        quote_multi_paragram: quote_multi_paragram_block,
-        paragram_rich_content: paragram_rich_block
+        paragram_rich_content: paragram_rich_block,
+        heading_content: heading_block,
+        code_content: code_block,
+        code_paragraph_content: code_paragraph_block,
+        language_code_content: language_code_block
     }
 
     for html_content in html_jsons:
         body_content = '<body>' + html_content + '</body>'
         yinxiang = Html2JsonYinXiang(body_content)
         yinxiang.process()
         json_obj = yinxiang.children
```

#### html2text {}

```diff
@@ -16,71 +16,15 @@
 { "object": "block", "numbered_list_item": { "rich_text": [ { "plain_text":
 "third", "text": { "content": "third" }, "type": "text" } ] }, "type":
 "numbered_list_item" } ] nested_bold_content = '
 underline_bold
 ' nested_bold_block = [ { "object": "block", "type": "paragraph", "paragraph":
 { "rich_text": [ { "plain_text": "underline bold", "text": { "content":
 "underline bold" }, "annotations": { "bold": True, "underline": True }, "type":
-"text" } ] } } ] quote_content = '
-Quote 1
-Quote 2
-Quote 3
-Quote 4(red)
-' quote_block = [ { "object": "block", "type": "quote", "quote": { "rich_text":
-[ { "plain_text": "Quote 1\nQuote 2\nQuote 3\n", "text": { "content": "Quote
-1\nQuote 2\nQuote 3\n" }, "type": "text" }, { "plain_text": "Quote 4(red)",
-"text": { "content": "Quote 4(red)" }, "annotations": { "color": "red" },
-"type": "text" } ] } } ] quote_multi_paragram = """
-Our models understand and process text by breaking it down into tokens. Tokens
-can be words or just chunks of characters. For example, the word
-âhamburgerâ gets broken up into the tokens âhamâ, âburâ and
-âgerâ, while a short and common word like âpearâ is a single token.
-Many tokens start with a whitespace, for example â helloâ and â byeâ.
-
-The number of tokens processed in a given API request depends on the length of
-both your inputs and outputs. As a rough rule of thumb, 1 token is
-approximately 4 characters or 0.75 words for English text. One limitation to
-keep in mind is that your text prompt and generated completion combined must be
-no more than the model's maximum context length (for most models this is 2048
-tokens, or about 1500 words). Check out our tokenizer_tool to learn more about
-how text translates to tokens.
-""" quote_multi_paragram_block = [ { "object": "block", "type": "paragraph",
-"paragraph": { "rich_text": [] } }, { "object": "block", "type": "quote",
-"quote": { "rich_text": [ { "plain_text": "Our models understand and process
-text by breaking it down into tokens. ", "text": { "content": "Our models
-understand and process text by breaking it down into tokens. " }, "type":
-"text" }, { "plain_text": "Tokens can be words or just chunks of characters.",
-"text": { "content": "Tokens can be words or just chunks of characters." },
-"annotations": { "color": "orange" }, "type": "text" }, { "plain_text": " For
-example, the word \u201chamburger\u201d gets broken up into the tokens
-\u201cham\u201d, \u201cbur\u201d and \u201cger\u201d, while a short and common
-word like \u201cpear\u201d is a single token. Many tokens start with a
-whitespace, for example \u201c hello\u201d and \u201c bye\u201d.\n\nThe number
-of tokens processed in a given API request depends on the length of both your
-inputs and outputs. As a rough rule of thumb, 1 token is approximately 4
-characters or 0.75 words for English text. One limitation to keep in mind is
-that your text prompt and generated completion combined must be no more than
-the model's maximum context length (for most models this is 2048 tokens, or
-about 1500 words). Check out our ", "text": { "content": " For example, the
-word \u201chamburger\u201d gets broken up into the tokens \u201cham\u201d,
-\u201cbur\u201d and \u201cger\u201d, while a short and common word like
-\u201cpear\u201d is a single token. Many tokens start with a whitespace, for
-example \u201c hello\u201d and \u201c bye\u201d.\n\nThe number of tokens
-processed in a given API request depends on the length of both your inputs and
-outputs. As a rough rule of thumb, 1 token is approximately 4 characters or
-0.75 words for English text. One limitation to keep in mind is that your text
-prompt and generated completion combined must be no more than the model's
-maximum context length (for most models this is 2048 tokens, or about 1500
-words). Check out our " }, "type": "text" }, { "href": "https://
-platform.openai.com/tokenizer", "plain_text": "tokenizer tool", "text":
-{ "link": { "url": "https://platform.openai.com/tokenizer" }, "content":
-"tokenizer tool" }, "type": "text" }, { "plain_text": " to learn more about how
-text translates to tokens.", "text": { "content": " to learn more about how
-text translates to tokens." }, "type": "text" } ] } } ] paragram_rich_content =
-'
+"text" } ] } } ] paragram_rich_content = '
 Normal textRed text, Green text, Gray textPurple text, Orange text, Yellow
 textLink, Underline text,Bold text,Strikethrough text,Italic text
 ' paragram_rich_block = [ { "object": "block", "type": "paragraph",
 "paragraph": { "rich_text": [ { "plain_text": "Normal text", "text":
 { "content": "Normal text" }, "type": "text" }, { "plain_text": "Red text",
 "text": { "content": "Red text" }, "annotations": { "color": "red" }, "type":
 "text" }, { "plain_text": ", ", "text": { "content": ", " }, "type": "text" },
@@ -103,18 +47,84 @@
 "type": "text" }, { "plain_text": "Bold text", "text": { "content": "Bold text"
 }, "annotations": { "bold": True }, "type": "text" }, { "plain_text": ",",
 "text": { "content": "," }, "type": "text" }, { "plain_text": "Strikethrough
 text", "text": { "content": "Strikethrough text" }, "annotations":
 { "strikethrough": True }, "type": "text" }, { "plain_text": ",", "text":
 { "content": "," }, "type": "text" }, { "plain_text": "Italic text", "text":
 { "content": "Italic text" }, "annotations": { "italic": True }, "type": "text"
-} ] } } ] def test_convert(): if 'GITHUB_ACTIONS' not in os.environ: from
+} ] } } ] heading_content = '
+****** Heading 1 ******
+***** Heading 2 *****
+**** Heading 3 ****
+*** Heading 4 ***
+** Heading 5 **
+* Heading 6 *
+' heading_block = [ { "object": "block", "type": "heading_1", "heading_1":
+{ "rich_text": [ { "plain_text": "Heading 1", "text": { "content": "Heading 1"
+}, "type": "text" } ] } }, { "object": "block", "type": "heading_2",
+"heading_2": { "rich_text": [ { "plain_text": "Heading 2", "text": { "content":
+"Heading 2" }, "type": "text" } ] } }, { "object": "block", "type":
+"heading_3", "heading_3": { "rich_text": [ { "plain_text": "Heading 3", "text":
+{ "content": "Heading 3" }, "type": "text" } ] } }, { "object": "block",
+"type": "heading_3", "heading_3": { "rich_text": [ { "plain_text": "Heading 4",
+"text": { "content": "Heading 4" }, "type": "text" } ] } }, { "object":
+"block", "type": "heading_3", "heading_3": { "rich_text": [ { "plain_text":
+"Heading 5", "text": { "content": "Heading 5" }, "type": "text" } ] } },
+{ "object": "block", "type": "heading_3", "heading_3": { "rich_text": [
+{ "plain_text": "Heading 6", "text": { "content": "Heading 6" }, "type": "text"
+} ] } } ] code_content = '
+Code Line 1
+Code Line 2
+Code Line 3
+Code Line 4(red)
+' code_block = [ { "object": "block", "type": "code", "code": { "rich_text": [
+{ "plain_text": "Code Line 1\nCode Line 2\nCode Line 3\n", "text": { "content":
+"Code Line 1\nCode Line 2\nCode Line 3\n" }, "type": "text" }, { "plain_text":
+"Code Line 4(red)", "text": { "content": "Code Line 4(red)" }, "type": "text",
+"annotations": { "color": "red" } } ], "language": "plain text" } } ]
+code_paragraph_content = '
+Quote 1
+2
+3
+Read 4
+5
+6. OpenAIâs mission is to create artificial intelligence systems that benefit
+everyone. To that end, we invest heavily in research and engineering to ensure
+our AI systems are safe and secure. However, as with any complex technology, we
+understand that vulnerabilities and flaws can emerge.
+' code_paragraph_block = [ { "object": "block", "type": "code", "code":
+{ "rich_text": [ { "plain_text": "Quote 1\n2\n3\n", "text": { "content": "Quote
+1\n2\n3\n" }, "type": "text" }, { "plain_text": "Read 4", "text": { "content":
+"Read 4" }, "type": "text", "annotations": { "color": "red" } },
+{ "plain_text": "\n", "text": { "content": "\n" }, "type": "text" },
+{ "plain_text": "5", "text": { "content": "5" }, "type": "text", "annotations":
+{ "color": "red" } }, { "plain_text": "\n6. ", "text": { "content": "\n6. " },
+"type": "text" }, { "href": "https://openai.com/", "plain_text": "OpenAI",
+"text": { "link": { "url": "https://openai.com/" }, "content": "OpenAI" },
+"type": "text" }, { "plain_text": "\u2019s mission is to create artificial
+intelligence systems that benefit everyone. To that end, we invest heavily in
+research and engineering to ensure our AI systems are safe and secure. However,
+as with any ", "text": { "content": "\u2019s mission is to create artificial
+intelligence systems that benefit everyone. To that end, we invest heavily in
+research and engineering to ensure our AI systems are safe and secure. However,
+as with any " }, "type": "text" }, { "plain_text": "complex technology",
+"text": { "content": "complex technology" }, "type": "text", "annotations":
+{ "color": "purple", "bold": True } }, { "plain_text": ", we understand that
+vulnerabilities and flaws can emerge.", "text": { "content": ", we understand
+that vulnerabilities and flaws can emerge." }, "type": "text" } ], "language":
+"plain text" } } ] language_code_content = '
+import os\nprint("hello")
+' language_code_block = [ { "object": "block", "type": "code", "code":
+{ "rich_text": [ { "plain_text": "import os\nprint(\"hello\")", "text":
+{ "content": "import os\nprint(\"hello\")" }, "type": "text" } ], "language":
+"python" } } ] def test_convert(): if 'GITHUB_ACTIONS' not in os.environ: from
 html2notion.utils import test_prepare_conf, logger test_prepare_conf()
 logger.info("prepare_conf_fixture") html_jsons = { link_content: link_block,
 order_list_content: ordered_list_block, nested_bold_content: nested_bold_block,
-quote_content: quote_block, quote_multi_paragram: quote_multi_paragram_block,
-paragram_rich_content: paragram_rich_block } for html_content in html_jsons:
+paragram_rich_content: paragram_rich_block, heading_content: heading_block,
+code_content: code_block, code_paragraph_content: code_paragraph_block,
+language_code_content: language_code_block } for html_content in html_jsons:
 body_content = '
 ' + html_content + '
 ' yinxiang = Html2JsonYinXiang(body_content) yinxiang.process() json_obj =
 yinxiang.children # print(json.dumps(json_obj, indent=4)) assert json_obj ==
 html_jsons[html_content] if __name__ == '__main__': test_convert()
```

