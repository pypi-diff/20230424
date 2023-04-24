# Comparing `tmp/alibabacloud_dms-enterprise20181101-1.45.0.tar.gz` & `tmp/alibabacloud_dms-enterprise20181101-1.46.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dms-enterprise20181101-1.45.0.tar", last modified: Tue Apr 11 03:36:53 2023, max compression
+gzip compressed data, was "dist/alibabacloud_dms-enterprise20181101-1.46.0.tar", last modified: Mon Apr 24 09:03:12 2023, max compression
```

## Comparing `alibabacloud_dms-enterprise20181101-1.45.0.tar` & `alibabacloud_dms-enterprise20181101-1.46.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:36:53.000000 alibabacloud_dms-enterprise20181101-1.45.0/
--rw-r--r--   0 root         (0) root         (0)     4668 2023-04-11 03:36:53.000000 alibabacloud_dms-enterprise20181101-1.45.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-11 03:36:53.000000 alibabacloud_dms-enterprise20181101-1.45.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-11 03:36:53.000000 alibabacloud_dms-enterprise20181101-1.45.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2395 2023-04-11 03:36:53.000000 alibabacloud_dms-enterprise20181101-1.45.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1055 2023-04-11 03:36:53.000000 alibabacloud_dms-enterprise20181101-1.45.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1140 2023-04-11 03:36:53.000000 alibabacloud_dms-enterprise20181101-1.45.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:36:53.000000 alibabacloud_dms-enterprise20181101-1.45.0/alibabacloud_dms_enterprise20181101/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 03:36:53.000000 alibabacloud_dms-enterprise20181101-1.45.0/alibabacloud_dms_enterprise20181101/__init__.py
--rw-r--r--   0 root         (0) root         (0)   746627 2023-04-11 03:36:53.000000 alibabacloud_dms-enterprise20181101-1.45.0/alibabacloud_dms_enterprise20181101/client.py
--rw-r--r--   0 root         (0) root         (0)  1685783 2023-04-11 03:36:53.000000 alibabacloud_dms-enterprise20181101-1.45.0/alibabacloud_dms_enterprise20181101/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:36:53.000000 alibabacloud_dms-enterprise20181101-1.45.0/alibabacloud_dms_enterprise20181101.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2395 2023-04-11 03:36:53.000000 alibabacloud_dms-enterprise20181101-1.45.0/alibabacloud_dms_enterprise20181101.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      508 2023-04-11 03:36:53.000000 alibabacloud_dms-enterprise20181101-1.45.0/alibabacloud_dms_enterprise20181101.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 03:36:53.000000 alibabacloud_dms-enterprise20181101-1.45.0/alibabacloud_dms_enterprise20181101.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-04-11 03:36:53.000000 alibabacloud_dms-enterprise20181101-1.45.0/alibabacloud_dms_enterprise20181101.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       36 2023-04-11 03:36:53.000000 alibabacloud_dms-enterprise20181101-1.45.0/alibabacloud_dms_enterprise20181101.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-11 03:36:53.000000 alibabacloud_dms-enterprise20181101-1.45.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2667 2023-04-11 03:36:53.000000 alibabacloud_dms-enterprise20181101-1.45.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 09:03:12.000000 alibabacloud_dms-enterprise20181101-1.46.0/
+-rw-r--r--   0 root         (0) root         (0)     4784 2023-04-24 09:03:11.000000 alibabacloud_dms-enterprise20181101-1.46.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-24 09:03:11.000000 alibabacloud_dms-enterprise20181101-1.46.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-24 09:03:11.000000 alibabacloud_dms-enterprise20181101-1.46.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2395 2023-04-24 09:03:12.000000 alibabacloud_dms-enterprise20181101-1.46.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1055 2023-04-24 09:03:11.000000 alibabacloud_dms-enterprise20181101-1.46.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1140 2023-04-24 09:03:11.000000 alibabacloud_dms-enterprise20181101-1.46.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 09:03:12.000000 alibabacloud_dms-enterprise20181101-1.46.0/alibabacloud_dms_enterprise20181101/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-24 09:03:11.000000 alibabacloud_dms-enterprise20181101-1.46.0/alibabacloud_dms_enterprise20181101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   789173 2023-04-24 09:03:11.000000 alibabacloud_dms-enterprise20181101-1.46.0/alibabacloud_dms_enterprise20181101/client.py
+-rw-r--r--   0 root         (0) root         (0)  1787794 2023-04-24 09:03:11.000000 alibabacloud_dms-enterprise20181101-1.46.0/alibabacloud_dms_enterprise20181101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 09:03:12.000000 alibabacloud_dms-enterprise20181101-1.46.0/alibabacloud_dms_enterprise20181101.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2395 2023-04-24 09:03:11.000000 alibabacloud_dms-enterprise20181101-1.46.0/alibabacloud_dms_enterprise20181101.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      508 2023-04-24 09:03:11.000000 alibabacloud_dms-enterprise20181101-1.46.0/alibabacloud_dms_enterprise20181101.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 09:03:11.000000 alibabacloud_dms-enterprise20181101-1.46.0/alibabacloud_dms_enterprise20181101.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-04-24 09:03:11.000000 alibabacloud_dms-enterprise20181101-1.46.0/alibabacloud_dms_enterprise20181101.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2023-04-24 09:03:11.000000 alibabacloud_dms-enterprise20181101-1.46.0/alibabacloud_dms_enterprise20181101.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-24 09:03:12.000000 alibabacloud_dms-enterprise20181101-1.46.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2667 2023-04-24 09:03:11.000000 alibabacloud_dms-enterprise20181101-1.46.0/setup.py
```

### Comparing `alibabacloud_dms-enterprise20181101-1.45.0/ChangeLog.md` & `alibabacloud_dms-enterprise20181101-1.46.0/ChangeLog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-04-11 Version: 1.45.0
+- Supported ListDataImportSQLPreCheckDetail,GetDataImportSQL,ListDataImportSQLType API.
+
 2023-01-13 Version: 1.44.0
 - Supported GetProxy, ListProxies to return RegionId information.
 - Supported SearchDatabase to return CatalogName information.
 
 2022-12-21 Version: 1.43.0
 - Supported GetProxyAccess API.
