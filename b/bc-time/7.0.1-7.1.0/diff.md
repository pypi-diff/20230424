# Comparing `tmp/bc_time-7.0.1.tar.gz` & `tmp/bc_time-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bc_time-7.0.1.tar", last modified: Mon Apr 17 10:52:25 2023, max compression
+gzip compressed data, was "bc_time-7.1.0.tar", last modified: Mon Apr 24 10:19:56 2023, max compression
```

## Comparing `bc_time-7.0.1.tar` & `bc_time-7.1.0.tar`

### file list

```diff
@@ -1,69 +1,70 @@
-drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-17 10:52:25.567971 bc_time-7.0.1/
--rw-r--r--   0 dburger    (501) staff       (20)     1067 2022-05-24 07:44:21.000000 bc_time-7.0.1/LICENSE.txt
--rw-r--r--   0 dburger    (501) staff       (20)     4987 2023-04-17 10:52:25.568027 bc_time-7.0.1/PKG-INFO
--rw-r--r--   0 dburger    (501) staff       (20)     4494 2023-04-17 10:51:52.000000 bc_time-7.0.1/README.md
--rw-r--r--   0 dburger    (501) staff       (20)      653 2023-04-17 10:52:25.568274 bc_time-7.0.1/setup.cfg
--rw-r--r--   0 dburger    (501) staff       (20)       38 2022-05-30 08:48:56.000000 bc_time-7.0.1/setup.py
-drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-17 10:52:25.556665 bc_time-7.0.1/src/
-drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-17 10:52:25.557953 bc_time-7.0.1/src/bc_time/
--rw-r--r--   0 dburger    (501) staff       (20)      932 2022-09-08 09:24:55.000000 bc_time-7.0.1/src/bc_time/__init__.py
-drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-17 10:52:25.559042 bc_time-7.0.1/src/bc_time/api/
--rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-30 07:05:50.000000 bc_time-7.0.1/src/bc_time/api/__init__.py
--rw-r--r--   0 dburger    (501) staff       (20)    10300 2023-03-17 11:28:56.000000 bc_time-7.0.1/src/bc_time/api/api.py
-drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-17 10:52:25.559494 bc_time-7.0.1/src/bc_time/api/constants/
--rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-23 11:26:48.000000 bc_time-7.0.1/src/bc_time/api/constants/__init__.py
--rw-r--r--   0 dburger    (501) staff       (20)      316 2023-03-17 10:38:21.000000 bc_time-7.0.1/src/bc_time/api/constants/api.py
-drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-17 10:52:25.561072 bc_time-7.0.1/src/bc_time/api/enumerators/
--rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-23 11:26:53.000000 bc_time-7.0.1/src/bc_time/api/enumerators/__init__.py
--rw-r--r--   0 dburger    (501) staff       (20)      127 2022-09-01 13:03:48.000000 bc_time-7.0.1/src/bc_time/api/enumerators/api_authorisation_type.py
--rw-r--r--   0 dburger    (501) staff       (20)      800 2022-09-08 09:24:55.000000 bc_time-7.0.1/src/bc_time/api/enumerators/content_type.py
--rw-r--r--   0 dburger    (501) staff       (20)      118 2022-07-13 12:37:22.000000 bc_time-7.0.1/src/bc_time/api/enumerators/device_communication_type.py
--rw-r--r--   0 dburger    (501) staff       (20)      883 2023-03-24 14:21:28.000000 bc_time-7.0.1/src/bc_time/api/enumerators/request_status.py
--rw-r--r--   0 dburger    (501) staff       (20)       96 2022-05-30 10:21:47.000000 bc_time-7.0.1/src/bc_time/api/enumerators/status.py
-drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-17 10:52:25.565277 bc_time-7.0.1/src/bc_time/api/objects/
--rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-30 07:57:56.000000 bc_time-7.0.1/src/bc_time/api/objects/__init__.py
--rw-r--r--   0 dburger    (501) staff       (20)      780 2023-03-17 11:22:52.000000 bc_time-7.0.1/src/bc_time/api/objects/api_authorisations.py
--rw-r--r--   0 dburger    (501) staff       (20)      239 2022-06-08 10:01:59.000000 bc_time-7.0.1/src/bc_time/api/objects/base.py
--rw-r--r--   0 dburger    (501) staff       (20)      400 2022-09-01 12:52:18.000000 bc_time-7.0.1/src/bc_time/api/objects/branches.py
--rw-r--r--   0 dburger    (501) staff       (20)     1312 2022-06-10 09:39:34.000000 bc_time-7.0.1/src/bc_time/api/objects/company_profiles.py
--rw-r--r--   0 dburger    (501) staff       (20)      407 2022-09-01 12:52:56.000000 bc_time-7.0.1/src/bc_time/api/objects/controllers.py
--rw-r--r--   0 dburger    (501) staff       (20)      339 2022-09-08 09:24:55.000000 bc_time-7.0.1/src/bc_time/api/objects/daily_overtime_data.py
--rw-r--r--   0 dburger    (501) staff       (20)      407 2022-09-01 13:12:19.000000 bc_time-7.0.1/src/bc_time/api/objects/departments.py
--rw-r--r--   0 dburger    (501) staff       (20)      399 2022-09-01 12:53:07.000000 bc_time-7.0.1/src/bc_time/api/objects/devices.py
--rw-r--r--   0 dburger    (501) staff       (20)      413 2022-09-01 12:53:22.000000 bc_time-7.0.1/src/bc_time/api/objects/employee_leave.py
--rw-r--r--   0 dburger    (501) staff       (20)      403 2022-09-29 07:57:01.000000 bc_time-7.0.1/src/bc_time/api/objects/employees.py
--rw-r--r--   0 dburger    (501) staff       (20)     1294 2022-06-08 10:01:52.000000 bc_time-7.0.1/src/bc_time/api/objects/group_base.py
--rw-r--r--   0 dburger    (501) staff       (20)      817 2022-09-01 12:12:32.000000 bc_time-7.0.1/src/bc_time/api/objects/object_base_read.py
--rw-r--r--   0 dburger    (501) staff       (20)      965 2022-09-01 12:12:38.000000 bc_time-7.0.1/src/bc_time/api/objects/object_base_write.py
--rw-r--r--   0 dburger    (501) staff       (20)      362 2022-06-08 10:35:28.000000 bc_time-7.0.1/src/bc_time/api/objects/settings.py
--rw-r--r--   0 dburger    (501) staff       (20)      556 2022-09-01 12:54:17.000000 bc_time-7.0.1/src/bc_time/api/objects/visitor_groups.py
--rw-r--r--   0 dburger    (501) staff       (20)      401 2022-09-01 12:54:29.000000 bc_time-7.0.1/src/bc_time/api/objects/visitors.py
-drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-17 10:52:25.565542 bc_time-7.0.1/src/bc_time/oauth2/
--rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-23 11:27:12.000000 bc_time-7.0.1/src/bc_time/oauth2/__init__.py
-drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-17 10:52:25.565892 bc_time-7.0.1/src/bc_time/oauth2/constants/
--rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-23 11:27:17.000000 bc_time-7.0.1/src/bc_time/oauth2/constants/__init__.py
--rw-r--r--   0 dburger    (501) staff       (20)      258 2023-04-17 10:31:54.000000 bc_time-7.0.1/src/bc_time/oauth2/constants/grant_type.py
--rw-r--r--   0 dburger    (501) staff       (20)     7366 2023-04-17 10:42:19.000000 bc_time-7.0.1/src/bc_time/oauth2/token.py
-drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-17 10:52:25.566198 bc_time-7.0.1/src/bc_time/requests/
--rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-23 11:27:26.000000 bc_time-7.0.1/src/bc_time/requests/__init__.py
--rw-r--r--   0 dburger    (501) staff       (20)      513 2022-09-07 09:21:24.000000 bc_time-7.0.1/src/bc_time/requests/base.py
-drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-17 10:52:25.566531 bc_time-7.0.1/src/bc_time/system/
--rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-20 14:56:44.000000 bc_time-7.0.1/src/bc_time/system/__init__.py
-drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-17 10:52:25.566765 bc_time-7.0.1/src/bc_time/system/constants/
--rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-23 14:36:08.000000 bc_time-7.0.1/src/bc_time/system/constants/__init__.py
-drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-17 10:52:25.566979 bc_time-7.0.1/src/bc_time/system/constants/datetime/
--rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-23 14:35:09.000000 bc_time-7.0.1/src/bc_time/system/constants/datetime/__init__.py
--rw-r--r--   0 dburger    (501) staff       (20)       78 2022-05-18 10:11:58.000000 bc_time-7.0.1/src/bc_time/system/constants/datetime/format.py
-drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-17 10:52:25.567389 bc_time-7.0.1/src/bc_time/system/constants/encryption/
--rw-r--r--   0 dburger    (501) staff       (20)        0 2022-09-02 13:20:51.000000 bc_time-7.0.1/src/bc_time/system/constants/encryption/__init__.py
--rw-r--r--   0 dburger    (501) staff       (20)       47 2022-08-30 08:08:54.000000 bc_time-7.0.1/src/bc_time/system/constants/encryption/crypt.py
-drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-17 10:52:25.567730 bc_time-7.0.1/src/bc_time/system/encryption/
--rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-20 14:56:50.000000 bc_time-7.0.1/src/bc_time/system/encryption/__init__.py
--rw-r--r--   0 dburger    (501) staff       (20)     4759 2022-10-18 13:53:04.000000 bc_time-7.0.1/src/bc_time/system/encryption/crypt.py
--rw-r--r--   0 dburger    (501) staff       (20)      473 2022-05-19 07:56:45.000000 bc_time-7.0.1/src/bc_time/system/validate.py
-drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-17 10:52:25.558848 bc_time-7.0.1/src/bc_time.egg-info/
--rw-r--r--   0 dburger    (501) staff       (20)     4987 2023-04-17 10:52:25.000000 bc_time-7.0.1/src/bc_time.egg-info/PKG-INFO
--rw-r--r--   0 dburger    (501) staff       (20)     1901 2023-04-17 10:52:25.000000 bc_time-7.0.1/src/bc_time.egg-info/SOURCES.txt
--rw-r--r--   0 dburger    (501) staff       (20)        1 2023-04-17 10:52:25.000000 bc_time-7.0.1/src/bc_time.egg-info/dependency_links.txt
--rw-r--r--   0 dburger    (501) staff       (20)       22 2023-04-17 10:52:25.000000 bc_time-7.0.1/src/bc_time.egg-info/requires.txt
--rw-r--r--   0 dburger    (501) staff       (20)        8 2023-04-17 10:52:25.000000 bc_time-7.0.1/src/bc_time.egg-info/top_level.txt
+drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-24 10:19:56.490054 bc_time-7.1.0/
+-rw-r--r--   0 dburger    (501) staff       (20)     1067 2022-05-24 07:44:21.000000 bc_time-7.1.0/LICENSE.txt
+-rw-r--r--   0 dburger    (501) staff       (20)     5008 2023-04-24 10:19:56.490096 bc_time-7.1.0/PKG-INFO
+-rw-r--r--   0 dburger    (501) staff       (20)     4515 2023-04-24 10:04:47.000000 bc_time-7.1.0/README.md
+-rw-r--r--   0 dburger    (501) staff       (20)      653 2023-04-24 10:19:56.490316 bc_time-7.1.0/setup.cfg
+-rw-r--r--   0 dburger    (501) staff       (20)       38 2022-05-30 08:48:56.000000 bc_time-7.1.0/setup.py
+drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-24 10:19:56.483140 bc_time-7.1.0/src/
+drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-24 10:19:56.484452 bc_time-7.1.0/src/bc_time/
+-rw-r--r--   0 dburger    (501) staff       (20)      997 2023-04-21 09:17:19.000000 bc_time-7.1.0/src/bc_time/__init__.py
+drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-24 10:19:56.485204 bc_time-7.1.0/src/bc_time/api/
+-rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-30 07:05:50.000000 bc_time-7.1.0/src/bc_time/api/__init__.py
+-rw-r--r--   0 dburger    (501) staff       (20)    10300 2023-03-17 11:28:56.000000 bc_time-7.1.0/src/bc_time/api/api.py
+drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-24 10:19:56.485393 bc_time-7.1.0/src/bc_time/api/constants/
+-rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-23 11:26:48.000000 bc_time-7.1.0/src/bc_time/api/constants/__init__.py
+-rw-r--r--   0 dburger    (501) staff       (20)      316 2023-03-17 10:38:21.000000 bc_time-7.1.0/src/bc_time/api/constants/api.py
+drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-24 10:19:56.486461 bc_time-7.1.0/src/bc_time/api/enumerators/
+-rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-23 11:26:53.000000 bc_time-7.1.0/src/bc_time/api/enumerators/__init__.py
+-rw-r--r--   0 dburger    (501) staff       (20)      127 2022-09-01 13:03:48.000000 bc_time-7.1.0/src/bc_time/api/enumerators/api_authorisation_type.py
+-rw-r--r--   0 dburger    (501) staff       (20)      832 2023-04-21 09:15:52.000000 bc_time-7.1.0/src/bc_time/api/enumerators/content_type.py
+-rw-r--r--   0 dburger    (501) staff       (20)      118 2022-07-13 12:37:22.000000 bc_time-7.1.0/src/bc_time/api/enumerators/device_communication_type.py
+-rw-r--r--   0 dburger    (501) staff       (20)      883 2023-03-24 14:21:28.000000 bc_time-7.1.0/src/bc_time/api/enumerators/request_status.py
+-rw-r--r--   0 dburger    (501) staff       (20)       96 2022-05-30 10:21:47.000000 bc_time-7.1.0/src/bc_time/api/enumerators/status.py
+drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-24 10:19:56.488319 bc_time-7.1.0/src/bc_time/api/objects/
+-rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-30 07:57:56.000000 bc_time-7.1.0/src/bc_time/api/objects/__init__.py
+-rw-r--r--   0 dburger    (501) staff       (20)      780 2023-03-17 11:22:52.000000 bc_time-7.1.0/src/bc_time/api/objects/api_authorisations.py
+-rw-r--r--   0 dburger    (501) staff       (20)      239 2022-06-08 10:01:59.000000 bc_time-7.1.0/src/bc_time/api/objects/base.py
+-rw-r--r--   0 dburger    (501) staff       (20)      400 2022-09-01 12:52:18.000000 bc_time-7.1.0/src/bc_time/api/objects/branches.py
+-rw-r--r--   0 dburger    (501) staff       (20)     1312 2022-06-10 09:39:34.000000 bc_time-7.1.0/src/bc_time/api/objects/company_profiles.py
+-rw-r--r--   0 dburger    (501) staff       (20)      407 2022-09-01 12:52:56.000000 bc_time-7.1.0/src/bc_time/api/objects/controllers.py
+-rw-r--r--   0 dburger    (501) staff       (20)      339 2022-09-08 09:24:55.000000 bc_time-7.1.0/src/bc_time/api/objects/daily_overtime_data.py
+-rw-r--r--   0 dburger    (501) staff       (20)      407 2022-09-01 13:12:19.000000 bc_time-7.1.0/src/bc_time/api/objects/departments.py
+-rw-r--r--   0 dburger    (501) staff       (20)      399 2022-09-01 12:53:07.000000 bc_time-7.1.0/src/bc_time/api/objects/devices.py
+-rw-r--r--   0 dburger    (501) staff       (20)      413 2022-09-01 12:53:22.000000 bc_time-7.1.0/src/bc_time/api/objects/employee_leave.py
+-rw-r--r--   0 dburger    (501) staff       (20)      403 2022-09-29 07:57:01.000000 bc_time-7.1.0/src/bc_time/api/objects/employees.py
+-rw-r--r--   0 dburger    (501) staff       (20)     1294 2022-06-08 10:01:52.000000 bc_time-7.1.0/src/bc_time/api/objects/group_base.py
+-rw-r--r--   0 dburger    (501) staff       (20)      817 2022-09-01 12:12:32.000000 bc_time-7.1.0/src/bc_time/api/objects/object_base_read.py
+-rw-r--r--   0 dburger    (501) staff       (20)      965 2022-09-01 12:12:38.000000 bc_time-7.1.0/src/bc_time/api/objects/object_base_write.py
+-rw-r--r--   0 dburger    (501) staff       (20)      341 2023-04-21 09:16:52.000000 bc_time-7.1.0/src/bc_time/api/objects/period_overtime_data.py
+-rw-r--r--   0 dburger    (501) staff       (20)      362 2022-06-08 10:35:28.000000 bc_time-7.1.0/src/bc_time/api/objects/settings.py
+-rw-r--r--   0 dburger    (501) staff       (20)      556 2022-09-01 12:54:17.000000 bc_time-7.1.0/src/bc_time/api/objects/visitor_groups.py
+-rw-r--r--   0 dburger    (501) staff       (20)      401 2022-09-01 12:54:29.000000 bc_time-7.1.0/src/bc_time/api/objects/visitors.py
+drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-24 10:19:56.488506 bc_time-7.1.0/src/bc_time/oauth2/
+-rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-23 11:27:12.000000 bc_time-7.1.0/src/bc_time/oauth2/__init__.py
+drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-24 10:19:56.488854 bc_time-7.1.0/src/bc_time/oauth2/constants/
+-rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-23 11:27:17.000000 bc_time-7.1.0/src/bc_time/oauth2/constants/__init__.py
+-rw-r--r--   0 dburger    (501) staff       (20)      258 2023-04-17 10:31:54.000000 bc_time-7.1.0/src/bc_time/oauth2/constants/grant_type.py
+-rw-r--r--   0 dburger    (501) staff       (20)     7366 2023-04-17 10:42:19.000000 bc_time-7.1.0/src/bc_time/oauth2/token.py
+drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-24 10:19:56.489048 bc_time-7.1.0/src/bc_time/requests/
+-rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-23 11:27:26.000000 bc_time-7.1.0/src/bc_time/requests/__init__.py
+-rw-r--r--   0 dburger    (501) staff       (20)      513 2022-09-07 09:21:24.000000 bc_time-7.1.0/src/bc_time/requests/base.py
+drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-24 10:19:56.489249 bc_time-7.1.0/src/bc_time/system/
+-rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-20 14:56:44.000000 bc_time-7.1.0/src/bc_time/system/__init__.py
+drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-24 10:19:56.489359 bc_time-7.1.0/src/bc_time/system/constants/
+-rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-23 14:36:08.000000 bc_time-7.1.0/src/bc_time/system/constants/__init__.py
+drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-24 10:19:56.489540 bc_time-7.1.0/src/bc_time/system/constants/datetime/
+-rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-23 14:35:09.000000 bc_time-7.1.0/src/bc_time/system/constants/datetime/__init__.py
+-rw-r--r--   0 dburger    (501) staff       (20)       78 2022-05-18 10:11:58.000000 bc_time-7.1.0/src/bc_time/system/constants/datetime/format.py
+drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-24 10:19:56.489731 bc_time-7.1.0/src/bc_time/system/constants/encryption/
+-rw-r--r--   0 dburger    (501) staff       (20)        0 2022-09-02 13:20:51.000000 bc_time-7.1.0/src/bc_time/system/constants/encryption/__init__.py
+-rw-r--r--   0 dburger    (501) staff       (20)       47 2022-08-30 08:08:54.000000 bc_time-7.1.0/src/bc_time/system/constants/encryption/crypt.py
+drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-24 10:19:56.489961 bc_time-7.1.0/src/bc_time/system/encryption/
+-rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-20 14:56:50.000000 bc_time-7.1.0/src/bc_time/system/encryption/__init__.py
+-rw-r--r--   0 dburger    (501) staff       (20)     4759 2022-10-18 13:53:04.000000 bc_time-7.1.0/src/bc_time/system/encryption/crypt.py
+-rw-r--r--   0 dburger    (501) staff       (20)      473 2022-05-19 07:56:45.000000 bc_time-7.1.0/src/bc_time/system/validate.py
+drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-24 10:19:56.485002 bc_time-7.1.0/src/bc_time.egg-info/
+-rw-r--r--   0 dburger    (501) staff       (20)     5008 2023-04-24 10:19:56.000000 bc_time-7.1.0/src/bc_time.egg-info/PKG-INFO
+-rw-r--r--   0 dburger    (501) staff       (20)     1949 2023-04-24 10:19:56.000000 bc_time-7.1.0/src/bc_time.egg-info/SOURCES.txt
+-rw-r--r--   0 dburger    (501) staff       (20)        1 2023-04-24 10:19:56.000000 bc_time-7.1.0/src/bc_time.egg-info/dependency_links.txt
+-rw-r--r--   0 dburger    (501) staff       (20)       22 2023-04-24 10:19:56.000000 bc_time-7.1.0/src/bc_time.egg-info/requires.txt
+-rw-r--r--   0 dburger    (501) staff       (20)        8 2023-04-24 10:19:56.000000 bc_time-7.1.0/src/bc_time.egg-info/top_level.txt
```

### Comparing `bc_time-7.0.1/LICENSE.txt` & `bc_time-7.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bc_time-7.0.1/PKG-INFO` & `bc_time-7.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bc_time
-Version: 7.0.1
+Version: 7.1.0
 Summary: SDK that helps with integration via the Binary City Time API.
 Home-page: https://bitbucket.org/dburger/bc_time_api_sdk/src/master/
 Author: Darius Burger
 Author-email: darius@bcity.me
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -118,14 +118,15 @@
 * CompanyProfiles
 * Controllers
 * Departments
 * Devices
 * DailyOvertimeData
 * Employees
 * EmployeeLeave
