# Comparing `tmp/autoDownload-0.0.7.tar.gz` & `tmp/autoDownload-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoDownload-0.0.7.tar", last modified: Fri Mar 31 07:12:27 2023, max compression
+gzip compressed data, was "autoDownload-0.0.9.tar", last modified: Mon Apr 24 06:12:42 2023, max compression
```

## Comparing `autoDownload-0.0.7.tar` & `autoDownload-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 07:12:27.174477 autoDownload-0.0.7/
--rw-rw-rw-   0        0        0     9719 2023-03-28 07:31:29.000000 autoDownload-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     1465 2023-03-31 07:12:27.174477 autoDownload-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      589 2023-03-29 04:52:44.000000 autoDownload-0.0.7/README.md
--rw-rw-rw-   0        0        0      731 2023-03-29 10:01:49.000000 autoDownload-0.0.7/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-31 07:12:27.169475 autoDownload-0.0.7/autoDownload/
--rw-rw-rw-   0        0        0    21883 2023-03-31 07:12:21.000000 autoDownload-0.0.7/autoDownload/__init__.py
--rw-rw-rw-   0        0        0     2463 2023-03-31 06:42:27.000000 autoDownload-0.0.7/autoDownload/terminal.py
-drwxrwxrwx   0        0        0        0 2023-03-31 07:12:27.173478 autoDownload-0.0.7/autoDownload.egg-info/
--rw-rw-rw-   0        0        0     1465 2023-03-31 07:12:27.000000 autoDownload-0.0.7/autoDownload.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2023-03-31 07:12:27.000000 autoDownload-0.0.7/autoDownload.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 07:12:27.000000 autoDownload-0.0.7/autoDownload.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-03-31 07:12:27.000000 autoDownload-0.0.7/autoDownload.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-03-31 07:12:27.000000 autoDownload-0.0.7/autoDownload.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-03-31 07:12:27.000000 autoDownload-0.0.7/autoDownload.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-31 07:12:27.174477 autoDownload-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1191 2023-03-31 06:42:52.000000 autoDownload-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 06:12:42.767547 autoDownload-0.0.9/
+-rw-rw-rw-   0        0        0     9719 2023-03-28 07:31:29.000000 autoDownload-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1465 2023-04-24 06:12:42.766547 autoDownload-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      590 2023-04-24 05:58:36.000000 autoDownload-0.0.9/README.md
+-rw-rw-rw-   0        0        0      731 2023-03-29 10:01:49.000000 autoDownload-0.0.9/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-24 06:12:42.754547 autoDownload-0.0.9/autoDownload/
+-rw-rw-rw-   0        0        0    21933 2023-04-24 02:58:04.000000 autoDownload-0.0.9/autoDownload/__init__.py
+-rw-rw-rw-   0        0        0     2463 2023-03-31 07:14:23.000000 autoDownload-0.0.9/autoDownload/terminal.py
+drwxrwxrwx   0        0        0        0 2023-04-24 06:12:42.765547 autoDownload-0.0.9/autoDownload.egg-info/
+-rw-rw-rw-   0        0        0     1465 2023-04-24 06:12:42.000000 autoDownload-0.0.9/autoDownload.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2023-04-24 06:12:42.000000 autoDownload-0.0.9/autoDownload.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 06:12:42.000000 autoDownload-0.0.9/autoDownload.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-24 06:12:42.000000 autoDownload-0.0.9/autoDownload.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-04-24 06:12:42.000000 autoDownload-0.0.9/autoDownload.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-24 06:12:42.000000 autoDownload-0.0.9/autoDownload.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 06:12:42.767547 autoDownload-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1191 2023-04-24 06:12:18.000000 autoDownload-0.0.9/setup.py
```

### Comparing `autoDownload-0.0.7/LICENSE` & `autoDownload-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `autoDownload-0.0.7/PKG-INFO` & `autoDownload-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoDownload
-Version: 0.0.7
+Version: 0.0.9
 Summary: download files quickly
 Home-page: https://kuankuan2007.gitee.io/docs/multithreaded-download/
 Author: kuankuan
 Author-email: 2163826131@qq.com
 License: Mulan PSL v2
 Keywords: requests,download,http,thread
 Platform: windows
```

### Comparing `autoDownload-0.0.7/README.md` & `autoDownload-0.0.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # 多线程下载(autoDownload)
 
