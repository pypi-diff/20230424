# Comparing `tmp/invenio-config-tuw-2023.1.0.tar.gz` & `tmp/invenio-config-tuw-2023.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio-config-tuw-2023.1.0.tar", last modified: Fri Jan 13 11:23:25 2023, max compression
+gzip compressed data, was "invenio-config-tuw-2023.2.0.tar", last modified: Mon Apr 24 16:22:47 2023, max compression
```

## Comparing `invenio-config-tuw-2023.1.0.tar` & `invenio-config-tuw-2023.2.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-01-13 11:23:25.032444 invenio-config-tuw-2023.1.0/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      124 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.1.0/.dockerignore
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      628 2022-11-23 16:27:25.000000 invenio-config-tuw-2023.1.0/.editorconfig
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        0 2022-11-23 16:27:25.000000 invenio-config-tuw-2023.1.0/.git-blame-ignore-revs
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-01-13 11:23:25.032444 invenio-config-tuw-2023.1.0/.tx/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1056 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.1.0/.tx/config
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      332 2021-07-15 09:46:09.000000 invenio-config-tuw-2023.1.0/AUTHORS.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2111 2023-01-13 11:22:31.000000 invenio-config-tuw-2023.1.0/CHANGES.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3392 2021-07-15 09:46:09.000000 invenio-config-tuw-2023.1.0/CONTRIBUTING.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      139 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.1.0/INSTALL.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1072 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.1.0/LICENSE
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1033 2022-11-23 16:27:25.000000 invenio-config-tuw-2023.1.0/MANIFEST.in
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5048 2023-01-13 11:23:25.032444 invenio-config-tuw-2023.1.0/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1960 2022-08-09 11:57:39.000000 invenio-config-tuw-2023.1.0/README.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      536 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.1.0/babel.ini
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-01-13 11:23:25.032444 invenio-config-tuw-2023.1.0/docs/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7457 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.1.0/docs/Makefile
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      278 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.1.0/docs/api.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      234 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.1.0/docs/authors.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      234 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.1.0/docs/changes.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    10226 2022-11-23 16:27:25.000000 invenio-config-tuw-2023.1.0/docs/conf.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      290 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.1.0/docs/configuration.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      239 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.1.0/docs/contributing.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      817 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.1.0/docs/index.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      234 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.1.0/docs/installation.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.1.0/docs/license.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7005 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.1.0/docs/make.bat
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       17 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.1.0/docs/requirements.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.1.0/docs/usage.rst
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-01-13 11:23:25.032444 invenio-config-tuw-2023.1.0/invenio_config_tuw/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      408 2023-01-13 11:22:31.000000 invenio-config-tuw-2023.1.0/invenio_config_tuw/__init__.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-01-13 11:23:25.032444 invenio-config-tuw-2023.1.0/invenio_config_tuw/auth/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      540 2021-07-15 09:46:09.000000 invenio-config-tuw-2023.1.0/invenio_config_tuw/auth/__init__.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1006 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.1.0/invenio_config_tuw/auth/config.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8631 2022-07-19 13:52:16.000000 invenio-config-tuw-2023.1.0/invenio_config_tuw/auth/handlers.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2540 2021-10-04 14:54:28.000000 invenio-config-tuw-2023.1.0/invenio_config_tuw/auth/utils.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     6662 2023-01-11 14:40:44.000000 invenio-config-tuw-2023.1.0/invenio_config_tuw/config.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2623 2022-11-24 12:57:07.000000 invenio-config-tuw-2023.1.0/invenio_config_tuw/ext.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1104 2022-10-28 12:03:49.000000 invenio-config-tuw-2023.1.0/invenio_config_tuw/formatters.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3937 2022-11-30 18:10:11.000000 invenio-config-tuw-2023.1.0/invenio_config_tuw/forms.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-01-13 11:23:25.032444 invenio-config-tuw-2023.1.0/invenio_config_tuw/permissions/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      780 2022-07-18 13:04:23.000000 invenio-config-tuw-2023.1.0/invenio_config_tuw/permissions/__init__.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3170 2022-10-11 13:14:29.000000 invenio-config-tuw-2023.1.0/invenio_config_tuw/permissions/generators.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    10423 2022-10-17 09:06:55.000000 invenio-config-tuw-2023.1.0/invenio_config_tuw/permissions/policies.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3862 2022-10-28 12:03:49.000000 invenio-config-tuw-2023.1.0/invenio_config_tuw/startup.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2739 2022-12-15 09:45:24.000000 invenio-config-tuw-2023.1.0/invenio_config_tuw/utils.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-01-13 11:23:25.032444 invenio-config-tuw-2023.1.0/invenio_config_tuw.egg-info/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5048 2023-01-13 11:23:25.000000 invenio-config-tuw-2023.1.0/invenio_config_tuw.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1270 2023-01-13 11:23:25.000000 invenio-config-tuw-2023.1.0/invenio_config_tuw.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2023-01-13 11:23:25.000000 invenio-config-tuw-2023.1.0/invenio_config_tuw.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      421 2023-01-13 11:23:25.000000 invenio-config-tuw-2023.1.0/invenio_config_tuw.egg-info/entry_points.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2023-01-13 11:23:24.000000 invenio-config-tuw-2023.1.0/invenio_config_tuw.egg-info/not-zip-safe
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2023-01-13 11:23:25.000000 invenio-config-tuw-2023.1.0/invenio_config_tuw.egg-info/requires.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       19 2023-01-13 11:23:25.000000 invenio-config-tuw-2023.1.0/invenio_config_tuw.egg-info/top_level.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      104 2022-11-23 16:27:25.000000 invenio-config-tuw-2023.1.0/pyproject.toml
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      492 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.1.0/requirements-devel.txt
--rwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)      411 2022-11-23 16:27:25.000000 invenio-config-tuw-2023.1.0/run-tests.sh
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2767 2023-01-13 11:23:25.036444 invenio-config-tuw-2023.1.0/setup.cfg
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      339 2022-11-23 16:27:25.000000 invenio-config-tuw-2023.1.0/setup.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-01-13 11:23:25.032444 invenio-config-tuw-2023.1.0/tests/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      990 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.1.0/tests/conftest.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      789 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.1.0/tests/test_invenio_config_tuw.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 16:22:47.909080 invenio-config-tuw-2023.2.0/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      124 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/.dockerignore
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      628 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.0/.editorconfig
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.0/.git-blame-ignore-revs
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 16:22:47.893079 invenio-config-tuw-2023.2.0/.tx/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1056 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/.tx/config
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      332 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/AUTHORS.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2221 2023-04-24 16:22:41.000000 invenio-config-tuw-2023.2.0/CHANGES.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3392 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/CONTRIBUTING.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      139 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/INSTALL.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1072 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/LICENSE
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1033 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.0/MANIFEST.in
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5158 2023-04-24 16:22:47.909080 invenio-config-tuw-2023.2.0/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1960 2022-10-28 12:08:23.000000 invenio-config-tuw-2023.2.0/README.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      536 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/babel.ini
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 16:22:47.901080 invenio-config-tuw-2023.2.0/docs/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7457 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/docs/Makefile
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      278 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/docs/api.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      234 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/docs/authors.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      234 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/docs/changes.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    10226 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.0/docs/conf.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      290 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/docs/configuration.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      239 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/docs/contributing.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      817 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/docs/index.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      234 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/docs/installation.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/docs/license.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7005 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/docs/make.bat
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       17 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/docs/requirements.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/docs/usage.rst
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 16:22:47.901080 invenio-config-tuw-2023.2.0/invenio_config_tuw/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      408 2023-04-24 16:22:41.000000 invenio-config-tuw-2023.2.0/invenio_config_tuw/__init__.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 16:22:47.905080 invenio-config-tuw-2023.2.0/invenio_config_tuw/auth/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      540 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/invenio_config_tuw/auth/__init__.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1006 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/invenio_config_tuw/auth/config.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8631 2022-10-28 12:08:23.000000 invenio-config-tuw-2023.2.0/invenio_config_tuw/auth/handlers.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2540 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/invenio_config_tuw/auth/utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     6700 2023-04-24 16:22:41.000000 invenio-config-tuw-2023.2.0/invenio_config_tuw/config.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2623 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.0/invenio_config_tuw/ext.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1104 2022-10-28 12:08:23.000000 invenio-config-tuw-2023.2.0/invenio_config_tuw/formatters.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3937 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.0/invenio_config_tuw/forms.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 16:22:47.909080 invenio-config-tuw-2023.2.0/invenio_config_tuw/permissions/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      780 2022-10-28 12:08:23.000000 invenio-config-tuw-2023.2.0/invenio_config_tuw/permissions/__init__.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3170 2022-10-28 12:08:23.000000 invenio-config-tuw-2023.2.0/invenio_config_tuw/permissions/generators.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    11136 2023-04-24 16:22:41.000000 invenio-config-tuw-2023.2.0/invenio_config_tuw/permissions/policies.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3862 2022-10-28 12:08:23.000000 invenio-config-tuw-2023.2.0/invenio_config_tuw/startup.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2739 2023-04-24 16:22:41.000000 invenio-config-tuw-2023.2.0/invenio_config_tuw/utils.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 16:22:47.905080 invenio-config-tuw-2023.2.0/invenio_config_tuw.egg-info/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5158 2023-04-24 16:22:47.000000 invenio-config-tuw-2023.2.0/invenio_config_tuw.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1270 2023-04-24 16:22:47.000000 invenio-config-tuw-2023.2.0/invenio_config_tuw.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2023-04-24 16:22:47.000000 invenio-config-tuw-2023.2.0/invenio_config_tuw.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      421 2023-04-24 16:22:47.000000 invenio-config-tuw-2023.2.0/invenio_config_tuw.egg-info/entry_points.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2023-04-24 16:22:47.000000 invenio-config-tuw-2023.2.0/invenio_config_tuw.egg-info/not-zip-safe
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2023-04-24 16:22:47.000000 invenio-config-tuw-2023.2.0/invenio_config_tuw.egg-info/requires.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       19 2023-04-24 16:22:47.000000 invenio-config-tuw-2023.2.0/invenio_config_tuw.egg-info/top_level.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      104 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.0/pyproject.toml
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      492 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/requirements-devel.txt
+-rwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)      411 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.0/run-tests.sh
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2767 2023-04-24 16:22:47.909080 invenio-config-tuw-2023.2.0/setup.cfg
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      339 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.0/setup.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-04-24 16:22:47.909080 invenio-config-tuw-2023.2.0/tests/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      990 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/tests/conftest.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      789 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.0/tests/test_invenio_config_tuw.py
```

### Comparing `invenio-config-tuw-2023.1.0/.editorconfig` & `invenio-config-tuw-2023.2.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.1.0/.tx/config` & `invenio-config-tuw-2023.2.0/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.1.0/CHANGES.rst` & `invenio-config-tuw-2023.2.0/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,19 @@
     Invenio-Config-TUW is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version 2023.2 (released 2023-04-24)
