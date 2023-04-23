# Comparing `tmp/Solarflare-0.0.4.tar.gz` & `tmp/Solarflare-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Solarflare-0.0.4.tar", last modified: Sun Apr 23 17:37:18 2023, max compression
+gzip compressed data, was "Solarflare-0.0.5.tar", last modified: Sun Apr 23 22:37:09 2023, max compression
```

## Comparing `Solarflare-0.0.4.tar` & `Solarflare-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:37:18.112101 Solarflare-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-23 17:37:18.112101 Solarflare-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-23 17:37:04.000000 Solarflare-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:37:18.108101 Solarflare-0.0.4/Solarflare/
--rw-r--r--   0 runner    (1001) docker     (123)    20110 2023-04-23 17:37:04.000000 Solarflare-0.0.4/Solarflare/conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-23 17:37:04.000000 Solarflare-0.0.4/Solarflare/nightcalc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-04-23 17:37:04.000000 Solarflare-0.0.4/Solarflare/solarflare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:37:18.112101 Solarflare-0.0.4/Solarflare.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-23 17:37:18.000000 Solarflare-0.0.4/Solarflare.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-23 17:37:18.000000 Solarflare-0.0.4/Solarflare.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 17:37:18.000000 Solarflare-0.0.4/Solarflare.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-23 17:37:18.000000 Solarflare-0.0.4/Solarflare.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 17:37:18.112101 Solarflare-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-23 17:37:04.000000 Solarflare-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:37:09.207240 Solarflare-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-23 22:37:09.207240 Solarflare-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-23 22:36:53.000000 Solarflare-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:37:09.203240 Solarflare-0.0.5/Solarflare/
+-rw-r--r--   0 runner    (1001) docker     (123)    20110 2023-04-23 22:36:53.000000 Solarflare-0.0.5/Solarflare/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-04-23 22:36:53.000000 Solarflare-0.0.5/Solarflare/nightcalc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-04-23 22:36:53.000000 Solarflare-0.0.5/Solarflare/solarflare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:37:09.203240 Solarflare-0.0.5/Solarflare.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-23 22:37:09.000000 Solarflare-0.0.5/Solarflare.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-23 22:37:09.000000 Solarflare-0.0.5/Solarflare.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 22:37:09.000000 Solarflare-0.0.5/Solarflare.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-23 22:37:09.000000 Solarflare-0.0.5/Solarflare.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 22:37:09.207240 Solarflare-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-23 22:36:53.000000 Solarflare-0.0.5/setup.py
```

### Comparing `Solarflare-0.0.4/Solarflare/conversions.py` & `Solarflare-0.0.5/Solarflare/conversions.py`

 * *Files identical despite different names*

### Comparing `Solarflare-0.0.4/Solarflare/nightcalc.py` & `Solarflare-0.0.5/Solarflare/nightcalc.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 import math
 import datetime
 
 LUNAR_MONTH = 29.530588853
+def sin(x): return math.sin(math.radians(x))
+def cos(x): return math.cos(math.radians(x))
+def tan(x): return math.tan(math.radians(x))
+def acos(x): return math.degrees(math.acos(x))
+def asin(x): return math.degrees(math.asin(x))
+def atan2(y, x): return math.degrees(math.atan2(y, x))
 
 def get_julian_date(date=None):
     """Returns the Julian date for the given date."""
     if date is None:
         date = datetime.datetime.utcnow()
     time = date.timestamp() # seconds since epoch
     tzoffset = date.utcoffset().total_seconds() / 60 if date.utcoffset() else 0 # minutes
@@ -101,14 +107,35 @@
     sep22 = datetime.datetime(year, 9, autumn)
     full_moon_after = next_full_moon(sep22)
     full_moon_before = previous_full_moon(sep22)
     if abs(full_moon_after - sep22) < abs(sep22 - full_moon_before):
         return full_moon_after
     else:
         return full_moon_before
+    
+def lunar_coordinates(date=datetime.datetime.now()):
+    jd = get_julian_date(date)
+    d = jd - 2451545
+    L = 218.316  + 13.176396 * (d)
+    M = 134.963 + 13.064993 * (d)
+    F = 93.272 + 13.229350 * (d)
+    long = L + 6.289 * sin(M)
+    latitude = 5.128 * sin(F)
+    dist = 385001 - 20905 * cos(M)
+    return (latitude, long, dist)
+
+def lunar_ra(date=datetime.datetime.now()):
+    lat, long, dist = lunar_coordinates(date)
+    a = atan2(sin(long) * cos(23.4397) - tan(lat) * sin(23.4397), cos(long))
+    return a
+
+def lunar_dec(date=datetime.datetime.now()):
+    B, la, dist = lunar_coordinates(date)
+    dec = asin(sin(B) * cos(23.4397) + cos(B) * sin(23.4397) * sin(la))
+    return dec
 
 class Moon:
     def __init__(self, latitude, longitude):
         self.lat = latitude
         self.long = longitude
 
     def upcoming_harvest_moon(self): return harvest_moon()
```

### Comparing `Solarflare-0.0.4/Solarflare/solarflare.py` & `Solarflare-0.0.5/Solarflare/solarflare.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 def tan(x): return math.tan(math.radians(x))
 def acos(x): return math.degrees(math.acos(x))
 def asin(x): return math.degrees(math.asin(x))
 def atan2(y, x): return math.degrees(math.atan2(y, x))
 
 # Version function
 def VERSION():
-    return "0.0.4"
+    return "0.0.5"
 
 # 1. TIME
 # for these calculations, it is convenient to use Julian dates.
 def julian_date(date=datetime.datetime.now()):
     time = date.timestamp() * 1000
     tzoffset = date.utcoffset().total_seconds() // 60 if date.utcoffset() else 0
     return (time / 86400000) - (tzoffset / 1440) + 2440587.5
```

### Comparing `Solarflare-0.0.4/setup.py` & `Solarflare-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='Solarflare',
-    version='0.0.4',
+    version='0.0.5',
     author='Siddhu Pendyala',
     author_email='elcientifico.pendyala@gmail.com',
     description='A Python library that deals with solar calculations',
     long_description = long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/PyndyalaCoder/Solarflare',
     project_urls = {
```

