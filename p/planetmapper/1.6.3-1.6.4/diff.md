# Comparing `tmp/planetmapper-1.6.3.tar.gz` & `tmp/planetmapper-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planetmapper-1.6.3.tar", last modified: Fri Apr 21 10:33:40 2023, max compression
+gzip compressed data, was "planetmapper-1.6.4.tar", last modified: Mon Apr 24 16:24:57 2023, max compression
```

## Comparing `planetmapper-1.6.3.tar` & `planetmapper-1.6.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:33:40.125534 planetmapper-1.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-21 10:33:40.125534 planetmapper-1.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-21 10:33:26.000000 planetmapper-1.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:33:40.121534 planetmapper-1.6.3/planetmapper/
--rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-04-21 10:33:26.000000 planetmapper-1.6.3/planetmapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13940 2023-04-21 10:33:26.000000 planetmapper-1.6.3/planetmapper/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-21 10:33:26.000000 planetmapper-1.6.3/planetmapper/basic_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    72134 2023-04-21 10:33:26.000000 planetmapper-1.6.3/planetmapper/body.py
--rw-r--r--   0 runner    (1001) docker     (123)    99198 2023-04-21 10:33:26.000000 planetmapper-1.6.3/planetmapper/body_xy.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-21 10:33:26.000000 planetmapper-1.6.3/planetmapper/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:33:40.125534 planetmapper-1.6.3/planetmapper/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-04-21 10:33:26.000000 planetmapper-1.6.3/planetmapper/data/rings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-21 10:33:26.000000 planetmapper-1.6.3/planetmapper/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)   114930 2023-04-21 10:33:26.000000 planetmapper-1.6.3/planetmapper/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-04-21 10:33:26.000000 planetmapper-1.6.3/planetmapper/kernel_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    43334 2023-04-21 10:33:26.000000 planetmapper-1.6.3/planetmapper/observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7855 2023-04-21 10:33:26.000000 planetmapper-1.6.3/planetmapper/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)    13008 2023-04-21 10:33:26.000000 planetmapper-1.6.3/planetmapper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:33:40.125534 planetmapper-1.6.3/planetmapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-21 10:33:40.000000 planetmapper-1.6.3/planetmapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-21 10:33:40.000000 planetmapper-1.6.3/planetmapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 10:33:40.000000 planetmapper-1.6.3/planetmapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-21 10:33:40.000000 planetmapper-1.6.3/planetmapper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-21 10:33:40.000000 planetmapper-1.6.3/planetmapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-21 10:33:40.000000 planetmapper-1.6.3/planetmapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-21 10:33:26.000000 planetmapper-1.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 10:33:40.125534 planetmapper-1.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-21 10:33:26.000000 planetmapper-1.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:33:40.125534 planetmapper-1.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10773 2023-04-21 10:33:26.000000 planetmapper-1.6.3/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-21 10:33:26.000000 planetmapper-1.6.3/tests/test_basic_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    20532 2023-04-21 10:33:26.000000 planetmapper-1.6.3/tests/test_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    25253 2023-04-21 10:33:26.000000 planetmapper-1.6.3/tests/test_body_xy.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-21 10:33:26.000000 planetmapper-1.6.3/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-21 10:33:26.000000 planetmapper-1.6.3/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-21 10:33:26.000000 planetmapper-1.6.3/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)    17684 2023-04-21 10:33:26.000000 planetmapper-1.6.3/tests/test_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-04-21 10:33:26.000000 planetmapper-1.6.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:24:57.092701 planetmapper-1.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-24 16:24:57.092701 planetmapper-1.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-24 16:24:45.000000 planetmapper-1.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:24:57.088701 planetmapper-1.6.4/planetmapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-04-24 16:24:45.000000 planetmapper-1.6.4/planetmapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13940 2023-04-24 16:24:45.000000 planetmapper-1.6.4/planetmapper/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-24 16:24:45.000000 planetmapper-1.6.4/planetmapper/basic_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72134 2023-04-24 16:24:45.000000 planetmapper-1.6.4/planetmapper/body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99198 2023-04-24 16:24:45.000000 planetmapper-1.6.4/planetmapper/body_xy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-24 16:24:45.000000 planetmapper-1.6.4/planetmapper/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:24:57.088701 planetmapper-1.6.4/planetmapper/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-04-24 16:24:45.000000 planetmapper-1.6.4/planetmapper/data/rings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-24 16:24:45.000000 planetmapper-1.6.4/planetmapper/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)   116142 2023-04-24 16:24:45.000000 planetmapper-1.6.4/planetmapper/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-04-24 16:24:45.000000 planetmapper-1.6.4/planetmapper/kernel_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43334 2023-04-24 16:24:45.000000 planetmapper-1.6.4/planetmapper/observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7855 2023-04-24 16:24:45.000000 planetmapper-1.6.4/planetmapper/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13008 2023-04-24 16:24:45.000000 planetmapper-1.6.4/planetmapper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:24:57.088701 planetmapper-1.6.4/planetmapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-24 16:24:57.000000 planetmapper-1.6.4/planetmapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-24 16:24:57.000000 planetmapper-1.6.4/planetmapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 16:24:57.000000 planetmapper-1.6.4/planetmapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-24 16:24:57.000000 planetmapper-1.6.4/planetmapper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-24 16:24:57.000000 planetmapper-1.6.4/planetmapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-24 16:24:57.000000 planetmapper-1.6.4/planetmapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-24 16:24:45.000000 planetmapper-1.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 16:24:57.092701 planetmapper-1.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-24 16:24:45.000000 planetmapper-1.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:24:57.092701 planetmapper-1.6.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10773 2023-04-24 16:24:45.000000 planetmapper-1.6.4/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-24 16:24:45.000000 planetmapper-1.6.4/tests/test_basic_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20532 2023-04-24 16:24:45.000000 planetmapper-1.6.4/tests/test_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25253 2023-04-24 16:24:45.000000 planetmapper-1.6.4/tests/test_body_xy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-24 16:24:45.000000 planetmapper-1.6.4/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-24 16:24:45.000000 planetmapper-1.6.4/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-24 16:24:45.000000 planetmapper-1.6.4/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17684 2023-04-24 16:24:45.000000 planetmapper-1.6.4/tests/test_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-04-24 16:24:45.000000 planetmapper-1.6.4/tests/test_utils.py
```

### Comparing `planetmapper-1.6.3/PKG-INFO` & `planetmapper-1.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planetmapper
-Version: 1.6.3
+Version: 1.6.4
 Summary: A Python module for visualising, navigating and mapping Solar System observations
 Home-page: https://github.com/ortk95/planetmapper
 Download-URL: https://pypi.org/project/planetmapper/
 Author: Oliver King
 Author-email: oliver.king95@gmail.com
 Project-URL: Documentation, https://planetmapper.readthedocs.io/
 Project-URL: GitHub, https://github.com/ortk95/planetmapper
