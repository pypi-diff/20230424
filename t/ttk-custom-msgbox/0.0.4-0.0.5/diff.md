# Comparing `tmp/ttk-custom-msgbox-0.0.4.tar.gz` & `tmp/ttk-custom-msgbox-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttk-custom-msgbox-0.0.4.tar", last modified: Mon Apr 24 19:50:26 2023, max compression
+gzip compressed data, was "ttk-custom-msgbox-0.0.5.tar", last modified: Mon Apr 24 20:30:04 2023, max compression
```

## Comparing `ttk-custom-msgbox-0.0.4.tar` & `ttk-custom-msgbox-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 19:50:26.337316 ttk-custom-msgbox-0.0.4/
--rw-rw-rw-   0        0        0     1090 2023-04-24 18:00:24.000000 ttk-custom-msgbox-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     4922 2023-04-24 19:50:26.337316 ttk-custom-msgbox-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     4309 2023-04-24 19:50:14.000000 ttk-custom-msgbox-0.0.4/README.md
--rw-rw-rw-   0        0        0      109 2023-04-24 19:04:53.000000 ttk-custom-msgbox-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      791 2023-04-24 19:50:26.338314 ttk-custom-msgbox-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-24 19:50:26.326255 ttk-custom-msgbox-0.0.4/ttk_custom_msgbox/
-drwxrwxrwx   0        0        0        0 2023-04-24 19:50:26.337316 ttk-custom-msgbox-0.0.4/ttk_custom_msgbox/ttk_custom_msgbox.egg-info/
--rw-rw-rw-   0        0        0     4922 2023-04-24 19:50:26.000000 ttk-custom-msgbox-0.0.4/ttk_custom_msgbox/ttk_custom_msgbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-04-24 19:50:26.000000 ttk-custom-msgbox-0.0.4/ttk_custom_msgbox/ttk_custom_msgbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 19:50:26.000000 ttk-custom-msgbox-0.0.4/ttk_custom_msgbox/ttk_custom_msgbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 19:50:26.000000 ttk-custom-msgbox-0.0.4/ttk_custom_msgbox/ttk_custom_msgbox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 20:30:04.278408 ttk-custom-msgbox-0.0.5/
+-rw-rw-rw-   0        0        0     1090 2023-04-24 18:00:24.000000 ttk-custom-msgbox-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     5005 2023-04-24 20:30:04.279416 ttk-custom-msgbox-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4392 2023-04-24 20:29:46.000000 ttk-custom-msgbox-0.0.5/README.md
+-rw-rw-rw-   0        0        0      109 2023-04-24 19:04:53.000000 ttk-custom-msgbox-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0      817 2023-04-24 20:30:04.282414 ttk-custom-msgbox-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-24 20:30:04.252653 ttk-custom-msgbox-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-24 20:30:04.268653 ttk-custom-msgbox-0.0.5/src/ttk_custom_msgbox/
+-rw-rw-rw-   0        0        0       81 2023-04-24 19:50:01.000000 ttk-custom-msgbox-0.0.5/src/ttk_custom_msgbox/__init__.py
+-rw-rw-rw-   0        0        0     3414 2023-04-24 18:35:19.000000 ttk-custom-msgbox-0.0.5/src/ttk_custom_msgbox/example.py
+-rw-rw-rw-   0        0        0    12806 2023-04-24 18:39:34.000000 ttk-custom-msgbox-0.0.5/src/ttk_custom_msgbox/ttk_custom_msgbox.py
+drwxrwxrwx   0        0        0        0 2023-04-24 20:30:04.278408 ttk-custom-msgbox-0.0.5/src/ttk_custom_msgbox.egg-info/
+-rw-rw-rw-   0        0        0     5005 2023-04-24 20:30:04.000000 ttk-custom-msgbox-0.0.5/src/ttk_custom_msgbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2023-04-24 20:30:04.000000 ttk-custom-msgbox-0.0.5/src/ttk_custom_msgbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 20:30:04.000000 ttk-custom-msgbox-0.0.5/src/ttk_custom_msgbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-24 20:30:04.000000 ttk-custom-msgbox-0.0.5/src/ttk_custom_msgbox.egg-info/top_level.txt
```

### Comparing `ttk-custom-msgbox-0.0.4/LICENSE` & `ttk-custom-msgbox-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ttk-custom-msgbox-0.0.4/PKG-INFO` & `ttk-custom-msgbox-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ttk-custom-msgbox
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple customizable messagebox for themed tkinter (ttk). Includes 3 built in messagebox types.
 Home-page: https://github.com/robertitoss1/ttk-custom-msgbox
 Author: Robert Salamon
 Author-email: 
 Project-URL: Bug Tracker, https://github.com/robertitoss1/ttk-custom-msgbox
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
@@ -13,40 +13,41 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 ## ttk-custom-msgbox
 Installation for Windows
 ```
-py -m pip install ttk-custom-msgbox==0.0.4
+py -m pip install ttk-custom-msgbox==0.0.5
 ```
 
 ## Description
 A simple customizable messagebox for themed tkinter (ttk).\
 Includes 3 built in messagebox types: \
 \
 INFO: \
