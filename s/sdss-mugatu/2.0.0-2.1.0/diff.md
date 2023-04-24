# Comparing `tmp/sdss-mugatu-2.0.0.tar.gz` & `tmp/sdss-mugatu-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss-mugatu-2.0.0.tar", max compression
+gzip compressed data, was "sdss-mugatu-2.1.0.tar", max compression
```

## Comparing `sdss-mugatu-2.0.0.tar` & `sdss-mugatu-2.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1504 2020-12-17 23:08:43.845089 sdss-mugatu-2.0.0/LICENSE.md
--rw-r--r--   0        0        0      468 2022-07-21 18:15:27.339825 sdss-mugatu-2.0.0/README.md
--rw-r--r--   0        0        0      814 2023-01-05 17:13:56.304944 sdss-mugatu-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      544 2020-12-17 23:08:43.893921 sdss-mugatu-2.0.0/python/mugatu/__init__.py
--rw-r--r--   0        0        0    12505 2021-05-26 17:34:23.788221 sdss-mugatu-2.0.0/python/mugatu/comm_designs.py
--rw-r--r--   0        0        0    70832 2022-11-29 19:32:23.070377 sdss-mugatu-2.0.0/python/mugatu/designmode.py
--rw-r--r--   0        0        0    24128 2022-11-01 20:48:07.161575 sdss-mugatu-2.0.0/python/mugatu/designs_to_targetdb.py
--rw-r--r--   0        0        0      123 2020-12-17 23:08:43.929881 sdss-mugatu-2.0.0/python/mugatu/etc/mugatu.yml
--rw-r--r--   0        0        0     2345 2022-04-11 22:05:06.045880 sdss-mugatu-2.0.0/python/mugatu/exceptions.py
--rw-r--r--   0        0        0    56425 2022-11-29 19:32:23.072628 sdss-mugatu-2.0.0/python/mugatu/fpsdesign.py
--rw-r--r--   0        0        0     2912 2021-12-15 21:36:43.244598 sdss-mugatu-2.0.0/python/mugatu/templates/dmode_check_w_dists.html
--rw-r--r--   0        0        0     3648 2021-12-15 21:31:24.094630 sdss-mugatu-2.0.0/python/mugatu/templates/dmode_check_w_dists_sky.html
--rw-r--r--   0        0        0     2507 2022-02-15 22:38:05.801913 sdss-mugatu-2.0.0/python/mugatu/templates/main_validation_page.html
--rw-r--r--   0        0        0      669 2021-12-15 20:58:33.216830 sdss-mugatu-2.0.0/python/mugatu/templates/valid_check.html
--rw-r--r--   0        0        0     1200 2021-12-15 21:26:38.661378 sdss-mugatu-2.0.0/python/mugatu/templates/valid_check_w_dists.html
--rw-r--r--   0        0        0     2719 2023-01-05 17:17:33.498819 sdss-mugatu-2.0.0/setup.py
--rw-r--r--   0        0        0     1536 2023-01-05 17:17:33.499326 sdss-mugatu-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1504 2020-12-17 23:08:43.845089 sdss-mugatu-2.1.0/LICENSE.md
+-rw-r--r--   0        0        0      468 2022-07-21 18:15:27.339825 sdss-mugatu-2.1.0/README.md
+-rw-r--r--   0        0        0      814 2023-04-24 20:11:36.718379 sdss-mugatu-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      544 2020-12-17 23:08:43.893921 sdss-mugatu-2.1.0/python/mugatu/__init__.py
+-rw-r--r--   0        0        0    12505 2021-05-26 17:34:23.788221 sdss-mugatu-2.1.0/python/mugatu/comm_designs.py
+-rw-r--r--   0        0        0    70758 2023-04-24 20:06:33.874805 sdss-mugatu-2.1.0/python/mugatu/designmode.py
+-rw-r--r--   0        0        0    24128 2022-11-01 20:48:07.161575 sdss-mugatu-2.1.0/python/mugatu/designs_to_targetdb.py
+-rw-r--r--   0        0        0      123 2020-12-17 23:08:43.929881 sdss-mugatu-2.1.0/python/mugatu/etc/mugatu.yml
+-rw-r--r--   0        0        0     2345 2022-04-11 22:05:06.045880 sdss-mugatu-2.1.0/python/mugatu/exceptions.py
+-rw-r--r--   0        0        0    56425 2022-11-29 19:32:23.072628 sdss-mugatu-2.1.0/python/mugatu/fpsdesign.py
+-rw-r--r--   0        0        0     2912 2021-12-15 21:36:43.244598 sdss-mugatu-2.1.0/python/mugatu/templates/dmode_check_w_dists.html
+-rw-r--r--   0        0        0     3648 2021-12-15 21:31:24.094630 sdss-mugatu-2.1.0/python/mugatu/templates/dmode_check_w_dists_sky.html
+-rw-r--r--   0        0        0     2507 2022-02-15 22:38:05.801913 sdss-mugatu-2.1.0/python/mugatu/templates/main_validation_page.html
+-rw-r--r--   0        0        0      669 2021-12-15 20:58:33.216830 sdss-mugatu-2.1.0/python/mugatu/templates/valid_check.html
+-rw-r--r--   0        0        0     1200 2021-12-15 21:26:38.661378 sdss-mugatu-2.1.0/python/mugatu/templates/valid_check_w_dists.html
+-rw-r--r--   0        0        0     2719 2023-04-24 20:14:23.213127 sdss-mugatu-2.1.0/setup.py
+-rw-r--r--   0        0        0     1536 2023-04-24 20:14:23.213631 sdss-mugatu-2.1.0/PKG-INFO
```

### Comparing `sdss-mugatu-2.0.0/LICENSE.md` & `sdss-mugatu-2.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss-mugatu-2.0.0/pyproject.toml` & `sdss-mugatu-2.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-mugatu"
-version = "2.0.0"
+version = "2.1.0"
 description = "Package to read, write and validate FPS designs"
 authors = ["Ilija Medan"]
 license = "BSD 3-Clause License"
 homepage = "https://pypi.org/project/sdss-mugatu/"
 repository = "https://github.com/sdss/mugatu"
 documentation = "https://mugatu.readthedocs.io/en/latest/"
 readme = "README.md"
