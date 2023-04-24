# Comparing `tmp/qufit-1.0.7.tar.gz` & `tmp/qufit-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qufit-1.0.7.tar", last modified: Fri Apr 14 07:10:49 2023, max compression
+gzip compressed data, was "qufit-1.0.8.tar", last modified: Mon Apr 24 06:32:59 2023, max compression
```

## Comparing `qufit-1.0.7.tar` & `qufit-1.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 07:10:49.946347 qufit-1.0.7/
--rw-rw-rw-   0        0        0      820 2023-04-14 07:10:49.944353 qufit-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      331 2022-11-06 13:08:56.000000 qufit-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 07:10:49.922448 qufit-1.0.7/qufit/
--rw-rw-rw-   0        0        0       16 2022-11-06 12:49:07.000000 qufit-1.0.7/qufit/__init__.py
--rw-rw-rw-   0        0        0    26204 2023-04-06 10:36:53.000000 qufit-1.0.7/qufit/dataTools.py
--rw-rw-rw-   0        0        0     3907 2022-09-21 03:02:11.000000 qufit-1.0.7/qufit/opt.py
--rw-rw-rw-   0        0        0    59935 2023-04-14 07:09:30.000000 qufit-1.0.7/qufit/optimize.py
-drwxrwxrwx   0        0        0        0 2023-04-14 07:10:49.942357 qufit-1.0.7/qufit.egg-info/
--rw-rw-rw-   0        0        0      820 2023-04-14 07:10:49.000000 qufit-1.0.7/qufit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-04-14 07:10:49.000000 qufit-1.0.7/qufit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 07:10:49.000000 qufit-1.0.7/qufit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-14 07:10:49.000000 qufit-1.0.7/qufit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 07:10:49.946347 qufit-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      707 2023-04-14 07:10:03.000000 qufit-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 06:32:59.945465 qufit-1.0.8/
+-rw-rw-rw-   0        0        0      820 2023-04-24 06:32:59.944469 qufit-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2022-11-06 13:08:56.000000 qufit-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 06:32:59.927513 qufit-1.0.8/qufit/
+-rw-rw-rw-   0        0        0       16 2022-11-06 12:49:07.000000 qufit-1.0.8/qufit/__init__.py
+-rw-rw-rw-   0        0        0    26204 2023-04-06 10:36:53.000000 qufit-1.0.8/qufit/dataTools.py
+-rw-rw-rw-   0        0        0     3907 2022-09-21 03:02:11.000000 qufit-1.0.8/qufit/opt.py
+-rw-rw-rw-   0        0        0    59937 2023-04-24 06:30:42.000000 qufit-1.0.8/qufit/optimize.py
+drwxrwxrwx   0        0        0        0 2023-04-24 06:32:59.943474 qufit-1.0.8/qufit.egg-info/
+-rw-rw-rw-   0        0        0      820 2023-04-24 06:32:59.000000 qufit-1.0.8/qufit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-04-24 06:32:59.000000 qufit-1.0.8/qufit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 06:32:59.000000 qufit-1.0.8/qufit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-24 06:32:59.000000 qufit-1.0.8/qufit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 06:32:59.945465 qufit-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      707 2023-04-24 06:32:45.000000 qufit-1.0.8/setup.py
```

### Comparing `qufit-1.0.7/PKG-INFO` & `qufit-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qufit
-Version: 1.0.7
+Version: 1.0.8
 Summary: 本模块包括了超导量子计算实验中常用模型的拟合函数于数据处理方法。
 Home-page: https://pypi.org/
 Author: 赵寿宽(sk zhao)
 Author-email: 2396776980@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `qufit-1.0.7/qufit/dataTools.py` & `qufit-1.0.8/qufit/dataTools.py`

 * *Files identical despite different names*

### Comparing `qufit-1.0.7/qufit/opt.py` & `qufit-1.0.8/qufit/opt.py`

 * *Files identical despite different names*

### Comparing `qufit-1.0.7/qufit/optimize.py` & `qufit-1.0.8/qufit/optimize.py`

 * *Files 0% similar despite different names*

```diff
@@ -823,15 +823,15 @@
     def __init__(self,responsetime=100,T1=20000,phi=np.pi/2,funcname=None,envelopemethod=None):
         T2_Fit.__init__(self,responsetime,T1,phi,funcname,envelopemethod)
         
     
     def guessRabi(self,x,y_new,y):
  
         res, _ = self.fitExp(x[5:-5],y_new[5:-5])
-        A, B, T1 = res
+        A, B, T1 = res.x
         T1 = 1 / T1
         if np.abs(self.T1-T1)>5000:
             T1 = self.T1
         Ag, Cg, Wg, phig = self.guessCos(x,y)
         return A, B, T1, Wg, phig
     
     def func_Rabi(self,x,paras):
```

### Comparing `qufit-1.0.7/qufit.egg-info/PKG-INFO` & `qufit-1.0.8/qufit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qufit
-Version: 1.0.7
+Version: 1.0.8
 Summary: 本模块包括了超导量子计算实验中常用模型的拟合函数于数据处理方法。
 Home-page: https://pypi.org/
 Author: 赵寿宽(sk zhao)
 Author-email: 2396776980@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `qufit-1.0.7/setup.py` & `qufit-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="qufit",
-    version="1.0.7",
+    version="1.0.8",
     author="赵寿宽(sk zhao)",
     author_email="2396776980@qq.com",
     description="本模块包括了超导量子计算实验中常用模型的拟合函数于数据处理方法。",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://pypi.org/",
     packages=setuptools.find_packages(),
```

