# Comparing `tmp/talisman-dm-1.0.0a5.tar.gz` & `tmp/talisman-dm-1.0.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/talisman-dm-1.0.0a5.tar", last modified: Mon Apr 10 10:58:44 2023, max compression
+gzip compressed data, was "dist/talisman-dm-1.0.0a6.tar", last modified: Mon Apr 24 13:34:20 2023, max compression
```

## Comparing `talisman-dm-1.0.0a5.tar` & `talisman-dm-1.0.0a6.tar`

### file list

```diff
@@ -1,97 +1,117 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/
--rw-r--r--   0 root         (0) root         (0)      778 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/README.md
--rw-rw-rw-   0 root         (0) root         (0)        7 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/VERSION
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1215 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/talisman_dm.egg-info/
--rw-r--r--   0 root         (0) root         (0)      778 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/talisman_dm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2450 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/talisman_dm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/talisman_dm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       80 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/talisman_dm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/talisman_dm.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/tdm/
--rw-rw-rw-   0 root         (0) root         (0)      244 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/tdm/abstract/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/abstract/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/tdm/abstract/datamodel/
--rw-rw-rw-   0 root         (0) root         (0)      663 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/abstract/datamodel/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1095 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/abstract/datamodel/base.py
--rw-rw-rw-   0 root         (0) root         (0)      247 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/abstract/datamodel/directive.py
--rw-rw-rw-   0 root         (0) root         (0)     3477 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/abstract/datamodel/document.py
--rw-rw-rw-   0 root         (0) root         (0)     1183 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/abstract/datamodel/fact.py
--rw-rw-rw-   0 root         (0) root         (0)      468 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/abstract/datamodel/link.py
--rw-rw-rw-   0 root         (0) root         (0)      258 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/abstract/datamodel/mention.py
--rw-rw-rw-   0 root         (0) root         (0)     1473 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/abstract/datamodel/node.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/tdm/abstract/json_schema/
--rw-rw-rw-   0 root         (0) root         (0)      278 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/abstract/json_schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4576 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/abstract/json_schema/composite.py
--rw-rw-rw-   0 root         (0) root         (0)     1098 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/abstract/json_schema/decorator.py
--rw-rw-rw-   0 root         (0) root         (0)     2902 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/abstract/json_schema/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/tdm/abstract/json_schema/serializers/
--rw-rw-rw-   0 root         (0) root         (0)      615 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/abstract/json_schema/serializers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1207 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/abstract/json_schema/serializers/abstract.py
--rw-rw-rw-   0 root         (0) root         (0)      704 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/abstract/json_schema/serializers/identifiable.py
--rw-rw-rw-   0 root         (0) root         (0)      653 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/abstract/json_schema/serializers/mention.py
--rw-rw-rw-   0 root         (0) root         (0)      641 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/abstract/json_schema/serializers/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)      543 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/abstract/json_schema/serializers/serializers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/tdm/datamodel/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/tdm/datamodel/directives/
--rw-rw-rw-   0 root         (0) root         (0)      239 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/directives/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      436 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/directives/account.py
--rw-rw-rw-   0 root         (0) root         (0)      759 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/directives/concept.py
--rw-rw-rw-   0 root         (0) root         (0)      488 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/directives/platform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/tdm/datamodel/document/
--rw-rw-rw-   0 root         (0) root         (0)      155 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/document/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6465 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/document/_base.py
--rw-rw-rw-   0 root         (0) root         (0)     2291 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/document/_container.py
--rw-rw-rw-   0 root         (0) root         (0)     1825 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/document/_factory.py
--rw-rw-rw-   0 root         (0) root         (0)    10015 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/document/_impl.py
--rw-rw-rw-   0 root         (0) root         (0)     7193 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/document/_structure.py
--rw-rw-rw-   0 root         (0) root         (0)      768 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/document/_types.py
--rw-rw-rw-   0 root         (0) root         (0)     4779 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/document/_view.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/tdm/datamodel/facts/
--rw-rw-rw-   0 root         (0) root         (0)      429 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/facts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/facts/concept.py
--rw-rw-rw-   0 root         (0) root         (0)      911 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/facts/links.py
--rw-rw-rw-   0 root         (0) root         (0)      555 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/facts/mention.py
--rw-rw-rw-   0 root         (0) root         (0)     1142 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/facts/value.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/tdm/datamodel/links/
--rw-rw-rw-   0 root         (0) root         (0)      155 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/links/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      675 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/links/reference.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/tdm/datamodel/mentions/
--rw-rw-rw-   0 root         (0) root         (0)      180 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/mentions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      724 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/mentions/image.py
--rw-rw-rw-   0 root         (0) root         (0)      233 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/mentions/node.py
--rw-rw-rw-   0 root         (0) root         (0)      614 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/mentions/text.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/tdm/datamodel/nodes/
--rw-rw-rw-   0 root         (0) root         (0)      649 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/nodes/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      428 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/nodes/base64.py
--rw-rw-rw-   0 root         (0) root         (0)      705 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/nodes/file.py
--rw-rw-rw-   0 root         (0) root         (0)     1113 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/nodes/structure.py
--rw-rw-rw-   0 root         (0) root         (0)      539 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/datamodel/nodes/text.py
--rw-rw-rw-   0 root         (0) root         (0)     1606 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/tdm/json_schema/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/json_schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      512 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/json_schema/directives.py
--rw-rw-rw-   0 root         (0) root         (0)      514 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/json_schema/facts.py
--rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/json_schema/links.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/json_schema/mentions.py
--rw-rw-rw-   0 root         (0) root         (0)     1789 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/json_schema/nodes.py
--rw-rw-rw-   0 root         (0) root         (0)     1033 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/legacy.py
--rw-rw-rw-   0 root         (0) root         (0)     2668 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/tdm/v0/
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/v0/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/tdm/v0/json_schema/
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/v0/json_schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/v0/json_schema/content.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 10:58:44.000000 talisman-dm-1.0.0a5/tdm/v0/json_schema/convert/
--rw-rw-rw-   0 root         (0) root         (0)      348 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/v0/json_schema/convert/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3901 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/v0/json_schema/convert/_facts.py
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/v0/json_schema/convert/_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     4648 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/v0/json_schema/convert/_nodes.py
--rw-rw-rw-   0 root         (0) root         (0)     1481 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/v0/json_schema/directive.py
--rw-rw-rw-   0 root         (0) root         (0)     3593 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/v0/json_schema/document.py
--rw-rw-rw-   0 root         (0) root         (0)     1453 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/v0/json_schema/fact.py
--rw-rw-rw-   0 root         (0) root         (0)      445 2023-04-10 10:58:39.000000 talisman-dm-1.0.0a5/tdm/v0/json_schema/metadata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:34:20.000000 talisman-dm-1.0.0a6/
+-rw-r--r--   0 root         (0) root         (0)      778 2023-04-24 13:34:20.000000 talisman-dm-1.0.0a6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-04-24 13:21:39.000000 talisman-dm-1.0.0a6/VERSION
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 13:34:20.000000 talisman-dm-1.0.0a6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1195 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:34:20.000000 talisman-dm-1.0.0a6/talisman_dm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      778 2023-04-24 13:34:20.000000 talisman-dm-1.0.0a6/talisman_dm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2993 2023-04-24 13:34:20.000000 talisman-dm-1.0.0a6/talisman_dm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 13:34:20.000000 talisman-dm-1.0.0a6/talisman_dm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-04-24 13:34:20.000000 talisman-dm-1.0.0a6/talisman_dm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-24 13:34:20.000000 talisman-dm-1.0.0a6/talisman_dm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:34:20.000000 talisman-dm-1.0.0a6/tdm/
+-rw-rw-rw-   0 root         (0) root         (0)      320 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:34:20.000000 talisman-dm-1.0.0a6/tdm/abstract/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-24 13:34:12.000000 talisman-dm-1.0.0a6/tdm/abstract/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:34:20.000000 talisman-dm-1.0.0a6/tdm/abstract/datamodel/
+-rw-rw-rw-   0 root         (0) root         (0)      908 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/abstract/datamodel/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1095 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/abstract/datamodel/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      247 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/abstract/datamodel/directive.py
+-rw-rw-rw-   0 root         (0) root         (0)     5052 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/abstract/datamodel/document.py
+-rw-rw-rw-   0 root         (0) root         (0)     3071 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/abstract/datamodel/fact.py
+-rw-rw-rw-   0 root         (0) root         (0)      604 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/abstract/datamodel/fact_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)      940 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/abstract/datamodel/link.py
+-rw-rw-rw-   0 root         (0) root         (0)     1793 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/abstract/datamodel/markup.py
+-rw-rw-rw-   0 root         (0) root         (0)      258 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/abstract/datamodel/mention.py
+-rw-rw-rw-   0 root         (0) root         (0)     1626 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/abstract/datamodel/node.py
+-rw-rw-rw-   0 root         (0) root         (0)      996 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/abstract/datamodel/value.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:34:20.000000 talisman-dm-1.0.0a6/tdm/abstract/json_schema/
+-rw-rw-rw-   0 root         (0) root         (0)      278 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/abstract/json_schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4947 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/abstract/json_schema/composite.py
+-rw-rw-rw-   0 root         (0) root         (0)     1184 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/abstract/json_schema/decorator.py
+-rw-rw-rw-   0 root         (0) root         (0)     4507 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/abstract/json_schema/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:34:20.000000 talisman-dm-1.0.0a6/tdm/abstract/json_schema/serializers/
+-rw-rw-rw-   0 root         (0) root         (0)      624 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/abstract/json_schema/serializers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1207 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/abstract/json_schema/serializers/abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)      704 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/abstract/json_schema/serializers/identifiable.py
+-rw-rw-rw-   0 root         (0) root         (0)      590 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/abstract/json_schema/serializers/markup.py
+-rw-rw-rw-   0 root         (0) root         (0)      653 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/abstract/json_schema/serializers/mention.py
+-rw-rw-rw-   0 root         (0) root         (0)      641 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/abstract/json_schema/serializers/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)      732 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/abstract/json_schema/serializers/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/abstract/json_schema/serializers/value.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:34:20.000000 talisman-dm-1.0.0a6/tdm/datamodel/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-24 13:34:12.000000 talisman-dm-1.0.0a6/tdm/datamodel/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:34:20.000000 talisman-dm-1.0.0a6/tdm/datamodel/directives/
+-rw-rw-rw-   0 root         (0) root         (0)      239 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/datamodel/directives/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      436 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/datamodel/directives/account.py
+-rw-rw-rw-   0 root         (0) root         (0)      768 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/datamodel/directives/concept.py
+-rw-rw-rw-   0 root         (0) root         (0)      488 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/datamodel/directives/platform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:34:20.000000 talisman-dm-1.0.0a6/tdm/datamodel/document/
+-rw-rw-rw-   0 root         (0) root         (0)      155 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/datamodel/document/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6465 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/datamodel/document/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2455 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/datamodel/document/_container.py
+-rw-rw-rw-   0 root         (0) root         (0)     1829 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/datamodel/document/_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)    13671 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/datamodel/document/_impl.py
+-rw-rw-rw-   0 root         (0) root         (0)     7193 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/datamodel/document/_structure.py
+-rw-rw-rw-   0 root         (0) root         (0)      768 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/datamodel/document/_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     5139 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/datamodel/document/_view.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:34:20.000000 talisman-dm-1.0.0a6/tdm/datamodel/facts/
+-rw-rw-rw-   0 root         (0) root         (0)      429 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/datamodel/facts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2424 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/datamodel/facts/concept.py
+-rw-rw-rw-   0 root         (0) root         (0)      911 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/datamodel/facts/links.py
+-rw-rw-rw-   0 root         (0) root         (0)     1106 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/datamodel/facts/mention.py
+-rw-rw-rw-   0 root         (0) root         (0)     2473 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/datamodel/facts/value.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:34:20.000000 talisman-dm-1.0.0a6/tdm/datamodel/links/
+-rw-rw-rw-   0 root         (0) root         (0)      155 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/datamodel/links/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      962 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/datamodel/links/reference.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:34:20.000000 talisman-dm-1.0.0a6/tdm/datamodel/mentions/
+-rw-rw-rw-   0 root         (0) root         (0)      180 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/datamodel/mentions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/datamodel/mentions/image.py
+-rw-rw-rw-   0 root         (0) root         (0)      233 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/datamodel/mentions/node.py
+-rw-rw-rw-   0 root         (0) root         (0)      759 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/datamodel/mentions/text.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:34:20.000000 talisman-dm-1.0.0a6/tdm/datamodel/nodes/
+-rw-rw-rw-   0 root         (0) root         (0)      649 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/datamodel/nodes/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      428 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/datamodel/nodes/base64.py
+-rw-rw-rw-   0 root         (0) root         (0)      705 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/datamodel/nodes/file.py
+-rw-rw-rw-   0 root         (0) root         (0)     1113 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/datamodel/nodes/structure.py
+-rw-rw-rw-   0 root         (0) root         (0)      938 2023-04-24 13:20:28.000000 talisman-dm-1.0.0a6/tdm/datamodel/nodes/text.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:34:20.000000 talisman-dm-1.0.0a6/tdm/datamodel/values/
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/datamodel/values/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      875 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/datamodel/values/date.py
+-rw-rw-rw-   0 root         (0) root         (0)      790 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/datamodel/values/geo.py
+-rw-rw-rw-   0 root         (0) root         (0)      333 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/datamodel/values/link.py
+-rw-rw-rw-   0 root         (0) root         (0)      717 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/datamodel/values/scalar.py
+-rw-rw-rw-   0 root         (0) root         (0)     2747 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:34:20.000000 talisman-dm-1.0.0a6/tdm/json_schema/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-24 13:34:12.000000 talisman-dm-1.0.0a6/tdm/json_schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      512 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/json_schema/directives.py
+-rw-rw-rw-   0 root         (0) root         (0)      514 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/json_schema/facts.py
+-rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/json_schema/links.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/json_schema/mentions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1789 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/json_schema/nodes.py
+-rw-rw-rw-   0 root         (0) root         (0)      513 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/json_schema/values.py
+-rw-rw-rw-   0 root         (0) root         (0)     1033 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/legacy.py
+-rw-rw-rw-   0 root         (0) root         (0)     2808 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:34:20.000000 talisman-dm-1.0.0a6/tdm/v0/
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/v0/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:34:20.000000 talisman-dm-1.0.0a6/tdm/v0/json_schema/
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/v0/json_schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/v0/json_schema/content.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:34:20.000000 talisman-dm-1.0.0a6/tdm/v0/json_schema/convert/
+-rw-rw-rw-   0 root         (0) root         (0)      348 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/v0/json_schema/convert/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4731 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/v0/json_schema/convert/_facts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1630 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/v0/json_schema/convert/_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     4725 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/v0/json_schema/convert/_nodes.py
+-rw-rw-rw-   0 root         (0) root         (0)     1481 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/v0/json_schema/directive.py
+-rw-rw-rw-   0 root         (0) root         (0)     3689 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/v0/json_schema/document.py
+-rw-rw-rw-   0 root         (0) root         (0)     1453 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/v0/json_schema/fact.py
+-rw-rw-rw-   0 root         (0) root         (0)      445 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/v0/json_schema/metadata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:34:20.000000 talisman-dm-1.0.0a6/tdm/wrapper/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-24 13:34:12.000000 talisman-dm-1.0.0a6/tdm/wrapper/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 13:34:20.000000 talisman-dm-1.0.0a6/tdm/wrapper/node/
+-rw-rw-rw-   0 root         (0) root         (0)      434 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/wrapper/node/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2633 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/wrapper/node/_decorator.py
+-rw-rw-rw-   0 root         (0) root         (0)      551 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/wrapper/node/_delegate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1647 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/wrapper/node/_impl.py
+-rw-rw-rw-   0 root         (0) root         (0)      445 2023-04-24 10:06:58.000000 talisman-dm-1.0.0a6/tdm/wrapper/node/_interface.py
```

### Comparing `talisman-dm-1.0.0a5/PKG-INFO` & `talisman-dm-1.0.0a6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talisman-dm
-Version: 1.0.0a5
+Version: 1.0.0a6
 Summary: Talisman Document Model python implementation
 Home-page: https://gitlab.at.ispras.ru/talisman/core/talisman-tdm
 Author: ISPRAS MODIS NLP team
 Author-email: modis@ispras.ru
 Maintainer: Vladimir Mayorov
 Maintainer-email: vmayorov@ispras.ru
 License: Apache Software License