```

### Comparing `sdss-mugatu-2.0.0/python/mugatu/__init__.py` & `sdss-mugatu-2.1.0/python/mugatu/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss-mugatu-2.0.0/python/mugatu/comm_designs.py` & `sdss-mugatu-2.1.0/python/mugatu/comm_designs.py`

 * *Files identical despite different names*

### Comparing `sdss-mugatu-2.0.0/python/mugatu/designmode.py` & `sdss-mugatu-2.1.0/python/mugatu/designmode.py`

 * *Files 1% similar despite different names*

```diff
@@ -504,15 +504,15 @@
                                                      mag_core)),
                                     axis=1)
     return adjusted_mag_bs
 
 
 def build_brigh_neigh_query(check_type, instrument, mag_lim,
                             racen, deccen, observatory=None,
-                            version_catdb='0.5.0'):
+                            version_catdb='1.0.0'):
     """
     Builds the database query needed to run bright
     neighbor check
 
     Parameters
     ----------
     check_type: str
@@ -555,33 +555,32 @@
         r_search = 1.5
     elif observatory == 'APO':
         r_search = 1.5
     else:
         r_search = 1.0
     if check_type == 'designmode':
         if instrument == 'BOSS':
-            cat = catalogdb.Gaia_DR2
+            cat = catalogdb.Gaia_DR3
             ra_col = catalogdb.Catalog.ra
             dec_col = catalogdb.Catalog.dec
             ra_col_str = 'ra'
             dec_col_str = 'dec'
-            mag_col = catalogdb.Gaia_DR2.phot_g_mean_mag
+            mag_col = catalogdb.Gaia_DR3.phot_g_mean_mag
             # run the query
             db_query_gaia = (catalogdb.Catalog.select(
                 ra_col,
                 dec_col,
                 mag_col,
                 catalogdb.Catalog.catalogid,
                 catalogdb.Catalog.pmra,
                 catalogdb.Catalog.pmdec)
                 .join(catalogdb.Version)
                 .switch(catalogdb.Catalog)
-                .join(catalogdb.CatalogToTIC_v8)
-                .join(catalogdb.TIC_v8)
-                .join(catalogdb.Gaia_DR2)
+                .join(catalogdb.CatalogToGaia_DR3)
+                .join(catalogdb.Gaia_DR3)
                 .where((cat.cone_search(racen,
                                         deccen,
                                         r_search,
                                         ra_col=ra_col_str,
                                         dec_col=dec_col_str)) &
                        (mag_col < mag_lim) &
                        (catalogdb.Version.plan == version_catdb)))
@@ -671,16 +670,15 @@
                 dec_col,
                 mag_col,
                 catalogdb.Catalog.catalogid,
                 catalogdb.Catalog.pmra,
                 catalogdb.Catalog.pmdec)
                 .join(catalogdb.Version)
                 .switch(catalogdb.Catalog)
-                .join(catalogdb.CatalogToTIC_v8)
-                .join(catalogdb.TIC_v8)
+                .join(catalogdb.CatalogToTwoMassPSC)
                 .join(cat)
                 .where((cat.cone_search(racen,
                                         deccen,
                                         r_search,
                                         ra_col=ra_col_str,
                                         dec_col=dec_col_str)) &
                        (mag_col < mag_lim) &
```

### Comparing `sdss-mugatu-2.0.0/python/mugatu/designs_to_targetdb.py` & `sdss-mugatu-2.1.0/python/mugatu/designs_to_targetdb.py`

 * *Files identical despite different names*

### Comparing `sdss-mugatu-2.0.0/python/mugatu/exceptions.py` & `sdss-mugatu-2.1.0/python/mugatu/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdss-mugatu-2.0.0/python/mugatu/fpsdesign.py` & `sdss-mugatu-2.1.0/python/mugatu/fpsdesign.py`

 * *Files identical despite different names*

### Comparing `sdss-mugatu-2.0.0/python/mugatu/templates/dmode_check_w_dists.html` & `sdss-mugatu-2.1.0/python/mugatu/templates/dmode_check_w_dists.html`

 * *Files identical despite different names*

### Comparing `sdss-mugatu-2.0.0/python/mugatu/templates/dmode_check_w_dists_sky.html` & `sdss-mugatu-2.1.0/python/mugatu/templates/dmode_check_w_dists_sky.html`

 * *Files identical despite different names*

### Comparing `sdss-mugatu-2.0.0/python/mugatu/templates/main_validation_page.html` & `sdss-mugatu-2.1.0/python/mugatu/templates/main_validation_page.html`

 * *Files identical despite different names*

### Comparing `sdss-mugatu-2.0.0/python/mugatu/templates/valid_check.html` & `sdss-mugatu-2.1.0/python/mugatu/templates/valid_check.html`

 * *Files identical despite different names*

### Comparing `sdss-mugatu-2.0.0/python/mugatu/templates/valid_check_w_dists.html` & `sdss-mugatu-2.1.0/python/mugatu/templates/valid_check_w_dists.html`

 * *Files identical despite different names*

### Comparing `sdss-mugatu-2.0.0/setup.py` & `sdss-mugatu-2.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
  'sdss-access==1.1.1',
  'sdss-coordio==1.5.2',
  'sdss-kaiju==1.3.1',
  'sdssdb>=0.5.4,<0.6.0']
 
 setup_kwargs = {
     'name': 'sdss-mugatu',
-    'version': '2.0.0',
+    'version': '2.1.0',
     'description': 'Package to read, write and validate FPS designs',
     'long_description': '# mugatu\n\n![Versions](https://img.shields.io/badge/python->3.8-blue)\n[![Documentation Status](https://readthedocs.org/projects/mugatu/badge/?version=latest)](https://mugatu.readthedocs.io/en/latest/#)\n<!---\n[![Travis (.org)](https://img.shields.io/travis/sdss/mugatu)](https://travis-ci.org/sdss/mugatu)\n[![codecov](https://codecov.io/gh/sdss/mugatu/branch/main/graph/badge.svg)](https://codecov.io/gh/sdss/mugatu)\n-->\n\nPackage to read, write and validate FPS designs\n',
     'author': 'Ilija Medan',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://pypi.org/project/sdss-mugatu/',
```

### Comparing `sdss-mugatu-2.0.0/PKG-INFO` & `sdss-mugatu-2.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-mugatu
-Version: 2.0.0
+Version: 2.1.0
 Summary: Package to read, write and validate FPS designs
 Home-page: https://pypi.org/project/sdss-mugatu/
 License: BSD 3-Clause License
 Author: Ilija Medan
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

