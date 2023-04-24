# Comparing `tmp/python_selenium_ctrl_package-0.0.97.tar.gz` & `tmp/python_selenium_ctrl_package-0.0.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_selenium_ctrl_package-0.0.97.tar", last modified: Thu Apr 20 08:35:03 2023, max compression
+gzip compressed data, was "python_selenium_ctrl_package-0.0.98.tar", last modified: Mon Apr 24 02:25:27 2023, max compression
```

## Comparing `python_selenium_ctrl_package-0.0.97.tar` & `python_selenium_ctrl_package-0.0.98.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 08:35:03.015519 python_selenium_ctrl_package-0.0.97/
--rw-rw-rw-   0        0        0     1061 2022-11-15 08:59:32.000000 python_selenium_ctrl_package-0.0.97/LICENSE
--rw-rw-rw-   0        0        0     1172 2023-04-20 08:35:03.015519 python_selenium_ctrl_package-0.0.97/PKG-INFO
--rw-rw-rw-   0        0        0      681 2023-04-19 08:10:05.000000 python_selenium_ctrl_package-0.0.97/README.md
--rw-rw-rw-   0        0        0      942 2023-04-20 08:34:41.000000 python_selenium_ctrl_package-0.0.97/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-20 08:35:03.015519 python_selenium_ctrl_package-0.0.97/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-20 08:35:02.848016 python_selenium_ctrl_package-0.0.97/src/
--rw-rw-rw-   0        0        0        0 2022-11-18 06:36:28.000000 python_selenium_ctrl_package-0.0.97/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 08:35:02.863641 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/
--rw-rw-rw-   0        0        0        0 2022-11-17 01:43:31.000000 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 08:35:02.894883 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/conf/
--rw-rw-rw-   0        0        0        0 2022-11-21 09:26:54.000000 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/conf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 08:35:02.894883 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/conf/app/
--rw-rw-rw-   0        0        0        0 2022-11-21 09:42:24.000000 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/conf/app/__init__.py
--rw-rw-rw-   0        0        0       90 2022-10-07 06:37:19.000000 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/conf/app/ports_conf.py
--rw-rw-rw-   0        0        0      166 2022-10-07 06:37:19.000000 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/conf/product_list.py
-drwxrwxrwx   0        0        0        0 2023-04-20 08:35:02.894883 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/conf/rwd/
-drwxrwxrwx   0        0        0        0 2023-04-20 08:35:02.910512 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/conf/rwd/Website/
--rw-rw-rw-   0        0        0        0 2022-11-21 09:27:37.000000 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/conf/rwd/Website/__init__.py
--rw-rw-rw-   0        0        0      153 2022-10-07 06:37:19.000000 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/conf/rwd/Website/base_url_conf.py
--rw-rw-rw-   0        0        0      104 2022-10-07 06:37:19.000000 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/conf/rwd/Website/opera_browser_conf.py
--rw-rw-rw-   0        0        0        0 2022-11-21 09:27:06.000000 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/conf/rwd/__init__.py
--rw-rw-rw-   0        0        0    41277 2023-04-19 07:45:54.000000 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/conftest_base.py
-drwxrwxrwx   0        0        0        0 2023-04-20 08:35:02.910512 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/drivers/
--rw-rw-rw-   0        0        0        0 2022-11-21 09:11:03.000000 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/drivers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 08:35:02.932712 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/drivers/browsers/
--rw-rw-rw-   0        0        0        0 2022-11-21 09:11:28.000000 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/drivers/browsers/__init__.py
--rw-rw-rw-   0        0        0     3897 2022-12-07 03:55:17.000000 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/drivers/browsers/browser_os_name_conf.py
--rw-rw-rw-   0        0        0     3471 2023-04-19 07:45:54.000000 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/drivers/browsers/local_browsers.py
--rw-rw-rw-   0        0        0     5926 2022-11-21 10:05:25.000000 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/drivers/browsers/remote_options.py
--rw-rw-rw-   0        0        0    16954 2023-04-19 08:09:13.000000 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/drivers/driverfactory.py
--rw-rw-rw-   0        0        0      544 2022-11-14 01:59:19.000000 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/main.py
-drwxrwxrwx   0        0        0        0 2023-04-20 08:35:02.952989 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/pages/
--rw-rw-rw-   0        0        0    57659 2023-04-19 07:45:54.000000 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/pages/Base_Page.py
--rw-rw-rw-   0        0        0    25414 2023-04-20 08:32:17.000000 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/pages/Mobile_Base_Page.py
--rw-rw-rw-   0        0        0        0 2022-11-18 06:45:15.000000 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/pages/__init__.py
--rw-rw-rw-   0        0        0      370 2022-11-30 02:56:37.000000 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/pages/mobile_zero_page.py
--rw-rw-rw-   0        0        0      422 2022-11-30 02:10:57.000000 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/pages/zero_page.py
-drwxrwxrwx   0        0        0        0 2023-04-20 08:35:02.952989 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/remoteTest/
--rw-rw-rw-   0        0        0     3816 2022-11-30 06:10:04.000000 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/remoteTest/BrowserStack_Library.py
--rw-rw-rw-   0        0        0        0 2022-11-21 08:57:28.000000 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/remoteTest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 08:35:02.984242 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/utils/
--rw-rw-rw-   0        0        0        0 2022-11-21 08:39:02.000000 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/utils/__init__.py
--rw-rw-rw-   0        0        0      874 2023-01-04 03:46:28.000000 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/utils/email_conf.py
-drwxrwxrwx   0        0        0        0 2023-04-20 08:35:03.015519 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/utils/general/
--rw-rw-rw-   0        0        0     4915 2023-03-23 09:33:36.000000 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/utils/general/Base_Logging.py
--rw-rw-rw-   0        0        0      723 2022-10-07 06:37:19.000000 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/utils/general/Gif_Maker.py
--rw-rw-rw-   0        0        0     8968 2023-04-11 08:09:09.000000 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/utils/general/Wrapit.py
--rw-rw-rw-   0        0        0        0 2022-11-21 08:39:31.000000 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/utils/general/__init__.py
--rw-rw-rw-   0        0        0     9380 2023-01-04 06:33:56.000000 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/utils/general/email_pytest_report.py
--rw-rw-rw-   0        0        0      379 2022-10-07 06:37:19.000000 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/utils/general/stop_test_exception_util.py
--rw-rw-rw-   0        0        0       19 2022-10-12 03:37:41.000000 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/utils/html_report_conf.py
--rw-rw-rw-   0        0        0      227 2022-10-07 06:37:19.000000 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/utils/remote_credentials.py
--rw-rw-rw-   0        0        0       28 2022-11-29 09:59:41.000000 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/utils/screenshot_conf.py
-drwxrwxrwx   0        0        0        0 2023-04-20 08:35:02.879223 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package.egg-info/
--rw-rw-rw-   0        0        0     1172 2023-04-20 08:35:02.000000 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2378 2023-04-20 08:35:02.000000 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 08:35:02.000000 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      272 2023-04-20 08:35:02.000000 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       38 2023-04-20 08:35:02.000000 python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 02:25:27.606095 python_selenium_ctrl_package-0.0.98/
+-rw-rw-rw-   0        0        0     1061 2022-11-15 08:59:32.000000 python_selenium_ctrl_package-0.0.98/LICENSE
+-rw-rw-rw-   0        0        0     1172 2023-04-24 02:25:27.606095 python_selenium_ctrl_package-0.0.98/PKG-INFO
+-rw-rw-rw-   0        0        0      681 2023-04-19 08:10:05.000000 python_selenium_ctrl_package-0.0.98/README.md
+-rw-rw-rw-   0        0        0      942 2023-04-24 02:25:06.000000 python_selenium_ctrl_package-0.0.98/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-24 02:25:27.606095 python_selenium_ctrl_package-0.0.98/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-24 02:25:27.400556 python_selenium_ctrl_package-0.0.98/src/
+-rw-rw-rw-   0        0        0        0 2022-11-18 06:36:28.000000 python_selenium_ctrl_package-0.0.98/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 02:25:27.419555 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/
+-rw-rw-rw-   0        0        0        0 2022-11-17 01:43:31.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 02:25:27.448606 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/conf/
+-rw-rw-rw-   0        0        0        0 2022-11-21 09:26:54.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/conf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 02:25:27.456630 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/conf/app/
+-rw-rw-rw-   0        0        0        0 2022-11-21 09:42:24.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/conf/app/__init__.py
+-rw-rw-rw-   0        0        0       90 2022-10-07 06:37:19.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/conf/app/ports_conf.py
+-rw-rw-rw-   0        0        0      166 2022-10-07 06:37:19.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/conf/product_list.py
+drwxrwxrwx   0        0        0        0 2023-04-24 02:25:27.457585 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/conf/rwd/
+drwxrwxrwx   0        0        0        0 2023-04-24 02:25:27.473586 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/conf/rwd/Website/
+-rw-rw-rw-   0        0        0        0 2022-11-21 09:27:37.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/conf/rwd/Website/__init__.py
+-rw-rw-rw-   0        0        0      153 2022-10-07 06:37:19.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/conf/rwd/Website/base_url_conf.py
+-rw-rw-rw-   0        0        0      104 2022-10-07 06:37:19.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/conf/rwd/Website/opera_browser_conf.py
+-rw-rw-rw-   0        0        0        0 2022-11-21 09:27:06.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/conf/rwd/__init__.py
+-rw-rw-rw-   0        0        0    41277 2023-04-19 07:45:54.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/conftest_base.py
+drwxrwxrwx   0        0        0        0 2023-04-24 02:25:27.483587 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/drivers/
+-rw-rw-rw-   0        0        0        0 2022-11-21 09:11:03.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/drivers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 02:25:27.502589 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/drivers/browsers/
+-rw-rw-rw-   0        0        0        0 2022-11-21 09:11:28.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/drivers/browsers/__init__.py
+-rw-rw-rw-   0        0        0     3897 2022-12-07 03:55:17.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/drivers/browsers/browser_os_name_conf.py
+-rw-rw-rw-   0        0        0     3501 2023-04-24 02:24:42.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/drivers/browsers/local_browsers.py
+-rw-rw-rw-   0        0        0     5926 2022-11-21 10:05:25.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/drivers/browsers/remote_options.py
+-rw-rw-rw-   0        0        0    16954 2023-04-19 08:09:13.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/drivers/driverfactory.py
+-rw-rw-rw-   0        0        0      544 2022-11-14 01:59:19.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/main.py
+drwxrwxrwx   0        0        0        0 2023-04-24 02:25:27.530602 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/pages/
+-rw-rw-rw-   0        0        0    57659 2023-04-19 07:45:54.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/pages/Base_Page.py
+-rw-rw-rw-   0        0        0    25414 2023-04-20 08:32:17.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/pages/Mobile_Base_Page.py
+-rw-rw-rw-   0        0        0        0 2022-11-18 06:45:15.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/pages/__init__.py
+-rw-rw-rw-   0        0        0      370 2022-11-30 02:56:37.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/pages/mobile_zero_page.py
+-rw-rw-rw-   0        0        0      422 2022-11-30 02:10:57.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/pages/zero_page.py
+drwxrwxrwx   0        0        0        0 2023-04-24 02:25:27.541556 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/remoteTest/
+-rw-rw-rw-   0        0        0     3816 2022-11-30 06:10:04.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/remoteTest/BrowserStack_Library.py
+-rw-rw-rw-   0        0        0        0 2022-11-21 08:57:28.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/remoteTest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 02:25:27.568094 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/utils/
+-rw-rw-rw-   0        0        0        0 2022-11-21 08:39:02.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/utils/__init__.py
+-rw-rw-rw-   0        0        0      874 2023-01-04 03:46:28.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/utils/email_conf.py
+drwxrwxrwx   0        0        0        0 2023-04-24 02:25:27.604096 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/utils/general/
+-rw-rw-rw-   0        0        0     4915 2023-03-23 09:33:36.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/utils/general/Base_Logging.py
+-rw-rw-rw-   0        0        0      723 2022-10-07 06:37:19.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/utils/general/Gif_Maker.py
+-rw-rw-rw-   0        0        0     8968 2023-04-11 08:09:09.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/utils/general/Wrapit.py
+-rw-rw-rw-   0        0        0        0 2022-11-21 08:39:31.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/utils/general/__init__.py
+-rw-rw-rw-   0        0        0     9380 2023-01-04 06:33:56.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/utils/general/email_pytest_report.py
+-rw-rw-rw-   0        0        0      379 2022-10-07 06:37:19.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/utils/general/stop_test_exception_util.py
+-rw-rw-rw-   0        0        0       19 2022-10-12 03:37:41.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/utils/html_report_conf.py
+-rw-rw-rw-   0        0        0      227 2022-10-07 06:37:19.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/utils/remote_credentials.py
+-rw-rw-rw-   0        0        0       28 2022-11-29 09:59:41.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/utils/screenshot_conf.py
+drwxrwxrwx   0        0        0        0 2023-04-24 02:25:27.444555 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package.egg-info/
+-rw-rw-rw-   0        0        0     1172 2023-04-24 02:25:27.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2378 2023-04-24 02:25:27.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 02:25:27.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      272 2023-04-24 02:25:27.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       38 2023-04-24 02:25:27.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package.egg-info/top_level.txt
```

### Comparing `python_selenium_ctrl_package-0.0.97/LICENSE` & `python_selenium_ctrl_package-0.0.98/LICENSE`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.97/PKG-INFO` & `python_selenium_ctrl_package-0.0.98/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_selenium_ctrl_package
-Version: 0.0.97
+Version: 0.0.98
 Summary: Base_page for selenium automation
 Author-email: "QHMS(App team)" <qhmsqaexpert@gmail.com>
 Keywords: python,automation,appium,selenium,pytest,automation framework
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `python_selenium_ctrl_package-0.0.97/README.md` & `python_selenium_ctrl_package-0.0.98/README.md`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.97/pyproject.toml` & `python_selenium_ctrl_package-0.0.98/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python_selenium_ctrl_package"
-version = "0.0.97"
+version = "0.0.98"
 authors = [
   { name="QHMS(App team)", email="qhmsqaexpert@gmail.com" },
 ]
 description = "Base_page for selenium automation"
 keywords = ['python', 'automation', 'appium', 'selenium', 'pytest', 'automation framework']
 dependencies = ['requests', 'reportportal-client', 'pytest', 'selenium', 'python_dotenv', 'Appium_Python_Client', 'pytest-xdist', 'pytest-html', 'pytest-rerunfailures', 'pytest_reportportal', 'pillow', 'tesults', 'loguru', 'imageio', 'questionary', 'clear-screen', 'prompt-toolkit', 'openpyxl', 'pytest-bdd', 'pandas', 'webdriver-manager', 'PyHamcrest']
 readme = "README.md"
```

