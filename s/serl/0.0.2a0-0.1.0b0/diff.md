# Comparing `tmp/serl-0.0.2a0.tar.gz` & `tmp/serl-0.1.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serl-0.0.2a0.tar", last modified: Thu Mar 30 16:19:36 2023, max compression
+gzip compressed data, was "serl-0.1.0b0.tar", last modified: Mon Apr 24 09:34:26 2023, max compression
```

## Comparing `serl-0.0.2a0.tar` & `serl-0.1.0b0.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-03-30 16:19:36.242234 serl-0.0.2a0/
--rw-rw-rw-   0        0        0     1091 2023-03-30 16:03:47.000000 serl-0.0.2a0/LICENSE
--rw-rw-rw-   0        0        0     2099 2023-03-30 16:19:36.242234 serl-0.0.2a0/PKG-INFO
--rw-rw-rw-   0        0        0      549 2023-03-30 16:14:34.000000 serl-0.0.2a0/README.md
--rw-rw-rw-   0        0        0       84 2023-03-30 16:03:47.000000 serl-0.0.2a0/pyproject.toml
--rw-rw-rw-   0        0        0      815 2023-03-30 16:19:36.244263 serl-0.0.2a0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-30 16:19:36.162909 serl-0.0.2a0/src/
-drwxrwxrwx   0        0        0        0 2023-03-30 16:19:36.207437 serl-0.0.2a0/src/serl/
--rw-rw-rw-   0        0        0        0 2023-03-30 16:03:47.000000 serl-0.0.2a0/src/serl/__init__.py
--rw-rw-rw-   0        0        0       74 2023-03-30 16:03:47.000000 serl-0.0.2a0/src/serl/__main__.py
--rw-rw-rw-   0        0        0     2267 2023-03-30 16:03:47.000000 serl-0.0.2a0/src/serl/config.py
--rw-rw-rw-   0        0        0     3309 2023-03-30 16:16:49.000000 serl-0.0.2a0/src/serl/constants.py
--rw-rw-rw-   0        0        0     3493 2023-03-30 16:03:47.000000 serl-0.0.2a0/src/serl/highlight.py
--rw-rw-rw-   0        0        0     2044 2023-03-30 16:03:47.000000 serl-0.0.2a0/src/serl/lexer.py
--rw-rw-rw-   0        0        0     3366 2023-03-30 16:03:47.000000 serl-0.0.2a0/src/serl/logger.py
--rw-rw-rw-   0        0        0    14101 2023-03-30 16:03:47.000000 serl-0.0.2a0/src/serl/main.py
--rw-rw-rw-   0        0        0     2954 2023-03-30 16:03:47.000000 serl-0.0.2a0/src/serl/parser.py
--rw-rw-rw-   0        0        0     3476 2023-03-30 16:03:47.000000 serl-0.0.2a0/src/serl/schema.py
--rw-rw-rw-   0        0        0     4021 2023-03-30 16:03:47.000000 serl-0.0.2a0/src/serl/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-30 16:19:36.234004 serl-0.0.2a0/src/serl.egg-info/
--rw-rw-rw-   0        0        0     2099 2023-03-30 16:19:36.000000 serl-0.0.2a0/src/serl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      535 2023-03-30 16:19:36.000000 serl-0.0.2a0/src/serl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-30 16:19:36.000000 serl-0.0.2a0/src/serl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-03-30 16:19:36.000000 serl-0.0.2a0/src/serl.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       75 2023-03-30 16:19:36.000000 serl-0.0.2a0/src/serl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-03-30 16:19:36.000000 serl-0.0.2a0/src/serl.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-30 16:19:36.240219 serl-0.0.2a0/tests/
--rw-rw-rw-   0        0        0      807 2023-03-30 16:03:47.000000 serl-0.0.2a0/tests/test_highlight.py
--rw-rw-rw-   0        0        0     1404 2023-03-30 16:03:47.000000 serl-0.0.2a0/tests/test_main.py
--rw-rw-rw-   0        0        0     1698 2023-03-30 16:03:47.000000 serl-0.0.2a0/tests/test_schema.py
--rw-rw-rw-   0        0        0     4027 2023-03-30 16:03:47.000000 serl-0.0.2a0/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:34:26.668791 serl-0.1.0b0/
+-rw-rw-rw-   0        0        0     1091 2023-03-30 16:03:47.000000 serl-0.1.0b0/LICENSE
+-rw-rw-rw-   0        0        0     2116 2023-04-24 09:34:26.668791 serl-0.1.0b0/PKG-INFO
+-rw-rw-rw-   0        0        0      552 2023-03-30 20:15:20.000000 serl-0.1.0b0/README.md
+-rw-rw-rw-   0        0        0       84 2023-03-30 16:03:47.000000 serl-0.1.0b0/pyproject.toml
+-rw-rw-rw-   0        0        0      830 2023-04-24 09:34:26.675340 serl-0.1.0b0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-24 09:34:26.581134 serl-0.1.0b0/src/
+drwxrwxrwx   0        0        0        0 2023-04-24 09:34:26.635625 serl-0.1.0b0/src/serl/
+-rw-rw-rw-   0        0        0        0 2023-03-30 16:03:47.000000 serl-0.1.0b0/src/serl/__init__.py
+-rw-rw-rw-   0        0        0       74 2023-03-30 16:03:47.000000 serl-0.1.0b0/src/serl/__main__.py
+-rw-rw-rw-   0        0        0     2726 2023-04-17 21:26:43.000000 serl-0.1.0b0/src/serl/config.py
+-rw-rw-rw-   0        0        0     3691 2023-04-24 09:28:08.000000 serl-0.1.0b0/src/serl/constants.py
+-rw-rw-rw-   0        0        0     3814 2023-04-21 14:35:48.000000 serl-0.1.0b0/src/serl/highlight.py
+-rw-rw-rw-   0        0        0     2670 2023-04-21 14:39:06.000000 serl-0.1.0b0/src/serl/lexer.py
+-rw-rw-rw-   0        0        0     3359 2023-04-17 20:35:29.000000 serl-0.1.0b0/src/serl/logger.py
+-rw-rw-rw-   0        0        0    18130 2023-04-24 09:20:33.000000 serl-0.1.0b0/src/serl/main.py
+-rw-rw-rw-   0        0        0     4893 2023-04-21 13:33:46.000000 serl-0.1.0b0/src/serl/parser.py
+-rw-rw-rw-   0        0        0     2933 2023-04-21 14:34:29.000000 serl-0.1.0b0/src/serl/schema.py
+-rw-rw-rw-   0        0        0     4588 2023-04-17 08:06:23.000000 serl-0.1.0b0/src/serl/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:34:26.656553 serl-0.1.0b0/src/serl.egg-info/
+-rw-rw-rw-   0        0        0     2116 2023-04-24 09:34:26.000000 serl-0.1.0b0/src/serl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      597 2023-04-24 09:34:26.000000 serl-0.1.0b0/src/serl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 09:34:26.000000 serl-0.1.0b0/src/serl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-04-24 09:34:26.000000 serl-0.1.0b0/src/serl.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       75 2023-04-24 09:34:26.000000 serl-0.1.0b0/src/serl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-24 09:34:26.000000 serl-0.1.0b0/src/serl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 09:34:26.667784 serl-0.1.0b0/tests/
+-rw-rw-rw-   0        0        0      572 2023-04-17 18:50:19.000000 serl-0.1.0b0/tests/test_config.py
+-rw-rw-rw-   0        0        0      807 2023-04-04 06:33:54.000000 serl-0.1.0b0/tests/test_highlight.py
+-rw-rw-rw-   0        0        0     1603 2023-04-17 18:39:39.000000 serl-0.1.0b0/tests/test_lexer.py
+-rw-rw-rw-   0        0        0     4461 2023-04-20 22:48:18.000000 serl-0.1.0b0/tests/test_main.py
+-rw-rw-rw-   0        0        0     2390 2023-04-17 18:00:20.000000 serl-0.1.0b0/tests/test_parser.py
+-rw-rw-rw-   0        0        0     1896 2023-04-17 08:06:23.000000 serl-0.1.0b0/tests/test_schema.py
+-rw-rw-rw-   0        0        0     5478 2023-04-17 17:32:39.000000 serl-0.1.0b0/tests/test_utils.py
```

### Comparing `serl-0.0.2a0/LICENSE` & `serl-0.1.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `serl-0.0.2a0/PKG-INFO` & `serl-0.1.0b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: serl
-Version: 0.0.2a0
+Version: 0.1.0b0
 Summary: Serialized Language (serl)
 Author: Harry Downing
 Author-email: harry.downing17@gmail.com
+License: MIT
 Project-URL: repository, https://github.com/harrydowning/serl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Serialized Language (serl)
-Serl is a command line tool used to manage and execute complete languages serialized with YAML.
+Serl is a command line tool used to manage and execute programming languages serialized with YAML.
 
 ### Development Workflow
 | Command | Description |
 | ------- | ----------- |
 | `pip install .` | Build/install locally |
 | `serl help` | Show the tool command line help screen |
 | `pytest tests` or `test.bat` | Run automated test suite |
```

