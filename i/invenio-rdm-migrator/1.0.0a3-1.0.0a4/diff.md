# Comparing `tmp/invenio-rdm-migrator-1.0.0a3.tar.gz` & `tmp/invenio-rdm-migrator-1.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-rdm-migrator-1.0.0a3.tar", last modified: Mon Apr  3 16:18:18 2023, max compression
+gzip compressed data, was "dist/invenio-rdm-migrator-1.0.0a4.tar", last modified: Mon Apr 24 08:51:28 2023, max compression
```

## Comparing `invenio-rdm-migrator-1.0.0a3.tar` & `invenio-rdm-migrator-1.0.0a4.tar`

### file list

```diff
@@ -1,86 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:18:18.000000 invenio-rdm-migrator-1.0.0a3/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:18:18.000000 invenio-rdm-migrator-1.0.0a3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:18:18.000000 invenio-rdm-migrator-1.0.0a3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13418 2023-04-03 16:18:18.000000 invenio-rdm-migrator-1.0.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:18:18.000000 invenio-rdm-migrator-1.0.0a3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:18:18.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:18:18.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/extract/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/extract/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:18:18.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/load/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/load/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/load/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/load/postgresql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:18:18.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:18:18.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/communities/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/communities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/communities/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/communities/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/communities/table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/communities/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:18:18.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/records/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/records/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/records/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/records/table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/records/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:18:18.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/requests/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/requests/load.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/requests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/requests/table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/requests/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/streams.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:18:18.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/users/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/users/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/users/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/users/table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/users/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:18:18.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/transform/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/transform/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:18:18.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13418 2023-04-03 16:18:18.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-03 16:18:18.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 16:18:18.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 16:18:18.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-03 16:18:18.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-03 16:18:18.000000 invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1410 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-03 16:18:18.000000 invenio-rdm-migrator-1.0.0a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:18:18.000000 invenio-rdm-migrator-1.0.0a3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:18:18.000000 invenio-rdm-migrator-1.0.0a3/tests/streams/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:18:18.000000 invenio-rdm-migrator-1.0.0a3/tests/streams/requests/
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/tests/streams/requests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/tests/streams/requests/test_requests_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/tests/streams/requests/test_requests_table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-04-03 16:18:10.000000 invenio-rdm-migrator-1.0.0a3/tests/streams/requests/test_requests_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/extract/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/extract/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/load/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/load/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/load/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/load/postgresql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/communities/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/communities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/communities/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/communities/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/communities/table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/communities/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/files/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/files/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/files/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/files/table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/files/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/records/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/records/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9595 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/records/table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/records/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/requests/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/requests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/requests/table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/requests/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/streams.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/users/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/users/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/users/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/users/table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/users/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/transform/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-04-24 08:51:27.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 08:51:27.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 08:51:27.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-24 08:51:27.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-24 08:51:27.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1410 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/tests/streams/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/tests/streams/communities/
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/tests/streams/communities/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/tests/streams/communities/test_communities_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/tests/streams/communities/test_communities_table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/tests/streams/communities/test_communities_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/tests/streams/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/tests/streams/files/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/tests/streams/files/test_files_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/tests/streams/files/test_files_table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/tests/streams/files/test_files_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/tests/streams/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/tests/streams/requests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/tests/streams/requests/test_requests_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/tests/streams/requests/test_requests_table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/tests/streams/requests/test_requests_transform.py
```

### Comparing `invenio-rdm-migrator-1.0.0a3/.editorconfig` & `invenio-rdm-migrator-1.0.0a4/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a3/.github/workflows/pypi-publish.yml` & `invenio-rdm-migrator-1.0.0a4/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a3/.github/workflows/tests.yml` & `invenio-rdm-migrator-1.0.0a4/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a3/CONTRIBUTING.rst` & `invenio-rdm-migrator-1.0.0a4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a3/LICENSE` & `invenio-rdm-migrator-1.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a3/MANIFEST.in` & `invenio-rdm-migrator-1.0.0a4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a3/PKG-INFO` & `invenio-rdm-migrator-1.0.0a4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-rdm-migrator
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: InvenioRDM module for data migration.
 Home-page: https://github.com/inveniosoftware/invenio-rdm-migrator
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2022 CERN.
@@ -179,16 +179,14 @@
         
         .. code-block:: python
         
             {
                 "record": self._record(entry),
                 "draft": self._draft(entry),
                 "parent": self._parent(entry),
-                "record_files": self._record_files(entry),
-                "draft_files": self._draft_files(entry),
             }
         
         This means that you will need to implement the functions for each key. Note
         that, only `_record` and `_parent` should return content, the others can return
         `None`. In this case we will need to re-think which methods should be
         `abstractmethod` and which ones be defaulted to `None/{}/some other default` in
         the base. You can find an example implementation at
