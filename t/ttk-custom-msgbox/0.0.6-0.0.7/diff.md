# Comparing `tmp/ttk-custom-msgbox-0.0.6.tar.gz` & `tmp/ttk-custom-msgbox-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttk-custom-msgbox-0.0.6.tar", last modified: Mon Apr 24 21:23:45 2023, max compression
+gzip compressed data, was "ttk-custom-msgbox-0.0.7.tar", last modified: Mon Apr 24 21:44:20 2023, max compression
```

## Comparing `ttk-custom-msgbox-0.0.6.tar` & `ttk-custom-msgbox-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 21:23:45.535851 ttk-custom-msgbox-0.0.6/
--rw-rw-rw-   0        0        0     1090 2023-04-24 18:00:24.000000 ttk-custom-msgbox-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     4948 2023-04-24 21:23:45.536852 ttk-custom-msgbox-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     4351 2023-04-24 21:22:32.000000 ttk-custom-msgbox-0.0.6/README.md
--rw-rw-rw-   0        0        0      109 2023-04-24 19:04:53.000000 ttk-custom-msgbox-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0      772 2023-04-24 21:23:45.536852 ttk-custom-msgbox-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-24 21:23:45.518401 ttk-custom-msgbox-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-04-24 21:23:45.527401 ttk-custom-msgbox-0.0.6/src/ttk_custom_msgbox/
--rw-rw-rw-   0        0        0       81 2023-04-24 19:50:01.000000 ttk-custom-msgbox-0.0.6/src/ttk_custom_msgbox/__init__.py
--rw-rw-rw-   0        0        0     5360 2023-04-24 18:20:22.000000 ttk-custom-msgbox-0.0.6/src/ttk_custom_msgbox/custom.png
--rw-rw-rw-   0        0        0     3808 2023-04-24 18:19:54.000000 ttk-custom-msgbox-0.0.6/src/ttk_custom_msgbox/error.png
--rw-rw-rw-   0        0        0     7471 2023-04-24 18:42:08.000000 ttk-custom-msgbox-0.0.6/src/ttk_custom_msgbox/example.png
--rw-rw-rw-   0        0        0     3414 2023-04-24 18:35:19.000000 ttk-custom-msgbox-0.0.6/src/ttk_custom_msgbox/example.py
--rw-rw-rw-   0        0        0     3623 2023-04-24 18:18:48.000000 ttk-custom-msgbox-0.0.6/src/ttk_custom_msgbox/info.png
--rw-rw-rw-   0        0        0    12806 2023-04-24 18:39:34.000000 ttk-custom-msgbox-0.0.6/src/ttk_custom_msgbox/ttk_custom_msgbox.py
--rw-rw-rw-   0        0        0     3782 2023-04-24 18:19:25.000000 ttk-custom-msgbox-0.0.6/src/ttk_custom_msgbox/warning.png
-drwxrwxrwx   0        0        0        0 2023-04-24 21:23:45.535851 ttk-custom-msgbox-0.0.6/src/ttk_custom_msgbox.egg-info/
--rw-rw-rw-   0        0        0     4948 2023-04-24 21:23:45.000000 ttk-custom-msgbox-0.0.6/src/ttk_custom_msgbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      496 2023-04-24 21:23:45.000000 ttk-custom-msgbox-0.0.6/src/ttk_custom_msgbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 21:23:45.000000 ttk-custom-msgbox-0.0.6/src/ttk_custom_msgbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-04-24 21:23:45.000000 ttk-custom-msgbox-0.0.6/src/ttk_custom_msgbox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 21:44:20.847898 ttk-custom-msgbox-0.0.7/
+-rw-rw-rw-   0        0        0     1090 2023-04-24 18:00:24.000000 ttk-custom-msgbox-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     5292 2023-04-24 21:44:20.847898 ttk-custom-msgbox-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4695 2023-04-24 21:43:50.000000 ttk-custom-msgbox-0.0.7/README.md
+-rw-rw-rw-   0        0        0      109 2023-04-24 19:04:53.000000 ttk-custom-msgbox-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0      772 2023-04-24 21:44:20.848900 ttk-custom-msgbox-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-24 21:44:20.827897 ttk-custom-msgbox-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-04-24 21:44:20.838898 ttk-custom-msgbox-0.0.7/src/ttk_custom_msgbox/
+-rw-rw-rw-   0        0        0       81 2023-04-24 19:50:01.000000 ttk-custom-msgbox-0.0.7/src/ttk_custom_msgbox/__init__.py
+-rw-rw-rw-   0        0        0     5360 2023-04-24 18:20:22.000000 ttk-custom-msgbox-0.0.7/src/ttk_custom_msgbox/custom.png
+-rw-rw-rw-   0        0        0     3808 2023-04-24 18:19:54.000000 ttk-custom-msgbox-0.0.7/src/ttk_custom_msgbox/error.png
+-rw-rw-rw-   0        0        0     7471 2023-04-24 18:42:08.000000 ttk-custom-msgbox-0.0.7/src/ttk_custom_msgbox/example.png
+-rw-rw-rw-   0        0        0     3414 2023-04-24 18:35:19.000000 ttk-custom-msgbox-0.0.7/src/ttk_custom_msgbox/example.py
+-rw-rw-rw-   0        0        0     3623 2023-04-24 18:18:48.000000 ttk-custom-msgbox-0.0.7/src/ttk_custom_msgbox/info.png
+-rw-rw-rw-   0        0        0    12806 2023-04-24 18:39:34.000000 ttk-custom-msgbox-0.0.7/src/ttk_custom_msgbox/ttk_custom_msgbox.py
+-rw-rw-rw-   0        0        0     3782 2023-04-24 18:19:25.000000 ttk-custom-msgbox-0.0.7/src/ttk_custom_msgbox/warning.png
+drwxrwxrwx   0        0        0        0 2023-04-24 21:44:20.846898 ttk-custom-msgbox-0.0.7/src/ttk_custom_msgbox.egg-info/
+-rw-rw-rw-   0        0        0     5292 2023-04-24 21:44:20.000000 ttk-custom-msgbox-0.0.7/src/ttk_custom_msgbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      496 2023-04-24 21:44:20.000000 ttk-custom-msgbox-0.0.7/src/ttk_custom_msgbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 21:44:20.000000 ttk-custom-msgbox-0.0.7/src/ttk_custom_msgbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-24 21:44:20.000000 ttk-custom-msgbox-0.0.7/src/ttk_custom_msgbox.egg-info/top_level.txt
```

### Comparing `ttk-custom-msgbox-0.0.6/LICENSE` & `ttk-custom-msgbox-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ttk-custom-msgbox-0.0.6/PKG-INFO` & `ttk-custom-msgbox-0.0.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,29 @@
-Metadata-Version: 2.1
-Name: ttk-custom-msgbox
-Version: 0.0.6
-Summary: A simple customizable messagebox for themed tkinter (ttk). Includes 3 built in messagebox types.
-Home-page: https://github.com/robertitoss1/ttk-custom-msgbox
-Author: Robert Salamon
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
-py -m pip install ttk-custom-msgbox==0.0.6
+py -m pip install ttk-custom-msgbox==0.0.7
 ```
 
 ## Description
 A simple customizable messagebox for themed tkinter (ttk).\
 Includes 3 built in messagebox types: 
 
-INFO:
-
-![](src/ttk_custom_msgbox/info.png)
-
-WARNING:
+INFO: \
+![](https://github.com/robertitoss1/ttk-custom-msgbox/blob/main/src/ttk_custom_msgbox/info.png?raw=true)
 
-![](src/ttk_custom_msgbox/warning.png)
+WARNING: \
+![](https://github.com/robertitoss1/ttk-custom-msgbox/blob/main/src/ttk_custom_msgbox/warning.png?raw=true)
 
-ERROR:
+ERROR: \
+![](https://github.com/robertitoss1/ttk-custom-msgbox/blob/main/src/ttk_custom_msgbox/error.png?raw=true)
 
-![](src/ttk_custom_msgbox/error.png)
-
-CUSTOM:
-
-![](src/ttk_custom_msgbox/custom.png)
+CUSTOM: \
+![](https://github.com/robertitoss1/ttk-custom-msgbox/blob/main/src/ttk_custom_msgbox/custom.png?raw=true)
 
 Even though the INFO, WARNING and ERROR messageboxes have predefined buttons, buttons can still be customized the same way as in the example bellow for the CUSTOM message box.
 ## Usage example
 
 ```python
 from tkinter import ttk
 from ttkthemes import themed_tk
