# Comparing `tmp/qufit-1.0.9.tar.gz` & `tmp/qufit-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qufit-1.0.9.tar", last modified: Mon Apr 24 06:45:45 2023, max compression
+gzip compressed data, was "qufit-1.1.0.tar", last modified: Mon Apr 24 07:04:53 2023, max compression
```

## Comparing `qufit-1.0.9.tar` & `qufit-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 06:45:45.892416 qufit-1.0.9/
--rw-rw-rw-   0        0        0      820 2023-04-24 06:45:45.892416 qufit-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      331 2022-11-06 13:08:56.000000 qufit-1.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 06:45:45.874254 qufit-1.0.9/qufit/
--rw-rw-rw-   0        0        0       16 2022-11-06 12:49:07.000000 qufit-1.0.9/qufit/__init__.py
--rw-rw-rw-   0        0        0    26204 2023-04-06 10:36:53.000000 qufit-1.0.9/qufit/dataTools.py
--rw-rw-rw-   0        0        0     3907 2022-09-21 03:02:11.000000 qufit-1.0.9/qufit/opt.py
--rw-rw-rw-   0        0        0    59929 2023-04-24 06:45:20.000000 qufit-1.0.9/qufit/optimize.py
-drwxrwxrwx   0        0        0        0 2023-04-24 06:45:45.890418 qufit-1.0.9/qufit.egg-info/
--rw-rw-rw-   0        0        0      820 2023-04-24 06:45:45.000000 qufit-1.0.9/qufit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-04-24 06:45:45.000000 qufit-1.0.9/qufit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 06:45:45.000000 qufit-1.0.9/qufit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-24 06:45:45.000000 qufit-1.0.9/qufit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 06:45:45.893413 qufit-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0      707 2023-04-24 06:45:32.000000 qufit-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 07:04:53.819732 qufit-1.1.0/
+-rw-rw-rw-   0        0        0      820 2023-04-24 07:04:53.818735 qufit-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2022-11-06 13:08:56.000000 qufit-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 07:04:53.795068 qufit-1.1.0/qufit/
+-rw-rw-rw-   0        0        0       16 2022-11-06 12:49:07.000000 qufit-1.1.0/qufit/__init__.py
+-rw-rw-rw-   0        0        0    26204 2023-04-06 10:36:53.000000 qufit-1.1.0/qufit/dataTools.py
+-rw-rw-rw-   0        0        0     3907 2022-09-21 03:02:11.000000 qufit-1.1.0/qufit/opt.py
+-rw-rw-rw-   0        0        0    59941 2023-04-24 07:03:24.000000 qufit-1.1.0/qufit/optimize.py
+drwxrwxrwx   0        0        0        0 2023-04-24 07:04:53.815744 qufit-1.1.0/qufit.egg-info/
+-rw-rw-rw-   0        0        0      820 2023-04-24 07:04:53.000000 qufit-1.1.0/qufit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-04-24 07:04:53.000000 qufit-1.1.0/qufit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 07:04:53.000000 qufit-1.1.0/qufit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-24 07:04:53.000000 qufit-1.1.0/qufit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 07:04:53.819732 qufit-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      707 2023-04-24 07:04:45.000000 qufit-1.1.0/setup.py
```

### Comparing `qufit-1.0.9/PKG-INFO` & `qufit-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qufit
-Version: 1.0.9
+Version: 1.1.0
 Summary: 本模块包括了超导量子计算实验中常用模型的拟合函数于数据处理方法。
 Home-page: https://pypi.org/
 Author: 赵寿宽(sk zhao)
 Author-email: 2396776980@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `qufit-1.0.9/qufit/dataTools.py` & `qufit-1.1.0/qufit/dataTools.py`

 * *Files identical despite different names*

### Comparing `qufit-1.0.9/qufit/opt.py` & `qufit-1.1.0/qufit/opt.py`

 * *Files identical despite different names*

### Comparing `qufit-1.0.9/qufit/optimize.py` & `qufit-1.1.0/qufit/optimize.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
         index0 = np.argmin(np.abs(x-num))
         y = y - np.min(y)
         peak = peakpercent*y[index0] if insitu else peakpercent*np.max(y)
         c = np.argwhere(y>peak)
         cdiff = np.diff(c[:,0])
         n_clusters = len(np.argwhere(cdiff>np.mean(cdiff))) + 1
         S = c[:,0]
-        d = np.mat(list(zip(S,S)))
+        d = np.asarray(np.mat(list(zip(S,S))))
 
         kmeans = KMeans(n_clusters=n_clusters,max_iter=100,tol=0.001)
         yfit = kmeans.fit_predict(d)
         xaxis = S[yfit==yfit[np.argmin(np.abs(S-index0))]]
         index =  int(np.mean(xaxis)) if mean else int(xaxis[np.argmax(y[xaxis])])
         bias0 = round(x[index],5)
         return bias0 ,index
```

### Comparing `qufit-1.0.9/qufit.egg-info/PKG-INFO` & `qufit-1.1.0/qufit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qufit
-Version: 1.0.9
+Version: 1.1.0
 Summary: 本模块包括了超导量子计算实验中常用模型的拟合函数于数据处理方法。
 Home-page: https://pypi.org/
 Author: 赵寿宽(sk zhao)
 Author-email: 2396776980@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `qufit-1.0.9/setup.py` & `qufit-1.1.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="qufit",
-    version="1.0.9",
+    version="1.1.0",
     author="赵寿宽(sk zhao)",
     author_email="2396776980@qq.com",
     description="本模块包括了超导量子计算实验中常用模型的拟合函数于数据处理方法。",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://pypi.org/",
     packages=setuptools.find_packages(),
```

