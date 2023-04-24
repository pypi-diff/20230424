# Comparing `tmp/vdk-control-service-api-1.0.6.tar.gz` & `tmp/vdk-control-service-api-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vdk-control-service-api-1.0.6.tar", last modified: Thu Dec 16 09:57:42 2021, max compression
+gzip compressed data, was "vdk-control-service-api-1.0.7.tar", last modified: Mon Apr 24 11:09:21 2023, max compression
```

## Comparing `vdk-control-service-api-1.0.6.tar` & `vdk-control-service-api-1.0.7.tar`

### file list

```diff
@@ -1,70 +1,196 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-16 09:57:42.000000 vdk-control-service-api-1.0.6/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-16 09:57:42.000000 vdk-control-service-api-1.0.6/taurus_datajob_api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-16 09:57:42.000000 vdk-control-service-api-1.0.6/taurus_datajob_api/api/
--rw-r--r--   0 root         (0) root         (0)      544 2021-12-16 09:57:40.000000 vdk-control-service-api-1.0.6/taurus_datajob_api/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    66382 2021-12-16 09:57:37.000000 vdk-control-service-api-1.0.6/taurus_datajob_api/api/data_jobs_api.py
--rw-r--r--   0 root         (0) root         (0)    39513 2021-12-16 09:57:37.000000 vdk-control-service-api-1.0.6/taurus_datajob_api/api/data_jobs_deployment_api.py
--rw-r--r--   0 root         (0) root         (0)    46242 2021-12-16 09:57:37.000000 vdk-control-service-api-1.0.6/taurus_datajob_api/api/data_jobs_execution_api.py
--rw-r--r--   0 root         (0) root         (0)    17600 2021-12-16 09:57:37.000000 vdk-control-service-api-1.0.6/taurus_datajob_api/api/data_jobs_properties_api.py
--rw-r--r--   0 root         (0) root         (0)     8604 2021-12-16 09:57:37.000000 vdk-control-service-api-1.0.6/taurus_datajob_api/api/data_jobs_service_api.py
--rw-r--r--   0 root         (0) root         (0)    23401 2021-12-16 09:57:37.000000 vdk-control-service-api-1.0.6/taurus_datajob_api/api/data_jobs_sources_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-16 09:57:42.000000 vdk-control-service-api-1.0.6/taurus_datajob_api/models/
--rw-r--r--   0 root         (0) root         (0)     4354 2021-12-16 09:57:40.000000 vdk-control-service-api-1.0.6/taurus_datajob_api/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8586 2021-12-16 09:57:34.000000 vdk-control-service-api-1.0.6/taurus_datajob_api/models/data_job.py
--rw-r--r--   0 root         (0) root         (0)     6251 2021-12-16 09:57:34.000000 vdk-control-service-api-1.0.6/taurus_datajob_api/models/data_job_api_info.py
--rw-r--r--   0 root         (0) root         (0)    12042 2021-12-16 09:57:34.000000 vdk-control-service-api-1.0.6/taurus_datajob_api/models/data_job_config.py
--rw-r--r--   0 root         (0) root         (0)    10787 2021-12-16 09:57:34.000000 vdk-control-service-api-1.0.6/taurus_datajob_api/models/data_job_contacts.py
--rw-r--r--   0 root         (0) root         (0)    13289 2021-12-16 09:57:34.000000 vdk-control-service-api-1.0.6/taurus_datajob_api/models/data_job_deployment.py
--rw-r--r--   0 root         (0) root         (0)    14551 2021-12-16 09:57:34.000000 vdk-control-service-api-1.0.6/taurus_datajob_api/models/data_job_deployment_status.py
--rw-r--r--   0 root         (0) root         (0)    15164 2021-12-16 09:57:34.000000 vdk-control-service-api-1.0.6/taurus_datajob_api/models/data_job_execution.py
--rw-r--r--   0 root         (0) root         (0)     6114 2021-12-16 09:57:34.000000 vdk-control-service-api-1.0.6/taurus_datajob_api/models/data_job_execution_logs.py
--rw-r--r--   0 root         (0) root         (0)     7135 2021-12-16 09:57:34.000000 vdk-control-service-api-1.0.6/taurus_datajob_api/models/data_job_execution_request.py
--rw-r--r--   0 root         (0) root         (0)     5499 2021-12-16 09:57:34.000000 vdk-control-service-api-1.0.6/taurus_datajob_api/models/data_job_mode.py
--rw-r--r--   0 root         (0) root         (0)     7779 2021-12-16 09:57:34.000000 vdk-control-service-api-1.0.6/taurus_datajob_api/models/data_job_page.py
--rw-r--r--   0 root         (0) root         (0)     6868 2021-12-16 09:57:34.000000 vdk-control-service-api-1.0.6/taurus_datajob_api/models/data_job_query_response.py
--rw-r--r--   0 root         (0) root         (0)     6976 2021-12-16 09:57:34.000000 vdk-control-service-api-1.0.6/taurus_datajob_api/models/data_job_query_response_with_error.py
--rw-r--r--   0 root         (0) root         (0)     8873 2021-12-16 09:57:34.000000 vdk-control-service-api-1.0.6/taurus_datajob_api/models/data_job_resources.py
--rw-r--r--   0 root         (0) root         (0)     7186 2021-12-16 09:57:34.000000 vdk-control-service-api-1.0.6/taurus_datajob_api/models/data_job_schedule.py
--rw-r--r--   0 root         (0) root         (0)     8808 2021-12-16 09:57:34.000000 vdk-control-service-api-1.0.6/taurus_datajob_api/models/data_job_summary.py
--rw-r--r--   0 root         (0) root         (0)     6433 2021-12-16 09:57:34.000000 vdk-control-service-api-1.0.6/taurus_datajob_api/models/data_job_version.py
--rw-r--r--   0 root         (0) root         (0)     6208 2021-12-16 09:57:34.000000 vdk-control-service-api-1.0.6/taurus_datajob_api/models/error.py
--rw-r--r--   0 root         (0) root         (0)     5275 2021-12-16 09:57:40.000000 vdk-control-service-api-1.0.6/taurus_datajob_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28250 2021-12-16 09:57:40.000000 vdk-control-service-api-1.0.6/taurus_datajob_api/api_client.py
--rw-r--r--   0 root         (0) root         (0)    15417 2021-12-16 09:57:40.000000 vdk-control-service-api-1.0.6/taurus_datajob_api/configuration.py
--rw-r--r--   0 root         (0) root         (0)     6459 2021-12-16 09:57:40.000000 vdk-control-service-api-1.0.6/taurus_datajob_api/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    15172 2021-12-16 09:57:40.000000 vdk-control-service-api-1.0.6/taurus_datajob_api/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-16 09:57:42.000000 vdk-control-service-api-1.0.6/test/
--rw-r--r--   0 root         (0) root         (0)     6192 2021-12-16 09:57:34.000000 vdk-control-service-api-1.0.6/test/test_data_job.py
--rw-r--r--   0 root         (0) root         (0)     4141 2021-12-16 09:57:34.000000 vdk-control-service-api-1.0.6/test/test_data_job_api_info.py
--rw-r--r--   0 root         (0) root         (0)     4823 2021-12-16 09:57:34.000000 vdk-control-service-api-1.0.6/test/test_data_job_config.py
--rw-r--r--   0 root         (0) root         (0)     4396 2021-12-16 09:57:34.000000 vdk-control-service-api-1.0.6/test/test_data_job_contacts.py
--rw-r--r--   0 root         (0) root         (0)     4852 2021-12-16 09:57:34.000000 vdk-control-service-api-1.0.6/test/test_data_job_deployment.py
--rw-r--r--   0 root         (0) root         (0)     5258 2021-12-16 09:57:34.000000 vdk-control-service-api-1.0.6/test/test_data_job_deployment_status.py
--rw-r--r--   0 root         (0) root         (0)     5600 2021-12-16 09:57:34.000000 vdk-control-service-api-1.0.6/test/test_data_job_execution.py
--rw-r--r--   0 root         (0) root         (0)     4165 2021-12-16 09:57:34.000000 vdk-control-service-api-1.0.6/test/test_data_job_execution_logs.py
--rw-r--r--   0 root         (0) root         (0)     4260 2021-12-16 09:57:34.000000 vdk-control-service-api-1.0.6/test/test_data_job_execution_request.py
--rw-r--r--   0 root         (0) root         (0)     4037 2021-12-16 09:57:34.000000 vdk-control-service-api-1.0.6/test/test_data_job_mode.py
--rw-r--r--   0 root         (0) root         (0)     4786 2021-12-16 09:57:34.000000 vdk-control-service-api-1.0.6/test/test_data_job_page.py
--rw-r--r--   0 root         (0) root         (0)     5054 2021-12-16 09:57:34.000000 vdk-control-service-api-1.0.6/test/test_data_job_query_response.py
--rw-r--r--   0 root         (0) root         (0)     5407 2021-12-16 09:57:34.000000 vdk-control-service-api-1.0.6/test/test_data_job_query_response_with_error.py
--rw-r--r--   0 root         (0) root         (0)     4236 2021-12-16 09:57:34.000000 vdk-control-service-api-1.0.6/test/test_data_job_resources.py
--rw-r--r--   0 root         (0) root         (0)     4126 2021-12-16 09:57:34.000000 vdk-control-service-api-1.0.6/test/test_data_job_schedule.py
--rw-r--r--   0 root         (0) root         (0)     4528 2021-12-16 09:57:34.000000 vdk-control-service-api-1.0.6/test/test_data_job_summary.py
--rw-r--r--   0 root         (0) root         (0)     4139 2021-12-16 09:57:34.000000 vdk-control-service-api-1.0.6/test/test_data_job_version.py
--rw-r--r--   0 root         (0) root         (0)     4757 2021-12-16 09:57:37.000000 vdk-control-service-api-1.0.6/test/test_data_jobs_api.py
--rw-r--r--   0 root         (0) root         (0)     4704 2021-12-16 09:57:37.000000 vdk-control-service-api-1.0.6/test/test_data_jobs_deployment_api.py
--rw-r--r--   0 root         (0) root         (0)     4900 2021-12-16 09:57:37.000000 vdk-control-service-api-1.0.6/test/test_data_jobs_execution_api.py
--rw-r--r--   0 root         (0) root         (0)     3826 2021-12-16 09:57:37.000000 vdk-control-service-api-1.0.6/test/test_data_jobs_properties_api.py
--rw-r--r--   0 root         (0) root         (0)     3602 2021-12-16 09:57:37.000000 vdk-control-service-api-1.0.6/test/test_data_jobs_service_api.py
--rw-r--r--   0 root         (0) root         (0)     3972 2021-12-16 09:57:37.000000 vdk-control-service-api-1.0.6/test/test_data_jobs_sources_api.py
--rw-r--r--   0 root         (0) root         (0)     4138 2021-12-16 09:57:34.000000 vdk-control-service-api-1.0.6/test/test_error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-16 09:57:42.000000 vdk-control-service-api-1.0.6/vdk_control_service_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3313 2021-12-16 09:57:42.000000 vdk-control-service-api-1.0.6/vdk_control_service_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2433 2021-12-16 09:57:42.000000 vdk-control-service-api-1.0.6/vdk_control_service_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-12-16 09:57:42.000000 vdk-control-service-api-1.0.6/vdk_control_service_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2021-12-16 09:57:42.000000 vdk-control-service-api-1.0.6/vdk_control_service_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2021-12-16 09:57:42.000000 vdk-control-service-api-1.0.6/vdk_control_service_api.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    12054 2021-12-16 09:57:40.000000 vdk-control-service-api-1.0.6/README.md
--rw-r--r--   0 root         (0) root         (0)       69 2021-12-16 09:57:42.000000 vdk-control-service-api-1.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     6700 2021-12-16 09:57:40.000000 vdk-control-service-api-1.0.6/setup.py
--rw-r--r--   0 root         (0) root         (0)     3313 2021-12-16 09:57:42.000000 vdk-control-service-api-1.0.6/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.323403 vdk-control-service-api-1.0.7/
+-rw-r--r--   0 root         (0) root         (0)     3190 2023-04-24 11:09:21.323403 vdk-control-service-api-1.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    20126 2023-04-24 11:09:20.000000 vdk-control-service-api-1.0.7/README.md
+-rw-r--r--   0 root         (0) root         (0)       69 2023-04-24 11:09:21.323403 vdk-control-service-api-1.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     6635 2023-04-24 11:09:20.000000 vdk-control-service-api-1.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.299403 vdk-control-service-api-1.0.7/taurus_datajob_api/
+-rw-r--r--   0 root         (0) root         (0)     3386 2023-04-24 11:09:20.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    61119 2023-04-24 11:09:20.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.299403 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/
+-rw-r--r--   0 root         (0) root         (0)      214 2023-04-24 11:09:20.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5328 2023-04-24 11:09:17.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/path_to_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.303403 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/paths/
+-rw-r--r--   0 root         (0) root         (0)      245 2023-04-24 11:09:17.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/paths/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      149 2023-04-24 11:09:16.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_info.py
+-rw-r--r--   0 root         (0) root         (0)      252 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs.py
+-rw-r--r--   0 root         (0) root         (0)      392 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name.py
+-rw-r--r--   0 root         (0) root         (0)      312 2023-04-24 11:09:14.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name_deployments.py
+-rw-r--r--   0 root         (0) root         (0)      499 2023-04-24 11:09:14.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id.py
+-rw-r--r--   0 root         (0) root         (0)      384 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions.py
+-rw-r--r--   0 root         (0) root         (0)      381 2023-04-24 11:09:16.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties.py
+-rw-r--r--   0 root         (0) root         (0)      186 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name_executions.py
+-rw-r--r--   0 root         (0) root         (0)      352 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name_executions_execution_id.py
+-rw-r--r--   0 root         (0) root         (0)      219 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name_executions_execution_id_logs.py
+-rw-r--r--   0 root         (0) root         (0)      178 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name_keytab.py
+-rw-r--r--   0 root         (0) root         (0)      426 2023-04-24 11:09:17.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name_sources.py
+-rw-r--r--   0 root         (0) root         (0)      190 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name_team_new_team.py
+-rw-r--r--   0 root         (0) root         (0)     1365 2023-04-24 11:09:17.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/tag_to_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.303403 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/tags/
+-rw-r--r--   0 root         (0) root         (0)      555 2023-04-24 11:09:17.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/tags/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3852 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/tags/data_jobs_api.py
+-rw-r--r--   0 root         (0) root         (0)     3737 2023-04-24 11:09:14.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/tags/data_jobs_deployment_api.py
+-rw-r--r--   0 root         (0) root         (0)     3999 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/tags/data_jobs_execution_api.py
+-rw-r--r--   0 root         (0) root         (0)     3368 2023-04-24 11:09:16.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/tags/data_jobs_properties_api.py
+-rw-r--r--   0 root         (0) root         (0)     3111 2023-04-24 11:09:16.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/tags/data_jobs_service_api.py
+-rw-r--r--   0 root         (0) root         (0)     3418 2023-04-24 11:09:17.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/tags/data_jobs_sources_api.py
+-rw-r--r--   0 root         (0) root         (0)    18077 2023-04-24 11:09:20.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     7117 2023-04-24 11:09:20.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.307403 vdk-control-service-api-1.0.7/taurus_datajob_api/model/
+-rw-r--r--   0 root         (0) root         (0)      352 2023-04-24 11:09:20.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6765 2023-04-24 11:09:05.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job.py
+-rw-r--r--   0 root         (0) root         (0)     6849 2023-04-24 11:09:05.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_api_info.py
+-rw-r--r--   0 root         (0) root         (0)     8809 2023-04-24 11:09:06.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_config.py
+-rw-r--r--   0 root         (0) root         (0)    11079 2023-04-24 11:09:07.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_contacts.py
+-rw-r--r--   0 root         (0) root         (0)    10382 2023-04-24 11:09:07.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_deployment.py
+-rw-r--r--   0 root         (0) root         (0)     3211 2023-04-24 11:09:07.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_deployment_id.py
+-rw-r--r--   0 root         (0) root         (0)    11264 2023-04-24 11:09:07.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_deployment_status.py
+-rw-r--r--   0 root         (0) root         (0)    12532 2023-04-24 11:09:08.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_execution.py
+-rw-r--r--   0 root         (0) root         (0)     5033 2023-04-24 11:09:08.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_execution_logs.py
+-rw-r--r--   0 root         (0) root         (0)     7013 2023-04-24 11:09:08.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_execution_request.py
+-rw-r--r--   0 root         (0) root         (0)     4081 2023-04-24 11:09:08.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_mode.py
+-rw-r--r--   0 root         (0) root         (0)     7116 2023-04-24 11:09:08.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_page.py
+-rw-r--r--   0 root         (0) root         (0)     4219 2023-04-24 11:09:08.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_properties.py
+-rw-r--r--   0 root         (0) root         (0)     6516 2023-04-24 11:09:08.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_query_response.py
+-rw-r--r--   0 root         (0) root         (0)     6534 2023-04-24 11:09:08.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_query_response_with_error.py
+-rw-r--r--   0 root         (0) root         (0)     6974 2023-04-24 11:09:09.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_resources.py
+-rw-r--r--   0 root         (0) root         (0)     5138 2023-04-24 11:09:09.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     6731 2023-04-24 11:09:09.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_summary.py
+-rw-r--r--   0 root         (0) root         (0)     5158 2023-04-24 11:09:09.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_version.py
+-rw-r--r--   0 root         (0) root         (0)     5936 2023-04-24 11:09:09.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/model/error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.307403 vdk-control-service-api-1.0.7/taurus_datajob_api/models/
+-rw-r--r--   0 root         (0) root         (0)     1856 2023-04-24 11:09:20.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.307403 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/
+-rw-r--r--   0 root         (0) root         (0)     1937 2023-04-24 11:09:17.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.307403 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_info/
+-rw-r--r--   0 root         (0) root         (0)      359 2023-04-24 11:09:16.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_info/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9663 2023-04-24 11:09:16.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_info/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.307403 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs/
+-rw-r--r--   0 root         (0) root         (0)      359 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13125 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs/get.py
+-rw-r--r--   0 root         (0) root         (0)    16868 2023-04-24 11:09:10.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.307403 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name/
+-rw-r--r--   0 root         (0) root         (0)      377 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10312 2023-04-24 11:09:11.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name/delete.py
+-rw-r--r--   0 root         (0) root         (0)    10613 2023-04-24 11:09:11.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name/get.py
+-rw-r--r--   0 root         (0) root         (0)    15339 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.307403 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments/
+-rw-r--r--   0 root         (0) root         (0)      401 2023-04-24 11:09:14.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13798 2023-04-24 11:09:13.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments/get.py
+-rw-r--r--   0 root         (0) root         (0)    17659 2023-04-24 11:09:13.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.307403 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/
+-rw-r--r--   0 root         (0) root         (0)      429 2023-04-24 11:09:14.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10729 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    10952 2023-04-24 11:09:13.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    15525 2023-04-24 11:09:13.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/patch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.311403 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions/
+-rw-r--r--   0 root         (0) root         (0)      451 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14554 2023-04-24 11:09:14.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions/get.py
+-rw-r--r--   0 root         (0) root         (0)    16006 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.311403 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties/
+-rw-r--r--   0 root         (0) root         (0)      451 2023-04-24 11:09:16.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10452 2023-04-24 11:09:16.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties/get.py
+-rw-r--r--   0 root         (0) root         (0)    13298 2023-04-24 11:09:16.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.311403 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions/
+-rw-r--r--   0 root         (0) root         (0)      399 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14185 2023-04-24 11:09:14.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.311403 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions_execution_id/
+-rw-r--r--   0 root         (0) root         (0)      425 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions_execution_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10765 2023-04-24 11:09:14.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions_execution_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11021 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions_execution_id/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.311403 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions_execution_id_logs/
+-rw-r--r--   0 root         (0) root         (0)      435 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions_execution_id_logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13907 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions_execution_id_logs/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.311403 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_keytab/
+-rw-r--r--   0 root         (0) root         (0)      391 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_keytab/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11209 2023-04-24 11:09:11.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_keytab/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.311403 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_sources/
+-rw-r--r--   0 root         (0) root         (0)      393 2023-04-24 11:09:17.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_sources/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12453 2023-04-24 11:09:17.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_sources/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11239 2023-04-24 11:09:16.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_sources/get.py
+-rw-r--r--   0 root         (0) root         (0)    17624 2023-04-24 11:09:17.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_sources/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.311403 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_team_new_team/
+-rw-r--r--   0 root         (0) root         (0)      405 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_team_new_team/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11166 2023-04-24 11:09:11.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_team_new_team/put.py
+-rw-r--r--   0 root         (0) root         (0)    13149 2023-04-24 11:09:20.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/rest.py
+-rw-r--r--   0 root         (0) root         (0)   100261 2023-04-24 11:09:20.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.295403 vdk-control-service-api-1.0.7/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.315403 vdk-control-service-api-1.0.7/test/test_models/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 11:09:20.000000 vdk-control-service-api-1.0.7/test/test_models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3149 2023-04-24 11:09:05.000000 vdk-control-service-api-1.0.7/test/test_models/test_data_job.py
+-rw-r--r--   0 root         (0) root         (0)     3179 2023-04-24 11:09:06.000000 vdk-control-service-api-1.0.7/test/test_models/test_data_job_api_info.py
+-rw-r--r--   0 root         (0) root         (0)     3174 2023-04-24 11:09:06.000000 vdk-control-service-api-1.0.7/test/test_models/test_data_job_config.py
+-rw-r--r--   0 root         (0) root         (0)     3182 2023-04-24 11:09:07.000000 vdk-control-service-api-1.0.7/test/test_models/test_data_job_contacts.py
+-rw-r--r--   0 root         (0) root         (0)     3190 2023-04-24 11:09:07.000000 vdk-control-service-api-1.0.7/test/test_models/test_data_job_deployment.py
+-rw-r--r--   0 root         (0) root         (0)     3199 2023-04-24 11:09:07.000000 vdk-control-service-api-1.0.7/test/test_models/test_data_job_deployment_id.py
+-rw-r--r--   0 root         (0) root         (0)     3215 2023-04-24 11:09:07.000000 vdk-control-service-api-1.0.7/test/test_models/test_data_job_deployment_status.py
+-rw-r--r--   0 root         (0) root         (0)     3186 2023-04-24 11:09:08.000000 vdk-control-service-api-1.0.7/test/test_models/test_data_job_execution.py
+-rw-r--r--   0 root         (0) root         (0)     3203 2023-04-24 11:09:08.000000 vdk-control-service-api-1.0.7/test/test_models/test_data_job_execution_logs.py
+-rw-r--r--   0 root         (0) root         (0)     3215 2023-04-24 11:09:08.000000 vdk-control-service-api-1.0.7/test/test_models/test_data_job_execution_request.py
+-rw-r--r--   0 root         (0) root         (0)     3166 2023-04-24 11:09:08.000000 vdk-control-service-api-1.0.7/test/test_models/test_data_job_mode.py
+-rw-r--r--   0 root         (0) root         (0)     3166 2023-04-24 11:09:08.000000 vdk-control-service-api-1.0.7/test/test_models/test_data_job_page.py
+-rw-r--r--   0 root         (0) root         (0)     3190 2023-04-24 11:09:08.000000 vdk-control-service-api-1.0.7/test/test_models/test_data_job_properties.py
+-rw-r--r--   0 root         (0) root         (0)     3203 2023-04-24 11:09:08.000000 vdk-control-service-api-1.0.7/test/test_models/test_data_job_query_response.py
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-04-24 11:09:09.000000 vdk-control-service-api-1.0.7/test/test_models/test_data_job_query_response_with_error.py
+-rw-r--r--   0 root         (0) root         (0)     3186 2023-04-24 11:09:09.000000 vdk-control-service-api-1.0.7/test/test_models/test_data_job_resources.py
+-rw-r--r--   0 root         (0) root         (0)     3182 2023-04-24 11:09:09.000000 vdk-control-service-api-1.0.7/test/test_models/test_data_job_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     3178 2023-04-24 11:09:09.000000 vdk-control-service-api-1.0.7/test/test_models/test_data_job_summary.py
+-rw-r--r--   0 root         (0) root         (0)     3178 2023-04-24 11:09:09.000000 vdk-control-service-api-1.0.7/test/test_models/test_data_job_version.py
+-rw-r--r--   0 root         (0) root         (0)     3140 2023-04-24 11:09:09.000000 vdk-control-service-api-1.0.7/test/test_models/test_error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.315403 vdk-control-service-api-1.0.7/test/test_paths/
+-rw-r--r--   0 root         (0) root         (0)     1995 2023-04-24 11:09:17.000000 vdk-control-service-api-1.0.7/test/test_paths/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.315403 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_info/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 11:09:16.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_info/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      928 2023-04-24 11:09:16.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_info/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.315403 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      891 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      918 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.319403 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      938 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      974 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      932 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.319403 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 11:09:14.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-04-24 11:09:14.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      997 2023-04-24 11:09:14.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.319403 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 11:09:14.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1082 2023-04-24 11:09:14.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      990 2023-04-24 11:09:14.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)     1334 2023-04-24 11:09:14.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/test_patch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.319403 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1036 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions/test_get.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.319403 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 11:09:16.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1009 2023-04-24 11:09:16.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties/test_get.py
+-rw-r--r--   0 root         (0) root         (0)     1035 2023-04-24 11:09:16.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.319403 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1037 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.319403 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions_execution_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions_execution_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions_execution_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      996 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions_execution_id/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.319403 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions_execution_id_logs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions_execution_id_logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1180 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions_execution_id_logs/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.319403 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_keytab/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_keytab/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      932 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_keytab/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.319403 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_sources/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 11:09:17.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_sources/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      957 2023-04-24 11:09:17.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_sources/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      954 2023-04-24 11:09:17.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_sources/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      948 2023-04-24 11:09:17.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_sources/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.323403 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_team_new_team/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_team_new_team/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      979 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_team_new_team/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.323403 vdk-control-service-api-1.0.7/vdk_control_service_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3190 2023-04-24 11:09:21.000000 vdk-control-service-api-1.0.7/vdk_control_service_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10920 2023-04-24 11:09:21.000000 vdk-control-service-api-1.0.7/vdk_control_service_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 11:09:21.000000 vdk-control-service-api-1.0.7/vdk_control_service_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      118 2023-04-24 11:09:21.000000 vdk-control-service-api-1.0.7/vdk_control_service_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-04-24 11:09:21.000000 vdk-control-service-api-1.0.7/vdk_control_service_api.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `vdk-control-service-api-1.0.6/taurus_datajob_api/models/__init__.py` & `vdk-control-service-api-1.0.7/taurus_datajob_api/apis/tags/data_jobs_execution_api.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 # coding: utf-8
 
-# flake8: noqa
 """
     Versatile Data Kit Control Service API
 
-    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction  The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br  The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time).                      The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning.                            Implementation of the API is not considered stable nor well tested.                            Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade.                          The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.   # noqa: E501
+    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
-# import models into model package
-from taurus_datajob_api.models.data_job import DataJob
-from taurus_datajob_api.models.data_job_api_info import DataJobApiInfo
-from taurus_datajob_api.models.data_job_config import DataJobConfig
-from taurus_datajob_api.models.data_job_contacts import DataJobContacts
-from taurus_datajob_api.models.data_job_deployment import DataJobDeployment
-from taurus_datajob_api.models.data_job_deployment_status import DataJobDeploymentStatus
-from taurus_datajob_api.models.data_job_execution import DataJobExecution
-from taurus_datajob_api.models.data_job_execution_logs import DataJobExecutionLogs
-from taurus_datajob_api.models.data_job_execution_request import DataJobExecutionRequest
-from taurus_datajob_api.models.data_job_mode import DataJobMode
-from taurus_datajob_api.models.data_job_page import DataJobPage
-from taurus_datajob_api.models.data_job_query_response import DataJobQueryResponse
-from taurus_datajob_api.models.data_job_query_response_with_error import DataJobQueryResponseWithError
-from taurus_datajob_api.models.data_job_resources import DataJobResources
-from taurus_datajob_api.models.data_job_schedule import DataJobSchedule
-from taurus_datajob_api.models.data_job_summary import DataJobSummary
-from taurus_datajob_api.models.data_job_version import DataJobVersion
-from taurus_datajob_api.models.error import Error
+from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions.get import DataJobDeploymentExecutionList
+from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs_job_name_executions_execution_id.delete import DataJobExecutionCancel
+from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs_job_name_executions.get import DataJobExecutionList
+from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs_job_name_executions_execution_id.get import DataJobExecutionRead
+from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions.post import DataJobExecutionStart
+from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs_job_name_executions_execution_id_logs.get import DataJobLogsDownload
+
+
+class DataJobsExecutionApi(
+    DataJobDeploymentExecutionList,
+    DataJobExecutionCancel,
+    DataJobExecutionList,
+    DataJobExecutionRead,
+    DataJobExecutionStart,
+    DataJobLogsDownload,
+):
+    """NOTE: This class is auto generated by OpenAPI Generator
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+    """
+    pass
```

