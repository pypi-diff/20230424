# Comparing `tmp/appstream-python-0.6.tar.gz` & `tmp/appstream-python-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appstream-python-0.6.tar", last modified: Tue Apr 11 13:01:28 2023, max compression
+gzip compressed data, was "appstream-python-0.6.1.tar", last modified: Mon Apr 24 13:23:40 2023, max compression
```

## Comparing `appstream-python-0.6.tar` & `appstream-python-0.6.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:01:28.729500 appstream-python-0.6/
--rw-r--r--   0 root         (0) root         (0)     1318 2023-04-11 13:00:59.000000 appstream-python-0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       71 2023-04-11 13:00:59.000000 appstream-python-0.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1284 2023-04-11 13:01:28.729500 appstream-python-0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      112 2023-04-11 13:00:59.000000 appstream-python-0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:01:28.729500 appstream-python-0.6/appstream_python/
--rw-r--r--   0 root         (0) root         (0)     2777 2023-04-11 13:00:59.000000 appstream-python-0.6/appstream_python/Collection.py
--rw-r--r--   0 root         (0) root         (0)    35396 2023-04-11 13:00:59.000000 appstream-python-0.6/appstream_python/Component.py
--rw-r--r--   0 root         (0) root         (0)     2186 2023-04-11 13:00:59.000000 appstream-python-0.6/appstream_python/StandardConstants.py
--rw-r--r--   0 root         (0) root         (0)      164 2023-04-11 13:00:59.000000 appstream-python-0.6/appstream_python/__init__.py
--rw-r--r--   0 root         (0) root         (0)      326 2023-04-11 13:00:59.000000 appstream-python-0.6/appstream_python/_helper.py
--rw-r--r--   0 root         (0) root         (0)        4 2023-04-11 13:00:59.000000 appstream-python-0.6/appstream_python/version.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:01:28.729500 appstream-python-0.6/appstream_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1284 2023-04-11 13:01:28.000000 appstream-python-0.6/appstream_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      512 2023-04-11 13:01:28.000000 appstream-python-0.6/appstream_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 13:01:28.000000 appstream-python-0.6/appstream_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-11 13:01:28.000000 appstream-python-0.6/appstream_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-04-11 13:01:28.000000 appstream-python-0.6/appstream_python.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1366 2023-04-11 13:00:59.000000 appstream-python-0.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 13:01:28.729500 appstream-python-0.6/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:01:28.729500 appstream-python-0.6/tests/
--rw-r--r--   0 root         (0) root         (0)     1114 2023-04-11 13:00:59.000000 appstream-python-0.6/tests/test_appstream_data.py
--rw-r--r--   0 root         (0) root         (0)     1147 2023-04-11 13:00:59.000000 appstream-python-0.6/tests/test_description.py
--rw-r--r--   0 root         (0) root         (0)     2982 2023-04-11 13:00:59.000000 appstream-python-0.6/tests/test_display_length.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:40.035801 appstream-python-0.6.1/
+-rw-r--r--   0 root         (0) root         (0)     1318 2023-04-24 13:22:10.000000 appstream-python-0.6.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       71 2023-04-24 13:22:10.000000 appstream-python-0.6.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1286 2023-04-24 13:23:40.035801 appstream-python-0.6.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      112 2023-04-24 13:22:10.000000 appstream-python-0.6.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:40.035801 appstream-python-0.6.1/appstream_python/
+-rw-r--r--   0 root         (0) root         (0)     2777 2023-04-24 13:22:10.000000 appstream-python-0.6.1/appstream_python/Collection.py
+-rw-r--r--   0 root         (0) root         (0)    35641 2023-04-24 13:22:10.000000 appstream-python-0.6.1/appstream_python/Component.py
+-rw-r--r--   0 root         (0) root         (0)     2186 2023-04-24 13:22:10.000000 appstream-python-0.6.1/appstream_python/StandardConstants.py
+-rw-r--r--   0 root         (0) root         (0)      164 2023-04-24 13:22:10.000000 appstream-python-0.6.1/appstream_python/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      326 2023-04-24 13:22:10.000000 appstream-python-0.6.1/appstream_python/_helper.py
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-24 13:22:10.000000 appstream-python-0.6.1/appstream_python/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:40.035801 appstream-python-0.6.1/appstream_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1286 2023-04-24 13:23:40.000000 appstream-python-0.6.1/appstream_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      512 2023-04-24 13:23:40.000000 appstream-python-0.6.1/appstream_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 13:23:40.000000 appstream-python-0.6.1/appstream_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-04-24 13:23:40.000000 appstream-python-0.6.1/appstream_python.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-04-24 13:23:40.000000 appstream-python-0.6.1/appstream_python.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1366 2023-04-24 13:22:10.000000 appstream-python-0.6.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 13:23:40.035801 appstream-python-0.6.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:40.035801 appstream-python-0.6.1/tests/
+-rw-r--r--   0 root         (0) root         (0)     1114 2023-04-24 13:22:10.000000 appstream-python-0.6.1/tests/test_appstream_data.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2023-04-24 13:22:10.000000 appstream-python-0.6.1/tests/test_description.py
+-rw-r--r--   0 root         (0) root         (0)     2982 2023-04-24 13:22:10.000000 appstream-python-0.6.1/tests/test_display_length.py
```

### Comparing `appstream-python-0.6/LICENSE` & `appstream-python-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `appstream-python-0.6/PKG-INFO` & `appstream-python-0.6.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appstream-python
-Version: 0.6
+Version: 0.6.1
 Summary: A library for dealing with Freedesktop Appstream data
 Author-email: JakobDev <jakobdev@gmx.de>
 License: BSD-2-Clause
 Project-URL: Documentation, https://appstream-python.readthedocs.io
 Project-URL: Issues, https://codeberg.org/JakobDev/appstream-python/issues
 Project-URL: Source, https://codeberg.org/JakobDev/appstream-python
 Project-URL: Donation, https://ko-fi.com/jakobdev
```