```

### Comparing `invenio-rdm-migrator-1.0.0a3/README.rst` & `invenio-rdm-migrator-1.0.0a4/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -171,16 +171,14 @@
 
 .. code-block:: python
 
     {
         "record": self._record(entry),
         "draft": self._draft(entry),
         "parent": self._parent(entry),
-        "record_files": self._record_files(entry),
-        "draft_files": self._draft_files(entry),
     }
 
 This means that you will need to implement the functions for each key. Note
 that, only `_record` and `_parent` should return content, the others can return
 `None`. In this case we will need to re-think which methods should be
 `abstractmethod` and which ones be defaulted to `None/{}/some other default` in
 the base. You can find an example implementation at
```

### Comparing `invenio-rdm-migrator-1.0.0a3/docs/Makefile` & `invenio-rdm-migrator-1.0.0a4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a3/docs/conf.py` & `invenio-rdm-migrator-1.0.0a4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a3/docs/index.rst` & `invenio-rdm-migrator-1.0.0a4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a3/docs/make.bat` & `invenio-rdm-migrator-1.0.0a4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/load/base.py` & `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/load/base.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/load/models.py` & `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/load/models.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/load/postgresql.py` & `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/load/postgresql.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/communities/__init__.py` & `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/communities/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,17 +8,19 @@
 """Invenio RDM migration users stream."""
 
 from .load import CommunityCopyLoad
 from .transform import (
     CommunityEntry,
     CommunityMemberEntry,
     CommunityTransform,
+    FeaturedCommunityEntry,
     ParentCommunityEntry,
 )
 
 __all__ = (
     "CommunityCopyLoad",
     "CommunityEntry",
     "CommunityMemberEntry",
     "CommunityTransform",
+    "FeaturedCommunityEntry",
     "ParentCommunityEntry",
 )
```

### Comparing `invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/communities/load.py` & `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/communities/load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/communities/models.py` & `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/communities/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -50,7 +50,20 @@
     active: bool
     community_id: str
     user_id: int
     group_id: int
     request_id: int
 
     _table_name: InitVar[str] = "communities_members"
+
+
+@dataclass
+class FeaturedCommunity:
+    """Featured community dataclass model."""
+
+    community_id: str
+    id: str
+    created: str
+    updated: str
+    start_date: str
+
+    _table_name: InitVar[str] = "communities_featured"
```

### Comparing `invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/communities/transform.py` & `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/communities/transform.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,19 +21,25 @@
         pass
 
     @abstractmethod
     def _community_members(self, entry):
         """Transform the community members."""
         pass
 
+    @abstractmethod
+    def _featured_community(self, entry):
+        """Transform the featured community."""
+        pass
+
     def _transform(self, entry):
         """Transform a single entry."""
         return {
             "community": self._community(entry),
             "community_members": self._community_members(entry),
+            "featured_community": self._featured_community(entry),
         }
 
 
 class CommunityEntry(Entry):
     """Transform a single community entry."""
 
     @abstractmethod
@@ -188,7 +194,34 @@
     def transform(self, entry):
         """Transform a record single entry."""
         return {
             "community": self._community(entry),
             "record": self._record(entry),
             "request": self._request(entry),
         }
+
+
+class FeaturedCommunityEntry(Entry):
+    """Transform a single featured community entry."""
+
+    @abstractmethod
+    def _created(self, entry):
+        """Returns the creation date."""
+        pass
+
+    @abstractmethod
+    def _updated(self, entry):
+        """Returns the update date."""
+        pass
+
+    @abstractmethod
+    def _start_date(self, entry):
+        """Returns the start date."""
+        pass
+
+    def transform(self, entry):
+        """Transform a featured community entry."""
+        return {
+            "created": self._created(entry),
+            "updated": self._updated(entry),
+            "start_date": self._start_date(entry),
+        }
```

### Comparing `invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/records/load.py` & `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/records/load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/records/models.py` & `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/records/models.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -23,30 +23,14 @@
     bucket_id: str
     parent_id: str
 
     _table_name: InitVar[str] = "rdm_records_metadata"
 
 
 @dataclass
-class RDMRecordFile:
-    """RDM Record File dataclass model."""
-
-    id: str
-    json: dict
-    created: str
-    updated: str
-    version_id: int
-    key: str
-    record_id: str
-    object_version_id: str
-
-    _table_name: InitVar[str] = "rdm_records_files"
-
-
-@dataclass
 class RDMParentMetadata:
     """RDM Parent Metadata dataclass model."""
 
     id: str
     json: dict
     created: str
     updated: str
@@ -83,11 +67,27 @@
     expires_at: str
     fork_version_id: int
 
     _table_name: InitVar[str] = "rdm_drafts_metadata"
 
 
 @dataclass
