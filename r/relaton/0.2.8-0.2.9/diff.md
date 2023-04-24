# Comparing `tmp/relaton-0.2.8.tar.gz` & `tmp/relaton-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relaton-0.2.8.tar", last modified: Sun Jul 10 17:09:46 2022, max compression
+gzip compressed data, was "relaton-0.2.9.tar", last modified: Thu Jul 14 00:17:00 2022, max compression
```

## Comparing `relaton-0.2.8.tar` & `relaton-0.2.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 17:09:46.759624 relaton-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-07-10 17:09:36.000000 relaton-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-07-10 17:09:36.000000 relaton-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1220 2022-07-10 17:09:46.759624 relaton-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      321 2022-07-10 17:09:36.000000 relaton-0.2.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 17:09:46.755624 relaton-0.2.8/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     3482 2022-07-10 17:09:36.000000 relaton-0.2.8/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3001 2022-07-10 17:09:36.000000 relaton-0.2.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1864 2022-07-10 17:09:36.000000 relaton-0.2.8/docs/development.rst
--rw-r--r--   0 runner    (1001) docker     (121)      675 2022-07-10 17:09:36.000000 relaton-0.2.8/docs/get-started.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2676 2022-07-10 17:09:36.000000 relaton-0.2.8/docs/glossary.rst
--rw-r--r--   0 runner    (1001) docker     (121)      367 2022-07-10 17:09:36.000000 relaton-0.2.8/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 17:09:46.755624 relaton-0.2.8/docs/ref/
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-07-10 17:09:36.000000 relaton-0.2.8/docs/ref/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1331 2022-07-10 17:09:36.000000 relaton-0.2.8/docs/ref/models.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1455 2022-07-10 17:09:36.000000 relaton-0.2.8/docs/ref/serializers.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 17:09:46.755624 relaton-0.2.8/relaton/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-07-10 17:09:36.000000 relaton-0.2.8/relaton/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 17:09:46.755624 relaton-0.2.8/relaton/models/
--rw-r--r--   0 runner    (1001) docker     (121)     1470 2022-07-10 17:09:36.000000 relaton-0.2.8/relaton/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5654 2022-07-10 17:09:36.000000 relaton-0.2.8/relaton/models/bibdata.py
--rw-r--r--   0 runner    (1001) docker     (121)      701 2022-07-10 17:09:36.000000 relaton-0.2.8/relaton/models/bibitemlocality.py
--rw-r--r--   0 runner    (1001) docker     (121)      694 2022-07-10 17:09:36.000000 relaton-0.2.8/relaton/models/contacts.py
--rw-r--r--   0 runner    (1001) docker     (121)      515 2022-07-10 17:09:36.000000 relaton-0.2.8/relaton/models/copyrights.py
--rw-r--r--   0 runner    (1001) docker     (121)     2946 2022-07-10 17:09:36.000000 relaton-0.2.8/relaton/models/dates.py
--rw-r--r--   0 runner    (1001) docker     (121)      222 2022-07-10 17:09:36.000000 relaton-0.2.8/relaton/models/links.py
--rw-r--r--   0 runner    (1001) docker     (121)      375 2022-07-10 17:09:36.000000 relaton-0.2.8/relaton/models/orgs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1403 2022-07-10 17:09:36.000000 relaton-0.2.8/relaton/models/people.py
--rw-r--r--   0 runner    (1001) docker     (121)      666 2022-07-10 17:09:36.000000 relaton-0.2.8/relaton/models/strings.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-10 17:09:36.000000 relaton-0.2.8/relaton/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 17:09:46.759624 relaton-0.2.8/relaton/serializers/
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-07-10 17:09:36.000000 relaton-0.2.8/relaton/serializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 17:09:46.759624 relaton-0.2.8/relaton/serializers/bibxml/
--rw-r--r--   0 runner    (1001) docker     (121)     2003 2022-07-10 17:09:36.000000 relaton-0.2.8/relaton/serializers/bibxml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2149 2022-07-10 17:09:36.000000 relaton-0.2.8/relaton/serializers/bibxml/abstracts.py
--rw-r--r--   0 runner    (1001) docker     (121)     1951 2022-07-10 17:09:36.000000 relaton-0.2.8/relaton/serializers/bibxml/anchor.py
--rw-r--r--   0 runner    (1001) docker     (121)     4194 2022-07-10 17:09:36.000000 relaton-0.2.8/relaton/serializers/bibxml/authors.py
--rw-r--r--   0 runner    (1001) docker     (121)     3809 2022-07-10 17:09:36.000000 relaton-0.2.8/relaton/serializers/bibxml/reference.py
--rw-r--r--   0 runner    (1001) docker     (121)     2088 2022-07-10 17:09:36.000000 relaton-0.2.8/relaton/serializers/bibxml/series.py
--rw-r--r--   0 runner    (1001) docker     (121)      680 2022-07-10 17:09:36.000000 relaton-0.2.8/relaton/serializers/bibxml/target.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 17:09:46.759624 relaton-0.2.8/relaton/serializers/bibxml_string/
--rw-r--r--   0 runner    (1001) docker     (121)      628 2022-07-10 17:09:36.000000 relaton-0.2.8/relaton/serializers/bibxml_string/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      302 2022-07-10 17:09:36.000000 relaton-0.2.8/relaton/serializers/types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 17:09:46.759624 relaton-0.2.8/relaton/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-10 17:09:36.000000 relaton-0.2.8/relaton/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    23619 2022-07-10 17:09:36.000000 relaton-0.2.8/relaton/tests/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (121)      574 2022-07-10 17:09:36.000000 relaton-0.2.8/relaton/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 17:09:46.755624 relaton-0.2.8/relaton.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1220 2022-07-10 17:09:46.000000 relaton-0.2.8/relaton.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-07-10 17:09:46.000000 relaton-0.2.8/relaton.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-10 17:09:46.000000 relaton-0.2.8/relaton.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-10 17:09:46.000000 relaton-0.2.8/relaton.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-07-10 17:09:46.000000 relaton-0.2.8/relaton.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-07-10 17:09:36.000000 relaton-0.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-07-10 17:09:36.000000 relaton-0.2.8/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-10 17:09:46.759624 relaton-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1868 2022-07-10 17:09:36.000000 relaton-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 00:17:00.307335 relaton-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-07-14 00:16:42.000000 relaton-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      161 2022-07-14 00:16:42.000000 relaton-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1220 2022-07-14 00:17:00.307335 relaton-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      321 2022-07-14 00:16:42.000000 relaton-0.2.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 00:17:00.299335 relaton-0.2.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)     3532 2022-07-14 00:16:42.000000 relaton-0.2.9/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3001 2022-07-14 00:16:42.000000 relaton-0.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1864 2022-07-14 00:16:42.000000 relaton-0.2.9/docs/development.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      675 2022-07-14 00:16:42.000000 relaton-0.2.9/docs/get-started.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2575 2022-07-14 00:16:42.000000 relaton-0.2.9/docs/glossary.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      367 2022-07-14 00:16:42.000000 relaton-0.2.9/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 00:17:00.303335 relaton-0.2.9/docs/ref/
+-rw-r--r--   0 runner    (1001) docker     (121)      107 2022-07-14 00:16:42.000000 relaton-0.2.9/docs/ref/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1331 2022-07-14 00:16:42.000000 relaton-0.2.9/docs/ref/models.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1455 2022-07-14 00:16:42.000000 relaton-0.2.9/docs/ref/serializers.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 00:17:00.303335 relaton-0.2.9/relaton/
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-07-14 00:16:42.000000 relaton-0.2.9/relaton/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 00:17:00.303335 relaton-0.2.9/relaton/models/
+-rw-r--r--   0 runner    (1001) docker     (121)     1470 2022-07-14 00:16:42.000000 relaton-0.2.9/relaton/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5654 2022-07-14 00:16:42.000000 relaton-0.2.9/relaton/models/bibdata.py
+-rw-r--r--   0 runner    (1001) docker     (121)      701 2022-07-14 00:16:42.000000 relaton-0.2.9/relaton/models/bibitemlocality.py
+-rw-r--r--   0 runner    (1001) docker     (121)      694 2022-07-14 00:16:42.000000 relaton-0.2.9/relaton/models/contacts.py
+-rw-r--r--   0 runner    (1001) docker     (121)      515 2022-07-14 00:16:42.000000 relaton-0.2.9/relaton/models/copyrights.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2946 2022-07-14 00:16:42.000000 relaton-0.2.9/relaton/models/dates.py
+-rw-r--r--   0 runner    (1001) docker     (121)      222 2022-07-14 00:16:42.000000 relaton-0.2.9/relaton/models/links.py
+-rw-r--r--   0 runner    (1001) docker     (121)      375 2022-07-14 00:16:42.000000 relaton-0.2.9/relaton/models/orgs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1403 2022-07-14 00:16:42.000000 relaton-0.2.9/relaton/models/people.py
+-rw-r--r--   0 runner    (1001) docker     (121)      666 2022-07-14 00:16:42.000000 relaton-0.2.9/relaton/models/strings.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 00:16:42.000000 relaton-0.2.9/relaton/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 00:17:00.303335 relaton-0.2.9/relaton/serializers/
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2022-07-14 00:16:42.000000 relaton-0.2.9/relaton/serializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 00:17:00.307335 relaton-0.2.9/relaton/serializers/bibxml/
+-rw-r--r--   0 runner    (1001) docker     (121)     2003 2022-07-14 00:16:42.000000 relaton-0.2.9/relaton/serializers/bibxml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2149 2022-07-14 00:16:42.000000 relaton-0.2.9/relaton/serializers/bibxml/abstracts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1951 2022-07-14 00:16:42.000000 relaton-0.2.9/relaton/serializers/bibxml/anchor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4194 2022-07-14 00:16:42.000000 relaton-0.2.9/relaton/serializers/bibxml/authors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3809 2022-07-14 00:16:42.000000 relaton-0.2.9/relaton/serializers/bibxml/reference.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2088 2022-07-14 00:16:42.000000 relaton-0.2.9/relaton/serializers/bibxml/series.py
+-rw-r--r--   0 runner    (1001) docker     (121)      680 2022-07-14 00:16:42.000000 relaton-0.2.9/relaton/serializers/bibxml/target.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 00:17:00.307335 relaton-0.2.9/relaton/serializers/bibxml_string/
+-rw-r--r--   0 runner    (1001) docker     (121)      628 2022-07-14 00:16:42.000000 relaton-0.2.9/relaton/serializers/bibxml_string/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      302 2022-07-14 00:16:42.000000 relaton-0.2.9/relaton/serializers/types.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 00:17:00.307335 relaton-0.2.9/relaton/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 00:16:42.000000 relaton-0.2.9/relaton/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23619 2022-07-14 00:16:42.000000 relaton-0.2.9/relaton/tests/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      574 2022-07-14 00:16:42.000000 relaton-0.2.9/relaton/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 00:17:00.303335 relaton-0.2.9/relaton.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1220 2022-07-14 00:17:00.000000 relaton-0.2.9/relaton.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-07-14 00:17:00.000000 relaton-0.2.9/relaton.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-14 00:17:00.000000 relaton-0.2.9/relaton.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-14 00:17:00.000000 relaton-0.2.9/relaton.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-07-14 00:17:00.000000 relaton-0.2.9/relaton.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-07-14 00:16:42.000000 relaton-0.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-07-14 00:16:42.000000 relaton-0.2.9/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-14 00:17:00.307335 relaton-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1868 2022-07-14 00:16:42.000000 relaton-0.2.9/setup.py
```

### Comparing `relaton-0.2.8/LICENSE` & `relaton-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `relaton-0.2.8/PKG-INFO` & `relaton-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relaton
-Version: 0.2.8
+Version: 0.2.9
 Summary: Library for working with Relaton bibliographic data models in Python. Provides Pydantic models and dataclasses, as well as parsers and serializers.
 Home-page: http://github.com/relaton/relaton-py/
 Author: Ribose Inc.
 Author-email: open@ribose.com
 License: BSD 2-clause
 Keywords: Relaton,bibliographic data,bibliography,Pydantic,dataclasses
 Platform: UNKNOWN
```

