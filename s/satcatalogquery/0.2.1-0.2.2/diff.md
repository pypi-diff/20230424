# Comparing `tmp/satcatalogquery-0.2.1-py3-none-any.whl.zip` & `tmp/satcatalogquery-0.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 16549 bytes, number of entries: 12
--rw-r--r--  2.0 unx      362 b- defN 22-Dec-29 04:27 satcatalogquery/Const.py
--rw-r--r--  2.0 unx      206 b- defN 23-Jan-04 10:48 satcatalogquery/__init__.py
--rw-r--r--  2.0 unx     6251 b- defN 23-Jan-02 12:12 satcatalogquery/data_download.py
--rw-r--r--  2.0 unx      339 b- defN 22-Dec-30 01:04 satcatalogquery/data_prepare.py
--rw-r--r--  2.0 unx    37141 b- defN 23-Jan-02 13:44 satcatalogquery/query.py
--rw-r--r--  2.0 unx     5339 b- defN 23-Jan-05 02:10 satcatalogquery/satcatclass.py
--rw-r--r--  2.0 unx      461 b- defN 22-Dec-29 05:56 satcatalogquery/try_download.py
--rw-r--r--  2.0 unx     1068 b- defN 23-Jan-05 02:21 satcatalogquery-0.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     5027 b- defN 23-Jan-05 02:21 satcatalogquery-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-05 02:21 satcatalogquery-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jan-05 02:21 satcatalogquery-0.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1021 b- defN 23-Jan-05 02:21 satcatalogquery-0.2.1.dist-info/RECORD
-12 files, 57323 bytes uncompressed, 14819 bytes compressed:  74.1%
+Zip file size: 19089 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      304 b- defN 23-Apr-23 08:30 satcatalogquery/Const.py
+-rw-r--r--  2.0 unx       98 b- defN 23-Apr-24 03:34 satcatalogquery/__init__.py
+-rw-r--r--  2.0 unx    22975 b- defN 23-Apr-24 09:07 satcatalogquery/classes.py
+-rw-r--r--  2.0 unx     6395 b- defN 23-Apr-24 09:26 satcatalogquery/data_download.py
+-rw-r--r--  2.0 unx      355 b- defN 23-Apr-23 08:35 satcatalogquery/data_prepare.py
+-rw-r--r--  2.0 unx    36773 b- defN 23-Apr-24 04:24 satcatalogquery/query.py
+-rw-r--r--  2.0 unx      457 b- defN 23-Apr-23 08:53 satcatalogquery/try_download.py
+-rw-r--r--  2.0 unx     1068 b- defN 23-Apr-24 09:48 satcatalogquery-0.2.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5488 b- defN 23-Apr-24 09:48 satcatalogquery-0.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-24 09:48 satcatalogquery-0.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Apr-24 09:48 satcatalogquery-0.2.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1017 b- defN 23-Apr-24 09:48 satcatalogquery-0.2.2.dist-info/RECORD
+12 files, 75038 bytes uncompressed, 17367 bytes compressed:  76.9%
```

## zipnote {}

```diff
@@ -1,37 +1,37 @@
 Filename: satcatalogquery/Const.py
 Comment: 
 
 Filename: satcatalogquery/__init__.py
 Comment: 
 
+Filename: satcatalogquery/classes.py
+Comment: 
+
 Filename: satcatalogquery/data_download.py
 Comment: 
 
 Filename: satcatalogquery/data_prepare.py
 Comment: 
 
 Filename: satcatalogquery/query.py
 Comment: 
 
-Filename: satcatalogquery/satcatclass.py
-Comment: 
-
 Filename: satcatalogquery/try_download.py
 Comment: 
 
-Filename: satcatalogquery-0.2.1.dist-info/LICENSE
+Filename: satcatalogquery-0.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: satcatalogquery-0.2.1.dist-info/METADATA
+Filename: satcatalogquery-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: satcatalogquery-0.2.1.dist-info/WHEEL
+Filename: satcatalogquery-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: satcatalogquery-0.2.1.dist-info/top_level.txt
+Filename: satcatalogquery-0.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: satcatalogquery-0.2.1.dist-info/RECORD
+Filename: satcatalogquery-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## satcatalogquery/Const.py

```diff
@@ -1,7 +1,7 @@
 # basic physical constants for the Reference Earth Model - WGS84
 mu = 398600.4418 # GM, [km^3/s^2]  
-Re = 6378.137 # Equatorial radius of the Earth from WGS84 ellipsoid model, [km]
-f = 1/298.257223563 # flattening
-Re_V = 6371.0008 # volumetric radius, [km] 
-rot = 7.292115e-5 # Rotational speed of the Earth from WGS84 ellipsoid model, [rad/s]
-J2 = 1.08262982e-3
+Re = 6378.137 # Equatorial radius, [km]
+f = 1/298.257223563 # Flatness
+Re_V = 6371.0008 # Volumetric radius, [km] 
+rot = 7.292115e-5 # Spin angular velocity, [rad/s]
+J2 = 1.08262982e-3 # Dynamic flatness
```

## satcatalogquery/__init__.py

```diff
@@ -1,7 +1,3 @@
 from . import data_prepare
-from .satcatclass import SatCatlog
-from .query import discos_query,celestrak_query,targets_query
-
-# Load and update the files
-data_prepare.satcat_load() 
-data_prepare.qsmag_load()
+from .classes import SatCatalog
+from .data_download import download_tle
```

## satcatalogquery/data_download.py

