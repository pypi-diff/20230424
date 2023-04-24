# Comparing `tmp/astroconst-0.0.6.tar.gz` & `tmp/astroconst-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astroconst-0.0.6.tar", last modified: Fri Oct 21 09:44:21 2022, max compression
+gzip compressed data, was "astroconst-0.0.7.tar", last modified: Mon Apr 24 10:16:30 2023, max compression
```

## Comparing `astroconst-0.0.6.tar` & `astroconst-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 sluys     (1000) sluys     (1000)        0 2022-10-21 09:44:21.736986 astroconst-0.0.6/
--rw-r--r--   0 sluys     (1000) sluys     (1000)    13827 2022-01-04 18:50:46.000000 astroconst-0.0.6/LICENCE
--rw-r--r--   0 sluys     (1000) sluys     (1000)     4013 2022-10-21 09:44:21.736986 astroconst-0.0.6/PKG-INFO
--rw-r--r--   0 sluys     (1000) sluys     (1000)     3128 2022-01-09 16:53:51.000000 astroconst-0.0.6/README.md
-drwxr-xr-x   0 sluys     (1000) sluys     (1000)        0 2022-10-21 09:44:21.735986 astroconst-0.0.6/astroconst/
--rw-r--r--   0 sluys     (1000) sluys     (1000)    13640 2022-10-21 08:49:01.000000 astroconst-0.0.6/astroconst/__init__.py
--rw-r--r--   0 sluys     (1000) sluys     (1000)     9525 2022-01-09 08:23:27.000000 astroconst-0.0.6/astroconst/aa.py
-drwxr-xr-x   0 sluys     (1000) sluys     (1000)        0 2022-10-21 09:44:21.736986 astroconst-0.0.6/astroconst.egg-info/
--rw-r--r--   0 sluys     (1000) sluys     (1000)     4013 2022-10-21 09:44:21.000000 astroconst-0.0.6/astroconst.egg-info/PKG-INFO
--rw-r--r--   0 sluys     (1000) sluys     (1000)      235 2022-10-21 09:44:21.000000 astroconst-0.0.6/astroconst.egg-info/SOURCES.txt
--rw-r--r--   0 sluys     (1000) sluys     (1000)        1 2022-10-21 09:44:21.000000 astroconst-0.0.6/astroconst.egg-info/dependency_links.txt
--rw-r--r--   0 sluys     (1000) sluys     (1000)        6 2022-10-21 09:44:21.000000 astroconst-0.0.6/astroconst.egg-info/requires.txt
--rw-r--r--   0 sluys     (1000) sluys     (1000)       11 2022-10-21 09:44:21.000000 astroconst-0.0.6/astroconst.egg-info/top_level.txt
--rw-r--r--   0 sluys     (1000) sluys     (1000)       38 2022-10-21 09:44:21.736986 astroconst-0.0.6/setup.cfg
--rwxr-xr-x   0 sluys     (1000) sluys     (1000)     1388 2022-10-21 09:33:47.000000 astroconst-0.0.6/setup.py
+drwxr-xr-x   0 sluys     (1000) sluys     (1000)        0 2023-04-24 10:16:30.001303 astroconst-0.0.7/
+-rw-r--r--   0 sluys     (1000) sluys     (1000)    13827 2022-01-04 18:50:46.000000 astroconst-0.0.7/LICENCE
+-rw-r--r--   0 sluys     (1000) sluys     (1000)     4013 2023-04-24 10:16:30.001303 astroconst-0.0.7/PKG-INFO
+-rw-r--r--   0 sluys     (1000) sluys     (1000)     3128 2022-01-09 16:53:51.000000 astroconst-0.0.7/README.md
+drwxr-xr-x   0 sluys     (1000) sluys     (1000)        0 2023-04-24 10:16:30.001303 astroconst-0.0.7/astroconst/
+-rw-r--r--   0 sluys     (1000) sluys     (1000)    14616 2023-02-22 16:24:43.000000 astroconst-0.0.7/astroconst/__init__.py
+-rw-r--r--   0 sluys     (1000) sluys     (1000)     9530 2023-01-30 10:58:23.000000 astroconst-0.0.7/astroconst/aa.py
+drwxr-xr-x   0 sluys     (1000) sluys     (1000)        0 2023-04-24 10:16:30.001303 astroconst-0.0.7/astroconst.egg-info/
+-rw-r--r--   0 sluys     (1000) sluys     (1000)     4013 2023-04-24 10:16:29.000000 astroconst-0.0.7/astroconst.egg-info/PKG-INFO
+-rw-r--r--   0 sluys     (1000) sluys     (1000)      235 2023-04-24 10:16:29.000000 astroconst-0.0.7/astroconst.egg-info/SOURCES.txt
+-rw-r--r--   0 sluys     (1000) sluys     (1000)        1 2023-04-24 10:16:29.000000 astroconst-0.0.7/astroconst.egg-info/dependency_links.txt
+-rw-r--r--   0 sluys     (1000) sluys     (1000)        6 2023-04-24 10:16:29.000000 astroconst-0.0.7/astroconst.egg-info/requires.txt
+-rw-r--r--   0 sluys     (1000) sluys     (1000)       11 2023-04-24 10:16:29.000000 astroconst-0.0.7/astroconst.egg-info/top_level.txt
+-rw-r--r--   0 sluys     (1000) sluys     (1000)       38 2023-04-24 10:16:30.001303 astroconst-0.0.7/setup.cfg
+-rwxr-xr-x   0 sluys     (1000) sluys     (1000)     1388 2023-04-24 09:52:26.000000 astroconst-0.0.7/setup.py
```

### Comparing `astroconst-0.0.6/LICENCE` & `astroconst-0.0.7/LICENCE`

 * *Files identical despite different names*

### Comparing `astroconst-0.0.6/PKG-INFO` & `astroconst-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astroconst
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python package that provides astronomical constants.
 Home-page: https://github.com/MarcvdSluys/AstroConst
 Author: Marc van der Sluys
 License: EUPL 1.2
 Keywords: constants,astronomy,physics,mathematics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `astroconst-0.0.6/README.md` & `astroconst-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `astroconst-0.0.6/astroconst/__init__.py` & `astroconst-0.0.7/astroconst/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-#  Copyright (c) 2022  Marc van der Sluys - marc.vandersluys.nl