```

### Comparing `talisman-dm-1.0.0a5/setup.py` & `talisman-dm-1.0.0a6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     long_description_content_type="text/markdown",
     url='https://gitlab.at.ispras.ru/talisman/core/talisman-tdm',
     author='ISPRAS MODIS NLP team',
     author_email='modis@ispras.ru',
     maintainer='Vladimir Mayorov',
     maintainer_email='vmayorov@ispras.ru',
     packages=find_packages(include=['tdm', 'tdm.*']),
-    install_requires=['pydantic>=1.10.5', 'typing-extensions>=4.0.1', 'intervaltree>=3.0.2', 'frozendict~=2.3.4'],
+    install_requires=['pydantic>=1.10.5', 'typing-extensions>=4.0.1', 'immutabledict~=2.2.4'],
     data_files=[('', ['VERSION'])],
     python_requires='>=3.7',
     license='Apache Software License',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
```

### Comparing `talisman-dm-1.0.0a5/talisman_dm.egg-info/PKG-INFO` & `talisman-dm-1.0.0a6/talisman_dm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talisman-dm
-Version: 1.0.0a5
+Version: 1.0.0a6
 Summary: Talisman Document Model python implementation
 Home-page: https://gitlab.at.ispras.ru/talisman/core/talisman-tdm
 Author: ISPRAS MODIS NLP team
 Author-email: modis@ispras.ru
 Maintainer: Vladimir Mayorov
 Maintainer-email: vmayorov@ispras.ru
 License: Apache Software License
