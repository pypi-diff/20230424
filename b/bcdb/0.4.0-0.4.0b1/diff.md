# Comparing `tmp/bcdb-0.4.0.tar.gz` & `tmp/bcdb-0.4.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcdb-0.4.0.tar", last modified: Mon Apr 24 13:16:12 2023, max compression
+gzip compressed data, was "bcdb-0.4.0b1.tar", last modified: Fri Dec  9 19:39:39 2022, max compression
```

## Comparing `bcdb-0.4.0.tar` & `bcdb-0.4.0b1.tar`

### file list

```diff
@@ -1,20 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 13:16:12.897502 bcdb-0.4.0/
--rw-rw-rw-   0        0        0    33094 2022-11-11 13:51:17.000000 bcdb-0.4.0/LICENSE
--rw-rw-rw-   0        0        0     3860 2023-04-24 13:16:12.898503 bcdb-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     2883 2023-03-19 15:10:06.000000 bcdb-0.4.0/README.md
--rw-rw-rw-   0        0        0      910 2023-02-25 14:02:23.000000 bcdb-0.4.0/pyproject.toml
--rw-rw-rw-   0        0        0     1296 2023-04-24 13:16:12.903506 bcdb-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0       73 2022-11-11 13:49:17.000000 bcdb-0.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:16:12.864503 bcdb-0.4.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-24 13:16:12.881505 bcdb-0.4.0/src/bcdb/
--rw-rw-rw-   0        0        0    43483 2023-04-24 13:13:11.000000 bcdb-0.4.0/src/bcdb/__init__.py
--rw-rw-rw-   0        0        0        0 2022-11-11 13:49:17.000000 bcdb-0.4.0/src/bcdb/py.typed
-drwxrwxrwx   0        0        0        0 2023-04-24 13:16:12.894503 bcdb-0.4.0/src/bcdb.egg-info/
--rw-rw-rw-   0        0        0     3860 2023-04-24 13:16:12.000000 bcdb-0.4.0/src/bcdb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-04-24 13:16:12.000000 bcdb-0.4.0/src/bcdb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 13:16:12.000000 bcdb-0.4.0/src/bcdb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-11-12 19:23:06.000000 bcdb-0.4.0/src/bcdb.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       25 2023-04-24 13:16:12.000000 bcdb-0.4.0/src/bcdb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-24 13:16:12.000000 bcdb-0.4.0/src/bcdb.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-24 13:16:12.896503 bcdb-0.4.0/tests/
--rw-rw-rw-   0        0        0    37265 2023-02-23 18:52:00.000000 bcdb-0.4.0/tests/test_bcdb.py
+drwxrwxrwx   0        0        0        0 2022-12-09 19:39:39.183036 bcdb-0.4.0b1/
+-rw-rw-rw-   0        0        0    33094 2022-11-11 13:51:17.000000 bcdb-0.4.0b1/LICENSE
+-rw-rw-rw-   0        0        0     3360 2022-12-09 19:39:39.183036 bcdb-0.4.0b1/PKG-INFO
+-rw-rw-rw-   0        0        0     2883 2022-11-16 19:52:59.000000 bcdb-0.4.0b1/README.md
+-rw-rw-rw-   0        0        0      134 2022-11-17 16:50:59.000000 bcdb-0.4.0b1/pyproject.toml
+-rw-rw-rw-   0        0        0      851 2022-12-09 19:39:39.188024 bcdb-0.4.0b1/setup.cfg
+-rw-rw-rw-   0        0        0       73 2022-11-11 13:49:17.000000 bcdb-0.4.0b1/setup.py
+drwxrwxrwx   0        0        0        0 2022-12-09 19:39:39.153116 bcdb-0.4.0b1/src/
+drwxrwxrwx   0        0        0        0 2022-12-09 19:39:39.169073 bcdb-0.4.0b1/src/bcdb/
+-rw-rw-rw-   0        0        0    41028 2022-12-09 19:38:55.000000 bcdb-0.4.0b1/src/bcdb/__init__.py
+-rw-rw-rw-   0        0        0        0 2022-11-11 13:49:17.000000 bcdb-0.4.0b1/src/bcdb/py.typed
+drwxrwxrwx   0        0        0        0 2022-12-09 19:39:39.182038 bcdb-0.4.0b1/src/bcdb.egg-info/
+-rw-rw-rw-   0        0        0     3360 2022-12-09 19:39:39.000000 bcdb-0.4.0b1/src/bcdb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2022-12-09 19:39:39.000000 bcdb-0.4.0b1/src/bcdb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-12-09 19:39:39.000000 bcdb-0.4.0b1/src/bcdb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-11-12 19:23:06.000000 bcdb-0.4.0b1/src/bcdb.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        5 2022-12-09 19:39:39.000000 bcdb-0.4.0b1/src/bcdb.egg-info/top_level.txt
```

### Comparing `bcdb-0.4.0/LICENSE` & `bcdb-0.4.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `bcdb-0.4.0/PKG-INFO` & `bcdb-0.4.0b1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,22 @@
 Metadata-Version: 2.1
 Name: bcdb
-Version: 0.4.0
+Version: 0.4.0b1
 Summary: Black Cat DataBase is a simple database.
 Home-page: https://github.com/koviubi56/bcdb
 Author: Koviubi56
 Author-email: koviubi56@duck.com
 License: GPL
 Keywords: db,database
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
 Platform: win32
-Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Database
-Classifier: Typing :: Typed
-Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Black Cat DataBase
 
 [![Hits-of-Code](https://hitsofcode.com/github/koviubi56/bcdb?branch=main)](https://hitsofcode.com/github/koviubi56/bcdb/view?branch=main)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/103515bdc600439d98a0f1ea1f767c71)](https://www.codacy.com/gh/koviubi56/bcdb/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=koviubi56/bcdb&amp;utm_campaign=Badge_Grade)
@@ -48,15 +37,15 @@
 
 ```bash
 pip install bcdb
 ```
 
 ## Requirements
 
-BCDB requires Python 3.11.
+BCDB requires Python 3.10.
 
 ## Usage
 
 ```python
 import bcdb
 from pathlib import Path