### Comparing `serl-0.0.2a0/README.md` & `serl-0.1.0b0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Serialized Language (serl)
-Serl is a command line tool used to manage and execute complete languages serialized with YAML.
+Serl is a command line tool used to manage and execute programming languages serialized with YAML.
 
 ### Development Workflow
 | Command | Description |
 | ------- | ----------- |
 | `pip install .` | Build/install locally |
 | `serl help` | Show the tool command line help screen |
 | `pytest tests` or `test.bat` | Run automated test suite |
```

### Comparing `serl-0.0.2a0/setup.cfg` & `serl-0.1.0b0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -10,42 +10,43 @@
 00000090: 2053 6572 6961 6c69 7a65 6420 4c61 6e67   Serialized Lang
 000000a0: 7561 6765 2028 7365 726c 290d 0a6c 6f6e  uage (serl)..lon
 000000b0: 675f 6465 7363 7269 7074 696f 6e20 3d20  g_description = 
 000000c0: 6669 6c65 3a20 5245 4144 4d45 2e6d 642c  file: README.md,
 000000d0: 204c 4943 454e 5345 0d0a 6c6f 6e67 5f64   LICENSE..long_d
 000000e0: 6573 6372 6970 7469 6f6e 5f63 6f6e 7465  escription_conte
 000000f0: 6e74 5f74 7970 6520 3d20 7465 7874 2f6d  nt_type = text/m
-00000100: 6172 6b64 6f77 6e0d 0a70 726f 6a65 6374  arkdown..project
-00000110: 5f75 726c 7320 3d20 0d0a 0972 6570 6f73  _urls = ...repos
-00000120: 6974 6f72 7920 3d20 6874 7470 733a 2f2f  itory = https://
-00000130: 6769 7468 7562 2e63 6f6d 2f68 6172 7279  github.com/harry
-00000140: 646f 776e 696e 672f 7365 726c 0d0a 636c  downing/serl..cl
-00000150: 6173 7369 6669 6572 7320 3d20 0d0a 0950  assifiers = ...P
-00000160: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000170: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000180: 2033 0d0a 094c 6963 656e 7365 203a 3a20   3...License :: 
-00000190: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
-000001a0: 4d49 5420 4c69 6365 6e73 650d 0a09 4f70  MIT License...Op
-000001b0: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
-000001c0: 3a20 4f53 2049 6e64 6570 656e 6465 6e74  : OS Independent
-000001d0: 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d 0a70  ....[options]..p
-000001e0: 6163 6b61 6765 5f64 6972 203d 200d 0a09  ackage_dir = ...
-000001f0: 3d20 7372 630d 0a70 6163 6b61 6765 7320  = src..packages 
-00000200: 3d20 6669 6e64 3a0d 0a70 7974 686f 6e5f  = find:..python_
-00000210: 7265 7175 6972 6573 203d 203e 3d33 2e31  requires = >=3.1
-00000220: 310d 0a69 6e73 7461 6c6c 5f72 6571 7569  1..install_requi
-00000230: 7265 7320 3d20 0d0a 0950 7959 414d 4c0d  res = ...PyYAML.
-00000240: 0a09 646f 636f 7074 0d0a 0970 6c79 3d3d  ..docopt...ply==
-00000250: 332e 3131 0d0a 0972 6567 6578 0d0a 096e  3.11...regex...n
-00000260: 6574 776f 726b 780d 0a09 6a73 6f6e 7363  etworkx...jsonsc
-00000270: 6865 6d61 0d0a 0950 7967 6d65 6e74 730d  hema...Pygments.
-00000280: 0a09 5069 6c6c 6f77 0d0a 0972 6571 7565  ..Pillow...reque
-00000290: 7374 730d 0a0d 0a5b 6f70 7469 6f6e 732e  sts....[options.
-000002a0: 7061 636b 6167 6573 2e66 696e 645d 0d0a  packages.find]..
-000002b0: 7768 6572 6520 3d20 7372 630d 0a0d 0a5b  where = src....[
-000002c0: 6f70 7469 6f6e 732e 656e 7472 795f 706f  options.entry_po
-000002d0: 696e 7473 5d0d 0a63 6f6e 736f 6c65 5f73  ints]..console_s
-000002e0: 6372 6970 7473 203d 200d 0a09 7365 726c  cripts = ...serl
-000002f0: 203d 2073 6572 6c2e 6d61 696e 3a6d 6169   = serl.main:mai
-00000300: 6e0d 0a0d 0a5b 6567 675f 696e 666f 5d0d  n....[egg_info].
-00000310: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
-00000320: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
+00000100: 6172 6b64 6f77 6e0d 0a6c 6963 656e 7365  arkdown..license
+00000110: 203d 204d 4954 0d0a 7072 6f6a 6563 745f   = MIT..project_
+00000120: 7572 6c73 203d 200d 0a09 7265 706f 7369  urls = ...reposi
+00000130: 746f 7279 203d 2068 7474 7073 3a2f 2f67  tory = https://g
+00000140: 6974 6875 622e 636f 6d2f 6861 7272 7964  ithub.com/harryd
+00000150: 6f77 6e69 6e67 2f73 6572 6c0d 0a63 6c61  owning/serl..cla
+00000160: 7373 6966 6965 7273 203d 200d 0a09 5072  ssifiers = ...Pr
+00000170: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000180: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000190: 330d 0a09 4c69 6365 6e73 6520 3a3a 204f  3...License :: O
+000001a0: 5349 2041 7070 726f 7665 6420 3a3a 204d  SI Approved :: M
+000001b0: 4954 204c 6963 656e 7365 0d0a 094f 7065  IT License...Ope
+000001c0: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+000001d0: 204f 5320 496e 6465 7065 6e64 656e 740d   OS Independent.
+000001e0: 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a 7061  ...[options]..pa
+000001f0: 636b 6167 655f 6469 7220 3d20 0d0a 093d  ckage_dir = ...=
+00000200: 2073 7263 0d0a 7061 636b 6167 6573 203d   src..packages =
+00000210: 2066 696e 643a 0d0a 7079 7468 6f6e 5f72   find:..python_r
+00000220: 6571 7569 7265 7320 3d20 3e3d 332e 3131  equires = >=3.11
+00000230: 0d0a 696e 7374 616c 6c5f 7265 7175 6972  ..install_requir
+00000240: 6573 203d 200d 0a09 5079 5941 4d4c 0d0a  es = ...PyYAML..
+00000250: 0964 6f63 6f70 740d 0a09 706c 793d 3d33  .docopt...ply==3
+00000260: 2e31 310d 0a09 7265 6765 780d 0a09 6e65  .11...regex...ne
+00000270: 7477 6f72 6b78 0d0a 096a 736f 6e73 6368  tworkx...jsonsch
+00000280: 656d 610d 0a09 5079 676d 656e 7473 0d0a  ema...Pygments..
+00000290: 0950 696c 6c6f 770d 0a09 7265 7175 6573  .Pillow...reques
+000002a0: 7473 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  ts....[options.p
+000002b0: 6163 6b61 6765 732e 6669 6e64 5d0d 0a77  ackages.find]..w
+000002c0: 6865 7265 203d 2073 7263 0d0a 0d0a 5b6f  here = src....[o
+000002d0: 7074 696f 6e73 2e65 6e74 7279 5f70 6f69  ptions.entry_poi
+000002e0: 6e74 735d 0d0a 636f 6e73 6f6c 655f 7363  nts]..console_sc
+000002f0: 7269 7074 7320 3d20 0d0a 0973 6572 6c20  ripts = ...serl 
+00000300: 3d20 7365 726c 2e6d 6169 6e3a 6d61 696e  = serl.main:main
+00000310: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
+00000320: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
+00000330: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
```

### Comparing `serl-0.0.2a0/src/serl/config.py` & `serl-0.1.0b0/src/serl/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-import os, re
-import yaml
-import requests
+import os
+import re
+
 import serl.logger as logger
 from serl.constants import SYSTEM_CONFIG_DIR, SYSTEM_CONFIG_ENV_DIR
 from serl.schema import validate
 
