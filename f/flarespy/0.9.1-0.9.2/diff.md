# Comparing `tmp/flarespy-0.9.1.tar.gz` & `tmp/flarespy-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flarespy-0.9.1.tar", max compression
+gzip compressed data, was "flarespy-0.9.2.tar", max compression
```

## Comparing `flarespy-0.9.1.tar` & `flarespy-0.9.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2022-09-03 06:20:05.854812 flarespy-0.9.1/LICENSE
--rw-r--r--   0        0        0      428 2023-04-23 17:08:09.188427 flarespy-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     3036 2023-02-03 08:53:00.981401 flarespy-0.9.1/src/flarespy/Flare_model.py
--rw-r--r--   0        0        0      118 2022-09-03 06:20:05.855706 flarespy-0.9.1/src/flarespy/__init__.py
--rw-r--r--   0        0        0   569289 2023-03-30 09:22:45.813451 flarespy-0.9.1/src/flarespy/data/model.dat
--rw-r--r--   0        0        0    31636 2023-04-23 17:07:01.712469 flarespy-0.9.1/src/flarespy/flarefinder.py
--rw-r--r--   0        0        0     7016 2023-04-23 16:22:07.776473 flarespy-0.9.1/src/flarespy/utils.py
--rw-r--r--   0        0        0       22 2023-04-23 17:08:09.193086 flarespy-0.9.1/src/flarespy/version.py
--rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 flarespy-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-09-03 06:20:05.854812 flarespy-0.9.2/LICENSE
+-rw-r--r--   0        0        0      428 2023-04-24 02:24:06.340501 flarespy-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     3036 2023-02-03 08:53:00.981401 flarespy-0.9.2/src/flarespy/Flare_model.py
+-rw-r--r--   0        0        0      118 2022-09-03 06:20:05.855706 flarespy-0.9.2/src/flarespy/__init__.py
+-rw-r--r--   0        0        0   569289 2023-03-30 09:22:45.813451 flarespy-0.9.2/src/flarespy/data/model.dat
+-rw-r--r--   0        0        0    34918 2023-04-24 15:00:46.700468 flarespy-0.9.2/src/flarespy/flarefinder.py
+-rw-r--r--   0        0        0     4831 2023-04-24 15:00:57.653084 flarespy-0.9.2/src/flarespy/utils.py
+-rw-r--r--   0        0        0       22 2023-04-24 02:24:06.342238 flarespy-0.9.2/src/flarespy/version.py
+-rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 flarespy-0.9.2/PKG-INFO
```

### Comparing `flarespy-0.9.1/LICENSE` & `flarespy-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flarespy-0.9.1/src/flarespy/Flare_model.py` & `flarespy-0.9.2/src/flarespy/Flare_model.py`

 * *Files identical despite different names*

### Comparing `flarespy-0.9.1/src/flarespy/data/model.dat` & `flarespy-0.9.2/src/flarespy/data/model.dat`

 * *Files identical despite different names*

### Comparing `flarespy-0.9.1/src/flarespy/flarefinder.py` & `flarespy-0.9.2/src/flarespy/flarefinder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,50 @@
 import logging
 import warnings
 
+import astropy.units as u
 import lightkurve as lk
 import numpy as np
 import pandas as pd
+from astropy.coordinates import SkyCoord
 from astropy.stats import mad_std
+from astropy.time import Time
 from astropy.utils.exceptions import AstropyUserWarning
 from astroquery.exceptions import TableParseError
-from astroquery.vizier import Vizier
+from astroquery.gaia import Gaia
 from astroquery.jplhorizons import Horizons
 from astroquery.mast import Catalogs
 from astroquery.simbad import Simbad
+from astroquery.vizier import Vizier
+from erfa import ErfaWarning
 from matplotlib import pyplot as plt
 from matplotlib.offsetbox import AnchoredText
 from matplotlib.ticker import MaxNLocator
 from wotan import flatten
 
 from .utils import (
+    STELLAR_PARAM_COLUMNS,
     calculate_stellar_luminosity,
     extend,
     fill_gaps,
     find_consecutive,
     get_flare_probability,
-    query_gaia_dr3_id,
 )
 
 logging.getLogger("astroquery").setLevel(logging.WARNING)
 
 CUSTOM_SIMBAD = Simbad()
 CUSTOM_SIMBAD.add_votable_fields("otype")
 CUSTOM_SIMBAD.add_votable_fields("otypes")
+CUSTOM_SIMBAD.add_votable_fields("ids")
 
 VIZIER = Vizier(columns=["Plx", "Gmag", "BP-RP"])
 
+Gaia.MAIN_GAIA_TABLE = "gaiadr3.gaia_source"
+
 EXCLUDED_OTYPES = ["CataclyV*", "CataclyV*_Candidate", "Nova", "Nova_Candidate"]
 
 
 def load_from_lightkurve(lc):
     with warnings.catch_warnings():
         warnings.simplefilter("error", category=lk.LightkurveWarning)
 
