# Comparing `tmp/ttk-custom-msgbox-0.0.5.tar.gz` & `tmp/ttk-custom-msgbox-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttk-custom-msgbox-0.0.5.tar", last modified: Mon Apr 24 20:30:04 2023, max compression
+gzip compressed data, was "ttk-custom-msgbox-0.0.6.tar", last modified: Mon Apr 24 21:23:45 2023, max compression
```

## Comparing `ttk-custom-msgbox-0.0.5.tar` & `ttk-custom-msgbox-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 20:30:04.278408 ttk-custom-msgbox-0.0.5/
--rw-rw-rw-   0        0        0     1090 2023-04-24 18:00:24.000000 ttk-custom-msgbox-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     5005 2023-04-24 20:30:04.279416 ttk-custom-msgbox-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     4392 2023-04-24 20:29:46.000000 ttk-custom-msgbox-0.0.5/README.md
--rw-rw-rw-   0        0        0      109 2023-04-24 19:04:53.000000 ttk-custom-msgbox-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0      817 2023-04-24 20:30:04.282414 ttk-custom-msgbox-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-24 20:30:04.252653 ttk-custom-msgbox-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-24 20:30:04.268653 ttk-custom-msgbox-0.0.5/src/ttk_custom_msgbox/
--rw-rw-rw-   0        0        0       81 2023-04-24 19:50:01.000000 ttk-custom-msgbox-0.0.5/src/ttk_custom_msgbox/__init__.py
--rw-rw-rw-   0        0        0     3414 2023-04-24 18:35:19.000000 ttk-custom-msgbox-0.0.5/src/ttk_custom_msgbox/example.py
--rw-rw-rw-   0        0        0    12806 2023-04-24 18:39:34.000000 ttk-custom-msgbox-0.0.5/src/ttk_custom_msgbox/ttk_custom_msgbox.py
-drwxrwxrwx   0        0        0        0 2023-04-24 20:30:04.278408 ttk-custom-msgbox-0.0.5/src/ttk_custom_msgbox.egg-info/
--rw-rw-rw-   0        0        0     5005 2023-04-24 20:30:04.000000 ttk-custom-msgbox-0.0.5/src/ttk_custom_msgbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2023-04-24 20:30:04.000000 ttk-custom-msgbox-0.0.5/src/ttk_custom_msgbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 20:30:04.000000 ttk-custom-msgbox-0.0.5/src/ttk_custom_msgbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-04-24 20:30:04.000000 ttk-custom-msgbox-0.0.5/src/ttk_custom_msgbox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 21:23:45.535851 ttk-custom-msgbox-0.0.6/
+-rw-rw-rw-   0        0        0     1090 2023-04-24 18:00:24.000000 ttk-custom-msgbox-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     4948 2023-04-24 21:23:45.536852 ttk-custom-msgbox-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4351 2023-04-24 21:22:32.000000 ttk-custom-msgbox-0.0.6/README.md
+-rw-rw-rw-   0        0        0      109 2023-04-24 19:04:53.000000 ttk-custom-msgbox-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0      772 2023-04-24 21:23:45.536852 ttk-custom-msgbox-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-24 21:23:45.518401 ttk-custom-msgbox-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-24 21:23:45.527401 ttk-custom-msgbox-0.0.6/src/ttk_custom_msgbox/
+-rw-rw-rw-   0        0        0       81 2023-04-24 19:50:01.000000 ttk-custom-msgbox-0.0.6/src/ttk_custom_msgbox/__init__.py
+-rw-rw-rw-   0        0        0     5360 2023-04-24 18:20:22.000000 ttk-custom-msgbox-0.0.6/src/ttk_custom_msgbox/custom.png
+-rw-rw-rw-   0        0        0     3808 2023-04-24 18:19:54.000000 ttk-custom-msgbox-0.0.6/src/ttk_custom_msgbox/error.png
+-rw-rw-rw-   0        0        0     7471 2023-04-24 18:42:08.000000 ttk-custom-msgbox-0.0.6/src/ttk_custom_msgbox/example.png
+-rw-rw-rw-   0        0        0     3414 2023-04-24 18:35:19.000000 ttk-custom-msgbox-0.0.6/src/ttk_custom_msgbox/example.py
+-rw-rw-rw-   0        0        0     3623 2023-04-24 18:18:48.000000 ttk-custom-msgbox-0.0.6/src/ttk_custom_msgbox/info.png
+-rw-rw-rw-   0        0        0    12806 2023-04-24 18:39:34.000000 ttk-custom-msgbox-0.0.6/src/ttk_custom_msgbox/ttk_custom_msgbox.py
+-rw-rw-rw-   0        0        0     3782 2023-04-24 18:19:25.000000 ttk-custom-msgbox-0.0.6/src/ttk_custom_msgbox/warning.png
+drwxrwxrwx   0        0        0        0 2023-04-24 21:23:45.535851 ttk-custom-msgbox-0.0.6/src/ttk_custom_msgbox.egg-info/
+-rw-rw-rw-   0        0        0     4948 2023-04-24 21:23:45.000000 ttk-custom-msgbox-0.0.6/src/ttk_custom_msgbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      496 2023-04-24 21:23:45.000000 ttk-custom-msgbox-0.0.6/src/ttk_custom_msgbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 21:23:45.000000 ttk-custom-msgbox-0.0.6/src/ttk_custom_msgbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-24 21:23:45.000000 ttk-custom-msgbox-0.0.6/src/ttk_custom_msgbox.egg-info/top_level.txt
```

### Comparing `ttk-custom-msgbox-0.0.5/LICENSE` & `ttk-custom-msgbox-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ttk-custom-msgbox-0.0.5/PKG-INFO` & `ttk-custom-msgbox-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 Metadata-Version: 2.1
 Name: ttk-custom-msgbox