+import yaml
+import requests
+
 def get_config_dir(path=[]) -> str:
     home = os.path.expanduser('~')
     config_dir = os.path.join(home, SYSTEM_CONFIG_DIR, *path)
     os.makedirs(config_dir, exist_ok=True)
     return config_dir
 
 def get_config_env_dir() -> str:
@@ -31,35 +34,46 @@
         return None
 
 def get_url_config_text(url: str) -> str | None:
     r = requests.get(url)
     r.raise_for_status()
     return r.text
 
-def get_config_text(language: str) -> str | None:
+def get_config_text(language: str, symlink: bool) -> str | None:
     if re.match(r'https?://.*', language):
         try:
             config_text = get_url_config_text(language)
         except requests.exceptions.ConnectionError as ce:
-            logger.error(ce)
+            logger.error(ce, code=1)
         except requests.exceptions.HTTPError as httpe:
-            logger.error(httpe)
+            logger.error(httpe, code=1)
         except requests.exceptions.RequestException as rqe:
-            logger.error(rqe)
+            logger.error(rqe, code=1)
     else:
-        # File config has higher precedence than system
-        config_text = get_file_config_text(language) or \
+        config_text = None
+        if not symlink:
+            # File config has higher precedence than system
+            config_text = get_file_config_text(language)
+        config_text = config_text or \
             get_file_config_text(language, get_config_dir())
         if config_text == None:
             logger.error(f"Could not find system or file config for " 
-                         f"\'{language}\'.")
+                         f"\'{language}\'.", code=1)
     return config_text
 
-def get_config(language: str) -> dict:
-    config_text = get_config_text(language)
-    config = yaml.safe_load(config_text) # TODO handle errors
+def get_config(language: str, symlink: bool) -> dict:
+    config_text = get_config_text(language, symlink)
+    try:
+        config = yaml.safe_load(config_text)
+    except yaml.YAMLError as err:
+        err.with_traceback(None)
+        logger.error(f'YAML parser error:\n\n{err}', code=1)
 
-    valid, error = validate(config)
-    if valid:
+    errs = validate(config)
+    if errs == []:
         return config
     else:
-        logger.error(f'Validation error in config \'{language}\'. {error}')
+        err_msg = lambda file, err: f'Validation error in \'{file}\': {err}'
+        last = errs.pop()
+        for err in errs:
+            logger.error(err_msg(language, err))
+        logger.error(err_msg(language, last), code=1)
```

### Comparing `serl-0.0.2a0/src/serl/highlight.py` & `serl-0.1.0b0/src/serl/highlight.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,52 @@
 import re
+
 import serl.logger as logger
+
 import pygments
 from pygments.style import Style, StyleMeta
 from pygments.util import ClassNotFound
 from pygments.lexer import RegexLexer
-from pygments.token import string_to_tokentype, Text, Comment, Whitespace
+from pygments.token import string_to_tokentype, Token, Comment, Whitespace
 from pygments.formatters import get_formatter_by_name
 from pygments.styles import get_style_by_name
 
+SerlToken = string_to_tokentype('Token.Serl')
 def get_pygments_lexer(_tokens: dict, ignore: str, tokentypes: dict):
     tokentypes = {t: ttype.title() for t, ttype in tokentypes.items()}
     class PygmentsLexer(RegexLexer):
         flags = re.VERBOSE
 
         tokens = {
             'root': [
                 (_tokens.get(name_or_pattern, name_or_pattern), 
                  string_to_tokentype(ttype)) 
                 for name_or_pattern, ttype in tokentypes.items()
-            ] + [
-                (pattern, Text) for name, pattern in _tokens.items()
-            ] + [
-                (r'\s', Whitespace), # TODO may not need
-                (ignore, Comment)
-            ]
+            ] + [(r'\s', Whitespace)]
         }
-    return PygmentsLexer()
+        if ignore:
+            tokens['root'].append((ignore, Comment))
+        tokens['root'].append(('.', SerlToken))
+    try:
+        return PygmentsLexer()
+    except ValueError as err:
+        logger.error(f'Syntax highlighter lexer error: {err}', code=1)
 
 def get_pygments_style(style: StyleMeta, user_styles: dict[str, str]):
     attrs = {
         attr: getattr(style, attr) 
         for attr in dir(style) 
         if not attr.startswith('_')
     }
 
     attrs['styles'] = attrs.get('styles', {}) | {
         string_to_tokentype(tokentype.title()): user_style
         for tokentype, user_style in user_styles.items()
     }
+    attrs['styles'][SerlToken] = attrs['styles'][Token]
     # Create class with type(...) to allow dynamic creation of attrs
     PygmentsStyle = type('PygmentsStyle', (Style,), attrs)
     return PygmentsStyle
 
 def parse_key_value(input: str) -> dict:
     result = {}
     str_re = r'(?s)([\'\"])(.*?)\1'
@@ -59,25 +64,25 @@
         try:
             name, value = option.split('=', 1)
         except ValueError:
             result[option] = True
             continue
         value %= str_vals
         try:
-            result[name] = eval(value)
+            result[name] = eval(value, {}, {})
         except NameError:
             result[name] = value
         except Exception as e:
             logger.warning(f'Error with option \'{option}\', {e}')
             continue
     return result
 
 def get_pygments_output(src: str, tokens: dict[str, str], ignore: str, 
                        tokentypes: dict[str, str], user_styles: dict[str, str],
-                       format: str, format_options: dict) -> str:
+                       format: str, format_options: dict, style_defs_arg):
     lexer = get_pygments_lexer(tokens, ignore, tokentypes)
     
     style_name = format_options.get('style', None)
     if style_name:
         try:
             style = get_style_by_name(style_name)
         except ClassNotFound:
@@ -86,10 +91,15 @@
             style = get_style_by_name('default')
         
         format_options['style'] = get_pygments_style(style, user_styles)
 
     try:
         formatter = get_formatter_by_name(format, **format_options)
     except ClassNotFound:
-        logger.error(f'No Pygment formmatter found for \'{format}\'.')
+        logger.error(f'No Pygment formmatter found for \'{format}\'.', code=1)
+    
+    try:
+        style_defs = formatter.get_style_defs(style_defs_arg)
+    except NotImplementedError:
+        style_defs = None
 