-![](msgbox_images/info.png)
+![](src/ttk_custom_msgbox/static/info.png)
 \
 WARNING: \
-![](msgbox_images/warning.png)
+![](src/ttk_custom_msgbox/static/warning.png)
 \
 ERROR: \
-![](msgbox_images/error.png)
+![](src/ttk_custom_msgbox/static/error.png)
 \
 CUSTOM: \
-![](msgbox_images/custom.png)
+![](src/ttk_custom_msgbox/static/custom.png)
 
 Even though the INFO, WARNING and ERROR messageboxes have predefined buttons, buttons can still be customized the same way as in the example bellow for the CUSTOM message box.
 ## Usage example
+
 ```python
 from tkinter import ttk
 from ttkthemes import themed_tk
 from tkinter import *
-from ttk_custom_msgbox import ThemedTkMsgBox
+from src.ttk_custom_msgbox import ThemedTkMsgBox
 
 # Example
 if __name__ == "__main__":
     # Change theme here:
     root = themed_tk.ThemedTk(theme="black")
 
     # Root window geometry
@@ -66,14 +67,15 @@
     master_frame.pack(fill="both", expand=True)
 
     # Be sure to set the master of the ThemedTkMsgBox as the root window which is
     # an instance of themed_tk.ThemedTk and NOT the main frame or else the message box
     # will not be properly centered to the main window.
     msgbox = ThemedTkMsgBox(master=root, wait_response=True)
 
+
     # function that shows msgbox when button is clicked.
     def custom_msg_button():
         # Define variable to store message
         message = "You can customize:\n" \
                   "- Title\n" \
                   "- Message\n" \
                   "- Buttons"
@@ -131,8 +133,8 @@
     error_button.pack(side=TOP, anchor=CENTER, pady=10)
 
     root.mainloop()
 
 ```
 
 This example will create a window with a buttons to display every messagebox type:\
-![](msgbox_images/example.png)
+![](src/ttk_custom_msgbox/static/example.png)
```

### Comparing `ttk-custom-msgbox-0.0.4/README.md` & `ttk-custom-msgbox-0.0.5/src/ttk_custom_msgbox.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,53 @@
+Metadata-Version: 2.1
+Name: ttk-custom-msgbox
+Version: 0.0.5
+Summary: A simple customizable messagebox for themed tkinter (ttk). Includes 3 built in messagebox types.
+Home-page: https://github.com/robertitoss1/ttk-custom-msgbox
+Author: Robert Salamon
+Author-email: 
+Project-URL: Bug Tracker, https://github.com/robertitoss1/ttk-custom-msgbox
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 
 ## ttk-custom-msgbox
 Installation for Windows
 ```
-py -m pip install ttk-custom-msgbox==0.0.4
+py -m pip install ttk-custom-msgbox==0.0.5
 ```
 
 ## Description
 A simple customizable messagebox for themed tkinter (ttk).\
 Includes 3 built in messagebox types: \
 \
 INFO: \
-![](msgbox_images/info.png)
+![](src/ttk_custom_msgbox/static/info.png)
 \
 WARNING: \
