# Comparing `tmp/ablerConfig-0.0.4-py3-none-any.whl.zip` & `tmp/ablerConfig-0.0.5.win32.zip`

## zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,162 +1,477 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                      2105 (0000000000000839h)
-  Actual end-cent-dir record offset:          2083 (0000000000000823h)
-  Expected end-cent-dir record offset:        2083 (0000000000000823h)
+  Zip archive file size:                      8637 (00000000000021BDh)
+  Actual end-cent-dir record offset:          8615 (00000000000021A7h)
+  Expected end-cent-dir record offset:        8615 (00000000000021A7h)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
-  central directory contains 5 entries.
-  The central directory is 397 (000000000000018Dh) bytes long,
+  central directory contains 16 entries.
+  The central directory is 1720 (00000000000006B8h) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 1686 (0000000000000696h).
+  is 6895 (0000000000001AEFh).
 
 
 Central directory entry #1:
 ---------------------------
 
-  ablerConfig/__init__.py
+  py-abler/
 
   offset of local header from start of archive:   0
                                                   (0000000000000000h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2023 Apr 24 07:37:56
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             9 characters
+  length of extra field:                          0 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             41FF00 hex
+  MS-DOS file attributes (10 hex):                dir 
+
+  There is no file comment.
+
+Central directory entry #2:
+---------------------------
+
+  py-abler/config/
+
+  offset of local header from start of archive:   39
+                                                  (0000000000000027h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2023 Apr 24 07:37:56
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             16 characters
+  length of extra field:                          0 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             41FF00 hex
+  MS-DOS file attributes (10 hex):                dir 
+
+  There is no file comment.
+
+Central directory entry #3:
+---------------------------
+
+  py-abler/config/venv/
+
+  offset of local header from start of archive:   85
+                                                  (0000000000000055h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2023 Apr 24 07:37:56
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             21 characters
+  length of extra field:                          0 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             41FF00 hex
+  MS-DOS file attributes (10 hex):                dir 
+
+  There is no file comment.
+
+Central directory entry #4:
+---------------------------
+
+  py-abler/config/venv/Lib/
+
+  offset of local header from start of archive:   136
+                                                  (0000000000000088h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2023 Apr 24 07:37:56
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             25 characters
+  length of extra field:                          0 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             41FF00 hex
+  MS-DOS file attributes (10 hex):                dir 
+
+  There is no file comment.
+
+Central directory entry #5:
+---------------------------
+
+  py-abler/config/venv/Lib/site-packages/
+
+  offset of local header from start of archive:   191
+                                                  (00000000000000BFh) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2023 Apr 24 07:37:56
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             39 characters
+  length of extra field:                          0 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             41FF00 hex
+  MS-DOS file attributes (10 hex):                dir 
+
+  There is no file comment.
+
+Central directory entry #6:
+---------------------------
+
+  py-abler/config/venv/Lib/site-packages/ablerConfig/
+
+  offset of local header from start of archive:   260
+                                                  (0000000000000104h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2023 Apr 24 07:37:56
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             51 characters
+  length of extra field:                          0 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             41FF00 hex
+  MS-DOS file attributes (10 hex):                dir 
+
+  There is no file comment.
+
+Central directory entry #7:
+---------------------------
+
+  py-abler/config/venv/Lib/site-packages/ablerConfig-0.0.5-py3.10.egg-info/
+
+  offset of local header from start of archive:   341
+                                                  (0000000000000155h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2023 Apr 24 07:37:56
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             73 characters
+  length of extra field:                          0 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             41FF00 hex
+  MS-DOS file attributes (10 hex):                dir 
+
+  There is no file comment.
+
+Central directory entry #8:
+---------------------------
+
+  py-abler/config/venv/Lib/site-packages/ablerConfig/__pycache__/
+
+  offset of local header from start of archive:   444
+                                                  (00000000000001BCh) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2023 Apr 24 07:37:56
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             63 characters
+  length of extra field:                          0 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             41FF00 hex
+  MS-DOS file attributes (10 hex):                dir 
+
+  There is no file comment.
+
+Central directory entry #9:
+---------------------------
+
+  py-abler/config/venv/Lib/site-packages/ablerConfig/__init__.py
+
+  offset of local header from start of archive:   537
+                                                  (0000000000000219h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Apr 23 23:22:00
+  file last modified on (DOS date/time):          2023 Apr 24 07:22:00
   32-bit CRC value (hex):                         b29b35a6
   compressed size:                                15 bytes
   uncompressed size:                              13 bytes
-  length of filename:                             23 characters
+  length of filename:                             62 characters
   length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             81B600 hex
   MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
-Central directory entry #2:
+Central directory entry #10:
 ---------------------------
 
-  ablerConfig-0.0.4.dist-info/METADATA
+  py-abler/config/venv/Lib/site-packages/ablerConfig/__pycache__/__init__.cpython-310.pyc
 
-  offset of local header from start of archive:   68
-                                                  (0000000000000044h) bytes
+  offset of local header from start of archive:   644
+                                                  (0000000000000284h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Apr 23 23:31:56
-  32-bit CRC value (hex):                         20a74c67
-  compressed size:                                992 bytes
-  uncompressed size:                              2050 bytes
-  length of filename:                             36 characters
+  file last modified on (DOS date/time):          2023 Apr 24 07:37:56
+  32-bit CRC value (hex):                         1fc44131
+  compressed size:                                133 bytes
+  uncompressed size:                              174 bytes
+  length of filename:                             87 characters
   length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             81B600 hex
   MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
-Central directory entry #3:
+Central directory entry #11:
 ---------------------------
 
-  ablerConfig-0.0.4.dist-info/WHEEL
+  py-abler/config/venv/Lib/site-packages/ablerConfig-0.0.5-py3.10.egg-info/dependency_links.txt
 
-  offset of local header from start of archive:   1126
-                                                  (0000000000000466h) bytes
+  offset of local header from start of archive:   894
+                                                  (000000000000037Eh) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Apr 23 23:31:56
-  32-bit CRC value (hex):                         cb21a249
-  compressed size:                                92 bytes
-  uncompressed size:                              92 bytes
-  length of filename:                             33 characters
+  file last modified on (DOS date/time):          2023 Apr 24 07:37:56
+  32-bit CRC value (hex):                         32d70693
+  compressed size:                                3 bytes
+  uncompressed size:                              1 bytes
+  length of filename:                             93 characters
   length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             81B600 hex
   MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
-Central directory entry #4:
+Central directory entry #12:
 ---------------------------
 
-  ablerConfig-0.0.4.dist-info/top_level.txt
+  py-abler/config/venv/Lib/site-packages/ablerConfig-0.0.5-py3.10.egg-info/PKG-INFO
 
-  offset of local header from start of archive:   1281
-                                                  (0000000000000501h) bytes
+  offset of local header from start of archive:   1020
+                                                  (00000000000003FCh) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Apr 23 23:31:56
-  32-bit CRC value (hex):                         caa12840
-  compressed size:                                14 bytes
-  uncompressed size:                              12 bytes
-  length of filename:                             41 characters
+  file last modified on (DOS date/time):          2023 Apr 24 07:37:56
+  32-bit CRC value (hex):                         e82d0b8b
+  compressed size:                                983 bytes
+  uncompressed size:                              2004 bytes
+  length of filename:                             81 characters
   length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             81B600 hex
   MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
-Central directory entry #5:
+Central directory entry #13:
+---------------------------
+
+  py-abler/config/venv/Lib/site-packages/ablerConfig-0.0.5-py3.10.egg-info/requires.txt
+
+  offset of local header from start of archive:   2114
+                                                  (0000000000000842h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2023 Apr 24 07:37:56
+  32-bit CRC value (hex):                         0af5971d
+  compressed size:                                11 bytes
+  uncompressed size:                              14 bytes
+  length of filename:                             85 characters
+  length of extra field:                          0 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             81B600 hex
+  MS-DOS file attributes (00 hex):                none
+
+  There is no file comment.
+
+Central directory entry #14:
+---------------------------
+
+  py-abler/config/venv/Lib/site-packages/ablerConfig-0.0.5-py3.10.egg-info/SOURCES.txt
+
+  offset of local header from start of archive:   2240
+                                                  (00000000000008C0h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2023 Apr 24 07:37:56
+  32-bit CRC value (hex):                         bf303e26
+  compressed size:                                113 bytes
+  uncompressed size:                              216 bytes
+  length of filename:                             84 characters
+  length of extra field:                          0 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             81B600 hex
+  MS-DOS file attributes (00 hex):                none
+
+  There is no file comment.
+
+Central directory entry #15:
 ---------------------------
 
-  ablerConfig-0.0.4.dist-info/RECORD
+  py-abler/config/venv/Lib/site-packages/ablerConfig-0.0.5-py3.10.egg-info/top_level.txt
 
-  offset of local header from start of archive:   1366
-                                                  (0000000000000556h) bytes
+  offset of local header from start of archive:   2467
+                                                  (00000000000009A3h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Apr 23 23:31:56
-  32-bit CRC value (hex):                         a7730098
-  compressed size:                                256 bytes
-  uncompressed size:                              392 bytes
-  length of filename:                             34 characters
+  file last modified on (DOS date/time):          2023 Apr 24 07:37:56
+  32-bit CRC value (hex):                         caa12840
+  compressed size:                                14 bytes
+  uncompressed size:                              12 bytes
+  length of filename:                             86 characters
   length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  non-MSDOS external file attributes:             81B400 hex
+  non-MSDOS external file attributes:             81B600 hex
   MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
+Central directory entry #16:
+---------------------------
+
+  py-abler/config/venv/Lib/site-packages/ablerConfig/__pycache__/config.pyc
+
+  offset of local header from start of archive:   2597
+                                                  (0000000000000A25h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   3.1
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2023 Apr 24 07:31:00
+  32-bit CRC value (hex):                         cc23157f
+  compressed size:                                4195 bytes
+  uncompressed size:                              8631 bytes
+  length of filename:                             73 characters
+  length of extra field:                          36 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             000000 hex
+  MS-DOS file attributes (20 hex):                arc 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x000a (PKWARE Win32) and 32 data bytes.  The first
+    20 are:   00 00 00 00 01 00 18 00 42 7c 68 aa 3b 76 d9 01 42 7c 68 aa.
+
+  There is no file comment.
+
```

## zipnote {}

```diff
@@ -1,16 +1,49 @@
-Filename: ablerConfig/__init__.py
+Filename: py-abler/
 Comment: 
 
-Filename: ablerConfig-0.0.4.dist-info/METADATA
+Filename: py-abler/config/
 Comment: 
 
-Filename: ablerConfig-0.0.4.dist-info/WHEEL
+Filename: py-abler/config/venv/
 Comment: 
 
-Filename: ablerConfig-0.0.4.dist-info/top_level.txt
+Filename: py-abler/config/venv/Lib/
 Comment: 
 
-Filename: ablerConfig-0.0.4.dist-info/RECORD
+Filename: py-abler/config/venv/Lib/site-packages/
+Comment: 
+
+Filename: py-abler/config/venv/Lib/site-packages/ablerConfig/
+Comment: 
+
+Filename: py-abler/config/venv/Lib/site-packages/ablerConfig-0.0.5-py3.10.egg-info/
+Comment: 
+
+Filename: py-abler/config/venv/Lib/site-packages/ablerConfig/__pycache__/
+Comment: 
+
+Filename: py-abler/config/venv/Lib/site-packages/ablerConfig/__init__.py
+Comment: 
+
+Filename: py-abler/config/venv/Lib/site-packages/ablerConfig/__pycache__/__init__.cpython-310.pyc
+Comment: 
+
+Filename: py-abler/config/venv/Lib/site-packages/ablerConfig-0.0.5-py3.10.egg-info/dependency_links.txt
+Comment: 
+
+Filename: py-abler/config/venv/Lib/site-packages/ablerConfig-0.0.5-py3.10.egg-info/PKG-INFO
+Comment: 
+
+Filename: py-abler/config/venv/Lib/site-packages/ablerConfig-0.0.5-py3.10.egg-info/requires.txt
+Comment: 
+
+Filename: py-abler/config/venv/Lib/site-packages/ablerConfig-0.0.5-py3.10.egg-info/SOURCES.txt
+Comment: 
+
+Filename: py-abler/config/venv/Lib/site-packages/ablerConfig-0.0.5-py3.10.egg-info/top_level.txt
+Comment: 
+
+Filename: py-abler/config/venv/Lib/site-packages/ablerConfig/__pycache__/config.pyc
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## Comparing `ablerConfig-0.0.4.dist-info/METADATA` & `py-abler/config/venv/Lib/site-packages/ablerConfig-0.0.5-py3.10.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ablerConfig
-Version: 0.0.4
+Version: 0.0.5
 Summary: 配置信息处理包
 Home-page: https://github.com/hanlaohan/abler-config
 Author: 憨老汉
 Author-email: hh28642257@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -12,16 +12,14 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Requires-Dist: pyjson5
-Requires-Dist: json5
 
 ablerConfig
 =============
 
 简介
 --
```