+class RDMRecordFile:
+    """RDM Record File dataclass model."""
+
+    id: str
+    json: dict
+    created: str
+    updated: str
+    version_id: int
+    key: str
+    record_id: str
+    object_version_id: str
+
+    _table_name: InitVar[str] = "rdm_records_files"
+
+
+@dataclass
 class RDMDraftFile(RDMRecordFile):
     """RDM Draft File dataclass model."""
 
     _table_name: InitVar[str] = "rdm_drafts_files"
```

### Comparing `invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/records/table_generator.py` & `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/records/table_generator.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import random
 from datetime import datetime
 
 from ...load.models import PersistentIdentifier
 from ...load.postgresql import TableGenerator, generate_uuid
 from ..communities.models import RDMParentCommunityMetadata
-from .models import RDMParentMetadata, RDMRecordMetadata, RDMVersionState
+from .models import RDMParentMetadata, RDMRecordFile, RDMRecordMetadata, RDMVersionState
 
 
 class RDMVersionStateTableGenerator(TableGenerator):
     """RDM version state computed table."""
 
     def __init__(self, parent_cache):
         """Constructor."""
@@ -61,32 +61,45 @@
         "pk": _pid_pk(),
         "obj_type": "rec",
         "pid_type": "recid",
         "status": "R",
     }
 
 
+def generate_files_uuids(data):
+    """Generate uuid for every file in the list.
+
+    Return the transformed list with the generated ids.
+    """
+    _files = data["record_files"]
+    for _file in _files:
+        _file["id"] = generate_uuid({})
+    return _files
+
+
 class RDMRecordTableGenerator(TableGenerator):
     """RDM Record and related tables load."""
 
     def __init__(self, parent_cache, communities_cache):
         """Constructor."""
         super().__init__(
             tables=[
                 PersistentIdentifier,
                 RDMParentMetadata,
                 RDMRecordMetadata,
                 RDMParentCommunityMetadata,
+                RDMRecordFile,
             ],
             pks=[
                 ("record.id", generate_uuid),
                 ("parent.id", generate_uuid),
                 ("record.json.pid", _generate_recid),
                 ("parent.json.pid", _generate_recid),
                 ("record.parent_id", lambda d: d["parent"]["id"]),
+                ("record_files", generate_files_uuids),
             ],
         )
         self.parent_cache = parent_cache
         self.communities_cache = communities_cache
 
     def _generate_rows(self, data, **kwargs):
         now = datetime.utcnow().isoformat()
@@ -179,14 +192,27 @@
             # parent in cache - update version
             cached_parent = self.parent_cache[parent["json"]["id"]]
             # check if current record is a new version of the cached one
             if cached_parent["version"]["latest_index"] < rec["index"]:
                 cached_parent["version"] = dict(
                     latest_index=rec["index"], latest_id=rec["id"]
                 )
+        # record files
+        record_files = data["record_files"]
+        for _file in record_files:
+            yield RDMRecordFile(
+                id=_file["id"],
+                json=_file["json"],
+                created=_file["created"],
+                updated=_file["updated"],
+                version_id=_file["version_id"],
+                key=_file["key"],
+                record_id=rec["id"],
+                object_version_id=_file["object_version_id"],
+            )
 
     def _resolve_references(self, data, **kwargs):
         """Resolve references e.g communities slug names."""
 
         def _resolve_communities(communities):
             default_slug = communities.get("default")
             default_id = self.communities_cache.get(default_slug)
```

### Comparing `invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/records/transform.py` & `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/records/transform.py`

 * *Files 16% similar despite different names*

```diff
@@ -134,7 +134,62 @@
                 "pids": self._pids(entry),
                 "files": self._files(entry),
                 "metadata": self._metadata(entry),
                 "access": self._access(entry),
                 "custom_fields": self._custom_fields(entry),
             },
         }