### Comparing `python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/conftest_base.py` & `python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/conftest_base.py`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/drivers/browsers/browser_os_name_conf.py` & `python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/drivers/browsers/browser_os_name_conf.py`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/drivers/browsers/local_browsers.py` & `python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/drivers/browsers/local_browsers.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         """Get webdriver for chrome."""
         options = webdriver.ChromeOptions()
         options.add_experimental_option('excludeSwitches', ['enable-logging'])
         if wdm == "Y":
             local_driver = webdriver.Chrome(
                 service=ChromeService(ChromeDriverManager().install()), options=options)
         else:
-            local_driver = webdriver.Chrome()
+            local_driver = webdriver.Chrome(options=options)
         return local_driver
 
     @staticmethod
     def edge_local():
         """Get webdriver for chrome."""
         local_driver = webdriver.Edge(executable_path='msedgedriver')
         # local_driver = webdriver.Chrome('./chromedriver/v92/chromedriver')
@@ -85,9 +85,9 @@
         options.add_argument('--disable-dev-shm-usage')
         options.add_argument('--no-sandbox')
         options.add_argument('--ignore-certificate-errors')
         if wdm == "Y":
             local_driver = webdriver.Chrome(
                 service=ChromeService(ChromeDriverManager().install()), options=options)
         else:
