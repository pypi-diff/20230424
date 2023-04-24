# Comparing `tmp/gnutools_python-2.3.4-py3-none-any.whl.zip` & `tmp/gnutools_python-2.3.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 12437 bytes, number of entries: 21
--rw-rw-r--  2.0 unx       48 b- defN 23-Apr-21 02:12 gnutools/__init__.py
+Zip file size: 12442 bytes, number of entries: 21
+-rw-rw-r--  2.0 unx       48 b- defN 23-Apr-24 01:02 gnutools/__init__.py
 -rw-rw-r--  2.0 unx      925 b- defN 23-Apr-20 03:05 gnutools/functional.py
 -rw-rw-r--  2.0 unx       26 b- defN 23-Apr-20 03:06 gnutools/audio/__init__.py
 -rw-rw-r--  2.0 unx      658 b- defN 23-Apr-20 03:06 gnutools/audio/functional.py
 -rw-rw-r--  2.0 unx     2673 b- defN 23-Apr-20 04:23 gnutools/concurrent/__init__.py
 -rw-rw-r--  2.0 unx       25 b- defN 23-Apr-20 03:06 gnutools/fs/__init__.py
 -rw-rw-r--  2.0 unx     4906 b- defN 23-Apr-20 03:05 gnutools/fs/functional.py
 -rw-rw-r--  2.0 unx       42 b- defN 23-Apr-20 03:06 gnutools/grid/__init__.py
@@ -11,13 +11,13 @@
 -rw-rw-r--  2.0 unx       26 b- defN 23-Apr-20 03:06 gnutools/remote/__init__.py
 -rw-rw-r--  2.0 unx      738 b- defN 23-Apr-20 03:05 gnutools/remote/functional.py
 -rw-rw-r--  2.0 unx       25 b- defN 23-Apr-20 03:06 gnutools/tests/__init__.py
 -rw-rw-r--  2.0 unx      183 b- defN 23-Apr-20 03:06 gnutools/tests/__main__.py
 -rw-rw-r--  2.0 unx      473 b- defN 23-Apr-20 03:06 gnutools/tests/functional.py
 -rw-rw-r--  2.0 unx       26 b- defN 23-Apr-20 03:06 gnutools/utils/__init__.py
 -rw-rw-r--  2.0 unx     4369 b- defN 23-Apr-20 03:06 gnutools/utils/functional.py
--rwxr-xr-x  2.0 unx     1079 b- defN 23-Apr-21 02:12 gnutools_python-2.3.4.dist-info/LICENSE
--rw-rw-r--  2.0 unx     5003 b- defN 23-Apr-21 02:12 gnutools_python-2.3.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-21 02:12 gnutools_python-2.3.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-Apr-21 02:12 gnutools_python-2.3.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1729 b- defN 23-Apr-21 02:12 gnutools_python-2.3.4.dist-info/RECORD
-21 files, 24922 bytes uncompressed, 9599 bytes compressed:  61.5%
+-rwxr-xr-x  2.0 unx     1079 b- defN 23-Apr-24 01:02 gnutools_python-2.3.5.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     5023 b- defN 23-Apr-24 01:02 gnutools_python-2.3.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-24 01:02 gnutools_python-2.3.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-Apr-24 01:02 gnutools_python-2.3.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1729 b- defN 23-Apr-24 01:02 gnutools_python-2.3.5.dist-info/RECORD
+21 files, 24942 bytes uncompressed, 9604 bytes compressed:  61.5%
```

## zipnote {}

```diff
@@ -42,23 +42,23 @@
 
 Filename: gnutools/utils/__init__.py
 Comment: 
 
 Filename: gnutools/utils/functional.py
 Comment: 
 
-Filename: gnutools_python-2.3.4.dist-info/LICENSE
+Filename: gnutools_python-2.3.5.dist-info/LICENSE
 Comment: 
 
-Filename: gnutools_python-2.3.4.dist-info/METADATA
+Filename: gnutools_python-2.3.5.dist-info/METADATA
 Comment: 
 
-Filename: gnutools_python-2.3.4.dist-info/WHEEL
+Filename: gnutools_python-2.3.5.dist-info/WHEEL
 Comment: 
 
-Filename: gnutools_python-2.3.4.dist-info/top_level.txt
+Filename: gnutools_python-2.3.5.dist-info/top_level.txt
 Comment: 
 
-Filename: gnutools_python-2.3.4.dist-info/RECORD
+Filename: gnutools_python-2.3.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gnutools/__init__.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "2.3.4"
+__version__ = "2.3.5"
 from .functional import *
```

## Comparing `gnutools_python-2.3.4.dist-info/LICENSE` & `gnutools_python-2.3.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gnutools_python-2.3.4.dist-info/METADATA` & `gnutools_python-2.3.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gnutools-python
-Version: 2.3.4
+Version: 2.3.5
 Summary: GNU Tools for python
 Home-page: https://github.com/JeanMaximilienCadic/gnutools-python
 Author: Jean Maximilien Cadic
 Author-email: git@cadic.jp
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
@@ -14,14 +14,15 @@
 Requires-Dist: pyYaml
 Requires-Dist: numpy
 Requires-Dist: rich
 Requires-Dist: tabulate
 Requires-Dist: pandas
 Requires-Dist: tqdm
 Requires-Dist: gdown
