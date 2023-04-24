# Comparing `tmp/ogjpn-1.0.2-py3-none-any.whl.zip` & `tmp/ogjpn-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 134601 bytes, number of entries: 34
+Zip file size: 134471 bytes, number of entries: 34
 -rw-r--r--  2.0 unx    42394 b- defN 23-Apr-15 16:07 ogjpn/SS.py
 -rw-r--r--  2.0 unx    41963 b- defN 23-Apr-15 16:07 ogjpn/TPI.py
--rw-r--r--  2.0 unx      593 b- defN 23-Apr-24 16:08 ogjpn/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-24 16:55 ogjpn/__init__.py
 -rw-r--r--  2.0 unx    15816 b- defN 23-Apr-15 16:07 ogjpn/_version.py
 -rw-r--r--  2.0 unx    19284 b- defN 23-Apr-15 16:07 ogjpn/aggregates.py
 -rw-r--r--  2.0 unx     7295 b- defN 23-Apr-18 12:17 ogjpn/bequest_transmission.py
 -rw-r--r--  2.0 unx    13942 b- defN 23-Apr-18 12:38 ogjpn/calibrate.py
 -rw-r--r--  2.0 unx    13020 b- defN 23-Apr-18 10:12 ogjpn/constants.py
 -rw-r--r--  2.0 unx    26165 b- defN 23-Apr-19 07:31 ogjpn/demographics.py
 -rw-r--r--  2.0 unx     5012 b- defN 23-Apr-16 11:02 ogjpn/deterministic_profiles.py
@@ -24,13 +24,13 @@
 -rw-r--r--  2.0 unx    25998 b- defN 23-Apr-15 16:07 ogjpn/parameters.py
 -rw-r--r--  2.0 unx    17823 b- defN 23-Apr-18 08:16 ogjpn/psid_data_setup.py
 -rw-r--r--  2.0 unx    20175 b- defN 23-Apr-15 16:07 ogjpn/tax.py
 -rw-r--r--  2.0 unx      240 b- defN 23-Apr-16 16:18 ogjpn/test.py
 -rw-r--r--  2.0 unx     7227 b- defN 23-Apr-16 11:11 ogjpn/transfer_distribution.py
 -rw-r--r--  2.0 unx    67569 b- defN 23-Apr-15 16:07 ogjpn/txfunc.py
 -rw-r--r--  2.0 unx    27678 b- defN 23-Apr-15 16:07 ogjpn/utils.py
--rw-r--r--  2.0 unx     1126 b- defN 23-Apr-24 16:27 ogjpn-1.0.2.dist-info/LICENSE.md
--rw-r--r--  2.0 unx    10427 b- defN 23-Apr-24 16:27 ogjpn-1.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-24 16:27 ogjpn-1.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Apr-24 16:27 ogjpn-1.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2608 b- defN 23-Apr-24 16:27 ogjpn-1.0.2.dist-info/RECORD
-34 files, 584623 bytes uncompressed, 130573 bytes compressed:  77.7%
+-rw-r--r--  2.0 unx     1126 b- defN 23-Apr-24 17:15 ogjpn-1.0.3.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx    10692 b- defN 23-Apr-24 17:15 ogjpn-1.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-24 17:15 ogjpn-1.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Apr-24 17:15 ogjpn-1.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2606 b- defN 23-Apr-24 17:15 ogjpn-1.0.3.dist-info/RECORD
+34 files, 584293 bytes uncompressed, 130443 bytes compressed:  77.7%
```

## zipnote {}

```diff
@@ -81,23 +81,23 @@
 
 Filename: ogjpn/txfunc.py
 Comment: 
 
 Filename: ogjpn/utils.py
 Comment: 
 
-Filename: ogjpn-1.0.2.dist-info/LICENSE.md
+Filename: ogjpn-1.0.3.dist-info/LICENSE.md
 Comment: 
 
-Filename: ogjpn-1.0.2.dist-info/METADATA
+Filename: ogjpn-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: ogjpn-1.0.2.dist-info/WHEEL
+Filename: ogjpn-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: ogjpn-1.0.2.dist-info/top_level.txt
+Filename: ogjpn-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: ogjpn-1.0.2.dist-info/RECORD
+Filename: ogjpn-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ogjpn/__init__.py