```

### Comparing `bcdb-0.4.0/README.md` & `bcdb-0.4.0b1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 ```bash
 pip install bcdb
 ```
 
 ## Requirements
 
-BCDB requires Python 3.11.
+BCDB requires Python 3.10.
 
 ## Usage
 
 ```python
 import bcdb
 from pathlib import Path
```

### Comparing `bcdb-0.4.0/setup.cfg` & `bcdb-0.4.0b1/setup.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -14,68 +14,41 @@
 000000d0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6b  s://github.com/k
 000000e0: 6f76 6975 6269 3536 2f62 6364 620d 0a61  oviubi56/bcdb..a
 000000f0: 7574 686f 7220 3d20 4b6f 7669 7562 6935  uthor = Koviubi5
 00000100: 360d 0a61 7574 686f 725f 656d 6169 6c20  6..author_email 
 00000110: 3d20 6b6f 7669 7562 6935 3640 6475 636b  = koviubi56@duck
 00000120: 2e63 6f6d 0d0a 6c69 6365 6e73 6520 3d20  .com..license = 
 00000130: 4750 4c0d 0a6c 6963 656e 7365 5f66 696c  GPL..license_fil
-00000140: 6573 203d 204c 4943 454e 5345 0d0a 706c  es = LICENSE..pl
-00000150: 6174 666f 726d 7320 3d20 756e 6978 2c20  atforms = unix, 
-00000160: 6c69 6e75 782c 206f 7378 2c20 6379 6777  linux, osx, cygw
-00000170: 696e 2c20 7769 6e33 320d 0a63 6c61 7373  in, win32..class
-00000180: 6966 6965 7273 203d 200d 0a09 4465 7665  ifiers = ...Deve
-00000190: 6c6f 706d 656e 7420 5374 6174 7573 203a  lopment Status :
-000001a0: 3a20 3320 2d20 416c 7068 610d 0a09 4c69  : 3 - Alpha...Li
-000001b0: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
-000001c0: 726f 7665 6420 3a3a 2047 4e55 2047 656e  roved :: GNU Gen
-000001d0: 6572 616c 2050 7562 6c69 6320 4c69 6365  eral Public Lice
-000001e0: 6e73 6520 7633 206f 7220 6c61 7465 7220  nse v3 or later 
-000001f0: 2847 504c 7633 2b29 0d0a 094e 6174 7572  (GPLv3+)...Natur
-00000200: 616c 204c 616e 6775 6167 6520 3a3a 2045  al Language :: E
-00000210: 6e67 6c69 7368 0d0a 094f 7065 7261 7469  nglish...Operati
-00000220: 6e67 2053 7973 7465 6d20 3a3a 204f 5320  ng System :: OS 
-00000230: 496e 6465 7065 6e64 656e 740d 0a09 5072  Independent...Pr
-00000240: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000250: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000260: 330d 0a09 5072 6f67 7261 6d6d 696e 6720  3...Programming 
-00000270: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000280: 6f6e 203a 3a20 3320 3a3a 204f 6e6c 790d  on :: 3 :: Only.
-00000290: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-000002a0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-000002b0: 203a 3a20 332e 3131 0d0a 0950 726f 6772   :: 3.11...Progr
-000002c0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000002d0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
-000002e0: 320d 0a09 5072 6f67 7261 6d6d 696e 6720  2...Programming 
-000002f0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000300: 6f6e 203a 3a20 496d 706c 656d 656e 7461  on :: Implementa
-00000310: 7469 6f6e 203a 3a20 4350 7974 686f 6e0d  tion :: CPython.
-00000320: 0a09 546f 7069 6320 3a3a 2044 6174 6162  ..Topic :: Datab
-00000330: 6173 650d 0a09 5479 7069 6e67 203a 3a20  ase...Typing :: 
-00000340: 5479 7065 640d 0a6b 6579 776f 7264 7320  Typed..keywords 
-00000350: 3d20 6462 2c20 6461 7461 6261 7365 0d0a  = db, database..
-00000360: 0d0a 5b6f 7074 696f 6e73 5d0d 0a70 6163  ..[options]..pac
-00000370: 6b61 6765 7320 3d20 0d0a 0962 6364 620d  kages = ...bcdb.
-00000380: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
-00000390: 7320 3d20 0d0a 0974 7970 696e 675f 6578  s = ...typing_ex
-000003a0: 7465 6e73 696f 6e73 3e3d 342e 302e 300d  tensions>=4.0.0.
-000003b0: 0a70 7974 686f 6e5f 7265 7175 6972 6573  .python_requires
-000003c0: 203d 203e 3d33 2e31 310d 0a70 6163 6b61   = >=3.11..packa
-000003d0: 6765 5f64 6972 203d 200d 0a09 3d73 7263  ge_dir = ...=src
-000003e0: 0d0a 7a69 705f 7361 6665 203d 206e 6f0d  ..zip_safe = no.
-000003f0: 0a0d 0a5b 6f70 7469 6f6e 732e 7061 636b  ...[options.pack
-00000400: 6167 655f 6461 7461 5d0d 0a62 6364 6220  age_data]..bcdb 
-00000410: 3d20 7079 2e74 7970 6564 0d0a 0d0a 5b70  = py.typed....[p
-00000420: 7963 6f64 6573 7479 6c65 5d0d 0a69 676e  ycodestyle]..ign
-00000430: 6f72 6520 3d20 4532 3033 0d0a 0d0a 5b70  ore = E203....[p
-00000440: 796c 616d 615d 0d0a 6967 6e6f 7265 203d  ylama]..ignore =
-00000450: 2057 3530 330d 0a0d 0a5b 666c 616b 6538   W503....[flake8
-00000460: 5d0d 0a65 7874 656e 642d 6967 6e6f 7265  ]..extend-ignore
-00000470: 203d 2057 3530 332c 5331 3031 0d0a 6578   = W503,S101..ex
-00000480: 7465 6e64 2d65 7863 6c75 6465 203d 2076  tend-exclude = v
-00000490: 656e 762c 2a63 6163 6865 2a0d 0a0d 0a5b  env,*cache*....[
-000004a0: 6973 6f72 745d 0d0a 7072 6f66 696c 6520  isort]..profile 
-000004b0: 3d20 626c 6163 6b0d 0a0d 0a5b 746f 6f6c  = black....[tool
-000004c0: 3a70 7974 6573 745d 0d0a 6661 756c 7468  :pytest]..faulth
-000004d0: 616e 646c 6572 5f74 696d 656f 7574 203d  andler_timeout =
-000004e0: 2035 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d   5....[egg_info]
-000004f0: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
-00000500: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
+00000140: 6520 3d20 4c49 4345 4e53 450d 0a70 6c61  e = LICENSE..pla
+00000150: 7466 6f72 6d73 203d 2075 6e69 782c 206c  tforms = unix, l
+00000160: 696e 7578 2c20 6f73 782c 2063 7967 7769  inux, osx, cygwi
+00000170: 6e2c 2077 696e 3332 0d0a 636c 6173 7369  n, win32..classi
+00000180: 6669 6572 7320 3d20 4c69 6365 6e73 6520  fiers = License 
+00000190: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
+000001a0: 3a3a 2047 4e55 2047 656e 6572 616c 2050  :: GNU General P
+000001b0: 7562 6c69 6320 4c69 6365 6e73 6520 7633  ublic License v3
+000001c0: 206f 7220 6c61 7465 7220 2847 504c 7633   or later (GPLv3
+000001d0: 2b29 0d0a 6b65 7977 6f72 6473 203d 2064  +)..keywords = d
+000001e0: 622c 2064 6174 6162 6173 650d 0a0d 0a5b  b, database....[
+000001f0: 6f70 7469 6f6e 735d 0d0a 7061 636b 6167  options]..packag
+00000200: 6573 203d 200d 0a09 6263 6462 0d0a 7061  es = ...bcdb..pa
+00000210: 636b 6167 655f 6469 7220 3d20 0d0a 093d  ckage_dir = ...=
+00000220: 7372 630d 0a7a 6970 5f73 6166 6520 3d20  src..zip_safe = 
+00000230: 6e6f 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  no....[options.p
+00000240: 6163 6b61 6765 5f64 6174 615d 0d0a 6263  ackage_data]..bc
+00000250: 6462 203d 2070 792e 7479 7065 640d 0a0d  db = py.typed...
+00000260: 0a5b 7079 636f 6465 7374 796c 655d 0d0a  .[pycodestyle]..
+00000270: 6967 6e6f 7265 203d 2045 3230 330d 0a0d  ignore = E203...
+00000280: 0a5b 7079 6c61 6d61 5d0d 0a69 676e 6f72  .[pylama]..ignor
+00000290: 6520 3d20 5735 3033 0d0a 0d0a 5b66 6c61  e = W503....[fla
+000002a0: 6b65 385d 0d0a 6578 7465 6e64 2d69 676e  ke8]..extend-ign
+000002b0: 6f72 6520 3d20 5735 3033 2c53 3130 310d  ore = W503,S101.
+000002c0: 0a65 7874 656e 642d 6578 636c 7564 6520  .extend-exclude 
+000002d0: 3d20 7665 6e76 2c2a 6361 6368 652a 0d0a  = venv,*cache*..
+000002e0: 0d0a 5b69 736f 7274 5d0d 0a70 726f 6669  ..[isort]..profi
+000002f0: 6c65 203d 2062 6c61 636b 0d0a 0d0a 5b74  le = black....[t
+00000300: 6f6f 6c3a 7079 7465 7374 5d0d 0a66 6175  ool:pytest]..fau
+00000310: 6c74 6861 6e64 6c65 725f 7469 6d65 6f75  lthandler_timeou
+00000320: 7420 3d20 350d 0a0d 0a5b 6567 675f 696e  t = 5....[egg_in
+00000330: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
+00000340: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
+00000350: 0a0d 0a                                  ...
```

### Comparing `bcdb-0.4.0/src/bcdb/__init__.py` & `bcdb-0.4.0b1/src/bcdb/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,39 +12,37 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
-__version__ = "0.4.0"
+__version__ = "0.4.0-beta.1"
 __author__ = "Koviubi56"
 __email__ = "koviubi56@duck.com"
-__license__ = "GNU GPLv3+"
+__license__ = "GNU GPLv3"
 __copyright__ = "Copyright (C) 2022 Koviubi56"
 __description__ = "Black Cat DataBase is a simple database."
 __url__ = "https://github.com/koviubi56/bcdb"
 
 import contextlib
 import dataclasses
 import enum
 import functools
 import pathlib
 import string as stringlib
 import threading
-import warnings
-from typing import Any, Callable, Collection, Generator, Generic, Iterable
+from typing import Any, Callable, Collection, Iterable
 
-from typing_extensions import Self, TypeAlias, TypeVarTuple
+from typing_extensions import Self, TypeAlias
 
 if not __debug__:
     raise Exception("BCDB cannot be used with the -O flag")
 
-Ts = TypeVarTuple("Ts")
-Where: TypeAlias = Callable[[tuple[*Ts]], bool]
+Where: TypeAlias = Callable[[tuple[Any, ...]], bool]
 
 
 def unique(iterable: Collection[Any]) -> bool:
     # v probably slower but should work
     # // seen: list[Any] = []
     # // for obj in iterable:
     # //     if obj in iterable:
@@ -53,15 +51,15 @@
     # // return True
 
     # * probably faster
     return len(iterable) == len(set(iterable))
 
 
 @dataclasses.dataclass(order=True, frozen=True)
-class Table(Generic[*Ts]):
+class Table:
     """
     A table.
 
     Args:
         file (pathlib.Path): The table file.
     """
 
@@ -101,18 +99,19 @@
             Other exceptions may be raised by other
             functions (Attribute.from_str) called by this function.
 
         Returns:
             list[Attribute]: The attributes
         """
         first_line = None
-        with self.file.open("r", encoding="utf-8") as file:
-            for line in file:
-                first_line = line
-                break
+        with self.lock:
+            with self.file.open("r", encoding="utf-8") as file:
+                for line in file:
+                    first_line = line
+                    break
         assert first_line, "invalid table file: empty"
         assert first_line.startswith(
             "BCDB "
         ), "invalid table file: doesn't start with BCDB"
         return [
             Attribute.from_str(string, self)
             for string in first_line.removeprefix("BCDB ").split(";;")
@@ -164,21 +163,21 @@
 
     def _contains(
         self, attribute_name: str, attribute_value: Any, rv_if_found: bool
     ) -> bool:
         # Internal function, please use `.contains()` and `.not_contains()`
         # instead.
         attr_idx = self.get_attribute_index(attribute_name)
-        for rownum, row in enumerate(self.get_rows_generator(), 1):
+        for rownum, row in enumerate(self.get_rows(), 2):
             try:
                 column = row[attr_idx]
             except IndexError as exc:  # pragma: no cover
                 raise AssertionError(
-                    f"invalid row {rownum} (line {rownum+1}): doesn't have a"
-                    f" column {attr_idx} (attribute {attribute_name})"
+                    f"invalid row at line {rownum}: doesn't have a column"
+                    f" {attr_idx} (attribute {attribute_name})"
                 ) from exc
             if column == attribute_value:
                 return rv_if_found
         return not rv_if_found
 
     def contains(self, attribute_name: str, attribute_value: Any) -> bool:
         """
@@ -190,16 +189,19 @@
         `not_contains` instead.
 
         Args:
             attribute_name (str): The attribute's (column's) name
             attribute_value (Any): The value to search for.
 
         Raises:
-            Exceptions may be raised by other functions (_contains) called by
-            this function.
+            AssertionError: If a row doesn't have that column
+
+            Other exceptions may be raised by other
+            functions (get_attribute_index, get_rows) called by this
+            function.
 
         Returns:
             bool: True if any rows contain `attribute_value` at the attribute
             with the name `attribute_name`, False otherwise
         """
         return self._contains(attribute_name, attribute_value, True)
 
@@ -214,147 +216,135 @@
         `contains` instead.
 
         Args:
             attribute_name (str): The attribute's (column's) name
             attribute_value (Any): The value to search for.
 
         Raises:
-            Exceptions may be raised by other functions (_contains) called by
-            this function.
+            AssertionError: If a row doesn't have that column
+
+            Other exceptions may be raised by other
+            functions (get_attribute_index, get_rows) called by this
+            function.
 
         Returns:
             bool: False if any rows contain `attribute_value` at the attribute
             with the name `attribute_name`, True otherwise
         """
         return self._contains(attribute_name, attribute_value, False)
 
-    def _contains_row(self, row: tuple[*Ts], rv_if_found: bool) -> bool:
+    def _contains_row(self, row: tuple[Any, ...], rv_if_found: bool) -> bool:
         # Internal function, please use `.contains_row()` and
         # `.not_contains_row()` instead