+
+- v11 compat: Update permission policies and disable archive download
+
+
 Version 2023.1 (released 2023-01-13)
 
 - Update definition of the default creator for new uploads
 
 
 Version 2022.3 (released 2022-10-28, updated 2022-11-30)
```

### Comparing `invenio-config-tuw-2023.1.0/CONTRIBUTING.rst` & `invenio-config-tuw-2023.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.1.0/LICENSE` & `invenio-config-tuw-2023.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.1.0/MANIFEST.in` & `invenio-config-tuw-2023.2.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.1.0/PKG-INFO` & `invenio-config-tuw-2023.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-config-tuw
-Version: 2023.1.0
+Version: 2023.2.0
 Summary: "Invenio module containing some customizations and configuration for TU Wien."
 Home-page: https://gitlab.tuwien.ac.at/fairdata/invenio-config-tuw
 Author: TU Wien
 Author-email: tudata@tuwien.ac.at
 License: MIT
 Keywords: invenio tu wien configuration
 Platform: any
@@ -94,14 +94,19 @@
     Invenio-Config-TUW is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version 2023.2 (released 2023-04-24)
+
+- v11 compat: Update permission policies and disable archive download
+
+
 Version 2023.1 (released 2023-01-13)
 
 - Update definition of the default creator for new uploads
 
 
 Version 2022.3 (released 2022-10-28, updated 2022-11-30)