### Comparing `vdk-control-service-api-1.0.6/taurus_datajob_api/models/data_job_execution_request.py` & `vdk-control-service-api-1.0.7/taurus_datajob_api/exceptions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,150 +1,147 @@
 # coding: utf-8
 
 """
     Versatile Data Kit Control Service API
 
-    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction  The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br  The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time).                      The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning.                            Implementation of the API is not considered stable nor well tested.                            Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade.                          The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.   # noqa: E501
+    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
+import dataclasses
+import typing
 
+from urllib3._collections import HTTPHeaderDict
 
-import pprint
-import re  # noqa: F401
 
-import six
+class OpenApiException(Exception):
+    """The base exception class for all OpenAPIExceptions"""
 
-from taurus_datajob_api.configuration import Configuration
 
-
-class DataJobExecutionRequest(object):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-    """
-
-    """
-    Attributes:
-      openapi_types (dict): The key is attribute name
-                            and the value is attribute type.
-      attribute_map (dict): The key is attribute name
-                            and the value is json key in definition.
-    """
-    openapi_types = {
-        'started_by': 'str',
-        'args': 'dict(str, object)'
-    }
-
-    attribute_map = {
-        'started_by': 'started_by',
-        'args': 'args'
-    }
-
-    def __init__(self, started_by=None, args=None, local_vars_configuration=None):  # noqa: E501
-        """DataJobExecutionRequest - a model defined in OpenAPI"""  # noqa: E501
-        if local_vars_configuration is None:
-            local_vars_configuration = Configuration()
-        self.local_vars_configuration = local_vars_configuration
-
-        self._started_by = None
-        self._args = None
-        self.discriminator = None
-
-        if started_by is not None:
-            self.started_by = started_by
-        if args is not None:
-            self.args = args
-
-    @property
-    def started_by(self):
-        """Gets the started_by of this DataJobExecutionRequest.  # noqa: E501
-
-        User or service that started the execution (e.g manual/auserov@example.mail.com or scheduled/runtime)  # noqa: E501
-
-        :return: The started_by of this DataJobExecutionRequest.  # noqa: E501
-        :rtype: str
+class ApiTypeError(OpenApiException, TypeError):
+    def __init__(self, msg, path_to_item=None, valid_classes=None,
+                 key_type=None):
+        """ Raises an exception for TypeErrors
+
+        Args:
+            msg (str): the exception message
+
+        Keyword Args:
+            path_to_item (list): a list of keys an indices to get to the
+                                 current_item
+                                 None if unset
+            valid_classes (tuple): the primitive classes that current item
+                                   should be an instance of
+                                   None if unset
+            key_type (bool): False if our value is a value in a dict
+                             True if it is a key in a dict
+                             False if our item is an item in a list
+                             None if unset
         """
-        return self._started_by
-
-    @started_by.setter
-    def started_by(self, started_by):
-        """Sets the started_by of this DataJobExecutionRequest.
+        self.path_to_item = path_to_item
+        self.valid_classes = valid_classes
+        self.key_type = key_type
+        full_msg = msg
+        if path_to_item:
+            full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
+        super(ApiTypeError, self).__init__(full_msg)
 
-        User or service that started the execution (e.g manual/auserov@example.mail.com or scheduled/runtime)  # noqa: E501
 
-        :param started_by: The started_by of this DataJobExecutionRequest.  # noqa: E501
-        :type: str
+class ApiValueError(OpenApiException, ValueError):
+    def __init__(self, msg, path_to_item=None):
         """
+        Args:
+            msg (str): the exception message
 
-        self._started_by = started_by
+        Keyword Args:
+            path_to_item (list) the path to the exception in the
+                received_data dict. None if unset
+        """
 
-    @property
-    def args(self):
-        """Gets the args of this DataJobExecutionRequest.  # noqa: E501
+        self.path_to_item = path_to_item
+        full_msg = msg
+        if path_to_item:
+            full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
+        super(ApiValueError, self).__init__(full_msg)
 
-        Data Job arguments  # noqa: E501
 
-        :return: The args of this DataJobExecutionRequest.  # noqa: E501
-        :rtype: dict(str, object)
+class ApiAttributeError(OpenApiException, AttributeError):
+    def __init__(self, msg, path_to_item=None):
         """
-        return self._args
-
-    @args.setter
-    def args(self, args):
-        """Sets the args of this DataJobExecutionRequest.
+        Raised when an attribute reference or assignment fails.
 
-        Data Job arguments  # noqa: E501
+        Args:
+            msg (str): the exception message
 
-        :param args: The args of this DataJobExecutionRequest.  # noqa: E501
-        :type: dict(str, object)
+        Keyword Args:
+            path_to_item (None/list) the path to the exception in the
+                received_data dict
         """
+        self.path_to_item = path_to_item
+        full_msg = msg
+        if path_to_item:
+            full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
+        super(ApiAttributeError, self).__init__(full_msg)
 
-        self._args = args
 
-    def to_dict(self):
-        """Returns the model properties as a dict"""
-        result = {}
-
-        for attr, _ in six.iteritems(self.openapi_types):
-            value = getattr(self, attr)
-            if isinstance(value, list):
-                result[attr] = list(map(
-                    lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
-                    value
-                ))
-            elif hasattr(value, "to_dict"):
-                result[attr] = value.to_dict()
-            elif isinstance(value, dict):
-                result[attr] = dict(map(
-                    lambda item: (item[0], item[1].to_dict())
-                    if hasattr(item[1], "to_dict") else item,
-                    value.items()
-                ))
-            else:
-                result[attr] = value
+class ApiKeyError(OpenApiException, KeyError):
+    def __init__(self, msg, path_to_item=None):
+        """
+        Args:
+            msg (str): the exception message
 
-        return result
+        Keyword Args:
+            path_to_item (None/list) the path to the exception in the
+                received_data dict
+        """
+        self.path_to_item = path_to_item
+        full_msg = msg
+        if path_to_item:
+            full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
+        super(ApiKeyError, self).__init__(full_msg)
 
-    def to_str(self):
-        """Returns the string representation of the model"""
-        return pprint.pformat(self.to_dict())
 
-    def __repr__(self):
-        """For `print` and `pprint`"""
-        return self.to_str()
+T = typing.TypeVar("T")
 
-    def __eq__(self, other):
-        """Returns true if both objects are equal"""
-        if not isinstance(other, DataJobExecutionRequest):
-            return False
 
-        return self.to_dict() == other.to_dict()
+@dataclasses.dataclass
+class ApiException(OpenApiException, typing.Generic[T]):
+    status: int
+    reason: str
+    api_response: typing.Optional[T] = None
 
-    def __ne__(self, other):
-        """Returns true if both objects are not equal"""
-        if not isinstance(other, DataJobExecutionRequest):
-            return True
+    @property
+    def body(self) -> typing.Union[str, bytes, None]:
+        if not self.api_response:
+            return None
+        return self.api_response.response.data
 
