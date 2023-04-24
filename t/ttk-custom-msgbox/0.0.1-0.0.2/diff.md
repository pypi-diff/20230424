# Comparing `tmp/ttk-custom-msgbox-0.0.1.tar.gz` & `tmp/ttk-custom-msgbox-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttk-custom-msgbox-0.0.1.tar", last modified: Mon Apr 24 19:09:42 2023, max compression
+gzip compressed data, was "ttk-custom-msgbox-0.0.2.tar", last modified: Mon Apr 24 19:26:05 2023, max compression
```

## Comparing `ttk-custom-msgbox-0.0.1.tar` & `ttk-custom-msgbox-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 19:09:42.599940 ttk-custom-msgbox-0.0.1/
--rw-rw-rw-   0        0        0     1090 2023-04-24 18:00:24.000000 ttk-custom-msgbox-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     4922 2023-04-24 19:09:42.599940 ttk-custom-msgbox-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4309 2023-04-24 18:53:33.000000 ttk-custom-msgbox-0.0.1/README.md
--rw-rw-rw-   0        0        0      109 2023-04-24 19:04:53.000000 ttk-custom-msgbox-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      780 2023-04-24 19:09:42.602949 ttk-custom-msgbox-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-24 19:09:42.589358 ttk-custom-msgbox-0.0.1/ttk-custom-msgbox/
-drwxrwxrwx   0        0        0        0 2023-04-24 19:09:42.599940 ttk-custom-msgbox-0.0.1/ttk-custom-msgbox/ttk_custom_msgbox.egg-info/
--rw-rw-rw-   0        0        0     4922 2023-04-24 19:09:42.000000 ttk-custom-msgbox-0.0.1/ttk-custom-msgbox/ttk_custom_msgbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-04-24 19:09:42.000000 ttk-custom-msgbox-0.0.1/ttk-custom-msgbox/ttk_custom_msgbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 19:09:42.000000 ttk-custom-msgbox-0.0.1/ttk-custom-msgbox/ttk_custom_msgbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 19:09:42.000000 ttk-custom-msgbox-0.0.1/ttk-custom-msgbox/ttk_custom_msgbox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 19:26:05.493014 ttk-custom-msgbox-0.0.2/
+-rw-rw-rw-   0        0        0     1090 2023-04-24 18:00:24.000000 ttk-custom-msgbox-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     4922 2023-04-24 19:26:05.493014 ttk-custom-msgbox-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4309 2023-04-24 19:25:59.000000 ttk-custom-msgbox-0.0.2/README.md
+-rw-rw-rw-   0        0        0      109 2023-04-24 19:04:53.000000 ttk-custom-msgbox-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      791 2023-04-24 19:26:05.494014 ttk-custom-msgbox-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-24 19:26:05.481013 ttk-custom-msgbox-0.0.2/ttk_custom_msgbox/
+drwxrwxrwx   0        0        0        0 2023-04-24 19:26:05.492015 ttk-custom-msgbox-0.0.2/ttk_custom_msgbox/ttk_custom_msgbox.egg-info/
+-rw-rw-rw-   0        0        0     4922 2023-04-24 19:26:05.000000 ttk-custom-msgbox-0.0.2/ttk_custom_msgbox/ttk_custom_msgbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2023-04-24 19:26:05.000000 ttk-custom-msgbox-0.0.2/ttk_custom_msgbox/ttk_custom_msgbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 19:26:05.000000 ttk-custom-msgbox-0.0.2/ttk_custom_msgbox/ttk_custom_msgbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 19:26:05.000000 ttk-custom-msgbox-0.0.2/ttk_custom_msgbox/ttk_custom_msgbox.egg-info/top_level.txt
```

### Comparing `ttk-custom-msgbox-0.0.1/LICENSE` & `ttk-custom-msgbox-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ttk-custom-msgbox-0.0.1/PKG-INFO` & `ttk-custom-msgbox-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ttk-custom-msgbox
-Version: 0.0.1
+Version: 0.0.2
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
-py -m pip install ttk-custom-msgbox==0.0.1
+py -m pip install ttk-custom-msgbox==0.0.2
 ```
 
 ## Description
 A simple customizable messagebox for themed tkinter (ttk).\
 Includes 3 built in messagebox types: \
 \
 INFO: \
```