```

### Comparing `invenio-config-tuw-2023.1.0/README.rst` & `invenio-config-tuw-2023.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.1.0/babel.ini` & `invenio-config-tuw-2023.2.0/babel.ini`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.1.0/docs/Makefile` & `invenio-config-tuw-2023.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.1.0/docs/conf.py` & `invenio-config-tuw-2023.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.1.0/docs/index.rst` & `invenio-config-tuw-2023.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.1.0/docs/make.bat` & `invenio-config-tuw-2023.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.1.0/invenio_config_tuw/auth/__init__.py` & `invenio-config-tuw-2023.2.0/invenio_config_tuw/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.1.0/invenio_config_tuw/auth/config.py` & `invenio-config-tuw-2023.2.0/invenio_config_tuw/auth/config.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.1.0/invenio_config_tuw/auth/handlers.py` & `invenio-config-tuw-2023.2.0/invenio_config_tuw/auth/handlers.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.1.0/invenio_config_tuw/auth/utils.py` & `invenio-config-tuw-2023.2.0/invenio_config_tuw/auth/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.1.0/invenio_config_tuw/config.py` & `invenio-config-tuw-2023.2.0/invenio_config_tuw/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,14 +177,16 @@
     "oai_datacite": {
         "serializer": "invenio_rdm_records.oai:oai_datacite_etree",
         "schema": "http://schema.datacite.org/oai/oai-1.1/oai.xsd",
         "namespace": "http://schema.datacite.org/oai/oai-1.1/",
     },
 }
 
+RDM_ARCHIVE_DOWNLOAD_ENABLED = False
+
 
 # Invenio-Requests
 # ================
 
 REQUESTS_PERMISSION_POLICY = TUWRequestsPermissionPolicy
```

