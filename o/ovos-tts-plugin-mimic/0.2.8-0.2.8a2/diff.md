# Comparing `tmp/ovos_tts_plugin_mimic-0.2.8-py3-none-any.whl.zip` & `tmp/ovos_tts_plugin_mimic-0.2.8a2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 8752 bytes, number of entries: 9
--rw-r--r--  2.0 unx     6408 b- defN 23-Apr-24 08:30 ovos_tts_plugin_mimic/__init__.py
--rw-r--r--  2.0 unx      177 b- defN 23-Apr-24 08:30 ovos_tts_plugin_mimic/version.py
--rw-r--r--  2.0 unx    11349 b- defN 23-Apr-24 08:30 ovos_tts_plugin_mimic-0.2.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     1063 b- defN 23-Apr-24 08:30 ovos_tts_plugin_mimic-0.2.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-24 08:30 ovos_tts_plugin_mimic-0.2.8.dist-info/WHEEL
--rw-r--r--  2.0 unx      186 b- defN 23-Apr-24 08:30 ovos_tts_plugin_mimic-0.2.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       22 b- defN 23-Apr-24 08:30 ovos_tts_plugin_mimic-0.2.8.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-24 08:30 ovos_tts_plugin_mimic-0.2.8.dist-info/zip-safe
--rw-rw-r--  2.0 unx      845 b- defN 23-Apr-24 08:30 ovos_tts_plugin_mimic-0.2.8.dist-info/RECORD
-9 files, 20143 bytes uncompressed, 7258 bytes compressed:  64.0%
+Zip file size: 8783 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     6408 b- defN 23-Apr-24 08:28 ovos_tts_plugin_mimic/__init__.py
+-rw-r--r--  2.0 unx      177 b- defN 23-Apr-24 08:28 ovos_tts_plugin_mimic/version.py
+-rw-r--r--  2.0 unx    11349 b- defN 23-Apr-24 08:29 ovos_tts_plugin_mimic-0.2.8a2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1065 b- defN 23-Apr-24 08:29 ovos_tts_plugin_mimic-0.2.8a2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-24 08:29 ovos_tts_plugin_mimic-0.2.8a2.dist-info/WHEEL
+-rw-r--r--  2.0 unx      186 b- defN 23-Apr-24 08:29 ovos_tts_plugin_mimic-0.2.8a2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       22 b- defN 23-Apr-24 08:29 ovos_tts_plugin_mimic-0.2.8a2.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-24 08:29 ovos_tts_plugin_mimic-0.2.8a2.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      859 b- defN 23-Apr-24 08:29 ovos_tts_plugin_mimic-0.2.8a2.dist-info/RECORD
+9 files, 20159 bytes uncompressed, 7261 bytes compressed:  64.0%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
 Filename: ovos_tts_plugin_mimic/__init__.py
 Comment: 
 
 Filename: ovos_tts_plugin_mimic/version.py
 Comment: 
 
-Filename: ovos_tts_plugin_mimic-0.2.8.dist-info/LICENSE
+Filename: ovos_tts_plugin_mimic-0.2.8a2.dist-info/LICENSE
 Comment: 
 
-Filename: ovos_tts_plugin_mimic-0.2.8.dist-info/METADATA
+Filename: ovos_tts_plugin_mimic-0.2.8a2.dist-info/METADATA
 Comment: 
 
-Filename: ovos_tts_plugin_mimic-0.2.8.dist-info/WHEEL
+Filename: ovos_tts_plugin_mimic-0.2.8a2.dist-info/WHEEL
 Comment: 
 
-Filename: ovos_tts_plugin_mimic-0.2.8.dist-info/entry_points.txt
+Filename: ovos_tts_plugin_mimic-0.2.8a2.dist-info/entry_points.txt
 Comment: 
 
-Filename: ovos_tts_plugin_mimic-0.2.8.dist-info/top_level.txt
+Filename: ovos_tts_plugin_mimic-0.2.8a2.dist-info/top_level.txt
 Comment: 
 