```

### Comparing `talisman-dm-1.0.0a5/tdm/abstract/datamodel/base.py` & `talisman-dm-1.0.0a6/tdm/abstract/datamodel/base.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a5/tdm/abstract/datamodel/document.py` & `talisman-dm-1.0.0a6/tdm/abstract/datamodel/document.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from abc import ABCMeta, abstractmethod
-from typing import Any, Dict, Iterable, Optional, Set, Tuple, Type, TypeVar, Union
+from typing import Any, Callable, Dict, Iterable, Iterator, Optional, Set, Tuple, Type, TypeVar, Union
 
+from .base import Identifiable
 from .directive import AbstractDirective
 from .fact import AbstractFact
 from .link import AbstractNodeLink
 from .node import AbstractNode
 
 _TD = TypeVar('_TD', bound='TalismanDocument')
+_Fact = TypeVar('_Fact', bound=AbstractFact)
+_NodeLink = TypeVar('_NodeLink', bound=AbstractNodeLink)
+_Node = TypeVar('_Node', bound=AbstractNode)
 
 NodeOrId = Union[str, AbstractNode]
 
 
 class TalismanDocument(metaclass=ABCMeta):
     @property
     @abstractmethod
@@ -19,14 +23,25 @@
 
     @property
     @abstractmethod
     def nodes(self) -> Dict[str, AbstractNode]:
         pass
 
     @abstractmethod
+    def get_node(self, id_: str) -> AbstractNode:
+        pass
+
+    @abstractmethod
+    def get_nodes(
+            self, type_: Type[_Node] = AbstractNode, *,
+            filter_: Union[Callable[[_Node], bool], Iterable[Callable[[_Node], bool]]] = tuple()
+    ) -> Iterator[_Node]:
+        pass
+
+    @abstractmethod
     def with_nodes(self: _TD, nodes: Iterable[AbstractNode]) -> _TD:
         pass
 
     @abstractmethod
     def without_nodes(self: _TD, nodes: Iterable[NodeOrId], *, cascade: bool = True) -> _TD:
         pass
 
@@ -49,48 +64,76 @@
         pass
 
     @abstractmethod
     def child_nodes(self, node: Union[str, AbstractNode]) -> Tuple[AbstractNode, ...]:
         pass
 
     @abstractmethod
-    def with_links(self: _TD, links: Dict[NodeOrId, Iterable[NodeOrId]], *, force: bool = False, update: bool = False) -> _TD:
+    def with_structure(self: _TD, structure: Dict[NodeOrId, Iterable[NodeOrId]], *, force: bool = False, update: bool = False) -> _TD:
         pass
 
     @abstractmethod
-    def with_link(self: _TD, parent: NodeOrId, child: NodeOrId, *, force: bool = False, update: bool = False) -> _TD:
+    def with_node_parent(self: _TD, child: NodeOrId, parent: NodeOrId, *, force: bool = False, update: bool = False) -> _TD:
         pass
 
     @abstractmethod
