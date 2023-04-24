# Comparing `tmp/vdk-control-service-api-1.0.7.tar.gz` & `tmp/vdk-control-service-api-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-control-service-api-1.0.7.tar", last modified: Mon Apr 24 11:09:21 2023, max compression
+gzip compressed data, was "vdk-control-service-api-1.0.8.tar", last modified: Mon Apr 24 13:23:29 2023, max compression
```

## Comparing `vdk-control-service-api-1.0.7.tar` & `vdk-control-service-api-1.0.8.tar`

### file list

```diff
@@ -1,196 +1,196 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.323403 vdk-control-service-api-1.0.7/
--rw-r--r--   0 root         (0) root         (0)     3190 2023-04-24 11:09:21.323403 vdk-control-service-api-1.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    20126 2023-04-24 11:09:20.000000 vdk-control-service-api-1.0.7/README.md
--rw-r--r--   0 root         (0) root         (0)       69 2023-04-24 11:09:21.323403 vdk-control-service-api-1.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     6635 2023-04-24 11:09:20.000000 vdk-control-service-api-1.0.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.299403 vdk-control-service-api-1.0.7/taurus_datajob_api/
--rw-r--r--   0 root         (0) root         (0)     3386 2023-04-24 11:09:20.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    61119 2023-04-24 11:09:20.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.299403 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/
--rw-r--r--   0 root         (0) root         (0)      214 2023-04-24 11:09:20.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5328 2023-04-24 11:09:17.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/path_to_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.303403 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/paths/
--rw-r--r--   0 root         (0) root         (0)      245 2023-04-24 11:09:17.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/paths/__init__.py
--rw-r--r--   0 root         (0) root         (0)      149 2023-04-24 11:09:16.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_info.py
--rw-r--r--   0 root         (0) root         (0)      252 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs.py
--rw-r--r--   0 root         (0) root         (0)      392 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name.py
--rw-r--r--   0 root         (0) root         (0)      312 2023-04-24 11:09:14.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name_deployments.py
--rw-r--r--   0 root         (0) root         (0)      499 2023-04-24 11:09:14.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id.py
--rw-r--r--   0 root         (0) root         (0)      384 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions.py
--rw-r--r--   0 root         (0) root         (0)      381 2023-04-24 11:09:16.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties.py
--rw-r--r--   0 root         (0) root         (0)      186 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name_executions.py
--rw-r--r--   0 root         (0) root         (0)      352 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name_executions_execution_id.py
--rw-r--r--   0 root         (0) root         (0)      219 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name_executions_execution_id_logs.py
--rw-r--r--   0 root         (0) root         (0)      178 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name_keytab.py
--rw-r--r--   0 root         (0) root         (0)      426 2023-04-24 11:09:17.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name_sources.py
--rw-r--r--   0 root         (0) root         (0)      190 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name_team_new_team.py
--rw-r--r--   0 root         (0) root         (0)     1365 2023-04-24 11:09:17.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/tag_to_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.303403 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/tags/
--rw-r--r--   0 root         (0) root         (0)      555 2023-04-24 11:09:17.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/tags/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3852 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/tags/data_jobs_api.py
--rw-r--r--   0 root         (0) root         (0)     3737 2023-04-24 11:09:14.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/tags/data_jobs_deployment_api.py
--rw-r--r--   0 root         (0) root         (0)     3999 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/tags/data_jobs_execution_api.py
--rw-r--r--   0 root         (0) root         (0)     3368 2023-04-24 11:09:16.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/tags/data_jobs_properties_api.py
--rw-r--r--   0 root         (0) root         (0)     3111 2023-04-24 11:09:16.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/tags/data_jobs_service_api.py
--rw-r--r--   0 root         (0) root         (0)     3418 2023-04-24 11:09:17.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/apis/tags/data_jobs_sources_api.py
--rw-r--r--   0 root         (0) root         (0)    18077 2023-04-24 11:09:20.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/configuration.py
--rw-r--r--   0 root         (0) root         (0)     7117 2023-04-24 11:09:20.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.307403 vdk-control-service-api-1.0.7/taurus_datajob_api/model/
--rw-r--r--   0 root         (0) root         (0)      352 2023-04-24 11:09:20.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6765 2023-04-24 11:09:05.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job.py
--rw-r--r--   0 root         (0) root         (0)     6849 2023-04-24 11:09:05.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_api_info.py
--rw-r--r--   0 root         (0) root         (0)     8809 2023-04-24 11:09:06.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_config.py
--rw-r--r--   0 root         (0) root         (0)    11079 2023-04-24 11:09:07.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_contacts.py
--rw-r--r--   0 root         (0) root         (0)    10382 2023-04-24 11:09:07.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_deployment.py
--rw-r--r--   0 root         (0) root         (0)     3211 2023-04-24 11:09:07.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_deployment_id.py
--rw-r--r--   0 root         (0) root         (0)    11264 2023-04-24 11:09:07.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_deployment_status.py
--rw-r--r--   0 root         (0) root         (0)    12532 2023-04-24 11:09:08.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_execution.py
--rw-r--r--   0 root         (0) root         (0)     5033 2023-04-24 11:09:08.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_execution_logs.py
--rw-r--r--   0 root         (0) root         (0)     7013 2023-04-24 11:09:08.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_execution_request.py
--rw-r--r--   0 root         (0) root         (0)     4081 2023-04-24 11:09:08.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_mode.py
--rw-r--r--   0 root         (0) root         (0)     7116 2023-04-24 11:09:08.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_page.py
--rw-r--r--   0 root         (0) root         (0)     4219 2023-04-24 11:09:08.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_properties.py
--rw-r--r--   0 root         (0) root         (0)     6516 2023-04-24 11:09:08.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_query_response.py
--rw-r--r--   0 root         (0) root         (0)     6534 2023-04-24 11:09:08.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_query_response_with_error.py
--rw-r--r--   0 root         (0) root         (0)     6974 2023-04-24 11:09:09.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_resources.py
--rw-r--r--   0 root         (0) root         (0)     5138 2023-04-24 11:09:09.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_schedule.py
--rw-r--r--   0 root         (0) root         (0)     6731 2023-04-24 11:09:09.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_summary.py
--rw-r--r--   0 root         (0) root         (0)     5158 2023-04-24 11:09:09.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_version.py
--rw-r--r--   0 root         (0) root         (0)     5936 2023-04-24 11:09:09.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/model/error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.307403 vdk-control-service-api-1.0.7/taurus_datajob_api/models/
--rw-r--r--   0 root         (0) root         (0)     1856 2023-04-24 11:09:20.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.307403 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/
--rw-r--r--   0 root         (0) root         (0)     1937 2023-04-24 11:09:17.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.307403 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_info/
--rw-r--r--   0 root         (0) root         (0)      359 2023-04-24 11:09:16.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_info/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9663 2023-04-24 11:09:16.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_info/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.307403 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs/
--rw-r--r--   0 root         (0) root         (0)      359 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13125 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs/get.py
--rw-r--r--   0 root         (0) root         (0)    16868 2023-04-24 11:09:10.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.307403 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name/
--rw-r--r--   0 root         (0) root         (0)      377 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10312 2023-04-24 11:09:11.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name/delete.py
--rw-r--r--   0 root         (0) root         (0)    10613 2023-04-24 11:09:11.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name/get.py
--rw-r--r--   0 root         (0) root         (0)    15339 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.307403 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments/
--rw-r--r--   0 root         (0) root         (0)      401 2023-04-24 11:09:14.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13798 2023-04-24 11:09:13.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments/get.py
--rw-r--r--   0 root         (0) root         (0)    17659 2023-04-24 11:09:13.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.307403 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/
--rw-r--r--   0 root         (0) root         (0)      429 2023-04-24 11:09:14.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10729 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    10952 2023-04-24 11:09:13.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/get.py
--rw-r--r--   0 root         (0) root         (0)    15525 2023-04-24 11:09:13.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/patch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.311403 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions/
--rw-r--r--   0 root         (0) root         (0)      451 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14554 2023-04-24 11:09:14.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions/get.py
--rw-r--r--   0 root         (0) root         (0)    16006 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.311403 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties/
--rw-r--r--   0 root         (0) root         (0)      451 2023-04-24 11:09:16.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10452 2023-04-24 11:09:16.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties/get.py
--rw-r--r--   0 root         (0) root         (0)    13298 2023-04-24 11:09:16.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.311403 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions/
--rw-r--r--   0 root         (0) root         (0)      399 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14185 2023-04-24 11:09:14.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.311403 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions_execution_id/
--rw-r--r--   0 root         (0) root         (0)      425 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions_execution_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10765 2023-04-24 11:09:14.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions_execution_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11021 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions_execution_id/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.311403 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions_execution_id_logs/
--rw-r--r--   0 root         (0) root         (0)      435 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions_execution_id_logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13907 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions_execution_id_logs/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.311403 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_keytab/
--rw-r--r--   0 root         (0) root         (0)      391 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_keytab/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11209 2023-04-24 11:09:11.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_keytab/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.311403 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_sources/
--rw-r--r--   0 root         (0) root         (0)      393 2023-04-24 11:09:17.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_sources/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12453 2023-04-24 11:09:17.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_sources/delete.py
--rw-r--r--   0 root         (0) root         (0)    11239 2023-04-24 11:09:16.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_sources/get.py
--rw-r--r--   0 root         (0) root         (0)    17624 2023-04-24 11:09:17.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_sources/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.311403 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_team_new_team/
--rw-r--r--   0 root         (0) root         (0)      405 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_team_new_team/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11166 2023-04-24 11:09:11.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_team_new_team/put.py
--rw-r--r--   0 root         (0) root         (0)    13149 2023-04-24 11:09:20.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/rest.py
--rw-r--r--   0 root         (0) root         (0)   100261 2023-04-24 11:09:20.000000 vdk-control-service-api-1.0.7/taurus_datajob_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.295403 vdk-control-service-api-1.0.7/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.315403 vdk-control-service-api-1.0.7/test/test_models/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 11:09:20.000000 vdk-control-service-api-1.0.7/test/test_models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3149 2023-04-24 11:09:05.000000 vdk-control-service-api-1.0.7/test/test_models/test_data_job.py
--rw-r--r--   0 root         (0) root         (0)     3179 2023-04-24 11:09:06.000000 vdk-control-service-api-1.0.7/test/test_models/test_data_job_api_info.py
--rw-r--r--   0 root         (0) root         (0)     3174 2023-04-24 11:09:06.000000 vdk-control-service-api-1.0.7/test/test_models/test_data_job_config.py
--rw-r--r--   0 root         (0) root         (0)     3182 2023-04-24 11:09:07.000000 vdk-control-service-api-1.0.7/test/test_models/test_data_job_contacts.py
--rw-r--r--   0 root         (0) root         (0)     3190 2023-04-24 11:09:07.000000 vdk-control-service-api-1.0.7/test/test_models/test_data_job_deployment.py
--rw-r--r--   0 root         (0) root         (0)     3199 2023-04-24 11:09:07.000000 vdk-control-service-api-1.0.7/test/test_models/test_data_job_deployment_id.py
--rw-r--r--   0 root         (0) root         (0)     3215 2023-04-24 11:09:07.000000 vdk-control-service-api-1.0.7/test/test_models/test_data_job_deployment_status.py
--rw-r--r--   0 root         (0) root         (0)     3186 2023-04-24 11:09:08.000000 vdk-control-service-api-1.0.7/test/test_models/test_data_job_execution.py
--rw-r--r--   0 root         (0) root         (0)     3203 2023-04-24 11:09:08.000000 vdk-control-service-api-1.0.7/test/test_models/test_data_job_execution_logs.py
--rw-r--r--   0 root         (0) root         (0)     3215 2023-04-24 11:09:08.000000 vdk-control-service-api-1.0.7/test/test_models/test_data_job_execution_request.py
--rw-r--r--   0 root         (0) root         (0)     3166 2023-04-24 11:09:08.000000 vdk-control-service-api-1.0.7/test/test_models/test_data_job_mode.py
--rw-r--r--   0 root         (0) root         (0)     3166 2023-04-24 11:09:08.000000 vdk-control-service-api-1.0.7/test/test_models/test_data_job_page.py
--rw-r--r--   0 root         (0) root         (0)     3190 2023-04-24 11:09:08.000000 vdk-control-service-api-1.0.7/test/test_models/test_data_job_properties.py
--rw-r--r--   0 root         (0) root         (0)     3203 2023-04-24 11:09:08.000000 vdk-control-service-api-1.0.7/test/test_models/test_data_job_query_response.py
--rw-r--r--   0 root         (0) root         (0)     3241 2023-04-24 11:09:09.000000 vdk-control-service-api-1.0.7/test/test_models/test_data_job_query_response_with_error.py
--rw-r--r--   0 root         (0) root         (0)     3186 2023-04-24 11:09:09.000000 vdk-control-service-api-1.0.7/test/test_models/test_data_job_resources.py
--rw-r--r--   0 root         (0) root         (0)     3182 2023-04-24 11:09:09.000000 vdk-control-service-api-1.0.7/test/test_models/test_data_job_schedule.py
--rw-r--r--   0 root         (0) root         (0)     3178 2023-04-24 11:09:09.000000 vdk-control-service-api-1.0.7/test/test_models/test_data_job_summary.py
--rw-r--r--   0 root         (0) root         (0)     3178 2023-04-24 11:09:09.000000 vdk-control-service-api-1.0.7/test/test_models/test_data_job_version.py
--rw-r--r--   0 root         (0) root         (0)     3140 2023-04-24 11:09:09.000000 vdk-control-service-api-1.0.7/test/test_models/test_error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.315403 vdk-control-service-api-1.0.7/test/test_paths/
--rw-r--r--   0 root         (0) root         (0)     1995 2023-04-24 11:09:17.000000 vdk-control-service-api-1.0.7/test/test_paths/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.315403 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_info/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 11:09:16.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_info/__init__.py
--rw-r--r--   0 root         (0) root         (0)      928 2023-04-24 11:09:16.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_info/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.315403 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs/__init__.py
--rw-r--r--   0 root         (0) root         (0)      891 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs/test_get.py
--rw-r--r--   0 root         (0) root         (0)      918 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.319403 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name/__init__.py
--rw-r--r--   0 root         (0) root         (0)      938 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      974 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name/test_get.py
--rw-r--r--   0 root         (0) root         (0)      932 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.319403 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 11:09:14.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments/__init__.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-04-24 11:09:14.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments/test_get.py
--rw-r--r--   0 root         (0) root         (0)      997 2023-04-24 11:09:14.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.319403 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 11:09:14.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1082 2023-04-24 11:09:14.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      990 2023-04-24 11:09:14.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)     1334 2023-04-24 11:09:14.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/test_patch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.319403 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1036 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions/test_get.py
--rw-r--r--   0 root         (0) root         (0)     1053 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.319403 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 11:09:16.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1009 2023-04-24 11:09:16.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties/test_get.py
--rw-r--r--   0 root         (0) root         (0)     1035 2023-04-24 11:09:16.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.319403 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1037 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.319403 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions_execution_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions_execution_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions_execution_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      996 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions_execution_id/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.319403 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions_execution_id_logs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions_execution_id_logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1180 2023-04-24 11:09:15.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions_execution_id_logs/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.319403 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_keytab/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_keytab/__init__.py
--rw-r--r--   0 root         (0) root         (0)      932 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_keytab/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.319403 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_sources/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 11:09:17.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_sources/__init__.py
--rw-r--r--   0 root         (0) root         (0)      957 2023-04-24 11:09:17.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_sources/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      954 2023-04-24 11:09:17.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_sources/test_get.py
--rw-r--r--   0 root         (0) root         (0)      948 2023-04-24 11:09:17.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_sources/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.323403 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_team_new_team/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_team_new_team/__init__.py
--rw-r--r--   0 root         (0) root         (0)      979 2023-04-24 11:09:12.000000 vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_team_new_team/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:09:21.323403 vdk-control-service-api-1.0.7/vdk_control_service_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3190 2023-04-24 11:09:21.000000 vdk-control-service-api-1.0.7/vdk_control_service_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10920 2023-04-24 11:09:21.000000 vdk-control-service-api-1.0.7/vdk_control_service_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 11:09:21.000000 vdk-control-service-api-1.0.7/vdk_control_service_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      118 2023-04-24 11:09:21.000000 vdk-control-service-api-1.0.7/vdk_control_service_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-04-24 11:09:21.000000 vdk-control-service-api-1.0.7/vdk_control_service_api.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.597642 vdk-control-service-api-1.0.8/
+-rw-r--r--   0 root         (0) root         (0)     3190 2023-04-24 13:23:29.597642 vdk-control-service-api-1.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    20126 2023-04-24 13:23:28.000000 vdk-control-service-api-1.0.8/README.md
+-rw-r--r--   0 root         (0) root         (0)       69 2023-04-24 13:23:29.597642 vdk-control-service-api-1.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     6635 2023-04-24 13:23:28.000000 vdk-control-service-api-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.573642 vdk-control-service-api-1.0.8/taurus_datajob_api/
+-rw-r--r--   0 root         (0) root         (0)     3386 2023-04-24 13:23:28.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    61119 2023-04-24 13:23:28.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.573642 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/
+-rw-r--r--   0 root         (0) root         (0)      214 2023-04-24 13:23:28.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5328 2023-04-24 13:23:25.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/path_to_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.577642 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/paths/
+-rw-r--r--   0 root         (0) root         (0)      245 2023-04-24 13:23:25.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/paths/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      149 2023-04-24 13:23:25.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_info.py
+-rw-r--r--   0 root         (0) root         (0)      252 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs.py
+-rw-r--r--   0 root         (0) root         (0)      392 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name.py
+-rw-r--r--   0 root         (0) root         (0)      312 2023-04-24 13:23:21.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name_deployments.py
+-rw-r--r--   0 root         (0) root         (0)      499 2023-04-24 13:23:21.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id.py
+-rw-r--r--   0 root         (0) root         (0)      384 2023-04-24 13:23:23.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions.py
+-rw-r--r--   0 root         (0) root         (0)      381 2023-04-24 13:23:24.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties.py
+-rw-r--r--   0 root         (0) root         (0)      186 2023-04-24 13:23:23.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name_executions.py
+-rw-r--r--   0 root         (0) root         (0)      352 2023-04-24 13:23:23.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name_executions_execution_id.py
+-rw-r--r--   0 root         (0) root         (0)      219 2023-04-24 13:23:23.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name_executions_execution_id_logs.py
+-rw-r--r--   0 root         (0) root         (0)      178 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name_keytab.py
+-rw-r--r--   0 root         (0) root         (0)      426 2023-04-24 13:23:25.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name_sources.py
+-rw-r--r--   0 root         (0) root         (0)      190 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/paths/data_jobs_for_team_team_name_jobs_job_name_team_new_team.py
+-rw-r--r--   0 root         (0) root         (0)     1365 2023-04-24 13:23:25.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/tag_to_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.577642 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/tags/
+-rw-r--r--   0 root         (0) root         (0)      555 2023-04-24 13:23:25.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/tags/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3852 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/tags/data_jobs_api.py
+-rw-r--r--   0 root         (0) root         (0)     3737 2023-04-24 13:23:21.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/tags/data_jobs_deployment_api.py
+-rw-r--r--   0 root         (0) root         (0)     3999 2023-04-24 13:23:23.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/tags/data_jobs_execution_api.py
+-rw-r--r--   0 root         (0) root         (0)     3368 2023-04-24 13:23:24.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/tags/data_jobs_properties_api.py
+-rw-r--r--   0 root         (0) root         (0)     3111 2023-04-24 13:23:25.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/tags/data_jobs_service_api.py
+-rw-r--r--   0 root         (0) root         (0)     3418 2023-04-24 13:23:25.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/apis/tags/data_jobs_sources_api.py
+-rw-r--r--   0 root         (0) root         (0)    18077 2023-04-24 13:23:28.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     7117 2023-04-24 13:23:28.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.581642 vdk-control-service-api-1.0.8/taurus_datajob_api/model/
+-rw-r--r--   0 root         (0) root         (0)      352 2023-04-24 13:23:28.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6765 2023-04-24 13:23:11.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job.py
+-rw-r--r--   0 root         (0) root         (0)     6849 2023-04-24 13:23:11.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_api_info.py
+-rw-r--r--   0 root         (0) root         (0)     8809 2023-04-24 13:23:12.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_config.py
+-rw-r--r--   0 root         (0) root         (0)    11079 2023-04-24 13:23:12.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_contacts.py
+-rw-r--r--   0 root         (0) root         (0)    10382 2023-04-24 13:23:13.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_deployment.py
+-rw-r--r--   0 root         (0) root         (0)     3211 2023-04-24 13:23:13.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_deployment_id.py
+-rw-r--r--   0 root         (0) root         (0)    11264 2023-04-24 13:23:13.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_deployment_status.py
+-rw-r--r--   0 root         (0) root         (0)    12532 2023-04-24 13:23:14.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_execution.py
+-rw-r--r--   0 root         (0) root         (0)     5033 2023-04-24 13:23:14.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_execution_logs.py
+-rw-r--r--   0 root         (0) root         (0)     7013 2023-04-24 13:23:14.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_execution_request.py
+-rw-r--r--   0 root         (0) root         (0)     4081 2023-04-24 13:23:14.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_mode.py
+-rw-r--r--   0 root         (0) root         (0)     7116 2023-04-24 13:23:14.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_page.py
+-rw-r--r--   0 root         (0) root         (0)     4219 2023-04-24 13:23:15.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_properties.py
+-rw-r--r--   0 root         (0) root         (0)     6516 2023-04-24 13:23:15.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_query_response.py
+-rw-r--r--   0 root         (0) root         (0)     6534 2023-04-24 13:23:15.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_query_response_with_error.py
+-rw-r--r--   0 root         (0) root         (0)     6974 2023-04-24 13:23:15.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_resources.py
+-rw-r--r--   0 root         (0) root         (0)     5138 2023-04-24 13:23:15.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     6731 2023-04-24 13:23:16.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_summary.py
+-rw-r--r--   0 root         (0) root         (0)     5158 2023-04-24 13:23:16.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_version.py
+-rw-r--r--   0 root         (0) root         (0)     5936 2023-04-24 13:23:16.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/model/error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.581642 vdk-control-service-api-1.0.8/taurus_datajob_api/models/
+-rw-r--r--   0 root         (0) root         (0)     1856 2023-04-24 13:23:28.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.581642 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/
+-rw-r--r--   0 root         (0) root         (0)     1937 2023-04-24 13:23:25.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.581642 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_info/
+-rw-r--r--   0 root         (0) root         (0)      359 2023-04-24 13:23:25.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_info/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9663 2023-04-24 13:23:24.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_info/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.581642 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs/
+-rw-r--r--   0 root         (0) root         (0)      359 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13125 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs/get.py
+-rw-r--r--   0 root         (0) root         (0)    16868 2023-04-24 13:23:17.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.581642 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name/
+-rw-r--r--   0 root         (0) root         (0)      377 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10312 2023-04-24 13:23:17.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name/delete.py
+-rw-r--r--   0 root         (0) root         (0)    10613 2023-04-24 13:23:18.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name/get.py
+-rw-r--r--   0 root         (0) root         (0)    15339 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.581642 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments/
+-rw-r--r--   0 root         (0) root         (0)      401 2023-04-24 13:23:21.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13798 2023-04-24 13:23:20.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments/get.py
+-rw-r--r--   0 root         (0) root         (0)    17659 2023-04-24 13:23:21.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.585642 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/
+-rw-r--r--   0 root         (0) root         (0)      429 2023-04-24 13:23:21.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10729 2023-04-24 13:23:20.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    10952 2023-04-24 13:23:21.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    15525 2023-04-24 13:23:20.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/patch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.585642 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions/
+-rw-r--r--   0 root         (0) root         (0)      451 2023-04-24 13:23:23.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14554 2023-04-24 13:23:22.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions/get.py
+-rw-r--r--   0 root         (0) root         (0)    16006 2023-04-24 13:23:23.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.585642 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties/
+-rw-r--r--   0 root         (0) root         (0)      451 2023-04-24 13:23:24.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10452 2023-04-24 13:23:24.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties/get.py
+-rw-r--r--   0 root         (0) root         (0)    13298 2023-04-24 13:23:24.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.585642 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions/
+-rw-r--r--   0 root         (0) root         (0)      399 2023-04-24 13:23:23.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14185 2023-04-24 13:23:22.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.585642 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions_execution_id/
+-rw-r--r--   0 root         (0) root         (0)      425 2023-04-24 13:23:23.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions_execution_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10765 2023-04-24 13:23:22.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions_execution_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11021 2023-04-24 13:23:22.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions_execution_id/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.585642 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions_execution_id_logs/
+-rw-r--r--   0 root         (0) root         (0)      435 2023-04-24 13:23:23.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions_execution_id_logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13907 2023-04-24 13:23:23.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions_execution_id_logs/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.585642 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_keytab/
+-rw-r--r--   0 root         (0) root         (0)      391 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_keytab/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11209 2023-04-24 13:23:18.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_keytab/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.585642 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_sources/
+-rw-r--r--   0 root         (0) root         (0)      393 2023-04-24 13:23:25.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_sources/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12453 2023-04-24 13:23:25.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_sources/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11239 2023-04-24 13:23:25.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_sources/get.py
+-rw-r--r--   0 root         (0) root         (0)    17624 2023-04-24 13:23:25.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_sources/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.589642 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_team_new_team/
+-rw-r--r--   0 root         (0) root         (0)      405 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_team_new_team/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11166 2023-04-24 13:23:18.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_team_new_team/put.py
+-rw-r--r--   0 root         (0) root         (0)    13149 2023-04-24 13:23:28.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/rest.py
+-rw-r--r--   0 root         (0) root         (0)   100261 2023-04-24 13:23:28.000000 vdk-control-service-api-1.0.8/taurus_datajob_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.569642 vdk-control-service-api-1.0.8/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.589642 vdk-control-service-api-1.0.8/test/test_models/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 13:23:28.000000 vdk-control-service-api-1.0.8/test/test_models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3149 2023-04-24 13:23:11.000000 vdk-control-service-api-1.0.8/test/test_models/test_data_job.py
+-rw-r--r--   0 root         (0) root         (0)     3179 2023-04-24 13:23:12.000000 vdk-control-service-api-1.0.8/test/test_models/test_data_job_api_info.py
+-rw-r--r--   0 root         (0) root         (0)     3174 2023-04-24 13:23:12.000000 vdk-control-service-api-1.0.8/test/test_models/test_data_job_config.py
+-rw-r--r--   0 root         (0) root         (0)     3182 2023-04-24 13:23:13.000000 vdk-control-service-api-1.0.8/test/test_models/test_data_job_contacts.py
+-rw-r--r--   0 root         (0) root         (0)     3190 2023-04-24 13:23:13.000000 vdk-control-service-api-1.0.8/test/test_models/test_data_job_deployment.py
+-rw-r--r--   0 root         (0) root         (0)     3199 2023-04-24 13:23:13.000000 vdk-control-service-api-1.0.8/test/test_models/test_data_job_deployment_id.py
+-rw-r--r--   0 root         (0) root         (0)     3215 2023-04-24 13:23:14.000000 vdk-control-service-api-1.0.8/test/test_models/test_data_job_deployment_status.py
+-rw-r--r--   0 root         (0) root         (0)     3186 2023-04-24 13:23:14.000000 vdk-control-service-api-1.0.8/test/test_models/test_data_job_execution.py
+-rw-r--r--   0 root         (0) root         (0)     3203 2023-04-24 13:23:14.000000 vdk-control-service-api-1.0.8/test/test_models/test_data_job_execution_logs.py
+-rw-r--r--   0 root         (0) root         (0)     3215 2023-04-24 13:23:14.000000 vdk-control-service-api-1.0.8/test/test_models/test_data_job_execution_request.py
+-rw-r--r--   0 root         (0) root         (0)     3166 2023-04-24 13:23:14.000000 vdk-control-service-api-1.0.8/test/test_models/test_data_job_mode.py
+-rw-r--r--   0 root         (0) root         (0)     3166 2023-04-24 13:23:15.000000 vdk-control-service-api-1.0.8/test/test_models/test_data_job_page.py
+-rw-r--r--   0 root         (0) root         (0)     3190 2023-04-24 13:23:15.000000 vdk-control-service-api-1.0.8/test/test_models/test_data_job_properties.py
+-rw-r--r--   0 root         (0) root         (0)     3203 2023-04-24 13:23:15.000000 vdk-control-service-api-1.0.8/test/test_models/test_data_job_query_response.py
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-04-24 13:23:15.000000 vdk-control-service-api-1.0.8/test/test_models/test_data_job_query_response_with_error.py
+-rw-r--r--   0 root         (0) root         (0)     3186 2023-04-24 13:23:15.000000 vdk-control-service-api-1.0.8/test/test_models/test_data_job_resources.py
+-rw-r--r--   0 root         (0) root         (0)     3182 2023-04-24 13:23:15.000000 vdk-control-service-api-1.0.8/test/test_models/test_data_job_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     3178 2023-04-24 13:23:16.000000 vdk-control-service-api-1.0.8/test/test_models/test_data_job_summary.py
+-rw-r--r--   0 root         (0) root         (0)     3178 2023-04-24 13:23:16.000000 vdk-control-service-api-1.0.8/test/test_models/test_data_job_version.py
+-rw-r--r--   0 root         (0) root         (0)     3140 2023-04-24 13:23:16.000000 vdk-control-service-api-1.0.8/test/test_models/test_error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.589642 vdk-control-service-api-1.0.8/test/test_paths/
+-rw-r--r--   0 root         (0) root         (0)     1995 2023-04-24 13:23:25.000000 vdk-control-service-api-1.0.8/test/test_paths/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.589642 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_info/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 13:23:25.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_info/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      928 2023-04-24 13:23:25.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_info/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.593642 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      891 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      918 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.593642 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      938 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      974 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      932 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.593642 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 13:23:21.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-04-24 13:23:21.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      997 2023-04-24 13:23:21.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.593642 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 13:23:21.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1082 2023-04-24 13:23:21.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      990 2023-04-24 13:23:21.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)     1334 2023-04-24 13:23:21.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/test_patch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.593642 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 13:23:23.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1036 2023-04-24 13:23:23.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions/test_get.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-04-24 13:23:23.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.593642 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 13:23:24.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1009 2023-04-24 13:23:24.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties/test_get.py
+-rw-r--r--   0 root         (0) root         (0)     1035 2023-04-24 13:23:24.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.593642 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 13:23:23.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1037 2023-04-24 13:23:23.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.593642 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions_execution_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 13:23:23.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions_execution_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-04-24 13:23:23.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions_execution_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      996 2023-04-24 13:23:23.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions_execution_id/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.593642 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions_execution_id_logs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 13:23:23.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions_execution_id_logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1180 2023-04-24 13:23:23.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions_execution_id_logs/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.597642 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_keytab/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_keytab/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      932 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_keytab/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.597642 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_sources/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 13:23:25.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_sources/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      957 2023-04-24 13:23:25.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_sources/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      954 2023-04-24 13:23:25.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_sources/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      948 2023-04-24 13:23:25.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_sources/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.597642 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_team_new_team/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_team_new_team/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      979 2023-04-24 13:23:19.000000 vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_team_new_team/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:23:29.597642 vdk-control-service-api-1.0.8/vdk_control_service_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3190 2023-04-24 13:23:29.000000 vdk-control-service-api-1.0.8/vdk_control_service_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10920 2023-04-24 13:23:29.000000 vdk-control-service-api-1.0.8/vdk_control_service_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 13:23:29.000000 vdk-control-service-api-1.0.8/vdk_control_service_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      118 2023-04-24 13:23:29.000000 vdk-control-service-api-1.0.8/vdk_control_service_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-04-24 13:23:29.000000 vdk-control-service-api-1.0.8/vdk_control_service_api.egg-info/top_level.txt
```

### Comparing `vdk-control-service-api-1.0.7/PKG-INFO` & `vdk-control-service-api-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-control-service-api
-Version: 1.0.7
+Version: 1.0.8
 Summary: Versatile Data Kit Control Service API
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: team@openapitools.org
 License: Apache 2.0
 Keywords: OpenAPI,OpenAPI-Generator,Versatile Data Kit Control Service API
 Requires-Python: >=3.7