### Comparing `relaton-0.2.8/docs/changelog.rst` & `relaton-0.2.9/docs/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =========
 Changelog
 =========
 
+v0.2.9
+======
+
+Adds ``BibitemLocality`` support.
+
 v0.2.8
 ======
 
 ``bibxml`` serializer:
 
 - Ensures returned ``anchor`` attribute satisfies XML schema
   (by replacing or dropping non-conforming characters).
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-========= Changelog ========= v0.2.8 ====== ``bibxml`` serializer: - Ensures
-returned ``anchor`` attribute satisfies XML schema (by replacing or dropping
-non-conforming characters). - No longer formats Internet Draft anchors in a
-special way. v0.2.7 ====== The ``bibxml_string`` serializer now complies with
-own documentation and pretty-prints the resulting XML string. v0.2.6 ====== The
-``bibxml`` serializer will now prioritize PDF links for ```` attribute value.
-v0.2.5 ====== The ``bibxml`` serializer: - Fixed an issue where ```` would be
-output instead of ````. - Missing bibliographic item title no longer causes
-serializer to fail. However, it has to supply a default title, since the
-xml2rfc spec requires ``
+========= Changelog ========= v0.2.9 ====== Adds ``BibitemLocality`` support.
+v0.2.8 ====== ``bibxml`` serializer: - Ensures returned ``anchor`` attribute
+satisfies XML schema (by replacing or dropping non-conforming characters). - No
+longer formats Internet Draft anchors in a special way. v0.2.7 ====== The
+``bibxml_string`` serializer now complies with own documentation and pretty-
+prints the resulting XML string. v0.2.6 ====== The ``bibxml`` serializer will
+now prioritize PDF links for ```` attribute value. v0.2.5 ====== The ``bibxml``
+serializer: - Fixed an issue where ```` would be output instead of ````. -
+Missing bibliographic item title no longer causes serializer to fail. However,
+it has to supply a default title, since the xml2rfc spec requires ``
 `` as root element, rely on presence of âincludesâ-type relations alone,
 rather than also require absence of titles. - Fix an issue with serializing
 Internet Drafts to XML v0.1.16 ======= - Allow multiple
 ``BibliographicItem.version`` entries v0.1.15 ======= - Make
 ``BibliographicItem.docid`` a list (and required property) v0.1.14 ======= -
 Corrected a problem with abstract conversion (``bibxml`` serializer) v0.1.11
 ======= - Fixed CodeCov badge syntax in README/PyPI description. v0.1.10
