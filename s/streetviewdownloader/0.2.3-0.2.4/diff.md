# Comparing `tmp/streetviewdownloader-0.2.3.tar.gz` & `tmp/streetviewdownloader-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streetviewdownloader-0.2.3.tar", last modified: Wed May 11 20:48:25 2022, max compression
+gzip compressed data, was "streetviewdownloader-0.2.4.tar", last modified: Mon Apr 24 14:16:46 2023, max compression
```

## Comparing `streetviewdownloader-0.2.3.tar` & `streetviewdownloader-0.2.4.tar`

### file list

```diff
@@ -1,35 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-11 20:48:25.164395 streetviewdownloader-0.2.3/
--rw-r--r--   0 root         (0) root         (0)     1840 2022-05-11 20:48:25.164395 streetviewdownloader-0.2.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1054 2022-05-11 20:48:00.000000 streetviewdownloader-0.2.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)       98 2022-05-11 20:48:00.000000 streetviewdownloader-0.2.3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1152 2022-05-11 20:48:25.165395 streetviewdownloader-0.2.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-11 20:48:25.154394 streetviewdownloader-0.2.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-11 20:48:25.162394 streetviewdownloader-0.2.3/src/streetviewdownloader/
--rw-rw-rw-   0 root         (0) root         (0)      621 2022-05-11 20:48:00.000000 streetviewdownloader-0.2.3/src/streetviewdownloader/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1344 2022-05-11 20:48:00.000000 streetviewdownloader-0.2.3/src/streetviewdownloader/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)      702 2022-05-11 20:48:00.000000 streetviewdownloader-0.2.3/src/streetviewdownloader/basepbfsource.py
--rw-rw-rw-   0 root         (0) root         (0)      540 2022-05-11 20:48:00.000000 streetviewdownloader-0.2.3/src/streetviewdownloader/basestreetviewdownloaderthread.py
--rw-rw-rw-   0 root         (0) root         (0)      803 2022-05-11 20:48:00.000000 streetviewdownloader-0.2.3/src/streetviewdownloader/basestreetviewsource.py
--rw-rw-rw-   0 root         (0) root         (0)     2008 2022-05-11 20:48:00.000000 streetviewdownloader-0.2.3/src/streetviewdownloader/bbbikesource.py
--rw-rw-rw-   0 root         (0) root         (0)     3611 2022-05-11 20:48:00.000000 streetviewdownloader-0.2.3/src/streetviewdownloader/cache.py
--rw-rw-rw-   0 root         (0) root         (0)     1747 2022-05-11 20:48:00.000000 streetviewdownloader-0.2.3/src/streetviewdownloader/cachingrequestssession.py
--rw-rw-rw-   0 root         (0) root         (0)     1519 2022-05-11 20:48:00.000000 streetviewdownloader-0.2.3/src/streetviewdownloader/extractfinder.py
--rw-rw-rw-   0 root         (0) root         (0)      966 2022-05-11 20:48:00.000000 streetviewdownloader-0.2.3/src/streetviewdownloader/geofabriksource.py
--rw-rw-rw-   0 root         (0) root         (0)     8846 2022-05-11 20:48:00.000000 streetviewdownloader-0.2.3/src/streetviewdownloader/pbffilereader.py
--rw-rw-rw-   0 root         (0) root         (0)     2559 2022-05-11 20:48:00.000000 streetviewdownloader-0.2.3/src/streetviewdownloader/streetnetworkdownloader.py
--rw-rw-rw-   0 root         (0) root         (0)     5160 2022-05-11 20:48:00.000000 streetviewdownloader-0.2.3/src/streetviewdownloader/streetnetworkpointgenerator.py
--rw-rw-rw-   0 root         (0) root         (0)     2922 2022-05-11 20:48:00.000000 streetviewdownloader-0.2.3/src/streetviewdownloader/streetviewdownloader.py
--rw-rw-rw-   0 root         (0) root         (0)     2349 2022-05-11 20:48:00.000000 streetviewdownloader-0.2.3/src/streetviewdownloader/streetviewimagedownloader.py
--rw-rw-rw-   0 root         (0) root         (0)     1958 2022-05-11 20:48:00.000000 streetviewdownloader-0.2.3/src/streetviewdownloader/streetviewimagedownloaderthread.py
--rw-rw-rw-   0 root         (0) root         (0)     1267 2022-05-11 20:48:00.000000 streetviewdownloader-0.2.3/src/streetviewdownloader/streetviewimagesource.py
--rw-rw-rw-   0 root         (0) root         (0)     2600 2022-05-11 20:48:00.000000 streetviewdownloader-0.2.3/src/streetviewdownloader/streetviewmetadatadownloader.py
--rw-rw-rw-   0 root         (0) root         (0)     2072 2022-05-11 20:48:00.000000 streetviewdownloader-0.2.3/src/streetviewdownloader/streetviewmetadatadownloaderthread.py
--rw-rw-rw-   0 root         (0) root         (0)     1078 2022-05-11 20:48:00.000000 streetviewdownloader-0.2.3/src/streetviewdownloader/streetviewmetadatasource.py
--rw-rw-rw-   0 root         (0) root         (0)     2042 2022-05-11 20:48:00.000000 streetviewdownloader-0.2.3/src/streetviewdownloader/streetviewstaticapiauth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-11 20:48:25.164395 streetviewdownloader-0.2.3/src/streetviewdownloader.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1840 2022-05-11 20:48:24.000000 streetviewdownloader-0.2.3/src/streetviewdownloader.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1348 2022-05-11 20:48:25.000000 streetviewdownloader-0.2.3/src/streetviewdownloader.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-11 20:48:24.000000 streetviewdownloader-0.2.3/src/streetviewdownloader.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       76 2022-05-11 20:48:24.000000 streetviewdownloader-0.2.3/src/streetviewdownloader.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       65 2022-05-11 20:48:25.000000 streetviewdownloader-0.2.3/src/streetviewdownloader.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2022-05-11 20:48:25.000000 streetviewdownloader-0.2.3/src/streetviewdownloader.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 14:16:46.533181 streetviewdownloader-0.2.4/
+-rw-r--r--   0 root         (0) root         (0)     1859 2023-04-24 14:16:46.532181 streetviewdownloader-0.2.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1054 2023-04-24 14:16:21.000000 streetviewdownloader-0.2.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-04-24 14:16:21.000000 streetviewdownloader-0.2.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 14:16:46.533181 streetviewdownloader-0.2.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 14:16:46.521180 streetviewdownloader-0.2.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 14:16:46.530181 streetviewdownloader-0.2.4/src/streetviewdownloader/
+-rw-rw-rw-   0 root         (0) root         (0)      621 2023-04-24 14:16:21.000000 streetviewdownloader-0.2.4/src/streetviewdownloader/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1344 2023-04-24 14:16:21.000000 streetviewdownloader-0.2.4/src/streetviewdownloader/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      702 2023-04-24 14:16:21.000000 streetviewdownloader-0.2.4/src/streetviewdownloader/basepbfsource.py
+-rw-rw-rw-   0 root         (0) root         (0)      540 2023-04-24 14:16:21.000000 streetviewdownloader-0.2.4/src/streetviewdownloader/basestreetviewdownloaderthread.py
+-rw-rw-rw-   0 root         (0) root         (0)      803 2023-04-24 14:16:21.000000 streetviewdownloader-0.2.4/src/streetviewdownloader/basestreetviewsource.py
+-rw-rw-rw-   0 root         (0) root         (0)     2008 2023-04-24 14:16:21.000000 streetviewdownloader-0.2.4/src/streetviewdownloader/bbbikesource.py
+-rw-rw-rw-   0 root         (0) root         (0)     3611 2023-04-24 14:16:21.000000 streetviewdownloader-0.2.4/src/streetviewdownloader/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     1747 2023-04-24 14:16:21.000000 streetviewdownloader-0.2.4/src/streetviewdownloader/cachingrequestssession.py
+-rw-rw-rw-   0 root         (0) root         (0)     1519 2023-04-24 14:16:21.000000 streetviewdownloader-0.2.4/src/streetviewdownloader/extractfinder.py
+-rw-rw-rw-   0 root         (0) root         (0)      966 2023-04-24 14:16:21.000000 streetviewdownloader-0.2.4/src/streetviewdownloader/geofabriksource.py
+-rw-rw-rw-   0 root         (0) root         (0)     8846 2023-04-24 14:16:21.000000 streetviewdownloader-0.2.4/src/streetviewdownloader/pbffilereader.py
+-rw-rw-rw-   0 root         (0) root         (0)     2559 2023-04-24 14:16:21.000000 streetviewdownloader-0.2.4/src/streetviewdownloader/streetnetworkdownloader.py
+-rw-rw-rw-   0 root         (0) root         (0)     5182 2023-04-24 14:16:21.000000 streetviewdownloader-0.2.4/src/streetviewdownloader/streetnetworkpointgenerator.py
+-rw-rw-rw-   0 root         (0) root         (0)     2922 2023-04-24 14:16:21.000000 streetviewdownloader-0.2.4/src/streetviewdownloader/streetviewdownloader.py
+-rw-rw-rw-   0 root         (0) root         (0)     2349 2023-04-24 14:16:21.000000 streetviewdownloader-0.2.4/src/streetviewdownloader/streetviewimagedownloader.py
+-rw-rw-rw-   0 root         (0) root         (0)     2032 2023-04-24 14:16:21.000000 streetviewdownloader-0.2.4/src/streetviewdownloader/streetviewimagedownloaderthread.py
+-rw-rw-rw-   0 root         (0) root         (0)     1267 2023-04-24 14:16:21.000000 streetviewdownloader-0.2.4/src/streetviewdownloader/streetviewimagesource.py
+-rw-rw-rw-   0 root         (0) root         (0)     2600 2023-04-24 14:16:21.000000 streetviewdownloader-0.2.4/src/streetviewdownloader/streetviewmetadatadownloader.py
+-rw-rw-rw-   0 root         (0) root         (0)     2072 2023-04-24 14:16:21.000000 streetviewdownloader-0.2.4/src/streetviewdownloader/streetviewmetadatadownloaderthread.py
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2023-04-24 14:16:21.000000 streetviewdownloader-0.2.4/src/streetviewdownloader/streetviewmetadatasource.py
+-rw-rw-rw-   0 root         (0) root         (0)     2042 2023-04-24 14:16:21.000000 streetviewdownloader-0.2.4/src/streetviewdownloader/streetviewstaticapiauth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 14:16:46.532181 streetviewdownloader-0.2.4/src/streetviewdownloader.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1859 2023-04-24 14:16:46.000000 streetviewdownloader-0.2.4/src/streetviewdownloader.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1287 2023-04-24 14:16:46.000000 streetviewdownloader-0.2.4/src/streetviewdownloader.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 14:16:46.000000 streetviewdownloader-0.2.4/src/streetviewdownloader.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-24 14:16:46.000000 streetviewdownloader-0.2.4/src/streetviewdownloader.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-24 14:16:46.000000 streetviewdownloader-0.2.4/src/streetviewdownloader.egg-info/top_level.txt
```

### Comparing `streetviewdownloader-0.2.3/PKG-INFO` & `streetviewdownloader-0.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: streetviewdownloader
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Python library and utility to download Google StreetView images
-Home-page: https://gitlab.com/christophfink/streetviewdownloader
-Author: Christoph Fink
-Author-email: christoph.fink@helsinki.fi
-License: GPLv3
-Project-URL: Documentation, https://streetviewdownloader.readthedocs.org/
-Project-URL: Change Log, https://gitlab.com/christophfink/streetviewdownloader/-/blob/main/CHANGELOG.md
-Project-URL: Bug Tracker, https://gitlab.com/christophfink/streetviewdownloader/-/issues
+Author-email: Christoph Fink <christoph.fink@helsinki.fi>
+License: GPL-3.0-or-later
+Project-URL: Documentation, https://streetviewdownloader.readthedocs.io/
+Project-URL: Repository, https://gitlab.com/christophfink/streetviewdownloader/
+Project-URL: Change log, https://gitlab.com/christophfink/streetviewdownloader/-/blob/main/CHANGELOG.md
+Project-URL: Bug tracker, https://gitlab.com/christophfink/streetviewdownloader/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # streetviewdownloader
```

### Comparing `streetviewdownloader-0.2.3/README.md` & `streetviewdownloader-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `streetviewdownloader-0.2.3/setup.cfg` & `streetviewdownloader-0.2.4/src/streetviewdownloader.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,49 @@
-[metadata]
-name = streetviewdownloader
-version = attr: streetviewdownloader.__version__
-license = GPLv3
-description = A Python library and utility to download Google StreetView images
-long_description = file: README.md
-long_description_content_type = text/markdown
-url = https://gitlab.com/christophfink/streetviewdownloader
-project_urls = 
-	Documentation = https://streetviewdownloader.readthedocs.org/
-	Change Log = https://gitlab.com/christophfink/streetviewdownloader/-/blob/main/CHANGELOG.md
-	Bug Tracker = https://gitlab.com/christophfink/streetviewdownloader/-/issues
-author = Christoph Fink
-author_email = christoph.fink@helsinki.fi
-classifiers = 
-	Programming Language :: Python :: 3
-	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-	Operating System :: OS Independent
-
-[options]
-packages = find:
-package_dir = 
-	=src
-python_requires = >= 3.9
-install_requires = 
-	ConfigArgParse
-	numpy
-	pygeos
-	pyproj
-	pyrosm
-	pyxdg
-	requests
-	shapely
-
-[options.packages.find]
-where = src
-include = *
-
-[options.entry_points]
-console_scripts = 
-	streetviewdownloader = streetviewdownloader.__main__:main
-
-[egg_info]
-tag_build = 
-tag_date = 0
+Metadata-Version: 2.1
+Name: streetviewdownloader
+Version: 0.2.4
+Summary: A Python library and utility to download Google StreetView images
+Author-email: Christoph Fink <christoph.fink@helsinki.fi>
+License: GPL-3.0-or-later
+Project-URL: Documentation, https://streetviewdownloader.readthedocs.io/
+Project-URL: Repository, https://gitlab.com/christophfink/streetviewdownloader/
+Project-URL: Change log, https://gitlab.com/christophfink/streetviewdownloader/-/blob/main/CHANGELOG.md
+Project-URL: Bug tracker, https://gitlab.com/christophfink/streetviewdownloader/-/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
 
+# streetviewdownloader
+
+**Streetviewdownloader** is a Python>=3.9 library and utility to download images from Google’s StreetView Static API.
+
+## Installation
+
+**Streetviewdownloader** is available from PyPi:
+
+```
+pip install streetviewdownloader
+```
+
+Alternatively, it can be built from source:
+
+```
+git clone https://gitlab.com/christoph.fink/streetviewdownloader
+cd streetviewdownloader
+pip install .
+```
+
+## Usage
+
+### Command line tool
+
+```
+streetviewdownloader --api-key YOUR_API_KEY --url-signing-key YOUR_URL_SIGNING_KEY --extent "POLYGON((24.9791 60.2021, 24.9609 60.2002, 24.9642 60.1894, 24.9826 60.1867, 24.9879 60.1950, 24.9791 60.2021))" --output-directory "Hermanni"
+```
+
+All command line options can alternatively be specified in a configuration file saved to `${XDG_CONFIG_HOME}/streetviewdownloader.yaml` or `%APPDATA%\streetviewdownloader.yaml`, depending on your operating system.
+
+### Library
+
+Streetviewdownloader can also be used via its Python API. Find examples and API reference at https://streetviewdownloader.readthedocs.io
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `streetviewdownloader-0.2.3/src/streetviewdownloader/__init__.py` & `streetviewdownloader-0.2.4/src/streetviewdownloader/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from .streetviewdownloader import StreetViewDownloader
 from .streetnetworkpointgenerator import StreetNetworkPointGenerator
 from .streetviewimagedownloader import StreetViewImageDownloader
 from .streetviewmetadatadownloader import StreetViewMetadataDownloader
 from .streetviewstaticapiauth import StreetViewStaticApiAuth
 
 