@@ -135,10 +117,9 @@
                               command=lambda: error_msg_button())
     error_button.pack(side=TOP, anchor=CENTER, pady=10)
 
     root.mainloop()
 
 ```
 
-This example will create a window with buttons to display every messagebox type:
-
-![](src/ttk_custom_msgbox/example.png)
+This example will create a window with buttons to display every messagebox type:\
+![](https://github.com/robertitoss1/ttk-custom-msgbox/blob/main/src/ttk_custom_msgbox/example.png?raw=true)
```

### Comparing `ttk-custom-msgbox-0.0.6/README.md` & `ttk-custom-msgbox-0.0.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,43 @@
+Metadata-Version: 2.1
+Name: ttk-custom-msgbox
+Version: 0.0.7
+Summary: A simple customizable messagebox for themed tkinter (ttk). Includes 3 built in messagebox types.
+Home-page: https://github.com/robertitoss1/ttk-custom-msgbox
+Author: Robert Salamon
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
-py -m pip install ttk-custom-msgbox==0.0.6
+py -m pip install ttk-custom-msgbox==0.0.7
 ```
 
 ## Description
 A simple customizable messagebox for themed tkinter (ttk).\
 Includes 3 built in messagebox types: 
 
-INFO:
-
-![](src/ttk_custom_msgbox/info.png)
-
-WARNING:
+INFO: \
+![](https://github.com/robertitoss1/ttk-custom-msgbox/blob/main/src/ttk_custom_msgbox/info.png?raw=true)
 
-![](src/ttk_custom_msgbox/warning.png)
+WARNING: \
+![](https://github.com/robertitoss1/ttk-custom-msgbox/blob/main/src/ttk_custom_msgbox/warning.png?raw=true)
 
-ERROR:
+ERROR: \
+![](https://github.com/robertitoss1/ttk-custom-msgbox/blob/main/src/ttk_custom_msgbox/error.png?raw=true)
 
-![](src/ttk_custom_msgbox/error.png)
-
-CUSTOM:
-
-![](src/ttk_custom_msgbox/custom.png)
+CUSTOM: \
+![](https://github.com/robertitoss1/ttk-custom-msgbox/blob/main/src/ttk_custom_msgbox/custom.png?raw=true)
 
 Even though the INFO, WARNING and ERROR messageboxes have predefined buttons, buttons can still be customized the same way as in the example bellow for the CUSTOM message box.
 ## Usage example
 
 ```python
 from tkinter import ttk
 from ttkthemes import themed_tk
