# Comparing `tmp/owl2yams-1.2.1.tar.gz` & `tmp/owl2yams-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owl2yams-1.2.1.tar", last modified: Thu Nov 17 16:08:31 2022, max compression
+gzip compressed data, was "dist/owl2yams-1.3.0.tar", last modified: Mon Apr 24 12:25:14 2023, max compression
```

## Comparing `owl2yams-1.2.1.tar` & `owl2yams-1.3.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-17 16:08:31.667056 owl2yams-1.2.1/
--rw-rw-rw-   0 root         (0) root         (0)      267 2022-11-17 16:08:18.000000 owl2yams-1.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2876 2022-11-17 16:08:31.667056 owl2yams-1.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2577 2022-11-17 16:08:18.000000 owl2yams-1.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-17 16:08:31.659056 owl2yams-1.2.1/owl2yams/
--rw-rw-rw-   0 root         (0) root         (0)    17378 2022-11-17 16:08:18.000000 owl2yams-1.2.1/owl2yams/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5346 2022-11-17 16:08:18.000000 owl2yams-1.2.1/owl2yams/ccplugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-17 16:08:31.659056 owl2yams-1.2.1/owl2yams/cw_react_admin/
--rw-rw-rw-   0 root         (0) root         (0)  1474880 2022-11-17 16:08:18.000000 owl2yams-1.2.1/owl2yams/cw_react_admin/main.js
--rw-rw-rw-   0 root         (0) root         (0)      480 2022-11-17 16:08:18.000000 owl2yams-1.2.1/owl2yams/generate_appjstemplate.py
--rw-rw-rw-   0 root         (0) root         (0)     4213 2022-11-17 16:08:18.000000 owl2yams-1.2.1/owl2yams/generate_entities.py
--rw-rw-rw-   0 root         (0) root         (0)      267 2022-11-17 16:08:18.000000 owl2yams-1.2.1/owl2yams/generate_init.py
--rw-rw-rw-   0 root         (0) root         (0)     1053 2022-11-17 16:08:18.000000 owl2yams-1.2.1/owl2yams/generate_postcreate.py
--rw-rw-rw-   0 root         (0) root         (0)     1069 2022-11-17 16:08:18.000000 owl2yams-1.2.1/owl2yams/generate_schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1550 2022-11-17 16:08:18.000000 owl2yams-1.2.1/owl2yams/generate_views.py
--rw-rw-rw-   0 root         (0) root         (0)   136241 2022-11-17 16:08:18.000000 owl2yams-1.2.1/owl2yams/prefixes.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-17 16:08:31.659056 owl2yams-1.2.1/owl2yams.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2876 2022-11-17 16:08:31.000000 owl2yams-1.2.1/owl2yams.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1240 2022-11-17 16:08:31.000000 owl2yams-1.2.1/owl2yams.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-17 16:08:31.000000 owl2yams-1.2.1/owl2yams.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2022-11-17 16:08:31.000000 owl2yams-1.2.1/owl2yams.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-17 16:08:31.000000 owl2yams-1.2.1/owl2yams.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       60 2022-11-17 16:08:31.000000 owl2yams-1.2.1/owl2yams.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2022-11-17 16:08:31.000000 owl2yams-1.2.1/owl2yams.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-17 16:08:31.667056 owl2yams-1.2.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1287 2022-11-17 16:08:18.000000 owl2yams-1.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-17 16:08:31.663056 owl2yams-1.2.1/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-17 16:08:31.667056 owl2yams-1.2.1/test/data/
--rw-rw-rw-   0 root         (0) root         (0)      293 2022-11-17 16:08:18.000000 owl2yams-1.2.1/test/data/test_attribute.owl
--rw-rw-rw-   0 root         (0) root         (0)       96 2022-11-17 16:08:18.000000 owl2yams-1.2.1/test/data/test_attribute.yams
--rw-rw-rw-   0 root         (0) root         (0)      293 2022-11-17 16:08:18.000000 owl2yams-1.2.1/test/data/test_attribute_owl_thing.owl
--rw-rw-rw-   0 root         (0) root         (0)      169 2022-11-17 16:08:18.000000 owl2yams-1.2.1/test/data/test_attribute_owl_thing.yams
--rw-rw-rw-   0 root         (0) root         (0)      104 2022-11-17 16:08:18.000000 owl2yams-1.2.1/test/data/test_class.owl
--rw-rw-rw-   0 root         (0) root         (0)       78 2022-11-17 16:08:18.000000 owl2yams-1.2.1/test/data/test_class.yams
--rw-rw-rw-   0 root         (0) root         (0)      216 2022-11-17 16:08:18.000000 owl2yams-1.2.1/test/data/test_hierarchy.owl
--rw-rw-rw-   0 root         (0) root         (0)      132 2022-11-17 16:08:18.000000 owl2yams-1.2.1/test/data/test_hierarchy.yams
--rw-rw-rw-   0 root         (0) root         (0)      197 2022-11-17 16:08:18.000000 owl2yams-1.2.1/test/data/test_multi_attribute.owl
--rw-rw-rw-   0 root         (0) root         (0)       30 2022-11-17 16:08:18.000000 owl2yams-1.2.1/test/data/test_multi_attribute.yams
--rw-rw-rw-   0 root         (0) root         (0)      179 2022-11-17 16:08:18.000000 owl2yams-1.2.1/test/data/test_multi_class.owl
--rw-rw-rw-   0 root         (0) root         (0)      119 2022-11-17 16:08:18.000000 owl2yams-1.2.1/test/data/test_multi_class.yams
--rw-rw-rw-   0 root         (0) root         (0)      193 2022-11-17 16:08:18.000000 owl2yams-1.2.1/test/data/test_multi_relation.owl
--rw-rw-rw-   0 root         (0) root         (0)       30 2022-11-17 16:08:18.000000 owl2yams-1.2.1/test/data/test_multi_relation.yams
--rw-rw-rw-   0 root         (0) root         (0)      295 2022-11-17 16:08:18.000000 owl2yams-1.2.1/test/data/test_relation.owl
--rw-rw-rw-   0 root         (0) root         (0)      196 2022-11-17 16:08:18.000000 owl2yams-1.2.1/test/data/test_relation.yams
--rw-rw-rw-   0 root         (0) root         (0)      306 2022-11-17 16:08:18.000000 owl2yams-1.2.1/test/data/test_relation_multi_range.owl
--rw-rw-rw-   0 root         (0) root         (0)      291 2022-11-17 16:08:18.000000 owl2yams-1.2.1/test/data/test_relation_multi_range.yams
--rw-rw-rw-   0 root         (0) root         (0)      264 2022-11-17 16:08:18.000000 owl2yams-1.2.1/test/data/test_relation_without_domain_range.owl
--rw-rw-rw-   0 root         (0) root         (0)      291 2022-11-17 16:08:18.000000 owl2yams-1.2.1/test/data/test_relation_without_domain_range.yams
--rw-rw-rw-   0 root         (0) root         (0)     4025 2022-11-17 16:08:18.000000 owl2yams-1.2.1/test/test_owl2yams.py
+drwxr-xr-x   0 murloc    (1000) murloc    (1000)        0 2023-04-24 12:25:14.000000 owl2yams-1.3.0/
+-rw-r--r--   0 murloc    (1000) murloc    (1000)      267 2022-11-17 15:54:54.000000 owl2yams-1.3.0/MANIFEST.in
+-rw-r--r--   0 murloc    (1000) murloc    (1000)     2876 2023-04-24 12:25:14.000000 owl2yams-1.3.0/PKG-INFO
+-rw-r--r--   0 murloc    (1000) murloc    (1000)     2577 2022-07-04 12:53:24.000000 owl2yams-1.3.0/README.md
+drwxr-xr-x   0 murloc    (1000) murloc    (1000)        0 2023-04-24 12:25:14.000000 owl2yams-1.3.0/owl2yams/
+-rw-r--r--   0 murloc    (1000) murloc    (1000)    18404 2023-04-24 12:20:23.000000 owl2yams-1.3.0/owl2yams/__init__.py
+-rw-r--r--   0 murloc    (1000) murloc    (1000)     5342 2023-04-24 12:17:06.000000 owl2yams-1.3.0/owl2yams/ccplugin.py
+drwxr-xr-x   0 murloc    (1000) murloc    (1000)        0 2023-04-24 12:25:14.000000 owl2yams-1.3.0/owl2yams/cw_react_admin/
+-rw-r--r--   0 murloc    (1000) murloc    (1000)  1474880 2022-11-17 14:01:32.000000 owl2yams-1.3.0/owl2yams/cw_react_admin/main.js
+-rw-r--r--   0 murloc    (1000) murloc    (1000)      480 2022-11-17 14:40:11.000000 owl2yams-1.3.0/owl2yams/generate_appjstemplate.py
+-rw-r--r--   0 murloc    (1000) murloc    (1000)     4213 2021-11-26 14:03:57.000000 owl2yams-1.3.0/owl2yams/generate_entities.py
+-rw-r--r--   0 murloc    (1000) murloc    (1000)      267 2022-11-17 13:50:43.000000 owl2yams-1.3.0/owl2yams/generate_init.py
+-rw-r--r--   0 murloc    (1000) murloc    (1000)     1052 2023-04-24 12:17:06.000000 owl2yams-1.3.0/owl2yams/generate_postcreate.py
+-rw-r--r--   0 murloc    (1000) murloc    (1000)     1069 2022-11-17 15:11:21.000000 owl2yams-1.3.0/owl2yams/generate_schema.py
+-rw-r--r--   0 murloc    (1000) murloc    (1000)     1550 2022-11-17 14:06:49.000000 owl2yams-1.3.0/owl2yams/generate_views.py
+-rw-r--r--   0 murloc    (1000) murloc    (1000)   136241 2021-11-25 15:02:23.000000 owl2yams-1.3.0/owl2yams/prefixes.json
+drwxr-xr-x   0 murloc    (1000) murloc    (1000)        0 2023-04-24 12:25:14.000000 owl2yams-1.3.0/owl2yams.egg-info/
+-rw-r--r--   0 murloc    (1000) murloc    (1000)     2876 2023-04-24 12:25:14.000000 owl2yams-1.3.0/owl2yams.egg-info/PKG-INFO
+-rw-r--r--   0 murloc    (1000) murloc    (1000)     1240 2023-04-24 12:25:14.000000 owl2yams-1.3.0/owl2yams.egg-info/SOURCES.txt
+-rw-r--r--   0 murloc    (1000) murloc    (1000)        1 2023-04-24 12:25:14.000000 owl2yams-1.3.0/owl2yams.egg-info/dependency_links.txt
+-rw-r--r--   0 murloc    (1000) murloc    (1000)       44 2023-04-24 12:25:14.000000 owl2yams-1.3.0/owl2yams.egg-info/entry_points.txt
+-rw-r--r--   0 murloc    (1000) murloc    (1000)        1 2021-10-12 13:30:58.000000 owl2yams-1.3.0/owl2yams.egg-info/not-zip-safe
+-rw-r--r--   0 murloc    (1000) murloc    (1000)       60 2023-04-24 12:25:14.000000 owl2yams-1.3.0/owl2yams.egg-info/requires.txt
+-rw-r--r--   0 murloc    (1000) murloc    (1000)        9 2023-04-24 12:25:14.000000 owl2yams-1.3.0/owl2yams.egg-info/top_level.txt
+-rw-r--r--   0 murloc    (1000) murloc    (1000)       38 2023-04-24 12:25:14.000000 owl2yams-1.3.0/setup.cfg
+-rw-r--r--   0 murloc    (1000) murloc    (1000)     1287 2023-04-24 12:22:32.000000 owl2yams-1.3.0/setup.py
+drwxr-xr-x   0 murloc    (1000) murloc    (1000)        0 2023-04-24 12:25:14.000000 owl2yams-1.3.0/test/
+drwxr-xr-x   0 murloc    (1000) murloc    (1000)        0 2023-04-24 12:25:14.000000 owl2yams-1.3.0/test/data/
+-rw-r--r--   0 murloc    (1000) murloc    (1000)      293 2021-10-26 13:13:22.000000 owl2yams-1.3.0/test/data/test_attribute.owl
+-rw-r--r--   0 murloc    (1000) murloc    (1000)       96 2021-11-24 14:17:42.000000 owl2yams-1.3.0/test/data/test_attribute.yams
+-rw-r--r--   0 murloc    (1000) murloc    (1000)      293 2021-10-26 15:46:23.000000 owl2yams-1.3.0/test/data/test_attribute_owl_thing.owl
+-rw-r--r--   0 murloc    (1000) murloc    (1000)      169 2021-11-24 14:17:42.000000 owl2yams-1.3.0/test/data/test_attribute_owl_thing.yams
+-rw-r--r--   0 murloc    (1000) murloc    (1000)      104 2021-10-26 12:52:43.000000 owl2yams-1.3.0/test/data/test_class.owl
+-rw-r--r--   0 murloc    (1000) murloc    (1000)       78 2021-11-24 14:17:42.000000 owl2yams-1.3.0/test/data/test_class.yams
+-rw-r--r--   0 murloc    (1000) murloc    (1000)      216 2021-10-26 13:24:20.000000 owl2yams-1.3.0/test/data/test_hierarchy.owl
+-rw-r--r--   0 murloc    (1000) murloc    (1000)      132 2021-11-24 14:17:42.000000 owl2yams-1.3.0/test/data/test_hierarchy.yams
+-rw-r--r--   0 murloc    (1000) murloc    (1000)      197 2021-10-26 14:02:16.000000 owl2yams-1.3.0/test/data/test_multi_attribute.owl
+-rw-r--r--   0 murloc    (1000) murloc    (1000)       30 2021-11-24 14:30:28.000000 owl2yams-1.3.0/test/data/test_multi_attribute.yams
+-rw-r--r--   0 murloc    (1000) murloc    (1000)      179 2021-10-26 13:41:53.000000 owl2yams-1.3.0/test/data/test_multi_class.owl
+-rw-r--r--   0 murloc    (1000) murloc    (1000)      119 2021-11-24 14:32:57.000000 owl2yams-1.3.0/test/data/test_multi_class.yams
+-rw-r--r--   0 murloc    (1000) murloc    (1000)      193 2021-10-26 14:14:35.000000 owl2yams-1.3.0/test/data/test_multi_relation.owl
+-rw-r--r--   0 murloc    (1000) murloc    (1000)       30 2021-11-24 14:34:53.000000 owl2yams-1.3.0/test/data/test_multi_relation.yams
+-rw-r--r--   0 murloc    (1000) murloc    (1000)      295 2021-10-26 13:15:12.000000 owl2yams-1.3.0/test/data/test_relation.owl
+-rw-r--r--   0 murloc    (1000) murloc    (1000)      196 2021-11-24 14:17:42.000000 owl2yams-1.3.0/test/data/test_relation.yams
+-rw-r--r--   0 murloc    (1000) murloc    (1000)      306 2021-10-26 15:51:01.000000 owl2yams-1.3.0/test/data/test_relation_multi_range.owl
+-rw-r--r--   0 murloc    (1000) murloc    (1000)      291 2021-11-24 14:17:42.000000 owl2yams-1.3.0/test/data/test_relation_multi_range.yams
+-rw-r--r--   0 murloc    (1000) murloc    (1000)      264 2021-10-26 15:43:32.000000 owl2yams-1.3.0/test/data/test_relation_without_domain_range.owl
+-rw-r--r--   0 murloc    (1000) murloc    (1000)      291 2021-11-24 14:17:42.000000 owl2yams-1.3.0/test/data/test_relation_without_domain_range.yams
+-rw-r--r--   0 murloc    (1000) murloc    (1000)     4025 2021-11-24 14:33:52.000000 owl2yams-1.3.0/test/test_owl2yams.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `owl2yams-1.2.1/PKG-INFO` & `owl2yams-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owl2yams
-Version: 1.2.1
+Version: 1.3.0
 Summary: A tools to transforms owl into yams schema
 Home-page: https://forge.extranet.logilab.fr/cubicweb/owl2yams
 Author: Fabien Amarger
 Author-email: famarger@logilab.fr
 License: LGPL
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `owl2yams-1.2.1/README.md` & `owl2yams-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `owl2yams-1.2.1/owl2yams/__init__.py` & `owl2yams-1.3.0/owl2yams/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,33 @@
-import subprocess
-import re
-import os
+import itertools
 import json
-import unicodedata
-from pathlib import Path
+import os
+import re
 import shutil
-from typing import Iterable, Optional, List, Dict, Tuple
-
-from redbaron import RedBaron
+import subprocess
+import unicodedata
 from argparse import ArgumentParser
-import itertools
-from rdflib import Graph, RDF, RDFS, OWL, XSD, URIRef  # type: ignore
+from pathlib import Path
+from typing import Dict, Iterable, List, Optional, Tuple
 from urllib.parse import urlparse
+
+from rdflib import OWL, RDF, RDFS, XSD, Graph, URIRef  # type: ignore
 from rdflib.term import BNode
+from redbaron import RedBaron
+from yams.buildobjs import RelationDefinition  # type: ignore
+from yams.buildobjs import EntityType, RelationType, register_base_types
 from yams.schema import Schema  # type: ignore
 from yams.serialize import serialize_to_python  # type: ignore
-from yams.buildobjs import (  # type: ignore
-    EntityType,
-    RelationDefinition,
-    RelationType,
-    register_base_types,
-)
 
-from owl2yams.generate_postcreate import generate_postcreate
+from owl2yams.generate_appjstemplate import generate_appjstemplate
 from owl2yams.generate_entities import generate_entities
+from owl2yams.generate_init import generate_init
+from owl2yams.generate_postcreate import generate_postcreate
 from owl2yams.generate_schema import generate_schema
 from owl2yams.generate_views import generate_views
-from owl2yams.generate_init import generate_init
-from owl2yams.generate_appjstemplate import generate_appjstemplate
 
 here = os.path.dirname(__file__)
 
 LITERAL_TYPES_TO_YAMS_TYPES = {
     RDFS.Literal: "String",
     XSD.string: "String",
     XSD.int: "Int",
@@ -47,15 +43,15 @@
 
 def strip_accents(s):
     return "".join(
         c for c in unicodedata.normalize("NFD", s) if unicodedata.category(c) != "Mn"
     )
 
 
-def fragment_from_uri(uri: str, titling=False) -> Optional[str]:
+def fragment_from_uri(uri: str, titling=False, no_prefix=False) -> Optional[str]:
     if uri == OWL.Thing or uri == RDFS.Class:
         return None
     url = urlparse(uri)
     # if url.fragment is not None, the fragment is done with `#`
     if url.fragment:
         fragment = url.fragment
     else:
@@ -69,30 +65,41 @@
     elif url.hostname is not None:
         prefix = url.hostname.replace("www.", "").replace(".", "_") + "_"
     if titling:
         prefix = prefix.title().replace("_", "")
     else:
         fragment = fragment.lower()
     fragment = strip_accents(fragment.replace("_", "").replace("-", ""))
-    return f"{prefix}{fragment}"
+    if no_prefix:
+        return fragment
+    else:
+        return f"{prefix}{fragment}"
 
 
 def property_range_domain_uris(owl_model, property_uri, domain=True):
     domain_range_property = "rdfs:domain"
     if not domain:
         domain_range_property = "rdfs:range"
 
     query_domains = f"""
     PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
     PREFIX owl: <http://www.w3.org/2002/07/owl#>
     SELECT DISTINCT ?uri WHERE {{
-        {{<{property_uri}> {domain_range_property} ?uri.}}
+        {{<{property_uri}> {domain_range_property} ?uri. FILTER(!isBlank(?uri))}}
         UNION
         {{<{property_uri}> {domain_range_property} ?z.
-        ?z owl:unionOf ?uri.}}
+            ?z owl:unionOf ?uri.
+            FILTER (isBlank(?z))
+            FILTER (!isBlank(?uri))
+        }}
+        UNION
+        {{<{property_uri}> {domain_range_property} ?z.
+            ?z owl:unionOf ?list.
+            ?list rdf:rest*/rdf:first ?uri.
+        }}
     }}
     """
 
     domain_uris = []
     # first, check if the property has its own domain defined
     for domain_res in owl_model.query(query_domains):
         domain_uri = domain_res.uri
