# Comparing `tmp/nista_library-3.0.6.tar.gz` & `tmp/nista_library-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nista_library-3.0.6.tar", max compression
+gzip compressed data, was "nista_library-4.0.0.tar", max compression
```

## Comparing `nista_library-3.0.6.tar` & `nista_library-4.0.0.tar`

### file list

```diff
@@ -1,85 +1,103 @@
--rw-r--r--   0        0        0     1117 2022-12-15 16:18:06.900340 nista_library-3.0.6/LICENSE.md
--rw-r--r--   0        0        0     4521 2022-12-15 16:18:06.900340 nista_library-3.0.6/README.md
--rw-r--r--   0        0        0      153 2022-12-15 16:18:06.900340 nista_library-3.0.6/data_point_client/__init__.py
--rw-r--r--   0        0        0       47 2022-12-15 16:18:06.900340 nista_library-3.0.6/data_point_client/api/__init__.py
--rw-r--r--   0        0        0        0 2022-12-15 16:18:06.900340 nista_library-3.0.6/data_point_client/api/data_export/__init__.py
--rw-r--r--   0        0        0     4167 2022-12-15 16:18:06.900340 nista_library-3.0.6/data_point_client/api/data_export/data_export_create_csv_export.py
--rw-r--r--   0        0        0        0 2022-12-15 16:18:06.900340 nista_library-3.0.6/data_point_client/api/data_point/__init__.py
--rw-r--r--   0        0        0     4319 2022-12-15 16:18:06.900340 nista_library-3.0.6/data_point_client/api/data_point/data_point_append_execution_result_data.py
--rw-r--r--   0        0        0     4213 2022-12-15 16:18:06.900340 nista_library-3.0.6/data_point_client/api/data_point/data_point_append_time_series_data.py
--rw-r--r--   0        0        0     4160 2022-12-15 16:18:06.900340 nista_library-3.0.6/data_point_client/api/data_point/data_point_create_chiller_samples.py
--rw-r--r--   0        0        0     4278 2022-12-15 16:18:06.900340 nista_library-3.0.6/data_point_client/api/data_point/data_point_create_data_point.py
--rw-r--r--   0        0        0     3310 2022-12-15 16:18:06.900340 nista_library-3.0.6/data_point_client/api/data_point/data_point_delete_data_point.py
--rw-r--r--   0        0        0     3315 2022-12-15 16:18:06.900340 nista_library-3.0.6/data_point_client/api/data_point/data_point_delete_data_point_cleanup_rule.py
--rw-r--r--   0        0        0     4309 2022-12-15 16:18:06.901340 nista_library-3.0.6/data_point_client/api/data_point/data_point_get_data.py
--rw-r--r--   0        0        0     3830 2022-12-15 16:18:06.901340 nista_library-3.0.6/data_point_client/api/data_point/data_point_get_data_point.py
--rw-r--r--   0        0        0     4151 2022-12-15 16:18:06.901340 nista_library-3.0.6/data_point_client/api/data_point/data_point_get_data_point_by_version.py
--rw-r--r--   0        0        0     7753 2022-12-15 16:18:06.901340 nista_library-3.0.6/data_point_client/api/data_point/data_point_get_data_points.py
--rw-r--r--   0        0        0     6536 2022-12-15 16:18:06.901340 nista_library-3.0.6/data_point_client/api/data_point/data_point_get_tags.py
--rw-r--r--   0        0        0     3642 2022-12-15 16:18:06.901340 nista_library-3.0.6/data_point_client/api/data_point/data_point_get_tags_2.py
--rw-r--r--   0        0        0     4234 2022-12-15 16:18:06.901340 nista_library-3.0.6/data_point_client/api/data_point/data_point_update_constant_data.py
--rw-r--r--   0        0        0     4279 2022-12-15 16:18:06.901340 nista_library-3.0.6/data_point_client/api/data_point/data_point_update_data_point.py
--rw-r--r--   0        0        0     4355 2022-12-15 16:18:06.901340 nista_library-3.0.6/data_point_client/api/data_point/data_point_update_data_point_cleanup_rule.py
--rw-r--r--   0        0        0     4099 2022-12-15 16:18:06.901340 nista_library-3.0.6/data_point_client/api/data_point/data_point_update_data_point_unit.py
--rw-r--r--   0        0        0     4206 2022-12-15 16:18:06.901340 nista_library-3.0.6/data_point_client/api/data_point/data_point_update_day_period_data.py
--rw-r--r--   0        0        0     4218 2022-12-15 16:18:06.901340 nista_library-3.0.6/data_point_client/api/data_point/data_point_update_time_series_data.py
--rw-r--r--   0        0        0     4218 2022-12-15 16:18:06.901340 nista_library-3.0.6/data_point_client/api/data_point/data_point_update_week_period_data.py
--rw-r--r--   0        0        0     1821 2022-12-15 16:18:06.901340 nista_library-3.0.6/data_point_client/client.py
--rw-r--r--   0        0        0     3873 2022-12-15 16:18:06.901340 nista_library-3.0.6/data_point_client/models/__init__.py
--rw-r--r--   0        0        0     1965 2022-12-15 16:18:06.901340 nista_library-3.0.6/data_point_client/models/append_execution_result_data_request.py
--rw-r--r--   0        0        0     1618 2022-12-15 16:18:06.901340 nista_library-3.0.6/data_point_client/models/append_time_series_request.py
--rw-r--r--   0        0        0     1858 2022-12-15 16:18:06.901340 nista_library-3.0.6/data_point_client/models/calculation_origin.py
--rw-r--r--   0        0        0     7547 2022-12-15 16:18:06.901340 nista_library-3.0.6/data_point_client/models/constant_data_bucket.py
--rw-r--r--   0        0        0     2965 2022-12-15 16:18:06.901340 nista_library-3.0.6/data_point_client/models/constant_data_point_data.py
--rw-r--r--   0        0        0     5874 2022-12-15 16:18:06.901340 nista_library-3.0.6/data_point_client/models/data_bucket_base.py
--rw-r--r--   0        0        0     2054 2022-12-15 16:18:06.902340 nista_library-3.0.6/data_point_client/models/data_export_request.py
--rw-r--r--   0        0        0     2016 2022-12-15 16:18:06.902340 nista_library-3.0.6/data_point_client/models/data_point_data_base.py
--rw-r--r--   0        0        0     2418 2022-12-15 16:18:06.902340 nista_library-3.0.6/data_point_client/models/data_point_data_response.py
--rw-r--r--   0        0        0      779 2022-12-15 16:18:06.902340 nista_library-3.0.6/data_point_client/models/data_point_origin.py
--rw-r--r--   0        0        0     3212 2022-12-15 16:18:06.902340 nista_library-3.0.6/data_point_client/models/data_point_request.py
--rw-r--r--   0        0        0     7362 2022-12-15 16:18:06.902340 nista_library-3.0.6/data_point_client/models/data_point_response_base.py
--rw-r--r--   0        0        0     7281 2022-12-15 16:18:06.902340 nista_library-3.0.6/data_point_client/models/day_data_by_hour_transfer.py
--rw-r--r--   0        0        0     7564 2022-12-15 16:18:06.902340 nista_library-3.0.6/data_point_client/models/day_period_data_bucket.py
--rw-r--r--   0        0        0     4321 2022-12-15 16:18:06.902340 nista_library-3.0.6/data_point_client/models/day_period_data_point_data.py
--rw-r--r--   0        0        0      192 2022-12-15 16:18:06.902340 nista_library-3.0.6/data_point_client/models/en_data_bucket_state.py
--rw-r--r--   0        0        0      208 2022-12-15 16:18:06.902340 nista_library-3.0.6/data_point_client/models/en_data_point_existence_dto.py
--rw-r--r--   0        0        0      214 2022-12-15 16:18:06.902340 nista_library-3.0.6/data_point_client/models/en_data_point_state_dto.py
--rw-r--r--   0        0        0      192 2022-12-15 16:18:06.902340 nista_library-3.0.6/data_point_client/models/en_data_point_status.py
--rw-r--r--   0        0        0      250 2022-12-15 16:18:06.902340 nista_library-3.0.6/data_point_client/models/en_data_point_type.py
--rw-r--r--   0        0        0      181 2022-12-15 16:18:06.902340 nista_library-3.0.6/data_point_client/models/en_operator.py
--rw-r--r--   0        0        0     2375 2022-12-15 16:18:06.902340 nista_library-3.0.6/data_point_client/models/file_origin.py
--rw-r--r--   0        0        0     2579 2022-12-15 16:18:06.902340 nista_library-3.0.6/data_point_client/models/get_constant_response.py
--rw-r--r--   0        0        0     2831 2022-12-15 16:18:06.902340 nista_library-3.0.6/data_point_client/models/get_data_request.py
--rw-r--r--   0        0        0      779 2022-12-15 16:18:06.902340 nista_library-3.0.6/data_point_client/models/get_data_response.py
--rw-r--r--   0        0        0     3900 2022-12-15 16:18:06.902340 nista_library-3.0.6/data_point_client/models/get_day_period_response.py
--rw-r--r--   0        0        0     2529 2022-12-15 16:18:06.902340 nista_library-3.0.6/data_point_client/models/get_series_response.py
--rw-r--r--   0        0        0     3227 2022-12-15 16:18:06.902340 nista_library-3.0.6/data_point_client/models/get_week_period_response.py
--rw-r--r--   0        0        0     1176 2022-12-15 16:18:06.902340 nista_library-3.0.6/data_point_client/models/gnista_unit_response.py
--rw-r--r--   0        0        0     3377 2022-12-15 16:18:06.902340 nista_library-3.0.6/data_point_client/models/problem_details.py
--rw-r--r--   0        0        0     1216 2022-12-15 16:18:06.903340 nista_library-3.0.6/data_point_client/models/problem_details_extensions.py
--rw-r--r--   0        0        0     1449 2022-12-15 16:18:06.903340 nista_library-3.0.6/data_point_client/models/remote_origin.py
--rw-r--r--   0        0        0     1247 2022-12-15 16:18:06.903340 nista_library-3.0.6/data_point_client/models/rule.py
--rw-r--r--   0        0        0     8984 2022-12-15 16:18:06.903340 nista_library-3.0.6/data_point_client/models/series_data_bucket.py
--rw-r--r--   0        0        0     3058 2022-12-15 16:18:06.903340 nista_library-3.0.6/data_point_client/models/series_data_point_data.py
--rw-r--r--   0        0        0     1446 2022-12-15 16:18:06.903340 nista_library-3.0.6/data_point_client/models/sub_series_request.py
--rw-r--r--   0        0        0     1215 2022-12-15 16:18:06.903340 nista_library-3.0.6/data_point_client/models/sub_series_request_values.py
--rw-r--r--   0        0        0     1631 2022-12-15 16:18:06.903340 nista_library-3.0.6/data_point_client/models/time_series_period.py
--rw-r--r--   0        0        0     2675 2022-12-15 16:18:06.903340 nista_library-3.0.6/data_point_client/models/time_series_response.py
--rw-r--r--   0        0        0     1220 2022-12-15 16:18:06.903340 nista_library-3.0.6/data_point_client/models/time_series_response_curve.py
--rw-r--r--   0        0        0     1401 2022-12-15 16:18:06.903340 nista_library-3.0.6/data_point_client/models/update_constant_data_request.py
--rw-r--r--   0        0        0     2725 2022-12-15 16:18:06.903340 nista_library-3.0.6/data_point_client/models/update_day_period_request.py
--rw-r--r--   0        0        0     2769 2022-12-15 16:18:06.903340 nista_library-3.0.6/data_point_client/models/update_time_series_request.py
--rw-r--r--   0        0        0     2052 2022-12-15 16:18:06.903340 nista_library-3.0.6/data_point_client/models/update_week_period_request.py
--rw-r--r--   0        0        0     7478 2022-12-15 16:18:06.903340 nista_library-3.0.6/data_point_client/models/week_data_transfere.py
--rw-r--r--   0        0        0     7576 2022-12-15 16:18:06.903340 nista_library-3.0.6/data_point_client/models/week_period_data_bucket.py
--rw-r--r--   0        0        0     3648 2022-12-15 16:18:06.903340 nista_library-3.0.6/data_point_client/models/week_period_data_point_data.py
--rw-r--r--   0        0        0       25 2022-12-15 16:18:06.903340 nista_library-3.0.6/data_point_client/py.typed
--rw-r--r--   0        0        0      974 2022-12-15 16:18:06.903340 nista_library-3.0.6/data_point_client/types.py
--rw-r--r--   0        0        0      944 2022-12-15 16:18:06.904340 nista_library-3.0.6/nista_library/__init__.py
--rw-r--r--   0        0        0     8865 2022-12-15 16:18:06.904340 nista_library-3.0.6/nista_library/nista_connetion.py
--rw-r--r--   0        0        0      915 2022-12-15 16:18:06.904340 nista_library-3.0.6/nista_library/nista_credential_manager.py
--rw-r--r--   0        0        0    12477 2022-12-15 16:18:06.904340 nista_library-3.0.6/nista_library/nista_data_point.py
--rw-r--r--   0        0        0     1682 2022-12-15 16:18:06.904340 nista_library-3.0.6/nista_library/nista_data_points.py
--rw-r--r--   0        0        0     1308 2022-12-15 16:18:06.905340 nista_library-3.0.6/pyproject.toml
--rw-r--r--   0        0        0     5726 1970-01-01 00:00:00.000000 nista_library-3.0.6/setup.py
--rw-r--r--   0        0        0     5564 1970-01-01 00:00:00.000000 nista_library-3.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1117 2023-04-24 07:40:31.257645 nista_library-4.0.0/LICENSE.md
+-rw-r--r--   0        0        0     4521 2023-04-24 07:40:31.258645 nista_library-4.0.0/README.md
+-rw-r--r--   0        0        0      153 2023-04-24 07:40:31.258645 nista_library-4.0.0/data_point_client/__init__.py
+-rw-r--r--   0        0        0       47 2023-04-24 07:40:31.258645 nista_library-4.0.0/data_point_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 07:40:31.258645 nista_library-4.0.0/data_point_client/api/data_export/__init__.py
+-rw-r--r--   0        0        0     5330 2023-04-24 07:40:31.258645 nista_library-4.0.0/data_point_client/api/data_export/data_export_create_csv_export.py
+-rw-r--r--   0        0        0        0 2023-04-24 07:40:31.258645 nista_library-4.0.0/data_point_client/api/data_point/__init__.py
+-rw-r--r--   0        0        0     5482 2023-04-24 07:40:31.258645 nista_library-4.0.0/data_point_client/api/data_point/data_point_append_execution_result_data.py
+-rw-r--r--   0        0        0     5376 2023-04-24 07:40:31.258645 nista_library-4.0.0/data_point_client/api/data_point/data_point_append_time_series_data.py
+-rw-r--r--   0        0        0     5768 2023-04-24 07:40:31.258645 nista_library-4.0.0/data_point_client/api/data_point/data_point_create_area.py
+-rw-r--r--   0        0        0     6225 2023-04-24 07:40:31.258645 nista_library-4.0.0/data_point_client/api/data_point/data_point_create_area_message.py
+-rw-r--r--   0        0        0     5323 2023-04-24 07:40:31.258645 nista_library-4.0.0/data_point_client/api/data_point/data_point_create_chiller_samples.py
+-rw-r--r--   0        0        0     5441 2023-04-24 07:40:31.258645 nista_library-4.0.0/data_point_client/api/data_point/data_point_create_data_point.py
+-rw-r--r--   0        0        0     4789 2023-04-24 07:40:31.258645 nista_library-4.0.0/data_point_client/api/data_point/data_point_delete_area.py
+-rw-r--r--   0        0        0     4473 2023-04-24 07:40:31.258645 nista_library-4.0.0/data_point_client/api/data_point/data_point_delete_data_point.py
+-rw-r--r--   0        0        0     4478 2023-04-24 07:40:31.258645 nista_library-4.0.0/data_point_client/api/data_point/data_point_delete_data_point_cleanup_rule.py
+-rw-r--r--   0        0        0     5168 2023-04-24 07:40:31.258645 nista_library-4.0.0/data_point_client/api/data_point/data_point_delete_message.py
+-rw-r--r--   0        0        0     5472 2023-04-24 07:40:31.258645 nista_library-4.0.0/data_point_client/api/data_point/data_point_get_data.py
+-rw-r--r--   0        0        0     5005 2023-04-24 07:40:31.258645 nista_library-4.0.0/data_point_client/api/data_point/data_point_get_data_point.py
+-rw-r--r--   0        0        0     5326 2023-04-24 07:40:31.258645 nista_library-4.0.0/data_point_client/api/data_point/data_point_get_data_point_by_version.py
+-rw-r--r--   0        0        0     8928 2023-04-24 07:40:31.259645 nista_library-4.0.0/data_point_client/api/data_point/data_point_get_data_points.py
+-rw-r--r--   0        0        0     7699 2023-04-24 07:40:31.259645 nista_library-4.0.0/data_point_client/api/data_point/data_point_get_tags.py
+-rw-r--r--   0        0        0     4805 2023-04-24 07:40:31.259645 nista_library-4.0.0/data_point_client/api/data_point/data_point_get_tags_2.py
+-rw-r--r--   0        0        0     5296 2023-04-24 07:40:31.259645 nista_library-4.0.0/data_point_client/api/data_point/data_point_list_areas.py
+-rw-r--r--   0        0        0     5769 2023-04-24 07:40:31.259645 nista_library-4.0.0/data_point_client/api/data_point/data_point_update_area.py
+-rw-r--r--   0        0        0     5397 2023-04-24 07:40:31.259645 nista_library-4.0.0/data_point_client/api/data_point/data_point_update_constant_data.py
+-rw-r--r--   0        0        0     5442 2023-04-24 07:40:31.259645 nista_library-4.0.0/data_point_client/api/data_point/data_point_update_data_point.py
+-rw-r--r--   0        0        0     5518 2023-04-24 07:40:31.259645 nista_library-4.0.0/data_point_client/api/data_point/data_point_update_data_point_cleanup_rule.py
+-rw-r--r--   0        0        0     5262 2023-04-24 07:40:31.259645 nista_library-4.0.0/data_point_client/api/data_point/data_point_update_data_point_unit.py
+-rw-r--r--   0        0        0     5369 2023-04-24 07:40:31.259645 nista_library-4.0.0/data_point_client/api/data_point/data_point_update_day_period_data.py
+-rw-r--r--   0        0        0     6226 2023-04-24 07:40:31.259645 nista_library-4.0.0/data_point_client/api/data_point/data_point_update_message.py
+-rw-r--r--   0        0        0     5381 2023-04-24 07:40:31.259645 nista_library-4.0.0/data_point_client/api/data_point/data_point_update_time_series_data.py
+-rw-r--r--   0        0        0     5381 2023-04-24 07:40:31.259645 nista_library-4.0.0/data_point_client/api/data_point/data_point_update_week_period_data.py
+-rw-r--r--   0        0        0     2817 2023-04-24 07:40:31.259645 nista_library-4.0.0/data_point_client/client.py
+-rw-r--r--   0        0        0      470 2023-04-24 07:40:31.259645 nista_library-4.0.0/data_point_client/errors.py
+-rw-r--r--   0        0        0     4795 2023-04-24 07:40:31.259645 nista_library-4.0.0/data_point_client/models/__init__.py
+-rw-r--r--   0        0        0     1965 2023-04-24 07:40:31.259645 nista_library-4.0.0/data_point_client/models/append_execution_result_data_request.py
+-rw-r--r--   0        0        0     1618 2023-04-24 07:40:31.259645 nista_library-4.0.0/data_point_client/models/append_time_series_request.py
+-rw-r--r--   0        0        0     4359 2023-04-24 07:40:31.259645 nista_library-4.0.0/data_point_client/models/area_of_interest_response.py
+-rw-r--r--   0        0        0     1858 2023-04-24 07:40:31.259645 nista_library-4.0.0/data_point_client/models/calculation_origin.py
+-rw-r--r--   0        0        0     7547 2023-04-24 07:40:31.259645 nista_library-4.0.0/data_point_client/models/constant_data_bucket.py
+-rw-r--r--   0        0        0     2965 2023-04-24 07:40:31.260645 nista_library-4.0.0/data_point_client/models/constant_data_point_data.py
+-rw-r--r--   0        0        0     2597 2023-04-24 07:40:31.260645 nista_library-4.0.0/data_point_client/models/continuous_location_rest.py
+-rw-r--r--   0        0        0      923 2023-04-24 07:40:31.260645 nista_library-4.0.0/data_point_client/models/create_area_message_request.py
+-rw-r--r--   0        0        0     2319 2023-04-24 07:40:31.260645 nista_library-4.0.0/data_point_client/models/create_area_request.py
+-rw-r--r--   0        0        0     5874 2023-04-24 07:40:31.260645 nista_library-4.0.0/data_point_client/models/data_bucket_base.py
+-rw-r--r--   0        0        0     2054 2023-04-24 07:40:31.260645 nista_library-4.0.0/data_point_client/models/data_export_request.py
+-rw-r--r--   0        0        0     2702 2023-04-24 07:40:31.260645 nista_library-4.0.0/data_point_client/models/data_point_comment_message_response.py
+-rw-r--r--   0        0        0     2016 2023-04-24 07:40:31.260645 nista_library-4.0.0/data_point_client/models/data_point_data_base.py
+-rw-r--r--   0        0        0     2418 2023-04-24 07:40:31.260645 nista_library-4.0.0/data_point_client/models/data_point_data_response.py
+-rw-r--r--   0        0        0      779 2023-04-24 07:40:31.260645 nista_library-4.0.0/data_point_client/models/data_point_origin.py
+-rw-r--r--   0        0        0     3212 2023-04-24 07:40:31.260645 nista_library-4.0.0/data_point_client/models/data_point_request.py
+-rw-r--r--   0        0        0     7362 2023-04-24 07:40:31.260645 nista_library-4.0.0/data_point_client/models/data_point_response_base.py
+-rw-r--r--   0        0        0     7281 2023-04-24 07:40:31.260645 nista_library-4.0.0/data_point_client/models/day_data_by_hour_transfer.py
+-rw-r--r--   0        0        0     7564 2023-04-24 07:40:31.260645 nista_library-4.0.0/data_point_client/models/day_period_data_bucket.py
+-rw-r--r--   0        0        0     4321 2023-04-24 07:40:31.260645 nista_library-4.0.0/data_point_client/models/day_period_data_point_data.py
+-rw-r--r--   0        0        0      191 2023-04-24 07:40:31.260645 nista_library-4.0.0/data_point_client/models/en_area_type_rest.py
+-rw-r--r--   0        0        0      192 2023-04-24 07:40:31.260645 nista_library-4.0.0/data_point_client/models/en_data_bucket_state.py
+-rw-r--r--   0        0        0      208 2023-04-24 07:40:31.260645 nista_library-4.0.0/data_point_client/models/en_data_point_existence_dto.py
+-rw-r--r--   0        0        0      214 2023-04-24 07:40:31.260645 nista_library-4.0.0/data_point_client/models/en_data_point_state_dto.py
+-rw-r--r--   0        0        0      192 2023-04-24 07:40:31.260645 nista_library-4.0.0/data_point_client/models/en_data_point_status.py
+-rw-r--r--   0        0        0      250 2023-04-24 07:40:31.260645 nista_library-4.0.0/data_point_client/models/en_data_point_type.py
+-rw-r--r--   0        0        0      181 2023-04-24 07:40:31.260645 nista_library-4.0.0/data_point_client/models/en_operator.py
+-rw-r--r--   0        0        0     2375 2023-04-24 07:40:31.260645 nista_library-4.0.0/data_point_client/models/file_origin.py
+-rw-r--r--   0        0        0     2579 2023-04-24 07:40:31.260645 nista_library-4.0.0/data_point_client/models/get_constant_response.py
+-rw-r--r--   0        0        0     3472 2023-04-24 07:40:31.261645 nista_library-4.0.0/data_point_client/models/get_data_request.py
+-rw-r--r--   0        0        0      779 2023-04-24 07:40:31.261645 nista_library-4.0.0/data_point_client/models/get_data_response.py
+-rw-r--r--   0        0        0     3900 2023-04-24 07:40:31.261645 nista_library-4.0.0/data_point_client/models/get_day_period_response.py
+-rw-r--r--   0        0        0     2529 2023-04-24 07:40:31.261645 nista_library-4.0.0/data_point_client/models/get_series_response.py
+-rw-r--r--   0        0        0     3227 2023-04-24 07:40:31.261645 nista_library-4.0.0/data_point_client/models/get_week_period_response.py
+-rw-r--r--   0        0        0     1176 2023-04-24 07:40:31.261645 nista_library-4.0.0/data_point_client/models/gnista_unit_response.py
+-rw-r--r--   0        0        0     1810 2023-04-24 07:40:31.261645 nista_library-4.0.0/data_point_client/models/live_data_origin.py
+-rw-r--r--   0        0        0      765 2023-04-24 07:40:31.261645 nista_library-4.0.0/data_point_client/models/location_rest.py
+-rw-r--r--   0        0        0     2045 2023-04-24 07:40:31.261645 nista_library-4.0.0/data_point_client/models/point_location_rest.py
+-rw-r--r--   0        0        0     3377 2023-04-24 07:40:31.261645 nista_library-4.0.0/data_point_client/models/problem_details.py
+-rw-r--r--   0        0        0     1215 2023-04-24 07:40:31.261645 nista_library-4.0.0/data_point_client/models/problem_details_extensions.py
+-rw-r--r--   0        0        0     1449 2023-04-24 07:40:31.261645 nista_library-4.0.0/data_point_client/models/remote_origin.py
+-rw-r--r--   0        0        0     1247 2023-04-24 07:40:31.261645 nista_library-4.0.0/data_point_client/models/rule.py
+-rw-r--r--   0        0        0     9273 2023-04-24 07:40:31.261645 nista_library-4.0.0/data_point_client/models/series_data_bucket.py
+-rw-r--r--   0        0        0     3058 2023-04-24 07:40:31.261645 nista_library-4.0.0/data_point_client/models/series_data_point_data.py
+-rw-r--r--   0        0        0     1446 2023-04-24 07:40:31.261645 nista_library-4.0.0/data_point_client/models/sub_series_request.py
+-rw-r--r--   0        0        0     1214 2023-04-24 07:40:31.261645 nista_library-4.0.0/data_point_client/models/sub_series_request_values.py
+-rw-r--r--   0        0        0     1631 2023-04-24 07:40:31.261645 nista_library-4.0.0/data_point_client/models/time_series_period.py
+-rw-r--r--   0        0        0     2675 2023-04-24 07:40:31.261645 nista_library-4.0.0/data_point_client/models/time_series_response.py
+-rw-r--r--   0        0        0     1219 2023-04-24 07:40:31.261645 nista_library-4.0.0/data_point_client/models/time_series_response_curve.py
+-rw-r--r--   0        0        0      923 2023-04-24 07:40:31.261645 nista_library-4.0.0/data_point_client/models/update_area_message_request.py
+-rw-r--r--   0        0        0     2674 2023-04-24 07:40:31.261645 nista_library-4.0.0/data_point_client/models/update_area_request.py
+-rw-r--r--   0        0        0     1401 2023-04-24 07:40:31.261645 nista_library-4.0.0/data_point_client/models/update_constant_data_request.py
+-rw-r--r--   0        0        0     2725 2023-04-24 07:40:31.261645 nista_library-4.0.0/data_point_client/models/update_day_period_request.py
+-rw-r--r--   0        0        0     3346 2023-04-24 07:40:31.261645 nista_library-4.0.0/data_point_client/models/update_time_series_request.py
+-rw-r--r--   0        0        0     2052 2023-04-24 07:40:31.262645 nista_library-4.0.0/data_point_client/models/update_week_period_request.py
+-rw-r--r--   0        0        0     7478 2023-04-24 07:40:31.262645 nista_library-4.0.0/data_point_client/models/week_data_transfere.py
+-rw-r--r--   0        0        0     7576 2023-04-24 07:40:31.262645 nista_library-4.0.0/data_point_client/models/week_period_data_bucket.py
+-rw-r--r--   0        0        0     3648 2023-04-24 07:40:31.262645 nista_library-4.0.0/data_point_client/models/week_period_data_point_data.py
+-rw-r--r--   0        0        0       25 2023-04-24 07:40:31.262645 nista_library-4.0.0/data_point_client/py.typed
+-rw-r--r--   0        0        0      974 2023-04-24 07:40:31.262645 nista_library-4.0.0/data_point_client/types.py
+-rw-r--r--   0        0        0      944 2023-04-24 07:40:31.262645 nista_library-4.0.0/nista_library/__init__.py
+-rw-r--r--   0        0        0     8866 2023-04-24 07:40:31.262645 nista_library-4.0.0/nista_library/nista_connetion.py
+-rw-r--r--   0        0        0      915 2023-04-24 07:40:31.263645 nista_library-4.0.0/nista_library/nista_credential_manager.py
+-rw-r--r--   0        0        0    12775 2023-04-24 07:40:31.263645 nista_library-4.0.0/nista_library/nista_data_point.py
+-rw-r--r--   0        0        0     1683 2023-04-24 07:40:31.263645 nista_library-4.0.0/nista_library/nista_data_points.py
+-rw-r--r--   0        0        0     1308 2023-04-24 07:40:31.264645 nista_library-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5514 1970-01-01 00:00:00.000000 nista_library-4.0.0/PKG-INFO
```

### Comparing `nista_library-3.0.6/LICENSE.md` & `nista_library-4.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nista_library-3.0.6/README.md` & `nista_library-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `nista_library-3.0.6/data_point_client/api/data_point/data_point_append_execution_result_data.py` & `nista_library-4.0.0/data_point_client/api/data_point/data_point_delete_area.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,173 +1,187 @@
 from http import HTTPStatus
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional
 
 import httpx
 
+from ... import errors
 from ...client import Client
-from ...models.append_execution_result_data_request import AppendExecutionResultDataRequest
 from ...models.problem_details import ProblemDetails
 from ...types import Response
 
 
 def _get_kwargs(
     workspace_id: str,
     data_point_id: str,
+    area_id: str,
     *,
     client: Client,
-    json_body: AppendExecutionResultDataRequest,
 ) -> Dict[str, Any]:
-    url = "{}/DataPoint/workspace/{workspaceId}/dataPoint/{dataPointId}/resultparts".format(
-        client.base_url, workspaceId=workspace_id, dataPointId=data_point_id
+    url = "{}/DataPoint/workspace/{workspaceId}/dataPoint/{dataPointId}/area/{areaId}".format(
+        client.base_url, workspaceId=workspace_id, dataPointId=data_point_id, areaId=area_id
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
-    json_json_body = json_body.to_dict()
-
     return {
-        "method": "post",
+        "method": "delete",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "json": json_json_body,
+        "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, ProblemDetails]]:
-    if response.status_code == HTTPStatus.ACCEPTED:
-        response_202 = cast(Any, None)
-        return response_202
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ProblemDetails]:
     if response.status_code == HTTPStatus.UNAUTHORIZED:
         response_401 = ProblemDetails.from_dict(response.json())
 
         return response_401
     if response.status_code == HTTPStatus.FORBIDDEN:
         response_403 = ProblemDetails.from_dict(response.json())
 
         return response_403
-    return None
+    if client.raise_on_unexpected_status:
+        raise errors.UnexpectedStatus(response.status_code, response.content)
+    else:
+        return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, ProblemDetails]]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ProblemDetails]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
-        parsed=_parse_response(response=response),
+        parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     workspace_id: str,
     data_point_id: str,
+    area_id: str,
     *,
     client: Client,
-    json_body: AppendExecutionResultDataRequest,
-) -> Response[Union[Any, ProblemDetails]]:
+) -> Response[ProblemDetails]:
     """
     Args:
         workspace_id (str):
         data_point_id (str):
-        json_body (AppendExecutionResultDataRequest):
+        area_id (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, ProblemDetails]]
+        Response[ProblemDetails]
     """
 
     kwargs = _get_kwargs(
         workspace_id=workspace_id,
         data_point_id=data_point_id,
+        area_id=area_id,
         client=client,
-        json_body=json_body,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     workspace_id: str,
     data_point_id: str,
+    area_id: str,
     *,
     client: Client,
-    json_body: AppendExecutionResultDataRequest,
-) -> Optional[Union[Any, ProblemDetails]]:
+) -> Optional[ProblemDetails]:
     """
     Args:
         workspace_id (str):
         data_point_id (str):
-        json_body (AppendExecutionResultDataRequest):
+        area_id (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, ProblemDetails]]
+        ProblemDetails
     """
 
     return sync_detailed(
         workspace_id=workspace_id,
         data_point_id=data_point_id,
+        area_id=area_id,
         client=client,
-        json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
     workspace_id: str,
     data_point_id: str,
+    area_id: str,
     *,
     client: Client,
-    json_body: AppendExecutionResultDataRequest,
-) -> Response[Union[Any, ProblemDetails]]:
+) -> Response[ProblemDetails]:
     """
     Args:
         workspace_id (str):
         data_point_id (str):
-        json_body (AppendExecutionResultDataRequest):
+        area_id (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, ProblemDetails]]
+        Response[ProblemDetails]
     """
 
     kwargs = _get_kwargs(
         workspace_id=workspace_id,
         data_point_id=data_point_id,
+        area_id=area_id,
         client=client,
-        json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
-    return _build_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     workspace_id: str,
     data_point_id: str,
+    area_id: str,
     *,
     client: Client,
-    json_body: AppendExecutionResultDataRequest,
-) -> Optional[Union[Any, ProblemDetails]]:
+) -> Optional[ProblemDetails]:
     """
     Args:
         workspace_id (str):
         data_point_id (str):
-        json_body (AppendExecutionResultDataRequest):
+        area_id (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, ProblemDetails]]
+        ProblemDetails
     """
 
     return (
         await asyncio_detailed(
             workspace_id=workspace_id,
             data_point_id=data_point_id,
+            area_id=area_id,
             client=client,
-            json_body=json_body,
         )
     ).parsed
```