-        return self.to_dict() != other.to_dict()
+    @property
+    def headers(self) -> typing.Optional[HTTPHeaderDict]:
+        if not self.api_response:
+            return None
+        return self.api_response.response.getheaders()
+
+    def __str__(self):
+        """Custom error messages for exception"""
+        error_message = "({0})\n"\
+                        "Reason: {1}\n".format(self.status, self.reason)
+        if self.headers:
+            error_message += "HTTP response headers: {0}\n".format(
+                self.headers)
+
+        if self.body:
+            error_message += "HTTP response body: {0}\n".format(self.body)
+
+        return error_message
+
+
+def render_path(path_to_item):
+    """Returns a string representation of a path"""
+    result = ""
+    for pth in path_to_item:
+        if isinstance(pth, int):
+            result += "[{0}]".format(pth)
+        else:
+            result += "['{0}']".format(pth)
+    return result
```

### Comparing `vdk-control-service-api-1.0.6/taurus_datajob_api/models/data_job_mode.py` & `vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_execution_logs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,100 +1,80 @@
 # coding: utf-8
 
 """
     Versatile Data Kit Control Service API
 
-    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction  The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br  The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time).                      The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning.                            Implementation of the API is not considered stable nor well tested.                            Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade.                          The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.   # noqa: E501
+    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import pprint
+from datetime import date, datetime  # noqa: F401
+import decimal  # noqa: F401
+import functools  # noqa: F401
+import io  # noqa: F401
 import re  # noqa: F401
+import typing  # noqa: F401
+import typing_extensions  # noqa: F401
+import uuid  # noqa: F401
 
-import six
+import frozendict  # noqa: F401
 
-from taurus_datajob_api.configuration import Configuration
+from taurus_datajob_api import schemas  # noqa: F401
 
 
-class DataJobMode(object):
+class DataJobExecutionLogs(
+    schemas.DictSchema
+):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
-    """
-
-    """
-    allowed enum values
-    """
-    TESTING = "testing"
-    RELEASE = "release"
-
-    allowable_values = [TESTING, RELEASE]  # noqa: E501
 
+    Executions of a Data Job
     """
-    Attributes:
-      openapi_types (dict): The key is attribute name
-                            and the value is attribute type.
-      attribute_map (dict): The key is attribute name
-                            and the value is json key in definition.
-    """
-    openapi_types = {
-    }
-
-    attribute_map = {
-    }
 
-    def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """DataJobMode - a model defined in OpenAPI"""  # noqa: E501
-        if local_vars_configuration is None:
-            local_vars_configuration = Configuration()
-        self.local_vars_configuration = local_vars_configuration
-        self.discriminator = None
-
-    def to_dict(self):
-        """Returns the model properties as a dict"""
-        result = {}
-
-        for attr, _ in six.iteritems(self.openapi_types):
-            value = getattr(self, attr)
-            if isinstance(value, list):
-                result[attr] = list(map(
-                    lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
-                    value
-                ))
-            elif hasattr(value, "to_dict"):
-                result[attr] = value.to_dict()
-            elif isinstance(value, dict):
-                result[attr] = dict(map(
-                    lambda item: (item[0], item[1].to_dict())
-                    if hasattr(item[1], "to_dict") else item,
-                    value.items()
-                ))
-            else:
-                result[attr] = value
-
-        return result
-
-    def to_str(self):
-        """Returns the string representation of the model"""
-        return pprint.pformat(self.to_dict())
-
-    def __repr__(self):
-        """For `print` and `pprint`"""
-        return self.to_str()
-
-    def __eq__(self, other):
-        """Returns true if both objects are equal"""
-        if not isinstance(other, DataJobMode):
-            return False
-
-        return self.to_dict() == other.to_dict()
-
-    def __ne__(self, other):
-        """Returns true if both objects are not equal"""
-        if not isinstance(other, DataJobMode):
-            return True
 
-        return self.to_dict() != other.to_dict()
+    class MetaOapg:
+        
+        class properties:
+            logs = schemas.StrSchema
+            __annotations__ = {
+                "logs": logs,
+            }
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["logs"]) -> MetaOapg.properties.logs: ...
+    
+    @typing.overload
+    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
+    
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["logs", ], str]):
+        # dict_instance[name] accessor
+        return super().__getitem__(name)
+    
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["logs"]) -> typing.Union[MetaOapg.properties.logs, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
+    
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["logs", ], str]):
+        return super().get_item_oapg(name)
+    
+
+    def __new__(
+        cls,
+        *_args: typing.Union[dict, frozendict.frozendict, ],
+        logs: typing.Union[MetaOapg.properties.logs, str, schemas.Unset] = schemas.unset,
+        _configuration: typing.Optional[schemas.Configuration] = None,
+        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+    ) -> 'DataJobExecutionLogs':
+        return super().__new__(
+            cls,
+            *_args,
+            logs=logs,
+            _configuration=_configuration,
+            **kwargs,
+        )
```

### Comparing `vdk-control-service-api-1.0.6/taurus_datajob_api/models/data_job_query_response.py` & `vdk-control-service-api-1.0.7/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,148 +1,48 @@
 # coding: utf-8
 
 """
     Versatile Data Kit Control Service API
 
-    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction  The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br  The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time).                      The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning.                            Implementation of the API is not considered stable nor well tested.                            Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade.                          The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.   # noqa: E501
+    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
+from setuptools import setup, find_packages  # noqa: H301
 
-import pprint
-import re  # noqa: F401
-
-import six
-
-from taurus_datajob_api.configuration import Configuration
-
-
-class DataJobQueryResponse(object):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
+NAME = "vdk-control-service-api"
+VERSION = "1.0.7"
+# To install the library, run the following
+#
+# python setup.py install
+#
+# prerequisite: setuptools
+# http://pypi.python.org/pypi/setuptools
+
+REQUIRES = [
+    "certifi >= 14.5.14",
+    "frozendict ~= 2.3.4",
+    "python-dateutil ~= 2.7.0",
+    "setuptools >= 21.0.0",
+    "typing_extensions ~= 4.3.0",
+    "urllib3 ~= 1.26.7",
+]
+
+setup(
+    name=NAME,
+    version=VERSION,
+    description="Versatile Data Kit Control Service API",
+    author="OpenAPI Generator community",
+    author_email="team@openapitools.org",
+    url="",
+    keywords=["OpenAPI", "OpenAPI-Generator", "Versatile Data Kit Control Service API"],
+    python_requires=">=3.7",
+    install_requires=REQUIRES,
+    packages=find_packages(exclude=["test", "tests"]),
+    include_package_data=True,
+    license="Apache 2.0",
+    long_description="""\
+    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.&lt;br&gt; &lt;br&gt; ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) &lt;br&gt; The API reflects the usual Data Job Development lifecycle:&lt;br&gt; &lt;li&gt; Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). &lt;li&gt; Download keytab. Develop and run the data job locally. &lt;li&gt; Deploy the data job in cloud runtime environment to run on a scheduled basis. &lt;br&gt;&lt;br&gt; If Authentication is enabled, pass OAuth2 access token in HTTP header &#x27;Authorization: Bearer [access-token-here]&#x27; (https://datatracker.ietf.org/doc/html/rfc6750). &lt;br The API promotes some best practices (inspired by https://12factor.net): &lt;li&gt; Explicitly declare and isolate dependencies. &lt;li&gt; Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. &lt;li&gt; Separation between the build, release/deploy, and run stages. &lt;li&gt; Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). &lt;li&gt; Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. &lt;li&gt; Keep development, staging, and production as similar as possible. &lt;br&gt;&lt;br&gt; &lt;b&gt;API Evolution&lt;/b&gt;&lt;br&gt; In the following sections, there are some terms that have a special meaning in the context of the APIs. &lt;br&gt;&lt;br&gt; &lt;li&gt; &lt;i&gt;Stable&lt;/i&gt; - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. &lt;li&gt; &lt;i&gt;Experimental&lt;/i&gt; - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. &lt;li&gt; &lt;i&gt;Deprecated&lt;/i&gt; - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
     """
-
-    """
-    Attributes:
-      openapi_types (dict): The key is attribute name
-                            and the value is attribute type.
-      attribute_map (dict): The key is attribute name
-                            and the value is json key in definition.
-    """
-    openapi_types = {
-        'errors': 'list[object]',
-        'data': 'DataJobPage'
-    }
-
-    attribute_map = {
-        'errors': 'errors',
-        'data': 'data'
-    }
-
-    def __init__(self, errors=None, data=None, local_vars_configuration=None):  # noqa: E501
-        """DataJobQueryResponse - a model defined in OpenAPI"""  # noqa: E501
-        if local_vars_configuration is None:
-            local_vars_configuration = Configuration()
-        self.local_vars_configuration = local_vars_configuration
-
-        self._errors = None
-        self._data = None
-        self.discriminator = None
-
-        if errors is not None:
-            self.errors = errors
-        if data is not None:
-            self.data = data
-
-    @property
-    def errors(self):
-        """Gets the errors of this DataJobQueryResponse.  # noqa: E501
-
-        Errors while making query (validation errors, exceptions, etc)  # noqa: E501
-
-        :return: The errors of this DataJobQueryResponse.  # noqa: E501
-        :rtype: list[object]
-        """
-        return self._errors
-
-    @errors.setter
-    def errors(self, errors):
-        """Sets the errors of this DataJobQueryResponse.
-
-        Errors while making query (validation errors, exceptions, etc)  # noqa: E501
-
-        :param errors: The errors of this DataJobQueryResponse.  # noqa: E501
-        :type: list[object]
-        """
-
-        self._errors = errors
-
-    @property
-    def data(self):
-        """Gets the data of this DataJobQueryResponse.  # noqa: E501
-
-
-        :return: The data of this DataJobQueryResponse.  # noqa: E501
-        :rtype: DataJobPage
-        """
-        return self._data
-
-    @data.setter
-    def data(self, data):
-        """Sets the data of this DataJobQueryResponse.
-
-
-        :param data: The data of this DataJobQueryResponse.  # noqa: E501
-        :type: DataJobPage
-        """
-
-        self._data = data
-
-    def to_dict(self):
-        """Returns the model properties as a dict"""
-        result = {}
-
-        for attr, _ in six.iteritems(self.openapi_types):
-            value = getattr(self, attr)
-            if isinstance(value, list):
-                result[attr] = list(map(
-                    lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
-                    value
-                ))
-            elif hasattr(value, "to_dict"):
-                result[attr] = value.to_dict()
-            elif isinstance(value, dict):
-                result[attr] = dict(map(
-                    lambda item: (item[0], item[1].to_dict())
-                    if hasattr(item[1], "to_dict") else item,
-                    value.items()
-                ))
-            else:
-                result[attr] = value
-
-        return result
-
-    def to_str(self):
-        """Returns the string representation of the model"""
-        return pprint.pformat(self.to_dict())
-
-    def __repr__(self):
-        """For `print` and `pprint`"""
-        return self.to_str()
-
-    def __eq__(self, other):
-        """Returns true if both objects are equal"""
-        if not isinstance(other, DataJobQueryResponse):
-            return False
-
-        return self.to_dict() == other.to_dict()
-
-    def __ne__(self, other):
-        """Returns true if both objects are not equal"""
-        if not isinstance(other, DataJobQueryResponse):
-            return True
-
-        return self.to_dict() != other.to_dict()
+)
```

### Comparing `vdk-control-service-api-1.0.6/taurus_datajob_api/models/data_job_query_response_with_error.py` & `vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_query_response.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,148 +1,117 @@
 # coding: utf-8
 
 """
     Versatile Data Kit Control Service API
 
-    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction  The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br  The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time).                      The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning.                            Implementation of the API is not considered stable nor well tested.                            Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade.                          The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.   # noqa: E501
+    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import pprint
+from datetime import date, datetime  # noqa: F401
+import decimal  # noqa: F401
+import functools  # noqa: F401
+import io  # noqa: F401
 import re  # noqa: F401
+import typing  # noqa: F401
+import typing_extensions  # noqa: F401
+import uuid  # noqa: F401
 
-import six
+import frozendict  # noqa: F401
 
-from taurus_datajob_api.configuration import Configuration
+from taurus_datajob_api import schemas  # noqa: F401
 
 
-class DataJobQueryResponseWithError(object):
+class DataJobQueryResponse(
+    schemas.DictSchema
+):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
-    """
 
+    Query response containing Data Jobs
     """
-    Attributes:
-      openapi_types (dict): The key is attribute name
-                            and the value is attribute type.
-      attribute_map (dict): The key is attribute name
-                            and the value is json key in definition.
-    """
-    openapi_types = {
-        'errors': 'list[object]',
-        'data': 'DataJobPage'
-    }
-
-    attribute_map = {
-        'errors': 'errors',
-        'data': 'data'
-    }
-
-    def __init__(self, errors=None, data=None, local_vars_configuration=None):  # noqa: E501
-        """DataJobQueryResponseWithError - a model defined in OpenAPI"""  # noqa: E501
-        if local_vars_configuration is None:
-            local_vars_configuration = Configuration()
-        self.local_vars_configuration = local_vars_configuration
-
-        self._errors = None
-        self._data = None
-        self.discriminator = None
-
-        if errors is not None:
-            self.errors = errors
-        if data is not None:
-            self.data = data
-
-    @property
-    def errors(self):
-        """Gets the errors of this DataJobQueryResponseWithError.  # noqa: E501
-
-        Errors while making query (validation errors, exceptions, etc)  # noqa: E501
-
-        :return: The errors of this DataJobQueryResponseWithError.  # noqa: E501
-        :rtype: list[object]
-        """
-        return self._errors
-
-    @errors.setter
-    def errors(self, errors):
-        """Sets the errors of this DataJobQueryResponseWithError.
-
-        Errors while making query (validation errors, exceptions, etc)  # noqa: E501
-
-        :param errors: The errors of this DataJobQueryResponseWithError.  # noqa: E501
-        :type: list[object]
-        """
-
-        self._errors = errors
-
-    @property
-    def data(self):
-        """Gets the data of this DataJobQueryResponseWithError.  # noqa: E501
-
-
-        :return: The data of this DataJobQueryResponseWithError.  # noqa: E501
-        :rtype: DataJobPage
-        """
-        return self._data
-
-    @data.setter
-    def data(self, data):
-        """Sets the data of this DataJobQueryResponseWithError.
-
-
-        :param data: The data of this DataJobQueryResponseWithError.  # noqa: E501
-        :type: DataJobPage
-        """
-
-        self._data = data
-
-    def to_dict(self):
-        """Returns the model properties as a dict"""
-        result = {}
-
-        for attr, _ in six.iteritems(self.openapi_types):
-            value = getattr(self, attr)
-            if isinstance(value, list):
-                result[attr] = list(map(
-                    lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
-                    value
-                ))
-            elif hasattr(value, "to_dict"):
-                result[attr] = value.to_dict()
-            elif isinstance(value, dict):
-                result[attr] = dict(map(
-                    lambda item: (item[0], item[1].to_dict())
-                    if hasattr(item[1], "to_dict") else item,
-                    value.items()
-                ))
-            else:
-                result[attr] = value
-
-        return result
-
-    def to_str(self):
-        """Returns the string representation of the model"""
-        return pprint.pformat(self.to_dict())
-
-    def __repr__(self):
-        """For `print` and `pprint`"""
-        return self.to_str()
-
-    def __eq__(self, other):
-        """Returns true if both objects are equal"""
-        if not isinstance(other, DataJobQueryResponseWithError):
-            return False
-
-        return self.to_dict() == other.to_dict()
-
-    def __ne__(self, other):
-        """Returns true if both objects are not equal"""
-        if not isinstance(other, DataJobQueryResponseWithError):
-            return True
 
-        return self.to_dict() != other.to_dict()
+
+    class MetaOapg:
+        
+        class properties:
+            
+            
+            class errors(
+                schemas.ListSchema
+            ):
+            
+            
+                class MetaOapg:
+                    items = schemas.DictSchema
+            
+                def __new__(
+                    cls,
+                    _arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, dict, frozendict.frozendict, ]], typing.List[typing.Union[MetaOapg.items, dict, frozendict.frozendict, ]]],
+                    _configuration: typing.Optional[schemas.Configuration] = None,
+                ) -> 'errors':
+                    return super().__new__(
+                        cls,
+                        _arg,
+                        _configuration=_configuration,
+                    )
+            
+                def __getitem__(self, i: int) -> MetaOapg.items:
+                    return super().__getitem__(i)
+        
+            @staticmethod
+            def data() -> typing.Type['DataJobPage']:
+                return DataJobPage
+            __annotations__ = {
+                "errors": errors,
+                "data": data,
+            }
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["errors"]) -> MetaOapg.properties.errors: ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["data"]) -> 'DataJobPage': ...
+    
+    @typing.overload
+    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
+    
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["errors", "data", ], str]):
+        # dict_instance[name] accessor
+        return super().__getitem__(name)
+    
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["errors"]) -> typing.Union[MetaOapg.properties.errors, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["data"]) -> typing.Union['DataJobPage', schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
+    
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["errors", "data", ], str]):
+        return super().get_item_oapg(name)
+    
+
+    def __new__(
+        cls,
+        *_args: typing.Union[dict, frozendict.frozendict, ],
+        errors: typing.Union[MetaOapg.properties.errors, list, tuple, schemas.Unset] = schemas.unset,
+        data: typing.Union['DataJobPage', schemas.Unset] = schemas.unset,
+        _configuration: typing.Optional[schemas.Configuration] = None,
+        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+    ) -> 'DataJobQueryResponse':
+        return super().__new__(
+            cls,
+            *_args,
+            errors=errors,
+            data=data,
+            _configuration=_configuration,
+            **kwargs,
+        )
+
+from taurus_datajob_api.model.data_job_page import DataJobPage
```

### Comparing `vdk-control-service-api-1.0.6/taurus_datajob_api/models/data_job_schedule.py` & `vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_query_response_with_error.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,122 +1,117 @@
 # coding: utf-8
 
 """
     Versatile Data Kit Control Service API
 