+#  Copyright (c) 2022-2023  Marc van der Sluys - marc.vandersluys.nl
 #   
 #  This file is part of the AstroConst Python package:
 #  A Python package that provides astronomical constants.
 #  See: https://github.com/MarcvdSluys/AstroConst
 #   
 #  This is free software: you can redistribute it and/or modify it under the terms of the European Union
 #  Public Licence 1.2 (EUPL 1.2).  This software is distributed in the hope that it will be useful, but
@@ -72,14 +72,15 @@
 
 # Calendar/time:
 jd1820 = 2385801;        """JD in 1820 (when ΔT=0)"""
 jd1875 = 2405890;        """JD at J1875.0 (when constellation boundaries were defined)"""
 jd1900 = 2415021;        """JD at J1900.0"""
 jd1950 = 2433283;        """JD at J1950.0"""
 jd2000 = 2451545;        """JD at J2000.0 (2000-01-01 12:00 UT)"""
+jd_hip = 2448349.0625;   """JD of the Hipparcos catalogue (1991-04-02 ~13:29 UT) - https://heasarc.gsfc.nasa.gov/W3Browse/all/hipparcos.html"""
 
 # Month names: 1-12 = Jan-Dec
 # en:
 months_en          = __np.array(['','January','February','March','April','May','June','July','August','September','October','November','December']);   """Capitalised month names in English."""  # (13x9)
 months_en_lc       = __np.array(['','january','february','march','april','may','june','july','august','september','october','november','december']);   """Lower-case month names in English."""  # (13x9)
 months_en_abr      = __np.array(['','Jan','Feb','Mar','Apr','May','Jun','Jul','Aug','Sep','Oct','Nov','Dec']);                                         """Capitalised month abbreviations in English."""  # (13x3)
 months_en_abr_lc   = __np.array(['','jan','feb','mar','apr','may','jun','jul','aug','sep','oct','nov','dec']);                                         """Lower-case month abbreviations in English."""  # (13x3)
@@ -133,29 +134,38 @@
 
 
 # Astronomical constants:
 r_sun = 6.9599e8;                       """Solar radius in SI (m)"""
 m_sun = 1.9891e30;                      """Solar mass in SI (kg)"""
 l_sun = 3.85e26;                        """Solar luminosity in SI (W)"""
 
