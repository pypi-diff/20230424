# Comparing `tmp/qt_command_palette-0.0.6.tar.gz` & `tmp/qt_command_palette-0.0.7.tar.gz`

## Comparing `qt_command_palette-0.0.6.tar` & `qt_command_palette-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/codecov.yml
--rw-r--r--   0        0        0   201915 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/example.gif
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/launch.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/setup.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/qt_command_palette/__about__.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/qt_command_palette/__init__.py
--rw-r--r--   0        0        0    10047 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/qt_command_palette/_api.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/qt_command_palette/_commands.py
--rw-r--r--   0        0        0     7516 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/qt_command_palette/_list.py
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/qt_command_palette/_storage.py
--rw-r--r--   0        0        0     4559 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/qt_command_palette/_widget.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/tests/_file_0.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/tests/_file_1.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/tests/test_register.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/tests/test_storage.py
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/.gitignore
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/LICENSE.txt
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/README.md
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3410 2020-02-02 00:00:00.000000 qt_command_palette-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/codecov.yml
+-rw-r--r--   0        0        0   201915 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/example.gif
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/launch.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/setup.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/qt_command_palette/__about__.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/qt_command_palette/__init__.py
+-rw-r--r--   0        0        0    10047 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/qt_command_palette/_api.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/qt_command_palette/_commands.py
+-rw-r--r--   0        0        0     7516 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/qt_command_palette/_list.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/qt_command_palette/_storage.py
+-rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/qt_command_palette/_widget.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/tests/__init__.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/tests/_file_0.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/tests/_file_1.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/tests/test_register.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/tests/test_storage.py
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/LICENSE.txt
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/README.md
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3410 2020-02-02 00:00:00.000000 qt_command_palette-0.0.7/PKG-INFO
```

### Comparing `qt_command_palette-0.0.6/.pre-commit-config.yaml` & `qt_command_palette-0.0.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `qt_command_palette-0.0.6/example.gif` & `qt_command_palette-0.0.7/example.gif`

 * *Files identical despite different names*

### Comparing `qt_command_palette-0.0.6/launch.py` & `qt_command_palette-0.0.7/launch.py`

 * *Files identical despite different names*

### Comparing `qt_command_palette-0.0.6/qt_command_palette/_api.py` & `qt_command_palette-0.0.7/qt_command_palette/_api.py`

 * *Files identical despite different names*

### Comparing `qt_command_palette-0.0.6/qt_command_palette/_commands.py` & `qt_command_palette-0.0.7/qt_command_palette/_commands.py`

 * *Files identical despite different names*

### Comparing `qt_command_palette-0.0.6/qt_command_palette/_list.py` & `qt_command_palette-0.0.7/qt_command_palette/_list.py`

 * *Files identical despite different names*

### Comparing `qt_command_palette-0.0.6/qt_command_palette/_storage.py` & `qt_command_palette-0.0.7/qt_command_palette/_storage.py`

 * *Files identical despite different names*

### Comparing `qt_command_palette-0.0.6/qt_command_palette/_widget.py` & `qt_command_palette-0.0.7/qt_command_palette/_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,18 @@
         """Show command palette widget in the center of the screen."""
         self._line.setText("")
         self._list.update_for_text("")
         self.setWindowFlags(Qt.WindowType.Dialog | Qt.WindowType.FramelessWindowHint)
         super().show()
 
         screen_rect = QtGui.QGuiApplication.primaryScreen().geometry()
-        self.resize(screen_rect.width() * 0.5, screen_rect.height() * 0.5)
+        self.resize(
+            int(screen_rect.width() * 0.5),
+            int(screen_rect.height() * 0.5),
+        )
         point = screen_rect.center() - self.rect().center()
         self.move(point)
 
         self.raise_()
         self._line.setFocus()
         return None
```

### Comparing `qt_command_palette-0.0.6/tests/test_register.py` & `qt_command_palette-0.0.7/tests/test_register.py`

 * *Files identical despite different names*

### Comparing `qt_command_palette-0.0.6/tests/test_storage.py` & `qt_command_palette-0.0.7/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `qt_command_palette-0.0.6/.gitignore` & `qt_command_palette-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `qt_command_palette-0.0.6/LICENSE.txt` & `qt_command_palette-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qt_command_palette-0.0.6/README.md` & `qt_command_palette-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `qt_command_palette-0.0.6/pyproject.toml` & `qt_command_palette-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qt_command_palette-0.0.6/PKG-INFO` & `qt_command_palette-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qt-command-palette
-Version: 0.0.6
+Version: 0.0.7
 Summary: A command palette widget for Qt applications
 Project-URL: Documentation, https://github.com/unknown/qt-command-palette#readme
 Project-URL: Issues, https://github.com/unknown/qt-command-palette/issues
 Project-URL: Source, https://github.com/unknown/qt-command-palette
 Author-email: Hanjin Liu <hanjin.liu@bs.s.u-tokyo.ac.jp>
 License: MIT License
```

