# Comparing `tmp/common-test-29.9.20.tar.gz` & `tmp/common-test-29.9.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common-test-29.9.20.tar", last modified: Fri Apr 14 00:31:46 2023, max compression
+gzip compressed data, was "common-test-29.9.22.tar", last modified: Mon Apr 24 05:36:33 2023, max compression
```

## Comparing `common-test-29.9.20.tar` & `common-test-29.9.22.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-14 00:31:46.475943 common-test-29.9.20/
--rw-r--r--   0 edz        (502) staff       (20)      623 2023-04-14 00:31:46.476146 common-test-29.9.20/PKG-INFO
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-14 00:31:46.451749 common-test-29.9.20/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:20.000000 common-test-29.9.20/common/__init__.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-14 00:31:46.453202 common-test-29.9.20/common/autotest/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:14.000000 common-test-29.9.20/common/autotest/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     5939 2023-04-14 00:29:21.000000 common-test-29.9.20/common/autotest/base_requests.py
--rw-r--r--   0 edz        (502) staff       (20)     6429 2023-03-22 09:11:35.000000 common-test-29.9.20/common/autotest/handle_allure.py
--rw-r--r--   0 edz        (502) staff       (20)    10703 2023-04-14 00:29:21.000000 common-test-29.9.20/common/autotest/handle_assert.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-14 00:31:46.455106 common-test-29.9.20/common/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:39.000000 common-test-29.9.20/common/common/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2050 2023-04-14 00:29:21.000000 common-test-29.9.20/common/common/api_driver.py
--rw-r--r--   0 edz        (502) staff       (20)     3462 2023-04-14 00:29:21.000000 common-test-29.9.20/common/common/constant.py
--rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:21.000000 common-test-29.9.20/common/common/test.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-14 00:31:46.455813 common-test-29.9.20/common/config/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:55.000000 common-test-29.9.20/common/config/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2429 2022-12-01 00:35:04.000000 common-test-29.9.20/common/config/config.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-14 00:31:46.457088 common-test-29.9.20/common/data/
--rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:37.000000 common-test-29.9.20/common/data/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    16494 2023-04-07 07:27:39.000000 common-test-29.9.20/common/data/data_process.py
--rw-r--r--   0 edz        (502) staff       (20)     8693 2023-04-14 00:29:21.000000 common-test-29.9.20/common/data/handle_common.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-14 00:31:46.460120 common-test-29.9.20/common/db/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:55.000000 common-test-29.9.20/common/db/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     3436 2023-04-14 00:29:21.000000 common-test-29.9.20/common/db/handle_db.py
--rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:27.000000 common-test-29.9.20/common/db/handle_db_batch.py
--rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:21.000000 common-test-29.9.20/common/db/handle_mysqldb.py
--rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:21.000000 common-test-29.9.20/common/db/handle_oracle.py
--rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:21.000000 common-test-29.9.20/common/db/handle_sqlserver.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-14 00:31:46.462478 common-test-29.9.20/common/file/
--rw-r--r--   0 edz        (502) staff       (20)     4508 2023-04-14 00:29:21.000000 common-test-29.9.20/common/file/ReadFile.py
--rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:53.000000 common-test-29.9.20/common/file/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    11639 2023-04-14 00:29:21.000000 common-test-29.9.20/common/file/handle_excel.py
--rw-r--r--   0 edz        (502) staff       (20)     2265 2023-04-14 00:29:21.000000 common-test-29.9.20/common/file/handle_file.py
--rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:21.000000 common-test-29.9.20/common/file/handle_reques.py
--rw-r--r--   0 edz        (502) staff       (20)     2201 2022-10-24 01:09:23.000000 common-test-29.9.20/common/file/handle_system.py
--rw-r--r--   0 edz        (502) staff       (20)     1000 2023-04-14 00:29:21.000000 common-test-29.9.20/common/file/handle_yaml.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-14 00:31:46.463028 common-test-29.9.20/common/mq/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:55.000000 common-test-29.9.20/common/mq/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:21.000000 common-test-29.9.20/common/mq/handle_rabbit.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-14 00:31:46.465066 common-test-29.9.20/common/plat/
--rw-r--r--   0 edz        (502) staff       (20)    12849 2023-04-14 00:29:21.000000 common-test-29.9.20/common/plat/ATF_platform.py
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:13.000000 common-test-29.9.20/common/plat/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:42.000000 common-test-29.9.20/common/plat/jenkin_platform.py
--rw-r--r--   0 edz        (502) staff       (20)    15697 2023-04-14 00:29:21.000000 common-test-29.9.20/common/plat/jira_platform.py
--rw-r--r--   0 edz        (502) staff       (20)    13513 2023-04-14 00:29:21.000000 common-test-29.9.20/common/plat/mysql_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     1056 2023-04-14 00:29:21.000000 common-test-29.9.20/common/plat/service_platform.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-14 00:31:46.471472 common-test-29.9.20/common/plugin/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:42.000000 common-test-29.9.20/common/plugin/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1330 2023-01-16 07:33:57.000000 common-test-29.9.20/common/plugin/allure_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     2054 2022-07-28 02:48:03.000000 common-test-29.9.20/common/plugin/assert_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     7574 2023-04-14 00:29:21.000000 common-test-29.9.20/common/plugin/atf_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     5988 2023-04-14 00:29:21.000000 common-test-29.9.20/common/plugin/data_bus.py
--rw-r--r--   0 edz        (502) staff       (20)     3009 2023-04-14 00:29:21.000000 common-test-29.9.20/common/plugin/data_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     9624 2023-04-14 00:29:21.000000 common-test-29.9.20/common/plugin/file_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:18.000000 common-test-29.9.20/common/plugin/hooks_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    13093 2023-01-16 07:46:45.000000 common-test-29.9.20/common/plugin/pytest_playwright.py
--rw-r--r--   0 edz        (502) staff       (20)    15927 2023-04-14 00:29:21.000000 common-test-29.9.20/common/plugin/pytest_plugin.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-14 00:31:46.475414 common-test-29.9.20/common_test.egg-info/
--rw-r--r--   0 edz        (502) staff       (20)      623 2023-04-14 00:31:46.000000 common-test-29.9.20/common_test.egg-info/PKG-INFO
--rw-r--r--   0 edz        (502) staff       (20)     1475 2023-04-14 00:31:46.000000 common-test-29.9.20/common_test.egg-info/SOURCES.txt
--rw-r--r--   0 edz        (502) staff       (20)        1 2023-04-14 00:31:46.000000 common-test-29.9.20/common_test.egg-info/dependency_links.txt
--rw-r--r--   0 edz        (502) staff       (20)       57 2023-04-14 00:31:46.000000 common-test-29.9.20/common_test.egg-info/entry_points.txt
--rw-r--r--   0 edz        (502) staff       (20)      560 2023-04-14 00:31:46.000000 common-test-29.9.20/common_test.egg-info/requires.txt
--rw-r--r--   0 edz        (502) staff       (20)        7 2023-04-14 00:31:46.000000 common-test-29.9.20/common_test.egg-info/top_level.txt
--rw-r--r--   0 edz        (502) staff       (20)      440 2023-04-14 00:31:46.477186 common-test-29.9.20/setup.cfg
--rw-r--r--   0 edz        (502) staff       (20)     1621 2023-04-11 07:05:24.000000 common-test-29.9.20/setup.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-24 05:36:33.574927 common-test-29.9.22/
+-rw-r--r--   0 edz        (502) staff       (20)      623 2023-04-24 05:36:33.575057 common-test-29.9.22/PKG-INFO
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-24 05:36:33.548661 common-test-29.9.22/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 common-test-29.9.22/common/__init__.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-24 05:36:33.550206 common-test-29.9.22/common/autotest/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 common-test-29.9.22/common/autotest/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     5993 2023-04-23 00:57:35.000000 common-test-29.9.22/common/autotest/base_requests.py
+-rw-r--r--   0 edz        (502) staff       (20)     6429 2023-03-22 09:11:00.000000 common-test-29.9.22/common/autotest/handle_allure.py
+-rw-r--r--   0 edz        (502) staff       (20)    10703 2023-04-14 00:29:00.000000 common-test-29.9.22/common/autotest/handle_assert.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-24 05:36:33.555089 common-test-29.9.22/common/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 common-test-29.9.22/common/common/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2126 2023-04-23 02:46:40.000000 common-test-29.9.22/common/common/api_driver.py
+-rw-r--r--   0 edz        (502) staff       (20)     3462 2023-04-14 00:29:00.000000 common-test-29.9.22/common/common/constant.py
+-rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 common-test-29.9.22/common/common/test.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-24 05:36:33.556773 common-test-29.9.22/common/config/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.22/common/config/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2429 2022-12-01 00:35:00.000000 common-test-29.9.22/common/config/config.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-24 05:36:33.559783 common-test-29.9.22/common/data/
+-rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 common-test-29.9.22/common/data/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    17498 2023-04-24 05:17:14.000000 common-test-29.9.22/common/data/data_process.py
+-rw-r--r--   0 edz        (502) staff       (20)     8662 2023-04-23 07:58:21.000000 common-test-29.9.22/common/data/handle_common.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-24 05:36:33.562447 common-test-29.9.22/common/db/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.22/common/db/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     3436 2023-04-14 00:29:00.000000 common-test-29.9.22/common/db/handle_db.py
+-rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 common-test-29.9.22/common/db/handle_db_batch.py
+-rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 common-test-29.9.22/common/db/handle_mysqldb.py
+-rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 common-test-29.9.22/common/db/handle_oracle.py
+-rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 common-test-29.9.22/common/db/handle_sqlserver.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-24 05:36:33.565445 common-test-29.9.22/common/file/
+-rw-r--r--   0 edz        (502) staff       (20)     4508 2023-04-14 00:29:00.000000 common-test-29.9.22/common/file/ReadFile.py
+-rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 common-test-29.9.22/common/file/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    11930 2023-04-24 05:17:14.000000 common-test-29.9.22/common/file/handle_excel.py
+-rw-r--r--   0 edz        (502) staff       (20)     2265 2023-04-14 00:29:00.000000 common-test-29.9.22/common/file/handle_file.py
+-rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 common-test-29.9.22/common/file/handle_reques.py
+-rw-r--r--   0 edz        (502) staff       (20)     2201 2022-10-24 01:09:00.000000 common-test-29.9.22/common/file/handle_system.py
+-rw-r--r--   0 edz        (502) staff       (20)     1000 2023-04-14 00:29:00.000000 common-test-29.9.22/common/file/handle_yaml.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-24 05:36:33.566063 common-test-29.9.22/common/mq/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.22/common/mq/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 common-test-29.9.22/common/mq/handle_rabbit.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-24 05:36:33.568243 common-test-29.9.22/common/plat/
+-rw-r--r--   0 edz        (502) staff       (20)    12849 2023-04-14 00:29:00.000000 common-test-29.9.22/common/plat/ATF_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 common-test-29.9.22/common/plat/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 common-test-29.9.22/common/plat/jenkin_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)    15697 2023-04-14 00:29:00.000000 common-test-29.9.22/common/plat/jira_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)    13513 2023-04-14 00:29:00.000000 common-test-29.9.22/common/plat/mysql_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     1056 2023-04-14 00:29:00.000000 common-test-29.9.22/common/plat/service_platform.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-24 05:36:33.572376 common-test-29.9.22/common/plugin/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 common-test-29.9.22/common/plugin/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1330 2023-01-16 07:33:00.000000 common-test-29.9.22/common/plugin/allure_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     2054 2022-07-28 02:48:00.000000 common-test-29.9.22/common/plugin/assert_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     7574 2023-04-14 00:29:00.000000 common-test-29.9.22/common/plugin/atf_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     5988 2023-04-14 00:29:00.000000 common-test-29.9.22/common/plugin/data_bus.py
+-rw-r--r--   0 edz        (502) staff       (20)     3908 2023-04-23 08:05:34.000000 common-test-29.9.22/common/plugin/data_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    11219 2023-04-24 05:18:09.000000 common-test-29.9.22/common/plugin/file_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 common-test-29.9.22/common/plugin/hooks_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    13093 2023-01-16 07:46:00.000000 common-test-29.9.22/common/plugin/pytest_playwright.py
+-rw-r--r--   0 edz        (502) staff       (20)    15927 2023-04-14 00:29:00.000000 common-test-29.9.22/common/plugin/pytest_plugin.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-04-24 05:36:33.574618 common-test-29.9.22/common_test.egg-info/
+-rw-r--r--   0 edz        (502) staff       (20)      623 2023-04-24 05:36:33.000000 common-test-29.9.22/common_test.egg-info/PKG-INFO
+-rw-r--r--   0 edz        (502) staff       (20)     1475 2023-04-24 05:36:33.000000 common-test-29.9.22/common_test.egg-info/SOURCES.txt
+-rw-r--r--   0 edz        (502) staff       (20)        1 2023-04-24 05:36:33.000000 common-test-29.9.22/common_test.egg-info/dependency_links.txt
+-rw-r--r--   0 edz        (502) staff       (20)       57 2023-04-24 05:36:33.000000 common-test-29.9.22/common_test.egg-info/entry_points.txt
+-rw-r--r--   0 edz        (502) staff       (20)      571 2023-04-24 05:36:33.000000 common-test-29.9.22/common_test.egg-info/requires.txt
+-rw-r--r--   0 edz        (502) staff       (20)        7 2023-04-24 05:36:33.000000 common-test-29.9.22/common_test.egg-info/top_level.txt
+-rw-r--r--   0 edz        (502) staff       (20)      440 2023-04-24 05:36:33.575783 common-test-29.9.22/setup.cfg
+-rw-r--r--   0 edz        (502) staff       (20)     1641 2023-04-24 05:34:13.000000 common-test-29.9.22/setup.py
```

### Comparing `common-test-29.9.20/PKG-INFO` & `common-test-29.9.22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-test
-Version: 29.9.20
+Version: 29.9.22
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `common-test-29.9.20/common/autotest/base_requests.py` & `common-test-29.9.22/common/autotest/base_requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
                 data = DataProcess.handle_data(data, False)
         except Exception as e:
             logger.info(f'测试数据：{data} 转换异常:' + repr(e))
         file = DataProcess.handler_files(file_obj)
         desc = f'测试接口详情:{url}'
         # 发送请求
         res = cls.http_request(url=url, method=method, parametric_key=parametric_key,
-                               header=header, data=data, file=file, desc=desc)
+                               header=DataProcess.setDictEncode(header), data=data, file=file, desc=desc)
         try:
             if DataProcess.isNotNull(get_system_key(Constant.RUN_TYPE)):
                 MysqlPlatForm.insert_api_data(url, method, header, data, res.elapsed.total_seconds(), res.status_code)
         except:
             logger.warning("保存请求数据异常")
         # 响应后操作
         if token == '写':
@@ -95,15 +95,15 @@
                 data = DataProcess.handle_data(data, False)
         except Exception as e:
             logger.info(f'测试数据：{data} 转换异常:' + repr(e))
         file_obj = DataProcess.handler_files(file)
         if step == '测试接口详情' and DataProcess.isNotNull(schemal_data['desc']):
             step = '测试接口详情:'+schemal_data['desc']
         res = cls.http_request(url=url, method=schemal_data['method'], parametric_key=schemal_data['datatype'],
-                               header=header, data=data, file=file_obj, cookie=cookie, desc=step)
+                               header=DataProcess.setDictEncode(header), data=data, file=file_obj, cookie=cookie, desc=step)
         try:
             if DataProcess.isNotNull(get_system_key(Constant.RUN_TYPE)):
                 MysqlPlatForm.insert_api_data(url, schemal_data['method'], header, data, res.elapsed.total_seconds(), res.status_code)
         except:
             logger.warning("保存请求数据异常")
         return res
```