```diff
@@ -8,21 +8,21 @@
 from colorama import Fore
 from time import sleep
 
 from .try_download import wget_download
 
 def download_satcat():
     """
-    Download or update the satellites catalog file from www.celestrak.com
+    Download or update the spatial objects catalog file from www.celestrak.com
 
     Usage: 
-    scfile = download_satcat()
+        scfile = download_satcat()
     
     Outputs: 
-    scfile -> [str] Local path of the satellites catalog file
+        scfile -> [str] Path of the spatial objects catalog file
     """
     home = str(Path.home())
     direc = home + '/src/satcat-data/'
     
     scfile = direc + 'satcat.csv'
     url = 'https://celestrak.com/pub/satcat.csv'
 
@@ -38,21 +38,21 @@
             wget_out = wget_download(url,scfile,desc) 
         else:
             print('The satellite catalog in {:s} is already the latest.'.format(direc))    
     return scfile
 
 def download_qsmag():
     """
-    Download or update the file which records the standard(intrinsic) magnitude for satellites from https://www.prismnet.com/~mmccants/programs/qsmag.zip
+    Download or update the file which records the standard(intrinsic) magnitude for space objects from https://www.prismnet.com/~mmccants/programs/qsmag.zip
     
     Usage: 
-    qsfile = download_qsmag()
+        qsfile = download_qsmag()
     
     Outputs: 
-    qsfile -> [str] Local path of the qs.mag file
+        qsfile -> [str] Path of the qs.mag file
     """
     home = str(Path.home())
     direc = home + '/src/satcat-data/'
     
     qsfile_zip = direc + 'qsmag.zip'
     qsfile = direc + 'qs.mag'
     url = 'https://www.prismnet.com/~mmccants/programs/qsmag.zip'
@@ -79,32 +79,32 @@
     return qsfile
 
 def download_tle(noradids,mode='keep',dir_TLE='TLE/'):
     """
     Download the TLE/3LE data from [SPACETRACK](https://www.space-track.org) automatically
 
     Usage: 
-    tlefile = tle_download(noradids)
-    tlefile = tle_download(noradids,'clear')
-    tlefile = tle_download('satno.txt')
+        tle_file = tle_download(noradids)
+        tle_file = tle_download(noradids,'clear')
+        tle_file = tle_download('satno.txt')
 
     Inputs:
-    noradids -> [str, int, list of str/int] NORADID of space targets. 
-    It can be a single NORADID, list of NORADID, or a file containing a set of NORADID.
-    The form and format of the file is as follows:
-    #satno
-    12345
-    23469
-    ...
+        noradids -> [str, int, list of str/int] NORADID of space targets. 
+        It can be a single NORADID, list of NORADID, or a file containing a set of NORADID.
+        The form and format of the file is as follows:
+        #satno
+        12345
+        23469
+        ...
 
-    Parameters:
-    mode -> [str,default='keep'] either keep the files stored in TLE directory or clear the TLE directory 
+        mode -> [str,optional,default='keep'] Either 'keep' the files stored in TLE directory or 'clear' the TLE directory 
+        dir_TLE -> [str,optional,default='TLE/'] Path to save TLE
 
     Outputs: 
-    tlefile  -> [str] Path of TLE/3LE file.
+        tle_file  -> [str] Path of TLE/3LE file.
     """
     # Check whether a list is empty or not
     if not noradids: raise Exception('noradids is empty.')
 
     if type(noradids) is list:
         if type(noradids[0]) is int: noradids = [str(i) for i in noradids]    
     else:
@@ -161,14 +161,15 @@
         for line in lines_tle:
             words = line.split()
             if words[0] == '2': valid_ids.append(words[1].lstrip('0'))
             file_tle.write(line+'\n')
         sleep(j+5) 
         j += 1   
     file_tle.close()
+    print()
 
     missed_ids = list(set(noradids)-set(valid_ids))
     if missed_ids: 
         missed_ids_filename = dir_TLE + 'missed_ids_{:s}.txt'.format(date_str)
         desc = '{:s}Note: space targets with unavailable TLE are stored in {:s}.{:s} '.format(Fore.RED,missed_ids_filename,Fore.RESET)
         print(desc) 
         np.savetxt(missed_ids_filename,missed_ids,fmt='%s')
```

## satcatalogquery/data_prepare.py

```diff
@@ -1,19 +1,19 @@
 from .data_download import download_satcat, download_qsmag
 
 def satcat_load():
     """
-    load the sats catalog file from CelesTrak
+    load the spatial objects catalog file from CelesTrak
     """
     global sc_file
 
     sc_file = download_satcat()
 
 def qsmag_load():
     """
-    load the standard(intrinsic) magnitude for satellites
+    load the standard(intrinsic) magnitude for spatial objects
     """
     global qs_file
 
     qs_file = download_qsmag()
```

## satcatalogquery/query.py

