# Comparing `tmp/PgsFile-0.0.6.tar.gz` & `tmp/PgsFile-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PgsFile-0.0.6.tar", last modified: Thu Apr  6 00:52:10 2023, max compression
+gzip compressed data, was "dist\PgsFile-0.0.7.tar", last modified: Mon Apr 24 07:38:07 2023, max compression
```

## Comparing `PgsFile-0.0.6.tar` & `PgsFile-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 00:52:10.000000 PgsFile-0.0.6/
--rw-rw-rw-   0        0        0     1138 2023-03-21 12:26:03.000000 PgsFile-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     1463 2023-04-06 00:52:10.000000 PgsFile-0.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-06 00:52:10.000000 PgsFile-0.0.6/PgsFile/
--rw-rw-rw-   0        0        0    15424 2023-04-06 00:45:45.000000 PgsFile-0.0.6/PgsFile/PgsFile.py
--rw-rw-rw-   0        0        0      599 2023-03-26 14:50:14.000000 PgsFile-0.0.6/PgsFile/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-06 00:52:10.000000 PgsFile-0.0.6/PgsFile.egg-info/
--rw-rw-rw-   0        0        0     1463 2023-04-06 00:52:10.000000 PgsFile-0.0.6/PgsFile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      189 2023-04-06 00:52:10.000000 PgsFile-0.0.6/PgsFile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 00:52:10.000000 PgsFile-0.0.6/PgsFile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-06 00:52:10.000000 PgsFile-0.0.6/PgsFile.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1018 2023-03-22 02:43:11.000000 PgsFile-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-04-06 00:52:10.000000 PgsFile-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      735 2023-04-06 00:49:37.000000 PgsFile-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 07:38:07.000000 PgsFile-0.0.7/
+-rw-rw-rw-   0        0        0     1138 2023-03-21 12:26:03.000000 PgsFile-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     1526 2023-04-24 07:38:07.000000 PgsFile-0.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-24 07:38:07.000000 PgsFile-0.0.7/PgsFile/
+-rw-rw-rw-   0        0        0    17173 2023-04-24 07:35:43.000000 PgsFile-0.0.7/PgsFile/PgsFile.py
+-rw-rw-rw-   0        0        0      637 2023-04-24 07:28:17.000000 PgsFile-0.0.7/PgsFile/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 07:38:07.000000 PgsFile-0.0.7/PgsFile.egg-info/
+-rw-rw-rw-   0        0        0     1526 2023-04-24 07:38:06.000000 PgsFile-0.0.7/PgsFile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2023-04-24 07:38:06.000000 PgsFile-0.0.7/PgsFile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 07:38:06.000000 PgsFile-0.0.7/PgsFile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-24 07:38:06.000000 PgsFile-0.0.7/PgsFile.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1068 2023-04-24 07:05:46.000000 PgsFile-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-24 07:38:07.000000 PgsFile-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      748 2023-04-24 07:30:15.000000 PgsFile-0.0.7/setup.py
```

### Comparing `PgsFile-0.0.6/LICENSE` & `PgsFile-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `PgsFile-0.0.6/PKG-INFO` & `PgsFile-0.0.7/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: PgsFile
-Version: 0.0.6
-Summary: To make file operations coding easier for literary students
+Version: 0.0.7
+Summary: To make file operations and wordlist coding easier for literary students
 Home-page:  
 Author: Pan Guisheng
 Author-email: 895284504@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Free For Educational Use
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Purpose: This module is to facilitate Python beginners, especially instructors and students of foreign languages and literature, for the convenience of easily operating txt, xlsx and json files. 
+Purpose: This module is to facilitate Python beginners, especially instructors and students of foreign languages and literature, for the convenience of easily operating txt, xlsx and json files as well as making word list. 
 
 Function 1: Useful for getting data from the files directly and saving processing results in the files. Either task can be done with a single line of code.
 
 Function 2: The functions of "FilePath" and "FileName" imported from the py file can effectively help you get all the absolute file paths in any folder (containing all the files of any sub-folder in the folder) of your PC disk and obtain the file names. This will be also realized within one line of code.
 
-Function 3: You can make a word list of a certain file or a batch of files, showing their word frequency sorted in reverse order, easily with the function of "word_list" in PgsFile.
+Function 3: You can make a word list of a certain file or a batch of files, showing their word frequency sorted in reverse order, easily with the function of "word_list" and "batch_word_list" in PgsFile.
 
 Author: Pan Guisheng, a PhD student at the Graduate Institute of Interpretation and Translation of Shanghai International Studies University
 E-mail: 895284504@qq.com
```