```

### Comparing `relaton-0.2.8/docs/conf.py` & `relaton-0.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `relaton-0.2.8/docs/development.rst` & `relaton-0.2.9/docs/development.rst`

 * *Files identical despite different names*

### Comparing `relaton-0.2.8/docs/get-started.rst` & `relaton-0.2.9/docs/get-started.rst`

 * *Files identical despite different names*

### Comparing `relaton-0.2.8/docs/glossary.rst` & `relaton-0.2.9/docs/glossary.rst`

 * *Files 10% similar despite different names*

```diff
@@ -26,23 +26,20 @@
        under :data:`BibliographicItem.docid <relaton.models.bibdata.BibliographicItem.docid>`,
        and each identifier is a :class:`relaton.models.bibdata.DocID` instance in Python.
 
    primary resource identifier
    primary document identifier
        Main characteristics of a primary identifier:
 
-       - Its ``id`` can be used to unambiguously reference the document (resource).
+       - Identifier value (in Python, the :data:`~relaton.models.bibdata.DocID.id` attribute)
+         can be used to unambiguously reference the document (resource).
        - A primary identifier is expected to be
          universally unique to this resource.
 
-       This service displays primary identifiers without identifier types,
-       as types tend to be self-explanatory.
-
-       The :data:`~relaton.models.bibdata.DocID.id` value of a primary identifier
-       uses format more or less similar to NIST’s PubID
+       Primary identifier uses format more or less similar to NIST’s PubID
        (possibly the only strongly standardized identifier format).
        It always starts with a prefix that denotes schema/document family.
 
        In Python, such identifiers have their :data:`~relaton.models.bibdata.DocID.primary`
        attribute set to ``True``.
 
    resource identifier type
```