### Comparing `nista_library-3.0.6/data_point_client/api/data_point/data_point_append_time_series_data.py` & `nista_library-4.0.0/data_point_client/api/data_point/data_point_delete_message.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,173 +1,200 @@
 from http import HTTPStatus
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional
 
 import httpx
 
+from ... import errors
 from ...client import Client
-from ...models.append_time_series_request import AppendTimeSeriesRequest
 from ...models.problem_details import ProblemDetails
 from ...types import Response
 
 
 def _get_kwargs(
     workspace_id: str,
     data_point_id: str,
+    area_id: str,
+    message_id: str,
     *,
     client: Client,
-    json_body: AppendTimeSeriesRequest,
 ) -> Dict[str, Any]:
-    url = "{}/DataPoint/workspace/{workspaceId}/dataPoint/{dataPointId}/parts".format(
-        client.base_url, workspaceId=workspace_id, dataPointId=data_point_id
+    url = "{}/DataPoint/workspace/{workspaceId}/dataPoint/{dataPointId}/area/{areaId}/message/{messageId}".format(
+        client.base_url, workspaceId=workspace_id, dataPointId=data_point_id, areaId=area_id, messageId=message_id
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
-    json_json_body = json_body.to_dict()
-
     return {
-        "method": "post",
+        "method": "delete",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "json": json_json_body,
+        "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, ProblemDetails]]:
-    if response.status_code == HTTPStatus.ACCEPTED:
-        response_202 = cast(Any, None)
-        return response_202
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ProblemDetails]:
     if response.status_code == HTTPStatus.UNAUTHORIZED:
         response_401 = ProblemDetails.from_dict(response.json())
 
         return response_401
     if response.status_code == HTTPStatus.FORBIDDEN:
         response_403 = ProblemDetails.from_dict(response.json())
 
         return response_403
-    return None
+    if client.raise_on_unexpected_status:
+        raise errors.UnexpectedStatus(response.status_code, response.content)
+    else:
+        return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, ProblemDetails]]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ProblemDetails]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
-        parsed=_parse_response(response=response),
+        parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     workspace_id: str,
     data_point_id: str,