-    return pygments.highlight(src, lexer, formatter),formatter.get_style_defs()
+    return pygments.highlight(src, lexer, formatter), style_defs
```

### Comparing `serl-0.0.2a0/src/serl/lexer.py` & `serl-0.1.0b0/tests/test_lexer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,67 +1,36 @@
-import re, regex
-import serl.logger as logger
-import ply.lex as lex
-import platform
-
-implementation = platform.python_implementation()
-using_cpython = implementation == 'CPython'
-
-def get_pattern_function(token, pattern, using_regex):
-    def f(t):
-        s, e = t.lexer.lexmatch.span()
-        string = t.lexer.lexmatch.string[s:e]
-        # Obtain capture groups
-        if using_regex and using_cpython:
-            m = regex.match(pattern, string, regex.VERBOSE)
-            t.value = m.allcaptures()
-        else:
-            m = re.match(pattern, string, re.VERBOSE)
-            t.value = (m.group(), *m.groups())
-        t.lexer.lineno += string.count('\n')
-        return t
-    
-    f.__doc__ = pattern
-    f.__name__ = token
-    return f
-
-def newline(t):
-    r'\n+'
-    t.lexer.lineno += len(t.value)
-
-def t_error(t):
-    logger.warning(f'Illegal character \'{t.value[0]}\' on line '
-                   f'{t.lexer.lineno}.')
-
-def get_ignore_func(pattern):
-    def f(t): pass
-    f.__name__ = 'ignore'
-    f.__doc__ = pattern
-    return f
-
-def build_lexer(_tokens: dict[str, str], token_map: dict[str,str], ignore: str,
-                using_regex: bool):
-    g = globals()
-    g['tokens'] = ()
-
-    for token, pattern in _tokens.items():
-        token_name = token_map[token]
-
-        g['tokens'] = (*g['tokens'], token_name)
-        g[f't_{token_name}'] = get_pattern_function(token, pattern, using_regex)
-
-    # TODO g['t_DEFAULT'] = r'.'
-    # Lower precedence than user rules
-    g['t_newline'] = newline
-    if ignore != None:
-        g['t_ignore_func'] = get_ignore_func(ignore)
-    
-    if using_regex:
-        if using_cpython:
-            lex.re = regex
-        else:
-            logger.error(f'Use of \'regex\' package requires \'CPython\' '
-                         f'implementation. Current implementation: '
-                         f'\'{implementation}\'.')
-    
-    errorlog = logger.LoggingWrapper(ply_repl=True)
-    return lex.lex(errorlog=errorlog)
+from types import SimpleNamespace
+import pytest
+import serl.lexer as lexer
+
+class MockLexToken(object):
+    def __init__(self, span=None, string=None, lineno=None, value=None):
+        self.lexer = SimpleNamespace(
+            lexmatch = SimpleNamespace(span=lambda: span, string=string),
+            lineno = lineno
+        )
+        self.value = value
+
+    def __eq__(self, __value: object) -> bool:
+        return __value.value == self.value and __value.lexer.lineno == self.lexer.lineno
+
+
+@pytest.mark.parametrize('token, pattern, using_regex, using_cpython, t, expected', [
+    ('TOK1', r':(\d+):', False, True, MockLexToken((3,8), 'aaa:123:a', 1), MockLexToken(lineno=1, value=(':123:', '123'))),
+    ('TOK2', r':(\d+):', True, True, MockLexToken((3,8), 'aaa:123:a', 2), MockLexToken(lineno=2, value=([':123:'], ['123']))),
+    ('TOK3', r'(\|(\d+))+\n', True, True, MockLexToken((5,20), 'start|1|22|333|4444\nend', 2), MockLexToken(lineno=3, value=(['|1|22|333|4444\n'], ['|1', '|22', '|333', '|4444'], ['1', '22', '333', '4444']))),
+])
+def test_get_pattern_func(token, pattern, using_regex, using_cpython, t, expected):
+    lexer.using_cpython = using_cpython
+    pattern_func = lexer.get_pattern_func(token, pattern, using_regex)
+    assert pattern_func.__doc__ == pattern
+    assert pattern_func.__name__ == token
+    t = pattern_func(t)
+    assert t == expected
+
+
+def test_get_ignore_func():
+    pattern = '.*!@#$%^&*()'
+    ignore_func = lexer.get_ignore_func(pattern)
+    assert ignore_func.__doc__ == pattern
+    assert ignore_func.__name__ == 'ignore'
+
```

### Comparing `serl-0.0.2a0/src/serl/logger.py` & `serl-0.1.0b0/src/serl/logger.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 import logging
 import re
+
 from serl.constants import PLY_ERR_MSG
 
 verbose = False
-strict = False
+error_seen = False
 
 logging.basicConfig(format='%(levelname)s: %(message)s')
 logging.getLogger().setLevel(logging.INFO)
 
 class LoggingWrapper():
-    def __init__(self, logger = logging, *, verbose=None, strict=None, 
-                 repl_map={}, ply_repl=False):
+    def __init__(self, logger = logging, *, verbose=None, repl_map={}, 
+                 ply_repl=False):
         self.logger = logger
         self.verbose = verbose
-        self.strict = strict
         self.repl_map = repl_map
         self.ply_repl = ply_repl
     
     def _repl(self, msg, args):
-        msg, args = self._ply_repl(msg, args)
         args = self._args_repl(msg, args)
-        msg %= args
+        msg = self._ply_repl(msg, args)
         return self._str_repl(msg)
 
     def _ply_repl(self, msg, args):
-        if not self.ply_repl or not msg in PLY_ERR_MSG:
-            return msg, args
-        else:
-            new_msg, arg_idxs = PLY_ERR_MSG[msg]
-            return new_msg, tuple(args[i] for i in arg_idxs)
+        msg %= args
+        if self.ply_repl:
+            for key, template in PLY_ERR_MSG.items():
+                match = re.match(key, msg)
+                if match: 
+                    return match.expand(template)
+        return msg
 
     def _str_repl(self, s: str) -> str:
         for pattern, repl in self.repl_map.items():
             s = s.replace(pattern, repl)
         return s
 
     def _args_repl(self, msg, args):
@@ -54,35 +55,34 @@
                      if t == 's' else args[0][k]
                      for k, t in matches},)
         
         return tuple([self._str_repl(str(args[i])) 
                           if t == 's' else args[i] 
                           for i, (_, t) in enumerate(matches)])
 
-    def info(self, msg, *args, important=False):
+    def info(self, msg, *args, important=False, **kwargs):
         msg = self._repl(msg, args)
         should_show = self.verbose if self.verbose != None else verbose
         if should_show or important:
-            self.logger.info(msg)
+            self.logger.info(msg, **kwargs)
 
     def debug(self, msg, *args, **kwargs):
         self.info(msg, *args, **kwargs)
 
-    def warning(self, msg, *args):
+    def warning(self, msg, *args, **kwargs):
         msg = self._repl(msg, args)
-        self.logger.warning(msg)
-        should_exit = self.strict if self.strict != None else strict
-        if should_exit:
-            exit(1)
+        self.logger.warning(msg, **kwargs)
 
-    def error(self, msg, *args, should_exit=True):
+    def error(self, msg, *args, code=0, **kwargs):
         msg = self._repl(msg, args)
-        self.logger.error(msg)
-        if should_exit:
-            exit(1)
+        self.logger.error(msg, **kwargs) 
+        global error_seen
+        error_seen = True
+        if code:
+            exit(code)
 
 def get_file_logger(filename: str, **kwargs):
     file_logger = logging.getLogger('file')
     file_handler = logging.FileHandler(filename, mode='w', delay=True)
     file_logger.addHandler(file_handler)
     file_logger.propagate = False
     return LoggingWrapper(file_logger, **kwargs)
@@ -91,12 +91,12 @@
 
 def info(msg, *args, **kwargs):
     logger.info(msg, *args, **kwargs)
 
 def debug(msg, *args, **kwargs):
     logger.debug(msg, *args, **kwargs)
 
-def warning(msg, *args):
-    logger.warning(msg, *args)
+def warning(msg, *args, **kwargs):
+    logger.warning(msg, *args, **kwargs)
 
-def error(msg, *args):
-    logger.error(msg, *args)
+def error(msg, *args, **kwargs):
+    logger.error(msg, *args, **kwargs)
```

### Comparing `serl-0.0.2a0/src/serl/main.py` & `serl-0.1.0b0/src/serl/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 import sys
 init_modules = sys.modules.copy().keys()
 
-import os, fileinput, subprocess, pathlib, re, venv, site, shutil
-from docopt import docopt
-import networkx as nx
+import os
+import fileinput
+import subprocess
+import pathlib
+import re
+import venv
+import site
+import shutil
+import ast
+import glob
+import traceback
+
 from serl.lexer import build_lexer
-from serl.parser import build_parser, AST
+from serl.parser import build_parser, SerlAST
 import serl.utils as utils
 import serl.logger as logger
 from serl.highlight import get_pygments_output, parse_key_value
 from serl.config import get_config, get_config_dir, get_config_env_dir, \
     get_config_text, system_config_exists, system_config_languages
 from serl.constants import CLI, SYMLINK_CLI, CLI_COMMANDS, NAME, VERSION, \
