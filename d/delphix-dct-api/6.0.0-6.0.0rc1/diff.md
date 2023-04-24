# Comparing `tmp/delphix-dct-api-6.0.0.tar.gz` & `tmp/delphix-dct-api-6.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delphix-dct-api-6.0.0.tar", last modified: Wed Mar 29 09:14:04 2023, max compression
+gzip compressed data, was "delphix-dct-api-6.0.0rc1.tar", last modified: Fri Mar 24 10:11:33 2023, max compression
```

## Comparing `delphix-dct-api-6.0.0.tar` & `delphix-dct-api-6.0.0rc1.tar`

### file list

```diff
@@ -1,635 +1,635 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-29 09:14:04.774996 delphix-dct-api-6.0.0/
--rw-r--r--   0 runner    (1001) docker     (116)      269 2023-03-29 09:14:04.774996 delphix-dct-api-6.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    64624 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-29 09:14:04.694995 delphix-dct-api-6.0.0/delphix/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-29 09:14:04.694995 delphix-dct-api-6.0.0/delphix/api/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-29 09:14:04.694995 delphix-dct-api-6.0.0/delphix/api/gateway/
--rw-r--r--   0 runner    (1001) docker     (116)      756 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-29 09:14:04.698995 delphix-dct-api-6.0.0/delphix/api/gateway/api/
--rw-r--r--   0 runner    (1001) docker     (116)      224 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    65198 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/api/accounts_api.py
--rw-r--r--   0 runner    (1001) docker     (116)   173762 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/api/authorization_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    54762 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/api/bookmarks_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    34507 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/api/cdbs_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     5650 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/api/connectivity_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    44574 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/api/connectors_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    56971 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/api/d_sources_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    58964 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/api/database_templates_api.py
--rw-r--r--   0 runner    (1001) docker     (116)   109504 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/api/environments_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    27195 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/api/executions_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    20449 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/api/groups_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    39107 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/api/jobs_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     9677 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/api/login_api.py
--rw-r--r--   0 runner    (1001) docker     (116)   138683 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/api/management_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    80140 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/api/masking_jobs_api.py
--rw-r--r--   0 runner    (1001) docker     (116)   116463 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/api/reporting_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     4690 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/api/saml_login_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    54724 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/api/snapshots_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    35881 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/api/sources_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     5352 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/api/test_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    51542 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/api/timeflows_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    35334 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/api/vcdbs_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    69811 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/api/vdb_groups_api.py
--rw-r--r--   0 runner    (1001) docker     (116)   144626 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/api/vdbs_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    20856 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/api/virtualization_policies_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    36847 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-29 09:14:04.698995 delphix-dct-api-6.0.0/delphix/api/gateway/apis/
--rw-r--r--   0 runner    (1001) docker     (116)     1998 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    16979 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/configuration.py
--rw-r--r--   0 runner    (1001) docker     (116)     5038 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-29 09:14:04.734995 delphix-dct-api-6.0.0/delphix/api/gateway/model/
--rw-r--r--   0 runner    (1001) docker     (116)      348 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    13907 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/access_group.py
--rw-r--r--   0 runner    (1001) docker     (116)    11286 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/access_group_account_ids_request.py
--rw-r--r--   0 runner    (1001) docker     (116)    15309 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/access_group_scope.py
--rw-r--r--   0 runner    (1001) docker     (116)    11448 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/access_group_scopes_request.py
--rw-r--r--   0 runner    (1001) docker     (116)    11198 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/access_group_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    15588 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/account.py
--rw-r--r--   0 runner    (1001) docker     (116)    16533 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/account_create_parameter.py
--rw-r--r--   0 runner    (1001) docker     (116)    14295 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/account_create_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11734 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/account_login_parameter.py
--rw-r--r--   0 runner    (1001) docker     (116)    14723 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/account_update_parameter.py
--rw-r--r--   0 runner    (1001) docker     (116)    12275 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/additional_mount_point.py
--rw-r--r--   0 runner    (1001) docker     (116)    11372 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/all_object_permissions_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11798 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/always_allowed_permission.py
--rw-r--r--   0 runner    (1001) docker     (116)    11833 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/always_allowed_permission_request.py
--rw-r--r--   0 runner    (1001) docker     (116)    11804 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/api_classification_config.py
--rw-r--r--   0 runner    (1001) docker     (116)    12702 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/api_classification_object.py
--rw-r--r--   0 runner    (1001) docker     (116)    13192 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/api_usage_data.py
--rw-r--r--   0 runner    (1001) docker     (116)    12106 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/api_usage_report_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    45609 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/base_provision_vdb_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    38003 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/base_provision_vdb_parameters_all_of.py
--rw-r--r--   0 runner    (1001) docker     (116)    13815 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/bookmark.py
--rw-r--r--   0 runner    (1001) docker     (116)    14458 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/bookmark_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    13327 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/cdb.py
--rw-r--r--   0 runner    (1001) docker     (116)    12076 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/change_password_parameter.py
--rw-r--r--   0 runner    (1001) docker     (116)    11932 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/connectivity_check_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    11247 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/connectivity_check_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    13356 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/connector.py
--rw-r--r--   0 runner    (1001) docker     (116)    11637 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/connector_test_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    12418 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/connector_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    12487 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/copy_masking_job_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    11409 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/copy_masking_job_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11491 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/create_bookmark_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11617 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/create_database_template_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11482 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/create_environment_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11494 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/create_environment_user_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11476 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/create_host_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    12373 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/create_role.py
--rw-r--r--   0 runner    (1001) docker     (116)    12549 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/create_vdb_group_request.py
--rw-r--r--   0 runner    (1001) docker     (116)    11247 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/create_vdb_group_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    17279 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/d_source.py
--rw-r--r--   0 runner    (1001) docker     (116)    13076 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/d_source_consumption_data.py
--rw-r--r--   0 runner    (1001) docker     (116)    11839 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/d_source_consumption_report_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    19622 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/d_source_snapshot_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    12945 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/d_source_usage_data.py
--rw-r--r--   0 runner    (1001) docker     (116)    11779 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/d_source_usage_report_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11434 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/data_point_by_snapshot_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    12272 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/data_point_by_timestamp_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    11490 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/data_point_from_bookmark_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    13058 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/database_template.py
--rw-r--r--   0 runner    (1001) docker     (116)    13463 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/database_template_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    12210 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/dataset_group.py
--rw-r--r--   0 runner    (1001) docker     (116)    11205 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/delete_database_template_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11175 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/delete_engine_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11190 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/delete_environment_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11202 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/delete_environment_user_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11169 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/delete_host_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11187 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/delete_masking_job_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11384 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/delete_scope_object_tags.py
--rw-r--r--   0 runner    (1001) docker     (116)    11528 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/delete_scoped_object_item.py
--rw-r--r--   0 runner    (1001) docker     (116)    11181 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/delete_snapshot_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11910 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/delete_tag.py
--rw-r--r--   0 runner    (1001) docker     (116)    11181 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/delete_timeflow_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11260 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/delete_vdb_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    11166 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/delete_vdb_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11193 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/disable_environment_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11333 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/disable_vdb_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    11169 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/disable_vdb_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    15475 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/domain.py
--rw-r--r--   0 runner    (1001) docker     (116)    11317 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/effective_scope.py
--rw-r--r--   0 runner    (1001) docker     (116)    11190 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/enable_environment_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11316 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/enable_vdb_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    11166 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/enable_vdb_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    16724 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/engine.py
--rw-r--r--   0 runner    (1001) docker     (116)    11106 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/engine_id_body.py
--rw-r--r--   0 runner    (1001) docker     (116)    21137 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/engine_registration_parameter.py
--rw-r--r--   0 runner    (1001) docker     (116)    15110 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/environment.py
--rw-r--r--   0 runner    (1001) docker     (116)    29606 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/environment_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    20313 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/environment_repository.py
--rw-r--r--   0 runner    (1001) docker     (116)    11149 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/environment_repository_all_of.py
--rw-r--r--   0 runner    (1001) docker     (116)    17594 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/environment_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    13401 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/environment_user.py
--rw-r--r--   0 runner    (1001) docker     (116)    15622 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/environment_user_params.py
--rw-r--r--   0 runner    (1001) docker     (116)    11530 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/error.py
--rw-r--r--   0 runner    (1001) docker     (116)    11592 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/error_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    12594 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/errors.py
--rw-r--r--   0 runner    (1001) docker     (116)    11327 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/execute_masking_job_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    11190 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/execute_masking_job_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    16753 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/execution.py
--rw-r--r--   0 runner    (1001) docker     (116)    11526 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/execution_cancel_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    11305 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/global_properties.py
--rw-r--r--   0 runner    (1001) docker     (116)    13015 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/hashicorp_vault.py
--rw-r--r--   0 runner    (1001) docker     (116)    12332 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/hook.py
--rw-r--r--   0 runner    (1001) docker     (116)    20772 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/host.py
--rw-r--r--   0 runner    (1001) docker     (116)    18094 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/host_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    18866 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/host_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    13953 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/job.py
--rw-r--r--   0 runner    (1001) docker     (116)    17452 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/ldap_config_params.py
--rw-r--r--   0 runner    (1001) docker     (116)    11740 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/ldap_config_validate_parameter.py
--rw-r--r--   0 runner    (1001) docker     (116)    11192 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/ldap_validate_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11221 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/link_d_source_default_request.py
--rw-r--r--   0 runner    (1001) docker     (116)    29530 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/link_d_source_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    11428 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/link_d_source_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11736 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/list_access_groups_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11695 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/list_accounts_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11738 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/list_bookmarks_by_vdb_groups_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11705 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/list_bookmarks_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11655 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/list_cdbs_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11715 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/list_connectors_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11982 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/list_d_sources_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11786 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/list_database_templates_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11306 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/list_environment_users.py
--rw-r--r--   0 runner    (1001) docker     (116)    12021 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/list_environments_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11715 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/list_executions_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11725 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/list_groups_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11766 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/list_hashicorp_vaults_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11941 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/list_jobs_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11848 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/list_masking_job_source_engines_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11726 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/list_masking_jobs_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11786 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/list_registered_engines_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11793 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/list_reporting_schedule_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11189 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/list_roles_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11705 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/list_snapshots_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11971 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/list_sources_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11705 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/list_timeflows_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11665 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/list_vcdbs_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11736 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/list_vdb_groups_by_bookmark_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11706 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/list_vdb_groups_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11941 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/list_vdbs_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11829 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/list_virtualization_policies_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    12897 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/login_token.py
--rw-r--r--   0 runner    (1001) docker     (116)    15504 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/masking_job.py
--rw-r--r--   0 runner    (1001) docker     (116)    11547 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/masking_job_connectors_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11515 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/masking_job_source_engine.py
--rw-r--r--   0 runner    (1001) docker     (116)    12238 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/masking_ruleset.py
--rw-r--r--   0 runner    (1001) docker     (116)    14855 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/metadata_db_info.py
--rw-r--r--   0 runner    (1001) docker     (116)    12496 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/migrate_masking_job_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    11190 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/migrate_masking_job_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11654 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/object_permission_access_groups.py
--rw-r--r--   0 runner    (1001) docker     (116)    12454 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/object_permission_account.py
--rw-r--r--   0 runner    (1001) docker     (116)    11445 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/object_permissions_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    13606 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/object_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (116)    12735 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/object_type_property.py
--rw-r--r--   0 runner    (1001) docker     (116)    12879 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/oracle_listener.py
--rw-r--r--   0 runner    (1001) docker     (116)    11388 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/oracle_rac_custom_env_file.py
--rw-r--r--   0 runner    (1001) docker     (116)    11700 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/oracle_rac_custom_env_var.py
--rw-r--r--   0 runner    (1001) docker     (116)    11730 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/oracle_virtual_ip.py
--rw-r--r--   0 runner    (1001) docker     (116)    12321 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/paginated_response_metadata.py
--rw-r--r--   0 runner    (1001) docker     (116)    14496 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/password_policies_params.py
--rw-r--r--   0 runner    (1001) docker     (116)    14622 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/permission_enum.py
--rw-r--r--   0 runner    (1001) docker     (116)    16832 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/permission_object.py
--rw-r--r--   0 runner    (1001) docker     (116)    12857 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/permission_property.py
--rw-r--r--   0 runner    (1001) docker     (116)    11693 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/permissions_request.py
--rw-r--r--   0 runner    (1001) docker     (116)    11205 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/primary_environment_user_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11371 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/product_history.py
--rw-r--r--   0 runner    (1001) docker     (116)    12286 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/product_info.py
--rw-r--r--   0 runner    (1001) docker     (116)    11514 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/provision_vdb_from_bookmark_defaults_request.py
--rw-r--r--   0 runner    (1001) docker     (116)    46983 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/provision_vdb_from_bookmark_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    11489 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/provision_vdb_from_bookmark_parameters_all_of.py
--rw-r--r--   0 runner    (1001) docker     (116)    13978 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/provision_vdb_group_from_bookmark_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    11542 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/provision_vdb_group_from_bookmark_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11427 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/provision_vdb_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    12560 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/provision_vdbby_snapshot_defaults_request.py
--rw-r--r--   0 runner    (1001) docker     (116)    48436 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/provision_vdbby_snapshot_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    12879 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/provision_vdbby_snapshot_parameters_all_of.py
--rw-r--r--   0 runner    (1001) docker     (116)    13636 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/provision_vdbby_timestamp_defaults_request.py
--rw-r--r--   0 runner    (1001) docker     (116)    49076 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/provision_vdbby_timestamp_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    12826 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/provision_vdbby_timestamp_parameters_all_of.py
--rw-r--r--   0 runner    (1001) docker     (116)    11193 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/refresh_environment_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    13623 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/refresh_vdb_from_bookmark_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    11205 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/refresh_vdb_from_bookmark_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11366 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/refresh_vdb_group_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    11184 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/refresh_vdb_group_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    12305 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/refresh_vdbby_location_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    11199 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/refresh_vdbby_location_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    13691 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/refresh_vdbby_snapshot_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    11199 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/refresh_vdbby_snapshot_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    15702 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/refresh_vdbby_timestamp_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    11811 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/refresh_vdbby_timestamp_parameters_all_of.py
--rw-r--r--   0 runner    (1001) docker     (116)    11202 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/refresh_vdbby_timestamp_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    27881 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/registered_engine.py
--rw-r--r--   0 runner    (1001) docker     (116)    11357 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/remove_masking_job_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    17552 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/reporting_schedule.py
--rw-r--r--   0 runner    (1001) docker     (116)    17660 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/reporting_schedule_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    17641 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/repository.py
--rw-r--r--   0 runner    (1001) docker     (116)    11554 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/reset_password_parameter.py
--rw-r--r--   0 runner    (1001) docker     (116)    14887 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/role.py
--rw-r--r--   0 runner    (1001) docker     (116)    11378 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/role_all_of.py
--rw-r--r--   0 runner    (1001) docker     (116)    11517 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/role_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    13626 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/rollback_vdb_from_bookmark_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    11208 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/rollback_vdb_from_bookmark_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11371 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/rollback_vdb_group_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    11187 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/rollback_vdb_group_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    13694 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/rollback_vdbby_snapshot_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    11202 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/rollback_vdbby_snapshot_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    14537 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/rollback_vdbby_timestamp_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    11205 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/rollback_vdbby_timestamp_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    15281 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/saml_config_params.py
--rw-r--r--   0 runner    (1001) docker     (116)    12281 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/scope_tag.py
--rw-r--r--   0 runner    (1001) docker     (116)    11509 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/scope_tags_request.py
--rw-r--r--   0 runner    (1001) docker     (116)    11381 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/scope_tags_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    12106 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/scoped_object_item.py
--rw-r--r--   0 runner    (1001) docker     (116)    11445 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/scoped_object_items_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11502 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/scoped_objects_request.py
--rw-r--r--   0 runner    (1001) docker     (116)    11742 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/search_access_groups_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11701 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/search_accounts_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11180 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/search_body.py
--rw-r--r--   0 runner    (1001) docker     (116)    11711 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/search_bookmarks_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11661 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/search_cdbs_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11721 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/search_connectors_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11702 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/search_d_sources_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11792 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/search_database_templates_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11749 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/search_dataset_group_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11762 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/search_engines_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11741 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/search_environments_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11721 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/search_executions_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11661 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/search_jobs_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11854 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/search_masking_job_source_engines_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11732 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/search_masking_jobs_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11671 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/search_roles_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11711 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/search_snapshots_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11691 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/search_sources_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11711 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/search_timeflows_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11671 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/search_vcdbs_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11709 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/search_vdb_group_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11661 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/search_vdbs_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11835 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/search_virtualization_policies_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    14702 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/smtp_config_params.py
--rw-r--r--   0 runner    (1001) docker     (116)    11239 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/smtp_config_validate.py
--rw-r--r--   0 runner    (1001) docker     (116)    23967 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (116)    11599 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/snapshot_compatible_repositories.py
--rw-r--r--   0 runner    (1001) docker     (116)    12996 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/snapshot_compatible_repository_request.py
--rw-r--r--   0 runner    (1001) docker     (116)    11184 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/snapshot_d_source_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    12133 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/snapshot_day_range.py
--rw-r--r--   0 runner    (1001) docker     (116)    11172 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/snapshot_vdb_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11302 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/snapshots_day_ranges_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    14989 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/source.py
--rw-r--r--   0 runner    (1001) docker     (116)    13026 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/ssh_verification_strategy.py
--rw-r--r--   0 runner    (1001) docker     (116)    11163 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/start_vdb_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11160 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/stop_vdb_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11162 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/switch_timeflow_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    11181 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/switch_timeflow_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11470 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/tag.py
--rw-r--r--   0 runner    (1001) docker     (116)    11362 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/tags_request.py
--rw-r--r--   0 runner    (1001) docker     (116)    11234 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/tags_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11653 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/task_event.py
--rw-r--r--   0 runner    (1001) docker     (116)    12655 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/time_to_update_sources_request.py
--rw-r--r--   0 runner    (1001) docker     (116)    11313 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/time_to_update_sources_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    17540 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/timeflow.py
--rw-r--r--   0 runner    (1001) docker     (116)    11266 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/token_info_request.py
--rw-r--r--   0 runner    (1001) docker     (116)    13858 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/token_info_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11205 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/unset_snapshot_retention_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    12231 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/update_access_group_scope.py
--rw-r--r--   0 runner    (1001) docker     (116)    11931 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/update_bookmark_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    11184 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/update_connector_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    12427 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/update_database_template_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    11205 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/update_database_template_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11190 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/update_environment_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11202 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/update_environment_user_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11169 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/update_host_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    13354 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/update_masking_job_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    11579 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/update_snapshot_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    11181 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/update_snapshot_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11198 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/update_timeflow_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    11181 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/update_timeflow_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11461 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/update_vdb_group_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    25740 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/update_vdb_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)    11166 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/update_vdb_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    14481 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/vcdb.py
--rw-r--r--   0 runner    (1001) docker     (116)    21762 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/vdb.py
--rw-r--r--   0 runner    (1001) docker     (116)    12088 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/vdb_group.py
--rw-r--r--   0 runner    (1001) docker     (116)    13503 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/vdb_inventory_data.py
--rw-r--r--   0 runner    (1001) docker     (116)    11778 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/vdb_inventory_report_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    16164 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/virtual_dataset_hooks.py
--rw-r--r--   0 runner    (1001) docker     (116)    12936 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/virtualization_policy.py
--rw-r--r--   0 runner    (1001) docker     (116)    11431 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/virtualization_schedule.py
--rw-r--r--   0 runner    (1001) docker     (116)    14405 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/virtualization_storage_summary_data.py
--rw-r--r--   0 runner    (1001) docker     (116)    11939 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model/virtualization_storage_summary_report_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    80117 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-29 09:14:04.734995 delphix-dct-api-6.0.0/delphix/api/gateway/models/
--rw-r--r--   0 runner    (1001) docker     (116)    24106 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    12647 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/delphix/api/gateway/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-29 09:14:04.738995 delphix-dct-api-6.0.0/delphix_dct_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      269 2023-03-29 09:14:04.000000 delphix-dct-api-6.0.0/delphix_dct_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    27798 2023-03-29 09:14:04.000000 delphix-dct-api-6.0.0/delphix_dct_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-29 09:14:04.000000 delphix-dct-api-6.0.0/delphix_dct_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       32 2023-03-29 09:14:04.000000 delphix-dct-api-6.0.0/delphix_dct_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        8 2023-03-29 09:14:04.000000 delphix-dct-api-6.0.0/delphix_dct_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       69 2023-03-29 09:14:04.774996 delphix-dct-api-6.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      942 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-29 09:14:04.774996 delphix-dct-api-6.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (116)      911 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/test/test_access_group.py
--rw-r--r--   0 runner    (1001) docker     (116)      841 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/test/test_access_group_account_ids_request.py
--rw-r--r--   0 runner    (1001) docker     (116)     1119 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/test/test_access_group_scope.py
--rw-r--r--   0 runner    (1001) docker     (116)      935 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/test/test_access_group_scopes_request.py
--rw-r--r--   0 runner    (1001) docker     (116)      833 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/test/test_access_group_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)      873 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/test/test_account.py
--rw-r--r--   0 runner    (1001) docker     (116)      866 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/test/test_account_create_parameter.py
--rw-r--r--   0 runner    (1001) docker     (116)      859 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/test/test_account_create_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      790 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/test/test_account_login_parameter.py
--rw-r--r--   0 runner    (1001) docker     (116)      797 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/test/test_account_update_parameter.py
--rw-r--r--   0 runner    (1001) docker     (116)     2564 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_accounts_api.py
--rw-r--r--   0 runner    (1001) docker     (116)      783 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/test/test_additional_mount_point.py
--rw-r--r--   0 runner    (1001) docker     (116)      962 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/test/test_all_object_permissions_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1033 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/test/test_always_allowed_permission.py
--rw-r--r--   0 runner    (1001) docker     (116)     1005 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/test/test_always_allowed_permission_request.py
--rw-r--r--   0 runner    (1001) docker     (116)      955 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/test/test_api_classification_config.py
--rw-r--r--   0 runner    (1001) docker     (116)      804 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/test/test_api_classification_object.py
--rw-r--r--   0 runner    (1001) docker     (116)      727 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/test/test_api_usage_data.py
--rw-r--r--   0 runner    (1001) docker     (116)      905 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/test/test_api_usage_report_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     6223 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_authorization_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     1722 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/test/test_base_provision_vdb_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)     1365 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/test/test_base_provision_vdb_parameters_all_of.py
--rw-r--r--   0 runner    (1001) docker     (116)      766 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/test/test_bookmark.py
--rw-r--r--   0 runner    (1001) docker     (116)      880 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/test/test_bookmark_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)     2135 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_bookmarks_api.py
--rw-r--r--   0 runner    (1001) docker     (116)      731 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/test/test_cdb.py
--rw-r--r--   0 runner    (1001) docker     (116)     1413 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_cdbs_api.py
--rw-r--r--   0 runner    (1001) docker     (116)      804 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/test/test_change_password_parameter.py
--rw-r--r--   0 runner    (1001) docker     (116)      785 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_connectivity_api.py
--rw-r--r--   0 runner    (1001) docker     (116)      832 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/test/test_connectivity_check_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)      818 2023-03-29 09:13:55.000000 delphix-dct-api-6.0.0/test/test_connectivity_check_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      773 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_connector.py
--rw-r--r--   0 runner    (1001) docker     (116)      790 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_connector_test_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      818 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_connector_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)     1919 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_connectors_api.py
--rw-r--r--   0 runner    (1001) docker     (116)      812 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_copy_masking_job_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)      867 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_copy_masking_job_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      955 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_create_bookmark_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1045 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_create_database_template_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      887 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_create_environment_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      916 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_create_environment_user_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      838 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_create_host_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      903 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_create_role.py
--rw-r--r--   0 runner    (1001) docker     (116)      860 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_create_vdb_group_request.py
--rw-r--r--   0 runner    (1001) docker     (116)      888 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_create_vdb_group_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      760 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_d_source.py
--rw-r--r--   0 runner    (1001) docker     (116)      798 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_d_source_consumption_data.py
--rw-r--r--   0 runner    (1001) docker     (116)     1176 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_d_source_consumption_report_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      819 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_d_source_snapshot_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)      756 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_d_source_usage_data.py
--rw-r--r--   0 runner    (1001) docker     (116)     1110 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_d_source_usage_report_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     2123 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_d_sources_api.py
--rw-r--r--   0 runner    (1001) docker     (116)      848 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_data_point_by_snapshot_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)      855 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_data_point_by_timestamp_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)      862 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_data_point_from_bookmark_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)      823 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_database_template.py
--rw-r--r--   0 runner    (1001) docker     (116)      937 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_database_template_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)     2622 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_database_templates_api.py
--rw-r--r--   0 runner    (1001) docker     (116)      726 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_dataset_group.py
--rw-r--r--   0 runner    (1001) docker     (116)      923 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_delete_database_template_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      852 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_delete_engine_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      887 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_delete_environment_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      916 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_delete_environment_user_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      838 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_delete_host_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      881 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_delete_masking_job_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      881 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_delete_scope_object_tags.py
--rw-r--r--   0 runner    (1001) docker     (116)      921 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_delete_scoped_object_item.py
--rw-r--r--   0 runner    (1001) docker     (116)      866 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_delete_snapshot_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      774 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_delete_tag.py
--rw-r--r--   0 runner    (1001) docker     (116)      866 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_delete_timeflow_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      776 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_delete_vdb_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)      831 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_delete_vdb_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      894 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_disable_environment_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      783 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_disable_vdb_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)      838 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_disable_vdb_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      683 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_domain.py
--rw-r--r--   0 runner    (1001) docker     (116)      740 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_effective_scope.py
--rw-r--r--   0 runner    (1001) docker     (116)      887 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_enable_environment_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      776 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_enable_vdb_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)      831 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_enable_vdb_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      752 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (116)      727 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_engine_id_body.py
--rw-r--r--   0 runner    (1001) docker     (116)      901 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_engine_registration_parameter.py
--rw-r--r--   0 runner    (1001) docker     (116)     1071 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_environment.py
--rw-r--r--   0 runner    (1001) docker     (116)      901 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_environment_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)     1050 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_environment_repository.py
--rw-r--r--   0 runner    (1001) docker     (116)      826 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_environment_repository_all_of.py
--rw-r--r--   0 runner    (1001) docker     (116)      832 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_environment_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)      747 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_environment_user.py
--rw-r--r--   0 runner    (1001) docker     (116)      790 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_environment_user_params.py
--rw-r--r--   0 runner    (1001) docker     (116)     3974 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_environments_api.py
--rw-r--r--   0 runner    (1001) docker     (116)      676 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_error.py
--rw-r--r--   0 runner    (1001) docker     (116)      733 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_error_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      760 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (116)      833 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_execute_masking_job_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)      888 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_execute_masking_job_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      798 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_execution.py
--rw-r--r--   0 runner    (1001) docker     (116)      818 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_execution_cancel_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)     1196 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_executions_api.py
--rw-r--r--   0 runner    (1001) docker     (116)      754 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_global_properties.py
--rw-r--r--   0 runner    (1001) docker     (116)     1041 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_groups_api.py
--rw-r--r--   0 runner    (1001) docker     (116)      809 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_hashicorp_vault.py
--rw-r--r--   0 runner    (1001) docker     (116)      669 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_hook.py
--rw-r--r--   0 runner    (1001) docker     (116)      788 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_host.py
--rw-r--r--   0 runner    (1001) docker     (116)     1053 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_host_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)     1053 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_host_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)      731 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_job.py
--rw-r--r--   0 runner    (1001) docker     (116)     1507 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_jobs_api.py
--rw-r--r--   0 runner    (1001) docker     (116)      836 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_ldap_config_params.py
--rw-r--r--   0 runner    (1001) docker     (116)      833 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_ldap_config_validate_parameter.py
--rw-r--r--   0 runner    (1001) docker     (116)      783 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_ldap_validate_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      820 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_link_d_source_default_request.py
--rw-r--r--   0 runner    (1001) docker     (116)      933 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_link_d_source_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)      846 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_link_d_source_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1073 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_list_access_groups_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1027 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_list_accounts_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1118 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_list_bookmarks_by_vdb_groups_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1038 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_list_bookmarks_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      983 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_list_cdbs_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1049 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_list_connectors_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1110 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_list_d_sources_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1128 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_list_database_templates_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      901 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_list_environment_users.py
--rw-r--r--   0 runner    (1001) docker     (116)     1152 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_list_environments_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1049 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_list_executions_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1034 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_list_groups_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1106 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_list_hashicorp_vaults_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1064 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_list_jobs_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1198 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_list_masking_job_source_engines_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1062 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_list_masking_jobs_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1128 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_list_registered_engines_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1132 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_list_reporting_schedule_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      835 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_list_roles_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1038 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_list_snapshots_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1097 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_list_sources_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1038 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_list_timeflows_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      994 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_list_vcdbs_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1112 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_list_vdb_groups_by_bookmark_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1040 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_list_vdb_groups_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1064 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_list_vdbs_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1179 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_list_virtualization_policies_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      843 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_login_api.py
--rw-r--r--   0 runner    (1001) docker     (116)      712 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_login_token.py
--rw-r--r--   0 runner    (1001) docker     (116)     5661 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_management_api.py
--rw-r--r--   0 runner    (1001) docker     (116)      895 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_masking_job.py
--rw-r--r--   0 runner    (1001) docker     (116)      933 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_masking_job_connectors_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      798 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_masking_job_source_engine.py
--rw-r--r--   0 runner    (1001) docker     (116)     3057 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_masking_jobs_api.py
--rw-r--r--   0 runner    (1001) docker     (116)      740 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_masking_ruleset.py
--rw-r--r--   0 runner    (1001) docker     (116)      741 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_metadata_db_info.py
--rw-r--r--   0 runner    (1001) docker     (116)      833 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_migrate_masking_job_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)      888 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_migrate_masking_job_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      840 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_object_permission_access_groups.py
--rw-r--r--   0 runner    (1001) docker     (116)      976 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_object_permission_account.py
--rw-r--r--   0 runner    (1001) docker     (116)      969 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_object_permissions_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      741 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_object_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (116)      769 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_object_type_property.py
--rw-r--r--   0 runner    (1001) docker     (116)      740 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_oracle_listener.py
--rw-r--r--   0 runner    (1001) docker     (116)      799 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_oracle_rac_custom_env_file.py
--rw-r--r--   0 runner    (1001) docker     (116)      792 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_oracle_rac_custom_env_var.py
--rw-r--r--   0 runner    (1001) docker     (116)      748 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_oracle_virtual_ip.py
--rw-r--r--   0 runner    (1001) docker     (116)      818 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_paginated_response_metadata.py
--rw-r--r--   0 runner    (1001) docker     (116)      797 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_password_policies_params.py
--rw-r--r--   0 runner    (1001) docker     (116)      740 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_permission_enum.py
--rw-r--r--   0 runner    (1001) docker     (116)     1015 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_permission_object.py
--rw-r--r--   0 runner    (1001) docker     (116)      768 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_permission_property.py
--rw-r--r--   0 runner    (1001) docker     (116)      890 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_permissions_request.py
--rw-r--r--   0 runner    (1001) docker     (116)      923 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_primary_environment_user_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      740 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_product_history.py
--rw-r--r--   0 runner    (1001) docker     (116)      833 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_product_info.py
--rw-r--r--   0 runner    (1001) docker     (116)      919 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_provision_vdb_from_bookmark_defaults_request.py
--rw-r--r--   0 runner    (1001) docker     (116)     2026 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_provision_vdb_from_bookmark_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)      920 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_provision_vdb_from_bookmark_parameters_all_of.py
--rw-r--r--   0 runner    (1001) docker     (116)     1152 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_provision_vdb_group_from_bookmark_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)     1064 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_provision_vdb_group_from_bookmark_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      852 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_provision_vdb_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      904 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_provision_vdbby_snapshot_defaults_request.py
--rw-r--r--   0 runner    (1001) docker     (116)     1994 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_provision_vdbby_snapshot_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)      905 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_provision_vdbby_snapshot_parameters_all_of.py
--rw-r--r--   0 runner    (1001) docker     (116)      911 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_provision_vdbby_timestamp_defaults_request.py
--rw-r--r--   0 runner    (1001) docker     (116)     2009 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_provision_vdbby_timestamp_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)      912 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_provision_vdbby_timestamp_parameters_all_of.py
--rw-r--r--   0 runner    (1001) docker     (116)      894 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_refresh_environment_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1054 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_refresh_vdb_from_bookmark_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)      924 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_refresh_vdb_from_bookmark_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      819 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_refresh_vdb_group_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)      874 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_refresh_vdb_group_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      854 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_refresh_vdbby_location_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)      909 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_refresh_vdbby_location_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1031 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_refresh_vdbby_snapshot_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)      909 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_refresh_vdbby_snapshot_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1248 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_refresh_vdbby_timestamp_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)      898 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_refresh_vdbby_timestamp_parameters_all_of.py
--rw-r--r--   0 runner    (1001) docker     (116)      916 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_refresh_vdbby_timestamp_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      823 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_registered_engine.py
--rw-r--r--   0 runner    (1001) docker     (116)      826 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_remove_masking_job_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)     4528 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_reporting_api.py
--rw-r--r--   0 runner    (1001) docker     (116)      830 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_reporting_schedule.py
--rw-r--r--   0 runner    (1001) docker     (116)      875 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_reporting_schedule_create_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)      711 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_repository.py
--rw-r--r--   0 runner    (1001) docker     (116)      797 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_reset_password_parameter.py
--rw-r--r--   0 runner    (1001) docker     (116)     1053 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_role.py
--rw-r--r--   0 runner    (1001) docker     (116)      706 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_role_all_of.py
--rw-r--r--   0 runner    (1001) docker     (116)      783 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_role_update_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)     1061 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_rollback_vdb_from_bookmark_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)      931 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_rollback_vdb_from_bookmark_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      826 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_rollback_vdb_group_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)      881 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_rollback_vdb_group_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1038 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_rollback_vdbby_snapshot_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)      916 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_rollback_vdbby_snapshot_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1049 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_rollback_vdbby_timestamp_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)      923 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_rollback_vdbby_timestamp_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      755 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_saml_config_params.py
--rw-r--r--   0 runner    (1001) docker     (116)      700 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_saml_login_api.py
--rw-r--r--   0 runner    (1001) docker     (116)      927 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_scope_tag.py
--rw-r--r--   0 runner    (1001) docker     (116)      845 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_scope_tags_request.py
--rw-r--r--   0 runner    (1001) docker     (116)      852 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_scope_tags_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      984 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_scoped_object_item.py
--rw-r--r--   0 runner    (1001) docker     (116)      942 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_scoped_object_items_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      906 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_scoped_objects_request.py
--rw-r--r--   0 runner    (1001) docker     (116)     1087 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_search_access_groups_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1041 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_search_accounts_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      712 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_search_body.py
--rw-r--r--   0 runner    (1001) docker     (116)     1052 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_search_bookmarks_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      997 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_search_cdbs_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1063 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_search_connectors_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1043 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_search_d_sources_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1142 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_search_database_templates_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1091 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_search_dataset_group_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1071 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_search_engines_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1085 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_search_environments_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1063 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_search_executions_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      997 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_search_jobs_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1212 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_search_masking_job_source_engines_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1076 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_search_masking_jobs_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1008 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_search_roles_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1052 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_search_snapshots_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1030 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_search_sources_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1052 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_search_timeflows_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1008 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_search_vcdbs_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1047 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_search_vdb_group_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      997 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_search_vdbs_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1193 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_search_virtualization_policies_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      755 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_smtp_config_params.py
--rw-r--r--   0 runner    (1001) docker     (116)      769 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_smtp_config_validate.py
--rw-r--r--   0 runner    (1001) docker     (116)      766 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (116)      995 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_snapshot_compatible_repositories.py
--rw-r--r--   0 runner    (1001) docker     (116)      889 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_snapshot_compatible_repository_request.py
--rw-r--r--   0 runner    (1001) docker     (116)      874 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_snapshot_d_source_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      755 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_snapshot_day_range.py
--rw-r--r--   0 runner    (1001) docker     (116)      845 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_snapshot_vdb_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     2033 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_snapshots_api.py
--rw-r--r--   0 runner    (1001) docker     (116)      949 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_snapshots_day_ranges_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      752 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_source.py
--rw-r--r--   0 runner    (1001) docker     (116)     1440 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_sources_api.py
--rw-r--r--   0 runner    (1001) docker     (116)      804 2023-03-29 09:13:56.000000 delphix-dct-api-6.0.0/test/test_ssh_verification_strategy.py
--rw-r--r--   0 runner    (1001) docker     (116)      824 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_start_vdb_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      817 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_stop_vdb_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      811 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_switch_timeflow_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)      866 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_switch_timeflow_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      662 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_tag.py
--rw-r--r--   0 runner    (1001) docker     (116)      788 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_tags_request.py
--rw-r--r--   0 runner    (1001) docker     (116)      795 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_tags_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      705 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_task_event.py
--rw-r--r--   0 runner    (1001) docker     (116)      753 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_test_api.py
--rw-r--r--   0 runner    (1001) docker     (116)      827 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_time_to_update_sources_request.py
--rw-r--r--   0 runner    (1001) docker     (116)      834 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_time_to_update_sources_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      766 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_timeflow.py
--rw-r--r--   0 runner    (1001) docker     (116)     2027 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_timeflows_api.py
--rw-r--r--   0 runner    (1001) docker     (116)      755 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_token_info_request.py
--rw-r--r--   0 runner    (1001) docker     (116)      762 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_token_info_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      923 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_unset_snapshot_retention_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      798 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_update_access_group_scope.py
--rw-r--r--   0 runner    (1001) docker     (116)      811 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_update_bookmark_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)      873 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_update_connector_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      868 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_update_database_template_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)      923 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_update_database_template_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      887 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_update_environment_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      916 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_update_environment_user_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      838 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_update_host_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      826 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_update_masking_job_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)      811 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_update_snapshot_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)      866 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_update_snapshot_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      811 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_update_timeflow_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)      866 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_update_timeflow_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      812 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_update_vdb_group_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)     1344 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_update_vdb_parameters.py
--rw-r--r--   0 runner    (1001) docker     (116)      831 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_update_vdb_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      738 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_vcdb.py
--rw-r--r--   0 runner    (1001) docker     (116)     1435 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_vcdbs_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     1005 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_vdb.py
--rw-r--r--   0 runner    (1001) docker     (116)      767 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_vdb_group.py
--rw-r--r--   0 runner    (1001) docker     (116)     2665 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_vdb_groups_api.py
--rw-r--r--   0 runner    (1001) docker     (116)      755 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_vdb_inventory_data.py
--rw-r--r--   0 runner    (1001) docker     (116)     1108 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_vdb_inventory_report_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     5165 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_vdbs_api.py
--rw-r--r--   0 runner    (1001) docker     (116)      849 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_virtual_dataset_hooks.py
--rw-r--r--   0 runner    (1001) docker     (116)     1202 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_virtualization_policies_api.py
--rw-r--r--   0 runner    (1001) docker     (116)      928 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_virtualization_policy.py
--rw-r--r--   0 runner    (1001) docker     (116)      796 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_virtualization_schedule.py
--rw-r--r--   0 runner    (1001) docker     (116)      868 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_virtualization_storage_summary_data.py
--rw-r--r--   0 runner    (1001) docker     (116)     1286 2023-03-29 09:13:57.000000 delphix-dct-api-6.0.0/test/test_virtualization_storage_summary_report_response.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-24 10:11:33.917050 delphix-dct-api-6.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (116)      272 2023-03-24 10:11:33.917050 delphix-dct-api-6.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)    64628 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-24 10:11:33.777049 delphix-dct-api-6.0.0rc1/delphix/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/delphix/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-24 10:11:33.777049 delphix-dct-api-6.0.0rc1/delphix/api/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/delphix/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-24 10:11:33.777049 delphix-dct-api-6.0.0rc1/delphix/api/gateway/
+-rw-r--r--   0 runner    (1001) docker     (116)      760 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-24 10:11:33.789049 delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/
+-rw-r--r--   0 runner    (1001) docker     (116)      224 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    65198 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/accounts_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)   173762 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/authorization_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    54762 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/bookmarks_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    34507 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/cdbs_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5650 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/connectivity_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    44574 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/connectors_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    56971 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/d_sources_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    58964 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/database_templates_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)   109504 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/environments_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    27195 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/executions_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    20449 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/groups_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    39107 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9677 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/login_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)   138683 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/management_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    80140 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/masking_jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)   116463 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/reporting_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4690 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/saml_login_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    54724 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/snapshots_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    35881 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/sources_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5352 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    51542 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/timeflows_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    35334 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/vcdbs_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    69811 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/vdb_groups_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)   144626 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/vdbs_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    20856 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/virtualization_policies_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    36851 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-24 10:11:33.789049 delphix-dct-api-6.0.0rc1/delphix/api/gateway/apis/
+-rw-r--r--   0 runner    (1001) docker     (116)     1998 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16983 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5038 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-24 10:11:33.853049 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/
+-rw-r--r--   0 runner    (1001) docker     (116)      348 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13907 2023-03-24 10:11:21.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/access_group.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11286 2023-03-24 10:11:21.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/access_group_account_ids_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15309 2023-03-24 10:11:21.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/access_group_scope.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11448 2023-03-24 10:11:21.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/access_group_scopes_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11198 2023-03-24 10:11:21.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/access_group_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15588 2023-03-24 10:11:21.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/account.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16533 2023-03-24 10:11:21.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/account_create_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14295 2023-03-24 10:11:21.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/account_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11734 2023-03-24 10:11:21.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/account_login_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14723 2023-03-24 10:11:21.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/account_update_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12275 2023-03-24 10:11:21.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/additional_mount_point.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11372 2023-03-24 10:11:21.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/all_object_permissions_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11798 2023-03-24 10:11:21.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/always_allowed_permission.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11833 2023-03-24 10:11:21.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/always_allowed_permission_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11804 2023-03-24 10:11:21.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/api_classification_config.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12702 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/api_classification_object.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13192 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/api_usage_data.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12106 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/api_usage_report_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    45609 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/base_provision_vdb_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    38003 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/base_provision_vdb_parameters_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13815 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/bookmark.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14458 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/bookmark_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13327 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/cdb.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12076 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/change_password_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11932 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/connectivity_check_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11247 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/connectivity_check_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13356 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/connector.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11637 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/connector_test_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12418 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/connector_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12487 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/copy_masking_job_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11409 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/copy_masking_job_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11491 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/create_bookmark_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11617 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/create_database_template_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11482 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/create_environment_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11494 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/create_environment_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11476 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/create_host_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12373 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/create_role.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12549 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/create_vdb_group_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11247 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/create_vdb_group_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17279 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/d_source.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13076 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/d_source_consumption_data.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11839 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/d_source_consumption_report_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    19622 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/d_source_snapshot_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12945 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/d_source_usage_data.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11779 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/d_source_usage_report_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11434 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/data_point_by_snapshot_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12272 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/data_point_by_timestamp_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11490 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/data_point_from_bookmark_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13058 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/database_template.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13463 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/database_template_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12210 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/dataset_group.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11205 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/delete_database_template_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11175 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/delete_engine_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11190 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/delete_environment_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11202 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/delete_environment_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11169 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/delete_host_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11187 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/delete_masking_job_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11384 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/delete_scope_object_tags.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11528 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/delete_scoped_object_item.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11181 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/delete_snapshot_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11910 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/delete_tag.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11181 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/delete_timeflow_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11260 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/delete_vdb_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11166 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/delete_vdb_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11193 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/disable_environment_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11333 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/disable_vdb_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11169 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/disable_vdb_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15475 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/domain.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11317 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/effective_scope.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11190 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/enable_environment_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11316 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/enable_vdb_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11166 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/enable_vdb_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16724 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/engine.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11106 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/engine_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (116)    21137 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/engine_registration_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15110 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/environment.py
+-rw-r--r--   0 runner    (1001) docker     (116)    29606 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/environment_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    20313 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/environment_repository.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11149 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/environment_repository_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17594 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/environment_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13401 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/environment_user.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15622 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/environment_user_params.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11530 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/error.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11592 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12594 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/errors.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11327 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/execute_masking_job_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11190 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/execute_masking_job_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16753 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/execution.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11526 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/execution_cancel_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11305 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/global_properties.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13015 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/hashicorp_vault.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12332 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/hook.py
+-rw-r--r--   0 runner    (1001) docker     (116)    20772 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/host.py
+-rw-r--r--   0 runner    (1001) docker     (116)    18094 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/host_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    18866 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/host_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13953 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/job.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17452 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/ldap_config_params.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11740 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/ldap_config_validate_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11192 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/ldap_validate_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11221 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/link_d_source_default_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)    29530 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/link_d_source_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11428 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/link_d_source_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11736 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_access_groups_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11695 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_accounts_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11738 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_bookmarks_by_vdb_groups_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11705 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_bookmarks_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11655 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_cdbs_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11715 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_connectors_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11982 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_d_sources_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11786 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_database_templates_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11306 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_environment_users.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12021 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_environments_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11715 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_executions_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11725 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_groups_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11766 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_hashicorp_vaults_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11941 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_jobs_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11848 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_masking_job_source_engines_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11726 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_masking_jobs_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11786 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_registered_engines_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11793 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_reporting_schedule_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11189 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_roles_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11705 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_snapshots_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11971 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_sources_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11705 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_timeflows_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11665 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_vcdbs_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11736 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_vdb_groups_by_bookmark_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11706 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_vdb_groups_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11941 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_vdbs_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11829 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_virtualization_policies_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12897 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/login_token.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15504 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/masking_job.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11547 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/masking_job_connectors_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11515 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/masking_job_source_engine.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12238 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/masking_ruleset.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14855 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/metadata_db_info.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12496 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/migrate_masking_job_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11190 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/migrate_masking_job_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11654 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/object_permission_access_groups.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12454 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/object_permission_account.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11445 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/object_permissions_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13606 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/object_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12735 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/object_type_property.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12879 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/oracle_listener.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11388 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/oracle_rac_custom_env_file.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11700 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/oracle_rac_custom_env_var.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11730 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/oracle_virtual_ip.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12321 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/paginated_response_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14496 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/password_policies_params.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14622 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/permission_enum.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16832 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/permission_object.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12857 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/permission_property.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11693 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/permissions_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11205 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/primary_environment_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11371 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/product_history.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12286 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/product_info.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11514 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/provision_vdb_from_bookmark_defaults_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)    46983 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/provision_vdb_from_bookmark_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11489 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/provision_vdb_from_bookmark_parameters_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13978 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/provision_vdb_group_from_bookmark_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11542 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/provision_vdb_group_from_bookmark_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11427 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/provision_vdb_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12560 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/provision_vdbby_snapshot_defaults_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)    48436 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/provision_vdbby_snapshot_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12879 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/provision_vdbby_snapshot_parameters_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13636 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/provision_vdbby_timestamp_defaults_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)    49076 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/provision_vdbby_timestamp_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12826 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/provision_vdbby_timestamp_parameters_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11193 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/refresh_environment_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13623 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/refresh_vdb_from_bookmark_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11205 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/refresh_vdb_from_bookmark_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11366 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/refresh_vdb_group_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11184 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/refresh_vdb_group_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12305 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/refresh_vdbby_location_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11199 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/refresh_vdbby_location_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13691 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/refresh_vdbby_snapshot_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11199 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/refresh_vdbby_snapshot_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15702 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/refresh_vdbby_timestamp_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11811 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/refresh_vdbby_timestamp_parameters_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11202 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/refresh_vdbby_timestamp_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    27881 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/registered_engine.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11357 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/remove_masking_job_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17552 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/reporting_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17660 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/reporting_schedule_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17641 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/repository.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11554 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/reset_password_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14887 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/role.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11378 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/role_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11517 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/role_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13626 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/rollback_vdb_from_bookmark_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11208 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/rollback_vdb_from_bookmark_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11371 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/rollback_vdb_group_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11187 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/rollback_vdb_group_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13694 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/rollback_vdbby_snapshot_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11202 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/rollback_vdbby_snapshot_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14537 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/rollback_vdbby_timestamp_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11205 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/rollback_vdbby_timestamp_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15281 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/saml_config_params.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12281 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/scope_tag.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11509 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/scope_tags_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11381 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/scope_tags_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12106 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/scoped_object_item.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11445 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/scoped_object_items_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11502 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/scoped_objects_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11742 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_access_groups_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11701 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_accounts_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11180 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_body.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11711 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_bookmarks_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11661 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_cdbs_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11721 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_connectors_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11702 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_d_sources_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11792 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_database_templates_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11749 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_dataset_group_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11762 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_engines_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11741 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_environments_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11721 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_executions_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11661 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_jobs_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11854 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_masking_job_source_engines_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11732 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_masking_jobs_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11671 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_roles_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11711 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_snapshots_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11691 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_sources_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11711 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_timeflows_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11671 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_vcdbs_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11709 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_vdb_group_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11661 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_vdbs_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11835 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_virtualization_policies_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14702 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/smtp_config_params.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11239 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/smtp_config_validate.py
+-rw-r--r--   0 runner    (1001) docker     (116)    23967 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11599 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/snapshot_compatible_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12996 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/snapshot_compatible_repository_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11184 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/snapshot_d_source_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12133 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/snapshot_day_range.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11172 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/snapshot_vdb_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11302 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/snapshots_day_ranges_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14989 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/source.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13026 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/ssh_verification_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11163 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/start_vdb_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11160 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/stop_vdb_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11162 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/switch_timeflow_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11181 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/switch_timeflow_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11470 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/tag.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11362 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/tags_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11234 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/tags_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11653 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/task_event.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12655 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/time_to_update_sources_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11313 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/time_to_update_sources_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17540 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/timeflow.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11266 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/token_info_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13858 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/token_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11205 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/unset_snapshot_retention_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12231 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/update_access_group_scope.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11931 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/update_bookmark_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11184 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/update_connector_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12427 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/update_database_template_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11205 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/update_database_template_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11190 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/update_environment_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11202 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/update_environment_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11169 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/update_host_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13354 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/update_masking_job_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11579 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/update_snapshot_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11181 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/update_snapshot_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11198 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/update_timeflow_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11181 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/update_timeflow_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11461 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/update_vdb_group_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    25740 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/update_vdb_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11166 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/update_vdb_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14481 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/vcdb.py
+-rw-r--r--   0 runner    (1001) docker     (116)    21762 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/vdb.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12088 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/vdb_group.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13503 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/vdb_inventory_data.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11778 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/vdb_inventory_report_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16164 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/virtual_dataset_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12936 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/virtualization_policy.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11431 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/virtualization_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14405 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/virtualization_storage_summary_data.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11939 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/virtualization_storage_summary_report_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)    80117 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-24 10:11:33.853049 delphix-dct-api-6.0.0rc1/delphix/api/gateway/models/
+-rw-r--r--   0 runner    (1001) docker     (116)    24106 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12647 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/delphix/api/gateway/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-24 10:11:33.857049 delphix-dct-api-6.0.0rc1/delphix_dct_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)      272 2023-03-24 10:11:33.000000 delphix-dct-api-6.0.0rc1/delphix_dct_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)    27798 2023-03-24 10:11:33.000000 delphix-dct-api-6.0.0rc1/delphix_dct_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-24 10:11:33.000000 delphix-dct-api-6.0.0rc1/delphix_dct_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       32 2023-03-24 10:11:33.000000 delphix-dct-api-6.0.0rc1/delphix_dct_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        8 2023-03-24 10:11:33.000000 delphix-dct-api-6.0.0rc1/delphix_dct_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       69 2023-03-24 10:11:33.917050 delphix-dct-api-6.0.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      946 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-24 10:11:33.917050 delphix-dct-api-6.0.0rc1/test/
+-rw-r--r--   0 runner    (1001) docker     (116)      911 2023-03-24 10:11:21.000000 delphix-dct-api-6.0.0rc1/test/test_access_group.py
+-rw-r--r--   0 runner    (1001) docker     (116)      841 2023-03-24 10:11:21.000000 delphix-dct-api-6.0.0rc1/test/test_access_group_account_ids_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1119 2023-03-24 10:11:21.000000 delphix-dct-api-6.0.0rc1/test/test_access_group_scope.py
+-rw-r--r--   0 runner    (1001) docker     (116)      935 2023-03-24 10:11:21.000000 delphix-dct-api-6.0.0rc1/test/test_access_group_scopes_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)      833 2023-03-24 10:11:21.000000 delphix-dct-api-6.0.0rc1/test/test_access_group_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)      873 2023-03-24 10:11:21.000000 delphix-dct-api-6.0.0rc1/test/test_account.py
+-rw-r--r--   0 runner    (1001) docker     (116)      866 2023-03-24 10:11:21.000000 delphix-dct-api-6.0.0rc1/test/test_account_create_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (116)      859 2023-03-24 10:11:21.000000 delphix-dct-api-6.0.0rc1/test/test_account_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      790 2023-03-24 10:11:21.000000 delphix-dct-api-6.0.0rc1/test/test_account_login_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (116)      797 2023-03-24 10:11:21.000000 delphix-dct-api-6.0.0rc1/test/test_account_update_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2564 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/test/test_accounts_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)      783 2023-03-24 10:11:21.000000 delphix-dct-api-6.0.0rc1/test/test_additional_mount_point.py
+-rw-r--r--   0 runner    (1001) docker     (116)      962 2023-03-24 10:11:21.000000 delphix-dct-api-6.0.0rc1/test/test_all_object_permissions_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1033 2023-03-24 10:11:21.000000 delphix-dct-api-6.0.0rc1/test/test_always_allowed_permission.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1005 2023-03-24 10:11:21.000000 delphix-dct-api-6.0.0rc1/test/test_always_allowed_permission_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)      955 2023-03-24 10:11:21.000000 delphix-dct-api-6.0.0rc1/test/test_api_classification_config.py
+-rw-r--r--   0 runner    (1001) docker     (116)      804 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_api_classification_object.py
+-rw-r--r--   0 runner    (1001) docker     (116)      727 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_api_usage_data.py
+-rw-r--r--   0 runner    (1001) docker     (116)      905 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_api_usage_report_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6223 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/test/test_authorization_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1722 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_base_provision_vdb_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1365 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_base_provision_vdb_parameters_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (116)      766 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_bookmark.py
+-rw-r--r--   0 runner    (1001) docker     (116)      880 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_bookmark_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2135 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/test/test_bookmarks_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)      731 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_cdb.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1413 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/test/test_cdbs_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)      804 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_change_password_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (116)      785 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/test/test_connectivity_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)      832 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_connectivity_check_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)      818 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_connectivity_check_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      773 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_connector.py
+-rw-r--r--   0 runner    (1001) docker     (116)      790 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_connector_test_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      818 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_connector_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1919 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/test/test_connectors_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)      812 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_copy_masking_job_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)      867 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_copy_masking_job_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      955 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_create_bookmark_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1045 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_create_database_template_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      887 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_create_environment_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      916 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_create_environment_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      838 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_create_host_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      903 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_create_role.py
+-rw-r--r--   0 runner    (1001) docker     (116)      860 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_create_vdb_group_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)      888 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_create_vdb_group_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      760 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_d_source.py
+-rw-r--r--   0 runner    (1001) docker     (116)      798 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_d_source_consumption_data.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1176 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_d_source_consumption_report_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      819 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_d_source_snapshot_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)      756 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_d_source_usage_data.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1110 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_d_source_usage_report_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2123 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/test/test_d_sources_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)      848 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_data_point_by_snapshot_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)      855 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_data_point_by_timestamp_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)      862 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_data_point_from_bookmark_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)      823 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_database_template.py
+-rw-r--r--   0 runner    (1001) docker     (116)      937 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_database_template_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2622 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/test/test_database_templates_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)      726 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_dataset_group.py
+-rw-r--r--   0 runner    (1001) docker     (116)      923 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_delete_database_template_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      852 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_delete_engine_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      887 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_delete_environment_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      916 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_delete_environment_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      838 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_delete_host_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      881 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_delete_masking_job_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      881 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_delete_scope_object_tags.py
+-rw-r--r--   0 runner    (1001) docker     (116)      921 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_delete_scoped_object_item.py
+-rw-r--r--   0 runner    (1001) docker     (116)      866 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_delete_snapshot_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      774 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_delete_tag.py
+-rw-r--r--   0 runner    (1001) docker     (116)      866 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_delete_timeflow_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      776 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_delete_vdb_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)      831 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_delete_vdb_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      894 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_disable_environment_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      783 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_disable_vdb_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)      838 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_disable_vdb_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      683 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_domain.py
+-rw-r--r--   0 runner    (1001) docker     (116)      740 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_effective_scope.py
+-rw-r--r--   0 runner    (1001) docker     (116)      887 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_enable_environment_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      776 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_enable_vdb_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)      831 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_enable_vdb_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      752 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (116)      727 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_engine_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (116)      901 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_engine_registration_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1071 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (116)      901 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_environment_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1050 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_environment_repository.py
+-rw-r--r--   0 runner    (1001) docker     (116)      826 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_environment_repository_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (116)      832 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_environment_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)      747 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_environment_user.py
+-rw-r--r--   0 runner    (1001) docker     (116)      790 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_environment_user_params.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3974 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/test/test_environments_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)      676 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (116)      733 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      760 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (116)      833 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_execute_masking_job_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)      888 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_execute_masking_job_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      798 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_execution.py
+-rw-r--r--   0 runner    (1001) docker     (116)      818 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_execution_cancel_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1196 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/test/test_executions_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)      754 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_global_properties.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1041 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/test/test_groups_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)      809 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_hashicorp_vault.py
+-rw-r--r--   0 runner    (1001) docker     (116)      669 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_hook.py
+-rw-r--r--   0 runner    (1001) docker     (116)      788 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_host.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1053 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_host_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1053 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_host_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)      731 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1507 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/test/test_jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)      836 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_ldap_config_params.py
+-rw-r--r--   0 runner    (1001) docker     (116)      833 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_ldap_config_validate_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (116)      783 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_ldap_validate_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      820 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_link_d_source_default_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)      933 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_link_d_source_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)      846 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_link_d_source_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1073 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_list_access_groups_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1027 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_list_accounts_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1118 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_list_bookmarks_by_vdb_groups_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1038 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_list_bookmarks_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      983 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_list_cdbs_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1049 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_list_connectors_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1110 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_list_d_sources_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1128 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_list_database_templates_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      901 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_list_environment_users.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1152 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_list_environments_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1049 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_list_executions_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1034 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_list_groups_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1106 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_list_hashicorp_vaults_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1064 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_list_jobs_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1198 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_list_masking_job_source_engines_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1062 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_list_masking_jobs_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1128 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_list_registered_engines_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1132 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_list_reporting_schedule_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      835 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_list_roles_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1038 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_list_snapshots_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1097 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_list_sources_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1038 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_list_timeflows_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      994 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_list_vcdbs_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1112 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_list_vdb_groups_by_bookmark_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1040 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_list_vdb_groups_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1064 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_list_vdbs_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1179 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_list_virtualization_policies_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      843 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/test/test_login_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)      712 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_login_token.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5661 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/test/test_management_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)      895 2023-03-24 10:11:22.000000 delphix-dct-api-6.0.0rc1/test/test_masking_job.py
+-rw-r--r--   0 runner    (1001) docker     (116)      933 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_masking_job_connectors_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      798 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_masking_job_source_engine.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3057 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/test/test_masking_jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)      740 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_masking_ruleset.py
+-rw-r--r--   0 runner    (1001) docker     (116)      741 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_metadata_db_info.py
+-rw-r--r--   0 runner    (1001) docker     (116)      833 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_migrate_masking_job_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)      888 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_migrate_masking_job_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      840 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_object_permission_access_groups.py
+-rw-r--r--   0 runner    (1001) docker     (116)      976 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_object_permission_account.py
+-rw-r--r--   0 runner    (1001) docker     (116)      969 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_object_permissions_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      741 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_object_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (116)      769 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_object_type_property.py
+-rw-r--r--   0 runner    (1001) docker     (116)      740 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_oracle_listener.py
+-rw-r--r--   0 runner    (1001) docker     (116)      799 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_oracle_rac_custom_env_file.py
+-rw-r--r--   0 runner    (1001) docker     (116)      792 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_oracle_rac_custom_env_var.py
+-rw-r--r--   0 runner    (1001) docker     (116)      748 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_oracle_virtual_ip.py
+-rw-r--r--   0 runner    (1001) docker     (116)      818 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_paginated_response_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (116)      797 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_password_policies_params.py
+-rw-r--r--   0 runner    (1001) docker     (116)      740 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_permission_enum.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1015 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_permission_object.py
+-rw-r--r--   0 runner    (1001) docker     (116)      768 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_permission_property.py
+-rw-r--r--   0 runner    (1001) docker     (116)      890 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_permissions_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)      923 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_primary_environment_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      740 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_product_history.py
+-rw-r--r--   0 runner    (1001) docker     (116)      833 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_product_info.py
+-rw-r--r--   0 runner    (1001) docker     (116)      919 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_provision_vdb_from_bookmark_defaults_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2026 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_provision_vdb_from_bookmark_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)      920 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_provision_vdb_from_bookmark_parameters_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1152 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_provision_vdb_group_from_bookmark_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1064 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_provision_vdb_group_from_bookmark_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      852 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_provision_vdb_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      904 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_provision_vdbby_snapshot_defaults_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1994 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_provision_vdbby_snapshot_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)      905 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_provision_vdbby_snapshot_parameters_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (116)      911 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_provision_vdbby_timestamp_defaults_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2009 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_provision_vdbby_timestamp_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)      912 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_provision_vdbby_timestamp_parameters_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (116)      894 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_refresh_environment_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1054 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_refresh_vdb_from_bookmark_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)      924 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_refresh_vdb_from_bookmark_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      819 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_refresh_vdb_group_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)      874 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_refresh_vdb_group_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      854 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_refresh_vdbby_location_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)      909 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_refresh_vdbby_location_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1031 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_refresh_vdbby_snapshot_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)      909 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_refresh_vdbby_snapshot_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1248 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_refresh_vdbby_timestamp_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)      898 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_refresh_vdbby_timestamp_parameters_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (116)      916 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_refresh_vdbby_timestamp_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      823 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_registered_engine.py
+-rw-r--r--   0 runner    (1001) docker     (116)      826 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_remove_masking_job_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4528 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/test/test_reporting_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)      830 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_reporting_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (116)      875 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_reporting_schedule_create_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)      711 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_repository.py
+-rw-r--r--   0 runner    (1001) docker     (116)      797 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_reset_password_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1053 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_role.py
+-rw-r--r--   0 runner    (1001) docker     (116)      706 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_role_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (116)      783 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_role_update_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1061 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_rollback_vdb_from_bookmark_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)      931 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_rollback_vdb_from_bookmark_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      826 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_rollback_vdb_group_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)      881 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_rollback_vdb_group_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1038 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_rollback_vdbby_snapshot_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)      916 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_rollback_vdbby_snapshot_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1049 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_rollback_vdbby_timestamp_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)      923 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_rollback_vdbby_timestamp_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      755 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_saml_config_params.py
+-rw-r--r--   0 runner    (1001) docker     (116)      700 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/test/test_saml_login_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)      927 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_scope_tag.py
+-rw-r--r--   0 runner    (1001) docker     (116)      845 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_scope_tags_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)      852 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_scope_tags_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      984 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_scoped_object_item.py
+-rw-r--r--   0 runner    (1001) docker     (116)      942 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_scoped_object_items_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      906 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_scoped_objects_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1087 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_search_access_groups_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1041 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_search_accounts_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      712 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_search_body.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1052 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_search_bookmarks_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      997 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_search_cdbs_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1063 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_search_connectors_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1043 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_search_d_sources_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1142 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_search_database_templates_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1091 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_search_dataset_group_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1071 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_search_engines_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1085 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_search_environments_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1063 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_search_executions_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      997 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_search_jobs_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1212 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_search_masking_job_source_engines_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1076 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_search_masking_jobs_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1008 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_search_roles_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1052 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_search_snapshots_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1030 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_search_sources_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1052 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_search_timeflows_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1008 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_search_vcdbs_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1047 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_search_vdb_group_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      997 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_search_vdbs_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1193 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_search_virtualization_policies_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      755 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_smtp_config_params.py
+-rw-r--r--   0 runner    (1001) docker     (116)      769 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_smtp_config_validate.py
+-rw-r--r--   0 runner    (1001) docker     (116)      766 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (116)      995 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_snapshot_compatible_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (116)      889 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_snapshot_compatible_repository_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)      874 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_snapshot_d_source_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      755 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_snapshot_day_range.py
+-rw-r--r--   0 runner    (1001) docker     (116)      845 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_snapshot_vdb_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2033 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/test/test_snapshots_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)      949 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_snapshots_day_ranges_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      752 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1440 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/test/test_sources_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)      804 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_ssh_verification_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (116)      824 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_start_vdb_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      817 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_stop_vdb_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      811 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_switch_timeflow_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)      866 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_switch_timeflow_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      662 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_tag.py
+-rw-r--r--   0 runner    (1001) docker     (116)      788 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_tags_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)      795 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_tags_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      705 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_task_event.py
+-rw-r--r--   0 runner    (1001) docker     (116)      753 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/test/test_test_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)      827 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_time_to_update_sources_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)      834 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_time_to_update_sources_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      766 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_timeflow.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2027 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/test/test_timeflows_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)      755 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_token_info_request.py
+-rw-r--r--   0 runner    (1001) docker     (116)      762 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_token_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      923 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_unset_snapshot_retention_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      798 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_update_access_group_scope.py
+-rw-r--r--   0 runner    (1001) docker     (116)      811 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_update_bookmark_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)      873 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_update_connector_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      868 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_update_database_template_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)      923 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_update_database_template_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      887 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_update_environment_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      916 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_update_environment_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      838 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_update_host_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      826 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_update_masking_job_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)      811 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_update_snapshot_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)      866 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_update_snapshot_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      811 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_update_timeflow_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)      866 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_update_timeflow_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      812 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_update_vdb_group_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1344 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_update_vdb_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (116)      831 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_update_vdb_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)      738 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_vcdb.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1435 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/test/test_vcdbs_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1005 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_vdb.py
+-rw-r--r--   0 runner    (1001) docker     (116)      767 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_vdb_group.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2665 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/test/test_vdb_groups_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)      755 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_vdb_inventory_data.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1108 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_vdb_inventory_report_response.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5165 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/test/test_vdbs_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)      849 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_virtual_dataset_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1202 2023-03-24 10:11:24.000000 delphix-dct-api-6.0.0rc1/test/test_virtualization_policies_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)      928 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_virtualization_policy.py
+-rw-r--r--   0 runner    (1001) docker     (116)      796 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_virtualization_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (116)      868 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_virtualization_storage_summary_data.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1286 2023-03-24 10:11:23.000000 delphix-dct-api-6.0.0rc1/test/test_virtualization_storage_summary_report_response.py
```

### Comparing `delphix-dct-api-6.0.0/README.md` & `delphix-dct-api-6.0.0rc1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # delphix-dct-api
 Delphix DCT API
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 3.1.0
-- Package version: 6.0.0
+- Package version: 6.0.0-rc1
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://support.delphix.com](https://support.delphix.com)
 
 ## Requirements.
 
 Python >= 3.6
