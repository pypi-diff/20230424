# Comparing `tmp/bacteria-0.1.4.tar.gz` & `tmp/bacteria-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bacteria-0.1.4.tar", last modified: Mon Apr 24 18:33:06 2023, max compression
+gzip compressed data, was "bacteria-0.1.5.tar", last modified: Mon Apr 24 19:07:53 2023, max compression
```

## Comparing `bacteria-0.1.4.tar` & `bacteria-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 18:33:06.137000 bacteria-0.1.4/
--rw-rw-rw-   0        0        0      593 2023-04-24 18:33:05.879000 bacteria-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1057 2023-04-21 18:30:09.000000 bacteria-0.1.4/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-24 18:33:05.472000 bacteria-0.1.4/bacteria/
--rw-rw-rw-   0        0        0       67 2023-04-23 10:02:48.000000 bacteria-0.1.4/bacteria/__init__.py
--rw-rw-rw-   0        0        0   148163 2023-04-24 18:27:11.000000 bacteria-0.1.4/bacteria/functions.py
--rw-rw-rw-   0        0        0    16748 2023-04-21 12:24:44.000000 bacteria-0.1.4/bacteria/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-04-24 18:33:05.822000 bacteria-0.1.4/bacteria.egg-info/
--rw-rw-rw-   0        0        0      593 2023-04-24 18:33:04.000000 bacteria-0.1.4/bacteria.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-04-24 18:33:04.000000 bacteria-0.1.4/bacteria.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 18:33:04.000000 bacteria-0.1.4/bacteria.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-04-24 18:33:04.000000 bacteria-0.1.4/bacteria.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-24 18:33:04.000000 bacteria-0.1.4/bacteria.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 18:33:06.134000 bacteria-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1128 2023-04-24 18:32:59.000000 bacteria-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 19:07:53.595000 bacteria-0.1.5/
+-rw-rw-rw-   0        0        0      593 2023-04-24 19:07:53.479000 bacteria-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1057 2023-04-21 18:30:09.000000 bacteria-0.1.5/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-24 19:07:53.082000 bacteria-0.1.5/bacteria/
+-rw-rw-rw-   0        0        0       67 2023-04-23 10:02:48.000000 bacteria-0.1.5/bacteria/__init__.py
+-rw-rw-rw-   0        0        0   148163 2023-04-24 19:07:40.000000 bacteria-0.1.5/bacteria/functions.py
+-rw-rw-rw-   0        0        0    16748 2023-04-21 12:24:44.000000 bacteria-0.1.5/bacteria/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-04-24 19:07:53.439000 bacteria-0.1.5/bacteria.egg-info/
+-rw-rw-rw-   0        0        0      593 2023-04-24 19:07:52.000000 bacteria-0.1.5/bacteria.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-04-24 19:07:52.000000 bacteria-0.1.5/bacteria.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 19:07:52.000000 bacteria-0.1.5/bacteria.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-04-24 19:07:52.000000 bacteria-0.1.5/bacteria.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-24 19:07:52.000000 bacteria-0.1.5/bacteria.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 19:07:53.563000 bacteria-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1128 2023-04-24 19:07:47.000000 bacteria-0.1.5/setup.py
```

### Comparing `bacteria-0.1.4/PKG-INFO` & `bacteria-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacteria
-Version: 0.1.4
+Version: 0.1.5
 Summary: Super Segger Analysis in Python.
 Home-page: https://bacteria.readthedocs.io
 License: MIT
 Download-URL: https://github.com/tuliofalmeida/bacteria
 Keywords: Data analysis,Cell analysis,Bacteria,SuperSegger
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bacteria-0.1.4/README.rst` & `bacteria-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `bacteria-0.1.4/bacteria/functions.py` & `bacteria-0.1.5/bacteria/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -3379,15 +3379,15 @@
             fig,ax = plt.subplots(2,3, figsize = (17,10))
 
             model = LinearRegression()
             model.fit(np.asarray(vol_dict['pre']['min']).reshape(len(vol_dict['pre']['min']), 1),
                     np.asarray(vol_dict['pre']['diff']).reshape(len(vol_dict['pre']['diff'])))
 
             ax[0][1].plot(vol_dict['pre']['min'],vol_dict['pre']['diff'],'.',color = color_pre)
-            ax[0][0].plot(vol_dict['pre']['min'],model.predict(np.asarray(vol_dict['pre']['min']).reshape(len(vol_dict['pre']['min']), 1)),
+            ax[0][1].plot(vol_dict['pre']['min'],model.predict(np.asarray(vol_dict['pre']['min']).reshape(len(vol_dict['pre']['min']), 1)),
                     'gray',label = 'Pre Coef: ' + str(model.coef_[0])[:5])
             ax[0][1].set_title('Pre {} min'.format(vol_dict['order']['pre']),fontsize = 17)
             ax[0][1].set_ylabel(r'Daughter Vm - Mother Vm [$\mu m^3$]',fontsize = 15)
             ax[0][1].set_xlabel(r'Volume minima [$\mu m^3$]',fontsize = 15)
             ax[0][1].set_ylim(0,5)
             ax[0][1].set_xlim(.5,5.5)
             ax[0][1].legend()
@@ -3407,15 +3407,15 @@
                     'gray',label = 'Pos Coef: ' + str(model.coef_[0])[:5])
             ax[0][2].set_title('Pos {} min'.format(vol_dict['order']['pos']),fontsize = 17)
             ax[0][2].set_xlabel(r'Volume minima [$\mu m^3$]',fontsize = 15)
             ax[0][2].set_ylim(0,5)
             ax[0][2].set_xlim(.5,5.5)
             ax[0][2].legend()
 
-            ax[1][2].hist(vol_dict['pos']['diff'],color = color_pre)
+            ax[1][2].hist(vol_dict['pos']['diff'],color = color_pos)
             ax[1][2].set_title('Pos {} Histogram'.format(vol_dict['order']['pos']),fontsize = 17)
             ax[1][2].set_xlabel(r'Daughter Vm - Mother Vm [$\mu m^3$]',fontsize = 15)
             y_min.append(ax[1][2].get_ylim()[0])
             y_max.append(ax[1][2].get_ylim()[1])
 
             model = LinearRegression()
             model.fit(np.asarray(vol_dict['all']['min']).reshape(len(vol_dict['all']['min']), 1),
```

### Comparing `bacteria-0.1.4/bacteria/pipeline.py` & `bacteria-0.1.5/bacteria/pipeline.py`

 * *Files identical despite different names*

### Comparing `bacteria-0.1.4/bacteria.egg-info/PKG-INFO` & `bacteria-0.1.5/bacteria.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacteria
-Version: 0.1.4
+Version: 0.1.5
 Summary: Super Segger Analysis in Python.
 Home-page: https://bacteria.readthedocs.io
 License: MIT
 Download-URL: https://github.com/tuliofalmeida/bacteria
 Keywords: Data analysis,Cell analysis,Bacteria,SuperSegger
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bacteria-0.1.4/setup.py` & `bacteria-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
  
 with open("README.rst", "r") as fh:
     long_description = fh.read()
   
 setuptools.setup(
     name = 'bacteria',         
     packages = ['bacteria'],   
-    version = '0.1.4',      
+    version = '0.1.5',      
     license='MIT',       
     description = 'Super Segger Analysis in Python.',
     long_description_content_type="text/x-rst",
     url = 'https://bacteria.readthedocs.io',  
     download_url = 'https://github.com/tuliofalmeida/bacteria',    
     keywords = ['Data analysis', 'Cell analysis', 'Bacteria', 'SuperSegger'],   
     install_requires=[
```