-        for got_row in self.get_rows_generator():
+        # sourcery skip: use-next
+        for got_row in self.get_rows():
             if got_row == row:
                 return rv_if_found
         return not rv_if_found
 
-    def contains_row(self, row: tuple[*Ts]) -> bool:
+    def contains_row(self, row: tuple[Any, ...]) -> bool:
         """
         Return True if `row` is in the table.
 
         If you would like to check only one column see `contains` instead.
 
         If you would like to check that no rows are `row` see
         `not_contains_row` instead.
 
-        Raises:
-            Exceptions may be raised by other functions (_contains_row) called
-            by this function.
-
         Args:
-            row (tuple[*Ts]): The row to look out for.
+            row (tuple[Any, ...]): The row to look out for.
 
         Returns:
             bool: True if `row` is in the table, False otherwise.
         """
         return self._contains_row(row, True)
 
-    def not_contains_row(self, row: tuple[*Ts]) -> bool:
+    def not_contains_row(self, row: tuple[Any, ...]) -> bool:
         """
         Return False if `row` is in the table.
 
         If you would like to check only one column see `not_contains` instead.
 
         If you would like to check that a row is `row` see
         `contains_row` instead.
 
-        Raises:
-            Exceptions may be raised by other functions (_contains_row) called
-            by this function.
-
         Args:
-            row (tuple[*Ts]): The row to look out for.
+            row (tuple[Any, ...]): The row to look out for.
 
         Returns:
             bool: False if `row` is in the table, True otherwise.
         """
         return self._contains_row(row, False)
 