-Version: 0.0.5
+Version: 0.0.6
 Summary: A simple customizable messagebox for themed tkinter (ttk). Includes 3 built in messagebox types.
 Home-page: https://github.com/robertitoss1/ttk-custom-msgbox
 Author: Robert Salamon
-Author-email: 
 Project-URL: Bug Tracker, https://github.com/robertitoss1/ttk-custom-msgbox
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 ## ttk-custom-msgbox
 Installation for Windows
 ```
-py -m pip install ttk-custom-msgbox==0.0.5
+py -m pip install ttk-custom-msgbox==0.0.6
 ```
 
 ## Description
 A simple customizable messagebox for themed tkinter (ttk).\
-Includes 3 built in messagebox types: \
-\
-INFO: \
-![](src/ttk_custom_msgbox/static/info.png)
-\
-WARNING: \
-![](src/ttk_custom_msgbox/static/warning.png)
-\
-ERROR: \
-![](src/ttk_custom_msgbox/static/error.png)
-\
-CUSTOM: \
-![](src/ttk_custom_msgbox/static/custom.png)
+Includes 3 built in messagebox types: 
+
+INFO:
+
+![](src/ttk_custom_msgbox/info.png)
+
+WARNING:
+
+![](src/ttk_custom_msgbox/warning.png)
+
+ERROR:
+
+![](src/ttk_custom_msgbox/error.png)
+
+CUSTOM:
+
+![](src/ttk_custom_msgbox/custom.png)
 
 Even though the INFO, WARNING and ERROR messageboxes have predefined buttons, buttons can still be customized the same way as in the example bellow for the CUSTOM message box.
 ## Usage example
 
 ```python
 from tkinter import ttk
 from ttkthemes import themed_tk
@@ -132,9 +135,10 @@
                               command=lambda: error_msg_button())
     error_button.pack(side=TOP, anchor=CENTER, pady=10)
 
     root.mainloop()
 
 ```
 
-This example will create a window with a buttons to display every messagebox type:\
-![](src/ttk_custom_msgbox/static/example.png)
+This example will create a window with buttons to display every messagebox type:
+
+![](src/ttk_custom_msgbox/example.png)
```

### Comparing `ttk-custom-msgbox-0.0.5/README.md` & `ttk-custom-msgbox-0.0.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 
 ## ttk-custom-msgbox
 Installation for Windows
 ```
-py -m pip install ttk-custom-msgbox==0.0.5
+py -m pip install ttk-custom-msgbox==0.0.6
 ```
 
 ## Description
 A simple customizable messagebox for themed tkinter (ttk).\