```diff
@@ -5,67 +5,65 @@
 import requests
 from datetime import datetime
 from time import sleep
 from colorama import Fore
 
 from . import Const
 from . import data_prepare
-from .satcatclass import SatCatlog
 
 
 def _discos_buildin_filter(params,expr):
     """
     A buildin function associated to the function discos_query. 
 
     Inputs:
-    params -> [dictionary] params in function discos_query
-    expr -> [str] filter expressions for DISCOS, for example, "eq(reentry.epoch,null)". 
+        params -> [dictionary] Parameters in function discos_query
+        expr -> [str] Filter expressions for DISCOS database query, for example, "eq(reentry.epoch,null)". 
 
     Outputs:
-    params_upgrade -> [dictionary] upgraded variable params in function discos_query    
+        params_upgrade -> [dictionary] upgraded parameters in function discos_query    
 
     For more infomation, please reference to https://discosweb.esoc.esa.int/apidocs
-
     """
     if 'filter' in params.keys(): 
         params['filter'] += '&(' + expr + ')'
     else:
         params['filter'] = expr 
     return params  
 
-def discos_query(COSPAR_ID=None,NORAD_ID=None,OBJECT_CLASS=None,PAYLOAD=None,DECAYED=None,DECAY_DATE=None,MASS=None,SHAPE=None,LENGTH=None,HEIGHT=None,DEPTH=None,RCSMin=None,RCSMax=None,RCSAvg=None,sort=None):
+def _discos_query(COSPAR_ID=None,NORAD_ID=None,OBJECT_CLASS=None,PAYLOAD=None,DECAYED=None,DECAY_DATE=None,MASS=None,SHAPE=None,LENGTH=None,HEIGHT=None,DEPTH=None,RCSMin=None,RCSMax=None,RCSAvg=None,sort=None):
     """
-    Query space targets by setting a series of specific parameters from the [DISCOS](https://discosweb.esoc.esa.int)(Database and Information System Characterising Objects in Space) database.
+    Given the geometric constraints of a spatial object, query the qualified spatial objects from the [DISCOS](https://discosweb.esoc.esa.int)(Database and Information System Characterising Objects in Space) database.
 
     Usage: 
-    satcatlog = discos_query(DECAYED=False,RCSAvg=[5,15])
+        satcatalog_df = discos_query(DECAYED=False,RCSAvg=[5,15])
 
-    Parameters:
-    COSPAR_ID -> [str or list of str, optional, default = None] Target IDs by the in Committee On SPAce Research; if None, this option is ignored. 
-    NORAD_ID -> [int, str, list, or filename(such as noradids.txt), optional, default = None] Target IDs by the North American Aerospace Defense Command; if None, this option is ignored.
-    OBJECT_CLASS -> [str or list of str, optional, default = None] Classification of targets; avaliable options include 'Payload', 'Payload Debris', 'Payload Fragmentation Debris', 
-    'Payload Mission Related Object', 'Rocket Body', 'Rocket Debris', 'Rocket Fragmentation Debris', 'Rocket Mission Related Object', 'Other Mission Related Object','Other Debris', Unknown', or any combination of them, 
-    for examle, ['Rocket Body', 'Rocket Debris', 'Rocket Fragmentation Debris']; If None, this option is ignored.  
-    PAYLOAD -> [bool, optional, default  = None] Identify whether a target belongs to payload or not. If True, payload; if False, non-payload; if None, this option is ignored.
-    DECAYED -> [bool, optional, default = None] it also called reentry; If False, targets are still in orbit by now; if True, then reentry; if None, this option is ignored.
-    DECAY_DATE -> [list of str with 2 elemnts, optional, default = None] Date of reentry; it must be in form of ['date1','date2'], such as ['2019-01-05','2020-05-30']; if None, then this option is ignored.
-    MASS -> [list of float with 2 elemnts, optional, default = None] Mass[kg] of a target; it must be in form of [m1,m2], such as [5.0,10.0]; if None, this option is ignored.
-    SHAPE -> [str or list of str, optional, default = None] Shape of targets; commonly used options include 'Cyl', 'Sphere', 'Cone', 'Dcone', Pan', 'Ell', 'Dish', 'Cable', 'Box', 'Rod', 'Poly', 'Sail', 'Ant', 
-    'Frust', 'Truss', 'Nozzle', and 'lrr'. Any combinations of them are also supported, for examle, ['Cyl', 'Sphere', 'Pan'] means 'or', and ['Cyl', 'Sphere', 'Pan', '+'] means 'and'; If None, this option is ignored.  
-    LENGTH -> [list of float with 2 elemnts, optional, default = None] Length[m] of a target; it must be in form of [l1,l2], such as [5.0,10.0]; if None, this option is ignored.
-    HEIFHT -> [list of float with 2 elemnts, optional, default = None] Height[m] of a target; it must be in form of [h1,h2], such as [5.0,10.0]; if None, this option is ignored.
-    DEPTH -> [list of float with 2 elemnts, optional, default = None] Depth[m] of a target; it must be in form of [d1,d2], such as [5.0,10.0]; if None, this option is ignored.
-    RCSMin -> [list of float with 2 elemnts, optional, default = None] Minimum Radar Cross Section[m2] of a target; it must be in form of [RCS1,RCS2], such as [0.5,2.0]; if None, this option is ignored.
-    RCSMax -> [list of float with 2 elemnts, optional, default = None] Maximum Radar Cross Section[m2] of a target; it must be in form of [RCS1,RCS2], such as [10.0,100.0]; if None, this option is ignored.
-    RCSAvg -> [list of float with 2 elemnts, optional, default = None] Average Radar Cross Section[m2] of a target; it must be in form of [RCS1,RCS2], such as [5,20]; if None, this option is ignored.
-    sort -> [str, optional, default = None] sort by features of targets in a specific order, such as by mass; avaliable options include 'COSPARID', NORADID', 'ObjectClass', 'DecayDate', 'Mass', 'Shape', 'Length', 'Height', 'Depth', 'RCSMin', 'RSCMax', and 'RCSAvg'.
-    If there is a negative sign '-' ahead, such as "-Mass", it will be sorted in descending order. If None, then sort by NORADID by default.
+    Inputs:
+        COSPAR_ID -> [str or list of str, optional, default = None] object IDs defined by the Committee On SPAce Research; if None, this option is ignored. 
+        NORAD_ID -> [int, str, list, or filename(such as 'noradids.txt'), optional, default = None] object IDs defined by the North American Aerospace Defense Command; if None, this option is ignored.
+        OBJECT_CLASS -> [str, list of str, optional, default = None] Classification of objects; available options are 'Payload', 'Payload Debris', 'Payload Fragmentation Debris', 
+        'Payload Mission Related Object', 'Rocket Body', 'Rocket Debris', 'Rocket Fragmentation Debris', 'Rocket Mission Related Object', 'Other Mission Related Object','Other Debris', Unknown', or any combination of them, 
+        for example, ['Rocket Body', 'Rocket Debris', 'Rocket Fragmentation Debris']; If None, this option is ignored.  
+        PAYLOAD -> [bool, optional, default = None] Whether an object is payload or not. If True, the object is a payload; if False, not a payload; if None, this option is ignored.
+        DECAYED -> [bool, optional, default = None] Whether an object is  decayed(re-entry) or not; If False, the object is still in orbit by now; if True, then decayed; if None, this option is ignored.
+        DECAY_DATE -> [list of str, optional, default = None] Date range of decay; it must be in form of ['date1','date2'], such as ['2019-01-05','2020-05-30']; if None, then this option is ignored.
+        MASS -> [list of float, optional, default = None] Mass[kg] range of an object; it must be in form of [m1,m2], such as [5.0,10.0]; if None, this option is ignored.
+        SHAPE -> [str or list of str, optional, default = None] Shape of an object; the usual choices include 'Cyl', 'Sphere', 'Cone', 'Dcone', Pan', 'Ell', 'Dish', 'Cable', 'Box', 'Rod', 'Poly', 'Sail', 'Ant', 
+        'Frust', 'Truss', 'Nozzle', and 'lrr'. Any combination of them is also supported, for examle, ['Cyl', 'Sphere', 'Pan'] means 'or', and ['Cyl', 'Sphere', 'Pan', '+'] means 'and'; If None, this option is ignored.  
+        LENGTH -> [list of float, optional, default = None] Length[m] range of an object; it must be in form of [l1,l2], such as [5.0,10.0]; if None, this option is ignored.
+        HEIFHT -> [list of float, optional, default = None] Height[m] range of an object; it must be in form of [h1,h2], such as [5.0,10.0]; if None, this option is ignored.
+        DEPTH -> [list of float, optional, default = None] Depth[m] range of an object; it must be in form of [d1,d2], such as [5.0,10.0]; if None, this option is ignored.
+        RCSMin -> [list of float, optional, default = None] Minimum Radar Cross Section(RCS)[m2] of an object; if None, this option is ignored.
+        RCSMax -> [list of float, optional, default = None] Maximum Radar Cross Section(RCS)[m2] of an object; if None, this option is ignored.
+        RCSAvg -> [list of float, optional, default = None] Average Radar Cross Section(RCS)[m2] of an object; if None, this option is ignored.
+        sort -> [str, optional, default = None] Sort according to attributes of spatial objects, such as mass; available options include 'COSPARID', NORADID', 'ObjectClass', 'DecayDate', 'Mass', 'Shape', 'Length', 'Height', 'Depth', 'RCSMin', 'RSCMax', and 'RCSAvg'.
+        If the attribute is prefixed with a '-', such as '-Mass', it will be sorted in descending order. If None, the spatial objects are sorted by NORADID by default.
     
     Outputs:
-    satcatlog -> instance of class SatCatlog
+        satcatalog_df -> Data frame containing the selected spatial objects
     """
     # DISCOS tokens
     home = str(Path.home())
     direc = home + '/src/discos-data/'
     tokenfile = direc + 'discos-token'
 
     if not path.exists(direc): makedirs(direc)
@@ -270,46 +268,47 @@
     old_column = ['height', 'xSectMax', 'name', 'satno', 'objectClass','mass', 'xSectMin', 'depth', 'xSectAvg', 'length', 'shape', 'cosparId']
     new_column = ['HEIGhT', 'RCSMax', 'OBJECT_NAME', 'NORAD_ID', 'OBJECT_CLASS', 'MASS', 'RCSMin[m2]', 'DEPTH', 'RCSAvg', 'LENGTH', 'SHAPE', 'COSPAR_ID']
     # units: MASS in [kg]; RCS in [m2]; DEPTH, LENGTH, and HEIGHT in [m]
     new_column_reorder = ['OBJECT_NAME','COSPAR_ID', 'NORAD_ID','OBJECT_CLASS','MASS','SHAPE','HEIGHT','LENGTH','DEPTH','RCSMin','RCSMax','RCSAvg']
     df = pd.DataFrame.from_dict(extract,dtype=object).rename(columns=dict(zip(old_column, new_column)), errors='raise')
     df = df.reindex(columns=new_column_reorder) 
     df = df.reset_index(drop=True)
-    mode = 'discos_catlog'
-
-    return SatCatlog(df,mode)   
+    
+    return df 
 
-def celestrak_query(COSPAR_ID=None,NORAD_ID=None,PAYLOAD=None,DECAYED=None,DECAY_DATE=None,PERIOD=None,INCLINATION=None,APOGEE=None,PERIGEE=None,MEAN_ALT=None,ECC=None,OWNER=None,TLE_STATUS=None,sort=None):
+def _celestrak_query(COSPAR_ID=None,NORAD_ID=None,PAYLOAD=None,DECAYED=None,DECAY_DATE=None,PERIOD=None,INCLINATION=None,APOGEE=None,PERIGEE=None,MEAN_ALT=None,ECC=None,OWNER=None,TLE_STATUS=None,sort=None):
     """
-    Query space targets that meet the requirements by setting a series of specific parameters from the [CELESTRAK](https://celestrak.com) database.
+    Given the orbital constraints of a space object, query the qualified space objects from the [CELESTRAK](https://celestrak.com) database.
 
     Usage:
-    satcatlog = celestrak_query(DECAYED=False,MEAN_ALT=[400,900])
+        satcatalog_df = celestrak_query(DECAYED=False,MEAN_ALT=[400,900])
 
-    Parameters:
-    COSPAR_ID     -> [str or list of str, optional, default = None] Target IDs by the in Committee On SPAce Research; if None, this option is ignored.
-    NORAD_ID      -> [int, str, list, or filename(such as noradids.txt), optional, default = None] Target IDs by the North American Aerospace Defense Command; if None, this option is ignored.
-    PAYLOAD       -> [bool, optional, default = None] Identify whether a target belongs to payload or not. If True, payload; if False, non-payload; if None, this option is ignored.
-    DECAYED       -> [bool, optional, default = None] It also called reentry; if False, targets are still in orbit by now; if True, then reentry; if None, this option is ignored.
-    DECAY_DATE    -> [list of str with 2 elemnts, optional, default = None] Date of reentry; it must be in form of ['date1','date2'], such as ['2019-01-05','2020-05-30']; if None, this option is ignored.
-    PERIOD        -> [list of float with 2 elemnts, optional, default = None] Orbit period[minutes] of targets; it must be in form of [period1,period2], such as [100.0,200.0]; if None, this option is ignored.  
-    INCLINATION   -> [list of float with 2 elemnts, optional, default = None] Orbit inclination[degrees] of targets; must be in form of [inc1,inc2], such as [45.0,80.0]; if None, this option is ignored.  
-    APOGEE        -> [list of float with 2 elemnts, optional, default = None] Apogee Altitude[km] of targets; it must be in form of [apoalt1,apoalt2], such as [800.0,1400.0]; if None, this option is ignored.  
-    PERIGEE       -> [list of float with 2 elemnts, optional, default = None] Perigee Altitude[km] of targets; it must be in form of [peralt1,peralt2], such as [300.0,400.0]; if None, this option is ignored.  
-    MEAN_ALT      -> [list of float with 2 elemnts, optional, default = None] Mean Altitude[km] of targets; it must be in form of [meanalt1,meanalt2], such as [300.0,800.0]; if None, then option is ignored. 
-    ECC           -> [list of float with 2 elemnts, optional, default = None] Eccentricity of targets; it must be in form of [ecc1,ecc2], such as [0.01,0.2]; if None, then option is ignored.   
-    OWNER         -> [str or list of str, optional, default = None] Satellite Ownership; country codes/names can be found at http://www.fao.org/countryprofiles/iso3list/en/; if None, this option is ignored.
-    TLE_STATUS    -> [bool, optional, default = None] Identify whether a TLE is valid. If True, TLE is valid; if False, No Current Elements, No Initial Elements, or No Elements Available; if None, this option is ignored.
-    sort          -> [str, optional, default = None] sort by features of targets in a specific order; avaliable options include 'COSPAR_ID', NORAD_ID', 'DECAY_DATE', 'PERIOD', 'INCLINATION', 'APOGEE', 'PERIGEE', 'MEAN_ALT', 'ECC',and 'OWNER'.
-    If there is a negative sign '-' ahead, such as "-DecayDate", it will be sorted in descending order. If None, then sort by NORADID by default.
+    Inputs:
+        COSPAR_ID -> [str or list of str, optional, default = None] object IDs defined by the Committee On SPAce Research; if None, this option is ignored. 
+        NORAD_ID -> [int, str, list, or filename(such as 'noradids.txt'), optional, default = None] object IDs defined by the North American Aerospace Defense Command; if None, this option is ignored.
+        PAYLOAD -> [bool, optional, default = None] Whether an object is payload or not. If True, the object is a payload; if False, not a payload; if None, this option is ignored.
+        DECAYED -> [bool, optional, default = None] Whether an object is  decayed(re-entry) or not; If False, the object is still in orbit by now; if True, then decayed; if None, this option is ignored.
+        DECAY_DATE -> [list of str, optional, default = None] Date range of decay; it must be in form of ['date1','date2'], such as ['2019-01-05','2020-05-30']; if None, then this option is ignored.
+        PERIOD -> [list of float, optional, default = None] Orbital period[minutes] range of a space object; it must be in form of [period1,period2], such as [100.0,200.0]; if None, this option is ignored.  
+        INCLINATION -> [list of float, optional, default = None] Range of inclination[degrees] of a space object; it must be in form of [inc1,inc2], such as [45.0,80.0]; if None, this option is ignored.  
+        APOGEE -> [list of float, optional, default = None] Range of Apogee Altitude[km]; it must be in form of [apoalt1,apoalt2], such as [800.0,1400.0]; if None, this option is ignored.  
+        PERIGEE -> [list of float, optional, default = None] Range of Perigee Altitude[km]; it must be in form of [peralt1,peralt2], such as [300.0,400.0]; if None, this option is ignored.  
+        MEAN_ALT -> [list of float, optional, default = None] Mean Altitude[km] of objects; it must be in form of [meanalt1,meanalt2], such as [300.0,800.0]; if None, then option is ignored. 
+        ECC -> [list of float, optional, default = None] Range of Eccentricity; it must be in form of [ecc1,ecc2], such as [0.01,0.2]; if None, then option is ignored.   
+        OWNER -> [str or list of str, optional, default = None] Ownership of a space object; and country codes/names can be found at http://www.fao.org/countryprofiles/iso3list/en/; if None, this option is ignored.
+        TLE_STATUS -> [bool, optional, default = None] Whether a TLE is valid. If False, it means No Current Elements, No Initial Elements, or No Elements Available; if None, this option is ignored.
+        sort -> [str, optional, default = None] Sort according to attributes of a spatial object, such as MEAN_ALT; available options include 'COSPAR_ID', NORAD_ID', 'DECAY_DATE', 'PERIOD', 'INCLINATION', 'APOGEE', 'PERIGEE', 'MEAN_ALT', 'ECC',and 'OWNER'.
+        If the attribute is prefixed with a '-', such as '-DecayDate', it will be sorted in descending order. If None, the spatial objects are sorted by NORADID by default.
     
     Outputs:
-    satcatlog -> instance of class SatCatlog
-    """
+        satcatalog_df -> Data frame containing the selected spatial objects
+    """  
 
+    # Load and update the satcat files from the [CELESTRAK](https://celestrak.com) database.
+    data_prepare.satcat_load()
     satcat_file = data_prepare.sc_file
 
     data = pd.read_csv(satcat_file) 
     columns_dict = {'OBJECT_ID': 'COSPAR_ID', 'NORAD_CAT_ID': 'NORAD_ID'}
     data.rename(columns=columns_dict, inplace=True)
     # unit description : 'PERIOD' in [min],'INCLINATION' in [deg], 'APOGEE' in [km],'PERIGEE' in [km],'RCS' in [m2]
 
@@ -479,76 +478,76 @@
         elif sort.__contains__('RCS'):
             df = df.sort_values(by=['RCS'],ascending=ascending_flag)    
         elif sort.__contains__('OWNER'):
             df = df.sort_values(by=['OWNER'],ascending=ascending_flag)
         else:
             raise Exception("Avaliable options include 'COSPAR_ID', NORAD_ID', 'DECAY_DATE', 'PERIOD', 'INCLINATION', 'APOGEE', 'PERIGEE', 'MEAN_ALT', 'ECC', 'LAUNCH_DATE', 'LAUNCH_SITE', 'RCS', and 'OWNER'. Also, a negative sign '-' can be added ahead to the option to sort in descending order.")
     df = df.reset_index(drop=True)
-    mode = 'celestrak_catlog'
 
-    return SatCatlog(df,mode)
+    return df
 
 def parseQSMagFile():
-    '''
-    Read and parse the qs.mag file for getting noradid and standard(intrinsic) magnitude for satellites.
-    '''
+    """
+    Get the noradid and standard(intrinsic) magnitude for space objects by reading and parsing the qs.mag file.
+    """
+
+    # Load and update the QSMag files from https://www.prismnet.com/~mmccants/programs/qsmag.zip
+    data_prepare.qsmag_load()
     qsfile = data_prepare.qs_file
 
     qsmag = np.genfromtxt(qsfile,skip_header=1,skip_footer=1,delimiter=[5,28,5],dtype=(int,str,float)) 
     df_qsmag = pd.DataFrame(qsmag).drop(columns=['f1']).rename(columns={"f0": "NORAD_ID", "f2": "StdMag"})
     return df_qsmag         
 
-def targets_query(COSPAR_ID=None,NORAD_ID=None,PAYLOAD=None,OBJECT_CLASS=None,DECAYED=None,DECAY_DATE=None,PERIOD=None,INCLINATION=None,APOGEE=None,PERIGEE=None,MEAN_ALT=None,ECC=None,TLE_STATUS=None,MASS=None,SHAPE=None,LENGTH=None,HEIGHT=None,DEPTH=None,RCSMin=None,RCSMax=None,RCSAvg=None,OWNER=None,sort=None):
+def _objects_query(COSPAR_ID=None,NORAD_ID=None,PAYLOAD=None,OBJECT_CLASS=None,DECAYED=None,DECAY_DATE=None,PERIOD=None,INCLINATION=None,APOGEE=None,PERIGEE=None,MEAN_ALT=None,ECC=None,TLE_STATUS=None,MASS=None,SHAPE=None,LENGTH=None,HEIGHT=None,DEPTH=None,RCSMin=None,RCSMax=None,RCSAvg=None,OWNER=None,sort=None):
     """
-    Query space targets that meet the requirements by setting a series of specific parameters from the the [DISCOS](https://discosweb.esoc.esa.int)(Database and Information System Characterising Objects in Space) database and the [CELESTRAK](https://celestrak.com) database.
+    Given the geometric and orbital constraints of a space object, query the qualified space objects from the [DISCOS](https://discosweb.esoc.esa.int)(Database and Information System Characterising Objects in Space) database and the [CELESTRAK](https://celestrak.com) database.
 
     Usage: 
-    satcatlog = targets_query(PAYLOAD=False,DECAYED=False,MEAN_ALT=[400,900],RCSAvg=[5,15])
+        satcatalog_df = objects_query(PAYLOAD=False,DECAYED=False,MEAN_ALT=[400,900],RCSAvg=[5,15])
 
-    Parameters:
-    COSPAR_ID     -> [str or list of str, optional, default = None] Target IDs by the in Committee On SPAce Research; if None, this option is ignored.
-    NORAD_ID      -> [int, str, list, or filename(such as noradids.txt), optional, default = None] Target IDs by the North American Aerospace Defense Command; if None, this option is ignored.
-    PAYLOAD       -> [bool, optional, fafault = None] Identify whether a target belongs to payload or not. If True, then targets belong to payload; if False, then non-payload; if None, then this option is ignored.
-    OBJECT_CLASS  -> [str or list of str, optional, default = None] Classification of targets; avaliable options include 'Payload', 'Payload Debris', 'Payload Fragmentation Debris', 
-    'Payload Mission Related Object', 'Rocket Body', 'Rocket Debris', 'Rocket Fragmentation Debris', 'Rocket Mission Related Object', 'Other Mission Related Object','Other Debris', Unknown', or any combination of them, 
-    for examle, ['Rocket Body', 'Rocket Debris', 'Rocket Fragmentation Debris']; If None, this option is ignored.
-    
-    DECAYED       -> [bool, optional, default = None] it also called reentry; If False, targets are still in orbit by now; if True, then reentry; if None, this option is ignored.
-    DECAY_DATE    -> [list of str with 2 elemnts, optional, default = None] Date of reentry; it must be in form of ['date1','date2'], such as ['2019-01-05','2020-05-30']; if None, then this option is ignored.
-    PERIOD        -> [list of float with 2 elemnts, optional, default = None] Orbit period[minutes] of targets; it must be in form of [period1,period2], such as [100.0,200.0]; if None, this option is ignored.  
-    INCLINATION   -> [list of float with 2 elemnts, optional, default = None] Orbit inclination[degrees] of targets; must be in form of [inc1,inc2], such as [45.0,80.0]; if None, this option is ignored.  
-    APOGEE        -> [list of float with 2 elemnts, optional, default = None] Apogee Altitude[km] of targets; it must be in form of [apoalt1,apoalt2], such as [800.0,1400.0]; if None, this option is ignored.  
-    PERIGEE       -> [list of float with 2 elemnts, optional, default = None] Perigee Altitude[km] of targets; it must be in form of [peralt1,peralt2], such as [300.0,400.0]; if None, this option is ignored.  
-    MEAN_ALT      -> [list of float with 2 elemnts, optional, default = None] Mean Altitude[km] of targets; it must be in form of [meanalt1,meanalt2], such as [300.0,800.0]; if None, then option is ignored. 
-    ECC           -> [list of float with 2 elemnts, optional, default = None] Eccentricity of targets; it must be in form of [ecc1,ecc2], such as [0.01,0.2]; if None, then option is ignored.   
-    TLE_STATUS    -> [bool, optional, default = None] Identify whether a TLE is valid. If True, TLE is valid; if False, No Current Elements, No Initial Elements, or No Elements Available; if None, this option is ignored.
-    MASS          -> [list of float with 2 elemnts, optional, default = None] Mass[kg] of a target; it must be in form of [m1,m2], such as [5.0,10.0]; if None, this option is ignored.
-    SHAPE -> [str or list of str, optional, default = None] Shape of targets; commonly used options include 'Cyl', 'Sphere', 'Cone', 'Dcone', Pan', 'Ell', 'Dish', 'Cable', 'Box', 'Rod', 'Poly', 'Sail', 'Ant', 
-    'Frust', 'Truss', 'Nozzle', and 'lrr'. Any combinations of them are also supported, for examle, ['Cyl', 'Sphere', 'Pan'] means 'or', and ['Cyl', 'Sphere', 'Pan', '+'] means 'and'; If None, this option is ignored.  
-    LENGTH        -> [list of float with 2 elemnts, optional, default = None] Length[m] of a target; it must be in form of [l1,l2], such as [5.0,10.0]; if None, this option is ignored.
-    HEIGHT        -> [list of float with 2 elemnts, optional, default = None] Height[m] of a target; it must be in form of [h1,h2], such as [5.0,10.0]; if None, this option is ignored.
-    DEPTH         -> [list of float with 2 elemnts, optional, default = None] Depth[m] of a target; it must be in form of [d1,d2], such as [5.0,10.0]; if None, this option is ignored.
-    RCSMin        -> [list of float with 2 elemnts, optional, default = None] Minimum Radar Cross Section[m2] of a target; it must be in form of [RCS1,RCS2], such as [0.5,2.0]; if None, this option is ignored.
-    RCSMax        -> [list of float with 2 elemnts, optional, default = None] Maximum Radar Cross Section[m2] of a target; it must be in form of [RCS1,RCS2], such as [10.0,100.0]; if None, this option is ignored.
-    RCSAvg        -> [list of float with 2 elemnts, optional, default = None] Average Radar Cross Section[m2] of a target; it must be in form of [RCS1,RCS2], such as [5,20]; if None, this option is ignored.
-    OWNER       -> [str or list of str, optional, default = None] Satellite Ownership; country codes/names can be found at http://www.fao.org/countryprofiles/iso3list/en/; if None, this option is ignored.
-    sort          -> [str, optional, default = None] sort by features of targets in a specific order, such as by mass; avaliable options include 'COSPAR_ID', NORAD_ID', 'OBJECT_CLASS', 'MASS', 'DECAY_DATE', 'SHAPE', 
-    'LENGTH', 'HEIGHT', 'DEPTH', 'RCSMin', 'RSCMax', 'RCSAvg', 'PERIOD', 'INCLINATION', 'APOGEE', 'PERIGEE', 'MEAN_ALT', 'ECC', and 'OWNER'.
-    If there is a negative sign '-' ahead, such as "-RCSAvg", it will be sorted in descending order. If None, then sort by NORADID by default.
+    Inputs:
+        COSPAR_ID -> [str or list of str, optional, default = None] object IDs defined by the Committee On SPAce Research; if None, this option is ignored. 
+        NORAD_ID -> [int, str, list, or filename(such as 'noradids.txt'), optional, default = None] object IDs defined by the North American Aerospace Defense Command; if None, this option is ignored.
+        OBJECT_CLASS -> [str, list of str, optional, default = None] Classification of objects; available options are 'Payload', 'Payload Debris', 'Payload Fragmentation Debris', 
+        'Payload Mission Related Object', 'Rocket Body', 'Rocket Debris', 'Rocket Fragmentation Debris', 'Rocket Mission Related Object', 'Other Mission Related Object','Other Debris', Unknown', or any combination of them, 
+        for example, ['Rocket Body', 'Rocket Debris', 'Rocket Fragmentation Debris']; If None, this option is ignored.  
+        DECAYED -> [bool, optional, default = None] Whether an object is  decayed(re-entry) or not; If False, the object is still in orbit by now; if True, then decayed; if None, this option is ignored.
+        DECAY_DATE -> [list of str, optional, default = None] Date range of decay; it must be in form of ['date1','date2'], such as ['2019-01-05','2020-05-30']; if None, then this option is ignored.
+        PERIOD -> [list of float, optional, default = None] Orbital period[minutes] range of a space object; it must be in form of [period1,period2], such as [100.0,200.0]; if None, this option is ignored.  
+        INCLINATION -> [list of float, optional, default = None] Range of inclination[degrees] of a space object; it must be in form of [inc1,inc2], such as [45.0,80.0]; if None, this option is ignored.  
+        APOGEE -> [list of float, optional, default = None] Range of Apogee Altitude[km]; it must be in form of [apoalt1,apoalt2], such as [800.0,1400.0]; if None, this option is ignored.  
+        PERIGEE -> [list of float, optional, default = None] Range of Perigee Altitude[km]; it must be in form of [peralt1,peralt2], such as [300.0,400.0]; if None, this option is ignored.  
+        MEAN_ALT -> [list of float, optional, default = None] Mean Altitude[km] of objects; it must be in form of [meanalt1,meanalt2], such as [300.0,800.0]; if None, then option is ignored. 
+        ECC -> [list of float, optional, default = None] Range of Eccentricity; it must be in form of [ecc1,ecc2], such as [0.01,0.2]; if None, then option is ignored.   
+        TLE_STATUS -> [bool, optional, default = None] Whether a TLE is valid. If False, it means No Current Elements, No Initial Elements, or No Elements Available; if None, this option is ignored.
+        MASS -> [list of float, optional, default = None] Mass[kg] range of an object; it must be in form of [m1,m2], such as [5.0,10.0]; if None, this option is ignored.
+        SHAPE -> [str or list of str, optional, default = None] Shape of an object; the usual choices include 'Cyl', 'Sphere', 'Cone', 'Dcone', Pan', 'Ell', 'Dish', 'Cable', 'Box', 'Rod', 'Poly', 'Sail', 'Ant', 
+        'Frust', 'Truss', 'Nozzle', and 'lrr'. Any combination of them is also supported, for examle, ['Cyl', 'Sphere', 'Pan'] means 'or', and ['Cyl', 'Sphere', 'Pan', '+'] means 'and'; If None, this option is ignored.  
+        LENGTH -> [list of float, optional, default = None] Length[m] range of an object; it must be in form of [l1,l2], such as [5.0,10.0]; if None, this option is ignored.
+        HEIFHT -> [list of float, optional, default = None] Height[m] range of an object; it must be in form of [h1,h2], such as [5.0,10.0]; if None, this option is ignored.
+        DEPTH -> [list of float, optional, default = None] Depth[m] range of an object; it must be in form of [d1,d2], such as [5.0,10.0]; if None, this option is ignored.
+        RCSMin -> [list of float, optional, default = None] Minimum Radar Cross Section(RCS)[m2] of an object; if None, this option is ignored.
+        RCSMax -> [list of float, optional, default = None] Maximum Radar Cross Section(RCS)[m2] of an object; if None, this option is ignored.
+        RCSAvg -> [list of float, optional, default = None] Average Radar Cross Section(RCS)[m2] of an object; if None, this option is ignored.
+        OWNER -> [str or list of str, optional, default = None] Ownership of a space object; and country codes/names can be found at http://www.fao.org/countryprofiles/iso3list/en/; if None, this option is ignored.
+        sort -> [str, optional, default = None] Sort according to attributes of a spatial object, such as by mass; available options include 'COSPAR_ID', NORAD_ID', 'OBJECT_CLASS', 'MASS', 'DECAY_DATE', 'SHAPE', 
+        'LENGTH', 'HEIGHT', 'DEPTH', 'RCSMin', 'RSCMax', 'RCSAvg', 'PERIOD', 'INCLINATION', 'APOGEE', 'PERIGEE', 'MEAN_ALT', 'ECC', and 'OWNER'.
+        If the attribute is prefixed with a '-', such as "-RCSAvg", it will be sorted in descending order. If None, the spatial objects are sorted by NORADID by default.
     
     Outputs:
-    satcatlog -> instance of class SatCatlog
-    """
+        satcatalog_df -> Data frame containing the selected spatial objects
+    """ 
     # Query space targets from the CELESTRAK database
-    df_celestrak = celestrak_query(COSPAR_ID,NORAD_ID,PAYLOAD,DECAYED,DECAY_DATE,PERIOD,INCLINATION,APOGEE,PERIGEE,MEAN_ALT,ECC,OWNER,TLE_STATUS).df.drop('OBJECT_NAME',axis=1)
+    df_celestrak = _celestrak_query(COSPAR_ID,NORAD_ID,PAYLOAD,DECAYED,DECAY_DATE,PERIOD,INCLINATION,APOGEE,PERIGEE,MEAN_ALT,ECC,OWNER,TLE_STATUS).drop('OBJECT_NAME',axis=1)
     # Query space targets from the DISCOS database
     noradids = list(df_celestrak['NORAD_ID'])
     if len(noradids) > 1000: noradids = NORAD_ID
     print('Go through the DISCOS database ... ')    
-    df_discos = discos_query(COSPAR_ID,noradids,OBJECT_CLASS,PAYLOAD,DECAYED,DECAY_DATE,MASS,SHAPE,LENGTH,HEIGHT,DEPTH,RCSMin,RCSMax,RCSAvg).df.dropna(subset=['NORAD_ID'])
+    df_discos = _discos_query(COSPAR_ID,noradids,OBJECT_CLASS,PAYLOAD,DECAYED,DECAY_DATE,MASS,SHAPE,LENGTH,HEIGHT,DEPTH,RCSMin,RCSMax,RCSAvg).dropna(subset=['NORAD_ID'])
 
     # Merge the CELESTRAK database and the DISCOS database
     df = pd.merge(df_celestrak, df_discos, on=['COSPAR_ID','NORAD_ID'],validate="one_to_one")
 
     # Merge the QSMAG database
     df_qsmag = parseQSMagFile()
     df = pd.merge(df, df_qsmag, on=['NORAD_ID'],how='left',validate="one_to_one")
@@ -610,10 +609,8 @@
         elif sort.__contains__('OWNER'):
             df = df.sort_values(by=['OWNER'],ascending=ascending_flag)
         else:
             raise Exception("Avaliable options include 'COSPAR_ID', NORAD_ID', 'DECAY_DATE', 'PERIOD', 'INCLINATION', \
                 'APOGEE', 'PERIGEE', 'MEAN_ALT', 'ECC', 'MASS','LENGTH','DEPTH','HEIGHT', 'RCSMin','RCSMax', 'RCSAvg',\
                 'StdMag','LAUNCH_DATE',and 'OWNER'. Also, a negative sign '-' can be added to the option to sort in descending order.")
     df = df.reset_index(drop=True)
-    mode = 'targets_catalog'
-
-    return SatCatlog(df,mode)               
+    return df
```

