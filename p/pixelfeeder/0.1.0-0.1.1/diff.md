# Comparing `tmp/pixelfeeder-0.1.0.tar.gz` & `tmp/pixelfeeder-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixelfeeder-0.1.0.tar", last modified: Mon Apr 17 13:16:11 2023, max compression
+gzip compressed data, was "pixelfeeder-0.1.1.tar", last modified: Mon Apr 24 10:18:56 2023, max compression
```

## Comparing `pixelfeeder-0.1.0.tar` & `pixelfeeder-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 karmanov  (1000) karmanov  (1000)        0 2023-04-17 13:16:11.611940 pixelfeeder-0.1.0/
--rw-r--r--   0 karmanov  (1000) karmanov  (1000)    11358 2023-04-11 18:41:54.000000 pixelfeeder-0.1.0/LICENSE
--rw-r--r--   0 karmanov  (1000) karmanov  (1000)     3870 2023-04-17 13:16:11.611940 pixelfeeder-0.1.0/PKG-INFO
--rw-r--r--   0 karmanov  (1000) karmanov  (1000)     3268 2023-04-17 13:15:53.000000 pixelfeeder-0.1.0/README.md
-drwxr-xr-x   0 karmanov  (1000) karmanov  (1000)        0 2023-04-17 13:16:11.611940 pixelfeeder-0.1.0/pixelfeeder/
--rw-r--r--   0 karmanov  (1000) karmanov  (1000)     1109 2023-04-13 19:04:30.000000 pixelfeeder-0.1.0/pixelfeeder/__init__.py
--rw-r--r--   0 karmanov  (1000) karmanov  (1000)     3610 2023-04-14 18:22:19.000000 pixelfeeder-0.1.0/pixelfeeder/cli.py
--rw-r--r--   0 karmanov  (1000) karmanov  (1000)     5169 2023-04-15 13:29:25.000000 pixelfeeder-0.1.0/pixelfeeder/flickr_data_reader.py
--rw-r--r--   0 karmanov  (1000) karmanov  (1000)    30398 2023-04-15 19:04:59.000000 pixelfeeder-0.1.0/pixelfeeder/gui.py
--rw-r--r--   0 karmanov  (1000) karmanov  (1000)     4156 2023-04-14 09:35:06.000000 pixelfeeder-0.1.0/pixelfeeder/pixelfed_uploader.py
--rw-r--r--   0 karmanov  (1000) karmanov  (1000)     4068 2023-04-14 17:36:19.000000 pixelfeeder-0.1.0/pixelfeeder/tools.py
-drwxr-xr-x   0 karmanov  (1000) karmanov  (1000)        0 2023-04-17 13:16:11.611940 pixelfeeder-0.1.0/pixelfeeder.egg-info/
--rw-r--r--   0 karmanov  (1000) karmanov  (1000)     3870 2023-04-17 13:16:11.000000 pixelfeeder-0.1.0/pixelfeeder.egg-info/PKG-INFO
--rw-r--r--   0 karmanov  (1000) karmanov  (1000)      398 2023-04-17 13:16:11.000000 pixelfeeder-0.1.0/pixelfeeder.egg-info/SOURCES.txt
--rw-r--r--   0 karmanov  (1000) karmanov  (1000)        1 2023-04-17 13:16:11.000000 pixelfeeder-0.1.0/pixelfeeder.egg-info/dependency_links.txt
--rw-r--r--   0 karmanov  (1000) karmanov  (1000)       92 2023-04-17 13:16:11.000000 pixelfeeder-0.1.0/pixelfeeder.egg-info/entry_points.txt
--rw-r--r--   0 karmanov  (1000) karmanov  (1000)       72 2023-04-17 13:16:11.000000 pixelfeeder-0.1.0/pixelfeeder.egg-info/requires.txt
--rw-r--r--   0 karmanov  (1000) karmanov  (1000)       12 2023-04-17 13:16:11.000000 pixelfeeder-0.1.0/pixelfeeder.egg-info/top_level.txt
--rw-r--r--   0 karmanov  (1000) karmanov  (1000)      393 2023-04-17 13:16:11.611940 pixelfeeder-0.1.0/setup.cfg
--rw-r--r--   0 karmanov  (1000) karmanov  (1000)     1950 2023-04-17 13:15:53.000000 pixelfeeder-0.1.0/setup.py
+drwxr-xr-x   0 karmanov  (1000) karmanov  (1000)        0 2023-04-24 10:18:56.001372 pixelfeeder-0.1.1/
+-rw-r--r--   0 karmanov  (1000) karmanov  (1000)    11358 2023-04-11 18:41:54.000000 pixelfeeder-0.1.1/LICENSE
+-rw-r--r--   0 karmanov  (1000) karmanov  (1000)     3884 2023-04-24 10:18:56.001372 pixelfeeder-0.1.1/PKG-INFO
+-rw-r--r--   0 karmanov  (1000) karmanov  (1000)     3282 2023-04-20 21:22:40.000000 pixelfeeder-0.1.1/README.md
+drwxr-xr-x   0 karmanov  (1000) karmanov  (1000)        0 2023-04-24 10:18:56.001372 pixelfeeder-0.1.1/pixelfeeder/
+-rw-r--r--   0 karmanov  (1000) karmanov  (1000)      997 2023-04-20 12:28:27.000000 pixelfeeder-0.1.1/pixelfeeder/__init__.py
+-rw-r--r--   0 karmanov  (1000) karmanov  (1000)     3610 2023-04-14 18:22:19.000000 pixelfeeder-0.1.1/pixelfeeder/cli.py
+-rw-r--r--   0 karmanov  (1000) karmanov  (1000)     5169 2023-04-15 13:29:25.000000 pixelfeeder-0.1.1/pixelfeeder/flickr_data_reader.py
+-rw-r--r--   0 karmanov  (1000) karmanov  (1000)    34692 2023-04-20 21:38:46.000000 pixelfeeder-0.1.1/pixelfeeder/gui.py
+-rw-r--r--   0 karmanov  (1000) karmanov  (1000)     3558 2023-04-20 21:12:20.000000 pixelfeeder-0.1.1/pixelfeeder/image_loader.py
+-rw-r--r--   0 karmanov  (1000) karmanov  (1000)     4156 2023-04-14 09:35:06.000000 pixelfeeder-0.1.1/pixelfeeder/pixelfed_uploader.py
+-rw-r--r--   0 karmanov  (1000) karmanov  (1000)     4068 2023-04-14 17:36:19.000000 pixelfeeder-0.1.1/pixelfeeder/tools.py
+drwxr-xr-x   0 karmanov  (1000) karmanov  (1000)        0 2023-04-24 10:18:56.001372 pixelfeeder-0.1.1/pixelfeeder.egg-info/
+-rw-r--r--   0 karmanov  (1000) karmanov  (1000)     3884 2023-04-24 10:18:55.000000 pixelfeeder-0.1.1/pixelfeeder.egg-info/PKG-INFO
+-rw-r--r--   0 karmanov  (1000) karmanov  (1000)      426 2023-04-24 10:18:55.000000 pixelfeeder-0.1.1/pixelfeeder.egg-info/SOURCES.txt
+-rw-r--r--   0 karmanov  (1000) karmanov  (1000)        1 2023-04-24 10:18:55.000000 pixelfeeder-0.1.1/pixelfeeder.egg-info/dependency_links.txt
+-rw-r--r--   0 karmanov  (1000) karmanov  (1000)       92 2023-04-24 10:18:55.000000 pixelfeeder-0.1.1/pixelfeeder.egg-info/entry_points.txt
+-rw-r--r--   0 karmanov  (1000) karmanov  (1000)       72 2023-04-24 10:18:55.000000 pixelfeeder-0.1.1/pixelfeeder.egg-info/requires.txt
+-rw-r--r--   0 karmanov  (1000) karmanov  (1000)       12 2023-04-24 10:18:55.000000 pixelfeeder-0.1.1/pixelfeeder.egg-info/top_level.txt
+-rw-r--r--   0 karmanov  (1000) karmanov  (1000)      393 2023-04-24 10:18:56.001372 pixelfeeder-0.1.1/setup.cfg
+-rw-r--r--   0 karmanov  (1000) karmanov  (1000)     1950 2023-04-24 10:17:30.000000 pixelfeeder-0.1.1/setup.py
```

### Comparing `pixelfeeder-0.1.0/LICENSE` & `pixelfeeder-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pixelfeeder-0.1.0/PKG-INFO` & `pixelfeeder-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7069 7865  : 2.1.Name: pixe
 00000020: 6c66 6565 6465 720a 5665 7273 696f 6e3a  lfeeder.Version:
-00000030: 2030 2e31 2e30 0a53 756d 6d61 7279 3a20   0.1.0.Summary: 
+00000030: 2030 2e31 2e31 0a53 756d 6d61 7279 3a20   0.1.1.Summary: 
 00000040: 496d 706f 7274 2046 6c69 636b 7220 6461  Import Flickr da
 00000050: 7461 2069 6e74 6f20 6120 5069 7865 6c66  ta into a Pixelf
 00000060: 6564 2061 6363 6f75 6e74 0a48 6f6d 652d  ed account.Home-
 00000070: 7061 6765 3a20 6874 7470 733a 2f2f 6769  page: https://gi
 00000080: 746c 6162 2e63 6f6d 2f62 6572 6765 6e74  tlab.com/bergent
 00000090: 726f 6c6c 2f70 6978 656c 6665 6564 6572  roll/pixelfeeder
 000000a0: 0a41 7574 686f 723a 2041 6e74 6f6e 204b  .Author: Anton K
@@ -216,27 +216,28 @@
 00000d70: 6775 6d65 6e74 7320 7573 6520 7468 6520  guments use the 
 00000d80: 602d 6860 202f 2060 2d2d 6865 6c70 6020  `-h` / `--help` 
 00000d90: 666c 6167 2e0a 0a23 2320 4755 490a 0a60  flag...## GUI..`
 00000da0: 6060 7368 656c 6c0a 7069 7865 6c66 6565  ``shell.pixelfee
 00000db0: 6465 722d 6775 6920 5b2d 2d63 6f6e 6669  der-gui [--confi
 00000dc0: 672d 6669 6c65 2043 4f4e 4649 475f 4649  g-file CONFIG_FI
 00000dd0: 4c45 5d20 5b2d 2d76 6572 626f 7365 5d20  LE] [--verbose] 