```

### Comparing `planetmapper-1.6.3/README.md` & `planetmapper-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.3/planetmapper/__init__.py` & `planetmapper-1.6.4/planetmapper/__init__.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.3/planetmapper/base.py` & `planetmapper-1.6.4/planetmapper/base.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.3/planetmapper/basic_body.py` & `planetmapper-1.6.4/planetmapper/basic_body.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.3/planetmapper/body.py` & `planetmapper-1.6.4/planetmapper/body.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.3/planetmapper/body_xy.py` & `planetmapper-1.6.4/planetmapper/body_xy.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.3/planetmapper/data/rings.json` & `planetmapper-1.6.4/planetmapper/data/rings.json`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.3/planetmapper/data_loader.py` & `planetmapper-1.6.4/planetmapper/data_loader.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.3/planetmapper/gui.py` & `planetmapper-1.6.4/planetmapper/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,17 +91,45 @@
 
 MAP_INTERPOLATIONS = ('nearest', 'linear', 'quadratic', 'cubic')
 MAP_PROJECTIONS = ('rectangular', 'orthographic', 'azimuthal')
 
 DEFAULT_HINT = ''
 
 
+# Deal with X11 font bug by replacing high codepoint chars with ASCII equivalents.
+# This seems to prevent the use of fonts which cause the X_OpenFont error which
+# XQuartz was producing when trying to run planetmapper over SSH on mac. This is a bit
+# of a hack and produces an uglier UI, but is better than always crashing.
+# TODO remove this when the bug is fixed in XQuartz
+# https://github.com/ortk95/planetmapper/issues/145
+try:
+    USE_X11_FONT_BUGFIX = bool(os.environ['PLANETMAPPER_USE_X11_FONT_BUGFIX'])
+except KeyError:
+    USE_X11_FONT_BUGFIX = False
+X11_FONT_BUGRIX_TRANSLATIONS = str.maketrans(
+    {
+        '↖': None,
+        '↑': '^',
+        '↗': None,
+        '←': '<',
+        '→': '>',
+        '↙': None,
+        '↓': 'v',
+        '↘': None,
+        '↺': '<',
+        '↻': '>',
+    }
+)
+
+
 def _main(*args):
     """Called with `planetmapper` from the command line"""
     print(f'Launching PlanetMapper {common.__version__}')
+    if USE_X11_FONT_BUGFIX:
+        print('Using X11 font bugfix')
     gui = GUI()
     if args:
         gui.set_observation(Observation(args[0]))
     gui.run()
 
 
 class Quit(Exception):
@@ -496,14 +524,15 @@
     ) -> None:
         label_frame = ttk.LabelFrame(frame, text=label)
         label_frame.pack(fill='x', pady=3, ipadx=1, ipady=1)
 
         button_frame = ttk.Frame(label_frame)
         button_frame.pack()
         for arrow, hint, fn, column, row in buttons:
+            arrow = self.maybe_replace_string_with_x11_bugfix(arrow)
             self.add_tooltip(
                 ttk.Button(button_frame, text=arrow, command=fn, width=1),
                 button_tooltip_base.format(hint=hint),
                 fn,
             ).grid(column=column, row=row, ipadx=ipadx, ipady=ipady, padx=2, pady=2)
 
         entry_frame = self.add_tooltip(ttk.Frame(label_frame), entry_tooltip)
@@ -1360,14 +1389,20 @@
             # hide value error message when trying to go r0<0
             pass
 
     # File IO
     def save_button(self) -> None:
         SaveObservation(self)
 
+    def maybe_replace_string_with_x11_bugfix(self, s: str) -> str:
+        # X11 font bug https://github.com/ortk95/planetmapper/issues/145
+        if USE_X11_FONT_BUGFIX:
+            s = s.translate(X11_FONT_BUGRIX_TRANSLATIONS)
+        return s
+
 
 class Popup:
     def get_int(
         self,
         string_variable: tk.StringVar | str,
         name: str,
         positive: bool = True,
```