## satcatalogquery/try_download.py

```diff
@@ -1,20 +1,19 @@
 import wget
 
 def wget_download(url,dir_file,desc=None):
     """
-    download files by wget command
+    Download files by wget command
 
     Inputs:
         url -> [str]
-        dir_file -> [str] output filename or directory
-    Parameters:
-        desc -> [str] description of the downloading   
+        dir_file -> [str] Path to save the files downloaded
+        desc -> [str,optional,default=None] Log description for file downloading 
     Outpits:
-        wget_out -> [str] path and filename where URL is downloaded to   
+        wget_out -> [str] Path of the files downloaded
 
     """
     if desc: print(desc)
     wget_out = wget.download(url,dir_file)
     print()
 
     return wget_out
```

## Comparing `satcatalogquery-0.2.1.dist-info/LICENSE` & `satcatalogquery-0.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `satcatalogquery-0.2.1.dist-info/METADATA` & `satcatalogquery-0.2.2.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 Metadata-Version: 2.1
 Name: satcatalogquery
-Version: 0.2.1
-Summary: A package to handle the space targets catalogue query
+Version: 0.2.2
+Summary: A package for querying orbital and geometric information of spatial objects
 Home-page: https://github.com/lcx366/SATQUERY
 Author: Chunxiao Li
 Author-email: lcx366@126.com
 License: MIT
