# Comparing `tmp/shopcloud_eventbus-1.2.0.tar.gz` & `tmp/shopcloud_eventbus-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shopcloud_eventbus-1.2.0.tar", last modified: Wed Mar 22 06:11:31 2023, max compression
+gzip compressed data, was "shopcloud_eventbus-1.3.0.tar", last modified: Mon Apr 24 07:18:45 2023, max compression
```

## Comparing `shopcloud_eventbus-1.2.0.tar` & `shopcloud_eventbus-1.3.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 06:11:31.765771 shopcloud_eventbus-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-22 06:11:21.000000 shopcloud_eventbus-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-03-22 06:11:31.765771 shopcloud_eventbus-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-03-22 06:11:21.000000 shopcloud_eventbus-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-03-22 06:11:21.000000 shopcloud_eventbus-1.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 06:11:31.761771 shopcloud_eventbus-1.2.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-22 06:11:21.000000 shopcloud_eventbus-1.2.0/scripts/eventbus
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 06:11:31.765771 shopcloud_eventbus-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-03-22 06:11:31.000000 shopcloud_eventbus-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 06:11:31.761771 shopcloud_eventbus-1.2.0/shopcloud_eventbus/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-22 06:11:21.000000 shopcloud_eventbus-1.2.0/shopcloud_eventbus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-03-22 06:11:21.000000 shopcloud_eventbus-1.2.0/shopcloud_eventbus/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7849 2023-03-22 06:11:21.000000 shopcloud_eventbus-1.2.0/shopcloud_eventbus/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-03-22 06:11:21.000000 shopcloud_eventbus-1.2.0/shopcloud_eventbus/events.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-22 06:11:21.000000 shopcloud_eventbus-1.2.0/shopcloud_eventbus/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-03-22 06:11:21.000000 shopcloud_eventbus-1.2.0/shopcloud_eventbus/file_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-22 06:11:21.000000 shopcloud_eventbus-1.2.0/shopcloud_eventbus/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-22 06:11:21.000000 shopcloud_eventbus-1.2.0/shopcloud_eventbus/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 06:11:31.765771 shopcloud_eventbus-1.2.0/shopcloud_eventbus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-03-22 06:11:31.000000 shopcloud_eventbus-1.2.0/shopcloud_eventbus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-03-22 06:11:31.000000 shopcloud_eventbus-1.2.0/shopcloud_eventbus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 06:11:31.000000 shopcloud_eventbus-1.2.0/shopcloud_eventbus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-22 06:11:31.000000 shopcloud_eventbus-1.2.0/shopcloud_eventbus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-22 06:11:31.000000 shopcloud_eventbus-1.2.0/shopcloud_eventbus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:18:45.841392 shopcloud_eventbus-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-24 07:18:36.000000 shopcloud_eventbus-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-24 07:18:45.841392 shopcloud_eventbus-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-24 07:18:36.000000 shopcloud_eventbus-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-24 07:18:36.000000 shopcloud_eventbus-1.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:18:45.841392 shopcloud_eventbus-1.3.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-24 07:18:36.000000 shopcloud_eventbus-1.3.0/scripts/eventbus
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 07:18:45.841392 shopcloud_eventbus-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-24 07:18:45.000000 shopcloud_eventbus-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:18:45.841392 shopcloud_eventbus-1.3.0/shopcloud_eventbus/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-24 07:18:36.000000 shopcloud_eventbus-1.3.0/shopcloud_eventbus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-24 07:18:36.000000 shopcloud_eventbus-1.3.0/shopcloud_eventbus/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-04-24 07:18:36.000000 shopcloud_eventbus-1.3.0/shopcloud_eventbus/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-24 07:18:36.000000 shopcloud_eventbus-1.3.0/shopcloud_eventbus/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-24 07:18:36.000000 shopcloud_eventbus-1.3.0/shopcloud_eventbus/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-04-24 07:18:36.000000 shopcloud_eventbus-1.3.0/shopcloud_eventbus/file_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-24 07:18:36.000000 shopcloud_eventbus-1.3.0/shopcloud_eventbus/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-24 07:18:36.000000 shopcloud_eventbus-1.3.0/shopcloud_eventbus/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 07:18:45.841392 shopcloud_eventbus-1.3.0/shopcloud_eventbus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-24 07:18:45.000000 shopcloud_eventbus-1.3.0/shopcloud_eventbus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-24 07:18:45.000000 shopcloud_eventbus-1.3.0/shopcloud_eventbus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 07:18:45.000000 shopcloud_eventbus-1.3.0/shopcloud_eventbus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-24 07:18:45.000000 shopcloud_eventbus-1.3.0/shopcloud_eventbus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-24 07:18:45.000000 shopcloud_eventbus-1.3.0/shopcloud_eventbus.egg-info/top_level.txt
```

### Comparing `shopcloud_eventbus-1.2.0/LICENSE` & `shopcloud_eventbus-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shopcloud_eventbus-1.2.0/PKG-INFO` & `shopcloud_eventbus-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shopcloud_eventbus
-Version: 1.2.0
+Version: 1.3.0
 Summary: CLI tool for the Shopcloud EventBus
 Home-page: https://github.com/Talk-Point/shopcloud-eventbus
 Author: Konstantin Stoldt
 Author-email: konstantin.stoldt@talk-point.de
 License: MIT
 Keywords: CLI
 Description-Content-Type: text/markdown