### Comparing `invenio-config-tuw-2023.1.0/invenio_config_tuw/ext.py` & `invenio-config-tuw-2023.2.0/invenio_config_tuw/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.1.0/invenio_config_tuw/formatters.py` & `invenio-config-tuw-2023.2.0/invenio_config_tuw/formatters.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.1.0/invenio_config_tuw/forms.py` & `invenio-config-tuw-2023.2.0/invenio_config_tuw/forms.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.1.0/invenio_config_tuw/permissions/__init__.py` & `invenio-config-tuw-2023.2.0/invenio_config_tuw/permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.1.0/invenio_config_tuw/permissions/generators.py` & `invenio-config-tuw-2023.2.0/invenio_config_tuw/permissions/generators.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.1.0/invenio_config_tuw/permissions/policies.py` & `invenio-config-tuw-2023.2.0/invenio_config_tuw/permissions/policies.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # Invenio-Config-TUW is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 from invenio_communities.permissions import CommunityPermissionPolicy
 from invenio_rdm_records.services import RDMRecordPermissionPolicy
 from invenio_rdm_records.services.generators import (
     CommunityAction,
+    IfFileIsLocal,
     IfRestricted,
     RecordOwners,
     SubmissionReviewer,
 )
 from invenio_records_permissions.generators import (
     AnyUser,
     AuthenticatedUser,
@@ -33,15 +34,15 @@
 
 # TODO override permissions for vocabularies and users-resources
 
 
 class TUWRecordPermissionPolicy(RDMRecordPermissionPolicy):
     """Record permission policy of TU Wien."""
 
-    # current state: invenio-rdm-records v0.39.1
+    # current state: invenio-rdm-records v1.3.5
     #
     # note: edit := create a draft from a record (i.e. putting it in edit mode),
     #               which does not imply the permission to save the edits
     # note: can_search_* is the permission for the search in general, the records
     #       (drafts) will be filtered as per can_read_* permissions
     #
     # fmt: off
@@ -66,24 +67,28 @@
     can_authenticated      = can_basics       + [AuthenticatedUser()]                                                   # noqa
     can_all                = can_basics       + [AnyUser()]                                                             # noqa
 
     # records
     can_search             = can_all                                                                                    # noqa
     can_read               = [IfRestricted("record", then_=can_view, else_=can_all)] + secret_links["view_record"]      # noqa
     can_read_files         = [IfRestricted("files", then_=can_view, else_=can_all) ] + secret_links["view_files"]       # noqa
+    can_get_content_files  = [IfFileIsLocal(then_=can_read_files, else_=[SystemProcess()]) ]                            # noqa
     can_create             = can_basics + [TrustedUsers(), DisableIfReadOnly()]                                         # noqa
 
     # drafts
-    can_search_drafts      = can_authenticated                                                                          # noqa
-    can_read_draft         = can_preview                                                                                # noqa
-    can_draft_read_files   = can_preview                                                                                # noqa
-    can_update_draft       = can_review + [DisableIfReadOnly()]                                                         # noqa
-    can_draft_create_files = can_review + [DisableIfReadOnly()]                                                         # noqa
-    can_draft_update_files = can_review + [DisableIfReadOnly()]                                                         # noqa
-    can_draft_delete_files = can_review + [DisableIfReadOnly()]                                                         # noqa
+    can_search_drafts           = can_authenticated                                                                     # noqa
+    can_read_draft              = can_preview                                                                           # noqa
+    can_draft_read_files        = can_preview                                                                           # noqa
+    can_update_draft            = can_review + [DisableIfReadOnly()]                                                    # noqa
+    can_draft_create_files      = can_review + [DisableIfReadOnly()]                                                    # noqa
+    can_draft_set_content_files = can_review + [DisableIfReadOnly()]                                                    # noqa
+    can_draft_get_content_files = can_review + [DisableIfReadOnly()]                                                    # noqa
+    can_draft_commit_files      = can_review + [DisableIfReadOnly()]                                                    # noqa
+    can_draft_update_files      = can_review + [DisableIfReadOnly()]                                                    # noqa
+    can_draft_delete_files      = can_review + [DisableIfReadOnly()]                                                    # noqa
 
     # PIDs
     can_pid_create         = can_review + [DisableIfReadOnly()]                                                         # noqa
     can_pid_register       = can_review + [DisableIfReadOnly()]                                                         # noqa
     can_pid_update         = can_review + [DisableIfReadOnly()]                                                         # noqa
     can_pid_discard        = can_review + [DisableIfReadOnly()]                                                         # noqa
     can_pid_delete         = can_review + [DisableIfReadOnly()]                                                         # noqa
@@ -98,48 +103,50 @@
     can_lift_embargo       = can_manage + [DisableIfReadOnly()]                                                         # noqa
     can_publish            = can_basics + [TrustedPublisherRecordOwners(), DisableIfReadOnly()]                         # noqa
 
     # disabled (record management in InvenioRDM goes through drafts)
     can_update             = [Disable()]                                                                                # noqa
     can_delete             = [Disable()]                                                                                # noqa
     can_create_files       = [Disable()]                                                                                # noqa
+    can_set_content_files  = [Disable()]                                                                                # noqa
+    can_commit_files       = [Disable()]                                                                                # noqa
     can_update_files       = [Disable()]                                                                                # noqa
     can_delete_files       = [Disable()]                                                                                # noqa
     # fmt: on
 
 
 class TUWRequestsPermissionPolicy(RequestsPermissionPolicy):
     """Requests permission policy of TU Wien."""
 
     # disable write operations if the system is in read-only mode
     #
-    # current state: invenio-requests v0.5.5
+    # current state: invenio-requests v1.0.5
 
     # fmt: off
     can_create         = RequestsPermissionPolicy.can_create         + [DisableIfReadOnly()]  # noqa
     can_update         = RequestsPermissionPolicy.can_update         + [DisableIfReadOnly()]  # noqa
     can_delete         = RequestsPermissionPolicy.can_delete         + [DisableIfReadOnly()]  # noqa
     can_action_submit  = RequestsPermissionPolicy.can_action_submit  + [DisableIfReadOnly()]  # noqa
     can_action_cancel  = RequestsPermissionPolicy.can_action_cancel  + [DisableIfReadOnly()]  # noqa
     can_action_expire  = RequestsPermissionPolicy.can_action_expire  + [DisableIfReadOnly()]  # noqa
     can_action_accept  = RequestsPermissionPolicy.can_action_accept  + [DisableIfReadOnly()]  # noqa
     can_action_decline = RequestsPermissionPolicy.can_action_decline + [DisableIfReadOnly()]  # noqa
-    can_create_comment = RequestsPermissionPolicy.can_read           + [DisableIfReadOnly()]  # noqa  # TODO s/can_read/can_create_comment for invenio-requests > 0.5.5
+    can_create_comment = RequestsPermissionPolicy.can_create_comment + [DisableIfReadOnly()]  # noqa
     can_update_comment = RequestsPermissionPolicy.can_update_comment + [DisableIfReadOnly()]  # noqa
     can_delete_comment = RequestsPermissionPolicy.can_delete_comment + [DisableIfReadOnly()]  # noqa
     # fmt: on
 
 
 class TUWCommunitiesPermissionPolicy(CommunityPermissionPolicy):
     """Communities permission policy of TU Wien."""
 
     # for now, we want to restrict the creation of communities to admins
     # and disable write operations if the system is in read-only mode
     #
-    # current state: invenio-communities v3.1.0
+    # current state: invenio-communities v4.1.2
     #
     # TODO: discuss who should have permissions to create communities
     #       -> new role?
     can_create = [SystemProcess(), DisableIfReadOnly()]
 
     # fmt: off
     can_update              = CommunityPermissionPolicy.can_update              + [DisableIfReadOnly()]  # noqa
```

### Comparing `invenio-config-tuw-2023.1.0/invenio_config_tuw/startup.py` & `invenio-config-tuw-2023.2.0/invenio_config_tuw/startup.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.1.0/invenio_config_tuw/utils.py` & `invenio-config-tuw-2023.2.0/invenio_config_tuw/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,12 +85,11 @@
         "person_or_org": {
             "family_name": last_name,
             "given_name": first_name,
             "identifiers": [],
             "name": full_name,
             "type": "personal",
         },
-        "role": "contactperson"
+        "role": "contactperson",
     }
 
     return [creator]