+Requires-Dist: h5py
 
 <h1 align="center">
   <br>
   <a href=https://drive.google.com/uc?id=1vHpmRHChj0lPvytmGUJ3mExcLgIYLMJj"><img src="https://drive.google.com/uc?id=1vHpmRHChj0lPvytmGUJ3mExcLgIYLMJj"></a>
   <br>
   GNUTOOLS
   <br>
```

### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: gnutools-python Version: 2.3.4 Summary: GNU Tools
+Metadata-Version: 2.1 Name: gnutools-python Version: 2.3.5 Summary: GNU Tools
 for python Home-page: https://github.com/JeanMaximilienCadic/gnutools-python
 Author: Jean Maximilien Cadic Author-email: git@cadic.jp License: MIT
 Classifier: Programming Language :: Python :: 3.6 Classifier: License :: OSI
 Approved :: MIT License Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: pyYaml Requires-Dist: numpy
 Requires-Dist: rich Requires-Dist: tabulate Requires-Dist: pandas Requires-
-Dist: tqdm Requires-Dist: gdown
+Dist: tqdm Requires-Dist: gdown Requires-Dist: h5py
                                     ******
       [https://drive.google.com/uc?id=1vHpmRHChj0lPvytmGUJ3mExcLgIYLMJj]
                                    GNUTOOLS
                                      ******
 Modules â¢ Code_structure â¢ Installing_the_application â¢ Makefile_commands
             â¢ Environments â¢ Running_the_application Ressources
 Gnutools is a Python package that provides a few perks: - Up to 3x speedup
```

## Comparing `gnutools_python-2.3.4.dist-info/RECORD` & `gnutools_python-2.3.5.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-gnutools/__init__.py,sha256=zAeKqr-3PYHsxKGH09lx66-FSgeQ5-uywEc56G0X_28,48
+gnutools/__init__.py,sha256=yTT5mMkWrZX7vYzkkdHpmsRNVy8TEAY2EIpWKvEmCqQ,48
 gnutools/functional.py,sha256=DBUd56_24SkuGkHUa5ipo_M4c1NJ55dmZqBy-xEcBgU,925
 gnutools/audio/__init__.py,sha256=QsZLoNOPzs17hbkFTJowo2Ik_wJ55Nl9OreWblIHQPk,26
 gnutools/audio/functional.py,sha256=m5JJPjDiuFeTw4Kq_5Up2AiKCh3rNT-8qgrWC2LBkbc,658
 gnutools/concurrent/__init__.py,sha256=_BbMEb6VS0m-bptWz0kkPZBMmq9O0gyZqAnTwIIDCSs,2673
 gnutools/fs/__init__.py,sha256=nmKq3MHGIpNcXUg8KWmTT9CmEwDc-df8U3VKesf6ogI,25
 gnutools/fs/functional.py,sha256=zHyU0R6ucyA82KJS0zAFcR2ZjtieBwUCYXNwq0w8wnA,4906
 gnutools/grid/__init__.py,sha256=2U-B_r4PMYgn7Fq4N0ktvehYLN-KkxRqiXB3802_GEU,42
@@ -10,12 +10,12 @@
 gnutools/remote/__init__.py,sha256=QsZLoNOPzs17hbkFTJowo2Ik_wJ55Nl9OreWblIHQPk,26
 gnutools/remote/functional.py,sha256=erXWVOwtGlSpnIt1sWRcpWgE6oAl8w2-tjG4xXUq7kw,738
 gnutools/tests/__init__.py,sha256=nmKq3MHGIpNcXUg8KWmTT9CmEwDc-df8U3VKesf6ogI,25
 gnutools/tests/__main__.py,sha256=SLTxa4eTSehaqfCuICRWfhmHngc6jgGnepm-Sj_UTgA,183
 gnutools/tests/functional.py,sha256=ZA_-HleON4RvBV8JvSsGlWLafFAmBS6mdpLWE-v43s0,473
 gnutools/utils/__init__.py,sha256=QsZLoNOPzs17hbkFTJowo2Ik_wJ55Nl9OreWblIHQPk,26
 gnutools/utils/functional.py,sha256=aSDuSYk0wVRaDT-pkS-p0Wdhl82KXEmaXKazBa-68ho,4369
-gnutools_python-2.3.4.dist-info/LICENSE,sha256=5LLn7mEAiZaHa_jloiSYF3tR4lz09gVuLW94NMVMN64,1079
-gnutools_python-2.3.4.dist-info/METADATA,sha256=uO5B7hCRECIkzpv98QPUy1IL9GFiiN4ckYw3ermKYaQ,5003
-gnutools_python-2.3.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-gnutools_python-2.3.4.dist-info/top_level.txt,sha256=r2ixkUA9ZgAx7olOT0VKo-mI4Lum5WWT7RUaUvd_erE,9
-gnutools_python-2.3.4.dist-info/RECORD,,
+gnutools_python-2.3.5.dist-info/LICENSE,sha256=5LLn7mEAiZaHa_jloiSYF3tR4lz09gVuLW94NMVMN64,1079
+gnutools_python-2.3.5.dist-info/METADATA,sha256=p08UHO6MUCere4bFi61JdO96k7ns5Fvt9uezbvYE7Qs,5023
+gnutools_python-2.3.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+gnutools_python-2.3.5.dist-info/top_level.txt,sha256=r2ixkUA9ZgAx7olOT0VKo-mI4Lum5WWT7RUaUvd_erE,9
+gnutools_python-2.3.5.dist-info/RECORD,,
```

