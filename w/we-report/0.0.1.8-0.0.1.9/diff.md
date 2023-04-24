# Comparing `tmp/we_report-0.0.1.8-py3-none-any.whl.zip` & `tmp/we_report-0.0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 8630 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-21 07:41 we_report/__init__.py
+Zip file size: 8753 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat      126 b- defN 23-Apr-20 09:46 we_report/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-21 07:41 we_report/data_type/__init__.py
 -rw-rw-rw-  2.0 fat     7440 b- defN 23-Mar-21 07:41 we_report/data_type/report_data.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-21 07:41 we_report/interface/__init__.py
 -rw-rw-rw-  2.0 fat     7307 b- defN 23-Mar-21 07:41 we_report/interface/excel_reporter.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-21 07:41 we_report/utils/__init__.py
 -rw-rw-rw-  2.0 fat      599 b- defN 23-Mar-21 07:41 we_report/utils/utils.py
--rw-rw-rw-  2.0 fat     1092 b- defN 23-Apr-20 09:25 we_report-0.0.1.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      778 b- defN 23-Apr-20 09:25 we_report-0.0.1.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-20 09:25 we_report-0.0.1.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-Apr-20 09:25 we_report-0.0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      996 b- defN 23-Apr-20 09:25 we_report-0.0.1.8.dist-info/RECORD
-12 files, 18314 bytes uncompressed, 6928 bytes compressed:  62.2%
+-rw-rw-rw-  2.0 fat     1092 b- defN 23-Apr-20 09:47 we_report-0.0.1.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      778 b- defN 23-Apr-20 09:47 we_report-0.0.1.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-20 09:47 we_report-0.0.1.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Apr-20 09:47 we_report-0.0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      998 b- defN 23-Apr-20 09:47 we_report-0.0.1.9.dist-info/RECORD
+12 files, 18442 bytes uncompressed, 7051 bytes compressed:  61.8%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: we_report/utils/__init__.py
 Comment: 
 
 Filename: we_report/utils/utils.py
 Comment: 
 
-Filename: we_report-0.0.1.8.dist-info/LICENSE
+Filename: we_report-0.0.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: we_report-0.0.1.8.dist-info/METADATA
+Filename: we_report-0.0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: we_report-0.0.1.8.dist-info/WHEEL
+Filename: we_report-0.0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: we_report-0.0.1.8.dist-info/top_level.txt
+Filename: we_report-0.0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: we_report-0.0.1.8.dist-info/RECORD
+Filename: we_report-0.0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## we_report/__init__.py

```diff
@@ -0,0 +1,8 @@
+00000000: 6672 6f6d 2077 655f 7265 706f 7274 2e64  from we_report.d
+00000010: 6174 615f 7479 7065 2e72 6570 6f72 745f  ata_type.report_
+00000020: 6461 7461 2069 6d70 6f72 7420 5061 6765  data import Page
+00000030: 4461 7461 2c20 5265 706f 7274 4461 7461  Data, ReportData
+00000040: 0d0a 6672 6f6d 2077 655f 7265 706f 7274  ..from we_report
+00000050: 2e69 6e74 6572 6661 6365 2e65 7863 656c  .interface.excel
+00000060: 5f72 6570 6f72 7465 7220 696d 706f 7274  _reporter import
+00000070: 2045 7863 656c 5265 706f 7274 0d0a        ExcelReport..
```

## Comparing `we_report-0.0.1.8.dist-info/LICENSE` & `we_report-0.0.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `we_report-0.0.1.8.dist-info/METADATA` & `we_report-0.0.1.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: we-report
-Version: 0.0.1.8
+Version: 0.0.1.9
 Summary: Wealth Engine ReportData Generator
 Home-page: http://192.168.1.7:10600/xiazeyu/we_report.git
 Author: Xia Zeyu
 Author-email: xiazeyu@wealthengine.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `we_report-0.0.1.8.dist-info/RECORD` & `we_report-0.0.1.9.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-we_report/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+we_report/__init__.py,sha256=9Q4Vsx44YmjZ5Ji1Wg4pmSqamVPHJTHDezLAHA37UG0,126
 we_report/data_type/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 we_report/data_type/report_data.py,sha256=nlnm3crZHLnx7_lr7lg9fKAQG0d8AS9H_Us1h3VCr0I,7440
 we_report/interface/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 we_report/interface/excel_reporter.py,sha256=nNPPDk8i3N3KVNPBpg6m_z-0nHImcPoqFhjICY8ZmPY,7307
 we_report/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 we_report/utils/utils.py,sha256=GkAJGbefPwIFypoKqMrhKiCnVNWBwRv47RtdPR0G5t0,599
-we_report-0.0.1.8.dist-info/LICENSE,sha256=unAISPdUaH8a0Vw-QIivpvGNO-x3h_irtPw7yj07b6c,1092
-we_report-0.0.1.8.dist-info/METADATA,sha256=eNWp-Xb27dLQXN_Vv1MO4SWAQe81dwSmtEWTlzsQwGk,778
-we_report-0.0.1.8.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-we_report-0.0.1.8.dist-info/top_level.txt,sha256=RZuqUTMBxg7Dc7a_DYNhzf_w_Isj1Id9mZTsDv1BzXw,10
-we_report-0.0.1.8.dist-info/RECORD,,
+we_report-0.0.1.9.dist-info/LICENSE,sha256=unAISPdUaH8a0Vw-QIivpvGNO-x3h_irtPw7yj07b6c,1092
+we_report-0.0.1.9.dist-info/METADATA,sha256=N9J2bIIGxHAoO7q11ZDLqU4L_FT2AuiSTMuNgvhd-4g,778
+we_report-0.0.1.9.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+we_report-0.0.1.9.dist-info/top_level.txt,sha256=RZuqUTMBxg7Dc7a_DYNhzf_w_Isj1Id9mZTsDv1BzXw,10
+we_report-0.0.1.9.dist-info/RECORD,,
```