-    def without_parent_links(self: _TD, nodes: Iterable[NodeOrId]) -> _TD:
+    def with_roots(self: _TD, nodes: Iterable[NodeOrId]) -> _TD:
         pass
 
     @abstractmethod
-    def without_links(self: _TD, links: Dict[NodeOrId, Iterable[NodeOrId]]) -> _TD:
+    def without_structure(self: _TD, structure: Dict[NodeOrId, Iterable[NodeOrId]]) -> _TD:
         pass
 
     @property
     @abstractmethod
     def node_links(self) -> Dict[Type[AbstractNodeLink], Iterable[AbstractNodeLink]]:
         pass
 
     @abstractmethod
+    def get_node_links(
+            self, type_: Type[_NodeLink] = AbstractNodeLink, *,
+            filter_: Union[Callable[[_NodeLink], bool], Iterable[Callable[[_NodeLink], bool]]] = tuple()
+    ) -> Iterator[_NodeLink]:
+        pass
+
+    @abstractmethod
+    def related_node_links(
+            self, obj: Union[Identifiable, str], type_: Type[_NodeLink] = AbstractNodeLink, *,
+            filter_: Union[Callable[[_NodeLink], bool], Iterable[Callable[[_NodeLink], bool]]] = tuple()
+    ) -> Iterator[_NodeLink]:
+        pass
+
+    @abstractmethod
     def with_node_links(self: _TD, links: Iterable[AbstractNodeLink], *, update: bool = False) -> _TD:
         pass
 
     @abstractmethod
     def without_node_links(self: _TD, links: Iterable[Union[str, AbstractNodeLink]], *, cascade: bool = False) -> _TD:
         pass
 
     @property
     @abstractmethod
     def facts(self) -> Dict[Type[AbstractFact], Iterable[AbstractFact]]:
         pass
 
     @abstractmethod
+    def get_facts(
+            self, type_: Type[_Fact] = AbstractFact, *,
+            filter_: Union[Callable[[_Fact], bool], Iterable[Callable[[_Fact], bool]]] = tuple()
+    ) -> Iterator[_Fact]:
+        pass
+
+    @abstractmethod
+    def related_facts(
+            self, obj: Union[Identifiable, str], type_: Type[_Fact] = AbstractFact, *,
+            filter_: Union[Callable[[_Fact], bool], Iterable[Callable[[_Fact], bool]]] = tuple()
+    ) -> Iterator[_Fact]:
+        pass
+
+    @abstractmethod
     def with_facts(self: _TD, facts: Iterable[AbstractFact], *, update: bool = False) -> _TD:
         pass
 
     @abstractmethod
     def without_facts(self: _TD, facts: Iterable[Union[str, AbstractFact]], *, cascade: bool = False) -> _TD:
         pass
```

### Comparing `talisman-dm-1.0.0a5/tdm/abstract/datamodel/node.py` & `talisman-dm-1.0.0a6/tdm/abstract/datamodel/node.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,53 +1,55 @@
 from dataclasses import dataclass, field
 from typing import Generic, Set, TypeVar
 
-from frozendict import frozendict
-
 from tdm.helper import generics_mapping
 from .base import Identifiable
+from .markup import AbstractMarkup, FrozenMarkup
 
 
 @dataclass(frozen=True)
 class BaseNodeMetadata:
     hidden: bool = False
 
 
 _NodeMetadata = TypeVar("_NodeMetadata", bound=BaseNodeMetadata)
 
 
 @dataclass(frozen=True)
 class AbstractNode(Identifiable, Generic[_NodeMetadata]):
     metadata: _NodeMetadata = None
+    markup: AbstractMarkup = field(default_factory=FrozenMarkup, hash=False)
 
     def __post_init__(self):
         super().__post_init__()
         if self.metadata is None:
             # hack for runtime metadata generation (if no value passed)
             object.__setattr__(self, 'metadata', self._generate_metadata())
+        object.__setattr__(self, 'markup', self._convert_markup(self.markup))
+
+    def _convert_markup(self, markup: AbstractMarkup) -> AbstractMarkup:
+        if not isinstance(markup, AbstractMarkup):
+            raise ValueError
+        return markup
 
     def _generate_metadata(self) -> _NodeMetadata:
         type_vars = generics_mapping(type(self))
-        return type_vars[self.__dataclass_fields__['metadata'].type]()
+        return type_vars[_NodeMetadata]()
 
     @classmethod
     def constant_fields(cls) -> Set[str]:
         return set()
 
 
 _Content = TypeVar('_Content')
 
 
 @dataclass(frozen=True)
 class _AbstractContentNode(Generic[_Content]):
     content: _Content
-    markup: dict = field(default_factory=frozendict, hash=False)
-
-    def __post_init__(self):
-        object.__setattr__(self, 'markup', frozendict(self.markup))
 
 
 @dataclass(frozen=True)
 class AbstractContentNode(AbstractNode[_NodeMetadata], _AbstractContentNode[_Content], Generic[_NodeMetadata, _Content]):
 
     @classmethod
     def constant_fields(cls) -> Set[str]:
```

### Comparing `talisman-dm-1.0.0a5/tdm/abstract/json_schema/composite.py` & `talisman-dm-1.0.0a6/tdm/abstract/json_schema/composite.py`

 * *Files 13% similar despite different names*

```diff
@@ -108,10 +108,16 @@
             if len(clss) == 1:
                 result[cls] = self._cls2label_model[clss[0]][1]
             else:
                 types = tuple(map(lambda cls_: self._cls2label_model[cls_][1], clss))
                 result[cls] = Annotated[Union[types], Field(discriminator=discriminator)] if discriminator is not None else Union[types]
 
         def serialize(element: _DATA) -> ElementModel[_DATA]:
+            if type(element) not in result:
+                try:
+                    supertype = next(filter(lambda t: t in result, type(element).mro()))
+                except StopIteration:
+                    raise ValueError(f"there is no applicable serializers for {type(element)} type (object: {element})")
+                result[type(element)] = result[supertype]
             return result[type(element)].serialize(element)
 
         return result, serialize
```

### Comparing `talisman-dm-1.0.0a5/tdm/abstract/json_schema/decorator.py` & `talisman-dm-1.0.0a6/tdm/abstract/json_schema/decorator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from typing import Type, TypeVar
 
-from tdm.abstract.datamodel import AbstractDirective, AbstractFact, AbstractNode, AbstractNodeLink, AbstractNodeMention
+from tdm.abstract.datamodel import AbstractDirective, AbstractFact, AbstractNode, AbstractNodeLink, AbstractNodeMention, AbstractValue
 from .composite import ModelsGenerator
 
 _MODELS_GENERATORS = {
     AbstractDirective: ModelsGenerator(AbstractDirective),
     AbstractFact: ModelsGenerator(AbstractFact),
     AbstractNodeLink: ModelsGenerator(AbstractNodeLink),
     AbstractNodeMention: ModelsGenerator(AbstractNodeMention, include_label=True),
-    AbstractNode: ModelsGenerator(AbstractNode, include_label=True)
+    AbstractNode: ModelsGenerator(AbstractNode, include_label=True),
+    AbstractValue: ModelsGenerator(AbstractValue, include_label=True)
 }
 
 _Element = TypeVar('_Element')
 
 
 def get_model_generator(cls: Type[_Element]) -> ModelsGenerator[_Element]:
     for cls_, generator in _MODELS_GENERATORS.items():
