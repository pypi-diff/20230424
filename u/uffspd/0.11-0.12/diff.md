# Comparing `tmp/uffspd-0.11.tar.gz` & `tmp/uffspd-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uffspd-0.11.tar", last modified: Mon Apr 24 13:23:19 2023, max compression
+gzip compressed data, was "uffspd-0.12.tar", last modified: Mon Apr 24 14:33:25 2023, max compression
```

## Comparing `uffspd-0.11.tar` & `uffspd-0.12.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 13:23:19.224645 uffspd-0.11/
--rw-rw-rw-   0        0        0     1148 2023-04-24 13:23:10.000000 uffspd-0.11/LICENSE.rst
--rw-rw-rw-   0        0        0      138 2023-04-24 13:23:09.000000 uffspd-0.11/MANIFEST.in
--rw-rw-rw-   0        0        0     7410 2023-04-24 13:23:19.224645 uffspd-0.11/PKG-INFO
--rw-rw-rw-   0        0        0     6672 2023-04-15 00:18:31.000000 uffspd-0.11/README.md
--rw-rw-rw-   0        0        0       85 2023-04-24 13:23:19.227637 uffspd-0.11/setup.cfg
--rw-rw-rw-   0        0        0     1602 2023-04-24 13:23:18.000000 uffspd-0.11/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:23:19.206693 uffspd-0.11/uffspd/
--rw-rw-rw-   0        0        0     1090 2023-04-15 00:18:31.000000 uffspd-0.11/uffspd/LICENSE
--rw-rw-rw-   0        0        0     6672 2023-04-15 00:18:31.000000 uffspd-0.11/uffspd/README.MD
--rw-rw-rw-   0        0        0     5405 2023-04-24 13:20:54.000000 uffspd-0.11/uffspd/__init__.py
--rw-rw-rw-   0        0        0       81 2023-04-24 13:23:18.000000 uffspd-0.11/uffspd/requirements.txt
--rw-rw-rw-   0        0        0    62540 2023-04-24 13:23:18.000000 uffspd-0.11/uffspd/thirdparty.json
--rwxrwxrwx   0        0        0  1540608 2023-04-24 13:05:29.000000 uffspd-0.11/uffspd/uffs.com
-drwxrwxrwx   0        0        0        0 2023-04-24 13:23:19.223648 uffspd-0.11/uffspd.egg-info/
--rw-rw-rw-   0        0        0     7410 2023-04-24 13:23:18.000000 uffspd-0.11/uffspd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-04-24 13:23:19.000000 uffspd-0.11/uffspd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 13:23:18.000000 uffspd-0.11/uffspd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-04-24 13:23:18.000000 uffspd-0.11/uffspd.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-24 13:23:18.000000 uffspd-0.11/uffspd.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 14:33:25.457947 uffspd-0.12/
+-rw-rw-rw-   0        0        0     1148 2023-04-24 14:33:16.000000 uffspd-0.12/LICENSE.rst
+-rw-rw-rw-   0        0        0      138 2023-04-24 14:33:14.000000 uffspd-0.12/MANIFEST.in
+-rw-rw-rw-   0        0        0     7410 2023-04-24 14:33:25.457947 uffspd-0.12/PKG-INFO
+-rw-rw-rw-   0        0        0     6672 2023-04-15 00:18:31.000000 uffspd-0.12/README.md
+-rw-rw-rw-   0        0        0       85 2023-04-24 14:33:25.457947 uffspd-0.12/setup.cfg
+-rw-rw-rw-   0        0        0     1602 2023-04-24 14:33:24.000000 uffspd-0.12/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:33:25.440373 uffspd-0.12/uffspd/
+-rw-rw-rw-   0        0        0     1090 2023-04-15 00:18:31.000000 uffspd-0.12/uffspd/LICENSE
+-rw-rw-rw-   0        0        0     6672 2023-04-15 00:18:31.000000 uffspd-0.12/uffspd/README.MD
+-rw-rw-rw-   0        0        0     5623 2023-04-24 14:32:27.000000 uffspd-0.12/uffspd/__init__.py
+-rw-rw-rw-   0        0        0       81 2023-04-24 14:33:24.000000 uffspd-0.12/uffspd/requirements.txt
+-rw-rw-rw-   0        0        0    62540 2023-04-24 14:33:24.000000 uffspd-0.12/uffspd/thirdparty.json
+-rwxrwxrwx   0        0        0  1540608 2023-04-24 14:24:48.000000 uffspd-0.12/uffspd/uffs.com
+drwxrwxrwx   0        0        0        0 2023-04-24 14:33:25.456922 uffspd-0.12/uffspd.egg-info/
+-rw-rw-rw-   0        0        0     7410 2023-04-24 14:33:25.000000 uffspd-0.12/uffspd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-04-24 14:33:25.000000 uffspd-0.12/uffspd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 14:33:25.000000 uffspd-0.12/uffspd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-04-24 14:33:25.000000 uffspd-0.12/uffspd.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-24 14:33:25.000000 uffspd-0.12/uffspd.egg-info/top_level.txt
```

### Comparing `uffspd-0.11/LICENSE.rst` & `uffspd-0.12/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `uffspd-0.11/PKG-INFO` & `uffspd-0.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uffspd
-Version: 0.11
+Version: 0.12
 Summary: Wrapper for the fastest file/folder list tool (UFFS) 350 GB in less than 3 Minutes (1.800.000 files and folders)
 Home-page: https://github.com/hansalemaos/uffspd
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: ripgrep,grep,search,replace,regex,regular expressions,re,os.listdir,shutil,ls
 Classifier: Development Status :: 4 - Beta
```