-    def get_rows_generator(
-        self, *, lock: bool = True
-    ) -> Generator[tuple[*Ts], None, None]:
+    def get_rows(self, *, lock: bool = True) -> list[tuple[Any, ...]]:
         """
-        Yield all rows in the table.
+        Get all rows in the table.
 
         Raises:
             AssertionError: if the table file doesn't start with `BCDB `
             AssertionError: if there are too many columns on a row
             AssertionError: if there are not enough columns on a row
 
             Other exceptions may be raised by other functions
             (Attribute.convert_and_verify) called by this function.
 
         Args:
             lock (bool, optional): Acquire lock before reading the file. This
             is only changed internally, please don't use this argument.
             Defaults to True.
 
-        Yields:
-            tuple[*Ts]: A row in the table. The tuples represent rows.
-            All of the tuples have the same length.
+        Returns:
+            list[tuple[Any, ...]]: All rows in the table. This is a list of
+            tuples. The tuples represent rows. All of the tuples should have
+            the same length.
         """
         with self.lock if lock else contextlib.nullcontext():
-            first_line = True
-
-            for linenum, line in enumerate(
-                self.file.open(encoding="utf-8"), 1
-            ):
-                if first_line:
-                    assert line.startswith(
-                        "BCDB "
-                    ), "invalid table file: doesn't start with BCDB"
-                    first_line = False
-                    continue
-                line = line.rstrip("\r\n")
-                column_: list[Any] = []
-                for columnnum, column in enumerate(line.split(";;")):
-                    if columnnum >= len(self.attributes):
-                        raise AssertionError(
-                            "invalid table file: too many columns on row"
-                            f" {linenum-1} (line {linenum})"
-                        )
-                    attr = self.attributes[columnnum]
-                    column_.append(attr.convert_and_verify(column))
-                if len(column_) != len(self.attributes):
+            contents = self.file.read_text(encoding="utf-8")
+        assert contents.startswith(
+            "BCDB "
+        ), "invalid table file: doesn't start with BCDB"
+        rows = contents.splitlines()
+        rows.pop(0)  # the BCDB... line
+        rv: list[tuple[Any, ...]] = []
+        column_: list[Any] = []
+        #                      the 1st line is BCDB...
+        #                                v
+        for rownum, row in enumerate(rows, 2):
+            for columnnum, column in enumerate(row.split(";;")):
+                if columnnum >= len(self.attributes):
                     raise AssertionError(
-                        "invalid table file: invalid columns on row"
-                        f" {linenum-1} (line {linenum}), expected"
-                        f" {len(self.attributes)}, got {len(column_)}"
+                        f"invalid table file: too many columns on row {rownum}"
                     )
-                yield tuple(column_)
-
-    def get_rows(self, *, lock: bool = True) -> list[tuple[*Ts]]:
-        warnings.warn(
-            "Consider using .get_rows_generator() instead.", RuntimeWarning
-        )
-        return list(self.get_rows_generator(lock=lock))
+                attr = self.attributes[columnnum]
+                column_.append(attr.convert_and_verify(column))
+            if len(column_) != len(self.attributes):
+                raise AssertionError(
+                    f"invalid table file: invalid columns on row {rownum},"
+                    f" expected {len(self.attributes)}, got {len(column_)}"
+                )
+            rv.append(tuple(column_))
+            column_ = []
+        return rv
 
-    def add_row(self, row: tuple[*Ts], *, lock: bool = True) -> None:
+    def add_row(self, row: tuple[Any, ...], *, lock: bool = True) -> None:
         """
         Add a row to the table.
 
         Raises:
             AssertionError: if the number of columns in `row` is not correct
 
             Other exceptions may be raised by other
             functions (Attribute.verify_before_writing) called by this
             function.
 
         Args:
-            row (tuple[*Ts]): The row. Each element in the tuple
+            row (tuple[Any, ...]): The row. Each element in the tuple
             represents a column.
             lock (bool, optional): Acquire lock. Don't change this!
+            ! [WARNING] DO NOT CHANGE THIS! THIS IS ONLY USED INTERNALLY!
         """
         assert len(row) == len(self.attributes), (
             f"invalid value for table {self.name}: invalid number of columns,"
             f" expected {len(self.attributes)}, got {len(row)}"
         )
         for idx, column in enumerate(row):
             attr = self.attributes[idx]
@@ -364,227 +354,190 @@
                 txt = ";;".join(
                     str(column).replace("\n", r"\n").replace("\r", r"\r")
                     for column in row
                 )
                 file.write(f"{txt}\n")
 
     def add_rows(
-        self, rows: Iterable[tuple[*Ts]], *, lock: bool = True
+        self, rows: Iterable[tuple[Any, ...]], *, lock: bool = True
     ) -> None:
         """
         Add multiple rows (like `list.extend()`).
 
         Raises:
             AssertionError: If `self.add_row` raises
 
         Args:
-            rows (Iterable[tuple[*Ts]]): The rows. Each item (tuple) is
+            rows (Iterable[tuple[Any, ...]]): The rows. Each item (tuple) is
             one row.
             lock (bool, optional): Same as in `self.add_row`. Defaults to True.
         """
         for rownum, row in enumerate(rows):
             try:
                 self.add_row(row, lock=lock)
             except AssertionError as exc:
                 raise AssertionError(
                     f"invalid row for add_rows at index {rownum} ({row}):"
                     f" {exc}"
                 ) from exc
 
