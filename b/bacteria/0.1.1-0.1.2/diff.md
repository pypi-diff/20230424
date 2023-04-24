# Comparing `tmp/bacteria-0.1.1.tar.gz` & `tmp/bacteria-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bacteria-0.1.1.tar", last modified: Sun Apr 23 13:19:08 2023, max compression
+gzip compressed data, was "bacteria-0.1.2.tar", last modified: Mon Apr 24 07:01:06 2023, max compression
```

## Comparing `bacteria-0.1.1.tar` & `bacteria-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 13:19:08.626000 bacteria-0.1.1/
--rw-rw-rw-   0        0        0      603 2023-04-23 13:19:08.399000 bacteria-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1057 2023-04-21 18:30:09.000000 bacteria-0.1.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-23 13:19:06.999000 bacteria-0.1.1/bacteria/
--rw-rw-rw-   0        0        0       67 2023-04-23 10:02:48.000000 bacteria-0.1.1/bacteria/__init__.py
--rw-rw-rw-   0        0        0   147713 2023-04-23 13:08:05.000000 bacteria-0.1.1/bacteria/functions.py
--rw-rw-rw-   0        0        0    16748 2023-04-21 12:24:44.000000 bacteria-0.1.1/bacteria/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-04-23 13:19:08.107000 bacteria-0.1.1/bacteria.egg-info/
--rw-rw-rw-   0        0        0      603 2023-04-23 13:19:02.000000 bacteria-0.1.1/bacteria.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-04-23 13:19:03.000000 bacteria-0.1.1/bacteria.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 13:19:02.000000 bacteria-0.1.1/bacteria.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-04-23 13:19:02.000000 bacteria-0.1.1/bacteria.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-23 13:19:03.000000 bacteria-0.1.1/bacteria.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 13:19:08.498000 bacteria-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1117 2023-04-23 13:18:26.000000 bacteria-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 07:01:06.890000 bacteria-0.1.2/
+-rw-rw-rw-   0        0        0      593 2023-04-24 07:01:06.750000 bacteria-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1057 2023-04-21 18:30:09.000000 bacteria-0.1.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-24 07:01:06.383000 bacteria-0.1.2/bacteria/
+-rw-rw-rw-   0        0        0       67 2023-04-23 10:02:48.000000 bacteria-0.1.2/bacteria/__init__.py
+-rw-rw-rw-   0        0        0   147781 2023-04-24 06:55:12.000000 bacteria-0.1.2/bacteria/functions.py
+-rw-rw-rw-   0        0        0    16748 2023-04-21 12:24:44.000000 bacteria-0.1.2/bacteria/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-04-24 07:01:06.724000 bacteria-0.1.2/bacteria.egg-info/
+-rw-rw-rw-   0        0        0      593 2023-04-24 07:01:05.000000 bacteria-0.1.2/bacteria.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-04-24 07:01:05.000000 bacteria-0.1.2/bacteria.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 07:01:05.000000 bacteria-0.1.2/bacteria.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-04-24 07:01:05.000000 bacteria-0.1.2/bacteria.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-24 07:01:05.000000 bacteria-0.1.2/bacteria.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 07:01:06.856000 bacteria-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1107 2023-04-24 06:59:22.000000 bacteria-0.1.2/setup.py
```

### Comparing `bacteria-0.1.1/PKG-INFO` & `bacteria-0.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: bacteria
-Version: 0.1.1
+Version: 0.1.2
 Summary: Super Segger Analysis in Python.
