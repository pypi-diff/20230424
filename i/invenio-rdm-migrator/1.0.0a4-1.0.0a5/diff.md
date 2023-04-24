# Comparing `tmp/invenio-rdm-migrator-1.0.0a4.tar.gz` & `tmp/invenio-rdm-migrator-1.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-rdm-migrator-1.0.0a4.tar", last modified: Mon Apr 24 08:51:28 2023, max compression
+gzip compressed data, was "dist/invenio-rdm-migrator-1.0.0a5.tar", last modified: Mon Apr 24 20:54:20 2023, max compression
```

## Comparing `invenio-rdm-migrator-1.0.0a4.tar` & `invenio-rdm-migrator-1.0.0a5.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/extract/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/extract/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/load/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/load/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/load/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/load/postgresql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/communities/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/communities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/communities/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/communities/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/communities/table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/communities/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/files/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/files/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/files/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/files/table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/files/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/records/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/records/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/records/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9595 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/records/table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/records/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/requests/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/requests/load.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/requests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/requests/table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/requests/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/streams.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/users/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/users/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/users/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/users/table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/users/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/transform/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/transform/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-04-24 08:51:27.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 08:51:27.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 08:51:27.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-24 08:51:27.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-24 08:51:27.000000 invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1410 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/tests/streams/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/tests/streams/communities/
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/tests/streams/communities/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/tests/streams/communities/test_communities_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/tests/streams/communities/test_communities_table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/tests/streams/communities/test_communities_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/tests/streams/files/
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/tests/streams/files/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/tests/streams/files/test_files_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/tests/streams/files/test_files_table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/tests/streams/files/test_files_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:51:28.000000 invenio-rdm-migrator-1.0.0a4/tests/streams/requests/
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/tests/streams/requests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/tests/streams/requests/test_requests_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/tests/streams/requests/test_requests_table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-04-24 08:51:22.000000 invenio-rdm-migrator-1.0.0a4/tests/streams/requests/test_requests_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/extract/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/extract/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/load/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/load/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/load/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/load/postgresql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/communities/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/communities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/communities/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/communities/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/communities/table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/communities/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/files/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/files/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/files/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/files/table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/files/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/records/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/records/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/records/table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/records/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/requests/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/requests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/requests/table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/requests/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/streams.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/users/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/users/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/users/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/users/table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/users/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/transform/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1410 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/tests/streams/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/tests/streams/communities/
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/tests/streams/communities/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/tests/streams/communities/test_communities_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/tests/streams/communities/test_communities_table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/tests/streams/communities/test_communities_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/tests/streams/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/tests/streams/files/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/tests/streams/files/test_files_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/tests/streams/files/test_files_table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/tests/streams/files/test_files_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:54:20.000000 invenio-rdm-migrator-1.0.0a5/tests/streams/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/tests/streams/requests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/tests/streams/requests/test_requests_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/tests/streams/requests/test_requests_table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-04-24 20:54:15.000000 invenio-rdm-migrator-1.0.0a5/tests/streams/requests/test_requests_transform.py
```

### Comparing `invenio-rdm-migrator-1.0.0a4/.editorconfig` & `invenio-rdm-migrator-1.0.0a5/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/.github/workflows/pypi-publish.yml` & `invenio-rdm-migrator-1.0.0a5/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/.github/workflows/tests.yml` & `invenio-rdm-migrator-1.0.0a5/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/CONTRIBUTING.rst` & `invenio-rdm-migrator-1.0.0a5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/LICENSE` & `invenio-rdm-migrator-1.0.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/MANIFEST.in` & `invenio-rdm-migrator-1.0.0a5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/PKG-INFO` & `invenio-rdm-migrator-1.0.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-rdm-migrator
-Version: 1.0.0a4
+Version: 1.0.0a5
 Summary: InvenioRDM module for data migration.
 Home-page: https://github.com/inveniosoftware/invenio-rdm-migrator
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2022 CERN.
```

### Comparing `invenio-rdm-migrator-1.0.0a4/README.rst` & `invenio-rdm-migrator-1.0.0a5/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/docs/Makefile` & `invenio-rdm-migrator-1.0.0a5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/docs/conf.py` & `invenio-rdm-migrator-1.0.0a5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/docs/index.rst` & `invenio-rdm-migrator-1.0.0a5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/docs/make.bat` & `invenio-rdm-migrator-1.0.0a5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/load/base.py` & `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/load/base.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/load/models.py` & `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/load/models.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/load/postgresql.py` & `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/load/postgresql.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/communities/__init__.py` & `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/communities/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/communities/load.py` & `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/communities/load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/communities/models.py` & `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/communities/models.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/communities/table_generator.py` & `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/communities/table_generator.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/communities/transform.py` & `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/communities/transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/files/__init__.py` & `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/files/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/files/load.py` & `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/files/load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/files/models.py` & `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/files/models.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/files/table_generator.py` & `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/files/table_generator.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/files/transform.py` & `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/files/transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/records/load.py` & `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/records/load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/records/models.py` & `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/records/models.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/records/table_generator.py` & `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/records/table_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,29 +72,35 @@
     """
     _files = data["record_files"]
     for _file in _files:
         _file["id"] = generate_uuid({})
     return _files
 
 
+def generate_record_uuid(data):
+    """Generate record uuid if not present."""
+    _id = data.get("id")
+    return _id if _id else generate_uuid(None)
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
                 RDMRecordFile,
             ],
             pks=[
-                ("record.id", generate_uuid),
+                ("record.id", generate_record_uuid),
                 ("parent.id", generate_uuid),
                 ("record.json.pid", _generate_recid),
                 ("parent.json.pid", _generate_recid),
                 ("record.parent_id", lambda d: d["parent"]["id"]),
                 ("record_files", generate_files_uuids),
             ],
         )
```

### Comparing `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/records/transform.py` & `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/records/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,19 @@
             yield self._transform(entry)
 
 
 class RDMRecordEntry(Entry):
     """Transform a single record entry."""
 
     @abstractmethod
+    def _id(self, entry):
+        """Returns the rdm record uuid."""
+        pass
+
+    @abstractmethod
     def _created(self, entry):
         """Returns the creation date of the record."""
         pass
 
     @abstractmethod
     def _updated(self, entry):
         """Returns the update date of the record."""
@@ -121,14 +126,15 @@
     def _custom_fields(self, entry):
         """Transform the custom fields of a record."""
         pass
 
     def transform(self, entry):
         """Transform a record single entry."""
         return {
+            "id": self._id(entry),
             "created": self._created(entry),
             "updated": self._updated(entry),
             "version_id": self._version_id(entry),
             "index": self._index(entry),
             "json": {
                 "id": self._recid(entry),
                 "pids": self._pids(entry),
```

### Comparing `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/requests/load.py` & `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/requests/load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/requests/models.py` & `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/requests/models.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/requests/table_generator.py` & `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/requests/table_generator.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/requests/transform.py` & `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/requests/transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/runner.py` & `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/runner.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/streams.py` & `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/streams.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/users/load.py` & `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/users/load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/users/models.py` & `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/users/models.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/users/table_generator.py` & `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/users/table_generator.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/streams/users/transform.py` & `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/streams/users/transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator/transform/base.py` & `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator/transform/base.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator.egg-info/PKG-INFO` & `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-rdm-migrator
-Version: 1.0.0a4
+Version: 1.0.0a5
 Summary: InvenioRDM module for data migration.
 Home-page: https://github.com/inveniosoftware/invenio-rdm-migrator
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2022 CERN.
```

### Comparing `invenio-rdm-migrator-1.0.0a4/invenio_rdm_migrator.egg-info/SOURCES.txt` & `invenio-rdm-migrator-1.0.0a5/invenio_rdm_migrator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/run-tests.sh` & `invenio-rdm-migrator-1.0.0a5/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/setup.cfg` & `invenio-rdm-migrator-1.0.0a5/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/tests/conftest.py` & `invenio-rdm-migrator-1.0.0a5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/tests/streams/communities/conftest.py` & `invenio-rdm-migrator-1.0.0a5/tests/streams/communities/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/tests/streams/communities/test_communities_load.py` & `invenio-rdm-migrator-1.0.0a5/tests/streams/communities/test_communities_load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/tests/streams/communities/test_communities_table_generator.py` & `invenio-rdm-migrator-1.0.0a5/tests/streams/communities/test_communities_table_generator.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/tests/streams/communities/test_communities_transform.py` & `invenio-rdm-migrator-1.0.0a5/tests/streams/communities/test_communities_transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/tests/streams/files/conftest.py` & `invenio-rdm-migrator-1.0.0a5/tests/streams/files/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/tests/streams/files/test_files_load.py` & `invenio-rdm-migrator-1.0.0a5/tests/streams/files/test_files_load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/tests/streams/files/test_files_table_generator.py` & `invenio-rdm-migrator-1.0.0a5/tests/streams/files/test_files_table_generator.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/tests/streams/files/test_files_transform.py` & `invenio-rdm-migrator-1.0.0a5/tests/streams/files/test_files_transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/tests/streams/requests/conftest.py` & `invenio-rdm-migrator-1.0.0a5/tests/streams/requests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/tests/streams/requests/test_requests_load.py` & `invenio-rdm-migrator-1.0.0a5/tests/streams/requests/test_requests_load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/tests/streams/requests/test_requests_table_generator.py` & `invenio-rdm-migrator-1.0.0a5/tests/streams/requests/test_requests_table_generator.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a4/tests/streams/requests/test_requests_transform.py` & `invenio-rdm-migrator-1.0.0a5/tests/streams/requests/test_requests_transform.py`

 * *Files identical despite different names*