+    area_id: str,
+    message_id: str,
     *,
     client: Client,
-    json_body: AppendTimeSeriesRequest,
-) -> Response[Union[Any, ProblemDetails]]:
+) -> Response[ProblemDetails]:
     """
     Args:
         workspace_id (str):
         data_point_id (str):
-        json_body (AppendTimeSeriesRequest):
+        area_id (str):
+        message_id (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, ProblemDetails]]
+        Response[ProblemDetails]
     """
 
     kwargs = _get_kwargs(
         workspace_id=workspace_id,
         data_point_id=data_point_id,
+        area_id=area_id,
+        message_id=message_id,
         client=client,
-        json_body=json_body,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     workspace_id: str,
     data_point_id: str,
+    area_id: str,
+    message_id: str,
     *,
     client: Client,
-    json_body: AppendTimeSeriesRequest,
-) -> Optional[Union[Any, ProblemDetails]]:
+) -> Optional[ProblemDetails]:
     """
     Args:
         workspace_id (str):
         data_point_id (str):
-        json_body (AppendTimeSeriesRequest):
+        area_id (str):
+        message_id (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, ProblemDetails]]
+        ProblemDetails
     """
 
     return sync_detailed(
         workspace_id=workspace_id,
         data_point_id=data_point_id,
+        area_id=area_id,
+        message_id=message_id,
         client=client,
-        json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
     workspace_id: str,
     data_point_id: str,
+    area_id: str,
+    message_id: str,
     *,
     client: Client,
-    json_body: AppendTimeSeriesRequest,
-) -> Response[Union[Any, ProblemDetails]]:
+) -> Response[ProblemDetails]:
     """
     Args:
         workspace_id (str):
         data_point_id (str):
-        json_body (AppendTimeSeriesRequest):
+        area_id (str):
+        message_id (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, ProblemDetails]]
+        Response[ProblemDetails]
     """
 
     kwargs = _get_kwargs(
         workspace_id=workspace_id,
         data_point_id=data_point_id,
+        area_id=area_id,
+        message_id=message_id,
         client=client,
-        json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
-    return _build_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     workspace_id: str,
     data_point_id: str,
+    area_id: str,
+    message_id: str,
     *,
     client: Client,
-    json_body: AppendTimeSeriesRequest,
-) -> Optional[Union[Any, ProblemDetails]]:
+) -> Optional[ProblemDetails]:
     """
     Args:
         workspace_id (str):
         data_point_id (str):
-        json_body (AppendTimeSeriesRequest):
+        area_id (str):
+        message_id (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, ProblemDetails]]
+        ProblemDetails
     """
 
     return (
         await asyncio_detailed(
             workspace_id=workspace_id,
             data_point_id=data_point_id,
+            area_id=area_id,
+            message_id=message_id,
             client=client,
-            json_body=json_body,
         )
     ).parsed
```

### Comparing `nista_library-3.0.6/data_point_client/api/data_point/data_point_create_data_point.py` & `nista_library-4.0.0/data_point_client/api/data_point/data_point_delete_data_point_cleanup_rule.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,177 +1,174 @@
 from http import HTTPStatus
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional
 
 import httpx
 
+from ... import errors
 from ...client import Client
-from ...models.data_point_request import DataPointRequest
 from ...models.problem_details import ProblemDetails
 from ...types import Response
 
 
 def _get_kwargs(
     workspace_id: str,
     data_point_id: str,
     *,
     client: Client,
-    json_body: DataPointRequest,
 ) -> Dict[str, Any]:
-    url = "{}/DataPoint/workspace/{workspaceId}/dataPoint/{dataPointId}".format(
+    url = "{}/DataPoint/workspace/{workspaceId}/dataPoint/{dataPointId}/rule".format(
         client.base_url, workspaceId=workspace_id, dataPointId=data_point_id
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
-    json_json_body = json_body.to_dict()
-
     return {
-        "method": "post",
+        "method": "delete",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "json": json_json_body,
+        "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, ProblemDetails]]:
-    if response.status_code == HTTPStatus.ACCEPTED:
-        response_202 = cast(Any, None)
-        return response_202
-    if response.status_code == HTTPStatus.BAD_REQUEST:
-        response_400 = ProblemDetails.from_dict(response.json())
-
-        return response_400
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ProblemDetails]:
     if response.status_code == HTTPStatus.UNAUTHORIZED:
         response_401 = ProblemDetails.from_dict(response.json())
 
         return response_401
     if response.status_code == HTTPStatus.FORBIDDEN:
         response_403 = ProblemDetails.from_dict(response.json())
 
         return response_403
-    return None
+    if client.raise_on_unexpected_status:
+        raise errors.UnexpectedStatus(response.status_code, response.content)
+    else:
+        return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, ProblemDetails]]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ProblemDetails]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
-        parsed=_parse_response(response=response),
+        parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     workspace_id: str,
     data_point_id: str,
     *,
     client: Client,
-    json_body: DataPointRequest,
-) -> Response[Union[Any, ProblemDetails]]:
+) -> Response[ProblemDetails]:
     """
     Args:
         workspace_id (str):
         data_point_id (str):
-        json_body (DataPointRequest):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, ProblemDetails]]
+        Response[ProblemDetails]
     """
 
     kwargs = _get_kwargs(
         workspace_id=workspace_id,
         data_point_id=data_point_id,
         client=client,
-        json_body=json_body,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     workspace_id: str,
     data_point_id: str,
     *,
     client: Client,
-    json_body: DataPointRequest,
-) -> Optional[Union[Any, ProblemDetails]]:
+) -> Optional[ProblemDetails]:
     """
     Args:
         workspace_id (str):
         data_point_id (str):
-        json_body (DataPointRequest):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, ProblemDetails]]
+        ProblemDetails
     """
 
     return sync_detailed(
         workspace_id=workspace_id,
         data_point_id=data_point_id,
         client=client,
-        json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
     workspace_id: str,
     data_point_id: str,
     *,
     client: Client,
-    json_body: DataPointRequest,
-) -> Response[Union[Any, ProblemDetails]]:
+) -> Response[ProblemDetails]:
     """
     Args:
         workspace_id (str):
         data_point_id (str):
-        json_body (DataPointRequest):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, ProblemDetails]]
+        Response[ProblemDetails]
     """
 
     kwargs = _get_kwargs(
         workspace_id=workspace_id,
         data_point_id=data_point_id,
         client=client,
-        json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
-    return _build_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     workspace_id: str,
     data_point_id: str,
     *,
     client: Client,
-    json_body: DataPointRequest,
-) -> Optional[Union[Any, ProblemDetails]]:
+) -> Optional[ProblemDetails]:
     """
     Args:
         workspace_id (str):
         data_point_id (str):
-        json_body (DataPointRequest):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, ProblemDetails]]
+        ProblemDetails
     """
 
     return (
         await asyncio_detailed(
             workspace_id=workspace_id,
             data_point_id=data_point_id,
             client=client,
-            json_body=json_body,
         )
     ).parsed
```

### Comparing `nista_library-3.0.6/data_point_client/api/data_point/data_point_delete_data_point.py` & `nista_library-4.0.0/data_point_client/api/data_point/data_point_delete_data_point.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional
 
 import httpx
 
