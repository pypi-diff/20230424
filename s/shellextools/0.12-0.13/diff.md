# Comparing `tmp/shellextools-0.12.tar.gz` & `tmp/shellextools-0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellextools-0.12.tar", last modified: Sun Apr 23 17:54:16 2023, max compression
+gzip compressed data, was "shellextools-0.13.tar", last modified: Mon Apr 24 01:09:09 2023, max compression
```

## Comparing `shellextools-0.12.tar` & `shellextools-0.13.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 17:54:16.958320 shellextools-0.12/
--rw-rw-rw-   0        0        0     1148 2023-04-23 17:53:54.000000 shellextools-0.12/LICENSE.rst
--rw-rw-rw-   0        0        0      209 2023-04-23 17:53:50.000000 shellextools-0.12/MANIFEST.in
--rw-rw-rw-   0        0        0     3573 2023-04-23 17:54:16.958320 shellextools-0.12/PKG-INFO
--rw-rw-rw-   0        0        0     2923 2023-04-23 15:59:07.000000 shellextools-0.12/README.md
--rw-rw-rw-   0        0        0       85 2023-04-23 17:54:16.959317 shellextools-0.12/setup.cfg
--rw-rw-rw-   0        0        0     1861 2023-04-23 17:54:16.000000 shellextools-0.12/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-23 17:54:16.954330 shellextools-0.12/shellextools/
--rw-rw-rw-   0        0        0     1148 2023-04-15 00:23:59.000000 shellextools-0.12/shellextools/LICENSE
--rw-rw-rw-   0        0        0     2923 2023-04-23 15:59:07.000000 shellextools-0.12/shellextools/README.md
--rw-rw-rw-   0        0        0    48251 2023-04-23 17:14:00.000000 shellextools-0.12/shellextools/__init__.py
--rw-rw-rw-   0        0        0     2728 2023-04-23 15:59:07.000000 shellextools-0.12/shellextools/getmultifiles.py
--rw-rw-rw-   0        0        0     2555 2023-04-23 15:59:07.000000 shellextools-0.12/shellextools/loggax3.py
--rw-rw-rw-   0        0        0      248 2023-04-23 17:54:16.000000 shellextools-0.12/shellextools/requirements.txt
--rw-rw-rw-   0        0        0     9983 2023-04-23 17:54:16.000000 shellextools-0.12/shellextools/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-04-23 17:54:16.957322 shellextools-0.12/shellextools.egg-info/
--rw-rw-rw-   0        0        0     3573 2023-04-23 17:54:16.000000 shellextools-0.12/shellextools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2023-04-23 17:54:16.000000 shellextools-0.12/shellextools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 17:54:16.000000 shellextools-0.12/shellextools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      236 2023-04-23 17:54:16.000000 shellextools-0.12/shellextools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-23 17:54:16.000000 shellextools-0.12/shellextools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 01:09:09.351475 shellextools-0.13/
+-rw-rw-rw-   0        0        0     1148 2023-04-24 01:08:53.000000 shellextools-0.13/LICENSE.rst
+-rw-rw-rw-   0        0        0      209 2023-04-24 01:08:52.000000 shellextools-0.13/MANIFEST.in
+-rw-rw-rw-   0        0        0     3804 2023-04-24 01:09:09.351475 shellextools-0.13/PKG-INFO
+-rw-rw-rw-   0        0        0     3154 2023-04-24 01:07:11.000000 shellextools-0.13/README.md
+-rw-rw-rw-   0        0        0       85 2023-04-24 01:09:09.352472 shellextools-0.13/setup.cfg
+-rw-rw-rw-   0        0        0     1861 2023-04-24 01:09:06.000000 shellextools-0.13/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:09:09.344459 shellextools-0.13/shellextools/
+-rw-rw-rw-   0        0        0     1148 2023-04-15 00:23:59.000000 shellextools-0.13/shellextools/LICENSE
+-rw-rw-rw-   0        0        0     3154 2023-04-24 01:07:11.000000 shellextools-0.13/shellextools/README.md
+-rw-rw-rw-   0        0        0    50720 2023-04-24 01:03:11.000000 shellextools-0.13/shellextools/__init__.py
+-rw-rw-rw-   0        0        0     2728 2023-04-23 18:11:16.000000 shellextools-0.13/shellextools/getmultifiles.py
+-rw-rw-rw-   0        0        0     2555 2023-04-23 18:11:16.000000 shellextools-0.13/shellextools/loggax3.py
+-rw-rw-rw-   0        0        0      248 2023-04-24 01:09:06.000000 shellextools-0.13/shellextools/requirements.txt
+-rw-rw-rw-   0        0        0     9983 2023-04-24 01:09:06.000000 shellextools-0.13/shellextools/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-04-24 01:09:09.350478 shellextools-0.13/shellextools.egg-info/
+-rw-rw-rw-   0        0        0     3804 2023-04-24 01:09:08.000000 shellextools-0.13/shellextools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2023-04-24 01:09:09.000000 shellextools-0.13/shellextools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 01:09:08.000000 shellextools-0.13/shellextools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      236 2023-04-24 01:09:08.000000 shellextools-0.13/shellextools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-24 01:09:08.000000 shellextools-0.13/shellextools.egg-info/top_level.txt
```

### Comparing `shellextools-0.12/LICENSE.rst` & `shellextools-0.13/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `shellextools-0.12/PKG-INFO` & `shellextools-0.13/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shellextools
-Version: 0.12
+Version: 0.13
 Summary: Adds Python functions/methods to the Windows context menu
 Home-page: https://github.com/hansalemaos/shellextools
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: Windows context menu,python,nutika
 Classifier: Development Status :: 4 - Beta
@@ -15,15 +15,19 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
 # Adds Python functions/methods to the Windows context menu
 
 ## pip install shellextools 
 
-### Here is an example:
+### Here are 2 examples:
+
+https://github.com/hansalemaos/rc_collage
+
+[![](https://i.ytimg.com/vi/c9OouCauJ1Y/oar2.jpg?sqp=-oaymwEaCJUDENAFSFXyq4qpAwwIARUAAIhCcAHAAQY=&rs=AOn4CLBa8cG36u-xxiLEfehP5JcSw_a89g)](https://www.youtube.com/shorts/c9OouCauJ1Y)
 
 https://github.com/hansalemaos/rc_pictools
 
 [![](https://i.ytimg.com/vi/EsSrjG5vNpY/oar2.jpg?sqp=-oaymwEaCJUDENAFSFXyq4qpAwwIARUAAIhCcAHAAQY=&rs=AOn4CLDG3OahMcwdMtadJPwRe9lQvviQWA)](https://www.youtube.com/shorts/EsSrjG5vNpY)
 
 
 ## Create a pyw file
```