### Comparing `common-test-29.9.20/common/autotest/handle_allure.py` & `common-test-29.9.22/common/autotest/handle_allure.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/autotest/handle_assert.py` & `common-test-29.9.22/common/autotest/handle_assert.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/common/api_driver.py` & `common-test-29.9.22/common/common/api_driver.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
         """
         :param method: 请求方法
         :param url: 请求url
         :param parametric_key: 入参关键字， params(查询参数类型，明文传输，一般在url?参数名=参数值), data(一般用于form表单类型参数)
         json(一般用于json类型请求参数)
         :param data: 参数数据，默认等于None
         :param file: 文件对象
+        :param desc: 自动化测试过程请求描述：打印到Report中
         :param header: 请求头
         :return: 返回res对象
         """
         session = cls.get_session()
         if parametric_key is None:
             res = session.request(method=method, url=url, headers=header, cookies=cookie, auth=_auth)
             allure_api_step(desc, url, method, header, '', '', res)
```

### Comparing `common-test-29.9.20/common/common/constant.py` & `common-test-29.9.22/common/common/constant.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/common/test.py` & `common-test-29.9.22/common/common/test.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/config/config.py` & `common-test-29.9.22/common/config/config.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/data/data_process.py` & `common-test-29.9.22/common/data/data_process.py`

 * *Files 4% similar despite different names*

```diff
@@ -150,17 +150,20 @@
             if isinstance(_template, list):
                 for _index in range(len(_template)):
                     _template[_index] = cls.handle_data_fromat(_template[_index], data, _no_content, _dataType)
                 return _template
             else:
                 if isinstance(_template, dict):
                     for key in _template.keys():