### Comparing `relaton-0.2.8/docs/ref/models.rst` & `relaton-0.2.9/docs/ref/models.rst`

 * *Files identical despite different names*

### Comparing `relaton-0.2.8/docs/ref/serializers.rst` & `relaton-0.2.9/docs/ref/serializers.rst`

 * *Files identical despite different names*

### Comparing `relaton-0.2.8/relaton/models/__init__.py` & `relaton-0.2.9/relaton/models/__init__.py`

 * *Files identical despite different names*

### Comparing `relaton-0.2.8/relaton/models/bibdata.py` & `relaton-0.2.9/relaton/models/bibdata.py`

 * *Files identical despite different names*

### Comparing `relaton-0.2.8/relaton/models/bibitemlocality.py` & `relaton-0.2.9/relaton/models/bibitemlocality.py`

 * *Files identical despite different names*

### Comparing `relaton-0.2.8/relaton/models/contacts.py` & `relaton-0.2.9/relaton/models/contacts.py`

 * *Files identical despite different names*

### Comparing `relaton-0.2.8/relaton/models/copyrights.py` & `relaton-0.2.9/relaton/models/copyrights.py`

 * *Files identical despite different names*

### Comparing `relaton-0.2.8/relaton/models/dates.py` & `relaton-0.2.9/relaton/models/dates.py`

 * *Files identical despite different names*