-    DEFAULT_REF, RETURN_VAR
-
-class Functionality():
-    def __init__(self, code: dict, commands: dict, grammar_map: dict):
-        self.code = utils.normalise_dict(code)
-        self.commands = utils.normalise_dict(commands)
-
-        items = self.code.items()
-        name, cd = next(iter(items), None)
-        self.main = cd if not name in grammar_map else None
-
-        dups = utils.get_dups(self.code, self.commands)
-        if len(dups) > 0:
-            msg = (f'Functionality defined in both \'code\' and \'command\' '
-                   f'for {", ".join(map(str, dups))}, \'code\' will take '
-                   f'precedence.')
-            logger.warning(msg)
+    DEFAULT_REF, SHELL_CHAR, VENV_CONFIG, EXCEPTION_ATTR 
 
-    def _get(self, d: dict, name: str, pos: int) -> str | None:
-        v = d.get(name, None)
-        if v and len(v) > pos:
-            return v[pos]
-        return None
+from docopt import docopt
+import networkx as nx
 
-    def get_code(self, name: str, pos: int) -> str | None:
-        return self._get(self.code, name, pos)
+class Traversable():
+    def __init__(self, f):
+        self.f = f
+    
+    def __call__(self, *args, **kwargs):
+        return self.f(*args, **kwargs)
+
+class TraversableFormat(dict):
+    def __getitem__(self, __key):
+        __val = super().__getitem__(__key)
+        if isinstance(__val, Traversable):
+            return __val()
+        return __val
 
-    def get_command(self, name: str, pos: int) -> str | None:
-        return self._get(self.commands, name, pos)
+    def __missing__(self, key):
+        return key
 
 def token_expansion(tokens: dict[str, str], split: list[str]) -> dict[str, str]:
     repl_tokens = utils.get_repl_tokens(tokens, split)
     token_graph = nx.DiGraph(utils.get_token_graph(repl_tokens))
     cycles = list(nx.simple_cycles(token_graph))
 
     if cycles:
@@ -85,233 +86,328 @@
         exit(e.returncode)
 
 def highlight(args: dict, src: str, tokens: dict, ignore: str, 
               tokentypes: dict, user_styles: dict):
     filename = args['--highlight']
     format = args['--format'] or os.path.splitext(filename)[1][1:]
     format_options = parse_key_value(args['--format-options'] or '')
+    style_defs_arg = args['--style-defs-arg']
         
     output = get_pygments_output(src, tokens, ignore, tokentypes, user_styles, 
-                                 format, format_options)
+                                 format, format_options, style_defs_arg)
     highlighted_src, style_defs = output
     if type(highlighted_src) == bytes:
         mode = 'wb'
     else:
         mode = 'w'
 
     with open(filename, mode) as file:
         file.write(highlighted_src)
     
-    if args['--style-defs']:
+    if args['--style-defs'] and style_defs:
         with open(args['--style-defs'], 'w') as file:
             file.write(style_defs)
     exit(0)
 
-def link_command(args):
+def command_line_link(args):
     language = args['<language>']
     dir = args['<dir>'] or ''
     
     src = extension(sys.argv[0])
     dst = extension(os.path.join(dir, language))
 
     if not system_config_exists(language):
         logger.warning(f'No system config for language \'{language}\'')
 
     try:
         os.symlink(src, dst)
         print(f'Successfully linked \'{language}\'.')
     except Exception as e:
-        logger.error(f'Symbolic link error: {e}')
+        logger.error(f'Symbolic link error: {e}', code=1)
 
-def run_command(args):
+def command_line_run(args):
     language = args['<language>']
     lang_name = utils.get_language_name(language)
-    config = get_config(language)
-
-    env = config.get('environment', None)
-    env_created = False
-    if env:
-        for sitepackage in site.getsitepackages():
-            sys.path.remove(sitepackage)
-        
-        env_name = os.path.join(get_config_env_dir(), env)
-        if not os.path.exists(env_name):
-            logger.info(f'Creating virtual environment \'{env}\'.', 
-                        important=True)
-            venv.create(env_name, with_pip=True)
-            env_created = True
-        
-        for sitepackage in site.getsitepackages([env_name]):
-            sys.path.append(sitepackage)
-        
-        context = venv.EnvBuilder().ensure_directories(env_name)
-        sys.executable = context.env_exe
-
-    if args['--requirements'] or env_created:
-        logger.info(f'Installing requirements.', important=True)
-        requirements(config.get('requirements', None))
+    config = get_config(language, get_link_filename())
 
     version = config.get('version', None)
     usage = config.get('usage', None)
     
     inputs = args['<args>']
-    debug_file = args['--debug']
+    debug_parser_file = args['--debug-parser']
+    debug_lexer = args['--debug-lexer']
 
     # User language docopt
     if usage != None:
         language_args = docopt(usage, argv=inputs, version=version)
         src_input = language_args.get('<src>', None)
         if not(isinstance(src_input, str) or src_input == None):
             logger.error('File to be parsed must be specified in usage pattern' 
                          ' as \'<src>\' (filepath), \'[<src>]\' '
-                         '(filepath or stdin) or nothing (stdin).')
+                         '(filepath or stdin) or nothing (stdin).', code=1)
     else:
+        language_args = {}
         src_input = next(iter(inputs), None) # First element if it exists
     
     # Read input file if prsent else read from stdin
     with fileinput.input(files=src_input or ()) as file:
         src = ''.join(file)
     
     meta = config.get('meta', {})
     meta_tokens = meta.get('tokens', {})
 
-    tokens = config['tokens']
+    tokens = config.get('tokens', {})
     ref = meta_tokens.get('ref', DEFAULT_REF)
     using_regex = meta_tokens.get('regex', False)
-    ignore = meta_tokens.get('ignore', '.')
+    ignore = meta_tokens.get('ignore', r'\s')
+    flags = meta_tokens.get('flags', 'VERBOSE')
+    default = meta_tokens.get('default', True)
     
     tokens_copy = tokens.copy()
     if ref != None:
         # if 'token' not used assume given string is prefix of token repl.
         ref += '' if 'token' in ref else 'token'
         logger.info(f'Performing token expansion with \'ref\' pattern '
                     f'\'{ref}\' (default: \'{DEFAULT_REF}\')')
         tokens = token_expansion(tokens, ref.split('token'))
     
     for token in tokens_copy:
         tb, ta = tokens_copy[token].strip(), tokens[token].strip()
-        if tb != ta:
+        if tb != ta: # TODO case where expansion is actually equal?
             logger.info(f'Token \'{token}\' expanded: \'{tb}\' -> \'{ta}\'')
 
     precedence = config.get('precedence', [])
-    sync = config.get('sync', [])
     grammar = config['grammar']
-    permissive = meta.get('permissive', True)
+    error_sym = config.get('error', None)
+    meta_grammar = meta.get('grammar', {})
+    permissive = meta_grammar.get('permissive', True)
 
     token_map = {k: f'TERMINAL{i}' for i, k, in enumerate(tokens.keys())}
     grammar_map = {k: f'NONTERMINAL{i}' for i, k in enumerate(grammar.keys())}
     common_keys = set(token_map.keys()).intersection(grammar_map.keys())
+    s = '\', \''
     if common_keys:
-        s = '\', \''
         logger.error(f'Grammar identifiers \'{s.join(common_keys)}\' already '
-                     f'used in tokens')
+                     f'used in tokens', code=1)
     
     symbol_map = token_map | grammar_map
     grammar = utils.normalise_grammar(symbol_map, grammar)
 
-    tokens_in_grammar = utils.get_tokens_in_grammar(token_map, grammar)
-    tokens = utils.filter_dict_keys(tokens, tokens_in_grammar)
-    token_map = utils.filter_dict_keys(token_map, tokens_in_grammar)
+    tokens_used, implicit_map = utils.get_tokens_in_grammar(token_map, 
+                                                            error_sym, grammar)
+    tokens = utils.keep_keys_in_list(tokens, tokens_used)
+    token_map = utils.keep_keys_in_list(token_map, tokens_used) | implicit_map
+    tokens |= {k: re.escape(k) for k, v in implicit_map.items()}
     symbol_map = token_map | grammar_map
 