-    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction  The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br  The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time).                      The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning.                            Implementation of the API is not considered stable nor well tested.                            Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade.                          The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.   # noqa: E501
+    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import pprint
+from datetime import date, datetime  # noqa: F401
+import decimal  # noqa: F401
+import functools  # noqa: F401
+import io  # noqa: F401
 import re  # noqa: F401
+import typing  # noqa: F401
+import typing_extensions  # noqa: F401
+import uuid  # noqa: F401
 
-import six
+import frozendict  # noqa: F401
 
-from taurus_datajob_api.configuration import Configuration
+from taurus_datajob_api import schemas  # noqa: F401
 
 
-class DataJobSchedule(object):
+class DataJobQueryResponseWithError(
+    schemas.DictSchema
+):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
-    """
 
+    Query response containing Data Jobs
     """
-    Attributes:
-      openapi_types (dict): The key is attribute name
-                            and the value is attribute type.
-      attribute_map (dict): The key is attribute name
-                            and the value is json key in definition.
-    """
-    openapi_types = {
-        'schedule_cron': 'str'
-    }
-
-    attribute_map = {
-        'schedule_cron': 'schedule_cron'
-    }
-
-    def __init__(self, schedule_cron=None, local_vars_configuration=None):  # noqa: E501
-        """DataJobSchedule - a model defined in OpenAPI"""  # noqa: E501
-        if local_vars_configuration is None:
-            local_vars_configuration = Configuration()
-        self.local_vars_configuration = local_vars_configuration
-
-        self._schedule_cron = None
-        self.discriminator = None
-
-        if schedule_cron is not None:
-            self.schedule_cron = schedule_cron
-
-    @property
-    def schedule_cron(self):
-        """Gets the schedule_cron of this DataJobSchedule.  # noqa: E501
-
-        For format see https://en.wikipedia.org/wiki/Cron<br> The cron expression is evaluated in UTC time. If it is time for a new job run and the previous job run hasn't finished yet, the cron job kills and replaces the currently running job run with a new job run. Jobs configured to run more often than once per hour are not supported and their schedule may be overridden by the platform. To distribute load evenly, Administrators may override the minute you specified. Use https://crontab.guru for help.   # noqa: E501
-
-        :return: The schedule_cron of this DataJobSchedule.  # noqa: E501
-        :rtype: str
-        """
-        return self._schedule_cron
-
-    @schedule_cron.setter
-    def schedule_cron(self, schedule_cron):
-        """Sets the schedule_cron of this DataJobSchedule.
-
-        For format see https://en.wikipedia.org/wiki/Cron<br> The cron expression is evaluated in UTC time. If it is time for a new job run and the previous job run hasn't finished yet, the cron job kills and replaces the currently running job run with a new job run. Jobs configured to run more often than once per hour are not supported and their schedule may be overridden by the platform. To distribute load evenly, Administrators may override the minute you specified. Use https://crontab.guru for help.   # noqa: E501
-
-        :param schedule_cron: The schedule_cron of this DataJobSchedule.  # noqa: E501
-        :type: str
-        """
-
-        self._schedule_cron = schedule_cron
-
-    def to_dict(self):
-        """Returns the model properties as a dict"""
-        result = {}
-
-        for attr, _ in six.iteritems(self.openapi_types):
-            value = getattr(self, attr)
-            if isinstance(value, list):
-                result[attr] = list(map(
-                    lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
-                    value
-                ))
-            elif hasattr(value, "to_dict"):
-                result[attr] = value.to_dict()
-            elif isinstance(value, dict):
-                result[attr] = dict(map(
-                    lambda item: (item[0], item[1].to_dict())
-                    if hasattr(item[1], "to_dict") else item,
-                    value.items()
-                ))
-            else:
-                result[attr] = value
-
-        return result
-
-    def to_str(self):
-        """Returns the string representation of the model"""
-        return pprint.pformat(self.to_dict())
-
-    def __repr__(self):
-        """For `print` and `pprint`"""
-        return self.to_str()
-
-    def __eq__(self, other):
-        """Returns true if both objects are equal"""
-        if not isinstance(other, DataJobSchedule):
-            return False
-
-        return self.to_dict() == other.to_dict()
-
-    def __ne__(self, other):
-        """Returns true if both objects are not equal"""
-        if not isinstance(other, DataJobSchedule):
-            return True
 
-        return self.to_dict() != other.to_dict()
+
+    class MetaOapg:
+        
+        class properties:
+            
+            
+            class errors(
+                schemas.ListSchema
+            ):
+            
+            
+                class MetaOapg:
+                    items = schemas.DictSchema
+            
+                def __new__(
+                    cls,
+                    _arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, dict, frozendict.frozendict, ]], typing.List[typing.Union[MetaOapg.items, dict, frozendict.frozendict, ]]],
+                    _configuration: typing.Optional[schemas.Configuration] = None,
+                ) -> 'errors':
+                    return super().__new__(
+                        cls,
+                        _arg,
+                        _configuration=_configuration,
+                    )
+            
+                def __getitem__(self, i: int) -> MetaOapg.items:
+                    return super().__getitem__(i)
+        
+            @staticmethod
+            def data() -> typing.Type['DataJobPage']:
+                return DataJobPage
+            __annotations__ = {
+                "errors": errors,
+                "data": data,
+            }
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["errors"]) -> MetaOapg.properties.errors: ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["data"]) -> 'DataJobPage': ...
+    
+    @typing.overload
+    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
+    
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["errors", "data", ], str]):
+        # dict_instance[name] accessor
+        return super().__getitem__(name)
+    
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["errors"]) -> typing.Union[MetaOapg.properties.errors, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["data"]) -> typing.Union['DataJobPage', schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
+    
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["errors", "data", ], str]):
+        return super().get_item_oapg(name)
+    
+
+    def __new__(
+        cls,
+        *_args: typing.Union[dict, frozendict.frozendict, ],
+        errors: typing.Union[MetaOapg.properties.errors, list, tuple, schemas.Unset] = schemas.unset,
+        data: typing.Union['DataJobPage', schemas.Unset] = schemas.unset,
+        _configuration: typing.Optional[schemas.Configuration] = None,
+        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+    ) -> 'DataJobQueryResponseWithError':
+        return super().__new__(
+            cls,
+            *_args,
+            errors=errors,
+            data=data,
+            _configuration=_configuration,
+            **kwargs,
+        )
+
+from taurus_datajob_api.model.data_job_page import DataJobPage
```

### Comparing `vdk-control-service-api-1.0.6/taurus_datajob_api/models/data_job_version.py` & `vdk-control-service-api-1.0.7/taurus_datajob_api/model/error.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,123 +1,107 @@
 # coding: utf-8
 
 """
     Versatile Data Kit Control Service API
 
-    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction  The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br  The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time).                      The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning.                            Implementation of the API is not considered stable nor well tested.                            Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade.                          The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.   # noqa: E501
+    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import pprint
+from datetime import date, datetime  # noqa: F401
+import decimal  # noqa: F401
+import functools  # noqa: F401
+import io  # noqa: F401
 import re  # noqa: F401
+import typing  # noqa: F401
+import typing_extensions  # noqa: F401
+import uuid  # noqa: F401
 
-import six
+import frozendict  # noqa: F401
 
-from taurus_datajob_api.configuration import Configuration
+from taurus_datajob_api import schemas  # noqa: F401
 
 
-class DataJobVersion(object):
+class Error(
+    schemas.DictSchema
+):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
-    """
 
+    Contains description for one or more errors detected.
     """
-    Attributes:
-      openapi_types (dict): The key is attribute name
-                            and the value is attribute type.
-      attribute_map (dict): The key is attribute name
-                            and the value is json key in definition.
-    """
-    openapi_types = {
-        'version_sha': 'str'
-    }
-
-    attribute_map = {
-        'version_sha': 'version_sha'
-    }
-
-    def __init__(self, version_sha=None, local_vars_configuration=None):  # noqa: E501
-        """DataJobVersion - a model defined in OpenAPI"""  # noqa: E501
-        if local_vars_configuration is None:
-            local_vars_configuration = Configuration()
-        self.local_vars_configuration = local_vars_configuration
-
-        self._version_sha = None
-        self.discriminator = None
-
-        self.version_sha = version_sha
-
-    @property
-    def version_sha(self):
-        """Gets the version_sha of this DataJobVersion.  # noqa: E501
-
-        SHA hash which specifies the latest deployed version of the data job  # noqa: E501
-
-        :return: The version_sha of this DataJobVersion.  # noqa: E501
-        :rtype: str
-        """
-        return self._version_sha
-
-    @version_sha.setter
-    def version_sha(self, version_sha):
-        """Sets the version_sha of this DataJobVersion.
-
-        SHA hash which specifies the latest deployed version of the data job  # noqa: E501
-
-        :param version_sha: The version_sha of this DataJobVersion.  # noqa: E501
-        :type: str
-        """
-        if self.local_vars_configuration.client_side_validation and version_sha is None:  # noqa: E501
-            raise ValueError("Invalid value for `version_sha`, must not be `None`")  # noqa: E501
-
-        self._version_sha = version_sha
-
-    def to_dict(self):
-        """Returns the model properties as a dict"""
-        result = {}
-
-        for attr, _ in six.iteritems(self.openapi_types):
-            value = getattr(self, attr)
-            if isinstance(value, list):
-                result[attr] = list(map(
-                    lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
-                    value
-                ))
-            elif hasattr(value, "to_dict"):
-                result[attr] = value.to_dict()
-            elif isinstance(value, dict):
-                result[attr] = dict(map(
-                    lambda item: (item[0], item[1].to_dict())
-                    if hasattr(item[1], "to_dict") else item,
-                    value.items()
-                ))
-            else:
-                result[attr] = value
-
-        return result
-
-    def to_str(self):
-        """Returns the string representation of the model"""
-        return pprint.pformat(self.to_dict())
-
-    def __repr__(self):
-        """For `print` and `pprint`"""
-        return self.to_str()
-
-    def __eq__(self, other):
-        """Returns true if both objects are equal"""
-        if not isinstance(other, DataJobVersion):
-            return False
-
-        return self.to_dict() == other.to_dict()
-
-    def __ne__(self, other):
-        """Returns true if both objects are not equal"""
-        if not isinstance(other, DataJobVersion):
-            return True
 
-        return self.to_dict() != other.to_dict()
+
+    class MetaOapg:
+        required = {
+            "messages",
+        }
+        
+        class properties:
+            
+            
+            class messages(
+                schemas.ListSchema
+            ):
+            
+            
+                class MetaOapg:
+                    items = schemas.StrSchema
+            
+                def __new__(
+                    cls,
+                    _arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, ]], typing.List[typing.Union[MetaOapg.items, str, ]]],
+                    _configuration: typing.Optional[schemas.Configuration] = None,
+                ) -> 'messages':
+                    return super().__new__(
+                        cls,
+                        _arg,
+                        _configuration=_configuration,
+                    )
+            
+                def __getitem__(self, i: int) -> MetaOapg.items:
+                    return super().__getitem__(i)
+            __annotations__ = {
+                "messages": messages,
+            }
+    
+    messages: MetaOapg.properties.messages
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["messages"]) -> MetaOapg.properties.messages: ...
+    
+    @typing.overload
+    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
+    
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["messages", ], str]):
+        # dict_instance[name] accessor
+        return super().__getitem__(name)
+    
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["messages"]) -> MetaOapg.properties.messages: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
+    
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["messages", ], str]):
+        return super().get_item_oapg(name)
+    
+
+    def __new__(
+        cls,
+        *_args: typing.Union[dict, frozendict.frozendict, ],
+        messages: typing.Union[MetaOapg.properties.messages, list, tuple, ],
+        _configuration: typing.Optional[schemas.Configuration] = None,
+        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+    ) -> 'Error':
+        return super().__new__(
+            cls,
+            *_args,
+            messages=messages,
+            _configuration=_configuration,
+            **kwargs,
+        )
```

### Comparing `vdk-control-service-api-1.0.6/taurus_datajob_api/configuration.py` & `vdk-control-service-api-1.0.7/taurus_datajob_api/configuration.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 # coding: utf-8
 
 """
     Versatile Data Kit Control Service API
 
-    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction  The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br  The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time).                      The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning.                            Implementation of the API is not considered stable nor well tested.                            Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade.                          The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.   # noqa: E501
+    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
 import copy
 import logging
 import multiprocessing
 import sys
 import urllib3
 
-import six
-from six.moves import http_client as httplib
+from http import client as http_client
+from taurus_datajob_api.exceptions import ApiValueError
+
 
+JSON_SCHEMA_VALIDATION_KEYWORDS = {
+    'multipleOf', 'maximum', 'exclusiveMaximum',
+    'minimum', 'exclusiveMinimum', 'maxLength',
+    'minLength', 'pattern', 'maxItems', 'minItems',
+    'uniqueItems', 'maxProperties', 'minProperties',
+}
 
 class Configuration(object):
     """NOTE: This class is auto generated by OpenAPI Generator
 
     Ref: https://openapi-generator.tech
     Do not edit the class manually.
 
@@ -45,57 +49,70 @@
          implementation.
       2. The client was generated using an older version of the OpenAPI document
          and the server has been upgraded since then.
       If a schema in the OpenAPI document defines the additionalProperties attribute,
       then all undeclared properties received by the server are injected into the
       additional properties map. In that case, there are undeclared properties, and
       nothing to discard.
+    :param disabled_client_side_validations (string): Comma-separated list of
+      JSON schema validation keywords to disable JSON schema structural validation
+      rules. The following keywords may be specified: multipleOf, maximum,
+      exclusiveMaximum, minimum, exclusiveMinimum, maxLength, minLength, pattern,
+      maxItems, minItems.
+      By default, the validation is performed for data generated locally by the client
+      and data received from the server, independent of any validation performed by
+      the server side. If the input data does not satisfy the JSON schema validation
+      rules specified in the OpenAPI document, an exception is raised.
+      If disabled_client_side_validations is set, structural validation is
+      disabled. This can be useful to troubleshoot data validation problem, such as
+      when the OpenAPI document validation rules do not match the actual API data
+      received by the server.
+    :param server_index: Index to servers configuration.
+    :param server_variables: Mapping with string values to replace variables in
+      templated server configuration. The validation of enums is performed for
+      variables with defined enum values before.
+    :param server_operation_index: Mapping from operation ID to an index to server
+      configuration.
+    :param server_operation_variables: Mapping from operation ID to a mapping with
+      string values to replace variables in templated server configuration.
+      The validation of enums is performed for variables with defined enum values before.
 
     :Example:
     """
 
     _default = None
 
-    def __init__(self, host="http://localhost",
-                 api_key=None, api_key_prefix=None,
-                 username=None, password=None,
-                 discard_unknown_keys=False,
-                 ):
+    def __init__(
+        self,
+        host=None,
+        discard_unknown_keys=False,
+        disabled_client_side_validations="",
+        server_index=None,
+        server_variables=None,
+        server_operation_index=None,
+        server_operation_variables=None,
+    ):
         """Constructor
         """
-        self.host = host
+        self._base_path = "http://localhost" if host is None else host
         """Default Base url
         """
+        self.server_index = 0 if server_index is None and host is None else server_index
+        self.server_operation_index = server_operation_index or {}
+        """Default server index
+        """
+        self.server_variables = server_variables or {}
+        self.server_operation_variables = server_operation_variables or {}
+        """Default server variables
+        """
         self.temp_folder_path = None
         """Temp file folder for downloading files
         """
         # Authentication Settings
-        self.api_key = {}
-        if api_key:
-            self.api_key = api_key
-        """dict to store API key(s)
-        """
-        self.api_key_prefix = {}
-        if api_key_prefix:
-            self.api_key_prefix = api_key_prefix
-        """dict to store API prefix (e.g. Bearer)
-        """
-        self.refresh_api_key_hook = None
-        """function hook to refresh API key if expired
-        """
-        self.username = username
-        """Username for HTTP basic authentication
-        """
-        self.password = password
-        """Password for HTTP basic authentication
-        """
-        self.discard_unknown_keys = discard_unknown_keys
-        self.access_token = None
-        """access token for OAuth/Bearer
-        """
+        self.disabled_client_side_validations = disabled_client_side_validations
         self.logger = {}
         """Logging Settings
         """
         self.logger["package_logger"] = logging.getLogger("taurus_datajob_api")
         self.logger["urllib3_logger"] = logging.getLogger("urllib3")
         self.logger_format = '%(asctime)s %(levelname)s %(message)s'
         """Log format
@@ -147,31 +164,44 @@
         """
         self.safe_chars_for_path_param = ''
         """Safe chars for path_param
         """
         self.retries = None
         """Adding retries to override urllib3 default value 3
         """
-        # Disable client side validation
+        # Enable client side validation
         self.client_side_validation = True
 
+        # Options to pass down to the underlying urllib3 socket
+        self.socket_options = None
+
     def __deepcopy__(self, memo):
         cls = self.__class__
         result = cls.__new__(cls)
         memo[id(self)] = result
         for k, v in self.__dict__.items():
             if k not in ('logger', 'logger_file_handler'):
                 setattr(result, k, copy.deepcopy(v, memo))
         # shallow copy of loggers
         result.logger = copy.copy(self.logger)
         # use setters to configure loggers
         result.logger_file = self.logger_file
         result.debug = self.debug
         return result
 
+    def __setattr__(self, name, value):
+        object.__setattr__(self, name, value)
+        if name == 'disabled_client_side_validations':
+            s = set(filter(None, value.split(',')))
+            for v in s:
+                if v not in JSON_SCHEMA_VALIDATION_KEYWORDS:
+                    raise ApiValueError(
+                        "Invalid keyword: '{0}''".format(v))
+            self._disabled_client_side_validations = s
+
     @classmethod
     def set_default(cls, default):
         """Set default instance of configuration.
 
         It stores default configuration, which can be
         returned by get_default_copy method.
 
@@ -217,15 +247,15 @@
         """
         self.__logger_file = value
         if self.__logger_file:
             # If set logging file,
             # then add file handler and remove stream handler.
             self.logger_file_handler = logging.FileHandler(self.__logger_file)
             self.logger_file_handler.setFormatter(self.logger_formatter)
