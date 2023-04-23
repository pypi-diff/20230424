# Comparing `tmp/amdgpu_stats-0.1.1.tar.gz` & `tmp/amdgpu_stats-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amdgpu_stats-0.1.1.tar", max compression
+gzip compressed data, was "amdgpu_stats-0.1.2.tar", max compression
```

## Comparing `amdgpu_stats-0.1.1.tar` & `amdgpu_stats-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1065 2023-04-23 18:43:59.684481 amdgpu_stats-0.1.1/LICENSE.md
--rw-r--r--   0        0        0     1442 2023-04-23 22:24:06.501687 amdgpu_stats-0.1.1/README.md
--rw-r--r--   0        0        0      503 2023-04-23 22:24:06.501687 amdgpu_stats-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-23 21:03:33.649030 amdgpu_stats-0.1.1/src/amdgpu_stats/__init__.py
--rw-r--r--   0        0        0      393 2023-04-23 21:06:47.224510 amdgpu_stats-0.1.1/src/amdgpu_stats/amdgpu_stats.css
--rwxr-xr-x   0        0        0    14918 2023-04-23 21:43:40.480892 amdgpu_stats-0.1.1/src/amdgpu_stats/amdgpu_stats.py
--rw-r--r--   0        0        0     2367 1970-01-01 00:00:00.000000 amdgpu_stats-0.1.1/setup.py
--rw-r--r--   0        0        0     2130 1970-01-01 00:00:00.000000 amdgpu_stats-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-23 18:43:59.684481 amdgpu_stats-0.1.2/LICENSE.md
+-rw-r--r--   0        0        0     1360 2023-04-23 22:42:12.010831 amdgpu_stats-0.1.2/README.md
+-rw-r--r--   0        0        0      503 2023-04-23 22:39:45.000000 amdgpu_stats-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-23 21:03:33.649030 amdgpu_stats-0.1.2/src/amdgpu_stats/__init__.py
+-rw-r--r--   0        0        0      393 2023-04-23 21:06:47.224510 amdgpu_stats-0.1.2/src/amdgpu_stats/amdgpu_stats.css
+-rwxr-xr-x   0        0        0    14918 2023-04-23 21:43:40.480892 amdgpu_stats-0.1.2/src/amdgpu_stats/amdgpu_stats.py
+-rw-r--r--   0        0        0     2283 1970-01-01 00:00:00.000000 amdgpu_stats-0.1.2/setup.py
+-rw-r--r--   0        0        0     2048 1970-01-01 00:00:00.000000 amdgpu_stats-0.1.2/PKG-INFO
```

### Comparing `amdgpu_stats-0.1.1/LICENSE.md` & `amdgpu_stats-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `amdgpu_stats-0.1.1/README.md` & `amdgpu_stats-0.1.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -25,22 +25,20 @@
 Log screen:
 ![Screenshot of log screen](https://raw.githubusercontent.com/joshlay/amdgpu_stats/master/screens/logging.png "Logging screen")
 
 Statistics are not logged; only toggling Dark/light mode and the stat names / source files.
 
 Tested _only_ on `RX6000` series cards; more may be supported. Please file an issue if finding incompatibility!
 
+## Installation / Usage
+```
+pip install amdgpu-stats
+```
+Once installed, run `amdgpu-stats` in your terminal of choice
 ## Requirements
 Only `Linux` is supported. Information is _completely_ sourced from interfaces in `sysfs`.
 
 It _may_ be necessary to update the `amdgpu.ppfeaturemask` parameter to enable metrics.
 
 This is assumed present for *control* over the elements being monitored. Untested without. 
 
 See [this Arch Wiki entry](https://wiki.archlinux.org/title/AMDGPU#Boot_parameter) for context.
-
-### Python
-The Fedora base repositories provide the requirements with these packages:
- - `python3-humanfriendly`
- - `python3-textual`
-
-See [requirements.txt](requirements.txt) for other distributions
```

### Comparing `amdgpu_stats-0.1.1/src/amdgpu_stats/amdgpu_stats.py` & `amdgpu_stats-0.1.2/src/amdgpu_stats/amdgpu_stats.py`

 * *Files identical despite different names*