@@ -124,32 +131,32 @@
             continue
         domain_uris.append(domain_uri)
 
     return domain_uris
 
 
 def yams_domain_from_urirefs(
-    uris: Iterable[URIRef], all_entity_types: Iterable[str]
+    uris: Iterable[URIRef], all_entity_types: Iterable[str], no_prefix=False
 ) -> List[str]:
     fragments: List[str] = []
     for uri in uris:
         if isinstance(uri, BNode):
             continue
-        fragment = fragment_from_uri(uri, titling=True)
+        fragment = fragment_from_uri(uri, titling=True, no_prefix=no_prefix)
         if fragment is not None:
             fragments.append(fragment)
         else:
             return list(all_entity_types)
     if not len(fragments):
         return list(all_entity_types)
     return fragments
 
 
 def owl_model_to_yams(
-    owl_model: Graph, instance_name: str
+    owl_model: Graph, instance_name: str, no_prefix=False
 ) -> Tuple[Schema, Dict[str, str], Dict[str, str]]:
     entitytype_fragment_to_uri: Dict[str, str] = {}
     relationtype_fragment_to_uri: Dict[str, str] = {}
     # 0. Create a new YAMS Schema
     schema = Schema(instance_name)
     register_base_types(schema)
 
@@ -168,15 +175,15 @@
     """
 
     # 1. fetch all classes
     for class_res in owl_model.query(class_query):
         class_uri = class_res.uri
         if isinstance(class_uri, BNode) or class_uri.startswith(XSD):
             continue
-        class_fragment = fragment_from_uri(class_uri, titling=True)
+        class_fragment = fragment_from_uri(class_uri, titling=True, no_prefix=no_prefix)
         if class_fragment is None:
             print(f"Warning: class {class_uri} could not be parsed")
             continue
         if class_fragment in schema:
             raise ValueError(
                 f"Error: class {class_uri} and"
                 f" {entitytype_fragment_to_uri[class_fragment]} use the same fragment"
@@ -184,15 +191,15 @@
         entity_schema = schema.add_entity_type(EntityType(class_fragment))
         entitytype_fragment_to_uri[class_fragment] = class_uri
         superior_classes = []
         for _, _, superior_class_uri in owl_model.triples(
             (class_uri, RDFS.subClassOf, None)
         ):
             superior_class_fragment = fragment_from_uri(
-                superior_class_uri, titling=True
+                superior_class_uri, titling=True, no_prefix=no_prefix
             )
             if superior_class_fragment is not None:
                 superior_classes.append(superior_class_fragment)
         if superior_classes:
             entity_schema._specialized_type = ", ".join(superior_classes)
 
     # 2. fetch all datatype properties
@@ -206,37 +213,45 @@
             UNION {?uri a owl:AnnotationProperty.}
             UNION {?uri rdfs:range ?z.
             FILTER (?z in (xsd:int, rdfs:Literal, xsd:date, xsd:float, xsd:integer))}
         }
     """
     for datatype_property_res in owl_model.query(datatype_property_query):
         datatype_property_uri = datatype_property_res.uri