-            for _, logger in six.iteritems(self.logger):
+            for _, logger in self.logger.items():
                 logger.addHandler(self.logger_file_handler)
 
     @property
     def debug(self):
         """Debug status
 
         :param value: The debug status, True or False.
@@ -239,25 +269,25 @@
 
         :param value: The debug status, True or False.
         :type: bool
         """
         self.__debug = value
         if self.__debug:
             # if debug status is True, turn on debug logging
-            for _, logger in six.iteritems(self.logger):
+            for _, logger in self.logger.items():
                 logger.setLevel(logging.DEBUG)
-            # turn on httplib debug
-            httplib.HTTPConnection.debuglevel = 1
+            # turn on http_client debug
+            http_client.HTTPConnection.debuglevel = 1
         else:
             # if debug status is False, turn off debug logging,
             # setting log level to default `logging.WARNING`
-            for _, logger in six.iteritems(self.logger):
+            for _, logger in self.logger.items():
                 logger.setLevel(logging.WARNING)
-            # turn off httplib debug
-            httplib.HTTPConnection.debuglevel = 0
+            # turn off http_client debug
+            http_client.HTTPConnection.debuglevel = 0
 
     @property
     def logger_format(self):
         """The logger format.
 
         The logger_formatter will be updated when sets logger_format.
 
@@ -274,23 +304,24 @@
 
         :param value: The format string.
         :type: str
         """
         self.__logger_format = value
         self.logger_formatter = logging.Formatter(self.__logger_format)
 
-    def get_api_key_with_prefix(self, identifier):
+    def get_api_key_with_prefix(self, identifier, alias=None):
         """Gets API key (with prefix if set).
 
         :param identifier: The identifier of apiKey.
+        :param alias: The alternative identifier of apiKey.
         :return: The token for api key authentication.
         """
         if self.refresh_api_key_hook is not None:
             self.refresh_api_key_hook(self)
-        key = self.api_key.get(identifier)
+        key = self.api_key.get(identifier, self.api_key.get(alias) if alias is not None else None)
         if key:
             prefix = self.api_key_prefix.get(identifier)
             if prefix:
                 return "%s %s" % (prefix, key)
             else:
                 return key
 
@@ -330,56 +361,71 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0\n"\
-               "SDK Package Version: 1.0.6".\
+               "SDK Package Version: 1.0.7".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
         return [
             {
-                'url': "/",
+                'url': "",
                 'description': "No description provided",
             }
         ]
 
-    def get_host_from_settings(self, index, variables=None):
+    def get_host_from_settings(self, index, variables=None, servers=None):
         """Gets host URL based on the index and variables
         :param index: array index of the host settings
         :param variables: hash of variable and the corresponding value
+        :param servers: an array of host settings or None
         :return: URL based on host settings
         """
+        if index is None:
+            return self._base_path
+
         variables = {} if variables is None else variables
-        servers = self.get_host_settings()
+        servers = self.get_host_settings() if servers is None else servers
 
         try:
             server = servers[index]
         except IndexError:
             raise ValueError(
                 "Invalid index {0} when selecting the host settings. "
                 "Must be less than {1}".format(index, len(servers)))
 
         url = server['url']
 
         # go through variables and replace placeholders
-        for variable_name, variable in server['variables'].items():
+        for variable_name, variable in server.get('variables', {}).items():
             used_value = variables.get(
                 variable_name, variable['default_value'])
 
             if 'enum_values' in variable \
                     and used_value not in variable['enum_values']:
                 raise ValueError(
                     "The variable `{0}` in the host URL has invalid value "
                     "{1}. Must be {2}.".format(
                         variable_name, variables[variable_name],
                         variable['enum_values']))
 
             url = url.replace("{" + variable_name + "}", used_value)
 
         return url
+
+    @property
+    def host(self):
+        """Return generated host."""
+        return self.get_host_from_settings(self.server_index, variables=self.server_variables)
+
+    @host.setter
+    def host(self, value):
+        """Fix base path."""
+        self._base_path = value
+        self.server_index = None
```

### Comparing `vdk-control-service-api-1.0.6/taurus_datajob_api/exceptions.py` & `vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_execution_request.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,120 +1,118 @@
 # coding: utf-8
 
 """
     Versatile Data Kit Control Service API
 
-    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction  The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br  The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time).                      The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning.                            Implementation of the API is not considered stable nor well tested.                            Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade.                          The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.   # noqa: E501
+    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
-
-import six
-
-
-class OpenApiException(Exception):
-    """The base exception class for all OpenAPIExceptions"""
-
-
-class ApiTypeError(OpenApiException, TypeError):
-    def __init__(self, msg, path_to_item=None, valid_classes=None,
-                 key_type=None):
-        """ Raises an exception for TypeErrors
-
-        Args:
-            msg (str): the exception message
-
-        Keyword Args:
-            path_to_item (list): a list of keys an indices to get to the
-                                 current_item
-                                 None if unset
-            valid_classes (tuple): the primitive classes that current item
-                                   should be an instance of
-                                   None if unset
-            key_type (bool): False if our value is a value in a dict
-                             True if it is a key in a dict
-                             False if our item is an item in a list
-                             None if unset
-        """
-        self.path_to_item = path_to_item
-        self.valid_classes = valid_classes
-        self.key_type = key_type
-        full_msg = msg
-        if path_to_item:
-            full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
-        super(ApiTypeError, self).__init__(full_msg)
-
-
-class ApiValueError(OpenApiException, ValueError):
-    def __init__(self, msg, path_to_item=None):
-        """
-        Args:
-            msg (str): the exception message
-
-        Keyword Args:
-            path_to_item (list) the path to the exception in the
-                received_data dict. None if unset
-        """
-
-        self.path_to_item = path_to_item
-        full_msg = msg
-        if path_to_item:
-            full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
-        super(ApiValueError, self).__init__(full_msg)
-
-
-class ApiKeyError(OpenApiException, KeyError):
-    def __init__(self, msg, path_to_item=None):
-        """
-        Args:
-            msg (str): the exception message
-
-        Keyword Args:
-            path_to_item (None/list) the path to the exception in the
-                received_data dict
-        """
-        self.path_to_item = path_to_item
-        full_msg = msg
-        if path_to_item:
-            full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
-        super(ApiKeyError, self).__init__(full_msg)
-
-
-class ApiException(OpenApiException):
-
-    def __init__(self, status=None, reason=None, http_resp=None):
-        if http_resp:
-            self.status = http_resp.status
-            self.reason = http_resp.reason
-            self.body = http_resp.data
-            self.headers = http_resp.getheaders()
-        else:
-            self.status = status
-            self.reason = reason
-            self.body = None
-            self.headers = None
-
-    def __str__(self):
-        """Custom error messages for exception"""
-        error_message = "({0})\n"\
-                        "Reason: {1}\n".format(self.status, self.reason)
-        if self.headers:
-            error_message += "HTTP response headers: {0}\n".format(
-                self.headers)
-
-        if self.body:
-            error_message += "HTTP response body: {0}\n".format(self.body)
-
-        return error_message
-
-
-def render_path(path_to_item):
-    """Returns a string representation of a path"""
-    result = ""
-    for pth in path_to_item:
-        if isinstance(pth, six.integer_types):
-            result += "[{0}]".format(pth)
-        else:
-            result += "['{0}']".format(pth)
-    return result
+from datetime import date, datetime  # noqa: F401
+import decimal  # noqa: F401
+import functools  # noqa: F401
+import io  # noqa: F401
+import re  # noqa: F401
+import typing  # noqa: F401
+import typing_extensions  # noqa: F401
+import uuid  # noqa: F401
+
+import frozendict  # noqa: F401
+
+from taurus_datajob_api import schemas  # noqa: F401
+
+
+class DataJobExecutionRequest(
+    schemas.DictSchema
+):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+
+    Request to start execution of Data Job. The job must have been deployed before that (see Deployment API) and will run its latest version.
+    """
+
+
+    class MetaOapg:
+        
+        class properties:
+            started_by = schemas.StrSchema
+            
+            
+            class args(
+                schemas.DictSchema
+            ):
+            
+            
+                class MetaOapg:
+                    additional_properties = schemas.AnyTypeSchema
+                
+                def __getitem__(self, name: typing.Union[str, ]) -> MetaOapg.additional_properties:
+                    # dict_instance[name] accessor
+                    return super().__getitem__(name)
+                
+                def get_item_oapg(self, name: typing.Union[str, ]) -> MetaOapg.additional_properties:
+                    return super().get_item_oapg(name)
+            
+                def __new__(
+                    cls,
+                    *_args: typing.Union[dict, frozendict.frozendict, ],
+                    _configuration: typing.Optional[schemas.Configuration] = None,
+                    **kwargs: typing.Union[MetaOapg.additional_properties, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+                ) -> 'args':
+                    return super().__new__(
+                        cls,
+                        *_args,
+                        _configuration=_configuration,
+                        **kwargs,
+                    )
+            __annotations__ = {
+                "started_by": started_by,
+                "args": args,
+            }
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["started_by"]) -> MetaOapg.properties.started_by: ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["args"]) -> MetaOapg.properties.args: ...
+    
+    @typing.overload
+    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
+    
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["started_by", "args", ], str]):
+        # dict_instance[name] accessor
+        return super().__getitem__(name)
+    
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["started_by"]) -> typing.Union[MetaOapg.properties.started_by, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["args"]) -> typing.Union[MetaOapg.properties.args, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
+    
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["started_by", "args", ], str]):
+        return super().get_item_oapg(name)
+    
+
+    def __new__(
+        cls,
+        *_args: typing.Union[dict, frozendict.frozendict, ],
+        started_by: typing.Union[MetaOapg.properties.started_by, str, schemas.Unset] = schemas.unset,
+        args: typing.Union[MetaOapg.properties.args, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
+        _configuration: typing.Optional[schemas.Configuration] = None,
+        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+    ) -> 'DataJobExecutionRequest':
+        return super().__new__(
+            cls,
+            *_args,
+            started_by=started_by,
+            args=args,
+            _configuration=_configuration,
+            **kwargs,
+        )
```

### Comparing `vdk-control-service-api-1.0.6/taurus_datajob_api/rest.py` & `vdk-control-service-api-1.0.7/taurus_datajob_api/rest.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,33 @@
 # coding: utf-8
 
 """
     Versatile Data Kit Control Service API
 
-    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction  The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br  The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time).                      The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning.                            Implementation of the API is not considered stable nor well tested.                            Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade.                          The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.   # noqa: E501
+    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
-import io
-import json
 import logging
-import re
 import ssl
+from urllib.parse import urlencode
+import typing
 
 import certifi
-# python 2 and python 3 compatibility library
-import six
-from six.moves.urllib.parse import urlencode
 import urllib3
+from urllib3._collections import HTTPHeaderDict
 
 from taurus_datajob_api.exceptions import ApiException, ApiValueError
 
 
 logger = logging.getLogger(__name__)
 
 
-class RESTResponse(io.IOBase):
-
-    def __init__(self, resp):
-        self.urllib3_response = resp
-        self.status = resp.status
-        self.reason = resp.reason
-        self.data = resp.data
-
-    def getheaders(self):
-        """Returns a dictionary of the response headers."""
-        return self.urllib3_response.getheaders()
-
-    def getheader(self, name, default=None):
-        """Returns a given response header."""
-        return self.urllib3_response.getheader(name, default)
-
-
 class RESTClientObject(object):
 
     def __init__(self, configuration, pools_size=4, maxsize=None):
         # urllib3.PoolManager will pass all kw parameters to connectionpool
         # https://github.com/shazow/urllib3/blob/f9409436f83aeb79fbaf090181cd81b784f1b8ce/urllib3/poolmanager.py#L75  # noqa: E501
         # https://github.com/shazow/urllib3/blob/f9409436f83aeb79fbaf090181cd81b784f1b8ce/urllib3/connectionpool.py#L680  # noqa: E501
         # maxsize is the number of requests to host that are allowed in parallel  # noqa: E501
@@ -72,14 +49,17 @@
         addition_pool_args = {}
         if configuration.assert_hostname is not None:
             addition_pool_args['assert_hostname'] = configuration.assert_hostname  # noqa: E501
 
         if configuration.retries is not None:
             addition_pool_args['retries'] = configuration.retries
 
+        if configuration.socket_options is not None:
+            addition_pool_args['socket_options'] = configuration.socket_options
+
         if maxsize is None:
             if configuration.connection_pool_maxsize is not None:
                 maxsize = configuration.connection_pool_maxsize
             else:
                 maxsize = 4
 
         # https pool manager
@@ -102,195 +82,173 @@
                 cert_reqs=cert_reqs,
                 ca_certs=ca_certs,
                 cert_file=configuration.cert_file,
                 key_file=configuration.key_file,
                 **addition_pool_args
             )
 
-    def request(self, method, url, query_params=None, headers=None,
-                body=None, post_params=None, _preload_content=True,
-                _request_timeout=None):
+    def request(
+        self,
+        method: str,
+        url: str,
+        headers: typing.Optional[HTTPHeaderDict] = None,
+        fields: typing.Optional[typing.Tuple[typing.Tuple[str, typing.Any], ...]] = None,
+        body: typing.Optional[typing.Union[str, bytes]] = None,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+    ) -> urllib3.HTTPResponse:
         """Perform requests.
 
         :param method: http request method
         :param url: http request url
-        :param query_params: query parameters in the url
         :param headers: http request headers
-        :param body: request json body, for `application/json`
-        :param post_params: request post parameters,
-                            `application/x-www-form-urlencoded`
-                            and `multipart/form-data`
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
+        :param body: request body, for other types
+        :param fields: request parameters for
+                                `application/x-www-form-urlencoded`
+                                or `multipart/form-data`
+        :param stream: if True, the urllib3.HTTPResponse object will
+                                be returned without reading/decoding response
+                                data. Default is False.
+        :param timeout: timeout setting for this request. If one
+                                number provided, it will be total request
+                                timeout. It can also be a pair (tuple) of
+                                (connection, read) timeouts.
         """
         method = method.upper()
         assert method in ['GET', 'HEAD', 'DELETE', 'POST', 'PUT',
                           'PATCH', 'OPTIONS']
 
-        if post_params and body:
+        if fields and body:
             raise ApiValueError(
-                "body parameter cannot be used with post_params parameter."
+                "body parameter cannot be used with fields parameter."
             )
 
-        post_params = post_params or {}
+        fields = fields or {}
         headers = headers or {}
 
-        timeout = None
-        if _request_timeout:
-            if isinstance(_request_timeout, (int, ) if six.PY3 else (int, long)):  # noqa: E501,F821
-                timeout = urllib3.Timeout(total=_request_timeout)
-            elif (isinstance(_request_timeout, tuple) and
-                  len(_request_timeout) == 2):
-                timeout = urllib3.Timeout(
-                    connect=_request_timeout[0], read=_request_timeout[1])
-
-        if 'Content-Type' not in headers:
-            headers['Content-Type'] = 'application/json'
+        if timeout:
+            if isinstance(timeout, (int, float)):  # noqa: E501,F821
+                timeout = urllib3.Timeout(total=timeout)
+            elif (isinstance(timeout, tuple) and
+                  len(timeout) == 2):
+                timeout = urllib3.Timeout(connect=timeout[0], read=timeout[1])
 
         try:
             # For `POST`, `PUT`, `PATCH`, `OPTIONS`, `DELETE`
             if method in ['POST', 'PUT', 'PATCH', 'OPTIONS', 'DELETE']:
-                if query_params:
-                    url += '?' + urlencode(query_params)
-                if re.search('json', headers['Content-Type'], re.IGNORECASE):
-                    request_body = None
-                    if body is not None:
-                        request_body = json.dumps(body)
+                if 'Content-Type' not in headers and body is None:
                     r = self.pool_manager.request(
-                        method, url,
-                        body=request_body,
-                        preload_content=_preload_content,
+                        method,
+                        url,
+                        preload_content=not stream,
                         timeout=timeout,
-                        headers=headers)
+                        headers=headers
+                    )
                 elif headers['Content-Type'] == 'application/x-www-form-urlencoded':  # noqa: E501
                     r = self.pool_manager.request(
                         method, url,
-                        fields=post_params,
+                        body=body,
+                        fields=fields,
                         encode_multipart=False,
-                        preload_content=_preload_content,
+                        preload_content=not stream,
                         timeout=timeout,
                         headers=headers)
                 elif headers['Content-Type'] == 'multipart/form-data':
                     # must del headers['Content-Type'], or the correct
                     # Content-Type which generated by urllib3 will be
                     # overwritten.
                     del headers['Content-Type']
                     r = self.pool_manager.request(
                         method, url,
-                        fields=post_params,
+                        fields=fields,
                         encode_multipart=True,
-                        preload_content=_preload_content,
+                        preload_content=not stream,
                         timeout=timeout,
                         headers=headers)
                 # Pass a `string` parameter directly in the body to support
                 # other content types than Json when `body` argument is
                 # provided in serialized form
                 elif isinstance(body, str) or isinstance(body, bytes):
                     request_body = body
                     r = self.pool_manager.request(
                         method, url,
                         body=request_body,
-                        preload_content=_preload_content,
+                        preload_content=not stream,
                         timeout=timeout,
                         headers=headers)
                 else:
                     # Cannot generate the request from given parameters
                     msg = """Cannot prepare a request message for provided
                              arguments. Please check that your arguments match
                              declared content type."""
                     raise ApiException(status=0, reason=msg)
             # For `GET`, `HEAD`
             else:
                 r = self.pool_manager.request(method, url,
-                                              fields=query_params,
-                                              preload_content=_preload_content,
+                                              preload_content=not stream,
                                               timeout=timeout,
                                               headers=headers)
         except urllib3.exceptions.SSLError as e:
             msg = "{0}\n{1}".format(type(e).__name__, str(e))
             raise ApiException(status=0, reason=msg)
 
-        if _preload_content:
-            r = RESTResponse(r)
-
-            # In the python 3, the response.data is bytes.
-            # we need to decode it to string.
-            if six.PY3:
-                r.data = r.data.decode('utf8')
-
+        if not stream:
             # log response body
             logger.debug("response body: %s", r.data)
 
-        if not 200 <= r.status <= 299:
-            raise ApiException(http_resp=r)
-
         return r
 
-    def GET(self, url, headers=None, query_params=None, _preload_content=True,
-            _request_timeout=None):
+    def GET(self, url, headers=None, stream=False,
+            timeout=None, fields=None) -> urllib3.HTTPResponse:
         return self.request("GET", url,
                             headers=headers,
-                            _preload_content=_preload_content,
-                            _request_timeout=_request_timeout,
-                            query_params=query_params)
+                            stream=stream,
+                            timeout=timeout,
+                            fields=fields)
 
-    def HEAD(self, url, headers=None, query_params=None, _preload_content=True,
-             _request_timeout=None):
+    def HEAD(self, url, headers=None, stream=False,
+             timeout=None, fields=None) -> urllib3.HTTPResponse:
         return self.request("HEAD", url,
                             headers=headers,
-                            _preload_content=_preload_content,
-                            _request_timeout=_request_timeout,
-                            query_params=query_params)
+                            stream=stream,
+                            timeout=timeout,
+                            fields=fields)
 
-    def OPTIONS(self, url, headers=None, query_params=None, post_params=None,
-                body=None, _preload_content=True, _request_timeout=None):
+    def OPTIONS(self, url, headers=None,
+                body=None, stream=False, timeout=None, fields=None) -> urllib3.HTTPResponse:
         return self.request("OPTIONS", url,
                             headers=headers,
-                            query_params=query_params,
-                            post_params=post_params,
-                            _preload_content=_preload_content,
-                            _request_timeout=_request_timeout,
-                            body=body)
+                            stream=stream,
+                            timeout=timeout,
+                            body=body, fields=fields)
 
-    def DELETE(self, url, headers=None, query_params=None, body=None,
-               _preload_content=True, _request_timeout=None):
+    def DELETE(self, url, headers=None, body=None,
+               stream=False, timeout=None, fields=None) -> urllib3.HTTPResponse:
         return self.request("DELETE", url,
                             headers=headers,
-                            query_params=query_params,
-                            _preload_content=_preload_content,
-                            _request_timeout=_request_timeout,
-                            body=body)
+                            stream=stream,
+                            timeout=timeout,
+                            body=body, fields=fields)
 
-    def POST(self, url, headers=None, query_params=None, post_params=None,
-             body=None, _preload_content=True, _request_timeout=None):
+    def POST(self, url, headers=None,
+             body=None, stream=False, timeout=None, fields=None) -> urllib3.HTTPResponse:
         return self.request("POST", url,
                             headers=headers,
-                            query_params=query_params,
-                            post_params=post_params,
-                            _preload_content=_preload_content,
-                            _request_timeout=_request_timeout,
-                            body=body)
+                            stream=stream,
+                            timeout=timeout,
+                            body=body, fields=fields)
 
-    def PUT(self, url, headers=None, query_params=None, post_params=None,
-            body=None, _preload_content=True, _request_timeout=None):
+    def PUT(self, url, headers=None,
+            body=None, stream=False, timeout=None, fields=None) -> urllib3.HTTPResponse:
         return self.request("PUT", url,
                             headers=headers,
-                            query_params=query_params,
-                            post_params=post_params,
-                            _preload_content=_preload_content,
-                            _request_timeout=_request_timeout,
-                            body=body)
+                            stream=stream,
+                            timeout=timeout,
+                            body=body, fields=fields)
 
-    def PATCH(self, url, headers=None, query_params=None, post_params=None,
-              body=None, _preload_content=True, _request_timeout=None):
+    def PATCH(self, url, headers=None,
+              body=None, stream=False, timeout=None, fields=None) -> urllib3.HTTPResponse:
         return self.request("PATCH", url,
                             headers=headers,
-                            query_params=query_params,
-                            post_params=post_params,
-                            _preload_content=_preload_content,
-                            _request_timeout=_request_timeout,
-                            body=body)
+                            stream=stream,
+                            timeout=timeout,
+                            body=body, fields=fields)
```

### Comparing `vdk-control-service-api-1.0.6/test/test_data_job_api_info.py` & `vdk-control-service-api-1.0.7/taurus_datajob_api/apis/tags/data_jobs_deployment_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,31 @@
 # coding: utf-8
 
 """
     Versatile Data Kit Control Service API
 
-    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction  The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br  The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time).                      The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning.                            Implementation of the API is not considered stable nor well tested.                            Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade.                          The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.   # noqa: E501
+    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
-import unittest
-import datetime
-
-import taurus_datajob_api
-from taurus_datajob_api.models.data_job_api_info import DataJobApiInfo  # noqa: E501
-from taurus_datajob_api.rest import ApiException
-
-class TestDataJobApiInfo(unittest.TestCase):
-    """DataJobApiInfo unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def make_instance(self, include_optional):
-        """Test DataJobApiInfo
-            include_option is a boolean, when False only required
-            params are included, when True both required and
-            optional params are included """
-        # model = taurus_datajob_api.models.data_job_api_info.DataJobApiInfo()  # noqa: E501
-        if include_optional :
-            return DataJobApiInfo(
-                api_version = '0'
-            )
-        else :
-            return DataJobApiInfo(
-                api_version = '0',
-        )
-
-    def testDataJobApiInfo(self):
-        """Test DataJobApiInfo"""
-        inst_req_only = self.make_instance(include_optional=False)
-        inst_req_and_optional = self.make_instance(include_optional=True)
-
-
-if __name__ == '__main__':
-    unittest.main()
+from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id.delete import DeploymentDelete
+from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs_job_name_deployments.get import DeploymentList
+from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id.patch import DeploymentPatch
+from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id.get import DeploymentRead
+from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs_job_name_deployments.post import DeploymentUpdate
+
+
+class DataJobsDeploymentApi(
+    DeploymentDelete,
+    DeploymentList,
+    DeploymentPatch,
+    DeploymentRead,
+    DeploymentUpdate,
+):
+    """NOTE: This class is auto generated by OpenAPI Generator
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+    """
+    pass
```

### Comparing `vdk-control-service-api-1.0.6/test/test_data_job_config.py` & `vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_properties.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,59 @@
 # coding: utf-8
 
 """
     Versatile Data Kit Control Service API
 