+* PeriodOvertimeData
 * Settings
 * Visitors
 * VisitorGroups
 
 # Available methods
 
 ## For (most) objects
```

### Comparing `bc_time-7.0.1/README.md` & `bc_time-7.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -103,14 +103,15 @@
 * CompanyProfiles
 * Controllers
 * Departments
 * Devices
 * DailyOvertimeData
 * Employees
 * EmployeeLeave
+* PeriodOvertimeData
 * Settings
 * Visitors
 * VisitorGroups
 
 # Available methods
 
 ## For (most) objects
```

### Comparing `bc_time-7.0.1/setup.cfg` & `bc_time-7.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bc_time
-version = 7.0.1
+version = 7.1.0
 author = Darius Burger
 author_email = darius@bcity.me
 description = SDK that helps with integration via the Binary City Time API.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://bitbucket.org/dburger/bc_time_api_sdk/src/master/
 classifiers =
```

### Comparing `bc_time-7.0.1/src/bc_time/__init__.py` & `bc_time-7.1.0/src/bc_time/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,8 +11,9 @@
 from .api.objects.controllers import Controllers
 from .api.objects.devices import Devices
 from .api.objects.employees import Employees
 from .api.objects.employee_leave import EmployeeLeave
 from .api.objects.settings import Settings
 from .api.objects.visitors import Visitors
 from .api.objects.visitor_groups import VisitorGroups