```

### Comparing `talisman-dm-1.0.0a5/tdm/abstract/json_schema/model.py` & `talisman-dm-1.0.0a6/tdm/model.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,78 +1,75 @@
-import dataclasses
-from dataclasses import fields
-from typing import Any, Dict, Generic, Optional, Type, TypeVar
+from typing import Dict, Optional, Tuple
 
-from pydantic import BaseModel, Extra, create_model, root_validator
-from typing_extensions import Literal, Self
+from immutabledict import immutabledict
+from pydantic import BaseModel, root_validator
+from typing_extensions import Literal
+
+from .abstract.datamodel import AbstractNode, TalismanDocument
+from .datamodel.document import TalismanDocumentFactory
+from .json_schema.directives import DirectivesModel
+from .json_schema.facts import FactsModel
+from .json_schema.links import NodeLinksModel
+from .json_schema.nodes import NodeModel, fill_children, serialize_node
+from .legacy import DocumentMetadataModel
 
-from tdm.helper import cache_result, generics_mapping, is_subclass
-from .serializers import AbstractElementModel, AbstractElementSerializer, BaseSerializers
 
-_Element = TypeVar('_Element')
-
-
-# hackish root validator solution as normal validators are not called for skipped required fields
-def set_type_if_none(cls, values):
-    if 'type' not in values:
-        values['type'] = cls.__fields__['type'].type_.__args__[0]  # get arg of Literal ('type' field type)
-    return values
-
-
-class ElementModel(BaseModel, AbstractElementModel[_Element], Generic[_Element]):
+class TalismanDocumentModel(BaseModel):
     class Config:
-        extra = Extra.forbid
-
-    def deserialize(self, typed_id2element: Dict[type, Dict[str, Any]]) -> _Element:
-        raise NotImplementedError
+        json_encoders = {
+            immutabledict: lambda x: dict(x)
+        }
+
+    VERSION: Literal['1.0'] = ...
+    id: str
+    main_node: str
+    content: Tuple[NodeModel, ...]
+    links: NodeLinksModel
+    facts: FactsModel
+    directives: DirectivesModel
+
+    metadata: Optional[DocumentMetadataModel]  # should be removed in future
+
+    @root_validator(pre=True)
+    def _set_version(cls, values):  # noqa N805: pydantic requires cls to be first argument in validators
+        if 'VERSION' not in values:
+            values['VERSION'] = '1.0'
+        return values
+
+    def deserialize(self) -> TalismanDocument:
+        id2node, structure = self._collect_nodes()
+
+        return TalismanDocumentFactory.construct(
+            content=id2node.values(),
+            structure=structure,
+            root=self.main_node,
+            node_links=self.links.deserialize(id2node),
+            facts=self.facts.deserialize(id2node),
+            directives=self.directives.deserialize(id2node),
+            metadata=self.metadata.to_metadata() if self.metadata is not None else None,
+            id_=self.id
+        )
+
+    def _collect_nodes(self) -> Tuple[Dict[str, AbstractNode], Dict[str, Tuple[str, ...]]]:
+        # try to avoid recursion
+        links: Dict[str, Tuple[str, ...]] = {}
+        id2node = {}
+
+        for node_model in self.content:
+            id2node[node_model.id] = node_model.deserialize({})
+            if node_model.children:
+                links[node_model.id] = node_model.children
+        return id2node, links
 
     @classmethod
-    def serialize(cls, element: _Element) -> Self:
-        kwargs = {}
-        for key, value in element.__dict__.items():
-            for type_, serializer in BaseSerializers.items():
-                if isinstance(value, type_):
-                    kwargs[key] = serializer.serialize(value)
-                    break
-            else:
-                kwargs[key] = value
-        return cls(**kwargs)
-
-
-_BaseType = TypeVar('_BaseType', bound=type)
-
-
-@cache_result()
-def create_model_for_type(type_: Type[_Element], label: Optional[str] = None) -> Type[ElementModel[_Element]]:
-    type_vars = generics_mapping(type_)
-
-    model_fields = {}
-    validators = {}
-
-    special_fields: Dict[str, AbstractElementSerializer] = {}
-
-    for field in fields(type_):
-        name = field.name
-        default_value = field.default if field.default is not dataclasses.MISSING else ...
-        field_type = type_vars.get(field.type, field.type)
-        for _type, serializer in BaseSerializers.items():
-            if is_subclass(field_type, _type):
-                field_type = serializer.field_type(field_type)
-                special_fields[name] = serializer
-        model_fields[name] = (field_type, default_value)
-    if label:
-        model_fields['type'] = (Literal[label], ...)
-        validators['set_if_none'] = root_validator(pre=True, allow_reuse=True)(set_type_if_none)
-
-    model = create_model(f"{type_.__name__}Model", __base__=ElementModel, __validators__=validators, **model_fields)
-
-    def deserialize(self: model, typed_id2element: Dict[type, Dict[str, Any]]) -> type_:
-        kwargs = {}
-        for f in set(type_.__dataclass_fields__).intersection(self.__dict__):
-            kwargs[f] = getattr(self, f)
-            if f in special_fields:
-                kwargs[f] = special_fields[f].deserialize(kwargs[f], typed_id2element)
-        return type_(**kwargs)
-
-    model.deserialize = deserialize
-
-    return model
+    def serialize(cls, document: TalismanDocument) -> 'TalismanDocumentModel':
+        node_models = tuple(serialize_node(node) for node in document.nodes.values())
+        fill_children(node_models, document)
+        return cls(
+            id=document.id,
+            main_node=document.main_root.id,
+            content=node_models,
+            links=NodeLinksModel.serialize(document.node_links),
+            facts=FactsModel.serialize(document.facts),
+            directives=DirectivesModel.serialize(document.directives),
+            metadata=DocumentMetadataModel(**document._metadata) if document._metadata is not None else None
+        )
```

### Comparing `talisman-dm-1.0.0a5/tdm/abstract/json_schema/serializers/abstract.py` & `talisman-dm-1.0.0a6/tdm/abstract/json_schema/serializers/abstract.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a5/tdm/abstract/json_schema/serializers/identifiable.py` & `talisman-dm-1.0.0a6/tdm/abstract/json_schema/serializers/identifiable.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a5/tdm/abstract/json_schema/serializers/mention.py` & `talisman-dm-1.0.0a6/tdm/abstract/json_schema/serializers/mention.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a5/tdm/abstract/json_schema/serializers/metadata.py` & `talisman-dm-1.0.0a6/tdm/abstract/json_schema/serializers/metadata.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a5/tdm/abstract/json_schema/serializers/serializers.py` & `talisman-dm-1.0.0a6/tdm/abstract/json_schema/serializers/serializers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-from tdm.abstract.datamodel import AbstractFact, AbstractNode, AbstractNodeMention, BaseNodeMetadata
+from tdm.abstract.datamodel import AbstractFact, AbstractMarkup, AbstractNode, AbstractNodeMention, AbstractValue, BaseNodeMetadata
 from .identifiable import IdSerializer