-
```

### Comparing `invenio-config-tuw-2023.1.0/invenio_config_tuw.egg-info/PKG-INFO` & `invenio-config-tuw-2023.2.0/invenio_config_tuw.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-config-tuw
-Version: 2023.1.0
+Version: 2023.2.0
 Summary: "Invenio module containing some customizations and configuration for TU Wien."
 Home-page: https://gitlab.tuwien.ac.at/fairdata/invenio-config-tuw
 Author: TU Wien
 Author-email: tudata@tuwien.ac.at
 License: MIT
 Keywords: invenio tu wien configuration
 Platform: any
@@ -94,14 +94,19 @@
     Invenio-Config-TUW is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version 2023.2 (released 2023-04-24)
+
+- v11 compat: Update permission policies and disable archive download
+
+
 Version 2023.1 (released 2023-01-13)
 
 - Update definition of the default creator for new uploads
 
 
 Version 2022.3 (released 2022-10-28, updated 2022-11-30)
```

### Comparing `invenio-config-tuw-2023.1.0/invenio_config_tuw.egg-info/SOURCES.txt` & `invenio-config-tuw-2023.2.0/invenio_config_tuw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.1.0/setup.cfg` & `invenio-config-tuw-2023.2.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 [options]
 include_package_data = True
 packages = find:
 python_requires = >=3.7
 zip_safe = False
 install_requires = 
 	Flask-BabelEx>=0.9.4
-	invenio-app-rdm>=10.0.0
+	invenio-app-rdm>=11.0.0
 	invenio-mail>=1.0.2,<1.1.0
 
 [options.extras_require]
 tests = 
 	pytest-black>=0.3.0,<0.3.10
 	check-manifest>=0.25
 	coverage>=4.0
```

### Comparing `invenio-config-tuw-2023.1.0/tests/conftest.py` & `invenio-config-tuw-2023.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.1.0/tests/test_invenio_config_tuw.py` & `invenio-config-tuw-2023.2.0/tests/test_invenio_config_tuw.py`

 * *Files identical despite different names*

