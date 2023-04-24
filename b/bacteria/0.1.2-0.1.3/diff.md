# Comparing `tmp/bacteria-0.1.2.tar.gz` & `tmp/bacteria-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bacteria-0.1.2.tar", last modified: Mon Apr 24 07:01:06 2023, max compression
+gzip compressed data, was "bacteria-0.1.3.tar", last modified: Mon Apr 24 18:27:45 2023, max compression
```

## Comparing `bacteria-0.1.2.tar` & `bacteria-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 07:01:06.890000 bacteria-0.1.2/
--rw-rw-rw-   0        0        0      593 2023-04-24 07:01:06.750000 bacteria-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1057 2023-04-21 18:30:09.000000 bacteria-0.1.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-24 07:01:06.383000 bacteria-0.1.2/bacteria/
--rw-rw-rw-   0        0        0       67 2023-04-23 10:02:48.000000 bacteria-0.1.2/bacteria/__init__.py
--rw-rw-rw-   0        0        0   147781 2023-04-24 06:55:12.000000 bacteria-0.1.2/bacteria/functions.py
--rw-rw-rw-   0        0        0    16748 2023-04-21 12:24:44.000000 bacteria-0.1.2/bacteria/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-04-24 07:01:06.724000 bacteria-0.1.2/bacteria.egg-info/
--rw-rw-rw-   0        0        0      593 2023-04-24 07:01:05.000000 bacteria-0.1.2/bacteria.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-04-24 07:01:05.000000 bacteria-0.1.2/bacteria.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 07:01:05.000000 bacteria-0.1.2/bacteria.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-04-24 07:01:05.000000 bacteria-0.1.2/bacteria.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-24 07:01:05.000000 bacteria-0.1.2/bacteria.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 07:01:06.856000 bacteria-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1107 2023-04-24 06:59:22.000000 bacteria-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 18:27:45.385000 bacteria-0.1.3/
+-rw-rw-rw-   0        0        0      593 2023-04-24 18:27:45.241000 bacteria-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1057 2023-04-21 18:30:09.000000 bacteria-0.1.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-24 18:27:44.770000 bacteria-0.1.3/bacteria/
+-rw-rw-rw-   0        0        0       67 2023-04-23 10:02:48.000000 bacteria-0.1.3/bacteria/__init__.py
+-rw-rw-rw-   0        0        0   148163 2023-04-24 18:27:11.000000 bacteria-0.1.3/bacteria/functions.py
+-rw-rw-rw-   0        0        0    16748 2023-04-21 12:24:44.000000 bacteria-0.1.3/bacteria/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-04-24 18:27:45.214000 bacteria-0.1.3/bacteria.egg-info/
+-rw-rw-rw-   0        0        0      593 2023-04-24 18:27:43.000000 bacteria-0.1.3/bacteria.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-04-24 18:27:43.000000 bacteria-0.1.3/bacteria.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 18:27:43.000000 bacteria-0.1.3/bacteria.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-04-24 18:27:43.000000 bacteria-0.1.3/bacteria.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-24 18:27:43.000000 bacteria-0.1.3/bacteria.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 18:27:45.355000 bacteria-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1107 2023-04-24 18:14:54.000000 bacteria-0.1.3/setup.py
```

### Comparing `bacteria-0.1.2/PKG-INFO` & `bacteria-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacteria
-Version: 0.1.2
+Version: 0.1.3
 Summary: Super Segger Analysis in Python.
 Home-page: https://bacteria.readthedocs.io
 License: MIT
 Download-URL: https://github.com/tuliofalmeida/bacteria
 Keywords: Data analysis,Cell analysis,Bacteria,SuperSegger
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bacteria-0.1.2/README.rst` & `bacteria-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `bacteria-0.1.2/bacteria/functions.py` & `bacteria-0.1.3/bacteria/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import scipy.io
 # import matlab.engine
 import numpy as np
 import pandas as pd
 import seaborn as sns
 import matplotlib.pyplot as plt
 # from IPython import display
+from tqdm import tqdm
 from scipy.stats import sem
 from natsort import natsorted # pip install natsort
 from datetime import date,timedelta
 from matplotlib.lines import Line2D
 from sklearn import preprocessing as pre
 from sklearn.linear_model import LinearRegression
 from scipy.signal import savgol_filter, argrelextrema
@@ -1398,33 +1399,26 @@
         DataFrame with the deravtives data alongside with 
         the time and volume 
     dict_derivative : dict
         A dict with other dicts that contains the 
         [volume,fluor,time,F/V and all derivatives] 
         of each cell at the slide window (cell number = key).
     """
-    # import sys
-    # if 'tqdm' in sys.modules:
-    #     print()
-    #     from tqdm.notebook import tqdm
-    # else:
-    #     bar = False
     if column == 'Volume':
         df_dev = pd.melt(df_3d, id_vars=['Cell ID','Time (fps)','F/V'], value_vars=[column]).sort_values(by=['Cell ID','Time (fps)'])
     else:
         df_dev = pd.melt(df_3d, id_vars=['Cell ID','Time (fps)','F/V','Volume'], value_vars=[column]).sort_values(by=['Cell ID','Time (fps)'])
 
     dict_derivative,vol_dict,time_dict,bin_dict,ratio_dict = {},{},{},{},{}
     dev_dict,dev_dict_norm,dev_dict_log,dev_dict_log_norm = {},{},{},{}
 
     cells = natsorted(set(df_dev['Cell ID']))
     count = 0
 
     if bar:
-        from tqdm.notebook import tqdm
         for idx in tqdm(range(len(cells))):
             cell = cells[count]
             count += 1
             time_frames = df_dev[(df_dev['Cell ID'] == cell) & (df_dev['Time (fps)'])]['Time (fps)'].values
             vol,deriv,deriv_log,deriv_norm,deriv_log_norm,time,ratio = [],[],[],[],[],[],[]
             model_deriv = LinearRegression()
             model_deriv_log = LinearRegression()
@@ -3206,15 +3200,19 @@
     size_birth,size_birth_pre,size_birth_pos = [],[],[]
     vol_dict['order']['pre'],vol_dict['order']['pos'] = pre,pos
     if adjust:
         for_range = 9
     else:
         for_range = 2
 
-    for cell in natsorted(df_2d['Cell ID'].values):
+    cells = natsorted(df_2d['Cell ID'].values)
+    count = 0
+    for idx in tqdm(range(len(cells))):
+        cell = cells[count]
+        count +=1
         temp_order = order
         daughter_cell1 = df_2d[df_2d['Cell ID']==cell]['Daughter1 ID'].values[0]
         daughter_cell2 = df_2d[df_2d['Cell ID']==cell]['Daughter2 ID'].values[0]
         
         if len(df_3d[df_3d['Cell ID']==daughter_cell1]) > 0:
             for attempt in range(for_range):
                 try:            
@@ -3277,15 +3275,15 @@
 
     vol_dict['all']['diff'],vol_dict['all']['min'],vol_dict['all']['birth'] = volume_diff,volume_minima,size_birth
     vol_dict['pre']['diff'],vol_dict['pre']['min'],vol_dict['pre']['birth'] = volume_diff_pre,volume_minima_pre,size_birth_pre
     vol_dict['pos']['diff'],vol_dict['pos']['min'],vol_dict['pos']['birth'] = volume_diff_pos,volume_minima_pos,size_birth_pos
 
     return vol_dict
 
-def plot_diff_minima(vol_dict,key = None, ax = None):
+def plot_diff_minima(vol_dict,key = None, color = None,color_pre= 'black', color_pos = 'red',ax = None):
     """
     Function to plot the difference between the minimas.
     The function will plot the 'pre' and 'pos' moments
     automatically if present in the dictionary. Also,
     plot the histogram of the diff. It's possible to 
     choose the key to plot ('all','pre' or 'pos'), if
     you pass just the key will plot the cloud and the
@@ -3299,14 +3297,23 @@
     --------------
     vol_dict : dict
         Dict with the values of the diff minima, output
         of 'diff_minima()'.
     key : str (optional)
         key used to plot just one moment, 'all', 'pre'
         or 'por'
+    color : str (optional)
+        color to plot the cloud and the histogram of 
+        'all' data
+    color_pre : str (optional)
+        color to plot the cloud and the histogram of 
+        'pre' data
+    color_pos : str (optional)
+        color to plot the cloud and the histogram of 
+        'pos' data
     ax : nd.array (optional)
         the ax position to plot
 
     Returns
     --------------
     None
     """
@@ -3332,15 +3339,15 @@
             if key == 'all':
                 ax[1].set_title('{} the time'.format(key.capitalize()),fontsize = 17)
             else:
                 ax[1].set_title('{} {} min'.format(key.capitalize(),vol_dict['order'][key]),fontsize = 17)
             ax[1].set_xlabel(r'Daughter Vm - Mother Vm [$\mu m^3$]',fontsize = 15)
         else:
             out = []
-            out.append(ax.plot(vol_dict[key]['min'],vol_dict[key]['diff'],'.'))
+            out.append(ax.plot(vol_dict[key]['min'],vol_dict[key]['diff'],'.'),color= color)
             out.append(ax.plot(vol_dict[key]['min'],model.predict(np.asarray(vol_dict[key]['min']).reshape(len(vol_dict[key]['min']), 1)),
                         'gray',label = 'Coef: ' + str(model.coef_[0])[:5]))
             out.append(ax.set_title('{} the time'.format(key.capitalize()),fontsize = 17))
             out.append(ax.set_xlabel(r'Volume minima [$\mu m^3$]',fontsize = 15))
             out.append(ax.set_ylabel(r'Daughter Vm - Mother Vm [$\mu m^3$]',fontsize = 15))
             out.append(ax.set_ylim(0,5))
             out.append(ax.set_xlim(.5,5.5))
@@ -3350,89 +3357,89 @@
     else:	
         if len(vol_dict['pre']['diff']) < 2 or len(vol_dict['pos']['diff']) < 2:
             fig,ax = plt.subplots(1,2, figsize = (13,5))
             model = LinearRegression()
             model.fit(np.asarray(vol_dict['all']['min']).reshape(len(vol_dict['all']['min']), 1),
                     np.asarray(vol_dict['all']['diff']).reshape(len(vol_dict['all']['diff'])))
 
-            ax[0].plot(vol_dict['all']['min'],vol_dict['all']['diff'],'.')
+            ax[0].plot(vol_dict['all']['min'],vol_dict['all']['diff'],'.',color = color)
             ax[0].plot(vol_dict['all']['min'],model.predict(np.asarray(vol_dict['all']['min']).reshape(len(vol_dict['all']['min']), 1)),
                     'gray',label = 'Coef: ' + str(model.coef_[0])[:5])
             ax[0].set_title('All the time',fontsize = 17)
             ax[0].set_xlabel(r'Volume minima [$\mu m^3$]',fontsize = 15)
             ax[0].set_ylabel(r'Daughter Vm - Mother Vm [$\mu m^3$]',fontsize = 15)
             ax[0].set_ylim(0,5)
             ax[0].set_xlim(.5,5.5)
             ax[0].legend()
             
-            ax[1].hist(vol_dict['all']['diff'])
+            ax[1].hist(vol_dict['all']['diff'],color=color)
             ax[1].set_title('All the time Histogram',fontsize = 17)
             ax[1].set_xlabel(r'Daughter Vm - Mother Vm [$\mu m^3$]',fontsize = 15)	 
         else:
             y_min,y_max = [],[]
             fig,ax = plt.subplots(2,3, figsize = (17,10))
 
             model = LinearRegression()
             model.fit(np.asarray(vol_dict['pre']['min']).reshape(len(vol_dict['pre']['min']), 1),
                     np.asarray(vol_dict['pre']['diff']).reshape(len(vol_dict['pre']['diff'])))
 
-            ax[0][0].plot(vol_dict['pre']['min'],vol_dict['pre']['diff'],'.',color = 'k')
+            ax[0][1].plot(vol_dict['pre']['min'],vol_dict['pre']['diff'],'.',color = color_pre)
             ax[0][0].plot(vol_dict['pre']['min'],model.predict(np.asarray(vol_dict['pre']['min']).reshape(len(vol_dict['pre']['min']), 1)),
                     'gray',label = 'Pre Coef: ' + str(model.coef_[0])[:5])
-            ax[0][0].set_title('Pre {} min'.format(vol_dict['order']['pre']),fontsize = 17)
-            ax[0][0].set_ylabel(r'Daughter Vm - Mother Vm [$\mu m^3$]',fontsize = 15)
-            ax[0][0].set_xlabel(r'Volume minima [$\mu m^3$]',fontsize = 15)
-            ax[0][0].set_ylim(0,5)
-            ax[0][0].set_xlim(.5,5.5)
-            ax[0][0].legend()
-
-            ax[1][0].hist(vol_dict['pre']['diff'],color = 'k')
-            ax[1][0].set_title('Pre {} Histogram'.format(vol_dict['order']['pre']),fontsize = 17)
-            ax[1][0].set_xlabel(r'Daughter Vm - Mother Vm [$\mu m^3$]',fontsize = 15)
-            y_min.append(ax[1][0].get_ylim()[0])
-            y_max.append(ax[1][0].get_ylim()[1])
-
-            model = LinearRegression()
-            model.fit(np.asarray(vol_dict['pos']['min']).reshape(len(vol_dict['pos']['min']), 1),
-                    np.asarray(vol_dict['pos']['diff']).reshape(len(vol_dict['pos']['diff'])))
-
-            ax[0][1].plot(vol_dict['pos']['min'],vol_dict['pos']['diff'],'.',color = 'red')
-            ax[0][1].plot(vol_dict['pos']['min'],model.predict(np.asarray(vol_dict['pos']['min']).reshape(len(vol_dict['pos']['min']), 1)),
-                    'gray',label = 'Pos Coef: ' + str(model.coef_[0])[:5])
-            ax[0][1].set_title('Pos {} min'.format(vol_dict['order']['pos']),fontsize = 17)
+            ax[0][1].set_title('Pre {} min'.format(vol_dict['order']['pre']),fontsize = 17)
+            ax[0][1].set_ylabel(r'Daughter Vm - Mother Vm [$\mu m^3$]',fontsize = 15)
             ax[0][1].set_xlabel(r'Volume minima [$\mu m^3$]',fontsize = 15)
             ax[0][1].set_ylim(0,5)
             ax[0][1].set_xlim(.5,5.5)
             ax[0][1].legend()
 
-            ax[1][1].hist(vol_dict['pos']['diff'],color = 'red')
-            ax[1][1].set_title('Pos {} Histogram'.format(vol_dict['order']['pos']),fontsize = 17)
+            ax[1][1].hist(vol_dict['pre']['diff'],color = color_pre)
+            ax[1][1].set_title('Pre {} Histogram'.format(vol_dict['order']['pre']),fontsize = 17)
             ax[1][1].set_xlabel(r'Daughter Vm - Mother Vm [$\mu m^3$]',fontsize = 15)
             y_min.append(ax[1][1].get_ylim()[0])
             y_max.append(ax[1][1].get_ylim()[1])
 
             model = LinearRegression()
-            model.fit(np.asarray(vol_dict['all']['min']).reshape(len(vol_dict['all']['min']), 1),
-                    np.asarray(vol_dict['all']['diff']).reshape(len(vol_dict['all']['diff'])))
+            model.fit(np.asarray(vol_dict['pos']['min']).reshape(len(vol_dict['pos']['min']), 1),
+                    np.asarray(vol_dict['pos']['diff']).reshape(len(vol_dict['pos']['diff'])))
 
-            ax[0][2].plot(vol_dict['all']['min'],vol_dict['all']['diff'],'.')
-            ax[0][2].plot(vol_dict['all']['min'],model.predict(np.asarray(vol_dict['all']['min']).reshape(len(vol_dict['all']['min']), 1)),
-                    'gray',label = 'Coef: ' + str(model.coef_[0])[:5])
-            ax[0][2].set_title('All the time',fontsize = 17)
+            ax[0][2].plot(vol_dict['pos']['min'],vol_dict['pos']['diff'],'.',color = color_pos)
+            ax[0][2].plot(vol_dict['pos']['min'],model.predict(np.asarray(vol_dict['pos']['min']).reshape(len(vol_dict['pos']['min']), 1)),
+                    'gray',label = 'Pos Coef: ' + str(model.coef_[0])[:5])
+            ax[0][2].set_title('Pos {} min'.format(vol_dict['order']['pos']),fontsize = 17)
             ax[0][2].set_xlabel(r'Volume minima [$\mu m^3$]',fontsize = 15)
             ax[0][2].set_ylim(0,5)
             ax[0][2].set_xlim(.5,5.5)
             ax[0][2].legend()
 
-            ax[1][2].hist(vol_dict['all']['diff'])
-            ax[1][2].set_title('All the time Histogram',fontsize = 17)
+            ax[1][2].hist(vol_dict['pos']['diff'],color = color_pre)
+            ax[1][2].set_title('Pos {} Histogram'.format(vol_dict['order']['pos']),fontsize = 17)
             ax[1][2].set_xlabel(r'Daughter Vm - Mother Vm [$\mu m^3$]',fontsize = 15)
             y_min.append(ax[1][2].get_ylim()[0])
             y_max.append(ax[1][2].get_ylim()[1])
 
+            model = LinearRegression()
+            model.fit(np.asarray(vol_dict['all']['min']).reshape(len(vol_dict['all']['min']), 1),
+                    np.asarray(vol_dict['all']['diff']).reshape(len(vol_dict['all']['diff'])))
+
+            ax[0][0].plot(vol_dict['all']['min'],vol_dict['all']['diff'],'.',color = color)
+            ax[0][0].plot(vol_dict['all']['min'],model.predict(np.asarray(vol_dict['all']['min']).reshape(len(vol_dict['all']['min']), 1)),
+                    'gray',label = 'Coef: ' + str(model.coef_[0])[:5])
+            ax[0][0].set_title('All the time',fontsize = 17)
+            ax[0][0].set_xlabel(r'Volume minima [$\mu m^3$]',fontsize = 15)
+            ax[0][0].set_ylim(0,5)
+            ax[0][0].set_xlim(.5,5.5)
+            ax[0][0].legend()
+
+            ax[1][0].hist(vol_dict['all']['diff'],color = color)
+            ax[1][0].set_title('All the time Histogram',fontsize = 17)
+            ax[1][0].set_xlabel(r'Daughter Vm - Mother Vm [$\mu m^3$]',fontsize = 15)
+            y_min.append(ax[1][0].get_ylim()[0])
+            y_max.append(ax[1][0].get_ylim()[1])
+
             ax[1][0].set_ylim(min(y_min),max(y_max)+100)
             ax[1][1].set_ylim(min(y_min),max(y_max)+100)
             ax[1][2].set_ylim(min(y_min),max(y_max)+100)
             ax[1][0].set_xlim(0,5.5)
             ax[1][1].set_xlim(0,5.5)
             ax[1][2].set_xlim(0,5.5)
```