+from .markup import MarkupSerializer
 from .mention import NodeMentionSerializer
 from .metadata import NodeMetadataSerializer
+from .value import ValueSerializer
 
 
 def build_serializers():
     result = {
         AbstractNode: IdSerializer(AbstractNode),
         AbstractFact: IdSerializer(AbstractFact),
         AbstractNodeMention: NodeMentionSerializer(),
-        BaseNodeMetadata: NodeMetadataSerializer()
+        BaseNodeMetadata: NodeMetadataSerializer(),
+        AbstractValue: ValueSerializer(),
+        AbstractMarkup: MarkupSerializer()
     }
     # other serializers could be added here
     return result
```

### Comparing `talisman-dm-1.0.0a5/tdm/datamodel/directives/concept.py` & `talisman-dm-1.0.0a6/tdm/datamodel/directives/concept.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import dataclass
 from typing import Optional, Tuple
 
-from frozendict import frozendict
+from immutabledict import immutabledict
 
 from tdm.abstract.datamodel import AbstractDirective, Identifiable
 from tdm.abstract.json_schema import generate_model
 
 
 @dataclass(frozen=True)
 class _CreateConceptDirective(AbstractDirective):
@@ -13,15 +13,15 @@
     concept_type: str
     filters: Tuple[dict, ...]
     notes: Optional[str] = None
     markers: Optional[str] = None
     access_level: Optional[str] = None
 
     def __post_init__(self):
-        filters = tuple(frozendict(f) for f in self.filters)
+        filters = tuple(immutabledict(f) for f in self.filters)
         object.__setattr__(self, 'filters', filters)
 
 
 @generate_model(label='create_concept')
 @dataclass(frozen=True)
 class CreateConceptDirective(Identifiable, _CreateConceptDirective):
     pass
```

### Comparing `talisman-dm-1.0.0a5/tdm/datamodel/document/_base.py` & `talisman-dm-1.0.0a6/tdm/datamodel/document/_base.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a5/tdm/datamodel/document/_container.py` & `talisman-dm-1.0.0a6/tdm/datamodel/document/_container.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from collections import defaultdict
 from itertools import chain
 from typing import Dict, Generic, Iterable, Iterator, Set, Tuple, Type, TypeVar, Union
 
-from frozendict import frozendict
+from immutabledict import immutabledict
 
 _T = TypeVar('_T')
 
 
 class TypedIdsContainer(Iterable[Tuple[str, type]], Generic[_T]):
     __slots__ = ('_base', '_id2type', '_type2ids')
 
     def __init__(self, base: Type[_T], data: Union[Dict[str, Type[_T]], Iterable[Tuple[str, Type[_T]]]]):
         self._base = base
         if not isinstance(data, dict):
             data = dict(data)
         if any(not issubclass(t, self._base) for t in data.values()):
             raise ValueError
-        self._id2type = frozendict(data)
+        self._id2type = immutabledict(data)
         # self._id2data = frozendict(data if isinstance(data, dict) else {item.id: item for item in data})
         self._type2ids = None
 
     @classmethod
     def create(cls, base: Type[_T], data: Iterable[Tuple[str, type]]):
         return data if isinstance(data, cls) and data._base is base else cls(base, data)
 
@@ -51,11 +51,12 @@
         if isinstance(item, str):
             return item in self._id2type
         return self._id2type.get(item[0], None) == item[1]
 
     def __eq__(self, o: object) -> bool:
         if not isinstance(o, TypedIdsContainer):
             return NotImplemented
-        return self._base is o._base and self._id2type == o._id2type
+        return self._base is o._base and self._id2type.keys() == o._id2type.keys() \
+            and all(issubclass(s, t) or issubclass(t, s) for s, t in map(lambda k: (self._id2type[k], o._id2type[k]), self._id2type))
 
     def __hash__(self) -> int:
-        return hash((self._base, self._id2type))
+        return hash((self._base, len(self._id2type)))
```

### Comparing `talisman-dm-1.0.0a5/tdm/datamodel/document/_factory.py` & `talisman-dm-1.0.0a6/tdm/datamodel/document/_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             facts: Iterable[AbstractFact] = (),
             directives: Iterable[AbstractDirective] = (),
             metadata: Optional[Dict[str, Any]] = None,
             *, id_: Optional[str] = None
     ) -> TalismanDocument:
         doc: TalismanDocumentImpl = self.create_document(id_=id_)
         doc = doc.with_elements((*content, *node_links, *facts, *directives)) \
-            .with_links(structure) \
+            .with_structure(structure) \
             .with_main_root(root) \
             .with_metadata(metadata)
         return doc
 
     @staticmethod
     def generate_id():
         return str(uuid.uuid4())
```

### Comparing `talisman-dm-1.0.0a5/tdm/datamodel/document/_structure.py` & `talisman-dm-1.0.0a6/tdm/datamodel/document/_structure.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a5/tdm/datamodel/document/_types.py` & `talisman-dm-1.0.0a6/tdm/datamodel/document/_types.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a5/tdm/datamodel/document/_view.py` & `talisman-dm-1.0.0a6/tdm/datamodel/document/_view.py`

 * *Files 8% similar despite different names*

```diff
@@ -101,23 +101,32 @@
 
     def get_dependencies(self, obj) -> Set[EnsureIdentifiable]:
         r = {getattr(obj, field_name) for field_name in id_fields}
         for field_name in restore_fields:
             r.update(getattr(self, field_name).get_dependencies(getattr(obj, field_name)))
         return r
 
+    def eq(self, other) -> bool:
+        if not isinstance(other, AbstractView):
+            return NotImplemented
+        self_orig = self.orig_type()
+        other_orig = other.orig_type()
+        return (issubclass(self_orig, other_orig) or issubclass(other_orig, self_orig)) and self.__dict__ == other.__dict__
+
     view_type = make_dataclass(
         cls_name=f"{type_.__name__}View",
         fields=class_fields,
         bases=(AbstractView,),
+        eq=False,
         namespace={
             'get_object': get_object,
             'validate_update': validate_update,
             'orig_type': lambda _: type_,
-            'get_dependencies': get_dependencies
+            'get_dependencies': get_dependencies,
+            '__eq__': eq
         },
         frozen=True
     )
 
     __depends_on__ = generate_depends_on(id_fields, restore_fields)
 
     def constructor(obj: _ST) -> _TT:
```

### Comparing `talisman-dm-1.0.0a5/tdm/datamodel/facts/links.py` & `talisman-dm-1.0.0a6/tdm/datamodel/facts/links.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a5/tdm/datamodel/nodes/__init__.py` & `talisman-dm-1.0.0a6/tdm/datamodel/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a5/tdm/datamodel/nodes/file.py` & `talisman-dm-1.0.0a6/tdm/datamodel/nodes/file.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a5/tdm/datamodel/nodes/structure.py` & `talisman-dm-1.0.0a6/tdm/datamodel/nodes/structure.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a5/tdm/json_schema/directives.py` & `talisman-dm-1.0.0a6/tdm/json_schema/directives.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a5/tdm/json_schema/facts.py` & `talisman-dm-1.0.0a6/tdm/json_schema/facts.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a5/tdm/json_schema/mentions.py` & `talisman-dm-1.0.0a6/tdm/json_schema/mentions.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a5/tdm/json_schema/nodes.py` & `talisman-dm-1.0.0a6/tdm/json_schema/nodes.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a5/tdm/legacy.py` & `talisman-dm-1.0.0a6/tdm/legacy.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a5/tdm/v0/json_schema/content.py` & `talisman-dm-1.0.0a6/tdm/v0/json_schema/content.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a5/tdm/v0/json_schema/convert/_facts.py` & `talisman-dm-1.0.0a6/tdm/v0/json_schema/convert/_facts.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,81 @@
 from operator import attrgetter
-from typing import Dict, Iterator, Optional, Tuple, Union
+from typing import Dict, Iterator, Optional, Sequence, Tuple, Type, Union
 
-from tdm.abstract.datamodel import AbstractFact, FactStatus, Identifiable, TalismanDocument
+from tdm.abstract.datamodel import AbstractFact, AbstractValue, FactStatus, Identifiable, TalismanDocument
 from tdm.datamodel.facts import AtomValueFact, ConceptFact, MentionFact, PropertyFact, RelationFact, RelationPropertyFact
+from tdm.datamodel.facts.concept import ConceptValue
 from tdm.datamodel.mentions import TextNodeMention
 from tdm.datamodel.nodes import TextNode
+from tdm.datamodel.values import StringValue
 from tdm.v0.json_schema.fact import AbstractFactModel, ConceptFactModel, PropertyFactModel, RelationFactModel, ValueFactModel
 
 
 def _fact_text(fact: AbstractFactModel) -> Optional[str]:
     if fact.metadata is not None and hasattr(fact.metadata, 'text'):
         return ' '.join(fact.metadata.text)
     if fact.mention:
         return ' '.join(map(attrgetter('value'), fact.mention))
     return None
 
 
-def convert_concept_fact(fact: ConceptFactModel, doc: TalismanDocument, titles: Dict[str, Tuple[str, str]]) -> Iterator[AbstractFact]:
+def convert_concept_fact(
+        fact: ConceptFactModel, doc: TalismanDocument, titles: Dict[str, Tuple[str, str]], value_types: Dict[str, Type[AbstractValue]]
+) -> Iterator[AbstractFact]:
     status = FactStatus(fact.status.value)
+    if isinstance(fact.value, str):
+        value = ConceptValue(fact.value)
+    elif isinstance(fact.value, Sequence):
+        value = tuple(ConceptValue(v) for v in fact.value)
+    else:
+        raise ValueError(f"illegal concept fact value {fact.value}")
     concept_fact = ConceptFact(
         status=status,
         type_id=fact.type_id,
-        value=fact.value,
+        value=value,
         id=fact.id  # preserve old id
     )
     yield concept_fact
     name = _fact_text(fact)
     if not name:
         return
     property_type_id, value_type_id = titles[fact.type_id]
+    if value_types[value_type_id] is not StringValue:
+        raise ValueError
     old_fashion_value = ValueFactModel(
         id=Identifiable.generate_id(),
         status=fact.status,
         type_id=value_type_id,
         value={'value': name},
         mention=fact.mention,
         metadata=fact.metadata
     )
-    value, *other = convert_value_fact(old_fashion_value, doc)
+    value, *other = convert_value_fact(old_fashion_value, doc, value_types)
     yield value
     yield from other
     yield PropertyFact(
         status=status,
         type_id=property_type_id,
         source=concept_fact,
         target=value
     )
 
 
-def convert_value_fact(fact: ValueFactModel, doc: TalismanDocument) -> Iterator[AbstractFact]:
+def convert_value_fact(fact: ValueFactModel, doc: TalismanDocument, value_types: Dict[str, Type[AbstractValue]]) -> Iterator[AbstractFact]:
     status = FactStatus(fact.status.value)
+    if isinstance(fact.value, dict):
+        value = value_types[fact.type_id].from_dict(fact.value)
+    elif isinstance(fact.value, Sequence):
+        value = tuple(value_types[fact.type_id].from_dict(v) for v in fact.value)
+    else:
+        raise ValueError
     value = AtomValueFact(
         status=status,
         type_id=fact.type_id,
-        value=fact.value,
+        value=value,
         id=fact.id
     )
     yield value
 
     if fact.mention:
         # get only first span of multi-span mention
         node = doc.nodes[fact.mention[0].node_id]
```

### Comparing `talisman-dm-1.0.0a5/tdm/v0/json_schema/convert/_metadata.py` & `talisman-dm-1.0.0a6/tdm/v0/json_schema/convert/_metadata.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 from itertools import chain
 from typing import Any, Dict, Iterable
 
 from tdm.abstract.datamodel import AbstractFact, FactStatus
 from tdm.datamodel.facts import AtomValueFact, ConceptFact, PropertyFact, RelationFact
+from tdm.datamodel.facts.concept import ConceptValue
+from tdm.datamodel.values import DoubleValue, IntValue, StringValue
 
 
 def get_metadata_facts(doc_id: str, metadata: Dict[str, Any]) -> Iterable[AbstractFact]:
-    document_fact = ConceptFact(FactStatus.APPROVED, "document", doc_id)
+    document_fact = ConceptFact(FactStatus.APPROVED, "document", ConceptValue(doc_id))
     result = [document_fact]
     metadata = metadata
     if not metadata:
         return result
     if 'parent_uuid' in metadata:
         result.append(
             RelationFact(
-                FactStatus.APPROVED, "parent", document_fact, ConceptFact(FactStatus.APPROVED, "document", metadata.pop('parent_uuid'))
+                FactStatus.APPROVED, "parent", document_fact,
+                ConceptFact(FactStatus.APPROVED, "document", ConceptValue(metadata.pop('parent_uuid')))
             )
         )
     for key, value in metadata.items():
         value_facts = generate_value(value)
         result.extend(
             PropertyFact(FactStatus.APPROVED, key, document_fact, value_fact) for value_fact in value_facts
         )
     return result
 
 
 def generate_value(val: Any) -> Iterable[AtomValueFact]:
     if isinstance(val, int):
-        return AtomValueFact(FactStatus.APPROVED, 'int', {'value': val}),
+        return AtomValueFact(FactStatus.APPROVED, 'int', IntValue(val)),
     if isinstance(val, str):
-        return AtomValueFact(FactStatus.APPROVED, 'str', {'value': val}),
+        return AtomValueFact(FactStatus.APPROVED, 'str', StringValue(val)),
     if isinstance(val, float):