### Comparing `shellextools-0.12/README.md` & `shellextools-0.13/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # Adds Python functions/methods to the Windows context menu
 
 ## pip install shellextools 
 
-### Here is an example:
+### Here are 2 examples:
+
+https://github.com/hansalemaos/rc_collage
+
+[![](https://i.ytimg.com/vi/c9OouCauJ1Y/oar2.jpg?sqp=-oaymwEaCJUDENAFSFXyq4qpAwwIARUAAIhCcAHAAQY=&rs=AOn4CLBa8cG36u-xxiLEfehP5JcSw_a89g)](https://www.youtube.com/shorts/c9OouCauJ1Y)
 
 https://github.com/hansalemaos/rc_pictools
 
 [![](https://i.ytimg.com/vi/EsSrjG5vNpY/oar2.jpg?sqp=-oaymwEaCJUDENAFSFXyq4qpAwwIARUAAIhCcAHAAQY=&rs=AOn4CLDG3OahMcwdMtadJPwRe9lQvviQWA)](https://www.youtube.com/shorts/EsSrjG5vNpY)
 
 
 ## Create a pyw file
```

### Comparing `shellextools-0.12/setup.py` & `shellextools-0.13/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
 #     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.12'''
+VERSION = '''0.13'''
 DESCRIPTION = '''Adds Python functions/methods to the Windows context menu'''
 
 # Setting up
 setup(
     name="shellextools",
     version=VERSION,
     license='MIT',
```

### Comparing `shellextools-0.12/shellextools/LICENSE` & `shellextools-0.13/shellextools/LICENSE`

 * *Files identical despite different names*

### Comparing `shellextools-0.12/shellextools/README.md` & `shellextools-0.13/shellextools/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # Adds Python functions/methods to the Windows context menu
 
 ## pip install shellextools 
 
-### Here is an example:
+### Here are 2 examples:
+
+https://github.com/hansalemaos/rc_collage
+
+[![](https://i.ytimg.com/vi/c9OouCauJ1Y/oar2.jpg?sqp=-oaymwEaCJUDENAFSFXyq4qpAwwIARUAAIhCcAHAAQY=&rs=AOn4CLBa8cG36u-xxiLEfehP5JcSw_a89g)](https://www.youtube.com/shorts/c9OouCauJ1Y)
 
 https://github.com/hansalemaos/rc_pictools
 
 [![](https://i.ytimg.com/vi/EsSrjG5vNpY/oar2.jpg?sqp=-oaymwEaCJUDENAFSFXyq4qpAwwIARUAAIhCcAHAAQY=&rs=AOn4CLDG3OahMcwdMtadJPwRe9lQvviQWA)](https://www.youtube.com/shorts/EsSrjG5vNpY)
 
 
 ## Create a pyw file
```

### Comparing `shellextools-0.12/shellextools/__init__.py` & `shellextools-0.13/shellextools/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -826,14 +826,74 @@
     tsfile = os.path.normpath(os.path.join(folder, f"{prefix}{tsfile}{suffix}"))
     if create_folder:
         if not os.path.exists(tsfile):
             os.makedirs(tsfile)
     return tsfile
 
 
+
+def get_filepath(exefile:str):
+    filepath = os.path.dirname(sys.argv[0])
+    fpa=os.path.normpath(os.path.join(filepath, exefile))
+    if os.path.exists(fpa):
+        filepath=fpa
+    else:
+        filepath = os.path.dirname(__file__)
+        fpa = os.path.normpath(os.path.join(filepath, exefile))
+        if os.path.exists(fpa):
+            filepath = fpa
+
+        else:
+            filepath = os.sep.join(os.path.dirname(sys.argv[0]).split(os.sep)[:-1])
+            fpa = os.path.normpath(os.path.join(filepath, exefile))
+            if os.path.exists(fpa):
+                filepath = fpa
+            else:
+                filepath = os.sep.join(os.path.dirname(__file__).split(os.sep)[:-1])
+                fpa = os.path.normpath(os.path.join(filepath, exefile))
+                if os.path.exists(fpa):
+                    filepath = fpa
+                else:
+                    fi = sys._getframe(1)
+                    dct = fi.f_globals
+                    f = dct.get("__file__", "")
+
+                    filepathpu = os.path.dirname(f)
+                    fpa = (os.path.join(filepathpu, exefile))
+                    if os.path.exists(fpa):
+                        filepath = fpa
+                    else:
+                        fpa=os.sep.join(os.path.dirname(filepathpu).split(os.sep)[:-1])
+                        fpa = os.path.normpath(os.path.join(fpa, exefile))
+                        if os.path.exists(fpa):
+                            filepath = fpa
+                        else:
+                            filepath=exefile
+    return filepath
+
+def get_monitors_resolution():
+    user32 = ctypes.windll.user32
+    def _get_monitors_resolution():
+        monitors = []
+        monitor_enum_proc = ctypes.WINFUNCTYPE(
+            ctypes.c_int, ctypes.c_ulong, ctypes.c_ulong, ctypes.POINTER(ctypes.wintypes.RECT), ctypes.c_double)
+        def callback(hMonitor, hdcMonitor, lprcMonitor, dwData):
+            monitors.append((lprcMonitor.contents.right - lprcMonitor.contents.left,
+                             lprcMonitor.contents.bottom - lprcMonitor.contents.top))
+            return 1
+        user32.EnumDisplayMonitors(None, None, monitor_enum_proc(callback), 0)
+        return monitors
+    resolutions = _get_monitors_resolution()
+    allmonitors = {}
+    for i, res in enumerate(resolutions):
+        allmonitors[i] = {'width': res[0], 'height': res[1]}
+    return allmonitors
+
+
+
 def execute_subprocess_multiple_commands_with_timeout_bin2(
     cmd: Union[list, str],
     subcommands: Union[list, tuple, None, str] = None,
     end_of_printline: str = "",
     print_output: bool = False,
     timeout: Optional[float] = None,
     cwd: str = os.getcwd(),
```

### Comparing `shellextools-0.12/shellextools/getmultifiles.py` & `shellextools-0.13/shellextools/getmultifiles.py`

 * *Files identical despite different names*

### Comparing `shellextools-0.12/shellextools/loggax3.py` & `shellextools-0.13/shellextools/loggax3.py`

 * *Files identical despite different names*

### Comparing `shellextools-0.12/shellextools/thirdparty.json` & `shellextools-0.13/shellextools/thirdparty.json`

 * *Files identical despite different names*

### Comparing `shellextools-0.12/shellextools.egg-info/PKG-INFO` & `shellextools-0.13/shellextools.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shellextools
-Version: 0.12
+Version: 0.13
 Summary: Adds Python functions/methods to the Windows context menu
 Home-page: https://github.com/hansalemaos/shellextools
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: Windows context menu,python,nutika
 Classifier: Development Status :: 4 - Beta
@@ -15,15 +15,19 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
 # Adds Python functions/methods to the Windows context menu
 
 ## pip install shellextools 
 
-### Here is an example:
+### Here are 2 examples:
+
+https://github.com/hansalemaos/rc_collage
+
+[![](https://i.ytimg.com/vi/c9OouCauJ1Y/oar2.jpg?sqp=-oaymwEaCJUDENAFSFXyq4qpAwwIARUAAIhCcAHAAQY=&rs=AOn4CLBa8cG36u-xxiLEfehP5JcSw_a89g)](https://www.youtube.com/shorts/c9OouCauJ1Y)
 
 https://github.com/hansalemaos/rc_pictools
 
 [![](https://i.ytimg.com/vi/EsSrjG5vNpY/oar2.jpg?sqp=-oaymwEaCJUDENAFSFXyq4qpAwwIARUAAIhCcAHAAQY=&rs=AOn4CLDG3OahMcwdMtadJPwRe9lQvviQWA)](https://www.youtube.com/shorts/EsSrjG5vNpY)
 
 
 ## Create a pyw file
```

