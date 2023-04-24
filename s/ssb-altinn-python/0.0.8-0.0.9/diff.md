# Comparing `tmp/ssb_altinn_python-0.0.8.tar.gz` & `tmp/ssb_altinn_python-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_altinn_python-0.0.8.tar", max compression
+gzip compressed data, was "ssb_altinn_python-0.0.9.tar", max compression
```

## Comparing `ssb_altinn_python-0.0.8.tar` & `ssb_altinn_python-0.0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1078 2023-04-23 17:11:56.083030 ssb_altinn_python-0.0.8/LICENSE
--rw-r--r--   0        0        0     3329 2023-04-23 17:11:56.083030 ssb_altinn_python-0.0.8/README.md
--rw-r--r--   0        0        0     1936 2023-04-23 17:12:15.463185 ssb_altinn_python-0.0.8/pyproject.toml
--rw-r--r--   0        0        0       78 2023-04-23 17:11:56.083030 ssb_altinn_python-0.0.8/src/altinn/__init__.py
--rw-r--r--   0        0        0      116 2023-04-23 17:11:56.083030 ssb_altinn_python-0.0.8/src/altinn/__main__.py
--rw-r--r--   0        0        0     2497 2023-04-23 17:12:15.463185 ssb_altinn_python-0.0.8/src/altinn/file.py
--rw-r--r--   0        0        0      419 2023-04-23 17:11:56.083030 ssb_altinn_python-0.0.8/src/altinn/flatten.py
--rw-r--r--   0        0        0       35 2023-04-23 17:11:56.083030 ssb_altinn_python-0.0.8/src/altinn/parser.py
--rw-r--r--   0        0        0        0 2023-04-23 17:11:56.083030 ssb_altinn_python-0.0.8/src/altinn/py.typed
--rw-r--r--   0        0        0       56 2023-04-23 17:11:56.087030 ssb_altinn_python-0.0.8/src/altinn/utils.py
--rw-r--r--   0        0        0     4204 1970-01-01 00:00:00.000000 ssb_altinn_python-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-04-24 09:23:25.688091 ssb_altinn_python-0.0.9/LICENSE
+-rw-r--r--   0        0        0     3626 2023-04-24 09:23:39.112791 ssb_altinn_python-0.0.9/README.md
+-rw-r--r--   0        0        0     1936 2023-04-24 09:23:39.112791 ssb_altinn_python-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0       96 2023-04-24 09:23:39.112791 ssb_altinn_python-0.0.9/src/altinn/__init__.py
+-rw-r--r--   0        0        0      116 2023-04-24 09:23:25.692091 ssb_altinn_python-0.0.9/src/altinn/__main__.py
+-rw-r--r--   0        0        0     1831 2023-04-24 09:23:39.112791 ssb_altinn_python-0.0.9/src/altinn/file.py
+-rw-r--r--   0        0        0      419 2023-04-24 09:23:25.692091 ssb_altinn_python-0.0.9/src/altinn/flatten.py
+-rw-r--r--   0        0        0     1853 2023-04-24 09:23:39.112791 ssb_altinn_python-0.0.9/src/altinn/parser.py
+-rw-r--r--   0        0        0        0 2023-04-24 09:23:25.692091 ssb_altinn_python-0.0.9/src/altinn/py.typed
+-rw-r--r--   0        0        0      497 2023-04-24 09:23:39.112791 ssb_altinn_python-0.0.9/src/altinn/utils.py
+-rw-r--r--   0        0        0     4501 1970-01-01 00:00:00.000000 ssb_altinn_python-0.0.9/PKG-INFO
```

### Comparing `ssb_altinn_python-0.0.8/LICENSE` & `ssb_altinn_python-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_altinn_python-0.0.8/README.md` & `ssb_altinn_python-0.0.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -34,14 +34,21 @@
 
 # Get file filename without '.xml'-postfix
 form.filename()
 # Returns: 'form_dc551844cd74'
 
 # Print a nicely formatted version of the file
 form.pretty_print()