-    def remove_row(
-        self,
-        where: Where,
-        must_remove: bool = True,
-        silence_warning: bool = False,
-    ) -> bool:
+    def remove_row(self, where: Where, must_remove: bool = True) -> bool:
         """
-        Remove the *first* row where `where(row)` is truthy.
+        Remove the first row where `where(row)` is truthy.
 
         Args:
-            where (Callable[[tuple[*Ts]], bool]): A function that accepts
+            where (Callable[[tuple[Any, ...]], bool]): A function that accepts
             a tuple as a positional argument, and returns a boolean.
             must_remove (bool, optional): If this is True, and no rows were
             removed, an AssertionError will be raised. Defaults to True.
-            silence_warning (bool, optional): By default if we detect a second
-            row that matched `where(row)` then we issue a warning. If this is
-            set to True, that won't happen. Defaults to False.
 
         Raises:
             AssertionError: If `must_remove` is True and no rows were removed
 
             Other exceptions may be raised by other
-            functions (get_rows_generator, write_rows) called by this
+            functions (get_rows, write_rows) called by this
             function.
 
         Returns:
             bool: True if a row was removed, False otherwise
         """
+        rows = self.get_rows()
         changes = False
-        new_rows: list[tuple[*Ts]] = []
-        # new_rows will be populated with the rows that were NOT removed
-        for row in self.get_rows_generator():
-            if where(row):
-                if changes:
-                    if not silence_warning:
-                        warnings.warn(
-                            "There were multiple rows where `where(row)`"
-                            " was truthy. If you want to remove ALL rows where"
-                            " `where(row)` is truthy, use .remove_rows()"
-                            " instead! If you know what you are doing, then"
-                            " pass silence_warning=True to this function"
-                            " call.",
-                            RuntimeWarning,
-                            stacklevel=2,
-                        )
-                    new_rows.append(row)
-                    # here we *do* add the row to new_rows
-                else:
-                    changes = True
-                    # here we don't add the row to new_rows
+        new_rows: list[tuple[Any, ...]] = []
+        for row in rows:
+            if (not changes) and where(row):
+                # remove row
+                changes = True
             else:
+                # row stays
                 new_rows.append(row)
-                # here we *do* add the row to new_rows
         if must_remove and (not changes):
             raise AssertionError(
-                "invalid row removal: must_remove is True, but nothing matched"
-                " `where(row)`; nothing got removed. (If this is intentional,"
-                " pass must_remove=False)"
+                "invalid row removal: must_remove but nothing was removed"
             )
         if changes:
-            # ^ If nothing is removed (changes == False), don't waste time and
-            #   energy
+            # ^ If nothing is removed, don't waste time and energy
             self.write_rows(new_rows, i_know_what_im_doing=True)
         return changes
 
-    def remove_rows(
-        self, where: Where, must_remove: bool = True, *, limit: int = 1000
-    ) -> int:
+    def remove_rows(self, where: Where, *, limit: int = 1000) -> int:
         """
         Remove all rows where `where(row)` is truthy.
 
         Args:
-            where (Callable[[tuple[*Ts]], bool]): A function that accepts
+            where (Callable[[tuple[Any, ...]], bool]): A function that accepts
             a tuple as a positional argument, and returns a boolean.
-            must_remove (bool, optional): If True, an exception will be raised
-            if no rows were removed. Defaults to True.
             limit (int, optional): The limit. If the number of removed rows
             exceeds this limit, the operation will be aborted (it won't even
             start). Defaults to 1000.
 
         Raises:
             AssertionError: If the number of removed rows exceeded `limit`
 
             Other exceptions may be raised by other
-            functions (get_rows_generator, write_rows) called by this
+            functions (get_rows, write_rows) called by this
             function.
 
         Returns:
             int: The number of rows removed.
         """
+        rows = self.get_rows()
         num_of_changes = 0
-        new_rows: list[tuple[*Ts]] = []
-        # new_rows will be populated with the rows that were NOT removed
-        for row in self.get_rows_generator():
+        new_rows: list[tuple[Any, ...]] = []
+        for row in rows:
             if where(row):
+                # remove row
                 num_of_changes += 1
-                # here we don't add the row to new_rows
             else:
+                # row stays
                 new_rows.append(row)
-                # here we *do* add the row to new_rows
-        if must_remove and (num_of_changes == 0):
-            raise AssertionError(
-                "invalid rows removal: must_remove is True, but nothing"
-                " matched `where(row)`; nothing got removed. (If this is"
-                " intentional, pass must_remove=False)"
-            )
         if num_of_changes > limit:
             raise AssertionError(
                 f"invalid removal of rows: exceeded the limit ({limit}) with"
                 f" {num_of_changes} number of rows removed. Modify the limit"
-                " argument to allow big removal of rows. (The database"
-                " remained untouched)"
+                " argument to allow big removal of rows."
             )
-        if num_of_changes:
-            # ^ If nothing is removed (changes == False), don't waste time and
-            #   energy
+        if num_of_changes > 0:
+            # ^ If nothing is removed, don't waste time and energy
             self.write_rows(new_rows, i_know_what_im_doing=True)
         return num_of_changes
 
     def write_rows(
         self,
-        rows: list[tuple[*Ts]],
+        rows: list[tuple[Any, ...]],
         *,
         i_know_what_im_doing: bool = False,
         lock: bool = True,
     ) -> None:  # sourcery skip: simplify-boolean-comparison
         """
         Remove ALL rows and replace them with `rows`. Usage is discouraged!
         ! [WARNING] ONLY USE THIS IF YOU KNOW WHAT YOU ARE DOING!
 
         Raises:
             Exceptions may be raised by other functions (add_row) called by
             this function.
 
         Args:
-            rows (list[tuple[*Ts]]): The rows that will be in the file.
-            i_know_what_im_doing (bool, optional): Defaults to False.
+            rows (list[tuple[Any, ...]]): The rows that will be in the file.
+            i_know_what_im_doing (bool, optional): Must be True to use this
+            function. Defaults to False.
             lock (bool, optional): Acquire lock before reading/writing. Please
             don't change it. Defaults to True.
         """