-    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction  The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br  The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time).                      The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning.                            Implementation of the API is not considered stable nor well tested.                            Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade.                          The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.   # noqa: E501
+    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
-import unittest
-import datetime
-
-import taurus_datajob_api
-from taurus_datajob_api.models.data_job_config import DataJobConfig  # noqa: E501
-from taurus_datajob_api.rest import ApiException
-
-class TestDataJobConfig(unittest.TestCase):
-    """DataJobConfig unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def make_instance(self, include_optional):
-        """Test DataJobConfig
-            include_option is a boolean, when False only required
-            params are included, when True both required and
-            optional params are included """
-        # model = taurus_datajob_api.models.data_job_config.DataJobConfig()  # noqa: E501
-        if include_optional :
-            return DataJobConfig(
-                db_default_type = 'TRINO', 
-                contacts = taurus_datajob_api.models.data_job_contacts.DataJobContacts(
-                    notified_on_job_failure_user_error = ["auserov@example.mail.com"], 
-                    notified_on_job_failure_platform_error = ["auserov@example.mail.com"], 
-                    notified_on_job_success = ["auserov@example.mail.com"], 
-                    notified_on_job_deploy = ["auserov@example.mail.com"], ), 
-                schedule = taurus_datajob_api.models.data_job_schedule.DataJobSchedule(
-                    schedule_cron = '0 0 13 * 5', ), 
-                generate_keytab = False, 
-                enable_execution_notifications = False, 
-                notification_delay_period_minutes = 60
-            )
-        else :
-            return DataJobConfig(
+from datetime import date, datetime  # noqa: F401
+import decimal  # noqa: F401
+import functools  # noqa: F401
+import io  # noqa: F401
+import re  # noqa: F401
+import typing  # noqa: F401
+import typing_extensions  # noqa: F401
+import uuid  # noqa: F401
+
+import frozendict  # noqa: F401
+
+from taurus_datajob_api import schemas  # noqa: F401
+
+
+class DataJobProperties(
+    schemas.DictSchema
+):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+
+    Properties of a Data Job
+    """
+
+
+    class MetaOapg:
+        additional_properties = schemas.DictSchema
+    
+    def __getitem__(self, name: typing.Union[str, ]) -> MetaOapg.additional_properties:
+        # dict_instance[name] accessor
+        return super().__getitem__(name)
+    
+    def get_item_oapg(self, name: typing.Union[str, ]) -> MetaOapg.additional_properties:
+        return super().get_item_oapg(name)
+
+    def __new__(
+        cls,
+        *_args: typing.Union[dict, frozendict.frozendict, ],
+        _configuration: typing.Optional[schemas.Configuration] = None,
+        **kwargs: typing.Union[MetaOapg.additional_properties, dict, frozendict.frozendict, ],
+    ) -> 'DataJobProperties':
+        return super().__new__(
+            cls,
+            *_args,
+            _configuration=_configuration,
+            **kwargs,
         )
-
-    def testDataJobConfig(self):
-        """Test DataJobConfig"""
-        inst_req_only = self.make_instance(include_optional=False)
-        inst_req_and_optional = self.make_instance(include_optional=True)
-
-
-if __name__ == '__main__':
-    unittest.main()
```

### Comparing `vdk-control-service-api-1.0.6/test/test_data_job_contacts.py` & `vdk-control-service-api-1.0.7/test/test_models/test_data_job_execution_request.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,55 +1,25 @@
 # coding: utf-8
 
 """
     Versatile Data Kit Control Service API
 
-    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction  The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br  The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time).                      The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning.                            Implementation of the API is not considered stable nor well tested.                            Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade.                          The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.   # noqa: E501
+    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
 import unittest
-import datetime
 
 import taurus_datajob_api
-from taurus_datajob_api.models.data_job_contacts import DataJobContacts  # noqa: E501
-from taurus_datajob_api.rest import ApiException
-
-class TestDataJobContacts(unittest.TestCase):
-    """DataJobContacts unit test stubs"""
+from taurus_datajob_api.model.data_job_execution_request import DataJobExecutionRequest
+from taurus_datajob_api import configuration
 
-    def setUp(self):
-        pass
 
-    def tearDown(self):
-        pass
-
-    def make_instance(self, include_optional):
-        """Test DataJobContacts
-            include_option is a boolean, when False only required
-            params are included, when True both required and
-            optional params are included """
-        # model = taurus_datajob_api.models.data_job_contacts.DataJobContacts()  # noqa: E501
-        if include_optional :
-            return DataJobContacts(
-                notified_on_job_failure_user_error = ["auserov@example.mail.com"], 
-                notified_on_job_failure_platform_error = ["auserov@example.mail.com"], 
-                notified_on_job_success = ["auserov@example.mail.com"], 
-                notified_on_job_deploy = ["auserov@example.mail.com"]
-            )
-        else :
-            return DataJobContacts(
-        )
-
-    def testDataJobContacts(self):
-        """Test DataJobContacts"""
-        inst_req_only = self.make_instance(include_optional=False)
-        inst_req_and_optional = self.make_instance(include_optional=True)
+class TestDataJobExecutionRequest(unittest.TestCase):
+    """DataJobExecutionRequest unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `vdk-control-service-api-1.0.6/test/test_data_job_deployment.py` & `vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_schedule.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,65 +1,80 @@
 # coding: utf-8
 
 """
     Versatile Data Kit Control Service API
 
-    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction  The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br  The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time).                      The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning.                            Implementation of the API is not considered stable nor well tested.                            Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade.                          The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.   # noqa: E501
+    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
-import unittest
-import datetime
-
-import taurus_datajob_api
-from taurus_datajob_api.models.data_job_deployment import DataJobDeployment  # noqa: E501
-from taurus_datajob_api.rest import ApiException
-
-class TestDataJobDeployment(unittest.TestCase):
-    """DataJobDeployment unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def make_instance(self, include_optional):
-        """Test DataJobDeployment
-            include_option is a boolean, when False only required
-            params are included, when True both required and
-            optional params are included """
-        # model = taurus_datajob_api.models.data_job_deployment.DataJobDeployment()  # noqa: E501
-        if include_optional :
-            return DataJobDeployment(
-                vdk_version = '2.1', 
-                job_version = '11a403ba', 
-                mode = 'release', 
-                id = 'release', 
-                enabled = False, 
-                deployed_by = 'auserov@example.mail.com', 
-                deployed_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                schedule = taurus_datajob_api.models.data_job_schedule.DataJobSchedule(
-                    schedule_cron = '0 0 13 * 5', ), 
-                resources = taurus_datajob_api.models.data_job_resources.DataJobResources(
-                    cpu_request = 10, 
-                    cpu_limit = 20, 
-                    memory_request = 1024, 
-                    memory_limit = 2048, )
-            )
-        else :
-            return DataJobDeployment(
+from datetime import date, datetime  # noqa: F401
+import decimal  # noqa: F401
+import functools  # noqa: F401
+import io  # noqa: F401
+import re  # noqa: F401
+import typing  # noqa: F401
+import typing_extensions  # noqa: F401
+import uuid  # noqa: F401
+
+import frozendict  # noqa: F401
+
+from taurus_datajob_api import schemas  # noqa: F401
+
+
+class DataJobSchedule(
+    schemas.DictSchema
+):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+
+    Schedule configuration
+    """
+
+
+    class MetaOapg:
+        
+        class properties:
+            schedule_cron = schemas.StrSchema
+            __annotations__ = {
+                "schedule_cron": schedule_cron,
+            }
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["schedule_cron"]) -> MetaOapg.properties.schedule_cron: ...
+    
+    @typing.overload
+    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
+    
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["schedule_cron", ], str]):
+        # dict_instance[name] accessor
+        return super().__getitem__(name)
+    
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["schedule_cron"]) -> typing.Union[MetaOapg.properties.schedule_cron, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
+    
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["schedule_cron", ], str]):
+        return super().get_item_oapg(name)
+    
+
+    def __new__(
+        cls,
+        *_args: typing.Union[dict, frozendict.frozendict, ],
+        schedule_cron: typing.Union[MetaOapg.properties.schedule_cron, str, schemas.Unset] = schemas.unset,
+        _configuration: typing.Optional[schemas.Configuration] = None,
+        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+    ) -> 'DataJobSchedule':
+        return super().__new__(
+            cls,
+            *_args,
+            schedule_cron=schedule_cron,
+            _configuration=_configuration,
+            **kwargs,
         )
-
-    def testDataJobDeployment(self):
-        """Test DataJobDeployment"""
-        inst_req_only = self.make_instance(include_optional=False)
-        inst_req_and_optional = self.make_instance(include_optional=True)
-
-
-if __name__ == '__main__':
-    unittest.main()
```

### Comparing `vdk-control-service-api-1.0.6/test/test_data_job_execution_logs.py` & `vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_mode.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,51 @@
 # coding: utf-8
 
 """
     Versatile Data Kit Control Service API
 
-    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction  The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br  The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time).                      The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning.                            Implementation of the API is not considered stable nor well tested.                            Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade.                          The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.   # noqa: E501
+    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
-import unittest
-import datetime
-
-import taurus_datajob_api
-from taurus_datajob_api.models.data_job_execution_logs import DataJobExecutionLogs  # noqa: E501
-from taurus_datajob_api.rest import ApiException
-
-class TestDataJobExecutionLogs(unittest.TestCase):
-    """DataJobExecutionLogs unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def make_instance(self, include_optional):
-        """Test DataJobExecutionLogs
-            include_option is a boolean, when False only required
-            params are included, when True both required and
-            optional params are included """
-        # model = taurus_datajob_api.models.data_job_execution_logs.DataJobExecutionLogs()  # noqa: E501
-        if include_optional :
-            return DataJobExecutionLogs(
-                logs = '0'
-            )
-        else :
-            return DataJobExecutionLogs(
-        )
-
-    def testDataJobExecutionLogs(self):
-        """Test DataJobExecutionLogs"""
-        inst_req_only = self.make_instance(include_optional=False)
-        inst_req_and_optional = self.make_instance(include_optional=True)
-
-
-if __name__ == '__main__':
-    unittest.main()
+from datetime import date, datetime  # noqa: F401
+import decimal  # noqa: F401
+import functools  # noqa: F401
+import io  # noqa: F401
+import re  # noqa: F401
+import typing  # noqa: F401
+import typing_extensions  # noqa: F401
+import uuid  # noqa: F401
+
+import frozendict  # noqa: F401
+
+from taurus_datajob_api import schemas  # noqa: F401
+
+
+class DataJobMode(
+    schemas.EnumBase,
+    schemas.StrSchema
+):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+
+    The execution mode that the data job is deployed in. Data Jobs used for development or testing purposes are marked as testing. This is used by Operations team on platform rollout and infrastructure changes adoption. For example, rollout and validation of testing jobs first, then proceeding with release data jobs. Also, testing and release jobs may have different limits and SLA targets.
+    """
+
+
+    class MetaOapg:
+        enum_value_to_name = {
+            "testing": "TESTING",
+            "release": "RELEASE",
+        }
+    
+    @schemas.classproperty
+    def TESTING(cls):
+        return cls("testing")
+    
+    @schemas.classproperty
+    def RELEASE(cls):
+        return cls("release")
```

### Comparing `vdk-control-service-api-1.0.6/test/test_data_job_mode.py` & `vdk-control-service-api-1.0.7/test/test_models/test_data_job_deployment.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,51 +1,25 @@
 # coding: utf-8
 
 """
     Versatile Data Kit Control Service API
 