-        return AtomValueFact(FactStatus.APPROVED, 'float', {'value': val}),
+        return AtomValueFact(FactStatus.APPROVED, 'float', DoubleValue(val)),
     if isinstance(val, Iterable):
         return tuple(chain.from_iterable(generate_value(v) for v in val))
     raise ValueError
```

### Comparing `talisman-dm-1.0.0a5/tdm/v0/json_schema/convert/_nodes.py` & `talisman-dm-1.0.0a6/tdm/v0/json_schema/convert/_nodes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from collections import defaultdict
 from typing import Callable, Dict, List, Tuple
 
-from tdm.abstract.datamodel import AbstractNode, AbstractNodeLink, BaseNodeMetadata
+from tdm.abstract.datamodel import AbstractNode, AbstractNodeLink, BaseNodeMetadata, FrozenMarkup
 from tdm.datamodel.links import TranslationNodeLink
 from tdm.datamodel.mentions import NodeMention
 from tdm.datamodel.nodes import ImageNode, ImageNodeMetadata, JSONNode, KeyNode, ListNode, ListNodeMetadata, TableCellNode, \
     TableNode, TableRowNode, TableRowNodeMetadata, TextNode, TextNodeMetadata
 from tdm.v0.json_schema.content import NodeType, TreeDocumentContentModel
 
 
 def _convert_text_node(node: TreeDocumentContentModel) -> TextNode:
     return TextNode(
         content=node.text,
-        markup=node.markup.dict(),
+        markup=FrozenMarkup.freeze(node.markup.dict()),
         id=node.id,
         metadata=TextNodeMetadata(hidden=node.metadata.hidden, language=node.metadata.language)
     )
 
 
 def _covert_key_node(node: TreeDocumentContentModel) -> KeyNode:
     return KeyNode(
         content=node.text,
-        markup=node.markup.dict(),
+        markup=FrozenMarkup.freeze(node.markup.dict()),
         id=node.id,
         metadata=TextNodeMetadata(hidden=node.metadata.hidden, language=node.metadata.language)
     )
 
 
 def _convert_list_node(node: TreeDocumentContentModel) -> ListNode:
     return ListNode(id=node.id, metadata=ListNodeMetadata(hidden=node.metadata.hidden))
@@ -42,15 +42,15 @@
 def _convert_table_row_node(node: TreeDocumentContentModel) -> TableRowNode:
     return TableRowNode(id=node.id, metadata=TableRowNodeMetadata(hidden=node.metadata.hidden))
 
 
 def _convert_image_node(node: TreeDocumentContentModel) -> ImageNode:
     return ImageNode(
         content=node.text,
-        markup=node.markup.dict(),
+        markup=FrozenMarkup.freeze(node.markup.dict()),
         id=node.id,
         metadata=ImageNodeMetadata(hidden=node.metadata.hidden)
     )
 
 
 NODE_CONVERTERS: Dict[NodeType, Callable[[TreeDocumentContentModel], AbstractNode]] = {
     NodeType.HEADER: _convert_text_node,
```

### Comparing `talisman-dm-1.0.0a5/tdm/v0/json_schema/directive.py` & `talisman-dm-1.0.0a6/tdm/v0/json_schema/directive.py`

 * *Files identical despite different names*

### Comparing `talisman-dm-1.0.0a5/tdm/v0/json_schema/document.py` & `talisman-dm-1.0.0a6/tdm/v0/json_schema/document.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from collections import defaultdict
-from typing import Dict, Optional, Tuple
+from typing import Dict, Optional, Tuple, Type
 
 from pydantic import BaseModel
 
-from tdm.abstract.datamodel import AbstractFact, TalismanDocument
+from tdm.abstract.datamodel import AbstractFact, AbstractValue, TalismanDocument
 from tdm.datamodel.document import TalismanDocumentFactory
 from tdm.legacy import DocumentMetadataModel
 from .content import TreeDocumentContentModel
 from .convert import build_structure, convert_concept_fact, convert_property_fact, convert_relation_fact, convert_value_fact, \
     get_metadata_facts
 from .directive import DirectiveModel
 from .fact import ConceptFactModel, FactModel, FactType, PropertyFactModel, RelationFactModel, ValueFactModel
@@ -16,19 +16,19 @@
 class TalismanDocumentModel(BaseModel):
     id: str
     content: TreeDocumentContentModel
     metadata: Optional[DocumentMetadataModel]
     facts: Optional[Tuple[FactModel, ...]]  # pydantic fails to serialize FrozenSet[FactModel]
     directives: Optional[Tuple[DirectiveModel, ...]]
 
-    def to_doc(self, titles: Dict[str, Tuple[str, str]]) -> TalismanDocument:
+    def to_doc(self, titles: Dict[str, Tuple[str, str]], value_types: Dict[str, Type[AbstractValue]]) -> TalismanDocument:
         result = TalismanDocumentFactory.create_document(id_=self.id)
 
         nodes, structure, node_links = build_structure(self.content)
-        result = result.with_nodes(nodes).with_links(structure).with_node_links(node_links, update=True).with_main_root(self.content.id)
+        result = result.with_nodes(nodes).with_structure(structure).with_node_links(node_links, update=True).with_main_root(self.content.id)
 
         # convert document metadata to facts
         metadata = self.metadata.to_metadata() if self.metadata else {}
         result = result.with_metadata(metadata).with_facts(get_metadata_facts(self.id, metadata), update=True)
 
         # now convert facts
         old_facts = defaultdict(set)
@@ -39,24 +39,24 @@
         facts_mapping: dict[str, AbstractFact] = {}
 
         # start with concept facts
         # old concept fact consists of <status, type_id, value, mention> and should be converted to chain
         # ConceptFact(type_id) <- Property(Name) -> AtomValueFact(value) <-  MentionFact -> TextNodeMention(mention)
         for old_concept_fact in old_facts.get(FactType.CONCEPT, []):
             old_concept_fact: ConceptFactModel
-            concept_fact, *other = convert_concept_fact(old_concept_fact, result, titles)
+            concept_fact, *other = convert_concept_fact(old_concept_fact, result, titles, value_types)
             facts_mapping[old_concept_fact.id] = concept_fact
             facts.extend((concept_fact, *other))
 
         # then convert ValueFacts
         # old value fact consists of <status, type_id, value, mention> and should be converted to chain
         # AtomValueFact(value) <- MentionFact -> TextNodeMention(mention)
         for old_value_fact in old_facts.get(FactType.VALUE, []):
             old_value_fact: ValueFactModel
-            value_fact, *other = convert_value_fact(old_value_fact, result)
+            value_fact, *other = convert_value_fact(old_value_fact, result, value_types)
             facts_mapping[old_value_fact.id] = value_fact
             facts.extend((value_fact, *other))
 
         # now relations
         # old relations should be mapped to new ones with trivial modifications
         for old_relation_fact in old_facts.get(FactType.RELATION, []):
             old_relation_fact: RelationFactModel
```

### Comparing `talisman-dm-1.0.0a5/tdm/v0/json_schema/fact.py` & `talisman-dm-1.0.0a6/tdm/v0/json_schema/fact.py`

 * *Files identical despite different names*