-00000de0: 5b2d 2d68 656c 705d 0a60 6060 0a0a 4772  [--help].```..Gr
-00000df0: 6170 6869 6361 6c20 696e 7465 7266 6163  aphical interfac
-00000e00: 6520 6861 7320 6d6f 7374 6c79 2074 6865  e has mostly the
-00000e10: 2073 616d 6520 6f70 7469 6f6e 7320 6173   same options as
-00000e20: 2074 6865 2043 4c49 2c20 6275 7420 7570   the CLI, but up
-00000e30: 6f61 6473 2069 6d61 6765 730a 6f6e 652d  oads images.one-
-00000e40: 6279 2d6f 6e65 2069 6e20 696e 7465 7261  by-one in intera
-00000e50: 6374 6976 6520 6d6f 6465 2e20 5573 6572  ctive mode. User
-00000e60: 2061 626c 6520 746f 2063 6f72 7265 6374   able to correct
-00000e70: 2063 6170 7469 6f6e 2061 6e64 2076 6973   caption and vis
-00000e80: 6962 696c 6974 790a 6f66 2061 2070 6f73  ibility.of a pos
-00000e90: 742e 2054 6f6f 6c20 7769 6c6c 206b 6565  t. Tool will kee
-00000ea0: 7020 706f 7369 7469 6f6e 2062 6574 7765  p position betwe
-00000eb0: 656e 2073 6573 7369 6f6e 732e 0a0a 3e20  en sessions...> 
-00000ec0: 4564 6974 7320 6172 6520 6e6f 7420 7065  Edits are not pe
-00000ed0: 7273 6973 7465 6e74 2066 6f72 206e 6f77  rsistent for now
-00000ee0: 2c20 736f 2069 7420 6973 2062 6574 7465  , so it is bette
-00000ef0: 7220 746f 206d 616b 6520 636f 7272 6563  r to make correc
-00000f00: 7469 6f6e 7320 6a75 7374 0a3e 2062 6566  tions just.> bef
-00000f10: 6f72 6520 7570 6c6f 6164 696e 670a       ore uploading.
+00000de0: 5b2d 2d73 6166 652d 6d6f 6465 5d20 5b2d  [--safe-mode] [-
+00000df0: 2d68 656c 705d 0a60 6060 0a0a 4772 6170  -help].```..Grap
+00000e00: 6869 6361 6c20 696e 7465 7266 6163 6520  hical interface 
+00000e10: 6861 7320 6d6f 7374 6c79 2074 6865 2073  has mostly the s
+00000e20: 616d 6520 6f70 7469 6f6e 7320 6173 2074  ame options as t
+00000e30: 6865 2043 4c49 2c20 6275 7420 7570 6f61  he CLI, but upoa
+00000e40: 6473 2069 6d61 6765 730a 6f6e 652d 6279  ds images.one-by
+00000e50: 2d6f 6e65 2069 6e20 696e 7465 7261 6374  -one in interact
+00000e60: 6976 6520 6d6f 6465 2e20 5573 6572 2061  ive mode. User a
+00000e70: 626c 6520 746f 2063 6f72 7265 6374 2063  ble to correct c
+00000e80: 6170 7469 6f6e 2061 6e64 2076 6973 6962  aption and visib
+00000e90: 696c 6974 790a 6f66 2061 2070 6f73 742e  ility.of a post.
+00000ea0: 2054 6f6f 6c20 7769 6c6c 206b 6565 7020   Tool will keep 
+00000eb0: 706f 7369 7469 6f6e 2062 6574 7765 656e  position between
+00000ec0: 2073 6573 7369 6f6e 732e 0a0a 3e20 4564   sessions...> Ed
+00000ed0: 6974 7320 6172 6520 6e6f 7420 7065 7273  its are not pers
+00000ee0: 6973 7465 6e74 2066 6f72 206e 6f77 2c20  istent for now, 
+00000ef0: 736f 2069 7420 6973 2062 6574 7465 7220  so it is better 
+00000f00: 746f 206d 616b 6520 636f 7272 6563 7469  to make correcti
+00000f10: 6f6e 7320 6a75 7374 0a3e 2062 6566 6f72  ons just.> befor
+00000f20: 6520 7570 6c6f 6164 696e 670a            e uploading.
```

### Comparing `pixelfeeder-0.1.0/README.md` & `pixelfeeder-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -178,28 +178,29 @@
 00000b10: 7468 6520 6172 6775 6d65 6e74 7320 7573  the arguments us
 00000b20: 6520 7468 6520 602d 6860 202f 2060 2d2d  e the `-h` / `--
 00000b30: 6865 6c70 6020 666c 6167 2e0a 0a23 2320  help` flag...## 
 00000b40: 4755 490a 0a60 6060 7368 656c 6c0a 7069  GUI..```shell.pi
 00000b50: 7865 6c66 6565 6465 722d 6775 6920 5b2d  xelfeeder-gui [-
 00000b60: 2d63 6f6e 6669 672d 6669 6c65 2043 4f4e  -config-file CON
 00000b70: 4649 475f 4649 4c45 5d20 5b2d 2d76 6572  FIG_FILE] [--ver
-00000b80: 626f 7365 5d20 5b2d 2d68 656c 705d 0a60  bose] [--help].`
-00000b90: 6060 0a0a 4772 6170 6869 6361 6c20 696e  ``..Graphical in
-00000ba0: 7465 7266 6163 6520 6861 7320 6d6f 7374  terface has most
-00000bb0: 6c79 2074 6865 2073 616d 6520 6f70 7469  ly the same opti
-00000bc0: 6f6e 7320 6173 2074 6865 2043 4c49 2c20  ons as the CLI, 
-00000bd0: 6275 7420 7570 6f61 6473 2069 6d61 6765  but upoads image
-00000be0: 730a 6f6e 652d 6279 2d6f 6e65 2069 6e20  s.one-by-one in 
-00000bf0: 696e 7465 7261 6374 6976 6520 6d6f 6465  interactive mode
-00000c00: 2e20 5573 6572 2061 626c 6520 746f 2063  . User able to c
-00000c10: 6f72 7265 6374 2063 6170 7469 6f6e 2061  orrect caption a
-00000c20: 6e64 2076 6973 6962 696c 6974 790a 6f66  nd visibility.of
-00000c30: 2061 2070 6f73 742e 2054 6f6f 6c20 7769   a post. Tool wi
-00000c40: 6c6c 206b 6565 7020 706f 7369 7469 6f6e  ll keep position
-00000c50: 2062 6574 7765 656e 2073 6573 7369 6f6e   between session
-00000c60: 732e 0a0a 3e20 4564 6974 7320 6172 6520  s...> Edits are 
-00000c70: 6e6f 7420 7065 7273 6973 7465 6e74 2066  not persistent f
-00000c80: 6f72 206e 6f77 2c20 736f 2069 7420 6973  or now, so it is
-00000c90: 2062 6574 7465 7220 746f 206d 616b 6520   better to make 
-00000ca0: 636f 7272 6563 7469 6f6e 7320 6a75 7374  corrections just
-00000cb0: 0a3e 2062 6566 6f72 6520 7570 6c6f 6164  .> before upload
-00000cc0: 696e 670a                                ing.
+00000b80: 626f 7365 5d20 5b2d 2d73 6166 652d 6d6f  bose] [--safe-mo
+00000b90: 6465 5d20 5b2d 2d68 656c 705d 0a60 6060  de] [--help].```
+00000ba0: 0a0a 4772 6170 6869 6361 6c20 696e 7465  ..Graphical inte
+00000bb0: 7266 6163 6520 6861 7320 6d6f 7374 6c79  rface has mostly
+00000bc0: 2074 6865 2073 616d 6520 6f70 7469 6f6e   the same option
+00000bd0: 7320 6173 2074 6865 2043 4c49 2c20 6275  s as the CLI, bu
+00000be0: 7420 7570 6f61 6473 2069 6d61 6765 730a  t upoads images.
+00000bf0: 6f6e 652d 6279 2d6f 6e65 2069 6e20 696e  one-by-one in in
+00000c00: 7465 7261 6374 6976 6520 6d6f 6465 2e20  teractive mode. 
+00000c10: 5573 6572 2061 626c 6520 746f 2063 6f72  User able to cor
+00000c20: 7265 6374 2063 6170 7469 6f6e 2061 6e64  rect caption and
+00000c30: 2076 6973 6962 696c 6974 790a 6f66 2061   visibility.of a
+00000c40: 2070 6f73 742e 2054 6f6f 6c20 7769 6c6c   post. Tool will
+00000c50: 206b 6565 7020 706f 7369 7469 6f6e 2062   keep position b
+00000c60: 6574 7765 656e 2073 6573 7369 6f6e 732e  etween sessions.
+00000c70: 0a0a 3e20 4564 6974 7320 6172 6520 6e6f  ..> Edits are no
+00000c80: 7420 7065 7273 6973 7465 6e74 2066 6f72  t persistent for
+00000c90: 206e 6f77 2c20 736f 2069 7420 6973 2062   now, so it is b
+00000ca0: 6574 7465 7220 746f 206d 616b 6520 636f  etter to make co
+00000cb0: 7272 6563 7469 6f6e 7320 6a75 7374 0a3e  rrections just.>
+00000cc0: 2062 6566 6f72 6520 7570 6c6f 6164 696e   before uploadin
+00000cd0: 670a                                     g.
```