+    if error_sym in symbol_map:
+        logger.error(f'Multiple definitions for \'{error_sym}\'.', code=1)
+    elif error_sym:
+        symbol_map[error_sym] = 'error'
+
+    if len(implicit_map):
+        logger.info(f'Implicit tokens: \'{s.join(implicit_map.keys())}\'')
+
     if args['--highlight']:
         tokentypes = config.get('tokentypes', {})
         user_styles = config.get('styles', {})
         highlight(args, src, tokens, ignore, tokentypes, user_styles)
 
-    lexer = build_lexer(tokens, token_map, ignore, using_regex)
-    parser = build_parser(lang_name, list(token_map.values()), symbol_map, 
-                          grammar, precedence, debug_file, sync, permissive)
-    # lexer.input(src)
-    # while True:
-    #     tok = lexer.token()
-    #     if not tok: 
-    #         break      # No more input
-    #     print(tok)
-
-    # ast = parser.parse(src, lexer=lexer)
-    code = config.get('code', {})
-    commands = config.get('commands', {})
-    functionality = Functionality(code, commands, grammar_map)
+    lexer = build_lexer(tokens, token_map, ignore, using_regex, flags, default)
+    parser = build_parser(
+        lang_name, list(token_map.values()), symbol_map, grammar, precedence,
+        debug_parser_file
+    )
+
+    # Debug lexer
+    lexer_clone = lexer.clone()
+    flipped_token_map = utils.flip_dict(token_map)
+    lexer_clone.input(src)
+    lines = src.count('\n') + 1
+    tokens_by_line = [[] for _ in range(lines)]
+    
+    while True:
+        tok = lexer_clone.token()
+        if not tok: 
+            break
+        if tok.type == 'default':
+            tokens_by_line[tok.lineno - 1].append('default')
+        else:
+            tokens_by_line[tok.lineno - 1].append(flipped_token_map[tok.type])
     
+    logger.info(f'Tokens Found:', important=debug_lexer)
+    for i, line in enumerate(tokens_by_line):
+        lineno = str(i + 1).rjust(len(str(lines)), ' ')
+        logger.info(f'  {lineno}: {" ".join(line)}', important=debug_lexer)
+    # Debug lexer
+
+    serl_ast = parser.parse(src, lexer=lexer, tracking=True)
+    if (not permissive and logger.error_seen) or not serl_ast:
+        logger.error('Parse Failed', code=1)
+    
+    code = utils.normalise_dict(config['code'])
+    main_code = utils.get_main_code(code, grammar_map)
+    
+    for code_name, code_list in code.items():
+        internal_name = grammar_map.get(code_name, None)
+        if not internal_name: continue
+        for i in range(len(grammar[internal_name])):
+            value = code_list[i] if len(code_list) > i else None
+            if value == None:
+                logger.warning(f'Code missing for $.code.{code_name}[{i}]')
+    
+    # #################################################################
+
+    venv_name = config.get('environment', None)
+    venv_created = False
+    if venv_name:
+        for sitepackage in site.getsitepackages():
+            sys.path.remove(sitepackage)
+        
+        venv_path = os.path.join(get_config_env_dir(), venv_name)
+        if not glob.glob(os.path.join(venv_path, VENV_CONFIG)):
+            logger.info(f'Creating virtual environment \'{venv_name}\'.', 
+                        important=True)
+            venv.create(venv_path, with_pip=True)
+            venv_created = True
+        
+        for sitepackage in site.getsitepackages([venv_path]):
+            sys.path.append(sitepackage)
+        
+        context = venv.EnvBuilder().ensure_directories(venv_path)
+        sys.executable = context.env_exe
+
+    if args['--requirements'] or venv_created:
+        logger.info(f'Installing requirements.', important=True)
+        requirements(config.get('requirements', None))
+
     # Remove module cache to allow for correct user import
     for module in sys.modules.copy().keys():
         if not module in init_modules:
             del sys.modules[module]
 
-    # root_execute = get_execute_func(ast, functionality, global_env)
-    # global_env = {
-    #     '__name__': lang_name,
-    #     'args': language_args,
-    #     ast[0]: root_execute
-    # }
-
-    # if functionality.main:
-    #     main = [cd for cd in functionality.main if cd != None]
-    #     for cd in main: 
-    #         exec(cd, global_env)
-    # else:
-    #     global_env[RETURN_VAR] = root_execute()
-    
-    # result = global_env.get(RETURN_VAR, None)
-    # if result:
-    #     print(result, end='')
+    global_env = {
+        '__name__': lang_name,
+        'args': language_args,
+    }
+    execute_func = get_execute_func(serl_ast, code, global_env)
+    sys.setrecursionlimit(10000)
+    try:
+        if main_code:
+            global_env[serl_ast[0]] = execute_func
+            result = exec_or_error(main_code[0], 0, main_code[1], global_env)
+        else:
+            result = execute_func()
+    except SyntaxError as err:
+        err.__traceback__ = None
+        err.__context__ = None
+        err.__notes__ = None
+        err.filename = getattr(err, EXCEPTION_ATTR, '')
+        logger.error(f'In {err.filename}:\n\n', exc_info=True, code=1)
+    except subprocess.CalledProcessError as err:
+        err.__notes__ = None
+        filename = getattr(err, EXCEPTION_ATTR, '')
+        logger.error(f'In {filename}:\n\n{err.stderr}',code=err.returncode)
+    except Exception as err:
+        filename_re = r'^\$\.code\.(.*?)\[(\d+)\]$'
+        frames = traceback.extract_tb(err.__traceback__)
+        frame = next((frame for frame in frames[::-1] 
+                        if re.match(filename_re, frame.filename)), frames[-1])
+        name, i = re.match(filename_re, frame.filename).groups()
+        i = int(i)
+        lineno = frame.lineno
+        err.__traceback__ = None
+        err.__context__ = None
+        code_lines = code[name][i].split('\n')
+        code_line = code_lines[lineno - 1]
+        err.__notes__ = None
+        err_msg = f'In {frame.filename}, line {lineno}:\n\n{code_line}\n\n'
+        logger.error(err_msg, exc_info=True, code=1)
+
+    if result:
+        print(result)
+
+def exec_and_eval(name, i, code, global_env, local_env=None):
+    filename = f'$.code.{name}[{i}]'
+    code_ast = ast.parse(code)
+
+    try:
+        last_stmt = code_ast.body.pop()
+        expr = ast.Expression(last_stmt.value)
+    except AttributeError:
+        return exec(compile(ast.parse(code), filename, mode='exec'), 
+                    global_env, local_env)
+    except IndexError:
+        return None
+
+    exec(compile(code_ast, filename, mode='exec'), global_env, local_env)
+    return eval(compile(expr, filename, mode='eval'), global_env, local_env)
+
+def run_command(command: str, env: dict):
+    command = command.format_map(TraversableFormat(**env))
+    return subprocess.run(command, capture_output=True, text=True, shell=True, 
+                          check=True).stdout
+
+def exec_or_error(name, i, code_str, global_env, local_env=None):
+    try:
+        if code_str.startswith(SHELL_CHAR):
+            local_env = local_env or {}
+            local_env = {'locals()': local_env} | local_env
+            return run_command(code_str[1:], global_env | local_env)
+        else:
+            return exec_and_eval(name, i, code_str, global_env, local_env)
+    except Exception as err:
+        if not getattr(err, EXCEPTION_ATTR, None):
+            setattr(err, EXCEPTION_ATTR, f'$.code.{name}[{i}]')
+        raise
 
-def get_execute_func(ast: AST, functionality: Functionality, global_env: dict):
-    name, i, value = ast
+def get_execute_func(serl_ast: SerlAST, code: dict, global_env: dict):
+    name, i, value = serl_ast
     env = {}
     for k, v in value.items():