```diff
@@ -1,38 +0,0 @@
-00000000: 2222 220a 5370 6563 6966 7920 7768 6174  """.Specify what
-00000010: 2069 7320 6176 6169 6c61 626c 6520 746f   is available to
-00000020: 2069 6d70 6f72 7420 6672 6f6d 2074 6865   import from the
-00000030: 206f 676a 706e 2070 6163 6b61 6765 2e0a   ogjpn package..
-00000040: 2222 220a 6672 6f6d 206f 676a 706e 2e53  """.from ogjpn.S
-00000050: 5320 696d 706f 7274 202a 0a66 726f 6d20  S import *.from 
-00000060: 6f67 6a70 6e2e 5450 4920 696d 706f 7274  ogjpn.TPI import
-00000070: 202a 0a66 726f 6d20 6f67 6a70 6e2e 6167   *.from ogjpn.ag
-00000080: 6772 6567 6174 6573 2069 6d70 6f72 7420  gregates import 
-00000090: 2a0a 6672 6f6d 206f 676a 706e 2e63 6f6e  *.from ogjpn.con
-000000a0: 7374 616e 7473 2069 6d70 6f72 7420 2a0a  stants import *.
-000000b0: 6672 6f6d 206f 676a 706e 2e65 6c6c 6970  from ogjpn.ellip
-000000c0: 7469 6361 6c5f 755f 6573 7420 696d 706f  tical_u_est impo
-000000d0: 7274 202a 0a66 726f 6d20 6f67 6a70 6e2e  rt *.from ogjpn.
-000000e0: 6578 6563 7574 6520 696d 706f 7274 202a  execute import *
-000000f0: 0a66 726f 6d20 6f67 6a70 6e2e 6669 726d  .from ogjpn.firm
-00000100: 2069 6d70 6f72 7420 2a0a 6672 6f6d 206f   import *.from o
-00000110: 676a 706e 2e66 6973 6361 6c20 696d 706f  gjpn.fiscal impo
-00000120: 7274 202a 0a66 726f 6d20 6f67 6a70 6e2e  rt *.from ogjpn.
-00000130: 686f 7573 6568 6f6c 6420 696d 706f 7274  household import
-00000140: 202a 0a66 726f 6d20 6f67 6a70 6e2e 6f75   *.from ogjpn.ou
-00000150: 7470 7574 5f70 6c6f 7473 2069 6d70 6f72  tput_plots impor
-00000160: 7420 2a0a 6672 6f6d 206f 676a 706e 2e6f  t *.from ogjpn.o
-00000170: 7574 7075 745f 7461 626c 6573 2069 6d70  utput_tables imp
-00000180: 6f72 7420 2a0a 6672 6f6d 206f 676a 706e  ort *.from ogjpn
-00000190: 2e70 6172 616d 6574 6572 5f70 6c6f 7473  .parameter_plots
-000001a0: 2069 6d70 6f72 7420 2a0a 6672 6f6d 206f   import *.from o
-000001b0: 676a 706e 2e70 6172 616d 6574 6572 5f74  gjpn.parameter_t
-000001c0: 6162 6c65 7320 696d 706f 7274 202a 0a66  ables import *.f
-000001d0: 726f 6d20 6f67 6a70 6e2e 7061 7261 6d65  rom ogjpn.parame
-000001e0: 7465 7273 2069 6d70 6f72 7420 2a0a 6672  ters import *.fr
-000001f0: 6f6d 206f 676a 706e 2e74 6178 2069 6d70  om ogjpn.tax imp
-00000200: 6f72 7420 2a0a 6672 6f6d 206f 676a 706e  ort *.from ogjpn
-00000210: 2e74 7866 756e 6320 696d 706f 7274 202a  .txfunc import *
-00000220: 0a66 726f 6d20 6f67 6a70 6e2e 7574 696c  .from ogjpn.util
-00000230: 7320 696d 706f 7274 202a 0a0a 5f5f 7665  s import *..__ve
-00000240: 7273 696f 6e5f 5f20 3d20 2231 2e30 2e31  rsion__ = "1.0.1
-00000250: 22                                       "
```

## Comparing `ogjpn-1.0.2.dist-info/LICENSE.md` & `ogjpn-1.0.3.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `ogjpn-1.0.2.dist-info/METADATA` & `ogjpn-1.0.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: ogjpn
-Version: 1.0.2
-Summary: An overlapping generations model in Japan
+Version: 1.0.3
+Summary: Overlapping-generations macroeconomic model for evaluating fiscal policy in Japan
 Home-page: https://github.com/Tatsuru-Kikuchi/OG-JPN
 Download-URL: https://github.com/Tatsuru-Kikuchi/OG-JPN
 Author: Tatsuru Kikuchi
-Author-email: tatsuru.kikuchi@e.u-tokyo.ac.jp
+Author-email: Tatsuru Kikuchi <tatsuru.kikuchi@e.u-tokyo.ac.jp>
 Maintainer: Tatsuru Kikuchi
 Maintainer-email: tatsuru.kikuchi@e.u-tokyo.ac.jp
 License: MIT License