-__version__ = "0.2.3"
+__version__ = "0.2.4"
 
 __all__ = [
     "StreetViewDownloader",
     "StreetNetworkPointGenerator",
     "StreetViewImageDownloader",
     "StreetViewMetadataDownloader",
     "StreetViewStaticApiAuth"
```

### Comparing `streetviewdownloader-0.2.3/src/streetviewdownloader/__main__.py` & `streetviewdownloader-0.2.4/src/streetviewdownloader/__main__.py`

 * *Files identical despite different names*

### Comparing `streetviewdownloader-0.2.3/src/streetviewdownloader/basepbfsource.py` & `streetviewdownloader-0.2.4/src/streetviewdownloader/basepbfsource.py`

 * *Files identical despite different names*

### Comparing `streetviewdownloader-0.2.3/src/streetviewdownloader/basestreetviewdownloaderthread.py` & `streetviewdownloader-0.2.4/src/streetviewdownloader/basestreetviewdownloaderthread.py`

 * *Files identical despite different names*

### Comparing `streetviewdownloader-0.2.3/src/streetviewdownloader/basestreetviewsource.py` & `streetviewdownloader-0.2.4/src/streetviewdownloader/basestreetviewsource.py`

 * *Files identical despite different names*

### Comparing `streetviewdownloader-0.2.3/src/streetviewdownloader/bbbikesource.py` & `streetviewdownloader-0.2.4/src/streetviewdownloader/bbbikesource.py`

 * *Files identical despite different names*

### Comparing `streetviewdownloader-0.2.3/src/streetviewdownloader/cache.py` & `streetviewdownloader-0.2.4/src/streetviewdownloader/cache.py`

 * *Files identical despite different names*

### Comparing `streetviewdownloader-0.2.3/src/streetviewdownloader/cachingrequestssession.py` & `streetviewdownloader-0.2.4/src/streetviewdownloader/cachingrequestssession.py`

 * *Files identical despite different names*

### Comparing `streetviewdownloader-0.2.3/src/streetviewdownloader/extractfinder.py` & `streetviewdownloader-0.2.4/src/streetviewdownloader/extractfinder.py`

 * *Files identical despite different names*

### Comparing `streetviewdownloader-0.2.3/src/streetviewdownloader/geofabriksource.py` & `streetviewdownloader-0.2.4/src/streetviewdownloader/geofabriksource.py`

 * *Files identical despite different names*

### Comparing `streetviewdownloader-0.2.3/src/streetviewdownloader/pbffilereader.py` & `streetviewdownloader-0.2.4/src/streetviewdownloader/pbffilereader.py`

 * *Files identical despite different names*

### Comparing `streetviewdownloader-0.2.3/src/streetviewdownloader/streetnetworkdownloader.py` & `streetviewdownloader-0.2.4/src/streetviewdownloader/streetnetworkdownloader.py`

 * *Files identical despite different names*

### Comparing `streetviewdownloader-0.2.3/src/streetviewdownloader/streetnetworkpointgenerator.py` & `streetviewdownloader-0.2.4/src/streetviewdownloader/streetnetworkpointgenerator.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         # cf. https://pythonspeed.com/articles/python-multiprocessing/
 
         points = pandas.concat(
             workers.starmap(
                 self._interpolate_along_lines,
                 zip(
                     numpy.array_split(street_network, num_workers),
-                    itertools.repeat(20)  # add 20 for every split array
+                    itertools.repeat(distance_between_points),  # repeat for every split array
                 ),
             )
         )
 
         points = (
             points
             .set_crs(self._good_enough_crs)
```

### Comparing `streetviewdownloader-0.2.3/src/streetviewdownloader/streetviewdownloader.py` & `streetviewdownloader-0.2.4/src/streetviewdownloader/streetviewdownloader.py`

 * *Files identical despite different names*

### Comparing `streetviewdownloader-0.2.3/src/streetviewdownloader/streetviewimagedownloader.py` & `streetviewdownloader-0.2.4/src/streetviewdownloader/streetviewimagedownloader.py`

 * *Files identical despite different names*

### Comparing `streetviewdownloader-0.2.3/src/streetviewdownloader/streetviewimagedownloaderthread.py` & `streetviewdownloader-0.2.4/src/streetviewdownloader/streetviewimagedownloaderthread.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,16 +47,17 @@
             pano_id[0:2],
             pano_id
         )
         if not os.path.exists(output_directory):
             os.makedirs(output_directory)
             images = self.source.get_images(pano_id)
             for heading, image in images.items():
-                filename = os.path.join(
-                    output_directory,
-                    "{pano_id:s}_{heading:03d}.jpg".format(
-                        pano_id=pano_id,
-                        heading=heading
+                if image is not None:
+                    filename = os.path.join(
+                        output_directory,
+                        "{pano_id:s}_{heading:03d}.jpg".format(
+                            pano_id=pano_id,
+                            heading=heading
+                        )
                     )
-                )
-                with open(filename, "wb") as image_file:
-                    image_file.write(image)
+                    with open(filename, "wb") as image_file:
+                        image_file.write(image)
```

### Comparing `streetviewdownloader-0.2.3/src/streetviewdownloader/streetviewimagesource.py` & `streetviewdownloader-0.2.4/src/streetviewdownloader/streetviewimagesource.py`

 * *Files identical despite different names*

### Comparing `streetviewdownloader-0.2.3/src/streetviewdownloader/streetviewmetadatadownloader.py` & `streetviewdownloader-0.2.4/src/streetviewdownloader/streetviewmetadatadownloader.py`

 * *Files identical despite different names*

### Comparing `streetviewdownloader-0.2.3/src/streetviewdownloader/streetviewmetadatadownloaderthread.py` & `streetviewdownloader-0.2.4/src/streetviewdownloader/streetviewmetadatadownloaderthread.py`

 * *Files identical despite different names*

### Comparing `streetviewdownloader-0.2.3/src/streetviewdownloader/streetviewmetadatasource.py` & `streetviewdownloader-0.2.4/src/streetviewdownloader/streetviewmetadatasource.py`

 * *Files identical despite different names*

### Comparing `streetviewdownloader-0.2.3/src/streetviewdownloader/streetviewstaticapiauth.py` & `streetviewdownloader-0.2.4/src/streetviewdownloader/streetviewstaticapiauth.py`

 * *Files identical despite different names*

### Comparing `streetviewdownloader-0.2.3/src/streetviewdownloader.egg-info/SOURCES.txt` & `streetviewdownloader-0.2.4/src/streetviewdownloader.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 README.md
 pyproject.toml
-setup.cfg
 src/streetviewdownloader/__init__.py
 src/streetviewdownloader/__main__.py
 src/streetviewdownloader/basepbfsource.py
 src/streetviewdownloader/basestreetviewdownloaderthread.py
 src/streetviewdownloader/basestreetviewsource.py
 src/streetviewdownloader/bbbikesource.py
 src/streetviewdownloader/cache.py
@@ -21,10 +20,9 @@
 src/streetviewdownloader/streetviewmetadatadownloader.py
 src/streetviewdownloader/streetviewmetadatadownloaderthread.py
 src/streetviewdownloader/streetviewmetadatasource.py
 src/streetviewdownloader/streetviewstaticapiauth.py
 src/streetviewdownloader.egg-info/PKG-INFO
 src/streetviewdownloader.egg-info/SOURCES.txt
 src/streetviewdownloader.egg-info/dependency_links.txt
-src/streetviewdownloader.egg-info/entry_points.txt
 src/streetviewdownloader.egg-info/requires.txt
 src/streetviewdownloader.egg-info/top_level.txt
```