+from ... import errors
 from ...client import Client
 from ...models.problem_details import ProblemDetails
 from ...types import Response
 
 
 def _get_kwargs(
     workspace_id: str,
@@ -23,49 +24,57 @@
 
     return {
         "method": "delete",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[ProblemDetails]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ProblemDetails]:
     if response.status_code == HTTPStatus.UNAUTHORIZED:
         response_401 = ProblemDetails.from_dict(response.json())
 
         return response_401
     if response.status_code == HTTPStatus.FORBIDDEN:
         response_403 = ProblemDetails.from_dict(response.json())
 
         return response_403
-    return None
+    if client.raise_on_unexpected_status:
+        raise errors.UnexpectedStatus(response.status_code, response.content)
+    else:
+        return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[ProblemDetails]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ProblemDetails]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
-        parsed=_parse_response(response=response),
+        parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     workspace_id: str,
     data_point_id: str,
     *,
     client: Client,
 ) -> Response[ProblemDetails]:
     """
     Args:
         workspace_id (str):
         data_point_id (str):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         Response[ProblemDetails]
     """
 
     kwargs = _get_kwargs(
         workspace_id=workspace_id,
         data_point_id=data_point_id,
@@ -73,30 +82,34 @@
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     workspace_id: str,
     data_point_id: str,
     *,
     client: Client,
 ) -> Optional[ProblemDetails]:
     """
     Args:
         workspace_id (str):
         data_point_id (str):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        Response[ProblemDetails]
+        ProblemDetails
     """
 
     return sync_detailed(
         workspace_id=workspace_id,
         data_point_id=data_point_id,
         client=client,
     ).parsed
@@ -109,43 +122,51 @@
     client: Client,
 ) -> Response[ProblemDetails]:
     """
     Args:
         workspace_id (str):
         data_point_id (str):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         Response[ProblemDetails]
     """
 
     kwargs = _get_kwargs(
         workspace_id=workspace_id,
         data_point_id=data_point_id,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
-    return _build_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     workspace_id: str,
     data_point_id: str,
     *,
     client: Client,
 ) -> Optional[ProblemDetails]:
     """
     Args:
         workspace_id (str):
         data_point_id (str):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        Response[ProblemDetails]
+        ProblemDetails
     """
 
     return (
         await asyncio_detailed(
             workspace_id=workspace_id,
             data_point_id=data_point_id,
             client=client,
```

### Comparing `nista_library-3.0.6/data_point_client/api/data_point/data_point_get_data.py` & `nista_library-4.0.0/data_point_client/api/data_point/data_point_get_data.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
+from ... import errors
 from ...client import Client
 from ...models.get_data_request import GetDataRequest
 from ...models.get_data_response import GetDataResponse
 from ...models.problem_details import ProblemDetails
 from ...types import Response
 
 
@@ -28,40 +29,44 @@
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[GetDataResponse, ProblemDetails]]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[GetDataResponse, ProblemDetails]]:
     if response.status_code == HTTPStatus.OK:
         response_200 = GetDataResponse.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.UNAUTHORIZED:
         response_401 = ProblemDetails.from_dict(response.json())
 
         return response_401
     if response.status_code == HTTPStatus.FORBIDDEN:
         response_403 = ProblemDetails.from_dict(response.json())
 
         return response_403
-    return None
+    if client.raise_on_unexpected_status:
+        raise errors.UnexpectedStatus(response.status_code, response.content)
+    else:
+        return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[GetDataResponse, ProblemDetails]]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[GetDataResponse, ProblemDetails]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
-        parsed=_parse_response(response=response),
+        parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     workspace_id: str,
     data_point_id: str,
     *,