+
+
+class RDMRecordFileEntry(Entry):
+    """Transform a single record file entry.
+
+    Connects records with files.
+    """
+
+    @abstractmethod
+    def _created(self, entry):
+        """Returns the creation date."""
+        pass
+
+    @abstractmethod
+    def _updated(self, entry):
+        """Returns the update date."""
+        pass
+
+    @abstractmethod
+    def _json(self, entry):
+        """Returns the rdm record file metadata."""
+        pass
+
+    @abstractmethod
+    def _version_id(self, entry):
+        """Returns the rdm record file version id."""
+        pass
+
+    @abstractmethod
+    def _key(self, entry):
+        """Returns the rdm record file key name."""
+        pass
+
+    @abstractmethod
+    def _object_version_id(self, entry):
+        """Returns the associated file object version ID."""
+        pass
+
+    def transform(self, entry):
+        """Transform a single record files entry."""
+        return {
+            "created": self._created(entry),
+            "updated": self._updated(entry),
+            "json": self._json(entry),
+            "version_id": self._version_id(entry),
+            "key": self._key(entry),
+            "object_version_id": self._object_version_id(entry),
+        }
+
+
+class RDMDraftFileEntry(RDMRecordFileEntry):
+    """Transform a single record file entry.
+
+    Connects draft with files.
+    """
```

### Comparing `invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/requests/load.py` & `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/requests/load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/requests/models.py` & `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/requests/models.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/requests/table_generator.py` & `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/requests/table_generator.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/requests/transform.py` & `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/requests/transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/runner.py` & `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/runner.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/streams.py` & `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/streams.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/users/load.py` & `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/users/load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/users/models.py` & `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/users/models.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/users/table_generator.py` & `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/users/table_generator.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/streams/users/transform.py` & `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/users/transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator/transform/base.py` & `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/transform/base.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator.egg-info/PKG-INFO` & `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-rdm-migrator
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: InvenioRDM module for data migration.
 Home-page: https://github.com/inveniosoftware/invenio-rdm-migrator
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2022 CERN.
@@ -179,16 +179,14 @@
         
         .. code-block:: python
         
             {
                 "record": self._record(entry),
                 "draft": self._draft(entry),
                 "parent": self._parent(entry),
-                "record_files": self._record_files(entry),
-                "draft_files": self._draft_files(entry),
             }
         
         This means that you will need to implement the functions for each key. Note
         that, only `_record` and `_parent` should return content, the others can return
         `None`. In this case we will need to re-think which methods should be
         `abstractmethod` and which ones be defaulted to `None/{}/some other default` in
         the base. You can find an example implementation at
```

### Comparing `invenio-rdm-migrator-1.0.0a3/invenio_rdm_migrator.egg-info/SOURCES.txt` & `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,19 @@
 invenio_rdm_migrator/streams/runner.py
 invenio_rdm_migrator/streams/streams.py
 invenio_rdm_migrator/streams/communities/__init__.py
 invenio_rdm_migrator/streams/communities/load.py
 invenio_rdm_migrator/streams/communities/models.py
 invenio_rdm_migrator/streams/communities/table_generator.py
 invenio_rdm_migrator/streams/communities/transform.py
+invenio_rdm_migrator/streams/files/__init__.py
+invenio_rdm_migrator/streams/files/load.py
+invenio_rdm_migrator/streams/files/models.py
+invenio_rdm_migrator/streams/files/table_generator.py
+invenio_rdm_migrator/streams/files/transform.py
 invenio_rdm_migrator/streams/records/__init__.py
 invenio_rdm_migrator/streams/records/load.py
 invenio_rdm_migrator/streams/records/models.py
 invenio_rdm_migrator/streams/records/table_generator.py
 invenio_rdm_migrator/streams/records/transform.py
 invenio_rdm_migrator/streams/requests/__init__.py
 invenio_rdm_migrator/streams/requests/load.py
@@ -58,11 +63,19 @@
 invenio_rdm_migrator/streams/users/load.py
 invenio_rdm_migrator/streams/users/models.py
 invenio_rdm_migrator/streams/users/table_generator.py
 invenio_rdm_migrator/streams/users/transform.py
 invenio_rdm_migrator/transform/__init__.py
 invenio_rdm_migrator/transform/base.py
 tests/conftest.py
+tests/streams/communities/conftest.py
+tests/streams/communities/test_communities_load.py
+tests/streams/communities/test_communities_table_generator.py
+tests/streams/communities/test_communities_transform.py
+tests/streams/files/conftest.py
+tests/streams/files/test_files_load.py
+tests/streams/files/test_files_table_generator.py
+tests/streams/files/test_files_transform.py
 tests/streams/requests/conftest.py
 tests/streams/requests/test_requests_load.py
 tests/streams/requests/test_requests_table_generator.py
 tests/streams/requests/test_requests_transform.py
```

### Comparing `invenio-rdm-migrator-1.0.0a3/run-tests.sh` & `invenio-rdm-migrator-1.0.0a4/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a3/setup.cfg` & `invenio-rdm-migrator-1.0.0a4/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a3/tests/conftest.py` & `invenio-rdm-migrator-1.0.0a4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a3/tests/streams/requests/conftest.py` & `invenio-rdm-migrator-1.0.0a4/tests/streams/requests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a3/tests/streams/requests/test_requests_load.py` & `invenio-rdm-migrator-1.0.0a4/tests/streams/requests/test_requests_load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a3/tests/streams/requests/test_requests_table_generator.py` & `invenio-rdm-migrator-1.0.0a4/tests/streams/requests/test_requests_table_generator.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a3/tests/streams/requests/test_requests_transform.py` & `invenio-rdm-migrator-1.0.0a4/tests/streams/requests/test_requests_transform.py`

 * *Files identical despite different names*