-        if isinstance(v, list):
-            env[k] = [get_execute_func(e, functionality, global_env) 
-                      if isinstance(e, AST) else e for e in v]
-        else:
-            exec_func = get_execute_func(v, functionality, global_env)
-            env[k] = exec_func if isinstance(v, AST) else v
+        env[k] = [get_execute_func(e, code, global_env) 
+                  if isinstance(e, SerlAST) else e for e in v]
+        env[k] = env[k][0] if len(env[k]) == 1 else env[k]
     
     active = True
     def execute(**local_env):
         # Make sure the function can only be called once
         nonlocal active
         if not active:
             return None
         active = False
 
-        cd = functionality.get_code(name, i)
-        cm = functionality.get_command(name, i)
-        if cd:
-            local_env |= env
-            exec(cd, global_env, local_env)
-            return local_env.get(RETURN_VAR, None)
-        elif cm:
-            # TODO add global and local vars to env TODO how to invoke code/command of child nonterminals
-            env = os.environ.copy() | {}
-            return subprocess.run(cm, capture_output=True, text=True, 
-                                  shell=True, env=env, check=True).stdout
-        else:
-            return env
-    return execute
+        code_list = code.get(name, None)
+        code_str = code_list[i] if code_list and len(code_list) > i else None
+        
+        if not code_str:
+            return env # TODO should 'None' be returned?
+
+        return exec_or_error(name, i, code_str, global_env, local_env | env)
+    
+    return Traversable(execute)
 
-def install_command(args):
+def command_line_install(args):
     language = args['<language>']
     alias = args['<alias>'] or utils.get_language_name(language)
     upgrade = args['--upgrade']
     
-    config_text = get_config_text(language)
+    config_text = get_config_text(language, False)
     config_dir = get_config_dir()
     filename = os.path.join(config_dir, alias)
     
     if os.path.isfile(filename) and not upgrade:
         logger.error(f'Language \'{alias}\' already exists. '
-                     f'Use -U or --upgrade to override.')
+                     f'Use -U or --upgrade to override.', code=1)
     
     with open(filename, 'w') as file:
         file.write(config_text)
     print(f'Successfully installed \'{alias}\'.')
 
-def uninstall_command(args: dict):
+def command_line_uninstall(args: dict):
     languages = args['<language>']
     envs = args['<env>']
     remove_venv = args['--venv']
     remove, files, prefix = os.remove, languages, get_config_dir()
     if remove_venv:
         remove, files, prefix = shutil.rmtree, envs, get_config_env_dir()
     
@@ -320,17 +416,24 @@
         try:
             remove(path)
             print(f'Successfully uninstalled \'{file}\'.')
         except FileNotFoundError:
             logger.warning(f'Skipping \'{file}\' as it is not already '
                            f'installed.')  
 
-def list_command(args):
+def command_line_list(args):
     languages = system_config_languages()
-    envs = os.listdir(get_config_env_dir())
+    config_env_dir = get_config_env_dir() + os.sep
+    glob_path = os.path.join(config_env_dir, '**', VENV_CONFIG)
+    envs = glob.glob(glob_path, recursive=True)
+    envs = [
+        str(pathlib.Path(path).parent.resolve()).removeprefix(config_env_dir) 
+        for path in envs
+    ]
+    
     files, name = languages, 'languages'
     if args['--venv']:
         files, name = envs, 'environments'
     
     if files == []:
         print(f'No {name} installed.')
     else:
@@ -365,22 +468,29 @@
     
     if command == 'help':
         print(CLI_COMMANDS.get(args['<command>'], CLI))
         exit(0)
     
     return base_args, args
 
+def get_link_filename() -> None | str:
+    filename = extension(sys.argv[0])
+    return filename if os.path.islink(filename) else None
+
 def main():
     version = f'{NAME} {VERSION}'
-    filename = extension(sys.argv[0])
+    filename = get_link_filename()
 
-    if os.path.islink(filename):
+    if filename:
         base_args, args = get_symlink_args(filename, version)
     else:
         base_args, args = get_args(version)
 
     logger.verbose = base_args.get('--verbose', False) or \
         args.get('--verbose', False)
