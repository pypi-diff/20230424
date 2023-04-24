# Comparing `tmp/algokit_utils-1.0.4b1-py3-none-any.whl.zip` & `tmp/algokit_utils-1.0.4b2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 31268 bytes, number of entries: 14
+Zip file size: 31270 bytes, number of entries: 14
 -rw-r--r--  2.0 unx     3493 b- defN 80-Jan-01 00:00 algokit_utils/__init__.py
 -rw-r--r--  2.0 unx     3568 b- defN 80-Jan-01 00:00 algokit_utils/_transfer.py
 -rw-r--r--  2.0 unx     7709 b- defN 80-Jan-01 00:00 algokit_utils/account.py
 -rw-r--r--  2.0 unx    53906 b- defN 80-Jan-01 00:00 algokit_utils/application_client.py
 -rw-r--r--  2.0 unx     7466 b- defN 80-Jan-01 00:00 algokit_utils/application_specification.py
 -rw-r--r--  2.0 unx    29956 b- defN 80-Jan-01 00:00 algokit_utils/deploy.py
 -rw-r--r--  2.0 unx     1981 b- defN 80-Jan-01 00:00 algokit_utils/logic_error.py
 -rw-r--r--  2.0 unx     3930 b- defN 80-Jan-01 00:00 algokit_utils/models.py
 -rw-r--r--  2.0 unx     3838 b- defN 80-Jan-01 00:00 algokit_utils/network_clients.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 algokit_utils/py.typed
--rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-1.0.4b1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1873 b- defN 80-Jan-01 00:00 algokit_utils-1.0.4b1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-1.0.4b1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1175 b- defN 16-Jan-01 00:00 algokit_utils-1.0.4b1.dist-info/RECORD
-14 files, 120059 bytes uncompressed, 29314 bytes compressed:  75.6%
+-rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-1.0.4b2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1873 b- defN 80-Jan-01 00:00 algokit_utils-1.0.4b2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-1.0.4b2.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1175 b- defN 16-Jan-01 00:00 algokit_utils-1.0.4b2.dist-info/RECORD
+14 files, 120059 bytes uncompressed, 29316 bytes compressed:  75.6%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: algokit_utils/network_clients.py
 Comment: 
 
 Filename: algokit_utils/py.typed
 Comment: 
 
-Filename: algokit_utils-1.0.4b1.dist-info/LICENSE
+Filename: algokit_utils-1.0.4b2.dist-info/LICENSE
 Comment: 
 
-Filename: algokit_utils-1.0.4b1.dist-info/METADATA
+Filename: algokit_utils-1.0.4b2.dist-info/METADATA
 Comment: 
 
-Filename: algokit_utils-1.0.4b1.dist-info/WHEEL
+Filename: algokit_utils-1.0.4b2.dist-info/WHEEL
 Comment: 
 
-Filename: algokit_utils-1.0.4b1.dist-info/RECORD
+Filename: algokit_utils-1.0.4b2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## algokit_utils/application_client.py

```diff
@@ -282,15 +282,15 @@
 
         :param str version: version to use when creating or updating app, if None version will be auto incremented
         :param algosdk.atomic_transaction_composer.TransactionSigner signer: signer to use when deploying app
         , if None uses self.signer
         :param str sender: sender address to use when deploying app, if None uses self.sender
         :param bool allow_delete: Used to set the `TMPL_DELETABLE` template variable to conditionally control if an app
         can be deleted
-        :param bool allow_update: Used to set the `TMPL_DELETABLE` template variable to conditionally control if an app
+        :param bool allow_update: Used to set the `TMPL_UPDATABLE` template variable to conditionally control if an app
         can be updated
         :param OnUpdate on_update: Determines what action to take if an application update is required
         :param OnSchemaBreak on_schema_break: Determines what action to take if an application schema requirements
         has increased beyond the current allocation
         :param dict[str, int|str|bytes] template_values: Values to use for `TMPL_*` template variables, dictionary keys
         should *NOT* include the TMPL_ prefix
         :param ABICreateCallArgs create_args: Arguments used when creating an application
```

## Comparing `algokit_utils-1.0.4b1.dist-info/LICENSE` & `algokit_utils-1.0.4b2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `algokit_utils-1.0.4b1.dist-info/METADATA` & `algokit_utils-1.0.4b2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algokit-utils
-Version: 1.0.4b1
+Version: 1.0.4b2
 Summary: Utilities for Algorand development for use by AlgoKit
 License: MIT
 Author: Algorand Foundation
 Author-email: contact@algorand.foundation
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `algokit_utils-1.0.4b1.dist-info/RECORD` & `algokit_utils-1.0.4b2.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 algokit_utils/__init__.py,sha256=wZm8zcJh-bj3HlMpK-yoNJwzNX6NEKnWDPuD4JoRifA,3493
 algokit_utils/_transfer.py,sha256=MAu9lLMK_g9GB40X2pb5zzDDsrDkqge1Onx5_CDSwwg,3568
 algokit_utils/account.py,sha256=-OQn9mhKxZkgXhab_ugRlKt18LRvK6KxJkH5bhFb-6k,7709
-algokit_utils/application_client.py,sha256=Y08HOxQFFGdQ6j4l7k18txxCg5chmMQvO2P7xw0tcMA,53906
+algokit_utils/application_client.py,sha256=3oON9YJ-fU3rFhxacSPNxrpmnHUgG349oMH_Id9NdIA,53906
 algokit_utils/application_specification.py,sha256=XusOe7VrGPun2UoNspC9Ei202NzPkxRNx5USXiABuXc,7466
 algokit_utils/deploy.py,sha256=Vg5K7xDSp7F8ImwT9FyboZDZFHeq_HeZgZyU26lvjE0,29956
 algokit_utils/logic_error.py,sha256=ypu2DSyus-Kjy51_1oE8T3LHVhRSOrc21Gpbau_WjAc,1981
 algokit_utils/models.py,sha256=46vPWFNMowMyNOhmlInq58gVtOg91xgPhQ0w-bIMacw,3930
 algokit_utils/network_clients.py,sha256=N4Xcp3xE2LUXtXIWuWUjQlPRhuGaDTW2gjjio_X45k8,3838
 algokit_utils/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-algokit_utils-1.0.4b1.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
-algokit_utils-1.0.4b1.dist-info/METADATA,sha256=tF50CnzirLQEMrElHu0Q9btTVn7Bey-jMmneOl1X6K8,1873
-algokit_utils-1.0.4b1.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-algokit_utils-1.0.4b1.dist-info/RECORD,,
+algokit_utils-1.0.4b2.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
+algokit_utils-1.0.4b2.dist-info/METADATA,sha256=Rt-3nxCk2aKMGVImxVe0-2ixbZ4huUVyPmutVRa1cSo,1873
+algokit_utils-1.0.4b2.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+algokit_utils-1.0.4b2.dist-info/RECORD,,
```