-![](msgbox_images/warning.png)
+![](src/ttk_custom_msgbox/static/warning.png)
 \
 ERROR: \
-![](msgbox_images/error.png)
+![](src/ttk_custom_msgbox/static/error.png)
 \
 CUSTOM: \
-![](msgbox_images/custom.png)
+![](src/ttk_custom_msgbox/static/custom.png)
 
 Even though the INFO, WARNING and ERROR messageboxes have predefined buttons, buttons can still be customized the same way as in the example bellow for the CUSTOM message box.
 ## Usage example
+
 ```python
 from tkinter import ttk
 from ttkthemes import themed_tk
 from tkinter import *
-from ttk_custom_msgbox import ThemedTkMsgBox
+from src.ttk_custom_msgbox import ThemedTkMsgBox
 
 # Example
 if __name__ == "__main__":
     # Change theme here:
     root = themed_tk.ThemedTk(theme="black")
 
     # Root window geometry
@@ -51,14 +67,15 @@
     master_frame.pack(fill="both", expand=True)
 
     # Be sure to set the master of the ThemedTkMsgBox as the root window which is
     # an instance of themed_tk.ThemedTk and NOT the main frame or else the message box
     # will not be properly centered to the main window.
     msgbox = ThemedTkMsgBox(master=root, wait_response=True)
 
+
     # function that shows msgbox when button is clicked.
     def custom_msg_button():
         # Define variable to store message
         message = "You can customize:\n" \
                   "- Title\n" \
                   "- Message\n" \
                   "- Buttons"
@@ -116,8 +133,8 @@
     error_button.pack(side=TOP, anchor=CENTER, pady=10)
 
     root.mainloop()
 
 ```
 
 This example will create a window with a buttons to display every messagebox type:\
-![](msgbox_images/example.png)
+![](src/ttk_custom_msgbox/static/example.png)
```

### Comparing `ttk-custom-msgbox-0.0.4/setup.cfg` & `ttk-custom-msgbox-0.0.5/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2074 746b 2d63 7573 746f 6d2d 6d73   = ttk-custom-ms
 00000020: 6762 6f78 0d0a 7665 7273 696f 6e20 3d20  gbox..version = 
-00000030: 302e 302e 340d 0a61 7574 686f 7220 3d20  0.0.4..author = 
+00000030: 302e 302e 350d 0a61 7574 686f 7220 3d20  0.0.5..author = 
 00000040: 526f 6265 7274 2053 616c 616d 6f6e 0d0a  Robert Salamon..
 00000050: 6175 7468 6f72 5f65 6d61 696c 203d 200d  author_email = .
 00000060: 0a64 6573 6372 6970 7469 6f6e 203d 2041  .description = A
 00000070: 2073 696d 706c 6520 6375 7374 6f6d 697a   simple customiz
 00000080: 6162 6c65 206d 6573 7361 6765 626f 7820  able messagebox 
 00000090: 666f 7220 7468 656d 6564 2074 6b69 6e74  for themed tkint
 000000a0: 6572 2028 7474 6b29 2e20 496e 636c 7564  er (ttk). Includ
@@ -15,36 +15,38 @@
 000000e0: 6e20 3d20 6669 6c65 3a20 5245 4144 4d45  n = file: README
 000000f0: 2e6d 640d 0a6c 6f6e 675f 6465 7363 7269  .md..long_descri
 00000100: 7074 696f 6e5f 636f 6e74 656e 745f 7479  ption_content_ty
 00000110: 7065 203d 2074 6578 742f 6d61 726b 646f  pe = text/markdo
 00000120: 776e 0d0a 7572 6c20 3d20 6874 7470 733a  wn..url = https:
 00000130: 2f2f 6769 7468 7562 2e63 6f6d 2f72 6f62  //github.com/rob
 00000140: 6572 7469 746f 7373 312f 7474 6b2d 6375  ertitoss1/ttk-cu