+sun_r = 6.9599e8;                       """Solar radius in SI (m)"""
+sun_m = 1.9891e30;                      """Solar mass in SI (kg)"""
+sun_l = 3.85e26;                        """Solar luminosity in SI (W)"""
+
 sol_const = 1361.5;                     """Solar constant in W/m^2 (Wikipedia)"""
 
 
 eps2000 = 0.409092804;                  """Obliquity of the ecliptic at J2000.0 (radians)"""
 
 
 
 # Planet data:
 r_earth = 6378136.6;                    """Equatorial radius of the Earth in SI (m), WGS84"""
+e_earth = 0.01671;                      """Orbital eccentricity of the Earth - https://en.wikipedia.org/wiki/Orbital_eccentricity"""
+
+earth_r = 6378136.6;                    """Equatorial radius of the Earth in SI (m), WGS84"""
+earth_e = 0.01671;                      """Orbital eccentricity of the Earth - https://en.wikipedia.org/wiki/Orbital_eccentricity"""
+
 
 pl_d = __np.array([3476.206e3, 4879.4e3, 12198e3, 2*r_earth, 6792.4e3, 142984e3, 120536e3, 51118e3, 49528e3, 2390e3]);  """Equatorial planet diameters (m); [0]=Moon; Venus = 12103.6km + clouds?"""
 pl_r = pl_d/2;  """Planet equatorial radii (m) = pland/2."""
-pl_a = __np.array([384400e3/au, 0.3871, 0.7233, 1, 1.5237, 5.2028, 9.5388, 19.191, 30.061, 39.529])*au;  """Planet semi-major axes (m); [0]=Moon"""
-pl_p = __np.array([0.0748, 0.240846, 0.615198, 1, 1.88082, 11.862, 29.4571, 84.0205, 164.8, 247.94])*year_trop;  """Planet orbital periods (s - https://en.wikipedia.org/wiki/Orbital_period); [0]=Moon."""
-
+pl_a = __np.array([384400e3/au, 0.3871,   0.7233,       1,  1.5237, 5.2028,  9.5388, 19.191,  30.061, 39.529])*au;         """Planet semi-major axes (m); [0]=Moon"""
+pl_p = __np.array([0.0748,    0.240846, 0.615198,       1, 1.88082, 11.862, 29.4571, 84.0205,  164.8, 247.94])*year_trop;  """Planet orbital periods (s - https://en.wikipedia.org/wiki/Orbital_period); [0]=Moon."""
+pl_e = __np.array([0.0549,      0.2056,   0.0068, 0.01671,  0.0934, 0.0484,  0.0541,  0.0472, 0.0086, 0.2488]);            """Planet orbital eccentricities (s - https://en.wikipedia.org/wiki/Orbital_eccentricity); [0]=Moon."""
 
 # Satellites:
 # satrad(4:8,30);   """Radii Galilean moons (m)"""
 # satdiam(4:8,30);  """Diameters Galilean moons (m)"""
 
 
 # English planet names:
```

### Comparing `astroconst-0.0.6/astroconst/aa.py` & `astroconst-0.0.7/astroconst/aa.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/bin/env python
 # -*- coding: utf-8 -*-
 #
-#  Copyright (c) 2022  Marc van der Sluys - marc.vandersluys.nl
+#  Copyright (c) 2022-2023  Marc van der Sluys - marc.vandersluys.nl
 #  
 #  This file is part of the AstroConst Python package:
 #  A Python package that provides astronomical constants.
 #  See: https://github.com/MarcvdSluys/AstroConst
 #  
 #  This is free software: you can redistribute it and/or modify it under the terms of the European Union
 #  Public Licence 1.2 (EUPL 1.2).  This software is distributed in the hope that it will be useful, but
```

### Comparing `astroconst-0.0.6/astroconst.egg-info/PKG-INFO` & `astroconst-0.0.7/astroconst.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astroconst
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python package that provides astronomical constants.
 Home-page: https://github.com/MarcvdSluys/AstroConst
 Author: Marc van der Sluys
 License: EUPL 1.2
 Keywords: constants,astronomy,physics,mathematics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `astroconst-0.0.6/setup.py` & `astroconst-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/bin/env python
 # -*- coding: utf-8 -*-
 
 """Setup.py for the AstroConst Python package."""
 
 
 # Package version:
-version='0.0.6'
+version='0.0.7'
 
 # Get long description from README.md:
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 # Set package properties:
 from setuptools import setup
```