@@ -70,14 +75,18 @@
 ) -> Response[Union[GetDataResponse, ProblemDetails]]:
     """
     Args:
         workspace_id (str):
         data_point_id (str):
         json_body (GetDataRequest):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         Response[Union[GetDataResponse, ProblemDetails]]
     """
 
     kwargs = _get_kwargs(
         workspace_id=workspace_id,
         data_point_id=data_point_id,
@@ -86,15 +95,15 @@
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     workspace_id: str,
     data_point_id: str,
     *,
     client: Client,
@@ -102,16 +111,20 @@
 ) -> Optional[Union[GetDataResponse, ProblemDetails]]:
     """
     Args:
         workspace_id (str):
         data_point_id (str):
         json_body (GetDataRequest):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        Response[Union[GetDataResponse, ProblemDetails]]
+        Union[GetDataResponse, ProblemDetails]
     """
 
     return sync_detailed(
         workspace_id=workspace_id,
         data_point_id=data_point_id,
         client=client,
         json_body=json_body,
@@ -127,29 +140,33 @@
 ) -> Response[Union[GetDataResponse, ProblemDetails]]:
     """
     Args:
         workspace_id (str):
         data_point_id (str):
         json_body (GetDataRequest):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         Response[Union[GetDataResponse, ProblemDetails]]
     """
 
     kwargs = _get_kwargs(
         workspace_id=workspace_id,
         data_point_id=data_point_id,
         client=client,
         json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
-    return _build_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     workspace_id: str,
     data_point_id: str,
     *,
     client: Client,
@@ -157,16 +174,20 @@
 ) -> Optional[Union[GetDataResponse, ProblemDetails]]:
     """
     Args:
         workspace_id (str):
         data_point_id (str):
         json_body (GetDataRequest):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        Response[Union[GetDataResponse, ProblemDetails]]
+        Union[GetDataResponse, ProblemDetails]
     """
 
     return (
         await asyncio_detailed(
             workspace_id=workspace_id,
             data_point_id=data_point_id,
             client=client,
```

### Comparing `nista_library-3.0.6/data_point_client/api/data_point/data_point_get_data_points.py` & `nista_library-4.0.0/data_point_client/api/data_point/data_point_get_data_points.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from http import HTTPStatus
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
+from ... import errors
 from ...client import Client
 from ...models.data_point_response_base import DataPointResponseBase
 from ...models.en_data_point_existence_dto import EnDataPointExistenceDTO
 from ...models.en_data_point_type import EnDataPointType
 from ...models.problem_details import ProblemDetails
 from ...types import UNSET, Response, Unset
 
@@ -67,19 +68,22 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[List["DataPointResponseBase"], ProblemDetails]]:
+def _parse_response(
+    *, client: Client, response: httpx.Response
+) -> Optional[Union[List["DataPointResponseBase"], ProblemDetails]]:
     if response.status_code == HTTPStatus.OK:
         response_200 = []
         _response_200 = response.json()
         for response_200_item_data in _response_200:
             response_200_item = DataPointResponseBase.from_dict(response_200_item_data)
 
             response_200.append(response_200_item)
@@ -89,23 +93,28 @@
         response_401 = ProblemDetails.from_dict(response.json())
 
         return response_401
     if response.status_code == HTTPStatus.FORBIDDEN:
         response_403 = ProblemDetails.from_dict(response.json())
 
         return response_403
-    return None
+    if client.raise_on_unexpected_status:
+        raise errors.UnexpectedStatus(response.status_code, response.content)
+    else:
+        return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[List["DataPointResponseBase"], ProblemDetails]]:
+def _build_response(
+    *, client: Client, response: httpx.Response
+) -> Response[Union[List["DataPointResponseBase"], ProblemDetails]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
-        parsed=_parse_response(response=response),
+        parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     workspace_id: str,
     *,
     client: Client,
@@ -118,14 +127,18 @@
     Args:
         workspace_id (str):
         type (Union[Unset, None, List[EnDataPointType]]):
         existence (Union[Unset, None, List[EnDataPointExistenceDTO]]):
         filter_smart_query (Union[Unset, None, str]):
         filter_tags (Union[Unset, None, List[str]]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         Response[Union[List['DataPointResponseBase'], ProblemDetails]]
     """
 
     kwargs = _get_kwargs(
         workspace_id=workspace_id,
         client=client,
@@ -136,15 +149,15 @@
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     workspace_id: str,
     *,
     client: Client,
     type: Union[Unset, None, List[EnDataPointType]] = UNSET,
@@ -156,16 +169,20 @@
     Args:
         workspace_id (str):
         type (Union[Unset, None, List[EnDataPointType]]):
         existence (Union[Unset, None, List[EnDataPointExistenceDTO]]):
         filter_smart_query (Union[Unset, None, str]):
         filter_tags (Union[Unset, None, List[str]]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        Response[Union[List['DataPointResponseBase'], ProblemDetails]]
+        Union[List['DataPointResponseBase'], ProblemDetails]
     """
 
     return sync_detailed(
         workspace_id=workspace_id,
         client=client,
         type=type,
         existence=existence,
@@ -187,14 +204,18 @@
     Args:
         workspace_id (str):
         type (Union[Unset, None, List[EnDataPointType]]):
         existence (Union[Unset, None, List[EnDataPointExistenceDTO]]):
         filter_smart_query (Union[Unset, None, str]):
         filter_tags (Union[Unset, None, List[str]]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         Response[Union[List['DataPointResponseBase'], ProblemDetails]]
     """
 
     kwargs = _get_kwargs(
         workspace_id=workspace_id,
         client=client,
@@ -203,15 +224,15 @@
         filter_smart_query=filter_smart_query,
         filter_tags=filter_tags,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
-    return _build_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     workspace_id: str,
     *,
     client: Client,
     type: Union[Unset, None, List[EnDataPointType]] = UNSET,
@@ -223,16 +244,20 @@
     Args:
         workspace_id (str):
         type (Union[Unset, None, List[EnDataPointType]]):
         existence (Union[Unset, None, List[EnDataPointExistenceDTO]]):
         filter_smart_query (Union[Unset, None, str]):
         filter_tags (Union[Unset, None, List[str]]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        Response[Union[List['DataPointResponseBase'], ProblemDetails]]
+        Union[List['DataPointResponseBase'], ProblemDetails]
     """
 
     return (
         await asyncio_detailed(
             workspace_id=workspace_id,
             client=client,
             type=type,
```

### Comparing `nista_library-3.0.6/data_point_client/api/data_point/data_point_get_tags.py` & `nista_library-4.0.0/data_point_client/api/data_point/data_point_get_tags.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from http import HTTPStatus
 from typing import Any, Dict, List, Optional, Union, cast
 
 import httpx
 
+from ... import errors
 from ...client import Client
 from ...models.en_data_point_existence_dto import EnDataPointExistenceDTO
 from ...models.en_data_point_type import EnDataPointType
 from ...models.problem_details import ProblemDetails
 from ...types import UNSET, Response, Unset
 
 
@@ -63,40 +64,44 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[List[str], ProblemDetails]]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[List[str], ProblemDetails]]:
     if response.status_code == HTTPStatus.OK:
         response_200 = cast(List[str], response.json())
 
         return response_200
     if response.status_code == HTTPStatus.UNAUTHORIZED:
         response_401 = ProblemDetails.from_dict(response.json())
 
         return response_401
     if response.status_code == HTTPStatus.FORBIDDEN:
         response_403 = ProblemDetails.from_dict(response.json())
 
         return response_403
-    return None
+    if client.raise_on_unexpected_status:
+        raise errors.UnexpectedStatus(response.status_code, response.content)
+    else:
+        return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[List[str], ProblemDetails]]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[List[str], ProblemDetails]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
-        parsed=_parse_response(response=response),
+        parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     workspace_id: str,
     *,
     client: Client,
@@ -107,14 +112,18 @@
     """
     Args:
         workspace_id (str):
         filter_tags (Union[Unset, None, List[str]]):
         type (Union[Unset, None, List[EnDataPointType]]):
         existence (Union[Unset, None, List[EnDataPointExistenceDTO]]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         Response[Union[List[str], ProblemDetails]]
     """
 
     kwargs = _get_kwargs(
         workspace_id=workspace_id,
         client=client,
@@ -124,15 +133,15 @@
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     workspace_id: str,
     *,
     client: Client,
     filter_tags: Union[Unset, None, List[str]] = UNSET,
@@ -142,16 +151,20 @@
     """
     Args:
         workspace_id (str):
         filter_tags (Union[Unset, None, List[str]]):
         type (Union[Unset, None, List[EnDataPointType]]):
         existence (Union[Unset, None, List[EnDataPointExistenceDTO]]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        Response[Union[List[str], ProblemDetails]]
+        Union[List[str], ProblemDetails]
     """
 
     return sync_detailed(
         workspace_id=workspace_id,
         client=client,
         filter_tags=filter_tags,
         type=type,
@@ -170,14 +183,18 @@
     """
     Args:
         workspace_id (str):
         filter_tags (Union[Unset, None, List[str]]):
         type (Union[Unset, None, List[EnDataPointType]]):
         existence (Union[Unset, None, List[EnDataPointExistenceDTO]]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         Response[Union[List[str], ProblemDetails]]
     """
 
     kwargs = _get_kwargs(
         workspace_id=workspace_id,
         client=client,
@@ -185,15 +202,15 @@
         type=type,
         existence=existence,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
-    return _build_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     workspace_id: str,
     *,
     client: Client,
     filter_tags: Union[Unset, None, List[str]] = UNSET,
@@ -203,16 +220,20 @@
     """
     Args:
         workspace_id (str):
         filter_tags (Union[Unset, None, List[str]]):
         type (Union[Unset, None, List[EnDataPointType]]):
         existence (Union[Unset, None, List[EnDataPointExistenceDTO]]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        Response[Union[List[str], ProblemDetails]]
+        Union[List[str], ProblemDetails]
     """
 
     return (
         await asyncio_detailed(
             workspace_id=workspace_id,
             client=client,
             filter_tags=filter_tags,
```

### Comparing `nista_library-3.0.6/data_point_client/api/data_point/data_point_update_data_point.py` & `nista_library-4.0.0/data_point_client/api/data_point/data_point_update_data_point_cleanup_rule.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,51 @@
 from http import HTTPStatus
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, List, Optional, Union, cast
 
 import httpx
 
+from ... import errors
 from ...client import Client
-from ...models.data_point_request import DataPointRequest
 from ...models.problem_details import ProblemDetails
+from ...models.rule import Rule
 from ...types import Response
 
 
 def _get_kwargs(
     workspace_id: str,
     data_point_id: str,
     *,
     client: Client,
-    json_body: DataPointRequest,
+    json_body: List["Rule"],
 ) -> Dict[str, Any]:
-    url = "{}/DataPoint/workspace/{workspaceId}/dataPoint/{dataPointId}".format(
+    url = "{}/DataPoint/workspace/{workspaceId}/dataPoint/{dataPointId}/rule".format(
         client.base_url, workspaceId=workspace_id, dataPointId=data_point_id
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
-    json_json_body = json_body.to_dict()
+    json_json_body = []
+    for json_body_item_data in json_body:
+        json_body_item = json_body_item_data.to_dict()
+
+        json_json_body.append(json_body_item)
 
     return {
         "method": "patch",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, ProblemDetails]]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, ProblemDetails]]:
     if response.status_code == HTTPStatus.ACCEPTED:
         response_202 = cast(Any, None)
         return response_202
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = ProblemDetails.from_dict(response.json())
 
         return response_400
@@ -47,38 +53,45 @@
         response_401 = ProblemDetails.from_dict(response.json())
 
         return response_401
     if response.status_code == HTTPStatus.FORBIDDEN:
         response_403 = ProblemDetails.from_dict(response.json())
 
         return response_403
-    return None
+    if client.raise_on_unexpected_status:
+        raise errors.UnexpectedStatus(response.status_code, response.content)
+    else:
+        return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, ProblemDetails]]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, ProblemDetails]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
-        parsed=_parse_response(response=response),
+        parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     workspace_id: str,
     data_point_id: str,
     *,
     client: Client,
-    json_body: DataPointRequest,
+    json_body: List["Rule"],
 ) -> Response[Union[Any, ProblemDetails]]:
     """
     Args:
         workspace_id (str):
         data_point_id (str):
-        json_body (DataPointRequest):
+        json_body (List['Rule']):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Union[Any, ProblemDetails]]
     """
 
     kwargs = _get_kwargs(
         workspace_id=workspace_id,
@@ -88,32 +101,36 @@
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     workspace_id: str,
     data_point_id: str,
     *,
     client: Client,
-    json_body: DataPointRequest,
+    json_body: List["Rule"],
 ) -> Optional[Union[Any, ProblemDetails]]:
     """
     Args:
         workspace_id (str):
         data_point_id (str):
-        json_body (DataPointRequest):
+        json_body (List['Rule']):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, ProblemDetails]]
+        Union[Any, ProblemDetails]
     """
 
     return sync_detailed(
         workspace_id=workspace_id,
         data_point_id=data_point_id,
         client=client,
         json_body=json_body,
@@ -121,21 +138,25 @@
 
 
 async def asyncio_detailed(
     workspace_id: str,
     data_point_id: str,
     *,
     client: Client,
-    json_body: DataPointRequest,
+    json_body: List["Rule"],
 ) -> Response[Union[Any, ProblemDetails]]:
     """
     Args:
         workspace_id (str):
         data_point_id (str):
-        json_body (DataPointRequest):
+        json_body (List['Rule']):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Union[Any, ProblemDetails]]
     """
 
     kwargs = _get_kwargs(
         workspace_id=workspace_id,
@@ -143,32 +164,36 @@
         client=client,
         json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
-    return _build_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     workspace_id: str,
     data_point_id: str,
     *,
     client: Client,
-    json_body: DataPointRequest,
+    json_body: List["Rule"],
 ) -> Optional[Union[Any, ProblemDetails]]:
     """
     Args:
         workspace_id (str):
         data_point_id (str):
-        json_body (DataPointRequest):
+        json_body (List['Rule']):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, ProblemDetails]]
+        Union[Any, ProblemDetails]
     """
 
     return (
         await asyncio_detailed(
             workspace_id=workspace_id,
             data_point_id=data_point_id,
             client=client,
```

### Comparing `nista_library-3.0.6/data_point_client/api/data_point/data_point_update_data_point_cleanup_rule.py` & `nista_library-4.0.0/data_point_client/api/data_point/data_point_update_data_point_unit.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,49 +1,46 @@
 from http import HTTPStatus
-from typing import Any, Dict, List, Optional, Union, cast
+from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
+from ... import errors
 from ...client import Client
 from ...models.problem_details import ProblemDetails
-from ...models.rule import Rule
 from ...types import Response
 
 
 def _get_kwargs(
     workspace_id: str,
     data_point_id: str,
     *,
     client: Client,
-    json_body: List["Rule"],
+    json_body: str,
 ) -> Dict[str, Any]:
-    url = "{}/DataPoint/workspace/{workspaceId}/dataPoint/{dataPointId}/rule".format(
+    url = "{}/DataPoint/workspace/{workspaceId}/dataPoint/{dataPointId}/unit".format(
         client.base_url, workspaceId=workspace_id, dataPointId=data_point_id
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
-    json_json_body = []
-    for json_body_item_data in json_body:
-        json_body_item = json_body_item_data.to_dict()
-
-        json_json_body.append(json_body_item)
+    json_json_body = json_body
 
     return {
         "method": "patch",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, ProblemDetails]]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, ProblemDetails]]:
     if response.status_code == HTTPStatus.ACCEPTED:
         response_202 = cast(Any, None)
         return response_202
     if response.status_code == HTTPStatus.BAD_REQUEST:
         response_400 = ProblemDetails.from_dict(response.json())
 
         return response_400
@@ -51,38 +48,45 @@
         response_401 = ProblemDetails.from_dict(response.json())
 
         return response_401
     if response.status_code == HTTPStatus.FORBIDDEN:
         response_403 = ProblemDetails.from_dict(response.json())
 
         return response_403
-    return None
+    if client.raise_on_unexpected_status:
+        raise errors.UnexpectedStatus(response.status_code, response.content)
+    else:
+        return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, ProblemDetails]]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, ProblemDetails]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
-        parsed=_parse_response(response=response),
+        parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     workspace_id: str,
     data_point_id: str,
     *,
     client: Client,
-    json_body: List["Rule"],
+    json_body: str,
 ) -> Response[Union[Any, ProblemDetails]]:
     """
     Args:
         workspace_id (str):
         data_point_id (str):
-        json_body (List['Rule']):
+        json_body (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Union[Any, ProblemDetails]]
     """
 
     kwargs = _get_kwargs(
         workspace_id=workspace_id,
@@ -92,32 +96,36 @@
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     workspace_id: str,
     data_point_id: str,
     *,
     client: Client,
-    json_body: List["Rule"],
+    json_body: str,
 ) -> Optional[Union[Any, ProblemDetails]]:
     """
     Args:
         workspace_id (str):
         data_point_id (str):
-        json_body (List['Rule']):
+        json_body (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, ProblemDetails]]
+        Union[Any, ProblemDetails]
     """
 
     return sync_detailed(
         workspace_id=workspace_id,
         data_point_id=data_point_id,
         client=client,
         json_body=json_body,
@@ -125,21 +133,25 @@
 
 
 async def asyncio_detailed(
     workspace_id: str,
     data_point_id: str,
     *,
     client: Client,
-    json_body: List["Rule"],
+    json_body: str,
 ) -> Response[Union[Any, ProblemDetails]]:
     """
     Args:
         workspace_id (str):
         data_point_id (str):
-        json_body (List['Rule']):
+        json_body (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Union[Any, ProblemDetails]]
     """
 
     kwargs = _get_kwargs(
         workspace_id=workspace_id,
@@ -147,32 +159,36 @@
         client=client,
         json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
-    return _build_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     workspace_id: str,
     data_point_id: str,
     *,
     client: Client,
-    json_body: List["Rule"],
+    json_body: str,
 ) -> Optional[Union[Any, ProblemDetails]]:
     """
     Args:
         workspace_id (str):
         data_point_id (str):
-        json_body (List['Rule']):
+        json_body (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, ProblemDetails]]
+        Union[Any, ProblemDetails]
     """
 
     return (
         await asyncio_detailed(
             workspace_id=workspace_id,
             data_point_id=data_point_id,
             client=client,
```

### Comparing `nista_library-3.0.6/data_point_client/api/data_point/data_point_update_data_point_unit.py` & `nista_library-4.0.0/data_point_client/api/data_point/data_point_update_day_period_data.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,83 +1,89 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
+from ... import errors
 from ...client import Client
 from ...models.problem_details import ProblemDetails
+from ...models.update_day_period_request import UpdateDayPeriodRequest
 from ...types import Response
 
 
 def _get_kwargs(
     workspace_id: str,
     data_point_id: str,
     *,
     client: Client,
-    json_body: str,
+    json_body: UpdateDayPeriodRequest,
 ) -> Dict[str, Any]:
-    url = "{}/DataPoint/workspace/{workspaceId}/dataPoint/{dataPointId}/unit".format(
+    url = "{}/DataPoint/workspace/{workspaceId}/dataPoint/{dataPointId}/dayperiod".format(
         client.base_url, workspaceId=workspace_id, dataPointId=data_point_id
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
-    json_json_body = json_body
+    json_json_body = json_body.to_dict()
 
     return {
-        "method": "patch",
+        "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, ProblemDetails]]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, ProblemDetails]]:
     if response.status_code == HTTPStatus.ACCEPTED:
         response_202 = cast(Any, None)
         return response_202
-    if response.status_code == HTTPStatus.BAD_REQUEST:
-        response_400 = ProblemDetails.from_dict(response.json())
-
-        return response_400
     if response.status_code == HTTPStatus.UNAUTHORIZED:
         response_401 = ProblemDetails.from_dict(response.json())
 
         return response_401
     if response.status_code == HTTPStatus.FORBIDDEN:
         response_403 = ProblemDetails.from_dict(response.json())
 
         return response_403
-    return None
+    if client.raise_on_unexpected_status:
+        raise errors.UnexpectedStatus(response.status_code, response.content)
+    else:
+        return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, ProblemDetails]]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, ProblemDetails]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
-        parsed=_parse_response(response=response),
+        parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     workspace_id: str,
     data_point_id: str,
     *,
     client: Client,
-    json_body: str,
+    json_body: UpdateDayPeriodRequest,
 ) -> Response[Union[Any, ProblemDetails]]:
     """
     Args:
         workspace_id (str):
         data_point_id (str):
-        json_body (str):
+        json_body (UpdateDayPeriodRequest):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Union[Any, ProblemDetails]]
     """
 
     kwargs = _get_kwargs(
         workspace_id=workspace_id,
@@ -87,32 +93,36 @@
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     workspace_id: str,
     data_point_id: str,
     *,
     client: Client,
-    json_body: str,
+    json_body: UpdateDayPeriodRequest,
 ) -> Optional[Union[Any, ProblemDetails]]:
     """
     Args:
         workspace_id (str):
         data_point_id (str):
-        json_body (str):
+        json_body (UpdateDayPeriodRequest):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, ProblemDetails]]
+        Union[Any, ProblemDetails]
     """
 
     return sync_detailed(
         workspace_id=workspace_id,
         data_point_id=data_point_id,
         client=client,
         json_body=json_body,
@@ -120,21 +130,25 @@
 
 
 async def asyncio_detailed(
     workspace_id: str,
     data_point_id: str,
     *,
     client: Client,
-    json_body: str,
+    json_body: UpdateDayPeriodRequest,
 ) -> Response[Union[Any, ProblemDetails]]:
     """
     Args:
         workspace_id (str):
         data_point_id (str):
-        json_body (str):
+        json_body (UpdateDayPeriodRequest):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Union[Any, ProblemDetails]]
     """
 
     kwargs = _get_kwargs(
         workspace_id=workspace_id,
@@ -142,32 +156,36 @@
         client=client,
         json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
-    return _build_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     workspace_id: str,
     data_point_id: str,
     *,
     client: Client,
-    json_body: str,
+    json_body: UpdateDayPeriodRequest,
 ) -> Optional[Union[Any, ProblemDetails]]:
     """
     Args:
         workspace_id (str):
         data_point_id (str):
-        json_body (str):
+        json_body (UpdateDayPeriodRequest):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, ProblemDetails]]
+        Union[Any, ProblemDetails]
     """
 
     return (
         await asyncio_detailed(
             workspace_id=workspace_id,
             data_point_id=data_point_id,
             client=client,
```

### Comparing `nista_library-3.0.6/data_point_client/api/data_point/data_point_update_day_period_data.py` & `nista_library-4.0.0/data_point_client/api/data_point/data_point_update_week_period_data.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,80 +1,89 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union, cast
 
 import httpx
 
+from ... import errors
 from ...client import Client
 from ...models.problem_details import ProblemDetails
-from ...models.update_day_period_request import UpdateDayPeriodRequest
+from ...models.update_week_period_request import UpdateWeekPeriodRequest
 from ...types import Response
 
 
 def _get_kwargs(
     workspace_id: str,
     data_point_id: str,
     *,
     client: Client,
-    json_body: UpdateDayPeriodRequest,
+    json_body: UpdateWeekPeriodRequest,
 ) -> Dict[str, Any]:
-    url = "{}/DataPoint/workspace/{workspaceId}/dataPoint/{dataPointId}/dayperiod".format(
+    url = "{}/DataPoint/workspace/{workspaceId}/dataPoint/{dataPointId}/weekperiod".format(
         client.base_url, workspaceId=workspace_id, dataPointId=data_point_id
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     json_json_body = json_body.to_dict()
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, ProblemDetails]]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Union[Any, ProblemDetails]]:
     if response.status_code == HTTPStatus.ACCEPTED:
         response_202 = cast(Any, None)
         return response_202
     if response.status_code == HTTPStatus.UNAUTHORIZED:
         response_401 = ProblemDetails.from_dict(response.json())
 
         return response_401
     if response.status_code == HTTPStatus.FORBIDDEN:
         response_403 = ProblemDetails.from_dict(response.json())
 
         return response_403
-    return None
+    if client.raise_on_unexpected_status:
+        raise errors.UnexpectedStatus(response.status_code, response.content)
+    else:
+        return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, ProblemDetails]]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[Union[Any, ProblemDetails]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
-        parsed=_parse_response(response=response),
+        parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     workspace_id: str,
     data_point_id: str,
     *,
     client: Client,
-    json_body: UpdateDayPeriodRequest,
+    json_body: UpdateWeekPeriodRequest,
 ) -> Response[Union[Any, ProblemDetails]]:
     """
     Args:
         workspace_id (str):
         data_point_id (str):
-        json_body (UpdateDayPeriodRequest):
+        json_body (UpdateWeekPeriodRequest):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Union[Any, ProblemDetails]]
     """
 
     kwargs = _get_kwargs(
         workspace_id=workspace_id,
@@ -84,32 +93,36 @@
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     workspace_id: str,
     data_point_id: str,
     *,
     client: Client,
-    json_body: UpdateDayPeriodRequest,
+    json_body: UpdateWeekPeriodRequest,
 ) -> Optional[Union[Any, ProblemDetails]]:
     """
     Args:
         workspace_id (str):
         data_point_id (str):
-        json_body (UpdateDayPeriodRequest):
+        json_body (UpdateWeekPeriodRequest):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, ProblemDetails]]
+        Union[Any, ProblemDetails]
     """
 
     return sync_detailed(
         workspace_id=workspace_id,
         data_point_id=data_point_id,
         client=client,
         json_body=json_body,
@@ -117,21 +130,25 @@
 
 
 async def asyncio_detailed(
     workspace_id: str,
     data_point_id: str,
     *,
     client: Client,
-    json_body: UpdateDayPeriodRequest,
+    json_body: UpdateWeekPeriodRequest,
 ) -> Response[Union[Any, ProblemDetails]]:
     """
     Args:
         workspace_id (str):
         data_point_id (str):
-        json_body (UpdateDayPeriodRequest):
+        json_body (UpdateWeekPeriodRequest):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Union[Any, ProblemDetails]]
     """
 
     kwargs = _get_kwargs(
         workspace_id=workspace_id,
@@ -139,32 +156,36 @@
         client=client,
         json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
-    return _build_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     workspace_id: str,
     data_point_id: str,
     *,
     client: Client,
-    json_body: UpdateDayPeriodRequest,
+    json_body: UpdateWeekPeriodRequest,
 ) -> Optional[Union[Any, ProblemDetails]]:
     """
     Args:
         workspace_id (str):
         data_point_id (str):
-        json_body (UpdateDayPeriodRequest):
+        json_body (UpdateWeekPeriodRequest):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, ProblemDetails]]
+        Union[Any, ProblemDetails]
     """
 
     return (
         await asyncio_detailed(
             workspace_id=workspace_id,
             data_point_id=data_point_id,
             client=client,
```

### Comparing `nista_library-3.0.6/data_point_client/api/data_point/data_point_update_time_series_data.py` & `nista_library-4.0.0/data_point_client/api/data_point/data_point_get_data_point_by_version.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,173 +1,196 @@
 from http import HTTPStatus
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
+from ... import errors
 from ...client import Client
+from ...models.data_point_response_base import DataPointResponseBase
 from ...models.problem_details import ProblemDetails
-from ...models.update_time_series_request import UpdateTimeSeriesRequest
 from ...types import Response
 
 
 def _get_kwargs(
     workspace_id: str,
     data_point_id: str,
+    version: int,
     *,
     client: Client,
-    json_body: UpdateTimeSeriesRequest,
 ) -> Dict[str, Any]:
-    url = "{}/DataPoint/workspace/{workspaceId}/dataPoint/{dataPointId}/timeseries".format(
-        client.base_url, workspaceId=workspace_id, dataPointId=data_point_id
+    url = "{}/DataPoint/workspace/{workspaceId}/dataPoint/{dataPointId}/version/{version}".format(
+        client.base_url, workspaceId=workspace_id, dataPointId=data_point_id, version=version
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
-    json_json_body = json_body.to_dict()
-
     return {
-        "method": "post",
+        "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "json": json_json_body,
+        "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, ProblemDetails]]:
-    if response.status_code == HTTPStatus.ACCEPTED:
-        response_202 = cast(Any, None)
-        return response_202
+def _parse_response(
+    *, client: Client, response: httpx.Response
+) -> Optional[Union[DataPointResponseBase, ProblemDetails]]:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = DataPointResponseBase.from_dict(response.json())
+
+        return response_200
     if response.status_code == HTTPStatus.UNAUTHORIZED:
         response_401 = ProblemDetails.from_dict(response.json())
 
         return response_401
     if response.status_code == HTTPStatus.FORBIDDEN:
         response_403 = ProblemDetails.from_dict(response.json())
 
         return response_403
-    return None
+    if client.raise_on_unexpected_status:
+        raise errors.UnexpectedStatus(response.status_code, response.content)
+    else:
+        return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, ProblemDetails]]:
+def _build_response(
+    *, client: Client, response: httpx.Response
+) -> Response[Union[DataPointResponseBase, ProblemDetails]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
-        parsed=_parse_response(response=response),
+        parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     workspace_id: str,
     data_point_id: str,
+    version: int,
     *,
     client: Client,
-    json_body: UpdateTimeSeriesRequest,
-) -> Response[Union[Any, ProblemDetails]]:
+) -> Response[Union[DataPointResponseBase, ProblemDetails]]:
     """
     Args:
         workspace_id (str):
         data_point_id (str):
-        json_body (UpdateTimeSeriesRequest):
+        version (int):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, ProblemDetails]]
+        Response[Union[DataPointResponseBase, ProblemDetails]]
     """
 
     kwargs = _get_kwargs(
         workspace_id=workspace_id,
         data_point_id=data_point_id,
+        version=version,
         client=client,
-        json_body=json_body,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     workspace_id: str,
     data_point_id: str,
+    version: int,
     *,
     client: Client,
-    json_body: UpdateTimeSeriesRequest,
-) -> Optional[Union[Any, ProblemDetails]]:
+) -> Optional[Union[DataPointResponseBase, ProblemDetails]]:
     """
     Args:
         workspace_id (str):
         data_point_id (str):
-        json_body (UpdateTimeSeriesRequest):
+        version (int):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, ProblemDetails]]
+        Union[DataPointResponseBase, ProblemDetails]
     """
 
     return sync_detailed(
         workspace_id=workspace_id,
         data_point_id=data_point_id,
+        version=version,
         client=client,
-        json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
     workspace_id: str,
     data_point_id: str,
+    version: int,
     *,
     client: Client,
-    json_body: UpdateTimeSeriesRequest,
-) -> Response[Union[Any, ProblemDetails]]:
+) -> Response[Union[DataPointResponseBase, ProblemDetails]]:
     """
     Args:
         workspace_id (str):
         data_point_id (str):
-        json_body (UpdateTimeSeriesRequest):
+        version (int):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, ProblemDetails]]
+        Response[Union[DataPointResponseBase, ProblemDetails]]
     """
 
     kwargs = _get_kwargs(
         workspace_id=workspace_id,
         data_point_id=data_point_id,
+        version=version,
         client=client,
-        json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
-    return _build_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     workspace_id: str,
     data_point_id: str,
+    version: int,
     *,
     client: Client,
-    json_body: UpdateTimeSeriesRequest,
-) -> Optional[Union[Any, ProblemDetails]]:
+) -> Optional[Union[DataPointResponseBase, ProblemDetails]]:
     """
     Args:
         workspace_id (str):
         data_point_id (str):
-        json_body (UpdateTimeSeriesRequest):
+        version (int):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Any, ProblemDetails]]
+        Union[DataPointResponseBase, ProblemDetails]
     """
 
     return (
         await asyncio_detailed(
             workspace_id=workspace_id,
             data_point_id=data_point_id,
+            version=version,
             client=client,
-            json_body=json_body,
         )
     ).parsed
```

### Comparing `nista_library-3.0.6/data_point_client/models/append_execution_result_data_request.py` & `nista_library-4.0.0/data_point_client/models/append_execution_result_data_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-3.0.6/data_point_client/models/append_time_series_request.py` & `nista_library-4.0.0/data_point_client/models/append_time_series_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-3.0.6/data_point_client/models/calculation_origin.py` & `nista_library-4.0.0/data_point_client/models/calculation_origin.py`

 * *Files identical despite different names*

### Comparing `nista_library-3.0.6/data_point_client/models/constant_data_bucket.py` & `nista_library-4.0.0/data_point_client/models/constant_data_bucket.py`

 * *Files identical despite different names*

### Comparing `nista_library-3.0.6/data_point_client/models/constant_data_point_data.py` & `nista_library-4.0.0/data_point_client/models/constant_data_point_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-3.0.6/data_point_client/models/data_bucket_base.py` & `nista_library-4.0.0/data_point_client/models/data_bucket_base.py`

 * *Files identical despite different names*

### Comparing `nista_library-3.0.6/data_point_client/models/data_export_request.py` & `nista_library-4.0.0/data_point_client/models/data_export_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-3.0.6/data_point_client/models/data_point_data_base.py` & `nista_library-4.0.0/data_point_client/models/data_point_data_base.py`

 * *Files identical despite different names*

### Comparing `nista_library-3.0.6/data_point_client/models/data_point_data_response.py` & `nista_library-4.0.0/data_point_client/models/data_point_data_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-3.0.6/data_point_client/models/data_point_origin.py` & `nista_library-4.0.0/data_point_client/models/data_point_origin.py`

 * *Files identical despite different names*

### Comparing `nista_library-3.0.6/data_point_client/models/data_point_request.py` & `nista_library-4.0.0/data_point_client/models/data_point_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-3.0.6/data_point_client/models/data_point_response_base.py` & `nista_library-4.0.0/data_point_client/models/data_point_response_base.py`

 * *Files identical despite different names*

### Comparing `nista_library-3.0.6/data_point_client/models/day_data_by_hour_transfer.py` & `nista_library-4.0.0/data_point_client/models/day_data_by_hour_transfer.py`

 * *Files identical despite different names*

### Comparing `nista_library-3.0.6/data_point_client/models/day_period_data_bucket.py` & `nista_library-4.0.0/data_point_client/models/day_period_data_bucket.py`

 * *Files identical despite different names*

### Comparing `nista_library-3.0.6/data_point_client/models/day_period_data_point_data.py` & `nista_library-4.0.0/data_point_client/models/day_period_data_point_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-3.0.6/data_point_client/models/file_origin.py` & `nista_library-4.0.0/data_point_client/models/file_origin.py`

 * *Files identical despite different names*

### Comparing `nista_library-3.0.6/data_point_client/models/get_constant_response.py` & `nista_library-4.0.0/data_point_client/models/get_constant_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-3.0.6/data_point_client/models/get_data_request.py` & `nista_library-4.0.0/data_point_client/models/get_data_request.py`

 * *Files 23% similar despite different names*

```diff
@@ -15,20 +15,24 @@
 class GetDataRequest:
     """
     Attributes:
         window_seconds (Union[Unset, int]):
         version (Union[Unset, None, int]):
         time_series_periods (Union[Unset, None, List['TimeSeriesPeriod']]):
         demanded_unit (Union[Unset, None, str]):
+        remove_time_zone (Union[Unset, bool]):
+        time_zone (Union[Unset, None, str]):
     """
 
     window_seconds: Union[Unset, int] = UNSET
     version: Union[Unset, None, int] = UNSET
     time_series_periods: Union[Unset, None, List["TimeSeriesPeriod"]] = UNSET
     demanded_unit: Union[Unset, None, str] = UNSET
+    remove_time_zone: Union[Unset, bool] = UNSET
+    time_zone: Union[Unset, None, str] = UNSET
 
     def to_dict(self) -> Dict[str, Any]:
         window_seconds = self.window_seconds
         version = self.version
         time_series_periods: Union[Unset, None, List[Dict[str, Any]]] = UNSET
         if not isinstance(self.time_series_periods, Unset):
             if self.time_series_periods is None:
@@ -37,25 +41,31 @@
                 time_series_periods = []
                 for time_series_periods_item_data in self.time_series_periods:
                     time_series_periods_item = time_series_periods_item_data.to_dict()
 
                     time_series_periods.append(time_series_periods_item)
 
         demanded_unit = self.demanded_unit
+        remove_time_zone = self.remove_time_zone
+        time_zone = self.time_zone
 
         field_dict: Dict[str, Any] = {}
         field_dict.update({})
         if window_seconds is not UNSET:
             field_dict["windowSeconds"] = window_seconds
         if version is not UNSET:
             field_dict["version"] = version
         if time_series_periods is not UNSET:
             field_dict["timeSeriesPeriods"] = time_series_periods
         if demanded_unit is not UNSET:
             field_dict["demandedUnit"] = demanded_unit
+        if remove_time_zone is not UNSET:
+            field_dict["removeTimeZone"] = remove_time_zone
+        if time_zone is not UNSET:
+            field_dict["timeZone"] = time_zone
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.time_series_period import TimeSeriesPeriod
 
@@ -69,15 +79,21 @@
         for time_series_periods_item_data in _time_series_periods or []:
             time_series_periods_item = TimeSeriesPeriod.from_dict(time_series_periods_item_data)
 
             time_series_periods.append(time_series_periods_item)
 
         demanded_unit = d.pop("demandedUnit", UNSET)
 
+        remove_time_zone = d.pop("removeTimeZone", UNSET)
+
+        time_zone = d.pop("timeZone", UNSET)
+
         get_data_request = cls(
             window_seconds=window_seconds,
             version=version,
             time_series_periods=time_series_periods,
             demanded_unit=demanded_unit,
+            remove_time_zone=remove_time_zone,
+            time_zone=time_zone,
         )
 
         return get_data_request
```

### Comparing `nista_library-3.0.6/data_point_client/models/get_data_response.py` & `nista_library-4.0.0/data_point_client/models/get_data_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-3.0.6/data_point_client/models/get_day_period_response.py` & `nista_library-4.0.0/data_point_client/models/get_day_period_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-3.0.6/data_point_client/models/get_series_response.py` & `nista_library-4.0.0/data_point_client/models/get_series_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-3.0.6/data_point_client/models/get_week_period_response.py` & `nista_library-4.0.0/data_point_client/models/get_week_period_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-3.0.6/data_point_client/models/gnista_unit_response.py` & `nista_library-4.0.0/data_point_client/models/gnista_unit_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-3.0.6/data_point_client/models/problem_details.py` & `nista_library-4.0.0/data_point_client/models/problem_details.py`

 * *Files identical despite different names*

### Comparing `nista_library-3.0.6/data_point_client/models/problem_details_extensions.py` & `nista_library-4.0.0/data_point_client/models/problem_details_extensions.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 @attr.s(auto_attribs=True)
 class ProblemDetailsExtensions:
     """ """
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
 
         return field_dict
 
     @classmethod
```

### Comparing `nista_library-3.0.6/data_point_client/models/remote_origin.py` & `nista_library-4.0.0/data_point_client/models/remote_origin.py`

 * *Files identical despite different names*

### Comparing `nista_library-3.0.6/data_point_client/models/rule.py` & `nista_library-4.0.0/data_point_client/models/rule.py`

 * *Files identical despite different names*

### Comparing `nista_library-3.0.6/data_point_client/models/series_data_bucket.py` & `nista_library-4.0.0/data_point_client/models/series_data_bucket.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
         gnista_unit (Union[Unset, None, GnistaUnitResponse]):
         error_details (Union[Unset, None, str]):
         warning_details (Union[Unset, None, str]):
         available_data_points (Union[Unset, None, List['DataPointDataResponse']]):
         rules_for_cleanup (Union[Unset, None, List['Rule']]):
         first_entry (Union[Unset, datetime.datetime]):
         last_entry (Union[Unset, datetime.datetime]):
+        time_zone (Union[Unset, None, str]):
     """
 
     discriminator: str
     version: Union[Unset, int] = UNSET
     created: Union[Unset, datetime.datetime] = UNSET
     status: Union[Unset, EnDataBucketState] = UNSET
     violations: Union[Unset, int] = UNSET
@@ -44,14 +45,15 @@
     gnista_unit: Union[Unset, None, "GnistaUnitResponse"] = UNSET
     error_details: Union[Unset, None, str] = UNSET
     warning_details: Union[Unset, None, str] = UNSET
     available_data_points: Union[Unset, None, List["DataPointDataResponse"]] = UNSET
     rules_for_cleanup: Union[Unset, None, List["Rule"]] = UNSET
     first_entry: Union[Unset, datetime.datetime] = UNSET
     last_entry: Union[Unset, datetime.datetime] = UNSET
+    time_zone: Union[Unset, None, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         discriminator = self.discriminator
         version = self.version
         created: Union[Unset, str] = UNSET
         if not isinstance(self.created, Unset):
@@ -95,14 +97,16 @@
         if not isinstance(self.first_entry, Unset):
             first_entry = self.first_entry.isoformat()
 
         last_entry: Union[Unset, str] = UNSET
         if not isinstance(self.last_entry, Unset):
             last_entry = self.last_entry.isoformat()
 
+        time_zone = self.time_zone
+
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "discriminator": discriminator,
             }
         )
@@ -126,14 +130,16 @@
             field_dict["availableDataPoints"] = available_data_points
         if rules_for_cleanup is not UNSET:
             field_dict["rulesForCleanup"] = rules_for_cleanup
         if first_entry is not UNSET:
             field_dict["firstEntry"] = first_entry
         if last_entry is not UNSET:
             field_dict["lastEntry"] = last_entry
+        if time_zone is not UNSET:
+            field_dict["timeZone"] = time_zone
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.data_point_data_response import DataPointDataResponse
         from ..models.gnista_unit_response import GnistaUnitResponse
@@ -199,28 +205,31 @@
         _last_entry = d.pop("lastEntry", UNSET)
         last_entry: Union[Unset, datetime.datetime]
         if isinstance(_last_entry, Unset):
             last_entry = UNSET
         else:
             last_entry = isoparse(_last_entry)
 
+        time_zone = d.pop("timeZone", UNSET)
+
         series_data_bucket = cls(
             discriminator=discriminator,
             version=version,
             created=created,
             status=status,
             violations=violations,
             unit=unit,
             gnista_unit=gnista_unit,
             error_details=error_details,
             warning_details=warning_details,
             available_data_points=available_data_points,
             rules_for_cleanup=rules_for_cleanup,
             first_entry=first_entry,
             last_entry=last_entry,
+            time_zone=time_zone,
         )
 
         series_data_bucket.additional_properties = d
         return series_data_bucket
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `nista_library-3.0.6/data_point_client/models/series_data_point_data.py` & `nista_library-4.0.0/data_point_client/models/series_data_point_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-3.0.6/data_point_client/models/sub_series_request.py` & `nista_library-4.0.0/data_point_client/models/sub_series_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-3.0.6/data_point_client/models/sub_series_request_values.py` & `nista_library-4.0.0/data_point_client/models/sub_series_request_values.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 @attr.s(auto_attribs=True)
 class SubSeriesRequestValues:
     """ """
 
     additional_properties: Dict[str, float] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
 
         return field_dict
 
     @classmethod
```

### Comparing `nista_library-3.0.6/data_point_client/models/time_series_period.py` & `nista_library-4.0.0/data_point_client/models/time_series_period.py`

 * *Files identical despite different names*

### Comparing `nista_library-3.0.6/data_point_client/models/time_series_response.py` & `nista_library-4.0.0/data_point_client/models/time_series_response.py`

 * *Files identical despite different names*

### Comparing `nista_library-3.0.6/data_point_client/models/time_series_response_curve.py` & `nista_library-4.0.0/data_point_client/models/time_series_response_curve.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 @attr.s(auto_attribs=True)
 class TimeSeriesResponseCurve:
     """ """
 
     additional_properties: Dict[str, float] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
 
         return field_dict
 
     @classmethod
```

### Comparing `nista_library-3.0.6/data_point_client/models/update_constant_data_request.py` & `nista_library-4.0.0/data_point_client/models/update_constant_data_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-3.0.6/data_point_client/models/update_day_period_request.py` & `nista_library-4.0.0/data_point_client/models/update_day_period_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-3.0.6/data_point_client/models/update_time_series_request.py` & `nista_library-4.0.0/data_point_client/models/update_time_series_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,20 +15,24 @@
 class UpdateTimeSeriesRequest:
     """
     Attributes:
         execution_id (Union[Unset, None, str]):
         sub_series (Union[Unset, None, List['SubSeriesRequest']]):
         warnings (Union[Unset, None, List[str]]):
         unit (Union[Unset, None, str]):
+        force_unit (Union[Unset, bool]):
+        time_zone (Union[Unset, None, str]):
     """
 
     execution_id: Union[Unset, None, str] = UNSET
     sub_series: Union[Unset, None, List["SubSeriesRequest"]] = UNSET
     warnings: Union[Unset, None, List[str]] = UNSET
     unit: Union[Unset, None, str] = UNSET
+    force_unit: Union[Unset, bool] = UNSET
+    time_zone: Union[Unset, None, str] = UNSET
 
     def to_dict(self) -> Dict[str, Any]:
         execution_id = self.execution_id
         sub_series: Union[Unset, None, List[Dict[str, Any]]] = UNSET
         if not isinstance(self.sub_series, Unset):
             if self.sub_series is None:
                 sub_series = None
@@ -43,25 +47,31 @@
         if not isinstance(self.warnings, Unset):
             if self.warnings is None:
                 warnings = None
             else:
                 warnings = self.warnings
 
         unit = self.unit
+        force_unit = self.force_unit
+        time_zone = self.time_zone
 
         field_dict: Dict[str, Any] = {}
         field_dict.update({})
         if execution_id is not UNSET:
             field_dict["executionId"] = execution_id
         if sub_series is not UNSET:
             field_dict["subSeries"] = sub_series
         if warnings is not UNSET:
             field_dict["warnings"] = warnings
         if unit is not UNSET:
             field_dict["unit"] = unit
+        if force_unit is not UNSET:
+            field_dict["forceUnit"] = force_unit
+        if time_zone is not UNSET:
+            field_dict["timeZone"] = time_zone
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.sub_series_request import SubSeriesRequest
 
@@ -75,15 +85,21 @@
 
             sub_series.append(sub_series_item)
 
         warnings = cast(List[str], d.pop("warnings", UNSET))
 
         unit = d.pop("unit", UNSET)
 
+        force_unit = d.pop("forceUnit", UNSET)
+
+        time_zone = d.pop("timeZone", UNSET)
+
         update_time_series_request = cls(
             execution_id=execution_id,
             sub_series=sub_series,
             warnings=warnings,
             unit=unit,
+            force_unit=force_unit,
+            time_zone=time_zone,
         )
 
         return update_time_series_request
```

### Comparing `nista_library-3.0.6/data_point_client/models/update_week_period_request.py` & `nista_library-4.0.0/data_point_client/models/update_week_period_request.py`

 * *Files identical despite different names*

### Comparing `nista_library-3.0.6/data_point_client/models/week_data_transfere.py` & `nista_library-4.0.0/data_point_client/models/week_data_transfere.py`

 * *Files identical despite different names*

### Comparing `nista_library-3.0.6/data_point_client/models/week_period_data_bucket.py` & `nista_library-4.0.0/data_point_client/models/week_period_data_bucket.py`

 * *Files identical despite different names*

### Comparing `nista_library-3.0.6/data_point_client/models/week_period_data_point_data.py` & `nista_library-4.0.0/data_point_client/models/week_period_data_point_data.py`

 * *Files identical despite different names*

### Comparing `nista_library-3.0.6/data_point_client/types.py` & `nista_library-4.0.0/data_point_client/types.py`

 * *Files identical despite different names*

### Comparing `nista_library-3.0.6/nista_library/__init__.py` & `nista_library-4.0.0/nista_library/__init__.py`

 * *Files identical despite different names*

### Comparing `nista_library-3.0.6/nista_library/nista_connetion.py` & `nista_library-4.0.0/nista_library/nista_connetion.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
                 client_id=self.client_id, client_secret=self.client_secret, scope=self.scope
             )
         else:
             log.info("Auth Code Flow")
             self._create_tokens_code_flow()
 
         if self.access_token is None:
-            raise Exception("No Token available")
+            raise ValueError("No Token available")
 
         return self.access_token
 
     def _get_service_info(
         self, scope: Optional[list] = None, client_id: str = "python", client_secret: Optional[str] = None
     ) -> ServiceInformation:
         if scope is None:
```

### Comparing `nista_library-3.0.6/nista_library/nista_credential_manager.py` & `nista_library-4.0.0/nista_library/nista_credential_manager.py`

 * *Files identical despite different names*

### Comparing `nista_library-3.0.6/nista_library/nista_data_point.py` & `nista_library-4.0.0/nista_library/nista_data_point.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 import uuid
 from typing import Any, List, Optional, Type, TypeVar, Union
 
 import pandas as pd
 from pandas import DataFrame
 from structlog import get_logger
+from zoneinfo import ZoneInfo
 
 from data_point_client import AuthenticatedClient
 from data_point_client.api.data_point import (
     data_point_append_execution_result_data,
     data_point_append_time_series_data,
     data_point_create_data_point,
     data_point_get_data,
@@ -45,15 +46,15 @@
 
 class NistaDataPoint:
     DATE_FORMAT = "%Y-%m-%dT%H:%M:%SZ"
     DATE_NAME = "Date"
     VALUE_NAME = "Value"
 
     @classmethod
-    def create_new(cls: Type[T], connection: NistaConnection, name: str, tags: List[str]) -> Union[T, None]:
+    def create_new(cls: Type[T], connection: NistaConnection, name: str, tags: List[str]) -> Optional[T]:
         token = connection.get_access_token()
         client = AuthenticatedClient(
             base_url=connection.datapoint_base_url, token=token, verify_ssl=connection.verify_ssl
         )
 
         new_id = uuid.uuid4()
         request = DataPointRequest(name=name, description="", existence=EnDataPointExistenceDTO.FULL, tags=tags)
@@ -89,20 +90,25 @@
         data_point = data_point_get_data_point.sync(
             client=client,
             data_point_id=self.data_point_id,
             workspace_id=self.connection.workspace_id,
         )
 
         if data_point is None:
-            raise Exception("Cannot load Datapoint")
-        self.name = data_point.name
+            raise ValueError("Cannot load Datapoint")
+
+        self.name = data_point.names
+        self.data_point_response = data_point
 
     # pylint: disable=too-many-arguments
     def get_data_point_data(
-        self, request: GetDataRequest, post_fix: bool = False, timeout: float = 30
+        self,
+        request: GetDataRequest,
+        post_fix: bool = False,
+        timeout: float = 30,
     ) -> Union[List[DataFrame], float, Unset, WeekDataTransfere, DayDataByHourTransfer, None]:
         token = self.connection.get_access_token()
         client = AuthenticatedClient(
             base_url=self.connection.datapoint_base_url,
             token=token,
             verify_ssl=self.connection.verify_ssl,
             timeout=timeout,
@@ -119,15 +125,14 @@
 
         content_text = byte_content.decode("utf-8")
         jscon_content = json.loads(content_text)
 
         content_type = jscon_content["discriminator"]
 
         if content_type == "GetSeriesResponse":
-
             series_response = GetSeriesResponse.from_dict(jscon_content)
             curves = series_response.curves
 
             if isinstance(curves, list):
                 data_frames = []
                 # pylint: disable=E1133
                 for curve in curves:
@@ -153,16 +158,16 @@
             day_response = GetDayPeriodResponse.from_dict(jscon_content)
             if day_response is not None:
                 return day_response.day_data
 
         return None
 
     def append_data_point_data(
-        self, data: Union[List[DataFrame], float], unit: Union[str, None], timeout: float = 5.0
-    ) -> Union[Response[Union[Any, ProblemDetails]], None]:
+        self, data: Union[List[DataFrame], float], unit: Optional[str] = None, timeout: float = 5.0
+    ) -> Optional[Response[Union[Any, ProblemDetails]]]:
         token = self.connection.get_access_token()
         client = AuthenticatedClient(
             base_url=self.connection.datapoint_base_url,
             token=token,
             verify_ssl=self.connection.verify_ssl,
             timeout=timeout,
         )
@@ -183,16 +188,16 @@
                 data_point_id=str(self.data_point_id),
                 json_body=append_request,
             )
 
         return None
 
     def append_data_point_result_parts(
-        self, data: Union[List[DataFrame], float], unit: Union[str, None], execution_id: uuid.UUID, timeout: float = 5.0
-    ) -> Union[Response[Union[Any, ProblemDetails]], None]:
+        self, data: Union[List[DataFrame], float], unit: Optional[str], execution_id: uuid.UUID, timeout: float = 5.0
+    ) -> Optional[Response[Union[Any, ProblemDetails]]]:
         token = self.connection.get_access_token()
         client = AuthenticatedClient(
             base_url=self.connection.datapoint_base_url,
             token=token,
             verify_ssl=self.connection.verify_ssl,
             timeout=timeout,
         )
@@ -217,17 +222,18 @@
             )
 
         return None
 
     def set_data_point_data(
         self,
         data: Union[List[DataFrame], float, WeekDataTransfere],
-        unit: Union[str, None],
-        execution_id: Union[str, None],
-    ) -> Union[Response[Union[Any, ProblemDetails]], None]:
+        unit: Optional[str] = None,
+        execution_id: Optional[str] = None,
+        time_zone: Optional[ZoneInfo] = None,
+    ) -> Optional[Response[Union[Any, ProblemDetails]]]:
         token = self.connection.get_access_token()
         client = AuthenticatedClient(
             base_url=self.connection.datapoint_base_url, token=token, verify_ssl=self.connection.verify_ssl
         )
 
         if isinstance(data, WeekDataTransfere):
             week_update_request = UpdateWeekPeriodRequest(execution_id=execution_id, unit=unit, week_data=data)
@@ -236,22 +242,28 @@
                 client=client,
                 data_point_id=str(self.data_point_id),
                 json_body=week_update_request,
             )
 
         if isinstance(data, list):
             sub_series: List[SubSeriesRequest] = []
+            if time_zone is None:
+                time_zone = ZoneInfo("UTC")
+
             for data_frame in data:
                 data_dict = self._to_dict(data_frame)
                 value = SubSeriesRequestValues.from_dict(src_dict=data_dict)
                 request = SubSeriesRequest(values=value)
                 sub_series.append(request)
 
             timeseries_update_request = UpdateTimeSeriesRequest(
-                sub_series=sub_series, unit=unit, execution_id=execution_id
+                sub_series=sub_series,
+                unit=unit,
+                execution_id=execution_id,
+                time_zone=time_zone.key,
             )
 
             return data_point_update_time_series_data.sync_detailed(
                 workspace_id=self.connection.workspace_id,
                 client=client,
                 data_point_id=str(self.data_point_id),
                 json_body=timeseries_update_request,
@@ -279,15 +291,14 @@
         for key in dct.keys():
             value = dct[key]
             key_string = key.strftime(self.DATE_FORMAT)
             result[key_string] = value
         return result
 
     def _from_time_frames(self, time_frames: dict, post_fix: bool, date_format: str = DATE_FORMAT) -> DataFrame:
-
         if not isinstance(time_frames, dict):
             raise TypeError
 
         value_column_name = self.name
 
         if value_column_name is None:
             value_column_name = self.VALUE_NAME
```

### Comparing `nista_library-3.0.6/nista_library/nista_data_points.py` & `nista_library-4.0.0/nista_library/nista_data_points.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         )
 
         data_point_list = data_point_get_data_points.sync(
             workspace_id=self.connection.workspace_id, client=client, existence=[EnDataPointExistenceDTO.FULL]
         )
         if isinstance(data_point_list, ProblemDetails):
             problems: ProblemDetails = data_point_list
-            raise Exception(problems)
+            raise ValueError(problems)
 
         if isinstance(data_point_list, list):
             list_of_data_points: List[DataPointResponseBase] = data_point_list
 
         for data_point in list_of_data_points:
             name: Optional[str] = None
             if isinstance(data_point.name, str):
```

### Comparing `nista_library-3.0.6/pyproject.toml` & `nista_library-4.0.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nista-library"
-version = "3.0.6"
+version = "4.0.0"
 description = "A client library for accessing nista.io"
 license = "MIT"
 
 authors = ["Markus Hoffmann <markus.hoffmann@nista.io>"]
 
 readme = "README.md"
 homepage = "https://nista.io"
@@ -14,15 +14,15 @@
     {include = "data_point_client"},
     {include = "nista_library"},
 ]
 include = ["LICENSE.md", "data_point_client/py.typed"]
 
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
+python = ">=3.9,<3.11"
 httpx = ">=0.15.4,<1.0.0"
 attrs = ">=20.1.0,<23.0.0"
 python-dateutil = "^2.8.0"
 pandas = "^1.3.2"
 oauth2-client = "^1.2.1"
 PyJWT = "^2.3.0"
 structlog = ">=21.0.0,<22.0.0"
@@ -33,15 +33,15 @@
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 mypy = "<1.0"
 flake8 = "<6.0.0"
 pylint = "<3.0.0"
 black = "<23.0.0"
-openapi-python-client = "^0.11.1"
+openapi-python-client = "<0.14.0"
 typer = "^0.4.1"
 
 [tool.poetry.group.dev.dependencies]
 black = {version = "^22.10.0", allow-prereleases = true}
 
 [tool.black]
 line-length = 120
```

### Comparing `nista_library-3.0.6/setup.py` & `nista_library-4.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,170 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nista-library
+Version: 4.0.0
+Summary: A client library for accessing nista.io
+Home-page: https://nista.io
+License: MIT
+Author: Markus Hoffmann
+Author-email: markus.hoffmann@nista.io
+Requires-Python: >=3.9,<3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: PyJWT (>=2.3.0,<3.0.0)
+Requires-Dist: attrs (>=20.1.0,<23.0.0)
+Requires-Dist: colorama (>=0.4.4,<0.5.0)
+Requires-Dist: httpx (>=0.15.4,<1.0.0)
+Requires-Dist: keyring (>=23.5.0,<24.0.0)
+Requires-Dist: oauth2-client (>=1.2.1,<2.0.0)
+Requires-Dist: pandas (>=1.3.2,<2.0.0)
+Requires-Dist: pyjwt (>=2.6.0,<3.0.0)
+Requires-Dist: python-dateutil (>=2.8.0,<3.0.0)
+Requires-Dist: structlog (>=21.0.0,<22.0.0)
+Project-URL: Repository, https://gitlab.com/campfiresolutions/public/nista.io-python-library.git
+Description-Content-Type: text/markdown
 
-packages = \
-['data_point_client',
- 'data_point_client.api',
- 'data_point_client.api.data_export',
- 'data_point_client.api.data_point',
- 'data_point_client.models',
- 'nista_library']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['PyJWT>=2.3.0,<3.0.0',
- 'attrs>=20.1.0,<23.0.0',
- 'colorama>=0.4.4,<0.5.0',
- 'httpx>=0.15.4,<1.0.0',
- 'keyring>=23.5.0,<24.0.0',
- 'oauth2-client>=1.2.1,<2.0.0',
- 'pandas>=1.3.2,<2.0.0',
- 'pyjwt>=2.6.0,<3.0.0',
- 'python-dateutil>=2.8.0,<3.0.0',
- 'structlog>=21.0.0,<22.0.0']
-
-setup_kwargs = {
-    'name': 'nista-library',
-    'version': '3.0.6',
-    'description': 'A client library for accessing nista.io',
-    'long_description': '[![Gitlab Pipeline](https://gitlab.com/campfiresolutions/public/nista.io-python-library/badges/main/pipeline.svg)](https://gitlab.com/campfiresolutions/public/nista.io-python-library/-/pipelines) [![Python Version](https://img.shields.io/pypi/pyversions/nista-library)](https://pypi.org/project/nista-library/) [![PyPI version](https://img.shields.io/pypi/v/nista-library)](https://pypi.org/project/nista-library/) [![License](https://img.shields.io/pypi/l/nista-library)](https://pypi.org/project/nista-library/) [![Downloads](https://img.shields.io/pypi/dm/nista-library)](https://pypi.org/project/nista-library/)\n\n# nista-library\n\nA client library for accessing nista.io\n\n## Tutorial\n\n### Create new Poetry Project\n\nNavigate to a folder where you want to create your project and type\n\n```shell\npoetry new my-nista-client\ncd my-nista-client\n```\n\n### Add reference to your Project\n\nNavigate to the newly created project and add the PyPI package\n\n```shell\npoetry add nista-library\n```\n\n### Your first DataPoint\n\nCreate a new file you want to use to receive data this demo.py\n\n```python\nfrom nista_library import KeyringNistaConnection, NistaDataPoint, NistaDataPoints\n\nconnection = KeyringNistaConnection()\n\ndata_point_id = "56c5c6ff-3f7d-4532-8fbf-a3795f7b48b8"\ndata_point = NistaDataPoint(connection=connection, data_point_id=data_point_id)\n\ndata_point_data = data_point.get_data_point_data()\n\nprint(data_point_data)\n```\n\nYou need to replace the `DataPointId` with an ID from your nista.io workspace.\n\nFor example the DataPointId of this DataPoint `https://aws.nista.io/secured/dashboard/datapoint/4684d681-8728-4f59-aeb0-ac3f3c573303` is `4684d681-8728-4f59-aeb0-ac3f3c573303`\n\n### Run and Login\n\nRun your file in poetry\'s virtual environment\n\n```console\n$ poetry run python demo.py\n2021-09-02 14:51.58 [info     ] Authentication has been started. Please follow the link to authenticate with your user: [nista_library.nista_connetion] url=https://aws.nista.io/authentication/connect/authorize?client_id=python&redirect_uri=http%3A%2F%2Flocalhost%3A4200%2Fhome&response_type=code&scope=data-api%20openid%20profile%20offline_access&state=myState\n```\n\nIn order to login copy the `url` into your Browser and Login to nista.io or, if allowed a browser window will open by itself.\n\n### Keystore\n\nOnce you loggedin, the library will try to store your access token in your private keystore. Next time you run your programm, it might request a password to access your keystore again to gain access to nista.io\nPlease take a look at [Keyring](https://pypi.org/project/keyring/) for details.\n\n## Advanced Example\n\n### Show received Data in a plot\n\n```shell\npoetry new my-nista-client\ncd my-nista-client\npoetry add nista-library\npoetry add structlib\npoetry add matplotlib\n```\n\n```python\nimport matplotlib.pyplot as plt\nfrom structlog import get_logger\n\nfrom nista_library import KeyringNistaConnection, NistaDataPoint, NistaDataPoints\n\nlog = get_logger()\n\nconnection = KeyringNistaConnection()\n\ndata_point_id = "56c5c6ff-3f7d-4532-8fbf-a3795f7b48b8"\ndata_point = NistaDataPoint(connection=connection, data_point_id=data_point_id)\n\ndata_point_data = data_point.get_data_point_data()\nlog.info("Data has been received. Plotting")\ndata_point_data.plot()\nplt.show()\n\n```\n\n### Filter by DataPoint Names\n\n```shell\npoetry new my-nista-client\ncd my-nista-client\npoetry add nista-library\npoetry add structlib\npoetry add matplotlib\n```\n\n```python\nimport matplotlib.pyplot as plt\nfrom structlog import get_logger\n\nfrom nista_library import KeyringNistaConnection, NistaDataPoint, NistaDataPoints\n\nlog = get_logger()\n\nconnection = KeyringNistaConnection()\n\ndataPoints = NistaDataPoints(connection=connection)\ndata_point_list = list(dataPoints.get_data_point_list())\n\nfor data_point in data_point_list:\n    log.info(data_point)\n\n# Find Specific Data Points\nfiltered_data_points = filter(\n    lambda data_point: data_point.name.startswith("371880214002"), data_point_list\n)\nfor data_point in filtered_data_points:\n    # get the data\n    data_point_data = data_point.get_data_point_data()\n    log.info(data_point_data)\n    data_point_data.plot()\n    plt.show()\n\n```\n\n## Links\n\n**Website**\n[![nista.io](https://www.nista.io/assets/images/nista-logo-small.svg)](nista.io)\n\n**PyPi**\n[![PyPi](https://pypi.org/static/images/logo-small.95de8436.svg)](https://pypi.org/project/nista-library/)\n\n**GIT Repository**\n[![Gitlab](https://about.gitlab.com/images/icons/logos/slp-logo.svg)](https://gitlab.com/campfiresolutions/public/nista.io-python-library)\n',
-    'author': 'Markus Hoffmann',
-    'author_email': 'markus.hoffmann@nista.io',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://nista.io',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.11',
-}
+[![Gitlab Pipeline](https://gitlab.com/campfiresolutions/public/nista.io-python-library/badges/main/pipeline.svg)](https://gitlab.com/campfiresolutions/public/nista.io-python-library/-/pipelines) [![Python Version](https://img.shields.io/pypi/pyversions/nista-library)](https://pypi.org/project/nista-library/) [![PyPI version](https://img.shields.io/pypi/v/nista-library)](https://pypi.org/project/nista-library/) [![License](https://img.shields.io/pypi/l/nista-library)](https://pypi.org/project/nista-library/) [![Downloads](https://img.shields.io/pypi/dm/nista-library)](https://pypi.org/project/nista-library/)
 
+# nista-library
+
+A client library for accessing nista.io
+
+## Tutorial
+
+### Create new Poetry Project
+
+Navigate to a folder where you want to create your project and type
+
+```shell
+poetry new my-nista-client
+cd my-nista-client
+```
+
+### Add reference to your Project
+
+Navigate to the newly created project and add the PyPI package
+
+```shell
+poetry add nista-library
+```
+
+### Your first DataPoint
+
+Create a new file you want to use to receive data this demo.py
+
+```python
+from nista_library import KeyringNistaConnection, NistaDataPoint, NistaDataPoints
+
+connection = KeyringNistaConnection()
+
+data_point_id = "56c5c6ff-3f7d-4532-8fbf-a3795f7b48b8"
+data_point = NistaDataPoint(connection=connection, data_point_id=data_point_id)
+
+data_point_data = data_point.get_data_point_data()
+
+print(data_point_data)
+```
+
+You need to replace the `DataPointId` with an ID from your nista.io workspace.
+
+For example the DataPointId of this DataPoint `https://aws.nista.io/secured/dashboard/datapoint/4684d681-8728-4f59-aeb0-ac3f3c573303` is `4684d681-8728-4f59-aeb0-ac3f3c573303`
+
+### Run and Login
+
+Run your file in poetry's virtual environment
+
+```console
+$ poetry run python demo.py
+2021-09-02 14:51.58 [info     ] Authentication has been started. Please follow the link to authenticate with your user: [nista_library.nista_connetion] url=https://aws.nista.io/authentication/connect/authorize?client_id=python&redirect_uri=http%3A%2F%2Flocalhost%3A4200%2Fhome&response_type=code&scope=data-api%20openid%20profile%20offline_access&state=myState
+```
+
+In order to login copy the `url` into your Browser and Login to nista.io or, if allowed a browser window will open by itself.
+
+### Keystore
+
+Once you loggedin, the library will try to store your access token in your private keystore. Next time you run your programm, it might request a password to access your keystore again to gain access to nista.io
+Please take a look at [Keyring](https://pypi.org/project/keyring/) for details.
+
+## Advanced Example
+
+### Show received Data in a plot
+
+```shell
+poetry new my-nista-client
+cd my-nista-client
+poetry add nista-library
+poetry add structlib
+poetry add matplotlib
+```
+
+```python
+import matplotlib.pyplot as plt
+from structlog import get_logger
+
+from nista_library import KeyringNistaConnection, NistaDataPoint, NistaDataPoints
+
+log = get_logger()
+
+connection = KeyringNistaConnection()
+
+data_point_id = "56c5c6ff-3f7d-4532-8fbf-a3795f7b48b8"
+data_point = NistaDataPoint(connection=connection, data_point_id=data_point_id)
+
+data_point_data = data_point.get_data_point_data()
+log.info("Data has been received. Plotting")
+data_point_data.plot()
+plt.show()
+
+```
+
+### Filter by DataPoint Names
+
+```shell
+poetry new my-nista-client
+cd my-nista-client
+poetry add nista-library
+poetry add structlib
+poetry add matplotlib
+```
+
+```python
+import matplotlib.pyplot as plt
+from structlog import get_logger
+
+from nista_library import KeyringNistaConnection, NistaDataPoint, NistaDataPoints
+
+log = get_logger()
+
+connection = KeyringNistaConnection()
+
+dataPoints = NistaDataPoints(connection=connection)
+data_point_list = list(dataPoints.get_data_point_list())
+
+for data_point in data_point_list:
+    log.info(data_point)
+
+# Find Specific Data Points
+filtered_data_points = filter(
+    lambda data_point: data_point.name.startswith("371880214002"), data_point_list
+)
+for data_point in filtered_data_points:
+    # get the data
+    data_point_data = data_point.get_data_point_data()
+    log.info(data_point_data)
+    data_point_data.plot()
+    plt.show()
+
+```
+
+## Links
+
+**Website**
+[![nista.io](https://www.nista.io/assets/images/nista-logo-small.svg)](nista.io)
+
+**PyPi**
+[![PyPi](https://pypi.org/static/images/logo-small.95de8436.svg)](https://pypi.org/project/nista-library/)
+
+**GIT Repository**
+[![Gitlab](https://about.gitlab.com/images/icons/logos/slp-logo.svg)](https://gitlab.com/campfiresolutions/public/nista.io-python-library)
 
-setup(**setup_kwargs)
```