### Comparing `pixelfeeder-0.1.0/pixelfeeder/cli.py` & `pixelfeeder-0.1.1/pixelfeeder/cli.py`

 * *Files identical despite different names*

### Comparing `pixelfeeder-0.1.0/pixelfeeder/flickr_data_reader.py` & `pixelfeeder-0.1.1/pixelfeeder/flickr_data_reader.py`

 * *Files identical despite different names*

### Comparing `pixelfeeder-0.1.0/pixelfeeder/gui.py` & `pixelfeeder-0.1.1/pixelfeeder/gui.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,35 +24,42 @@
 import webbrowser
 
 from pathlib import Path
 from tkinter import ttk, filedialog, scrolledtext
 from typing import Any, Callable, List, Optional, Union
 
 import PIL.Image
+import PIL.ImageFile
 import PIL.ImageTk
 import argcomplete
 import xdg_base_dirs
 
 from pixelfeeder.flickr_data_reader import (
     DEFAULT_CAPTION_ORDER, FlickrData, FlickrDataReader, FlickrVisibility, metadata_to_caption
 )
+from pixelfeeder.image_loader import BaseImageLoader, ImageLoader, CachingImageLoader, ImageLoaderError
 from pixelfeeder.pixelfed_uploader import PixelfedVisibility, PixelfedClient, PixelfedClientError
 from pixelfeeder.tools import NumericKwargs, load_config, save_config
 
 MasterType = Union[tkinter.Tk, tkinter.Widget]
 
 APP_NAME = 'Pixelfeeder'
 EXIF_ORIENTATION_MAP = {1: 0, 3: 180, 6: 270, 8: 90}
 PADDING = 5
 FRAME_RELIEF = tkinter.GROOVE
 PADDING_KWARGS = NumericKwargs(padx=PADDING, pady=PADDING)
 IPADDING_KWARGS = NumericKwargs(ipadx=PADDING, ipady=PADDING)
 BUTTON_IPADDING_KWARGS = NumericKwargs(ipadx=PADDING, ipady=PADDING/2)
 SIDE_FRAME_WIDTH = '384p'
 
+CACHED_FILES_LIMIT = 10
+PRELOAD_WINDOW = 5
+
+LOGGER = logging.getLogger(__name__)
+
 
 def set_custom_themes() -> None:
     style = ttk.Style()
     style.configure(
         'ClearButton.TButton',
         highlight='grey',
         font=('Monospace', 8, 'bold'),
@@ -68,113 +75,196 @@
 def set_text_content(field: tkinter.Text, text: Optional[str] = None) -> None:
     if text is None:
         text = ''
     field.delete('1.0', tkinter.END)
     field.insert(tkinter.END, text)
 
 
+class KeypressWrapper:
+    keyboard_pause = 100
+
+    def __init__(self, app: tkinter.Tk, callback: Callable[[], None], pause_ms: Optional[int] = None) -> None:
+        if pause_ms is None:
+            pause_ms = self.keyboard_pause
+
+        self.master = app
+        self.callback = callback
+        self.pause = pause_ms
+
+        self.kb_block = False
+
+    def __call__(self, _: tkinter.Event):
+        if not self.kb_block:
+            self.callback()
+        self.kb_block = True
+        self.master.after(self.pause, self._unset_kb_block)
+
+    def _unset_kb_block(self) -> None:
+        self.kb_block = False
+
+
+class ImageScale(ttk.Scale):
+    label_update_period = 10
+    label_hide_period = 1000
+    deffered_callback_period = 200
+
+    def __init__(self, master: tkinter.Widget, callback: Callable[[], None], variable: tkinter.IntVar) -> None:
+        super().__init__(master, command=self._command, variable=variable)
+        self._var = variable
+        self._load_image_job_id = ''
+        self._update_label_job_id = ''
+        self._hide_label_job_id = ''
+        self._callback = callback
+        self._handle_label = ttk.Label(
+            self.master,
+            justify=tkinter.CENTER,
+            background='white',
+            relief=tkinter.SOLID,
+            border=1,
+            padding='2p')
+
+    @property
+    def value(self) -> int:
+        return self._var.get()
+
+    def _command(self, _: str) -> None:
+        if self._load_image_job_id:
+            self.master.after_cancel(self._load_image_job_id)
+        self._load_image_job_id = self.master.after(self.deffered_callback_period, self._callback)
+
+        if self._update_label_job_id:
+            self.master.after_cancel(self._update_label_job_id)
+        self._update_label_job_id = self.master.after(self.label_update_period, self._update_label)
+
+        if self._hide_label_job_id:
+            self.master.after_cancel(self._hide_label_job_id)
+        self._hide_label_job_id = self.master.after(self.label_hide_period, self._handle_label.place_forget)
+
+    def _update_label(self) -> None:
+        handler_x, handler_y = self.coords()
+        self._handle_label.configure(text=self.value + 1)
+        self._handle_label.place(
+            in_=self,
+            x=handler_x,
+            y=handler_y - self.winfo_height() / 2,
+            bordermode=tkinter.OUTSIDE,
+            anchor=tkinter.S)
+
+
 class Image(ttk.LabelFrame):
     exif_tags = {v: k for k, v in PIL.Image.ExifTags.TAGS.items()}
     exif_orientation_key = exif_tags['Orientation']
     photo_tag = 'PHOTO'
     frame_relief = tkinter.GROOVE
     placeholder = '(EMPTY)'
 
     def __init__(
             self,
             master: MasterType,
             input_frame: 'InputFrame',
             settings: 'Settings',
-            log_screen: 'LogScreen'):
+            log_screen: 'LogScreen',
+            image_loader: BaseImageLoader):
         super().__init__(master, text=self.placeholder, relief=FRAME_RELIEF, labelanchor=tkinter.S)
 