-            local_driver = webdriver.Chrome()
+            local_driver = webdriver.Chrome(options=options)
         return local_driver
```

### Comparing `python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/drivers/browsers/remote_options.py` & `python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/drivers/browsers/remote_options.py`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/drivers/driverfactory.py` & `python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/drivers/driverfactory.py`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/main.py` & `python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/main.py`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/pages/Base_Page.py` & `python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/pages/Base_Page.py`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/pages/Mobile_Base_Page.py` & `python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/pages/Mobile_Base_Page.py`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/remoteTest/BrowserStack_Library.py` & `python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/remoteTest/BrowserStack_Library.py`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/utils/email_conf.py` & `python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/utils/email_conf.py`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/utils/general/Base_Logging.py` & `python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/utils/general/Base_Logging.py`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/utils/general/Gif_Maker.py` & `python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/utils/general/Gif_Maker.py`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/utils/general/Wrapit.py` & `python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/utils/general/Wrapit.py`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package/utils/general/email_pytest_report.py` & `python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/utils/general/email_pytest_report.py`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package.egg-info/PKG-INFO` & `python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-selenium-ctrl-package
-Version: 0.0.97
+Version: 0.0.98
 Summary: Base_page for selenium automation
 Author-email: "QHMS(App team)" <qhmsqaexpert@gmail.com>
 Keywords: python,automation,appium,selenium,pytest,automation framework
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `python_selenium_ctrl_package-0.0.97/src/python_selenium_ctrl_package.egg-info/SOURCES.txt` & `python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package.egg-info/SOURCES.txt`

 * *Files identical despite different names*

