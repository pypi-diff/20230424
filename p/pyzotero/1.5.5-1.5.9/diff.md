# Comparing `tmp/pyzotero-1.5.5.tar.gz` & `tmp/pyzotero-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyzotero-1.5.5.tar", last modified: Tue Jul  5 09:41:13 2022, max compression
+gzip compressed data, was "pyzotero-1.5.9.tar", last modified: Mon Apr 24 11:46:24 2023, max compression
```

## Comparing `pyzotero-1.5.5.tar` & `pyzotero-1.5.9.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 sth        (501) staff       (20)        0 2022-07-05 09:41:13.864596 pyzotero-1.5.5/
--rw-r--r--   0 sth        (501) staff       (20)      158 2022-03-01 10:41:04.000000 pyzotero-1.5.5/ pyproject.toml
--rw-r--r--   0 sth        (501) staff       (20)      157 2022-03-01 10:41:04.000000 pyzotero-1.5.5/.coveragerc
-drwxr-xr-x   0 sth        (501) staff       (20)        0 2022-07-05 09:41:13.841211 pyzotero-1.5.5/.github/
-drwxr-xr-x   0 sth        (501) staff       (20)        0 2022-07-05 09:41:13.842433 pyzotero-1.5.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 sth        (501) staff       (20)      932 2021-08-10 14:02:08.000000 pyzotero-1.5.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 sth        (501) staff       (20)      466 2021-08-10 14:02:08.000000 pyzotero-1.5.5/.github/ISSUE_TEMPLATE/usage_question.md
--rw-r--r--   0 sth        (501) staff       (20)     1427 2021-03-20 15:31:10.000000 pyzotero-1.5.5/.github/pull_request_template.md
-drwxr-xr-x   0 sth        (501) staff       (20)        0 2022-07-05 09:41:13.843032 pyzotero-1.5.5/.github/workflows/
--rw-r--r--   0 sth        (501) staff       (20)     1008 2022-03-01 10:41:04.000000 pyzotero-1.5.5/.github/workflows/tests.yml
--rw-r--r--   0 sth        (501) staff       (20)       69 2022-03-01 10:41:04.000000 pyzotero-1.5.5/.gitignore
--rw-r--r--   0 sth        (501) staff       (20)       85 2018-08-23 15:26:30.000000 pyzotero-1.5.5/.readthedocs.yml
--rw-r--r--   0 sth        (501) staff       (20)      110 2018-08-23 15:26:30.000000 pyzotero-1.5.5/AUTHORS
--rw-r--r--   0 sth        (501) staff       (20)      450 2021-08-10 14:02:08.000000 pyzotero-1.5.5/CITATION.cff
--rw-r--r--   0 sth        (501) staff       (20)     1451 2018-11-30 12:38:33.000000 pyzotero-1.5.5/CONTRIBUTING.md
--rw-r--r--   0 sth        (501) staff       (20)     1466 2022-03-01 10:41:04.000000 pyzotero-1.5.5/CONTRIBUTORS.md
--rw-r--r--   0 sth        (501) staff       (20)       60 2021-07-29 12:10:45.000000 pyzotero-1.5.5/MANIFEST.in
--rw-r--r--   0 sth        (501) staff       (20)     5157 2022-07-05 09:41:13.864848 pyzotero-1.5.5/PKG-INFO
--rw-r--r--   0 sth        (501) staff       (20)     4050 2022-03-01 13:55:51.000000 pyzotero-1.5.5/README.md
--rw-r--r--   0 sth        (501) staff       (20)        0 2018-08-23 15:26:30.000000 pyzotero-1.5.5/__init__.py
-drwxr-xr-x   0 sth        (501) staff       (20)        0 2022-07-05 09:41:13.847832 pyzotero-1.5.5/doc/
--rw-r--r--   0 sth        (501) staff       (20)     4598 2018-08-23 15:26:30.000000 pyzotero-1.5.5/doc/Makefile
-drwxr-xr-x   0 sth        (501) staff       (20)        0 2022-07-05 09:41:13.849178 pyzotero-1.5.5/doc/_templates/
--rw-r--r--   0 sth        (501) staff       (20)      820 2018-08-23 15:26:30.000000 pyzotero-1.5.5/doc/_templates/layout.html
--rw-r--r--   0 sth        (501) staff       (20)   461760 2018-08-23 15:26:30.000000 pyzotero-1.5.5/doc/cat.png
--rw-r--r--   0 sth        (501) staff       (20)     8342 2022-03-01 10:41:04.000000 pyzotero-1.5.5/doc/conf.py
--rw-r--r--   0 sth        (501) staff       (20)    44497 2022-03-01 10:41:04.000000 pyzotero-1.5.5/doc/index.rst
--rw-r--r--   0 sth        (501) staff       (20)      639 2022-03-01 10:41:04.000000 pyzotero-1.5.5/dump_contributors.py
--rw-r--r--   0 sth        (501) staff       (20)     1081 2018-08-23 15:26:30.000000 pyzotero-1.5.5/license.txt
--rw-r--r--   0 sth        (501) staff       (20)     1294 2022-03-01 13:55:51.000000 pyzotero-1.5.5/pre-deploy.py
-drwxr-xr-x   0 sth        (501) staff       (20)        0 2022-07-05 09:41:13.851387 pyzotero-1.5.5/pyzotero/
--rw-r--r--   0 sth        (501) staff       (20)        0 2018-08-23 15:26:30.000000 pyzotero-1.5.5/pyzotero/__init__.py
--rw-r--r--   0 sth        (501) staff       (20)       22 2022-07-05 09:36:26.000000 pyzotero-1.5.5/pyzotero/version.py
--rw-r--r--   0 sth        (501) staff       (20)    74854 2022-07-05 09:36:13.000000 pyzotero-1.5.5/pyzotero/zotero.py
--rw-r--r--   0 sth        (501) staff       (20)     3664 2022-03-01 10:41:04.000000 pyzotero-1.5.5/pyzotero/zotero_errors.py
-drwxr-xr-x   0 sth        (501) staff       (20)        0 2022-07-05 09:41:13.854171 pyzotero-1.5.5/pyzotero.egg-info/
--rw-r--r--   0 sth        (501) staff       (20)     5157 2022-07-05 09:41:13.000000 pyzotero-1.5.5/pyzotero.egg-info/PKG-INFO
--rw-r--r--   0 sth        (501) staff       (20)     1416 2022-07-05 09:41:13.000000 pyzotero-1.5.5/pyzotero.egg-info/SOURCES.txt
--rw-r--r--   0 sth        (501) staff       (20)        1 2022-07-05 09:41:13.000000 pyzotero-1.5.5/pyzotero.egg-info/dependency_links.txt
--rw-r--r--   0 sth        (501) staff       (20)        1 2021-12-10 17:09:59.000000 pyzotero-1.5.5/pyzotero.egg-info/not-zip-safe
--rw-r--r--   0 sth        (501) staff       (20)       92 2022-07-05 09:41:13.000000 pyzotero-1.5.5/pyzotero.egg-info/requires.txt
--rw-r--r--   0 sth        (501) staff       (20)        9 2022-07-05 09:41:13.000000 pyzotero-1.5.5/pyzotero.egg-info/top_level.txt
--rw-r--r--   0 sth        (501) staff       (20)     1459 2022-07-05 09:41:13.865612 pyzotero-1.5.5/setup.cfg
--rwxr-xr-x   0 sth        (501) staff       (20)      151 2022-03-01 10:41:04.000000 pyzotero-1.5.5/setup.py
-drwxr-xr-x   0 sth        (501) staff       (20)        0 2022-07-05 09:41:13.854539 pyzotero-1.5.5/tests/
-drwxr-xr-x   0 sth        (501) staff       (20)        0 2022-07-05 09:41:13.863998 pyzotero-1.5.5/tests/api_responses/
--rw-r--r--   0 sth        (501) staff       (20)        0 2022-03-01 10:41:04.000000 pyzotero-1.5.5/tests/api_responses/__init__.py
--rw-r--r--   0 sth        (501) staff       (20)     1562 2022-03-01 10:41:04.000000 pyzotero-1.5.5/tests/api_responses/attachments_doc.json
--rw-r--r--   0 sth        (501) staff       (20)      985 2022-03-01 10:41:04.000000 pyzotero-1.5.5/tests/api_responses/citation_doc.xml
--rw-r--r--   0 sth        (501) staff       (20)      898 2022-03-01 10:41:04.000000 pyzotero-1.5.5/tests/api_responses/collection_doc.json
--rw-r--r--   0 sth        (501) staff       (20)     1323 2022-03-01 10:41:04.000000 pyzotero-1.5.5/tests/api_responses/collection_tags.json
--rw-r--r--   0 sth        (501) staff       (20)       46 2022-03-01 10:41:04.000000 pyzotero-1.5.5/tests/api_responses/collection_versions.json
--rw-r--r--   0 sth        (501) staff       (20)    13646 2022-03-01 10:41:04.000000 pyzotero-1.5.5/tests/api_responses/collections_doc.json
--rw-r--r--   0 sth        (501) staff       (20)       87 2022-03-01 10:41:04.000000 pyzotero-1.5.5/tests/api_responses/creation_doc.json
--rw-r--r--   0 sth        (501) staff       (20)      810 2022-03-01 10:41:04.000000 pyzotero-1.5.5/tests/api_responses/groups_doc.json
--rw-r--r--   0 sth        (501) staff       (20)     3242 2022-03-01 10:41:04.000000 pyzotero-1.5.5/tests/api_responses/item_doc.json
--rw-r--r--   0 sth        (501) staff       (20)     7842 2022-03-01 10:41:04.000000 pyzotero-1.5.5/tests/api_responses/item_fields.json
--rw-r--r--   0 sth        (501) staff       (20)       21 2022-03-01 10:41:04.000000 pyzotero-1.5.5/tests/api_responses/item_file.pdf
--rw-r--r--   0 sth        (501) staff       (20)      226 2022-03-01 10:41:04.000000 pyzotero-1.5.5/tests/api_responses/item_template.json
--rw-r--r--   0 sth        (501) staff       (20)     2252 2022-03-01 10:41:04.000000 pyzotero-1.5.5/tests/api_responses/item_types.json
--rw-r--r--   0 sth        (501) staff       (20)       46 2022-03-01 10:41:04.000000 pyzotero-1.5.5/tests/api_responses/item_versions.json
--rw-r--r--   0 sth        (501) staff       (20)    49217 2022-03-01 10:41:04.000000 pyzotero-1.5.5/tests/api_responses/items_doc.json
--rw-r--r--   0 sth        (501) staff       (20)       90 2022-03-01 10:41:04.000000 pyzotero-1.5.5/tests/api_responses/keys_doc.txt
--rw-r--r--   0 sth        (501) staff       (20)      525 2022-03-01 10:41:04.000000 pyzotero-1.5.5/tests/api_responses/tags_doc.json
--rw-r--r--   0 sth        (501) staff       (20)    27808 2022-03-01 13:34:59.000000 pyzotero-1.5.5/tests/test_zotero.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:46:24.328023 pyzotero-1.5.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-24 11:46:13.000000 pyzotero-1.5.9/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:46:24.320023 pyzotero-1.5.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:46:24.320023 pyzotero-1.5.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-24 11:46:13.000000 pyzotero-1.5.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-24 11:46:13.000000 pyzotero-1.5.9/.github/ISSUE_TEMPLATE/usage_question.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-24 11:46:13.000000 pyzotero-1.5.9/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:46:24.320023 pyzotero-1.5.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-04-24 11:46:13.000000 pyzotero-1.5.9/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-24 11:46:13.000000 pyzotero-1.5.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-24 11:46:13.000000 pyzotero-1.5.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-24 11:46:13.000000 pyzotero-1.5.9/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-24 11:46:13.000000 pyzotero-1.5.9/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-24 11:46:13.000000 pyzotero-1.5.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-24 11:46:13.000000 pyzotero-1.5.9/CONTRIBUTORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-04-24 11:46:24.328023 pyzotero-1.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-04-24 11:46:13.000000 pyzotero-1.5.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 11:46:13.000000 pyzotero-1.5.9/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:46:24.324023 pyzotero-1.5.9/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-04-24 11:46:13.000000 pyzotero-1.5.9/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:46:24.324023 pyzotero-1.5.9/doc/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-24 11:46:13.000000 pyzotero-1.5.9/doc/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)   461760 2023-04-24 11:46:13.000000 pyzotero-1.5.9/doc/cat.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-04-24 11:46:13.000000 pyzotero-1.5.9/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44493 2023-04-24 11:46:13.000000 pyzotero-1.5.9/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-24 11:46:13.000000 pyzotero-1.5.9/dump_contributors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-24 11:46:13.000000 pyzotero-1.5.9/license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-24 11:46:13.000000 pyzotero-1.5.9/manifest.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-24 11:46:13.000000 pyzotero-1.5.9/pre-deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-24 11:46:13.000000 pyzotero-1.5.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:46:24.324023 pyzotero-1.5.9/pyzotero/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 11:46:13.000000 pyzotero-1.5.9/pyzotero/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-24 11:46:13.000000 pyzotero-1.5.9/pyzotero/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74840 2023-04-24 11:46:13.000000 pyzotero-1.5.9/pyzotero/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-04-24 11:46:13.000000 pyzotero-1.5.9/pyzotero/zotero_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:46:24.324023 pyzotero-1.5.9/pyzotero.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-04-24 11:46:24.000000 pyzotero-1.5.9/pyzotero.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-24 11:46:24.000000 pyzotero-1.5.9/pyzotero.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 11:46:24.000000 pyzotero-1.5.9/pyzotero.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 11:46:24.000000 pyzotero-1.5.9/pyzotero.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-24 11:46:24.000000 pyzotero-1.5.9/pyzotero.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-24 11:46:24.000000 pyzotero-1.5.9/pyzotero.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-24 11:46:24.328023 pyzotero-1.5.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      151 2023-04-24 11:46:13.000000 pyzotero-1.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:46:24.324023 pyzotero-1.5.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:46:24.328023 pyzotero-1.5.9/tests/api_responses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 11:46:13.000000 pyzotero-1.5.9/tests/api_responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-24 11:46:13.000000 pyzotero-1.5.9/tests/api_responses/attachments_doc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-24 11:46:13.000000 pyzotero-1.5.9/tests/api_responses/citation_doc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-24 11:46:13.000000 pyzotero-1.5.9/tests/api_responses/collection_doc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-24 11:46:13.000000 pyzotero-1.5.9/tests/api_responses/collection_tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-24 11:46:13.000000 pyzotero-1.5.9/tests/api_responses/collection_versions.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13646 2023-04-24 11:46:13.000000 pyzotero-1.5.9/tests/api_responses/collections_doc.json
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-24 11:46:13.000000 pyzotero-1.5.9/tests/api_responses/creation_doc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-24 11:46:13.000000 pyzotero-1.5.9/tests/api_responses/groups_doc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-24 11:46:13.000000 pyzotero-1.5.9/tests/api_responses/item_doc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-04-24 11:46:13.000000 pyzotero-1.5.9/tests/api_responses/item_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-24 11:46:13.000000 pyzotero-1.5.9/tests/api_responses/item_file.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-24 11:46:13.000000 pyzotero-1.5.9/tests/api_responses/item_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-04-24 11:46:13.000000 pyzotero-1.5.9/tests/api_responses/item_types.json
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-24 11:46:13.000000 pyzotero-1.5.9/tests/api_responses/item_versions.json
+-rw-r--r--   0 runner    (1001) docker     (123)    49217 2023-04-24 11:46:13.000000 pyzotero-1.5.9/tests/api_responses/items_doc.json
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-24 11:46:13.000000 pyzotero-1.5.9/tests/api_responses/keys_doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-24 11:46:13.000000 pyzotero-1.5.9/tests/api_responses/tags_doc.json
+-rw-r--r--   0 runner    (1001) docker     (123)    27808 2023-04-24 11:46:13.000000 pyzotero-1.5.9/tests/test_zotero.py
```

### Comparing `pyzotero-1.5.5/.github/ISSUE_TEMPLATE/bug_report.md` & `pyzotero-1.5.9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `pyzotero-1.5.5/.github/pull_request_template.md` & `pyzotero-1.5.9/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pyzotero-1.5.5/CONTRIBUTING.md` & `pyzotero-1.5.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyzotero-1.5.5/CONTRIBUTORS.md` & `pyzotero-1.5.9/CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `pyzotero-1.5.5/PKG-INFO` & `pyzotero-1.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: pyzotero
-Version: 1.5.5
+Version: 1.5.9
 Summary: Python wrapper for the Zotero API
 Home-page: https://github.com/urschrei/pyzotero
 Author: Stephan Hügel
 Author-email: urschrei@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/urschrei/pyzotero
 Project-URL: Tracker, https://github.com/urschrei/pyzotero/issues
 Keywords: zotero
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: test
 Provides-Extra: all
 License-File: license.txt
 
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/Pyzotero.svg?style=flat)](https://pypi.python.org/pypi/Pyzotero/) [![Docs](https://readthedocs.org/projects/pyzotero/badge/?version=latest)](http://pyzotero.readthedocs.org/en/latest/?badge=latest) [![MIT licensed](https://img.shields.io/badge/license-MIT-blue.svg)](license.txt) [![PyPI Version](https://img.shields.io/pypi/v/Pyzotero.svg)](https://pypi.python.org/pypi/Pyzotero) [![Anaconda-Server Badge](https://anaconda.org/conda-forge/pyzotero/badges/version.svg)](https://anaconda.org/conda-forge/pyzotero) [![Downloads](https://pepy.tech/badge/pyzotero)](https://pepy.tech/project/pyzotero)  
 
@@ -55,15 +54,15 @@
 
 # Documentation
 
 Full documentation of available Pyzotero methods, code examples, and sample output is available on [Read The Docs][3].
 
 # Installation
 
-* Using [pip][10]: `pip install pyzotero` (it's available as a wheel, and is tested on Python 3.6 and up)
+* Using [pip][10]: `pip install pyzotero` (it's available as a wheel, and is tested on Python 3.7 and up)
 * Using Anaconda:`conda config --add channels conda-forge && conda install pyzotero`
 * From a local clone, if you wish to install Pyzotero from a specific branch: 
 
 Example:
 
 ``` bash
 git clone git://github.com/urschrei/pyzotero.git
```

### Comparing `pyzotero-1.5.5/README.md` & `pyzotero-1.5.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 # Documentation
 
 Full documentation of available Pyzotero methods, code examples, and sample output is available on [Read The Docs][3].
 
 # Installation
 
-* Using [pip][10]: `pip install pyzotero` (it's available as a wheel, and is tested on Python 3.6 and up)
+* Using [pip][10]: `pip install pyzotero` (it's available as a wheel, and is tested on Python 3.7 and up)
 * Using Anaconda:`conda config --add channels conda-forge && conda install pyzotero`
 * From a local clone, if you wish to install Pyzotero from a specific branch: 
 
 Example:
 
 ``` bash
 git clone git://github.com/urschrei/pyzotero.git
```

### Comparing `pyzotero-1.5.5/doc/Makefile` & `pyzotero-1.5.9/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pyzotero-1.5.5/doc/_templates/layout.html` & `pyzotero-1.5.9/doc/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `pyzotero-1.5.5/doc/cat.png` & `pyzotero-1.5.9/doc/cat.png`

 * *Files identical despite different names*

### Comparing `pyzotero-1.5.5/doc/conf.py` & `pyzotero-1.5.9/doc/conf.py`

 * *Files identical despite different names*

### Comparing `pyzotero-1.5.5/doc/index.rst` & `pyzotero-1.5.9/doc/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -662,15 +662,15 @@
         # set parameters on the call itself
         z = zot.top(limit=7, start=3)
 
         # set parameters using explicit method
         zot.add_parameters(limit=7, start=3)
         z = zot.top()
 
-The following parameters are are **optional**.
+The following parameters are **optional**.
 
 **You may also set a search term here, using the 'itemType', 'q', 'qmode', or 'tag' parameters**.
 
 This area of the Zotero Read API is under development, and may change frequently. See `the API documentation <https://www.zotero.org/support/dev/web_api/v3/basics#read_requests>`_ for the most up-to-date details of search syntax usage and export format details.
```

### Comparing `pyzotero-1.5.5/dump_contributors.py` & `pyzotero-1.5.9/dump_contributors.py`

 * *Files identical despite different names*

### Comparing `pyzotero-1.5.5/license.txt` & `pyzotero-1.5.9/license.txt`

 * *Files identical despite different names*

### Comparing `pyzotero-1.5.5/pre-deploy.py` & `pyzotero-1.5.9/pre-deploy.py`

 * *Files identical despite different names*

### Comparing `pyzotero-1.5.5/pyzotero/zotero.py` & `pyzotero-1.5.9/pyzotero/zotero.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 
 __author__ = "Stephan Hügel"
 __api_version__ = "3"
 __version__ = pzv.__version__
 
 import requests
 from requests import Request
-import socket
 import feedparser
 import bibtexparser
 import json
 import copy
 import uuid
 import time
 import threading
```

### Comparing `pyzotero-1.5.5/pyzotero/zotero_errors.py` & `pyzotero-1.5.9/pyzotero/zotero_errors.py`

 * *Files identical despite different names*

### Comparing `pyzotero-1.5.5/pyzotero.egg-info/PKG-INFO` & `pyzotero-1.5.9/pyzotero.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: pyzotero
-Version: 1.5.5
+Version: 1.5.9
 Summary: Python wrapper for the Zotero API
 Home-page: https://github.com/urschrei/pyzotero
 Author: Stephan Hügel
 Author-email: urschrei@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/urschrei/pyzotero
 Project-URL: Tracker, https://github.com/urschrei/pyzotero/issues
 Keywords: zotero
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: test
 Provides-Extra: all
 License-File: license.txt
 
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/Pyzotero.svg?style=flat)](https://pypi.python.org/pypi/Pyzotero/) [![Docs](https://readthedocs.org/projects/pyzotero/badge/?version=latest)](http://pyzotero.readthedocs.org/en/latest/?badge=latest) [![MIT licensed](https://img.shields.io/badge/license-MIT-blue.svg)](license.txt) [![PyPI Version](https://img.shields.io/pypi/v/Pyzotero.svg)](https://pypi.python.org/pypi/Pyzotero) [![Anaconda-Server Badge](https://anaconda.org/conda-forge/pyzotero/badges/version.svg)](https://anaconda.org/conda-forge/pyzotero) [![Downloads](https://pepy.tech/badge/pyzotero)](https://pepy.tech/project/pyzotero)  
 
@@ -55,15 +54,15 @@
 
 # Documentation
 
 Full documentation of available Pyzotero methods, code examples, and sample output is available on [Read The Docs][3].
 
 # Installation
 
-* Using [pip][10]: `pip install pyzotero` (it's available as a wheel, and is tested on Python 3.6 and up)
+* Using [pip][10]: `pip install pyzotero` (it's available as a wheel, and is tested on Python 3.7 and up)
 * Using Anaconda:`conda config --add channels conda-forge && conda install pyzotero`
 * From a local clone, if you wish to install Pyzotero from a specific branch: 
 
 Example:
 
 ``` bash
 git clone git://github.com/urschrei/pyzotero.git
```

### Comparing `pyzotero-1.5.5/pyzotero.egg-info/SOURCES.txt` & `pyzotero-1.5.9/pyzotero.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,21 @@
- pyproject.toml
 .coveragerc
 .gitignore
 .readthedocs.yml
 AUTHORS
 CITATION.cff
 CONTRIBUTING.md
 CONTRIBUTORS.md
-MANIFEST.in
 README.md
 __init__.py
 dump_contributors.py
 license.txt
 manifest.in
 pre-deploy.py
-readme.md
+pyproject.toml
 setup.cfg
 setup.py
 .github/pull_request_template.md
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/usage_question.md
 .github/workflows/tests.yml
 doc/Makefile
```

### Comparing `pyzotero-1.5.5/setup.cfg` & `pyzotero-1.5.9/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 description = Python wrapper for the Zotero API
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8
 url = https://github.com/urschrei/pyzotero
 author = Stephan Hügel
 author_email = urschrei@gmail.com
 license = MIT
-license_file = license.txt
+license_files = license.txt
 keywords = zotero
 classifiers = 
 	Programming Language :: Python
-	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	Intended Audience :: Education
@@ -33,15 +32,15 @@
 platforms = any
 include_package_data = True
 install_requires = 
 	feedparser >= 6
 	pytz
 	requests >= 2.21.0
 	bibtexparser
-python_requires = >=3.6
+python_requires = >=3.7
 setup_requires = 
 	setuptools_scm
 tests_require = 
 	pytest >= 6.2.2
 	httpretty
 	python-dateutil
 test_suite = test
```

### Comparing `pyzotero-1.5.5/tests/api_responses/attachments_doc.json` & `pyzotero-1.5.9/tests/api_responses/attachments_doc.json`

 * *Files identical despite different names*

### Comparing `pyzotero-1.5.5/tests/api_responses/citation_doc.xml` & `pyzotero-1.5.9/tests/api_responses/citation_doc.xml`

 * *Files identical despite different names*

### Comparing `pyzotero-1.5.5/tests/api_responses/collection_doc.json` & `pyzotero-1.5.9/tests/api_responses/collection_doc.json`

 * *Files identical despite different names*

### Comparing `pyzotero-1.5.5/tests/api_responses/collection_tags.json` & `pyzotero-1.5.9/tests/api_responses/collection_tags.json`

 * *Files identical despite different names*

### Comparing `pyzotero-1.5.5/tests/api_responses/collections_doc.json` & `pyzotero-1.5.9/tests/api_responses/collections_doc.json`

 * *Files identical despite different names*

### Comparing `pyzotero-1.5.5/tests/api_responses/groups_doc.json` & `pyzotero-1.5.9/tests/api_responses/groups_doc.json`

 * *Files identical despite different names*

### Comparing `pyzotero-1.5.5/tests/api_responses/item_doc.json` & `pyzotero-1.5.9/tests/api_responses/item_doc.json`

 * *Files identical despite different names*

### Comparing `pyzotero-1.5.5/tests/api_responses/item_fields.json` & `pyzotero-1.5.9/tests/api_responses/item_fields.json`

 * *Files identical despite different names*

### Comparing `pyzotero-1.5.5/tests/api_responses/item_types.json` & `pyzotero-1.5.9/tests/api_responses/item_types.json`

 * *Files identical despite different names*

### Comparing `pyzotero-1.5.5/tests/api_responses/items_doc.json` & `pyzotero-1.5.9/tests/api_responses/items_doc.json`

 * *Files identical despite different names*

### Comparing `pyzotero-1.5.5/tests/api_responses/tags_doc.json` & `pyzotero-1.5.9/tests/api_responses/tags_doc.json`

 * *Files identical despite different names*

### Comparing `pyzotero-1.5.5/tests/test_zotero.py` & `pyzotero-1.5.9/tests/test_zotero.py`

 * *Files identical despite different names*