+
+# Print an unformatted version of the file. Does not require the file to be parseable by an xml-library. Useful for inspecting unvalid xml-files.
+form.print()
+
+# Check if xml-file is valid. Useful to inspect xml-files with formal errors in the xml-schema.
+form.validate()
+# Returns True og False
 ```
 
 ## Requirements
 
 - dapla-toolbelt >=1.6.2,<2.0.0
 - defusedxml >=0.7.1,<0.8.0
 - pytest >=7.2.2,<8.0.0
```

### Comparing `ssb_altinn_python-0.0.8/pyproject.toml` & `ssb_altinn_python-0.0.9/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssb-altinn-python"
-version = "0.0.8"
+version = "0.0.9"
 description = "SSB Altinn Python"
 authors = ["Øyvind Bruer-Skarsbø <obr@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/skars82/ssb-altinn-python"
 repository = "https://github.com/skars82/ssb-altinn-python"
 documentation = "https://ssb-altinn-python.readthedocs.io"
```

### Comparing `ssb_altinn_python-0.0.8/src/altinn/file.py` & `ssb_altinn_python-0.0.9/src/altinn/file.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,39 @@
 """This module contains the main function for running the Altinn application."""
 
-import os
-from typing import Optional
-
 from dapla import FileClient
 from defusedxml.ElementTree import ParseError
 from defusedxml.minidom import parseString
 
+from .utils import is_dapla
+
 
 def main() -> None:
     """Placeholder function for the main function.
 
     This function is called when the altinn package is run as a script.
     """
     pass
 
 
-def is_dapla() -> bool:
-    """Check whether the current environment is running a Dapla JupyterLab instance.
-
-    Returns:
-        bool: True if the current environment is running a Dapla JupyterLab instance,
-        False otherwise.
-    """
-    jupyter_image_spec: Optional[str] = os.environ.get("JUPYTER_IMAGE_SPEC")
-    return bool(jupyter_image_spec and "dapla-jupyterlab" in jupyter_image_spec)
-
-
 class FileInfo:
     """This class represents an Altinn application."""
 
     def __init__(self, file_path: str) -> None:
         """Initialize an XmlFile object with the given file path.
 
         Args:
             file_path (str): The path to the XML file.
         """
-        if is_dapla():
-            self.file_path = file_path
-        else:
+        self.file_path = file_path
+        if not is_dapla():
             print(
                 """FileInfo class can only be instantiated in a Dapla JupyterLab
                   environment."""
             )
-            # Alternatively, you can print a message and return,
-            # without raising an exception
-            # print("XmlFile class can only be instantiated in a Dapla
-            # JupyterLab environment.")
-            # return
 
     def filename(self) -> str:
         """Get the name of the XML file.
 
         Returns:
             str: The name of the XML file.
         """
```

### Comparing `ssb_altinn_python-0.0.8/PKG-INFO` & `ssb_altinn_python-0.0.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssb-altinn-python
-Version: 0.0.8
+Version: 0.0.9
 Summary: SSB Altinn Python
 Home-page: https://github.com/skars82/ssb-altinn-python
 License: MIT
 Author: Øyvind Bruer-Skarsbø
 Author-email: obr@ssb.no
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -56,14 +56,21 @@
 
 # Get file filename without '.xml'-postfix
 form.filename()
 # Returns: 'form_dc551844cd74'
 
 # Print a nicely formatted version of the file
 form.pretty_print()
+
+# Print an unformatted version of the file. Does not require the file to be parseable by an xml-library. Useful for inspecting unvalid xml-files.
+form.print()
+
+# Check if xml-file is valid. Useful to inspect xml-files with formal errors in the xml-schema.
+form.validate()
+# Returns True og False
 ```
 
 ## Requirements
 
 - dapla-toolbelt >=1.6.2,<2.0.0
 - defusedxml >=0.7.1,<0.8.0
 - pytest >=7.2.2,<8.0.0
```