-    logger.strict = base_args.get('--strict', False) or \
-        args.get('--strict', False)
-
-    globals()[f"{base_args['<command>']}_command"](args)
+    
+    try:
+        globals()[f'command_line_{base_args["<command>"]}'](args)
+    except Exception:
+        if not logger.error_seen:
+            raise
+        exit(1)
```

### Comparing `serl-0.0.2a0/src/serl/schema.py` & `serl-0.1.0b0/src/serl/schema.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from typing import Tuple
 import jsonschema
 
 meta = {
     'type': 'object',
     'properties': {
         'tokens': {
             'type': 'object',
@@ -11,32 +10,30 @@
                     'type': ['string', 'null']
                 },
                 'regex': {
                     'type': 'boolean'
                 },
                 'ignore': {
                     'type': ['string', 'null']
+                },
+                'flags': {
+                    'type': 'string'
+                },
+                'default': {
+                    'type': 'boolean'
                 }
             }
         },
         'grammar': {
             'type': 'object',
             'properties': {
                 'permissive': {
                     'type': 'boolean'
                 }
             }
-        },
-        'commands': {
-            'type': 'object',
-            'properties': {
-                'prefix': {
-                    'type': 'string'
-                }
-            }
         }
     }
 }
 
 config_schema = {
     'type': 'object',
     'properties': {
@@ -57,15 +54,15 @@
         },
         'precedence': {
             'type': 'array',
             'items': {
                 'type': 'string'
             }
         },
-        'sync': {
+        'error': {
             'type': 'string'
         },
         'grammar': {
             'type': 'object',
             'patternProperties': {
                 '^.*$': {
                     'type': ['string', 'array'],
@@ -82,25 +79,14 @@
                     'type': ['string', 'array'],
                     'items': {
                         'type': ['string', 'null']
                     }
                 }
             },
         },
-        'commands': {
-            'type': 'object',
-            'patternProperties': {
-                '^.*$': {
-                    'type': ['string', 'array'],
-                    'items': {
-                        'type': ['string', 'null']
-                    }
-                }
-            },
-        },
         'tokentypes': { # TODO might rename
             'type': 'object',
             'patternProperties': {
                 '^.*$': {
                     'type': 'string',
                 }
             },
@@ -116,21 +102,14 @@
         'environment': {
             'type': 'string'
         },
         'requirements': {
             'type': 'string'
         }
     },
-    'anyOf': [
-        {'required': ['tokens', 'grammar', 'code']},
-        {'required': ['tokens', 'grammar', 'commands']},
-    ]
-    
+    'required': ['grammar', 'code'] 
 }
 
-def validate(config: dict) -> Tuple[bool, str]:
-    try:
-        jsonschema.validate(config, config_schema)
-    except jsonschema.exceptions.ValidationError as ve:
-        error = f'{ve.message} for key \'{".".join(ve.absolute_path)}\'.'
-        return False, error
-    return True, ''
+def validate(config: dict) -> list[str]:
+    validator = jsonschema.Draft202012Validator(config_schema)
+    errs = validator.iter_errors(config)
+    return [f'{err.message} for \'{err.json_path}\'.' for err in errs]
```

### Comparing `serl-0.0.2a0/src/serl/utils.py` & `serl-0.1.0b0/src/serl/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-import re, os
-from typing import Callable
+import re
+import os
+from typing import Callable, Iterable
 
 def expand(rule: str, symbol_map: list[tuple[str, str]], 
            symbol_f: Callable[[str], str] = lambda x: x, 
            repl_f: Callable[[str], str] = lambda x: x):
     if symbol_map == []:
         return rule
     symbol, repl = symbol_map[0]
@@ -44,57 +45,70 @@
         exp_repl_tokens[exp_tok] = expand(exp_repl_tokens[exp_tok], 
                                           sorted_repl_tokens)
     return exp_repl_tokens
 
 def normalise_dict(d: dict) -> dict[str, list[str]]:
     return {k:v if type(v) == list else [v] for k,v in d.items()}
 
+def expand_grammar_rule(rule, sorted_symbol_map):
+    exp_rule = expand(rule, sorted_symbol_map, re.escape, lambda x: f' {x} ')
+    return re.sub(r'\s+', ' ', exp_rule).strip()
+
 def normalise_grammar(symbol_map: dict[str, str],
                       grammar: dict) -> dict[str, list[str]]:
     sorted_symbol_map = list(get_sorted_map(symbol_map).items())
     norm_grammar = {}
     for nt, rules in normalise_dict(grammar).items():       
         for i, rule in enumerate(rules):
-            exp_rule = expand(rule, sorted_symbol_map, re.escape, lambda x: f' {x} ')
-            rules[i] = re.sub(r'\s+', ' ', exp_rule).strip()
+            rules[i] = expand_grammar_rule(rule, sorted_symbol_map)
         norm_grammar[symbol_map[nt]] = rules
     return norm_grammar
 
-def get_tokens_in_grammar(token_map: dict[str, str], 
-                          norm_grammar: dict[str, list[str]]) -> list[str]:
+def get_tokens_in_grammar(token_map: dict[str, str], error: str,
+                          norm_grammar: dict[str, list[str]]):
     tokens = list(token_map.values())
-    rules = [rule for rules in norm_grammar.values() for rule in rules]
-    used = set()
-    for rule in rules:
-        for token in tokens:
-            if re.search(fr'\b{token}\b', rule):
-                rule = re.sub(fr'\b{token}\b', '', rule)
-                used.add(token)
-    return [token for token, token_name in token_map.items() 
-            if token_name in used]
-
-def get_dups(d1: dict[str, list[str]], 
-             d2: dict[str, list[str]]) -> list[tuple[str, int]]:
-    dups = []
-    for k, v1 in d1.items():
-        v2 = d2.get(k, None)
-        if v2:
-            l = min(len(v1), len(v2))
-            v1, v2 = v1[:l], v2[:l]
-            dups += [(k, i) for i in range(l) 
-                     if type(v1[i]) == type(v2[i]) and type(v1[i]) == str]
-    return dups
+    nonterms = norm_grammar.keys()
+    flipped_token_map = flip_dict(token_map)
+    
+    tokens_used, implicit_map = set(), dict()
+    for nt, rules in norm_grammar.items():
+        for i, rule in enumerate(rules):
+            new_rule = ''
+            for symbol in rule.split(' '):
+                if symbol in tokens:
+                    tokens_used.add(flipped_token_map[symbol])
+                elif symbol in nonterms:
+                    pass
+                elif symbol == error:
+                    symbol = 'error'
+                else:
+                    if not implicit_map.get(symbol, None):
+                        implicit_map[symbol] = f'ITERMINAL{len(implicit_map)}'
+                    symbol = implicit_map[symbol]
+                new_rule += f'{symbol} '
+            norm_grammar[nt][i] = new_rule.strip()
+    # Order implicit tokens by length
+    return list(tokens_used), get_sorted_map(implicit_map)
 
 def flip_dict(d: dict) -> dict:
     return {v: k for k, v in d.items()}
 
 def get_language_name(language: str):
     name, ext = os.path.splitext(os.path.basename(language))
     return name
 
-def filter_dict_keys(d: dict, l: list[str]):
-    return {k: v for k, v in d.items() if k in l}
+def keep_keys_in_list(d: dict, i: Iterable):
+    return {k: v for k, v in d.items() if k in i}
 
-def get_valid_identifier(s):
+def get_valid_identifier(s: str):
    s = re.sub('[^0-9a-zA-Z_]', '', s)
    s = re.sub('^[^a-zA-Z_]+', '', s)
-   return s
+   return s
+
+def get_main_code(
+        code: dict[str, list[str]], grammar_map: dict[str, str]
+    ) -> tuple[str, str] | None:
+    item = next(iter(code.items()), None)
+    if item:
+        return None if item[0] in grammar_map else (item[0], next(iter(item[1]), None))
+    else:
+        return None
```

### Comparing `serl-0.0.2a0/src/serl.egg-info/PKG-INFO` & `serl-0.1.0b0/src/serl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: serl
-Version: 0.0.2a0
+Version: 0.1.0b0
 Summary: Serialized Language (serl)
 Author: Harry Downing
 Author-email: harry.downing17@gmail.com
+License: MIT
 Project-URL: repository, https://github.com/harrydowning/serl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Serialized Language (serl)
-Serl is a command line tool used to manage and execute complete languages serialized with YAML.
+Serl is a command line tool used to manage and execute programming languages serialized with YAML.
 
 ### Development Workflow
 | Command | Description |
 | ------- | ----------- |
 | `pip install .` | Build/install locally |
 | `serl help` | Show the tool command line help screen |
 | `pytest tests` or `test.bat` | Run automated test suite |
```

### Comparing `serl-0.0.2a0/src/serl.egg-info/SOURCES.txt` & `serl-0.1.0b0/src/serl.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -15,11 +15,14 @@
 src/serl/utils.py
 src/serl.egg-info/PKG-INFO
 src/serl.egg-info/SOURCES.txt
 src/serl.egg-info/dependency_links.txt
 src/serl.egg-info/entry_points.txt
 src/serl.egg-info/requires.txt
 src/serl.egg-info/top_level.txt
+tests/test_config.py
 tests/test_highlight.py
+tests/test_lexer.py
 tests/test_main.py
+tests/test_parser.py
 tests/test_schema.py
 tests/test_utils.py
```

### Comparing `serl-0.0.2a0/tests/test_highlight.py` & `serl-0.1.0b0/tests/test_highlight.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,13 +8,13 @@
      {'key1': 'value1, key2', 'key3': 'value3', 'key4': 'key, value='}),
     ('key1=value1, key2', {'key1': 'value1', 'key2': True}),
     ('key1, key2, key3', {'key1': True, 'key2': True, 'key3': True}),
     ('key1=["list", "of", \'strings\'], key2=value2', 
      {'key1': ['list', 'of', 'strings'], 'key2': 'value2'})
 ]
 
-@pytest.mark.parametrize("input, expected", test_data, 
+@pytest.mark.parametrize('input, expected', test_data, 
                          ids=[f'input{i}' for i in range(len(test_data))])
 def test_parse_key_value(input, expected):
     actual = highlight.parse_key_value(input)
     assert actual == expected
```

### Comparing `serl-0.0.2a0/tests/test_schema.py` & `serl-0.1.0b0/tests/test_schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,84 +8,95 @@
     usage: string
     tokens:
         token: string
     grammar:
         rule: string
     code:
         rule: string
-    """, True),
+    """, []),
     ("""
     version: 1
     usage: string
     tokens:
         token: string
     grammar:
         rule: string
     code:
         rule: string
-    """, True),
+    """, []),
     ("""
     usage: string
     tokens:
         token: string
     grammar:
         rule: string
     code:
         rule: string
-    """, True),
+    """, []),
     ("""
     version: string
     tokens:
         token: string
     grammar:
         rule: string
     code:
         rule: string
-    """, True),
+    """, []),
     ("""
     tokens:
         token: string
     grammar:
         rule: string
     code:
         rule: string
-    """, True),
+    """, []),
     ("""
     tokens:
-        _ignore: string
+        token: string
     grammar:
         rule: string
     code:
         rule: string
-    """, True),
+    Notes: string
+    """, []),
     ("""
     version: string
     usage: string
     grammar:
         rule: string
     code:
         rule: string
-    """, False),
+    """, []),
     ("""
     version: string
     usage: string
     tokens:
         token: string
     code:
         rule: string
-    """, False),
+    """, ['']),
     ("""
     version: string
     usage: string
     tokens:
         token: string
     grammar:
         rule: string
-    """, False),
+    """, ['']),
+    ("""
+    version: string
+    usage: string
+    tokens:
+        token: string
+    grammar:
+        rule: string
+    code:
+        rule: [1,2,3,4,5,6,7,8,9,10]
+    """, [''] * 10),
 ]
 
 @pytest.mark.parametrize("test_config, expected", test_data, 
                          ids=[f'config{i}' for i in range(len(test_data))])
 def test_validate(test_config, expected):
     config = yaml.safe_load(test_config)
-    valid, _ = schema.validate(config)
-    assert valid == expected
+    errs = schema.validate(config)
+    assert len(errs) == len(expected)
```