### Comparing `amdgpu_stats-0.1.1/setup.py` & `amdgpu_stats-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 ['humanfriendly>=10.0', 'textual>=0.10']
 
 entry_points = \
 {'console_scripts': ['amdgpu-stats = amdgpu_stats.amdgpu_stats:main']}
 
 setup_kwargs = {
     'name': 'amdgpu-stats',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'A simple TUI (using Textual) that shows AMD GPU statistics',
-    'long_description': '# amdgpu_stats\n\nSimple TUI _(using [Textual](https://textual.textualize.io/))_ that shows AMD GPU statistics\n\n- GPU Utilization\n- Temperatures _(as applicable)_\n    - Edge\n    - Junction\n    - Memory\n- Core clock\n- Core voltage\n- Memory clock\n- Power consumption\n- Power limits\n    - Default\n    - Configured\n    - Board capability\n - Fan RPM\n    - Current\n    - Target\n\nMain screen:\n![Screenshot of main screen](https://raw.githubusercontent.com/joshlay/amdgpu_stats/master/screens/main.png "Main screen")\n\nLog screen:\n![Screenshot of log screen](https://raw.githubusercontent.com/joshlay/amdgpu_stats/master/screens/logging.png "Logging screen")\n\nStatistics are not logged; only toggling Dark/light mode and the stat names / source files.\n\nTested _only_ on `RX6000` series cards; more may be supported. Please file an issue if finding incompatibility!\n\n## Requirements\nOnly `Linux` is supported. Information is _completely_ sourced from interfaces in `sysfs`.\n\nIt _may_ be necessary to update the `amdgpu.ppfeaturemask` parameter to enable metrics.\n\nThis is assumed present for *control* over the elements being monitored. Untested without. \n\nSee [this Arch Wiki entry](https://wiki.archlinux.org/title/AMDGPU#Boot_parameter) for context.\n\n### Python\nThe Fedora base repositories provide the requirements with these packages:\n - `python3-humanfriendly`\n - `python3-textual`\n\nSee [requirements.txt](requirements.txt) for other distributions\n',
+    'long_description': '# amdgpu_stats\n\nSimple TUI _(using [Textual](https://textual.textualize.io/))_ that shows AMD GPU statistics\n\n- GPU Utilization\n- Temperatures _(as applicable)_\n    - Edge\n    - Junction\n    - Memory\n- Core clock\n- Core voltage\n- Memory clock\n- Power consumption\n- Power limits\n    - Default\n    - Configured\n    - Board capability\n - Fan RPM\n    - Current\n    - Target\n\nMain screen:\n![Screenshot of main screen](https://raw.githubusercontent.com/joshlay/amdgpu_stats/master/screens/main.png "Main screen")\n\nLog screen:\n![Screenshot of log screen](https://raw.githubusercontent.com/joshlay/amdgpu_stats/master/screens/logging.png "Logging screen")\n\nStatistics are not logged; only toggling Dark/light mode and the stat names / source files.\n\nTested _only_ on `RX6000` series cards; more may be supported. Please file an issue if finding incompatibility!\n\n## Installation / Usage\n```\npip install amdgpu-stats\n```\nOnce installed, run `amdgpu-stats` in your terminal of choice\n## Requirements\nOnly `Linux` is supported. Information is _completely_ sourced from interfaces in `sysfs`.\n\nIt _may_ be necessary to update the `amdgpu.ppfeaturemask` parameter to enable metrics.\n\nThis is assumed present for *control* over the elements being monitored. Untested without. \n\nSee [this Arch Wiki entry](https://wiki.archlinux.org/title/AMDGPU#Boot_parameter) for context.\n',
     'author': 'Josh Lay',
     'author_email': 'pypi@jlay.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/joshlay/amdgpu_stats',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `amdgpu_stats-0.1.1/PKG-INFO` & `amdgpu_stats-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amdgpu-stats
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple TUI (using Textual) that shows AMD GPU statistics
 Home-page: https://github.com/joshlay/amdgpu_stats
 License: MIT
 Author: Josh Lay
 Author-email: pypi@jlay.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -44,23 +44,21 @@
 Log screen:
 ![Screenshot of log screen](https://raw.githubusercontent.com/joshlay/amdgpu_stats/master/screens/logging.png "Logging screen")
 
 Statistics are not logged; only toggling Dark/light mode and the stat names / source files.
 
 Tested _only_ on `RX6000` series cards; more may be supported. Please file an issue if finding incompatibility!
 
+## Installation / Usage
+```
+pip install amdgpu-stats
+```
+Once installed, run `amdgpu-stats` in your terminal of choice
 ## Requirements
 Only `Linux` is supported. Information is _completely_ sourced from interfaces in `sysfs`.
 
 It _may_ be necessary to update the `amdgpu.ppfeaturemask` parameter to enable metrics.
 
 This is assumed present for *control* over the elements being monitored. Untested without. 
 
 See [this Arch Wiki entry](https://wiki.archlinux.org/title/AMDGPU#Boot_parameter) for context.
 
-### Python
-The Fedora base repositories provide the requirements with these packages:
- - `python3-humanfriendly`
- - `python3-textual`
-
-See [requirements.txt](requirements.txt) for other distributions
-
```