+Project-URL: Homepage, https://github.com/Tatsuru-Kikuchi/OG-JPN
+Project-URL: Bug Tracker, https://github.com/Tatsuru-Kikuchi/OG-JPN/issues
+Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: numpy
 Requires-Dist: psutil
 Requires-Dist: scipy (>=1.5.0)
 Requires-Dist: pandas (>=1.2.5)
 Requires-Dist: matplotlib
```

## Comparing `ogjpn-1.0.2.dist-info/RECORD` & `ogjpn-1.0.3.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ogjpn/SS.py,sha256=Oc0qNTnuxIipeEb-n-6D6Uj1AqdhWONQ9RP7_RX89UM,42394
 ogjpn/TPI.py,sha256=hCAAG1I0YVXNxf_HeEwXXLVHsh5MfR-zR_AIDAVa6_4,41963
-ogjpn/__init__.py,sha256=m0ifD_WRbgRUjBoQrFKBaw2ppBY_HPEi3Aif7ATocc8,593
+ogjpn/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ogjpn/_version.py,sha256=03ZEAAuUK7KVFOeaJ86zgQwNPPD6ZL479w-bbPJnarw,15816
 ogjpn/aggregates.py,sha256=c1Kvx8b5JPCCftTaEyn0VEEnziYtFpBH0vcG_VxKCZE,19284
 ogjpn/bequest_transmission.py,sha256=6LcFITm7ye4iuN1RdcHvMNwYyI04w8P73stBB2wXsPo,7295
 ogjpn/calibrate.py,sha256=Sn8Nq1kqkKoxhoSuhE4HqQ774ihr0RKjtuCKDxCyhbM,13942
 ogjpn/constants.py,sha256=up1gDpBJWTfL8ClbTGc3Pw7Q5QVhJk-fVoPHX3rs5cg,13020
 ogjpn/demographics.py,sha256=sXl7f09qHbh0dCRS0uUfzZcbSGKLCvD3CrdaOWGF-U4,26165
 ogjpn/deterministic_profiles.py,sha256=hXVTAnm2JNLZUDamBBmSrsm0YApTbKwphapxFc2D4mE,5012
@@ -23,12 +23,12 @@
 ogjpn/parameters.py,sha256=LP8JrZn8KK9pj3labSTgL8rBACHYXVD5abQgQJyZJqs,25998
 ogjpn/psid_data_setup.py,sha256=47IY7SQmdaOM6bZ20GnprQHoJCZ4fIY2wrOaTOTZgzI,17823
 ogjpn/tax.py,sha256=P2CpbvxAwGnGrkuBMDwzP2qAbCZBydjwcQXa9sxBCnE,20175
 ogjpn/test.py,sha256=qLzux6lIvJcAxPze59oByUAW-7i4kSJQnEetKCnxyIY,240
 ogjpn/transfer_distribution.py,sha256=QpUFMFJhJWGujbH3I05Et9_JcwTTHoYp1dT2uzKN_vA,7227
 ogjpn/txfunc.py,sha256=N6Pnua0mVnF9bZ_wQ8CdZXen2YNbE5i_pOiI_lPAXHI,67569
 ogjpn/utils.py,sha256=W932OFn-uXCvDXbFFre2-QjHQ7qkonTMhxXs-Bo0zuE,27678
-ogjpn-1.0.2.dist-info/LICENSE.md,sha256=TODCLQ3yXjW1rYT7tXuIW-R-6-MFvnVyrzyo19eXxo8,1126
-ogjpn-1.0.2.dist-info/METADATA,sha256=bKljXKaz45jHDTp-dBhVmVpoj1xjpl8oa9WxYeK9Lag,10427
-ogjpn-1.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-ogjpn-1.0.2.dist-info/top_level.txt,sha256=VKfiGBqXZzYBl_yx8_DuiWAJI2IDqZWiSGWEVnUKASQ,6
-ogjpn-1.0.2.dist-info/RECORD,,
+ogjpn-1.0.3.dist-info/LICENSE.md,sha256=TODCLQ3yXjW1rYT7tXuIW-R-6-MFvnVyrzyo19eXxo8,1126
+ogjpn-1.0.3.dist-info/METADATA,sha256=Ku48lMmu7o-7T6cJE71WvkVoMkJcFhOhhTOhbRzsrTk,10692
+ogjpn-1.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ogjpn-1.0.3.dist-info/top_level.txt,sha256=VKfiGBqXZzYBl_yx8_DuiWAJI2IDqZWiSGWEVnUKASQ,6
+ogjpn-1.0.3.dist-info/RECORD,,
```