```

### Comparing `alibabacloud_dms-enterprise20181101-1.45.0/LICENSE` & `alibabacloud_dms-enterprise20181101-1.46.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dms-enterprise20181101-1.45.0/PKG-INFO` & `alibabacloud_dms-enterprise20181101-1.46.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dms-enterprise20181101
-Version: 1.45.0
+Version: 1.46.0
 Summary: Alibaba Cloud dms-enterprise (20181101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dms-enterprise20181101-1.45.0/README-CN.md` & `alibabacloud_dms-enterprise20181101-1.46.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dms-enterprise20181101-1.45.0/README.md` & `alibabacloud_dms-enterprise20181101-1.46.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dms-enterprise20181101-1.45.0/alibabacloud_dms_enterprise20181101/client.py` & `alibabacloud_dms-enterprise20181101-1.46.0/alibabacloud_dms_enterprise20181101/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1415,14 +1415,116 @@
         
         @param request: CreateDataCronClearOrderRequest
         @return: CreateDataCronClearOrderResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_data_cron_clear_order_with_options_async(request, runtime)
 
+    def create_data_export_order_with_options(
+        self,
+        tmp_req: dms_enterprise_20181101_models.CreateDataExportOrderRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.CreateDataExportOrderResponse:
+        UtilClient.validate_model(tmp_req)
+        request = dms_enterprise_20181101_models.CreateDataExportOrderShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.plugin_param):
+            request.plugin_param_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.plugin_param, 'PluginParam', 'json')
+        if not UtilClient.is_unset(tmp_req.related_user_list):
+            request.related_user_list_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.related_user_list, 'RelatedUserList', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.attachment_key):
+            query['AttachmentKey'] = request.attachment_key
+        if not UtilClient.is_unset(request.comment):
+            query['Comment'] = request.comment
+        if not UtilClient.is_unset(request.parent_id):
+            query['ParentId'] = request.parent_id
+        if not UtilClient.is_unset(request.plugin_param_shrink):
+            query['PluginParam'] = request.plugin_param_shrink
+        if not UtilClient.is_unset(request.related_user_list_shrink):
+            query['RelatedUserList'] = request.related_user_list_shrink
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreateDataExportOrder',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.CreateDataExportOrderResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def create_data_export_order_with_options_async(
+        self,
+        tmp_req: dms_enterprise_20181101_models.CreateDataExportOrderRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.CreateDataExportOrderResponse:
+        UtilClient.validate_model(tmp_req)
+        request = dms_enterprise_20181101_models.CreateDataExportOrderShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.plugin_param):
+            request.plugin_param_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.plugin_param, 'PluginParam', 'json')
+        if not UtilClient.is_unset(tmp_req.related_user_list):
+            request.related_user_list_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.related_user_list, 'RelatedUserList', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.attachment_key):
+            query['AttachmentKey'] = request.attachment_key
+        if not UtilClient.is_unset(request.comment):
+            query['Comment'] = request.comment
+        if not UtilClient.is_unset(request.parent_id):
+            query['ParentId'] = request.parent_id
+        if not UtilClient.is_unset(request.plugin_param_shrink):
+            query['PluginParam'] = request.plugin_param_shrink
+        if not UtilClient.is_unset(request.related_user_list_shrink):
+            query['RelatedUserList'] = request.related_user_list_shrink
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreateDataExportOrder',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.CreateDataExportOrderResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def create_data_export_order(
+        self,
+        request: dms_enterprise_20181101_models.CreateDataExportOrderRequest,
+    ) -> dms_enterprise_20181101_models.CreateDataExportOrderResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.create_data_export_order_with_options(request, runtime)
+
+    async def create_data_export_order_async(
+        self,
+        request: dms_enterprise_20181101_models.CreateDataExportOrderRequest,
+    ) -> dms_enterprise_20181101_models.CreateDataExportOrderResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.create_data_export_order_with_options_async(request, runtime)
+
     def create_data_import_order_with_options(
         self,
         tmp_req: dms_enterprise_20181101_models.CreateDataImportOrderRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dms_enterprise_20181101_models.CreateDataImportOrderResponse:
         """
         For more information about the Large Data Import feature, see [Import data](~~161439~~).
@@ -1539,14 +1641,210 @@
         
         @param request: CreateDataImportOrderRequest
         @return: CreateDataImportOrderResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_data_import_order_with_options_async(request, runtime)
 
+    def create_data_track_order_with_options(
+        self,
+        tmp_req: dms_enterprise_20181101_models.CreateDataTrackOrderRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.CreateDataTrackOrderResponse:
+        UtilClient.validate_model(tmp_req)
+        request = dms_enterprise_20181101_models.CreateDataTrackOrderShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.param):
+            request.param_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.param, 'Param', 'json')
+        if not UtilClient.is_unset(tmp_req.related_user_list):
+            request.related_user_list_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.related_user_list, 'RelatedUserList', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.comment):
+            query['Comment'] = request.comment
+        if not UtilClient.is_unset(request.param_shrink):
+            query['Param'] = request.param_shrink
+        if not UtilClient.is_unset(request.related_user_list_shrink):
+            query['RelatedUserList'] = request.related_user_list_shrink
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreateDataTrackOrder',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.CreateDataTrackOrderResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def create_data_track_order_with_options_async(
+        self,
+        tmp_req: dms_enterprise_20181101_models.CreateDataTrackOrderRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.CreateDataTrackOrderResponse:
+        UtilClient.validate_model(tmp_req)
+        request = dms_enterprise_20181101_models.CreateDataTrackOrderShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.param):
+            request.param_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.param, 'Param', 'json')
+        if not UtilClient.is_unset(tmp_req.related_user_list):
+            request.related_user_list_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.related_user_list, 'RelatedUserList', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.comment):
+            query['Comment'] = request.comment
+        if not UtilClient.is_unset(request.param_shrink):
+            query['Param'] = request.param_shrink
+        if not UtilClient.is_unset(request.related_user_list_shrink):
+            query['RelatedUserList'] = request.related_user_list_shrink
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreateDataTrackOrder',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.CreateDataTrackOrderResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def create_data_track_order(
+        self,
+        request: dms_enterprise_20181101_models.CreateDataTrackOrderRequest,
+    ) -> dms_enterprise_20181101_models.CreateDataTrackOrderResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.create_data_track_order_with_options(request, runtime)
+
+    async def create_data_track_order_async(
+        self,
+        request: dms_enterprise_20181101_models.CreateDataTrackOrderRequest,
+    ) -> dms_enterprise_20181101_models.CreateDataTrackOrderResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.create_data_track_order_with_options_async(request, runtime)
+
+    def create_database_export_order_with_options(
+        self,
+        tmp_req: dms_enterprise_20181101_models.CreateDatabaseExportOrderRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.CreateDatabaseExportOrderResponse:
+        UtilClient.validate_model(tmp_req)
+        request = dms_enterprise_20181101_models.CreateDatabaseExportOrderShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.plugin_param):
+            request.plugin_param_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.plugin_param, 'PluginParam', 'json')
+        if not UtilClient.is_unset(tmp_req.related_user_list):
+            request.related_user_list_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.related_user_list, 'RelatedUserList', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.attachment_key):
+            query['AttachmentKey'] = request.attachment_key
+        if not UtilClient.is_unset(request.comment):
+            query['Comment'] = request.comment
+        if not UtilClient.is_unset(request.parent_id):
+            query['ParentId'] = request.parent_id
+        if not UtilClient.is_unset(request.plugin_param_shrink):
+            query['PluginParam'] = request.plugin_param_shrink
+        if not UtilClient.is_unset(request.related_user_list_shrink):
+            query['RelatedUserList'] = request.related_user_list_shrink
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreateDatabaseExportOrder',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.CreateDatabaseExportOrderResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def create_database_export_order_with_options_async(
+        self,
+        tmp_req: dms_enterprise_20181101_models.CreateDatabaseExportOrderRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.CreateDatabaseExportOrderResponse:
+        UtilClient.validate_model(tmp_req)
+        request = dms_enterprise_20181101_models.CreateDatabaseExportOrderShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.plugin_param):
+            request.plugin_param_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.plugin_param, 'PluginParam', 'json')
+        if not UtilClient.is_unset(tmp_req.related_user_list):
+            request.related_user_list_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.related_user_list, 'RelatedUserList', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.attachment_key):
+            query['AttachmentKey'] = request.attachment_key
+        if not UtilClient.is_unset(request.comment):
+            query['Comment'] = request.comment
+        if not UtilClient.is_unset(request.parent_id):
+            query['ParentId'] = request.parent_id
+        if not UtilClient.is_unset(request.plugin_param_shrink):
+            query['PluginParam'] = request.plugin_param_shrink
+        if not UtilClient.is_unset(request.related_user_list_shrink):
+            query['RelatedUserList'] = request.related_user_list_shrink
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreateDatabaseExportOrder',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.CreateDatabaseExportOrderResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def create_database_export_order(
+        self,
+        request: dms_enterprise_20181101_models.CreateDatabaseExportOrderRequest,
+    ) -> dms_enterprise_20181101_models.CreateDatabaseExportOrderResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.create_database_export_order_with_options(request, runtime)
+
+    async def create_database_export_order_async(
+        self,
+        request: dms_enterprise_20181101_models.CreateDatabaseExportOrderRequest,
+    ) -> dms_enterprise_20181101_models.CreateDatabaseExportOrderResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.create_database_export_order_with_options_async(request, runtime)
+
     def create_free_lock_correct_order_with_options(
         self,
         tmp_req: dms_enterprise_20181101_models.CreateFreeLockCorrectOrderRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dms_enterprise_20181101_models.CreateFreeLockCorrectOrderResponse:
         """
         For more information about the lock-free change feature, see [Overview](~~207847~~).
@@ -4273,14 +4571,136 @@
         
         @param request: DisableUserRequest
         @return: DisableUserResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.disable_user_with_options_async(request, runtime)
 
+    def download_data_track_result_with_options(
+        self,
+        tmp_req: dms_enterprise_20181101_models.DownloadDataTrackResultRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.DownloadDataTrackResultResponse:
+        UtilClient.validate_model(tmp_req)
+        request = dms_enterprise_20181101_models.DownloadDataTrackResultShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.column_filter):
+            request.column_filter_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.column_filter, 'ColumnFilter', 'json')
+        if not UtilClient.is_unset(tmp_req.event_id_list):
+            request.event_id_list_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.event_id_list, 'EventIdList', 'json')
+        if not UtilClient.is_unset(tmp_req.filter_table_list):
+            request.filter_table_list_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.filter_table_list, 'FilterTableList', 'json')
+        if not UtilClient.is_unset(tmp_req.filter_type_list):
+            request.filter_type_list_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.filter_type_list, 'FilterTypeList', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.column_filter_shrink):
+            query['ColumnFilter'] = request.column_filter_shrink
+        if not UtilClient.is_unset(request.event_id_list_shrink):
+            query['EventIdList'] = request.event_id_list_shrink
+        if not UtilClient.is_unset(request.filter_end_time):
+            query['FilterEndTime'] = request.filter_end_time
+        if not UtilClient.is_unset(request.filter_start_time):
+            query['FilterStartTime'] = request.filter_start_time
+        if not UtilClient.is_unset(request.filter_table_list_shrink):
+            query['FilterTableList'] = request.filter_table_list_shrink
+        if not UtilClient.is_unset(request.filter_type_list_shrink):
+            query['FilterTypeList'] = request.filter_type_list_shrink
+        if not UtilClient.is_unset(request.order_id):
+            query['OrderId'] = request.order_id
+        if not UtilClient.is_unset(request.rollback_sqltype):
+            query['RollbackSQLType'] = request.rollback_sqltype
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DownloadDataTrackResult',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.DownloadDataTrackResultResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def download_data_track_result_with_options_async(
+        self,
+        tmp_req: dms_enterprise_20181101_models.DownloadDataTrackResultRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.DownloadDataTrackResultResponse:
+        UtilClient.validate_model(tmp_req)
+        request = dms_enterprise_20181101_models.DownloadDataTrackResultShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.column_filter):
+            request.column_filter_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.column_filter, 'ColumnFilter', 'json')
+        if not UtilClient.is_unset(tmp_req.event_id_list):
+            request.event_id_list_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.event_id_list, 'EventIdList', 'json')
+        if not UtilClient.is_unset(tmp_req.filter_table_list):
+            request.filter_table_list_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.filter_table_list, 'FilterTableList', 'json')
+        if not UtilClient.is_unset(tmp_req.filter_type_list):
+            request.filter_type_list_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.filter_type_list, 'FilterTypeList', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.column_filter_shrink):
+            query['ColumnFilter'] = request.column_filter_shrink
+        if not UtilClient.is_unset(request.event_id_list_shrink):
+            query['EventIdList'] = request.event_id_list_shrink
+        if not UtilClient.is_unset(request.filter_end_time):
+            query['FilterEndTime'] = request.filter_end_time
+        if not UtilClient.is_unset(request.filter_start_time):
+            query['FilterStartTime'] = request.filter_start_time
+        if not UtilClient.is_unset(request.filter_table_list_shrink):
+            query['FilterTableList'] = request.filter_table_list_shrink
+        if not UtilClient.is_unset(request.filter_type_list_shrink):
+            query['FilterTypeList'] = request.filter_type_list_shrink
+        if not UtilClient.is_unset(request.order_id):
+            query['OrderId'] = request.order_id
+        if not UtilClient.is_unset(request.rollback_sqltype):
+            query['RollbackSQLType'] = request.rollback_sqltype
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DownloadDataTrackResult',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.DownloadDataTrackResultResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def download_data_track_result(
+        self,
+        request: dms_enterprise_20181101_models.DownloadDataTrackResultRequest,
+    ) -> dms_enterprise_20181101_models.DownloadDataTrackResultResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.download_data_track_result_with_options(request, runtime)
+
+    async def download_data_track_result_async(
+        self,
+        request: dms_enterprise_20181101_models.DownloadDataTrackResultRequest,
+    ) -> dms_enterprise_20181101_models.DownloadDataTrackResultResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.download_data_track_result_with_options_async(request, runtime)
+
     def edit_logic_database_with_options(
         self,
         tmp_req: dms_enterprise_20181101_models.EditLogicDatabaseRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dms_enterprise_20181101_models.EditLogicDatabaseResponse:
         UtilClient.validate_model(tmp_req)
         request = dms_enterprise_20181101_models.EditLogicDatabaseShrinkRequest()
@@ -6067,14 +6487,236 @@
     async def get_data_import_sql_async(
         self,
         request: dms_enterprise_20181101_models.GetDataImportSQLRequest,
     ) -> dms_enterprise_20181101_models.GetDataImportSQLResponse:
         runtime = util_models.RuntimeOptions()
         return await self.get_data_import_sqlwith_options_async(request, runtime)
 
+    def get_data_track_job_degree_with_options(
+        self,
+        request: dms_enterprise_20181101_models.GetDataTrackJobDegreeRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.GetDataTrackJobDegreeResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.order_id):
+            query['OrderId'] = request.order_id
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetDataTrackJobDegree',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.GetDataTrackJobDegreeResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_data_track_job_degree_with_options_async(
+        self,
+        request: dms_enterprise_20181101_models.GetDataTrackJobDegreeRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.GetDataTrackJobDegreeResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.order_id):
+            query['OrderId'] = request.order_id
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetDataTrackJobDegree',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.GetDataTrackJobDegreeResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_data_track_job_degree(
+        self,
+        request: dms_enterprise_20181101_models.GetDataTrackJobDegreeRequest,
+    ) -> dms_enterprise_20181101_models.GetDataTrackJobDegreeResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.get_data_track_job_degree_with_options(request, runtime)
+
+    async def get_data_track_job_degree_async(
+        self,
+        request: dms_enterprise_20181101_models.GetDataTrackJobDegreeRequest,
+    ) -> dms_enterprise_20181101_models.GetDataTrackJobDegreeResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.get_data_track_job_degree_with_options_async(request, runtime)
+
+    def get_data_track_job_table_meta_with_options(
+        self,
+        request: dms_enterprise_20181101_models.GetDataTrackJobTableMetaRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.GetDataTrackJobTableMetaResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.order_id):
+            query['OrderId'] = request.order_id
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetDataTrackJobTableMeta',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.GetDataTrackJobTableMetaResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_data_track_job_table_meta_with_options_async(
+        self,
+        request: dms_enterprise_20181101_models.GetDataTrackJobTableMetaRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.GetDataTrackJobTableMetaResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.order_id):
+            query['OrderId'] = request.order_id
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetDataTrackJobTableMeta',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.GetDataTrackJobTableMetaResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_data_track_job_table_meta(
+        self,
+        request: dms_enterprise_20181101_models.GetDataTrackJobTableMetaRequest,
+    ) -> dms_enterprise_20181101_models.GetDataTrackJobTableMetaResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.get_data_track_job_table_meta_with_options(request, runtime)
+
+    async def get_data_track_job_table_meta_async(
+        self,
+        request: dms_enterprise_20181101_models.GetDataTrackJobTableMetaRequest,
+    ) -> dms_enterprise_20181101_models.GetDataTrackJobTableMetaResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.get_data_track_job_table_meta_with_options_async(request, runtime)
+
+    def get_data_track_order_detail_with_options(
+        self,
+        request: dms_enterprise_20181101_models.GetDataTrackOrderDetailRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.GetDataTrackOrderDetailResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.order_id):
+            query['OrderId'] = request.order_id
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetDataTrackOrderDetail',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.GetDataTrackOrderDetailResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_data_track_order_detail_with_options_async(
+        self,
+        request: dms_enterprise_20181101_models.GetDataTrackOrderDetailRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.GetDataTrackOrderDetailResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.order_id):
+            query['OrderId'] = request.order_id
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetDataTrackOrderDetail',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.GetDataTrackOrderDetailResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_data_track_order_detail(
+        self,
+        request: dms_enterprise_20181101_models.GetDataTrackOrderDetailRequest,
+    ) -> dms_enterprise_20181101_models.GetDataTrackOrderDetailResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.get_data_track_order_detail_with_options(request, runtime)
+
+    async def get_data_track_order_detail_async(
+        self,
+        request: dms_enterprise_20181101_models.GetDataTrackOrderDetailRequest,
+    ) -> dms_enterprise_20181101_models.GetDataTrackOrderDetailResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.get_data_track_order_detail_with_options_async(request, runtime)
+
     def get_database_with_options(
         self,
         request: dms_enterprise_20181101_models.GetDatabaseRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dms_enterprise_20181101_models.GetDatabaseResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -6153,14 +6795,92 @@
     async def get_database_async(
         self,
         request: dms_enterprise_20181101_models.GetDatabaseRequest,
     ) -> dms_enterprise_20181101_models.GetDatabaseResponse:
         runtime = util_models.RuntimeOptions()
         return await self.get_database_with_options_async(request, runtime)
 
+    def get_database_export_order_detail_with_options(
+        self,
+        request: dms_enterprise_20181101_models.GetDatabaseExportOrderDetailRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.GetDatabaseExportOrderDetailResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        body = {}
+        if not UtilClient.is_unset(request.order_id):
+            body['OrderId'] = request.order_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='GetDatabaseExportOrderDetail',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.GetDatabaseExportOrderDetailResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_database_export_order_detail_with_options_async(
+        self,
+        request: dms_enterprise_20181101_models.GetDatabaseExportOrderDetailRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.GetDatabaseExportOrderDetailResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        body = {}
+        if not UtilClient.is_unset(request.order_id):
+            body['OrderId'] = request.order_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='GetDatabaseExportOrderDetail',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.GetDatabaseExportOrderDetailResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_database_export_order_detail(
+        self,
+        request: dms_enterprise_20181101_models.GetDatabaseExportOrderDetailRequest,
+    ) -> dms_enterprise_20181101_models.GetDatabaseExportOrderDetailResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.get_database_export_order_detail_with_options(request, runtime)
+
+    async def get_database_export_order_detail_async(
+        self,
+        request: dms_enterprise_20181101_models.GetDatabaseExportOrderDetailRequest,
+    ) -> dms_enterprise_20181101_models.GetDatabaseExportOrderDetailResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.get_database_export_order_detail_with_options_async(request, runtime)
+
     def get_instance_with_options(
         self,
         request: dms_enterprise_20181101_models.GetInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dms_enterprise_20181101_models.GetInstanceResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -13825,14 +14545,92 @@
     async def publish_and_deploy_task_flow_async(
         self,
         request: dms_enterprise_20181101_models.PublishAndDeployTaskFlowRequest,
     ) -> dms_enterprise_20181101_models.PublishAndDeployTaskFlowResponse:
         runtime = util_models.RuntimeOptions()
         return await self.publish_and_deploy_task_flow_with_options_async(request, runtime)
 
+    def query_data_track_result_download_status_with_options(
+        self,
+        request: dms_enterprise_20181101_models.QueryDataTrackResultDownloadStatusRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.QueryDataTrackResultDownloadStatusResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.download_key_id):
+            query['DownloadKeyId'] = request.download_key_id
+        if not UtilClient.is_unset(request.order_id):
+            query['OrderId'] = request.order_id
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='QueryDataTrackResultDownloadStatus',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.QueryDataTrackResultDownloadStatusResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def query_data_track_result_download_status_with_options_async(
+        self,
+        request: dms_enterprise_20181101_models.QueryDataTrackResultDownloadStatusRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.QueryDataTrackResultDownloadStatusResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.download_key_id):
+            query['DownloadKeyId'] = request.download_key_id
+        if not UtilClient.is_unset(request.order_id):
+            query['OrderId'] = request.order_id
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='QueryDataTrackResultDownloadStatus',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.QueryDataTrackResultDownloadStatusResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def query_data_track_result_download_status(
+        self,
+        request: dms_enterprise_20181101_models.QueryDataTrackResultDownloadStatusRequest,
+    ) -> dms_enterprise_20181101_models.QueryDataTrackResultDownloadStatusResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.query_data_track_result_download_status_with_options(request, runtime)
+
+    async def query_data_track_result_download_status_async(
+        self,
+        request: dms_enterprise_20181101_models.QueryDataTrackResultDownloadStatusRequest,
+    ) -> dms_enterprise_20181101_models.QueryDataTrackResultDownloadStatusResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.query_data_track_result_download_status_with_options_async(request, runtime)
+
     def re_deploy_lh_dag_version_with_options(
         self,
         request: dms_enterprise_20181101_models.ReDeployLhDagVersionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dms_enterprise_20181101_models.ReDeployLhDagVersionResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -14837,14 +15635,124 @@
     async def revoke_user_permission_async(
         self,
         request: dms_enterprise_20181101_models.RevokeUserPermissionRequest,
     ) -> dms_enterprise_20181101_models.RevokeUserPermissionResponse:
         runtime = util_models.RuntimeOptions()
         return await self.revoke_user_permission_with_options_async(request, runtime)
 
+    def search_data_track_result_with_options(
+        self,
+        tmp_req: dms_enterprise_20181101_models.SearchDataTrackResultRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.SearchDataTrackResultResponse:
+        UtilClient.validate_model(tmp_req)
+        request = dms_enterprise_20181101_models.SearchDataTrackResultShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.column_filter):
+            request.column_filter_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.column_filter, 'ColumnFilter', 'json')
+        if not UtilClient.is_unset(tmp_req.filter_table_list):
+            request.filter_table_list_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.filter_table_list, 'FilterTableList', 'json')
+        if not UtilClient.is_unset(tmp_req.filter_type_list):
+            request.filter_type_list_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.filter_type_list, 'FilterTypeList', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.column_filter_shrink):
+            query['ColumnFilter'] = request.column_filter_shrink
+        if not UtilClient.is_unset(request.filter_end_time):
+            query['FilterEndTime'] = request.filter_end_time
+        if not UtilClient.is_unset(request.filter_start_time):
+            query['FilterStartTime'] = request.filter_start_time
+        if not UtilClient.is_unset(request.filter_table_list_shrink):
+            query['FilterTableList'] = request.filter_table_list_shrink
+        if not UtilClient.is_unset(request.filter_type_list_shrink):
+            query['FilterTypeList'] = request.filter_type_list_shrink
+        if not UtilClient.is_unset(request.order_id):
+            query['OrderId'] = request.order_id
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SearchDataTrackResult',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.SearchDataTrackResultResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def search_data_track_result_with_options_async(
+        self,
+        tmp_req: dms_enterprise_20181101_models.SearchDataTrackResultRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.SearchDataTrackResultResponse:
+        UtilClient.validate_model(tmp_req)
+        request = dms_enterprise_20181101_models.SearchDataTrackResultShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.column_filter):
+            request.column_filter_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.column_filter, 'ColumnFilter', 'json')
+        if not UtilClient.is_unset(tmp_req.filter_table_list):
+            request.filter_table_list_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.filter_table_list, 'FilterTableList', 'json')
+        if not UtilClient.is_unset(tmp_req.filter_type_list):
+            request.filter_type_list_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.filter_type_list, 'FilterTypeList', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.column_filter_shrink):
+            query['ColumnFilter'] = request.column_filter_shrink
+        if not UtilClient.is_unset(request.filter_end_time):
+            query['FilterEndTime'] = request.filter_end_time
+        if not UtilClient.is_unset(request.filter_start_time):
+            query['FilterStartTime'] = request.filter_start_time
+        if not UtilClient.is_unset(request.filter_table_list_shrink):
+            query['FilterTableList'] = request.filter_table_list_shrink
+        if not UtilClient.is_unset(request.filter_type_list_shrink):
+            query['FilterTypeList'] = request.filter_type_list_shrink
+        if not UtilClient.is_unset(request.order_id):
+            query['OrderId'] = request.order_id
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SearchDataTrackResult',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.SearchDataTrackResultResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def search_data_track_result(
+        self,
+        request: dms_enterprise_20181101_models.SearchDataTrackResultRequest,
+    ) -> dms_enterprise_20181101_models.SearchDataTrackResultResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.search_data_track_result_with_options(request, runtime)
+
+    async def search_data_track_result_async(
+        self,
+        request: dms_enterprise_20181101_models.SearchDataTrackResultRequest,
+    ) -> dms_enterprise_20181101_models.SearchDataTrackResultResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.search_data_track_result_with_options_async(request, runtime)
+
     def search_database_with_options(
         self,
         request: dms_enterprise_20181101_models.SearchDatabaseRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dms_enterprise_20181101_models.SearchDatabaseResponse:
         UtilClient.validate_model(request)
         query = {}
```

### Comparing `alibabacloud_dms-enterprise20181101-1.45.0/alibabacloud_dms_enterprise20181101/models.py` & `alibabacloud_dms-enterprise20181101-1.46.0/alibabacloud_dms_enterprise20181101/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -3467,14 +3467,382 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateDataCronClearOrderResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateDataExportOrderRequestPluginParamWatermark(TeaModel):
+    def __init__(
+        self,
+        column_name: str = None,
+        data_watermark: str = None,
+        file_watermark: str = None,
+        keys: List[str] = None,
+        watermark_types: List[str] = None,
+    ):
+        self.column_name = column_name
+        self.data_watermark = data_watermark
+        self.file_watermark = file_watermark
+        self.keys = keys
+        self.watermark_types = watermark_types
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.column_name is not None:
+            result['ColumnName'] = self.column_name
+        if self.data_watermark is not None:
+            result['DataWatermark'] = self.data_watermark
+        if self.file_watermark is not None:
+            result['FileWatermark'] = self.file_watermark
+        if self.keys is not None:
+            result['Keys'] = self.keys
+        if self.watermark_types is not None:
+            result['WatermarkTypes'] = self.watermark_types
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ColumnName') is not None:
+            self.column_name = m.get('ColumnName')
+        if m.get('DataWatermark') is not None:
+            self.data_watermark = m.get('DataWatermark')
+        if m.get('FileWatermark') is not None:
+            self.file_watermark = m.get('FileWatermark')
+        if m.get('Keys') is not None:
+            self.keys = m.get('Keys')
+        if m.get('WatermarkTypes') is not None:
+            self.watermark_types = m.get('WatermarkTypes')
+        return self
+
+
+class CreateDataExportOrderRequestPluginParam(TeaModel):
+    def __init__(
+        self,
+        affect_rows: int = None,
+        classify: str = None,
+        db_id: int = None,
+        exe_sql: str = None,
+        ignore_affect_rows: bool = None,
+        ignore_affect_rows_reason: str = None,
+        instance_id: int = None,
+        logic: bool = None,
+        watermark: CreateDataExportOrderRequestPluginParamWatermark = None,
+    ):
+        self.affect_rows = affect_rows
+        self.classify = classify
+        self.db_id = db_id
+        self.exe_sql = exe_sql
+        self.ignore_affect_rows = ignore_affect_rows
+        self.ignore_affect_rows_reason = ignore_affect_rows_reason
+        self.instance_id = instance_id
+        self.logic = logic
+        self.watermark = watermark
+
+    def validate(self):
+        if self.watermark:
+            self.watermark.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.affect_rows is not None:
+            result['AffectRows'] = self.affect_rows
+        if self.classify is not None:
+            result['Classify'] = self.classify
+        if self.db_id is not None:
+            result['DbId'] = self.db_id
+        if self.exe_sql is not None:
+            result['ExeSQL'] = self.exe_sql
+        if self.ignore_affect_rows is not None:
+            result['IgnoreAffectRows'] = self.ignore_affect_rows
+        if self.ignore_affect_rows_reason is not None:
+            result['IgnoreAffectRowsReason'] = self.ignore_affect_rows_reason
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.logic is not None:
+            result['Logic'] = self.logic
+        if self.watermark is not None:
+            result['Watermark'] = self.watermark.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AffectRows') is not None:
+            self.affect_rows = m.get('AffectRows')
+        if m.get('Classify') is not None:
+            self.classify = m.get('Classify')
+        if m.get('DbId') is not None:
+            self.db_id = m.get('DbId')
+        if m.get('ExeSQL') is not None:
+            self.exe_sql = m.get('ExeSQL')
+        if m.get('IgnoreAffectRows') is not None:
+            self.ignore_affect_rows = m.get('IgnoreAffectRows')
+        if m.get('IgnoreAffectRowsReason') is not None:
+            self.ignore_affect_rows_reason = m.get('IgnoreAffectRowsReason')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('Logic') is not None:
+            self.logic = m.get('Logic')
+        if m.get('Watermark') is not None:
+            temp_model = CreateDataExportOrderRequestPluginParamWatermark()
+            self.watermark = temp_model.from_map(m['Watermark'])
+        return self
+
+
+class CreateDataExportOrderRequest(TeaModel):
+    def __init__(
+        self,
+        attachment_key: str = None,
+        comment: str = None,
+        parent_id: int = None,
+        plugin_param: CreateDataExportOrderRequestPluginParam = None,
+        related_user_list: List[int] = None,
+        tid: int = None,
+    ):
+        self.attachment_key = attachment_key
+        self.comment = comment
+        self.parent_id = parent_id
+        self.plugin_param = plugin_param
+        self.related_user_list = related_user_list
+        self.tid = tid
+
+    def validate(self):
+        if self.plugin_param:
+            self.plugin_param.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.attachment_key is not None:
+            result['AttachmentKey'] = self.attachment_key
+        if self.comment is not None:
+            result['Comment'] = self.comment
+        if self.parent_id is not None:
+            result['ParentId'] = self.parent_id
+        if self.plugin_param is not None:
+            result['PluginParam'] = self.plugin_param.to_map()
+        if self.related_user_list is not None:
+            result['RelatedUserList'] = self.related_user_list
+        if self.tid is not None:
+            result['Tid'] = self.tid
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AttachmentKey') is not None:
+            self.attachment_key = m.get('AttachmentKey')
+        if m.get('Comment') is not None:
+            self.comment = m.get('Comment')
+        if m.get('ParentId') is not None:
+            self.parent_id = m.get('ParentId')
+        if m.get('PluginParam') is not None:
+            temp_model = CreateDataExportOrderRequestPluginParam()
+            self.plugin_param = temp_model.from_map(m['PluginParam'])
+        if m.get('RelatedUserList') is not None:
+            self.related_user_list = m.get('RelatedUserList')
+        if m.get('Tid') is not None:
+            self.tid = m.get('Tid')
+        return self
+
+
+class CreateDataExportOrderShrinkRequest(TeaModel):
+    def __init__(
+        self,
+        attachment_key: str = None,
+        comment: str = None,
+        parent_id: int = None,
+        plugin_param_shrink: str = None,
+        related_user_list_shrink: str = None,
+        tid: int = None,
+    ):
+        self.attachment_key = attachment_key
+        self.comment = comment
+        self.parent_id = parent_id
+        self.plugin_param_shrink = plugin_param_shrink
+        self.related_user_list_shrink = related_user_list_shrink
+        self.tid = tid
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.attachment_key is not None:
+            result['AttachmentKey'] = self.attachment_key
+        if self.comment is not None:
+            result['Comment'] = self.comment
+        if self.parent_id is not None:
+            result['ParentId'] = self.parent_id
+        if self.plugin_param_shrink is not None:
+            result['PluginParam'] = self.plugin_param_shrink
+        if self.related_user_list_shrink is not None:
+            result['RelatedUserList'] = self.related_user_list_shrink
+        if self.tid is not None:
+            result['Tid'] = self.tid
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AttachmentKey') is not None:
+            self.attachment_key = m.get('AttachmentKey')
+        if m.get('Comment') is not None:
+            self.comment = m.get('Comment')
+        if m.get('ParentId') is not None:
+            self.parent_id = m.get('ParentId')
+        if m.get('PluginParam') is not None:
+            self.plugin_param_shrink = m.get('PluginParam')
+        if m.get('RelatedUserList') is not None:
+            self.related_user_list_shrink = m.get('RelatedUserList')
+        if m.get('Tid') is not None:
+            self.tid = m.get('Tid')
+        return self
+
+
+class CreateDataExportOrderResponseBodyCreateOrderResult(TeaModel):
+    def __init__(
+        self,
+        create_order_result: List[int] = None,
+    ):
+        self.create_order_result = create_order_result
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.create_order_result is not None:
+            result['CreateOrderResult'] = self.create_order_result
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CreateOrderResult') is not None:
+            self.create_order_result = m.get('CreateOrderResult')
+        return self
+
+
+class CreateDataExportOrderResponseBody(TeaModel):
+    def __init__(
+        self,
+        create_order_result: CreateDataExportOrderResponseBodyCreateOrderResult = None,
+        error_code: str = None,
+        error_message: str = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.create_order_result = create_order_result
+        self.error_code = error_code
+        self.error_message = error_message
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        if self.create_order_result:
+            self.create_order_result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.create_order_result is not None:
+            result['CreateOrderResult'] = self.create_order_result.to_map()
+        if self.error_code is not None:
+            result['ErrorCode'] = self.error_code
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CreateOrderResult') is not None:
+            temp_model = CreateDataExportOrderResponseBodyCreateOrderResult()
+            self.create_order_result = temp_model.from_map(m['CreateOrderResult'])
+        if m.get('ErrorCode') is not None:
+            self.error_code = m.get('ErrorCode')
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class CreateDataExportOrderResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CreateDataExportOrderResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = CreateDataExportOrderResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class CreateDataImportOrderRequestParamDbItemList(TeaModel):
     def __init__(
         self,
         db_id: int = None,
         logic: bool = None,
     ):
         # The ID of the database. The database can be a physical database or a logical database.
@@ -3881,14 +4249,614 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateDataImportOrderResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateDataTrackOrderRequestParam(TeaModel):
+    def __init__(
+        self,
+        db_id: str = None,
+        job_end_time: str = None,
+        job_start_time: str = None,
+        table_names: List[str] = None,
+        track_types: List[str] = None,
+    ):
+        self.db_id = db_id
+        self.job_end_time = job_end_time
+        self.job_start_time = job_start_time
+        self.table_names = table_names
+        self.track_types = track_types
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.db_id is not None:
+            result['DbId'] = self.db_id
+        if self.job_end_time is not None:
+            result['JobEndTime'] = self.job_end_time
+        if self.job_start_time is not None:
+            result['JobStartTime'] = self.job_start_time
+        if self.table_names is not None:
+            result['TableNames'] = self.table_names
+        if self.track_types is not None:
+            result['TrackTypes'] = self.track_types
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DbId') is not None:
+            self.db_id = m.get('DbId')
+        if m.get('JobEndTime') is not None:
+            self.job_end_time = m.get('JobEndTime')
+        if m.get('JobStartTime') is not None:
+            self.job_start_time = m.get('JobStartTime')
+        if m.get('TableNames') is not None:
+            self.table_names = m.get('TableNames')
+        if m.get('TrackTypes') is not None:
+            self.track_types = m.get('TrackTypes')
+        return self
+
+
+class CreateDataTrackOrderRequest(TeaModel):
+    def __init__(
+        self,
+        comment: str = None,
+        param: CreateDataTrackOrderRequestParam = None,
+        related_user_list: List[str] = None,
+        tid: int = None,
+    ):
+        self.comment = comment
+        self.param = param
+        self.related_user_list = related_user_list
+        self.tid = tid
+
+    def validate(self):
+        if self.param:
+            self.param.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.comment is not None:
+            result['Comment'] = self.comment
+        if self.param is not None:
+            result['Param'] = self.param.to_map()
+        if self.related_user_list is not None:
+            result['RelatedUserList'] = self.related_user_list
+        if self.tid is not None:
+            result['Tid'] = self.tid
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Comment') is not None:
+            self.comment = m.get('Comment')
+        if m.get('Param') is not None:
+            temp_model = CreateDataTrackOrderRequestParam()
+            self.param = temp_model.from_map(m['Param'])
+        if m.get('RelatedUserList') is not None:
+            self.related_user_list = m.get('RelatedUserList')
+        if m.get('Tid') is not None:
+            self.tid = m.get('Tid')
+        return self
+
+
+class CreateDataTrackOrderShrinkRequest(TeaModel):
+    def __init__(
+        self,
+        comment: str = None,
+        param_shrink: str = None,
+        related_user_list_shrink: str = None,
+        tid: int = None,
+    ):
+        self.comment = comment
+        self.param_shrink = param_shrink
+        self.related_user_list_shrink = related_user_list_shrink
+        self.tid = tid
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.comment is not None:
+            result['Comment'] = self.comment
+        if self.param_shrink is not None:
+            result['Param'] = self.param_shrink
+        if self.related_user_list_shrink is not None:
+            result['RelatedUserList'] = self.related_user_list_shrink
+        if self.tid is not None:
+            result['Tid'] = self.tid
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Comment') is not None:
+            self.comment = m.get('Comment')
+        if m.get('Param') is not None:
+            self.param_shrink = m.get('Param')
+        if m.get('RelatedUserList') is not None:
+            self.related_user_list_shrink = m.get('RelatedUserList')
+        if m.get('Tid') is not None:
+            self.tid = m.get('Tid')
+        return self
+
+
+class CreateDataTrackOrderResponseBody(TeaModel):
+    def __init__(
+        self,
+        create_order_result: List[int] = None,
+        error_code: str = None,
+        error_message: str = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.create_order_result = create_order_result
+        self.error_code = error_code
+        self.error_message = error_message
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.create_order_result is not None:
+            result['CreateOrderResult'] = self.create_order_result
+        if self.error_code is not None:
+            result['ErrorCode'] = self.error_code
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CreateOrderResult') is not None:
+            self.create_order_result = m.get('CreateOrderResult')
+        if m.get('ErrorCode') is not None:
+            self.error_code = m.get('ErrorCode')
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class CreateDataTrackOrderResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CreateDataTrackOrderResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = CreateDataTrackOrderResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class CreateDatabaseExportOrderRequestPluginParamConfig(TeaModel):
+    def __init__(
+        self,
+        data_option: List[str] = None,
+        export_content: str = None,
+        export_types: List[str] = None,
+        sqlext_option: List[str] = None,
+        selected_tables: List[str] = None,
+        tables: Dict[str, str] = None,
+        target_option: str = None,
+    ):
+        self.data_option = data_option
+        self.export_content = export_content
+        self.export_types = export_types
+        self.sqlext_option = sqlext_option
+        self.selected_tables = selected_tables
+        self.tables = tables
+        self.target_option = target_option
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.data_option is not None:
+            result['DataOption'] = self.data_option
+        if self.export_content is not None:
+            result['ExportContent'] = self.export_content
+        if self.export_types is not None:
+            result['ExportTypes'] = self.export_types
+        if self.sqlext_option is not None:
+            result['SQLExtOption'] = self.sqlext_option
+        if self.selected_tables is not None:
+            result['SelectedTables'] = self.selected_tables
+        if self.tables is not None:
+            result['Tables'] = self.tables
+        if self.target_option is not None:
+            result['TargetOption'] = self.target_option
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DataOption') is not None:
+            self.data_option = m.get('DataOption')
+        if m.get('ExportContent') is not None:
+            self.export_content = m.get('ExportContent')
+        if m.get('ExportTypes') is not None:
+            self.export_types = m.get('ExportTypes')
+        if m.get('SQLExtOption') is not None:
+            self.sqlext_option = m.get('SQLExtOption')
+        if m.get('SelectedTables') is not None:
+            self.selected_tables = m.get('SelectedTables')
+        if m.get('Tables') is not None:
+            self.tables = m.get('Tables')
+        if m.get('TargetOption') is not None:
+            self.target_option = m.get('TargetOption')
+        return self
+
+
+class CreateDatabaseExportOrderRequestPluginParam(TeaModel):
+    def __init__(
+        self,
+        classify: str = None,
+        config: CreateDatabaseExportOrderRequestPluginParamConfig = None,
+        db_id: int = None,
+        instance_id: int = None,
+        logic: bool = None,
+        search_name: str = None,
+    ):
+        self.classify = classify
+        self.config = config
+        self.db_id = db_id
+        self.instance_id = instance_id
+        self.logic = logic
+        self.search_name = search_name
+
+    def validate(self):
+        if self.config:
+            self.config.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.classify is not None:
+            result['Classify'] = self.classify
+        if self.config is not None:
+            result['Config'] = self.config.to_map()
+        if self.db_id is not None:
+            result['DbId'] = self.db_id
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.logic is not None:
+            result['Logic'] = self.logic
+        if self.search_name is not None:
+            result['SearchName'] = self.search_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Classify') is not None:
+            self.classify = m.get('Classify')
+        if m.get('Config') is not None:
+            temp_model = CreateDatabaseExportOrderRequestPluginParamConfig()
+            self.config = temp_model.from_map(m['Config'])
+        if m.get('DbId') is not None:
+            self.db_id = m.get('DbId')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('Logic') is not None:
+            self.logic = m.get('Logic')
+        if m.get('SearchName') is not None:
+            self.search_name = m.get('SearchName')
+        return self
+
+
+class CreateDatabaseExportOrderRequest(TeaModel):
+    def __init__(
+        self,
+        attachment_key: str = None,
+        comment: str = None,
+        parent_id: int = None,
+        plugin_param: CreateDatabaseExportOrderRequestPluginParam = None,
+        related_user_list: List[int] = None,
+        tid: int = None,
+    ):
+        self.attachment_key = attachment_key
+        self.comment = comment
+        self.parent_id = parent_id
+        self.plugin_param = plugin_param
+        self.related_user_list = related_user_list
+        self.tid = tid
+
+    def validate(self):
+        if self.plugin_param:
+            self.plugin_param.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.attachment_key is not None:
+            result['AttachmentKey'] = self.attachment_key
+        if self.comment is not None:
+            result['Comment'] = self.comment
+        if self.parent_id is not None:
+            result['ParentId'] = self.parent_id
+        if self.plugin_param is not None:
+            result['PluginParam'] = self.plugin_param.to_map()
+        if self.related_user_list is not None:
+            result['RelatedUserList'] = self.related_user_list
+        if self.tid is not None:
+            result['Tid'] = self.tid
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AttachmentKey') is not None:
+            self.attachment_key = m.get('AttachmentKey')
+        if m.get('Comment') is not None:
+            self.comment = m.get('Comment')
+        if m.get('ParentId') is not None:
+            self.parent_id = m.get('ParentId')
+        if m.get('PluginParam') is not None:
+            temp_model = CreateDatabaseExportOrderRequestPluginParam()
+            self.plugin_param = temp_model.from_map(m['PluginParam'])
+        if m.get('RelatedUserList') is not None:
+            self.related_user_list = m.get('RelatedUserList')
+        if m.get('Tid') is not None:
+            self.tid = m.get('Tid')
+        return self
+
+
+class CreateDatabaseExportOrderShrinkRequest(TeaModel):
+    def __init__(
+        self,
+        attachment_key: str = None,
+        comment: str = None,
+        parent_id: int = None,
+        plugin_param_shrink: str = None,
+        related_user_list_shrink: str = None,
+        tid: int = None,
+    ):
+        self.attachment_key = attachment_key
+        self.comment = comment
+        self.parent_id = parent_id
+        self.plugin_param_shrink = plugin_param_shrink
+        self.related_user_list_shrink = related_user_list_shrink
+        self.tid = tid
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.attachment_key is not None:
+            result['AttachmentKey'] = self.attachment_key
+        if self.comment is not None:
+            result['Comment'] = self.comment
+        if self.parent_id is not None:
+            result['ParentId'] = self.parent_id
+        if self.plugin_param_shrink is not None:
+            result['PluginParam'] = self.plugin_param_shrink
+        if self.related_user_list_shrink is not None:
+            result['RelatedUserList'] = self.related_user_list_shrink
+        if self.tid is not None:
+            result['Tid'] = self.tid
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AttachmentKey') is not None:
+            self.attachment_key = m.get('AttachmentKey')
+        if m.get('Comment') is not None:
+            self.comment = m.get('Comment')
+        if m.get('ParentId') is not None:
+            self.parent_id = m.get('ParentId')
+        if m.get('PluginParam') is not None:
+            self.plugin_param_shrink = m.get('PluginParam')
+        if m.get('RelatedUserList') is not None:
+            self.related_user_list_shrink = m.get('RelatedUserList')
+        if m.get('Tid') is not None:
+            self.tid = m.get('Tid')
+        return self
+
+
+class CreateDatabaseExportOrderResponseBodyCreateOrderResult(TeaModel):
+    def __init__(
+        self,
+        create_order_result: List[int] = None,
+    ):
+        self.create_order_result = create_order_result
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.create_order_result is not None:
+            result['CreateOrderResult'] = self.create_order_result
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CreateOrderResult') is not None:
+            self.create_order_result = m.get('CreateOrderResult')
+        return self
+
+
+class CreateDatabaseExportOrderResponseBody(TeaModel):
+    def __init__(
+        self,
+        create_order_result: CreateDatabaseExportOrderResponseBodyCreateOrderResult = None,
+        error_code: str = None,
+        error_message: str = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.create_order_result = create_order_result
+        self.error_code = error_code
+        self.error_message = error_message
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        if self.create_order_result:
+            self.create_order_result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.create_order_result is not None:
+            result['CreateOrderResult'] = self.create_order_result.to_map()
+        if self.error_code is not None:
+            result['ErrorCode'] = self.error_code
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CreateOrderResult') is not None:
+            temp_model = CreateDatabaseExportOrderResponseBodyCreateOrderResult()
+            self.create_order_result = temp_model.from_map(m['CreateOrderResult'])
+        if m.get('ErrorCode') is not None:
+            self.error_code = m.get('ErrorCode')
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class CreateDatabaseExportOrderResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CreateDatabaseExportOrderResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = CreateDatabaseExportOrderResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class CreateFreeLockCorrectOrderRequestParamDbItemList(TeaModel):
     def __init__(
         self,
         db_id: int = None,
         logic: bool = None,
     ):
         # The ID of the database. The database can be a physical database or a logical database.
@@ -8970,14 +9938,318 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DisableUserResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DownloadDataTrackResultRequestColumnFilter(TeaModel):
+    def __init__(
+        self,
+        between_end: str = None,
+        between_start: str = None,
+        column_name: str = None,
+        in_list: List[str] = None,
+        operator: str = None,
+        value: str = None,
+    ):
+        self.between_end = between_end
+        self.between_start = between_start
+        self.column_name = column_name
+        self.in_list = in_list
+        self.operator = operator
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.between_end is not None:
+            result['BetweenEnd'] = self.between_end
+        if self.between_start is not None:
+            result['BetweenStart'] = self.between_start
+        if self.column_name is not None:
+            result['ColumnName'] = self.column_name
+        if self.in_list is not None:
+            result['InList'] = self.in_list
+        if self.operator is not None:
+            result['Operator'] = self.operator
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('BetweenEnd') is not None:
+            self.between_end = m.get('BetweenEnd')
+        if m.get('BetweenStart') is not None:
+            self.between_start = m.get('BetweenStart')
+        if m.get('ColumnName') is not None:
+            self.column_name = m.get('ColumnName')
+        if m.get('InList') is not None:
+            self.in_list = m.get('InList')
+        if m.get('Operator') is not None:
+            self.operator = m.get('Operator')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class DownloadDataTrackResultRequest(TeaModel):
+    def __init__(
+        self,
+        column_filter: DownloadDataTrackResultRequestColumnFilter = None,
+        event_id_list: List[int] = None,
+        filter_end_time: str = None,
+        filter_start_time: str = None,
+        filter_table_list: List[str] = None,
+        filter_type_list: List[str] = None,
+        order_id: int = None,
+        rollback_sqltype: str = None,
+        tid: int = None,
+    ):
+        self.column_filter = column_filter
+        self.event_id_list = event_id_list
+        self.filter_end_time = filter_end_time
+        self.filter_start_time = filter_start_time
+        self.filter_table_list = filter_table_list
+        self.filter_type_list = filter_type_list
+        self.order_id = order_id
+        self.rollback_sqltype = rollback_sqltype
+        self.tid = tid
+
+    def validate(self):
+        if self.column_filter:
+            self.column_filter.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.column_filter is not None:
+            result['ColumnFilter'] = self.column_filter.to_map()
+        if self.event_id_list is not None:
+            result['EventIdList'] = self.event_id_list
+        if self.filter_end_time is not None:
+            result['FilterEndTime'] = self.filter_end_time
+        if self.filter_start_time is not None:
+            result['FilterStartTime'] = self.filter_start_time
+        if self.filter_table_list is not None:
+            result['FilterTableList'] = self.filter_table_list
+        if self.filter_type_list is not None:
+            result['FilterTypeList'] = self.filter_type_list
+        if self.order_id is not None:
+            result['OrderId'] = self.order_id
+        if self.rollback_sqltype is not None:
+            result['RollbackSQLType'] = self.rollback_sqltype
+        if self.tid is not None:
+            result['Tid'] = self.tid
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ColumnFilter') is not None:
+            temp_model = DownloadDataTrackResultRequestColumnFilter()
+            self.column_filter = temp_model.from_map(m['ColumnFilter'])
+        if m.get('EventIdList') is not None:
+            self.event_id_list = m.get('EventIdList')
+        if m.get('FilterEndTime') is not None:
+            self.filter_end_time = m.get('FilterEndTime')
+        if m.get('FilterStartTime') is not None:
+            self.filter_start_time = m.get('FilterStartTime')
+        if m.get('FilterTableList') is not None:
+            self.filter_table_list = m.get('FilterTableList')
+        if m.get('FilterTypeList') is not None:
+            self.filter_type_list = m.get('FilterTypeList')
+        if m.get('OrderId') is not None:
+            self.order_id = m.get('OrderId')
+        if m.get('RollbackSQLType') is not None:
+            self.rollback_sqltype = m.get('RollbackSQLType')
+        if m.get('Tid') is not None:
+            self.tid = m.get('Tid')
+        return self
+
+
+class DownloadDataTrackResultShrinkRequest(TeaModel):
+    def __init__(
+        self,
+        column_filter_shrink: str = None,
+        event_id_list_shrink: str = None,
+        filter_end_time: str = None,
+        filter_start_time: str = None,
+        filter_table_list_shrink: str = None,
+        filter_type_list_shrink: str = None,
+        order_id: int = None,
+        rollback_sqltype: str = None,
+        tid: int = None,
+    ):
+        self.column_filter_shrink = column_filter_shrink
+        self.event_id_list_shrink = event_id_list_shrink
+        self.filter_end_time = filter_end_time
+        self.filter_start_time = filter_start_time
+        self.filter_table_list_shrink = filter_table_list_shrink
+        self.filter_type_list_shrink = filter_type_list_shrink
+        self.order_id = order_id
+        self.rollback_sqltype = rollback_sqltype
+        self.tid = tid
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.column_filter_shrink is not None:
+            result['ColumnFilter'] = self.column_filter_shrink
+        if self.event_id_list_shrink is not None:
+            result['EventIdList'] = self.event_id_list_shrink
+        if self.filter_end_time is not None:
+            result['FilterEndTime'] = self.filter_end_time
+        if self.filter_start_time is not None:
+            result['FilterStartTime'] = self.filter_start_time
+        if self.filter_table_list_shrink is not None:
+            result['FilterTableList'] = self.filter_table_list_shrink
+        if self.filter_type_list_shrink is not None:
+            result['FilterTypeList'] = self.filter_type_list_shrink
+        if self.order_id is not None:
+            result['OrderId'] = self.order_id
+        if self.rollback_sqltype is not None:
+            result['RollbackSQLType'] = self.rollback_sqltype
+        if self.tid is not None:
+            result['Tid'] = self.tid
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ColumnFilter') is not None:
+            self.column_filter_shrink = m.get('ColumnFilter')
+        if m.get('EventIdList') is not None:
+            self.event_id_list_shrink = m.get('EventIdList')
+        if m.get('FilterEndTime') is not None:
+            self.filter_end_time = m.get('FilterEndTime')
+        if m.get('FilterStartTime') is not None:
+            self.filter_start_time = m.get('FilterStartTime')
+        if m.get('FilterTableList') is not None:
+            self.filter_table_list_shrink = m.get('FilterTableList')
+        if m.get('FilterTypeList') is not None:
+            self.filter_type_list_shrink = m.get('FilterTypeList')
+        if m.get('OrderId') is not None:
+            self.order_id = m.get('OrderId')
+        if m.get('RollbackSQLType') is not None:
+            self.rollback_sqltype = m.get('RollbackSQLType')
+        if m.get('Tid') is not None:
+            self.tid = m.get('Tid')
+        return self
+
+
+class DownloadDataTrackResultResponseBody(TeaModel):
+    def __init__(
+        self,
+        download_key_id: str = None,
+        error_code: str = None,
+        error_message: str = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.download_key_id = download_key_id
+        self.error_code = error_code
+        self.error_message = error_message
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.download_key_id is not None:
+            result['DownloadKeyId'] = self.download_key_id
+        if self.error_code is not None:
+            result['ErrorCode'] = self.error_code
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DownloadKeyId') is not None:
+            self.download_key_id = m.get('DownloadKeyId')
+        if m.get('ErrorCode') is not None:
+            self.error_code = m.get('ErrorCode')
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class DownloadDataTrackResultResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DownloadDataTrackResultResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DownloadDataTrackResultResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class EditLogicDatabaseRequest(TeaModel):
     def __init__(
         self,
         alias: str = None,
         database_ids: List[int] = None,
         logic_db_id: int = None,
         tid: int = None,
@@ -13918,14 +15190,640 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetDataImportSQLResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetDataTrackJobDegreeRequest(TeaModel):
+    def __init__(
+        self,
+        order_id: int = None,
+        tid: int = None,
+    ):
+        self.order_id = order_id
+        self.tid = tid
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.order_id is not None:
+            result['OrderId'] = self.order_id
+        if self.tid is not None:
+            result['Tid'] = self.tid
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('OrderId') is not None:
+            self.order_id = m.get('OrderId')
+        if m.get('Tid') is not None:
+            self.tid = m.get('Tid')
+        return self
+
+
+class GetDataTrackJobDegreeResponseBodyJobDegree(TeaModel):
+    def __init__(
+        self,
+        download_completion_degree: float = None,
+        filter_completion_degree: float = None,
+        job_status: str = None,
+        list_completion_degree: float = None,
+        status_desc: str = None,
+    ):
+        self.download_completion_degree = download_completion_degree
+        self.filter_completion_degree = filter_completion_degree
+        self.job_status = job_status
+        self.list_completion_degree = list_completion_degree
+        self.status_desc = status_desc
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.download_completion_degree is not None:
+            result['DownloadCompletionDegree'] = self.download_completion_degree
+        if self.filter_completion_degree is not None:
+            result['FilterCompletionDegree'] = self.filter_completion_degree
+        if self.job_status is not None:
+            result['JobStatus'] = self.job_status
+        if self.list_completion_degree is not None:
+            result['ListCompletionDegree'] = self.list_completion_degree
+        if self.status_desc is not None:
+            result['StatusDesc'] = self.status_desc
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DownloadCompletionDegree') is not None:
+            self.download_completion_degree = m.get('DownloadCompletionDegree')
+        if m.get('FilterCompletionDegree') is not None:
+            self.filter_completion_degree = m.get('FilterCompletionDegree')
+        if m.get('JobStatus') is not None:
+            self.job_status = m.get('JobStatus')
+        if m.get('ListCompletionDegree') is not None:
+            self.list_completion_degree = m.get('ListCompletionDegree')
+        if m.get('StatusDesc') is not None:
+            self.status_desc = m.get('StatusDesc')
+        return self
+
+
+class GetDataTrackJobDegreeResponseBody(TeaModel):
+    def __init__(
+        self,
+        error_code: str = None,
+        error_message: str = None,
+        job_degree: GetDataTrackJobDegreeResponseBodyJobDegree = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.error_code = error_code
+        self.error_message = error_message
+        self.job_degree = job_degree
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        if self.job_degree:
+            self.job_degree.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.error_code is not None:
+            result['ErrorCode'] = self.error_code
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        if self.job_degree is not None:
+            result['JobDegree'] = self.job_degree.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ErrorCode') is not None:
+            self.error_code = m.get('ErrorCode')
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        if m.get('JobDegree') is not None:
+            temp_model = GetDataTrackJobDegreeResponseBodyJobDegree()
+            self.job_degree = temp_model.from_map(m['JobDegree'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class GetDataTrackJobDegreeResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetDataTrackJobDegreeResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetDataTrackJobDegreeResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class GetDataTrackJobTableMetaRequest(TeaModel):
+    def __init__(
+        self,
+        order_id: int = None,
+        tid: int = None,
+    ):
+        self.order_id = order_id
+        self.tid = tid
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.order_id is not None:
+            result['OrderId'] = self.order_id
+        if self.tid is not None:
+            result['Tid'] = self.tid
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('OrderId') is not None:
+            self.order_id = m.get('OrderId')
+        if m.get('Tid') is not None:
+            self.tid = m.get('Tid')
+        return self
+
+
+class GetDataTrackJobTableMetaResponseBodyTableMetaListColumns(TeaModel):
+    def __init__(
+        self,
+        charset: str = None,
+        column_name: str = None,
+        column_position: int = None,
+        column_type: str = None,
+        fictive: bool = None,
+    ):
+        self.charset = charset
+        self.column_name = column_name
+        self.column_position = column_position
+        self.column_type = column_type
+        self.fictive = fictive
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.charset is not None:
+            result['Charset'] = self.charset
+        if self.column_name is not None:
+            result['ColumnName'] = self.column_name
+        if self.column_position is not None:
+            result['ColumnPosition'] = self.column_position
+        if self.column_type is not None:
+            result['ColumnType'] = self.column_type
+        if self.fictive is not None:
+            result['Fictive'] = self.fictive
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Charset') is not None:
+            self.charset = m.get('Charset')
+        if m.get('ColumnName') is not None:
+            self.column_name = m.get('ColumnName')
+        if m.get('ColumnPosition') is not None:
+            self.column_position = m.get('ColumnPosition')
+        if m.get('ColumnType') is not None:
+            self.column_type = m.get('ColumnType')
+        if m.get('Fictive') is not None:
+            self.fictive = m.get('Fictive')
+        return self
+
+
+class GetDataTrackJobTableMetaResponseBodyTableMetaList(TeaModel):
+    def __init__(
+        self,
+        columns: List[GetDataTrackJobTableMetaResponseBodyTableMetaListColumns] = None,
+        schema_name: str = None,
+        table_name: str = None,
+    ):
+        self.columns = columns
+        self.schema_name = schema_name
+        self.table_name = table_name
+
+    def validate(self):
+        if self.columns:
+            for k in self.columns:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Columns'] = []
+        if self.columns is not None:
+            for k in self.columns:
+                result['Columns'].append(k.to_map() if k else None)
+        if self.schema_name is not None:
+            result['SchemaName'] = self.schema_name
+        if self.table_name is not None:
+            result['TableName'] = self.table_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.columns = []
+        if m.get('Columns') is not None:
+            for k in m.get('Columns'):
+                temp_model = GetDataTrackJobTableMetaResponseBodyTableMetaListColumns()
+                self.columns.append(temp_model.from_map(k))
+        if m.get('SchemaName') is not None:
+            self.schema_name = m.get('SchemaName')
+        if m.get('TableName') is not None:
+            self.table_name = m.get('TableName')
+        return self
+
+
+class GetDataTrackJobTableMetaResponseBody(TeaModel):
+    def __init__(
+        self,
+        error_code: str = None,
+        error_message: str = None,
+        request_id: str = None,
+        success: bool = None,
+        table_meta_list: List[GetDataTrackJobTableMetaResponseBodyTableMetaList] = None,
+    ):
+        self.error_code = error_code
+        self.error_message = error_message
+        self.request_id = request_id
+        self.success = success
+        self.table_meta_list = table_meta_list
+
+    def validate(self):
+        if self.table_meta_list:
+            for k in self.table_meta_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.error_code is not None:
+            result['ErrorCode'] = self.error_code
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        result['TableMetaList'] = []
+        if self.table_meta_list is not None:
+            for k in self.table_meta_list:
+                result['TableMetaList'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ErrorCode') is not None:
+            self.error_code = m.get('ErrorCode')
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        self.table_meta_list = []
+        if m.get('TableMetaList') is not None:
+            for k in m.get('TableMetaList'):
+                temp_model = GetDataTrackJobTableMetaResponseBodyTableMetaList()
+                self.table_meta_list.append(temp_model.from_map(k))
+        return self
+
+
+class GetDataTrackJobTableMetaResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetDataTrackJobTableMetaResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetDataTrackJobTableMetaResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class GetDataTrackOrderDetailRequest(TeaModel):
+    def __init__(
+        self,
+        order_id: int = None,
+        tid: int = None,
+    ):
+        self.order_id = order_id
+        self.tid = tid
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.order_id is not None:
+            result['OrderId'] = self.order_id
+        if self.tid is not None:
+            result['Tid'] = self.tid
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('OrderId') is not None:
+            self.order_id = m.get('OrderId')
+        if m.get('Tid') is not None:
+            self.tid = m.get('Tid')
+        return self
+
+
+class GetDataTrackOrderDetailResponseBodyDataTrackOrderDetail(TeaModel):
+    def __init__(
+        self,
+        database_search_name: str = None,
+        db_id: int = None,
+        job_end_time: str = None,
+        job_start_time: str = None,
+        job_status: str = None,
+        logic: bool = None,
+        schema_name: str = None,
+        status_desc: str = None,
+        table_names: List[str] = None,
+        track_types: List[str] = None,
+    ):
+        self.database_search_name = database_search_name
+        self.db_id = db_id
+        self.job_end_time = job_end_time
+        self.job_start_time = job_start_time
+        self.job_status = job_status
+        self.logic = logic
+        self.schema_name = schema_name
+        self.status_desc = status_desc
+        self.table_names = table_names
+        self.track_types = track_types
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.database_search_name is not None:
+            result['DatabaseSearchName'] = self.database_search_name
+        if self.db_id is not None:
+            result['DbId'] = self.db_id
+        if self.job_end_time is not None:
+            result['JobEndTime'] = self.job_end_time
+        if self.job_start_time is not None:
+            result['JobStartTime'] = self.job_start_time
+        if self.job_status is not None:
+            result['JobStatus'] = self.job_status
+        if self.logic is not None:
+            result['Logic'] = self.logic
+        if self.schema_name is not None:
+            result['SchemaName'] = self.schema_name
+        if self.status_desc is not None:
+            result['StatusDesc'] = self.status_desc
+        if self.table_names is not None:
+            result['TableNames'] = self.table_names
+        if self.track_types is not None:
+            result['TrackTypes'] = self.track_types
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DatabaseSearchName') is not None:
+            self.database_search_name = m.get('DatabaseSearchName')
+        if m.get('DbId') is not None:
+            self.db_id = m.get('DbId')
+        if m.get('JobEndTime') is not None:
+            self.job_end_time = m.get('JobEndTime')
+        if m.get('JobStartTime') is not None:
+            self.job_start_time = m.get('JobStartTime')
+        if m.get('JobStatus') is not None:
+            self.job_status = m.get('JobStatus')
+        if m.get('Logic') is not None:
+            self.logic = m.get('Logic')
+        if m.get('SchemaName') is not None:
+            self.schema_name = m.get('SchemaName')
+        if m.get('StatusDesc') is not None:
+            self.status_desc = m.get('StatusDesc')
+        if m.get('TableNames') is not None:
+            self.table_names = m.get('TableNames')
+        if m.get('TrackTypes') is not None:
+            self.track_types = m.get('TrackTypes')
+        return self
+
+
+class GetDataTrackOrderDetailResponseBody(TeaModel):
+    def __init__(
+        self,
+        data_track_order_detail: GetDataTrackOrderDetailResponseBodyDataTrackOrderDetail = None,
+        error_code: str = None,
+        error_message: str = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.data_track_order_detail = data_track_order_detail
+        self.error_code = error_code
+        self.error_message = error_message
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        if self.data_track_order_detail:
+            self.data_track_order_detail.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.data_track_order_detail is not None:
+            result['DataTrackOrderDetail'] = self.data_track_order_detail.to_map()
+        if self.error_code is not None:
+            result['ErrorCode'] = self.error_code
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DataTrackOrderDetail') is not None:
+            temp_model = GetDataTrackOrderDetailResponseBodyDataTrackOrderDetail()
+            self.data_track_order_detail = temp_model.from_map(m['DataTrackOrderDetail'])
+        if m.get('ErrorCode') is not None:
+            self.error_code = m.get('ErrorCode')
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class GetDataTrackOrderDetailResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetDataTrackOrderDetailResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetDataTrackOrderDetailResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetDatabaseRequest(TeaModel):
     def __init__(
         self,
         host: str = None,
         port: int = None,
         schema_name: str = None,
         sid: str = None,
@@ -14289,14 +16187,414 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetDatabaseResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetDatabaseExportOrderDetailRequest(TeaModel):
+    def __init__(
+        self,
+        order_id: int = None,
+        tid: int = None,
+    ):
+        self.order_id = order_id
+        self.tid = tid
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.order_id is not None:
+            result['OrderId'] = self.order_id
+        if self.tid is not None:
+            result['Tid'] = self.tid
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('OrderId') is not None:
+            self.order_id = m.get('OrderId')
+        if m.get('Tid') is not None:
+            self.tid = m.get('Tid')
+        return self
+
+
+class GetDatabaseExportOrderDetailResponseBodyDatabaseExportOrderDetailKeyInfoConfigExportTypes(TeaModel):
+    def __init__(
+        self,
+        export_types: List[str] = None,
+    ):
+        self.export_types = export_types
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.export_types is not None:
+            result['ExportTypes'] = self.export_types
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ExportTypes') is not None:
+            self.export_types = m.get('ExportTypes')
+        return self
+
+
+class GetDatabaseExportOrderDetailResponseBodyDatabaseExportOrderDetailKeyInfoConfigSQLExtOption(TeaModel):
+    def __init__(
+        self,
+        sqlext_option: List[str] = None,
+    ):
+        self.sqlext_option = sqlext_option
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.sqlext_option is not None:
+            result['SQLExtOption'] = self.sqlext_option
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('SQLExtOption') is not None:
+            self.sqlext_option = m.get('SQLExtOption')
+        return self
+
+
+class GetDatabaseExportOrderDetailResponseBodyDatabaseExportOrderDetailKeyInfoConfigSelectedTables(TeaModel):
+    def __init__(
+        self,
+        selected_tables: List[str] = None,
+    ):
+        self.selected_tables = selected_tables
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.selected_tables is not None:
+            result['SelectedTables'] = self.selected_tables
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('SelectedTables') is not None:
+            self.selected_tables = m.get('SelectedTables')
+        return self
+
+
+class GetDatabaseExportOrderDetailResponseBodyDatabaseExportOrderDetailKeyInfoConfig(TeaModel):
+    def __init__(
+        self,
+        db_name: str = None,
+        export_content: str = None,
+        export_types: GetDatabaseExportOrderDetailResponseBodyDatabaseExportOrderDetailKeyInfoConfigExportTypes = None,
+        sqlext_option: GetDatabaseExportOrderDetailResponseBodyDatabaseExportOrderDetailKeyInfoConfigSQLExtOption = None,
+        selected_tables: GetDatabaseExportOrderDetailResponseBodyDatabaseExportOrderDetailKeyInfoConfigSelectedTables = None,
+        target_option: str = None,
+    ):
+        self.db_name = db_name
+        self.export_content = export_content
+        self.export_types = export_types
+        self.sqlext_option = sqlext_option
+        self.selected_tables = selected_tables
+        self.target_option = target_option
+
+    def validate(self):
+        if self.export_types:
+            self.export_types.validate()
+        if self.sqlext_option:
+            self.sqlext_option.validate()
+        if self.selected_tables:
+            self.selected_tables.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.db_name is not None:
+            result['DbName'] = self.db_name
+        if self.export_content is not None:
+            result['ExportContent'] = self.export_content
+        if self.export_types is not None:
+            result['ExportTypes'] = self.export_types.to_map()
+        if self.sqlext_option is not None:
+            result['SQLExtOption'] = self.sqlext_option.to_map()
+        if self.selected_tables is not None:
+            result['SelectedTables'] = self.selected_tables.to_map()
+        if self.target_option is not None:
+            result['TargetOption'] = self.target_option
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DbName') is not None:
+            self.db_name = m.get('DbName')
+        if m.get('ExportContent') is not None:
+            self.export_content = m.get('ExportContent')
+        if m.get('ExportTypes') is not None:
+            temp_model = GetDatabaseExportOrderDetailResponseBodyDatabaseExportOrderDetailKeyInfoConfigExportTypes()
+            self.export_types = temp_model.from_map(m['ExportTypes'])
+        if m.get('SQLExtOption') is not None:
+            temp_model = GetDatabaseExportOrderDetailResponseBodyDatabaseExportOrderDetailKeyInfoConfigSQLExtOption()
+            self.sqlext_option = temp_model.from_map(m['SQLExtOption'])
+        if m.get('SelectedTables') is not None:
+            temp_model = GetDatabaseExportOrderDetailResponseBodyDatabaseExportOrderDetailKeyInfoConfigSelectedTables()
+            self.selected_tables = temp_model.from_map(m['SelectedTables'])
+        if m.get('TargetOption') is not None:
+            self.target_option = m.get('TargetOption')
+        return self
+
+
+class GetDatabaseExportOrderDetailResponseBodyDatabaseExportOrderDetailKeyInfo(TeaModel):
+    def __init__(
+        self,
+        audit_date: str = None,
+        config: GetDatabaseExportOrderDetailResponseBodyDatabaseExportOrderDetailKeyInfoConfig = None,
+        db_id: int = None,
+        download_url: str = None,
+    ):
+        self.audit_date = audit_date
+        self.config = config
+        self.db_id = db_id
+        self.download_url = download_url
+
+    def validate(self):
+        if self.config:
+            self.config.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.audit_date is not None:
+            result['AuditDate'] = self.audit_date
+        if self.config is not None:
+            result['Config'] = self.config.to_map()
+        if self.db_id is not None:
+            result['DbId'] = self.db_id
+        if self.download_url is not None:
+            result['DownloadURL'] = self.download_url
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AuditDate') is not None:
+            self.audit_date = m.get('AuditDate')
+        if m.get('Config') is not None:
+            temp_model = GetDatabaseExportOrderDetailResponseBodyDatabaseExportOrderDetailKeyInfoConfig()
+            self.config = temp_model.from_map(m['Config'])
+        if m.get('DbId') is not None:
+            self.db_id = m.get('DbId')
+        if m.get('DownloadURL') is not None:
+            self.download_url = m.get('DownloadURL')
+        return self
+
+
+class GetDatabaseExportOrderDetailResponseBodyDatabaseExportOrderDetail(TeaModel):
+    def __init__(
+        self,
+        comment: str = None,
+        committer: str = None,
+        committer_id: str = None,
+        id: int = None,
+        key_info: GetDatabaseExportOrderDetailResponseBodyDatabaseExportOrderDetailKeyInfo = None,
+        log: str = None,
+        search_name: str = None,
+        status_desc: str = None,
+        workflow_status_desc: str = None,
+    ):
+        self.comment = comment
+        self.committer = committer
+        self.committer_id = committer_id
+        self.id = id
+        self.key_info = key_info
+        self.log = log
+        self.search_name = search_name
+        self.status_desc = status_desc
+        self.workflow_status_desc = workflow_status_desc
+
+    def validate(self):
+        if self.key_info:
+            self.key_info.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.comment is not None:
+            result['Comment'] = self.comment
+        if self.committer is not None:
+            result['Committer'] = self.committer
+        if self.committer_id is not None:
+            result['CommitterId'] = self.committer_id
+        if self.id is not None:
+            result['Id'] = self.id
+        if self.key_info is not None:
+            result['KeyInfo'] = self.key_info.to_map()
+        if self.log is not None:
+            result['Log'] = self.log
+        if self.search_name is not None:
+            result['SearchName'] = self.search_name
+        if self.status_desc is not None:
+            result['StatusDesc'] = self.status_desc
+        if self.workflow_status_desc is not None:
+            result['WorkflowStatusDesc'] = self.workflow_status_desc
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Comment') is not None:
+            self.comment = m.get('Comment')
+        if m.get('Committer') is not None:
+            self.committer = m.get('Committer')
+        if m.get('CommitterId') is not None:
+            self.committer_id = m.get('CommitterId')
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        if m.get('KeyInfo') is not None:
+            temp_model = GetDatabaseExportOrderDetailResponseBodyDatabaseExportOrderDetailKeyInfo()
+            self.key_info = temp_model.from_map(m['KeyInfo'])
+        if m.get('Log') is not None:
+            self.log = m.get('Log')
+        if m.get('SearchName') is not None:
+            self.search_name = m.get('SearchName')
+        if m.get('StatusDesc') is not None:
+            self.status_desc = m.get('StatusDesc')
+        if m.get('WorkflowStatusDesc') is not None:
+            self.workflow_status_desc = m.get('WorkflowStatusDesc')
+        return self
+
+
+class GetDatabaseExportOrderDetailResponseBody(TeaModel):
+    def __init__(
+        self,
+        database_export_order_detail: GetDatabaseExportOrderDetailResponseBodyDatabaseExportOrderDetail = None,
+        error_code: str = None,
+        error_message: str = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.database_export_order_detail = database_export_order_detail
+        self.error_code = error_code
+        self.error_message = error_message
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        if self.database_export_order_detail:
+            self.database_export_order_detail.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.database_export_order_detail is not None:
+            result['DatabaseExportOrderDetail'] = self.database_export_order_detail.to_map()
+        if self.error_code is not None:
+            result['ErrorCode'] = self.error_code
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DatabaseExportOrderDetail') is not None:
+            temp_model = GetDatabaseExportOrderDetailResponseBodyDatabaseExportOrderDetail()
+            self.database_export_order_detail = temp_model.from_map(m['DatabaseExportOrderDetail'])
+        if m.get('ErrorCode') is not None:
+            self.error_code = m.get('ErrorCode')
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class GetDatabaseExportOrderDetailResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetDatabaseExportOrderDetailResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetDatabaseExportOrderDetailResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetInstanceRequest(TeaModel):
     def __init__(
         self,
         host: str = None,
         port: int = None,
         sid: str = None,
         tid: int = None,
@@ -21133,18 +23431,16 @@
         self,
         table_guid: str = None,
         tid: int = None,
     ):
         # The GUID of the table in Data Management (DMS).
         # 
         # > 
-        # 
-        # *   You can call the [ListLogicTables](~~141875~~) operation with ReturnGuid set to true to query the GUIDs of logical tables in a specific logical database.
-        # 
-        # *   You can call the [ListTables](~~141878~~) operation with ReturnGuid set to true to query the GUIDs of tables in a specific physical database.
+        # > - You can call the [ListLogicTables](~~141875~~) operation with ReturnGuid set to true to query the GUIDs of logical tables in a specific logical database.
+        # > - You can call the [ListTables](~~141878~~) operation with ReturnGuid set to true to query the GUIDs of tables in a specific physical database.
         self.table_guid = table_guid
         # The ID of the tenant.
         # 
         # > To view the ID of the tenant, move the pointer over the profile picture in the upper-right corner of the DMS console. For more information, see the "View information about the current tenant" section of the [Tenant information](~~181330~~) topic.
         self.tid = tid
 
     def validate(self):
@@ -21216,15 +23512,15 @@
         self.region_id = region_id
         # The number of tables.
         self.table_count = table_count
         # The expression of the names of logical tables.
         # 
         # **\
         # 
-        # **Description**This parameter is not returned for physical tables.
+        # **Description** This parameter is not returned for physical tables.
         self.table_name_expr = table_name_expr
         # The names of tables.
         # 
         # > The table names are separated by commas (,).
         self.table_name_list = table_name_list
 
     def validate(self):
@@ -25452,14 +27748,15 @@
 
 
 class ListDDLPublishRecordsResponseBodyDDLPublishRecordList(TeaModel):
     def __init__(
         self,
         audit_expire_time: str = None,
         audit_status: str = None,
+        comment: str = None,
         creator_id: int = None,
         finality: bool = None,
         finality_reason: str = None,
         publish_status: str = None,
         publish_task_info_list: List[ListDDLPublishRecordsResponseBodyDDLPublishRecordListPublishTaskInfoList] = None,
         risk_level: str = None,
         status_desc: str = None,
@@ -25471,14 +27768,15 @@
         # 
         # *   **EXEMPT_PASS**: The ticket passes without approval.
         # *   **TO_AUDIT**: The ticket is pending for approval.
         # *   **CANCEL**: The ticket is canceled.
         # *   **SUCCESS**: The ticket is approved.
         # *   **FAIL**: The ticket fails to pass the approval.
         self.audit_status = audit_status
+        self.comment = comment
         # The ID of the user who creates the ticket. You can obtain the user ID by calling the [GetUser](~~147098~~) operation and querying the value of the UserId parameter. The value is not the unique ID (UID) of the Alibaba Cloud account.
         self.creator_id = creator_id
         # Indicates whether the approval is terminated. Valid values:
         # 
         # *   **true**: The approval is terminated.
         # *   **false**: The approval is not terminated.
         # 
@@ -25520,14 +27818,16 @@
             return _map
 
         result = dict()
         if self.audit_expire_time is not None:
             result['AuditExpireTime'] = self.audit_expire_time
         if self.audit_status is not None:
             result['AuditStatus'] = self.audit_status
+        if self.comment is not None:
+            result['Comment'] = self.comment
         if self.creator_id is not None:
             result['CreatorId'] = self.creator_id
         if self.finality is not None:
             result['Finality'] = self.finality
         if self.finality_reason is not None:
             result['FinalityReason'] = self.finality_reason
         if self.publish_status is not None:
@@ -25546,14 +27846,16 @@
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AuditExpireTime') is not None:
             self.audit_expire_time = m.get('AuditExpireTime')
         if m.get('AuditStatus') is not None:
             self.audit_status = m.get('AuditStatus')
+        if m.get('Comment') is not None:
+            self.comment = m.get('Comment')
         if m.get('CreatorId') is not None:
             self.creator_id = m.get('CreatorId')
         if m.get('Finality') is not None:
             self.finality = m.get('Finality')
         if m.get('FinalityReason') is not None:
             self.finality_reason = m.get('FinalityReason')
         if m.get('PublishStatus') is not None:
@@ -40077,14 +42379,195 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = PublishAndDeployTaskFlowResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class QueryDataTrackResultDownloadStatusRequest(TeaModel):
+    def __init__(
+        self,
+        download_key_id: str = None,
+        order_id: int = None,
+        tid: int = None,
+    ):
+        self.download_key_id = download_key_id
+        self.order_id = order_id
+        self.tid = tid
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.download_key_id is not None:
+            result['DownloadKeyId'] = self.download_key_id
+        if self.order_id is not None:
+            result['OrderId'] = self.order_id
+        if self.tid is not None:
+            result['Tid'] = self.tid
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DownloadKeyId') is not None:
+            self.download_key_id = m.get('DownloadKeyId')
+        if m.get('OrderId') is not None:
+            self.order_id = m.get('OrderId')
+        if m.get('Tid') is not None:
+            self.tid = m.get('Tid')
+        return self
+
+
+class QueryDataTrackResultDownloadStatusResponseBodyStatusResult(TeaModel):
+    def __init__(
+        self,
+        download_status: str = None,
+        download_url: str = None,
+        status_desc: str = None,
+        total_count: int = None,
+    ):
+        self.download_status = download_status
+        self.download_url = download_url
+        self.status_desc = status_desc
+        self.total_count = total_count
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.download_status is not None:
+            result['DownloadStatus'] = self.download_status
+        if self.download_url is not None:
+            result['DownloadUrl'] = self.download_url
+        if self.status_desc is not None:
+            result['StatusDesc'] = self.status_desc
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DownloadStatus') is not None:
+            self.download_status = m.get('DownloadStatus')
+        if m.get('DownloadUrl') is not None:
+            self.download_url = m.get('DownloadUrl')
+        if m.get('StatusDesc') is not None:
+            self.status_desc = m.get('StatusDesc')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class QueryDataTrackResultDownloadStatusResponseBody(TeaModel):
+    def __init__(
+        self,
+        error_code: str = None,
+        error_message: str = None,
+        request_id: str = None,
+        status_result: QueryDataTrackResultDownloadStatusResponseBodyStatusResult = None,
+        success: bool = None,
+    ):
+        self.error_code = error_code
+        self.error_message = error_message
+        self.request_id = request_id
+        self.status_result = status_result
+        self.success = success
+
+    def validate(self):
+        if self.status_result:
+            self.status_result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.error_code is not None:
+            result['ErrorCode'] = self.error_code
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.status_result is not None:
+            result['StatusResult'] = self.status_result.to_map()
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ErrorCode') is not None:
+            self.error_code = m.get('ErrorCode')
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('StatusResult') is not None:
+            temp_model = QueryDataTrackResultDownloadStatusResponseBodyStatusResult()
+            self.status_result = temp_model.from_map(m['StatusResult'])
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class QueryDataTrackResultDownloadStatusResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: QueryDataTrackResultDownloadStatusResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = QueryDataTrackResultDownloadStatusResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ReDeployLhDagVersionRequest(TeaModel):
     def __init__(
         self,
         dag_id: int = None,
         dag_version: int = None,
         tid: int = None,
     ):
@@ -41777,14 +44260,513 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = RevokeUserPermissionResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class SearchDataTrackResultRequestColumnFilter(TeaModel):
+    def __init__(
+        self,
+        between_end: str = None,
+        between_start: str = None,
+        column_name: str = None,
+        in_list: List[str] = None,
+        operator: str = None,
+        value: str = None,
+    ):
+        self.between_end = between_end
+        self.between_start = between_start
+        self.column_name = column_name
+        self.in_list = in_list
+        self.operator = operator
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.between_end is not None:
+            result['BetweenEnd'] = self.between_end
+        if self.between_start is not None:
+            result['BetweenStart'] = self.between_start
+        if self.column_name is not None:
+            result['ColumnName'] = self.column_name
+        if self.in_list is not None:
+            result['InList'] = self.in_list
+        if self.operator is not None:
+            result['Operator'] = self.operator
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('BetweenEnd') is not None:
+            self.between_end = m.get('BetweenEnd')
+        if m.get('BetweenStart') is not None:
+            self.between_start = m.get('BetweenStart')
+        if m.get('ColumnName') is not None:
+            self.column_name = m.get('ColumnName')
+        if m.get('InList') is not None:
+            self.in_list = m.get('InList')
+        if m.get('Operator') is not None:
+            self.operator = m.get('Operator')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class SearchDataTrackResultRequest(TeaModel):
+    def __init__(
+        self,
+        column_filter: SearchDataTrackResultRequestColumnFilter = None,
+        filter_end_time: str = None,
+        filter_start_time: str = None,
+        filter_table_list: List[str] = None,
+        filter_type_list: List[str] = None,
+        order_id: int = None,
+        tid: int = None,
+    ):
+        self.column_filter = column_filter
+        self.filter_end_time = filter_end_time
+        self.filter_start_time = filter_start_time
+        self.filter_table_list = filter_table_list
+        self.filter_type_list = filter_type_list
+        self.order_id = order_id
+        self.tid = tid
+
+    def validate(self):
+        if self.column_filter:
+            self.column_filter.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.column_filter is not None:
+            result['ColumnFilter'] = self.column_filter.to_map()
+        if self.filter_end_time is not None:
+            result['FilterEndTime'] = self.filter_end_time
+        if self.filter_start_time is not None:
+            result['FilterStartTime'] = self.filter_start_time
+        if self.filter_table_list is not None:
+            result['FilterTableList'] = self.filter_table_list
+        if self.filter_type_list is not None:
+            result['FilterTypeList'] = self.filter_type_list
+        if self.order_id is not None:
+            result['OrderId'] = self.order_id
+        if self.tid is not None:
+            result['Tid'] = self.tid
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ColumnFilter') is not None:
+            temp_model = SearchDataTrackResultRequestColumnFilter()
+            self.column_filter = temp_model.from_map(m['ColumnFilter'])
+        if m.get('FilterEndTime') is not None:
+            self.filter_end_time = m.get('FilterEndTime')
+        if m.get('FilterStartTime') is not None:
+            self.filter_start_time = m.get('FilterStartTime')
+        if m.get('FilterTableList') is not None:
+            self.filter_table_list = m.get('FilterTableList')
+        if m.get('FilterTypeList') is not None:
+            self.filter_type_list = m.get('FilterTypeList')
+        if m.get('OrderId') is not None:
+            self.order_id = m.get('OrderId')
+        if m.get('Tid') is not None:
+            self.tid = m.get('Tid')
+        return self
+
+
+class SearchDataTrackResultShrinkRequest(TeaModel):
+    def __init__(
+        self,
+        column_filter_shrink: str = None,
+        filter_end_time: str = None,
+        filter_start_time: str = None,
+        filter_table_list_shrink: str = None,
+        filter_type_list_shrink: str = None,
+        order_id: int = None,
+        tid: int = None,
+    ):
+        self.column_filter_shrink = column_filter_shrink
+        self.filter_end_time = filter_end_time
+        self.filter_start_time = filter_start_time
+        self.filter_table_list_shrink = filter_table_list_shrink
+        self.filter_type_list_shrink = filter_type_list_shrink
+        self.order_id = order_id
+        self.tid = tid
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.column_filter_shrink is not None:
+            result['ColumnFilter'] = self.column_filter_shrink
+        if self.filter_end_time is not None:
+            result['FilterEndTime'] = self.filter_end_time
+        if self.filter_start_time is not None:
+            result['FilterStartTime'] = self.filter_start_time
+        if self.filter_table_list_shrink is not None:
+            result['FilterTableList'] = self.filter_table_list_shrink
+        if self.filter_type_list_shrink is not None:
+            result['FilterTypeList'] = self.filter_type_list_shrink
+        if self.order_id is not None:
+            result['OrderId'] = self.order_id
+        if self.tid is not None:
+            result['Tid'] = self.tid
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ColumnFilter') is not None:
+            self.column_filter_shrink = m.get('ColumnFilter')
+        if m.get('FilterEndTime') is not None:
+            self.filter_end_time = m.get('FilterEndTime')
+        if m.get('FilterStartTime') is not None:
+            self.filter_start_time = m.get('FilterStartTime')
+        if m.get('FilterTableList') is not None:
+            self.filter_table_list_shrink = m.get('FilterTableList')
+        if m.get('FilterTypeList') is not None:
+            self.filter_type_list_shrink = m.get('FilterTypeList')
+        if m.get('OrderId') is not None:
+            self.order_id = m.get('OrderId')
+        if m.get('Tid') is not None:
+            self.tid = m.get('Tid')
+        return self
+
+
+class SearchDataTrackResultResponseBodyTrackResultEventList(TeaModel):
+    def __init__(
+        self,
+        data_after: List[str] = None,
+        data_before: List[str] = None,
+        event_id: int = None,
+        event_length: int = None,
+        event_timestamp: str = None,
+        event_type: str = None,
+        roll_sql: str = None,
+    ):
+        self.data_after = data_after
+        self.data_before = data_before
+        self.event_id = event_id
+        self.event_length = event_length
+        self.event_timestamp = event_timestamp
+        self.event_type = event_type
+        self.roll_sql = roll_sql
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.data_after is not None:
+            result['DataAfter'] = self.data_after
+        if self.data_before is not None:
+            result['DataBefore'] = self.data_before
+        if self.event_id is not None:
+            result['EventId'] = self.event_id
+        if self.event_length is not None:
+            result['EventLength'] = self.event_length
+        if self.event_timestamp is not None:
+            result['EventTimestamp'] = self.event_timestamp
+        if self.event_type is not None:
+            result['EventType'] = self.event_type
+        if self.roll_sql is not None:
+            result['RollSQL'] = self.roll_sql
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DataAfter') is not None:
+            self.data_after = m.get('DataAfter')
+        if m.get('DataBefore') is not None:
+            self.data_before = m.get('DataBefore')
+        if m.get('EventId') is not None:
+            self.event_id = m.get('EventId')
+        if m.get('EventLength') is not None:
+            self.event_length = m.get('EventLength')
+        if m.get('EventTimestamp') is not None:
+            self.event_timestamp = m.get('EventTimestamp')
+        if m.get('EventType') is not None:
+            self.event_type = m.get('EventType')
+        if m.get('RollSQL') is not None:
+            self.roll_sql = m.get('RollSQL')
+        return self
+
+
+class SearchDataTrackResultResponseBodyTrackResultTableInfoListColumns(TeaModel):
+    def __init__(
+        self,
+        column_name: str = None,
+        column_position: int = None,
+        column_type: str = None,
+        fictive: bool = None,
+    ):
+        self.column_name = column_name
+        self.column_position = column_position
+        self.column_type = column_type
+        self.fictive = fictive
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.column_name is not None:
+            result['ColumnName'] = self.column_name
+        if self.column_position is not None:
+            result['ColumnPosition'] = self.column_position
+        if self.column_type is not None:
+            result['ColumnType'] = self.column_type
+        if self.fictive is not None:
+            result['Fictive'] = self.fictive
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ColumnName') is not None:
+            self.column_name = m.get('ColumnName')
+        if m.get('ColumnPosition') is not None:
+            self.column_position = m.get('ColumnPosition')
+        if m.get('ColumnType') is not None:
+            self.column_type = m.get('ColumnType')
+        if m.get('Fictive') is not None:
+            self.fictive = m.get('Fictive')
+        return self
+
+
+class SearchDataTrackResultResponseBodyTrackResultTableInfoList(TeaModel):
+    def __init__(
+        self,
+        columns: List[SearchDataTrackResultResponseBodyTrackResultTableInfoListColumns] = None,
+        description: str = None,
+        schema_name: str = None,
+        table_name: str = None,
+    ):
+        self.columns = columns
+        self.description = description
+        self.schema_name = schema_name
+        self.table_name = table_name
+
+    def validate(self):
+        if self.columns:
+            for k in self.columns:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Columns'] = []
+        if self.columns is not None:
+            for k in self.columns:
+                result['Columns'].append(k.to_map() if k else None)
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.schema_name is not None:
+            result['SchemaName'] = self.schema_name
+        if self.table_name is not None:
+            result['TableName'] = self.table_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.columns = []
+        if m.get('Columns') is not None:
+            for k in m.get('Columns'):
+                temp_model = SearchDataTrackResultResponseBodyTrackResultTableInfoListColumns()
+                self.columns.append(temp_model.from_map(k))
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('SchemaName') is not None:
+            self.schema_name = m.get('SchemaName')
+        if m.get('TableName') is not None:
+            self.table_name = m.get('TableName')
+        return self
+
+
+class SearchDataTrackResultResponseBodyTrackResult(TeaModel):
+    def __init__(
+        self,
+        event_list: List[SearchDataTrackResultResponseBodyTrackResultEventList] = None,
+        table_info_list: List[SearchDataTrackResultResponseBodyTrackResultTableInfoList] = None,
+        total_count: int = None,
+    ):
+        self.event_list = event_list
+        self.table_info_list = table_info_list
+        self.total_count = total_count
+
+    def validate(self):
+        if self.event_list:
+            for k in self.event_list:
+                if k:
+                    k.validate()
+        if self.table_info_list:
+            for k in self.table_info_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['EventList'] = []
+        if self.event_list is not None:
+            for k in self.event_list:
+                result['EventList'].append(k.to_map() if k else None)
+        result['TableInfoList'] = []
+        if self.table_info_list is not None:
+            for k in self.table_info_list:
+                result['TableInfoList'].append(k.to_map() if k else None)
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.event_list = []
+        if m.get('EventList') is not None:
+            for k in m.get('EventList'):
+                temp_model = SearchDataTrackResultResponseBodyTrackResultEventList()
+                self.event_list.append(temp_model.from_map(k))
+        self.table_info_list = []
+        if m.get('TableInfoList') is not None:
+            for k in m.get('TableInfoList'):
+                temp_model = SearchDataTrackResultResponseBodyTrackResultTableInfoList()
+                self.table_info_list.append(temp_model.from_map(k))
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class SearchDataTrackResultResponseBody(TeaModel):
+    def __init__(
+        self,
+        error_code: str = None,
+        error_message: str = None,
+        request_id: str = None,
+        success: bool = None,
+        track_result: SearchDataTrackResultResponseBodyTrackResult = None,
+    ):
+        self.error_code = error_code
+        self.error_message = error_message
+        self.request_id = request_id
+        self.success = success
+        self.track_result = track_result
+
+    def validate(self):
+        if self.track_result:
+            self.track_result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.error_code is not None:
+            result['ErrorCode'] = self.error_code
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        if self.track_result is not None:
+            result['TrackResult'] = self.track_result.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ErrorCode') is not None:
+            self.error_code = m.get('ErrorCode')
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        if m.get('TrackResult') is not None:
+            temp_model = SearchDataTrackResultResponseBodyTrackResult()
+            self.track_result = temp_model.from_map(m['TrackResult'])
+        return self
+
+
+class SearchDataTrackResultResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SearchDataTrackResultResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SearchDataTrackResultResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class SearchDatabaseRequest(TeaModel):
     def __init__(
         self,
         db_type: str = None,
         env_type: str = None,
         page_number: int = None,
         page_size: int = None,
```

### Comparing `alibabacloud_dms-enterprise20181101-1.45.0/alibabacloud_dms_enterprise20181101.egg-info/PKG-INFO` & `alibabacloud_dms-enterprise20181101-1.46.0/alibabacloud_dms_enterprise20181101.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dms-enterprise20181101
-Version: 1.45.0
+Version: 1.46.0
 Summary: Alibaba Cloud dms-enterprise (20181101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dms-enterprise20181101-1.45.0/setup.py` & `alibabacloud_dms-enterprise20181101-1.46.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dms-enterprise20181101.
 
-Created on 11/04/2023
+Created on 24/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dms_enterprise20181101"
 NAME = "alibabacloud_dms-enterprise20181101" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud dms-enterprise (20181101) SDK Library for Python"
```

