# Comparing `tmp/genshin_account_switcher-1.2.1-py3-none-any.whl.zip` & `tmp/genshin_account_switcher-1.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 20178 bytes, number of entries: 13
--rw-r--r--  2.0 unx        0 b- defN 22-Nov-26 07:46 src/__init__.py
--rw-r--r--  2.0 unx     3237 b- defN 22-Nov-27 12:00 src/config.py
--rw-r--r--  2.0 unx     4133 b- defN 22-Nov-27 12:02 src/gui.py
--rw-r--r--  2.0 unx     5311 b- defN 22-Nov-27 12:00 src/main.py
--rw-r--r--  2.0 unx      855 b- defN 22-Nov-27 12:02 src/utils.py
--rw-r--r--  2.0 unx     1350 b- defN 22-Nov-26 09:00 src/genshin/__init__.py
--rw-r--r--  2.0 unx     2428 b- defN 22-Nov-26 09:00 src/genshin/linux.py
--rw-r--r--  2.0 unx    34227 b- defN 22-Nov-27 12:10 genshin_account_switcher-1.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     2360 b- defN 22-Nov-27 12:10 genshin_account_switcher-1.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Nov-27 12:10 genshin_account_switcher-1.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       59 b- defN 22-Nov-27 12:10 genshin_account_switcher-1.2.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       16 b- defN 22-Nov-27 12:10 genshin_account_switcher-1.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1083 b- defN 22-Nov-27 12:10 genshin_account_switcher-1.2.1.dist-info/RECORD
-13 files, 55151 bytes uncompressed, 18358 bytes compressed:  66.7%
+Zip file size: 20163 bytes, number of entries: 13
+-rw-r--r--  2.0 unx        0 b- defN 22-Nov-25 14:58 src/__init__.py
+-rw-r--r--  2.0 unx     3237 b- defN 22-Nov-28 06:31 src/config.py
+-rw-r--r--  2.0 unx     4133 b- defN 22-Nov-28 06:31 src/gui.py
+-rw-r--r--  2.0 unx     5311 b- defN 22-Nov-28 06:31 src/main.py
+-rw-r--r--  2.0 unx      855 b- defN 22-Nov-28 06:31 src/utils.py
+-rw-r--r--  2.0 unx     1350 b- defN 22-Nov-28 06:31 src/genshin/__init__.py
+-rw-r--r--  2.0 unx     2283 b- defN 23-Apr-24 10:48 src/genshin/linux.py
+-rw-r--r--  2.0 unx    34227 b- defN 23-Apr-24 10:51 genshin_account_switcher-1.2.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2360 b- defN 23-Apr-24 10:51 genshin_account_switcher-1.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-24 10:51 genshin_account_switcher-1.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       59 b- defN 23-Apr-24 10:51 genshin_account_switcher-1.2.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       16 b- defN 23-Apr-24 10:51 genshin_account_switcher-1.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1083 b- defN 23-Apr-24 10:51 genshin_account_switcher-1.2.2.dist-info/RECORD
+13 files, 55006 bytes uncompressed, 18343 bytes compressed:  66.7%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: src/genshin/__init__.py
 Comment: 
 
 Filename: src/genshin/linux.py
 Comment: 
 
-Filename: genshin_account_switcher-1.2.1.dist-info/LICENSE
+Filename: genshin_account_switcher-1.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: genshin_account_switcher-1.2.1.dist-info/METADATA
+Filename: genshin_account_switcher-1.2.2.dist-info/METADATA
 Comment: 
 
-Filename: genshin_account_switcher-1.2.1.dist-info/WHEEL
+Filename: genshin_account_switcher-1.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: genshin_account_switcher-1.2.1.dist-info/entry_points.txt
+Filename: genshin_account_switcher-1.2.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: genshin_account_switcher-1.2.1.dist-info/top_level.txt
+Filename: genshin_account_switcher-1.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: genshin_account_switcher-1.2.1.dist-info/RECORD
+Filename: genshin_account_switcher-1.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## src/genshin/linux.py