-```
-pip install import autoDownload
+```bash
+pip install autoDownload
 ```
 
 ## import使用方法
 
 ```python
 import autoDownload
 autoDownload.AutoDownload(url,file,key=values...)
 ```
 
 ## 命令行使用方法
 
 参见
 
-```
+```bash
 auto-download -h
 ```
 
 ## 关于作者
 
 作者主页[宽宽2007](https://kuankuan2007.gitee.io "作者主页")
```

### Comparing `autoDownload-0.0.7/README.rst` & `autoDownload-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `autoDownload-0.0.7/autoDownload/__init__.py` & `autoDownload-0.0.9/autoDownload/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import requests
 import logging
 import threading
 import rich.progress
 import rich.text
 import os
-from typing import Callable,Any,List
+from typing import Callable,Any,List,Union
 import tempfile
 import random
 import time
 class ConnectError(Exception):
     def __init__(self,url:str) -> None:
         super().__init__(self)
         self.url=url
@@ -47,15 +47,15 @@
 
         return rich.text.Text(formatted, style=style)
 class _Part:
     """
     A download task. It mean a part of the file we are downloading.
     It include the range of this task, the response, the statue, etc.
     """
-    def __init__(self,start_:int,to:int,num:int=0,fileName:str="",stream:None|requests.Response=None) -> None:
+    def __init__(self,start_:int,to:int,num:int=0,fileName:str="",stream:Union[None,requests.Response]=None) -> None:
         """
         New a Part object
         :param start_: the start position of the part
         :param to: the end position of the part
         :param num: the num of the part
         :param fileName: the tempfile name of the part
         :param stream: the response of the part
@@ -64,15 +64,15 @@
         self.start=start_
         self.to=to
         self.fileName=fileName
         self.speed=0
         self.retryTime=0
         self.statue="init"
         self.stream=stream
-        self.progress:None|rich.progress.TaskID=None
+        self.progress:Union[None,rich.progress.TaskID]=None
         self.now:int=0
         self.histoyTime:int=0
         self.historyNum:int=0
         self.speeds:str=""
         self.statueNum:int=0
         self.startTime:float=1.0
     def split(self,position:int):
@@ -87,18 +87,18 @@
         self.to=position
         return new
     def __lt__(self,other):
         if self.start!=other.start:
             return  self.start<other.start
         return self.to<other.to
 class AutoDownload:
-    def __init__(self,url:str,file:str,chunkSize:int=1024,maxRetry:int=5,maxThreadRetry:int=-1,timeout:int|None=30,continueDownloadTest:bool=False,startSize:int=0,openType:str="wb",
+    def __init__(self,url:str,file:str,chunkSize:int=1024,maxRetry:int=5,maxThreadRetry:int=-1,timeout:Union[int,None]=30,continueDownloadTest:bool=False,startSize:int=0,openType:str="wb",
                  error:bool=True,log:bool=True,showProgressBar:bool=True,transient:bool=False,
                  threaded:bool=False,threadNum:int=0,maxThreadNum:int=10,desiredCompletionTime:int=30,
-                 callbackFunction:None|Callable[[bool], Any]=None,deamon:bool=False,header:dict={})->None:
+                 callbackFunction:Union[None,Callable[[bool], Any]]=None,deamon:bool=False,header:dict={})->None:
         """
         Download file from url to file
         :param url: url to download
         :param file: file name
         :param chunkSize: chunk size
         :param maxRetry: max retry times for the first connection. If it's less than 0, it means infinity
         :param maxThreadRetry: max retry times for the other connection. If it's less than 0, it means infinity
@@ -176,30 +176,30 @@
         Show error message and raise it.
         :param err: the error
         """
         self._logShower("%s:%s"%(err.__class__.__name__,str(err)),logging.ERROR)
         self.fail=True
         if self.error:
             raise err
-    def start(self)->bool|None:
+    def start(self)->Union[bool,None]:
         """
         Start the download.
         :return: True if success, False if fail, None if self.threaded is True.
         """
         if self.continueDownloadTest:
             if os.path.isfile(self.file) and os.access(self.file,os.W_OK):#文件是否存在 and 是否可读
                 self.startSize=os.path.getsize(self.file)
                 self.openType="ab"
             else:
                 self._errorShower(FileNotFoundError("Can not open file '%s' for download."%(self.file)))
                 return False
         os.makedirs(self.tempFileDir)
         if self.threaded:threading.Thread(target=self._wait,daemon=self.deamon,name="Download controller")
         else:return self._wait()
-    def changeUnit(self,num:int|float)->str:
+    def changeUnit(self,num:Union[int,float])->str:
         """
         Change the unit of the data size.
         :param num: the size of the data
         :return: the formatted string 
         """
         units=["B","KB","MB","GB","TB"]
         if num<0:
@@ -445,14 +445,15 @@
                     self._waitList.remove(partNum)
                     part.now=part.to-part.start
                     part.speed=0
                     part.speeds="--"
                     self._logShower(f"Part {partNum} is finished",level=logging.DEBUG)
                     self._finished()
                     return
+
             except BaseException as err:
                 if retryNum==self.maxThreadRetry:
                     self._errorShower(err)
                 retryNum+=1
                 part.statue=f"retry {retryNum}"
                 part.statueNum=1
                 self._logShower("Part %d %s:%s"%(partNum,err.__class__.__name__,str(err)),level=logging.WARNING)
```

### Comparing `autoDownload-0.0.7/autoDownload/terminal.py` & `autoDownload-0.0.9/autoDownload/terminal.py`

 * *Files identical despite different names*

### Comparing `autoDownload-0.0.7/autoDownload.egg-info/PKG-INFO` & `autoDownload-0.0.9/autoDownload.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoDownload
-Version: 0.0.7
+Version: 0.0.9
 Summary: download files quickly
 Home-page: https://kuankuan2007.gitee.io/docs/multithreaded-download/
 Author: kuankuan
 Author-email: 2163826131@qq.com
 License: Mulan PSL v2
 Keywords: requests,download,http,thread
 Platform: windows
```

### Comparing `autoDownload-0.0.7/setup.py` & `autoDownload-0.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 from distutils.core import setup
 
 setup(
     name = 'autoDownload',
-    version = '0.0.7',
+    version = '0.0.9',
     keywords = ['requests',"download","http","thread"],
     description = 'download files quickly',
     long_description = open("README.rst","r",encoding="utf-8").read(),
     author = 'kuankuan',
     author_email = '2163826131@qq.com',
     url="https://kuankuan2007.gitee.io/docs/multithreaded-download/",
     install_requires = [
```