-    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction  The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br  The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time).                      The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning.                            Implementation of the API is not considered stable nor well tested.                            Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade.                          The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.   # noqa: E501
+    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
 import unittest
-import datetime
 
 import taurus_datajob_api
-from taurus_datajob_api.models.data_job_mode import DataJobMode  # noqa: E501
-from taurus_datajob_api.rest import ApiException
-
-class TestDataJobMode(unittest.TestCase):
-    """DataJobMode unit test stubs"""
+from taurus_datajob_api.model.data_job_deployment import DataJobDeployment
+from taurus_datajob_api import configuration
 
-    def setUp(self):
-        pass
 
-    def tearDown(self):
-        pass
-
-    def make_instance(self, include_optional):
-        """Test DataJobMode
-            include_option is a boolean, when False only required
-            params are included, when True both required and
-            optional params are included """
-        # model = taurus_datajob_api.models.data_job_mode.DataJobMode()  # noqa: E501
-        if include_optional :
-            return DataJobMode(
-            )
-        else :
-            return DataJobMode(
-        )
-
-    def testDataJobMode(self):
-        """Test DataJobMode"""
-        inst_req_only = self.make_instance(include_optional=False)
-        inst_req_and_optional = self.make_instance(include_optional=True)
+class TestDataJobDeployment(unittest.TestCase):
+    """DataJobDeployment unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `vdk-control-service-api-1.0.6/test/test_data_job_page.py` & `vdk-control-service-api-1.0.7/taurus_datajob_api/apis/tags/data_jobs_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,35 @@
 # coding: utf-8
 
 """
     Versatile Data Kit Control Service API
 
-    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction  The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br  The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time).                      The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning.                            Implementation of the API is not considered stable nor well tested.                            Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade.                          The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.   # noqa: E501
+    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
-import unittest
-import datetime
-
-import taurus_datajob_api
-from taurus_datajob_api.models.data_job_page import DataJobPage  # noqa: E501
-from taurus_datajob_api.rest import ApiException
-
-class TestDataJobPage(unittest.TestCase):
-    """DataJobPage unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def make_instance(self, include_optional):
-        """Test DataJobPage
-            include_option is a boolean, when False only required
-            params are included, when True both required and
-            optional params are included """
-        # model = taurus_datajob_api.models.data_job_page.DataJobPage()  # noqa: E501
-        if include_optional :
-            return DataJobPage(
-                content = {"application/json":[{"jobName":"starshot-processing-vmc-fact-daily","config":{"team":"starshot","description":"Data Job responsible for transforming vmc related fact tables on daily basis","schedule":{"scheduleCron":"5 0 * 8 *","nextRun":1618914371},"sourceUrl":"https://github.com/product-analytics/data-jobs/tree/master/starshot-processing-vmc-fact-daily","contacts":{"notifiedOnJobFailureUserError":"[auser@example.mail.com]","notifiedOnJobFailurePlatformError":"[auser2@example.mail.com, auser@example.mail.com]","notifiedOnJobSuccess":"[auser@example.mail.com]","notifiedOnJobDeploy":"[auser2@example.mail.com, auser@example.mail.com]"}}},"..."]}, 
-                total_items = 100, 
-                total_pages = 5
-            )
-        else :
-            return DataJobPage(
-        )
-
-    def testDataJobPage(self):
-        """Test DataJobPage"""
-        inst_req_only = self.make_instance(include_optional=False)
-        inst_req_and_optional = self.make_instance(include_optional=True)
-
-
-if __name__ == '__main__':
-    unittest.main()
+from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs.post import DataJobCreate
+from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs_job_name.delete import DataJobDelete
+from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs_job_name_keytab.get import DataJobKeytabDownload
+from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs_job_name.get import DataJobRead
+from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs_job_name_team_new_team.put import DataJobTeamUpdate
+from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs_job_name.put import DataJobUpdate
+from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs.get import JobsQuery
+
+
+class DataJobsApi(
+    DataJobCreate,
+    DataJobDelete,
+    DataJobKeytabDownload,
+    DataJobRead,
+    DataJobTeamUpdate,
+    DataJobUpdate,
+    JobsQuery,
+):
+    """NOTE: This class is auto generated by OpenAPI Generator
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+    """
+    pass
```

### Comparing `vdk-control-service-api-1.0.6/test/test_data_job_query_response.py` & `vdk-control-service-api-1.0.7/test/test_models/test_data_job_config.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,58 +1,25 @@
 # coding: utf-8
 
 """
     Versatile Data Kit Control Service API
 
-    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction  The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br  The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time).                      The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning.                            Implementation of the API is not considered stable nor well tested.                            Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade.                          The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.   # noqa: E501
+    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
 import unittest
-import datetime
 
 import taurus_datajob_api
-from taurus_datajob_api.models.data_job_query_response import DataJobQueryResponse  # noqa: E501
-from taurus_datajob_api.rest import ApiException
-
-class TestDataJobQueryResponse(unittest.TestCase):
-    """DataJobQueryResponse unit test stubs"""
+from taurus_datajob_api.model.data_job_config import DataJobConfig
+from taurus_datajob_api import configuration
 
-    def setUp(self):
-        pass
 
-    def tearDown(self):
-        pass
-
-    def make_instance(self, include_optional):
-        """Test DataJobQueryResponse
-            include_option is a boolean, when False only required
-            params are included, when True both required and
-            optional params are included """
-        # model = taurus_datajob_api.models.data_job_query_response.DataJobQueryResponse()  # noqa: E501
-        if include_optional :
-            return DataJobQueryResponse(
-                errors = [
-                    None
-                    ], 
-                data = taurus_datajob_api.models.data_job_page.DataJobPage(
-                    content = {"application/json":[{"jobName":"starshot-processing-vmc-fact-daily","config":{"team":"starshot","description":"Data Job responsible for transforming vmc related fact tables on daily basis","schedule":{"scheduleCron":"5 0 * 8 *","nextRun":1618914371},"sourceUrl":"https://github.com/product-analytics/data-jobs/tree/master/starshot-processing-vmc-fact-daily","contacts":{"notifiedOnJobFailureUserError":"[auser@example.mail.com]","notifiedOnJobFailurePlatformError":"[auser2@example.mail.com, auser@example.mail.com]","notifiedOnJobSuccess":"[auser@example.mail.com]","notifiedOnJobDeploy":"[auser2@example.mail.com, auser@example.mail.com]"}}},"..."]}, 
-                    total_items = 100, 
-                    total_pages = 5, )
-            )
-        else :
-            return DataJobQueryResponse(
-        )
-
-    def testDataJobQueryResponse(self):
-        """Test DataJobQueryResponse"""
-        inst_req_only = self.make_instance(include_optional=False)
-        inst_req_and_optional = self.make_instance(include_optional=True)
+class TestDataJobConfig(unittest.TestCase):
+    """DataJobConfig unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `vdk-control-service-api-1.0.6/test/test_data_job_query_response_with_error.py` & `vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_version.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,85 @@
 # coding: utf-8
 
 """
     Versatile Data Kit Control Service API
 
-    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction  The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br  The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time).                      The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning.                            Implementation of the API is not considered stable nor well tested.                            Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade.                          The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.   # noqa: E501
+    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
-import unittest
-import datetime
-
-import taurus_datajob_api
-from taurus_datajob_api.models.data_job_query_response_with_error import DataJobQueryResponseWithError  # noqa: E501
-from taurus_datajob_api.rest import ApiException
-
-class TestDataJobQueryResponseWithError(unittest.TestCase):
-    """DataJobQueryResponseWithError unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def make_instance(self, include_optional):
-        """Test DataJobQueryResponseWithError
-            include_option is a boolean, when False only required
-            params are included, when True both required and
-            optional params are included """
-        # model = taurus_datajob_api.models.data_job_query_response_with_error.DataJobQueryResponseWithError()  # noqa: E501
-        if include_optional :
-            return DataJobQueryResponseWithError(
-                errors = {"application/json":[{"message":"Validation error of type FieldUndefined","locations":[],"description":"Field 'someField' in type 'DataJob' is undefined","validationErrorType":"FieldUndefined","queryPath":["jobs","content","someField"],"extensions":null,"errorType":"ValidationError","path":null}]}, 
-                data = taurus_datajob_api.models.data_job_page.DataJobPage(
-                    content = {"application/json":[{"jobName":"starshot-processing-vmc-fact-daily","config":{"team":"starshot","description":"Data Job responsible for transforming vmc related fact tables on daily basis","schedule":{"scheduleCron":"5 0 * 8 *","nextRun":1618914371},"sourceUrl":"https://github.com/product-analytics/data-jobs/tree/master/starshot-processing-vmc-fact-daily","contacts":{"notifiedOnJobFailureUserError":"[auser@example.mail.com]","notifiedOnJobFailurePlatformError":"[auser2@example.mail.com, auser@example.mail.com]","notifiedOnJobSuccess":"[auser@example.mail.com]","notifiedOnJobDeploy":"[auser2@example.mail.com, auser@example.mail.com]"}}},"..."]}, 
-                    total_items = 100, 
-                    total_pages = 5, )
-            )
-        else :
-            return DataJobQueryResponseWithError(
+from datetime import date, datetime  # noqa: F401
+import decimal  # noqa: F401
+import functools  # noqa: F401
+import io  # noqa: F401
+import re  # noqa: F401
+import typing  # noqa: F401
+import typing_extensions  # noqa: F401
+import uuid  # noqa: F401
+
+import frozendict  # noqa: F401
+
+from taurus_datajob_api import schemas  # noqa: F401
+
+
+class DataJobVersion(
+    schemas.DictSchema
+):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+
+    Data Job version
+    """
+
+
+    class MetaOapg:
+        required = {
+            "version_sha",
+        }
+        
+        class properties:
+            version_sha = schemas.StrSchema
+            __annotations__ = {
+                "version_sha": version_sha,
+            }
+    
+    version_sha: MetaOapg.properties.version_sha
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["version_sha"]) -> MetaOapg.properties.version_sha: ...
+    
+    @typing.overload
+    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
+    
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["version_sha", ], str]):
+        # dict_instance[name] accessor
+        return super().__getitem__(name)
+    
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["version_sha"]) -> MetaOapg.properties.version_sha: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
+    
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["version_sha", ], str]):
+        return super().get_item_oapg(name)
+    
+
+    def __new__(
+        cls,
+        *_args: typing.Union[dict, frozendict.frozendict, ],
+        version_sha: typing.Union[MetaOapg.properties.version_sha, str, ],
+        _configuration: typing.Optional[schemas.Configuration] = None,
+        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+    ) -> 'DataJobVersion':
+        return super().__new__(
+            cls,
+            *_args,
+            version_sha=version_sha,
+            _configuration=_configuration,
+            **kwargs,
         )
-
-    def testDataJobQueryResponseWithError(self):
-        """Test DataJobQueryResponseWithError"""
-        inst_req_only = self.make_instance(include_optional=False)
-        inst_req_and_optional = self.make_instance(include_optional=True)
-
-
-if __name__ == '__main__':
-    unittest.main()
```

### Comparing `vdk-control-service-api-1.0.6/test/test_data_job_resources.py` & `vdk-control-service-api-1.0.7/test/test_models/test_data_job_execution.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,55 +1,25 @@
 # coding: utf-8
 
 """
     Versatile Data Kit Control Service API
 
-    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction  The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br  The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time).                      The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning.                            Implementation of the API is not considered stable nor well tested.                            Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade.                          The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.   # noqa: E501
+    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
 import unittest
-import datetime
 
 import taurus_datajob_api
-from taurus_datajob_api.models.data_job_resources import DataJobResources  # noqa: E501
-from taurus_datajob_api.rest import ApiException
-
-class TestDataJobResources(unittest.TestCase):
-    """DataJobResources unit test stubs"""
+from taurus_datajob_api.model.data_job_execution import DataJobExecution
+from taurus_datajob_api import configuration
 
-    def setUp(self):
-        pass
 
-    def tearDown(self):
-        pass
-
-    def make_instance(self, include_optional):
-        """Test DataJobResources
-            include_option is a boolean, when False only required
-            params are included, when True both required and
-            optional params are included """
-        # model = taurus_datajob_api.models.data_job_resources.DataJobResources()  # noqa: E501
-        if include_optional :
-            return DataJobResources(
-                cpu_request = 10, 
-                cpu_limit = 20, 
-                memory_request = 1024, 
-                memory_limit = 2048
-            )
-        else :
-            return DataJobResources(
-        )
-
-    def testDataJobResources(self):
-        """Test DataJobResources"""
-        inst_req_only = self.make_instance(include_optional=False)
-        inst_req_and_optional = self.make_instance(include_optional=True)
+class TestDataJobExecution(unittest.TestCase):
+    """DataJobExecution unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `vdk-control-service-api-1.0.6/test/test_data_job_schedule.py` & `vdk-control-service-api-1.0.7/test/test_models/test_data_job_schedule.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,52 +1,25 @@
 # coding: utf-8
 
 """
     Versatile Data Kit Control Service API
 
-    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction  The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br  The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time).                      The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning.                            Implementation of the API is not considered stable nor well tested.                            Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade.                          The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.   # noqa: E501
+    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
 import unittest
-import datetime
 
 import taurus_datajob_api
-from taurus_datajob_api.models.data_job_schedule import DataJobSchedule  # noqa: E501
-from taurus_datajob_api.rest import ApiException
+from taurus_datajob_api.model.data_job_schedule import DataJobSchedule
+from taurus_datajob_api import configuration
+
 
 class TestDataJobSchedule(unittest.TestCase):
     """DataJobSchedule unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
-    def make_instance(self, include_optional):
-        """Test DataJobSchedule
-            include_option is a boolean, when False only required
-            params are included, when True both required and
-            optional params are included """
-        # model = taurus_datajob_api.models.data_job_schedule.DataJobSchedule()  # noqa: E501
-        if include_optional :
-            return DataJobSchedule(
-                schedule_cron = '0 0 13 * 5'
-            )
-        else :
-            return DataJobSchedule(
-        )
-
-    def testDataJobSchedule(self):
-        """Test DataJobSchedule"""
-        inst_req_only = self.make_instance(include_optional=False)
-        inst_req_and_optional = self.make_instance(include_optional=True)
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `vdk-control-service-api-1.0.6/test/test_data_job_version.py` & `vdk-control-service-api-1.0.7/test/test_models/test_data_job_properties.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,25 @@
 # coding: utf-8
 
 """
     Versatile Data Kit Control Service API
 
-    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction  The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br  The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time).                      The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning.                            Implementation of the API is not considered stable nor well tested.                            Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade.                          The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.   # noqa: E501
+    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
 import unittest
-import datetime
 
 import taurus_datajob_api
-from taurus_datajob_api.models.data_job_version import DataJobVersion  # noqa: E501
-from taurus_datajob_api.rest import ApiException
-
-class TestDataJobVersion(unittest.TestCase):
-    """DataJobVersion unit test stubs"""
+from taurus_datajob_api.model.data_job_properties import DataJobProperties
+from taurus_datajob_api import configuration
 
-    def setUp(self):
-        pass
 
-    def tearDown(self):
-        pass
-
-    def make_instance(self, include_optional):
-        """Test DataJobVersion
-            include_option is a boolean, when False only required
-            params are included, when True both required and
-            optional params are included """
-        # model = taurus_datajob_api.models.data_job_version.DataJobVersion()  # noqa: E501
-        if include_optional :
-            return DataJobVersion(
-                version_sha = '0'
-            )
-        else :
-            return DataJobVersion(
-                version_sha = '0',
-        )
-
-    def testDataJobVersion(self):
-        """Test DataJobVersion"""
-        inst_req_only = self.make_instance(include_optional=False)
-        inst_req_and_optional = self.make_instance(include_optional=True)
+class TestDataJobProperties(unittest.TestCase):
+    """DataJobProperties unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `vdk-control-service-api-1.0.6/test/test_data_jobs_properties_api.py` & `vdk-control-service-api-1.0.7/test/test_models/test_data_job_query_response_with_error.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,47 +1,25 @@
 # coding: utf-8
 
 """
     Versatile Data Kit Control Service API
 
-    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction  The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br  The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time).                      The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning.                            Implementation of the API is not considered stable nor well tested.                            Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade.                          The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.   # noqa: E501
+    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
 import unittest
 
 import taurus_datajob_api
-from taurus_datajob_api.api.data_jobs_properties_api import DataJobsPropertiesApi  # noqa: E501
-from taurus_datajob_api.rest import ApiException
-
-
-class TestDataJobsPropertiesApi(unittest.TestCase):
-    """DataJobsPropertiesApi unit test stubs"""
-
-    def setUp(self):
-        self.api = taurus_datajob_api.api.data_jobs_properties_api.DataJobsPropertiesApi()  # noqa: E501
-
-    def tearDown(self):
-        pass
-
-    def test_data_job_properties_read(self):
-        """Test case for data_job_properties_read
-
-        Get Data Job properties.  # noqa: E501
-        """
-        pass
+from taurus_datajob_api.model.data_job_query_response_with_error import DataJobQueryResponseWithError
+from taurus_datajob_api import configuration
 
-    def test_data_job_properties_update(self):
-        """Test case for data_job_properties_update
 
-        Update Data Job properties.  # noqa: E501
-        """
-        pass
+class TestDataJobQueryResponseWithError(unittest.TestCase):
+    """DataJobQueryResponseWithError unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `vdk-control-service-api-1.0.6/test/test_data_jobs_service_api.py` & `vdk-control-service-api-1.0.7/test/test_models/test_data_job_api_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,25 @@
 # coding: utf-8
 
 """
     Versatile Data Kit Control Service API
 
-    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction  The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br  The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time).                      The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning.                            Implementation of the API is not considered stable nor well tested.                            Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade.                          The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.   # noqa: E501
+    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
 import unittest
 
 import taurus_datajob_api
-from taurus_datajob_api.api.data_jobs_service_api import DataJobsServiceApi  # noqa: E501
-from taurus_datajob_api.rest import ApiException
-
-
-class TestDataJobsServiceApi(unittest.TestCase):
-    """DataJobsServiceApi unit test stubs"""
-
-    def setUp(self):
-        self.api = taurus_datajob_api.api.data_jobs_service_api.DataJobsServiceApi()  # noqa: E501
-
-    def tearDown(self):
-        pass
+from taurus_datajob_api.model.data_job_api_info import DataJobApiInfo
+from taurus_datajob_api import configuration
 
-    def test_info(self):
-        """Test case for info
 
