# Comparing `tmp/PLAN-Tools-0.6.tar.gz` & `tmp/PLAN-Tools-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PLAN-Tools-0.6.tar", last modified: Mon Apr 24 14:35:36 2023, max compression
+gzip compressed data, was "PLAN-Tools-0.7.tar", last modified: Mon Apr 24 16:04:37 2023, max compression
```

## Comparing `PLAN-Tools-0.6.tar` & `PLAN-Tools-0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 14:35:36.290247 PLAN-Tools-0.6/
--rw-r--r--   0 runner    (1001) docker     (122)     8845 2023-04-24 14:35:36.290247 PLAN-Tools-0.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 14:35:36.290247 PLAN-Tools-0.6/PLAN_Tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8845 2023-04-24 14:35:36.000000 PLAN-Tools-0.6/PLAN_Tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      371 2023-04-24 14:35:36.000000 PLAN-Tools-0.6/PLAN_Tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-24 14:35:36.000000 PLAN-Tools-0.6/PLAN_Tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-04-24 14:35:36.000000 PLAN-Tools-0.6/PLAN_Tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-24 14:35:36.000000 PLAN-Tools-0.6/PLAN_Tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     7637 2023-04-24 14:35:24.000000 PLAN-Tools-0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 14:35:36.290247 PLAN-Tools-0.6/plan_tools/
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-04-24 14:35:24.000000 PLAN-Tools-0.6/plan_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13199 2023-04-24 14:35:24.000000 PLAN-Tools-0.6/plan_tools/entry_point.py
--rw-r--r--   0 runner    (1001) docker     (122)     1761 2023-04-24 14:35:24.000000 PLAN-Tools-0.6/plan_tools/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 14:35:36.290247 PLAN-Tools-0.6/plan_tools/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 14:35:24.000000 PLAN-Tools-0.6/plan_tools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1487 2023-04-24 14:35:24.000000 PLAN-Tools-0.6/plan_tools/tests/test_entry_point.py
--rw-r--r--   0 runner    (1001) docker     (122)      415 2023-04-24 14:35:24.000000 PLAN-Tools-0.6/plan_tools/tests/test_runtime.py
--rw-r--r--   0 runner    (1001) docker     (122)      170 2023-04-24 14:35:36.290247 PLAN-Tools-0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-04-24 14:35:24.000000 PLAN-Tools-0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 16:04:37.748157 PLAN-Tools-0.7/
+-rw-r--r--   0 runner    (1001) docker     (122)     8845 2023-04-24 16:04:37.748157 PLAN-Tools-0.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 16:04:37.748157 PLAN-Tools-0.7/PLAN_Tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8845 2023-04-24 16:04:37.000000 PLAN-Tools-0.7/PLAN_Tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      371 2023-04-24 16:04:37.000000 PLAN-Tools-0.7/PLAN_Tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-24 16:04:37.000000 PLAN-Tools-0.7/PLAN_Tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-04-24 16:04:37.000000 PLAN-Tools-0.7/PLAN_Tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-24 16:04:37.000000 PLAN-Tools-0.7/PLAN_Tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     7637 2023-04-24 16:04:24.000000 PLAN-Tools-0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 16:04:37.748157 PLAN-Tools-0.7/plan_tools/
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-04-24 16:04:24.000000 PLAN-Tools-0.7/plan_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13308 2023-04-24 16:04:24.000000 PLAN-Tools-0.7/plan_tools/entry_point.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1761 2023-04-24 16:04:24.000000 PLAN-Tools-0.7/plan_tools/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 16:04:37.748157 PLAN-Tools-0.7/plan_tools/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 16:04:24.000000 PLAN-Tools-0.7/plan_tools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1751 2023-04-24 16:04:24.000000 PLAN-Tools-0.7/plan_tools/tests/test_entry_point.py
+-rw-r--r--   0 runner    (1001) docker     (122)      415 2023-04-24 16:04:24.000000 PLAN-Tools-0.7/plan_tools/tests/test_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (122)      170 2023-04-24 16:04:37.748157 PLAN-Tools-0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-04-24 16:04:24.000000 PLAN-Tools-0.7/setup.py
```

### Comparing `PLAN-Tools-0.6/PKG-INFO` & `PLAN-Tools-0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PLAN-Tools
-Version: 0.6
+Version: 0.7
 Summary: A set of tools to help with Pip Links And Nonsense
 Home-page: https://github.com/Myoldmopar/PlanTools
 Author: Edwin Lee, for NREL, for United States Department of Energy
 License: ModifiedBSD
 Description: # PLAN-TOOLS
         
         [![Flake8](https://github.com/Myoldmopar/PLAN-Tools/actions/workflows/flake8.yml/badge.svg)](https://github.com/Myoldmopar/PLAN-Tools/actions/workflows/flake8.yml)
```

### Comparing `PLAN-Tools-0.6/PLAN_Tools.egg-info/PKG-INFO` & `PLAN-Tools-0.7/PLAN_Tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PLAN-Tools
-Version: 0.6
+Version: 0.7
 Summary: A set of tools to help with Pip Links And Nonsense
 Home-page: https://github.com/Myoldmopar/PlanTools
 Author: Edwin Lee, for NREL, for United States Department of Energy
 License: ModifiedBSD
 Description: # PLAN-TOOLS
         
         [![Flake8](https://github.com/Myoldmopar/PLAN-Tools/actions/workflows/flake8.yml/badge.svg)](https://github.com/Myoldmopar/PLAN-Tools/actions/workflows/flake8.yml)
```

### Comparing `PLAN-Tools-0.6/README.md` & `PLAN-Tools-0.7/README.md`

 * *Files identical despite different names*

### Comparing `PLAN-Tools-0.6/plan_tools/entry_point.py` & `PLAN-Tools-0.7/plan_tools/entry_point.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,23 +78,23 @@
         target_exe = scripts_dir / self.installed_binary_name
         icon_file = self.get_package_icon_for_link()
         desktop_file = self.get_path_to_link_file()
         self.write_desktop_file(desktop_file, target_exe, scripts_dir, icon_file)
         return 0
 
     def write_desktop_file(self, desktop_file: Path, target_exe: Path, scripts_dir: Path, icon_file: Path):
-        icon_file_string: str = str(icon_file) if icon_file.exists() else ''
         if system() == 'Windows':
+            def escape_path(path_: Path) -> str:
+                return str(path_).replace('\\', '/')
+
+            icon_file_string: str = escape_path(icon_file) if icon_file.exists() else ''
             self.desktop_file_data_check = {'exe': target_exe, 'cwd': scripts_dir, 'icon': icon_file_string}
             if self.test_mode:
                 return
             else:  # pragma: no cover
-                def escape_path(path_: Path) -> str:
-                    return str(path_).replace('\\', '/')
-
                 shortcut_path = escape_path(desktop_file)
                 target = escape_path(target_exe)
                 working_dir = escape_path(scripts_dir)
                 js_content = f'''var sh = WScript.CreateObject("WScript.Shell");
 var shortcut = sh.CreateShortcut("{shortcut_path}");
 shortcut.TargetPath = "{target}";
 shortcut.WorkingDirectory = "{working_dir}";
@@ -108,15 +108,15 @@
                 finally:
                     unlink(script_path)
         elif system() == 'Linux':
             desktop_file_contents = f"""[Desktop Entry]
 Name={self.pretty_link_name}
 Comment={self.description}
 Exec={target_exe}
-Icon={icon_file_string}
+Icon={str(icon_file) if icon_file.exists() else ''}
 Type=Application
 Path={scripts_dir}
 Terminal=false
 StartupWMClass={self.wm_class}"""
             self.desktop_file_data_check = {'contents': desktop_file_contents}
             if self.test_mode:
                 return
@@ -201,30 +201,31 @@
             user_scripts_dir = Path(get_path('scripts'))
             global_scripts_dir = Path(USER_BASE) / 'bin'
         else:  # assuming 'Darwin'
             user_scripts_dir = Path(USER_BASE) / 'bin'
             global_scripts_dir = Path(get_path('scripts'))
         user_exe = user_scripts_dir / self.installed_binary_name
         global_exe = global_scripts_dir / self.installed_binary_name
-        if user_exe.exists() and global_exe.exists():
+        if user_exe.exists() and global_exe.exists():  # pragma: no cover
+            # I'm going to allow this to be uncovered because it will be awkward to get this set up properly
             print(f"Detected the {self.installed_binary_name} binary in both user and global locations.")
             print("Due to this ambiguity, I cannot figure out to which one I should link.")
             print(f"User install location: {user_exe}")
             print(f"Global install location: {global_exe}")
             print("I am going to assume the user directory!!")
             return user_scripts_dir
         elif user_exe.exists():
             return user_scripts_dir
         elif global_exe.exists():
             return global_scripts_dir
         else:
-            print(f"Could not find {self.installed_binary_name} binary at either user or global location.")
-            print("This is weird since you are running this script...did you actually pip install this tool?")
-            print("Make sure to pip install the tool and then retry")
-            raise Exception("Could not find executable at user or global location")
+            msg = f"Could not find {self.installed_binary_name} binary at either user or global location."
+            msg += "This is weird since you are running this script...did you actually pip install this tool?"
+            msg += "Make sure to pip install the tool and then retry"
+            raise Exception(msg)
 
     def get_package_icon_for_link(self):
         if system() == 'Windows':
             return self.package_root / 'icons' / 'icon.ico'  # I think png might work here as well
         elif system() == 'Linux':
             return self.package_root / 'icons' / 'icon.png'
         else:  # assuming 'Darwin'
```

### Comparing `PLAN-Tools-0.6/plan_tools/runtime.py` & `PLAN-Tools-0.7/plan_tools/runtime.py`

 * *Files identical despite different names*

### Comparing `PLAN-Tools-0.6/plan_tools/tests/test_entry_point.py` & `PLAN-Tools-0.7/plan_tools/tests/test_entry_point.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from unittest import TestCase
 
 from plan_tools.entry_point import EntryPoint
 
 
 class TestEntryPoint(TestCase):
 
-    def test_entry_point(self):
+    def test_entry_point_success(self):
         # it will be difficult to test the resulting paths on CI
         # we can at least test that it is returning good types
         # for now I'm going to try to test it with pip... :)
         e = EntryPoint("pip", "pip", "Setup Tools", "Descriptive", "wm-class", test_mode=True)
         e.run()
         found_exe_dir = e.get_pip_entry_point_exe_dir()
         self.assertIsInstance(found_exe_dir, Path)
@@ -26,7 +26,12 @@
             self.assertIn('contents_dir', e.desktop_file_data_check)
             self.assertIn('mac_os_dir', e.desktop_file_data_check)
             self.assertIn('resource_dir', e.desktop_file_data_check)
             self.assertIn('exe', e.desktop_file_data_check)
             self.assertIn('icon', e.desktop_file_data_check)
             self.assertIn('plist_path', e.desktop_file_data_check)
             self.assertIn('plist_contents', e.desktop_file_data_check)
+
+    def test_entry_point_cannot_find_binary(self):
+        e = EntryPoint("does not matter", "does not exist!", "Nice Name", "Descriptive", "wm-class", test_mode=True)
+        with self.assertRaises(Exception):
+            e.get_pip_entry_point_exe_dir()
```

### Comparing `PLAN-Tools-0.6/setup.py` & `PLAN-Tools-0.7/setup.py`

 * *Files identical despite different names*