### Comparing `appstream-python-0.6/appstream_python/Collection.py` & `appstream-python-0.6.1/appstream_python/Collection.py`

 * *Files identical despite different names*

### Comparing `appstream-python-0.6/appstream_python/Component.py` & `appstream-python-0.6.1/appstream_python/Component.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,17 +65,23 @@
         """Returns a list with all languages of the tag"""
         return list(self._translations.keys())
 
     def load_tags(self, tag_list: list[etree.Element]) -> None:
         """Load a list of Tags"""
         for i in tag_list:
             if i.get("{http://www.w3.org/XML/1998/namespace}lang") is None:
-                self._text = i.text.strip()
+                if i.text is not None:
+                    self._text = i.text.strip()
+                else:
+                    self._text = ""
             else:
-                self._translations[i.get("{http://www.w3.org/XML/1998/namespace}lang")] = i.text.strip()
+                if i.text is not None:
+                    self._translations[i.get(_XML_LANG)] = i.text.strip()
+                else:
+                    self._translations[i.get(_XML_LANG)] = ""
 
     def write_tags(self, parent_tag: etree.Element, tag_name: str) -> None:
         """Writes a Tag"""
         default_tag = etree.SubElement(parent_tag, tag_name)
         default_tag.text = self._text
 
         for key, value in self._translations.items():
@@ -117,15 +123,16 @@
         if tag.get("{http://www.w3.org/XML/1998/namespace}lang") is None:
             current_text = ""
             for i in tag.getchildren():
                 if i.get(_XML_LANG) is None:
                     current_text = i.text.strip()
                     self._translated_data[current_text] = {}
                 else:
-                    self._translated_data[current_text][i.get(_XML_LANG)] = i.text.strip()
+                    if current_text in self._translated_data:
+                        self._translated_data[current_text][i.get(_XML_LANG)] = i.text.strip()
         else:
             if tag.get("{http://www.w3.org/XML/1998/namespace}lang") not in self._translated_lists:
                 self._translated_lists[tag.get("{http://www.w3.org/XML/1998/namespace}lang")] = []
             for i in tag.getchildren():
                 self._translated_lists[tag.get("{http://www.w3.org/XML/1998/namespace}lang")].append(i.text.strip())
 
     def write_all_tag(self, parent_tag: etree.Element, tag_name: str) -> None:
@@ -434,19 +441,19 @@
             self.images.append(img)
 
         self.caption.load_tags(tag.findall("caption"))
 
 
 class DisplayLength:
     "Represents a <display_length> tag"
-    def __init__(self, px: int = 0, compare: Optional[str] = None) -> None:
+    def __init__(self, px: int = 0, compare: str = "ge") -> None:
         self.px: int = px
         "The logical pixels"
 
-        self.compare: Optional[str] = compare
+        self.compare: str = compare
         "Compare"
 
     def compare_px(self, value: int) -> bool:
         """
         Compares the length with the given logical pixels
 
         :param value: The logical pixels to compare
@@ -474,15 +481,15 @@
         display_length = cls()
 
         try:
             display_length.px = int(tag.text)
         except ValueError:
             display_length.px = cls.string_to_px(tag.text)
 
-        display_length.compare = tag.get("compare")
+        display_length.compare = tag.get("compare", "ge")
 
         return display_length
 
     @staticmethod
     def string_to_px(string: str) -> int:
         """
         Converts a Lenght String (e.g.small) to logical pixels value
```

### Comparing `appstream-python-0.6/appstream_python/StandardConstants.py` & `appstream-python-0.6.1/appstream_python/StandardConstants.py`

 * *Files identical despite different names*

### Comparing `appstream-python-0.6/appstream_python.egg-info/PKG-INFO` & `appstream-python-0.6.1/appstream_python.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appstream-python
-Version: 0.6
+Version: 0.6.1
 Summary: A library for dealing with Freedesktop Appstream data
 Author-email: JakobDev <jakobdev@gmx.de>
 License: BSD-2-Clause
 Project-URL: Documentation, https://appstream-python.readthedocs.io
 Project-URL: Issues, https://codeberg.org/JakobDev/appstream-python/issues
 Project-URL: Source, https://codeberg.org/JakobDev/appstream-python
 Project-URL: Donation, https://ko-fi.com/jakobdev
```

### Comparing `appstream-python-0.6/appstream_python.egg-info/SOURCES.txt` & `appstream-python-0.6.1/appstream_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `appstream-python-0.6/pyproject.toml` & `appstream-python-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `appstream-python-0.6/tests/test_appstream_data.py` & `appstream-python-0.6.1/tests/test_appstream_data.py`

 * *Files identical despite different names*

### Comparing `appstream-python-0.6/tests/test_description.py` & `appstream-python-0.6.1/tests/test_description.py`

 * *Files identical despite different names*

### Comparing `appstream-python-0.6/tests/test_display_length.py` & `appstream-python-0.6.1/tests/test_display_length.py`

 * *Files identical despite different names*