-        Get API and Data Jobs Service info  # noqa: E501
-        """
-        pass
+class TestDataJobApiInfo(unittest.TestCase):
+    """DataJobApiInfo unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `vdk-control-service-api-1.0.6/test/test_data_jobs_sources_api.py` & `vdk-control-service-api-1.0.7/taurus_datajob_api/apis/tags/data_jobs_sources_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,27 @@
 # coding: utf-8
 
 """
     Versatile Data Kit Control Service API
 
-    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction  The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br  The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time).                      The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning.                            Implementation of the API is not considered stable nor well tested.                            Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade.                          The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.   # noqa: E501
+    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
-import unittest
-
-import taurus_datajob_api
-from taurus_datajob_api.api.data_jobs_sources_api import DataJobsSourcesApi  # noqa: E501
-from taurus_datajob_api.rest import ApiException
-
-
-class TestDataJobsSourcesApi(unittest.TestCase):
-    """DataJobsSourcesApi unit test stubs"""
-
-    def setUp(self):
-        self.api = taurus_datajob_api.api.data_jobs_sources_api.DataJobsSourcesApi()  # noqa: E501
-
-    def tearDown(self):
-        pass
-
-    def test_data_job_sources_download(self):
-        """Test case for data_job_sources_download
-
-        Download data job source code. | (Not Implemented)  # noqa: E501
-        """
-        pass
-
-    def test_sources_delete(self):
-        """Test case for sources_delete
-
-        Delete Data Job source.  # noqa: E501
-        """
-        pass
-
-    def test_sources_upload(self):
-        """Test case for sources_upload
-
-        Upload Data Job source code. | (Stable)  # noqa: E501
-        """
-        pass
-
-
-if __name__ == '__main__':
-    unittest.main()
+from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs_job_name_sources.get import DataJobSourcesDownload
+from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs_job_name_sources.delete import SourcesDelete
+from taurus_datajob_api.paths.data_jobs_for_team_team_name_jobs_job_name_sources.post import SourcesUpload
+
+
+class DataJobsSourcesApi(
+    DataJobSourcesDownload,
+    SourcesDelete,
+    SourcesUpload,
+):
+    """NOTE: This class is auto generated by OpenAPI Generator
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+    """
+    pass
```

### Comparing `vdk-control-service-api-1.0.6/test/test_error.py` & `vdk-control-service-api-1.0.7/test/test_models/test_data_job_contacts.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,25 @@
 # coding: utf-8
 
 """
     Versatile Data Kit Control Service API
 
-    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction  The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br  The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time).                      The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning.                            Implementation of the API is not considered stable nor well tested.                            Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade.                          The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.   # noqa: E501
+    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import absolute_import
-
 import unittest
-import datetime
 
 import taurus_datajob_api
-from taurus_datajob_api.models.error import Error  # noqa: E501
-from taurus_datajob_api.rest import ApiException
-
-class TestError(unittest.TestCase):
-    """Error unit test stubs"""
+from taurus_datajob_api.model.data_job_contacts import DataJobContacts
+from taurus_datajob_api import configuration
 
-    def setUp(self):
-        pass
 
-    def tearDown(self):
-        pass
-
-    def make_instance(self, include_optional):
-        """Test Error
-            include_option is a boolean, when False only required
-            params are included, when True both required and
-            optional params are included """
-        # model = taurus_datajob_api.models.error.Error()  # noqa: E501
-        if include_optional :
-            return Error(
-                messages = ["Data Job starshot-processing-vmc-fact-daily not found"]
-            )
-        else :
-            return Error(
-                messages = ["Data Job starshot-processing-vmc-fact-daily not found"],
-        )
-
-    def testError(self):
-        """Test Error"""
-        inst_req_only = self.make_instance(include_optional=False)
-        inst_req_and_optional = self.make_instance(include_optional=True)
+class TestDataJobContacts(unittest.TestCase):
+    """DataJobContacts unit test stubs"""
+    _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `vdk-control-service-api-1.0.6/vdk_control_service_api.egg-info/PKG-INFO` & `vdk-control-service-api-1.0.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: vdk-control-service-api
-Version: 1.0.6
+Version: 1.0.7
 Summary: Versatile Data Kit Control Service API
-Home-page: UNKNOWN
+Home-page: 
 Author: OpenAPI Generator community
 Author-email: team@openapitools.org
 License: Apache 2.0
-Description:     The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction  The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.&lt;br&gt; &lt;br&gt; ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) &lt;br&gt; The API reflects the usual Data Job Development lifecycle:&lt;br&gt; &lt;li&gt; Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). &lt;li&gt; Download keytab. Develop and run the data job locally. &lt;li&gt; Deploy the data job in cloud runtime environment to run on a scheduled basis. &lt;br&gt;&lt;br&gt; If Authentication is enabled, pass OAuth2 access token in HTTP header &#39;Authorization: Bearer [access-token-here]&#39; (https://datatracker.ietf.org/doc/html/rfc6750). &lt;br  The API promotes some best practices (inspired by https://12factor.net): &lt;li&gt; Explicitly declare and isolate dependencies. &lt;li&gt; Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. &lt;li&gt; Separation between the build, release/deploy, and run stages. &lt;li&gt; Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). &lt;li&gt; Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. &lt;li&gt; Keep development, staging, and production as similar as possible. &lt;br&gt;&lt;br&gt; &lt;b&gt;API Evolution&lt;/b&gt;&lt;br&gt; In the following sections, there are some terms that have a special meaning in the context of the APIs. &lt;br&gt;&lt;br&gt; &lt;li&gt; &lt;i&gt;Stable&lt;/i&gt; - The implementation of the API has been battle-tested (has been in production for some time).                      The API is a subject to semantic versioning model and will follow deprecation policy. &lt;li&gt; &lt;i&gt;Experimental&lt;/i&gt; - May disappear without notice and is not a subject to semantic versioning.                            Implementation of the API is not considered stable nor well tested.                            Generally this is given to clients to experiment within testing environment. Must not be used in production. &lt;li&gt; &lt;i&gt;Deprecated&lt;/i&gt; - API is expected to be removed within next one or two major version upgrade.                          The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.   # noqa: E501
-            
 Keywords: OpenAPI,OpenAPI-Generator,Versatile Data Kit Control Service API
-Platform: UNKNOWN
+Requires-Python: >=3.7
+
+    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.&lt;br&gt; &lt;br&gt; ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) &lt;br&gt; The API reflects the usual Data Job Development lifecycle:&lt;br&gt; &lt;li&gt; Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). &lt;li&gt; Download keytab. Develop and run the data job locally. &lt;li&gt; Deploy the data job in cloud runtime environment to run on a scheduled basis. &lt;br&gt;&lt;br&gt; If Authentication is enabled, pass OAuth2 access token in HTTP header &#x27;Authorization: Bearer [access-token-here]&#x27; (https://datatracker.ietf.org/doc/html/rfc6750). &lt;br The API promotes some best practices (inspired by https://12factor.net): &lt;li&gt; Explicitly declare and isolate dependencies. &lt;li&gt; Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. &lt;li&gt; Separation between the build, release/deploy, and run stages. &lt;li&gt; Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). &lt;li&gt; Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. &lt;li&gt; Keep development, staging, and production as similar as possible. &lt;br&gt;&lt;br&gt; &lt;b&gt;API Evolution&lt;/b&gt;&lt;br&gt; In the following sections, there are some terms that have a special meaning in the context of the APIs. &lt;br&gt;&lt;br&gt; &lt;li&gt; &lt;i&gt;Stable&lt;/i&gt; - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. &lt;li&gt; &lt;i&gt;Experimental&lt;/i&gt; - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. &lt;li&gt; &lt;i&gt;Deprecated&lt;/i&gt; - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
+
```

### Comparing `vdk-control-service-api-1.0.6/setup.py` & `vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_page.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,122 @@
 # coding: utf-8
 
 """
     Versatile Data Kit Control Service API
 
-    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction  The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br  The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time).                      The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning.                            Implementation of the API is not considered stable nor well tested.                            Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade.                          The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.   # noqa: E501
+    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
+from datetime import date, datetime  # noqa: F401
+import decimal  # noqa: F401
+import functools  # noqa: F401
+import io  # noqa: F401
+import re  # noqa: F401
+import typing  # noqa: F401
+import typing_extensions  # noqa: F401
+import uuid  # noqa: F401
 
-from setuptools import setup, find_packages  # noqa: H301
+import frozendict  # noqa: F401
 
-NAME = "vdk-control-service-api"
-VERSION = "1.0.6"
-# To install the library, run the following
-#
-# python setup.py install
-#
-# prerequisite: setuptools
-# http://pypi.python.org/pypi/setuptools
-
-REQUIRES = ["urllib3 >= 1.15", "six >= 1.10", "certifi", "python-dateutil"]
-
-setup(
-    name=NAME,
-    version=VERSION,
-    description="Versatile Data Kit Control Service API",
-    author="OpenAPI Generator community",
-    author_email="team@openapitools.org",
-    url="",
-    keywords=["OpenAPI", "OpenAPI-Generator", "Versatile Data Kit Control Service API"],
-    install_requires=REQUIRES,
-    packages=find_packages(exclude=["test", "tests"]),
-    include_package_data=True,
-    license="Apache 2.0",
-    long_description="""\
-    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction  The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.&lt;br&gt; &lt;br&gt; ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) &lt;br&gt; The API reflects the usual Data Job Development lifecycle:&lt;br&gt; &lt;li&gt; Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). &lt;li&gt; Download keytab. Develop and run the data job locally. &lt;li&gt; Deploy the data job in cloud runtime environment to run on a scheduled basis. &lt;br&gt;&lt;br&gt; If Authentication is enabled, pass OAuth2 access token in HTTP header &#39;Authorization: Bearer [access-token-here]&#39; (https://datatracker.ietf.org/doc/html/rfc6750). &lt;br  The API promotes some best practices (inspired by https://12factor.net): &lt;li&gt; Explicitly declare and isolate dependencies. &lt;li&gt; Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. &lt;li&gt; Separation between the build, release/deploy, and run stages. &lt;li&gt; Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). &lt;li&gt; Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. &lt;li&gt; Keep development, staging, and production as similar as possible. &lt;br&gt;&lt;br&gt; &lt;b&gt;API Evolution&lt;/b&gt;&lt;br&gt; In the following sections, there are some terms that have a special meaning in the context of the APIs. &lt;br&gt;&lt;br&gt; &lt;li&gt; &lt;i&gt;Stable&lt;/i&gt; - The implementation of the API has been battle-tested (has been in production for some time).                      The API is a subject to semantic versioning model and will follow deprecation policy. &lt;li&gt; &lt;i&gt;Experimental&lt;/i&gt; - May disappear without notice and is not a subject to semantic versioning.                            Implementation of the API is not considered stable nor well tested.                            Generally this is given to clients to experiment within testing environment. Must not be used in production. &lt;li&gt; &lt;i&gt;Deprecated&lt;/i&gt; - API is expected to be removed within next one or two major version upgrade.                          The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.   # noqa: E501
+from taurus_datajob_api import schemas  # noqa: F401
+
+
+class DataJobPage(
+    schemas.DictSchema
+):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
+
+    Page object containing Data Jobs list with information for total elements and pages
     """
-)
+
+
+    class MetaOapg:
+        
+        class properties:
+            
+            
+            class content(
+                schemas.ListSchema
+            ):
+            
+            
+                class MetaOapg:
+                    items = schemas.DictSchema
+            
+                def __new__(
+                    cls,
+                    _arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, dict, frozendict.frozendict, ]], typing.List[typing.Union[MetaOapg.items, dict, frozendict.frozendict, ]]],
+                    _configuration: typing.Optional[schemas.Configuration] = None,
+                ) -> 'content':
+                    return super().__new__(
+                        cls,
+                        _arg,
+                        _configuration=_configuration,
+                    )
+            
+                def __getitem__(self, i: int) -> MetaOapg.items:
+                    return super().__getitem__(i)
+            totalItems = schemas.IntSchema
+            totalPages = schemas.IntSchema
+            __annotations__ = {
+                "content": content,
+                "totalItems": totalItems,
+                "totalPages": totalPages,
+            }
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["content"]) -> MetaOapg.properties.content: ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["totalItems"]) -> MetaOapg.properties.totalItems: ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["totalPages"]) -> MetaOapg.properties.totalPages: ...
+    
+    @typing.overload
+    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
+    
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["content", "totalItems", "totalPages", ], str]):
+        # dict_instance[name] accessor
+        return super().__getitem__(name)
+    
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["content"]) -> typing.Union[MetaOapg.properties.content, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["totalItems"]) -> typing.Union[MetaOapg.properties.totalItems, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["totalPages"]) -> typing.Union[MetaOapg.properties.totalPages, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
+    
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["content", "totalItems", "totalPages", ], str]):
+        return super().get_item_oapg(name)
+    
+
+    def __new__(
+        cls,
+        *_args: typing.Union[dict, frozendict.frozendict, ],
+        content: typing.Union[MetaOapg.properties.content, list, tuple, schemas.Unset] = schemas.unset,
+        totalItems: typing.Union[MetaOapg.properties.totalItems, decimal.Decimal, int, schemas.Unset] = schemas.unset,
+        totalPages: typing.Union[MetaOapg.properties.totalPages, decimal.Decimal, int, schemas.Unset] = schemas.unset,
+        _configuration: typing.Optional[schemas.Configuration] = None,
+        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+    ) -> 'DataJobPage':
+        return super().__new__(
+            cls,
+            *_args,
+            content=content,
+            totalItems=totalItems,
+            totalPages=totalPages,
+            _configuration=_configuration,
+            **kwargs,
+        )
```

### Comparing `vdk-control-service-api-1.0.6/PKG-INFO` & `vdk-control-service-api-1.0.7/vdk_control_service_api.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: vdk-control-service-api
-Version: 1.0.6
+Version: 1.0.7
 Summary: Versatile Data Kit Control Service API
-Home-page: UNKNOWN
+Home-page: 
 Author: OpenAPI Generator community
 Author-email: team@openapitools.org
 License: Apache 2.0
-Description:     The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction  The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.&lt;br&gt; &lt;br&gt; ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) &lt;br&gt; The API reflects the usual Data Job Development lifecycle:&lt;br&gt; &lt;li&gt; Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). &lt;li&gt; Download keytab. Develop and run the data job locally. &lt;li&gt; Deploy the data job in cloud runtime environment to run on a scheduled basis. &lt;br&gt;&lt;br&gt; If Authentication is enabled, pass OAuth2 access token in HTTP header &#39;Authorization: Bearer [access-token-here]&#39; (https://datatracker.ietf.org/doc/html/rfc6750). &lt;br  The API promotes some best practices (inspired by https://12factor.net): &lt;li&gt; Explicitly declare and isolate dependencies. &lt;li&gt; Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. &lt;li&gt; Separation between the build, release/deploy, and run stages. &lt;li&gt; Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). &lt;li&gt; Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. &lt;li&gt; Keep development, staging, and production as similar as possible. &lt;br&gt;&lt;br&gt; &lt;b&gt;API Evolution&lt;/b&gt;&lt;br&gt; In the following sections, there are some terms that have a special meaning in the context of the APIs. &lt;br&gt;&lt;br&gt; &lt;li&gt; &lt;i&gt;Stable&lt;/i&gt; - The implementation of the API has been battle-tested (has been in production for some time).                      The API is a subject to semantic versioning model and will follow deprecation policy. &lt;li&gt; &lt;i&gt;Experimental&lt;/i&gt; - May disappear without notice and is not a subject to semantic versioning.                            Implementation of the API is not considered stable nor well tested.                            Generally this is given to clients to experiment within testing environment. Must not be used in production. &lt;li&gt; &lt;i&gt;Deprecated&lt;/i&gt; - API is expected to be removed within next one or two major version upgrade.                          The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.   # noqa: E501
-            
 Keywords: OpenAPI,OpenAPI-Generator,Versatile Data Kit Control Service API
-Platform: UNKNOWN
+Requires-Python: >=3.7
+
+    The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.&lt;br&gt; &lt;br&gt; ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) &lt;br&gt; The API reflects the usual Data Job Development lifecycle:&lt;br&gt; &lt;li&gt; Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). &lt;li&gt; Download keytab. Develop and run the data job locally. &lt;li&gt; Deploy the data job in cloud runtime environment to run on a scheduled basis. &lt;br&gt;&lt;br&gt; If Authentication is enabled, pass OAuth2 access token in HTTP header &#x27;Authorization: Bearer [access-token-here]&#x27; (https://datatracker.ietf.org/doc/html/rfc6750). &lt;br The API promotes some best practices (inspired by https://12factor.net): &lt;li&gt; Explicitly declare and isolate dependencies. &lt;li&gt; Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. &lt;li&gt; Separation between the build, release/deploy, and run stages. &lt;li&gt; Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). &lt;li&gt; Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. &lt;li&gt; Keep development, staging, and production as similar as possible. &lt;br&gt;&lt;br&gt; &lt;b&gt;API Evolution&lt;/b&gt;&lt;br&gt; In the following sections, there are some terms that have a special meaning in the context of the APIs. &lt;br&gt;&lt;br&gt; &lt;li&gt; &lt;i&gt;Stable&lt;/i&gt; - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. &lt;li&gt; &lt;i&gt;Experimental&lt;/i&gt; - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. &lt;li&gt; &lt;i&gt;Deprecated&lt;/i&gt; - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
+
```