@@ -121,10 +131,9 @@
                               command=lambda: error_msg_button())
     error_button.pack(side=TOP, anchor=CENTER, pady=10)
 
     root.mainloop()
 
 ```
 
-This example will create a window with buttons to display every messagebox type:
-
-![](src/ttk_custom_msgbox/example.png)
+This example will create a window with buttons to display every messagebox type:\
+![](https://github.com/robertitoss1/ttk-custom-msgbox/blob/main/src/ttk_custom_msgbox/example.png?raw=true)
```

### Comparing `ttk-custom-msgbox-0.0.6/setup.cfg` & `ttk-custom-msgbox-0.0.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2074 746b 2d63 7573 746f 6d2d 6d73   = ttk-custom-ms
 00000020: 6762 6f78 0d0a 7665 7273 696f 6e20 3d20  gbox..version = 
-00000030: 302e 302e 360d 0a61 7574 686f 7220 3d20  0.0.6..author = 
+00000030: 302e 302e 370d 0a61 7574 686f 7220 3d20  0.0.7..author = 
 00000040: 526f 6265 7274 2053 616c 616d 6f6e 0d0a  Robert Salamon..
 00000050: 6465 7363 7269 7074 696f 6e20 3d20 4120  description = A 
 00000060: 7369 6d70 6c65 2063 7573 746f 6d69 7a61  simple customiza
 00000070: 626c 6520 6d65 7373 6167 6562 6f78 2066  ble messagebox f
 00000080: 6f72 2074 6865 6d65 6420 746b 696e 7465  or themed tkinte
 00000090: 7220 2874 746b 292e 2049 6e63 6c75 6465  r (ttk). Include
 000000a0: 7320 3320 6275 696c 7420 696e 206d 6573  s 3 built in mes