### Comparing `uffspd-0.11/README.md` & `uffspd-0.12/README.md`

 * *Files identical despite different names*

### Comparing `uffspd-0.11/setup.py` & `uffspd-0.12/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
 #     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.11'''
+VERSION = '''0.12'''
 DESCRIPTION = '''Wrapper for the fastest file/folder list tool (UFFS) 350 GB in less than 3 Minutes (1.800.000 files and folders)'''
 
 # Setting up
 setup(
     name="uffspd",
     version=VERSION,
     license='MIT',
```

### Comparing `uffspd-0.11/uffspd/LICENSE` & `uffspd-0.12/uffspd/LICENSE`

 * *Files identical despite different names*

### Comparing `uffspd-0.11/uffspd/README.MD` & `uffspd-0.12/uffspd/README.MD`

 * *Files identical despite different names*

### Comparing `uffspd-0.11/uffspd/__init__.py` & `uffspd-0.12/uffspd/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -123,18 +123,23 @@
         feax = vartolist(file_extensions)
         file_extensions = "--ext=" + (
             ",".join([x.strip(". ") for x in feax]).strip().strip(".")
         )
     exefile = os.path.normpath(uffs_com_path)
     parsedpath = pathlib.Path(path2search).as_posix()
     wholecmdsearch = [rf"{exefile}", "--columns=all", file_extensions, parsedpath]
+    startupinfo = subprocess.STARTUPINFO()
+    creationflags = 0 | subprocess.CREATE_NO_WINDOW
+    startupinfo.wShowWindow = subprocess.SW_HIDE
     dada = subprocess.run(
         wholecmdsearch,
         shell=False,
         capture_output=True,
+        startupinfo=startupinfo,
+        creationflags=creationflags
     )
     out = dada.stdout
     dat2 = out.splitlines()
     df2 = pd.DataFrame(dat2)
     df3 = df2.copy()
     df = df3[0].s_str().rsplit(b",", n=24, expand=True)
     newcols = [
```

### Comparing `uffspd-0.11/uffspd/thirdparty.json` & `uffspd-0.12/uffspd/thirdparty.json`

 * *Files identical despite different names*

### Comparing `uffspd-0.11/uffspd/uffs.com` & `uffspd-0.12/uffspd/uffs.com`

 * *Files identical despite different names*

### Comparing `uffspd-0.11/uffspd.egg-info/PKG-INFO` & `uffspd-0.12/uffspd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uffspd
-Version: 0.11
+Version: 0.12
 Summary: Wrapper for the fastest file/folder list tool (UFFS) 350 GB in less than 3 Minutes (1.800.000 files and folders)
 Home-page: https://github.com/hansalemaos/uffspd
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: ripgrep,grep,search,replace,regex,regular expressions,re,os.listdir,shutil,ls
 Classifier: Development Status :: 4 - Beta
```

