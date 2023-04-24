# Comparing `tmp/ssb_altinn_python-0.2.0.tar.gz` & `tmp/ssb_altinn_python-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_altinn_python-0.2.0.tar", max compression
+gzip compressed data, was "ssb_altinn_python-0.2.1.tar", max compression
```

## Comparing `ssb_altinn_python-0.2.0.tar` & `ssb_altinn_python-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1078 2023-04-24 10:28:54.669603 ssb_altinn_python-0.2.0/LICENSE
--rw-r--r--   0        0        0     3626 2023-04-24 10:28:54.669603 ssb_altinn_python-0.2.0/README.md
--rw-r--r--   0        0        0     1967 2023-04-24 10:29:13.517774 ssb_altinn_python-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      131 2023-04-24 10:28:54.669603 ssb_altinn_python-0.2.0/src/altinn/__init__.py
--rw-r--r--   0        0        0      198 2023-04-24 10:29:13.517774 ssb_altinn_python-0.2.0/src/altinn/__main__.py
--rw-r--r--   0        0        0     1831 2023-04-24 10:28:54.669603 ssb_altinn_python-0.2.0/src/altinn/file.py
--rw-r--r--   0        0        0      419 2023-04-24 10:28:54.669603 ssb_altinn_python-0.2.0/src/altinn/flatten.py
--rw-r--r--   0        0        0     2327 2023-04-24 10:28:54.669603 ssb_altinn_python-0.2.0/src/altinn/parser.py
--rw-r--r--   0        0        0        0 2023-04-24 10:28:54.669603 ssb_altinn_python-0.2.0/src/altinn/py.typed
--rw-r--r--   0        0        0      497 2023-04-24 10:28:54.669603 ssb_altinn_python-0.2.0/src/altinn/utils.py
--rw-r--r--   0        0        0     4555 1970-01-01 00:00:00.000000 ssb_altinn_python-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-04-24 11:01:56.658266 ssb_altinn_python-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3626 2023-04-24 11:01:56.658266 ssb_altinn_python-0.2.1/README.md
+-rw-r--r--   0        0        0     1967 2023-04-24 11:02:10.830386 ssb_altinn_python-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      131 2023-04-24 11:01:56.658266 ssb_altinn_python-0.2.1/src/altinn/__init__.py
+-rw-r--r--   0        0        0      198 2023-04-24 11:01:56.658266 ssb_altinn_python-0.2.1/src/altinn/__main__.py
+-rw-r--r--   0        0        0     1831 2023-04-24 11:01:56.658266 ssb_altinn_python-0.2.1/src/altinn/file.py
+-rw-r--r--   0        0        0      419 2023-04-24 11:01:56.658266 ssb_altinn_python-0.2.1/src/altinn/flatten.py
+-rw-r--r--   0        0        0     2366 2023-04-24 11:02:10.830386 ssb_altinn_python-0.2.1/src/altinn/parser.py
+-rw-r--r--   0        0        0        0 2023-04-24 11:01:56.658266 ssb_altinn_python-0.2.1/src/altinn/py.typed
+-rw-r--r--   0        0        0      497 2023-04-24 11:01:56.658266 ssb_altinn_python-0.2.1/src/altinn/utils.py
+-rw-r--r--   0        0        0     4555 1970-01-01 00:00:00.000000 ssb_altinn_python-0.2.1/PKG-INFO
```

### Comparing `ssb_altinn_python-0.2.0/LICENSE` & `ssb_altinn_python-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_altinn_python-0.2.0/README.md` & `ssb_altinn_python-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ssb_altinn_python-0.2.0/pyproject.toml` & `ssb_altinn_python-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssb-altinn-python"
-version = "0.2.0"
+version = "0.2.1"
 description = "SSB Altinn Python"
 authors = ["Øyvind Bruer-Skarsbø <obr@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/skars82/ssb-altinn-python"
 repository = "https://github.com/skars82/ssb-altinn-python"
 documentation = "https://ssb-altinn-python.readthedocs.io"
```

### Comparing `ssb_altinn_python-0.2.0/src/altinn/file.py` & `ssb_altinn_python-0.2.1/src/altinn/file.py`

 * *Files identical despite different names*

### Comparing `ssb_altinn_python-0.2.0/src/altinn/parser.py` & `ssb_altinn_python-0.2.1/src/altinn/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,18 +65,18 @@
             if element is None:
                 element = kontakt.find(tag)
             if element is None:
                 element = skjemadata.find(tag)
             if element is not None:
                 value = element.text
                 data.append(value)
+                result_dict[tag] = value
             else:
                 data.append(None)
-
-                result_dict[tag] = value
+                result_dict[tag] = None
 
         return result_dict
 
     def to_dataframe(self) -> pd.DataFrame:
         """Parse single XML file to a pandas DataFrame.
 
         Returns:
```

### Comparing `ssb_altinn_python-0.2.0/PKG-INFO` & `ssb_altinn_python-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssb-altinn-python
-Version: 0.2.0
+Version: 0.2.1
 Summary: SSB Altinn Python
 Home-page: https://github.com/skars82/ssb-altinn-python
 License: MIT
 Author: Øyvind Bruer-Skarsbø
 Author-email: obr@ssb.no
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

