# Comparing `tmp/ttk-custom-msgbox-0.0.2.tar.gz` & `tmp/ttk-custom-msgbox-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttk-custom-msgbox-0.0.2.tar", last modified: Mon Apr 24 19:26:05 2023, max compression
+gzip compressed data, was "ttk-custom-msgbox-0.0.3.tar", last modified: Mon Apr 24 19:40:06 2023, max compression
```

## Comparing `ttk-custom-msgbox-0.0.2.tar` & `ttk-custom-msgbox-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 19:26:05.493014 ttk-custom-msgbox-0.0.2/
--rw-rw-rw-   0        0        0     1090 2023-04-24 18:00:24.000000 ttk-custom-msgbox-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     4922 2023-04-24 19:26:05.493014 ttk-custom-msgbox-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4309 2023-04-24 19:25:59.000000 ttk-custom-msgbox-0.0.2/README.md
--rw-rw-rw-   0        0        0      109 2023-04-24 19:04:53.000000 ttk-custom-msgbox-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      791 2023-04-24 19:26:05.494014 ttk-custom-msgbox-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-24 19:26:05.481013 ttk-custom-msgbox-0.0.2/ttk_custom_msgbox/
-drwxrwxrwx   0        0        0        0 2023-04-24 19:26:05.492015 ttk-custom-msgbox-0.0.2/ttk_custom_msgbox/ttk_custom_msgbox.egg-info/
--rw-rw-rw-   0        0        0     4922 2023-04-24 19:26:05.000000 ttk-custom-msgbox-0.0.2/ttk_custom_msgbox/ttk_custom_msgbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-04-24 19:26:05.000000 ttk-custom-msgbox-0.0.2/ttk_custom_msgbox/ttk_custom_msgbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 19:26:05.000000 ttk-custom-msgbox-0.0.2/ttk_custom_msgbox/ttk_custom_msgbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 19:26:05.000000 ttk-custom-msgbox-0.0.2/ttk_custom_msgbox/ttk_custom_msgbox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 19:40:06.166932 ttk-custom-msgbox-0.0.3/
+-rw-rw-rw-   0        0        0     1090 2023-04-24 18:00:24.000000 ttk-custom-msgbox-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     4922 2023-04-24 19:40:06.166932 ttk-custom-msgbox-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4309 2023-04-24 19:38:33.000000 ttk-custom-msgbox-0.0.3/README.md
+-rw-rw-rw-   0        0        0      109 2023-04-24 19:04:53.000000 ttk-custom-msgbox-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      791 2023-04-24 19:40:06.169932 ttk-custom-msgbox-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-24 19:40:06.153932 ttk-custom-msgbox-0.0.3/ttk_custom_msgbox/
+drwxrwxrwx   0        0        0        0 2023-04-24 19:40:06.165933 ttk-custom-msgbox-0.0.3/ttk_custom_msgbox/ttk_custom_msgbox.egg-info/
+-rw-rw-rw-   0        0        0     4922 2023-04-24 19:40:06.000000 ttk-custom-msgbox-0.0.3/ttk_custom_msgbox/ttk_custom_msgbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2023-04-24 19:40:06.000000 ttk-custom-msgbox-0.0.3/ttk_custom_msgbox/ttk_custom_msgbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 19:40:06.000000 ttk-custom-msgbox-0.0.3/ttk_custom_msgbox/ttk_custom_msgbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 19:40:06.000000 ttk-custom-msgbox-0.0.3/ttk_custom_msgbox/ttk_custom_msgbox.egg-info/top_level.txt
```

### Comparing `ttk-custom-msgbox-0.0.2/LICENSE` & `ttk-custom-msgbox-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ttk-custom-msgbox-0.0.2/PKG-INFO` & `ttk-custom-msgbox-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ttk-custom-msgbox
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple customizable messagebox for themed tkinter (ttk). Includes 3 built in messagebox types.
 Home-page: https://github.com/robertitoss1/ttk-custom-msgbox
 Author: Robert Salamon
 Author-email: 
 Project-URL: Bug Tracker, https://github.com/robertitoss1/ttk-custom-msgbox
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
@@ -13,15 +13,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 ## ttk-custom-msgbox
 Installation for Windows
 ```
-py -m pip install ttk-custom-msgbox==0.0.2
+py -m pip install ttk-custom-msgbox==0.0.3
 ```
 
 ## Description
 A simple customizable messagebox for themed tkinter (ttk).\
 Includes 3 built in messagebox types: \
 \
 INFO: \
```

### Comparing `ttk-custom-msgbox-0.0.2/README.md` & `ttk-custom-msgbox-0.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 ## ttk-custom-msgbox
 Installation for Windows
 ```
-py -m pip install ttk-custom-msgbox==0.0.2
+py -m pip install ttk-custom-msgbox==0.0.3
 ```
 
 ## Description
 A simple customizable messagebox for themed tkinter (ttk).\
 Includes 3 built in messagebox types: \
 \
 INFO: \
```

### Comparing `ttk-custom-msgbox-0.0.2/setup.cfg` & `ttk-custom-msgbox-0.0.3/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2074 746b 2d63 7573 746f 6d2d 6d73   = ttk-custom-ms
 00000020: 6762 6f78 0d0a 7665 7273 696f 6e20 3d20  gbox..version = 
-00000030: 302e 302e 320d 0a61 7574 686f 7220 3d20  0.0.2..author = 
+00000030: 302e 302e 330d 0a61 7574 686f 7220 3d20  0.0.3..author = 
 00000040: 526f 6265 7274 2053 616c 616d 6f6e 0d0a  Robert Salamon..
 00000050: 6175 7468 6f72 5f65 6d61 696c 203d 200d  author_email = .
 00000060: 0a64 6573 6372 6970 7469 6f6e 203d 2041  .description = A
 00000070: 2073 696d 706c 6520 6375 7374 6f6d 697a   simple customiz
 00000080: 6162 6c65 206d 6573 7361 6765 626f 7820  able messagebox 
 00000090: 666f 7220 7468 656d 6564 2074 6b69 6e74  for themed tkint
 000000a0: 6572 2028 7474 6b29 2e20 496e 636c 7564  er (ttk). Includ
```

### Comparing `ttk-custom-msgbox-0.0.2/ttk_custom_msgbox/ttk_custom_msgbox.egg-info/PKG-INFO` & `ttk-custom-msgbox-0.0.3/ttk_custom_msgbox/ttk_custom_msgbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ttk-custom-msgbox
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple customizable messagebox for themed tkinter (ttk). Includes 3 built in messagebox types.
 Home-page: https://github.com/robertitoss1/ttk-custom-msgbox
 Author: Robert Salamon
 Author-email: 
 Project-URL: Bug Tracker, https://github.com/robertitoss1/ttk-custom-msgbox
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
@@ -13,15 +13,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 ## ttk-custom-msgbox
 Installation for Windows
 ```
-py -m pip install ttk-custom-msgbox==0.0.2
+py -m pip install ttk-custom-msgbox==0.0.3
 ```
 
 ## Description
 A simple customizable messagebox for themed tkinter (ttk).\
 Includes 3 built in messagebox types: \
 \
 INFO: \
```