-Filename: ovos_tts_plugin_mimic-0.2.8.dist-info/zip-safe
+Filename: ovos_tts_plugin_mimic-0.2.8a2.dist-info/zip-safe
 Comment: 
 
-Filename: ovos_tts_plugin_mimic-0.2.8.dist-info/RECORD
+Filename: ovos_tts_plugin_mimic-0.2.8a2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ovos_tts_plugin_mimic/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 2
 VERSION_BUILD = 8
-VERSION_ALPHA = 0
+VERSION_ALPHA = 2
 # END_VERSION_BLOCK
```

## Comparing `ovos_tts_plugin_mimic-0.2.8.dist-info/LICENSE` & `ovos_tts_plugin_mimic-0.2.8a2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ovos_tts_plugin_mimic-0.2.8.dist-info/METADATA` & `ovos_tts_plugin_mimic-0.2.8a2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-tts-plugin-mimic
-Version: 0.2.8
+Version: 0.2.8a2
 Summary: mimic tts plugin for OpenVoiceOS
 Home-page: https://github.com/OpenVoiceOS/ovos-tts-plugin-mimic
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Keywords: mycroft plugin tts OVOS OpenVoiceOS
 Platform: UNKNOWN
```

## Comparing `ovos_tts_plugin_mimic-0.2.8.dist-info/RECORD` & `ovos_tts_plugin_mimic-0.2.8a2.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ovos_tts_plugin_mimic/__init__.py,sha256=oIott377j6-Ys3IKZLQs2Z0TxqBNQ-yr_AhLRG2FasM,6408
-ovos_tts_plugin_mimic/version.py,sha256=cwd1s5K8IGcWtgoiXBzGpT2FLFCpYs5ENThMYArXY2U,177
-ovos_tts_plugin_mimic-0.2.8.dist-info/LICENSE,sha256=fYHkowW9JcaEcqCPTXYBayNJ9J1lGdYVb7Mf9oy6oEY,11349
-ovos_tts_plugin_mimic-0.2.8.dist-info/METADATA,sha256=oGdVRriHGLOmF7K0i9ayLdvJzVEciXnccS7b2-xQX6E,1063
-ovos_tts_plugin_mimic-0.2.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ovos_tts_plugin_mimic-0.2.8.dist-info/entry_points.txt,sha256=cpMDp3sVYWI7-Zrn2LaccI0BClDVNaxg_DqLzJ9herw,186
-ovos_tts_plugin_mimic-0.2.8.dist-info/top_level.txt,sha256=wHdv3nP76RPxU4Mrw1HE2P3kTZOz6X4iJ_AQB4_fGtc,22
-ovos_tts_plugin_mimic-0.2.8.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-ovos_tts_plugin_mimic-0.2.8.dist-info/RECORD,,
+ovos_tts_plugin_mimic/version.py,sha256=NN7KkFKdBuVhWyCXuDk9kKMoX5nHT9llvz6PzpcScac,177
+ovos_tts_plugin_mimic-0.2.8a2.dist-info/LICENSE,sha256=fYHkowW9JcaEcqCPTXYBayNJ9J1lGdYVb7Mf9oy6oEY,11349
+ovos_tts_plugin_mimic-0.2.8a2.dist-info/METADATA,sha256=8Dk84w2m1MKIlIQHV1zMlzi0QEeprKvFGMQZW0P-7Hc,1065
+ovos_tts_plugin_mimic-0.2.8a2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ovos_tts_plugin_mimic-0.2.8a2.dist-info/entry_points.txt,sha256=cpMDp3sVYWI7-Zrn2LaccI0BClDVNaxg_DqLzJ9herw,186
+ovos_tts_plugin_mimic-0.2.8a2.dist-info/top_level.txt,sha256=wHdv3nP76RPxU4Mrw1HE2P3kTZOz6X4iJ_AQB4_fGtc,22
+ovos_tts_plugin_mimic-0.2.8a2.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+ovos_tts_plugin_mimic-0.2.8a2.dist-info/RECORD,,
```