-        assert i_know_what_im_doing is True, (
-            "You don't know what you're doing. This function REMOVES **ALL**"
-            " ROWS, then adds the new rows."
-        )
+        assert (
+            i_know_what_im_doing is True
+        ), "You don't know what you are doing."
         with self.lock if lock else contextlib.nullcontext():
             # remove ALL rows
             with self.file.open("r", encoding="utf-8") as file:
                 # get the first line ("BCDB ...")
                 first_line = file.readlines()[0]
             with self.file.open("w", encoding="utf-8") as file:
                 # and then write that to the file
                 file.write(first_line)
 
-            # [we are still in the lock, and we do lock=False], because other
+            # we are still in the lock, and we do lock=False, because other
             # operations might be waiting, but this must finish first
-            self.add_rows(rows, lock=False)
+            for row in rows:
+                self.add_row(row, lock=False)
 
     def map(  # noqa: A003
         self,
-        func: Callable[[tuple[*Ts]], tuple[*Ts] | None],
+        func: Callable[[tuple[Any, ...]], tuple[Any, ...] | None],
         *,
         write: bool = False,
-    ) -> list[tuple[*Ts]]:
+    ) -> list[tuple[Any, ...]]:
         """
         Use `func` on all rows (like the built-in `map()`).
 
         Args:
-            func (Callable[[tuple[*Ts]], tuple[*Ts]  |  None]): The
+            func (Callable[[tuple[Any, ...]], tuple[Any, ...]  |  None]): The
             function to call. It must return a tuple or None. If it returns
             None, then that row is considered to be removed (it will only be
             actually removed if `write=True`).
             write (bool, optional): Write the new values to the database. Only
             use this if you know what you are doing! Defaults to False.
 
         Raises:
             AssertionError: if the return value of `func` is a tuple, but its
             length is not the same as the number of attributes
             AssertionError: if the return value of `func` is not a tuple, and
             isn't None
 
             Other exceptions may be raised by other
-            functions (get_rows_generator, write_rows) called by this
+            functions (get_rows, write_rows) called by this
             function.
 
         Returns:
-            list[tuple[*Ts]]: The new rows
+            list[tuple[Any, ...]]: The new rows
         """
         with self.lock:
             # * the actual map part
-            new_rows: list[tuple[*Ts]] = []
-            for row in self.get_rows_generator(lock=False):
+            new_rows: list[tuple[Any, ...]] = []
+            for row in self.get_rows(lock=False):
                 new_row = func(row)
                 if new_row is None:
                     pass
                 elif isinstance(new_row, tuple):
                     assert len(new_row) == len(self.attributes), (
                         "invalid return value returned by map function:"
                         f" tuple's ({new_row}) length ({len(new_row)}) must be"
@@ -602,43 +555,43 @@
                 self.write_rows(
                     new_rows, i_know_what_im_doing=True, lock=False
                 )
             # * and return
             return new_rows
 
     def filter(  # noqa: A003
-        self, func: Callable[[tuple[*Ts]], bool], *, write: bool = False
-    ) -> list[tuple[*Ts]]:
+        self, func: Callable[[tuple[Any, ...]], bool], *, write: bool = False
+    ) -> list[tuple[Any, ...]]:
         """
         Retain rows where `func(row)` is truthy (like the built-in `filter()`).
 
         Args:
-            func (Callable[[tuple[*Ts]], bool]): The function to call. It
+            func (Callable[[tuple[Any, ...]], bool]): The function to call. It
             must return a bool. If it returns False, then that row is
             considered to be removed (it will only be actually removed if
             `write=True`).
             write (bool, optional): Write the retained values to the database.
             Only use this if you know what you are doing! Defaults to False.
 
         Raises:
             Exceptions may be raised by other functions (map) called by this
             function.
 
         Returns:
-            list[tuple[*Ts]]: The new rows
+            list[tuple[Any, ...]]: The new rows
         """
 
-        def _func(row: tuple[*Ts]) -> tuple[*Ts] | None:
+        def _func(row: tuple[Any, ...]) -> tuple[Any, ...] | None:
             return (row) if (func(row)) else (None)
 
         return self.map(_func, write=write)
 
     def get_row_where(
         self, attribute_name: str, attribute_value: Any
-    ) -> tuple[*Ts]:
+    ) -> tuple[Any, ...]:
         """
         Get the row where the column at `attribute_name` is `attribute_value`.
 
         Args:
             attribute_name (str): The attribute's (column's) name.
             attribute_value (Any): Its value.
 
@@ -646,19 +599,19 @@
             AssertionError: If there are no rows that match
             AssertionError: If there are multiple rows that match
 
             Other exceptions may be raised by other
             functions (get_attribute_index, filter) called by this function.
 
         Returns:
-            tuple[*Ts]: The row
+            tuple[Any, ...]: The row
         """
         attr_idx = self.get_attribute_index(attribute_name)
 
-        def _func(row: tuple[*Ts]) -> bool:
+        def _func(row: tuple[Any, ...]) -> bool:
             # ? for some reason mypy yells at us?
             # error: Returning Any from function declared to return "bool"
             return (  # type: ignore[no-any-return]
                 row[attr_idx] == attribute_value
             )
 
         rv = self.filter(_func)
@@ -676,15 +629,15 @@
         return rv[0]
 
     def get_rows_where(
         self,
         attribute_name: str,
         attribute_value: Any,
         allow_empty: bool = False,
-    ) -> list[tuple[*Ts]]:
+    ) -> list[tuple[Any, ...]]:
         """
         Get all rows where the column at `attribute_name` is `attribute_value`.
 
         Args:
             attribute_name (str): The attribute's (column's) name.
             attribute_value (Any): Its value.
             allow_empty (bool, optional): Allow empty results? Defaults to
@@ -693,19 +646,19 @@
         Raises:
             AssertionError: If there are no rows that match and `allow_empty`
 
             Other exceptions may be raised by other
             functions (get_attribute_index, filter) called by this function.
 
         Returns:
-            list[tuple[*Ts]]: The rows
+            list[tuple[Any, ...]]: The rows
         """
         attr_idx = self.get_attribute_index(attribute_name)
 