-Keywords: DISCOS,CelesTrak
+Keywords: DISCOS,CelesTrak,SpaceTrack,Space Debris
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: spacetrack
 Requires-Dist: numpy (>=1.21.2)
 Requires-Dist: matplotlib
 Requires-Dist: pandas
 Requires-Dist: wget
 Requires-Dist: colorama
 
 # Welcome to the SATQUERY package
 
-[![PyPI version shields.io](https://img.shields.io/pypi/v/satcatalogquery.svg)](https://pypi.python.org/pypi/satcatalogquery/) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/satcatalogquery.svg)](https://pypi.python.org/pypi/satcatalogquery/) [![PyPI status](https://img.shields.io/pypi/status/satcatalogquery.svg)](https://pypi.python.org/pypi/satcatalogquery/) [![GitHub contributors](https://img.shields.io/github/contributors/lcx366/SATQUERY.svg)](https://GitHub.com/lcx366/SATQUERY/graphs/contributors/) [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/lcx366/SATQUERY/graphs/commit-activity) [![GitHub license](https://img.shields.io/github/license/lcx366/SATQUERY.svg)](https://github.com/lcx366/SATQUERY/blob/master/LICENSE) [![Documentation Status](https://readthedocs.org/projects/pystmos/badge/?version=latest)](http://satcatalogquery.readthedocs.io/?badge=latest) [![Build Status](https://travis-ci.org/lcx366/satcatalogquery.svg?branch=master)](https://travis-ci.org/lcx366/satcatalogquery)
+[![PyPI version shields.io](https://img.shields.io/pypi/v/satcatalogquery.svg)](https://pypi.python.org/pypi/satcatalogquery/) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/satcatalogquery.svg)](https://pypi.python.org/pypi/satcatalogquery/) [![PyPI status](https://img.shields.io/pypi/status/satcatalogquery.svg)](https://pypi.python.org/pypi/satcatalogquery/) [![GitHub contributors](https://img.shields.io/github/contributors/lcx366/SATQUERY.svg)](https://GitHub.com/lcx366/SATQUERY/graphs/contributors/) [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/lcx366/SATQUERY/graphs/commit-activity) [![GitHub license](https://img.shields.io/github/license/lcx366/SATQUERY.svg)](https://github.com/lcx366/SATQUERY/blob/master/LICENSE) [![Documentation Status](https://readthedocs.org/projects/satcatalogquery/badge/?version=latest)](http://satcatalogquery.readthedocs.io/?badge=latest) [![Build Status](https://travis-ci.org/lcx366/satcatalogquery.svg?branch=master)](https://travis-ci.org/lcx366/satcatalogquery)
 
-This package is an archive of scientific routines for data processing related to the space targets catalogue query. 
-Currently, operations on  targets catalogue query include:
+This package is an archive of scientific routines for querying orbital and geometric information of spatial objects.
+Currently, operations on objects catalogue query include:
 
-1. targets catalogue query on shape info from DISCOS(Database and Information System Characterising Objects in Space) database;
-2. targets catalogue query on orbit info from CelesTrak database;
-3. targets catalogue query on both shape and orbit from a combined database;
+1. Query of spatial objects on geometric information from DISCOS(Database and Information System Characterising Objects in Space) database;
+2. Query of spatial objects on orbital information from CelesTrak database;
+3. Query of spatial objects on both geometric and orbital information from a combined database;
 
 ## How to Install
 
 On Linux, macOS and Windows architectures, the binary wheels can be installed using pip by executing one of the following commands:
 
 ```
 pip install satcatalogquery
@@ -55,47 +56,44 @@
 51454
 37637
 26758
 44691
 ```
 
 ```python
->>> from satcatalogquery import discos_query
->>> satcatlog = discos_query(NORAD_ID=[52132,51454,37637,26758,44691])
->>> # satcatog = discos_query(NORAD_ID='satno.txt')
+>>> from satcatalogquery import SatCatalog
+>>> satcatlog = SatCatalog.discos_query(NORAD_ID=[52132,51454,37637,26758,44691])
+>>> # satcatog = SatCatalog.discos_query(NORAD_ID='satno.txt')
 >>> satcatlog.df # output pandas dataframe
->>> satcatlog.save() # save dataframe to .csv file
+>>> satcatlog.to_csv() # save dataframe to .csv file
 ```
 
 Query by mutiple options at the same time, such as COSPAR_ID, MASS, SHAPE, RCSAvg, etc.
 
 ```python
->>> from satcatalogquery import discos_query
->>> satcatlog = discos_query(SHAPE=['Box','Pan'],RCSAvg=[0.5,100],DECAYED=False)
+>>> satcatlog = SatCatalog.discos_query(SHAPE=['Box','Pan'],RCSAvg=[0.5,10],DECAYED=False)
 ```
 
 #### Targets catalogue query from CelesTrak
 
 ```python
->>> from satcatalogquery import celestrak_query
->>> satcatlog = celestrak_query(MEAN_ALT=[300,2000],ECC=[0.01,0.1],PAYLOAD=False)
+>>> satcatlog = SatCatalog.celestrak_query(MEAN_ALT=[300,2000],ECC=[0.01,0.1],PAYLOAD=False)
 ```
 
 ### Targets catalogue query from combined database
 
 ```python
->>> from satcatalogquery import targets_query
->>> satcatlog = targets_query(DECAYED=False,RCSAvg=[0.25,1e4],MEAN_ALT=[250,2000],TLE_STATUS=True,sort='RCSAvg')
+>>> satcatlog = SatCatalog.objects_query(DECAYED=False,RCSAvg=[0.25,10],MEAN_ALT=[250,2000],TLE_STATUS=True,sort='RCSAvg')
 ```
 
 ### Create object `SatCatlog` from a loacl .csv file
 
 ```python
->>> from satcatalogquery import SatCatlog
->>> satcatlog = SatCatlog.from_csv('filename.csv')
+>>> from satcatalogquery import SatCatalog
+>>> satcatlog = SatCatalog.from_csv('filename.csv')
 ```
 
 ### Statistics
 
 ```python
 >>> satcatlog.hist1d('RCSAvg')
 >>> satcatlog.hist1d(['StdMag','LAUNCH_DATE'])
@@ -121,16 +119,32 @@
 
 ### Download TLE from results of targets catalogue query
 
 ```python
 >>> tle_path = satcatlog.get_tle()
 ```
 
+### Download TLE from Norad IDs
+
+```python
+>>> from satcatalogquery import download_tle
+>>> tle_file = download_tle([52132,51454,37637,26758,44691])
+>>> print(tle_file)
+```
+
 ## Change log
 
+- **0.2.2 — Apr 24, 2023**
+  
+  - Change the method `.save()` to `.to_csv()` 
+  
+  - Add methods `.discos_query()`, `.celestrak_query()`, `.objects_query()`to class SatCatalog
+
+  - Change class `SatCatlog` to `SatCatalog` 
+
 - **0.2.1 — Jan 4, 2023**
   
   - Add method `from_csv` and `pie` to class SatCatlog
   
   - Add statistics figures to README.md
 
 - **0.1.1 — Jan 2,  2023**
```

## Comparing `satcatalogquery-0.2.1.dist-info/RECORD` & `satcatalogquery-0.2.2.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-satcatalogquery/Const.py,sha256=TfU_OP_GIa6dZEIDEs7Jt-0KFlKcdBcVyg8AMECjn4k,362
-satcatalogquery/__init__.py,sha256=FOeqFMlne1ohrvl9Go56Fze6_KIpzrqiiXoI6iFd0x0,206
-satcatalogquery/data_download.py,sha256=RpLaNM25EE0-SPSgCL7VtJcmgsEWZ6WH3CmKkxM0ocs,6251
-satcatalogquery/data_prepare.py,sha256=-DnRxHrhdqxmBkFS8h9NxW0SBjrCoqffAXnuFjwGreM,339
-satcatalogquery/query.py,sha256=hrg3eTq3IIuBnzrZJErFvLbg1iUNeBGoJCJ3PYVCoKU,37141
-satcatalogquery/satcatclass.py,sha256=GUHjdjwHiBOjBHmhViURUkApHdkv8gtz5zBvhQY-TVo,5339
-satcatalogquery/try_download.py,sha256=_Wxs_6Zm7-bL6lgnHbbI-F4nBoF8GDdz73NkJ9PlC14,461
-satcatalogquery-0.2.1.dist-info/LICENSE,sha256=1mo8gGwn9nEfzoruoWYAD1ttN40DofMYGQNef1rsytY,1068
-satcatalogquery-0.2.1.dist-info/METADATA,sha256=VQdvrKm351J8PM_YS-O3OhKhTbE7T_Zy2MIwGeTgq6U,5027
-satcatalogquery-0.2.1.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-satcatalogquery-0.2.1.dist-info/top_level.txt,sha256=HoHpR1NJLfGlD0rCuFAoleEfAzeVKVIHkczHFQBSjg8,16
-satcatalogquery-0.2.1.dist-info/RECORD,,
+satcatalogquery/Const.py,sha256=avNzqPAjUiGjmwoULPYixBDOCO2dVLrD2Rt7QyFjT0Y,304
+satcatalogquery/__init__.py,sha256=Jx3-ulJMqmHUcz2DYFDiHMNwdX9S7QBQZP7W8LHIbzs,98
+satcatalogquery/classes.py,sha256=A2ck_igz6YjBUxwmpZdc7mFDPfVRcNQhz5hiRMCnbS8,22975
+satcatalogquery/data_download.py,sha256=gS_701MmuNHEx6LyR4D3OFVQoH-keWUFQnVnrj2mfG0,6395
+satcatalogquery/data_prepare.py,sha256=qJ-7by16eYiIprZM6CaQaMVZLwUncYBpNqGD0KlsulY,355
+satcatalogquery/query.py,sha256=2W35aM0TfKLCv6fGgpabjwehwLSdxp4SPF0B-lXoJNk,36773
+satcatalogquery/try_download.py,sha256=uqebfXlSI0I0_TomawI8wRg3PoEn1uYcPmksH90rynQ,457
+satcatalogquery-0.2.2.dist-info/LICENSE,sha256=1mo8gGwn9nEfzoruoWYAD1ttN40DofMYGQNef1rsytY,1068
+satcatalogquery-0.2.2.dist-info/METADATA,sha256=96ZDIupTVH2SRXWOVhvazDlKSc_r0oUYfs4ajji9ujM,5488
+satcatalogquery-0.2.2.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+satcatalogquery-0.2.2.dist-info/top_level.txt,sha256=HoHpR1NJLfGlD0rCuFAoleEfAzeVKVIHkczHFQBSjg8,16
+satcatalogquery-0.2.2.dist-info/RECORD,,
```