-Home-page: https://github.com/tuliofalmeida/bacteria
+Home-page: https://bacteria.readthedocs.io
 License: MIT
 Download-URL: https://github.com/tuliofalmeida/bacteria
 Keywords: Data analysis,Cell analysis,Bacteria,SuperSegger
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `bacteria-0.1.1/README.rst` & `bacteria-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `bacteria-0.1.1/bacteria/functions.py` & `bacteria-0.1.2/bacteria/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1327,15 +1327,15 @@
         Value for the higher CI (default 97.5%)
     """
     values = [np.random.choice(arr,size=len(arr),replace=True).mean() for i in range(times)] 
     ci_low,ci_high = np.percentile(values,[100*(1-conf)/2,100*(1-(1-conf)/2)])
     
     return ci_low,ci_high
 
-def progressbar(it, prefix="", size=60, out=sys.stdout):
+def _progressbar(it, prefix="", size=60, out=sys.stdout):
     """
     Binarize the data and make the mean for each bin.
     Suport function for fluor_lineage(). Bins are
     calculated based on the time data (previous reshaped
     and sclaed) using np.histogram(), default values for bins
     is 10.
     
@@ -1398,31 +1398,33 @@
         DataFrame with the deravtives data alongside with 
         the time and volume 
     dict_derivative : dict
         A dict with other dicts that contains the 
         [volume,fluor,time,F/V and all derivatives] 
         of each cell at the slide window (cell number = key).
     """
-    import sys
-    if 'tqdm' in sys.modules:
-        from tqdm.notebook import tqdm
-    else:
-        bar = False
+    # import sys
+    # if 'tqdm' in sys.modules:
+    #     print()
+    #     from tqdm.notebook import tqdm
+    # else:
+    #     bar = False
     if column == 'Volume':
         df_dev = pd.melt(df_3d, id_vars=['Cell ID','Time (fps)','F/V'], value_vars=[column]).sort_values(by=['Cell ID','Time (fps)'])
     else:
         df_dev = pd.melt(df_3d, id_vars=['Cell ID','Time (fps)','F/V','Volume'], value_vars=[column]).sort_values(by=['Cell ID','Time (fps)'])
 
     dict_derivative,vol_dict,time_dict,bin_dict,ratio_dict = {},{},{},{},{}
     dev_dict,dev_dict_norm,dev_dict_log,dev_dict_log_norm = {},{},{},{}
 
     cells = natsorted(set(df_dev['Cell ID']))
     count = 0
 
     if bar:
+        from tqdm.notebook import tqdm
         for idx in tqdm(range(len(cells))):
             cell = cells[count]
             count += 1
             time_frames = df_dev[(df_dev['Cell ID'] == cell) & (df_dev['Time (fps)'])]['Time (fps)'].values
             vol,deriv,deriv_log,deriv_norm,deriv_log_norm,time,ratio = [],[],[],[],[],[],[]
             model_deriv = LinearRegression()
             model_deriv_log = LinearRegression()
```

### Comparing `bacteria-0.1.1/bacteria/pipeline.py` & `bacteria-0.1.2/bacteria/pipeline.py`

 * *Files identical despite different names*

### Comparing `bacteria-0.1.1/bacteria.egg-info/PKG-INFO` & `bacteria-0.1.2/bacteria.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: bacteria
-Version: 0.1.1
+Version: 0.1.2
 Summary: Super Segger Analysis in Python.
-Home-page: https://github.com/tuliofalmeida/bacteria
+Home-page: https://bacteria.readthedocs.io
 License: MIT
 Download-URL: https://github.com/tuliofalmeida/bacteria
 Keywords: Data analysis,Cell analysis,Bacteria,SuperSegger
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `bacteria-0.1.1/setup.py` & `bacteria-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,19 +3,19 @@
  
 with open("README.rst", "r") as fh:
     long_description = fh.read()
   
 setuptools.setup(
     name = 'bacteria',         
     packages = ['bacteria'],   
-    version = '0.1.1',      
+    version = '0.1.2',      
     license='MIT',       
     description = 'Super Segger Analysis in Python.',
     long_description_content_type="text/x-rst",
-    url = 'https://github.com/tuliofalmeida/bacteria',  
+    url = 'https://bacteria.readthedocs.io',  
     download_url = 'https://github.com/tuliofalmeida/bacteria',    
     keywords = ['Data analysis', 'Cell analysis', 'Bacteria', 'SuperSegger'],   
     install_requires=[           
             'numpy',
             'pandas',
             'graphviz',
             'scikit-learn',
```