### Comparing `PgsFile-0.0.6/PgsFile/PgsFile.py` & `PgsFile-0.0.7/PgsFile/PgsFile.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,957 +8,1067 @@
 00000070: 6620 6765 745f 6461 7461 5f74 6578 7428  f get_data_text(
 00000080: 7061 7468 293a 0d0a 2020 2020 2727 270d  path):..    '''.
 00000090: 0a20 2020 2050 6172 616d 6574 6572 730d  .    Parameters.
 000000a0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d  .    ----------.
 000000b0: 0a20 2020 2070 6174 6820 3a20 5459 5045  .    path : TYPE
 000000c0: 2073 7472 696e 670d 0a20 2020 2020 2020   string..       
 000000d0: 2044 4553 4352 4950 5449 4f4e 2e20 0d0a   DESCRIPTION. ..
-000000e0: 0909 5573 696e 6720 7061 7468 2074 6f20  ..Using path to 
-000000f0: 6765 7420 6461 7461 2066 726f 6d20 6120  get data from a 
-00000100: 7369 6e67 6c65 2074 7874 2066 696c 652e  single txt file.
-00000110: 2065 672e 2044 3a2f 2f72 6177 5f74 6578   eg. D://raw_tex
-00000120: 742e 7478 740d 0a20 2020 2020 2020 2054  t.txt..        T
-00000130: 6865 6f72 6574 6963 616c 6c79 2c20 6974  heoretically, it
-00000140: 2073 7570 706f 7274 7320 616c 6c20 7468   supports all th
-00000150: 6520 7465 7874 2065 6e63 6f64 696e 6720  e text encoding 
-00000160: 666f 726d 6174 732c 206c 696b 6520 7574  formats, like ut
-00000170: 662d 382c 2075 6e69 636f 6465 2c20 616e  f-8, unicode, an
-00000180: 7369 2c20 6762 6b20 6574 632e 0d0a 0d0a  si, gbk etc.....
-00000190: 2020 2020 5265 7475 726e 730d 0a20 2020      Returns..   
-000001a0: 202d 2d2d 2d2d 2d2d 0d0a 2020 2020 7465   -------..    te
-000001b0: 7874 203a 2054 5950 4520 7374 7269 6e67  xt : TYPE string
-000001c0: 0d0a 2020 2020 2020 2020 4445 5343 5249  ..        DESCRI
-000001d0: 5054 494f 4e2e 200d 0a09 0949 7420 7265  PTION. ....It re
-000001e0: 7475 726e 7320 616c 6c20 7468 6520 7465  turns all the te
-000001f0: 7874 2063 6f6e 7465 6e74 2066 726f 6d20  xt content from 
-00000200: 7468 6520 7461 7267 6574 2066 696c 652e  the target file.
-00000210: 0d0a 0d0a 2020 2020 2727 270d 0a20 2020  ....    '''..   
-00000220: 2069 6d70 6f72 7420 6368 6172 6465 740d   import chardet.
-00000230: 0a20 2020 2070 6174 683d 7061 7468 2e72  .    path=path.r
-00000240: 6570 6c61 6365 2822 5c6e 222c 2222 290d  eplace("\n","").
-00000250: 0a20 2020 2066 3d6f 7065 6e28 7061 7468  .    f=open(path
-00000260: 2c27 7262 2729 2020 0d0a 2020 2020 6461  ,'rb')  ..    da
-00000270: 7461 3d66 2e72 6561 6428 2920 200d 0a20  ta=f.read()  .. 
-00000280: 2020 2066 2e63 6c6f 7365 2829 0d0a 2020     f.close()..  
-00000290: 2020 6669 6c65 5f65 6e63 6f64 696e 673d    file_encoding=
-000002a0: 6368 6172 6465 742e 6465 7465 6374 2864  chardet.detect(d
-000002b0: 6174 6129 2e67 6574 2827 656e 636f 6469  ata).get('encodi
-000002c0: 6e67 2729 2020 0d0a 2020 2020 6631 3d6f  ng')  ..    f1=o
-000002d0: 7065 6e28 7061 7468 2c27 7227 2c20 656e  pen(path,'r', en
-000002e0: 636f 6469 6e67 3d66 696c 655f 656e 636f  coding=file_enco
-000002f0: 6469 6e67 2c20 6572 726f 7273 3d27 6967  ding, errors='ig
-00000300: 6e6f 7265 2729 2020 0d0a 2020 2020 7465  nore')  ..    te
-00000310: 7874 3d66 312e 7265 6164 2829 2e72 6570  xt=f1.read().rep
-00000320: 6c61 6365 2822 e280 9922 2c22 2722 290d  lace("...","'").
-00000330: 0a20 2020 2066 312e 636c 6f73 6528 290d  .    f1.close().
-00000340: 0a20 2020 2072 6574 7572 6e20 7465 7874  .    return text
-00000350: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
-00000360: 6465 6620 6765 745f 6461 7461 5f6c 696e  def get_data_lin
-00000370: 6573 2870 6174 6829 3a0d 0a20 2020 2027  es(path):..    '
-00000380: 2727 0d0a 2020 2020 5061 7261 6d65 7465  ''..    Paramete
-00000390: 7273 0d0a 2020 2020 2d2d 2d2d 2d2d 2d2d  rs..    --------
-000003a0: 2d2d 0d0a 2020 2020 7061 7468 203a 2054  --..    path : T
-000003b0: 5950 4520 7374 7269 6e67 0d0a 2020 2020  YPE string..    
-000003c0: 2020 2020 4445 5343 5249 5054 494f 4e2e      DESCRIPTION.
-000003d0: 0d0a 0909 5573 696e 6720 7061 7468 2074  ....Using path t
-000003e0: 6f20 6765 7420 6461 7461 2066 726f 6d20  o get data from 
-000003f0: 6120 7369 6e67 6c65 2074 7874 2066 696c  a single txt fil
-00000400: 652e 2065 672e 2044 3a2f 2f72 6177 5f74  e. eg. D://raw_t
-00000410: 6578 742e 7478 7420 2020 2020 0d0a 0909  ext.txt     ....
-00000420: 5468 656f 7265 7469 6361 6c6c 792c 2069  Theoretically, i
-00000430: 7420 7375 7070 6f72 7473 2061 6c6c 2074  t supports all t
-00000440: 6865 2074 6578 7420 656e 636f 6469 6e67  he text encoding
-00000450: 2066 6f72 6d61 7473 2c20 6c69 6b65 2075   formats, like u
-00000460: 7466 2d38 2c20 756e 6963 6f64 652c 2061  tf-8, unicode, a
-00000470: 6e73 692c 2067 626b 2065 7463 2e0d 0a0d  nsi, gbk etc....
-00000480: 0a20 2020 2052 6574 7572 6e73 0d0a 2020  .    Returns..  
-00000490: 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020 206c    -------..    l
-000004a0: 696e 6573 203a 2054 5950 4520 6c69 7374  ines : TYPE list
-000004b0: 0d0a 2020 2020 2020 2020 4445 5343 5249  ..        DESCRI
-000004c0: 5054 494f 4e2e 200d 0a09 0949 7420 7265  PTION. ....It re
-000004d0: 7475 726e 7320 6120 6c69 7374 2063 6f6e  turns a list con
-000004e0: 7461 696e 696e 6720 616c 6c20 7468 6520  taining all the 
-000004f0: 7061 7261 6772 6170 6873 206f 6620 7468  paragraphs of th
-00000500: 6520 7461 7267 6574 2066 696c 652e 0d0a  e target file...
-00000510: 0d0a 2020 2020 2727 270d 0a20 2020 2069  ..    '''..    i
-00000520: 6d70 6f72 7420 6368 6172 6465 740d 0a20  mport chardet.. 
-00000530: 2020 2070 6174 683d 7061 7468 2e72 6570     path=path.rep
-00000540: 6c61 6365 2822 5c6e 222c 2222 290d 0a20  lace("\n","").. 
-00000550: 2020 2066 3d6f 7065 6e28 7061 7468 2c27     f=open(path,'
-00000560: 7262 2729 2020 0d0a 2020 2020 6461 7461  rb')  ..    data
-00000570: 3d66 2e72 6561 6428 2920 200d 0a20 2020  =f.read()  ..   
-00000580: 2066 2e63 6c6f 7365 2829 0d0a 2020 2020   f.close()..    
-00000590: 6669 6c65 5f65 6e63 6f64 696e 673d 6368  file_encoding=ch
-000005a0: 6172 6465 742e 6465 7465 6374 2864 6174  ardet.detect(dat
-000005b0: 6129 2e67 6574 2827 656e 636f 6469 6e67  a).get('encoding
-000005c0: 2729 2020 0d0a 2020 2020 6631 3d6f 7065  ')  ..    f1=ope
-000005d0: 6e28 7061 7468 2c27 7227 2c20 656e 636f  n(path,'r', enco
-000005e0: 6469 6e67 3d66 696c 655f 656e 636f 6469  ding=file_encodi
-000005f0: 6e67 2c20 6572 726f 7273 3d27 6967 6e6f  ng, errors='igno
-00000600: 7265 2729 2020 0d0a 2020 2020 6c69 6e65  re')  ..    line
-00000610: 733d 6631 2e72 6561 646c 696e 6573 2829  s=f1.readlines()
-00000620: 0d0a 2020 2020 6c69 6e65 733d 5b6c 2e72  ..    lines=[l.r
-00000630: 6570 6c61 6365 2822 e280 9922 2c22 2722  eplace("...","'"
-00000640: 2920 666f 7220 6c20 696e 206c 696e 6573  ) for l in lines
-00000650: 2069 6620 6c65 6e28 6c2e 7374 7269 7028   if len(l.strip(
-00000660: 2929 2021 3d30 5d0d 0a20 2020 2066 312e  )) !=0]..    f1.
-00000670: 636c 6f73 6528 290d 0a20 2020 2072 6574  close()..    ret
-00000680: 7572 6e20 6c69 6e65 730d 0a0d 0a64 6566  urn lines....def
-00000690: 2077 7269 7465 5f74 6f5f 7478 7428 6669   write_to_txt(fi
-000006a0: 6c65 5f70 6174 682c 7465 7874 2c6d 6f64  le_path,text,mod
-000006b0: 653d 4e6f 6e65 2c65 6e63 6f64 696e 673d  e=None,encoding=
-000006c0: 4e6f 6e65 293a 0d0a 2020 2020 2727 270d  None):..    '''.
-000006d0: 0a20 2020 2050 6172 616d 6574 6572 730d  .    Parameters.
-000006e0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d  .    ----------.
-000006f0: 0a20 2020 2066 696c 655f 7061 7468 203a  .    file_path :
-00000700: 2054 5950 4520 7374 7269 6e67 0d0a 2020   TYPE string..  
-00000710: 2020 2020 2020 4445 5343 5249 5054 494f        DESCRIPTIO
-00000720: 4e2e 0d0a 2020 2020 7465 7874 203a 2054  N...    text : T
-00000730: 5950 450d 0a20 2020 2020 2020 2044 4553  YPE..        DES
-00000740: 4352 4950 5449 4f4e 2e20 7374 7269 6e67  CRIPTION. string
-00000750: 0d0a 2020 2020 6d6f 6465 203a 2054 5950  ..    mode : TYP
-00000760: 452c 206f 7074 696f 6e61 6c20 2320 773b  E, optional # w;
-00000770: 612b 0d0a 2020 2020 2020 2020 4445 5343  a+..        DESC
-00000780: 5249 5054 494f 4e2e 2054 6865 2064 6566  RIPTION. The def
-00000790: 6175 6c74 2069 7320 4e6f 6e65 2e0d 0a20  ault is None... 
-000007a0: 2020 2065 6e63 6f64 696e 6720 3a20 5459     encoding : TY
-000007b0: 5045 2c20 6f70 7469 6f6e 616c 2023 2075  PE, optional # u
-000007c0: 7466 2d38 0d0a 2020 2020 2020 2020 4445  tf-8..        DE
-000007d0: 5343 5249 5054 494f 4e2e 2054 6865 2064  SCRIPTION. The d
-000007e0: 6566 6175 6c74 2069 7320 4e6f 6e65 2e0d  efault is None..
-000007f0: 0a0d 0a20 2020 2052 6574 7572 6e73 0d0a  ...    Returns..
-00000800: 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020      -------..   
-00000810: 204e 6f6e 652e 0d0a 0d0a 2020 2020 2727   None.....    ''
-00000820: 270d 0a20 2020 2069 6620 6d6f 6465 2069  '..    if mode i
-00000830: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
-00000840: 206d 6f64 653d 2277 220d 0a20 2020 2065   mode="w"..    e
-00000850: 6c73 653a 0d0a 2020 2020 2020 2020 6d6f  lse:..        mo
-00000860: 6465 3d6d 6f64 650d 0a20 2020 2069 6620  de=mode..    if 
-00000870: 656e 636f 6469 6e67 2069 7320 4e6f 6e65  encoding is None
-00000880: 3a0d 0a20 2020 2020 2020 2065 6e63 6f64  :..        encod
-00000890: 696e 673d 2275 7466 2d38 220d 0a20 2020  ing="utf-8"..   
-000008a0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-000008b0: 656e 636f 6469 6e67 3d65 6e63 6f64 696e  encoding=encodin
-000008c0: 6720 2020 200d 0a20 2020 2066 3d6f 7065  g    ..    f=ope
-000008d0: 6e28 6669 6c65 5f70 6174 682c 6d6f 6465  n(file_path,mode
-000008e0: 3d6d 6f64 652c 656e 636f 6469 6e67 3d65  =mode,encoding=e
-000008f0: 6e63 6f64 696e 6729 0d0a 2020 2020 662e  ncoding)..    f.
-00000900: 7772 6974 6528 7465 7874 2e73 7472 6970  write(text.strip
-00000910: 2829 2b22 5c6e 2229 0d0a 2020 2020 662e  ()+"\n")..    f.
-00000920: 636c 6f73 6528 290d 0a0d 0a64 6566 2067  close()....def g
-00000930: 6574 5f64 6174 615f 6578 6365 6c28 6578  et_data_excel(ex
-00000940: 6365 6c5f 7061 7468 2c63 6f6c 756d 6e5f  cel_path,column_
-00000950: 6964 2c73 6865 6574 5f6e 616d 653d 4e6f  id,sheet_name=No
-00000960: 6e65 293a 0d0a 2020 2020 2727 270d 0a20  ne):..    '''.. 
-00000970: 2020 2050 6172 616d 6574 6572 730d 0a20     Parameters.. 
-00000980: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20     ----------.. 
-00000990: 2020 2065 7863 656c 5f70 6174 6820 3a20     excel_path : 
-000009a0: 5459 5045 0d0a 2020 2020 2020 2020 4445  TYPE..        DE
-000009b0: 5343 5249 5054 494f 4e2e 2044 3a2f 2f64  SCRIPTION. D://d
-000009c0: 6174 615f 7079 7468 6f6e 2e78 6c73 780d  ata_python.xlsx.
-000009d0: 0a20 2020 2020 2020 200d 0a20 2020 2063  .        ..    c
-000009e0: 6f6c 756d 6e5f 6964 203a 2054 5950 4520  olumn_id : TYPE 
-000009f0: 496e 7420 302c 312c 322c 330d 0a20 2020  Int 0,1,2,3..   
-00000a00: 2020 2020 2044 4553 4352 4950 5449 4f4e       DESCRIPTION
-00000a10: 2e20 3020 6d65 616e 7320 7468 6520 6669  . 0 means the fi
-00000a20: 7273 7420 636f 6c75 6d6e 2c20 3120 6d65  rst column, 1 me
-00000a30: 616e 7320 7468 6520 7365 636f 6e64 2e0d  ans the second..
-00000a40: 0a20 2020 2020 2020 200d 0a20 2020 2073  .        ..    s
-00000a50: 6865 6574 5f6e 616d 6520 3a20 5459 5045  heet_name : TYPE
-00000a60: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
-00000a70: 2020 2020 4445 5343 5249 5054 494f 4e2e      DESCRIPTION.
-00000a80: 2054 6865 2064 6566 6175 6c74 2069 7320   The default is 
-00000a90: 4e6f 6e65 2e0d 0a0d 0a20 2020 2052 6574  None.....    Ret
-00000aa0: 7572 6e73 0d0a 2020 2020 2d2d 2d2d 2d2d  urns..    ------
-00000ab0: 2d0d 0a20 2020 2054 5950 4520 6c69 7374  -..    TYPE list
-00000ac0: 0d0a 2020 2020 2020 2020 4445 5343 5249  ..        DESCRI
-00000ad0: 5054 494f 4e2e 2072 6574 7572 6e20 6120  PTION. return a 
-00000ae0: 6c69 7374 206f 6620 6461 7461 2e0d 0a20  list of data... 
-00000af0: 2020 2027 2727 0d0a 2020 2020 0d0a 2020     '''..    ..  
-00000b00: 2020 696d 706f 7274 2070 616e 6461 7320    import pandas 
-00000b10: 6173 2070 640d 0a20 2020 2069 6620 7368  as pd..    if sh
-00000b20: 6565 745f 6e61 6d65 2069 7320 4e6f 6e65  eet_name is None
-00000b30: 3a0d 0a20 2020 2020 2020 2073 6865 6574  :..        sheet
-00000b40: 5f6e 616d 653d 300d 0a20 2020 2065 6c73  _name=0..    els
-00000b50: 653a 0d0a 2020 2020 2020 2073 6865 6574  e:..       sheet
-00000b60: 5f6e 616d 653d 7368 6565 745f 6e61 6d65  _name=sheet_name
-00000b70: 2020 0d0a 2020 2020 6466 3d70 642e 7265    ..    df=pd.re
-00000b80: 6164 5f65 7863 656c 2865 7863 656c 5f70  ad_excel(excel_p
-00000b90: 6174 682c 6b65 6570 5f64 6566 6175 6c74  ath,keep_default
-00000ba0: 5f6e 613d 4661 6c73 652c 2073 6865 6574  _na=False, sheet
-00000bb0: 5f6e 616d 653d 7368 6565 745f 6e61 6d65  _name=sheet_name
-00000bc0: 2c68 6561 6465 723d 4e6f 6e65 2920 0d0a  ,header=None) ..
-00000bd0: 2020 2020 696e 7465 723d 6466 2e69 6c6f      inter=df.ilo
-00000be0: 635b 303a 2c63 6f6c 756d 6e5f 6964 5d20  c[0:,column_id] 
-00000bf0: 23e6 8f90 e58f 96e7 acac e4ba 8ce5 8897  #...............
-00000c00: e689 80e6 9c89 e8a1 8c20 200d 0a20 2020  .........  ..   
-00000c10: 2072 6574 7572 6e20 6c69 7374 2869 6e74   return list(int
-00000c20: 6572 290d 0a0d 0a64 6566 2077 7269 7465  er)....def write
-00000c30: 5f74 6f5f 6578 6365 6c28 6578 6365 6c5f  _to_excel(excel_
-00000c40: 7061 7468 2c64 6963 5f6f 665f 6c69 7374  path,dic_of_list
-00000c50: 2c73 6865 6574 5f6e 616d 653d 4e6f 6e65  ,sheet_name=None
-00000c60: 2c69 6e64 6578 3d4e 6f6e 6529 3a0d 0a20  ,index=None):.. 
-00000c70: 2020 2027 2727 0d0a 2020 2020 5061 7261     '''..    Para
-00000c80: 6d65 7465 7273 0d0a 2020 2020 2d2d 2d2d  meters..    ----
-00000c90: 2d2d 2d2d 2d2d 0d0a 2020 2020 6578 6365  ------..    exce
-00000ca0: 6c5f 7061 7468 203a 2054 5950 450d 0a20  l_path : TYPE.. 
-00000cb0: 2020 2020 2020 2044 4553 4352 4950 5449         DESCRIPTI
-00000cc0: 4f4e 2e20 443a 2f2f 7265 7375 6c74 732e  ON. D://results.
-00000cd0: 786c 7378 0d0a 2020 2020 2020 2020 0d0a  xlsx..        ..
-00000ce0: 2020 2020 6469 635f 6f66 5f6c 6973 7420      dic_of_list 
-00000cf0: 3a20 5459 5045 0d0a 2020 2020 2020 2020  : TYPE..        
-00000d00: 4445 5343 5249 5054 494f 4e2e 207b 2263  DESCRIPTION. {"c
-00000d10: 6f6c 223a 5b22 6122 2c22 6222 2c22 6322  ol":["a","b","c"
-00000d20: 2c22 6422 5d2c 2266 7265 7122 3a5b 312c  ,"d"],"freq":[1,
-00000d30: 322c 332c 345d 7d0d 0a20 2020 2020 2020  2,3,4]}..       
-00000d40: 200d 0a20 2020 2073 6865 6574 5f6e 616d   ..    sheet_nam
-00000d50: 6520 3a20 5459 5045 2c20 6f70 7469 6f6e  e : TYPE, option
-00000d60: 616c 0d0a 2020 2020 2020 2020 4445 5343  al..        DESC
-00000d70: 5249 5054 494f 4e2e 2054 6865 2064 6566  RIPTION. The def
-00000d80: 6175 6c74 2069 7320 4e6f 6e65 2e0d 0a20  ault is None... 
-00000d90: 2020 2020 2020 200d 0a20 2020 2069 6e64         ..    ind
-00000da0: 6578 203a 2054 5950 452c 206f 7074 696f  ex : TYPE, optio
-00000db0: 6e61 6c0d 0a20 2020 2020 2020 2044 4553  nal..        DES
-00000dc0: 4352 4950 5449 4f4e 2e20 5468 6520 6465  CRIPTION. The de
-00000dd0: 6661 756c 7420 6973 204e 6f6e 652e 0d0a  fault is None...
-00000de0: 2020 2020 2020 2020 0d0a 2020 2020 5265          ..    Re
-00000df0: 7475 726e 730d 0a20 2020 202d 2d2d 2d2d  turns..    -----
-00000e00: 2d2d 0d0a 2020 2020 4e6f 6e65 2e0d 0a0d  --..    None....
-00000e10: 0a20 2020 2027 2727 0d0a 2020 2020 696d  .    '''..    im
-00000e20: 706f 7274 2070 616e 6461 7320 6173 2070  port pandas as p
-00000e30: 640d 0a20 2020 2069 6620 7368 6565 745f  d..    if sheet_
-00000e40: 6e61 6d65 2069 7320 4e6f 6e65 3a0d 0a20  name is None:.. 
-00000e50: 2020 2020 2020 2073 6865 6574 5f6e 616d         sheet_nam
-00000e60: 653d 2273 6865 6574 3122 0d0a 2020 2020  e="sheet1"..    
-00000e70: 656c 7365 3a0d 0a20 2020 2020 2020 7368  else:..       sh
-00000e80: 6565 745f 6e61 6d65 3d73 6865 6574 5f6e  eet_name=sheet_n
-00000e90: 616d 650d 0a20 2020 2069 6620 696e 6465  ame..    if inde
-00000ea0: 7820 6973 204e 6f6e 653a 0d0a 2020 2020  x is None:..    
-00000eb0: 2020 2020 696e 6465 783d 4661 6c73 650d      index=False.
-00000ec0: 0a20 2020 2065 6c73 653a 0d0a 2020 2020  .    else:..    
-00000ed0: 2020 2020 696e 6465 783d 5472 7565 2020      index=True  
-00000ee0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00000ef0: 0d0a 2020 2020 6466 3d70 642e 4461 7461  ..    df=pd.Data
-00000f00: 4672 616d 6528 6469 635f 6f66 5f6c 6973  Frame(dic_of_lis
-00000f10: 7429 0d0a 2020 2020 6466 2e73 7479 6c65  t)..    df.style
-00000f20: 2e74 6f5f 6578 6365 6c28 6578 6365 6c5f  .to_excel(excel_
-00000f30: 7061 7468 2c20 7368 6565 745f 6e61 6d65  path, sheet_name
-00000f40: 3d73 6865 6574 5f6e 616d 652c 7374 6172  =sheet_name,star
-00000f50: 7463 6f6c 3d30 2c20 696e 6465 783d 696e  tcol=0, index=in
-00000f60: 6465 7829 0d0a 2020 2020 0d0a 200d 0a64  dex)..    .. ..d
-00000f70: 6566 2067 6574 5f64 6174 615f 6a73 6f6e  ef get_data_json
-00000f80: 286a 736f 6e5f 7061 7468 293a 0d0a 2020  (json_path):..  
-00000f90: 2020 2727 270d 0a20 2020 2050 6172 616d    '''..    Param
-00000fa0: 6574 6572 730d 0a20 2020 202d 2d2d 2d2d  eters..    -----
-00000fb0: 2d2d 2d2d 2d0d 0a20 2020 206a 736f 6e5f  -----..    json_
-00000fc0: 7061 7468 203a 2054 5950 4520 443a 2f2f  path : TYPE D://
-00000fd0: 6461 7461 2e6a 736f 6e0d 0a20 2020 2020  data.json..     
-00000fe0: 2020 2044 4553 4352 4950 5449 4f4e 2e0d     DESCRIPTION..
-00000ff0: 0a0d 0a20 2020 2052 6574 7572 6e73 0d0a  ...    Returns..
-00001000: 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020      -------..   
-00001010: 206c 6f61 645f 6469 6374 203a 2054 5950   load_dict : TYP
-00001020: 4520 6469 6374 0d0a 2020 2020 2020 2020  E dict..        
-00001030: 4445 5343 5249 5054 494f 4e2e 2072 6574  DESCRIPTION. ret
-00001040: 7572 6e20 6120 6469 6374 206f 6620 6461  urn a dict of da
-00001050: 7461 2e0d 0a0d 0a20 2020 2027 2727 0d0a  ta.....    '''..
-00001060: 2020 2020 696d 706f 7274 206a 736f 6e0d      import json.
-00001070: 0a20 2020 2074 7279 3a0d 0a20 2020 2020  .    try:..     
-00001080: 2020 2066 3d6f 7065 6e28 6a73 6f6e 5f70     f=open(json_p
-00001090: 6174 682c 2272 222c 656e 636f 6469 6e67  ath,"r",encoding
-000010a0: 3d22 7574 662d 3822 290d 0a20 2020 2020  ="utf-8")..     
-000010b0: 2020 206c 6f61 645f 6469 6374 3d6a 736f     load_dict=jso
-000010c0: 6e2e 6c6f 6164 2866 2920 2020 200d 0a20  n.load(f)    .. 
-000010d0: 2020 2020 2020 2072 6574 7572 6e20 6c6f         return lo
-000010e0: 6164 5f64 6963 7420 2020 2020 2020 2020  ad_dict         
-000010f0: 2020 200d 0a20 2020 2065 7863 6570 743a     ..    except:
-00001100: 0d0a 2020 2020 2020 2020 663d 6f70 656e  ..        f=open
-00001110: 286a 736f 6e5f 7061 7468 2c22 7222 2c65  (json_path,"r",e
-00001120: 6e63 6f64 696e 673d 2275 7466 2d38 2d73  ncoding="utf-8-s
-00001130: 6967 2229 0d0a 2020 2020 2020 2020 6c6f  ig")..        lo
-00001140: 6164 5f64 6963 743d 6a73 6f6e 2e6c 6f61  ad_dict=json.loa
-00001150: 6428 6629 2020 2020 0d0a 2020 2020 2020  d(f)    ..      
-00001160: 2020 7265 7475 726e 206c 6f61 645f 6469    return load_di
-00001170: 6374 0d0a 0d0a 6465 6620 7772 6974 655f  ct....def write_
-00001180: 746f 5f6a 736f 6e28 6a73 6f6e 5f70 6174  to_json(json_pat
-00001190: 682c 6d79 5f64 6963 293a 0d0a 2020 2020  h,my_dic):..    
-000011a0: 2727 270d 0a0d 0a20 2020 2050 6172 616d  '''....    Param
-000011b0: 6574 6572 730d 0a20 2020 202d 2d2d 2d2d  eters..    -----
-000011c0: 2d2d 2d2d 2d0d 0a20 2020 206a 736f 6e5f  -----..    json_
-000011d0: 7061 7468 203a 2054 5950 4520 7374 7269  path : TYPE stri
-000011e0: 6e67 0d0a 2020 2020 2020 2020 4445 5343  ng..        DESC
-000011f0: 5249 5054 494f 4e2e 2044 3a2f 2f64 6174  RIPTION. D://dat
-00001200: 612e 6a73 6f6e 0d0a 2020 2020 2020 2020  a.json..        
-00001210: 0d0a 2020 2020 6d79 5f64 6963 203a 2054  ..    my_dic : T
-00001220: 5950 4520 6469 6374 206f 7220 6c69 7374  YPE dict or list
-00001230: 0d0a 2020 2020 2020 2020 4445 5343 5249  ..        DESCRI
-00001240: 5054 494f 4e2e 200d 0a20 2020 2020 2020  PTION. ..       
-00001250: 2074 7970 6531 3a20 7b22 7061 6e73 223a   type1: {"pans":
-00001260: 317d 0d0a 2020 2020 2020 2020 7479 7065  1}..        type
-00001270: 323a 207b 2277 6f72 6422 3a5b 2261 222c  2: {"word":["a",
-00001280: 2262 222c 2263 225d 7d0d 0a20 2020 2020  "b","c"]}..     
-00001290: 2020 2074 7970 6533 3a20 5b7b 2270 616e     type3: [{"pan
-000012a0: 7322 3a31 7d2c 7b22 676c 656e 6e61 223a  s":1},{"glenna":
-000012b0: 327d 5d0d 0a20 2020 2020 2020 2074 7970  2}]..        typ
-000012c0: 6534 3a20 5b7b 2277 6f72 6422 3a5b 2261  e4: [{"word":["a
-000012d0: 222c 2262 222c 2263 225d 7d2c 7b22 6672  ","b","c"]},{"fr
-000012e0: 6571 223a 5b31 2c32 2c33 2c34 2c35 2c36  eq":[1,2,3,4,5,6
-000012f0: 5d7d 5d0d 0a0d 0a20 2020 2052 6574 7572  ]}]....    Retur
-00001300: 6e73 0d0a 2020 2020 2d2d 2d2d 2d2d 2d0d  ns..    -------.
-00001310: 0a20 2020 204e 6f6e 652e 0d0a 0d0a 2020  .    None.....  
-00001320: 2020 2727 270d 0a20 2020 2069 6d70 6f72    '''..    impor
-00001330: 7420 6a73 6f6e 0d0a 2020 2020 6632 203d  t json..    f2 =
-00001340: 206f 7065 6e28 6a73 6f6e 5f70 6174 682c   open(json_path,
-00001350: 2022 7722 2c20 656e 636f 6469 6e67 3d22   "w", encoding="
-00001360: 7574 662d 3822 2c20 6572 726f 7273 3d22  utf-8", errors="
-00001370: 6967 6e6f 7265 2229 0d0a 2020 2020 6632  ignore")..    f2
-00001380: 2e77 7269 7465 286a 736f 6e2e 6475 6d70  .write(json.dump
-00001390: 7328 6d79 5f64 6963 2c65 6e73 7572 655f  s(my_dic,ensure_
-000013a0: 6173 6369 693d 4661 6c73 6529 2920 2365  ascii=False)) #e
-000013b0: 6e73 7572 655f 6173 6369 693d 4661 6c73  nsure_ascii=Fals
-000013c0: 6520 e8ae a9e4 b8ad e696 87e4 b88d e586  e ..............
-000013d0: 8de4 b9b1 e7a0 810d 0a20 2020 2066 322e  .........    f2.
-000013e0: 636c 6f73 6528 2920 0d0a 2020 2020 0d0a  close() ..    ..
-000013f0: 6465 6620 4669 6c65 5061 7468 2872 6f6f  def FilePath(roo
-00001400: 7429 3a0d 0a20 2020 2027 2727 e8af bbe5  t):..    '''....
-00001410: 8f96 e689 80e6 9c89 e696 87e4 bbb6 efbc  ................
-00001420: 8ce5 8897 e587 bae6 af8f e4b8 aae6 9687  ................
-00001430: e4bb b6e7 9a84 e8b7 afe5 be84 2727 270d  ............'''.
-00001440: 0a20 2020 2046 696c 656c 6973 743d 5b5d  .    Filelist=[]
-00001450: 0d0a 2020 2020 666f 7220 686f 6d65 2c20  ..    for home, 
-00001460: 6469 7273 2c20 6669 6c65 7320 696e 206f  dirs, files in o
-00001470: 732e 7761 6c6b 2872 6f6f 7429 3a0d 0a20  s.walk(root):.. 
-00001480: 2020 2020 2020 2066 6f72 2066 696c 656e         for filen
-00001490: 616d 6520 696e 2066 696c 6573 3a0d 0a20  ame in files:.. 
-000014a0: 2020 2020 2020 2020 2020 2046 696c 656c             Filel
-000014b0: 6973 742e 6170 7065 6e64 286f 732e 7061  ist.append(os.pa
-000014c0: 7468 2e6a 6f69 6e28 686f 6d65 2c20 6669  th.join(home, fi
-000014d0: 6c65 6e61 6d65 2929 0d0a 2020 2020 7265  lename))..    re
-000014e0: 7475 726e 2046 696c 656c 6973 740d 0a0d  turn Filelist...
-000014f0: 0a64 6566 2046 696c 654e 616d 6528 6669  .def FileName(fi
-00001500: 6c65 5f70 6174 6829 3a0d 0a20 2020 2069  le_path):..    i
-00001510: 6e74 6572 3d6f 732e 7061 7468 2e62 6173  nter=os.path.bas
-00001520: 656e 616d 6528 6669 6c65 5f70 6174 6829  ename(file_path)
-00001530: 0d0a 2020 2020 7265 7475 726e 2069 6e74  ..    return int
-00001540: 6572 0d0a 0d0a 0d0a 4269 6750 756e 6374  er......BigPunct
-00001550: 7561 7469 6f6e 3d22 2222 2122 2324 265c  uation="""!"#$&\
-00001560: 2728 292a 2b2c 2d2f 3a3b 3c3d 3e3f 405b  '()*+,-/:;<=>?@[
-00001570: 5c5c 5d5e 5f60 7b7c 7d2e 257e efbc 82ef  \\]^_`{|}.%~....
-00001580: bc83 efbc 84ef bc85 efbc 86ef bc87 3fe3  ..............?.
-00001590: 8082 efbc 88ef bc89 efbc 8aef bc8b efbc  ................
-000015a0: 8cef bc8d efbc 8fef bc9a efbc 9bef bc9c  ................
-000015b0: efbc 9def bc9e efbc a0ef bcbb efbc bcef  ................
-000015c0: bcbd efbc beef bcbf efbd 80ef bd9b efbd  ................
-000015d0: 9cef bd9d efbd 9eef bd9f efbd a0ef bda2  ................
-000015e0: efbd a3ef bda4 5c75 3330 3030 e380 81e3  ......\u3000....
-000015f0: 8083 e380 88e3 8089 e380 8ae3 808b e380  ................
-00001600: 8ce3 808d e380 8ee3 808f e380 90e3 8091  ................
-00001610: e380 94e3 8095 e380 96e3 8097 e380 98e3  ................
-00001620: 8099 e380 9ae3 809b e380 9ce3 809d e380  ................
-00001630: 9ee3 809f e380 b0e3 80be e380 bfe2 8093  ................
-00001640: e280 94e2 8098 e280 99e2 809b e280 9ce2  ................
-00001650: 809d e280 9ee2 809f e280 a6e2 80a7 efb9  ................
-00001660: 8fef b991 efb9 94c2 b7ef bc81 efbc 9fef  ................
-00001670: bda1 e380 8260 6027 2722 2222 2020 2023  .....``''"""   #
-00001680: e999 a4e5 8ebb e88b b1e6 9687 e6a0 87e7  ................
-00001690: 82b9 2e25 0d0a 5374 6f70 5461 6773 3d22  ...%..StopTags="
-000016a0: 2222 e297 863a 20e3 8081 2f20 e380 822f  ""...: .../ .../
-000016b0: 202d 2d2d 2f20 2d2f 202d 2d2f 202d 2d20   ---/ -/ --/ -- 
-000016c0: 3a2f 203b 2f20 3f2f 203f 3f2f 203f e294  :/ ;/ ?/ ??/ ?..
-000016d0: 9620 402f 205b 2f20 5d2f 205e 2f20 e280  . @/ [/ ]/ ^/ ..
-000016e0: 982f 20e2 8099 2f20 222f 2022 2f20 e380  ./ .../ "/ "/ ..
-000016f0: 882f 20e3 8089 2f20 e380 8a2f 20e3 808b  ./ .../ .../ ...
-00001700: 2f20 e380 902f 20e3 8091 2f20 3e2f 20e2  / .../ .../ >/ .
-00001710: 88b6 2f20 e296 a02f 20e2 978f 2f20 c2b7  ../ .../ .../ ..
-00001720: 2f20 e280 a62f 2021 2f20 232f 2025 2c2f  / .../ !/ #/ %,/
-00001730: 2025 2f20 5c27 2f20 282f 2029 2f20 2a2f   %/ \'/ (/ )/ */
-00001740: 202b 2f20 2c2f 202d 2f20 2f2f 206e 7020   +/ ,/ -/ // np 
-00001750: 7620 6e20 7720 6d20 6120 7820 7420 7120  v n w m a x t q 
-00001760: 6a20 6e69 206e 7320 6420 6920 6620 7520  j ni ns d i f u 
-00001770: 7020 6720 6e7a 2063 2072 2069 6420 7320  p g nz c r id s 
-00001780: 6b20 6820 6f20 6520 2f20 233f 2f20 2d2d  k h o e / #?/ --
-00001790: 2f22 2222 2023 e794 a8e6 9da5 e581 9ce7  /""" #..........
-000017a0: 94a8 e8af 8de6 80a7 e6a0 87e6 b3a8 0d0a  ................
-000017b0: 5370 6563 6961 6c3d 2222 22e2 88b6 20e2  Special="""... .
-000017c0: 96a0 20e2 978f 20e2 91a0 20e2 91a1 20e2  .. ... ... ... .
-000017d0: 91a2 20c3 9720 e284 8320 e285 a220 e291  .. .. ... ... ..
-000017e0: a320 e291 a420 e297 8620 e291 a520 c2b1  . ... ... ... ..
-000017f0: 20e2 91a6 20e2 91a7 20e2 8692 20e2 91a8   ... ... ... ...
-00001800: 20e2 96b2 20e2 91a9 20e2 9480 20c3 b720   ... ... ... .. 
-00001810: cebc 20ce b320 ceb2 20e2 85a1 20e2 85a0  .. .. .. ... ...
-00001820: 20e2 80b0 20e2 96a1 20e3 8087 20e2 978b   ... ... ... ...
-00001830: 20e2 85a4 20e2 85a3 20e2 9885 20ef b990   ... ... ... ...
-00001840: 20c2 b020 e280 bb20 efb8 b020 ceb1 20e2   .. ... ... .. .
-00001850: 8095 20e2 89a0 20e2 9688 20d0 be20 ceb8  .. ... ... .. ..
-00001860: 20cf 8920 e292 8820 e292 8920 e292 8a20   .. ... ... ... 
-00001870: d0bd 20e2 89a4 20c3 ac20 c78e 20e2 89a5  .. ... .. .. ...
-00001880: 20d1 8020 d182 20d1 8120 d0ba 20d0 b920   .. .. .. .. .. 
-00001890: d0b0 20d0 b820 e285 a520 c3a9 20c3 a820  .. .. ... .. .. 
-000018a0: efb9 a220 efb9 9d20 efb9 9e20 7f20 c481  ... ... ... . ..
-000018b0: 20e2 928b 20c3 b920 cf80 20e2 9787 20ce   ... .. .. ... .
-000018c0: a920 d0a4 20d1 8b20 d0af 20d0 bf20 d09a  . .. .. .. .. ..
-000018d0: 20d0 b220 d183 20d0 bc20 c792 20c3 bc20   .. .. .. .. .. 
-000018e0: c3a1 20c7 9420 e292 8c20 e292 8d20 e4a6  .. .. ... ... ..
-000018f0: 8620 e285 a920 e285 a620 e286 9020 2222  . ... ... ... ""
-00001900: 220d 0a53 746f 7057 6f72 6473 3d22 2222  "..StopWords="""
-00001910: e280 94e2 8094 e280 9420 e380 8bef bc89  ......... ......
-00001920: efbc 8c20 efbc 89c3 b7ef bc88 efbc 91ef  ... ............
-00001930: bc8d 20e2 809d efbc 8c20 efbc 89e3 8081  .. ...... ......
-00001940: 20ef bc9d efbc 8820 3a20 e286 9220 e284   ...... : ... ..
-00001950: 8320 2026 202a 20e4 b880 e4b8 8020 7e7e  .  & * ...... ~~
-00001960: 7e7e 20e2 8099 202e 2020 e380 8e20 2ee4  ~~ ... .  ... ..
-00001970: b880 202e 2f20 2d2d 2020 e380 8f20 efbc  .. ./ --  ... ..
-00001980: 9de2 80b3 20e3 8090 20ef bcbb efbc 8aef  .... ... .......
-00001990: bcbd 20ef bd9d efbc 9e20 efbc bbe2 91a4  .. ...... ......
-000019a0: efbc bdef bcbd 20ef bcbb e291 a0ef bca4  ...... .........
-000019b0: efbc bd20 efbd 83ef bcbd 20ef bd8e efbd  ... ...... .....
-000019c0: 87e6 9889 20ef bc8a 202f 2f20 efbc bb20  .... ... // ... 
-000019d0: efbc bd20 efbc bbe2 91a1 efbd 85ef bcbd  ... ............
-000019e0: 20ef bcbb e291 a1ef bd87 efbc bd20 efbc   ............ ..
-000019f0: 9def bd9b 207d 20ef bc8c e4b9 9f20 20e2  .... } ......  .
-00001a00: 8098 20ef bca1 20ef bcbb e291 a0e2 91a5  .. ... .........
-00001a10: efbc bd20 efbc bbe2 91a1 efbc a2ef bcbd  ... ............
-00001a20: 2020 efbc bbe2 91a0 efbd 81ef bcbd 20ef    ............ .
-00001a30: bcbb e291 a3ef bd81 efbc bd20 efbc bbe2  ........... ....
-00001a40: 91a0 e291 a2ef bcbd 20ef bcbb e291 a2ef  ........ .......
-00001a50: bd88 efbc bd20 e291 a2ef bcbd 20ef bc91  ..... ...... ...
-00001a60: efbc 8e20 20ef bc8d efbc 8d20 20ef bcbb  ...  ......  ...
-00001a70: e291 a1ef bd82 efbc bd20 e280 99e2 8098  ......... ......
-00001a80: 2020 c397 c397 c397 2020 efbc bbe2 91a0    ......  ......
-00001a90: e291 a7ef bcbd 20ef bc90 efbc 9aef bc92  ...... .........
-00001aa0: 2020 efbc 9def bcbb 20ef bcbb e291 a4ef    ...... .......
-00001ab0: bd82 efbc bd20 efbc bbe2 91a1 efbd 83ef  ..... ..........
-00001ac0: bcbd 2020 efbc bbe2 91a3 efbd 82ef bcbd  ..  ............
-00001ad0: 20ef bcbb e291 a1e2 91a2 efbc bd20 efbc   ............ ..
-00001ae0: bbe2 91a2 efbd 81ef bcbd 20ef bcbb e291  .......... .....
-00001af0: a3ef bd83 efbc bd20 efbc bbe2 91a0 e291  ....... ........
-00001b00: a4ef bcbd 20ef bcbb e291 a0e2 91a6 efbc  .... ...........
-00001b10: bd20 efbc bbe2 91a0 efbd 87ef bcbd 20e2  . ............ .
-00001b20: 8888 efbc bb20 20ef bcbb e291 a0e2 91a8  .....  .........
-00001b30: efbc bd20 efbc bbe2 91a0 e291 a3ef bcbd  ... ............
-00001b40: 20ef bcbb e291 a0ef bd83 efbc bd20 efbc   ............ ..
-00001b50: bbe2 91a1 efbd 86ef bcbd 20ef bcbb e291  .......... .....
-00001b60: a1e2 91a7 efbc bd20 efbc bbe2 91a1 e291  ....... ........
-00001b70: a0ef bcbd 20ef bcbb e291 a0ef bca3 efbc  .... ...........
-00001b80: bd20 efbc bbe2 91a2 efbd 83ef bcbd 20ef  . ............ .
-00001b90: bcbb e291 a2ef bd87 efbc bd20 efbc bbe2  ........... ....
-00001ba0: 91a1 e291 a4ef bcbd 20ef bcbb e291 a1e2  ........ .......
-00001bb0: 91a1 efbc bd20 e4b8 802e 20ef bcbb e291  ..... .... .....
-00001bc0: a0ef bd88 efbc bd20 2ee6 95b0 20ef bcbb  ....... .... ...
-00001bd0: efbc bd20 efbc bbe2 91a0 efbc a2ef bcbd  ... ............
-00001be0: 20e6 95b0 2f20 efbc bbe2 91a0 efbd 89ef   .../ ..........
-00001bf0: bcbd 20ef bcbb e291 a2ef bd85 efbc bd20  .. ............ 
-00001c00: efbc bbe2 91a0 e291 a0ef bcbd 20ef bcbb  ............ ...
-00001c10: e291 a3ef bd84 efbc bd20 efbc bbe2 91a3  ......... ......
-00001c20: efbd 85ef bcbd 20ef bcbb e291 a2ef bd82  ...... .........
-00001c30: efbc bd20 efbc bbe2 91a4 efbd 81ef bcbd  ... ............
-00001c40: 20ef bcbb e291 a0ef bca1 efbc bd20 efbc   ............ ..
-00001c50: bbe2 91a1 e291 a7ef bcbd 20ef bcbb e291  .......... .....
-00001c60: a1e2 91a6 efbc bd20 efbc bbe2 91a0 efbd  ....... ........
-00001c70: 84ef bcbd 20ef bcbb e291 a1ef bd8a efbc  .... ...........
-00001c80: bd20 e380 95e3 8094 20ef bcbd efbc bb20  . ...... ...... 
-00001c90: 3a2f 2f20 e280 b2e2 8888 20ef bcbb e291  :// ...... .....
-00001ca0: a1e2 91a3 20ef bcbb e291 a4ef bd85 efbc  .... ...........
-00001cb0: bd20 efbc 91ef bc92 efbc 8520 efbd 82ef  . ......... ....
-00001cc0: bcbd 202e 2e2e 202e 2e2e 2e2e 2e2e 2e2e  .. ... .........
-00001cd0: 2e2e 2e2e 2e2e 2e2e 2e2e 20e2 80a6 e280  .......... .....
-00001ce0: a6e2 80a6 e280 a6e2 80a6 e280 a6e2 80a6  ................
-00001cf0: e280 a6e2 80a6 e280 a6e2 80a6 e280 a6e2  ................
+000000e0: 2020 2020 0909 5573 696e 6720 7061 7468      ..Using path
+000000f0: 2074 6f20 6765 7420 6461 7461 2066 726f   to get data fro
+00000100: 6d20 6120 7369 6e67 6c65 2074 7874 2066  m a single txt f
+00000110: 696c 652e 2065 672e 2044 3a5c 7261 775f  ile. eg. D:\raw_
+00000120: 7465 7874 2e74 7874 0d0a 2020 2020 2020  text.txt..      
+00000130: 2020 2020 2020 5468 656f 7265 7469 6361        Theoretica
+00000140: 6c6c 792c 2069 7420 7375 7070 6f72 7473  lly, it supports
+00000150: 2061 6c6c 2074 6865 2074 6578 7420 656e   all the text en
+00000160: 636f 6469 6e67 2066 6f72 6d61 7473 2c20  coding formats, 
+00000170: 6c69 6b65 2075 7466 2d38 2c20 756e 6963  like utf-8, unic
+00000180: 6f64 652c 2061 6e73 692c 2067 626b 2065  ode, ansi, gbk e
+00000190: 7463 2e0d 0a0d 0a20 2020 2052 6574 7572  tc.....    Retur
+000001a0: 6e73 0d0a 2020 2020 2d2d 2d2d 2d2d 2d0d  ns..    -------.
+000001b0: 0a20 2020 2074 6578 7420 3a20 5459 5045  .    text : TYPE
+000001c0: 2073 7472 696e 670d 0a20 2020 2020 2020   string..       
+000001d0: 2044 4553 4352 4950 5449 4f4e 2e20 0d0a   DESCRIPTION. ..
+000001e0: 2020 2020 0909 4974 2072 6574 7572 6e73      ..It returns
+000001f0: 2061 6c6c 2074 6865 2074 6578 7420 636f   all the text co
+00000200: 6e74 656e 7420 6672 6f6d 2074 6865 2074  ntent from the t
+00000210: 6172 6765 7420 6669 6c65 2e0d 0a0d 0a20  arget file..... 
+00000220: 2020 2027 2727 0d0a 2020 2020 696d 706f     '''..    impo
+00000230: 7274 2063 6861 7264 6574 0d0a 2020 2020  rt chardet..    
+00000240: 7061 7468 3d70 6174 682e 7265 706c 6163  path=path.replac
+00000250: 6528 225c 6e22 2c22 2229 0d0a 2020 2020  e("\n","")..    
+00000260: 663d 6f70 656e 2870 6174 682c 2772 6227  f=open(path,'rb'
+00000270: 2920 200d 0a20 2020 2064 6174 613d 662e  )  ..    data=f.
+00000280: 7265 6164 2829 2020 0d0a 2020 2020 662e  read()  ..    f.
+00000290: 636c 6f73 6528 290d 0a20 2020 2066 696c  close()..    fil
+000002a0: 655f 656e 636f 6469 6e67 3d63 6861 7264  e_encoding=chard
+000002b0: 6574 2e64 6574 6563 7428 6461 7461 292e  et.detect(data).
+000002c0: 6765 7428 2765 6e63 6f64 696e 6727 2920  get('encoding') 
+000002d0: 200d 0a20 2020 2066 313d 6f70 656e 2870   ..    f1=open(p
+000002e0: 6174 682c 2772 272c 2065 6e63 6f64 696e  ath,'r', encodin
+000002f0: 673d 6669 6c65 5f65 6e63 6f64 696e 672c  g=file_encoding,
+00000300: 2065 7272 6f72 733d 2769 676e 6f72 6527   errors='ignore'
+00000310: 2920 200d 0a20 2020 2074 6578 743d 6631  )  ..    text=f1
+00000320: 2e72 6561 6428 292e 7265 706c 6163 6528  .read().replace(
+00000330: 22e2 8099 222c 2227 2229 0d0a 2020 2020  "...","'")..    
+00000340: 6631 2e63 6c6f 7365 2829 0d0a 2020 2020  f1.close()..    
+00000350: 7265 7475 726e 2074 6578 740d 0a20 2020  return text..   
+00000360: 2020 2020 2020 2020 200d 0a64 6566 2067           ..def g
+00000370: 6574 5f64 6174 615f 6c69 6e65 7328 7061  et_data_lines(pa
+00000380: 7468 293a 0d0a 2020 2020 2727 270d 0a20  th):..    '''.. 
+00000390: 2020 2050 6172 616d 6574 6572 730d 0a20     Parameters.. 
+000003a0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20     ----------.. 
+000003b0: 2020 2070 6174 6820 3a20 5459 5045 2073     path : TYPE s
+000003c0: 7472 696e 670d 0a20 2020 2020 2020 2044  tring..        D
+000003d0: 4553 4352 4950 5449 4f4e 2e0d 0a20 2020  ESCRIPTION...   
+000003e0: 2009 0955 7369 6e67 2070 6174 6820 746f   ..Using path to
+000003f0: 2067 6574 2064 6174 6120 6672 6f6d 2061   get data from a
+00000400: 2073 696e 676c 6520 7478 7420 6669 6c65   single txt file
+00000410: 2e20 6567 2e20 443a 5c72 6177 5f74 6578  . eg. D:\raw_tex
+00000420: 742e 7478 7420 2020 2020 0d0a 2020 2020  t.txt     ..    
+00000430: 0909 5468 656f 7265 7469 6361 6c6c 792c  ..Theoretically,
+00000440: 2069 7420 7375 7070 6f72 7473 2061 6c6c   it supports all
+00000450: 2074 6865 2074 6578 7420 656e 636f 6469   the text encodi
+00000460: 6e67 2066 6f72 6d61 7473 2c20 6c69 6b65  ng formats, like
+00000470: 2075 7466 2d38 2c20 756e 6963 6f64 652c   utf-8, unicode,
+00000480: 2061 6e73 692c 2067 626b 2065 7463 2e0d   ansi, gbk etc..
+00000490: 0a0d 0a20 2020 2052 6574 7572 6e73 0d0a  ...    Returns..
+000004a0: 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020      -------..   
+000004b0: 206c 696e 6573 203a 2054 5950 4520 6c69   lines : TYPE li
+000004c0: 7374 0d0a 2020 2020 2020 2020 4445 5343  st..        DESC
+000004d0: 5249 5054 494f 4e2e 200d 0a20 2020 2009  RIPTION. ..    .
+000004e0: 0949 7420 7265 7475 726e 7320 6120 6c69  .It returns a li
+000004f0: 7374 2063 6f6e 7461 696e 696e 6720 616c  st containing al
+00000500: 6c20 7468 6520 7061 7261 6772 6170 6873  l the paragraphs
+00000510: 206f 6620 7468 6520 7461 7267 6574 2066   of the target f
+00000520: 696c 652e 0d0a 0d0a 2020 2020 2727 270d  ile.....    '''.
+00000530: 0a20 2020 2069 6d70 6f72 7420 6368 6172  .    import char
+00000540: 6465 740d 0a20 2020 2070 6174 683d 7061  det..    path=pa
+00000550: 7468 2e72 6570 6c61 6365 2822 5c6e 222c  th.replace("\n",
+00000560: 2222 290d 0a20 2020 2066 3d6f 7065 6e28  "")..    f=open(
+00000570: 7061 7468 2c27 7262 2729 2020 0d0a 2020  path,'rb')  ..  
+00000580: 2020 6461 7461 3d66 2e72 6561 6428 2920    data=f.read() 
+00000590: 200d 0a20 2020 2066 2e63 6c6f 7365 2829   ..    f.close()
+000005a0: 0d0a 2020 2020 6669 6c65 5f65 6e63 6f64  ..    file_encod
+000005b0: 696e 673d 6368 6172 6465 742e 6465 7465  ing=chardet.dete
+000005c0: 6374 2864 6174 6129 2e67 6574 2827 656e  ct(data).get('en
+000005d0: 636f 6469 6e67 2729 2020 0d0a 2020 2020  coding')  ..    
+000005e0: 6631 3d6f 7065 6e28 7061 7468 2c27 7227  f1=open(path,'r'
+000005f0: 2c20 656e 636f 6469 6e67 3d66 696c 655f  , encoding=file_
+00000600: 656e 636f 6469 6e67 2c20 6572 726f 7273  encoding, errors
+00000610: 3d27 6967 6e6f 7265 2729 2020 0d0a 2020  ='ignore')  ..  
+00000620: 2020 6c69 6e65 733d 6631 2e72 6561 646c    lines=f1.readl
+00000630: 696e 6573 2829 0d0a 2020 2020 6c69 6e65  ines()..    line
+00000640: 733d 5b6c 2e72 6570 6c61 6365 2822 e280  s=[l.replace("..
+00000650: 9922 2c22 2722 2920 666f 7220 6c20 696e  .","'") for l in
+00000660: 206c 696e 6573 2069 6620 6c65 6e28 6c2e   lines if len(l.
+00000670: 7374 7269 7028 2929 2021 3d30 5d0d 0a20  strip()) !=0].. 
+00000680: 2020 2066 312e 636c 6f73 6528 290d 0a20     f1.close().. 
+00000690: 2020 2072 6574 7572 6e20 6c69 6e65 730d     return lines.
+000006a0: 0a0d 0a64 6566 2077 7269 7465 5f74 6f5f  ...def write_to_
+000006b0: 7478 7428 6669 6c65 5f70 6174 682c 7465  txt(file_path,te
+000006c0: 7874 2c6d 6f64 653d 4e6f 6e65 2c65 6e63  xt,mode=None,enc
+000006d0: 6f64 696e 673d 4e6f 6e65 293a 0d0a 2020  oding=None):..  
+000006e0: 2020 2727 270d 0a20 2020 2050 6172 616d    '''..    Param
+000006f0: 6574 6572 730d 0a20 2020 202d 2d2d 2d2d  eters..    -----
+00000700: 2d2d 2d2d 2d0d 0a20 2020 2066 696c 655f  -----..    file_
+00000710: 7061 7468 203a 2054 5950 4520 7374 7269  path : TYPE stri
+00000720: 6e67 0d0a 2020 2020 2020 2020 4445 5343  ng..        DESC
+00000730: 5249 5054 494f 4e2e 0d0a 2020 2020 7465  RIPTION...    te
+00000740: 7874 203a 2054 5950 450d 0a20 2020 2020  xt : TYPE..     
+00000750: 2020 2044 4553 4352 4950 5449 4f4e 2e20     DESCRIPTION. 
+00000760: 7374 7269 6e67 0d0a 2020 2020 6d6f 6465  string..    mode
+00000770: 203a 2054 5950 452c 206f 7074 696f 6e61   : TYPE, optiona
+00000780: 6c20 2320 773b 612b 0d0a 2020 2020 2020  l # w;a+..      
+00000790: 2020 4445 5343 5249 5054 494f 4e2e 2054    DESCRIPTION. T
+000007a0: 6865 2064 6566 6175 6c74 2069 7320 4e6f  he default is No
+000007b0: 6e65 2e0d 0a20 2020 2065 6e63 6f64 696e  ne...    encodin
+000007c0: 6720 3a20 5459 5045 2c20 6f70 7469 6f6e  g : TYPE, option
+000007d0: 616c 2023 2075 7466 2d38 0d0a 2020 2020  al # utf-8..    
+000007e0: 2020 2020 4445 5343 5249 5054 494f 4e2e      DESCRIPTION.
+000007f0: 2054 6865 2064 6566 6175 6c74 2069 7320   The default is 
+00000800: 4e6f 6e65 2e0d 0a0d 0a20 2020 2052 6574  None.....    Ret
+00000810: 7572 6e73 0d0a 2020 2020 2d2d 2d2d 2d2d  urns..    ------
+00000820: 2d0d 0a20 2020 204e 6f6e 652e 0d0a 0d0a  -..    None.....
+00000830: 2020 2020 2727 270d 0a20 2020 2069 6620      '''..    if 
+00000840: 6d6f 6465 2069 7320 4e6f 6e65 3a0d 0a20  mode is None:.. 
+00000850: 2020 2020 2020 206d 6f64 653d 2277 220d         mode="w".
+00000860: 0a20 2020 2065 6c73 653a 0d0a 2020 2020  .    else:..    
+00000870: 2020 2020 6d6f 6465 3d6d 6f64 650d 0a20      mode=mode.. 
+00000880: 2020 2069 6620 656e 636f 6469 6e67 2069     if encoding i
+00000890: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
+000008a0: 2065 6e63 6f64 696e 673d 2275 7466 2d38   encoding="utf-8
+000008b0: 220d 0a20 2020 2065 6c73 653a 0d0a 2020  "..    else:..  
+000008c0: 2020 2020 2020 656e 636f 6469 6e67 3d65        encoding=e
+000008d0: 6e63 6f64 696e 6720 2020 200d 0a20 2020  ncoding    ..   
+000008e0: 2066 3d6f 7065 6e28 6669 6c65 5f70 6174   f=open(file_pat
+000008f0: 682c 6d6f 6465 3d6d 6f64 652c 656e 636f  h,mode=mode,enco
+00000900: 6469 6e67 3d65 6e63 6f64 696e 6729 0d0a  ding=encoding)..
+00000910: 2020 2020 662e 7772 6974 6528 7465 7874      f.write(text
+00000920: 2e73 7472 6970 2829 2b22 5c6e 2229 0d0a  .strip()+"\n")..
+00000930: 2020 2020 662e 636c 6f73 6528 290d 0a0d      f.close()...
+00000940: 0a64 6566 2067 6574 5f64 6174 615f 6578  .def get_data_ex
+00000950: 6365 6c28 6578 6365 6c5f 7061 7468 2c63  cel(excel_path,c
+00000960: 6f6c 756d 6e5f 6964 2c73 6865 6574 5f6e  olumn_id,sheet_n
+00000970: 616d 653d 4e6f 6e65 293a 0d0a 2020 2020  ame=None):..    
+00000980: 2727 270d 0a20 2020 2050 6172 616d 6574  '''..    Paramet
+00000990: 6572 730d 0a20 2020 202d 2d2d 2d2d 2d2d  ers..    -------
+000009a0: 2d2d 2d0d 0a20 2020 2065 7863 656c 5f70  ---..    excel_p
+000009b0: 6174 6820 3a20 5459 5045 0d0a 2020 2020  ath : TYPE..    
+000009c0: 2020 2020 4445 5343 5249 5054 494f 4e2e      DESCRIPTION.
+000009d0: 2044 3a5c 6461 7461 5f70 7974 686f 6e2e   D:\data_python.
+000009e0: 786c 7378 0d0a 2020 2020 2020 2020 0d0a  xlsx..        ..
+000009f0: 2020 2020 636f 6c75 6d6e 5f69 6420 3a20      column_id : 
+00000a00: 5459 5045 2049 6e74 2030 2c31 2c32 2c33  TYPE Int 0,1,2,3
+00000a10: 0d0a 2020 2020 2020 2020 4445 5343 5249  ..        DESCRI
+00000a20: 5054 494f 4e2e 2030 206d 6561 6e73 2074  PTION. 0 means t
+00000a30: 6865 2066 6972 7374 2063 6f6c 756d 6e2c  he first column,
+00000a40: 2031 206d 6561 6e73 2074 6865 2073 6563   1 means the sec
+00000a50: 6f6e 642e 0d0a 2020 2020 2020 2020 0d0a  ond...        ..
+00000a60: 2020 2020 7368 6565 745f 6e61 6d65 203a      sheet_name :
+00000a70: 2054 5950 452c 206f 7074 696f 6e61 6c0d   TYPE, optional.
+00000a80: 0a20 2020 2020 2020 2044 4553 4352 4950  .        DESCRIP
+00000a90: 5449 4f4e 2e20 5468 6520 6465 6661 756c  TION. The defaul
+00000aa0: 7420 6973 204e 6f6e 652e 0d0a 0d0a 2020  t is None.....  
+00000ab0: 2020 5265 7475 726e 730d 0a20 2020 202d    Returns..    -
+00000ac0: 2d2d 2d2d 2d2d 0d0a 2020 2020 5459 5045  ------..    TYPE
+00000ad0: 206c 6973 740d 0a20 2020 2020 2020 2044   list..        D
+00000ae0: 4553 4352 4950 5449 4f4e 2e20 7265 7475  ESCRIPTION. retu
+00000af0: 726e 2061 206c 6973 7420 6f66 2064 6174  rn a list of dat
+00000b00: 612e 0d0a 2020 2020 2727 270d 0a20 2020  a...    '''..   
+00000b10: 200d 0a20 2020 2069 6d70 6f72 7420 7061   ..    import pa
+00000b20: 6e64 6173 2061 7320 7064 0d0a 2020 2020  ndas as pd..    
+00000b30: 6966 2073 6865 6574 5f6e 616d 6520 6973  if sheet_name is
+00000b40: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00000b50: 7368 6565 745f 6e61 6d65 3d30 0d0a 2020  sheet_name=0..  
+00000b60: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+00000b70: 7368 6565 745f 6e61 6d65 3d73 6865 6574  sheet_name=sheet
+00000b80: 5f6e 616d 6520 200d 0a20 2020 2064 663d  _name  ..    df=
+00000b90: 7064 2e72 6561 645f 6578 6365 6c28 6578  pd.read_excel(ex
+00000ba0: 6365 6c5f 7061 7468 2c6b 6565 705f 6465  cel_path,keep_de
+00000bb0: 6661 756c 745f 6e61 3d46 616c 7365 2c20  fault_na=False, 
+00000bc0: 7368 6565 745f 6e61 6d65 3d73 6865 6574  sheet_name=sheet
+00000bd0: 5f6e 616d 652c 6865 6164 6572 3d4e 6f6e  _name,header=Non
+00000be0: 6529 200d 0a20 2020 2069 6e74 6572 3d64  e) ..    inter=d
+00000bf0: 662e 696c 6f63 5b30 3a2c 636f 6c75 6d6e  f.iloc[0:,column
+00000c00: 5f69 645d 2023 e68f 90e5 8f96 e7ac ace4  _id] #..........
+00000c10: ba8c e588 97e6 8980 e69c 89e8 a18c 2020  ..............  
+00000c20: 0d0a 2020 2020 7265 7475 726e 206c 6973  ..    return lis
+00000c30: 7428 696e 7465 7229 0d0a 0d0a 6465 6620  t(inter)....def 
+00000c40: 7772 6974 655f 746f 5f65 7863 656c 2865  write_to_excel(e
+00000c50: 7863 656c 5f70 6174 682c 6469 635f 6f66  xcel_path,dic_of
+00000c60: 5f6c 6973 742c 7368 6565 745f 6e61 6d65  _list,sheet_name
+00000c70: 3d4e 6f6e 652c 696e 6465 783d 4e6f 6e65  =None,index=None
+00000c80: 293a 0d0a 2020 2020 2727 270d 0a20 2020  ):..    '''..   
+00000c90: 2050 6172 616d 6574 6572 730d 0a20 2020   Parameters..   
+00000ca0: 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020   ----------..   
+00000cb0: 2065 7863 656c 5f70 6174 6820 3a20 5459   excel_path : TY
+00000cc0: 5045 0d0a 2020 2020 2020 2020 4445 5343  PE..        DESC
+00000cd0: 5249 5054 494f 4e2e 2044 3a5c 7265 7375  RIPTION. D:\resu
+00000ce0: 6c74 732e 786c 7378 0d0a 2020 2020 2020  lts.xlsx..      
+00000cf0: 2020 0d0a 2020 2020 6469 635f 6f66 5f6c    ..    dic_of_l
+00000d00: 6973 7420 3a20 5459 5045 0d0a 2020 2020  ist : TYPE..    
+00000d10: 2020 2020 4445 5343 5249 5054 494f 4e2e      DESCRIPTION.
+00000d20: 207b 2263 6f6c 223a 5b22 6122 2c22 6222   {"col":["a","b"
+00000d30: 2c22 6322 2c22 6422 5d2c 2266 7265 7122  ,"c","d"],"freq"
+00000d40: 3a5b 312c 322c 332c 345d 7d0d 0a20 2020  :[1,2,3,4]}..   
+00000d50: 2020 2020 200d 0a20 2020 2073 6865 6574       ..    sheet
+00000d60: 5f6e 616d 6520 3a20 5459 5045 2c20 6f70  _name : TYPE, op
+00000d70: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
+00000d80: 4445 5343 5249 5054 494f 4e2e 2054 6865  DESCRIPTION. The
+00000d90: 2064 6566 6175 6c74 2069 7320 4e6f 6e65   default is None
+00000da0: 2e0d 0a20 2020 2020 2020 200d 0a20 2020  ...        ..   
+00000db0: 2069 6e64 6578 203a 2054 5950 452c 206f   index : TYPE, o
+00000dc0: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
+00000dd0: 2044 4553 4352 4950 5449 4f4e 2e20 5468   DESCRIPTION. Th
+00000de0: 6520 6465 6661 756c 7420 6973 204e 6f6e  e default is Non
+00000df0: 652e 0d0a 2020 2020 2020 2020 0d0a 2020  e...        ..  
+00000e00: 2020 5265 7475 726e 730d 0a20 2020 202d    Returns..    -
+00000e10: 2d2d 2d2d 2d2d 0d0a 2020 2020 4e6f 6e65  ------..    None
+00000e20: 2e0d 0a0d 0a20 2020 2027 2727 0d0a 2020  .....    '''..  
+00000e30: 2020 696d 706f 7274 2070 616e 6461 7320    import pandas 
+00000e40: 6173 2070 640d 0a20 2020 2069 6620 7368  as pd..    if sh
+00000e50: 6565 745f 6e61 6d65 2069 7320 4e6f 6e65  eet_name is None
+00000e60: 3a0d 0a20 2020 2020 2020 2073 6865 6574  :..        sheet
+00000e70: 5f6e 616d 653d 2273 6865 6574 3122 0d0a  _name="sheet1"..
+00000e80: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00000e90: 2020 7368 6565 745f 6e61 6d65 3d73 6865    sheet_name=she
+00000ea0: 6574 5f6e 616d 650d 0a20 2020 2069 6620  et_name..    if 
+00000eb0: 696e 6465 7820 6973 204e 6f6e 653a 0d0a  index is None:..
+00000ec0: 2020 2020 2020 2020 696e 6465 783d 4661          index=Fa
+00000ed0: 6c73 650d 0a20 2020 2065 6c73 653a 0d0a  lse..    else:..
+00000ee0: 2020 2020 2020 2020 696e 6465 783d 5472          index=Tr
+00000ef0: 7565 2020 2020 2020 2020 0d0a 2020 2020  ue        ..    
+00000f00: 2020 2020 0d0a 2020 2020 6466 3d70 642e      ..    df=pd.
+00000f10: 4461 7461 4672 616d 6528 6469 635f 6f66  DataFrame(dic_of
+00000f20: 5f6c 6973 7429 0d0a 2020 2020 6466 2e73  _list)..    df.s
+00000f30: 7479 6c65 2e74 6f5f 6578 6365 6c28 6578  tyle.to_excel(ex
+00000f40: 6365 6c5f 7061 7468 2c20 7368 6565 745f  cel_path, sheet_
+00000f50: 6e61 6d65 3d73 6865 6574 5f6e 616d 652c  name=sheet_name,
+00000f60: 7374 6172 7463 6f6c 3d30 2c20 696e 6465  startcol=0, inde
+00000f70: 783d 696e 6465 7829 0d0a 2020 2020 0d0a  x=index)..    ..
+00000f80: 200d 0a64 6566 2067 6574 5f64 6174 615f   ..def get_data_
+00000f90: 6a73 6f6e 286a 736f 6e5f 7061 7468 293a  json(json_path):
+00000fa0: 0d0a 2020 2020 2727 270d 0a20 2020 2050  ..    '''..    P
+00000fb0: 6172 616d 6574 6572 730d 0a20 2020 202d  arameters..    -
+00000fc0: 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020 206a  ---------..    j
+00000fd0: 736f 6e5f 7061 7468 203a 2054 5950 4520  son_path : TYPE 
+00000fe0: 443a 5c64 6174 612e 6a73 6f6e 0d0a 2020  D:\data.json..  
+00000ff0: 2020 2020 2020 4445 5343 5249 5054 494f        DESCRIPTIO
+00001000: 4e2e 0d0a 0d0a 2020 2020 5265 7475 726e  N.....    Return
+00001010: 730d 0a20 2020 202d 2d2d 2d2d 2d2d 0d0a  s..    -------..
+00001020: 2020 2020 6c6f 6164 5f64 6963 7420 3a20      load_dict : 
+00001030: 5459 5045 2064 6963 740d 0a20 2020 2020  TYPE dict..     
+00001040: 2020 2044 4553 4352 4950 5449 4f4e 2e20     DESCRIPTION. 
+00001050: 7265 7475 726e 2061 2064 6963 7420 6f66  return a dict of
+00001060: 2064 6174 612e 0d0a 2020 2020 2727 270d   data...    '''.
+00001070: 0a20 2020 2069 6d70 6f72 7420 6a73 6f6e  .    import json
+00001080: 0d0a 2020 2020 7472 793a 0d0a 2020 2020  ..    try:..    
+00001090: 2020 2020 663d 6f70 656e 286a 736f 6e5f      f=open(json_
+000010a0: 7061 7468 2c22 7222 2c65 6e63 6f64 696e  path,"r",encodin
+000010b0: 673d 2275 7466 2d38 2229 0d0a 2020 2020  g="utf-8")..    
+000010c0: 2020 2020 6c6f 6164 5f64 6963 743d 6a73      load_dict=js
+000010d0: 6f6e 2e6c 6f61 6428 6629 2020 2020 0d0a  on.load(f)    ..
+000010e0: 2020 2020 2020 2020 7265 7475 726e 206c          return l
+000010f0: 6f61 645f 6469 6374 2020 2020 2020 2020  oad_dict        
+00001100: 2020 2020 0d0a 2020 2020 6578 6365 7074      ..    except
+00001110: 3a0d 0a20 2020 2020 2020 2066 3d6f 7065  :..        f=ope
+00001120: 6e28 6a73 6f6e 5f70 6174 682c 2272 222c  n(json_path,"r",
+00001130: 656e 636f 6469 6e67 3d22 7574 662d 382d  encoding="utf-8-
+00001140: 7369 6722 290d 0a20 2020 2020 2020 206c  sig")..        l
+00001150: 6f61 645f 6469 6374 3d6a 736f 6e2e 6c6f  oad_dict=json.lo
+00001160: 6164 2866 2920 2020 200d 0a20 2020 2020  ad(f)    ..     
+00001170: 2020 2072 6574 7572 6e20 6c6f 6164 5f64     return load_d
+00001180: 6963 740d 0a0d 0a64 6566 2077 7269 7465  ict....def write
+00001190: 5f74 6f5f 6a73 6f6e 286a 736f 6e5f 7061  _to_json(json_pa
+000011a0: 7468 2c6d 795f 6469 6329 3a0d 0a20 2020  th,my_dic):..   
+000011b0: 2027 2727 0d0a 2020 2020 5061 7261 6d65   '''..    Parame
+000011c0: 7465 7273 0d0a 2020 2020 2d2d 2d2d 2d2d  ters..    ------
+000011d0: 2d2d 2d2d 0d0a 2020 2020 6a73 6f6e 5f70  ----..    json_p
+000011e0: 6174 6820 3a20 5459 5045 2073 7472 696e  ath : TYPE strin
+000011f0: 670d 0a20 2020 2020 2020 2044 4553 4352  g..        DESCR
+00001200: 4950 5449 4f4e 2e20 443a 5c64 6174 612e  IPTION. D:\data.
+00001210: 6a73 6f6e 0d0a 2020 2020 2020 2020 0d0a  json..        ..
+00001220: 2020 2020 6d79 5f64 6963 203a 2054 5950      my_dic : TYP
+00001230: 4520 6469 6374 206f 7220 6c69 7374 0d0a  E dict or list..
+00001240: 2020 2020 2020 2020 4445 5343 5249 5054          DESCRIPT
+00001250: 494f 4e2e 200d 0a20 2020 2020 2020 2020  ION. ..         
+00001260: 2020 2074 7970 6531 3a20 7b22 7061 6e73     type1: {"pans
+00001270: 223a 317d 0d0a 2020 2020 2020 2020 2020  ":1}..          
+00001280: 2020 7479 7065 323a 207b 2277 6f72 6422    type2: {"word"
+00001290: 3a5b 2261 222c 2262 222c 2263 225d 7d0d  :["a","b","c"]}.
+000012a0: 0a20 2020 2020 2020 2020 2020 2074 7970  .            typ
+000012b0: 6533 3a20 5b7b 2270 616e 7322 3a31 7d2c  e3: [{"pans":1},
+000012c0: 7b22 676c 656e 6e61 223a 327d 5d0d 0a20  {"glenna":2}].. 
+000012d0: 2020 2020 2020 2020 2020 2074 7970 6534             type4
+000012e0: 3a20 5b7b 2277 6f72 6422 3a5b 2261 222c  : [{"word":["a",
+000012f0: 2262 222c 2263 225d 7d2c 7b22 6672 6571  "b","c"]},{"freq
+00001300: 223a 5b31 2c32 2c33 2c34 2c35 2c36 5d7d  ":[1,2,3,4,5,6]}
+00001310: 5d0d 0a0d 0a20 2020 2052 6574 7572 6e73  ]....    Returns
+00001320: 0d0a 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20  ..    -------.. 
+00001330: 2020 204e 6f6e 652e 0d0a 0d0a 2020 2020     None.....    
+00001340: 2727 270d 0a20 2020 2069 6d70 6f72 7420  '''..    import 
+00001350: 6a73 6f6e 0d0a 2020 2020 6632 203d 206f  json..    f2 = o
+00001360: 7065 6e28 6a73 6f6e 5f70 6174 682c 2022  pen(json_path, "
+00001370: 7722 2c20 656e 636f 6469 6e67 3d22 7574  w", encoding="ut
+00001380: 662d 3822 2c20 6572 726f 7273 3d22 6967  f-8", errors="ig
+00001390: 6e6f 7265 2229 0d0a 2020 2020 6632 2e77  nore")..    f2.w
+000013a0: 7269 7465 286a 736f 6e2e 6475 6d70 7328  rite(json.dumps(
+000013b0: 6d79 5f64 6963 2c65 6e73 7572 655f 6173  my_dic,ensure_as
+000013c0: 6369 693d 4661 6c73 6529 2920 2365 6e73  cii=False)) #ens
+000013d0: 7572 655f 6173 6369 693d 4661 6c73 6520  ure_ascii=False 
+000013e0: e8ae a9e4 b8ad e696 87e4 b88d e586 8de4  ................
+000013f0: b9b1 e7a0 810d 0a20 2020 2066 322e 636c  .......    f2.cl
+00001400: 6f73 6528 2920 0d0a 2020 2020 0d0a 6465  ose() ..    ..de
+00001410: 6620 4669 6c65 5061 7468 2872 6f6f 7429  f FilePath(root)
+00001420: 3a0d 0a20 2020 2027 2727 e8af bbe5 8f96  :..    '''......
+00001430: e689 80e6 9c89 e696 87e4 bbb6 efbc 8ce5  ................
+00001440: 8897 e587 bae6 af8f e4b8 aae6 9687 e4bb  ................
+00001450: b6e7 9a84 e8b7 afe5 be84 2727 270d 0a20  ..........'''.. 
+00001460: 2020 2046 696c 656c 6973 743d 5b5d 0d0a     Filelist=[]..
+00001470: 2020 2020 666f 7220 686f 6d65 2c20 6469      for home, di
+00001480: 7273 2c20 6669 6c65 7320 696e 206f 732e  rs, files in os.
+00001490: 7761 6c6b 2872 6f6f 7429 3a0d 0a20 2020  walk(root):..   
+000014a0: 2020 2020 2066 6f72 2066 696c 656e 616d       for filenam
+000014b0: 6520 696e 2066 696c 6573 3a0d 0a20 2020  e in files:..   
+000014c0: 2020 2020 2020 2020 2046 696c 656c 6973           Filelis
+000014d0: 742e 6170 7065 6e64 286f 732e 7061 7468  t.append(os.path
+000014e0: 2e6a 6f69 6e28 686f 6d65 2c20 6669 6c65  .join(home, file
+000014f0: 6e61 6d65 2929 0d0a 2020 2020 7265 7475  name))..    retu
+00001500: 726e 2046 696c 656c 6973 740d 0a0d 0a64  rn Filelist....d
+00001510: 6566 2046 696c 654e 616d 6528 6669 6c65  ef FileName(file
+00001520: 5f70 6174 6829 3a0d 0a20 2020 2069 6e74  _path):..    int
+00001530: 6572 3d6f 732e 7061 7468 2e62 6173 656e  er=os.path.basen
+00001540: 616d 6528 6669 6c65 5f70 6174 6829 0d0a  ame(file_path)..
+00001550: 2020 2020 7265 7475 726e 2069 6e74 6572      return inter
+00001560: 0d0a 0d0a 0d0a 4269 6750 756e 6374 7561  ......BigPunctua
+00001570: 7469 6f6e 3d22 2222 2122 2324 265c 2728  tion="""!"#$&\'(
+00001580: 292a 2b2c 2d2f 3a3b 3c3d 3e3f 405b 5c5c  )*+,-/:;<=>?@[\\
+00001590: 5d5e 5f60 7b7c 7d2e 257e efbc 82ef bc83  ]^_`{|}.%~......
+000015a0: efbc 84ef bc85 efbc 86ef bc87 3fe3 8082  ............?...
+000015b0: efbc 88ef bc89 efbc 8aef bc8b efbc 8cef  ................
+000015c0: bc8d efbc 8fef bc9a efbc 9bef bc9c efbc  ................
+000015d0: 9def bc9e efbc a0ef bcbb efbc bcef bcbd  ................
+000015e0: efbc beef bcbf efbd 80ef bd9b efbd 9cef  ................
+000015f0: bd9d efbd 9eef bd9f efbd a0ef bda2 efbd  ................
+00001600: a3ef bda4 5c75 3330 3030 e380 81e3 8083  ....\u3000......
+00001610: e380 88e3 8089 e380 8ae3 808b e380 8ce3  ................
+00001620: 808d e380 8ee3 808f e380 90e3 8091 e380  ................
+00001630: 94e3 8095 e380 96e3 8097 e380 98e3 8099  ................
+00001640: e380 9ae3 809b e380 9ce3 809d e380 9ee3  ................
+00001650: 809f e380 b0e3 80be e380 bfe2 8093 e280  ................
+00001660: 94e2 8098 e280 99e2 809b e280 9ce2 809d  ................
+00001670: e280 9ee2 809f e280 a6e2 80a7 efb9 8fef  ................
+00001680: b991 efb9 94c2 b7ef bc81 efbc 9fef bda1  ................
+00001690: e380 8260 6027 2722 2222 2020 2023 e999  ...``''"""   #..
+000016a0: a4e5 8ebb e88b b1e6 9687 e6a0 87e7 82b9  ................
+000016b0: 2e25 0d0a 5374 6f70 5461 6773 3d22 2222  .%..StopTags="""
+000016c0: e297 863a 20e3 8081 2f20 e380 822f 202d  ...: .../ .../ -
+000016d0: 2d2d 2f20 2d2f 202d 2d2f 202d 2d20 3a2f  --/ -/ --/ -- :/
+000016e0: 203b 2f20 3f2f 203f 3f2f 203f e294 9620   ;/ ?/ ??/ ?... 
+000016f0: 402f 205b 2f20 5d2f 205e 2f20 e280 982f  @/ [/ ]/ ^/ .../
+00001700: 20e2 8099 2f20 222f 2022 2f20 e380 882f   .../ "/ "/ .../
+00001710: 20e3 8089 2f20 e380 8a2f 20e3 808b 2f20   .../ .../ .../ 
+00001720: e380 902f 20e3 8091 2f20 3e2f 20e2 88b6  .../ .../ >/ ...
+00001730: 2f20 e296 a02f 20e2 978f 2f20 c2b7 2f20  / .../ .../ ../ 
+00001740: e280 a62f 2021 2f20 232f 2025 2c2f 2025  .../ !/ #/ %,/ %
+00001750: 2f20 5c27 2f20 282f 2029 2f20 2a2f 202b  / \'/ (/ )/ */ +
+00001760: 2f20 2c2f 202d 2f20 2f2f 206e 7020 7620  / ,/ -/ // np v 
+00001770: 6e20 7720 6d20 6120 7820 7420 7120 6a20  n w m a x t q j 
+00001780: 6e69 206e 7320 6420 6920 6620 7520 7020  ni ns d i f u p 
+00001790: 6720 6e7a 2063 2072 2069 6420 7320 6b20  g nz c r id s k 
+000017a0: 6820 6f20 6520 2f20 233f 2f20 2d2d 2f22  h o e / #?/ --/"
+000017b0: 2222 2023 e794 a8e6 9da5 e581 9ce7 94a8  "" #............
+000017c0: e8af 8de6 80a7 e6a0 87e6 b3a8 0d0a 5370  ..............Sp
+000017d0: 6563 6961 6c3d 2222 22e2 88b6 20e2 96a0  ecial="""... ...
+000017e0: 20e2 978f 20e2 91a0 20e2 91a1 20e2 91a2   ... ... ... ...
+000017f0: 20c3 9720 e284 8320 e285 a220 e291 a320   .. ... ... ... 
+00001800: e291 a420 e297 8620 e291 a520 c2b1 20e2  ... ... ... .. .
+00001810: 91a6 20e2 91a7 20e2 8692 20e2 91a8 20e2  .. ... ... ... .
+00001820: 96b2 20e2 91a9 20e2 9480 20c3 b720 cebc  .. ... ... .. ..
+00001830: 20ce b320 ceb2 20e2 85a1 20e2 85a0 20e2   .. .. ... ... .
+00001840: 80b0 20e2 96a1 20e3 8087 20e2 978b 20e2  .. ... ... ... .
+00001850: 85a4 20e2 85a3 20e2 9885 20ef b990 20c2  .. ... ... ... .
+00001860: b020 e280 bb20 efb8 b020 ceb1 20e2 8095  . ... ... .. ...
+00001870: 20e2 89a0 20e2 9688 20d0 be20 ceb8 20cf   ... ... .. .. .
+00001880: 8920 e292 8820 e292 8920 e292 8a20 d0bd  . ... ... ... ..
+00001890: 20e2 89a4 20c3 ac20 c78e 20e2 89a5 20d1   ... .. .. ... .
+000018a0: 8020 d182 20d1 8120 d0ba 20d0 b920 d0b0  . .. .. .. .. ..
+000018b0: 20d0 b820 e285 a520 c3a9 20c3 a820 efb9   .. ... .. .. ..
+000018c0: a220 efb9 9d20 efb9 9e20 7f20 c481 20e2  . ... ... . .. .
+000018d0: 928b 20c3 b920 cf80 20e2 9787 20ce a920  .. .. .. ... .. 
+000018e0: d0a4 20d1 8b20 d0af 20d0 bf20 d09a 20d0  .. .. .. .. .. .
+000018f0: b220 d183 20d0 bc20 c792 20c3 bc20 c3a1  . .. .. .. .. ..
+00001900: 20c7 9420 e292 8c20 e292 8d20 e4a6 8620   .. ... ... ... 
+00001910: e285 a920 e285 a620 e286 9020 2222 220d  ... ... ... """.
+00001920: 0a53 746f 7057 6f72 6473 3d22 2222 e280  .StopWords="""..
+00001930: 94e2 8094 e280 9420 e380 8bef bc89 efbc  ....... ........
+00001940: 8c20 efbc 89c3 b7ef bc88 efbc 91ef bc8d  . ..............
+00001950: 20e2 809d efbc 8c20 efbc 89e3 8081 20ef   ...... ...... .
+00001960: bc9d efbc 8820 3a20 e286 9220 e284 8320  ..... : ... ... 
+00001970: 2026 202a 20e4 b880 e4b8 8020 7e7e 7e7e   & * ...... ~~~~
+00001980: 20e2 8099 202e 2020 e380 8e20 2ee4 b880   ... .  ... ....
+00001990: 202e 2f20 2d2d 2020 e380 8f20 efbc 9de2   ./ --  ... ....
+000019a0: 80b3 20e3 8090 20ef bcbb efbc 8aef bcbd  .. ... .........
+000019b0: 20ef bd9d efbc 9e20 efbc bbe2 91a4 efbc   ...... ........
+000019c0: bdef bcbd 20ef bcbb e291 a0ef bca4 efbc  .... ...........
+000019d0: bd20 efbd 83ef bcbd 20ef bd8e efbd 87e6  . ...... .......
+000019e0: 9889 20ef bc8a 202f 2f20 efbc bb20 efbc  .. ... // ... ..
+000019f0: bd20 efbc bbe2 91a1 efbd 85ef bcbd 20ef  . ............ .
+00001a00: bcbb e291 a1ef bd87 efbc bd20 efbc 9def  ........... ....
+00001a10: bd9b 207d 20ef bc8c e4b9 9f20 20e2 8098  .. } ......  ...
+00001a20: 20ef bca1 20ef bcbb e291 a0e2 91a5 efbc   ... ...........
+00001a30: bd20 efbc bbe2 91a1 efbc a2ef bcbd 2020  . ............  
+00001a40: efbc bbe2 91a0 efbd 81ef bcbd 20ef bcbb  ............ ...
+00001a50: e291 a3ef bd81 efbc bd20 efbc bbe2 91a0  ......... ......
+00001a60: e291 a2ef bcbd 20ef bcbb e291 a2ef bd88  ...... .........
+00001a70: efbc bd20 e291 a2ef bcbd 20ef bc91 efbc  ... ...... .....
+00001a80: 8e20 20ef bc8d efbc 8d20 20ef bcbb e291  .  ......  .....
+00001a90: a1ef bd82 efbc bd20 e280 99e2 8098 2020  ....... ......  
+00001aa0: c397 c397 c397 2020 efbc bbe2 91a0 e291  ......  ........
+00001ab0: a7ef bcbd 20ef bc90 efbc 9aef bc92 2020  .... .........  
+00001ac0: efbc 9def bcbb 20ef bcbb e291 a4ef bd82  ...... .........
+00001ad0: efbc bd20 efbc bbe2 91a1 efbd 83ef bcbd  ... ............
+00001ae0: 2020 efbc bbe2 91a3 efbd 82ef bcbd 20ef    ............ .
+00001af0: bcbb e291 a1e2 91a2 efbc bd20 efbc bbe2  ........... ....
+00001b00: 91a2 efbd 81ef bcbd 20ef bcbb e291 a3ef  ........ .......
+00001b10: bd83 efbc bd20 efbc bbe2 91a0 e291 a4ef  ..... ..........
+00001b20: bcbd 20ef bcbb e291 a0e2 91a6 efbc bd20  .. ............ 
+00001b30: efbc bbe2 91a0 efbd 87ef bcbd 20e2 8888  ............ ...
+00001b40: efbc bb20 20ef bcbb e291 a0e2 91a8 efbc  ...  ...........
+00001b50: bd20 efbc bbe2 91a0 e291 a3ef bcbd 20ef  . ............ .
+00001b60: bcbb e291 a0ef bd83 efbc bd20 efbc bbe2  ........... ....
+00001b70: 91a1 efbd 86ef bcbd 20ef bcbb e291 a1e2  ........ .......
+00001b80: 91a7 efbc bd20 efbc bbe2 91a1 e291 a0ef  ..... ..........
+00001b90: bcbd 20ef bcbb e291 a0ef bca3 efbc bd20  .. ............ 
+00001ba0: efbc bbe2 91a2 efbd 83ef bcbd 20ef bcbb  ............ ...
+00001bb0: e291 a2ef bd87 efbc bd20 efbc bbe2 91a1  ......... ......
+00001bc0: e291 a4ef bcbd 20ef bcbb e291 a1e2 91a1  ...... .........
+00001bd0: efbc bd20 e4b8 802e 20ef bcbb e291 a0ef  ... .... .......
+00001be0: bd88 efbc bd20 2ee6 95b0 20ef bcbb efbc  ..... .... .....
+00001bf0: bd20 efbc bbe2 91a0 efbc a2ef bcbd 20e6  . ............ .
+00001c00: 95b0 2f20 efbc bbe2 91a0 efbd 89ef bcbd  ../ ............
+00001c10: 20ef bcbb e291 a2ef bd85 efbc bd20 efbc   ............ ..
+00001c20: bbe2 91a0 e291 a0ef bcbd 20ef bcbb e291  .......... .....
+00001c30: a3ef bd84 efbc bd20 efbc bbe2 91a3 efbd  ....... ........
+00001c40: 85ef bcbd 20ef bcbb e291 a2ef bd82 efbc  .... ...........
+00001c50: bd20 efbc bbe2 91a4 efbd 81ef bcbd 20ef  . ............ .
+00001c60: bcbb e291 a0ef bca1 efbc bd20 efbc bbe2  ........... ....
+00001c70: 91a1 e291 a7ef bcbd 20ef bcbb e291 a1e2  ........ .......
+00001c80: 91a6 efbc bd20 efbc bbe2 91a0 efbd 84ef  ..... ..........
+00001c90: bcbd 20ef bcbb e291 a1ef bd8a efbc bd20  .. ............ 
+00001ca0: e380 95e3 8094 20ef bcbd efbc bb20 3a2f  ...... ...... :/
+00001cb0: 2f20 e280 b2e2 8888 20ef bcbb e291 a1e2  / ...... .......
+00001cc0: 91a3 20ef bcbb e291 a4ef bd85 efbc bd20  .. ............ 
+00001cd0: efbc 91ef bc92 efbc 8520 efbd 82ef bcbd  ......... ......
+00001ce0: 202e 2e2e 202e 2e2e 2e2e 2e2e 2e2e 2e2e   ... ...........
+00001cf0: 2e2e 2e2e 2e2e 2e2e 20e2 80a6 e280 a6e2  ........ .......
 00001d00: 80a6 e280 a6e2 80a6 e280 a6e2 80a6 e280  ................
-00001d10: a6e2 80a6 e291 a220 efbc baef bcb8 efbc  ....... ........
-00001d20: a6ef bca9 efbc b4ef bcac 20ef bcbb e291  .......... .....
-00001d30: a2ef bca6 efbc bd20 e380 8d20 efbc bbe2  ....... ... ....
-00001d40: 91a0 efbd 8fef bcbd 20ef bcbd e288 a7e2  ........ .......
-00001d50: 80b2 efbc 9def bcbb 2020 e288 aacf 86e2  ........  ......
-00001d60: 8888 20e2 80b2 efbd 9c20 efbd 9bef bc8d  .. ...... ......
-00001d70: 20e2 91a1 efbd 8320 efbd 9d20 efbc bbe2   ...... ... ....
-00001d80: 91a2 e291 a0ef bcbd 20ef bcb2 efbc 8eef  ........ .......
-00001d90: bcac efbc 8e20 efbc bbe2 91a0 efbc a5ef  ..... ..........
-00001da0: bcbd 20ce a820 efbc 8def bcbb efbc 8aef  .. .. ..........
-00001db0: bcbd efbc 8d20 e286 9120 2ee6 97a5 2020  ..... ... ....  
-00001dc0: efbc bbe2 91a1 efbd 84ef bcbd 20ef bcbb  ............ ...
-00001dd0: e291 a120 efbc bbe2 91a1 e291 a6ef bcbd  ... ............
-00001de0: 20ef bcbb e291 a1e2 91a1 efbc bd20 efbc   ............ ..
-00001df0: bbe2 91a2 efbd 85ef bcbd 20ef bcbb e291  .......... .....
-00001e00: a0ef bd89 efbc bd20 efbc bbe2 91a0 efbc  ....... ........
-00001e10: a2ef bcbd 20ef bcbb e291 a0ef bd88 efbc  .... ...........
-00001e20: bd20 efbc bbe2 91a0 efbd 84ef bcbd 20ef  . ............ .
-00001e30: bcbb e291 a0ef bd87 efbc bd20 efbc bbe2  ........... ....
-00001e40: 91a0 e291 a1ef bcbd 20ef bcbb e291 a1ef  ........ .......
-00001e50: bd81 efbc bd20 efbd 86ef bcbd 20ef bcbb  ..... ...... ...
-00001e60: e291 a9ef bcbd 20ef bd81 efbc bd20 efbc  ...... ...... ..
-00001e70: bbe2 91a0 efbd 85ef bcbd 20ef bcbb e291  .......... .....
-00001e80: a1ef bd88 efbc bd20 efbc bbe2 91a1 e291  ....... ........
-00001e90: a5ef bcbd 20ef bcbb e291 a2ef bd84 efbc  .... ...........
-00001ea0: bd20 efbc bbe2 91a1 e291 a9ef bcbd 20ef  . ............ .
-00001eb0: bd85 efbc bd20 e380 8920 e380 9120 e585  ..... ... ... ..
-00001ec0: 83ef bc8f e590 a820 efbc bbe2 91a1 e291  ....... ........
-00001ed0: a9ef bcbd 20ef bc92 efbc 8eef bc93 efbc  .... ...........
-00001ee0: 8520 efbc 95ef bc9a efbc 9020 2020 efbc  . .........   ..
-00001ef0: bbe2 91a0 efbc bd20 3a3a 20ef bcbb e291  ....... :: .....
-00001f00: a1ef bcbd 20ef bcbb e291 a2ef bcbd 20ef  .... ......... .
-00001f10: bcbb e291 a3ef bcbd 20ef bcbb e291 a4ef  ........ .......
-00001f20: bcbd 20ef bcbb e291 a5ef bcbd 20ef bcbb  .. ......... ...
-00001f30: e291 a6ef bcbd 20ef bcbb e291 a7ef bcbd  ...... .........
-00001f40: 20ef bcbb e291 a8ef bcbd 2020 e280 a6e2   .........  ....
-00001f50: 80a6 20e2 8094 e280 9420 3f20 e380 8120  .. ...... ? ... 
-00001f60: e380 8220 e280 9c20 e280 9d20 e380 8a20  ... ... ... ... 
-00001f70: e380 8b20 efbc 8120 efbc 8c20 efbc 9a20  ... ... ... ... 
-00001f80: efbc 9b20 efbc 9f20 efbc 8e20 2c20 efbc  ... ... ... , ..
-00001f90: 8e20 2720 3f20 20c2 b720 e280 94e2 8094  . ' ?  .. ......
-00001fa0: e280 9420 e294 80e2 9480 203f 2020 e280  ... ...... ?  ..
-00001fb0: 9420 3c20 3e20 efbc 8820 efbc 8920 e380  . < > ... ... ..
-00001fc0: 9420 e380 9520 5b20 5d20 2820 2920 2d20  . ... [ ] ( ) - 
-00001fd0: 2b20 efbd 9e20 c397 20ef bc8f 202f 20e2  + ... .. ... / .
-00001fe0: 91a0 20e2 91a1 20e2 91a2 20e2 91a3 20e2  .. ... ... ... .
-00001ff0: 91a4 20e2 91a5 20e2 91a6 20e2 91a7 20e2  .. ... ... ... .
-00002000: 91a8 20e2 91a9 20e2 85a2 20d0 9220 2220  .. ... ... .. " 
-00002010: 3b20 2320 4020 ceb3 20ce bc20 cf86 20cf  ; # @ .. .. .. .
-00002020: 86ef bc8e 20c3 9720 20ce 9420 e296 a020  .... ..  .. ... 
-00002030: e296 b220 7375 6220 6578 7020 2073 7570  ... sub exp  sup
-00002040: 2073 7562 204c 6578 2020 efbc 8320 efbc   sub Lex  ... ..
-00002050: 8520 efbc 8620 efbc 8720 efbc 8b20 efbc  . ... ... ... ..
-00002060: 8bce be20 efbc 8bef bc8b 20ef bc8d 20ef  ... ...... ... .
-00002070: bc8d ceb2 20ef bc9c 20ef bc9c c2b1 20ef  .... ... ..... .
-00002080: bc9c ce94 20ef bc9c cebb 20ef bc9c cf86  .... ..... .....
-00002090: 20ef bc9c efbc 9c20 3d20 efbc 9d20 efbc   ...... = ... ..
-000020a0: 9de2 9886 20ef bc9d efbc 8d20 efbc 9e20  .... ...... ... 
-000020b0: efbc 9ece bb20 efbc bf20 efbd 9ec2 b120  ..... ... ..... 
-000020c0: efbd 9eef bc8b 20ef bcbb e291 a4ef bd86  ...... .........
-000020d0: efbc bd20 efbc bbe2 91a4 efbd 84ef bcbd  ... ............
-000020e0: 20ef bcbb e291 a1ef bd89 efbc bd20 e289   ............ ..
-000020f0: 8820 20ef bcbb e291 a1ef bca7 efbc bd20  .  ............ 
-00002100: efbc bbe2 91a0 efbd 86ef bcbd 20ef bcac  ............ ...
-00002110: efbc a920 e388 a720 20ef bcbb efbc 8d20  ... ...  ...... 
-00002120: 2e2e 2e2e 2e2e 20e3 8089 20ef bcbb e291  ...... ... .....
-00002130: a2e2 91a9 efbc bd20 e7ac ace4 ba8c 20e4  ....... ...... .
-00002140: b880 e795 aa20 e4b8 80e7 9bb4 20e4 b880  ..... ...... ...
-00002150: e4b8 aa20 e4b8 80e4 ba9b 20e8 aeb8 e5a4  ... ...... .....
-00002160: 9a20 e7a7 8d20 e69c 89e7 9a84 e698 af20  . ... ......... 
-00002170: e4b9 9fe5 b0b1 e698 afe8 afb4 20e6 9cab  ............ ...
-00002180: 2323 e69c ab20 e595 8a20 e998 bf20 e593  ##... ... ... ..
-00002190: 8e20 e593 8ee5 9180 20e5 938e e593 9f20  . ...... ...... 
-000021a0: e594 8920 e4bf ba20 e4bf bae4 bbac 20e6  ... ... ...... .
-000021b0: 8c89 20e6 8c89 e785 a720 e590 a720 e590  .. ...... ... ..
-000021c0: a7e5 9392 20e6 8a8a 20e7 bda2 e4ba 8620  .... ... ...... 
-000021d0: e8a2 ab20 e69c ac20 e69c ace7 9d80 20e6  ... ... ...... .
-000021e0: af94 20e6 af94 e696 b920 e6af 94e5 a682  .. ...... ......
-000021f0: 20e9 8499 e4ba ba20 e5bd bc20 e5bd bce6   ...... ... ....
-00002200: ada4 20e8 beb9 20e5 88ab 20e5 88ab e79a  .. ... ... .....
-00002210: 8420 e588 abe8 afb4 20e5 b9b6 20e5 b9b6  . ...... ... ...
-00002220: e4b8 9420 e4b8 8de6 af94 20e4 b88d e688  ... ...... .....
-00002230: 9020 e4b8 8de5 8d95 20e4 b88d e4bd 8620  . ...... ...... 
-00002240: e4b8 8de7 8bac 20e4 b88d e7ae a120 e4b8  ...... ...... ..
-00002250: 8de5 8589 20e4 b88d e8bf 8720 e4b8 8de4  .... ...... ....
-00002260: bb85 20e4 b88d e68b 9820 e4b8 8de8 aeba  .. ...... ......
-00002270: 20e4 b88d e680 9520 e4b8 8de7 84b6 20e4   ...... ...... .
-00002280: b88d e5a6 8220 e4b8 8de7 89b9 20e4 b88d  ..... ...... ...
-00002290: e683 9f20 e4b8 8de9 97ae 20e4 b88d e58f  ... ...... .....
-000022a0: aa20 e69c 9d20 e69c 9de7 9d80 20e8 b681  . ... ...... ...
-000022b0: 20e8 b681 e79d 8020 e4b9 9820 e586 b220   ...... ... ... 
-000022c0: e999 a420 e999 a4e6 ada4 e4b9 8be5 a496  ... ............
-000022d0: 20e9 99a4 e99d 9e20 e999 a4e4 ba86 20e6   ...... ...... .
-000022e0: ada4 20e6 ada4 e997 b420 e6ad a4e5 a496  .. ...... ......
-000022f0: 20e4 bb8e 20e4 bb8e e880 8c20 e689 9320   ... ...... ... 
-00002300: e5be 8520 e4bd 8620 e4bd 86e6 98af 20e5  ... ... ...... .
-00002310: bd93 20e5 bd93 e79d 8020 e588 b020 e5be  .. ...... ... ..
-00002320: 9720 e79a 8420 e79a 84e8 af9d 20e7 ad89  . ... ...... ...
-00002330: 20e7 ad89 e7ad 8920 e59c b020 e7ac ac20   ...... ... ... 
-00002340: e58f aee5 929a 20e5 afb9 20e5 afb9 e4ba  ...... ... .....
-00002350: 8e20 e5a4 9a20 e5a4 9ae5 b091 20e8 808c  . ... ...... ...
-00002360: 20e8 808c e586 b520 e880 8ce4 b894 20e8   ...... ...... .
-00002370: 808c e698 af20 e880 8ce5 a496 20e8 808c  ..... ...... ...
-00002380: e8a8 8020 e880 8ce5 b7b2 20e5 b094 e590  ... ...... .....
-00002390: 8e20 e58f 8de8 bf87 e69d a520 e58f 8de8  . ......... ....
-000023a0: bf87 e69d a5e8 afb4 20e5 8f8d e4b9 8b20  ........ ...... 
-000023b0: e99d 9ee4 bd86 20e9 9d9e e5be 9220 e590  ...... ...... ..
-000023c0: a6e5 8899 20e5 988e 20e5 988e e799 bb20  .... ... ...... 
-000023d0: e8af a520 e8b5 b620 e4b8 aa20 e590 8420  ... ... ... ... 
-000023e0: e590 84e4 b8aa 20e5 9084 e4bd 8d20 e590  ...... ...... ..
-000023f0: 84e7 a78d 20e5 9084 e887 aa20 e7bb 9920  .... ...... ... 
-00002400: e6a0 b9e6 8dae 20e8 b79f 20e6 9585 20e6  ...... ... ... .
-00002410: 9585 e6ad a420 e59b bae7 84b6 20e5 85b3  ..... ...... ...
-00002420: e4ba 8e20 e7ae a120 e5bd 9220 e69e 9ce7  ... ... ... ....
-00002430: 84b6 20e6 9e9c e79c 9f20 e8bf 8720 e593  .. ...... ... ..
-00002440: 8820 e593 88e5 9388 20e5 91b5 20e5 928c  . ...... ... ...
-00002450: 20e4 bd95 20e4 bd95 e5a4 8420 e4bd 95e5   ... ...... ....
-00002460: 86b5 20e4 bd95 e697 b620 e598 bf20 e593  .. ...... ... ..
-00002470: bc20 e593 bce5 94b7 20e5 91bc e593 a720  . ...... ...... 
-00002480: e4b9 8e20 e593 9720 e8bf 98e6 98af 20e8  ... ... ...... .
-00002490: bf98 e69c 8920 e68d a2e5 8fa5 e8af 9de8  ..... ..........
-000024a0: afb4 20e6 8da2 e8a8 80e4 b98b 20e6 8896  .. ......... ...
-000024b0: 20e6 8896 e698 af20 e688 96e8 8085 20e6   ...... ...... .
-000024c0: 9e81 e4ba 8620 e58f 8a20 e58f 8ae5 85b6  ..... ... ......
-000024d0: 20e5 8f8a e887 b320 e58d b320 e58d b3e4   ...... ... ....
-000024e0: bebf 20e5 8db3 e688 9620 e58d b3e4 bba4  .. ...... ......
-000024f0: 20e5 8db3 e88b a520 e58d b3e4 bdbf 20e5   ...... ...... .
-00002500: 87a0 20e5 87a0 e697 b620 e5b7 b120 e697  .. ...... ... ..
-00002510: a220 e697 a2e7 84b6 20e6 97a2 e698 af20  . ...... ...... 
-00002520: e7bb a7e8 808c 20e5 8aa0 e4b9 8b20 e581  ...... ...... ..
-00002530: 87e5 a682 20e5 8187 e88b a520 e581 87e4  .... ...... ....
-00002540: bdbf 20e9 89b4 e4ba 8e20 e5b0 8620 e8be  .. ...... ... ..
-00002550: 8320 e8be 83e4 b98b 20e5 8fab 20e6 8ea5  . ...... ... ...
-00002560: e79d 8020 e7bb 93e6 9e9c 20e5 809f 20e7  ... ...... ... .
-00002570: b4a7 e68e a5e7 9d80 20e8 bf9b e880 8c20  ........ ...... 
-00002580: e5b0 bd20 e5b0 bde7 aea1 20e7 bb8f 20e7  ... ...... ... .
-00002590: bb8f e8bf 8720 e5b0 b120 e5b0 b1e6 98af  ..... ... ......
-000025a0: 20e5 b0b1 e698 afe8 afb4 20e6 8dae 20e5   ......... ... .
-000025b0: 85b7 e4bd 93e5 9cb0 e8af b420 e585 b7e4  ........... ....
-000025c0: bd93 e8af b4e6 9da5 20e5 bc80 e5a7 8b20  ........ ...... 
-000025d0: e5bc 80e5 a496 20e9 9da0 20e5 92b3 20e5  ...... ... ... .
-000025e0: 8faf 20e5 8faf e8a7 8120 e58f afe6 98af  .. ...... ......
-000025f0: 20e5 8faf e4bb a520 e586 b5e4 b894 20e5   ...... ...... .
-00002600: 95a6 20e6 9da5 20e6 9da5 e79d 8020 e7a6  .. ... ...... ..
-00002610: bb20 e4be 8be5 a682 20e5 93a9 20e8 bf9e  . ...... ... ...
-00002620: 20e8 bf9e e590 8c20 e4b8 a4e8 8085 20e4   ...... ...... .
-00002630: ba86 20e4 b8b4 20e5 8fa6 20e5 8fa6 e5a4  .. ... ... .....
-00002640: 9620 e58f a6e4 b880 e696 b9e9 9da2 20e8  . ............ .
-00002650: aeba 20e5 989b 20e5 9097 20e6 85a2 e8af  .. ... ... .....
-00002660: b420 e6bc abe8 afb4 20e5 8692 20e4 b988  . ...... ... ...
-00002670: 20e6 af8f 20e6 af8f e5bd 9320 e4bb ac20   ... ...... ... 
-00002680: e88e abe8 8ba5 20e6 9f90 20e6 9f90 e4b8  ...... ... .....
-00002690: aa20 e69f 90e4 ba9b 20e6 8bbf 20e5 93aa  . ...... ... ...
-000026a0: 20e5 93aa e8be b920 e593 aae5 84bf 20e5   ...... ...... .
-000026b0: 93aa e4b8 aa20 e593 aae9 878c 20e5 93aa  ..... ...... ...
-000026c0: e5b9 b420 e593 aae6 8095 20e5 93aa e5a4  ... ...... .....
-000026d0: a920 e593 aae4 ba9b 20e5 93aa e6a0 b720  . ...... ...... 
-000026e0: e982 a320 e982 a3e8 beb9 20e9 82a3 e584  ... ...... .....
-000026f0: bf20 e982 a3e4 b8aa 20e9 82a3 e4bc 9ae5  . ...... .......
-00002700: 84bf 20e9 82a3 e987 8c20 e982 a3e4 b988  .. ...... ......
-00002710: 20e9 82a3 e4b9 88e4 ba9b 20e9 82a3 e4b9   ......... .....
-00002720: 88e6 a0b7 20e9 82a3 e697 b620 e982 a3e4  .... ...... ....
-00002730: ba9b 20e9 82a3 e6a0 b720 e4b9 8320 e4b9  .. ...... ... ..
-00002740: 83e8 87b3 20e5 91a2 20e8 83bd 20e4 bda0  .... ... ... ...
-00002750: 20e4 bda0 e4bb ac20 e682 a820 e5ae 8120   ...... ... ... 
-00002760: e5ae 81e5 8faf 20e5 ae81 e882 af20 e5ae  ...... ...... ..
-00002770: 81e6 84bf 20e5 93a6 20e5 9195 20e5 95aa  .... ... ... ...
-00002780: e8be be20 e697 81e4 baba 20e5 91b8 20e5  ... ...... ... .
-00002790: 87ad 20e5 87ad e580 9f20 e585 b620 e585  .. ...... ... ..
-000027a0: b6e6 aca1 20e5 85b6 e4ba 8c20 e585 b6e4  .... ...... ....
-000027b0: bb96 20e5 85b6 e5ae 8320 e585 b6e4 b880  .. ...... ......
-000027c0: 20e5 85b6 e4bd 9920 e585 b6e4 b8ad 20e8   ...... ...... .
-000027d0: b5b7 20e8 b5b7 e8a7 8120 e8b5 b7e8 a781  .. ...... ......
-000027e0: 20e5 b282 e4bd 8620 e681 b0e6 81b0 e79b   ...... ........
-000027f0: b8e5 8f8d 20e5 898d e590 8e20 e589 8de8  .... ...... ....
-00002800: 8085 20e4 b894 20e7 84b6 e880 8c20 e784  .. ... ...... ..
-00002810: b6e5 908e 20e7 84b6 e588 9920 e8ae a920  .... ...... ... 
-00002820: e4ba bae5 aeb6 20e4 bbbb 20e4 bbbb e4bd  ...... ... .....
-00002830: 9520 e4bb bbe5 87ad 20e5 a682 20e5 a682  . ...... ... ...
-00002840: e6ad a420 e5a6 82e6 9e9c 20e5 a682 e4bd  ... ...... .....
-00002850: 9520 e5a6 82e5 85b6 20e5 a682 e88b a520  . ...... ...... 
-00002860: e5a6 82e4 b88a e689 80e8 bfb0 20e8 8ba5  ............ ...
-00002870: 20e8 8ba5 e99d 9e20 e88b a5e6 98af 20e5   ...... ...... .
-00002880: 95a5 20e4 b88a e4b8 8b20 e5b0 9ae4 b894  .. ...... ......
-00002890: 20e8 aebe e88b a520 e8ae bee4 bdbf 20e7   ...... ...... .
-000028a0: 949a e880 8c20 e794 9ae4 b988 20e7 949a  ..... ...... ...
-000028b0: e887 b320 e79c 81e5 be97 20e6 97b6 e580  ... ...... .....
-000028c0: 9920 e4bb 80e4 b988 20e4 bb80 e4b9 88e6  . ...... .......
-000028d0: a0b7 20e4 bdbf e5be 9720 e698 af20 e698  .. ...... ... ..
-000028e0: afe7 9a84 20e9 a696 e585 8820 e8b0 8120  .... ...... ... 
-000028f0: e8b0 81e7 9fa5 20e9 a1ba 20e9 a1ba e79d  ...... ... .....
-00002900: 8020 e4bc bce7 9a84 20e8 99bd 20e8 99bd  . ...... ... ...
-00002910: e784 b620 e899 bde8 afb4 20e8 99bd e588  ... ...... .....
-00002920: 9920 e99a 8f20 e99a 8fe7 9d80 20e6 8980  . ... ...... ...
-00002930: 20e6 8980 e4bb a520 e4bb 9620 e4bb 96e4   ...... ... ....
-00002940: bbac 20e4 bb96 e4ba ba20 e5ae 8320 e5ae  .. ...... ... ..
-00002950: 83e4 bbac 20e5 a5b9 20e5 a5b9 e4bb ac20  .... ... ...... 
-00002960: e580 9820 e580 98e6 8896 20e5 8098 e784  ... ...... .....
-00002970: b620 e580 98e8 8ba5 20e5 8098 e4bd bf20  . ...... ...... 
-00002980: e885 be20 e69b bf20 e980 9ae8 bf87 20e5  ... ... ...... .
-00002990: 908c 20e5 908c e697 b620 e593 8720 e4b8  .. ...... ... ..
-000029a0: 87e4 b880 20e5 be80 20e6 9c9b 20e4 b8ba  .... ... ... ...
-000029b0: 20e4 b8ba e4bd 9520 e4b8 bae4 ba86 20e4   ...... ...... .
-000029c0: b8ba e4bb 80e4 b988 20e4 b8ba e79d 8020  ........ ...... 
-000029d0: e596 8220 e597 a1e5 97a1 20e6 8891 20e6  ... ...... ... .
-000029e0: 8891 e4bb ac20 e591 9c20 e591 9ce5 91bc  ..... ... ......
-000029f0: 20e4 b98c e4b9 8e20 e697 a0e8 aeba 20e6   ...... ...... .
-00002a00: 97a0 e5ae 8120 e6af 8be5 ae81 20e5 98bb  ..... ...... ...
-00002a10: 20e5 9093 20e7 9bb8 e5af b9e8 808c e8a8   ... ...........
-00002a20: 8020 e583 8f20 e590 9120 e590 91e7 9d80  . ... ... ......
-00002a30: 20e5 9898 20e5 9180 20e7 8489 20e6 b2bf   ... ... ... ...
-00002a40: 20e6 b2bf e79d 8020 e8a6 8120 e8a6 81e4   ...... ... ....
-00002a50: b88d 20e8 a681 e4b8 8de7 84b6 20e8 a681  .. ......... ...
-00002a60: e4b8 8de6 98af 20e8 a681 e4b9 8820 e8a6  ...... ...... ..
-00002a70: 81e6 98af 20e4 b99f 20e4 b99f e7bd a220  .... ... ...... 
-00002a80: e4b9 9fe5 a5bd 20e4 b880 20e4 b880 e888  ...... ... .....
-00002a90: ac20 e4b8 80e6 97a6 20e4 b880 e696 b9e9  . ...... .......
-00002aa0: 9da2 20e4 b880 e69d a520 e4b8 80e5 8887  .. ...... ......
-00002ab0: 20e4 b880 e6a0 b720 e4b8 80e5 8899 20e4   ...... ...... .
-00002ac0: be9d 20e4 be9d e785 a720 e79f a320 e4bb  .. ...... ... ..
-00002ad0: a520 e4bb a5e4 bebf 20e4 bba5 e58f 8a20  . ...... ...... 
-00002ae0: e4bb a5e5 858d 20e4 bba5 e887 b320 e4bb  ...... ...... ..
-00002af0: a5e8 87b3 e4ba 8e20 e4bb a5e8 87b4 20e6  ....... ...... .
-00002b00: 8a91 e688 9620 e59b a020 e59b a0e6 ada4  ..... ... ......
-00002b10: 20e5 9ba0 e880 8c20 e59b a0e4 b8ba 20e5   ...... ...... .
-00002b20: 939f 20e7 94a8 20e7 94b1 20e7 94b1 e6ad  .. ... ... .....
-00002b30: a4e5 8faf e8a7 8120 e794 b1e4 ba8e 20e6  ....... ...... .
-00002b40: 9c89 20e6 9c89 e79a 8420 e69c 89e5 85b3  .. ...... ......
-00002b50: 20e6 9c89 e4ba 9b20 e58f 8820 e4ba 8e20   ...... ... ... 
-00002b60: e4ba 8ee6 98af 20e4 ba8e e698 afe4 b98e  ...... .........
-00002b70: 20e4 b88e 20e4 b88e e6ad a4e5 908c e697   ... ...........
-00002b80: b620 e4b8 8ee5 90a6 20e4 b88e e585 b620  . ...... ...... 
-00002b90: e8b6 8ae6 98af 20e4 ba91 e4ba 9120 e593  ...... ...... ..
-00002ba0: 8920 e586 8de8 afb4 20e5 868d e880 8520  . ...... ...... 
-00002bb0: e59c a820 e59c a8e4 b88b 20e5 92b1 20e5  ... ...... ... .
-00002bc0: 92b1 e4bb ac20 e588 9920 e680 8e20 e680  ..... ... ... ..
-00002bd0: 8ee4 b988 20e6 808e e4b9 88e5 8a9e 20e6  .... ......... .
-00002be0: 808e e4b9 88e6 a0b7 20e6 808e e6a0 b720  ........ ...... 
-00002bf0: e592 8b20 e785 a720 e785 a7e7 9d80 20e8  ... ... ...... .
-00002c00: 8085 20e8 bf99 20e8 bf99 e8be b920 e8bf  .. ... ...... ..
-00002c10: 99e5 84bf 20e8 bf99 e4b8 aa20 e8bf 99e4  .... ...... ....
-00002c20: bc9a e584 bf20 e8bf 99e5 b0b1 e698 afe8  ..... ..........
-00002c30: afb4 20e8 bf99 e987 8c20 e8bf 99e4 b988  .. ...... ......
-00002c40: 20e8 bf99 e4b9 88e7 82b9 e584 bf20 e8bf   ............ ..
-00002c50: 99e4 b988 e4ba 9b20 e8bf 99e4 b988 e6a0  ....... ........
-00002c60: b720 e8bf 99e6 97b6 20e8 bf99 e4ba 9b20  . ...... ...... 
-00002c70: e8bf 99e6 a0b7 20e6 ada3 e5a6 8220 e590  ...... ...... ..
-00002c80: b120 e4b9 8b20 e4b9 8be7 b1bb 20e4 b98b  . ... ...... ...
-00002c90: e689 80e4 bba5 20e4 b98b e4b8 8020 e58f  ...... ...... ..
-00002ca0: aae6 98af 20e5 8faa e999 9020 e58f aae8  .... ...... ....
-00002cb0: a681 20e5 8faa e69c 8920 e887 b320 e887  .. ...... ... ..
-00002cc0: b3e4 ba8e 20e8 afb8 e4bd 8d20 e79d 8020  .... ...... ... 
-00002cd0: e79d 80e5 91a2 20e8 87aa 20e8 87aa e4bb  ...... ... .....
-00002ce0: 8e20 e887 aae4 b8aa e584 bf20 e887 aae5  . ......... ....
-00002cf0: 9084 e584 bf20 e887 aae5 b7b1 20e8 87aa  ..... ...... ...
-00002d00: e5ae b620 e887 aae8 baab 20e7 bbbc e4b8  ... ...... .....
-00002d10: 8ae6 8980 e8bf b020 e680 bbe7 9a84 e69d  ....... ........
-00002d20: a5e7 9c8b 20e6 80bb e79a 84e6 9da5 e8af  .... ...........
-00002d30: b420 e680 bbe7 9a84 e8af b4e6 9da5 20e6  . ............ .
-00002d40: 80bb e880 8ce8 a880 e4b9 8b20 e680 bbe4  ........... ....
-00002d50: b98b 20e7 bab5 20e7 bab5 e4bb a420 e7ba  .. ... ...... ..
-00002d60: b5e7 84b6 20e7 bab5 e4bd bf20 e981 b5e7  .... ...... ....
-00002d70: 85a7 20e4 bd9c e4b8 ba20 e585 ae20 e591  .. ...... ... ..
-00002d80: 8320 e591 9720 e592 9a20 e592 a620 e596  . ... ... ... ..
-00002d90: 8f20 e595 9020 e596 94e5 94b7 20e5 97ac  . ... ...... ...
-00002da0: 20e5 97af 20e5 97b3 2222 2220 0d0a 456e   ... ...""" ..En
-00002db0: 5075 6e63 7475 6174 696f 6e3d 2222 2221  Punctuation="""!
-00002dc0: 2223 2425 265c 2728 292a 2b2c 2d2e 2f3a  "#$%&\'()*+,-./:
-00002dd0: 3b3c 3d3e 3f40 5b5c 5c5d 5e5f 607b 7c7d  ;<=>?@[\\]^_`{|}
-00002de0: 7e22 2222 0d0a 0d0a 6465 6620 776f 7264  ~"""....def word
-00002df0: 5f6c 6973 7428 7370 6c69 745f 776f 7264  _list(split_word
-00002e00: 7329 3a0d 0a20 2020 2022 2222 0d0a 0d0a  s):..    """....
-00002e10: 2020 2020 5061 7261 6d65 7465 7273 0d0a      Parameters..
-00002e20: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a      ----------..
-00002e30: 2020 2020 7370 6c69 745f 776f 7264 7320      split_words 
-00002e40: 3a20 5459 5045 0d0a 2020 2020 2020 2020  : TYPE..        
-00002e50: 4445 5343 5249 5054 494f 4e2e 5b27 4927  DESCRIPTION.['I'
-00002e60: 2c27 636f 756c 6427 2c22 6e27 7422 2c27  ,'could',"n't",'
-00002e70: 6265 6c69 6576 6527 2c27 6974 272c 272e  believe','it','.
-00002e80: 272c 2749 272c 2764 6f27 2c22 6e27 7422  ','I','do',"n't"
-00002e90: 2c27 6c69 6b65 272c 2769 7427 2c27 2e27  ,'like','it','.'
-00002ea0: 5d0d 0a0d 0a20 2020 2052 6574 7572 6e73  ]....    Returns
-00002eb0: 0d0a 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20  ..    -------.. 
-00002ec0: 2020 2066 696e 616c 5f64 6963 203a 2054     final_dic : T
-00002ed0: 5950 450d 0a20 2020 2020 2020 2044 4553  YPE..        DES
-00002ee0: 4352 4950 5449 4f4e 2e20 5b28 2749 272c  CRIPTION. [('I',
-00002ef0: 2032 292c 2028 226e 2774 222c 2032 292c   2), ("n't", 2),
-00002f00: 2028 2769 7427 2c20 3229 2c20 2827 2e27   ('it', 2), ('.'
-00002f10: 2c20 3229 2c20 2827 636f 756c 6427 2c20  , 2), ('could', 
-00002f20: 3129 2c20 2827 6265 6c69 6576 6527 2c20  1), ('believe', 
-00002f30: 3129 2c20 2827 646f 272c 2031 292c 2028  1), ('do', 1), (
-00002f40: 276c 696b 6527 2c20 3129 5d0d 0a0d 0a20  'like', 1)].... 
-00002f50: 2020 2022 2222 0d0a 2020 2020 6672 6f6d     """..    from
-00002f60: 2063 6f6c 6c65 6374 696f 6e73 2069 6d70   collections imp
-00002f70: 6f72 7420 436f 756e 7465 720d 0a20 2020  ort Counter..   
-00002f80: 206d 795f 6469 633d 6469 6374 2843 6f75   my_dic=dict(Cou
-00002f90: 6e74 6572 2873 706c 6974 5f77 6f72 6473  nter(split_words
-00002fa0: 2929 0d0a 2020 2020 6669 6e61 6c5f 6469  ))..    final_di
-00002fb0: 633d 736f 7274 6564 286d 795f 6469 632e  c=sorted(my_dic.
-00002fc0: 6974 656d 7328 292c 6b65 793d 6c61 6d62  items(),key=lamb
-00002fd0: 6461 2078 3a78 5b31 5d2c 7265 7665 7273  da x:x[1],revers
-00002fe0: 653d 5472 7565 290d 0a20 2020 2072 6574  e=True)..    ret
-00002ff0: 7572 6e20 6669 6e61 6c5f 6469 6320 2020  urn final_dic   
-00003000: 200d 0a09 0d0a 6465 6620 636c 6561 6e5f   .....def clean_
-00003010: 6c69 7374 286d 6574 6129 3a0d 0a20 2020  list(meta):..   
-00003020: 2022 2222 0d0a 2020 2020 5061 7261 6d65   """..    Parame
-00003030: 7465 7273 0d0a 2020 2020 2d2d 2d2d 2d2d  ters..    ------
-00003040: 2d2d 2d2d 0d0a 2020 2020 6d65 7461 203a  ----..    meta :
-00003050: 2054 5950 450d 0a20 2020 2020 2020 2044   TYPE..        D
-00003060: 4553 4352 4950 5449 4f4e 2e20 6c69 7374  ESCRIPTION. list
-00003070: 2074 7970 6520 2320 5b27 5c6e 5c6e 5c74   type # ['\n\n\t
-00003080: 5c74 5c74 5c74 5c74 272c 27e6 9da5 e6ba  \t\t\t\t','.....
-00003090: 90ef bc9a e696 b0e6 b091 e699 9ae6 8aa5  ................
-000030a0: 272c 275c 7861 305c 7861 305c 7861 305c  ','\xa0\xa0\xa0\
-000030b0: 7861 305c 6e5c 745c 745c 745c 745c 7427  xa0\n\t\t\t\t\t'
-000030c0: 2c27 5c6e 5c6e 5c74 5c74 5c74 5c74 5c74  ,'\n\n\t\t\t\t\t
-000030d0: 5c6e 5c74 5c74 5c74 5c74 5c74 5c74 272c  \n\t\t\t\t\t\t',
-000030e0: 27e8 aeb0 e880 85ef bc9a e999 86e6 a293  '...............
-000030f0: e58d 8e27 5d0d 0a0d 0a20 2020 2052 6574  ...']....    Ret
-00003100: 7572 6e73 0d0a 2020 2020 2d2d 2d2d 2d2d  urns..    ------
-00003110: 2d0d 0a20 2020 2072 6573 756c 7420 3a20  -..    result : 
-00003120: 5459 5045 0d0a 2020 2020 2020 2020 4445  TYPE..        DE
-00003130: 5343 5249 5054 494f 4e2e 0d0a 2020 2020  SCRIPTION...    
-00003140: 2020 2020 7374 7269 6e67 3a0d 0a20 2020      string:..   
-00003150: 2020 2020 2020 2020 20e6 9da5 e6ba 90ef           .......
-00003160: bc9a e696 b0e6 b091 e699 9ae6 8aa5 0d0a  ................
-00003170: 2020 2020 2020 2020 2020 2020 e8ae b0e8              ....
-00003180: 8085 efbc 9ae9 9986 e6a2 93e5 8d8e 0d0a  ................
-00003190: 2020 2020 2020 2020 2020 2020 e4bd 9ce8              ....
-000031a0: 8085 efbc 9ae9 9986 e6a2 93e5 8d8e 0d0a  ................
-000031b0: 2020 2020 2020 2020 2020 2020 e7bc 96e8              ....
-000031c0: be91 efbc 9ae8 a398 e9a2 96e7 90bc 0d0a  ................
-000031d0: 2020 2020 2020 2020 2020 2020 3230 3232              2022
-000031e0: 2d30 372d 3231 2031 373a 3437 0d0a 2020  -07-21 17:47..  
-000031f0: 2020 2222 220d 0a20 2020 2072 6573 756c    """..    resul
-00003200: 743d 225c 6e22 2e6a 6f69 6e28 5b6c 696e  t="\n".join([lin
-00003210: 652e 7374 7269 7028 2920 666f 7220 6c69  e.strip() for li
-00003220: 6e65 2069 6e20 6d65 7461 2069 6620 6c69  ne in meta if li
-00003230: 6e65 2e73 7472 6970 2829 213d 227c 2220  ne.strip()!="|" 
-00003240: 616e 6420 6c65 6e28 6c69 6e65 2e73 7472  and len(line.str
-00003250: 6970 2829 2921 3d30 5d29 0d0a 2020 2020  ip())!=0])..    
-00003260: 7265 7475 726e 2072 6573 756c 740d 0a0d  return result...
-00003270: 0a79 6864 3d5b 224d 6f7a 696c 6c61 2f35  .yhd=["Mozilla/5
-00003280: 2e30 2028 5769 6e64 6f77 7320 4e54 2031  .0 (Windows NT 1
-00003290: 302e 303b 2057 4f57 3634 2920 4170 706c  0.0; WOW64) Appl
-000032a0: 6557 6562 4b69 742f 3533 372e 3336 2028  eWebKit/537.36 (
-000032b0: 4b48 544d 4c2c 206c 696b 6520 4765 636b  KHTML, like Geck
-000032c0: 6f29 2043 6872 6f6d 652f 3738 2e30 2e33  o) Chrome/78.0.3
-000032d0: 3930 342e 3130 3820 5361 6661 7269 2f35  904.108 Safari/5
-000032e0: 3337 2e33 3622 2c27 4d6f 7a69 6c6c 612f  37.36",'Mozilla/
-000032f0: 352e 3020 2857 696e 646f 7773 204e 5420  5.0 (Windows NT 
-00003300: 3130 2e30 3b20 574f 5736 3429 2041 7070  10.0; WOW64) App
-00003310: 6c65 5765 624b 6974 2f35 3337 2e33 3620  leWebKit/537.36 
-00003320: 284b 4854 4d4c 2c20 6c69 6b65 2047 6563  (KHTML, like Gec
-00003330: 6b6f 2920 4368 726f 6d65 2f37 382e 302e  ko) Chrome/78.0.
-00003340: 3339 3034 2e31 3038 2053 6166 6172 692f  3904.108 Safari/
-00003350: 3533 372e 3336 272c 274d 6f7a 696c 6c61  537.36','Mozilla
-00003360: 2f34 2e30 2028 636f 6d70 6174 6962 6c65  /4.0 (compatible
-00003370: 3b20 4d53 4945 2036 2e30 3b20 2920 4f70  ; MSIE 6.0; ) Op
-00003380: 6572 612f 5543 5745 4237 2e30 2e32 2e33  era/UCWEB7.0.2.3
-00003390: 372f 3238 2f39 3939 272c 274d 6f7a 696c  7/28/999','Mozil
-000033a0: 6c61 2f34 2e30 2028 636f 6d70 6174 6962  la/4.0 (compatib
-000033b0: 6c65 3b20 4d53 4945 2037 2e30 3b20 5769  le; MSIE 7.0; Wi
-000033c0: 6e64 6f77 7320 4e54 2035 2e31 2927 2c27  ndows NT 5.1)','
-000033d0: 4d6f 7a69 6c6c 612f 342e 3020 2863 6f6d  Mozilla/4.0 (com
-000033e0: 7061 7469 626c 653b 204d 5349 4520 372e  patible; MSIE 7.
-000033f0: 303b 2057 696e 646f 7773 204e 5420 352e  0; Windows NT 5.
-00003400: 3129 272c 274d 6f7a 696c 6c61 2f34 2e30  1)','Mozilla/4.0
-00003410: 2028 636f 6d70 6174 6962 6c65 3b20 4d53   (compatible; MS
-00003420: 4945 2037 2e30 3b20 5769 6e64 6f77 7320  IE 7.0; Windows 
-00003430: 4e54 2035 2e31 3b20 3336 3053 4529 272c  NT 5.1; 360SE)',
-00003440: 274d 6f7a 696c 6c61 2f34 2e30 2028 636f  'Mozilla/4.0 (co
-00003450: 6d70 6174 6962 6c65 3b20 4d53 4945 2037  mpatible; MSIE 7
-00003460: 2e30 3b20 5769 6e64 6f77 7320 4e54 2035  .0; Windows NT 5
-00003470: 2e31 3b20 4176 616e 7420 4272 6f77 7365  .1; Avant Browse
-00003480: 7229 272c 274d 6f7a 696c 6c61 2f34 2e30  r)','Mozilla/4.0
-00003490: 2028 636f 6d70 6174 6962 6c65 3b20 4d53   (compatible; MS
-000034a0: 4945 2037 2e30 3b20 5769 6e64 6f77 7320  IE 7.0; Windows 
-000034b0: 4e54 2035 2e31 3b20 4d61 7874 686f 6e20  NT 5.1; Maxthon 
-000034c0: 322e 3029 272c 274d 6f7a 696c 6c61 2f34  2.0)','Mozilla/4
-000034d0: 2e30 2028 636f 6d70 6174 6962 6c65 3b20  .0 (compatible; 
-000034e0: 4d53 4945 2037 2e30 3b20 5769 6e64 6f77  MSIE 7.0; Window
-000034f0: 7320 4e54 2035 2e31 3b20 5465 6e63 656e  s NT 5.1; Tencen
-00003500: 7454 7261 7665 6c65 7220 342e 3029 272c  tTraveler 4.0)',
-00003510: 274d 6f7a 696c 6c61 2f34 2e30 2028 636f  'Mozilla/4.0 (co
-00003520: 6d70 6174 6962 6c65 3b20 4d53 4945 2037  mpatible; MSIE 7
-00003530: 2e30 3b20 5769 6e64 6f77 7320 4e54 2035  .0; Windows NT 5
-00003540: 2e31 3b20 5468 6520 576f 726c 6429 272c  .1; The World)',
-00003550: 274d 6f7a 696c 6c61 2f34 2e30 2028 636f  'Mozilla/4.0 (co
-00003560: 6d70 6174 6962 6c65 3b20 4d53 4945 2038  mpatible; MSIE 8
-00003570: 2e30 3b20 5769 6e64 6f77 7320 4e54 2036  .0; Windows NT 6
-00003580: 2e30 3b20 5472 6964 656e 742f 342e 3029  .0; Trident/4.0)
-00003590: 272c 274d 6f7a 696c 6c61 2f35 2e30 2028  ','Mozilla/5.0 (
-000035a0: 426c 6163 6b42 6572 7279 3b20 553b 2042  BlackBerry; U; B
-000035b0: 6c61 636b 4265 7272 7920 3938 3030 3b20  lackBerry 9800; 
-000035c0: 656e 2920 4170 706c 6557 6562 4b69 742f  en) AppleWebKit/
-000035d0: 3533 342e 312b 2028 4b48 544d 4c2c 206c  534.1+ (KHTML, l
-000035e0: 696b 6520 4765 636b 6f29 2056 6572 7369  ike Gecko) Versi
-000035f0: 6f6e 2f36 2e30 2e30 2e33 3337 204d 6f62  on/6.0.0.337 Mob
-00003600: 696c 6520 5361 6661 7269 2f35 3334 2e31  ile Safari/534.1
-00003610: 2b27 2c27 4d6f 7a69 6c6c 612f 352e 3020  +','Mozilla/5.0 
-00003620: 2863 6f6d 7061 7469 626c 653b 204d 5349  (compatible; MSI
-00003630: 4520 392e 303b 2057 696e 646f 7773 204e  E 9.0; Windows N
-00003640: 5420 362e 313b 2054 7269 6465 6e74 2f35  T 6.1; Trident/5
-00003650: 2e30 272c 274d 6f7a 696c 6c61 2f35 2e30  .0','Mozilla/5.0
-00003660: 2028 636f 6d70 6174 6962 6c65 3b20 4d53   (compatible; MS
-00003670: 4945 2039 2e30 3b20 5769 6e64 6f77 7320  IE 9.0; Windows 
-00003680: 5068 6f6e 6520 4f53 2037 2e35 3b20 5472  Phone OS 7.5; Tr
-00003690: 6964 656e 742f 352e 303b 2049 454d 6f62  ident/5.0; IEMob
-000036a0: 696c 652f 392e 303b 2048 5443 3b20 5469  ile/9.0; HTC; Ti
-000036b0: 7461 6e29 272c 274d 6f7a 696c 6c61 2f35  tan)','Mozilla/5
-000036c0: 2e30 2028 6950 6164 3b20 553b 2043 5055  .0 (iPad; U; CPU
-000036d0: 204f 5320 345f 335f 3320 6c69 6b65 204d   OS 4_3_3 like M
-000036e0: 6163 204f 5320 583b 2065 6e2d 7573 2920  ac OS X; en-us) 
-000036f0: 4170 706c 6557 6562 4b69 742f 3533 332e  AppleWebKit/533.
-00003700: 3137 2e39 2028 4b48 544d 4c2c 206c 696b  17.9 (KHTML, lik
-00003710: 6520 4765 636b 6f29 2056 6572 7369 6f6e  e Gecko) Version
-00003720: 2f35 2e30 2e32 204d 6f62 696c 652f 384a  /5.0.2 Mobile/8J
-00003730: 3220 5361 6661 7269 2f36 3533 332e 3138  2 Safari/6533.18
-00003740: 2e35 272c 274d 6f7a 696c 6c61 2f35 2e30  .5','Mozilla/5.0
-00003750: 2028 6950 686f 6e65 3b20 553b 2043 5055   (iPhone; U; CPU
-00003760: 2069 5068 6f6e 6520 4f53 2034 5f33 5f33   iPhone OS 4_3_3
-00003770: 206c 696b 6520 4d61 6320 4f53 2058 3b20   like Mac OS X; 
-00003780: 656e 2d75 7329 2041 7070 6c65 5765 624b  en-us) AppleWebK
-00003790: 6974 2f35 3333 2e31 372e 3920 284b 4854  it/533.17.9 (KHT
-000037a0: 4d4c 2c20 6c69 6b65 2047 6563 6b6f 2920  ML, like Gecko) 
-000037b0: 5665 7273 696f 6e2f 352e 302e 3220 4d6f  Version/5.0.2 Mo
-000037c0: 6269 6c65 2f38 4a32 2053 6166 6172 692f  bile/8J2 Safari/
-000037d0: 3635 3333 2e31 382e 3527 2c27 4d6f 7a69  6533.18.5','Mozi
-000037e0: 6c6c 612f 352e 3020 2869 506f 643b 2055  lla/5.0 (iPod; U
-000037f0: 3b20 4350 5520 6950 686f 6e65 204f 5320  ; CPU iPhone OS 
-00003800: 345f 335f 3320 6c69 6b65 204d 6163 204f  4_3_3 like Mac O
-00003810: 5320 583b 2065 6e2d 7573 2920 4170 706c  S X; en-us) Appl
-00003820: 6557 6562 4b69 742f 3533 332e 3137 2e39  eWebKit/533.17.9
-00003830: 2028 4b48 544d 4c2c 206c 696b 6520 4765   (KHTML, like Ge
-00003840: 636b 6f29 2056 6572 7369 6f6e 2f35 2e30  cko) Version/5.0
-00003850: 2e32 204d 6f62 696c 652f 384a 3220 5361  .2 Mobile/8J2 Sa
-00003860: 6661 7269 2f36 3533 332e 3138 2e35 272c  fari/6533.18.5',
-00003870: 274d 6f7a 696c 6c61 2f35 2e30 2028 4c69  'Mozilla/5.0 (Li
-00003880: 6e75 783b 2055 3b20 416e 6472 6f69 6420  nux; U; Android 
-00003890: 322e 332e 373b 2065 6e2d 7573 3b20 4e65  2.3.7; en-us; Ne
-000038a0: 7875 7320 4f6e 6520 4275 696c 642f 4652  xus One Build/FR
-000038b0: 4639 3129 2041 7070 6c65 5765 624b 6974  F91) AppleWebKit
-000038c0: 2f35 3333 2e31 2028 4b48 544d 4c2c 206c  /533.1 (KHTML, l
-000038d0: 696b 6520 4765 636b 6f29 2056 6572 7369  ike Gecko) Versi
-000038e0: 6f6e 2f34 2e30 204d 6f62 696c 6520 5361  on/4.0 Mobile Sa
-000038f0: 6661 7269 2f35 3333 2e31 272c 274d 6f7a  fari/533.1','Moz
-00003900: 696c 6c61 2f35 2e30 2028 4c69 6e75 783b  illa/5.0 (Linux;
-00003910: 2055 3b20 416e 6472 6f69 6420 332e 303b   U; Android 3.0;
-00003920: 2065 6e2d 7573 3b20 586f 6f6d 2042 7569   en-us; Xoom Bui
-00003930: 6c64 2f48 5249 3339 2920 4170 706c 6557  ld/HRI39) AppleW
-00003940: 6562 4b69 742f 3533 342e 3133 2028 4b48  ebKit/534.13 (KH
-00003950: 544d 4c2c 206c 696b 6520 4765 636b 6f29  TML, like Gecko)
-00003960: 2056 6572 7369 6f6e 2f34 2e30 2053 6166   Version/4.0 Saf
-00003970: 6172 692f 3533 342e 3133 272c 274d 6f7a  ari/534.13','Moz
-00003980: 696c 6c61 2f35 2e30 2028 4d61 6369 6e74  illa/5.0 (Macint
-00003990: 6f73 683b 2049 6e74 656c 204d 6163 204f  osh; Intel Mac O
-000039a0: 5320 5820 3130 2e36 3b20 7276 3a32 2e30  S X 10.6; rv:2.0
-000039b0: 2e31 2920 4765 636b 6f2f 3230 3130 3031  .1) Gecko/201001
-000039c0: 3031 2046 6972 6566 6f78 2f34 2e30 2e31  01 Firefox/4.0.1
-000039d0: 272c 274d 6f7a 696c 6c61 2f35 2e30 2028  ','Mozilla/5.0 (
-000039e0: 5769 6e64 6f77 7320 4e54 2036 2e31 3b20  Windows NT 6.1; 
-000039f0: 7276 3a32 2e30 2e31 2920 4765 636b 6f2f  rv:2.0.1) Gecko/
-00003a00: 3230 3130 3031 3031 2046 6972 6566 6f78  20100101 Firefox
-00003a10: 2f34 2e30 2e31 272c 274d 6f7a 696c 6c61  /4.0.1','Mozilla
-00003a20: 2f35 2e30 2028 5769 6e64 6f77 733b 2055  /5.0 (Windows; U
-00003a30: 3b20 5769 6e64 6f77 7320 4e54 2036 2e31  ; Windows NT 6.1
-00003a40: 3b20 656e 2d75 7329 2041 7070 6c65 5765  ; en-us) AppleWe
-00003a50: 624b 6974 2f35 3334 2e35 3020 284b 4854  bKit/534.50 (KHT
-00003a60: 4d4c 2c20 6c69 6b65 2047 6563 6b6f 2920  ML, like Gecko) 
-00003a70: 5665 7273 696f 6e2f 352e 3120 5361 6661  Version/5.1 Safa
-00003a80: 7269 2f35 3334 2e35 3027 2c27 4d6f 7a69  ri/534.50','Mozi
-00003a90: 6c6c 612f 352e 3020 2857 696e 646f 7773  lla/5.0 (Windows
-00003aa0: 3b20 553b 2057 696e 646f 7773 204e 5420  ; U; Windows NT 
-00003ab0: 362e 313b 2065 6e2d 5553 3b20 7276 3a31  6.1; en-US; rv:1
-00003ac0: 2e39 2e31 2e36 2920 4765 636b 6f2f 3230  .9.1.6) Gecko/20
-00003ad0: 3039 3132 3031 2046 6972 6566 6f78 2f33  091201 Firefox/3
-00003ae0: 2e35 2e36 272c 274e 4f4b 4941 3537 3030  .5.6','NOKIA5700
-00003af0: 2f20 5543 5745 4237 2e30 2e32 2e33 372f  / UCWEB7.0.2.37/
-00003b00: 3238 2f39 3939 272c 274f 7065 6e77 6176  28/999','Openwav
-00003b10: 652f 2055 4357 4542 372e 302e 322e 3337  e/ UCWEB7.0.2.37
-00003b20: 2f32 382f 3939 3927 2c27 4f70 6572 612f  /28/999','Opera/
-00003b30: 392e 3830 2028 416e 6472 6f69 6420 322e  9.80 (Android 2.
-00003b40: 332e 343b 204c 696e 7578 3b20 4f70 6572  3.4; Linux; Oper
-00003b50: 6120 4d6f 6269 2f62 7569 6c64 2d31 3130  a Mobi/build-110
-00003b60: 3731 3830 3934 353b 2055 3b20 656e 2d47  7180945; U; en-G
-00003b70: 4229 2050 7265 7374 6f2f 322e 382e 3134  B) Presto/2.8.14
-00003b80: 3920 5665 7273 696f 6e2f 3131 2e31 3027  9 Version/11.10'
-00003b90: 2c27 4f70 6572 612f 392e 3830 2028 4d61  ,'Opera/9.80 (Ma
-00003ba0: 6369 6e74 6f73 683b 2049 6e74 656c 204d  cintosh; Intel M
-00003bb0: 6163 204f 5320 5820 3130 2e36 2e38 3b20  ac OS X 10.6.8; 
-00003bc0: 553b 2065 6e29 2050 7265 7374 6f2f 322e  U; en) Presto/2.
-00003bd0: 382e 3133 3120 5665 7273 696f 6e2f 3131  8.131 Version/11
-00003be0: 2e31 3127 2c27 4f70 6572 612f 392e 3830  .11','Opera/9.80
-00003bf0: 2028 5769 6e64 6f77 7320 4e54 2036 2e31   (Windows NT 6.1
-00003c00: 3b20 553b 2065 6e29 2050 7265 7374 6f2f  ; U; en) Presto/
-00003c10: 322e 382e 3133 3120 5665 7273 696f 6e2f  2.8.131 Version/
-00003c20: 3131 2e31 3127 2c27 5543 5745 4237 2e30  11.11','UCWEB7.0
-00003c30: 2e32 2e33 372f 3238 2f39 3939 275d 0d0a  .2.37/28/999']..
+00001d10: a6e2 80a6 e280 a6e2 80a6 e280 a6e2 80a6  ................
+00001d20: e280 a6e2 80a6 e280 a6e2 80a6 e280 a6e2  ................
+00001d30: 80a6 e291 a220 efbc baef bcb8 efbc a6ef  ..... ..........
+00001d40: bca9 efbc b4ef bcac 20ef bcbb e291 a2ef  ........ .......
+00001d50: bca6 efbc bd20 e380 8d20 efbc bbe2 91a0  ..... ... ......
+00001d60: efbd 8fef bcbd 20ef bcbd e288 a7e2 80b2  ...... .........
+00001d70: efbc 9def bcbb 2020 e288 aacf 86e2 8888  ......  ........
+00001d80: 20e2 80b2 efbd 9c20 efbd 9bef bc8d 20e2   ...... ...... .
+00001d90: 91a1 efbd 8320 efbd 9d20 efbc bbe2 91a2  ..... ... ......
+00001da0: e291 a0ef bcbd 20ef bcb2 efbc 8eef bcac  ...... .........
+00001db0: efbc 8e20 efbc bbe2 91a0 efbc a5ef bcbd  ... ............
+00001dc0: 20ce a820 efbc 8def bcbb efbc 8aef bcbd   .. ............
+00001dd0: efbc 8d20 e286 9120 2ee6 97a5 2020 efbc  ... ... ....  ..
+00001de0: bbe2 91a1 efbd 84ef bcbd 20ef bcbb e291  .......... .....
+00001df0: a120 efbc bbe2 91a1 e291 a6ef bcbd 20ef  . ............ .
+00001e00: bcbb e291 a1e2 91a1 efbc bd20 efbc bbe2  ........... ....
+00001e10: 91a2 efbd 85ef bcbd 20ef bcbb e291 a0ef  ........ .......
+00001e20: bd89 efbc bd20 efbc bbe2 91a0 efbc a2ef  ..... ..........
+00001e30: bcbd 20ef bcbb e291 a0ef bd88 efbc bd20  .. ............ 
+00001e40: efbc bbe2 91a0 efbd 84ef bcbd 20ef bcbb  ............ ...
+00001e50: e291 a0ef bd87 efbc bd20 efbc bbe2 91a0  ......... ......
+00001e60: e291 a1ef bcbd 20ef bcbb e291 a1ef bd81  ...... .........
+00001e70: efbc bd20 efbd 86ef bcbd 20ef bcbb e291  ... ...... .....
+00001e80: a9ef bcbd 20ef bd81 efbc bd20 efbc bbe2  .... ...... ....
+00001e90: 91a0 efbd 85ef bcbd 20ef bcbb e291 a1ef  ........ .......
+00001ea0: bd88 efbc bd20 efbc bbe2 91a1 e291 a5ef  ..... ..........
+00001eb0: bcbd 20ef bcbb e291 a2ef bd84 efbc bd20  .. ............ 
+00001ec0: efbc bbe2 91a1 e291 a9ef bcbd 20ef bd85  ............ ...
+00001ed0: efbc bd20 e380 8920 e380 9120 e585 83ef  ... ... ... ....
+00001ee0: bc8f e590 a820 efbc bbe2 91a1 e291 a9ef  ..... ..........
+00001ef0: bcbd 20ef bc92 efbc 8eef bc93 efbc 8520  .. ............ 
+00001f00: efbc 95ef bc9a efbc 9020 2020 efbc bbe2  .........   ....
+00001f10: 91a0 efbc bd20 3a3a 20ef bcbb e291 a1ef  ..... :: .......
+00001f20: bcbd 20ef bcbb e291 a2ef bcbd 20ef bcbb  .. ......... ...
+00001f30: e291 a3ef bcbd 20ef bcbb e291 a4ef bcbd  ...... .........
+00001f40: 20ef bcbb e291 a5ef bcbd 20ef bcbb e291   ......... .....
+00001f50: a6ef bcbd 20ef bcbb e291 a7ef bcbd 20ef  .... ......... .
+00001f60: bcbb e291 a8ef bcbd 2020 e280 a6e2 80a6  ........  ......
+00001f70: 20e2 8094 e280 9420 3f20 e380 8120 e380   ...... ? ... ..
+00001f80: 8220 e280 9c20 e280 9d20 e380 8a20 e380  . ... ... ... ..
+00001f90: 8b20 efbc 8120 efbc 8c20 efbc 9a20 efbc  . ... ... ... ..
+00001fa0: 9b20 efbc 9f20 efbc 8e20 2c20 efbc 8e20  . ... ... , ... 
+00001fb0: 2720 3f20 20c2 b720 e280 94e2 8094 e280  ' ?  .. ........
+00001fc0: 9420 e294 80e2 9480 203f 2020 e280 9420  . ...... ?  ... 
+00001fd0: 3c20 3e20 efbc 8820 efbc 8920 e380 9420  < > ... ... ... 
+00001fe0: e380 9520 5b20 5d20 2820 2920 2d20 2b20  ... [ ] ( ) - + 
+00001ff0: efbd 9e20 c397 20ef bc8f 202f 20e2 91a0  ... .. ... / ...
+00002000: 20e2 91a1 20e2 91a2 20e2 91a3 20e2 91a4   ... ... ... ...
+00002010: 20e2 91a5 20e2 91a6 20e2 91a7 20e2 91a8   ... ... ... ...
+00002020: 20e2 91a9 20e2 85a2 20d0 9220 2220 3b20   ... ... .. " ; 
+00002030: 2320 4020 ceb3 20ce bc20 cf86 20cf 86ef  # @ .. .. .. ...
+00002040: bc8e 20c3 9720 20ce 9420 e296 a020 e296  .. ..  .. ... ..
+00002050: b220 7375 6220 6578 7020 2073 7570 2073  . sub exp  sup s
+00002060: 7562 204c 6578 2020 efbc 8320 efbc 8520  ub Lex  ... ... 
+00002070: efbc 8620 efbc 8720 efbc 8b20 efbc 8bce  ... ... ... ....
+00002080: be20 efbc 8bef bc8b 20ef bc8d 20ef bc8d  . ...... ... ...
+00002090: ceb2 20ef bc9c 20ef bc9c c2b1 20ef bc9c  .. ... ..... ...
+000020a0: ce94 20ef bc9c cebb 20ef bc9c cf86 20ef  .. ..... ..... .
+000020b0: bc9c efbc 9c20 3d20 efbc 9d20 efbc 9de2  ..... = ... ....
+000020c0: 9886 20ef bc9d efbc 8d20 efbc 9e20 efbc  .. ...... ... ..
+000020d0: 9ece bb20 efbc bf20 efbd 9ec2 b120 efbd  ... ... ..... ..
+000020e0: 9eef bc8b 20ef bcbb e291 a4ef bd86 efbc  .... ...........
+000020f0: bd20 efbc bbe2 91a4 efbd 84ef bcbd 20ef  . ............ .
+00002100: bcbb e291 a1ef bd89 efbc bd20 e289 8820  ........... ... 
+00002110: 20ef bcbb e291 a1ef bca7 efbc bd20 efbc   ............ ..
+00002120: bbe2 91a0 efbd 86ef bcbd 20ef bcac efbc  .......... .....
+00002130: a920 e388 a720 20ef bcbb efbc 8d20 2e2e  . ...  ...... ..
+00002140: 2e2e 2e2e 20e3 8089 20ef bcbb e291 a2e2  .... ... .......
+00002150: 91a9 efbc bd20 e7ac ace4 ba8c 20e4 b880  ..... ...... ...
+00002160: e795 aa20 e4b8 80e7 9bb4 20e4 b880 e4b8  ... ...... .....
+00002170: aa20 e4b8 80e4 ba9b 20e8 aeb8 e5a4 9a20  . ...... ...... 
+00002180: e7a7 8d20 e69c 89e7 9a84 e698 af20 e4b9  ... ......... ..
+00002190: 9fe5 b0b1 e698 afe8 afb4 20e6 9cab 2323  .......... ...##
+000021a0: e69c ab20 e595 8a20 e998 bf20 e593 8e20  ... ... ... ... 
+000021b0: e593 8ee5 9180 20e5 938e e593 9f20 e594  ...... ...... ..
+000021c0: 8920 e4bf ba20 e4bf bae4 bbac 20e6 8c89  . ... ...... ...
+000021d0: 20e6 8c89 e785 a720 e590 a720 e590 a7e5   ...... ... ....
+000021e0: 9392 20e6 8a8a 20e7 bda2 e4ba 8620 e8a2  .. ... ...... ..
+000021f0: ab20 e69c ac20 e69c ace7 9d80 20e6 af94  . ... ...... ...
+00002200: 20e6 af94 e696 b920 e6af 94e5 a682 20e9   ...... ...... .
+00002210: 8499 e4ba ba20 e5bd bc20 e5bd bce6 ada4  ..... ... ......
+00002220: 20e8 beb9 20e5 88ab 20e5 88ab e79a 8420   ... ... ...... 
+00002230: e588 abe8 afb4 20e5 b9b6 20e5 b9b6 e4b8  ...... ... .....
+00002240: 9420 e4b8 8de6 af94 20e4 b88d e688 9020  . ...... ...... 
+00002250: e4b8 8de5 8d95 20e4 b88d e4bd 8620 e4b8  ...... ...... ..
+00002260: 8de7 8bac 20e4 b88d e7ae a120 e4b8 8de5  .... ...... ....
+00002270: 8589 20e4 b88d e8bf 8720 e4b8 8de4 bb85  .. ...... ......
+00002280: 20e4 b88d e68b 9820 e4b8 8de8 aeba 20e4   ...... ...... .
+00002290: b88d e680 9520 e4b8 8de7 84b6 20e4 b88d  ..... ...... ...
+000022a0: e5a6 8220 e4b8 8de7 89b9 20e4 b88d e683  ... ...... .....
+000022b0: 9f20 e4b8 8de9 97ae 20e4 b88d e58f aa20  . ...... ...... 
+000022c0: e69c 9d20 e69c 9de7 9d80 20e8 b681 20e8  ... ...... ... .
+000022d0: b681 e79d 8020 e4b9 9820 e586 b220 e999  ..... ... ... ..
+000022e0: a420 e999 a4e6 ada4 e4b9 8be5 a496 20e9  . ............ .
+000022f0: 99a4 e99d 9e20 e999 a4e4 ba86 20e6 ada4  ..... ...... ...
+00002300: 20e6 ada4 e997 b420 e6ad a4e5 a496 20e4   ...... ...... .
+00002310: bb8e 20e4 bb8e e880 8c20 e689 9320 e5be  .. ...... ... ..
+00002320: 8520 e4bd 8620 e4bd 86e6 98af 20e5 bd93  . ... ...... ...
+00002330: 20e5 bd93 e79d 8020 e588 b020 e5be 9720   ...... ... ... 
+00002340: e79a 8420 e79a 84e8 af9d 20e7 ad89 20e7  ... ...... ... .
+00002350: ad89 e7ad 8920 e59c b020 e7ac ac20 e58f  ..... ... ... ..
+00002360: aee5 929a 20e5 afb9 20e5 afb9 e4ba 8e20  .... ... ...... 
+00002370: e5a4 9a20 e5a4 9ae5 b091 20e8 808c 20e8  ... ...... ... .
+00002380: 808c e586 b520 e880 8ce4 b894 20e8 808c  ..... ...... ...
+00002390: e698 af20 e880 8ce5 a496 20e8 808c e8a8  ... ...... .....
+000023a0: 8020 e880 8ce5 b7b2 20e5 b094 e590 8e20  . ...... ...... 
+000023b0: e58f 8de8 bf87 e69d a520 e58f 8de8 bf87  ......... ......
+000023c0: e69d a5e8 afb4 20e5 8f8d e4b9 8b20 e99d  ...... ...... ..
+000023d0: 9ee4 bd86 20e9 9d9e e5be 9220 e590 a6e5  .... ...... ....
+000023e0: 8899 20e5 988e 20e5 988e e799 bb20 e8af  .. ... ...... ..
+000023f0: a520 e8b5 b620 e4b8 aa20 e590 8420 e590  . ... ... ... ..
+00002400: 84e4 b8aa 20e5 9084 e4bd 8d20 e590 84e7  .... ...... ....
+00002410: a78d 20e5 9084 e887 aa20 e7bb 9920 e6a0  .. ...... ... ..
+00002420: b9e6 8dae 20e8 b79f 20e6 9585 20e6 9585  .... ... ... ...
+00002430: e6ad a420 e59b bae7 84b6 20e5 85b3 e4ba  ... ...... .....
+00002440: 8e20 e7ae a120 e5bd 9220 e69e 9ce7 84b6  . ... ... ......
+00002450: 20e6 9e9c e79c 9f20 e8bf 8720 e593 8820   ...... ... ... 
+00002460: e593 88e5 9388 20e5 91b5 20e5 928c 20e4  ...... ... ... .
+00002470: bd95 20e4 bd95 e5a4 8420 e4bd 95e5 86b5  .. ...... ......
+00002480: 20e4 bd95 e697 b620 e598 bf20 e593 bc20   ...... ... ... 
+00002490: e593 bce5 94b7 20e5 91bc e593 a720 e4b9  ...... ...... ..
+000024a0: 8e20 e593 9720 e8bf 98e6 98af 20e8 bf98  . ... ...... ...
+000024b0: e69c 8920 e68d a2e5 8fa5 e8af 9de8 afb4  ... ............
+000024c0: 20e6 8da2 e8a8 80e4 b98b 20e6 8896 20e6   ......... ... .
+000024d0: 8896 e698 af20 e688 96e8 8085 20e6 9e81  ..... ...... ...
+000024e0: e4ba 8620 e58f 8a20 e58f 8ae5 85b6 20e5  ... ... ...... .
+000024f0: 8f8a e887 b320 e58d b320 e58d b3e4 bebf  ..... ... ......
+00002500: 20e5 8db3 e688 9620 e58d b3e4 bba4 20e5   ...... ...... .
+00002510: 8db3 e88b a520 e58d b3e4 bdbf 20e5 87a0  ..... ...... ...
+00002520: 20e5 87a0 e697 b620 e5b7 b120 e697 a220   ...... ... ... 
+00002530: e697 a2e7 84b6 20e6 97a2 e698 af20 e7bb  ...... ...... ..
+00002540: a7e8 808c 20e5 8aa0 e4b9 8b20 e581 87e5  .... ...... ....
+00002550: a682 20e5 8187 e88b a520 e581 87e4 bdbf  .. ...... ......
+00002560: 20e9 89b4 e4ba 8e20 e5b0 8620 e8be 8320   ...... ... ... 
+00002570: e8be 83e4 b98b 20e5 8fab 20e6 8ea5 e79d  ...... ... .....
+00002580: 8020 e7bb 93e6 9e9c 20e5 809f 20e7 b4a7  . ...... ... ...
+00002590: e68e a5e7 9d80 20e8 bf9b e880 8c20 e5b0  ...... ...... ..
+000025a0: bd20 e5b0 bde7 aea1 20e7 bb8f 20e7 bb8f  . ...... ... ...
+000025b0: e8bf 8720 e5b0 b120 e5b0 b1e6 98af 20e5  ... ... ...... .
+000025c0: b0b1 e698 afe8 afb4 20e6 8dae 20e5 85b7  ........ ... ...
+000025d0: e4bd 93e5 9cb0 e8af b420 e585 b7e4 bd93  ......... ......
+000025e0: e8af b4e6 9da5 20e5 bc80 e5a7 8b20 e5bc  ...... ...... ..
+000025f0: 80e5 a496 20e9 9da0 20e5 92b3 20e5 8faf  .... ... ... ...
+00002600: 20e5 8faf e8a7 8120 e58f afe6 98af 20e5   ...... ...... .
+00002610: 8faf e4bb a520 e586 b5e4 b894 20e5 95a6  ..... ...... ...
+00002620: 20e6 9da5 20e6 9da5 e79d 8020 e7a6 bb20   ... ...... ... 
+00002630: e4be 8be5 a682 20e5 93a9 20e8 bf9e 20e8  ...... ... ... .
+00002640: bf9e e590 8c20 e4b8 a4e8 8085 20e4 ba86  ..... ...... ...
+00002650: 20e4 b8b4 20e5 8fa6 20e5 8fa6 e5a4 9620   ... ... ...... 
+00002660: e58f a6e4 b880 e696 b9e9 9da2 20e8 aeba  ............ ...
+00002670: 20e5 989b 20e5 9097 20e6 85a2 e8af b420   ... ... ...... 
+00002680: e6bc abe8 afb4 20e5 8692 20e4 b988 20e6  ...... ... ... .
+00002690: af8f 20e6 af8f e5bd 9320 e4bb ac20 e88e  .. ...... ... ..
+000026a0: abe8 8ba5 20e6 9f90 20e6 9f90 e4b8 aa20  .... ... ...... 
+000026b0: e69f 90e4 ba9b 20e6 8bbf 20e5 93aa 20e5  ...... ... ... .
+000026c0: 93aa e8be b920 e593 aae5 84bf 20e5 93aa  ..... ...... ...
+000026d0: e4b8 aa20 e593 aae9 878c 20e5 93aa e5b9  ... ...... .....
+000026e0: b420 e593 aae6 8095 20e5 93aa e5a4 a920  . ...... ...... 
+000026f0: e593 aae4 ba9b 20e5 93aa e6a0 b720 e982  ...... ...... ..
+00002700: a320 e982 a3e8 beb9 20e9 82a3 e584 bf20  . ...... ...... 
+00002710: e982 a3e4 b8aa 20e9 82a3 e4bc 9ae5 84bf  ...... .........
+00002720: 20e9 82a3 e987 8c20 e982 a3e4 b988 20e9   ...... ...... .
+00002730: 82a3 e4b9 88e4 ba9b 20e9 82a3 e4b9 88e6  ........ .......
+00002740: a0b7 20e9 82a3 e697 b620 e982 a3e4 ba9b  .. ...... ......
+00002750: 20e9 82a3 e6a0 b720 e4b9 8320 e4b9 83e8   ...... ... ....
+00002760: 87b3 20e5 91a2 20e8 83bd 20e4 bda0 20e4  .. ... ... ... .
+00002770: bda0 e4bb ac20 e682 a820 e5ae 8120 e5ae  ..... ... ... ..
+00002780: 81e5 8faf 20e5 ae81 e882 af20 e5ae 81e6  .... ...... ....
+00002790: 84bf 20e5 93a6 20e5 9195 20e5 95aa e8be  .. ... ... .....
+000027a0: be20 e697 81e4 baba 20e5 91b8 20e5 87ad  . ...... ... ...
+000027b0: 20e5 87ad e580 9f20 e585 b620 e585 b6e6   ...... ... ....
+000027c0: aca1 20e5 85b6 e4ba 8c20 e585 b6e4 bb96  .. ...... ......
+000027d0: 20e5 85b6 e5ae 8320 e585 b6e4 b880 20e5   ...... ...... .
+000027e0: 85b6 e4bd 9920 e585 b6e4 b8ad 20e8 b5b7  ..... ...... ...
+000027f0: 20e8 b5b7 e8a7 8120 e8b5 b7e8 a781 20e5   ...... ...... .
+00002800: b282 e4bd 8620 e681 b0e6 81b0 e79b b8e5  ..... ..........
+00002810: 8f8d 20e5 898d e590 8e20 e589 8de8 8085  .. ...... ......
+00002820: 20e4 b894 20e7 84b6 e880 8c20 e784 b6e5   ... ...... ....
+00002830: 908e 20e7 84b6 e588 9920 e8ae a920 e4ba  .. ...... ... ..
+00002840: bae5 aeb6 20e4 bbbb 20e4 bbbb e4bd 9520  .... ... ...... 
+00002850: e4bb bbe5 87ad 20e5 a682 20e5 a682 e6ad  ...... ... .....
+00002860: a420 e5a6 82e6 9e9c 20e5 a682 e4bd 9520  . ...... ...... 
+00002870: e5a6 82e5 85b6 20e5 a682 e88b a520 e5a6  ...... ...... ..
+00002880: 82e4 b88a e689 80e8 bfb0 20e8 8ba5 20e8  .......... ... .
+00002890: 8ba5 e99d 9e20 e88b a5e6 98af 20e5 95a5  ..... ...... ...
+000028a0: 20e4 b88a e4b8 8b20 e5b0 9ae4 b894 20e8   ...... ...... .
+000028b0: aebe e88b a520 e8ae bee4 bdbf 20e7 949a  ..... ...... ...
+000028c0: e880 8c20 e794 9ae4 b988 20e7 949a e887  ... ...... .....
+000028d0: b320 e79c 81e5 be97 20e6 97b6 e580 9920  . ...... ...... 
+000028e0: e4bb 80e4 b988 20e4 bb80 e4b9 88e6 a0b7  ...... .........
+000028f0: 20e4 bdbf e5be 9720 e698 af20 e698 afe7   ...... ... ....
+00002900: 9a84 20e9 a696 e585 8820 e8b0 8120 e8b0  .. ...... ... ..
+00002910: 81e7 9fa5 20e9 a1ba 20e9 a1ba e79d 8020  .... ... ...... 
+00002920: e4bc bce7 9a84 20e8 99bd 20e8 99bd e784  ...... ... .....
+00002930: b620 e899 bde8 afb4 20e8 99bd e588 9920  . ...... ...... 
+00002940: e99a 8f20 e99a 8fe7 9d80 20e6 8980 20e6  ... ...... ... .
+00002950: 8980 e4bb a520 e4bb 9620 e4bb 96e4 bbac  ..... ... ......
+00002960: 20e4 bb96 e4ba ba20 e5ae 8320 e5ae 83e4   ...... ... ....
+00002970: bbac 20e5 a5b9 20e5 a5b9 e4bb ac20 e580  .. ... ...... ..
+00002980: 9820 e580 98e6 8896 20e5 8098 e784 b620  . ...... ...... 
+00002990: e580 98e8 8ba5 20e5 8098 e4bd bf20 e885  ...... ...... ..
+000029a0: be20 e69b bf20 e980 9ae8 bf87 20e5 908c  . ... ...... ...
+000029b0: 20e5 908c e697 b620 e593 8720 e4b8 87e4   ...... ... ....
+000029c0: b880 20e5 be80 20e6 9c9b 20e4 b8ba 20e4  .. ... ... ... .
+000029d0: b8ba e4bd 9520 e4b8 bae4 ba86 20e4 b8ba  ..... ...... ...
+000029e0: e4bb 80e4 b988 20e4 b8ba e79d 8020 e596  ...... ...... ..
+000029f0: 8220 e597 a1e5 97a1 20e6 8891 20e6 8891  . ...... ... ...
+00002a00: e4bb ac20 e591 9c20 e591 9ce5 91bc 20e4  ... ... ...... .
+00002a10: b98c e4b9 8e20 e697 a0e8 aeba 20e6 97a0  ..... ...... ...
+00002a20: e5ae 8120 e6af 8be5 ae81 20e5 98bb 20e5  ... ...... ... .
+00002a30: 9093 20e7 9bb8 e5af b9e8 808c e8a8 8020  .. ............ 
+00002a40: e583 8f20 e590 9120 e590 91e7 9d80 20e5  ... ... ...... .
+00002a50: 9898 20e5 9180 20e7 8489 20e6 b2bf 20e6  .. ... ... ... .
+00002a60: b2bf e79d 8020 e8a6 8120 e8a6 81e4 b88d  ..... ... ......
+00002a70: 20e8 a681 e4b8 8de7 84b6 20e8 a681 e4b8   ......... .....
+00002a80: 8de6 98af 20e8 a681 e4b9 8820 e8a6 81e6  .... ...... ....
+00002a90: 98af 20e4 b99f 20e4 b99f e7bd a220 e4b9  .. ... ...... ..
+00002aa0: 9fe5 a5bd 20e4 b880 20e4 b880 e888 ac20  .... ... ...... 
+00002ab0: e4b8 80e6 97a6 20e4 b880 e696 b9e9 9da2  ...... .........
+00002ac0: 20e4 b880 e69d a520 e4b8 80e5 8887 20e4   ...... ...... .
+00002ad0: b880 e6a0 b720 e4b8 80e5 8899 20e4 be9d  ..... ...... ...
+00002ae0: 20e4 be9d e785 a720 e79f a320 e4bb a520   ...... ... ... 
+00002af0: e4bb a5e4 bebf 20e4 bba5 e58f 8a20 e4bb  ...... ...... ..
+00002b00: a5e5 858d 20e4 bba5 e887 b320 e4bb a5e8  .... ...... ....
+00002b10: 87b3 e4ba 8e20 e4bb a5e8 87b4 20e6 8a91  ..... ...... ...
+00002b20: e688 9620 e59b a020 e59b a0e6 ada4 20e5  ... ... ...... .
+00002b30: 9ba0 e880 8c20 e59b a0e4 b8ba 20e5 939f  ..... ...... ...
+00002b40: 20e7 94a8 20e7 94b1 20e7 94b1 e6ad a4e5   ... ... .......
+00002b50: 8faf e8a7 8120 e794 b1e4 ba8e 20e6 9c89  ..... ...... ...
+00002b60: 20e6 9c89 e79a 8420 e69c 89e5 85b3 20e6   ...... ...... .
+00002b70: 9c89 e4ba 9b20 e58f 8820 e4ba 8e20 e4ba  ..... ... ... ..
+00002b80: 8ee6 98af 20e4 ba8e e698 afe4 b98e 20e4  .... ......... .
+00002b90: b88e 20e4 b88e e6ad a4e5 908c e697 b620  .. ............ 
+00002ba0: e4b8 8ee5 90a6 20e4 b88e e585 b620 e8b6  ...... ...... ..
+00002bb0: 8ae6 98af 20e4 ba91 e4ba 9120 e593 8920  .... ...... ... 
+00002bc0: e586 8de8 afb4 20e5 868d e880 8520 e59c  ...... ...... ..
+00002bd0: a820 e59c a8e4 b88b 20e5 92b1 20e5 92b1  . ...... ... ...
+00002be0: e4bb ac20 e588 9920 e680 8e20 e680 8ee4  ... ... ... ....
+00002bf0: b988 20e6 808e e4b9 88e5 8a9e 20e6 808e  .. ......... ...
+00002c00: e4b9 88e6 a0b7 20e6 808e e6a0 b720 e592  ...... ...... ..
+00002c10: 8b20 e785 a720 e785 a7e7 9d80 20e8 8085  . ... ...... ...
+00002c20: 20e8 bf99 20e8 bf99 e8be b920 e8bf 99e5   ... ...... ....
+00002c30: 84bf 20e8 bf99 e4b8 aa20 e8bf 99e4 bc9a  .. ...... ......
+00002c40: e584 bf20 e8bf 99e5 b0b1 e698 afe8 afb4  ... ............
+00002c50: 20e8 bf99 e987 8c20 e8bf 99e4 b988 20e8   ...... ...... .
+00002c60: bf99 e4b9 88e7 82b9 e584 bf20 e8bf 99e4  ........... ....
+00002c70: b988 e4ba 9b20 e8bf 99e4 b988 e6a0 b720  ..... ......... 
+00002c80: e8bf 99e6 97b6 20e8 bf99 e4ba 9b20 e8bf  ...... ...... ..
+00002c90: 99e6 a0b7 20e6 ada3 e5a6 8220 e590 b120  .... ...... ... 
+00002ca0: e4b9 8b20 e4b9 8be7 b1bb 20e4 b98b e689  ... ...... .....
+00002cb0: 80e4 bba5 20e4 b98b e4b8 8020 e58f aae6  .... ...... ....
+00002cc0: 98af 20e5 8faa e999 9020 e58f aae8 a681  .. ...... ......
+00002cd0: 20e5 8faa e69c 8920 e887 b320 e887 b3e4   ...... ... ....
+00002ce0: ba8e 20e8 afb8 e4bd 8d20 e79d 8020 e79d  .. ...... ... ..
+00002cf0: 80e5 91a2 20e8 87aa 20e8 87aa e4bb 8e20  .... ... ...... 
+00002d00: e887 aae4 b8aa e584 bf20 e887 aae5 9084  ......... ......
+00002d10: e584 bf20 e887 aae5 b7b1 20e8 87aa e5ae  ... ...... .....
+00002d20: b620 e887 aae8 baab 20e7 bbbc e4b8 8ae6  . ...... .......
+00002d30: 8980 e8bf b020 e680 bbe7 9a84 e69d a5e7  ..... ..........
+00002d40: 9c8b 20e6 80bb e79a 84e6 9da5 e8af b420  .. ............ 
+00002d50: e680 bbe7 9a84 e8af b4e6 9da5 20e6 80bb  ............ ...
+00002d60: e880 8ce8 a880 e4b9 8b20 e680 bbe4 b98b  ......... ......
+00002d70: 20e7 bab5 20e7 bab5 e4bb a420 e7ba b5e7   ... ...... ....
+00002d80: 84b6 20e7 bab5 e4bd bf20 e981 b5e7 85a7  .. ...... ......
+00002d90: 20e4 bd9c e4b8 ba20 e585 ae20 e591 8320   ...... ... ... 
+00002da0: e591 9720 e592 9a20 e592 a620 e596 8f20  ... ... ... ... 
+00002db0: e595 9020 e596 94e5 94b7 20e5 97ac 20e5  ... ...... ... .
+00002dc0: 97af 20e5 97b3 2222 2220 0d0a 456e 5075  .. ...""" ..EnPu
+00002dd0: 6e63 7475 6174 696f 6e3d 2222 2221 2223  nctuation="""!"#
+00002de0: 2425 265c 2728 292a 2b2c 2d2e 2f3a 3b3c  $%&\'()*+,-./:;<
+00002df0: 3d3e 3f40 5b5c 5c5d 5e5f 607b 7c7d 7e22  =>?@[\\]^_`{|}~"
+00002e00: 2222 0d0a 0d0a 6465 6620 776f 7264 5f6c  ""....def word_l
+00002e10: 6973 7428 7370 6c69 745f 776f 7264 7329  ist(split_words)
+00002e20: 3a0d 0a20 2020 2022 2222 0d0a 2020 2020  :..    """..    
+00002e30: 5061 7261 6d65 7465 7273 0d0a 2020 2020  Parameters..    
+00002e40: 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020  ----------..    
+00002e50: 7370 6c69 745f 776f 7264 7320 3a20 5459  split_words : TY
+00002e60: 5045 206c 6973 7420 6f66 2073 7472 696e  PE list of strin
+00002e70: 6773 0d0a 2020 2020 2020 2020 4445 5343  gs..        DESC
+00002e80: 5249 5054 494f 4e2e 0d0a 2020 2020 2020  RIPTION...      
+00002e90: 2020 2020 2020 5b27 4927 2c27 636f 756c        ['I','coul
+00002ea0: 6427 2c22 6e27 7422 2c27 6265 6c69 6576  d',"n't",'believ
+00002eb0: 6527 2c27 6974 272c 272e 272c 2749 272c  e','it','.','I',
+00002ec0: 2764 6f27 2c22 6e27 7422 2c27 6c69 6b65  'do',"n't",'like
+00002ed0: 272c 2769 7427 2c27 2e27 5d0d 0a0d 0a20  ','it','.'].... 
+00002ee0: 2020 2052 6574 7572 6e73 0d0a 2020 2020     Returns..    
+00002ef0: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2066 696e  -------..    fin
+00002f00: 616c 5f64 6963 203a 2054 5950 4520 6c69  al_dic : TYPE li
+00002f10: 7374 206f 6620 7475 706c 6573 0d0a 2020  st of tuples..  
+00002f20: 2020 2020 2020 4445 5343 5249 5054 494f        DESCRIPTIO
+00002f30: 4e2e 200d 0a20 2020 2020 2020 2020 2020  N. ..           
+00002f40: 205b 2827 4927 2c20 3229 2c20 2822 6e27   [('I', 2), ("n'
+00002f50: 7422 2c20 3229 2c20 2827 6974 272c 2032  t", 2), ('it', 2
+00002f60: 292c 2028 272e 272c 2032 292c 2028 2763  ), ('.', 2), ('c
+00002f70: 6f75 6c64 272c 2031 292c 2028 2762 656c  ould', 1), ('bel
+00002f80: 6965 7665 272c 2031 292c 2028 2764 6f27  ieve', 1), ('do'
+00002f90: 2c20 3129 2c20 2827 6c69 6b65 272c 2031  , 1), ('like', 1
+00002fa0: 295d 0d0a 2020 2020 2222 220d 0a20 2020  )]..    """..   
+00002fb0: 2066 726f 6d20 636f 6c6c 6563 7469 6f6e   from collection
+00002fc0: 7320 696d 706f 7274 2043 6f75 6e74 6572  s import Counter
+00002fd0: 0d0a 2020 2020 6d79 5f64 6963 3d64 6963  ..    my_dic=dic
+00002fe0: 7428 436f 756e 7465 7228 7370 6c69 745f  t(Counter(split_
+00002ff0: 776f 7264 7329 290d 0a20 2020 2066 696e  words))..    fin
+00003000: 616c 5f64 6963 3d73 6f72 7465 6428 6d79  al_dic=sorted(my
+00003010: 5f64 6963 2e69 7465 6d73 2829 2c6b 6579  _dic.items(),key
+00003020: 3d6c 616d 6264 6120 783a 785b 315d 2c72  =lambda x:x[1],r
+00003030: 6576 6572 7365 3d54 7275 6529 0d0a 2020  everse=True)..  
+00003040: 2020 7265 7475 726e 2066 696e 616c 5f64    return final_d
+00003050: 6963 2020 2020 0d0a 0d0a 6465 6620 6261  ic    ....def ba
+00003060: 7463 685f 776f 7264 5f6c 6973 7428 696e  tch_word_list(in
+00003070: 7075 745f 726f 6f74 293a 0d0a 2020 2020  put_root):..    
+00003080: 2727 270d 0a20 2020 2050 6172 616d 6574  '''..    Paramet
+00003090: 6572 730d 0a20 2020 202d 2d2d 2d2d 2d2d  ers..    -------
+000030a0: 2d2d 2d0d 0a20 2020 2069 6e70 7574 5f72  ---..    input_r
+000030b0: 6f6f 7420 3a20 5459 5045 2073 7472 696e  oot : TYPE strin
+000030c0: 670d 0a20 2020 2020 2020 2044 4553 4352  g..        DESCR
+000030d0: 4950 5449 4f4e 2e0d 0a20 2020 2020 2020  IPTION...       
+000030e0: 2020 2020 2049 7427 7320 6120 666f 6c64       It's a fold
+000030f0: 6572 2070 6174 6820 6c69 6b65 2044 3a5c  er path like D:\
+00003100: 7365 675f 6f6e 6c79 200d 0a20 2020 2020  seg_only ..     
+00003110: 2020 2020 2020 204e 6f74 6564 2074 6861         Noted tha
+00003120: 7420 616c 6c20 7465 7874 2066 696c 6573  t all text files
+00003130: 2069 6e20 7468 6520 666f 6c64 6572 2073   in the folder s
+00003140: 686f 756c 6420 6265 2074 6f6b 656e 697a  hould be tokeniz
+00003150: 6564 2074 6578 7473 2e0d 0a20 2020 2020  ed texts...     
+00003160: 2020 2020 2020 2046 6f72 2065 7861 6d70         For examp
+00003170: 6c65 2c20 7468 6520 7465 7874 206f 6620  le, the text of 
+00003180: 443a 5c73 6567 5f6f 6e6c 795c 312e 7478  D:\seg_only\1.tx
+00003190: 7420 7368 6f75 6c64 2062 6520 6c69 6b65  t should be like
+000031a0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000031b0: 2020 2050 6773 4669 6c65 2069 7320 5079     PgsFile is Py
+000031c0: 7468 6f6e 206c 6962 7261 7279 2074 6f20  thon library to 
+000031d0: 6661 6369 6c69 7461 7465 2050 7974 686f  facilitate Pytho
+000031e0: 6e20 6265 6769 6e6e 6572 7320 2c20 0d0a  n beginners , ..
+000031f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003200: 6573 7065 6369 616c 6c79 2069 6e73 7472  especially instr
+00003210: 7563 746f 7273 2061 6e64 2073 7475 6465  uctors and stude
+00003220: 6e74 7320 6f66 2066 6f72 6569 676e 206c  nts of foreign l
+00003230: 616e 6775 6167 6573 2061 6e64 206c 6974  anguages and lit
+00003240: 6572 6174 7572 652c 200d 0a20 2020 2020  erature, ..     
+00003250: 2020 2020 2020 2020 2020 2066 6f72 2074             for t
+00003260: 6865 2063 6f6e 7665 6e69 656e 6365 206f  he convenience o
+00003270: 6620 6561 7369 6c79 206f 7065 7261 7469  f easily operati
+00003280: 6e67 2074 7874 202c 200d 0a20 2020 2020  ng txt , ..     
+00003290: 2020 2020 2020 2020 2020 2078 6c73 7820             xlsx 
+000032a0: 616e 6420 6a73 6f6e 2066 696c 6573 2061  and json files a
+000032b0: 7320 7765 6c6c 2061 7320 6d61 6b69 6e67  s well as making
+000032c0: 2077 6f72 6420 6c69 7374 202e 2020 2020   word list .    
+000032d0: 2020 2020 200d 0a0d 0a20 2020 2052 6574       ....    Ret
+000032e0: 7572 6e73 0d0a 2020 2020 2d2d 2d2d 2d2d  urns..    ------
+000032f0: 2d0d 0a20 2020 2073 6f72 7465 645f 776f  -..    sorted_wo
+00003300: 7264 7320 3a20 5459 5045 206c 6973 7420  rds : TYPE list 
+00003310: 6d61 6465 206f 6620 7475 706c 6573 2e0d  made of tuples..
+00003320: 0a20 2020 2020 2020 2044 4553 4352 4950  .        DESCRIP
+00003330: 5449 4f4e 2e20 0d0a 2020 2020 2020 2020  TION. ..        
+00003340: 2020 2020 4361 7074 696f 6e3a 205b 2877      Caption: [(w
+00003350: 6f72 642c 205b 776f 7264 5f66 7265 712c  ord, [word_freq,
+00003360: 2064 6f63 756d 656e 745f 6672 6571 5d29   document_freq])
+00003370: 5d0d 0a20 2020 2020 2020 2020 2020 205b  ]..            [
+00003380: 2827 7468 6527 2c20 5b35 3433 2c20 3135  ('the', [543, 15
+00003390: 5d29 2c0d 0a20 2020 2020 2020 2020 2020  ]),..           
+000033a0: 2028 2761 6e64 272c 205b 3333 332c 2031   ('and', [333, 1
+000033b0: 355d 292c 0d0a 2020 2020 2020 2020 2020  5]),..          
+000033c0: 2020 2827 666f 7227 2c20 5b39 382c 2031    ('for', [98, 1
+000033d0: 335d 292c 0d0a 2020 2020 2020 2020 2020  3]),..          
+000033e0: 2020 2827 5079 7468 6f6e 272c 205b 3430    ('Python', [40
+000033f0: 2c20 395d 292c 0d0a 2020 2020 2020 2020  , 9]),..        
+00003400: 2020 2020 2827 456e 676c 6973 6827 2c20      ('English', 
+00003410: 5b32 312c 2032 5d29 2c0d 0a20 2020 2020  [21, 2]),..     
+00003420: 2020 2020 2020 2028 2750 6773 4669 6c65         ('PgsFile
+00003430: 272c 205b 3132 2c20 325d 292c 0d0a 2020  ', [12, 2]),..  
+00003440: 2020 2020 2020 2020 2020 2827 6265 6769            ('begi
+00003450: 6e6e 6572 7327 2c20 5b32 2c20 325d 292c  nners', [2, 2]),
+00003460: 0d0a 2020 2020 2020 2020 2020 2020 2827  ..            ('
+00003470: 6c69 7465 7261 7475 7265 272c 205b 312c  literature', [1,
+00003480: 2031 5d29 2c5d 0d0a 2020 2020 2727 270d   1]),]..    '''.
+00003490: 0a20 2020 2066 726f 6d20 5067 7346 696c  .    from PgsFil
+000034a0: 6520 696d 706f 7274 2067 6574 5f64 6174  e import get_dat
+000034b0: 615f 7465 7874 2061 7320 6774 2c20 4669  a_text as gt, Fi
+000034c0: 6c65 5061 7468 2061 7320 6670 2c20 4269  lePath as fp, Bi
+000034d0: 6750 756e 6374 7561 7469 6f6e 2061 7320  gPunctuation as 
+000034e0: 6270 0d0a 2020 2020 2320 696e 7075 745f  bp..    # input_
+000034f0: 726f 6f74 3d72 2244 3a5c 3034 375f 5363  root=r"D:\047_Sc
+00003500: 7261 7069 6e67 5c73 6567 5f6f 6e6c 7922  raping\seg_only"
+00003510: 0d0a 2020 2020 6669 6c65 5f6e 616d 6573  ..    file_names
+00003520: 3d66 7028 696e 7075 745f 726f 6f74 290d  =fp(input_root).
+00003530: 0a20 2020 200d 0a20 2020 2066 726f 6d20  .    ..    from 
+00003540: 636f 6c6c 6563 7469 6f6e 7320 696d 706f  collections impo
+00003550: 7274 2064 6566 6175 6c74 6469 6374 0d0a  rt defaultdict..
+00003560: 2020 2020 776f 7264 5f63 6f75 6e74 7320      word_counts 
+00003570: 3d20 6465 6661 756c 7464 6963 7428 6c61  = defaultdict(la
+00003580: 6d62 6461 3a20 5b30 2c20 305d 290d 0a20  mbda: [0, 0]).. 
+00003590: 2020 200d 0a20 2020 2066 6f72 2066 696c     ..    for fil
+000035a0: 655f 6e61 6d65 2069 6e20 6669 6c65 5f6e  e_name in file_n
+000035b0: 616d 6573 3a0d 0a20 2020 2020 2020 2077  ames:..        w
+000035c0: 6f72 6473 203d 205b 7720 666f 7220 7720  ords = [w for w 
+000035d0: 696e 2067 7428 6669 6c65 5f6e 616d 6529  in gt(file_name)
+000035e0: 2e73 706c 6974 2829 2069 6620 7720 6e6f  .split() if w no
+000035f0: 7420 696e 2062 705d 0d0a 2020 2020 2020  t in bp]..      
+00003600: 2020 666f 7220 776f 7264 2069 6e20 7365    for word in se
+00003610: 7428 776f 7264 7329 3a0d 0a20 2020 2020  t(words):..     
+00003620: 2020 2020 2020 2077 6f72 645f 636f 756e         word_coun
+00003630: 7473 5b77 6f72 645d 5b30 5d20 2b3d 2077  ts[word][0] += w
+00003640: 6f72 6473 2e63 6f75 6e74 2877 6f72 6429  ords.count(word)
+00003650: 0d0a 2020 2020 2020 2020 2020 2020 776f  ..            wo
+00003660: 7264 5f63 6f75 6e74 735b 776f 7264 5d5b  rd_counts[word][
+00003670: 315d 202b 3d20 310d 0a20 2020 2073 6f72  1] += 1..    sor
+00003680: 7465 645f 776f 7264 7320 3d20 736f 7274  ted_words = sort
+00003690: 6564 2877 6f72 645f 636f 756e 7473 2e69  ed(word_counts.i
+000036a0: 7465 6d73 2829 2c20 6b65 793d 6c61 6d62  tems(), key=lamb
+000036b0: 6461 2078 3a20 785b 315d 2c20 7265 7665  da x: x[1], reve
+000036c0: 7273 653d 5472 7565 290d 0a20 2020 2072  rse=True)..    r
+000036d0: 6574 7572 6e20 736f 7274 6564 5f77 6f72  eturn sorted_wor
+000036e0: 6473 200d 0a0d 0a09 0d0a 6465 6620 636c  ds .......def cl
+000036f0: 6561 6e5f 6c69 7374 286d 6574 6129 3a0d  ean_list(meta):.
+00003700: 0a20 2020 2022 2222 0d0a 2020 2020 5061  .    """..    Pa
+00003710: 7261 6d65 7465 7273 0d0a 2020 2020 2d2d  rameters..    --
+00003720: 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020 6d65  --------..    me
+00003730: 7461 203a 2054 5950 4520 6c69 7374 0d0a  ta : TYPE list..
+00003740: 2020 2020 2020 2020 4445 5343 5249 5054          DESCRIPT
+00003750: 494f 4e2e 2023 205b 275c 6e5c 6e5c 745c  ION. # ['\n\n\t\
+00003760: 745c 745c 745c 7427 2c27 e69d a5e6 ba90  t\t\t\t','......
+00003770: efbc 9ae6 96b0 e6b0 91e6 999a e68a a527  ...............'
+00003780: 2c27 5c78 6130 5c78 6130 5c78 6130 5c78  ,'\xa0\xa0\xa0\x
+00003790: 6130 5c6e 5c74 5c74 5c74 5c74 5c74 272c  a0\n\t\t\t\t\t',
+000037a0: 275c 6e5c 6e5c 745c 745c 745c 745c 745c  '\n\n\t\t\t\t\t\
+000037b0: 6e5c 745c 745c 745c 745c 745c 7427 2c27  n\t\t\t\t\t\t','
+000037c0: e8ae b0e8 8085 efbc 9ae9 9986 e6a2 93e5  ................
+000037d0: 8d8e 275d 0d0a 0d0a 2020 2020 5265 7475  ..']....    Retu
+000037e0: 726e 730d 0a20 2020 202d 2d2d 2d2d 2d2d  rns..    -------
+000037f0: 0d0a 2020 2020 7265 7375 6c74 203a 2054  ..    result : T
+00003800: 5950 4520 7374 7269 6e67 0d0a 2020 2020  YPE string..    
+00003810: 2020 2020 4445 5343 5249 5054 494f 4e2e      DESCRIPTION.
+00003820: 0d0a 2020 2020 2020 2020 2020 2020 e69d  ..            ..
+00003830: a5e6 ba90 efbc 9ae6 96b0 e6b0 91e6 999a  ................
+00003840: e68a a50d 0a20 2020 2020 2020 2020 2020  .....           
+00003850: 20e8 aeb0 e880 85ef bc9a e999 86e6 a293   ...............
+00003860: e58d 8e0d 0a20 2020 2020 2020 2020 2020  .....           
+00003870: 20e4 bd9c e880 85ef bc9a e999 86e6 a293   ...............
+00003880: e58d 8e0d 0a20 2020 2020 2020 2020 2020  .....           
+00003890: 20e7 bc96 e8be 91ef bc9a e8a3 98e9 a296   ...............
+000038a0: e790 bc0d 0a20 2020 2020 2020 2020 2020  .....           
+000038b0: 2032 3032 322d 3037 2d32 3120 3137 3a34   2022-07-21 17:4
+000038c0: 370d 0a20 2020 2022 2222 0d0a 2020 2020  7..    """..    
+000038d0: 7265 7375 6c74 3d22 5c6e 222e 6a6f 696e  result="\n".join
+000038e0: 285b 6c69 6e65 2e73 7472 6970 2829 2066  ([line.strip() f
+000038f0: 6f72 206c 696e 6520 696e 206d 6574 6120  or line in meta 
+00003900: 6966 206c 696e 652e 7374 7269 7028 2921  if line.strip()!
+00003910: 3d22 7c22 2061 6e64 206c 656e 286c 696e  ="|" and len(lin
+00003920: 652e 7374 7269 7028 2929 213d 305d 290d  e.strip())!=0]).
+00003930: 0a20 2020 2072 6574 7572 6e20 7265 7375  .    return resu
+00003940: 6c74 0d0a 0d0a 7968 643d 5b22 4d6f 7a69  lt....yhd=["Mozi
+00003950: 6c6c 612f 352e 3020 2857 696e 646f 7773  lla/5.0 (Windows
+00003960: 204e 5420 3130 2e30 3b20 574f 5736 3429   NT 10.0; WOW64)
+00003970: 2041 7070 6c65 5765 624b 6974 2f35 3337   AppleWebKit/537
+00003980: 2e33 3620 284b 4854 4d4c 2c20 6c69 6b65  .36 (KHTML, like
+00003990: 2047 6563 6b6f 2920 4368 726f 6d65 2f37   Gecko) Chrome/7
+000039a0: 382e 302e 3339 3034 2e31 3038 2053 6166  8.0.3904.108 Saf
+000039b0: 6172 692f 3533 372e 3336 222c 274d 6f7a  ari/537.36",'Moz
+000039c0: 696c 6c61 2f35 2e30 2028 5769 6e64 6f77  illa/5.0 (Window
+000039d0: 7320 4e54 2031 302e 303b 2057 4f57 3634  s NT 10.0; WOW64
+000039e0: 2920 4170 706c 6557 6562 4b69 742f 3533  ) AppleWebKit/53
+000039f0: 372e 3336 2028 4b48 544d 4c2c 206c 696b  7.36 (KHTML, lik
+00003a00: 6520 4765 636b 6f29 2043 6872 6f6d 652f  e Gecko) Chrome/
+00003a10: 3738 2e30 2e33 3930 342e 3130 3820 5361  78.0.3904.108 Sa
+00003a20: 6661 7269 2f35 3337 2e33 3627 2c27 4d6f  fari/537.36','Mo
+00003a30: 7a69 6c6c 612f 342e 3020 2863 6f6d 7061  zilla/4.0 (compa
+00003a40: 7469 626c 653b 204d 5349 4520 362e 303b  tible; MSIE 6.0;
+00003a50: 2029 204f 7065 7261 2f55 4357 4542 372e   ) Opera/UCWEB7.
+00003a60: 302e 322e 3337 2f32 382f 3939 3927 2c27  0.2.37/28/999','
+00003a70: 4d6f 7a69 6c6c 612f 342e 3020 2863 6f6d  Mozilla/4.0 (com
+00003a80: 7061 7469 626c 653b 204d 5349 4520 372e  patible; MSIE 7.
+00003a90: 303b 2057 696e 646f 7773 204e 5420 352e  0; Windows NT 5.
+00003aa0: 3129 272c 274d 6f7a 696c 6c61 2f34 2e30  1)','Mozilla/4.0
+00003ab0: 2028 636f 6d70 6174 6962 6c65 3b20 4d53   (compatible; MS
+00003ac0: 4945 2037 2e30 3b20 5769 6e64 6f77 7320  IE 7.0; Windows 
+00003ad0: 4e54 2035 2e31 2927 2c27 4d6f 7a69 6c6c  NT 5.1)','Mozill
+00003ae0: 612f 342e 3020 2863 6f6d 7061 7469 626c  a/4.0 (compatibl
+00003af0: 653b 204d 5349 4520 372e 303b 2057 696e  e; MSIE 7.0; Win
+00003b00: 646f 7773 204e 5420 352e 313b 2033 3630  dows NT 5.1; 360
+00003b10: 5345 2927 2c27 4d6f 7a69 6c6c 612f 342e  SE)','Mozilla/4.
+00003b20: 3020 2863 6f6d 7061 7469 626c 653b 204d  0 (compatible; M
+00003b30: 5349 4520 372e 303b 2057 696e 646f 7773  SIE 7.0; Windows
+00003b40: 204e 5420 352e 313b 2041 7661 6e74 2042   NT 5.1; Avant B
+00003b50: 726f 7773 6572 2927 2c27 4d6f 7a69 6c6c  rowser)','Mozill
+00003b60: 612f 342e 3020 2863 6f6d 7061 7469 626c  a/4.0 (compatibl
+00003b70: 653b 204d 5349 4520 372e 303b 2057 696e  e; MSIE 7.0; Win
+00003b80: 646f 7773 204e 5420 352e 313b 204d 6178  dows NT 5.1; Max
+00003b90: 7468 6f6e 2032 2e30 2927 2c27 4d6f 7a69  thon 2.0)','Mozi
+00003ba0: 6c6c 612f 342e 3020 2863 6f6d 7061 7469  lla/4.0 (compati
+00003bb0: 626c 653b 204d 5349 4520 372e 303b 2057  ble; MSIE 7.0; W
+00003bc0: 696e 646f 7773 204e 5420 352e 313b 2054  indows NT 5.1; T
+00003bd0: 656e 6365 6e74 5472 6176 656c 6572 2034  encentTraveler 4
+00003be0: 2e30 2927 2c27 4d6f 7a69 6c6c 612f 342e  .0)','Mozilla/4.
+00003bf0: 3020 2863 6f6d 7061 7469 626c 653b 204d  0 (compatible; M
+00003c00: 5349 4520 372e 303b 2057 696e 646f 7773  SIE 7.0; Windows
+00003c10: 204e 5420 352e 313b 2054 6865 2057 6f72   NT 5.1; The Wor
+00003c20: 6c64 2927 2c27 4d6f 7a69 6c6c 612f 342e  ld)','Mozilla/4.
+00003c30: 3020 2863 6f6d 7061 7469 626c 653b 204d  0 (compatible; M
+00003c40: 5349 4520 382e 303b 2057 696e 646f 7773  SIE 8.0; Windows
+00003c50: 204e 5420 362e 303b 2054 7269 6465 6e74   NT 6.0; Trident
+00003c60: 2f34 2e30 2927 2c27 4d6f 7a69 6c6c 612f  /4.0)','Mozilla/
+00003c70: 352e 3020 2842 6c61 636b 4265 7272 793b  5.0 (BlackBerry;
+00003c80: 2055 3b20 426c 6163 6b42 6572 7279 2039   U; BlackBerry 9
+00003c90: 3830 303b 2065 6e29 2041 7070 6c65 5765  800; en) AppleWe
+00003ca0: 624b 6974 2f35 3334 2e31 2b20 284b 4854  bKit/534.1+ (KHT
+00003cb0: 4d4c 2c20 6c69 6b65 2047 6563 6b6f 2920  ML, like Gecko) 
+00003cc0: 5665 7273 696f 6e2f 362e 302e 302e 3333  Version/6.0.0.33
+00003cd0: 3720 4d6f 6269 6c65 2053 6166 6172 692f  7 Mobile Safari/
+00003ce0: 3533 342e 312b 272c 274d 6f7a 696c 6c61  534.1+','Mozilla
+00003cf0: 2f35 2e30 2028 636f 6d70 6174 6962 6c65  /5.0 (compatible
+00003d00: 3b20 4d53 4945 2039 2e30 3b20 5769 6e64  ; MSIE 9.0; Wind
+00003d10: 6f77 7320 4e54 2036 2e31 3b20 5472 6964  ows NT 6.1; Trid
+00003d20: 656e 742f 352e 3027 2c27 4d6f 7a69 6c6c  ent/5.0','Mozill
+00003d30: 612f 352e 3020 2863 6f6d 7061 7469 626c  a/5.0 (compatibl
+00003d40: 653b 204d 5349 4520 392e 303b 2057 696e  e; MSIE 9.0; Win
+00003d50: 646f 7773 2050 686f 6e65 204f 5320 372e  dows Phone OS 7.
+00003d60: 353b 2054 7269 6465 6e74 2f35 2e30 3b20  5; Trident/5.0; 
+00003d70: 4945 4d6f 6269 6c65 2f39 2e30 3b20 4854  IEMobile/9.0; HT
+00003d80: 433b 2054 6974 616e 2927 2c27 4d6f 7a69  C; Titan)','Mozi
+00003d90: 6c6c 612f 352e 3020 2869 5061 643b 2055  lla/5.0 (iPad; U
+00003da0: 3b20 4350 5520 4f53 2034 5f33 5f33 206c  ; CPU OS 4_3_3 l
+00003db0: 696b 6520 4d61 6320 4f53 2058 3b20 656e  ike Mac OS X; en
+00003dc0: 2d75 7329 2041 7070 6c65 5765 624b 6974  -us) AppleWebKit
+00003dd0: 2f35 3333 2e31 372e 3920 284b 4854 4d4c  /533.17.9 (KHTML
+00003de0: 2c20 6c69 6b65 2047 6563 6b6f 2920 5665  , like Gecko) Ve
+00003df0: 7273 696f 6e2f 352e 302e 3220 4d6f 6269  rsion/5.0.2 Mobi
+00003e00: 6c65 2f38 4a32 2053 6166 6172 692f 3635  le/8J2 Safari/65
+00003e10: 3333 2e31 382e 3527 2c27 4d6f 7a69 6c6c  33.18.5','Mozill
+00003e20: 612f 352e 3020 2869 5068 6f6e 653b 2055  a/5.0 (iPhone; U
+00003e30: 3b20 4350 5520 6950 686f 6e65 204f 5320  ; CPU iPhone OS 
+00003e40: 345f 335f 3320 6c69 6b65 204d 6163 204f  4_3_3 like Mac O
+00003e50: 5320 583b 2065 6e2d 7573 2920 4170 706c  S X; en-us) Appl
+00003e60: 6557 6562 4b69 742f 3533 332e 3137 2e39  eWebKit/533.17.9
+00003e70: 2028 4b48 544d 4c2c 206c 696b 6520 4765   (KHTML, like Ge
+00003e80: 636b 6f29 2056 6572 7369 6f6e 2f35 2e30  cko) Version/5.0
+00003e90: 2e32 204d 6f62 696c 652f 384a 3220 5361  .2 Mobile/8J2 Sa
+00003ea0: 6661 7269 2f36 3533 332e 3138 2e35 272c  fari/6533.18.5',
+00003eb0: 274d 6f7a 696c 6c61 2f35 2e30 2028 6950  'Mozilla/5.0 (iP
+00003ec0: 6f64 3b20 553b 2043 5055 2069 5068 6f6e  od; U; CPU iPhon
+00003ed0: 6520 4f53 2034 5f33 5f33 206c 696b 6520  e OS 4_3_3 like 
+00003ee0: 4d61 6320 4f53 2058 3b20 656e 2d75 7329  Mac OS X; en-us)
+00003ef0: 2041 7070 6c65 5765 624b 6974 2f35 3333   AppleWebKit/533
+00003f00: 2e31 372e 3920 284b 4854 4d4c 2c20 6c69  .17.9 (KHTML, li
+00003f10: 6b65 2047 6563 6b6f 2920 5665 7273 696f  ke Gecko) Versio
+00003f20: 6e2f 352e 302e 3220 4d6f 6269 6c65 2f38  n/5.0.2 Mobile/8
+00003f30: 4a32 2053 6166 6172 692f 3635 3333 2e31  J2 Safari/6533.1
+00003f40: 382e 3527 2c27 4d6f 7a69 6c6c 612f 352e  8.5','Mozilla/5.
+00003f50: 3020 284c 696e 7578 3b20 553b 2041 6e64  0 (Linux; U; And
+00003f60: 726f 6964 2032 2e33 2e37 3b20 656e 2d75  roid 2.3.7; en-u
+00003f70: 733b 204e 6578 7573 204f 6e65 2042 7569  s; Nexus One Bui
+00003f80: 6c64 2f46 5246 3931 2920 4170 706c 6557  ld/FRF91) AppleW
+00003f90: 6562 4b69 742f 3533 332e 3120 284b 4854  ebKit/533.1 (KHT
+00003fa0: 4d4c 2c20 6c69 6b65 2047 6563 6b6f 2920  ML, like Gecko) 
+00003fb0: 5665 7273 696f 6e2f 342e 3020 4d6f 6269  Version/4.0 Mobi
+00003fc0: 6c65 2053 6166 6172 692f 3533 332e 3127  le Safari/533.1'
+00003fd0: 2c27 4d6f 7a69 6c6c 612f 352e 3020 284c  ,'Mozilla/5.0 (L
+00003fe0: 696e 7578 3b20 553b 2041 6e64 726f 6964  inux; U; Android
+00003ff0: 2033 2e30 3b20 656e 2d75 733b 2058 6f6f   3.0; en-us; Xoo
+00004000: 6d20 4275 696c 642f 4852 4933 3929 2041  m Build/HRI39) A
+00004010: 7070 6c65 5765 624b 6974 2f35 3334 2e31  ppleWebKit/534.1
+00004020: 3320 284b 4854 4d4c 2c20 6c69 6b65 2047  3 (KHTML, like G
+00004030: 6563 6b6f 2920 5665 7273 696f 6e2f 342e  ecko) Version/4.
+00004040: 3020 5361 6661 7269 2f35 3334 2e31 3327  0 Safari/534.13'
+00004050: 2c27 4d6f 7a69 6c6c 612f 352e 3020 284d  ,'Mozilla/5.0 (M
+00004060: 6163 696e 746f 7368 3b20 496e 7465 6c20  acintosh; Intel 
+00004070: 4d61 6320 4f53 2058 2031 302e 363b 2072  Mac OS X 10.6; r
+00004080: 763a 322e 302e 3129 2047 6563 6b6f 2f32  v:2.0.1) Gecko/2
+00004090: 3031 3030 3130 3120 4669 7265 666f 782f  0100101 Firefox/
+000040a0: 342e 302e 3127 2c27 4d6f 7a69 6c6c 612f  4.0.1','Mozilla/
+000040b0: 352e 3020 2857 696e 646f 7773 204e 5420  5.0 (Windows NT 
+000040c0: 362e 313b 2072 763a 322e 302e 3129 2047  6.1; rv:2.0.1) G
+000040d0: 6563 6b6f 2f32 3031 3030 3130 3120 4669  ecko/20100101 Fi
+000040e0: 7265 666f 782f 342e 302e 3127 2c27 4d6f  refox/4.0.1','Mo
+000040f0: 7a69 6c6c 612f 352e 3020 2857 696e 646f  zilla/5.0 (Windo
+00004100: 7773 3b20 553b 2057 696e 646f 7773 204e  ws; U; Windows N
+00004110: 5420 362e 313b 2065 6e2d 7573 2920 4170  T 6.1; en-us) Ap
+00004120: 706c 6557 6562 4b69 742f 3533 342e 3530  pleWebKit/534.50
+00004130: 2028 4b48 544d 4c2c 206c 696b 6520 4765   (KHTML, like Ge
+00004140: 636b 6f29 2056 6572 7369 6f6e 2f35 2e31  cko) Version/5.1
+00004150: 2053 6166 6172 692f 3533 342e 3530 272c   Safari/534.50',
+00004160: 274d 6f7a 696c 6c61 2f35 2e30 2028 5769  'Mozilla/5.0 (Wi
+00004170: 6e64 6f77 733b 2055 3b20 5769 6e64 6f77  ndows; U; Window
+00004180: 7320 4e54 2036 2e31 3b20 656e 2d55 533b  s NT 6.1; en-US;
+00004190: 2072 763a 312e 392e 312e 3629 2047 6563   rv:1.9.1.6) Gec
+000041a0: 6b6f 2f32 3030 3931 3230 3120 4669 7265  ko/20091201 Fire
+000041b0: 666f 782f 332e 352e 3627 2c27 4e4f 4b49  fox/3.5.6','NOKI
+000041c0: 4135 3730 302f 2055 4357 4542 372e 302e  A5700/ UCWEB7.0.
+000041d0: 322e 3337 2f32 382f 3939 3927 2c27 4f70  2.37/28/999','Op
+000041e0: 656e 7761 7665 2f20 5543 5745 4237 2e30  enwave/ UCWEB7.0
+000041f0: 2e32 2e33 372f 3238 2f39 3939 272c 274f  .2.37/28/999','O
+00004200: 7065 7261 2f39 2e38 3020 2841 6e64 726f  pera/9.80 (Andro
+00004210: 6964 2032 2e33 2e34 3b20 4c69 6e75 783b  id 2.3.4; Linux;
+00004220: 204f 7065 7261 204d 6f62 692f 6275 696c   Opera Mobi/buil
+00004230: 642d 3131 3037 3138 3039 3435 3b20 553b  d-1107180945; U;
+00004240: 2065 6e2d 4742 2920 5072 6573 746f 2f32   en-GB) Presto/2
+00004250: 2e38 2e31 3439 2056 6572 7369 6f6e 2f31  .8.149 Version/1
+00004260: 312e 3130 272c 274f 7065 7261 2f39 2e38  1.10','Opera/9.8
+00004270: 3020 284d 6163 696e 746f 7368 3b20 496e  0 (Macintosh; In
+00004280: 7465 6c20 4d61 6320 4f53 2058 2031 302e  tel Mac OS X 10.
+00004290: 362e 383b 2055 3b20 656e 2920 5072 6573  6.8; U; en) Pres
+000042a0: 746f 2f32 2e38 2e31 3331 2056 6572 7369  to/2.8.131 Versi
+000042b0: 6f6e 2f31 312e 3131 272c 274f 7065 7261  on/11.11','Opera
+000042c0: 2f39 2e38 3020 2857 696e 646f 7773 204e  /9.80 (Windows N
+000042d0: 5420 362e 313b 2055 3b20 656e 2920 5072  T 6.1; U; en) Pr
+000042e0: 6573 746f 2f32 2e38 2e31 3331 2056 6572  esto/2.8.131 Ver
+000042f0: 7369 6f6e 2f31 312e 3131 272c 2755 4357  sion/11.11','UCW
+00004300: 4542 372e 302e 322e 3337 2f32 382f 3939  EB7.0.2.37/28/99
+00004310: 3927 5d0d 0a                             9']..
```

### Comparing `PgsFile-0.0.6/PgsFile/__init__.py` & `PgsFile-0.0.7/PgsFile/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,11 +13,12 @@
 from .PgsFile import BigPunctuation
 from .PgsFile import StopTags
 from .PgsFile import Special
 from .PgsFile import StopWords
 from .PgsFile import EnPunctuation
 
 from .PgsFile import word_list
+from .PgsFile import batch_word_list
 from .PgsFile import clean_list
 from .PgsFile import yhd
 
 name = "PgsFile"
```

### Comparing `PgsFile-0.0.6/PgsFile.egg-info/PKG-INFO` & `PgsFile-0.0.7/PgsFile.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: PgsFile
-Version: 0.0.6
-Summary: To make file operations coding easier for literary students
+Version: 0.0.7
+Summary: To make file operations and wordlist coding easier for literary students
 Home-page:  
 Author: Pan Guisheng
 Author-email: 895284504@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Free For Educational Use
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Purpose: This module is to facilitate Python beginners, especially instructors and students of foreign languages and literature, for the convenience of easily operating txt, xlsx and json files. 
+Purpose: This module is to facilitate Python beginners, especially instructors and students of foreign languages and literature, for the convenience of easily operating txt, xlsx and json files as well as making word list. 
 
 Function 1: Useful for getting data from the files directly and saving processing results in the files. Either task can be done with a single line of code.
 
 Function 2: The functions of "FilePath" and "FileName" imported from the py file can effectively help you get all the absolute file paths in any folder (containing all the files of any sub-folder in the folder) of your PC disk and obtain the file names. This will be also realized within one line of code.
 
-Function 3: You can make a word list of a certain file or a batch of files, showing their word frequency sorted in reverse order, easily with the function of "word_list" in PgsFile.
+Function 3: You can make a word list of a certain file or a batch of files, showing their word frequency sorted in reverse order, easily with the function of "word_list" and "batch_word_list" in PgsFile.
 
 Author: Pan Guisheng, a PhD student at the Graduate Institute of Interpretation and Translation of Shanghai International Studies University
 E-mail: 895284504@qq.com
```

### Comparing `PgsFile-0.0.6/README.md` & `PgsFile-0.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Purpose: This module is to facilitate Python beginners, especially instructors and students of foreign languages and literature, for the convenience of easily operating txt, xlsx and json files. 
+Purpose: This module is to facilitate Python beginners, especially instructors and students of foreign languages and literature, for the convenience of easily operating txt, xlsx and json files as well as making word list. 
 
 Function 1: Useful for getting data from the files directly and saving processing results in the files. Either task can be done with a single line of code.
 
 Function 2: The functions of "FilePath" and "FileName" imported from the py file can effectively help you get all the absolute file paths in any folder (containing all the files of any sub-folder in the folder) of your PC disk and obtain the file names. This will be also realized within one line of code.
 
-Function 3: You can make a word list of a certain file or a batch of files, showing their word frequency sorted in reverse order, easily with the function of "word_list" in PgsFile.
+Function 3: You can make a word list of a certain file or a batch of files, showing their word frequency sorted in reverse order, easily with the function of "word_list" and "batch_word_list" in PgsFile.
 
 Author: Pan Guisheng, a PhD student at the Graduate Institute of Interpretation and Translation of Shanghai International Studies University
 E-mail: 895284504@qq.com
```

### Comparing `PgsFile-0.0.6/setup.py` & `PgsFile-0.0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="PgsFile",
-    version="0.0.6",
+    version="0.0.7",
     author="Pan Guisheng",
     author_email="895284504@qq.com",
-    description="To make file operations coding easier for literary students",
+    description="To make file operations and wordlist coding easier for literary students",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url=" ",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: Free For Educational Use",
```