-        self.logger = logging.getLogger(f'{__name__}{self.__class__.__name__}')
-
         self._input_frame = input_frame
         self._settings = settings
         self._log_screen = log_screen
 
-        self._index = 0
-
+        self._image_loader = image_loader
         self._photo_data: FlickrData
         self._photo_paths: List[str] = []
         self._image_orig: Optional[PIL.Image] = None
         self._image: PIL.Image
         self._photo_image: PIL.ImageTk.PhotoImage
+        self._current_image_path: Optional[str] = None
 
+        self._index_var = tkinter.IntVar(value=0)
         self._canvas = tkinter.Canvas(self, bg='gray')
+        self._scale = ImageScale(
+            self,
+            callback=self._load_image,
+            variable=self._index_var,)
 
         self._canvas.bind('<Configure>', self._refresh)
 
-        self._canvas.pack(fill='both', expand=True, **PADDING_KWARGS)
-        self._input_frame.set_enabled(False)
+        self._canvas.pack(fill=tkinter.BOTH, expand=True, **PADDING_KWARGS)
+        self._scale.pack(fill=tkinter.X, expand=False, **PADDING_KWARGS)
+        self._input_frame.enable()
+
+    @property
+    def index(self) -> int:
+        return self._index_var.get()
+
+    @index.setter
+    def index(self, value: int) -> None:
+        images_num = len(self._photo_paths)
+        if images_num:
+            value = value % images_num
+        else:
+            value = 0
+        self._index_var.set(value)
+        self._load_image()
 
     @property
     def image_path(self) -> Optional[str]:
         if not self._photo_paths:
             return None
-        return self._photo_paths[self._index]
+        return self._photo_paths[self.index]
 
     def change_path(self) -> None:
+        self._image_loader.clear()
+
         images_dir = self._input_frame.images_dir
         metadata_dir = self._input_frame.metadata_dir
 
         assert images_dir
         assert metadata_dir
 
         flickr_data_reader = FlickrDataReader(images_dir, metadata_dir)
 
-        self.logger.debug(f'Searching data in {images_dir} images dir, {metadata_dir} metadata dir')
+        LOGGER.debug(f'Searching data in {images_dir} images dir, {metadata_dir} metadata dir')
         self._photo_data = flickr_data_reader.get_photo_dict()
         for issue in self._photo_data.issues:
             self._log_screen.warning(str(issue))
         sorted_data = dict(sorted(self._photo_data.items(), key=lambda i: i[1]['id']))
         self._photo_paths = list(sorted_data.keys())
 
-        self._index = 0
+        self.index = 0
+        self._scale.configure(to=len(self._photo_paths) - 1)
 
         self._load_image()
 
     def seek_image(self, image_path: Optional[str]) -> None:
         if image_path is None:
             return
         try:
-            self._index = self._photo_paths.index(image_path)
+            self.index = self._photo_paths.index(image_path)
         except ValueError:
-            self.logger.warning(f'File {image_path} not found')
+            LOGGER.warning(f'File {image_path} not found')
             return
         self._load_image()
 
     def next(self) -> None:
-        if not self._photo_paths:
-            self.logger.debug('Empty images list')
-        self._index += 1
-        if self._index >= len(self._photo_paths):
-            self._index = 0
-        self._load_image()
+        self.index += 1
 
     def prev(self) -> None:
-        if not self._photo_paths:
-            self.logger.debug('Empty images list')
-        self._index -= 1
-        if self._index < 0:
-            self._index = len(self._photo_paths) - 1
-        self._load_image()
+        self.index -= 1
 
     def refresh(self) -> None:
         self._canvas.event_generate(
             '<Configure>',
             width=self._canvas.winfo_width(),
             height=self._canvas.winfo_height())
 
     def reload(self) -> None:
         self._load_image()
 
     def _refresh(self, event: tkinter.Event) -> None:
-        self.logger.debug('Resizing image by event %s', event)
+        LOGGER.debug('Resizing image by event %s', event)
         if not self._image_orig:
             self._clear_canvas()
             return
 
         self._image = self._image_orig.copy()
 
         self._image.thumbnail((event.width, event.height), PIL.Image.Resampling.LANCZOS)
@@ -186,58 +276,81 @@
             image=self._photo_image,
             anchor=tkinter.CENTER,
             tags=self.photo_tag)
 
     def _clear_canvas(self) -> None:
         self._canvas.delete(self.photo_tag)
 
+    def _try_to_preload_images(self) -> None:
+        ind1, ind2 = self.index - PRELOAD_WINDOW, self.index + PRELOAD_WINDOW
+
+        if ind2 - ind1 >= len(self._photo_paths):
+            paths = self._photo_paths
+        elif ind1 >= 0:
+            paths = self._photo_paths[ind1: ind2]
+        else:
+            paths = self._photo_paths[:ind2] + self._photo_paths[ind1:]
+
+        self._image_loader.preload(paths)
+
     def _load_image(self) -> None:
         image_path = self.image_path
+        if self._current_image_path == image_path:
+            return
 
         if image_path:
-            self._input_frame.set_enabled(True)
+            self._input_frame.enable()
+            self._scale.configure(state=tkinter.NORMAL)
             metadata = self._photo_data[image_path]
             try:
                 caption = metadata_to_caption(
                     metadata=metadata,
                     order=self._settings.caption_order,
                     datetime_format=self._settings.caption_datetime_format)
             except KeyError as error:
                 self._log_screen.error(f'Unknown caption field {error}')
                 caption = ''
 
             self._input_frame.set_caption_text(caption)
 
             self._input_frame.visibility = str(metadata['privacy'])
 
-            self._image_orig = PIL.Image.open(image_path)
+            try:
+                self._image_orig = self._image_loader.open(image_path)
+            except ImageLoaderError as error:
+                self._log_screen.error(f'Error on loading {image_path}:')
+                self._log_screen.warning(str(error))
+                self._image_orig = self._image_loader.open_truncated(image_path)
 
             exif = self._image_orig.getexif()
             orientation_tag = exif.get(self.exif_orientation_key, 0)
             if orientation_tag in (2, 4):
                 self._image_orig = self._image_orig.transpose(PIL.Image.FLIP_LEFT_RIGHT)
                 orientation_tag -= 1
 
             if orientation_tag in (5, 7):
                 self._image_orig = self._image_orig.transpose(PIL.Image.FLIP_)
                 orientation_tag += 1
 
             if orientation_tag in EXIF_ORIENTATION_MAP:
                 self._image_orig = self._image_orig.rotate(EXIF_ORIENTATION_MAP[orientation_tag], expand=True)
 
-            new_text = f'{Path(image_path).name} [{self._index + 1}/{len(self._photo_paths)}]'
+            new_text = f'{Path(image_path).name} [{self.index + 1}/{len(self._photo_paths)}]'
             self.configure(text=new_text)
         else:
-            self.logger.debug('Empty images list')
+            LOGGER.debug('Empty images list')
             self._input_frame.set_caption_text('')
             self._input_frame.visibility = ''
             self._image_orig = None
             self.configure(text=self.placeholder)
-            self._input_frame.set_enabled(False)
+            self._scale.configure(state=tkinter.DISABLED)
+            self._input_frame.disable()
         self.refresh()
+        self._current_image_path = image_path
+        self._try_to_preload_images()
 
 
 class WrappedLabel(ttk.Label):
     """ Label widget which changes wraphlength to width of itself
 
     Needs to be fill='x' and expand=True in Pack to takes effect.
     """
@@ -258,16 +371,14 @@
             add=True)
 
 
 class InputFrame(ttk.Frame):
     def __init__(self, master: MasterType) -> None:
         super().__init__(master)
 
-        self.logger = logging.getLogger(f'{__name__}{self.__class__.__name__}')
-
         self._images_dir_var = tkinter.StringVar()
         self._metadata_dir_var = tkinter.StringVar()
 
         caption_frame = ttk.LabelFrame(self, text='Caption')
         self._caption = tkinter.Text(caption_frame, height=8)
         upload_frame = ttk.Frame(self, relief='flat',)
         visibility_frame = ttk.LabelFrame(upload_frame, relief=FRAME_RELIEF, text='Visibility')
@@ -358,16 +469,16 @@
     def button_set_command(self, name: str, callback: Callable[[], None]) -> None:
         but = getattr(self, f'_button_{name}')
         but.configure(command=callback)
 
     def set_caption_text(self, text: str) -> None:
         set_text_content(self._caption, text)
 
-    def set_enabled(self, enabled: bool) -> None:
-        self.logger.debug(f'Setting inputs to enabled={enabled}')
+    def _set_state(self, enabled: bool) -> None:
+        LOGGER.debug(f'Setting inputs to enabled={enabled}')
         text_state: Any
         if enabled:
             state = 'enabled'
             text_state = tkinter.NORMAL
             list_state = 'readonly'
             bg_color = 'white'
         else:
@@ -377,28 +488,32 @@
             bg_color = 'darkgray'
         self._caption.configure(state=text_state, background=bg_color)
         self._visibility_list.configure(state=list_state)
         self._button_upload.configure(state=state)
         self._button_prev.configure(state=state)
         self._button_next.configure(state=state)
 
+    def enable(self) -> None:
+        self._set_state(enabled=True)
+
+    def disable(self) -> None:
+        self._set_state(enabled=False)
+
 
 class Settings(ttk.Frame):
     default_caption_order = DEFAULT_CAPTION_ORDER
     default_caption_datetime_format = '%c'
 
     def __init__(
             self,
             master: tkinter.Widget,
             config_path: Path,
             on_change_callback: Callable[[], None]) -> None:
         super().__init__(master=master, relief=FRAME_RELIEF)
 
-        self.logger = logging.getLogger(f'{__name__}{self.__class__.__name__}')
-
         self._on_change = on_change_callback
 
         self.config_path = config_path
 
         inner_frame = ttk.Frame(self, relief=tkinter.FLAT, width=50)
 
         self._instance_var = tkinter.StringVar()
@@ -478,15 +593,15 @@
 
     @property
     def caption_datetime_format(self) -> str:
         return self._caption_datetime_format_var.get()
 
     @property
     def is_sufficient(self) -> bool:
-        self.logger.debug(f'Sufficience: instance is {self.instance} and {self.token}')
+        LOGGER.debug(f'Sufficience: instance is {self.instance} and {self.token}')
         return bool(self.instance and self.token)
 
     @property
     def theme(self) -> str:
         return self._theme_list.get()
 
     @property
@@ -589,18 +704,17 @@
 class Application(tkinter.Tk):
     state_file_path = xdg_base_dirs.xdg_data_home() / APP_NAME.lower() / 'last_state.yaml'
     loop_period = 1/100
     update_gui_task_name = 'Update GUI'
     tab_main_index = 0
     tab_settings_index = 1
 
-    def __init__(self, config_path: Path, debug=False) -> None:
+    def __init__(self, config_path: Path, debug=False, safe_mode=False) -> None:
         super().__init__(sync=debug)
 