-        def _func(row: tuple[*Ts]) -> bool:
+        def _func(row: tuple[Any, ...]) -> bool:
             # ? for some reason mypy yells at us?
             # error: Returning Any from function declared to return "bool"
             return (  # type: ignore[no-any-return]
                 row[attr_idx] == attribute_value
             )
 
         rv = self.filter(_func)
@@ -731,32 +684,32 @@
             `attribute.name`
             AssertionError: if a row doesn't have a column with that
             attribute (corrupted table file?)
             AssertionError: if `obj` doesn't exist in the other table
 
             Other exceptions may be raised by other
             functions (get_attribute, Attribute.check_from, __post_init__,
-            get_rows_generator) called by this function.
+            get_rows) called by this function.
         """
         if isinstance(attribute, str):
             attribute = self.get_attribute(attribute)
         if not attribute.from_:
             return
         table_file = attribute.check_from()
         attr_idx = self.attributes.index(attribute)
         from_table = self.__class__(table_file)
         from_table.get_attribute(attribute.name)
-        for rownum, row in enumerate(from_table.get_rows_generator(), 1):
+        for idx, row in enumerate(from_table.get_rows(), 2):
             try:
                 if row[attr_idx] == obj:
                     break
             except IndexError as exc:  # pragma: no cover
                 raise AssertionError(
                     f"invalid table file: no column {attr_idx + 1} at row"
-                    f" {rownum} (line {rownum+1})"
+                    f" {idx}"
                 ) from exc
         else:  # no break
             raise AssertionError(
                 f"invalid value for attribute {attribute.name}: {obj!r} does"
                 f" not exist in from table {from_table.name}"
             )
 
@@ -786,26 +739,26 @@
             which_column = self.attributes.index(attribute)
         except ValueError as exc:
             raise AssertionError(
                 f"invalid table file: cannot find attribute {attribute.name}"
                 f" within table {self.name}"
             ) from exc
         if attribute.requirements == AttributeRequirements.UNIQUE:
-            for rownum, row in enumerate(self.get_rows_generator(), 1):
+            for idx, row in enumerate(self.get_rows()):
                 try:
                     if row[which_column] == obj:
                         raise AssertionError(
                             f"invalid value at attribute {attribute.name}:"
                             " attribute is unique, but it already appears on"
-                            f" row {rownum} (line {rownum + 1})"
+                            f" row {idx + 2}"
                         )
                 except IndexError as exc:  # pragma: no cover
                     raise AssertionError(
-                        f"invalid table file: row {rownum} (line {rownum + 1})"
-                        f" doesn't have column {which_column + 1}"
+                        f"invalid table file: row {idx + 2} doesn't have"
+                        f" column {which_column + 1}"
                     ) from exc
         else:  # pragma: no cover
             raise AssertionError(
                 f"invalid table file: unknown requirement"
                 f" {attribute.requirements!r}"
             )
 
@@ -974,18 +927,15 @@
                 return True
             if string.lower() == "false":
                 return False
             raise AssertionError(
                 f"invalid table file: {string!r} isn't boolean"
             )
         if self.type_ == AttributeType.FLOAT:
-            assert "." in string, (
-                f"invalid table file: {string!r} isn't float (if it's a whole"
-                ' number, then add ".0")'
-            )
+            assert "." in string, f"invalid table file: {string!r} isn't float"
             return float(string)
         if self.type_ == AttributeType.INTEGER:
             assert (
                 "." not in string
             ), f"invalid table file: {string!r} isn't integer"
             return int(string)
         if self.type_ == AttributeType.STRING:
@@ -1102,15 +1052,15 @@
         Returns:
             Table: The new table.
         """
         assert isinstance(self.directory, pathlib.Path)
         assert all(
             val in stringlib.ascii_letters + stringlib.digits
             for val in table_name
-        ), f"invalid table name: {table_name!r} (must match [a-zA-Z1-9])"
+        ), f"invalid table name: {table_name!r}"
         assert all(isinstance(val, Attribute) for val in table_attributes), (
             "invalid table attribute: must be a list of Attribute, got"
             f" {table_attributes!r}"
         )
         assert table_attributes, "invalid table attributes: empty"
         assert unique(
             self.tables + [table_name]
```

### Comparing `bcdb-0.4.0/src/bcdb.egg-info/PKG-INFO` & `bcdb-0.4.0b1/src/bcdb.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,22 @@
 Metadata-Version: 2.1
 Name: bcdb
-Version: 0.4.0
+Version: 0.4.0b1
 Summary: Black Cat DataBase is a simple database.
 Home-page: https://github.com/koviubi56/bcdb
 Author: Koviubi56
 Author-email: koviubi56@duck.com
 License: GPL
 Keywords: db,database
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
 Platform: win32
-Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Database
-Classifier: Typing :: Typed
-Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Black Cat DataBase
 
 [![Hits-of-Code](https://hitsofcode.com/github/koviubi56/bcdb?branch=main)](https://hitsofcode.com/github/koviubi56/bcdb/view?branch=main)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/103515bdc600439d98a0f1ea1f767c71)](https://www.codacy.com/gh/koviubi56/bcdb/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=koviubi56/bcdb&amp;utm_campaign=Badge_Grade)
@@ -48,15 +37,15 @@
 
 ```bash
 pip install bcdb
 ```
 
 ## Requirements
 
-BCDB requires Python 3.11.
+BCDB requires Python 3.10.
 
 ## Usage
 
 ```python
 import bcdb
 from pathlib import Path
```