-Includes 3 built in messagebox types: \
-\
-INFO: \
-![](src/ttk_custom_msgbox/static/info.png)
-\
-WARNING: \
-![](src/ttk_custom_msgbox/static/warning.png)
-\
-ERROR: \
-![](src/ttk_custom_msgbox/static/error.png)
-\
-CUSTOM: \
-![](src/ttk_custom_msgbox/static/custom.png)
+Includes 3 built in messagebox types: 
+
+INFO:
+
+![](src/ttk_custom_msgbox/info.png)
+
+WARNING:
+
+![](src/ttk_custom_msgbox/warning.png)
+
+ERROR:
+
+![](src/ttk_custom_msgbox/error.png)
+
+CUSTOM:
+
+![](src/ttk_custom_msgbox/custom.png)
 
 Even though the INFO, WARNING and ERROR messageboxes have predefined buttons, buttons can still be customized the same way as in the example bellow for the CUSTOM message box.
 ## Usage example
 
 ```python
 from tkinter import ttk
 from ttkthemes import themed_tk
@@ -117,9 +121,10 @@
                               command=lambda: error_msg_button())
     error_button.pack(side=TOP, anchor=CENTER, pady=10)
 
     root.mainloop()
 
 ```
 
-This example will create a window with a buttons to display every messagebox type:\
-![](src/ttk_custom_msgbox/static/example.png)
+This example will create a window with buttons to display every messagebox type:
+
+![](src/ttk_custom_msgbox/example.png)
```

### Comparing `ttk-custom-msgbox-0.0.5/setup.cfg` & `ttk-custom-msgbox-0.0.6/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,49 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2074 746b 2d63 7573 746f 6d2d 6d73   = ttk-custom-ms
 00000020: 6762 6f78 0d0a 7665 7273 696f 6e20 3d20  gbox..version = 
-00000030: 302e 302e 350d 0a61 7574 686f 7220 3d20  0.0.5..author = 
+00000030: 302e 302e 360d 0a61 7574 686f 7220 3d20  0.0.6..author = 
 00000040: 526f 6265 7274 2053 616c 616d 6f6e 0d0a  Robert Salamon..