-        self.logger = logging.getLogger(f'{__name__}{self.__class__.__name__}')
         self._loop = asyncio.get_event_loop()
         self._loop.create_task(self._update(), name=self.update_gui_task_name)
 
         self.title(APP_NAME)
 
         self._notebook = ttk.Notebook(self)
         main_frame = ttk.Frame(self._notebook)
@@ -612,29 +726,38 @@
 
         side_frame = ttk.Frame(main_frame, width=SIDE_FRAME_WIDTH)
         side_frame.pack_propagate(False)
         self._input_frame = InputFrame(side_frame)
         self._settings_frame = Settings(settings_tab, config_path, self.init_pixelfed_client)
         log_screen_frame = ttk.LabelFrame(side_frame, text='Messages', relief=FRAME_RELIEF)
         self._log_screen = LogScreen(log_screen_frame)
+
+        image_loader: BaseImageLoader
+        if safe_mode:
+            image_loader = ImageLoader()
+        else:
+            image_loader = CachingImageLoader(debug=debug, cached_files_limit=CACHED_FILES_LIMIT)
+        self._image_loader_stop_callback = image_loader.stop
+
         self._image = Image(
             main_frame,
             self._input_frame,
             self._settings_frame,
-            self._log_screen)
+            self._log_screen,
+            image_loader)
 
         self._load_state()
         self.init_pixelfed_client()
 
         self.protocol('WM_DELETE_WINDOW', self._on_exit)
 
         self._notebook.bind('<<NotebookTabChanged>>', self._on_tab_change)
-        self.bind('<Control-n>', lambda _: self._image.next())
-        self.bind('<Control-p>', lambda _: self._image.prev())
-        self.bind('<Control-u>', lambda _: self._create_upload_task())
+        self.bind('<Control-n>', KeypressWrapper(self, self._image.next))
+        self.bind('<Control-p>', KeypressWrapper(self, self._image.prev))
+        self.bind('<Control-u>', KeypressWrapper(self, self._create_upload_task))
         self.bind('<Control-q>', self.exit)
 
         self._input_frame.button_set_command('prev', self._image.prev)
         self._input_frame.button_set_command('next', self._image.next)
         self._input_frame.button_set_command('open_images_dir', self._open_images_dir)
         self._input_frame.button_set_command('open_metadata_dir', self._open_metadata_dir)
         self._input_frame.button_set_command('upload', self._create_upload_task)
@@ -681,20 +804,20 @@
         tab = self._notebook.select()
         tab_index = self._notebook.index(tab)
 
         if tab_index == self.tab_settings_index:
             self._settings_is_active = True
         else:
             if self._settings_is_active:
-                self.logger.debug('Cancel unsaved changes of setting')
+                LOGGER.debug('Cancel unsaved changes of setting')
                 self._settings_frame.cancel_action()
             self._settings_is_active = False
 
         if tab_index == self.tab_main_index:
-            self.logger.debug('Reloading image after switching to main tab')
+            LOGGER.debug('Reloading image after switching to main tab')
             self._image.reload()
 
     def _open_images_dir(self) -> None:
         directory = filedialog.askdirectory(
             parent=self, title='Images directory')
         if not directory:
             return
@@ -737,26 +860,27 @@
             self._log_screen.error(f'Failed to upload {img_name}:')
             self._log_screen.error(str(error))
         else:
             self._log_screen.success(f'Image {img_name} posted')
             self._log_screen.url(url)
 
     def _on_exit(self) -> None:
-        self.logger.info(f'Saving state file {self.state_file_path}')
+        self._image_loader_stop_callback()
+        LOGGER.info(f'Saving state file {self.state_file_path}')
         data = {
             'images_dir': self._input_frame.images_dir,
             'metadata_dir': self._input_frame.metadata_dir,
             'image_path': self._image.image_path,
         }
         for task in asyncio.all_tasks():
             name = task.get_name()
             if name == self.update_gui_task_name:
-                self.logger.info(f'Cancelling task {task.get_name()}')
+                LOGGER.info(f'Cancelling task {task.get_name()}')
             else:
-                self.logger.warning(f'Cancelling task {task.get_name()}')
+                LOGGER.warning(f'Cancelling task {task.get_name()}')
             task.cancel()
         self._loop.stop()
         save_config(self.state_file_path, data, create_missing=True)
         self.destroy()
 
     def _load_state(self) -> None:
         data = load_config(self.state_file_path, create_missing=True)
@@ -779,18 +903,22 @@
         type=Path,
         default=Path(default_config_path),
         help='Alterative path to config')
     parser.add_argument(
         '-v', '--verbose',
         action='store_true',
         help='Debug mode')
+    parser.add_argument(
+        '-s', '--safe-mode',
+        action='store_true',
+        help='Disables some perfomance featrues to avoid IO troubles')
 
     argcomplete.autocomplete(parser)
     return parser
 
 
 def main() -> None:
     locale.setlocale(locale.LC_TIME, locale.getlocale())
     args = get_argparser().parse_args()
     logging.basicConfig(level=logging.DEBUG if args.verbose else logging.WARNING)
-    app = Application(args.config_file, debug=args.verbose)
+    app = Application(args.config_file, debug=args.verbose, safe_mode=args.safe_mode)
     app.run()
```

### Comparing `pixelfeeder-0.1.0/pixelfeeder/pixelfed_uploader.py` & `pixelfeeder-0.1.1/pixelfeeder/pixelfed_uploader.py`

 * *Files identical despite different names*

### Comparing `pixelfeeder-0.1.0/pixelfeeder/tools.py` & `pixelfeeder-0.1.1/pixelfeeder/tools.py`

 * *Files identical despite different names*

### Comparing `pixelfeeder-0.1.0/pixelfeeder.egg-info/PKG-INFO` & `pixelfeeder-0.1.1/pixelfeeder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7069 7865  : 2.1.Name: pixe
 00000020: 6c66 6565 6465 720a 5665 7273 696f 6e3a  lfeeder.Version:
-00000030: 2030 2e31 2e30 0a53 756d 6d61 7279 3a20   0.1.0.Summary: 
+00000030: 2030 2e31 2e31 0a53 756d 6d61 7279 3a20   0.1.1.Summary: 
 00000040: 496d 706f 7274 2046 6c69 636b 7220 6461  Import Flickr da
 00000050: 7461 2069 6e74 6f20 6120 5069 7865 6c66  ta into a Pixelf
 00000060: 6564 2061 6363 6f75 6e74 0a48 6f6d 652d  ed account.Home-
 00000070: 7061 6765 3a20 6874 7470 733a 2f2f 6769  page: https://gi
 00000080: 746c 6162 2e63 6f6d 2f62 6572 6765 6e74  tlab.com/bergent
 00000090: 726f 6c6c 2f70 6978 656c 6665 6564 6572  roll/pixelfeeder
 000000a0: 0a41 7574 686f 723a 2041 6e74 6f6e 204b  .Author: Anton K
@@ -216,27 +216,28 @@
 00000d70: 6775 6d65 6e74 7320 7573 6520 7468 6520  guments use the 
 00000d80: 602d 6860 202f 2060 2d2d 6865 6c70 6020  `-h` / `--help` 
 00000d90: 666c 6167 2e0a 0a23 2320 4755 490a 0a60  flag...## GUI..`
 00000da0: 6060 7368 656c 6c0a 7069 7865 6c66 6565  ``shell.pixelfee
 00000db0: 6465 722d 6775 6920 5b2d 2d63 6f6e 6669  der-gui [--confi
 00000dc0: 672d 6669 6c65 2043 4f4e 4649 475f 4649  g-file CONFIG_FI
 00000dd0: 4c45 5d20 5b2d 2d76 6572 626f 7365 5d20  LE] [--verbose] 
-00000de0: 5b2d 2d68 656c 705d 0a60 6060 0a0a 4772  [--help].```..Gr
-00000df0: 6170 6869 6361 6c20 696e 7465 7266 6163  aphical interfac
-00000e00: 6520 6861 7320 6d6f 7374 6c79 2074 6865  e has mostly the
-00000e10: 2073 616d 6520 6f70 7469 6f6e 7320 6173   same options as
-00000e20: 2074 6865 2043 4c49 2c20 6275 7420 7570   the CLI, but up
-00000e30: 6f61 6473 2069 6d61 6765 730a 6f6e 652d  oads images.one-
-00000e40: 6279 2d6f 6e65 2069 6e20 696e 7465 7261  by-one in intera
-00000e50: 6374 6976 6520 6d6f 6465 2e20 5573 6572  ctive mode. User
-00000e60: 2061 626c 6520 746f 2063 6f72 7265 6374   able to correct
-00000e70: 2063 6170 7469 6f6e 2061 6e64 2076 6973   caption and vis
-00000e80: 6962 696c 6974 790a 6f66 2061 2070 6f73  ibility.of a pos
-00000e90: 742e 2054 6f6f 6c20 7769 6c6c 206b 6565  t. Tool will kee
-00000ea0: 7020 706f 7369 7469 6f6e 2062 6574 7765  p position betwe
-00000eb0: 656e 2073 6573 7369 6f6e 732e 0a0a 3e20  en sessions...> 
-00000ec0: 4564 6974 7320 6172 6520 6e6f 7420 7065  Edits are not pe
-00000ed0: 7273 6973 7465 6e74 2066 6f72 206e 6f77  rsistent for now
-00000ee0: 2c20 736f 2069 7420 6973 2062 6574 7465  , so it is bette
-00000ef0: 7220 746f 206d 616b 6520 636f 7272 6563  r to make correc
-00000f00: 7469 6f6e 7320 6a75 7374 0a3e 2062 6566  tions just.> bef
-00000f10: 6f72 6520 7570 6c6f 6164 696e 670a       ore uploading.
+00000de0: 5b2d 2d73 6166 652d 6d6f 6465 5d20 5b2d  [--safe-mode] [-
+00000df0: 2d68 656c 705d 0a60 6060 0a0a 4772 6170  -help].```..Grap
+00000e00: 6869 6361 6c20 696e 7465 7266 6163 6520  hical interface 
+00000e10: 6861 7320 6d6f 7374 6c79 2074 6865 2073  has mostly the s
+00000e20: 616d 6520 6f70 7469 6f6e 7320 6173 2074  ame options as t
+00000e30: 6865 2043 4c49 2c20 6275 7420 7570 6f61  he CLI, but upoa
+00000e40: 6473 2069 6d61 6765 730a 6f6e 652d 6279  ds images.one-by
+00000e50: 2d6f 6e65 2069 6e20 696e 7465 7261 6374  -one in interact
+00000e60: 6976 6520 6d6f 6465 2e20 5573 6572 2061  ive mode. User a
+00000e70: 626c 6520 746f 2063 6f72 7265 6374 2063  ble to correct c
+00000e80: 6170 7469 6f6e 2061 6e64 2076 6973 6962  aption and visib
+00000e90: 696c 6974 790a 6f66 2061 2070 6f73 742e  ility.of a post.
+00000ea0: 2054 6f6f 6c20 7769 6c6c 206b 6565 7020   Tool will keep 
+00000eb0: 706f 7369 7469 6f6e 2062 6574 7765 656e  position between
+00000ec0: 2073 6573 7369 6f6e 732e 0a0a 3e20 4564   sessions...> Ed
+00000ed0: 6974 7320 6172 6520 6e6f 7420 7065 7273  its are not pers
+00000ee0: 6973 7465 6e74 2066 6f72 206e 6f77 2c20  istent for now, 
+00000ef0: 736f 2069 7420 6973 2062 6574 7465 7220  so it is better 
+00000f00: 746f 206d 616b 6520 636f 7272 6563 7469  to make correcti
+00000f10: 6f6e 7320 6a75 7374 0a3e 2062 6566 6f72  ons just.> befor
+00000f20: 6520 7570 6c6f 6164 696e 670a            e uploading.
```

### Comparing `pixelfeeder-0.1.0/setup.py` & `pixelfeeder-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from setuptools import setup, find_packages
 
 here = Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name='pixelfeeder',
-    version='0.1.0',
+    version='0.1.1',
     author='Anton Karmanov',
     author_email='a.karmanov@inventati.org',
     python_requires='>=3.8',
     url='https://gitlab.com/bergentroll/pixelfeeder',
     description='Import Flickr data into a Pixelfed account',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