```

### Comparing `vdk-control-service-api-1.0.7/README.md` & `vdk-control-service-api-1.0.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction
 The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br
 The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 1.0
-- Package version: 1.0.7
+- Package version: 1.0.8
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python &gt;&#x3D;3.7
 
 ## Migration from other generators like python and python-legacy
```

### Comparing `vdk-control-service-api-1.0.7/setup.py` & `vdk-control-service-api-1.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "vdk-control-service-api"
-VERSION = "1.0.7"
+VERSION = "1.0.8"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/__init__.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     The Data Jobs API of Versatile Data Kit Control Service. Data Jobs allows Data Engineers to implement automated pull ingestion (E in ELT) and batch data transformation into a database (T in ELT). See also https://github.com/vmware/versatile-data-kit/wiki/Introduction The API has resource-oriented URLs, JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs. The API enables creating, deploying, managing and executing Data Jobs in the runtime environment.<br> <br> ![](https://github.com/vmware/versatile-data-kit/wiki/vdk-data-job-lifecycle-state-diagram.png) <br> The API reflects the usual Data Job Development lifecycle:<br> <li> Create a new data job (webhook to further configure the job, e.g authorize its creation, setup permissions, etc). <li> Download keytab. Develop and run the data job locally. <li> Deploy the data job in cloud runtime environment to run on a scheduled basis. <br><br> If Authentication is enabled, pass OAuth2 access token in HTTP header 'Authorization: Bearer [access-token-here]' (https://datatracker.ietf.org/doc/html/rfc6750). <br The API promotes some best practices (inspired by https://12factor.net): <li> Explicitly declare and isolate dependencies. <li> Strict separation of configurations from code. Configurations vary substantially across deploys, code does not. <li> Separation between the build, release/deploy, and run stages. <li> Data Jobs are stateless and share-nothing processes. Any data that needs to be persisted must be stored in a stateful backing service (e.g IProperties). <li> Implementation is assumed to be atomic and idempotent - should be OK for a job to fail somewhere in the middle; subsequent restart should not cause data corruption. <li> Keep development, staging, and production as similar as possible. <br><br> <b>API Evolution</b><br> In the following sections, there are some terms that have a special meaning in the context of the APIs. <br><br> <li> <i>Stable</i> - The implementation of the API has been battle-tested (has been in production for some time). The API is a subject to semantic versioning model and will follow deprecation policy. <li> <i>Experimental</i> - May disappear without notice and is not a subject to semantic versioning. Implementation of the API is not considered stable nor well tested. Generally this is given to clients to experiment within testing environment. Must not be used in production. <li> <i>Deprecated</i> - API is expected to be removed within next one or two major version upgrade. The deprecation notice/comment will say when the API will be removed and what alternatives should be used instead.  # noqa: E501
 
     The version of the OpenAPI document: 1.0
     Generated by: https://openapi-generator.tech
 """
 
-__version__ = "1.0.7"
+__version__ = "1.0.8"
 
 # import ApiClient
 from taurus_datajob_api.api_client import ApiClient
 
 # import Configuration
 from taurus_datajob_api.configuration import Configuration
```

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/api_client.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -999,15 +999,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = HTTPHeaderDict()
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.0.7/python'
+        self.user_agent = 'OpenAPI-Generator/1.0.8/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/apis/path_to_api.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/apis/tag_to_api.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/apis/tag_to_api.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/apis/tags/__init__.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/apis/tags/__init__.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/apis/tags/data_jobs_api.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/apis/tags/data_jobs_api.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/apis/tags/data_jobs_deployment_api.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/apis/tags/data_jobs_deployment_api.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/apis/tags/data_jobs_execution_api.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/apis/tags/data_jobs_execution_api.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/apis/tags/data_jobs_properties_api.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/apis/tags/data_jobs_properties_api.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/apis/tags/data_jobs_service_api.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/apis/tags/data_jobs_service_api.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/apis/tags/data_jobs_sources_api.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/apis/tags/data_jobs_sources_api.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/configuration.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -361,15 +361,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0\n"\
-               "SDK Package Version: 1.0.7".\
+               "SDK Package Version: 1.0.8".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/exceptions.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_api_info.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_api_info.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_config.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_config.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_contacts.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_contacts.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_deployment.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_deployment.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_deployment_id.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_deployment_id.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_deployment_status.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_deployment_status.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_execution.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_execution.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_execution_logs.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_execution_logs.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_execution_request.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_execution_request.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_mode.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_mode.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_page.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_page.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_properties.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_properties.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_query_response.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_query_response.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_query_response_with_error.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_query_response_with_error.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_resources.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_resources.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_schedule.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_schedule.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_summary.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_summary.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/model/data_job_version.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/model/data_job_version.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/model/error.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/model/error.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/models/__init__.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/paths/__init__.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_info/get.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_info/get.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs/get.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs/get.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs/post.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs/post.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name/delete.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name/delete.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name/get.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name/get.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name/put.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name/put.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments/get.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments/get.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments/post.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments/post.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/delete.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/delete.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/get.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/get.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/patch.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/patch.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions/get.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions/get.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions/post.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions/post.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties/get.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties/get.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties/put.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties/put.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions/get.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions/get.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions_execution_id/delete.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions_execution_id/delete.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions_execution_id/get.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions_execution_id/get.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions_execution_id_logs/get.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_executions_execution_id_logs/get.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_keytab/get.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_keytab/get.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_sources/delete.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_sources/delete.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_sources/get.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_sources/get.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_sources/post.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_sources/post.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_team_new_team/put.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/paths/data_jobs_for_team_team_name_jobs_job_name_team_new_team/put.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/rest.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/rest.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/taurus_datajob_api/schemas.py` & `vdk-control-service-api-1.0.8/taurus_datajob_api/schemas.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_models/test_data_job.py` & `vdk-control-service-api-1.0.8/test/test_models/test_data_job.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_models/test_data_job_api_info.py` & `vdk-control-service-api-1.0.8/test/test_models/test_data_job_api_info.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_models/test_data_job_config.py` & `vdk-control-service-api-1.0.8/test/test_models/test_data_job_config.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_models/test_data_job_contacts.py` & `vdk-control-service-api-1.0.8/test/test_models/test_data_job_contacts.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_models/test_data_job_deployment.py` & `vdk-control-service-api-1.0.8/test/test_models/test_data_job_deployment.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_models/test_data_job_deployment_id.py` & `vdk-control-service-api-1.0.8/test/test_models/test_data_job_deployment_id.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_models/test_data_job_deployment_status.py` & `vdk-control-service-api-1.0.8/test/test_models/test_data_job_deployment_status.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_models/test_data_job_execution.py` & `vdk-control-service-api-1.0.8/test/test_models/test_data_job_execution.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_models/test_data_job_execution_logs.py` & `vdk-control-service-api-1.0.8/test/test_models/test_data_job_execution_logs.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_models/test_data_job_execution_request.py` & `vdk-control-service-api-1.0.8/test/test_models/test_data_job_execution_request.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_models/test_data_job_mode.py` & `vdk-control-service-api-1.0.8/test/test_models/test_data_job_mode.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_models/test_data_job_page.py` & `vdk-control-service-api-1.0.8/test/test_models/test_data_job_page.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_models/test_data_job_properties.py` & `vdk-control-service-api-1.0.8/test/test_models/test_data_job_properties.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_models/test_data_job_query_response.py` & `vdk-control-service-api-1.0.8/test/test_models/test_data_job_query_response.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_models/test_data_job_query_response_with_error.py` & `vdk-control-service-api-1.0.8/test/test_models/test_data_job_query_response_with_error.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_models/test_data_job_resources.py` & `vdk-control-service-api-1.0.8/test/test_models/test_data_job_resources.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_models/test_data_job_schedule.py` & `vdk-control-service-api-1.0.8/test/test_models/test_data_job_schedule.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_models/test_data_job_summary.py` & `vdk-control-service-api-1.0.8/test/test_models/test_data_job_summary.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_models/test_data_job_version.py` & `vdk-control-service-api-1.0.8/test/test_models/test_data_job_version.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_models/test_error.py` & `vdk-control-service-api-1.0.8/test/test_models/test_error.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_paths/__init__.py` & `vdk-control-service-api-1.0.8/test/test_paths/__init__.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_info/test_get.py` & `vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_info/test_get.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs/test_get.py` & `vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs/test_get.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs/test_post.py` & `vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs/test_post.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name/test_delete.py` & `vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name/test_delete.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name/test_get.py` & `vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name/test_get.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name/test_put.py` & `vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name/test_put.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments/test_get.py` & `vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments/test_get.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments/test_post.py` & `vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments/test_post.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/test_delete.py` & `vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/test_get.py` & `vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/test_get.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/test_patch.py` & `vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id/test_patch.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions/test_get.py` & `vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions/test_get.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions/test_post.py` & `vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_executions/test_post.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties/test_get.py` & `vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties/test_get.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties/test_put.py` & `vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_deployments_deployment_id_properties/test_put.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions/test_get.py` & `vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions/test_get.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions_execution_id/test_delete.py` & `vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions_execution_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions_execution_id/test_get.py` & `vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions_execution_id/test_get.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions_execution_id_logs/test_get.py` & `vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_executions_execution_id_logs/test_get.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_keytab/test_get.py` & `vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_keytab/test_get.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_sources/test_delete.py` & `vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_sources/test_delete.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_sources/test_get.py` & `vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_sources/test_get.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_sources/test_post.py` & `vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_sources/test_post.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_team_new_team/test_put.py` & `vdk-control-service-api-1.0.8/test/test_paths/test_data_jobs_for_team_team_name_jobs_job_name_team_new_team/test_put.py`

 * *Files identical despite different names*

### Comparing `vdk-control-service-api-1.0.7/vdk_control_service_api.egg-info/PKG-INFO` & `vdk-control-service-api-1.0.8/vdk_control_service_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-control-service-api
-Version: 1.0.7
+Version: 1.0.8
 Summary: Versatile Data Kit Control Service API
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: team@openapitools.org
 License: Apache 2.0
 Keywords: OpenAPI,OpenAPI-Generator,Versatile Data Kit Control Service API
 Requires-Python: >=3.7
```

### Comparing `vdk-control-service-api-1.0.7/vdk_control_service_api.egg-info/SOURCES.txt` & `vdk-control-service-api-1.0.8/vdk_control_service_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