-00000050: 6175 7468 6f72 5f65 6d61 696c 203d 200d  author_email = .
-00000060: 0a64 6573 6372 6970 7469 6f6e 203d 2041  .description = A
-00000070: 2073 696d 706c 6520 6375 7374 6f6d 697a   simple customiz
-00000080: 6162 6c65 206d 6573 7361 6765 626f 7820  able messagebox 
-00000090: 666f 7220 7468 656d 6564 2074 6b69 6e74  for themed tkint
-000000a0: 6572 2028 7474 6b29 2e20 496e 636c 7564  er (ttk). Includ
-000000b0: 6573 2033 2062 7569 6c74 2069 6e20 6d65  es 3 built in me
-000000c0: 7373 6167 6562 6f78 2074 7970 6573 2e0d  ssagebox types..
-000000d0: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
-000000e0: 6e20 3d20 6669 6c65 3a20 5245 4144 4d45  n = file: README
-000000f0: 2e6d 640d 0a6c 6f6e 675f 6465 7363 7269  .md..long_descri
-00000100: 7074 696f 6e5f 636f 6e74 656e 745f 7479  ption_content_ty
-00000110: 7065 203d 2074 6578 742f 6d61 726b 646f  pe = text/markdo
-00000120: 776e 0d0a 7572 6c20 3d20 6874 7470 733a  wn..url = https:
-00000130: 2f2f 6769 7468 7562 2e63 6f6d 2f72 6f62  //github.com/rob
-00000140: 6572 7469 746f 7373 312f 7474 6b2d 6375  ertitoss1/ttk-cu
-00000150: 7374 6f6d 2d6d 7367 626f 780d 0a69 6e63  stom-msgbox..inc
-00000160: 6c75 6465 5f70 6163 6b61 6765 5f64 6174  lude_package_dat
-00000170: 6120 3d20 5472 7565 0d0a 7061 636b 6167  a = True..packag
-00000180: 655f 6461 7461 203d 207b 2727 3a20 5b27  e_data = {'': ['
-00000190: 7374 6174 6963 2f2a 275d 7d2c 0d0a 7072  static/*']},..pr
-000001a0: 6f6a 6563 745f 7572 6c73 203d 200d 0a09  oject_urls = ...
-000001b0: 4275 6720 5472 6163 6b65 7220 3d20 6874  Bug Tracker = ht
-000001c0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000001d0: 2f72 6f62 6572 7469 746f 7373 312f 7474  /robertitoss1/tt
-000001e0: 6b2d 6375 7374 6f6d 2d6d 7367 626f 780d  k-custom-msgbox.
-000001f0: 0a63 6c61 7373 6966 6965 7273 203d 200d  .classifiers = .
-00000200: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-00000210: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000220: 203a 3a20 332e 3130 0d0a 094c 6963 656e   :: 3.10...Licen
-00000230: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
-00000240: 6564 203a 3a20 4d49 5420 4c69 6365 6e73  ed :: MIT Licens
-00000250: 650d 0a09 4f70 6572 6174 696e 6720 5379  e...Operating Sy
-00000260: 7374 656d 203a 3a20 4d69 6372 6f73 6f66  stem :: Microsof
-00000270: 7420 3a3a 2057 696e 646f 7773 203a 3a20  t :: Windows :: 
-00000280: 5769 6e64 6f77 7320 3130 0d0a 0d0a 5b6f  Windows 10....[o
-00000290: 7074 696f 6e73 5d0d 0a70 6163 6b61 6765  ptions]..package
-000002a0: 5f64 6972 203d 200d 0a09 3d20 7372 630d  _dir = ...= src.
-000002b0: 0a70 6163 6b61 6765 7320 3d20 6669 6e64  .packages = find
-000002c0: 3a0d 0a70 7974 686f 6e5f 7265 7175 6972  :..python_requir
-000002d0: 6573 203d 203e 3d33 2e31 300d 0a0d 0a5b  es = >=3.10....[
-000002e0: 6f70 7469 6f6e 732e 7061 636b 6167 6573  options.packages
-000002f0: 2e66 696e 645d 0d0a 7768 6572 6520 3d20  .find]..where = 
-00000300: 7372 630d 0a0d 0a5b 6567 675f 696e 666f  src....[egg_info
-00000310: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
-00000320: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
-00000330: 0a                                       .
+00000050: 6465 7363 7269 7074 696f 6e20 3d20 4120  description = A 
+00000060: 7369 6d70 6c65 2063 7573 746f 6d69 7a61  simple customiza
+00000070: 626c 6520 6d65 7373 6167 6562 6f78 2066  ble messagebox f
+00000080: 6f72 2074 6865 6d65 6420 746b 696e 7465  or themed tkinte
+00000090: 7220 2874 746b 292e 2049 6e63 6c75 6465  r (ttk). Include
+000000a0: 7320 3320 6275 696c 7420 696e 206d 6573  s 3 built in mes
+000000b0: 7361 6765 626f 7820 7479 7065 732e 0d0a  sagebox types...
+000000c0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
+000000d0: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
+000000e0: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
+000000f0: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
+00000100: 6520 3d20 7465 7874 2f6d 6172 6b64 6f77  e = text/markdow
+00000110: 6e0d 0a75 726c 203d 2068 7474 7073 3a2f  n..url = https:/
+00000120: 2f67 6974 6875 622e 636f 6d2f 726f 6265  /github.com/robe
+00000130: 7274 6974 6f73 7331 2f74 746b 2d63 7573  rtitoss1/ttk-cus
+00000140: 746f 6d2d 6d73 6762 6f78 0d0a 7072 6f6a  tom-msgbox..proj
+00000150: 6563 745f 7572 6c73 203d 200d 0a09 4275  ect_urls = ...Bu
+00000160: 6720 5472 6163 6b65 7220 3d20 6874 7470  g Tracker = http
+00000170: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f72  s://github.com/r
+00000180: 6f62 6572 7469 746f 7373 312f 7474 6b2d  obertitoss1/ttk-
+00000190: 6375 7374 6f6d 2d6d 7367 626f 780d 0a63  custom-msgbox..c
+000001a0: 6c61 7373 6966 6965 7273 203d 200d 0a09  lassifiers = ...
+000001b0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000001c0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+000001d0: 3a20 332e 3130 0d0a 094c 6963 656e 7365  : 3.10...License
+000001e0: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
+000001f0: 203a 3a20 4d49 5420 4c69 6365 6e73 650d   :: MIT License.
+00000200: 0a09 4f70 6572 6174 696e 6720 5379 7374  ..Operating Syst
+00000210: 656d 203a 3a20 4d69 6372 6f73 6f66 7420  em :: Microsoft 
+00000220: 3a3a 2057 696e 646f 7773 203a 3a20 5769  :: Windows :: Wi
+00000230: 6e64 6f77 7320 3130 0d0a 0d0a 5b6f 7074  ndows 10....[opt
+00000240: 696f 6e73 5d0d 0a70 6163 6b61 6765 5f64  ions]..package_d
+00000250: 6972 203d 200d 0a09 3d20 7372 630d 0a70  ir = ...= src..p
+00000260: 6163 6b61 6765 7320 3d20 6669 6e64 3a0d  ackages = find:.
+00000270: 0a70 7974 686f 6e5f 7265 7175 6972 6573  .python_requires
+00000280: 203d 203e 3d33 2e31 300d 0a0d 0a5b 6f70   = >=3.10....[op
+00000290: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
+000002a0: 696e 645d 0d0a 7768 6572 6520 3d20 7372  ind]..where = sr
+000002b0: 630d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  c....[options.pa
+000002c0: 636b 6167 655f 6461 7461 5d0d 0a2a 203d  ckage_data]..* =
+000002d0: 202a 2e70 6e67 0d0a 0d0a 5b65 6767 5f69   *.png....[egg_i
+000002e0: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
+000002f0: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
+00000300: 0d0a 0d0a                                ....
```

### Comparing `ttk-custom-msgbox-0.0.5/src/ttk_custom_msgbox/example.py` & `ttk-custom-msgbox-0.0.6/src/ttk_custom_msgbox/example.py`

 * *Files identical despite different names*

### Comparing `ttk-custom-msgbox-0.0.5/src/ttk_custom_msgbox/ttk_custom_msgbox.py` & `ttk-custom-msgbox-0.0.6/src/ttk_custom_msgbox/ttk_custom_msgbox.py`

 * *Files identical despite different names*

### Comparing `ttk-custom-msgbox-0.0.5/src/ttk_custom_msgbox.egg-info/PKG-INFO` & `ttk-custom-msgbox-0.0.6/src/ttk_custom_msgbox.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 Metadata-Version: 2.1
 Name: ttk-custom-msgbox
-Version: 0.0.5
+Version: 0.0.6
 Summary: A simple customizable messagebox for themed tkinter (ttk). Includes 3 built in messagebox types.
 Home-page: https://github.com/robertitoss1/ttk-custom-msgbox
 Author: Robert Salamon
-Author-email: 
 Project-URL: Bug Tracker, https://github.com/robertitoss1/ttk-custom-msgbox
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 ## ttk-custom-msgbox
 Installation for Windows
 ```
-py -m pip install ttk-custom-msgbox==0.0.5
+py -m pip install ttk-custom-msgbox==0.0.6
 ```
 
 ## Description
 A simple customizable messagebox for themed tkinter (ttk).\
-Includes 3 built in messagebox types: \
-\
-INFO: \
-![](src/ttk_custom_msgbox/static/info.png)
-\
-WARNING: \
-![](src/ttk_custom_msgbox/static/warning.png)
-\
-ERROR: \
-![](src/ttk_custom_msgbox/static/error.png)
-\
-CUSTOM: \
-![](src/ttk_custom_msgbox/static/custom.png)
+Includes 3 built in messagebox types: 
+
+INFO:
+
+![](src/ttk_custom_msgbox/info.png)
+
+WARNING:
+
+![](src/ttk_custom_msgbox/warning.png)
+
+ERROR:
+
+![](src/ttk_custom_msgbox/error.png)
+
+CUSTOM:
+
+![](src/ttk_custom_msgbox/custom.png)
 
 Even though the INFO, WARNING and ERROR messageboxes have predefined buttons, buttons can still be customized the same way as in the example bellow for the CUSTOM message box.
 ## Usage example
 
 ```python
 from tkinter import ttk
 from ttkthemes import themed_tk
@@ -132,9 +135,10 @@
                               command=lambda: error_msg_button())
     error_button.pack(side=TOP, anchor=CENTER, pady=10)
 
     root.mainloop()
 
 ```
 
-This example will create a window with a buttons to display every messagebox type:\
-![](src/ttk_custom_msgbox/static/example.png)
+This example will create a window with buttons to display every messagebox type:
+
+![](src/ttk_custom_msgbox/example.png)
```