### Comparing `planetmapper-1.6.3/planetmapper/kernel_downloader.py` & `planetmapper-1.6.4/planetmapper/kernel_downloader.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.3/planetmapper/observation.py` & `planetmapper-1.6.4/planetmapper/observation.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.3/planetmapper/progress.py` & `planetmapper-1.6.4/planetmapper/progress.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.3/planetmapper/utils.py` & `planetmapper-1.6.4/planetmapper/utils.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.3/planetmapper.egg-info/PKG-INFO` & `planetmapper-1.6.4/planetmapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planetmapper
-Version: 1.6.3
+Version: 1.6.4
 Summary: A Python module for visualising, navigating and mapping Solar System observations
 Home-page: https://github.com/ortk95/planetmapper
 Download-URL: https://pypi.org/project/planetmapper/
 Author: Oliver King
 Author-email: oliver.king95@gmail.com
 Project-URL: Documentation, https://planetmapper.readthedocs.io/
 Project-URL: GitHub, https://github.com/ortk95/planetmapper
```

### Comparing `planetmapper-1.6.3/planetmapper.egg-info/SOURCES.txt` & `planetmapper-1.6.4/planetmapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.3/setup.py` & `planetmapper-1.6.4/setup.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.3/tests/test_base.py` & `planetmapper-1.6.4/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.3/tests/test_basic_body.py` & `planetmapper-1.6.4/tests/test_basic_body.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.3/tests/test_body.py` & `planetmapper-1.6.4/tests/test_body.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.3/tests/test_body_xy.py` & `planetmapper-1.6.4/tests/test_body_xy.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.3/tests/test_init.py` & `planetmapper-1.6.4/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.3/tests/test_observation.py` & `planetmapper-1.6.4/tests/test_observation.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.3/tests/test_utils.py` & `planetmapper-1.6.4/tests/test_utils.py`

 * *Files identical despite different names*

