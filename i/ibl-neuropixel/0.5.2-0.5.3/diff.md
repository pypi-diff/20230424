# Comparing `tmp/ibl-neuropixel-0.5.2.tar.gz` & `tmp/ibl-neuropixel-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibl-neuropixel-0.5.2.tar", last modified: Wed Apr 19 13:58:46 2023, max compression
+gzip compressed data, was "ibl-neuropixel-0.5.3.tar", last modified: Mon Apr 24 09:36:49 2023, max compression
```

## Comparing `ibl-neuropixel-0.5.2.tar` & `ibl-neuropixel-0.5.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 13:58:46.803216 ibl-neuropixel-0.5.2/
--rw-rw-rw-   0        0        0     1087 2022-05-11 13:53:32.000000 ibl-neuropixel-0.5.2/LICENSE
--rw-rw-rw-   0        0        0       25 2022-05-11 13:53:32.000000 ibl-neuropixel-0.5.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2015 2023-04-19 13:58:46.802216 ibl-neuropixel-0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     1369 2022-05-11 13:53:32.000000 ibl-neuropixel-0.5.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-19 13:58:46.803216 ibl-neuropixel-0.5.2/setup.cfg
--rw-rw-rw-   0        0        0     1072 2023-04-19 13:55:37.000000 ibl-neuropixel-0.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-19 13:58:46.785216 ibl-neuropixel-0.5.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-19 13:58:46.790216 ibl-neuropixel-0.5.2/src/ibl_neuropixel.egg-info/
--rw-rw-rw-   0        0        0     2015 2023-04-19 13:58:46.000000 ibl-neuropixel-0.5.2/src/ibl_neuropixel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      531 2023-04-19 13:58:46.000000 ibl-neuropixel-0.5.2/src/ibl_neuropixel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 13:58:46.000000 ibl-neuropixel-0.5.2/src/ibl_neuropixel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-04-19 13:58:46.000000 ibl-neuropixel-0.5.2/src/ibl_neuropixel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-04-19 13:58:46.000000 ibl-neuropixel-0.5.2/src/ibl_neuropixel.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-19 13:58:46.801216 ibl-neuropixel-0.5.2/src/neurodsp/
--rw-rw-rw-   0        0        0        0 2022-05-11 13:53:32.000000 ibl-neuropixel-0.5.2/src/neurodsp/__init__.py
--rw-rw-rw-   0        0        0     6071 2023-04-19 09:09:00.000000 ibl-neuropixel-0.5.2/src/neurodsp/cadzow.py
--rw-rw-rw-   0        0        0     2371 2022-05-11 13:53:32.000000 ibl-neuropixel-0.5.2/src/neurodsp/cuda_tools.py
--rw-rw-rw-   0        0        0     2763 2022-05-11 13:53:32.000000 ibl-neuropixel-0.5.2/src/neurodsp/destripe_gpu.py
--rw-rw-rw-   0        0        0     5838 2022-05-11 13:53:32.000000 ibl-neuropixel-0.5.2/src/neurodsp/filter_gpu.py
--rw-rw-rw-   0        0        0    10529 2022-05-11 13:53:32.000000 ibl-neuropixel-0.5.2/src/neurodsp/fourier.py
--rw-rw-rw-   0        0        0     7947 2022-05-11 13:53:32.000000 ibl-neuropixel-0.5.2/src/neurodsp/smooth.py
--rw-rw-rw-   0        0        0     8976 2023-04-19 09:09:00.000000 ibl-neuropixel-0.5.2/src/neurodsp/utils.py
--rw-rw-rw-   0        0        0    33238 2023-04-19 09:09:00.000000 ibl-neuropixel-0.5.2/src/neurodsp/voltage.py
--rw-rw-rw-   0        0        0     4658 2023-04-19 09:09:00.000000 ibl-neuropixel-0.5.2/src/neurodsp/waveforms.py
--rw-rw-rw-   0        0        0    35321 2023-04-19 13:55:37.000000 ibl-neuropixel-0.5.2/src/neuropixel.py
--rw-rw-rw-   0        0        0    33747 2023-04-19 13:56:50.000000 ibl-neuropixel-0.5.2/src/spikeglx.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:36:49.742417 ibl-neuropixel-0.5.3/
+-rw-rw-rw-   0        0        0     1087 2022-05-11 13:53:32.000000 ibl-neuropixel-0.5.3/LICENSE
+-rw-rw-rw-   0        0        0       25 2022-05-11 13:53:32.000000 ibl-neuropixel-0.5.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2015 2023-04-24 09:36:49.741416 ibl-neuropixel-0.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1369 2022-05-11 13:53:32.000000 ibl-neuropixel-0.5.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-24 09:36:49.742417 ibl-neuropixel-0.5.3/setup.cfg
+-rw-rw-rw-   0        0        0     1072 2023-04-24 09:35:44.000000 ibl-neuropixel-0.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:36:49.708415 ibl-neuropixel-0.5.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-24 09:36:49.717416 ibl-neuropixel-0.5.3/src/ibl_neuropixel.egg-info/
+-rw-rw-rw-   0        0        0     2015 2023-04-24 09:36:49.000000 ibl-neuropixel-0.5.3/src/ibl_neuropixel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      531 2023-04-24 09:36:49.000000 ibl-neuropixel-0.5.3/src/ibl_neuropixel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 09:36:49.000000 ibl-neuropixel-0.5.3/src/ibl_neuropixel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-04-24 09:36:49.000000 ibl-neuropixel-0.5.3/src/ibl_neuropixel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-04-24 09:36:49.000000 ibl-neuropixel-0.5.3/src/ibl_neuropixel.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 09:36:49.739416 ibl-neuropixel-0.5.3/src/neurodsp/
+-rw-rw-rw-   0        0        0        0 2022-05-11 13:53:32.000000 ibl-neuropixel-0.5.3/src/neurodsp/__init__.py
+-rw-rw-rw-   0        0        0     6071 2023-04-24 09:18:28.000000 ibl-neuropixel-0.5.3/src/neurodsp/cadzow.py
+-rw-rw-rw-   0        0        0     2371 2022-05-11 13:53:32.000000 ibl-neuropixel-0.5.3/src/neurodsp/cuda_tools.py
+-rw-rw-rw-   0        0        0     2763 2022-05-11 13:53:32.000000 ibl-neuropixel-0.5.3/src/neurodsp/destripe_gpu.py
+-rw-rw-rw-   0        0        0     5838 2022-05-11 13:53:32.000000 ibl-neuropixel-0.5.3/src/neurodsp/filter_gpu.py
+-rw-rw-rw-   0        0        0    10529 2022-05-11 13:53:32.000000 ibl-neuropixel-0.5.3/src/neurodsp/fourier.py
+-rw-rw-rw-   0        0        0     7947 2022-05-11 13:53:32.000000 ibl-neuropixel-0.5.3/src/neurodsp/smooth.py
+-rw-rw-rw-   0        0        0     8976 2023-04-19 09:09:00.000000 ibl-neuropixel-0.5.3/src/neurodsp/utils.py
+-rw-rw-rw-   0        0        0    33238 2023-04-24 09:18:28.000000 ibl-neuropixel-0.5.3/src/neurodsp/voltage.py
+-rw-rw-rw-   0        0        0     4658 2023-04-24 09:18:28.000000 ibl-neuropixel-0.5.3/src/neurodsp/waveforms.py
+-rw-rw-rw-   0        0        0    35321 2023-04-24 09:19:36.000000 ibl-neuropixel-0.5.3/src/neuropixel.py
+-rw-rw-rw-   0        0        0    33762 2023-04-24 09:35:44.000000 ibl-neuropixel-0.5.3/src/spikeglx.py
```

### Comparing `ibl-neuropixel-0.5.2/LICENSE` & `ibl-neuropixel-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.5.2/PKG-INFO` & `ibl-neuropixel-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibl-neuropixel
-Version: 0.5.2
+Version: 0.5.3
 Summary: Collection of tools for Neuropixel 1.0 and 2.0 probes data
 Home-page: https://github.com/int-brain-lab/ibl-neuropixel
 Author: The International Brain Laboratory
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/int-brain-lab/ibl-neuropixel/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ibl-neuropixel-0.5.2/README.md` & `ibl-neuropixel-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.5.2/setup.py` & `ibl-neuropixel-0.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     require = [x.strip() for x in f.readlines() if not x.startswith('git+')]
 
 setuptools.setup(
     name="ibl-neuropixel",
-    version="0.5.2",
+    version="0.5.3",
     author="The International Brain Laboratory",
     description="Collection of tools for Neuropixel 1.0 and 2.0 probes data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/int-brain-lab/ibl-neuropixel",
     project_urls={
         "Bug Tracker": "https://github.com/int-brain-lab/ibl-neuropixel/issues",
```

### Comparing `ibl-neuropixel-0.5.2/src/ibl_neuropixel.egg-info/PKG-INFO` & `ibl-neuropixel-0.5.3/src/ibl_neuropixel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibl-neuropixel
-Version: 0.5.2
+Version: 0.5.3
 Summary: Collection of tools for Neuropixel 1.0 and 2.0 probes data
 Home-page: https://github.com/int-brain-lab/ibl-neuropixel
 Author: The International Brain Laboratory
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/int-brain-lab/ibl-neuropixel/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ibl-neuropixel-0.5.2/src/ibl_neuropixel.egg-info/SOURCES.txt` & `ibl-neuropixel-0.5.3/src/ibl_neuropixel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.5.2/src/neurodsp/cadzow.py` & `ibl-neuropixel-0.5.3/src/neurodsp/cadzow.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.5.2/src/neurodsp/cuda_tools.py` & `ibl-neuropixel-0.5.3/src/neurodsp/cuda_tools.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.5.2/src/neurodsp/destripe_gpu.py` & `ibl-neuropixel-0.5.3/src/neurodsp/destripe_gpu.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.5.2/src/neurodsp/filter_gpu.py` & `ibl-neuropixel-0.5.3/src/neurodsp/filter_gpu.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.5.2/src/neurodsp/fourier.py` & `ibl-neuropixel-0.5.3/src/neurodsp/fourier.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.5.2/src/neurodsp/smooth.py` & `ibl-neuropixel-0.5.3/src/neurodsp/smooth.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.5.2/src/neurodsp/utils.py` & `ibl-neuropixel-0.5.3/src/neurodsp/utils.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.5.2/src/neurodsp/voltage.py` & `ibl-neuropixel-0.5.3/src/neurodsp/voltage.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.5.2/src/neurodsp/waveforms.py` & `ibl-neuropixel-0.5.3/src/neurodsp/waveforms.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.5.2/src/neuropixel.py` & `ibl-neuropixel-0.5.3/src/neuropixel.py`

 * *Files identical despite different names*

### Comparing `ibl-neuropixel-0.5.2/src/spikeglx.py` & `ibl-neuropixel-0.5.3/src/spikeglx.py`

 * *Files 0% similar despite different names*

```diff
@@ -573,23 +573,23 @@
     :return: dictionary of arrays 'shank', 'col', 'row', 'flag', one value per active site
     """
     if 'snsShankMap' in meta_data.keys():
         chmap = re.findall(r'([0-9]*:[0-9]*:[0-9]*:[0-9]*)', meta_data['snsShankMap'])
     elif 'snsGeomMap' in meta_data.keys():
         chmap = re.findall(r'([0-9]*:[0-9]*:[0-9]*:[0-9]*)', meta_data['snsGeomMap'])
     else:
-        chmap = None
+        return None
     # for digital nidq types, the key exists but does not contain any information
     if not chmap:
         return {'shank': None, 'col': None, 'row': None, 'flag': None}
     # shank#, col#, row#, drawflag
     # (nb: drawflag is one should be drawn and considered spatial average)
     chmap = np.array([np.float32(cm.split(':')) for cm in chmap])
     return {k: chmap[:, v] for (k, v) in {'shank': 0, 'col': 1, 'row': 2, 'flag': 3}.items()}
-
+                
 
 def _conversion_sample2v_from_meta(meta_data):
     """
     Interpret the meta data to extract an array of conversion factors for each channel
     so the output data is in Volts
     Conversion factor is: int2volt / channelGain
     For Lf/Ap interpret the gain string from metadata
```