@@ -427,82 +435,127 @@
         Query the stellar parameters of the target star.
 
         This method queries various stellar parameters of the target star, such as parallax,
         Gmag, BP-RP, Tmag, and contamination ratio, from Gaia DR3, TIC, and SIMBAD databases.
         It also checks if the target star has an excluded object type.
         """
 
-        self._query_basic_info()
+        self._query_gaia_dr3_id()
+
+        obs_duration = np.round(self.meta["TIMEDEL"] * np.nonzero(~np.isnan(self.flux.value))[0].size, 4)
+        self.stellar_parameters.obs_duration = obs_duration
+
         self._query_object_type()
-        self._query_gaia_dr3()
+        self._query_gaia_dr3_params()
         self._query_tic()
 
-    def _query_basic_info(self):
-        gaia_dr3_id = query_gaia_dr3_id(self.ticid)
-        obs_duration = np.round(self.meta["TIMEDEL"] * np.nonzero(~np.isnan(self.flux.value))[0].size, 4)
+    def _query_gaia_dr3_id(self):
+        """
+        Query Gaia DR3 ID from TIC ID.
+        """
 
-        self.stellar_parameters = pd.Series(
-            index=[
-                "gaia_dr3_source_id",
-                "obj_type",
-                "Plx",
-                "Gmag",
-                "BP-RP",
-                "Tmag",
-                "cont_ratio",
-                "obs_duration",
-            ],
-            dtype=object,
-        )
+        if self.stellar_parameters is None:
+            self.stellar_parameters = pd.Series(index=STELLAR_PARAM_COLUMNS, dtype=object)
 
-        self.stellar_parameters.gaia_dr3_source_id = gaia_dr3_id
-        self.stellar_parameters.obs_duration = obs_duration
+        gaia_dr3_source_id = ""
+        with warnings.catch_warnings():
+            warnings.simplefilter("error", category=UserWarning)
+            try:
+                simbad_result = CUSTOM_SIMBAD.query_object(self.label)
+                id_list = simbad_result["IDS"][0].split("|")
+                for i in id_list:
+                    if "Gaia DR3" in i:
+                        gaia_dr3_source_id = str(i.split(" ")[-1])
+                self._is_cv(simbad_result)
+            except TableParseError:
+                pass
+
+            if gaia_dr3_source_id == "":
+                mast_result = Catalogs.query_criteria(catalog="TIC", ID=self.ticid)
+                gaia2_source_id = mast_result["GAIA"].data.data[0]
+                if gaia2_source_id != "":
+                    query = """
+                            SELECT dr2_source_id, dr3_source_id
+                            FROM gaiadr3.dr2_neighbourhood
+                            WHERE dr2_source_id = {gaia2_source_id}
+                            """
+                    cross_result = Gaia.launch_job(query.format(gaia2_source_id=gaia2_source_id)).get_results()
+                    gaia_dr3_source_id = str(cross_result["dr3_source_id"][0])
+                else:
+                    ra = mast_result["ra"].data.data[0] * u.deg
+                    dec = mast_result["dec"].data.data[0] * u.deg
+                    pm_ra = mast_result["pmRA"].data.data[0] * u.mas / u.yr
+                    pm_dec = mast_result["pmDEC"].data.data[0] * u.mas / u.yr
+                    if ~np.isnan(pm_ra) and ~np.isnan(pm_dec):
+                        coords_j2000 = SkyCoord(
+                            ra, dec, pm_ra_cosdec=pm_ra, pm_dec=pm_dec, frame="icrs", obstime=Time("J2000")
+                        )
+                        with warnings.catch_warnings():
+                            warnings.filterwarnings("ignore", category=ErfaWarning)
+                            coords = coords_j2000.apply_space_motion(new_obstime=Time("J2016"))
+                    else:
+                        coords = SkyCoord(ra, dec, frame="icrs")
+                    radius = u.Quantity(1, u.arcmin)
+                    gaia_result = Gaia.cone_search_async(coords, radius, columns=["source_id"]).get_results()
+                    if (gaia_result["dist"] < (3 / 3600)).any():
+                        gaia_dr3_source_id = str(gaia_result["source_id"].data.data[0])
+
+        self.stellar_parameters.gaia_dr3_source_id = gaia_dr3_source_id
 
     def _query_object_type(self):
         """
         Query object info from SIMBAD
         """
 
-        query_result = None
+        if self.stellar_parameters is None:
+            self.stellar_parameters = pd.Series(index=STELLAR_PARAM_COLUMNS, dtype=object)
+
         with warnings.catch_warnings():
             warnings.simplefilter("error", category=UserWarning)
             try:
-                query_result = CUSTOM_SIMBAD.query_object(self.label)
+                simbad_result = CUSTOM_SIMBAD.query_object(self.label)
             except TableParseError:
-                if self.stellar_parameters is None:
-                    self._query_basic_info()
-                gaia_dr3_id = self.stellar_parameters.gaia_dr3_source_id
-
-                if isinstance(gaia_dr3_id, str):
-                    try:
-                        query_result = CUSTOM_SIMBAD.query_object(f"Gaia DR3 {gaia_dr3_id}")
-                    except TableParseError:
-                        pass
-
-        self.meta["EXCLUDE"] = False
-        if query_result is None:
-            self.stellar_parameters["obj_type"] = np.nan
+                try:
+                    obj_coord = SkyCoord(self.ra, self.dec, unit=(u.deg, u.deg), frame="icrs")
+                    simbad_result = CUSTOM_SIMBAD.query_region(obj_coord, radius=3 * u.arcsec)
+                    if len(simbad_result) > 1:
+                        simbad_coords = SkyCoord(
+                            simbad_result["RA"].data.data,
+                            simbad_result["DEC"].data.data,
+                            unit=(u.hourangle, u.deg),
+                        )
+                        distance = obj_coord.separation(simbad_coords)
+                        simbad_result = simbad_result[distance.value.argmin()]
+
+                except TableParseError:
+                    simbad_result = None
+
+        if simbad_result is not None:
+            self._is_cv(simbad_result)
+
+    def _is_cv(self, simbad_result):
+        obj_type = simbad_result["OTYPE"][0]
+        self.stellar_parameters.obj_type = obj_type
+        obj_type_list = simbad_result["OTYPES"][0].split("|")
+        if obj_type in EXCLUDED_OTYPES or "CV*" in obj_type_list:
+            self.meta["EXCLUDE"] = True
         else:
-            obj_type = query_result["OTYPE"][0]
-            obj_type_list = query_result["OTYPES"][0].split("|")
-            self.stellar_parameters.obj_type = obj_type
-
-            if obj_type in EXCLUDED_OTYPES or "CV*" in obj_type_list:
-                self.meta["EXCLUDE"] = True
+            self.meta["EXCLUDE"] = False
 
-    def _query_gaia_dr3(self):
+    def _query_gaia_dr3_params(self):
         """
         Query parallax, Gmag and BP-RP from Gaia DR3
         """
 
-        if self.stellar_parameters is None:
-            self._query_basic_info()
+        if (self.stellar_parameters is None) or (not isinstance(self.stellar_parameters.gaia_dr3_source_id, str)):
+            self._query_gaia_dr3_id()
+
         gaia_dr3_id = self.stellar_parameters.gaia_dr3_source_id
 
-        if isinstance(gaia_dr3_id, str):
+        if gaia_dr3_id != "":
             result = VIZIER.query_constraints("I/355/gaiadr3", Source=gaia_dr3_id)[0]
             plx = result["Plx"].data.data[0]
             if plx > 0:
                 self.stellar_parameters["Plx"] = np.round(plx, 4)
             self.stellar_parameters["Gmag"] = np.round(result["Gmag"].data.data[0], 4)
             self.stellar_parameters["BP-RP"] = np.round(result["BP-RP"].data.data[0], 4)
 
@@ -576,16 +629,21 @@
                 time, flux = fill_gaps(time, flux, candidate.cadenceno)
 
             if flux.size >= 4:
                 proba_array[row.Index] = round(get_flare_probability(time, flux), 3)
         self.candidate_parameters["flare_prob"] = proba_array
 
     def _calculate_energy(self, ed):
-        if self.stellar_parameters is None:
-            self._query_gaia_dr3()
+        if (self.stellar_parameters is None) or (not isinstance(self.stellar_parameters.gaia_dr3_source_id, str)):
+            self._query_gaia_dr3_id()
+
+        if np.isnan(self.stellar_parameters.Gmag):
+            self._query_gaia_dr3_params()
+
+        if np.isnan(self.stellar_parameters.Tmag):
             self._query_tic()
 
         stellar_lum = calculate_stellar_luminosity(self.stellar_parameters.Tmag, self.stellar_parameters.Plx)
 
         if np.isnan(stellar_lum):
             self.candidate_parameters["energy"] = np.nan
         else:
@@ -600,15 +658,16 @@
         This method performs a series of steps to identify flares in the light curve. It queries
         the stellar parameters of the target star, detrends the light curve, finds the flare
         candidates, detects if the candidates are caused by SSO encounters, and calculates the
         candidate parameters. The results are stored in the class attributes.
         """
 
         if exclude_cv:
-            self._query_object_type()
+            if not hasattr(self.stellar_parameters, "EXCLUDE"):
+                self._query_object_type()
         else:
             self.meta["EXCLUDE"] = False
 
         if not self.meta["EXCLUDE"]:
             self.detrend()
             self.find_candidates()
```

### Comparing `flarespy-0.9.1/PKG-INFO` & `flarespy-0.9.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flarespy
-Version: 0.9.1
+Version: 0.9.2
 Summary: Find flares in TESS light curves
 Home-page: https://github.com/keyuxing/flarespy
 License: MIT
 Author: Keyu Xing
 Author-email: kyxing@mail.bnu.edu.cn
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

