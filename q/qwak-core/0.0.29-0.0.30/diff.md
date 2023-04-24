# Comparing `tmp/qwak_core-0.0.29.tar.gz` & `tmp/qwak_core-0.0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_core-0.0.29.tar", max compression
+gzip compressed data, was "qwak_core-0.0.30.tar", max compression
```

## Comparing `qwak_core-0.0.29.tar` & `qwak_core-0.0.30.tar`

### file list

```diff
@@ -1,535 +1,535 @@
--rw-r--r--   0        0        0      264 2023-04-24 06:21:26.051415 qwak_core-0.0.29/README.md
--rw-r--r--   0        0        0        0 2023-04-24 06:22:14.007379 qwak_core-0.0.29/_qwak_proto/__init__.py
--rw-r--r--   0        0        0     5378 2023-04-24 06:22:14.027379 qwak_core-0.0.29/_qwak_proto/qwak/administration/account/v1/account_pb2.py
--rw-r--r--   0        0        0     6623 2023-04-24 06:21:59.199390 qwak_core-0.0.29/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.027379 qwak_core-0.0.29/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
--rw-r--r--   0        0        0     2390 2023-04-24 06:22:14.023379 qwak_core-0.0.29/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
--rw-r--r--   0        0        0     1475 2023-04-24 06:21:58.931390 qwak_core-0.0.29/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.023379 qwak_core-0.0.29/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     2106 2023-04-24 06:22:14.023379 qwak_core-0.0.29/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
--rw-r--r--   0        0        0     1207 2023-04-24 06:21:59.067390 qwak_core-0.0.29/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.027379 qwak_core-0.0.29/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
--rw-r--r--   0        0        0     6751 2023-04-24 06:22:14.019379 qwak_core-0.0.29/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
--rw-r--r--   0        0        0     4346 2023-04-24 06:21:58.543390 qwak_core-0.0.29/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
--rw-r--r--   0        0        0     7662 2023-04-24 06:22:14.019379 qwak_core-0.0.29/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-04-24 06:22:14.019379 qwak_core-0.0.29/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
--rw-r--r--   0        0        0     2650 2023-04-24 06:21:58.675390 qwak_core-0.0.29/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.019379 qwak_core-0.0.29/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
--rw-r--r--   0        0        0     4864 2023-04-24 06:22:14.023379 qwak_core-0.0.29/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
--rw-r--r--   0        0        0     5792 2023-04-24 06:21:58.803390 qwak_core-0.0.29/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.023379 qwak_core-0.0.29/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
--rw-r--r--   0        0        0     4635 2023-04-24 06:22:14.011379 qwak_core-0.0.29/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
--rw-r--r--   0        0        0     3664 2023-04-24 06:21:58.415390 qwak_core-0.0.29/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
--rw-r--r--   0        0        0     3167 2023-04-24 06:22:14.011379 qwak_core-0.0.29/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
--rw-r--r--   0        0        0     5670 2023-04-24 06:22:14.011379 qwak_core-0.0.29/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
--rw-r--r--   0        0        0     8035 2023-04-24 06:21:59.327389 qwak_core-0.0.29/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.011379 qwak_core-0.0.29/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     4512 2023-04-24 06:22:14.015379 qwak_core-0.0.29/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
--rw-r--r--   0        0        0     5690 2023-04-24 06:21:59.591389 qwak_core-0.0.29/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.015379 qwak_core-0.0.29/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
--rw-r--r--   0        0        0    16001 2023-04-24 06:22:14.015379 qwak_core-0.0.29/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
--rw-r--r--   0        0        0    12387 2023-04-24 06:21:59.723389 qwak_core-0.0.29/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
--rw-r--r--   0        0        0    16458 2023-04-24 06:22:14.015379 qwak_core-0.0.29/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2464 2023-04-24 06:22:14.011379 qwak_core-0.0.29/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
--rw-r--r--   0        0        0     1347 2023-04-24 06:21:59.455389 qwak_core-0.0.29/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.015379 qwak_core-0.0.29/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     6425 2023-04-24 06:22:14.015379 qwak_core-0.0.29/_qwak_proto/qwak/administration/v0/users/user_pb2.py
--rw-r--r--   0        0        0    10323 2023-04-24 06:21:59.851389 qwak_core-0.0.29/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.019379 qwak_core-0.0.29/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
--rw-r--r--   0        0        0     9577 2023-04-24 06:22:14.055379 qwak_core-0.0.29/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
--rw-r--r--   0        0        0    13624 2023-04-24 06:22:01.723388 qwak_core-0.0.29/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.055379 qwak_core-0.0.29/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
--rw-r--r--   0        0        0     9270 2023-04-24 06:22:14.055379 qwak_core-0.0.29/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
--rw-r--r--   0        0        0     5571 2023-04-24 06:22:01.851388 qwak_core-0.0.29/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
--rw-r--r--   0        0        0    10742 2023-04-24 06:22:14.059379 qwak_core-0.0.29/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
--rw-r--r--   0        0        0     7365 2023-04-24 06:22:14.103379 qwak_core-0.0.29/_qwak_proto/qwak/analytics/analytics_pb2.py
--rw-r--r--   0        0        0    11839 2023-04-24 06:22:05.555385 qwak_core-0.0.29/_qwak_proto/qwak/analytics/analytics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.107379 qwak_core-0.0.29/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
--rw-r--r--   0        0        0     9396 2023-04-24 06:22:14.107379 qwak_core-0.0.29/_qwak_proto/qwak/analytics/analytics_service_pb2.py
--rw-r--r--   0        0        0     7896 2023-04-24 06:22:05.683385 qwak_core-0.0.29/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
--rw-r--r--   0        0        0    11917 2023-04-24 06:22:14.107379 qwak_core-0.0.29/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
--rw-r--r--   0        0        0     9021 2023-04-24 06:22:14.111379 qwak_core-0.0.29/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
--rw-r--r--   0        0        0     5865 2023-04-24 06:22:06.347384 qwak_core-0.0.29/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
--rw-r--r--   0        0        0    11486 2023-04-24 06:22:14.111379 qwak_core-0.0.29/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
--rw-r--r--   0        0        0     8807 2023-04-24 06:22:14.107379 qwak_core-0.0.29/_qwak_proto/qwak/audience/v1/audience_pb2.py
--rw-r--r--   0        0        0    13570 2023-04-24 06:22:06.215384 qwak_core-0.0.29/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.107379 qwak_core-0.0.29/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
--rw-r--r--   0        0        0     5497 2023-04-24 06:22:14.111379 qwak_core-0.0.29/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     7820 2023-04-24 06:22:06.483384 qwak_core-0.0.29/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.111379 qwak_core-0.0.29/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     2937 2023-04-24 06:22:14.111379 qwak_core-0.0.29/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
--rw-r--r--   0        0        0     2014 2023-04-24 06:22:06.615384 qwak_core-0.0.29/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
--rw-r--r--   0        0        0     2991 2023-04-24 06:22:14.115379 qwak_core-0.0.29/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
--rw-r--r--   0        0        0    11441 2023-04-24 06:22:14.163379 qwak_core-0.0.29/_qwak_proto/qwak/automation/v1/action_pb2.py
--rw-r--r--   0        0        0    17892 2023-04-24 06:22:10.747381 qwak_core-0.0.29/_qwak_proto/qwak/automation/v1/action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.163379 qwak_core-0.0.29/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
--rw-r--r--   0        0        0     5494 2023-04-24 06:22:14.159379 qwak_core-0.0.29/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     7776 2023-04-24 06:22:10.487381 qwak_core-0.0.29/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.163379 qwak_core-0.0.29/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     3373 2023-04-24 06:22:14.163379 qwak_core-0.0.29/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
--rw-r--r--   0        0        0     4400 2023-04-24 06:22:10.615381 qwak_core-0.0.29/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.163379 qwak_core-0.0.29/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
--rw-r--r--   0        0        0    17887 2023-04-24 06:22:14.159379 qwak_core-0.0.29/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
--rw-r--r--   0        0        0    12310 2023-04-24 06:22:10.075382 qwak_core-0.0.29/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
--rw-r--r--   0        0        0    23338 2023-04-24 06:22:14.159379 qwak_core-0.0.29/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     3873 2023-04-24 06:22:14.159379 qwak_core-0.0.29/_qwak_proto/qwak/automation/v1/automation_pb2.py
--rw-r--r--   0        0        0     5291 2023-04-24 06:22:10.355381 qwak_core-0.0.29/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.159379 qwak_core-0.0.29/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
--rw-r--r--   0        0        0     2383 2023-04-24 06:22:14.167379 qwak_core-0.0.29/_qwak_proto/qwak/automation/v1/common_pb2.py
--rw-r--r--   0        0        0     2446 2023-04-24 06:22:11.135381 qwak_core-0.0.29/_qwak_proto/qwak/automation/v1/common_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.167379 qwak_core-0.0.29/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
--rw-r--r--   0        0        0     5209 2023-04-24 06:22:14.167379 qwak_core-0.0.29/_qwak_proto/qwak/automation/v1/notification_pb2.py
--rw-r--r--   0        0        0     5492 2023-04-24 06:22:11.007381 qwak_core-0.0.29/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.167379 qwak_core-0.0.29/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
--rw-r--r--   0        0        0     3604 2023-04-24 06:22:14.167379 qwak_core-0.0.29/_qwak_proto/qwak/automation/v1/trigger_pb2.py
--rw-r--r--   0        0        0     4212 2023-04-24 06:22:10.875381 qwak_core-0.0.29/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.167379 qwak_core-0.0.29/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
--rw-r--r--   0        0        0    10275 2023-04-24 06:22:14.195379 qwak_core-0.0.29/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
--rw-r--r--   0        0        0    14803 2023-04-24 06:22:13.535379 qwak_core-0.0.29/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.195379 qwak_core-0.0.29/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
--rw-r--r--   0        0        0     2042 2023-04-24 06:22:14.191379 qwak_core-0.0.29/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
--rw-r--r--   0        0        0     1904 2023-04-24 06:22:13.263379 qwak_core-0.0.29/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.195379 qwak_core-0.0.29/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
--rw-r--r--   0        0        0    37419 2023-04-24 06:22:14.195379 qwak_core-0.0.29/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
--rw-r--r--   0        0        0    48027 2023-04-24 06:22:13.403379 qwak_core-0.0.29/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
--rw-r--r--   0        0        0    29918 2023-04-24 06:22:14.195379 qwak_core-0.0.29/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
--rw-r--r--   0        0        0    18658 2023-04-24 06:22:14.131379 qwak_core-0.0.29/_qwak_proto/qwak/build/v1/build_api_pb2.py
--rw-r--r--   0        0        0    15525 2023-04-24 06:22:07.975383 qwak_core-0.0.29/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
--rw-r--r--   0        0        0    18652 2023-04-24 06:22:14.131379 qwak_core-0.0.29/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
--rw-r--r--   0        0        0    16953 2023-04-24 06:22:14.131379 qwak_core-0.0.29/_qwak_proto/qwak/build/v1/build_pb2.py
--rw-r--r--   0        0        0    25941 2023-04-24 06:22:07.835383 qwak_core-0.0.29/_qwak_proto/qwak/build/v1/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.131379 qwak_core-0.0.29/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
--rw-r--r--   0        0        0    11034 2023-04-24 06:22:14.123379 qwak_core-0.0.29/_qwak_proto/qwak/builds/build_pb2.py
--rw-r--r--   0        0        0    18276 2023-04-24 06:22:07.559383 qwak_core-0.0.29/_qwak_proto/qwak/builds/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.123379 qwak_core-0.0.29/_qwak_proto/qwak/builds/build_pb2_grpc.py
--rw-r--r--   0        0        0     4777 2023-04-24 06:22:14.123379 qwak_core-0.0.29/_qwak_proto/qwak/builds/build_url_pb2.py
--rw-r--r--   0        0        0     5773 2023-04-24 06:22:07.691383 qwak_core-0.0.29/_qwak_proto/qwak/builds/build_url_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.127379 qwak_core-0.0.29/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
--rw-r--r--   0        0        0    12490 2023-04-24 06:22:14.127379 qwak_core-0.0.29/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
--rw-r--r--   0        0        0     9351 2023-04-24 06:22:08.107383 qwak_core-0.0.29/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
--rw-r--r--   0        0        0    14916 2023-04-24 06:22:14.127379 qwak_core-0.0.29/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
--rw-r--r--   0        0        0    38245 2023-04-24 06:22:14.127379 qwak_core-0.0.29/_qwak_proto/qwak/builds/builds_pb2.py
--rw-r--r--   0        0        0    52572 2023-04-24 06:22:08.395383 qwak_core-0.0.29/_qwak_proto/qwak/builds/builds_pb2.pyi
--rw-r--r--   0        0        0    11572 2023-04-24 06:22:14.127379 qwak_core-0.0.29/_qwak_proto/qwak/builds/builds_pb2_grpc.py
--rw-r--r--   0        0        0     1671 2023-04-24 06:22:14.143379 qwak_core-0.0.29/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
--rw-r--r--   0        0        0     1689 2023-04-24 06:22:08.671383 qwak_core-0.0.29/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.143379 qwak_core-0.0.29/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4328 2023-04-24 06:22:14.143379 qwak_core-0.0.29/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-04-24 06:22:08.803382 qwak_core-0.0.29/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-04-24 06:22:14.143379 qwak_core-0.0.29/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     7716 2023-04-24 06:22:14.119379 qwak_core-0.0.29/_qwak_proto/qwak/deployment/alert_pb2.py
--rw-r--r--   0        0        0    11197 2023-04-24 06:22:07.159384 qwak_core-0.0.29/_qwak_proto/qwak/deployment/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.119379 qwak_core-0.0.29/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
--rw-r--r--   0        0        0    11580 2023-04-24 06:22:14.119379 qwak_core-0.0.29/_qwak_proto/qwak/deployment/alert_service_pb2.py
--rw-r--r--   0        0        0     7373 2023-04-24 06:22:07.295384 qwak_core-0.0.29/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
--rw-r--r--   0        0        0    12803 2023-04-24 06:22:14.123379 qwak_core-0.0.29/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
--rw-r--r--   0        0        0     2162 2023-04-24 06:22:14.115379 qwak_core-0.0.29/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
--rw-r--r--   0        0        0     2685 2023-04-24 06:22:06.887384 qwak_core-0.0.29/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.115379 qwak_core-0.0.29/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
--rw-r--r--   0        0        0    42956 2023-04-24 06:22:14.115379 qwak_core-0.0.29/_qwak_proto/qwak/deployment/deployment_pb2.py
--rw-r--r--   0        0        0    62847 2023-04-24 06:22:06.755384 qwak_core-0.0.29/_qwak_proto/qwak/deployment/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.115379 qwak_core-0.0.29/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    38320 2023-04-24 06:22:14.119379 qwak_core-0.0.29/_qwak_proto/qwak/deployment/deployment_service_pb2.py
--rw-r--r--   0        0        0    33325 2023-04-24 06:22:07.023384 qwak_core-0.0.29/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
--rw-r--r--   0        0        0    20242 2023-04-24 06:22:14.119379 qwak_core-0.0.29/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2527 2023-04-24 06:22:14.047379 qwak_core-0.0.29/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
--rw-r--r--   0        0        0     2791 2023-04-24 06:22:01.059388 qwak_core-0.0.29/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.047379 qwak_core-0.0.29/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-04-24 06:22:14.047379 qwak_core-0.0.29/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
--rw-r--r--   0        0        0    12641 2023-04-24 06:22:01.195388 qwak_core-0.0.29/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.051379 qwak_core-0.0.29/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
--rw-r--r--   0        0        0    15709 2023-04-24 06:22:14.051379 qwak_core-0.0.29/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
--rw-r--r--   0        0        0    16335 2023-04-24 06:22:01.327388 qwak_core-0.0.29/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
--rw-r--r--   0        0        0    10706 2023-04-24 06:22:14.051379 qwak_core-0.0.29/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
--rw-r--r--   0        0        0     4787 2023-04-24 06:22:14.091379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
--rw-r--r--   0        0        0     6713 2023-04-24 06:22:04.751386 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.091379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
--rw-r--r--   0        0        0     9721 2023-04-24 06:22:14.091379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
--rw-r--r--   0        0        0     7409 2023-04-24 06:22:04.623386 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
--rw-r--r--   0        0        0    12256 2023-04-24 06:22:14.091379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
--rw-r--r--   0        0        0     9535 2023-04-24 06:22:14.079379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
--rw-r--r--   0        0        0    10460 2023-04-24 06:22:03.547386 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.079379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
--rw-r--r--   0        0        0     5268 2023-04-24 06:22:14.075379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/features/execution_pb2.py
--rw-r--r--   0        0        0     8525 2023-04-24 06:22:03.395386 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.075379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
--rw-r--r--   0        0        0    10074 2023-04-24 06:22:14.071379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
--rw-r--r--   0        0        0    14303 2023-04-24 06:22:02.971387 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.071379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
--rw-r--r--   0        0        0    27847 2023-04-24 06:22:14.075379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
--rw-r--r--   0        0        0    20073 2023-04-24 06:22:03.267387 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
--rw-r--r--   0        0        0    33080 2023-04-24 06:22:14.075379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
--rw-r--r--   0        0        0    12638 2023-04-24 06:22:14.079379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
--rw-r--r--   0        0        0    14071 2023-04-24 06:22:03.679386 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.079379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
--rw-r--r--   0        0        0    10044 2023-04-24 06:22:14.079379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
--rw-r--r--   0        0        0     6846 2023-04-24 06:22:03.815386 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
--rw-r--r--   0        0        0    11647 2023-04-24 06:22:14.083379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
--rw-r--r--   0        0        0    24876 2023-04-24 06:22:14.071379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
--rw-r--r--   0        0        0    36861 2023-04-24 06:22:03.127387 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.075379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
--rw-r--r--   0        0        0     2872 2023-04-24 06:22:14.083379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
--rw-r--r--   0        0        0     2428 2023-04-24 06:22:03.955386 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.083379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
--rw-r--r--   0        0        0     4196 2023-04-24 06:22:14.091379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
--rw-r--r--   0        0        0     7323 2023-04-24 06:22:13.663379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.095379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
--rw-r--r--   0        0        0     9895 2023-04-24 06:22:14.095379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
--rw-r--r--   0        0        0     9029 2023-04-24 06:22:13.803379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
--rw-r--r--   0        0        0    12090 2023-04-24 06:22:14.095379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     3596 2023-04-24 06:22:14.095379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
--rw-r--r--   0        0        0     6664 2023-04-24 06:22:05.151385 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.095379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
--rw-r--r--   0        0        0    11930 2023-04-24 06:22:14.099379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
--rw-r--r--   0        0        0    11052 2023-04-24 06:22:05.283385 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
--rw-r--r--   0        0        0    14459 2023-04-24 06:22:14.099379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     5158 2023-04-24 06:22:14.099379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/reports/report_pb2.py
--rw-r--r--   0        0        0     7436 2023-04-24 06:22:05.415385 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.099379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
--rw-r--r--   0        0        0     4549 2023-04-24 06:22:14.103379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
--rw-r--r--   0        0        0     6442 2023-04-24 06:22:05.951385 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.103379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
--rw-r--r--   0        0        0    16693 2023-04-24 06:22:14.099379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
--rw-r--r--   0        0        0    20355 2023-04-24 06:22:05.819385 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
--rw-r--r--   0        0        0     4809 2023-04-24 06:22:14.103379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
--rw-r--r--   0        0        0     2553 2023-04-24 06:22:14.103379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
--rw-r--r--   0        0        0     4000 2023-04-24 06:22:06.083384 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.103379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
--rw-r--r--   0        0        0    13329 2023-04-24 06:22:14.083379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
--rw-r--r--   0        0        0    23039 2023-04-24 06:22:04.087386 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.083379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
--rw-r--r--   0        0        0     5087 2023-04-24 06:22:14.087379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
--rw-r--r--   0        0        0     6011 2023-04-24 06:22:04.219386 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.087379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
--rw-r--r--   0        0        0    12309 2023-04-24 06:22:14.087379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
--rw-r--r--   0        0        0     9244 2023-04-24 06:22:04.355386 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
--rw-r--r--   0        0        0    17071 2023-04-24 06:22:14.087379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
--rw-r--r--   0        0        0    11014 2023-04-24 06:22:14.087379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
--rw-r--r--   0        0        0    15865 2023-04-24 06:22:04.487386 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.087379 qwak_core-0.0.29/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
--rw-r--r--   0        0        0     4727 2023-04-24 06:22:14.171379 qwak_core-0.0.29/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
--rw-r--r--   0        0        0     5122 2023-04-24 06:22:11.271381 qwak_core-0.0.29/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.171379 qwak_core-0.0.29/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4648 2023-04-24 06:22:14.171379 qwak_core-0.0.29/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4170 2023-04-24 06:22:11.403381 qwak_core-0.0.29/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-04-24 06:22:14.171379 qwak_core-0.0.29/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     5349 2023-04-24 06:22:14.171379 qwak_core-0.0.29/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
--rw-r--r--   0        0        0     5363 2023-04-24 06:22:11.535380 qwak_core-0.0.29/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.175379 qwak_core-0.0.29/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4437 2023-04-24 06:22:14.175379 qwak_core-0.0.29/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4127 2023-04-24 06:22:11.671380 qwak_core-0.0.29/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-04-24 06:22:14.175379 qwak_core-0.0.29/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     6073 2023-04-24 06:22:14.175379 qwak_core-0.0.29/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
--rw-r--r--   0        0        0     5366 2023-04-24 06:22:11.811380 qwak_core-0.0.29/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
--rw-r--r--   0        0        0     7395 2023-04-24 06:22:14.175379 qwak_core-0.0.29/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
--rw-r--r--   0        0        0     4636 2023-04-24 06:22:14.179379 qwak_core-0.0.29/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
--rw-r--r--   0        0        0     4239 2023-04-24 06:22:11.939380 qwak_core-0.0.29/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.179379 qwak_core-0.0.29/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     2376 2023-04-24 06:22:14.147379 qwak_core-0.0.29/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
--rw-r--r--   0        0        0     3018 2023-04-24 06:22:08.931383 qwak_core-0.0.29/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.147379 qwak_core-0.0.29/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4325 2023-04-24 06:22:14.147379 qwak_core-0.0.29/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-04-24 06:22:09.127382 qwak_core-0.0.29/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-04-24 06:22:14.147379 qwak_core-0.0.29/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     6401 2023-04-24 06:22:14.059379 qwak_core-0.0.29/_qwak_proto/qwak/fitness_service/constructs_pb2.py
--rw-r--r--   0        0        0    10192 2023-04-24 06:22:02.435387 qwak_core-0.0.29/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.063379 qwak_core-0.0.29/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-04-24 06:22:14.063379 qwak_core-0.0.29/_qwak_proto/qwak/fitness_service/fitness_pb2.py
--rw-r--r--   0        0        0     4115 2023-04-24 06:22:02.563387 qwak_core-0.0.29/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.063379 qwak_core-0.0.29/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
--rw-r--r--   0        0        0     7123 2023-04-24 06:22:14.067379 qwak_core-0.0.29/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
--rw-r--r--   0        0        0     3981 2023-04-24 06:22:02.695387 qwak_core-0.0.29/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
--rw-r--r--   0        0        0     8546 2023-04-24 06:22:14.067379 qwak_core-0.0.29/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
--rw-r--r--   0        0        0     8428 2023-04-24 06:22:14.067379 qwak_core-0.0.29/_qwak_proto/qwak/fitness_service/status_pb2.py
--rw-r--r--   0        0        0    12205 2023-04-24 06:22:02.827387 qwak_core-0.0.29/_qwak_proto/qwak/fitness_service/status_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.071379 qwak_core-0.0.29/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
--rw-r--r--   0        0        0     8196 2023-04-24 06:22:14.123379 qwak_core-0.0.29/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
--rw-r--r--   0        0        0    10867 2023-04-24 06:22:07.423384 qwak_core-0.0.29/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
--rw-r--r--   0        0        0     4700 2023-04-24 06:22:14.123379 qwak_core-0.0.29/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
--rw-r--r--   0        0        0     7803 2023-04-24 06:22:14.179379 qwak_core-0.0.29/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
--rw-r--r--   0        0        0    10487 2023-04-24 06:22:12.071380 qwak_core-0.0.29/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.179379 qwak_core-0.0.29/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
--rw-r--r--   0        0        0     3704 2023-04-24 06:22:14.179379 qwak_core-0.0.29/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
--rw-r--r--   0        0        0     3759 2023-04-24 06:22:12.199380 qwak_core-0.0.29/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.179379 qwak_core-0.0.29/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
--rw-r--r--   0        0        0    22089 2023-04-24 06:22:14.183379 qwak_core-0.0.29/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
--rw-r--r--   0        0        0    25879 2023-04-24 06:22:12.339380 qwak_core-0.0.29/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.183379 qwak_core-0.0.29/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
--rw-r--r--   0        0        0    13157 2023-04-24 06:22:14.183379 qwak_core-0.0.29/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
--rw-r--r--   0        0        0    21705 2023-04-24 06:22:12.471380 qwak_core-0.0.29/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.183379 qwak_core-0.0.29/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-04-24 06:22:14.183379 qwak_core-0.0.29/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
--rw-r--r--   0        0        0    16128 2023-04-24 06:22:12.603380 qwak_core-0.0.29/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.187379 qwak_core-0.0.29/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
--rw-r--r--   0        0        0    45273 2023-04-24 06:22:14.187379 qwak_core-0.0.29/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
--rw-r--r--   0        0        0    35031 2023-04-24 06:22:12.747380 qwak_core-0.0.29/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
--rw-r--r--   0        0        0    67567 2023-04-24 06:22:14.187379 qwak_core-0.0.29/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2023-04-24 06:22:14.187379 qwak_core-0.0.29/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
--rw-r--r--   0        0        0     2637 2023-04-24 06:22:12.879380 qwak_core-0.0.29/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.187379 qwak_core-0.0.29/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
--rw-r--r--   0        0        0     3459 2023-04-24 06:22:14.151379 qwak_core-0.0.29/_qwak_proto/qwak/logging/log_filter_pb2.py
--rw-r--r--   0        0        0     4169 2023-04-24 06:22:09.447382 qwak_core-0.0.29/_qwak_proto/qwak/logging/log_filter_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.151379 qwak_core-0.0.29/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
--rw-r--r--   0        0        0     2233 2023-04-24 06:22:14.155379 qwak_core-0.0.29/_qwak_proto/qwak/logging/log_line_pb2.py
--rw-r--r--   0        0        0     2135 2023-04-24 06:22:09.939382 qwak_core-0.0.29/_qwak_proto/qwak/logging/log_line_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.155379 qwak_core-0.0.29/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
--rw-r--r--   0        0        0     3126 2023-04-24 06:22:14.151379 qwak_core-0.0.29/_qwak_proto/qwak/logging/log_reader_service_pb2.py
--rw-r--r--   0        0        0     3479 2023-04-24 06:22:09.591382 qwak_core-0.0.29/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
--rw-r--r--   0        0        0     2831 2023-04-24 06:22:14.155379 qwak_core-0.0.29/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
--rw-r--r--   0        0        0     9322 2023-04-24 06:22:14.155379 qwak_core-0.0.29/_qwak_proto/qwak/logging/log_source_pb2.py
--rw-r--r--   0        0        0    13291 2023-04-24 06:22:09.755382 qwak_core-0.0.29/_qwak_proto/qwak/logging/log_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.155379 qwak_core-0.0.29/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
--rw-r--r--   0        0        0    22744 2023-04-24 06:22:14.139379 qwak_core-0.0.29/_qwak_proto/qwak/models/models_pb2.py
--rw-r--r--   0        0        0    27142 2023-04-24 06:22:08.539383 qwak_core-0.0.29/_qwak_proto/qwak/models/models_pb2.pyi
--rw-r--r--   0        0        0    14733 2023-04-24 06:22:14.139379 qwak_core-0.0.29/_qwak_proto/qwak/models/models_pb2_grpc.py
--rw-r--r--   0        0        0    10745 2023-04-24 06:22:14.043379 qwak_core-0.0.29/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
--rw-r--r--   0        0        0     6790 2023-04-24 06:22:02.135387 qwak_core-0.0.29/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
--rw-r--r--   0        0        0    13657 2023-04-24 06:22:14.043379 qwak_core-0.0.29/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
--rw-r--r--   0        0        0    11564 2023-04-24 06:22:14.039379 qwak_core-0.0.29/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
--rw-r--r--   0        0        0    14927 2023-04-24 06:22:01.995387 qwak_core-0.0.29/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.043379 qwak_core-0.0.29/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
--rw-r--r--   0        0        0     5283 2023-04-24 06:22:14.043379 qwak_core-0.0.29/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
--rw-r--r--   0        0        0     3745 2023-04-24 06:22:02.267387 qwak_core-0.0.29/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
--rw-r--r--   0        0        0     5551 2023-04-24 06:22:14.047379 qwak_core-0.0.29/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
--rw-r--r--   0        0        0     8701 2023-04-24 06:22:14.131379 qwak_core-0.0.29/_qwak_proto/qwak/projects/projects_pb2.py
--rw-r--r--   0        0        0     9794 2023-04-24 06:22:08.251383 qwak_core-0.0.29/_qwak_proto/qwak/projects/projects_pb2.pyi
--rw-r--r--   0        0        0     7931 2023-04-24 06:22:14.139379 qwak_core-0.0.29/_qwak_proto/qwak/projects/projects_pb2_grpc.py
--rw-r--r--   0        0        0     4752 2023-04-24 06:22:14.147379 qwak_core-0.0.29/_qwak_proto/qwak/secret_service/secret_service_pb2.py
--rw-r--r--   0        0        0     2818 2023-04-24 06:22:09.279382 qwak_core-0.0.29/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
--rw-r--r--   0        0        0     6253 2023-04-24 06:22:14.151379 qwak_core-0.0.29/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
--rw-r--r--   0        0        0     6225 2023-04-24 06:22:14.039379 qwak_core-0.0.29/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
--rw-r--r--   0        0        0     7267 2023-04-24 06:22:00.523388 qwak_core-0.0.29/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.039379 qwak_core-0.0.29/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
--rw-r--r--   0        0        0    16176 2023-04-24 06:22:14.031379 qwak_core-0.0.29/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
--rw-r--r--   0        0        0    10166 2023-04-24 06:22:00.387389 qwak_core-0.0.29/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
--rw-r--r--   0        0        0    19988 2023-04-24 06:22:14.035379 qwak_core-0.0.29/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
--rw-r--r--   0        0        0     1751 2023-04-24 06:22:14.027379 qwak_core-0.0.29/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
--rw-r--r--   0        0        0      777 2023-04-24 06:21:59.979389 qwak_core-0.0.29/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.027379 qwak_core-0.0.29/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
--rw-r--r--   0        0        0     2392 2023-04-24 06:22:14.027379 qwak_core-0.0.29/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
--rw-r--r--   0        0        0     2129 2023-04-24 06:22:00.115389 qwak_core-0.0.29/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.031379 qwak_core-0.0.29/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
--rw-r--r--   0        0        0    10389 2023-04-24 06:22:14.031379 qwak_core-0.0.29/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
--rw-r--r--   0        0        0     8148 2023-04-24 06:22:00.251389 qwak_core-0.0.29/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
--rw-r--r--   0        0        0    10512 2023-04-24 06:22:14.031379 qwak_core-0.0.29/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
--rw-r--r--   0        0        0     6843 2023-04-24 06:22:14.191379 qwak_core-0.0.29/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
--rw-r--r--   0        0        0     4585 2023-04-24 06:22:13.135379 qwak_core-0.0.29/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
--rw-r--r--   0        0        0     8228 2023-04-24 06:22:14.191379 qwak_core-0.0.29/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
--rw-r--r--   0        0        0     7816 2023-04-24 06:22:14.191379 qwak_core-0.0.29/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
--rw-r--r--   0        0        0    11958 2023-04-24 06:22:13.007379 qwak_core-0.0.29/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.191379 qwak_core-0.0.29/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
--rw-r--r--   0        0        0     4083 2023-04-24 06:22:14.051379 qwak_core-0.0.29/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
--rw-r--r--   0        0        0     4036 2023-04-24 06:22:01.455388 qwak_core-0.0.29/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.051379 qwak_core-0.0.29/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
--rw-r--r--   0        0        0     3001 2023-04-24 06:22:14.055379 qwak_core-0.0.29/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
--rw-r--r--   0        0        0     2574 2023-04-24 06:22:01.587388 qwak_core-0.0.29/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-24 06:22:14.055379 qwak_core-0.0.29/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
--rw-r--r--   0        0        0     1906 2023-04-24 06:22:15.419378 qwak_core-0.0.29/pyproject.toml
--rw-r--r--   0        0        0      447 2023-04-24 06:22:15.419378 qwak_core-0.0.29/qwak/__init__.py
--rw-r--r--   0        0        0     1204 2023-04-24 06:21:26.051415 qwak_core-0.0.29/qwak/automations/__init__.py
--rw-r--r--   0        0        0     3132 2023-04-24 06:21:26.051415 qwak_core-0.0.29/qwak/automations/automation_executions.py
--rw-r--r--   0        0        0    32139 2023-04-24 06:21:26.051415 qwak_core-0.0.29/qwak/automations/automations.py
--rw-r--r--   0        0        0        0 2023-04-24 06:21:26.051415 qwak_core-0.0.29/qwak/clients/__init__.py
--rw-r--r--   0        0        0      224 2023-04-24 06:21:26.051415 qwak_core-0.0.29/qwak/clients/administration/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 06:21:26.051415 qwak_core-0.0.29/qwak/clients/administration/authenticated_user/__init__.py
--rw-r--r--   0        0        0     1456 2023-04-24 06:21:26.051415 qwak_core-0.0.29/qwak/clients/administration/authenticated_user/client.py
--rw-r--r--   0        0        0        0 2023-04-24 06:21:26.051415 qwak_core-0.0.29/qwak/clients/administration/authentication/__init__.py
--rw-r--r--   0        0        0     1076 2023-04-24 06:21:26.051415 qwak_core-0.0.29/qwak/clients/administration/authentication/client.py
--rw-r--r--   0        0        0        0 2023-04-24 06:21:26.051415 qwak_core-0.0.29/qwak/clients/administration/eco_system/__init__.py
--rw-r--r--   0        0        0     5478 2023-04-24 06:21:26.051415 qwak_core-0.0.29/qwak/clients/administration/eco_system/client.py
--rw-r--r--   0        0        0        0 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/administration/environment/__init__.py
--rw-r--r--   0        0        0     2704 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/administration/environment/client.py
--rw-r--r--   0        0        0        0 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/administration/self_service/__init__.py
--rw-r--r--   0        0        0     2602 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/administration/self_service/client.py
--rw-r--r--   0        0        0       43 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/alert_management/__init__.py
--rw-r--r--   0        0        0     2226 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/alert_management/client.py
--rw-r--r--   0        0        0       42 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/analytics/__init__.py
--rw-r--r--   0        0        0     3093 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/analytics/client.py
--rw-r--r--   0        0        0       35 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/audience/__init__.py
--rw-r--r--   0        0        0     2110 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/audience/client.py
--rw-r--r--   0        0        0        0 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/automation_management/__init__.py
--rw-r--r--   0        0        0     8836 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/automation_management/client.py
--rw-r--r--   0        0        0       38 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/autoscaling/__init__.py
--rw-r--r--   0        0        0     1240 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/autoscaling/client.py
--rw-r--r--   0        0        0       77 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/batch_job_management/__init__.py
--rw-r--r--   0        0        0    17275 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/batch_job_management/client.py
--rw-r--r--   0        0        0     6242 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/batch_job_management/executions_config.py
--rw-r--r--   0        0        0     1846 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/batch_job_management/results.py
--rw-r--r--   0        0        0       43 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/build_management/__init__.py
--rw-r--r--   0        0        0     4731 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/build_management/client.py
--rw-r--r--   0        0        0       44 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/build_orchestrator/__init__.py
--rw-r--r--   0        0        0    14950 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/build_orchestrator/client.py
--rw-r--r--   0        0        0        0 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/data_versioning/__init__.py
--rw-r--r--   0        0        0     1835 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/data_versioning/client.py
--rw-r--r--   0        0        0        0 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/deployment/__init__.py
--rw-r--r--   0        0        0     6269 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/deployment/client.py
--rw-r--r--   0        0        0       53 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/feature_store/__init__.py
--rw-r--r--   0        0        0     2635 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/feature_store/job_registry_client.py
--rw-r--r--   0        0        0    15898 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/feature_store/management_client.py
--rw-r--r--   0        0        0     4963 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/feature_store/operator_client.py
--rw-r--r--   0        0        0        0 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/file_versioning/__init__.py
--rw-r--r--   0        0        0     1939 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/file_versioning/client.py
--rw-r--r--   0        0        0       41 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/kube_deployment_captain/__init__.py
--rw-r--r--   0        0        0     9276 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/kube_deployment_captain/client.py
--rw-r--r--   0        0        0       34 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/logging_client/__init__.py
--rw-r--r--   0        0        0     4255 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/logging_client/client.py
--rw-r--r--   0        0        0       43 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/model_management/__init__.py
--rw-r--r--   0        0        0     3695 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/model_management/client.py
--rw-r--r--   0        0        0        0 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/project/__init__.py
--rw-r--r--   0        0        0     2128 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/project/client.py
--rw-r--r--   0        0        0       40 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/secret_service/__init__.py
--rw-r--r--   0        0        0     2585 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/secret_service/client.py
--rw-r--r--   0        0        0       50 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/user_application_instance/__init__.py
--rw-r--r--   0        0        0     6013 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/clients/user_application_instance/client.py
--rw-r--r--   0        0        0      380 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/exceptions/__init__.py
--rw-r--r--   0        0        0      559 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/exceptions/quiet_error.py
--rw-r--r--   0        0        0      469 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/exceptions/qwak_build_exception.py
--rw-r--r--   0        0        0      135 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/exceptions/qwak_exception.py
--rw-r--r--   0        0        0      579 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/exceptions/qwak_http_exception.py
--rw-r--r--   0        0        0      100 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/exceptions/qwak_inference_exception.py
--rw-r--r--   0        0        0      274 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/exceptions/qwak_load_model_failed_exception.py
--rw-r--r--   0        0        0      211 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/exceptions/qwak_login_exception.py
--rw-r--r--   0        0        0      152 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/exceptions/qwak_mock_http_exception.py
--rw-r--r--   0        0        0      153 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/exceptions/qwak_model_initialization_exception.py
--rw-r--r--   0        0        0      152 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/exceptions/qwak_not_found_exception.py
--rw-r--r--   0        0        0      356 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/exceptions/qwak_quiet_build_exception.py
--rw-r--r--   0        0        0        0 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/feature_store/__init__.py
--rw-r--r--   0        0        0     1201 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/feature_store/data_sources/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/feature_store/data_sources/batch_sources/__init__.py
--rw-r--r--   0        0        0     1927 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/feature_store/data_sources/batch_sources/_batch.py
--rw-r--r--   0        0        0      666 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/feature_store/data_sources/batch_sources/_jdbc.py
--rw-r--r--   0        0        0     3059 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/feature_store/data_sources/batch_sources/big_query.py
--rw-r--r--   0        0        0     2006 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/feature_store/data_sources/batch_sources/csv.py
--rw-r--r--   0        0        0     2167 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/feature_store/data_sources/batch_sources/elastic_search.py
--rw-r--r--   0        0        0     2961 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
--rw-r--r--   0        0        0     1930 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/feature_store/data_sources/batch_sources/mongodb.py
--rw-r--r--   0        0        0     1669 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/feature_store/data_sources/batch_sources/mysql.py
--rw-r--r--   0        0        0     1730 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/feature_store/data_sources/batch_sources/parquet.py
--rw-r--r--   0        0        0     1722 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/feature_store/data_sources/batch_sources/postgres.py
--rw-r--r--   0        0        0     3216 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/feature_store/data_sources/batch_sources/redshift.py
--rw-r--r--   0        0        0     2616 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/feature_store/data_sources/batch_sources/snowflake.py
--rw-r--r--   0        0        0     1839 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/feature_store/data_sources/batch_sources/vertica.py
--rw-r--r--   0        0        0        0 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/feature_store/entities/__init__.py
--rw-r--r--   0        0        0     1794 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/feature_store/entities/entity.py
--rw-r--r--   0        0        0        0 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/feature_store/feature_sets/__init__.py
--rw-r--r--   0        0        0     1547 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/feature_store/feature_sets/backfill.py
--rw-r--r--   0        0        0    16848 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/feature_store/feature_sets/batch.py
--rw-r--r--   0        0        0      263 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/feature_store/feature_sets/context.py
--rw-r--r--   0        0        0     1630 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/feature_store/feature_sets/execution_spec.py
--rw-r--r--   0        0        0      584 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/feature_store/feature_sets/metadata.py
--rw-r--r--   0        0        0     6820 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/feature_store/feature_sets/read_policies.py
--rw-r--r--   0        0        0     1554 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/feature_store/feature_sets/transformations.py
--rw-r--r--   0        0        0        0 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/feature_store/online/__init__.py
--rw-r--r--   0        0        0     8808 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/feature_store/online/client.py
--rw-r--r--   0        0        0      226 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/inner/__init__.py
--rw-r--r--   0        0        0      954 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/inner/const.py
--rw-r--r--   0        0        0     1377 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/inner/di_configuration/__init__.py
--rw-r--r--   0        0        0     5933 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/inner/di_configuration/account.py
--rw-r--r--   0        0        0       73 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/inner/di_configuration/config.yml
--rw-r--r--   0        0        0      621 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/inner/di_configuration/containers.py
--rw-r--r--   0        0        0      344 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/inner/di_configuration/session.py
--rw-r--r--   0        0        0     2336 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/inner/model_loggers_utils.py
--rw-r--r--   0        0        0      266 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/inner/runtime_di/__init__.py
--rw-r--r--   0        0        0      349 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/inner/runtime_di/containers.py
--rw-r--r--   0        0        0      627 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/inner/singleton_meta.py
--rw-r--r--   0        0        0       74 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/inner/tool/__init__.py
--rw-r--r--   0        0        0     3414 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/inner/tool/auth.py
--rw-r--r--   0        0        0        0 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/inner/tool/grpc/__init__.py
--rw-r--r--   0        0        0      560 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/inner/tool/grpc/grpc_auth.py
--rw-r--r--   0        0        0     5804 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/inner/tool/grpc/grpc_tools.py
--rw-r--r--   0        0        0      473 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/inner/tool/grpc/grpc_try_wrapping.py
--rw-r--r--   0        0        0      435 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/inner/tool/retry_utils.py
--rw-r--r--   0        0        0      218 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/inner/tool/run_config/__init__.py
--rw-r--r--   0        0        0     3148 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/inner/tool/run_config/base.py
--rw-r--r--   0        0        0     6071 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/inner/tool/run_config/utils.py
--rw-r--r--   0        0        0        0 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/model/__init__.py
--rw-r--r--   0        0        0     1739 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/model/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/model/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      198 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/model/adapters/input_adapters/base_input_adapter.py
--rw-r--r--   0        0        0      210 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
--rw-r--r--   0        0        0      205 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/model/adapters/input_adapters/file_input_adapter.py
--rw-r--r--   0        0        0      206 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/model/adapters/input_adapters/image_input_adapter.py
--rw-r--r--   0        0        0      205 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/model/adapters/input_adapters/json_input_adapter.py
--rw-r--r--   0        0        0     2175 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/model/adapters/input_adapters/multi_input_adapter.py
--rw-r--r--   0        0        0     3208 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/model/adapters/input_adapters/numpy_input_adapter.py
--rw-r--r--   0        0        0      862 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/model/adapters/input_adapters/proto_input_adapter.py
--rw-r--r--   0        0        0      207 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/model/adapters/input_adapters/string_input_adapter.py
--rw-r--r--   0        0        0      209 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
--rw-r--r--   0        0        0        0 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/model/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      315 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/model/adapters/output_adapters/base_output_adapter.py
--rw-r--r--   0        0        0      221 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
--rw-r--r--   0        0        0      219 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/model/adapters/output_adapters/default_output_adapter.py
--rw-r--r--   0        0        0      216 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/model/adapters/output_adapters/json_output_adapter.py
--rw-r--r--   0        0        0     1065 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/model/adapters/output_adapters/numpy_output_adapter.py
--rw-r--r--   0        0        0      517 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/model/adapters/output_adapters/proto_output_adapter.py
--rw-r--r--   0        0        0      115 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
--rw-r--r--   0        0        0      220 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
--rw-r--r--   0        0        0      303 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/model/analytics_logging.py
--rw-r--r--   0        0        0     2865 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/model/base.py
--rw-r--r--   0        0        0        0 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/model/decorators/__init__.py
--rw-r--r--   0        0        0     1288 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/model/decorators/api.py
--rw-r--r--   0        0        0      861 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/model/decorators/api_implementation.py
--rw-r--r--   0        0        0     1503 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/model/experiment_tracking.py
--rw-r--r--   0        0        0      726 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/model/schema.py
--rw-r--r--   0        0        0     2964 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/model/schema_entities.py
--rw-r--r--   0        0        0        0 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/model/utils/__init__.py
--rw-r--r--   0        0        0      320 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/model/utils/extract_wrapped_function.py
--rw-r--r--   0        0        0        0 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/model_loggers/__init__.py
--rw-r--r--   0        0        0     2701 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/model_loggers/artifact_logger.py
--rw-r--r--   0        0        0     5186 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/model_loggers/data_logger.py
--rw-r--r--   0        0        0      852 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/model_loggers/model_logger.py
--rw-r--r--   0        0        0        0 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/qwak_client/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/qwak_client/builds/__init__.py
--rw-r--r--   0        0        0     3698 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/qwak_client/builds/build.py
--rw-r--r--   0        0        0        0 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/qwak_client/builds/filters/__init__.py
--rw-r--r--   0        0        0     1185 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/qwak_client/builds/filters/metric_filter.py
--rw-r--r--   0        0        0     1088 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/qwak_client/builds/filters/parameter_filter.py
--rw-r--r--   0        0        0    15535 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/qwak_client/client.py
--rw-r--r--   0        0        0        0 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/qwak_client/deployments/__init__.py
--rw-r--r--   0        0        0    13221 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/qwak_client/deployments/deployment.py
--rw-r--r--   0        0        0        0 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/qwak_client/models/__init__.py
--rw-r--r--   0        0        0     1921 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/qwak_client/models/model.py
--rw-r--r--   0        0        0      533 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/qwak_client/models/model_metadata.py
--rw-r--r--   0        0        0        0 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/qwak_client/projects/__init__.py
--rw-r--r--   0        0        0     2284 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/qwak_client/projects/project.py
--rw-r--r--   0        0        0        0 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/testing/__init__.py
--rw-r--r--   0        0        0      318 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak/testing/fixtures.py
--rw-r--r--   0        0        0       46 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak_services_mock/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak_services_mock/mocks/__init__.py
--rw-r--r--   0        0        0     2150 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak_services_mock/mocks/alert_manager_service_api.py
--rw-r--r--   0        0        0     2129 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak_services_mock/mocks/analytics_api.py
--rw-r--r--   0        0        0     2647 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak_services_mock/mocks/audience_service_api.py
--rw-r--r--   0        0        0     1067 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak_services_mock/mocks/authentication_service.py
--rw-r--r--   0        0        0     8211 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak_services_mock/mocks/automation_management_service.py
--rw-r--r--   0        0        0     1019 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak_services_mock/mocks/autoscaling_service_api.py
--rw-r--r--   0        0        0    12145 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak_services_mock/mocks/batch_job_manager_service.py
--rw-r--r--   0        0        0     3841 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak_services_mock/mocks/build_management.py
--rw-r--r--   0        0        0     3909 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak_services_mock/mocks/build_orchestrator_build_api.py
--rw-r--r--   0        0        0     4150 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak_services_mock/mocks/build_orchestrator_service_api.py
--rw-r--r--   0        0        0     1412 2023-04-24 06:21:26.055415 qwak_core-0.0.29/qwak_services_mock/mocks/data_versioning_service.py
--rw-r--r--   0        0        0    18268 2023-04-24 06:21:26.059414 qwak_core-0.0.29/qwak_services_mock/mocks/deployment_management_service.py
--rw-r--r--   0        0        0     1158 2023-04-24 06:21:26.059414 qwak_core-0.0.29/qwak_services_mock/mocks/ecosystem_service_api.py
--rw-r--r--   0        0        0     1536 2023-04-24 06:21:26.059414 qwak_core-0.0.29/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
--rw-r--r--   0        0        0     1782 2023-04-24 06:21:26.059414 qwak_core-0.0.29/qwak_services_mock/mocks/feature_store_entities_manager_api.py
--rw-r--r--   0        0        0     3261 2023-04-24 06:21:26.059414 qwak_core-0.0.29/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
--rw-r--r--   0        0        0     5776 2023-04-24 06:21:26.059414 qwak_core-0.0.29/qwak_services_mock/mocks/features_online_serving_api.py
--rw-r--r--   0        0        0     1001 2023-04-24 06:21:26.059414 qwak_core-0.0.29/qwak_services_mock/mocks/features_operator_v3_service.py
--rw-r--r--   0        0        0     2276 2023-04-24 06:21:26.059414 qwak_core-0.0.29/qwak_services_mock/mocks/features_set_state_service_api.py
--rw-r--r--   0        0        0     1127 2023-04-24 06:21:26.059414 qwak_core-0.0.29/qwak_services_mock/mocks/feedback_service.py
--rw-r--r--   0        0        0     1412 2023-04-24 06:21:26.059414 qwak_core-0.0.29/qwak_services_mock/mocks/file_versioning_service.py
--rw-r--r--   0        0        0     2696 2023-04-24 06:21:26.059414 qwak_core-0.0.29/qwak_services_mock/mocks/job_registry_service_api.py
--rw-r--r--   0        0        0     1583 2023-04-24 06:21:26.059414 qwak_core-0.0.29/qwak_services_mock/mocks/kube_captain_service_api.py
--rw-r--r--   0        0        0     7381 2023-04-24 06:21:26.059414 qwak_core-0.0.29/qwak_services_mock/mocks/logging_service.py
--rw-r--r--   0        0        0     3566 2023-04-24 06:21:26.059414 qwak_core-0.0.29/qwak_services_mock/mocks/model_management_service.py
--rw-r--r--   0        0        0     3090 2023-04-24 06:21:26.059414 qwak_core-0.0.29/qwak_services_mock/mocks/project_manager_service.py
--rw-r--r--   0        0        0     3995 2023-04-24 06:21:26.059414 qwak_core-0.0.29/qwak_services_mock/mocks/qwak_mocks.py
--rw-r--r--   0        0        0     1406 2023-04-24 06:21:26.059414 qwak_core-0.0.29/qwak_services_mock/mocks/secret_service.py
--rw-r--r--   0        0        0     1205 2023-04-24 06:21:26.059414 qwak_core-0.0.29/qwak_services_mock/mocks/self_service_user_service.py
--rw-r--r--   0        0        0     4083 2023-04-24 06:21:26.059414 qwak_core-0.0.29/qwak_services_mock/mocks/user_application_instance_service_api.py
--rw-r--r--   0        0        0        0 2023-04-24 06:21:26.059414 qwak_core-0.0.29/qwak_services_mock/mocks/utils/__init__.py
--rw-r--r--   0        0        0      159 2023-04-24 06:21:26.059414 qwak_core-0.0.29/qwak_services_mock/mocks/utils/exception_handlers.py
--rw-r--r--   0        0        0    13054 2023-04-24 06:21:26.059414 qwak_core-0.0.29/qwak_services_mock/services_mock.py
--rw-r--r--   0        0        0        0 2023-04-24 06:21:26.059414 qwak_core-0.0.29/qwak_services_mock/utils/__init__.py
--rw-r--r--   0        0        0      265 2023-04-24 06:21:26.059414 qwak_core-0.0.29/qwak_services_mock/utils/service_utils.py
--rw-r--r--   0        0        0     4507 1970-01-01 00:00:00.000000 qwak_core-0.0.29/setup.py
--rw-r--r--   0        0        0     1468 1970-01-01 00:00:00.000000 qwak_core-0.0.29/PKG-INFO
+-rw-r--r--   0        0        0      264 2023-04-24 08:15:15.378400 qwak_core-0.0.30/README.md
+-rw-r--r--   0        0        0        0 2023-04-24 08:16:15.570356 qwak_core-0.0.30/_qwak_proto/__init__.py
+-rw-r--r--   0        0        0     5378 2023-04-24 08:16:15.590356 qwak_core-0.0.30/_qwak_proto/qwak/administration/account/v1/account_pb2.py
+-rw-r--r--   0        0        0     6623 2023-04-24 08:16:01.190367 qwak_core-0.0.30/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.590356 qwak_core-0.0.30/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
+-rw-r--r--   0        0        0     2390 2023-04-24 08:16:15.586356 qwak_core-0.0.30/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
+-rw-r--r--   0        0        0     1475 2023-04-24 08:16:00.934367 qwak_core-0.0.30/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.586356 qwak_core-0.0.30/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     2106 2023-04-24 08:16:15.586356 qwak_core-0.0.30/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
+-rw-r--r--   0        0        0     1207 2023-04-24 08:16:01.062367 qwak_core-0.0.30/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.590356 qwak_core-0.0.30/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
+-rw-r--r--   0        0        0     6751 2023-04-24 08:16:15.582356 qwak_core-0.0.30/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
+-rw-r--r--   0        0        0     4346 2023-04-24 08:16:00.546367 qwak_core-0.0.30/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
+-rw-r--r--   0        0        0     7662 2023-04-24 08:16:15.582356 qwak_core-0.0.30/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-04-24 08:16:15.582356 qwak_core-0.0.30/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
+-rw-r--r--   0        0        0     2650 2023-04-24 08:16:00.678367 qwak_core-0.0.30/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.586356 qwak_core-0.0.30/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0     4864 2023-04-24 08:16:15.586356 qwak_core-0.0.30/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
+-rw-r--r--   0        0        0     5792 2023-04-24 08:16:00.806367 qwak_core-0.0.30/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.586356 qwak_core-0.0.30/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
+-rw-r--r--   0        0        0     4635 2023-04-24 08:16:15.574356 qwak_core-0.0.30/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
+-rw-r--r--   0        0        0     3664 2023-04-24 08:16:00.418367 qwak_core-0.0.30/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
+-rw-r--r--   0        0        0     3167 2023-04-24 08:16:15.574356 qwak_core-0.0.30/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5670 2023-04-24 08:16:15.574356 qwak_core-0.0.30/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
+-rw-r--r--   0        0        0     8035 2023-04-24 08:16:01.326367 qwak_core-0.0.30/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.574356 qwak_core-0.0.30/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     4512 2023-04-24 08:16:15.578356 qwak_core-0.0.30/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
+-rw-r--r--   0        0        0     5690 2023-04-24 08:16:01.586367 qwak_core-0.0.30/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.578356 qwak_core-0.0.30/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
+-rw-r--r--   0        0        0    16001 2023-04-24 08:16:15.578356 qwak_core-0.0.30/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
+-rw-r--r--   0        0        0    12387 2023-04-24 08:16:01.722366 qwak_core-0.0.30/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
+-rw-r--r--   0        0        0    16458 2023-04-24 08:16:15.578356 qwak_core-0.0.30/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2464 2023-04-24 08:16:15.574356 qwak_core-0.0.30/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
+-rw-r--r--   0        0        0     1347 2023-04-24 08:16:01.458366 qwak_core-0.0.30/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.578356 qwak_core-0.0.30/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     6425 2023-04-24 08:16:15.582356 qwak_core-0.0.30/_qwak_proto/qwak/administration/v0/users/user_pb2.py
+-rw-r--r--   0        0        0    10323 2023-04-24 08:16:01.850366 qwak_core-0.0.30/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.582356 qwak_core-0.0.30/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
+-rw-r--r--   0        0        0     9577 2023-04-24 08:16:15.610356 qwak_core-0.0.30/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
+-rw-r--r--   0        0        0    13624 2023-04-24 08:16:03.722365 qwak_core-0.0.30/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.610356 qwak_core-0.0.30/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
+-rw-r--r--   0        0        0     9270 2023-04-24 08:16:15.610356 qwak_core-0.0.30/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
+-rw-r--r--   0        0        0     5571 2023-04-24 08:16:03.862365 qwak_core-0.0.30/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
+-rw-r--r--   0        0        0    10742 2023-04-24 08:16:15.614356 qwak_core-0.0.30/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7365 2023-04-24 08:16:15.658356 qwak_core-0.0.30/_qwak_proto/qwak/analytics/analytics_pb2.py
+-rw-r--r--   0        0        0    11839 2023-04-24 08:16:07.478362 qwak_core-0.0.30/_qwak_proto/qwak/analytics/analytics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.658356 qwak_core-0.0.30/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
+-rw-r--r--   0        0        0     9396 2023-04-24 08:16:15.662356 qwak_core-0.0.30/_qwak_proto/qwak/analytics/analytics_service_pb2.py
+-rw-r--r--   0        0        0     7896 2023-04-24 08:16:07.606362 qwak_core-0.0.30/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
+-rw-r--r--   0        0        0    11917 2023-04-24 08:16:15.662356 qwak_core-0.0.30/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9021 2023-04-24 08:16:15.662356 qwak_core-0.0.30/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
+-rw-r--r--   0        0        0     5865 2023-04-24 08:16:08.266362 qwak_core-0.0.30/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
+-rw-r--r--   0        0        0    11486 2023-04-24 08:16:15.666356 qwak_core-0.0.30/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
+-rw-r--r--   0        0        0     8807 2023-04-24 08:16:15.662356 qwak_core-0.0.30/_qwak_proto/qwak/audience/v1/audience_pb2.py
+-rw-r--r--   0        0        0    13570 2023-04-24 08:16:08.134362 qwak_core-0.0.30/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.662356 qwak_core-0.0.30/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
+-rw-r--r--   0        0        0     5497 2023-04-24 08:16:15.666356 qwak_core-0.0.30/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     7820 2023-04-24 08:16:08.402361 qwak_core-0.0.30/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.666356 qwak_core-0.0.30/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     2937 2023-04-24 08:16:15.666356 qwak_core-0.0.30/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
+-rw-r--r--   0        0        0     2014 2023-04-24 08:16:08.542361 qwak_core-0.0.30/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
+-rw-r--r--   0        0        0     2991 2023-04-24 08:16:15.666356 qwak_core-0.0.30/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11441 2023-04-24 08:16:15.710356 qwak_core-0.0.30/_qwak_proto/qwak/automation/v1/action_pb2.py
+-rw-r--r--   0        0        0    17892 2023-04-24 08:16:12.286358 qwak_core-0.0.30/_qwak_proto/qwak/automation/v1/action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.710356 qwak_core-0.0.30/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
+-rw-r--r--   0        0        0     5494 2023-04-24 08:16:15.706356 qwak_core-0.0.30/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     7776 2023-04-24 08:16:12.026359 qwak_core-0.0.30/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.706356 qwak_core-0.0.30/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     3373 2023-04-24 08:16:15.706356 qwak_core-0.0.30/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
+-rw-r--r--   0        0        0     4400 2023-04-24 08:16:12.154359 qwak_core-0.0.30/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.710356 qwak_core-0.0.30/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
+-rw-r--r--   0        0        0    17887 2023-04-24 08:16:15.702356 qwak_core-0.0.30/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
+-rw-r--r--   0        0        0    12310 2023-04-24 08:16:11.766359 qwak_core-0.0.30/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
+-rw-r--r--   0        0        0    23338 2023-04-24 08:16:15.702356 qwak_core-0.0.30/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3873 2023-04-24 08:16:15.706356 qwak_core-0.0.30/_qwak_proto/qwak/automation/v1/automation_pb2.py
+-rw-r--r--   0        0        0     5291 2023-04-24 08:16:11.894359 qwak_core-0.0.30/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.706356 qwak_core-0.0.30/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
+-rw-r--r--   0        0        0     2383 2023-04-24 08:16:15.714356 qwak_core-0.0.30/_qwak_proto/qwak/automation/v1/common_pb2.py
+-rw-r--r--   0        0        0     2446 2023-04-24 08:16:12.674358 qwak_core-0.0.30/_qwak_proto/qwak/automation/v1/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.714356 qwak_core-0.0.30/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
+-rw-r--r--   0        0        0     5209 2023-04-24 08:16:15.710356 qwak_core-0.0.30/_qwak_proto/qwak/automation/v1/notification_pb2.py
+-rw-r--r--   0        0        0     5492 2023-04-24 08:16:12.546358 qwak_core-0.0.30/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.714356 qwak_core-0.0.30/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
+-rw-r--r--   0        0        0     3604 2023-04-24 08:16:15.710356 qwak_core-0.0.30/_qwak_proto/qwak/automation/v1/trigger_pb2.py
+-rw-r--r--   0        0        0     4212 2023-04-24 08:16:12.414358 qwak_core-0.0.30/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.710356 qwak_core-0.0.30/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
+-rw-r--r--   0        0        0    10275 2023-04-24 08:16:15.742356 qwak_core-0.0.30/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
+-rw-r--r--   0        0        0    14803 2023-04-24 08:16:15.118357 qwak_core-0.0.30/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.742356 qwak_core-0.0.30/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
+-rw-r--r--   0        0        0     2042 2023-04-24 08:16:15.738356 qwak_core-0.0.30/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
+-rw-r--r--   0        0        0     1904 2023-04-24 08:16:14.838357 qwak_core-0.0.30/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.738356 qwak_core-0.0.30/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
+-rw-r--r--   0        0        0    37419 2023-04-24 08:16:15.738356 qwak_core-0.0.30/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
+-rw-r--r--   0        0        0    48027 2023-04-24 08:16:14.982357 qwak_core-0.0.30/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
+-rw-r--r--   0        0        0    29918 2023-04-24 08:16:15.742356 qwak_core-0.0.30/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
+-rw-r--r--   0        0        0    18658 2023-04-24 08:16:15.686356 qwak_core-0.0.30/_qwak_proto/qwak/build/v1/build_api_pb2.py
+-rw-r--r--   0        0        0    15525 2023-04-24 08:16:09.898360 qwak_core-0.0.30/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
+-rw-r--r--   0        0        0    18652 2023-04-24 08:16:15.686356 qwak_core-0.0.30/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
+-rw-r--r--   0        0        0    16953 2023-04-24 08:16:15.682356 qwak_core-0.0.30/_qwak_proto/qwak/build/v1/build_pb2.py
+-rw-r--r--   0        0        0    25941 2023-04-24 08:16:09.762360 qwak_core-0.0.30/_qwak_proto/qwak/build/v1/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.686356 qwak_core-0.0.30/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
+-rw-r--r--   0        0        0    11034 2023-04-24 08:16:15.678356 qwak_core-0.0.30/_qwak_proto/qwak/builds/build_pb2.py
+-rw-r--r--   0        0        0    18276 2023-04-24 08:16:09.498361 qwak_core-0.0.30/_qwak_proto/qwak/builds/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.678356 qwak_core-0.0.30/_qwak_proto/qwak/builds/build_pb2_grpc.py
+-rw-r--r--   0        0        0     4777 2023-04-24 08:16:15.678356 qwak_core-0.0.30/_qwak_proto/qwak/builds/build_url_pb2.py
+-rw-r--r--   0        0        0     5773 2023-04-24 08:16:09.630360 qwak_core-0.0.30/_qwak_proto/qwak/builds/build_url_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.678356 qwak_core-0.0.30/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
+-rw-r--r--   0        0        0    12490 2023-04-24 08:16:15.682356 qwak_core-0.0.30/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
+-rw-r--r--   0        0        0     9351 2023-04-24 08:16:10.030360 qwak_core-0.0.30/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
+-rw-r--r--   0        0        0    14916 2023-04-24 08:16:15.682356 qwak_core-0.0.30/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
+-rw-r--r--   0        0        0    38245 2023-04-24 08:16:15.682356 qwak_core-0.0.30/_qwak_proto/qwak/builds/builds_pb2.py
+-rw-r--r--   0        0        0    52572 2023-04-24 08:16:10.318360 qwak_core-0.0.30/_qwak_proto/qwak/builds/builds_pb2.pyi
+-rw-r--r--   0        0        0    11572 2023-04-24 08:16:15.682356 qwak_core-0.0.30/_qwak_proto/qwak/builds/builds_pb2_grpc.py
+-rw-r--r--   0        0        0     1671 2023-04-24 08:16:15.690356 qwak_core-0.0.30/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
+-rw-r--r--   0        0        0     1689 2023-04-24 08:16:10.586360 qwak_core-0.0.30/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.690356 qwak_core-0.0.30/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4328 2023-04-24 08:16:15.690356 qwak_core-0.0.30/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-04-24 08:16:10.714360 qwak_core-0.0.30/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-04-24 08:16:15.690356 qwak_core-0.0.30/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7716 2023-04-24 08:16:15.674356 qwak_core-0.0.30/_qwak_proto/qwak/deployment/alert_pb2.py
+-rw-r--r--   0        0        0    11197 2023-04-24 08:16:09.102361 qwak_core-0.0.30/_qwak_proto/qwak/deployment/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.674356 qwak_core-0.0.30/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
+-rw-r--r--   0        0        0    11580 2023-04-24 08:16:15.674356 qwak_core-0.0.30/_qwak_proto/qwak/deployment/alert_service_pb2.py
+-rw-r--r--   0        0        0     7373 2023-04-24 08:16:09.234361 qwak_core-0.0.30/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
+-rw-r--r--   0        0        0    12803 2023-04-24 08:16:15.674356 qwak_core-0.0.30/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2162 2023-04-24 08:16:15.670356 qwak_core-0.0.30/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
+-rw-r--r--   0        0        0     2685 2023-04-24 08:16:08.822361 qwak_core-0.0.30/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.670356 qwak_core-0.0.30/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
+-rw-r--r--   0        0        0    42956 2023-04-24 08:16:15.670356 qwak_core-0.0.30/_qwak_proto/qwak/deployment/deployment_pb2.py
+-rw-r--r--   0        0        0    62847 2023-04-24 08:16:08.686361 qwak_core-0.0.30/_qwak_proto/qwak/deployment/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.670356 qwak_core-0.0.30/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    38320 2023-04-24 08:16:15.670356 qwak_core-0.0.30/_qwak_proto/qwak/deployment/deployment_service_pb2.py
+-rw-r--r--   0        0        0    33325 2023-04-24 08:16:08.970361 qwak_core-0.0.30/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
+-rw-r--r--   0        0        0    20242 2023-04-24 08:16:15.674356 qwak_core-0.0.30/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2527 2023-04-24 08:16:15.602356 qwak_core-0.0.30/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
+-rw-r--r--   0        0        0     2791 2023-04-24 08:16:03.050365 qwak_core-0.0.30/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.602356 qwak_core-0.0.30/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-04-24 08:16:15.606356 qwak_core-0.0.30/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
+-rw-r--r--   0        0        0    12641 2023-04-24 08:16:03.178365 qwak_core-0.0.30/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.606356 qwak_core-0.0.30/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
+-rw-r--r--   0        0        0    15709 2023-04-24 08:16:15.606356 qwak_core-0.0.30/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
+-rw-r--r--   0        0        0    16335 2023-04-24 08:16:03.318365 qwak_core-0.0.30/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
+-rw-r--r--   0        0        0    10706 2023-04-24 08:16:15.606356 qwak_core-0.0.30/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4787 2023-04-24 08:16:15.646356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
+-rw-r--r--   0        0        0     6713 2023-04-24 08:16:06.698363 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.646356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     9721 2023-04-24 08:16:15.646356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
+-rw-r--r--   0        0        0     7409 2023-04-24 08:16:06.566363 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
+-rw-r--r--   0        0        0    12256 2023-04-24 08:16:15.646356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9535 2023-04-24 08:16:15.634356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
+-rw-r--r--   0        0        0    10460 2023-04-24 08:16:05.506363 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.634356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
+-rw-r--r--   0        0        0     5268 2023-04-24 08:16:15.630356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/features/execution_pb2.py
+-rw-r--r--   0        0        0     8525 2023-04-24 08:16:05.378364 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.630356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
+-rw-r--r--   0        0        0    10074 2023-04-24 08:16:15.626356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
+-rw-r--r--   0        0        0    14303 2023-04-24 08:16:04.970364 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.626356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
+-rw-r--r--   0        0        0    27847 2023-04-24 08:16:15.630356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
+-rw-r--r--   0        0        0    20073 2023-04-24 08:16:05.246364 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
+-rw-r--r--   0        0        0    33080 2023-04-24 08:16:15.630356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12638 2023-04-24 08:16:15.634356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
+-rw-r--r--   0        0        0    14071 2023-04-24 08:16:05.638363 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.634356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
+-rw-r--r--   0        0        0    10044 2023-04-24 08:16:15.634356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
+-rw-r--r--   0        0        0     6846 2023-04-24 08:16:05.770363 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
+-rw-r--r--   0        0        0    11647 2023-04-24 08:16:15.634356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
+-rw-r--r--   0        0        0    24876 2023-04-24 08:16:15.626356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
+-rw-r--r--   0        0        0    36861 2023-04-24 08:16:05.106364 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.630356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
+-rw-r--r--   0        0        0     2872 2023-04-24 08:16:15.638356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
+-rw-r--r--   0        0        0     2428 2023-04-24 08:16:05.898363 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.638356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
+-rw-r--r--   0        0        0     4196 2023-04-24 08:16:15.646356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
+-rw-r--r--   0        0        0     7323 2023-04-24 08:16:15.250357 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.650356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
+-rw-r--r--   0        0        0     9895 2023-04-24 08:16:15.650356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
+-rw-r--r--   0        0        0     9029 2023-04-24 08:16:15.382356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
+-rw-r--r--   0        0        0    12090 2023-04-24 08:16:15.650356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3596 2023-04-24 08:16:15.650356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
+-rw-r--r--   0        0        0     6664 2023-04-24 08:16:07.086362 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.650356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
+-rw-r--r--   0        0        0    11930 2023-04-24 08:16:15.650356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
+-rw-r--r--   0        0        0    11052 2023-04-24 08:16:07.218362 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
+-rw-r--r--   0        0        0    14459 2023-04-24 08:16:15.654356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5158 2023-04-24 08:16:15.654356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/reports/report_pb2.py
+-rw-r--r--   0        0        0     7436 2023-04-24 08:16:07.346362 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.654356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
+-rw-r--r--   0        0        0     4549 2023-04-24 08:16:15.658356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
+-rw-r--r--   0        0        0     6442 2023-04-24 08:16:07.870362 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.658356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
+-rw-r--r--   0        0        0    16693 2023-04-24 08:16:15.654356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
+-rw-r--r--   0        0        0    20355 2023-04-24 08:16:07.738362 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
+-rw-r--r--   0        0        0     4809 2023-04-24 08:16:15.654356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
+-rw-r--r--   0        0        0     2553 2023-04-24 08:16:15.658356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
+-rw-r--r--   0        0        0     4000 2023-04-24 08:16:07.998362 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.658356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
+-rw-r--r--   0        0        0    13329 2023-04-24 08:16:15.638356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
+-rw-r--r--   0        0        0    23039 2023-04-24 08:16:06.038363 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.638356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
+-rw-r--r--   0        0        0     5087 2023-04-24 08:16:15.638356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
+-rw-r--r--   0        0        0     6011 2023-04-24 08:16:06.170363 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.642356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
+-rw-r--r--   0        0        0    12309 2023-04-24 08:16:15.642356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
+-rw-r--r--   0        0        0     9244 2023-04-24 08:16:06.302363 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
+-rw-r--r--   0        0        0    17071 2023-04-24 08:16:15.642356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11014 2023-04-24 08:16:15.642356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
+-rw-r--r--   0        0        0    15865 2023-04-24 08:16:06.434363 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.642356 qwak_core-0.0.30/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
+-rw-r--r--   0        0        0     4727 2023-04-24 08:16:15.714356 qwak_core-0.0.30/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
+-rw-r--r--   0        0        0     5122 2023-04-24 08:16:12.810358 qwak_core-0.0.30/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.714356 qwak_core-0.0.30/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4648 2023-04-24 08:16:15.718356 qwak_core-0.0.30/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4170 2023-04-24 08:16:12.950358 qwak_core-0.0.30/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-04-24 08:16:15.718356 qwak_core-0.0.30/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5349 2023-04-24 08:16:15.718356 qwak_core-0.0.30/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
+-rw-r--r--   0        0        0     5363 2023-04-24 08:16:13.082358 qwak_core-0.0.30/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.718356 qwak_core-0.0.30/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4437 2023-04-24 08:16:15.718356 qwak_core-0.0.30/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4127 2023-04-24 08:16:13.222358 qwak_core-0.0.30/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-04-24 08:16:15.722356 qwak_core-0.0.30/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6073 2023-04-24 08:16:15.722356 qwak_core-0.0.30/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
+-rw-r--r--   0        0        0     5366 2023-04-24 08:16:13.366358 qwak_core-0.0.30/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
+-rw-r--r--   0        0        0     7395 2023-04-24 08:16:15.722356 qwak_core-0.0.30/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4636 2023-04-24 08:16:15.722356 qwak_core-0.0.30/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
+-rw-r--r--   0        0        0     4239 2023-04-24 08:16:13.498358 qwak_core-0.0.30/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.722356 qwak_core-0.0.30/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     2376 2023-04-24 08:16:15.694356 qwak_core-0.0.30/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
+-rw-r--r--   0        0        0     3018 2023-04-24 08:16:10.842360 qwak_core-0.0.30/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.694356 qwak_core-0.0.30/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4325 2023-04-24 08:16:15.694356 qwak_core-0.0.30/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-04-24 08:16:10.970359 qwak_core-0.0.30/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-04-24 08:16:15.694356 qwak_core-0.0.30/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6401 2023-04-24 08:16:15.614356 qwak_core-0.0.30/_qwak_proto/qwak/fitness_service/constructs_pb2.py
+-rw-r--r--   0        0        0    10192 2023-04-24 08:16:04.394364 qwak_core-0.0.30/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.618356 qwak_core-0.0.30/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-04-24 08:16:15.618356 qwak_core-0.0.30/_qwak_proto/qwak/fitness_service/fitness_pb2.py
+-rw-r--r--   0        0        0     4115 2023-04-24 08:16:04.530364 qwak_core-0.0.30/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.618356 qwak_core-0.0.30/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
+-rw-r--r--   0        0        0     7123 2023-04-24 08:16:15.622356 qwak_core-0.0.30/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
+-rw-r--r--   0        0        0     3981 2023-04-24 08:16:04.662364 qwak_core-0.0.30/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
+-rw-r--r--   0        0        0     8546 2023-04-24 08:16:15.622356 qwak_core-0.0.30/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8428 2023-04-24 08:16:15.622356 qwak_core-0.0.30/_qwak_proto/qwak/fitness_service/status_pb2.py
+-rw-r--r--   0        0        0    12205 2023-04-24 08:16:04.830364 qwak_core-0.0.30/_qwak_proto/qwak/fitness_service/status_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.626356 qwak_core-0.0.30/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
+-rw-r--r--   0        0        0     8196 2023-04-24 08:16:15.674356 qwak_core-0.0.30/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
+-rw-r--r--   0        0        0    10867 2023-04-24 08:16:09.366361 qwak_core-0.0.30/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
+-rw-r--r--   0        0        0     4700 2023-04-24 08:16:15.678356 qwak_core-0.0.30/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
+-rw-r--r--   0        0        0     7803 2023-04-24 08:16:15.722356 qwak_core-0.0.30/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
+-rw-r--r--   0        0        0    10487 2023-04-24 08:16:13.630358 qwak_core-0.0.30/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.726356 qwak_core-0.0.30/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
+-rw-r--r--   0        0        0     3704 2023-04-24 08:16:15.726356 qwak_core-0.0.30/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
+-rw-r--r--   0        0        0     3759 2023-04-24 08:16:13.758357 qwak_core-0.0.30/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.726356 qwak_core-0.0.30/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
+-rw-r--r--   0        0        0    22089 2023-04-24 08:16:15.726356 qwak_core-0.0.30/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
+-rw-r--r--   0        0        0    25879 2023-04-24 08:16:13.902357 qwak_core-0.0.30/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.726356 qwak_core-0.0.30/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
+-rw-r--r--   0        0        0    13157 2023-04-24 08:16:15.730356 qwak_core-0.0.30/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
+-rw-r--r--   0        0        0    21705 2023-04-24 08:16:14.038357 qwak_core-0.0.30/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.730356 qwak_core-0.0.30/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-04-24 08:16:15.730356 qwak_core-0.0.30/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
+-rw-r--r--   0        0        0    16128 2023-04-24 08:16:14.174357 qwak_core-0.0.30/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.730356 qwak_core-0.0.30/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    45273 2023-04-24 08:16:15.730356 qwak_core-0.0.30/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
+-rw-r--r--   0        0        0    35031 2023-04-24 08:16:14.314357 qwak_core-0.0.30/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
+-rw-r--r--   0        0        0    67567 2023-04-24 08:16:15.734356 qwak_core-0.0.30/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2023-04-24 08:16:15.734356 qwak_core-0.0.30/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
+-rw-r--r--   0        0        0     2637 2023-04-24 08:16:14.446357 qwak_core-0.0.30/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.734356 qwak_core-0.0.30/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
+-rw-r--r--   0        0        0     3459 2023-04-24 08:16:15.698356 qwak_core-0.0.30/_qwak_proto/qwak/logging/log_filter_pb2.py
+-rw-r--r--   0        0        0     4169 2023-04-24 08:16:11.238359 qwak_core-0.0.30/_qwak_proto/qwak/logging/log_filter_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.698356 qwak_core-0.0.30/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
+-rw-r--r--   0        0        0     2233 2023-04-24 08:16:15.702356 qwak_core-0.0.30/_qwak_proto/qwak/logging/log_line_pb2.py
+-rw-r--r--   0        0        0     2135 2023-04-24 08:16:11.630359 qwak_core-0.0.30/_qwak_proto/qwak/logging/log_line_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.702356 qwak_core-0.0.30/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
+-rw-r--r--   0        0        0     3126 2023-04-24 08:16:15.698356 qwak_core-0.0.30/_qwak_proto/qwak/logging/log_reader_service_pb2.py
+-rw-r--r--   0        0        0     3479 2023-04-24 08:16:11.370359 qwak_core-0.0.30/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
+-rw-r--r--   0        0        0     2831 2023-04-24 08:16:15.698356 qwak_core-0.0.30/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9322 2023-04-24 08:16:15.698356 qwak_core-0.0.30/_qwak_proto/qwak/logging/log_source_pb2.py
+-rw-r--r--   0        0        0    13291 2023-04-24 08:16:11.498359 qwak_core-0.0.30/_qwak_proto/qwak/logging/log_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.702356 qwak_core-0.0.30/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
+-rw-r--r--   0        0        0    22744 2023-04-24 08:16:15.690356 qwak_core-0.0.30/_qwak_proto/qwak/models/models_pb2.py
+-rw-r--r--   0        0        0    27142 2023-04-24 08:16:10.458360 qwak_core-0.0.30/_qwak_proto/qwak/models/models_pb2.pyi
+-rw-r--r--   0        0        0    14733 2023-04-24 08:16:15.690356 qwak_core-0.0.30/_qwak_proto/qwak/models/models_pb2_grpc.py
+-rw-r--r--   0        0        0    10745 2023-04-24 08:16:15.602356 qwak_core-0.0.30/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
+-rw-r--r--   0        0        0     6790 2023-04-24 08:16:04.130365 qwak_core-0.0.30/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
+-rw-r--r--   0        0        0    13657 2023-04-24 08:16:15.602356 qwak_core-0.0.30/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11564 2023-04-24 08:16:15.598356 qwak_core-0.0.30/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
+-rw-r--r--   0        0        0    14927 2023-04-24 08:16:03.998365 qwak_core-0.0.30/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.598356 qwak_core-0.0.30/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
+-rw-r--r--   0        0        0     5283 2023-04-24 08:16:15.602356 qwak_core-0.0.30/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
+-rw-r--r--   0        0        0     3745 2023-04-24 08:16:04.262364 qwak_core-0.0.30/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
+-rw-r--r--   0        0        0     5551 2023-04-24 08:16:15.602356 qwak_core-0.0.30/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8701 2023-04-24 08:16:15.686356 qwak_core-0.0.30/_qwak_proto/qwak/projects/projects_pb2.py
+-rw-r--r--   0        0        0     9794 2023-04-24 08:16:10.170360 qwak_core-0.0.30/_qwak_proto/qwak/projects/projects_pb2.pyi
+-rw-r--r--   0        0        0     7931 2023-04-24 08:16:15.686356 qwak_core-0.0.30/_qwak_proto/qwak/projects/projects_pb2_grpc.py
+-rw-r--r--   0        0        0     4752 2023-04-24 08:16:15.694356 qwak_core-0.0.30/_qwak_proto/qwak/secret_service/secret_service_pb2.py
+-rw-r--r--   0        0        0     2818 2023-04-24 08:16:11.106359 qwak_core-0.0.30/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
+-rw-r--r--   0        0        0     6253 2023-04-24 08:16:15.698356 qwak_core-0.0.30/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6225 2023-04-24 08:16:15.598356 qwak_core-0.0.30/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
+-rw-r--r--   0        0        0     7267 2023-04-24 08:16:02.534366 qwak_core-0.0.30/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.598356 qwak_core-0.0.30/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
+-rw-r--r--   0        0        0    16176 2023-04-24 08:16:15.594356 qwak_core-0.0.30/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
+-rw-r--r--   0        0        0    10166 2023-04-24 08:16:02.402366 qwak_core-0.0.30/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
+-rw-r--r--   0        0        0    19988 2023-04-24 08:16:15.598356 qwak_core-0.0.30/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1751 2023-04-24 08:16:15.590356 qwak_core-0.0.30/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
+-rw-r--r--   0        0        0      777 2023-04-24 08:16:01.978366 qwak_core-0.0.30/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.590356 qwak_core-0.0.30/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2023-04-24 08:16:15.594356 qwak_core-0.0.30/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
+-rw-r--r--   0        0        0     2129 2023-04-24 08:16:02.106366 qwak_core-0.0.30/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.594356 qwak_core-0.0.30/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
+-rw-r--r--   0        0        0    10389 2023-04-24 08:16:15.594356 qwak_core-0.0.30/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
+-rw-r--r--   0        0        0     8148 2023-04-24 08:16:02.238366 qwak_core-0.0.30/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
+-rw-r--r--   0        0        0    10512 2023-04-24 08:16:15.594356 qwak_core-0.0.30/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6843 2023-04-24 08:16:15.738356 qwak_core-0.0.30/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
+-rw-r--r--   0        0        0     4585 2023-04-24 08:16:14.706357 qwak_core-0.0.30/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
+-rw-r--r--   0        0        0     8228 2023-04-24 08:16:15.738356 qwak_core-0.0.30/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
+-rw-r--r--   0        0        0     7816 2023-04-24 08:16:15.734356 qwak_core-0.0.30/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
+-rw-r--r--   0        0        0    11958 2023-04-24 08:16:14.578357 qwak_core-0.0.30/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.734356 qwak_core-0.0.30/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
+-rw-r--r--   0        0        0     4083 2023-04-24 08:16:15.606356 qwak_core-0.0.30/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
+-rw-r--r--   0        0        0     4036 2023-04-24 08:16:03.454365 qwak_core-0.0.30/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.610356 qwak_core-0.0.30/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
+-rw-r--r--   0        0        0     3001 2023-04-24 08:16:15.610356 qwak_core-0.0.30/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
+-rw-r--r--   0        0        0     2574 2023-04-24 08:16:03.586365 qwak_core-0.0.30/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-04-24 08:16:15.610356 qwak_core-0.0.30/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
+-rw-r--r--   0        0        0     1906 2023-04-24 08:16:16.854355 qwak_core-0.0.30/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-04-24 08:16:16.854355 qwak_core-0.0.30/qwak/__init__.py
+-rw-r--r--   0        0        0     1204 2023-04-24 08:15:15.378400 qwak_core-0.0.30/qwak/automations/__init__.py
+-rw-r--r--   0        0        0     3132 2023-04-24 08:15:15.378400 qwak_core-0.0.30/qwak/automations/automation_executions.py
+-rw-r--r--   0        0        0    32139 2023-04-24 08:15:15.378400 qwak_core-0.0.30/qwak/automations/automations.py
+-rw-r--r--   0        0        0        0 2023-04-24 08:15:15.378400 qwak_core-0.0.30/qwak/clients/__init__.py
+-rw-r--r--   0        0        0      224 2023-04-24 08:15:15.378400 qwak_core-0.0.30/qwak/clients/administration/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 08:15:15.378400 qwak_core-0.0.30/qwak/clients/administration/authenticated_user/__init__.py
+-rw-r--r--   0        0        0     1456 2023-04-24 08:15:15.378400 qwak_core-0.0.30/qwak/clients/administration/authenticated_user/client.py
+-rw-r--r--   0        0        0        0 2023-04-24 08:15:15.378400 qwak_core-0.0.30/qwak/clients/administration/authentication/__init__.py
+-rw-r--r--   0        0        0     1076 2023-04-24 08:15:15.378400 qwak_core-0.0.30/qwak/clients/administration/authentication/client.py
+-rw-r--r--   0        0        0        0 2023-04-24 08:15:15.378400 qwak_core-0.0.30/qwak/clients/administration/eco_system/__init__.py
+-rw-r--r--   0        0        0     5478 2023-04-24 08:15:15.378400 qwak_core-0.0.30/qwak/clients/administration/eco_system/client.py
+-rw-r--r--   0        0        0        0 2023-04-24 08:15:15.378400 qwak_core-0.0.30/qwak/clients/administration/environment/__init__.py
+-rw-r--r--   0        0        0     2704 2023-04-24 08:15:15.378400 qwak_core-0.0.30/qwak/clients/administration/environment/client.py
+-rw-r--r--   0        0        0        0 2023-04-24 08:15:15.378400 qwak_core-0.0.30/qwak/clients/administration/self_service/__init__.py
+-rw-r--r--   0        0        0     2602 2023-04-24 08:15:15.378400 qwak_core-0.0.30/qwak/clients/administration/self_service/client.py
+-rw-r--r--   0        0        0       43 2023-04-24 08:15:15.378400 qwak_core-0.0.30/qwak/clients/alert_management/__init__.py
+-rw-r--r--   0        0        0     2226 2023-04-24 08:15:15.378400 qwak_core-0.0.30/qwak/clients/alert_management/client.py
+-rw-r--r--   0        0        0       42 2023-04-24 08:15:15.378400 qwak_core-0.0.30/qwak/clients/analytics/__init__.py
+-rw-r--r--   0        0        0     3093 2023-04-24 08:15:15.378400 qwak_core-0.0.30/qwak/clients/analytics/client.py
+-rw-r--r--   0        0        0       35 2023-04-24 08:15:15.378400 qwak_core-0.0.30/qwak/clients/audience/__init__.py
+-rw-r--r--   0        0        0     2110 2023-04-24 08:15:15.378400 qwak_core-0.0.30/qwak/clients/audience/client.py
+-rw-r--r--   0        0        0        0 2023-04-24 08:15:15.378400 qwak_core-0.0.30/qwak/clients/automation_management/__init__.py
+-rw-r--r--   0        0        0     8836 2023-04-24 08:15:15.378400 qwak_core-0.0.30/qwak/clients/automation_management/client.py
+-rw-r--r--   0        0        0       38 2023-04-24 08:15:15.378400 qwak_core-0.0.30/qwak/clients/autoscaling/__init__.py
+-rw-r--r--   0        0        0     1240 2023-04-24 08:15:15.378400 qwak_core-0.0.30/qwak/clients/autoscaling/client.py
+-rw-r--r--   0        0        0       77 2023-04-24 08:15:15.378400 qwak_core-0.0.30/qwak/clients/batch_job_management/__init__.py
+-rw-r--r--   0        0        0    17275 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/clients/batch_job_management/client.py
+-rw-r--r--   0        0        0     6242 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/clients/batch_job_management/executions_config.py
+-rw-r--r--   0        0        0     1846 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/clients/batch_job_management/results.py
+-rw-r--r--   0        0        0       43 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/clients/build_management/__init__.py
+-rw-r--r--   0        0        0     4731 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/clients/build_management/client.py
+-rw-r--r--   0        0        0       44 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/clients/build_orchestrator/__init__.py
+-rw-r--r--   0        0        0    14950 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/clients/build_orchestrator/client.py
+-rw-r--r--   0        0        0        0 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/clients/data_versioning/__init__.py
+-rw-r--r--   0        0        0     1835 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/clients/data_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/clients/deployment/__init__.py
+-rw-r--r--   0        0        0     6269 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/clients/deployment/client.py
+-rw-r--r--   0        0        0       53 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/clients/feature_store/__init__.py
+-rw-r--r--   0        0        0     2635 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/clients/feature_store/job_registry_client.py
+-rw-r--r--   0        0        0    15898 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/clients/feature_store/management_client.py
+-rw-r--r--   0        0        0     4963 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/clients/feature_store/operator_client.py
+-rw-r--r--   0        0        0        0 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/clients/file_versioning/__init__.py
+-rw-r--r--   0        0        0     1939 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/clients/file_versioning/client.py
+-rw-r--r--   0        0        0       41 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/clients/kube_deployment_captain/__init__.py
+-rw-r--r--   0        0        0     9276 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/clients/kube_deployment_captain/client.py
+-rw-r--r--   0        0        0       34 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/clients/logging_client/__init__.py
+-rw-r--r--   0        0        0     4255 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/clients/logging_client/client.py
+-rw-r--r--   0        0        0       43 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/clients/model_management/__init__.py
+-rw-r--r--   0        0        0     3695 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/clients/model_management/client.py
+-rw-r--r--   0        0        0        0 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/clients/project/__init__.py
+-rw-r--r--   0        0        0     2128 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/clients/project/client.py
+-rw-r--r--   0        0        0       40 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/clients/secret_service/__init__.py
+-rw-r--r--   0        0        0     2585 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/clients/secret_service/client.py
+-rw-r--r--   0        0        0       50 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/clients/user_application_instance/__init__.py
+-rw-r--r--   0        0        0     6013 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/clients/user_application_instance/client.py
+-rw-r--r--   0        0        0      380 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/exceptions/__init__.py
+-rw-r--r--   0        0        0      559 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/exceptions/quiet_error.py
+-rw-r--r--   0        0        0      469 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/exceptions/qwak_build_exception.py
+-rw-r--r--   0        0        0      135 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/exceptions/qwak_exception.py
+-rw-r--r--   0        0        0      579 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/exceptions/qwak_http_exception.py
+-rw-r--r--   0        0        0      100 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/exceptions/qwak_inference_exception.py
+-rw-r--r--   0        0        0      274 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/exceptions/qwak_load_model_failed_exception.py
+-rw-r--r--   0        0        0      211 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/exceptions/qwak_login_exception.py
+-rw-r--r--   0        0        0      152 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/exceptions/qwak_mock_http_exception.py
+-rw-r--r--   0        0        0      153 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/exceptions/qwak_model_initialization_exception.py
+-rw-r--r--   0        0        0      152 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/exceptions/qwak_not_found_exception.py
+-rw-r--r--   0        0        0      356 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/exceptions/qwak_quiet_build_exception.py
+-rw-r--r--   0        0        0        0 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/feature_store/__init__.py
+-rw-r--r--   0        0        0     1201 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/feature_store/data_sources/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/feature_store/data_sources/batch_sources/__init__.py
+-rw-r--r--   0        0        0     2108 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/feature_store/data_sources/batch_sources/_batch.py
+-rw-r--r--   0        0        0      666 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/feature_store/data_sources/batch_sources/_jdbc.py
+-rw-r--r--   0        0        0     3059 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/feature_store/data_sources/batch_sources/big_query.py
+-rw-r--r--   0        0        0     2006 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/feature_store/data_sources/batch_sources/csv.py
+-rw-r--r--   0        0        0     2167 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/feature_store/data_sources/batch_sources/elastic_search.py
+-rw-r--r--   0        0        0     2961 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
+-rw-r--r--   0        0        0     1930 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/feature_store/data_sources/batch_sources/mongodb.py
+-rw-r--r--   0        0        0     1669 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/feature_store/data_sources/batch_sources/mysql.py
+-rw-r--r--   0        0        0     1730 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/feature_store/data_sources/batch_sources/parquet.py
+-rw-r--r--   0        0        0     1722 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/feature_store/data_sources/batch_sources/postgres.py
+-rw-r--r--   0        0        0     3216 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/feature_store/data_sources/batch_sources/redshift.py
+-rw-r--r--   0        0        0     2616 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/feature_store/data_sources/batch_sources/snowflake.py
+-rw-r--r--   0        0        0     1839 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/feature_store/data_sources/batch_sources/vertica.py
+-rw-r--r--   0        0        0        0 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/feature_store/entities/__init__.py
+-rw-r--r--   0        0        0     1794 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/feature_store/entities/entity.py
+-rw-r--r--   0        0        0        0 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/feature_store/feature_sets/__init__.py
+-rw-r--r--   0        0        0     1547 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/feature_store/feature_sets/backfill.py
+-rw-r--r--   0        0        0    17012 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/feature_store/feature_sets/batch.py
+-rw-r--r--   0        0        0      263 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/feature_store/feature_sets/context.py
+-rw-r--r--   0        0        0     1630 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/feature_store/feature_sets/execution_spec.py
+-rw-r--r--   0        0        0      584 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/feature_store/feature_sets/metadata.py
+-rw-r--r--   0        0        0     6820 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/feature_store/feature_sets/read_policies.py
+-rw-r--r--   0        0        0     1554 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/feature_store/feature_sets/transformations.py
+-rw-r--r--   0        0        0        0 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/feature_store/online/__init__.py
+-rw-r--r--   0        0        0     8808 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/feature_store/online/client.py
+-rw-r--r--   0        0        0      226 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/inner/__init__.py
+-rw-r--r--   0        0        0      954 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/inner/const.py
+-rw-r--r--   0        0        0     1377 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/inner/di_configuration/__init__.py
+-rw-r--r--   0        0        0     5933 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/inner/di_configuration/account.py
+-rw-r--r--   0        0        0       73 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/inner/di_configuration/config.yml
+-rw-r--r--   0        0        0      621 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/inner/di_configuration/containers.py
+-rw-r--r--   0        0        0      344 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/inner/di_configuration/session.py
+-rw-r--r--   0        0        0     2336 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/inner/model_loggers_utils.py
+-rw-r--r--   0        0        0      266 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/inner/runtime_di/__init__.py
+-rw-r--r--   0        0        0      349 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/inner/runtime_di/containers.py
+-rw-r--r--   0        0        0      627 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/inner/singleton_meta.py
+-rw-r--r--   0        0        0       74 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/inner/tool/__init__.py
+-rw-r--r--   0        0        0     3414 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/inner/tool/auth.py
+-rw-r--r--   0        0        0        0 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/inner/tool/grpc/__init__.py
+-rw-r--r--   0        0        0      560 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/inner/tool/grpc/grpc_auth.py
+-rw-r--r--   0        0        0     5804 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/inner/tool/grpc/grpc_tools.py
+-rw-r--r--   0        0        0      473 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/inner/tool/grpc/grpc_try_wrapping.py
+-rw-r--r--   0        0        0      435 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/inner/tool/retry_utils.py
+-rw-r--r--   0        0        0      218 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/inner/tool/run_config/__init__.py
+-rw-r--r--   0        0        0     3148 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/inner/tool/run_config/base.py
+-rw-r--r--   0        0        0     6071 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/inner/tool/run_config/utils.py
+-rw-r--r--   0        0        0        0 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/model/__init__.py
+-rw-r--r--   0        0        0     1739 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/model/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/model/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      198 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/model/adapters/input_adapters/base_input_adapter.py
+-rw-r--r--   0        0        0      210 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/model/adapters/input_adapters/file_input_adapter.py
+-rw-r--r--   0        0        0      206 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/model/adapters/input_adapters/image_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/model/adapters/input_adapters/json_input_adapter.py
+-rw-r--r--   0        0        0     2175 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/model/adapters/input_adapters/multi_input_adapter.py
+-rw-r--r--   0        0        0     3208 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/model/adapters/input_adapters/numpy_input_adapter.py
+-rw-r--r--   0        0        0      862 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/model/adapters/input_adapters/proto_input_adapter.py
+-rw-r--r--   0        0        0      207 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/model/adapters/input_adapters/string_input_adapter.py
+-rw-r--r--   0        0        0      209 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
+-rw-r--r--   0        0        0        0 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/model/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      315 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/model/adapters/output_adapters/base_output_adapter.py
+-rw-r--r--   0        0        0      221 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
+-rw-r--r--   0        0        0      219 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/model/adapters/output_adapters/default_output_adapter.py
+-rw-r--r--   0        0        0      216 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/model/adapters/output_adapters/json_output_adapter.py
+-rw-r--r--   0        0        0     1065 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/model/adapters/output_adapters/numpy_output_adapter.py
+-rw-r--r--   0        0        0      517 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/model/adapters/output_adapters/proto_output_adapter.py
+-rw-r--r--   0        0        0      115 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
+-rw-r--r--   0        0        0      220 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
+-rw-r--r--   0        0        0      303 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/model/analytics_logging.py
+-rw-r--r--   0        0        0     2865 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/model/base.py
+-rw-r--r--   0        0        0        0 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/model/decorators/__init__.py
+-rw-r--r--   0        0        0     1288 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/model/decorators/api.py
+-rw-r--r--   0        0        0      861 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/model/decorators/api_implementation.py
+-rw-r--r--   0        0        0     1503 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/model/experiment_tracking.py
+-rw-r--r--   0        0        0      726 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/model/schema.py
+-rw-r--r--   0        0        0     2964 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/model/schema_entities.py
+-rw-r--r--   0        0        0        0 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/model/utils/__init__.py
+-rw-r--r--   0        0        0      320 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/model/utils/extract_wrapped_function.py
+-rw-r--r--   0        0        0        0 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/model_loggers/__init__.py
+-rw-r--r--   0        0        0     2701 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/model_loggers/artifact_logger.py
+-rw-r--r--   0        0        0     5186 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/model_loggers/data_logger.py
+-rw-r--r--   0        0        0      852 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/model_loggers/model_logger.py
+-rw-r--r--   0        0        0        0 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/qwak_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/qwak_client/builds/__init__.py
+-rw-r--r--   0        0        0     3698 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/qwak_client/builds/build.py
+-rw-r--r--   0        0        0        0 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/qwak_client/builds/filters/__init__.py
+-rw-r--r--   0        0        0     1185 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/qwak_client/builds/filters/metric_filter.py
+-rw-r--r--   0        0        0     1088 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/qwak_client/builds/filters/parameter_filter.py
+-rw-r--r--   0        0        0    15535 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/qwak_client/client.py
+-rw-r--r--   0        0        0        0 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/qwak_client/deployments/__init__.py
+-rw-r--r--   0        0        0    13221 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/qwak_client/deployments/deployment.py
+-rw-r--r--   0        0        0        0 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/qwak_client/models/__init__.py
+-rw-r--r--   0        0        0     1921 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/qwak_client/models/model.py
+-rw-r--r--   0        0        0      533 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/qwak_client/models/model_metadata.py
+-rw-r--r--   0        0        0        0 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/qwak_client/projects/__init__.py
+-rw-r--r--   0        0        0     2284 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/qwak_client/projects/project.py
+-rw-r--r--   0        0        0        0 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/testing/__init__.py
+-rw-r--r--   0        0        0      318 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak/testing/fixtures.py
+-rw-r--r--   0        0        0       46 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak_services_mock/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak_services_mock/mocks/__init__.py
+-rw-r--r--   0        0        0     2150 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak_services_mock/mocks/alert_manager_service_api.py
+-rw-r--r--   0        0        0     2129 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak_services_mock/mocks/analytics_api.py
+-rw-r--r--   0        0        0     2647 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak_services_mock/mocks/audience_service_api.py
+-rw-r--r--   0        0        0     1067 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak_services_mock/mocks/authentication_service.py
+-rw-r--r--   0        0        0     8211 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak_services_mock/mocks/automation_management_service.py
+-rw-r--r--   0        0        0     1019 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak_services_mock/mocks/autoscaling_service_api.py
+-rw-r--r--   0        0        0    12145 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak_services_mock/mocks/batch_job_manager_service.py
+-rw-r--r--   0        0        0     3841 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak_services_mock/mocks/build_management.py
+-rw-r--r--   0        0        0     3909 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak_services_mock/mocks/build_orchestrator_build_api.py
+-rw-r--r--   0        0        0     4150 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak_services_mock/mocks/build_orchestrator_service_api.py
+-rw-r--r--   0        0        0     1412 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak_services_mock/mocks/data_versioning_service.py
+-rw-r--r--   0        0        0    18268 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak_services_mock/mocks/deployment_management_service.py
+-rw-r--r--   0        0        0     1158 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak_services_mock/mocks/ecosystem_service_api.py
+-rw-r--r--   0        0        0     1536 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
+-rw-r--r--   0        0        0     1782 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak_services_mock/mocks/feature_store_entities_manager_api.py
+-rw-r--r--   0        0        0     3261 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
+-rw-r--r--   0        0        0     5776 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak_services_mock/mocks/features_online_serving_api.py
+-rw-r--r--   0        0        0     1001 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak_services_mock/mocks/features_operator_v3_service.py
+-rw-r--r--   0        0        0     2276 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak_services_mock/mocks/features_set_state_service_api.py
+-rw-r--r--   0        0        0     1127 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak_services_mock/mocks/feedback_service.py
+-rw-r--r--   0        0        0     1412 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak_services_mock/mocks/file_versioning_service.py
+-rw-r--r--   0        0        0     2696 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak_services_mock/mocks/job_registry_service_api.py
+-rw-r--r--   0        0        0     1583 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak_services_mock/mocks/kube_captain_service_api.py
+-rw-r--r--   0        0        0     7381 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak_services_mock/mocks/logging_service.py
+-rw-r--r--   0        0        0     3566 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak_services_mock/mocks/model_management_service.py
+-rw-r--r--   0        0        0     3090 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak_services_mock/mocks/project_manager_service.py
+-rw-r--r--   0        0        0     3995 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak_services_mock/mocks/qwak_mocks.py
+-rw-r--r--   0        0        0     1406 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak_services_mock/mocks/secret_service.py
+-rw-r--r--   0        0        0     1205 2023-04-24 08:15:15.382400 qwak_core-0.0.30/qwak_services_mock/mocks/self_service_user_service.py
+-rw-r--r--   0        0        0     4083 2023-04-24 08:15:15.386400 qwak_core-0.0.30/qwak_services_mock/mocks/user_application_instance_service_api.py
+-rw-r--r--   0        0        0        0 2023-04-24 08:15:15.386400 qwak_core-0.0.30/qwak_services_mock/mocks/utils/__init__.py
+-rw-r--r--   0        0        0      159 2023-04-24 08:15:15.386400 qwak_core-0.0.30/qwak_services_mock/mocks/utils/exception_handlers.py
+-rw-r--r--   0        0        0    13054 2023-04-24 08:15:15.386400 qwak_core-0.0.30/qwak_services_mock/services_mock.py
+-rw-r--r--   0        0        0        0 2023-04-24 08:15:15.386400 qwak_core-0.0.30/qwak_services_mock/utils/__init__.py
+-rw-r--r--   0        0        0      265 2023-04-24 08:15:15.386400 qwak_core-0.0.30/qwak_services_mock/utils/service_utils.py
+-rw-r--r--   0        0        0     4507 1970-01-01 00:00:00.000000 qwak_core-0.0.30/setup.py
+-rw-r--r--   0        0        0     1468 1970-01-01 00:00:00.000000 qwak_core-0.0.30/PKG-INFO
```

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/administration/account/v1/account_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/administration/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py` & `qwak_core-0.0.30/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py` & `qwak_core-0.0.30/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py` & `qwak_core-0.0.30/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/administration/v0/users/user_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/administration/v0/users/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py` & `qwak_core-0.0.30/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/analytics/analytics_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/analytics/analytics_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/analytics/analytics_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/analytics/analytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/analytics/analytics_service_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/analytics/analytics_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py` & `qwak_core-0.0.30/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/audience/v1/audience_api_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/audience/v1/audience_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py` & `qwak_core-0.0.30/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/audience/v1/audience_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/audience/v1/audience_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/audience/v1/audience_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/audience/v1/audience_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py` & `qwak_core-0.0.30/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/automation/v1/action_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/automation/v1/action_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/automation/v1/action_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/automation/v1/action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py` & `qwak_core-0.0.30/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/automation/v1/automation_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/automation/v1/automation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/automation/v1/automation_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/automation/v1/automation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/automation/v1/common_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/automation/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/automation/v1/common_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/automation/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/automation/v1/notification_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/automation/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/automation/v1/notification_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/automation/v1/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/automation/v1/trigger_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/automation/v1/trigger_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py` & `qwak_core-0.0.30/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/build/v1/build_api_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/build/v1/build_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/build/v1/build_api_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/build/v1/build_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py` & `qwak_core-0.0.30/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/build/v1/build_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/build/v1/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/build/v1/build_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/build/v1/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/builds/build_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/builds/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/builds/build_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/builds/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/builds/build_url_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/builds/build_url_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/builds/build_url_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/builds/build_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py` & `qwak_core-0.0.30/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/builds/builds_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/builds/builds_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/builds/builds_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/builds/builds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/builds/builds_pb2_grpc.py` & `qwak_core-0.0.30/_qwak_proto/qwak/builds/builds_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py` & `qwak_core-0.0.30/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/deployment/alert_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/deployment/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/deployment/alert_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/deployment/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/deployment/alert_service_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/deployment/alert_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/deployment/alert_service_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/deployment/alert_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py` & `qwak_core-0.0.30/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/deployment/deployment_messages_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/deployment/deployment_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/deployment/deployment_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/deployment/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/deployment/deployment_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/deployment/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/deployment/deployment_service_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/deployment/deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py` & `qwak_core-0.0.30/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py` & `qwak_core-0.0.30/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/entities/entity_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/entities/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/features/execution_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/features/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/jobs/job_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/jobs/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/reports/report_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/reports/report_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/serving/serving_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/serving/serving_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/sources/batch_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/sources/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.30/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.30/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py` & `qwak_core-0.0.30/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py` & `qwak_core-0.0.30/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/fitness_service/constructs_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/fitness_service/constructs_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/fitness_service/fitness_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/fitness_service/fitness_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py` & `qwak_core-0.0.30/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/fitness_service/status_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/fitness_service/status_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/fitness_service/status_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/fitness_service/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/inference/feedback/feedback_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/inference/feedback/feedback_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py` & `qwak_core-0.0.30/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py` & `qwak_core-0.0.30/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/logging/log_filter_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/logging/log_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/logging/log_filter_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/logging/log_filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/logging/log_line_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/logging/log_line_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/logging/log_line_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/logging/log_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/logging/log_reader_service_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/logging/log_reader_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py` & `qwak_core-0.0.30/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/logging/log_source_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/logging/log_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/logging/log_source_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/logging/log_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/models/models_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/models/models_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/models/models_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/models/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/models/models_pb2_grpc.py` & `qwak_core-0.0.30/_qwak_proto/qwak/models/models_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py` & `qwak_core-0.0.30/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py` & `qwak_core-0.0.30/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/projects/projects_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/projects/projects_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/projects/projects_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/projects/projects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/projects/projects_pb2_grpc.py` & `qwak_core-0.0.30/_qwak_proto/qwak/projects/projects_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/secret_service/secret_service_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/secret_service/secret_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py` & `qwak_core-0.0.30/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py` & `qwak_core-0.0.30/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/self_service/user/v1/user_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/self_service/user/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py` & `qwak_core-0.0.30/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py` & `qwak_core-0.0.30/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/traffic/v1/traffic_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/traffic/v1/traffic_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/user_application/v0/user_application_pb2.py` & `qwak_core-0.0.30/_qwak_proto/qwak/user_application/v0/user_application_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi` & `qwak_core-0.0.30/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/pyproject.toml` & `qwak_core-0.0.30/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-core"
-version = "0.0.29"
+version = "0.0.30"
 description = "Qwak Core contains the necessary objects and communication tools for using the Qwak Platform"
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 packages = [
     {include = "qwak"},
     {include = "_qwak_proto"},
```