-                        _template[key] = cls.handle_data_fromat(_template[key], data, _no_content, _dataType)
+                        if key.find('$') != 0:
+                            _template[key] = cls.handle_data_fromat(_template[key], data, _no_content, _dataType)
                 return _template
 
+
+
     @classmethod
     def handle_data(cls, variable: str, jsonformat:bool=True) -> dict:
         """请求数据处理
         :param variable: 请求数据，传入的是可转换字典/json的字符串,其中可以包含变量表达式
         return 处理之后的json/dict类型的字典数据
         """
         if variable == '':
@@ -385,16 +388,46 @@
                     scriptmethod = scrtpArr[0]
             scriptname = get_system_key(Constant.CURRENT_PATH) + os.sep + caseArr[0]
             return testname,gitname,scripturl, scriptclass, scriptmethod, scriptname
         except Exception as e:
             logger.info(f'解析用例脚本路径URL：用例名称:{testname} 脚本路径:{caseurl} 异常信息：{e}')
             return testname, "", "", "", "",""
 
+    @classmethod
+    def is_contain_chinese(self, check_str):
+        """
+        判断字符串中是否包含中文
+        :param check_str: {str} 需要检测的字符串
+        :return: {bool} 包含返回True， 不包含返回False
+        """
+        for ch in check_str:
+            if u'\u4e00' <= ch <= u'\u9fff':
+                return True
+        return False
+
+    @classmethod
+    def setDictEncode(self, dict):
+        """
+        处理header中的特殊字符串 空格、int、float、中文
+        :param dict:
+        :return:
+        """
+        for key, value in dict.items():
+            if value == " ":
+                dict[key] = ""
+            if type(value) == type(1):
+                dict[key] = str(value)
+                continue
+            if type(value) == type(1.2):
+                dict[key] = str(value)
+                continue
+            if self.is_contain_chinese(value):
+                dict[key] = value.encode('UTF-8')
+        return dict
+
 
 if __name__ == '__main__':