```

### Comparing `shopcloud_eventbus-1.2.0/README.md` & `shopcloud_eventbus-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `shopcloud_eventbus-1.2.0/setup.py` & `shopcloud_eventbus-1.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = {
     "name": 'shopcloud_eventbus',
-    "version": '1.2.0',
+    "version": '1.3.0',
     "description": 'CLI tool for the Shopcloud EventBus',
     "long_description_content_type": "text/markdown",
     "long_description": README,
     "license": 'MIT',
     "packages": find_packages(),
     "author": 'Konstantin Stoldt',
     "author_email": 'konstantin.stoldt@talk-point.de',
```

### Comparing `shopcloud_eventbus-1.2.0/shopcloud_eventbus/__main__.py` & `shopcloud_eventbus-1.3.0/shopcloud_eventbus/__main__.py`

 * *Files identical despite different names*

### Comparing `shopcloud_eventbus-1.2.0/shopcloud_eventbus/cli.py` & `shopcloud_eventbus-1.3.0/shopcloud_eventbus/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,20 +199,21 @@
                 secrethub_namesapce = helpers.ask_for('Namespace', 'talk-point')
                 secrethub_repo = helpers.ask_for('Repo')
 
                 config.secrethub_endpoint_user = f'{secrethub_namesapce}/{secrethub_repo}/production/evenbus-user'
                 config.secrethub_endpoint_pwd = f'{secrethub_namesapce}/{secrethub_repo}/production/evenbus-pwd'
 
                 if helpers.ask_for_yes_no('Create items on secrethub?'):
+                    username = 'api-eventbus'
                     pwd = helpers.generate_safe_password_32()
-                    hub.write(config.secrethub_endpoint_user, 'api-eventbus')
+                    hub.write(config.secrethub_endpoint_user, username)
                     hub.write(config.secrethub_endpoint_pwd, pwd)
 
                     print('# Django')
-                    print(f'- Create user "eventbus" with password {pwd}')
+                    print(f'- Create user "{username}" with password {pwd}')
                     helpers.ask_for_enter()
             else:
                 config.secrethub_endpoint_user = args.secrethub_endpoint_user
                 config.secrethub_endpoint_pwd = args.secrethub_endpoint_pwd
 
             config.save()
             print(helpers.bcolors.OKGREEN + f'Config saved under `{Config.FILENAME}`' + helpers.bcolors.ENDC)
```

### Comparing `shopcloud_eventbus-1.2.0/shopcloud_eventbus/events.py` & `shopcloud_eventbus-1.3.0/shopcloud_eventbus/events.py`

 * *Files identical despite different names*

### Comparing `shopcloud_eventbus-1.2.0/shopcloud_eventbus/file_content.py` & `shopcloud_eventbus-1.3.0/shopcloud_eventbus/file_content.py`

 * *Files identical despite different names*

### Comparing `shopcloud_eventbus-1.2.0/shopcloud_eventbus/helpers.py` & `shopcloud_eventbus-1.3.0/shopcloud_eventbus/helpers.py`

 * *Files identical despite different names*

### Comparing `shopcloud_eventbus-1.2.0/shopcloud_eventbus.egg-info/PKG-INFO` & `shopcloud_eventbus-1.3.0/shopcloud_eventbus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shopcloud-eventbus
-Version: 1.2.0
+Version: 1.3.0
 Summary: CLI tool for the Shopcloud EventBus
 Home-page: https://github.com/Talk-Point/shopcloud-eventbus
 Author: Konstantin Stoldt
 Author-email: konstantin.stoldt@talk-point.de
 License: MIT
 Keywords: CLI
 Description-Content-Type: text/markdown
```

### Comparing `shopcloud_eventbus-1.2.0/shopcloud_eventbus.egg-info/SOURCES.txt` & `shopcloud_eventbus-1.3.0/shopcloud_eventbus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