### Comparing `qwak_core-0.0.29/qwak/automations/__init__.py` & `qwak_core-0.0.30/qwak/automations/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/automations/automation_executions.py` & `qwak_core-0.0.30/qwak/automations/automation_executions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/automations/automations.py` & `qwak_core-0.0.30/qwak/automations/automations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/clients/administration/authenticated_user/client.py` & `qwak_core-0.0.30/qwak/clients/administration/authenticated_user/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/clients/administration/authentication/client.py` & `qwak_core-0.0.30/qwak/clients/administration/authentication/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/clients/administration/eco_system/client.py` & `qwak_core-0.0.30/qwak/clients/administration/eco_system/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/clients/administration/environment/client.py` & `qwak_core-0.0.30/qwak/clients/administration/environment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/clients/administration/self_service/client.py` & `qwak_core-0.0.30/qwak/clients/administration/self_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/clients/alert_management/client.py` & `qwak_core-0.0.30/qwak/clients/alert_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/clients/analytics/client.py` & `qwak_core-0.0.30/qwak/clients/analytics/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/clients/audience/client.py` & `qwak_core-0.0.30/qwak/clients/audience/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/clients/automation_management/client.py` & `qwak_core-0.0.30/qwak/clients/automation_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/clients/autoscaling/client.py` & `qwak_core-0.0.30/qwak/clients/autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/clients/batch_job_management/client.py` & `qwak_core-0.0.30/qwak/clients/batch_job_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/clients/batch_job_management/executions_config.py` & `qwak_core-0.0.30/qwak/clients/batch_job_management/executions_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/clients/batch_job_management/results.py` & `qwak_core-0.0.30/qwak/clients/batch_job_management/results.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/clients/build_management/client.py` & `qwak_core-0.0.30/qwak/clients/build_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/clients/build_orchestrator/client.py` & `qwak_core-0.0.30/qwak/clients/build_orchestrator/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/clients/data_versioning/client.py` & `qwak_core-0.0.30/qwak/clients/data_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/clients/deployment/client.py` & `qwak_core-0.0.30/qwak/clients/deployment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/clients/feature_store/job_registry_client.py` & `qwak_core-0.0.30/qwak/clients/feature_store/job_registry_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/clients/feature_store/management_client.py` & `qwak_core-0.0.30/qwak/clients/feature_store/management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/clients/feature_store/operator_client.py` & `qwak_core-0.0.30/qwak/clients/feature_store/operator_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/clients/file_versioning/client.py` & `qwak_core-0.0.30/qwak/clients/file_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/clients/kube_deployment_captain/client.py` & `qwak_core-0.0.30/qwak/clients/kube_deployment_captain/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/clients/logging_client/client.py` & `qwak_core-0.0.30/qwak/clients/logging_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/clients/model_management/client.py` & `qwak_core-0.0.30/qwak/clients/model_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/clients/project/client.py` & `qwak_core-0.0.30/qwak/clients/project/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/clients/secret_service/client.py` & `qwak_core-0.0.30/qwak/clients/secret_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/clients/user_application_instance/client.py` & `qwak_core-0.0.30/qwak/clients/user_application_instance/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/exceptions/quiet_error.py` & `qwak_core-0.0.30/qwak/exceptions/quiet_error.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/exceptions/qwak_http_exception.py` & `qwak_core-0.0.30/qwak/exceptions/qwak_http_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/feature_store/data_sources/__init__.py` & `qwak_core-0.0.30/qwak/feature_store/data_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/feature_store/data_sources/batch_sources/_batch.py` & `qwak_core-0.0.30/qwak/feature_store/data_sources/batch_sources/_batch.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,24 +30,29 @@
         pass
 
     @classmethod
     @abstractmethod
     def _from_proto(cls, proto):
         pass
 