-from .api.objects.daily_overtime_data import DailyOvertimeData
+from .api.objects.daily_overtime_data import DailyOvertimeData
+from .api.objects.period_overtime_data import PeriodOvertimeData
```

### Comparing `bc_time-7.0.1/src/bc_time/api/api.py` & `bc_time-7.1.0/src/bc_time/api/api.py`

 * *Files identical despite different names*

### Comparing `bc_time-7.0.1/src/bc_time/api/enumerators/content_type.py` & `bc_time-7.1.0/src/bc_time/api/enumerators/content_type.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,8 +20,9 @@
     visitor_security_area_duration = 352 # How much time spent in area(s).
     controller = 111
     company_profile_user_membership = 114
     company_profile_user_membership_email_confirm = 115
     visitor_group_membership = 116
     visitor_group_area_membership = 117
     current_company_profile = 118
-    daily_overtime_data = 202
+    daily_overtime_data = 202
+    period_overtime_data = 203
```

### Comparing `bc_time-7.0.1/src/bc_time/api/enumerators/request_status.py` & `bc_time-7.1.0/src/bc_time/api/enumerators/request_status.py`

 * *Files identical despite different names*

### Comparing `bc_time-7.0.1/src/bc_time/api/objects/api_authorisations.py` & `bc_time-7.1.0/src/bc_time/api/objects/api_authorisations.py`

 * *Files identical despite different names*

### Comparing `bc_time-7.0.1/src/bc_time/api/objects/company_profiles.py` & `bc_time-7.1.0/src/bc_time/api/objects/company_profiles.py`

 * *Files identical despite different names*

### Comparing `bc_time-7.0.1/src/bc_time/api/objects/group_base.py` & `bc_time-7.1.0/src/bc_time/api/objects/group_base.py`

 * *Files identical despite different names*

### Comparing `bc_time-7.0.1/src/bc_time/api/objects/object_base_read.py` & `bc_time-7.1.0/src/bc_time/api/objects/object_base_read.py`

 * *Files identical despite different names*

### Comparing `bc_time-7.0.1/src/bc_time/api/objects/object_base_write.py` & `bc_time-7.1.0/src/bc_time/api/objects/object_base_write.py`

 * *Files identical despite different names*

### Comparing `bc_time-7.0.1/src/bc_time/api/objects/visitor_groups.py` & `bc_time-7.1.0/src/bc_time/api/objects/visitor_groups.py`

 * *Files identical despite different names*

### Comparing `bc_time-7.0.1/src/bc_time/oauth2/token.py` & `bc_time-7.1.0/src/bc_time/oauth2/token.py`

 * *Files identical despite different names*

### Comparing `bc_time-7.0.1/src/bc_time/requests/base.py` & `bc_time-7.1.0/src/bc_time/requests/base.py`

 * *Files identical despite different names*

### Comparing `bc_time-7.0.1/src/bc_time/system/encryption/crypt.py` & `bc_time-7.1.0/src/bc_time/system/encryption/crypt.py`

 * *Files identical despite different names*

### Comparing `bc_time-7.0.1/src/bc_time.egg-info/PKG-INFO` & `bc_time-7.1.0/src/bc_time.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bc-time
-Version: 7.0.1
+Version: 7.1.0
 Summary: SDK that helps with integration via the Binary City Time API.
 Home-page: https://bitbucket.org/dburger/bc_time_api_sdk/src/master/
 Author: Darius Burger
 Author-email: darius@bcity.me
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -118,14 +118,15 @@
 * CompanyProfiles
 * Controllers
 * Departments
 * Devices
 * DailyOvertimeData
 * Employees
 * EmployeeLeave
+* PeriodOvertimeData
 * Settings
 * Visitors
 * VisitorGroups
 
 # Available methods
 
 ## For (most) objects
```

### Comparing `bc_time-7.0.1/src/bc_time.egg-info/SOURCES.txt` & `bc_time-7.1.0/src/bc_time.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 src/bc_time/api/objects/departments.py
 src/bc_time/api/objects/devices.py
 src/bc_time/api/objects/employee_leave.py
 src/bc_time/api/objects/employees.py
 src/bc_time/api/objects/group_base.py
 src/bc_time/api/objects/object_base_read.py
 src/bc_time/api/objects/object_base_write.py
+src/bc_time/api/objects/period_overtime_data.py
 src/bc_time/api/objects/settings.py
 src/bc_time/api/objects/visitor_groups.py
 src/bc_time/api/objects/visitors.py
 src/bc_time/oauth2/__init__.py
 src/bc_time/oauth2/token.py
 src/bc_time/oauth2/constants/__init__.py
 src/bc_time/oauth2/constants/grant_type.py
```