-00000150: 7374 6f6d 2d6d 7367 626f 780d 0a70 726f  stom-msgbox..pro
-00000160: 6a65 6374 5f75 726c 7320 3d20 0d0a 0942  ject_urls = ...B
-00000170: 7567 2054 7261 636b 6572 203d 2068 7474  ug Tracker = htt
-00000180: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000190: 726f 6265 7274 6974 6f73 7331 2f74 746b  robertitoss1/ttk
-000001a0: 2d63 7573 746f 6d2d 6d73 6762 6f78 0d0a  -custom-msgbox..
-000001b0: 636c 6173 7369 6669 6572 7320 3d20 0d0a  classifiers = ..
-000001c0: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
-000001d0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-000001e0: 3a3a 2033 2e31 300d 0a09 4c69 6365 6e73  :: 3.10...Licens
-000001f0: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
-00000200: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
-00000210: 0d0a 094f 7065 7261 7469 6e67 2053 7973  ...Operating Sys
-00000220: 7465 6d20 3a3a 204d 6963 726f 736f 6674  tem :: Microsoft
-00000230: 203a 3a20 5769 6e64 6f77 7320 3a3a 2057   :: Windows :: W
-00000240: 696e 646f 7773 2031 300d 0a0d 0a5b 6f70  indows 10....[op
-00000250: 7469 6f6e 735d 0d0a 7061 636b 6167 655f  tions]..package_
-00000260: 6469 7220 3d20 0d0a 093d 2074 746b 5f63  dir = ...= ttk_c
-00000270: 7573 746f 6d5f 6d73 6762 6f78 0d0a 7061  ustom_msgbox..pa
-00000280: 636b 6167 6573 203d 2066 696e 643a 0d0a  ckages = find:..
-00000290: 7079 7468 6f6e 5f72 6571 7569 7265 7320  python_requires 
-000002a0: 3d20 3e3d 332e 3130 0d0a 0d0a 5b6f 7074  = >=3.10....[opt
-000002b0: 696f 6e73 2e70 6163 6b61 6765 732e 6669  ions.packages.fi
-000002c0: 6e64 5d0d 0a77 6865 7265 203d 2074 746b  nd]..where = ttk
-000002d0: 2d74 746b 5f63 7573 746f 6d5f 6d73 6762  -ttk_custom_msgb
-000002e0: 6f78 2d6d 7367 626f 780d 0a0d 0a5b 6567  ox-msgbox....[eg
-000002f0: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
-00000300: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
-00000310: 3d20 300d 0a0d 0a                        = 0....
+00000150: 7374 6f6d 2d6d 7367 626f 780d 0a69 6e63  stom-msgbox..inc
+00000160: 6c75 6465 5f70 6163 6b61 6765 5f64 6174  lude_package_dat
+00000170: 6120 3d20 5472 7565 0d0a 7061 636b 6167  a = True..packag
+00000180: 655f 6461 7461 203d 207b 2727 3a20 5b27  e_data = {'': ['
+00000190: 7374 6174 6963 2f2a 275d 7d2c 0d0a 7072  static/*']},..pr
+000001a0: 6f6a 6563 745f 7572 6c73 203d 200d 0a09  oject_urls = ...
+000001b0: 4275 6720 5472 6163 6b65 7220 3d20 6874  Bug Tracker = ht
+000001c0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000001d0: 2f72 6f62 6572 7469 746f 7373 312f 7474  /robertitoss1/tt
+000001e0: 6b2d 6375 7374 6f6d 2d6d 7367 626f 780d  k-custom-msgbox.
+000001f0: 0a63 6c61 7373 6966 6965 7273 203d 200d  .classifiers = .
+00000200: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+00000210: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000220: 203a 3a20 332e 3130 0d0a 094c 6963 656e   :: 3.10...Licen
+00000230: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
+00000240: 6564 203a 3a20 4d49 5420 4c69 6365 6e73  ed :: MIT Licens
+00000250: 650d 0a09 4f70 6572 6174 696e 6720 5379  e...Operating Sy
+00000260: 7374 656d 203a 3a20 4d69 6372 6f73 6f66  stem :: Microsof
+00000270: 7420 3a3a 2057 696e 646f 7773 203a 3a20  t :: Windows :: 
+00000280: 5769 6e64 6f77 7320 3130 0d0a 0d0a 5b6f  Windows 10....[o
+00000290: 7074 696f 6e73 5d0d 0a70 6163 6b61 6765  ptions]..package
+000002a0: 5f64 6972 203d 200d 0a09 3d20 7372 630d  _dir = ...= src.
+000002b0: 0a70 6163 6b61 6765 7320 3d20 6669 6e64  .packages = find
+000002c0: 3a0d 0a70 7974 686f 6e5f 7265 7175 6972  :..python_requir
+000002d0: 6573 203d 203e 3d33 2e31 300d 0a0d 0a5b  es = >=3.10....[
+000002e0: 6f70 7469 6f6e 732e 7061 636b 6167 6573  options.packages
+000002f0: 2e66 696e 645d 0d0a 7768 6572 6520 3d20  .find]..where = 
+00000300: 7372 630d 0a0d 0a5b 6567 675f 696e 666f  src....[egg_info
+00000310: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
+00000320: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
+00000330: 0a                                       .
```

### Comparing `ttk-custom-msgbox-0.0.4/ttk_custom_msgbox/ttk_custom_msgbox.egg-info/PKG-INFO` & `ttk-custom-msgbox-0.0.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,38 @@
-Metadata-Version: 2.1
-Name: ttk-custom-msgbox
-Version: 0.0.4
-Summary: A simple customizable messagebox for themed tkinter (ttk). Includes 3 built in messagebox types.
-Home-page: https://github.com/robertitoss1/ttk-custom-msgbox
-Author: Robert Salamon
-Author-email: 
-Project-URL: Bug Tracker, https://github.com/robertitoss1/ttk-custom-msgbox
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows :: Windows 10
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 
 ## ttk-custom-msgbox
 Installation for Windows
 ```
-py -m pip install ttk-custom-msgbox==0.0.4
+py -m pip install ttk-custom-msgbox==0.0.5
 ```
 
 ## Description
 A simple customizable messagebox for themed tkinter (ttk).\
 Includes 3 built in messagebox types: \
 \
 INFO: \
-![](msgbox_images/info.png)
+![](src/ttk_custom_msgbox/static/info.png)
 \
 WARNING: \
-![](msgbox_images/warning.png)
+![](src/ttk_custom_msgbox/static/warning.png)
 \
 ERROR: \
-![](msgbox_images/error.png)
+![](src/ttk_custom_msgbox/static/error.png)
 \
 CUSTOM: \
-![](msgbox_images/custom.png)
+![](src/ttk_custom_msgbox/static/custom.png)
 
 Even though the INFO, WARNING and ERROR messageboxes have predefined buttons, buttons can still be customized the same way as in the example bellow for the CUSTOM message box.
 ## Usage example
+
 ```python
 from tkinter import ttk
 from ttkthemes import themed_tk
 from tkinter import *
-from ttk_custom_msgbox import ThemedTkMsgBox
+from src.ttk_custom_msgbox import ThemedTkMsgBox
 
 # Example
 if __name__ == "__main__":
     # Change theme here:
     root = themed_tk.ThemedTk(theme="black")
 
     # Root window geometry
@@ -66,14 +52,15 @@
     master_frame.pack(fill="both", expand=True)
 
     # Be sure to set the master of the ThemedTkMsgBox as the root window which is
     # an instance of themed_tk.ThemedTk and NOT the main frame or else the message box
     # will not be properly centered to the main window.
     msgbox = ThemedTkMsgBox(master=root, wait_response=True)
 
+
     # function that shows msgbox when button is clicked.
     def custom_msg_button():
         # Define variable to store message
         message = "You can customize:\n" \
                   "- Title\n" \
                   "- Message\n" \
                   "- Buttons"
@@ -131,8 +118,8 @@
     error_button.pack(side=TOP, anchor=CENTER, pady=10)
 
     root.mainloop()
 
 ```
 
 This example will create a window with a buttons to display every messagebox type:\
-![](msgbox_images/example.png)
+![](src/ttk_custom_msgbox/static/example.png)
```

