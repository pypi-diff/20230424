# Comparing `tmp/PLAN-Tools-0.5.tar.gz` & `tmp/PLAN-Tools-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PLAN-Tools-0.5.tar", last modified: Thu Apr  6 18:08:05 2023, max compression
+gzip compressed data, was "PLAN-Tools-0.6.tar", last modified: Mon Apr 24 14:35:36 2023, max compression
```

## Comparing `PLAN-Tools-0.5.tar` & `PLAN-Tools-0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 18:08:05.370363 PLAN-Tools-0.5/
--rw-r--r--   0 runner    (1001) docker     (122)     8806 2023-04-06 18:08:05.370363 PLAN-Tools-0.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 18:08:05.370363 PLAN-Tools-0.5/PLAN_Tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8806 2023-04-06 18:08:05.000000 PLAN-Tools-0.5/PLAN_Tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      371 2023-04-06 18:08:05.000000 PLAN-Tools-0.5/PLAN_Tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-06 18:08:05.000000 PLAN-Tools-0.5/PLAN_Tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-04-06 18:08:05.000000 PLAN-Tools-0.5/PLAN_Tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-06 18:08:05.000000 PLAN-Tools-0.5/PLAN_Tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     7637 2023-04-06 18:07:53.000000 PLAN-Tools-0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 18:08:05.370363 PLAN-Tools-0.5/plan_tools/
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-04-06 18:07:53.000000 PLAN-Tools-0.5/plan_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12720 2023-04-06 18:07:53.000000 PLAN-Tools-0.5/plan_tools/entry_point.py
--rw-r--r--   0 runner    (1001) docker     (122)     1761 2023-04-06 18:07:53.000000 PLAN-Tools-0.5/plan_tools/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 18:08:05.370363 PLAN-Tools-0.5/plan_tools/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-06 18:07:53.000000 PLAN-Tools-0.5/plan_tools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1487 2023-04-06 18:07:53.000000 PLAN-Tools-0.5/plan_tools/tests/test_entry_point.py
--rw-r--r--   0 runner    (1001) docker     (122)      415 2023-04-06 18:07:53.000000 PLAN-Tools-0.5/plan_tools/tests/test_runtime.py
--rw-r--r--   0 runner    (1001) docker     (122)      170 2023-04-06 18:08:05.374363 PLAN-Tools-0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1134 2023-04-06 18:07:53.000000 PLAN-Tools-0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 14:35:36.290247 PLAN-Tools-0.6/
+-rw-r--r--   0 runner    (1001) docker     (122)     8845 2023-04-24 14:35:36.290247 PLAN-Tools-0.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 14:35:36.290247 PLAN-Tools-0.6/PLAN_Tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8845 2023-04-24 14:35:36.000000 PLAN-Tools-0.6/PLAN_Tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      371 2023-04-24 14:35:36.000000 PLAN-Tools-0.6/PLAN_Tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-24 14:35:36.000000 PLAN-Tools-0.6/PLAN_Tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-04-24 14:35:36.000000 PLAN-Tools-0.6/PLAN_Tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-24 14:35:36.000000 PLAN-Tools-0.6/PLAN_Tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     7637 2023-04-24 14:35:24.000000 PLAN-Tools-0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 14:35:36.290247 PLAN-Tools-0.6/plan_tools/
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-04-24 14:35:24.000000 PLAN-Tools-0.6/plan_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13199 2023-04-24 14:35:24.000000 PLAN-Tools-0.6/plan_tools/entry_point.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1761 2023-04-24 14:35:24.000000 PLAN-Tools-0.6/plan_tools/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 14:35:36.290247 PLAN-Tools-0.6/plan_tools/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-24 14:35:24.000000 PLAN-Tools-0.6/plan_tools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1487 2023-04-24 14:35:24.000000 PLAN-Tools-0.6/plan_tools/tests/test_entry_point.py
+-rw-r--r--   0 runner    (1001) docker     (122)      415 2023-04-24 14:35:24.000000 PLAN-Tools-0.6/plan_tools/tests/test_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (122)      170 2023-04-24 14:35:36.290247 PLAN-Tools-0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-04-24 14:35:24.000000 PLAN-Tools-0.6/setup.py
```

### Comparing `PLAN-Tools-0.5/PKG-INFO` & `PLAN-Tools-0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: PLAN-Tools
-Version: 0.5
+Version: 0.6
 Summary: A set of tools to help with Pip Links And Nonsense
 Home-page: https://github.com/Myoldmopar/PlanTools