-    aa="cell388334_cell"
-    print(aa.find('cell'))
-    print(aa)
+    print('_11'.find('__'))
```

### Comparing `common-test-29.9.20/common/data/handle_common.py` & `common-test-29.9.22/common/data/handle_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
     :param data: 在该项目中一般为响应字典，从字典取值出来
     :param expr: 查找用的正则表达式
     return content： 替换表达式后的字符串
     """
     if isinstance(content, str):
         content = content.replace('\\', '')
     else:
-        content = str(content)
         content = str(content).replace('\\', '')
 
     for i in re.findall(expr, content):
         if i.find(".") >= 0:
             from common.plugin.data_bus import DataBus
             _content = DataBus.get_key(i)
```

### Comparing `common-test-29.9.20/common/db/handle_db.py` & `common-test-29.9.22/common/db/handle_db.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/db/handle_db_batch.py` & `common-test-29.9.22/common/db/handle_db_batch.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/db/handle_mysqldb.py` & `common-test-29.9.22/common/db/handle_mysqldb.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/db/handle_oracle.py` & `common-test-29.9.22/common/db/handle_oracle.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/db/handle_sqlserver.py` & `common-test-29.9.22/common/db/handle_sqlserver.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/file/ReadFile.py` & `common-test-29.9.22/common/file/ReadFile.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/file/handle_excel.py` & `common-test-29.9.22/common/file/handle_excel.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,15 +193,15 @@
     exlSpace = sh.merged_cells.ranges
 
     for spaceData in exlSpace:
         datavalue = spaceData.start_cell.value
         # print(datavalue)
         return datavalue
 
-def excel_to_list(data_file, sheet,_index:int=1,_filter:dict=None, _replace: bool=True):
+def excel_to_list(data_file, sheet,_index:int=1,_filter:dict=None, _replace: bool=True, _checkData:bool=True):
     """
     读取Excel中特定sheet的数据，按行将数据存入数组datalist
     :param data_file:Excel文件目录
     :param sheet:需要读取的sheet名称
     :return:datalist
     """
     data_file = adjust_path_data(data_file)
@@ -213,70 +213,75 @@
     # 跳过标题行，从第二行开始取数据
     _mysql = None
     if DataProcess.isNotNull(get_system_key(Constant.TEST_SRTCYCLE_ID)):
         _config = {'key': 'traffic', 'env': 'test'}
         _mysql = MysqlDB(_config)
     for row in range(_index, sh.nrows):
         d = dict()
-        d['_excelPath'] = data_file
-        d['_sheetName'] = sheet
         # 将标题和每行数据组装成字典
         for col in range(0, sh.ncols):
             # 获取指定单元格数据(行，列)
             cell_data = sh.cell_value(row, col)
             ctype = sh.cell(row, col).ctype
             if ctype == 2 and cell_data % 1 == 0.0:
                 cell_data = int(cell_data)
             if ctype == 3:
                 date = datetime(*xldate_as_tuple(cell_data, 0))
                 cell_data = date.strftime('%Y-%m-%d')
             col_title = sh.cell_value(0, col).strip()
             d[col_title] = cell_data
+            d['$'+col_title] = cell_data
             d[col_title+'_cell'] = {"row": row, "col": col}
-        #d = dict(zip(header, sh.row_values(i)))
-        if check_excel_data(d, _mysql, _filter):
+        if check_excel_data(d, _mysql, _filter, _checkData):
             if _replace:
                 temp = DataBus.get_data(d)
+                temp['_excelPath'] = data_file
+                temp['_sheetName'] = sheet
             else:
                 temp = d
+                temp['_excelPath'] = data_file
+                temp['_sheetName'] = sheet
             print_info(f'添加单个参数化用例数据: {temp}')
             data_list.append(temp)
-    if DataProcess.isNotNull(get_system_key(Constant.TEST_SRTCYCLE_ID)):
-        _mysql.close()
-    print_info(f'用例参数化数据: {data_list}')
+        if DataProcess.isNotNull(get_system_key(Constant.TEST_SRTCYCLE_ID)):
+            _mysql.close()
+        print_info(f'用例参数化数据: {data_list}')
     return data_list
 
-def check_excel_data(testdata:dict, _mysql, _filter):
-    casename = format_caseName(testdata[Constant.CASE_TITLE])
-    caseNo = testdata[Constant.CASE_NO]
-    if DataProcess.isNotNull(get_system_key('type')) and get_system_key('type').strip() == '脚本同步':
-        return True
-    if DataProcess.isNotNull(casename) == False or DataProcess.isNotNull(caseNo) == False:
-        return False
-    if DataProcess.isNotNull(get_system_key(Constant.TEST_SRTCYCLE_ID)) and _mysql is not None:
-        cycleId = get_system_key(Constant.TEST_SRTCYCLE_ID)
-        _sql = f"select * from `traffic_test`.`test_autotest_run` where `status` = '{Constant.STATUS_PRE}' and cycleId='{cycleId}' and casename='{casename}'"
-        _info = _mysql.execute(_sql).fetchall()
-        if len(_info) < 1:
-            _sql = f"select * from `traffic_test`.`test_autotest_run` where `status` = '{Constant.STATUS_PRE}' and cycleId='{cycleId}' and caseid='{caseNo}'"
-            _info = _mysql.execute(_sql).fetchall()
-        if len(_info) < 1:
-            return False
-        else:
-            _temp = _info[0]
-            logger.info(f"执行参数化用例编号:{_temp['caseid']} 用例名称：{_temp['casename']}  运行ID:{_temp['caserunid']} ")
-            print_info(f'执行参数化测试数据: {testdata}')
-            return True
-    if testdata[Constant.CASE_STATUS].strip() == '否':
-        return False
-    if DataProcess.isNotNull(get_system_key(Constant.TEST_CASE_NAME_LIST)):
-        if testdata[Constant.CASE_TITLE] in eval(get_system_key(Constant.TEST_CASE_NAME_LIST)):
+
+
+def check_excel_data(testdata:dict, _mysql, _filter, _checkData):
+    if _checkData:
+        casename = format_caseName(testdata[Constant.CASE_TITLE])
+        caseNo = testdata[Constant.CASE_NO]
+        if DataProcess.isNotNull(get_system_key('type')) and get_system_key('type').strip() == '脚本同步':
             return True
-        else:
+        if DataProcess.isNotNull(casename) == False or DataProcess.isNotNull(caseNo) == False:
             return False
+        if DataProcess.isNotNull(get_system_key(Constant.TEST_SRTCYCLE_ID)) and _mysql is not None:
+            cycleId = get_system_key(Constant.TEST_SRTCYCLE_ID)
+            _sql = f"select * from `traffic_test`.`test_autotest_run` where `status` = '{Constant.STATUS_PRE}' and cycleId='{cycleId}' and casename='{casename}'"
+            _info = _mysql.execute(_sql).fetchall()
+            if len(_info) < 1:
+                _sql = f"select * from `traffic_test`.`test_autotest_run` where `status` = '{Constant.STATUS_PRE}' and cycleId='{cycleId}' and caseid='{caseNo}'"
+                _info = _mysql.execute(_sql).fetchall()
+            if len(_info) < 1:
+                return False
+            else:
+                _temp = _info[0]
+                logger.info(f"执行参数化用例编号:{_temp['caseid']} 用例名称：{_temp['casename']}  运行ID:{_temp['caserunid']} ")
+                print_info(f'执行参数化测试数据: {testdata}')
+                return True
+        if testdata[Constant.CASE_STATUS].strip() == '否':
+            return False
+        if DataProcess.isNotNull(get_system_key(Constant.TEST_CASE_NAME_LIST)):
+            if testdata[Constant.CASE_TITLE] in eval(get_system_key(Constant.TEST_CASE_NAME_LIST)):
+                return True
+            else:
+                return False
     if DataProcess.isNotNull(_filter):
         for k, v in _filter.items():
             if testdata[k] == v:
                 return True
         return False
     return True
```

### Comparing `common-test-29.9.20/common/file/handle_file.py` & `common-test-29.9.22/common/file/handle_file.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/file/handle_reques.py` & `common-test-29.9.22/common/file/handle_reques.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/file/handle_system.py` & `common-test-29.9.22/common/file/handle_system.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/file/handle_yaml.py` & `common-test-29.9.22/common/file/handle_yaml.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/mq/handle_rabbit.py` & `common-test-29.9.22/common/mq/handle_rabbit.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/plat/ATF_platform.py` & `common-test-29.9.22/common/plat/ATF_platform.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/plat/jenkin_platform.py` & `common-test-29.9.22/common/plat/jenkin_platform.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/plat/jira_platform.py` & `common-test-29.9.22/common/plat/jira_platform.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/plat/mysql_platform.py` & `common-test-29.9.22/common/plat/mysql_platform.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/plat/service_platform.py` & `common-test-29.9.22/common/plat/service_platform.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/plugin/allure_plugin.py` & `common-test-29.9.22/common/plugin/allure_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/plugin/assert_plugin.py` & `common-test-29.9.22/common/plugin/assert_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/plugin/atf_plugin.py` & `common-test-29.9.22/common/plugin/atf_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/plugin/data_bus.py` & `common-test-29.9.22/common/plugin/data_bus.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/plugin/file_plugin.py` & `common-test-29.9.22/common/plugin/file_plugin.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,15 +20,50 @@
         """
            读取Excel中特定sheet的数据，按行将数据存入数组datalist[从第二行开始读数据】
            :param data_file:Excel文件目录
            :param sheet:需要读取的sheet名称
            :return:datalist
            """
         DataBus.save_init_data()
-        return excel_to_list(path.join(file_path, file_name), sheet, _index, _filter, _replace)
+        _list = excel_to_list(path.join(file_path, file_name), sheet, _index, _filter, _replace)
+        for _temp in _list:
+            for key in _temp.keys():
+                name, _sheet, _filter = self.handle_excel_data(_temp[key],file_name,sheet)
+                if DataProcess.isNotNull(name):
+                    _subData = excel_to_list(path.join(file_path, file_name), _sheet, _index, _filter, _replace, _checkData=False)
+                    if _subData.__len__() > 0:
+                        _temp[key] = _subData[0]
+                        _temp["$"+key] = _subData
+        return _list
+
+    @classmethod
+    def handle_excel_data(self, _str:str, _fileName:str, _sheetName:str):
+        """
+        处理Excel数据格式$[excel文件名称.SheetName.fileter==1]
+        """
+        if isinstance(_str, str) and _str.find('$[') >= 0:
+            _str = _str.replace('$[',"").replace(']',"")
+            _arr = _str.split('==')
+            _sub= _arr[0].split('.')
+            if _sub.__len__() == 3:
+                _fileName = _sub[0]
+                _sheetName = _sub[1]
+                _fileter = {_sub[2]:_arr[1]}
+            if  _sub.__len__() == 2:
+                _fileName = _fileName
+                _sheetName = _sub[0]
+                _fileter = {_sub[1]:_arr[1]}
+            if _sub.__len__() == 1:
+                _fileName = _fileName
+                _sheetName = _sheetName
+                _fileter = {_sub[0]:_arr[1]}
+            return _fileName,_sheetName,_fileter
+        else:
+            return "","",""
+
 
     @classmethod
     def write_case_data(self, item: dict, key, value):
         """
          回填测试数据到Excel中
                    :param data_file:Excel文件目录
                    :param sheet:需要读取的sheet名称
@@ -260,16 +295,23 @@
             if _dict[Constant.CASE_TITLE] in _mark:
                 _flag = True
             else:
                 _flag = False
         return _flag
 
 
+
 if __name__ == '__main__':
-    str="['aa','bb']"
+    _xml=FilePlugin.excel_to_dict("data.xls",sheet="Sheet1",_filter={'需求名称':'bocc上传提交'})
+    print(_xml[0].get('$上传文件')[2].get('用例编号'))
+
+
+
+
+
```

### Comparing `common-test-29.9.20/common/plugin/hooks_plugin.py` & `common-test-29.9.22/common/plugin/hooks_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/plugin/pytest_playwright.py` & `common-test-29.9.22/common/plugin/pytest_playwright.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common/plugin/pytest_plugin.py` & `common-test-29.9.22/common/plugin/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common_test.egg-info/PKG-INFO` & `common-test-29.9.22/common_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-test
-Version: 29.9.20
+Version: 29.9.22
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `common-test-29.9.20/common_test.egg-info/SOURCES.txt` & `common-test-29.9.22/common_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `common-test-29.9.20/common_test.egg-info/requires.txt` & `common-test-29.9.22/common_test.egg-info/requires.txt`

 * *Files 23% similar despite different names*

```diff
@@ -25,7 +25,8 @@
 deepdiff==5.8.1
 dnspython==2.2.1
 jsonschema==4.17.0
 xmlschema==1.0.14
 pymongo==3.5.1
 redis-py-cluster==2.1.3
 redis==3.5.3
+bs4==0.0.1
```

### Comparing `common-test-29.9.20/setup.py` & `common-test-29.9.22/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,16 +30,17 @@
         "assertpy==1.1",
         "deepdiff==5.8.1",
         "dnspython==2.2.1",
         "jsonschema==4.17.0",
         "xmlschema==1.0.14",
         "pymongo==3.5.1",
         "redis-py-cluster==2.1.3",
-        "redis==3.5.3"
-        # "selenium==4.6.0",
+        "redis==3.5.3",
+        #"ddddocr==1.4.7",
+        "bs4==0.0.1"
     ],
     entry_points={"pytest11": ["playwright = common.plugin.pytest_playwright"]},
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