-        datatype_property_uri_fragment = fragment_from_uri(datatype_property_uri)
+        datatype_property_uri_fragment = fragment_from_uri(
+            datatype_property_uri, no_prefix=no_prefix
+        )
         if datatype_property_uri_fragment is None:
             print(f"Warning: data property {datatype_property_uri} could not be parsed")
             continue
         if datatype_property_uri_fragment in schema:
             datatype_property_uri_fragment = datatype_property_uri_fragment + "_bis"
         schema.add_relation_type(RelationType(datatype_property_uri_fragment))
         relationtype_fragment_to_uri[
             datatype_property_uri_fragment
         ] = datatype_property_uri
         # take first range, if no range use RDFS.Literal
         _, _, literal_type = next(
             owl_model.triples((datatype_property_uri, RDFS.range, None)),
             (None, None, RDFS.Literal),
         )
-        yams_type = LITERAL_TYPES_TO_YAMS_TYPES[literal_type]
+        try:
+            yams_type = LITERAL_TYPES_TO_YAMS_TYPES[literal_type]
+        except Exception:
+            print(
+                f"replace {datatype_property_uri} range with String (cause BlankNode)"
+            )
+            yams_type = "String"
 
         domain_fragments = yams_domain_from_urirefs(
             property_range_domain_uris(owl_model, datatype_property_uri, domain=True),
             entitytype_fragment_to_uri.keys(),
+            no_prefix=no_prefix,
         )
         for domain_fragment in domain_fragments:
-
             # if the parent of the domain is already in domain_fragments
             domain_parents_str = schema[domain_fragment]._specialized_type or ""
             domain_parents = domain_parents_str.split(", ")
             if set(domain_parents).intersection(set(domain_fragments)):
                 continue
             schema.add_relation_def(
                 RelationDefinition(
@@ -247,32 +262,36 @@
     # 3. fetch all object properties
 
     for (
         object_property_uri,
         _,
         _,
     ) in owl_model.triples((None, RDF.type, OWL.ObjectProperty)):
-        object_property_uri_fragment = fragment_from_uri(object_property_uri)
+        object_property_uri_fragment = fragment_from_uri(
+            object_property_uri, no_prefix=no_prefix
+        )
         if object_property_uri_fragment is None:
             print(f"Warning: object property {object_property_uri} could not be parsed")
             continue
         if object_property_uri_fragment in schema:
             object_property_uri_fragment += "_bis"
         schema.add_relation_type(RelationType(object_property_uri_fragment))
         relationtype_fragment_to_uri[object_property_uri_fragment] = object_property_uri
         all_types = list(entitytype_fragment_to_uri.keys())
 
         domain_fragments = yams_domain_from_urirefs(
             property_range_domain_uris(owl_model, object_property_uri, domain=True),
             all_types,
+            no_prefix=no_prefix,
         )
 
         range_fragments = yams_domain_from_urirefs(
             property_range_domain_uris(owl_model, object_property_uri, domain=False),
             all_types,
+            no_prefix=no_prefix,
         )
 
         for domain_fragment, range_fragment in itertools.product(
             domain_fragments, range_fragments
         ):
             schema.add_relation_def(
                 RelationDefinition(
@@ -297,23 +316,24 @@
 def generate_cubicweb_cube(
     owl_file="owl2yams/model.owl",
     instance_name="owl_instance",
     parse_format="turtle",
     dry_run=False,
     only_cube=False,
     base_url="http://localhost:8080/",
+    no_prefix=False,
 ):
     owl_model = Graph()
     owl_model.parse(owl_file, format=parse_format)
 
     (
         schema,
         entitytype_fragment_to_uri,
         relationtype_fragment_to_uri,
-    ) = owl_model_to_yams(owl_model, instance_name)
+    ) = owl_model_to_yams(owl_model, instance_name, no_prefix=no_prefix)
 
     if dry_run:
         print(serialize_to_python(schema))
         return
 
     cube_name = instance_name.replace("_", "-")
     cube_master_folder = f"cubicweb-{cube_name}"
@@ -493,17 +513,23 @@
     )
     parser.add_argument(
         "--base-url",
         "-b",
         default="http://localhost:8080/",
         help="Set CW URI base-url",
     )
+    parser.add_argument(
+        "--no-prefix",
+        action="store_true",
+        help="Do not prefix YAMS object with domain name",
+    )
 
     args = parser.parse_args()
     generate_cubicweb_cube(
         args.owl_model,
         args.instance_name,
         args.parse_format,
         args.dry_run,
         args.only_cube,
         args.base_url,
+        args.no_prefix,
     )
```

### Comparing `owl2yams-1.2.1/owl2yams/ccplugin.py` & `owl2yams-1.3.0/owl2yams/ccplugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,20 +115,20 @@
                             temp_relations[instance_uri] = []
                         temp_relations[instance_uri].append(
                             (relation_type, object_value)
                         )
                 entity = cnx.create_entity(entity_type.name, **temp_attributes)
                 entity.cw_set(label=tuple(temp_labels))
 
-            for (instance_uri, relations) in temp_relations.items():
+            for instance_uri, relations in temp_relations.items():
                 try:
                     entity = self.get_entity_from_uri(cnx, instance_uri)
                 except (NoResultError, MultipleResultsError):
                     continue
-                for (relation, object_uri) in relations:
+                for relation, object_uri in relations:
                     try:
                         object_entity = self.get_entity_from_uri(cnx, object_uri)
                     except (NoResultError, MultipleResultsError):
                         continue
                     set_relations = {}
                     set_relations[relation.name] = object_entity.eid
                     entity.cw_set(**set_relations)
```

### Comparing `owl2yams-1.2.1/owl2yams/cw_react_admin/main.js` & `owl2yams-1.3.0/owl2yams/cw_react_admin/main.js`

 * *Files identical despite different names*

### Comparing `owl2yams-1.2.1/owl2yams/generate_entities.py` & `owl2yams-1.3.0/owl2yams/generate_entities.py`

 * *Files identical despite different names*

### Comparing `owl2yams-1.2.1/owl2yams/generate_postcreate.py` & `owl2yams-1.3.0/owl2yams/generate_postcreate.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 """
 )
 
 
 def generate_postcreate(
     entitytype_to_uri: Dict[str, str], relationtype_to_uri: Dict[str, str]
 ) -> str:
-
     mapping = []
     for yams_class_name, uri_with_namespace in entitytype_to_uri.items():
         mapping.append((yams_class_name, str(uri_with_namespace), "CWEType"))
     for yams_relation_name, uri_with_namespace in relationtype_to_uri.items():
         mapping.append((yams_relation_name, str(uri_with_namespace), "CWRType"))
 
     rendered = postcreate_template.render(mapping=mapping)
```

### Comparing `owl2yams-1.2.1/owl2yams/generate_schema.py` & `owl2yams-1.3.0/owl2yams/generate_schema.py`

 * *Files identical despite different names*

### Comparing `owl2yams-1.2.1/owl2yams/generate_views.py` & `owl2yams-1.3.0/owl2yams/generate_views.py`

 * *Files identical despite different names*

### Comparing `owl2yams-1.2.1/owl2yams/prefixes.json` & `owl2yams-1.3.0/owl2yams/prefixes.json`

 * *Files identical despite different names*

### Comparing `owl2yams-1.2.1/owl2yams.egg-info/PKG-INFO` & `owl2yams-1.3.0/owl2yams.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owl2yams
-Version: 1.2.1
+Version: 1.3.0
 Summary: A tools to transforms owl into yams schema
 Home-page: https://forge.extranet.logilab.fr/cubicweb/owl2yams
 Author: Fabien Amarger
 Author-email: famarger@logilab.fr
 License: LGPL
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `owl2yams-1.2.1/owl2yams.egg-info/SOURCES.txt` & `owl2yams-1.3.0/owl2yams.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `owl2yams-1.2.1/setup.py` & `owl2yams-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 here = osp.abspath(osp.dirname(__file__))
 # Get the long description from the relevant file
 with open(osp.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 distname = "owl2yams"
-version = "1.2.1"
+version = "1.3.0"
 license = "LGPL"
 description = "A tools to transforms owl into yams schema"
 author = "Fabien Amarger"
 author_email = "famarger@logilab.fr"
 requires = {
     "cubicweb": None,
     "yams": ">=0.45.5",
```

### Comparing `owl2yams-1.2.1/test/test_owl2yams.py` & `owl2yams-1.3.0/test/test_owl2yams.py`

 * *Files identical despite different names*