### Comparing `ttk-custom-msgbox-0.0.1/README.md` & `ttk-custom-msgbox-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 ## ttk-custom-msgbox
 Installation for Windows
 ```
-py -m pip install ttk-custom-msgbox==0.0.1
+py -m pip install ttk-custom-msgbox==0.0.2
 ```
 
 ## Description
 A simple customizable messagebox for themed tkinter (ttk).\
 Includes 3 built in messagebox types: \
 \
 INFO: \
```

### Comparing `ttk-custom-msgbox-0.0.1/setup.cfg` & `ttk-custom-msgbox-0.0.2/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2074 746b 2d63 7573 746f 6d2d 6d73   = ttk-custom-ms
 00000020: 6762 6f78 0d0a 7665 7273 696f 6e20 3d20  gbox..version = 
-00000030: 302e 302e 310d 0a61 7574 686f 7220 3d20  0.0.1..author = 
+00000030: 302e 302e 320d 0a61 7574 686f 7220 3d20  0.0.2..author = 
 00000040: 526f 6265 7274 2053 616c 616d 6f6e 0d0a  Robert Salamon..
 00000050: 6175 7468 6f72 5f65 6d61 696c 203d 200d  author_email = .
 00000060: 0a64 6573 6372 6970 7469 6f6e 203d 2041  .description = A
 00000070: 2073 696d 706c 6520 6375 7374 6f6d 697a   simple customiz
 00000080: 6162 6c65 206d 6573 7361 6765 626f 7820  able messagebox 
 00000090: 666f 7220 7468 656d 6564 2074 6b69 6e74  for themed tkint
 000000a0: 6572 2028 7474 6b29 2e20 496e 636c 7564  er (ttk). Includ
@@ -32,18 +32,19 @@
 000001f0: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
 00000200: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
 00000210: 0d0a 094f 7065 7261 7469 6e67 2053 7973  ...Operating Sys
 00000220: 7465 6d20 3a3a 204d 6963 726f 736f 6674  tem :: Microsoft
 00000230: 203a 3a20 5769 6e64 6f77 7320 3a3a 2057   :: Windows :: W
 00000240: 696e 646f 7773 2031 300d 0a0d 0a5b 6f70  indows 10....[op
 00000250: 7469 6f6e 735d 0d0a 7061 636b 6167 655f  tions]..package_
-00000260: 6469 7220 3d20 0d0a 093d 2074 746b 2d63  dir = ...= ttk-c
-00000270: 7573 746f 6d2d 6d73 6762 6f78 0d0a 7061  ustom-msgbox..pa
+00000260: 6469 7220 3d20 0d0a 093d 2074 746b 5f63  dir = ...= ttk_c
+00000270: 7573 746f 6d5f 6d73 6762 6f78 0d0a 7061  ustom_msgbox..pa
 00000280: 636b 6167 6573 203d 2066 696e 643a 0d0a  ckages = find:..
 00000290: 7079 7468 6f6e 5f72 6571 7569 7265 7320  python_requires 
 000002a0: 3d20 3e3d 332e 3130 0d0a 0d0a 5b6f 7074  = >=3.10....[opt
 000002b0: 696f 6e73 2e70 6163 6b61 6765 732e 6669  ions.packages.fi
 000002c0: 6e64 5d0d 0a77 6865 7265 203d 2074 746b  nd]..where = ttk
-000002d0: 2d63 7573 746f 6d2d 6d73 6762 6f78 0d0a  -custom-msgbox..
-000002e0: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
-000002f0: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
-00000300: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
+000002d0: 2d74 746b 5f63 7573 746f 6d5f 6d73 6762  -ttk_custom_msgb
+000002e0: 6f78 2d6d 7367 626f 780d 0a0d 0a5b 6567  ox-msgbox....[eg
+000002f0: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
+00000300: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
+00000310: 3d20 300d 0a0d 0a                        = 0....
```

### Comparing `ttk-custom-msgbox-0.0.1/ttk-custom-msgbox/ttk_custom_msgbox.egg-info/PKG-INFO` & `ttk-custom-msgbox-0.0.2/ttk_custom_msgbox/ttk_custom_msgbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ttk-custom-msgbox
-Version: 0.0.1
+Version: 0.0.2
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
-py -m pip install ttk-custom-msgbox==0.0.1
+py -m pip install ttk-custom-msgbox==0.0.2
 ```
 
 ## Description
 A simple customizable messagebox for themed tkinter (ttk).\
 Includes 3 built in messagebox types: \
 \
 INFO: \
```