### Comparing `bacteria-0.1.2/bacteria/pipeline.py` & `bacteria-0.1.3/bacteria/pipeline.py`

 * *Files identical despite different names*

### Comparing `bacteria-0.1.2/bacteria.egg-info/PKG-INFO` & `bacteria-0.1.3/bacteria.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacteria
-Version: 0.1.2
+Version: 0.1.3
 Summary: Super Segger Analysis in Python.
 Home-page: https://bacteria.readthedocs.io
 License: MIT
 Download-URL: https://github.com/tuliofalmeida/bacteria
 Keywords: Data analysis,Cell analysis,Bacteria,SuperSegger
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bacteria-0.1.2/setup.py` & `bacteria-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
  
 with open("README.rst", "r") as fh:
     long_description = fh.read()
   
 setuptools.setup(
     name = 'bacteria',         
     packages = ['bacteria'],   
-    version = '0.1.2',      
+    version = '0.1.3',      
     license='MIT',       
     description = 'Super Segger Analysis in Python.',
     long_description_content_type="text/x-rst",
     url = 'https://bacteria.readthedocs.io',  
     download_url = 'https://github.com/tuliofalmeida/bacteria',    
     keywords = ['Data analysis', 'Cell analysis', 'Bacteria', 'SuperSegger'],   
     install_requires=[
```