-Author: Edwin Lee
-Author-email: 
-License: UNKNOWN
+Author: Edwin Lee, for NREL, for United States Department of Energy
+License: ModifiedBSD
 Description: # PLAN-TOOLS
         
         [![Flake8](https://github.com/Myoldmopar/PLAN-Tools/actions/workflows/flake8.yml/badge.svg)](https://github.com/Myoldmopar/PLAN-Tools/actions/workflows/flake8.yml)
         [![Run Tests](https://github.com/Myoldmopar/PLAN-Tools/actions/workflows/test.yml/badge.svg)](https://github.com/Myoldmopar/PLAN-Tools/actions/workflows/test.yml)
         [![Coverage Status](https://coveralls.io/repos/github/Myoldmopar/PLAN-Tools/badge.svg?branch=main)](https://coveralls.io/github/Myoldmopar/PLAN-Tools?branch=main)
         [![PyPIRelease](https://github.com/Myoldmopar/PLAN-Tools/actions/workflows/release.yml/badge.svg)](https://github.com/Myoldmopar/PLAN-Tools/actions/workflows/release.yml)
         [![Documentation Status](https://readthedocs.org/projects/plan-tools/badge/?version=latest)](https://plan-tools.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `PLAN-Tools-0.5/PLAN_Tools.egg-info/PKG-INFO` & `PLAN-Tools-0.6/PLAN_Tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: PLAN-Tools
-Version: 0.5
+Version: 0.6
 Summary: A set of tools to help with Pip Links And Nonsense
 Home-page: https://github.com/Myoldmopar/PlanTools
-Author: Edwin Lee
-Author-email: 
-License: UNKNOWN
+Author: Edwin Lee, for NREL, for United States Department of Energy
+License: ModifiedBSD
 Description: # PLAN-TOOLS
         
         [![Flake8](https://github.com/Myoldmopar/PLAN-Tools/actions/workflows/flake8.yml/badge.svg)](https://github.com/Myoldmopar/PLAN-Tools/actions/workflows/flake8.yml)
         [![Run Tests](https://github.com/Myoldmopar/PLAN-Tools/actions/workflows/test.yml/badge.svg)](https://github.com/Myoldmopar/PLAN-Tools/actions/workflows/test.yml)
         [![Coverage Status](https://coveralls.io/repos/github/Myoldmopar/PLAN-Tools/badge.svg?branch=main)](https://coveralls.io/github/Myoldmopar/PLAN-Tools?branch=main)
         [![PyPIRelease](https://github.com/Myoldmopar/PLAN-Tools/actions/workflows/release.yml/badge.svg)](https://github.com/Myoldmopar/PLAN-Tools/actions/workflows/release.yml)
         [![Documentation Status](https://readthedocs.org/projects/plan-tools/badge/?version=latest)](https://plan-tools.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `PLAN-Tools-0.5/README.md` & `PLAN-Tools-0.6/README.md`

 * *Files identical despite different names*

### Comparing `PLAN-Tools-0.5/plan_tools/entry_point.py` & `PLAN-Tools-0.6/plan_tools/entry_point.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from shutil import copyfile
-from os import chmod, path, stat, symlink
+from os import chmod, path, stat, symlink, fdopen, unlink
 from pathlib import Path
 from platform import system
 from site import USER_BASE, getusersitepackages
+from subprocess import check_call
 from sys import argv
 from sysconfig import get_path
+from tempfile import mkstemp
 from typing import List
 
 
 class EntryPoint:
     """
     This class represents a single executable that is packaged up by setuptools using the entry_points method.
     The entry points may live in either the console_scripts or the gui_scripts subsections.
@@ -76,29 +78,39 @@
         target_exe = scripts_dir / self.installed_binary_name
         icon_file = self.get_package_icon_for_link()
         desktop_file = self.get_path_to_link_file()
         self.write_desktop_file(desktop_file, target_exe, scripts_dir, icon_file)
         return 0
 
     def write_desktop_file(self, desktop_file: Path, target_exe: Path, scripts_dir: Path, icon_file: Path):
-        icon_file_string = icon_file if icon_file.exists() else ''
+        icon_file_string: str = str(icon_file) if icon_file.exists() else ''
         if system() == 'Windows':
             self.desktop_file_data_check = {'exe': target_exe, 'cwd': scripts_dir, 'icon': icon_file_string}
             if self.test_mode:
                 return
             else:  # pragma: no cover
-                # maybe someday we could actually test this in CI
-                # noinspection PyUnresolvedReferences
-                from win32com.client import Dispatch
-                shell = Dispatch('WScript.Shell')
-                s = shell.CreateShortCut(str(desktop_file))
-                s.Targetpath = str(target_exe)
-                s.WorkingDirectory = str(scripts_dir)
-                s.IconLocation = str(icon_file_string)
-                s.save()
+                def escape_path(path_: Path) -> str:
+                    return str(path_).replace('\\', '/')
+
+                shortcut_path = escape_path(desktop_file)
+                target = escape_path(target_exe)
+                working_dir = escape_path(scripts_dir)
+                js_content = f'''var sh = WScript.CreateObject("WScript.Shell");
+var shortcut = sh.CreateShortcut("{shortcut_path}");
+shortcut.TargetPath = "{target}";
+shortcut.WorkingDirectory = "{working_dir}";
+shortcut.IconLocation = "{icon_file_string}";
+shortcut.Save();'''
+                script_fd, script_path = mkstemp('.js')
+                try:
+                    with fdopen(script_fd, 'w') as f:
+                        f.write(js_content)
+                    check_call([R'wscript.exe', script_path])
+                finally:
+                    unlink(script_path)
         elif system() == 'Linux':
             desktop_file_contents = f"""[Desktop Entry]
 Name={self.pretty_link_name}
 Comment={self.description}
 Exec={target_exe}
 Icon={icon_file_string}
 Type=Application
```

### Comparing `PLAN-Tools-0.5/plan_tools/runtime.py` & `PLAN-Tools-0.6/plan_tools/runtime.py`

 * *Files identical despite different names*

### Comparing `PLAN-Tools-0.5/plan_tools/tests/test_entry_point.py` & `PLAN-Tools-0.6/plan_tools/tests/test_entry_point.py`

 * *Files identical despite different names*

### Comparing `PLAN-Tools-0.5/setup.py` & `PLAN-Tools-0.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,34 +5,29 @@
 
 from plan_tools import NAME, VERSION
 
 this_dir = os.path.abspath(os.path.dirname(__file__))
 with codecs.open(os.path.join(this_dir, 'README.md'), encoding='utf-8') as i_file:
     long_description = i_file.read()
 
-install_requires = []
-if system() == 'Windows':
-    install_requires.append('pypiwin32')
-
 setup(
     name=NAME,
     version=VERSION,
     packages=find_packages(exclude=['test', 'tests', 'test.*']),
     url='https://github.com/Myoldmopar/PlanTools',
-    license='',
-    author='Edwin Lee',
-    author_email='',
+    license='ModifiedBSD',
+    author='Edwin Lee, for NREL, for United States Department of Energy',
     description='A set of tools to help with Pip Links And Nonsense',
     long_description=long_description,
     long_description_content_type='text/markdown',
     test_suite='nose.collector',
     tests_require=['nose'],
     keywords='energyplus',
     include_package_data=True,  # use /MANIFEST.in file for declaring package data
-    install_requires=install_requires,
+    install_requires=[],
     entry_points={
         'console_scripts': [
             'plan_tool=plan_tools.runner:cli',
         ],
     },
     python_requires='>=3.5',
 )
```