```diff
@@ -1,24 +1,18 @@
 """Module for finding and interacting with the Linux Genshin Impact
 installation"""
-from os import getlogin
+from getpass import getuser
 from pathlib import Path
 from typing import List, Optional
 
 _GENSHIN_LOCATIONS = [
     # Anime Game Launcher
-    "~/.local/share/anime-game-launcher/game",
-    # Anime Game Launcher GTK
-    "~/.local/share/anime-game-launcher-gtk/game",
-    # Anime Game Launcher GTK - Flatpak
-    "~/.var/app/moe.launcher.an-anime-game-launcher-gtk/data/"
-    "anime-game-launcher/game",
+    "~/.local/share/anime-game-launcher/Genshin Impact",
     # Anime Game Launcher - Flatpak
-    "~/.var/app/com.gitlab.KRypt0n_.an-anime-game-launcher/data/"
-    "anime-game-launcher/game",
+    "~/.var/app/moe.launcher.an-anime-game-launcher/data/anime-game-launcher/Genshin Impact",
 ]
 
 _USER_REG_PATH = "user.reg"
 _UID_INFO_FILE = "drive_c/users/%s/AppData/LocalLow/miHoYo/" \
                  "Genshin Impact/UidInfo.txt"
 
 
@@ -45,30 +39,30 @@
 def get_uid() -> Optional[str]:
     """ Get the UID of the current installation """
     install_dir = _get_install_dir()
 
     if install_dir is None:
         return None
 
-    uid_path = Path(install_dir, _UID_INFO_FILE % getlogin())
+    uid_path = Path(install_dir, _UID_INFO_FILE % _get_username())
 
     if not uid_path.exists():
         return None
 
     return uid_path.read_text(encoding="utf8").strip()
 
 
 def write_uid(uid: str) -> None:
     """ Write a UID to the UidInfo.txt file """
     install_dir = _get_install_dir()
 
     if install_dir is None:
         return
 
-    uid_path = Path(install_dir, _UID_INFO_FILE % getlogin())
+    uid_path = Path(install_dir, _UID_INFO_FILE % _get_username())
     uid_path.write_text(f"{uid}\n", encoding="utf8")
 
 
 def read_user_registry() -> Optional[bytes]:
     """ Read the user registry """
     install_dir = _get_install_dir()
 
@@ -88,7 +82,11 @@
     install_dir = _get_install_dir()
 
     if install_dir is None:
         return
 
     user_reg_path = Path(install_dir, _USER_REG_PATH)
     user_reg_path.write_bytes(data)
+
+
+def _get_username() -> str:
+    return getuser()
```

## Comparing `genshin_account_switcher-1.2.1.dist-info/LICENSE` & `genshin_account_switcher-1.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `genshin_account_switcher-1.2.1.dist-info/METADATA` & `genshin_account_switcher-1.2.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genshin-account-switcher
-Version: 1.2.1
+Version: 1.2.2
 Summary: Simple account switcher for Genshin Impact on Linux.
 Home-page: https://github.com/atomicptr/genshin-account-switcher
 Author: Christopher Kaster
 Author-email: me@atomicptr.de
 Classifier: Topic :: Games/Entertainment
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

## Comparing `genshin_account_switcher-1.2.1.dist-info/RECORD` & `genshin_account_switcher-1.2.2.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 src/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 src/config.py,sha256=pI9w8DYO_bgLQuufcL0dxLxya-hv7eLshdc_n8KWPgU,3237
 src/gui.py,sha256=kB2Aabc2evwVgEbAryre28BXC31fOwuPodWZgNQO7mE,4133
 src/main.py,sha256=9-wSZEsL9hL0hCt8hboBPELdkLepnUZBbQ17UmEXquY,5311
 src/utils.py,sha256=rnM-XvbABxEotJG6tD2zkmMsHZUy3WHkV7rS_Z3Ifh0,855
 src/genshin/__init__.py,sha256=7fN7nBjSSrLZyOH8ZJCEmtdxwCUmOJsDZOomyQ10MvM,1350
-src/genshin/linux.py,sha256=FGnctNrvitQ2T0HnD3WR-wfPh1LgmuxCejq8rOMe-qc,2428
-genshin_account_switcher-1.2.1.dist-info/LICENSE,sha256=mYluISwUlRhyOocFBuQndyF5ZKqTzDtalcVTCKd34gE,34227
-genshin_account_switcher-1.2.1.dist-info/METADATA,sha256=lt7Dh7Es_cczPP5YCCtn-8mNhE5p4--xVO5tjI7FTqw,2360
-genshin_account_switcher-1.2.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-genshin_account_switcher-1.2.1.dist-info/entry_points.txt,sha256=iuwGgE_yEg3wr_SHe-cFzvBwxTSbWhEwNy4OY8RgUUk,59
-genshin_account_switcher-1.2.1.dist-info/top_level.txt,sha256=YcVwFNe982fxcRix5gdyyDT02HWGy1VVPKQRfmf7B1I,16
-genshin_account_switcher-1.2.1.dist-info/RECORD,,
+src/genshin/linux.py,sha256=vO271ptXgHrNOdXr384XGQQPJqoNeb06-0c34rJmdhE,2283
+genshin_account_switcher-1.2.2.dist-info/LICENSE,sha256=mYluISwUlRhyOocFBuQndyF5ZKqTzDtalcVTCKd34gE,34227
+genshin_account_switcher-1.2.2.dist-info/METADATA,sha256=0pDwR7yhZVqcduyg6Im6waUPRUEBjBjL1bbmmlw0Goo,2360
+genshin_account_switcher-1.2.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+genshin_account_switcher-1.2.2.dist-info/entry_points.txt,sha256=iuwGgE_yEg3wr_SHe-cFzvBwxTSbWhEwNy4OY8RgUUk,59
+genshin_account_switcher-1.2.2.dist-info/top_level.txt,sha256=YcVwFNe982fxcRix5gdyyDT02HWGy1VVPKQRfmf7B1I,16
+genshin_account_switcher-1.2.2.dist-info/RECORD,,
```