### Comparing `relaton-0.2.8/relaton/models/people.py` & `relaton-0.2.9/relaton/models/people.py`

 * *Files identical despite different names*

### Comparing `relaton-0.2.8/relaton/models/strings.py` & `relaton-0.2.9/relaton/models/strings.py`

 * *Files identical despite different names*

### Comparing `relaton-0.2.8/relaton/serializers/bibxml/__init__.py` & `relaton-0.2.9/relaton/serializers/bibxml/__init__.py`

 * *Files identical despite different names*

### Comparing `relaton-0.2.8/relaton/serializers/bibxml/abstracts.py` & `relaton-0.2.9/relaton/serializers/bibxml/abstracts.py`

 * *Files identical despite different names*

### Comparing `relaton-0.2.8/relaton/serializers/bibxml/anchor.py` & `relaton-0.2.9/relaton/serializers/bibxml/anchor.py`

 * *Files identical despite different names*

### Comparing `relaton-0.2.8/relaton/serializers/bibxml/authors.py` & `relaton-0.2.9/relaton/serializers/bibxml/authors.py`

 * *Files identical despite different names*

### Comparing `relaton-0.2.8/relaton/serializers/bibxml/reference.py` & `relaton-0.2.9/relaton/serializers/bibxml/reference.py`

 * *Files identical despite different names*

### Comparing `relaton-0.2.8/relaton/serializers/bibxml/series.py` & `relaton-0.2.9/relaton/serializers/bibxml/series.py`

 * *Files identical despite different names*

### Comparing `relaton-0.2.8/relaton/serializers/bibxml/target.py` & `relaton-0.2.9/relaton/serializers/bibxml/target.py`

 * *Files identical despite different names*

### Comparing `relaton-0.2.8/relaton/serializers/bibxml_string/__init__.py` & `relaton-0.2.9/relaton/serializers/bibxml_string/__init__.py`

 * *Files identical despite different names*

### Comparing `relaton-0.2.8/relaton/tests/test_serializers.py` & `relaton-0.2.9/relaton/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `relaton-0.2.8/relaton/util.py` & `relaton-0.2.9/relaton/util.py`

 * *Files identical despite different names*

### Comparing `relaton-0.2.8/relaton.egg-info/PKG-INFO` & `relaton-0.2.9/relaton.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relaton
-Version: 0.2.8
+Version: 0.2.9
 Summary: Library for working with Relaton bibliographic data models in Python. Provides Pydantic models and dataclasses, as well as parsers and serializers.
 Home-page: http://github.com/relaton/relaton-py/
 Author: Ribose Inc.
 Author-email: open@ribose.com
 License: BSD 2-clause
 Keywords: Relaton,bibliographic data,bibliography,Pydantic,dataclasses
 Platform: UNKNOWN
```

### Comparing `relaton-0.2.8/relaton.egg-info/SOURCES.txt` & `relaton-0.2.9/relaton.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `relaton-0.2.8/setup.py` & `relaton-0.2.9/setup.py`

 * *Files identical despite different names*