-    def get_sample(self, number_of_rows: int = 10):
+    def get_sample(self, number_of_rows: int = 10) -> "pd.DataFrame":
         """
         Tries to get a sample of length `number_rows` from the data source.
         Args:
             number_of_rows: number of rows to get from data source
         Returns:
             A tuple containing the resulting dataframe and a tuple of the columns names and types.
             (the types are pyspark dataframe types)
         """
 
+        try:
+            import pandas as pd
+        except ImportError:
+            raise QwakException("Missing Pandas dependency required for getting sample")
+
         if number_of_rows > 1000:
             raise ValueError(f"`number_rows` must be under 1000, got: {number_of_rows}")
 
         operator_client = FeaturesOperatorClient()
         ds_spec = self._to_proto()
 
         result = operator_client.validate_data_source_blocking(
```

### Comparing `qwak_core-0.0.29/qwak/feature_store/data_sources/batch_sources/_jdbc.py` & `qwak_core-0.0.30/qwak/feature_store/data_sources/batch_sources/_jdbc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/feature_store/data_sources/batch_sources/big_query.py` & `qwak_core-0.0.30/qwak/feature_store/data_sources/batch_sources/big_query.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/feature_store/data_sources/batch_sources/csv.py` & `qwak_core-0.0.30/qwak/feature_store/data_sources/batch_sources/csv.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/feature_store/data_sources/batch_sources/elastic_search.py` & `qwak_core-0.0.30/qwak/feature_store/data_sources/batch_sources/elastic_search.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/feature_store/data_sources/batch_sources/filesystem_config.py` & `qwak_core-0.0.30/qwak/feature_store/data_sources/batch_sources/filesystem_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/feature_store/data_sources/batch_sources/mongodb.py` & `qwak_core-0.0.30/qwak/feature_store/data_sources/batch_sources/mongodb.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/feature_store/data_sources/batch_sources/mysql.py` & `qwak_core-0.0.30/qwak/feature_store/data_sources/batch_sources/mysql.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/feature_store/data_sources/batch_sources/parquet.py` & `qwak_core-0.0.30/qwak/feature_store/data_sources/batch_sources/parquet.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/feature_store/data_sources/batch_sources/postgres.py` & `qwak_core-0.0.30/qwak/feature_store/data_sources/batch_sources/postgres.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/feature_store/data_sources/batch_sources/redshift.py` & `qwak_core-0.0.30/qwak/feature_store/data_sources/batch_sources/redshift.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/feature_store/data_sources/batch_sources/snowflake.py` & `qwak_core-0.0.30/qwak/feature_store/data_sources/batch_sources/snowflake.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/feature_store/data_sources/batch_sources/vertica.py` & `qwak_core-0.0.30/qwak/feature_store/data_sources/batch_sources/vertica.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/feature_store/entities/entity.py` & `qwak_core-0.0.30/qwak/feature_store/entities/entity.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/feature_store/feature_sets/backfill.py` & `qwak_core-0.0.30/qwak/feature_store/feature_sets/backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/feature_store/feature_sets/batch.py` & `qwak_core-0.0.30/qwak/feature_store/feature_sets/batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -428,14 +428,20 @@
             # 3	      2	        2021-01-01 18:00:00	              34
         """
 
         """
         Fetches a sample of the Featureset transformation by loading requested sample of data from the data source
         and executing the transformation on that data.
         """
+
+        try:
+            import pandas as pd
+        except ImportError:
+            raise QwakException("Missing Pandas dependency required for getting sample")
+
         if 0 >= number_of_rows > 1000:
             raise ValueError(
                 f"`number_rows` must be under 1000 and positive, got: {number_of_rows}"
             )
 
         operator_client = FeaturesOperatorClient()
         registry_client = FeatureRegistryClient()
```

### Comparing `qwak_core-0.0.29/qwak/feature_store/feature_sets/execution_spec.py` & `qwak_core-0.0.30/qwak/feature_store/feature_sets/execution_spec.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/feature_store/feature_sets/metadata.py` & `qwak_core-0.0.30/qwak/feature_store/feature_sets/metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/feature_store/feature_sets/read_policies.py` & `qwak_core-0.0.30/qwak/feature_store/feature_sets/read_policies.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/feature_store/feature_sets/transformations.py` & `qwak_core-0.0.30/qwak/feature_store/feature_sets/transformations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/feature_store/online/client.py` & `qwak_core-0.0.30/qwak/feature_store/online/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/inner/const.py` & `qwak_core-0.0.30/qwak/inner/const.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/inner/di_configuration/__init__.py` & `qwak_core-0.0.30/qwak/inner/di_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/inner/di_configuration/account.py` & `qwak_core-0.0.30/qwak/inner/di_configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/inner/di_configuration/containers.py` & `qwak_core-0.0.30/qwak/inner/di_configuration/containers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/inner/model_loggers_utils.py` & `qwak_core-0.0.30/qwak/inner/model_loggers_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/inner/singleton_meta.py` & `qwak_core-0.0.30/qwak/inner/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/inner/tool/auth.py` & `qwak_core-0.0.30/qwak/inner/tool/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/inner/tool/grpc/grpc_auth.py` & `qwak_core-0.0.30/qwak/inner/tool/grpc/grpc_auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/inner/tool/grpc/grpc_tools.py` & `qwak_core-0.0.30/qwak/inner/tool/grpc/grpc_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/inner/tool/run_config/base.py` & `qwak_core-0.0.30/qwak/inner/tool/run_config/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/inner/tool/run_config/utils.py` & `qwak_core-0.0.30/qwak/inner/tool/run_config/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/model/adapters/__init__.py` & `qwak_core-0.0.30/qwak/model/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/model/adapters/input_adapters/multi_input_adapter.py` & `qwak_core-0.0.30/qwak/model/adapters/input_adapters/multi_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/model/adapters/input_adapters/numpy_input_adapter.py` & `qwak_core-0.0.30/qwak/model/adapters/input_adapters/numpy_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/model/adapters/input_adapters/proto_input_adapter.py` & `qwak_core-0.0.30/qwak/model/adapters/input_adapters/proto_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/model/adapters/output_adapters/numpy_output_adapter.py` & `qwak_core-0.0.30/qwak/model/adapters/output_adapters/numpy_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/model/adapters/output_adapters/proto_output_adapter.py` & `qwak_core-0.0.30/qwak/model/adapters/output_adapters/proto_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/model/base.py` & `qwak_core-0.0.30/qwak/model/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/model/decorators/api.py` & `qwak_core-0.0.30/qwak/model/decorators/api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/model/decorators/api_implementation.py` & `qwak_core-0.0.30/qwak/model/decorators/api_implementation.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/model/experiment_tracking.py` & `qwak_core-0.0.30/qwak/model/experiment_tracking.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/model/schema.py` & `qwak_core-0.0.30/qwak/model/schema.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/model/schema_entities.py` & `qwak_core-0.0.30/qwak/model/schema_entities.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/model_loggers/artifact_logger.py` & `qwak_core-0.0.30/qwak/model_loggers/artifact_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/model_loggers/data_logger.py` & `qwak_core-0.0.30/qwak/model_loggers/data_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/model_loggers/model_logger.py` & `qwak_core-0.0.30/qwak/model_loggers/model_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/qwak_client/builds/build.py` & `qwak_core-0.0.30/qwak/qwak_client/builds/build.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/qwak_client/builds/filters/metric_filter.py` & `qwak_core-0.0.30/qwak/qwak_client/builds/filters/metric_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/qwak_client/builds/filters/parameter_filter.py` & `qwak_core-0.0.30/qwak/qwak_client/builds/filters/parameter_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/qwak_client/client.py` & `qwak_core-0.0.30/qwak/qwak_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/qwak_client/deployments/deployment.py` & `qwak_core-0.0.30/qwak/qwak_client/deployments/deployment.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/qwak_client/models/model.py` & `qwak_core-0.0.30/qwak/qwak_client/models/model.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/qwak_client/models/model_metadata.py` & `qwak_core-0.0.30/qwak/qwak_client/models/model_metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak/qwak_client/projects/project.py` & `qwak_core-0.0.30/qwak/qwak_client/projects/project.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak_services_mock/mocks/alert_manager_service_api.py` & `qwak_core-0.0.30/qwak_services_mock/mocks/alert_manager_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak_services_mock/mocks/analytics_api.py` & `qwak_core-0.0.30/qwak_services_mock/mocks/analytics_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak_services_mock/mocks/audience_service_api.py` & `qwak_core-0.0.30/qwak_services_mock/mocks/audience_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak_services_mock/mocks/authentication_service.py` & `qwak_core-0.0.30/qwak_services_mock/mocks/authentication_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak_services_mock/mocks/automation_management_service.py` & `qwak_core-0.0.30/qwak_services_mock/mocks/automation_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak_services_mock/mocks/autoscaling_service_api.py` & `qwak_core-0.0.30/qwak_services_mock/mocks/autoscaling_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak_services_mock/mocks/batch_job_manager_service.py` & `qwak_core-0.0.30/qwak_services_mock/mocks/batch_job_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak_services_mock/mocks/build_management.py` & `qwak_core-0.0.30/qwak_services_mock/mocks/build_management.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak_services_mock/mocks/build_orchestrator_build_api.py` & `qwak_core-0.0.30/qwak_services_mock/mocks/build_orchestrator_build_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak_services_mock/mocks/build_orchestrator_service_api.py` & `qwak_core-0.0.30/qwak_services_mock/mocks/build_orchestrator_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak_services_mock/mocks/data_versioning_service.py` & `qwak_core-0.0.30/qwak_services_mock/mocks/data_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak_services_mock/mocks/deployment_management_service.py` & `qwak_core-0.0.30/qwak_services_mock/mocks/deployment_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak_services_mock/mocks/ecosystem_service_api.py` & `qwak_core-0.0.30/qwak_services_mock/mocks/ecosystem_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py` & `qwak_core-0.0.30/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak_services_mock/mocks/feature_store_entities_manager_api.py` & `qwak_core-0.0.30/qwak_services_mock/mocks/feature_store_entities_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py` & `qwak_core-0.0.30/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak_services_mock/mocks/features_online_serving_api.py` & `qwak_core-0.0.30/qwak_services_mock/mocks/features_online_serving_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak_services_mock/mocks/features_operator_v3_service.py` & `qwak_core-0.0.30/qwak_services_mock/mocks/features_operator_v3_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak_services_mock/mocks/features_set_state_service_api.py` & `qwak_core-0.0.30/qwak_services_mock/mocks/features_set_state_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak_services_mock/mocks/feedback_service.py` & `qwak_core-0.0.30/qwak_services_mock/mocks/feedback_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak_services_mock/mocks/file_versioning_service.py` & `qwak_core-0.0.30/qwak_services_mock/mocks/file_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak_services_mock/mocks/job_registry_service_api.py` & `qwak_core-0.0.30/qwak_services_mock/mocks/job_registry_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak_services_mock/mocks/kube_captain_service_api.py` & `qwak_core-0.0.30/qwak_services_mock/mocks/kube_captain_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak_services_mock/mocks/logging_service.py` & `qwak_core-0.0.30/qwak_services_mock/mocks/logging_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak_services_mock/mocks/model_management_service.py` & `qwak_core-0.0.30/qwak_services_mock/mocks/model_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak_services_mock/mocks/project_manager_service.py` & `qwak_core-0.0.30/qwak_services_mock/mocks/project_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak_services_mock/mocks/qwak_mocks.py` & `qwak_core-0.0.30/qwak_services_mock/mocks/qwak_mocks.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak_services_mock/mocks/secret_service.py` & `qwak_core-0.0.30/qwak_services_mock/mocks/secret_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak_services_mock/mocks/self_service_user_service.py` & `qwak_core-0.0.30/qwak_services_mock/mocks/self_service_user_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak_services_mock/mocks/user_application_instance_service_api.py` & `qwak_core-0.0.30/qwak_services_mock/mocks/user_application_instance_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/qwak_services_mock/services_mock.py` & `qwak_core-0.0.30/qwak_services_mock/services_mock.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.29/setup.py` & `qwak_core-0.0.30/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
  'protobuf>=3.10,<4',
  'python-jose',
  'requests',
  'typeguard>=2,<3']
 
 setup_kwargs = {
     'name': 'qwak-core',
-    'version': '0.0.29',
+    'version': '0.0.30',
     'description': 'Qwak Core contains the necessary objects and communication tools for using the Qwak Platform',
     'long_description': '# Qwak Core\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Core contains all the objects and tools necessary to use the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_core-0.0.29/PKG-INFO` & `qwak_core-0.0.30/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-core
-Version: 0.0.29
+Version: 0.0.30
 Summary: Qwak Core contains the necessary objects and communication tools for using the Qwak Platform
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