```

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/__init__.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     The version of the OpenAPI document: 3.1.0
     Contact: support@delphix.com
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "6.0.0"
+__version__ = "6.0.0-rc1"
 
 # import ApiClient
 from delphix.api.gateway.api_client import ApiClient
 
 # import Configuration
 from delphix.api.gateway.configuration import Configuration
```

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/api/accounts_api.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/accounts_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/api/authorization_api.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/authorization_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/api/bookmarks_api.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/bookmarks_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/api/cdbs_api.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/cdbs_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/api/connectivity_api.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/connectivity_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/api/connectors_api.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/connectors_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/api/d_sources_api.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/d_sources_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/api/database_templates_api.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/database_templates_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/api/environments_api.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/environments_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/api/executions_api.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/executions_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/api/groups_api.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/groups_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/api/jobs_api.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/jobs_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/api/login_api.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/login_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/api/management_api.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/management_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/api/masking_jobs_api.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/masking_jobs_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/api/reporting_api.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/reporting_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/api/saml_login_api.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/saml_login_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/api/snapshots_api.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/snapshots_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/api/sources_api.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/sources_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/api/test_api.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/test_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/api/timeflows_api.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/timeflows_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/api/vcdbs_api.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/vcdbs_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/api/vdb_groups_api.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/vdb_groups_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/api/vdbs_api.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/vdbs_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/api/virtualization_policies_api.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/api/virtualization_policies_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/api_client.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/6.0.0/python'
+        self.user_agent = 'OpenAPI-Generator/6.0.0-rc1/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/apis/__init__.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/configuration.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -403,15 +403,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 3.1.0\n"\
-               "SDK Package Version: 6.0.0".\
+               "SDK Package Version: 6.0.0-rc1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/exceptions.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/exceptions.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/access_group.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/access_group.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/access_group_account_ids_request.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/access_group_account_ids_request.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/access_group_scope.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/access_group_scope.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/access_group_scopes_request.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/access_group_scopes_request.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/access_group_update_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/access_group_update_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/account.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/account.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/account_create_parameter.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/account_create_parameter.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/account_create_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/account_create_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/account_login_parameter.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/account_login_parameter.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/account_update_parameter.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/account_update_parameter.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/additional_mount_point.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/additional_mount_point.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/all_object_permissions_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/all_object_permissions_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/always_allowed_permission.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/always_allowed_permission.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/always_allowed_permission_request.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/always_allowed_permission_request.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/api_classification_config.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/api_classification_config.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/api_classification_object.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/api_classification_object.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/api_usage_data.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/api_usage_data.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/api_usage_report_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/api_usage_report_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/base_provision_vdb_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/base_provision_vdb_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/base_provision_vdb_parameters_all_of.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/base_provision_vdb_parameters_all_of.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/bookmark.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/bookmark.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/bookmark_create_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/bookmark_create_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/cdb.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/cdb.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/change_password_parameter.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/change_password_parameter.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/connectivity_check_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/connectivity_check_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/connectivity_check_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/connectivity_check_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/connector.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/connector.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/connector_test_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/connector_test_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/connector_update_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/connector_update_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/copy_masking_job_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/copy_masking_job_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/copy_masking_job_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/copy_masking_job_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/create_bookmark_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/create_bookmark_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/create_database_template_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/create_database_template_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/create_environment_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/create_environment_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/create_environment_user_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/create_environment_user_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/create_host_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/create_host_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/create_role.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/create_role.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/create_vdb_group_request.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/create_vdb_group_request.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/create_vdb_group_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/create_vdb_group_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/d_source.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/d_source.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/d_source_consumption_data.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/d_source_consumption_data.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/d_source_consumption_report_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/d_source_consumption_report_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/d_source_snapshot_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/d_source_snapshot_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/d_source_usage_data.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/d_source_usage_data.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/d_source_usage_report_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/d_source_usage_report_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/data_point_by_snapshot_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/data_point_by_snapshot_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/data_point_by_timestamp_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/data_point_by_timestamp_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/data_point_from_bookmark_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/data_point_from_bookmark_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/database_template.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/database_template.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/database_template_create_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/database_template_create_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/dataset_group.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/dataset_group.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/delete_database_template_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/delete_database_template_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/delete_engine_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/delete_engine_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/delete_environment_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/delete_environment_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/delete_environment_user_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/delete_environment_user_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/delete_host_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/delete_host_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/delete_masking_job_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/delete_masking_job_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/delete_scope_object_tags.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/delete_scope_object_tags.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/delete_scoped_object_item.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/delete_scoped_object_item.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/delete_snapshot_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/delete_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/delete_tag.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/delete_tag.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/delete_timeflow_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/delete_timeflow_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/delete_vdb_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/delete_vdb_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/delete_vdb_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/delete_vdb_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/disable_environment_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/disable_environment_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/disable_vdb_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/disable_vdb_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/disable_vdb_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/disable_vdb_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/domain.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/domain.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/effective_scope.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/effective_scope.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/enable_environment_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/enable_environment_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/enable_vdb_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/enable_vdb_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/enable_vdb_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/enable_vdb_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/engine.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/engine.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/engine_id_body.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/engine_id_body.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/engine_registration_parameter.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/engine_registration_parameter.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/environment.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/environment.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/environment_create_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/environment_create_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/environment_repository.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/environment_repository.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/environment_repository_all_of.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/environment_repository_all_of.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/environment_update_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/environment_update_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/environment_user.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/environment_user.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/environment_user_params.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/environment_user_params.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/error.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/error.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/error_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/error_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/errors.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/errors.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/execute_masking_job_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/execute_masking_job_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/execute_masking_job_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/execute_masking_job_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/execution.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/execution.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/execution_cancel_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/execution_cancel_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/global_properties.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/global_properties.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/hashicorp_vault.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/hashicorp_vault.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/hook.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/hook.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/host.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/host.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/host_create_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/host_create_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/host_update_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/host_update_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/job.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/job.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/ldap_config_params.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/ldap_config_params.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/ldap_config_validate_parameter.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/ldap_config_validate_parameter.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/ldap_validate_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/ldap_validate_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/link_d_source_default_request.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/link_d_source_default_request.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/link_d_source_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/link_d_source_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/link_d_source_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/link_d_source_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/list_access_groups_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_access_groups_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/list_accounts_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_accounts_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/list_bookmarks_by_vdb_groups_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_bookmarks_by_vdb_groups_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/list_bookmarks_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_bookmarks_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/list_cdbs_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_cdbs_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/list_connectors_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_connectors_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/list_d_sources_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_d_sources_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/list_database_templates_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_database_templates_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/list_environment_users.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_environment_users.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/list_environments_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_environments_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/list_executions_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_executions_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/list_groups_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_groups_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/list_hashicorp_vaults_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_hashicorp_vaults_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/list_jobs_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_jobs_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/list_masking_job_source_engines_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_masking_job_source_engines_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/list_masking_jobs_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_masking_jobs_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/list_registered_engines_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_registered_engines_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/list_reporting_schedule_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_reporting_schedule_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/list_roles_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_roles_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/list_snapshots_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_snapshots_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/list_sources_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_sources_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/list_timeflows_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_timeflows_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/list_vcdbs_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_vcdbs_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/list_vdb_groups_by_bookmark_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_vdb_groups_by_bookmark_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/list_vdb_groups_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_vdb_groups_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/list_vdbs_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_vdbs_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/list_virtualization_policies_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/list_virtualization_policies_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/login_token.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/login_token.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/masking_job.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/masking_job.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/masking_job_connectors_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/masking_job_connectors_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/masking_job_source_engine.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/masking_job_source_engine.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/masking_ruleset.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/masking_ruleset.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/metadata_db_info.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/metadata_db_info.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/migrate_masking_job_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/migrate_masking_job_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/migrate_masking_job_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/migrate_masking_job_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/object_permission_access_groups.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/object_permission_access_groups.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/object_permission_account.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/object_permission_account.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/object_permissions_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/object_permissions_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/object_type_enum.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/object_type_enum.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/object_type_property.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/object_type_property.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/oracle_listener.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/oracle_listener.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/oracle_rac_custom_env_file.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/oracle_rac_custom_env_file.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/oracle_rac_custom_env_var.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/oracle_rac_custom_env_var.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/oracle_virtual_ip.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/oracle_virtual_ip.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/paginated_response_metadata.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/paginated_response_metadata.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/password_policies_params.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/password_policies_params.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/permission_enum.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/permission_enum.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/permission_object.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/permission_object.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/permission_property.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/permission_property.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/permissions_request.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/permissions_request.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/primary_environment_user_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/primary_environment_user_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/product_history.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/product_history.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/product_info.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/product_info.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/provision_vdb_from_bookmark_defaults_request.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/provision_vdb_from_bookmark_defaults_request.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/provision_vdb_from_bookmark_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/provision_vdb_from_bookmark_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/provision_vdb_from_bookmark_parameters_all_of.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/provision_vdb_from_bookmark_parameters_all_of.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/provision_vdb_group_from_bookmark_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/provision_vdb_group_from_bookmark_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/provision_vdb_group_from_bookmark_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/provision_vdb_group_from_bookmark_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/provision_vdb_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/provision_vdb_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/provision_vdbby_snapshot_defaults_request.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/provision_vdbby_snapshot_defaults_request.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/provision_vdbby_snapshot_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/provision_vdbby_snapshot_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/provision_vdbby_snapshot_parameters_all_of.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/provision_vdbby_snapshot_parameters_all_of.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/provision_vdbby_timestamp_defaults_request.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/provision_vdbby_timestamp_defaults_request.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/provision_vdbby_timestamp_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/provision_vdbby_timestamp_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/provision_vdbby_timestamp_parameters_all_of.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/provision_vdbby_timestamp_parameters_all_of.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/refresh_environment_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/refresh_environment_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/refresh_vdb_from_bookmark_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/refresh_vdb_from_bookmark_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/refresh_vdb_from_bookmark_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/refresh_vdb_from_bookmark_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/refresh_vdb_group_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/refresh_vdb_group_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/refresh_vdb_group_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/refresh_vdb_group_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/refresh_vdbby_location_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/refresh_vdbby_location_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/refresh_vdbby_location_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/refresh_vdbby_location_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/refresh_vdbby_snapshot_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/refresh_vdbby_snapshot_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/refresh_vdbby_snapshot_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/refresh_vdbby_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/refresh_vdbby_timestamp_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/refresh_vdbby_timestamp_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/refresh_vdbby_timestamp_parameters_all_of.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/refresh_vdbby_timestamp_parameters_all_of.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/refresh_vdbby_timestamp_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/refresh_vdbby_timestamp_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/registered_engine.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/registered_engine.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/remove_masking_job_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/remove_masking_job_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/reporting_schedule.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/reporting_schedule.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/reporting_schedule_create_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/reporting_schedule_create_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/repository.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/repository.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/reset_password_parameter.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/reset_password_parameter.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/role.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/role.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/role_all_of.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/role_all_of.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/role_update_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/role_update_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/rollback_vdb_from_bookmark_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/rollback_vdb_from_bookmark_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/rollback_vdb_from_bookmark_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/rollback_vdb_from_bookmark_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/rollback_vdb_group_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/rollback_vdb_group_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/rollback_vdb_group_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/rollback_vdb_group_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/rollback_vdbby_snapshot_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/rollback_vdbby_snapshot_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/rollback_vdbby_snapshot_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/rollback_vdbby_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/rollback_vdbby_timestamp_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/rollback_vdbby_timestamp_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/rollback_vdbby_timestamp_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/rollback_vdbby_timestamp_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/saml_config_params.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/saml_config_params.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/scope_tag.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/scope_tag.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/scope_tags_request.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/scope_tags_request.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/scope_tags_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/scope_tags_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/scoped_object_item.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/scoped_object_item.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/scoped_object_items_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/scoped_object_items_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/scoped_objects_request.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/scoped_objects_request.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/search_access_groups_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_access_groups_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/search_accounts_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_accounts_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/search_body.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_body.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/search_bookmarks_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_bookmarks_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/search_cdbs_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_cdbs_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/search_connectors_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_connectors_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/search_d_sources_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_d_sources_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/search_database_templates_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_database_templates_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/search_dataset_group_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_dataset_group_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/search_engines_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_engines_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/search_environments_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_environments_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/search_executions_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_executions_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/search_jobs_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_jobs_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/search_masking_job_source_engines_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_masking_job_source_engines_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/search_masking_jobs_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_masking_jobs_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/search_roles_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_roles_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/search_snapshots_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_snapshots_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/search_sources_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_sources_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/search_timeflows_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_timeflows_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/search_vcdbs_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_vcdbs_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/search_vdb_group_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_vdb_group_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/search_vdbs_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_vdbs_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/search_virtualization_policies_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/search_virtualization_policies_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/smtp_config_params.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/smtp_config_params.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/smtp_config_validate.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/smtp_config_validate.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/snapshot.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/snapshot.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/snapshot_compatible_repositories.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/snapshot_compatible_repositories.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/snapshot_compatible_repository_request.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/snapshot_compatible_repository_request.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/snapshot_d_source_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/snapshot_d_source_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/snapshot_day_range.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/snapshot_day_range.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/snapshot_vdb_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/snapshot_vdb_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/snapshots_day_ranges_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/snapshots_day_ranges_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/source.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/source.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/ssh_verification_strategy.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/ssh_verification_strategy.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/start_vdb_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/start_vdb_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/stop_vdb_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/stop_vdb_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/switch_timeflow_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/switch_timeflow_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/switch_timeflow_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/switch_timeflow_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/tag.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/tag.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/tags_request.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/tags_request.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/tags_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/tags_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/task_event.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/task_event.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/time_to_update_sources_request.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/time_to_update_sources_request.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/time_to_update_sources_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/time_to_update_sources_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/timeflow.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/timeflow.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/token_info_request.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/token_info_request.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/token_info_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/token_info_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/unset_snapshot_retention_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/unset_snapshot_retention_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/update_access_group_scope.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/update_access_group_scope.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/update_bookmark_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/update_bookmark_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/update_connector_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/update_connector_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/update_database_template_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/update_database_template_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/update_database_template_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/update_database_template_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/update_environment_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/update_environment_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/update_environment_user_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/update_environment_user_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/update_host_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/update_host_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/update_masking_job_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/update_masking_job_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/update_snapshot_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/update_snapshot_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/update_snapshot_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/update_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/update_timeflow_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/update_timeflow_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/update_timeflow_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/update_timeflow_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/update_vdb_group_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/update_vdb_group_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/update_vdb_parameters.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/update_vdb_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/update_vdb_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/update_vdb_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/vcdb.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/vcdb.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/vdb.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/vdb.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/vdb_group.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/vdb_group.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/vdb_inventory_data.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/vdb_inventory_data.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/vdb_inventory_report_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/vdb_inventory_report_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/virtual_dataset_hooks.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/virtual_dataset_hooks.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/virtualization_policy.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/virtualization_policy.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/virtualization_schedule.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/virtualization_schedule.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/virtualization_storage_summary_data.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/virtualization_storage_summary_data.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model/virtualization_storage_summary_report_response.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model/virtualization_storage_summary_report_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/model_utils.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/model_utils.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/models/__init__.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/models/__init__.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix/api/gateway/rest.py` & `delphix-dct-api-6.0.0rc1/delphix/api/gateway/rest.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/delphix_dct_api.egg-info/SOURCES.txt` & `delphix-dct-api-6.0.0rc1/delphix_dct_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/setup.py` & `delphix-dct-api-6.0.0rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "delphix-dct-api"
-VERSION = "6.0.0"
+VERSION = "6.0.0-rc1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `delphix-dct-api-6.0.0/test/test_access_group.py` & `delphix-dct-api-6.0.0rc1/test/test_access_group.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_access_group_account_ids_request.py` & `delphix-dct-api-6.0.0rc1/test/test_access_group_account_ids_request.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_access_group_scope.py` & `delphix-dct-api-6.0.0rc1/test/test_access_group_scope.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_access_group_scopes_request.py` & `delphix-dct-api-6.0.0rc1/test/test_access_group_scopes_request.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_access_group_update_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_access_group_update_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_account.py` & `delphix-dct-api-6.0.0rc1/test/test_account.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_account_create_parameter.py` & `delphix-dct-api-6.0.0rc1/test/test_account_create_parameter.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_account_create_response.py` & `delphix-dct-api-6.0.0rc1/test/test_account_create_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_account_login_parameter.py` & `delphix-dct-api-6.0.0rc1/test/test_account_login_parameter.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_account_update_parameter.py` & `delphix-dct-api-6.0.0rc1/test/test_account_update_parameter.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_accounts_api.py` & `delphix-dct-api-6.0.0rc1/test/test_accounts_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_additional_mount_point.py` & `delphix-dct-api-6.0.0rc1/test/test_additional_mount_point.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_all_object_permissions_response.py` & `delphix-dct-api-6.0.0rc1/test/test_all_object_permissions_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_always_allowed_permission.py` & `delphix-dct-api-6.0.0rc1/test/test_always_allowed_permission.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_always_allowed_permission_request.py` & `delphix-dct-api-6.0.0rc1/test/test_always_allowed_permission_request.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_api_classification_config.py` & `delphix-dct-api-6.0.0rc1/test/test_api_classification_config.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_api_classification_object.py` & `delphix-dct-api-6.0.0rc1/test/test_api_classification_object.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_api_usage_data.py` & `delphix-dct-api-6.0.0rc1/test/test_api_usage_data.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_api_usage_report_response.py` & `delphix-dct-api-6.0.0rc1/test/test_api_usage_report_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_authorization_api.py` & `delphix-dct-api-6.0.0rc1/test/test_authorization_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_base_provision_vdb_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_base_provision_vdb_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_base_provision_vdb_parameters_all_of.py` & `delphix-dct-api-6.0.0rc1/test/test_base_provision_vdb_parameters_all_of.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_bookmark.py` & `delphix-dct-api-6.0.0rc1/test/test_bookmark.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_bookmark_create_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_bookmark_create_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_bookmarks_api.py` & `delphix-dct-api-6.0.0rc1/test/test_bookmarks_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_cdb.py` & `delphix-dct-api-6.0.0rc1/test/test_cdb.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_cdbs_api.py` & `delphix-dct-api-6.0.0rc1/test/test_cdbs_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_change_password_parameter.py` & `delphix-dct-api-6.0.0rc1/test/test_change_password_parameter.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_connectivity_api.py` & `delphix-dct-api-6.0.0rc1/test/test_connectivity_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_connectivity_check_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_connectivity_check_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_connectivity_check_response.py` & `delphix-dct-api-6.0.0rc1/test/test_connectivity_check_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_connector.py` & `delphix-dct-api-6.0.0rc1/test/test_connector.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_connector_test_response.py` & `delphix-dct-api-6.0.0rc1/test/test_connector_test_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_connector_update_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_connector_update_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_connectors_api.py` & `delphix-dct-api-6.0.0rc1/test/test_connectors_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_copy_masking_job_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_copy_masking_job_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_copy_masking_job_response.py` & `delphix-dct-api-6.0.0rc1/test/test_copy_masking_job_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_create_bookmark_response.py` & `delphix-dct-api-6.0.0rc1/test/test_create_bookmark_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_create_database_template_response.py` & `delphix-dct-api-6.0.0rc1/test/test_create_database_template_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_create_environment_response.py` & `delphix-dct-api-6.0.0rc1/test/test_create_environment_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_create_environment_user_response.py` & `delphix-dct-api-6.0.0rc1/test/test_create_environment_user_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_create_host_response.py` & `delphix-dct-api-6.0.0rc1/test/test_create_host_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_create_role.py` & `delphix-dct-api-6.0.0rc1/test/test_create_role.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_create_vdb_group_request.py` & `delphix-dct-api-6.0.0rc1/test/test_create_vdb_group_request.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_create_vdb_group_response.py` & `delphix-dct-api-6.0.0rc1/test/test_create_vdb_group_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_d_source.py` & `delphix-dct-api-6.0.0rc1/test/test_d_source.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_d_source_consumption_data.py` & `delphix-dct-api-6.0.0rc1/test/test_d_source_consumption_data.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_d_source_consumption_report_response.py` & `delphix-dct-api-6.0.0rc1/test/test_d_source_consumption_report_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_d_source_snapshot_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_d_source_snapshot_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_d_source_usage_data.py` & `delphix-dct-api-6.0.0rc1/test/test_d_source_usage_data.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_d_source_usage_report_response.py` & `delphix-dct-api-6.0.0rc1/test/test_d_source_usage_report_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_d_sources_api.py` & `delphix-dct-api-6.0.0rc1/test/test_d_sources_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_data_point_by_snapshot_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_data_point_by_snapshot_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_data_point_by_timestamp_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_data_point_by_timestamp_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_data_point_from_bookmark_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_data_point_from_bookmark_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_database_template.py` & `delphix-dct-api-6.0.0rc1/test/test_database_template.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_database_template_create_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_database_template_create_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_database_templates_api.py` & `delphix-dct-api-6.0.0rc1/test/test_database_templates_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_dataset_group.py` & `delphix-dct-api-6.0.0rc1/test/test_dataset_group.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_delete_database_template_response.py` & `delphix-dct-api-6.0.0rc1/test/test_delete_database_template_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_delete_engine_response.py` & `delphix-dct-api-6.0.0rc1/test/test_delete_engine_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_delete_environment_response.py` & `delphix-dct-api-6.0.0rc1/test/test_delete_environment_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_delete_environment_user_response.py` & `delphix-dct-api-6.0.0rc1/test/test_delete_environment_user_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_delete_host_response.py` & `delphix-dct-api-6.0.0rc1/test/test_delete_host_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_delete_masking_job_response.py` & `delphix-dct-api-6.0.0rc1/test/test_delete_masking_job_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_delete_scope_object_tags.py` & `delphix-dct-api-6.0.0rc1/test/test_delete_scope_object_tags.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_delete_scoped_object_item.py` & `delphix-dct-api-6.0.0rc1/test/test_delete_scoped_object_item.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_delete_snapshot_response.py` & `delphix-dct-api-6.0.0rc1/test/test_delete_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_delete_tag.py` & `delphix-dct-api-6.0.0rc1/test/test_delete_tag.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_delete_timeflow_response.py` & `delphix-dct-api-6.0.0rc1/test/test_delete_timeflow_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_delete_vdb_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_delete_vdb_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_delete_vdb_response.py` & `delphix-dct-api-6.0.0rc1/test/test_delete_vdb_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_disable_environment_response.py` & `delphix-dct-api-6.0.0rc1/test/test_disable_environment_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_disable_vdb_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_disable_vdb_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_disable_vdb_response.py` & `delphix-dct-api-6.0.0rc1/test/test_disable_vdb_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_domain.py` & `delphix-dct-api-6.0.0rc1/test/test_domain.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_effective_scope.py` & `delphix-dct-api-6.0.0rc1/test/test_effective_scope.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_enable_environment_response.py` & `delphix-dct-api-6.0.0rc1/test/test_enable_environment_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_enable_vdb_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_enable_vdb_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_enable_vdb_response.py` & `delphix-dct-api-6.0.0rc1/test/test_enable_vdb_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_engine.py` & `delphix-dct-api-6.0.0rc1/test/test_engine.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_engine_id_body.py` & `delphix-dct-api-6.0.0rc1/test/test_engine_id_body.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_engine_registration_parameter.py` & `delphix-dct-api-6.0.0rc1/test/test_engine_registration_parameter.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_environment.py` & `delphix-dct-api-6.0.0rc1/test/test_environment.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_environment_create_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_environment_create_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_environment_repository.py` & `delphix-dct-api-6.0.0rc1/test/test_environment_repository.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_environment_repository_all_of.py` & `delphix-dct-api-6.0.0rc1/test/test_environment_repository_all_of.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_environment_update_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_environment_update_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_environment_user.py` & `delphix-dct-api-6.0.0rc1/test/test_environment_user.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_environment_user_params.py` & `delphix-dct-api-6.0.0rc1/test/test_environment_user_params.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_environments_api.py` & `delphix-dct-api-6.0.0rc1/test/test_environments_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_error.py` & `delphix-dct-api-6.0.0rc1/test/test_error.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_error_response.py` & `delphix-dct-api-6.0.0rc1/test/test_error_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_errors.py` & `delphix-dct-api-6.0.0rc1/test/test_errors.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_execute_masking_job_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_execute_masking_job_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_execute_masking_job_response.py` & `delphix-dct-api-6.0.0rc1/test/test_execute_masking_job_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_execution.py` & `delphix-dct-api-6.0.0rc1/test/test_execution.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_execution_cancel_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_execution_cancel_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_executions_api.py` & `delphix-dct-api-6.0.0rc1/test/test_executions_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_global_properties.py` & `delphix-dct-api-6.0.0rc1/test/test_global_properties.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_groups_api.py` & `delphix-dct-api-6.0.0rc1/test/test_groups_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_hashicorp_vault.py` & `delphix-dct-api-6.0.0rc1/test/test_hashicorp_vault.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_hook.py` & `delphix-dct-api-6.0.0rc1/test/test_hook.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_host.py` & `delphix-dct-api-6.0.0rc1/test/test_host.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_host_create_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_host_create_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_host_update_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_host_update_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_job.py` & `delphix-dct-api-6.0.0rc1/test/test_job.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_jobs_api.py` & `delphix-dct-api-6.0.0rc1/test/test_jobs_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_ldap_config_params.py` & `delphix-dct-api-6.0.0rc1/test/test_ldap_config_params.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_ldap_config_validate_parameter.py` & `delphix-dct-api-6.0.0rc1/test/test_ldap_config_validate_parameter.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_ldap_validate_response.py` & `delphix-dct-api-6.0.0rc1/test/test_ldap_validate_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_link_d_source_default_request.py` & `delphix-dct-api-6.0.0rc1/test/test_link_d_source_default_request.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_link_d_source_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_link_d_source_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_link_d_source_response.py` & `delphix-dct-api-6.0.0rc1/test/test_link_d_source_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_list_access_groups_response.py` & `delphix-dct-api-6.0.0rc1/test/test_list_access_groups_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_list_accounts_response.py` & `delphix-dct-api-6.0.0rc1/test/test_list_accounts_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_list_bookmarks_by_vdb_groups_response.py` & `delphix-dct-api-6.0.0rc1/test/test_list_bookmarks_by_vdb_groups_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_list_bookmarks_response.py` & `delphix-dct-api-6.0.0rc1/test/test_list_bookmarks_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_list_cdbs_response.py` & `delphix-dct-api-6.0.0rc1/test/test_list_cdbs_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_list_connectors_response.py` & `delphix-dct-api-6.0.0rc1/test/test_list_connectors_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_list_d_sources_response.py` & `delphix-dct-api-6.0.0rc1/test/test_list_d_sources_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_list_database_templates_response.py` & `delphix-dct-api-6.0.0rc1/test/test_list_database_templates_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_list_environment_users.py` & `delphix-dct-api-6.0.0rc1/test/test_list_environment_users.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_list_environments_response.py` & `delphix-dct-api-6.0.0rc1/test/test_list_environments_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_list_executions_response.py` & `delphix-dct-api-6.0.0rc1/test/test_list_executions_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_list_groups_response.py` & `delphix-dct-api-6.0.0rc1/test/test_list_groups_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_list_hashicorp_vaults_response.py` & `delphix-dct-api-6.0.0rc1/test/test_list_hashicorp_vaults_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_list_jobs_response.py` & `delphix-dct-api-6.0.0rc1/test/test_list_jobs_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_list_masking_job_source_engines_response.py` & `delphix-dct-api-6.0.0rc1/test/test_list_masking_job_source_engines_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_list_masking_jobs_response.py` & `delphix-dct-api-6.0.0rc1/test/test_list_masking_jobs_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_list_registered_engines_response.py` & `delphix-dct-api-6.0.0rc1/test/test_list_registered_engines_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_list_reporting_schedule_response.py` & `delphix-dct-api-6.0.0rc1/test/test_list_reporting_schedule_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_list_roles_response.py` & `delphix-dct-api-6.0.0rc1/test/test_list_roles_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_list_snapshots_response.py` & `delphix-dct-api-6.0.0rc1/test/test_list_snapshots_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_list_sources_response.py` & `delphix-dct-api-6.0.0rc1/test/test_list_sources_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_list_timeflows_response.py` & `delphix-dct-api-6.0.0rc1/test/test_list_timeflows_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_list_vcdbs_response.py` & `delphix-dct-api-6.0.0rc1/test/test_list_vcdbs_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_list_vdb_groups_by_bookmark_response.py` & `delphix-dct-api-6.0.0rc1/test/test_list_vdb_groups_by_bookmark_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_list_vdb_groups_response.py` & `delphix-dct-api-6.0.0rc1/test/test_list_vdb_groups_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_list_vdbs_response.py` & `delphix-dct-api-6.0.0rc1/test/test_list_vdbs_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_list_virtualization_policies_response.py` & `delphix-dct-api-6.0.0rc1/test/test_list_virtualization_policies_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_login_api.py` & `delphix-dct-api-6.0.0rc1/test/test_login_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_login_token.py` & `delphix-dct-api-6.0.0rc1/test/test_login_token.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_management_api.py` & `delphix-dct-api-6.0.0rc1/test/test_management_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_masking_job.py` & `delphix-dct-api-6.0.0rc1/test/test_masking_job.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_masking_job_connectors_response.py` & `delphix-dct-api-6.0.0rc1/test/test_masking_job_connectors_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_masking_job_source_engine.py` & `delphix-dct-api-6.0.0rc1/test/test_masking_job_source_engine.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_masking_jobs_api.py` & `delphix-dct-api-6.0.0rc1/test/test_masking_jobs_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_masking_ruleset.py` & `delphix-dct-api-6.0.0rc1/test/test_masking_ruleset.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_metadata_db_info.py` & `delphix-dct-api-6.0.0rc1/test/test_metadata_db_info.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_migrate_masking_job_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_migrate_masking_job_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_migrate_masking_job_response.py` & `delphix-dct-api-6.0.0rc1/test/test_migrate_masking_job_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_object_permission_access_groups.py` & `delphix-dct-api-6.0.0rc1/test/test_object_permission_access_groups.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_object_permission_account.py` & `delphix-dct-api-6.0.0rc1/test/test_object_permission_account.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_object_permissions_response.py` & `delphix-dct-api-6.0.0rc1/test/test_object_permissions_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_object_type_enum.py` & `delphix-dct-api-6.0.0rc1/test/test_object_type_enum.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_object_type_property.py` & `delphix-dct-api-6.0.0rc1/test/test_object_type_property.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_oracle_listener.py` & `delphix-dct-api-6.0.0rc1/test/test_oracle_listener.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_oracle_rac_custom_env_file.py` & `delphix-dct-api-6.0.0rc1/test/test_oracle_rac_custom_env_file.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_oracle_rac_custom_env_var.py` & `delphix-dct-api-6.0.0rc1/test/test_oracle_rac_custom_env_var.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_oracle_virtual_ip.py` & `delphix-dct-api-6.0.0rc1/test/test_oracle_virtual_ip.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_paginated_response_metadata.py` & `delphix-dct-api-6.0.0rc1/test/test_paginated_response_metadata.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_password_policies_params.py` & `delphix-dct-api-6.0.0rc1/test/test_password_policies_params.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_permission_enum.py` & `delphix-dct-api-6.0.0rc1/test/test_permission_enum.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_permission_object.py` & `delphix-dct-api-6.0.0rc1/test/test_permission_object.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_permission_property.py` & `delphix-dct-api-6.0.0rc1/test/test_permission_property.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_permissions_request.py` & `delphix-dct-api-6.0.0rc1/test/test_permissions_request.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_primary_environment_user_response.py` & `delphix-dct-api-6.0.0rc1/test/test_primary_environment_user_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_product_history.py` & `delphix-dct-api-6.0.0rc1/test/test_product_history.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_product_info.py` & `delphix-dct-api-6.0.0rc1/test/test_product_info.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_provision_vdb_from_bookmark_defaults_request.py` & `delphix-dct-api-6.0.0rc1/test/test_provision_vdb_from_bookmark_defaults_request.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_provision_vdb_from_bookmark_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_provision_vdb_from_bookmark_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_provision_vdb_from_bookmark_parameters_all_of.py` & `delphix-dct-api-6.0.0rc1/test/test_provision_vdb_from_bookmark_parameters_all_of.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_provision_vdb_group_from_bookmark_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_provision_vdb_group_from_bookmark_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_provision_vdb_group_from_bookmark_response.py` & `delphix-dct-api-6.0.0rc1/test/test_provision_vdb_group_from_bookmark_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_provision_vdb_response.py` & `delphix-dct-api-6.0.0rc1/test/test_provision_vdb_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_provision_vdbby_snapshot_defaults_request.py` & `delphix-dct-api-6.0.0rc1/test/test_provision_vdbby_snapshot_defaults_request.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_provision_vdbby_snapshot_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_provision_vdbby_snapshot_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_provision_vdbby_snapshot_parameters_all_of.py` & `delphix-dct-api-6.0.0rc1/test/test_provision_vdbby_snapshot_parameters_all_of.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_provision_vdbby_timestamp_defaults_request.py` & `delphix-dct-api-6.0.0rc1/test/test_provision_vdbby_timestamp_defaults_request.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_provision_vdbby_timestamp_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_provision_vdbby_timestamp_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_provision_vdbby_timestamp_parameters_all_of.py` & `delphix-dct-api-6.0.0rc1/test/test_provision_vdbby_timestamp_parameters_all_of.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_refresh_environment_response.py` & `delphix-dct-api-6.0.0rc1/test/test_refresh_environment_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_refresh_vdb_from_bookmark_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_refresh_vdb_from_bookmark_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_refresh_vdb_from_bookmark_response.py` & `delphix-dct-api-6.0.0rc1/test/test_refresh_vdb_from_bookmark_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_refresh_vdb_group_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_refresh_vdb_group_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_refresh_vdb_group_response.py` & `delphix-dct-api-6.0.0rc1/test/test_refresh_vdb_group_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_refresh_vdbby_location_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_refresh_vdbby_location_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_refresh_vdbby_location_response.py` & `delphix-dct-api-6.0.0rc1/test/test_refresh_vdbby_location_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_refresh_vdbby_snapshot_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_refresh_vdbby_snapshot_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_refresh_vdbby_snapshot_response.py` & `delphix-dct-api-6.0.0rc1/test/test_refresh_vdbby_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_refresh_vdbby_timestamp_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_refresh_vdbby_timestamp_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_refresh_vdbby_timestamp_parameters_all_of.py` & `delphix-dct-api-6.0.0rc1/test/test_refresh_vdbby_timestamp_parameters_all_of.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_refresh_vdbby_timestamp_response.py` & `delphix-dct-api-6.0.0rc1/test/test_refresh_vdbby_timestamp_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_registered_engine.py` & `delphix-dct-api-6.0.0rc1/test/test_registered_engine.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_remove_masking_job_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_remove_masking_job_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_reporting_api.py` & `delphix-dct-api-6.0.0rc1/test/test_reporting_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_reporting_schedule.py` & `delphix-dct-api-6.0.0rc1/test/test_reporting_schedule.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_reporting_schedule_create_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_reporting_schedule_create_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_repository.py` & `delphix-dct-api-6.0.0rc1/test/test_repository.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_reset_password_parameter.py` & `delphix-dct-api-6.0.0rc1/test/test_reset_password_parameter.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_role.py` & `delphix-dct-api-6.0.0rc1/test/test_role.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_role_all_of.py` & `delphix-dct-api-6.0.0rc1/test/test_role_all_of.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_role_update_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_role_update_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_rollback_vdb_from_bookmark_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_rollback_vdb_from_bookmark_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_rollback_vdb_from_bookmark_response.py` & `delphix-dct-api-6.0.0rc1/test/test_rollback_vdb_from_bookmark_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_rollback_vdb_group_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_rollback_vdb_group_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_rollback_vdb_group_response.py` & `delphix-dct-api-6.0.0rc1/test/test_rollback_vdb_group_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_rollback_vdbby_snapshot_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_rollback_vdbby_snapshot_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_rollback_vdbby_snapshot_response.py` & `delphix-dct-api-6.0.0rc1/test/test_rollback_vdbby_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_rollback_vdbby_timestamp_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_rollback_vdbby_timestamp_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_rollback_vdbby_timestamp_response.py` & `delphix-dct-api-6.0.0rc1/test/test_rollback_vdbby_timestamp_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_saml_config_params.py` & `delphix-dct-api-6.0.0rc1/test/test_saml_config_params.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_saml_login_api.py` & `delphix-dct-api-6.0.0rc1/test/test_saml_login_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_scope_tag.py` & `delphix-dct-api-6.0.0rc1/test/test_scope_tag.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_scope_tags_request.py` & `delphix-dct-api-6.0.0rc1/test/test_scope_tags_request.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_scope_tags_response.py` & `delphix-dct-api-6.0.0rc1/test/test_scope_tags_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_scoped_object_item.py` & `delphix-dct-api-6.0.0rc1/test/test_scoped_object_item.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_scoped_object_items_response.py` & `delphix-dct-api-6.0.0rc1/test/test_scoped_object_items_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_scoped_objects_request.py` & `delphix-dct-api-6.0.0rc1/test/test_scoped_objects_request.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_search_access_groups_response.py` & `delphix-dct-api-6.0.0rc1/test/test_search_access_groups_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_search_accounts_response.py` & `delphix-dct-api-6.0.0rc1/test/test_search_accounts_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_search_body.py` & `delphix-dct-api-6.0.0rc1/test/test_search_body.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_search_bookmarks_response.py` & `delphix-dct-api-6.0.0rc1/test/test_search_bookmarks_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_search_cdbs_response.py` & `delphix-dct-api-6.0.0rc1/test/test_search_cdbs_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_search_connectors_response.py` & `delphix-dct-api-6.0.0rc1/test/test_search_connectors_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_search_d_sources_response.py` & `delphix-dct-api-6.0.0rc1/test/test_search_d_sources_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_search_database_templates_response.py` & `delphix-dct-api-6.0.0rc1/test/test_search_database_templates_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_search_dataset_group_response.py` & `delphix-dct-api-6.0.0rc1/test/test_search_dataset_group_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_search_engines_response.py` & `delphix-dct-api-6.0.0rc1/test/test_search_engines_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_search_environments_response.py` & `delphix-dct-api-6.0.0rc1/test/test_search_environments_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_search_executions_response.py` & `delphix-dct-api-6.0.0rc1/test/test_search_executions_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_search_jobs_response.py` & `delphix-dct-api-6.0.0rc1/test/test_search_jobs_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_search_masking_job_source_engines_response.py` & `delphix-dct-api-6.0.0rc1/test/test_search_masking_job_source_engines_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_search_masking_jobs_response.py` & `delphix-dct-api-6.0.0rc1/test/test_search_masking_jobs_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_search_roles_response.py` & `delphix-dct-api-6.0.0rc1/test/test_search_roles_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_search_snapshots_response.py` & `delphix-dct-api-6.0.0rc1/test/test_search_snapshots_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_search_sources_response.py` & `delphix-dct-api-6.0.0rc1/test/test_search_sources_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_search_timeflows_response.py` & `delphix-dct-api-6.0.0rc1/test/test_search_timeflows_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_search_vcdbs_response.py` & `delphix-dct-api-6.0.0rc1/test/test_search_vcdbs_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_search_vdb_group_response.py` & `delphix-dct-api-6.0.0rc1/test/test_search_vdb_group_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_search_vdbs_response.py` & `delphix-dct-api-6.0.0rc1/test/test_search_vdbs_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_search_virtualization_policies_response.py` & `delphix-dct-api-6.0.0rc1/test/test_search_virtualization_policies_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_smtp_config_params.py` & `delphix-dct-api-6.0.0rc1/test/test_smtp_config_params.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_smtp_config_validate.py` & `delphix-dct-api-6.0.0rc1/test/test_smtp_config_validate.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_snapshot.py` & `delphix-dct-api-6.0.0rc1/test/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_snapshot_compatible_repositories.py` & `delphix-dct-api-6.0.0rc1/test/test_snapshot_compatible_repositories.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_snapshot_compatible_repository_request.py` & `delphix-dct-api-6.0.0rc1/test/test_snapshot_compatible_repository_request.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_snapshot_d_source_response.py` & `delphix-dct-api-6.0.0rc1/test/test_snapshot_d_source_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_snapshot_day_range.py` & `delphix-dct-api-6.0.0rc1/test/test_snapshot_day_range.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_snapshot_vdb_response.py` & `delphix-dct-api-6.0.0rc1/test/test_snapshot_vdb_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_snapshots_api.py` & `delphix-dct-api-6.0.0rc1/test/test_snapshots_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_snapshots_day_ranges_response.py` & `delphix-dct-api-6.0.0rc1/test/test_snapshots_day_ranges_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_source.py` & `delphix-dct-api-6.0.0rc1/test/test_source.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_sources_api.py` & `delphix-dct-api-6.0.0rc1/test/test_sources_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_ssh_verification_strategy.py` & `delphix-dct-api-6.0.0rc1/test/test_ssh_verification_strategy.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_start_vdb_response.py` & `delphix-dct-api-6.0.0rc1/test/test_start_vdb_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_stop_vdb_response.py` & `delphix-dct-api-6.0.0rc1/test/test_stop_vdb_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_switch_timeflow_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_switch_timeflow_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_switch_timeflow_response.py` & `delphix-dct-api-6.0.0rc1/test/test_switch_timeflow_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_tag.py` & `delphix-dct-api-6.0.0rc1/test/test_tag.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_tags_request.py` & `delphix-dct-api-6.0.0rc1/test/test_tags_request.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_tags_response.py` & `delphix-dct-api-6.0.0rc1/test/test_tags_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_task_event.py` & `delphix-dct-api-6.0.0rc1/test/test_task_event.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_test_api.py` & `delphix-dct-api-6.0.0rc1/test/test_test_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_time_to_update_sources_request.py` & `delphix-dct-api-6.0.0rc1/test/test_time_to_update_sources_request.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_time_to_update_sources_response.py` & `delphix-dct-api-6.0.0rc1/test/test_time_to_update_sources_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_timeflow.py` & `delphix-dct-api-6.0.0rc1/test/test_timeflow.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_timeflows_api.py` & `delphix-dct-api-6.0.0rc1/test/test_timeflows_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_token_info_request.py` & `delphix-dct-api-6.0.0rc1/test/test_token_info_request.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_token_info_response.py` & `delphix-dct-api-6.0.0rc1/test/test_token_info_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_unset_snapshot_retention_response.py` & `delphix-dct-api-6.0.0rc1/test/test_unset_snapshot_retention_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_update_access_group_scope.py` & `delphix-dct-api-6.0.0rc1/test/test_update_access_group_scope.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_update_bookmark_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_update_bookmark_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_update_connector_response.py` & `delphix-dct-api-6.0.0rc1/test/test_update_connector_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_update_database_template_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_update_database_template_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_update_database_template_response.py` & `delphix-dct-api-6.0.0rc1/test/test_update_database_template_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_update_environment_response.py` & `delphix-dct-api-6.0.0rc1/test/test_update_environment_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_update_environment_user_response.py` & `delphix-dct-api-6.0.0rc1/test/test_update_environment_user_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_update_host_response.py` & `delphix-dct-api-6.0.0rc1/test/test_update_host_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_update_masking_job_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_update_masking_job_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_update_snapshot_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_update_snapshot_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_update_snapshot_response.py` & `delphix-dct-api-6.0.0rc1/test/test_update_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_update_timeflow_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_update_timeflow_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_update_timeflow_response.py` & `delphix-dct-api-6.0.0rc1/test/test_update_timeflow_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_update_vdb_group_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_update_vdb_group_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_update_vdb_parameters.py` & `delphix-dct-api-6.0.0rc1/test/test_update_vdb_parameters.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_update_vdb_response.py` & `delphix-dct-api-6.0.0rc1/test/test_update_vdb_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_vcdb.py` & `delphix-dct-api-6.0.0rc1/test/test_vcdb.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_vcdbs_api.py` & `delphix-dct-api-6.0.0rc1/test/test_vcdbs_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_vdb.py` & `delphix-dct-api-6.0.0rc1/test/test_vdb.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_vdb_group.py` & `delphix-dct-api-6.0.0rc1/test/test_vdb_group.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_vdb_groups_api.py` & `delphix-dct-api-6.0.0rc1/test/test_vdb_groups_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_vdb_inventory_data.py` & `delphix-dct-api-6.0.0rc1/test/test_vdb_inventory_data.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_vdb_inventory_report_response.py` & `delphix-dct-api-6.0.0rc1/test/test_vdb_inventory_report_response.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_vdbs_api.py` & `delphix-dct-api-6.0.0rc1/test/test_vdbs_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_virtual_dataset_hooks.py` & `delphix-dct-api-6.0.0rc1/test/test_virtual_dataset_hooks.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_virtualization_policies_api.py` & `delphix-dct-api-6.0.0rc1/test/test_virtualization_policies_api.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_virtualization_policy.py` & `delphix-dct-api-6.0.0rc1/test/test_virtualization_policy.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_virtualization_schedule.py` & `delphix-dct-api-6.0.0rc1/test/test_virtualization_schedule.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_virtualization_storage_summary_data.py` & `delphix-dct-api-6.0.0rc1/test/test_virtualization_storage_summary_data.py`

 * *Files identical despite different names*

### Comparing `delphix-dct-api-6.0.0/test/test_virtualization_storage_summary_report_response.py` & `delphix-dct-api-6.0.0rc1/test/test_virtualization_storage_summary_report_response.py`

 * *Files identical despite different names*