```

### Comparing `ttk-custom-msgbox-0.0.6/src/ttk_custom_msgbox/custom.png` & `ttk-custom-msgbox-0.0.7/src/ttk_custom_msgbox/custom.png`

 * *Files identical despite different names*

### Comparing `ttk-custom-msgbox-0.0.6/src/ttk_custom_msgbox/error.png` & `ttk-custom-msgbox-0.0.7/src/ttk_custom_msgbox/error.png`

 * *Files identical despite different names*

### Comparing `ttk-custom-msgbox-0.0.6/src/ttk_custom_msgbox/example.png` & `ttk-custom-msgbox-0.0.7/src/ttk_custom_msgbox/example.png`

 * *Files identical despite different names*

### Comparing `ttk-custom-msgbox-0.0.6/src/ttk_custom_msgbox/example.py` & `ttk-custom-msgbox-0.0.7/src/ttk_custom_msgbox/example.py`

 * *Files identical despite different names*

### Comparing `ttk-custom-msgbox-0.0.6/src/ttk_custom_msgbox/info.png` & `ttk-custom-msgbox-0.0.7/src/ttk_custom_msgbox/info.png`

 * *Files identical despite different names*

### Comparing `ttk-custom-msgbox-0.0.6/src/ttk_custom_msgbox/ttk_custom_msgbox.py` & `ttk-custom-msgbox-0.0.7/src/ttk_custom_msgbox/ttk_custom_msgbox.py`

 * *Files identical despite different names*

### Comparing `ttk-custom-msgbox-0.0.6/src/ttk_custom_msgbox/warning.png` & `ttk-custom-msgbox-0.0.7/src/ttk_custom_msgbox/warning.png`

 * *Files identical despite different names*

### Comparing `ttk-custom-msgbox-0.0.6/src/ttk_custom_msgbox.egg-info/PKG-INFO` & `ttk-custom-msgbox-0.0.7/src/ttk_custom_msgbox.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ttk-custom-msgbox
-Version: 0.0.6
+Version: 0.0.7
 Summary: A simple customizable messagebox for themed tkinter (ttk). Includes 3 built in messagebox types.
 Home-page: https://github.com/robertitoss1/ttk-custom-msgbox
 Author: Robert Salamon
 Project-URL: Bug Tracker, https://github.com/robertitoss1/ttk-custom-msgbox
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
@@ -12,36 +12,32 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 ## ttk-custom-msgbox
 Installation for Windows
 ```
-py -m pip install ttk-custom-msgbox==0.0.6
+py -m pip install ttk-custom-msgbox==0.0.7
 ```
 
 ## Description
 A simple customizable messagebox for themed tkinter (ttk).\
 Includes 3 built in messagebox types: 
 
-INFO:
+INFO: \
+![](https://github.com/robertitoss1/ttk-custom-msgbox/blob/main/src/ttk_custom_msgbox/info.png?raw=true)
 
-![](src/ttk_custom_msgbox/info.png)
+WARNING: \
+![](https://github.com/robertitoss1/ttk-custom-msgbox/blob/main/src/ttk_custom_msgbox/warning.png?raw=true)
 
-WARNING:
+ERROR: \
+![](https://github.com/robertitoss1/ttk-custom-msgbox/blob/main/src/ttk_custom_msgbox/error.png?raw=true)
 
-![](src/ttk_custom_msgbox/warning.png)
-
-ERROR:
-
-![](src/ttk_custom_msgbox/error.png)
-
-CUSTOM:
-
-![](src/ttk_custom_msgbox/custom.png)
+CUSTOM: \
+![](https://github.com/robertitoss1/ttk-custom-msgbox/blob/main/src/ttk_custom_msgbox/custom.png?raw=true)
 
 Even though the INFO, WARNING and ERROR messageboxes have predefined buttons, buttons can still be customized the same way as in the example bellow for the CUSTOM message box.
 ## Usage example
 
 ```python
 from tkinter import ttk
 from ttkthemes import themed_tk
@@ -135,10 +131,9 @@
                               command=lambda: error_msg_button())
     error_button.pack(side=TOP, anchor=CENTER, pady=10)
 
     root.mainloop()
 
 ```
 
-This example will create a window with buttons to display every messagebox type:
-
-![](src/ttk_custom_msgbox/example.png)
+This example will create a window with buttons to display every messagebox type:\
+![](https://github.com/robertitoss1/ttk-custom-msgbox/blob/main/src/ttk_custom_msgbox/example.png?raw=true)
```

