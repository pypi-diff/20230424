# Comparing `tmp/oarepo-model-builder-multilingual-2.0.6.tar.gz` & `tmp/oarepo-model-builder-multilingual-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-multilingual-2.0.6.tar", last modified: Wed Mar 29 08:13:44 2023, max compression
+gzip compressed data, was "oarepo-model-builder-multilingual-2.0.7.tar", last modified: Mon Apr 24 11:38:32 2023, max compression
```

## Comparing `oarepo-model-builder-multilingual-2.0.6.tar` & `oarepo-model-builder-multilingual-2.0.7.tar`

### file list

```diff
@@ -1,67 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:13:44.764251 oarepo-model-builder-multilingual-2.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-03-29 08:13:44.764251 oarepo-model-builder-multilingual-2.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:13:44.756251 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:13:44.760251 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/builders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/builders/mult_setup_cfg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:13:44.760251 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/builtin_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/builtin_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/builtin_models/i18n.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:13:44.760251 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/datatypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/datatypes/multilings.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/faker.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/i18n.json5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:13:44.760251 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/invenio/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/invenio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/invenio/invenio_multilingual_poetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/invenio/invenio_record_dumper_multilingual.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/invenio/invenio_search_multilingual.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:13:44.760251 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/invenio/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/invenio/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/invenio/templates/invenio_record_dumper_multilingual.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/invenio/templates/invenio_record_multilingual.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/invenio/templates/invenio_record_search_multilingual.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:13:44.760251 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/model_preprocessors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/model_preprocessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/model_preprocessors/multilingual.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/multilingual_jsonschema.json5
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/multilingual_settings.json5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:13:44.760251 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/property_preprocessors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/property_preprocessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/property_preprocessors/i18nStr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/property_preprocessors/multilingual.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/ui_jsonschema.json5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:13:44.760251 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/utils/supported_langs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:13:44.760251 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/validation/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:13:44.756251 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-03-29 08:13:44.000000 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-03-29 08:13:44.000000 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 08:13:44.000000 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-03-29 08:13:44.000000 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-29 08:13:44.000000 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-29 08:13:44.000000 oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-03-29 08:13:44.764251 oarepo-model-builder-multilingual-2.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:13:44.760251 oarepo-model-builder-multilingual-2.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/tests/mock_filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/tests/model.json5
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/tests/multilingual_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    12322 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/tests/test_build_from_entrypoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/tests/test_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/tests/test_i18nStr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/tests/test_marshmallow_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/tests/test_multi_facets.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/tests/test_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-03-29 08:12:59.000000 oarepo-model-builder-multilingual-2.0.6/tests/test_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:38:32.134138 oarepo-model-builder-multilingual-2.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-04-24 11:38:32.134138 oarepo-model-builder-multilingual-2.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:38:32.122138 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:38:32.126138 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/builders/mult_setup_cfg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:38:32.126138 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/builtin_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/builtin_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/builtin_models/i18n.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:38:32.126138 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/datatypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/datatypes/multilings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/faker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/i18n.json5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:38:32.126138 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/invenio/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/invenio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/invenio/invenio_multilingual_poetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/invenio/invenio_record_dumper_multilingual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/invenio/invenio_search_multilingual.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:38:32.126138 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/invenio/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/invenio/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/invenio/templates/invenio_record_dumper_multilingual.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/invenio/templates/invenio_record_multilingual.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/invenio/templates/invenio_record_search_multilingual.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:38:32.126138 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/model_preprocessors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/model_preprocessors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/model_preprocessors/multilingual.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/multilingual_jsonschema.json5
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/multilingual_settings.json5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:38:32.130138 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/property_preprocessors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/property_preprocessors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/property_preprocessors/i18nStr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/property_preprocessors/multilingual.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/ui_jsonschema.json5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:38:32.130138 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/utils/supported_langs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:38:32.130138 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:38:32.126138 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-04-24 11:38:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-04-24 11:38:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 11:38:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-24 11:38:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-24 11:38:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-24 11:38:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-24 11:38:32.134138 oarepo-model-builder-multilingual-2.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:38:32.130138 oarepo-model-builder-multilingual-2.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/tests/mock_filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/tests/model.json5
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/tests/multilingual_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10639 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/tests/test_build_from_entrypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/tests/test_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/tests/test_i18nStr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/tests/test_marshmallow_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/tests/test_multi_facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/tests/test_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/tests/test_ui.py
```

### Comparing `oarepo-model-builder-multilingual-2.0.6/LICENSE` & `oarepo-model-builder-multilingual-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.6/PKG-INFO` & `oarepo-model-builder-multilingual-2.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-multilingual
-Version: 2.0.6
+Version: 2.0.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
 # OARepo Model Builder Multilingual
 
 plugin for the [oarepo-model-builder module](https://github.com/oarepo/oarepo-model-builder) that adds support for
```

### Comparing `oarepo-model-builder-multilingual-2.0.6/README.md` & `oarepo-model-builder-multilingual-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/datatypes/multilings.py` & `oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/datatypes/multilings.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/faker.py` & `oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/faker.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/invenio/invenio_multilingual_poetry.py` & `oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/invenio/invenio_multilingual_poetry.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/invenio/invenio_record_dumper_multilingual.py` & `oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/invenio/invenio_record_dumper_multilingual.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/invenio/invenio_search_multilingual.py` & `oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/invenio/invenio_search_multilingual.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/invenio/templates/invenio_record_search_multilingual.py.jinja2` & `oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/invenio/templates/invenio_record_search_multilingual.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/model_preprocessors/multilingual.py` & `oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/model_preprocessors/multilingual.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/property_preprocessors/i18nStr.py` & `oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/property_preprocessors/i18nStr.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/property_preprocessors/multilingual.py` & `oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/property_preprocessors/multilingual.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/utils/supported_langs.py` & `oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/utils/supported_langs.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual/validation/__init__.py` & `oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual.egg-info/PKG-INFO` & `oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-multilingual
-Version: 2.0.6
+Version: 2.0.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
 # OARepo Model Builder Multilingual
 
 plugin for the [oarepo-model-builder module](https://github.com/oarepo/oarepo-model-builder) that adds support for
```

### Comparing `oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual.egg-info/SOURCES.txt` & `oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 oarepo_model_builder_multilingual/property_preprocessors/__init__.py
 oarepo_model_builder_multilingual/property_preprocessors/i18nStr.py
 oarepo_model_builder_multilingual/property_preprocessors/multilingual.py
 oarepo_model_builder_multilingual/utils/__init__.py
 oarepo_model_builder_multilingual/utils/supported_langs.py
 oarepo_model_builder_multilingual/validation/__init__.py
 tests/__init__.py
-tests/conftest.py
 tests/mock_filesystem.py
 tests/model.json5
 tests/multilingual_schema.py
 tests/test_build_from_entrypoints.py
 tests/test_cfg.py
 tests/test_helper.py
 tests/test_i18nStr.py
```

### Comparing `oarepo-model-builder-multilingual-2.0.6/oarepo_model_builder_multilingual.egg-info/entry_points.txt` & `oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.6/setup.cfg` & `oarepo-model-builder-multilingual-2.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-model-builder-multilingual
-version = 2.0.6
+version = 2.0.7
 description = 
 authors = ["Alzbeta Pokorna <alzbeta.pokorna@cesnet.cz>"]
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
```

### Comparing `oarepo-model-builder-multilingual-2.0.6/tests/mock_filesystem.py` & `oarepo-model-builder-multilingual-2.0.7/tests/mock_filesystem.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.6/tests/multilingual_schema.py` & `oarepo-model-builder-multilingual-2.0.7/tests/multilingual_schema.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.6/tests/test_build_from_entrypoints.py` & `oarepo-model-builder-multilingual-2.0.7/tests/test_build_from_entrypoints.py`

 * *Files 18% similar despite different names*

```diff
@@ -36,16 +36,16 @@
                         "lang": {"type": "string"},
                         "value": {"type": "string"},
                     },
                 },
                 "type": "array",
             },
             "id": {"type": "string"},
-            "created": {"type": "string", "format": "date"},
-            "updated": {"type": "string", "format": "date"},
+            "created": {"type": "string", "format": "date-time"},
+            "updated": {"type": "string", "format": "date-time"},
             "$schema": {"type": "string"},
         },
     }
 
 
 def test_mapping():
     schema = basic_schema()
@@ -163,85 +163,34 @@
 
     filesystem = MockFilesystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
     builder.build(schema, "")
 
     data = builder.filesystem.open(os.path.join("test", "records", "multilingual_dumper.py")).read()
+    print(data)
     assert re.sub(r"\s", "", data) == re.sub(
         r"\s",
         "",
         """
 
-from invenio_records.dumpers import SearchDumperExt
-from functools import reduce
-import operator
-from copy import deepcopy
-from deepmerge import always_merger
+from oarepo_runtime.i18n.dumper import MultilingualDumper
 
+class MultilingualSearchDumper(MultilingualDumper):
+    \"""TestRecord search dumper.\"""
 
-def getFromDict(dataDict, mapList):
-    return reduce(operator.getitem, mapList, dataDict)
+    paths = ['/a', '/b', '/c/d', '/c/f']
+    SUPPORTED_LANGS = ['cs', 'en']
 
-class MultilingualDumper(SearchDumperExt):
-    \"""TestRecord search dumper.\"""
     def dump(self, record, data):
-        paths = ['/a', '/b', '/c/d', '/c/f']
-        SUPPORTED_LANGS = ['cs', 'en']
-
-        for path in paths:
-            new_elements = {}
-            record2 = record
-            path_array = path.split('/')
-            path_array2 = []
-
-            for x in path_array:
-                path_array2.append(x)
-
-            path_array2.pop(0)
-            path_array2 = path_array2[:-1]
-
-            for x in path_array2:
-                record2 = record2[x]
-            path_array.pop(0)
-            multilingual_element = getFromDict(record, path_array)
-
-            for rec in multilingual_element:
-                if rec['lang'] in SUPPORTED_LANGS:
-                    el_name = path_array[-1]  + "_" + rec['lang']
-                    always_merger.merge(new_elements, {el_name: rec['value']})
-
-            always_merger.merge(record2, new_elements)
-        data.update(deepcopy(dict(record)))
-        return data
+        super().dump(record, data)
 
     def load(self, record, data):
-        paths = ['/a', '/b', '/c/d', '/c/f']
-        SUPPORTED_LANGS = ['cs', 'en']
-        for path in paths:
-            record2 = record
-            path_array = path.split('/')
-            path_array2 = []
-            for x in path_array:
-                path_array2.append(x)
-
-            path_array2.pop(0)
-            path_array2 = path_array2[:-1]
-
-            for x in path_array2:
-                record2 = record2[x]
-
-            path_array.pop(0)
-            multilingual_element = getFromDict(record, path_array)
-            for rec in multilingual_element:
-                if rec['lang'] in SUPPORTED_LANGS:
-                    el_name = path_array[-1]  + "_" + rec['lang']
-                    del record2[el_name]
-        return data
-    """,
+        super().load(record, data)
+""",
     )
 
 def test_generated_schema2():
     schema = load_model(
         "test.yaml",
         "test",
         model_content={
```

### Comparing `oarepo-model-builder-multilingual-2.0.6/tests/test_cfg.py` & `oarepo-model-builder-multilingual-2.0.7/tests/test_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.6/tests/test_helper.py` & `oarepo-model-builder-multilingual-2.0.7/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.6/tests/test_i18nStr.py` & `oarepo-model-builder-multilingual-2.0.7/tests/test_i18nStr.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.6/tests/test_marshmallow_ui.py` & `oarepo-model-builder-multilingual-2.0.7/tests/test_marshmallow_ui.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.6/tests/test_multi_facets.py` & `oarepo-model-builder-multilingual-2.0.7/tests/test_multi_facets.py`

 * *Files 14% similar despite different names*

```diff
@@ -46,20 +46,17 @@
 
     print(data)
     assert re.sub(r"\s", "", data) == re.sub(
         r"\s",
         "",
         """
 from invenio_records_resources.services import SearchOptions as InvenioSearchOptions
+from flask_babelex import lazy_gettext as _
 from . import facets
 
-def _(x):
-    \"""Identity function for string extraction.\"""
-    return x
-
 
 
 class TestSearchOptions(InvenioSearchOptions):
     \"""TestRecord search options.\"""
 
     facets = {
 
@@ -93,17 +90,17 @@
 
 
     '_schema': facets._schema,
 
 
     }
     sort_options = {
-
+        
         **InvenioSearchOptions.sort_options,
-
+        
 
 
     'a': {'fields': ['a']},"bestmatch": dict(
                 title=_('Best match'),
                 fields=['_score'],  # ES defaults to desc on `_score` field
             ),
             "newest": dict(
@@ -182,106 +179,119 @@
     print(data)
     assert re.sub(r"\s", "", data) == re.sub(
         r"\s",
         "",
         """
 \"""Facet definitions.\"""
 
-from invenio_records_resources.services.records.facets import TermsFacet
 from invenio_search.engine import dsl
+from flask_babelex import lazy_gettext as _
+
+
+
+from invenio_records_resources.services.records.facets import TermsFacet
+
+
+
+from oarepo_runtime.facets.date import DateTimeFacet
+
+
+
 from oarepo_runtime.facets.nested_facet import NestedLabeledFacet
 
 
 
 
-d_navic_kxh = NestedLabeledFacet(path ="d", nested_facet = TermsFacet(field="d.navic.kxh"))
+
+
+d_navic_kxh = NestedLabeledFacet(path ="d", nested_facet = TermsFacet(field="d.navic.kxh", label=_("d/navic/kxh.label")))
 
 
 
-d_lang = NestedLabeledFacet(path ="d", nested_facet = TermsFacet(field="d.lang"))
+d_lang = NestedLabeledFacet(path ="d", nested_facet = TermsFacet(field="d.lang", label=_("d/lang.label")))
 
 
 
 d_cs_keyword = TermsFacet(field="d_cs.keyword")
 
 
 
 d_en_keyword = TermsFacet(field="d_en.keyword")
 
 
 
-d_value_keyword = NestedLabeledFacet(path ="d", nested_facet = TermsFacet(field="d.value.keyword"))
+d_value_keyword = NestedLabeledFacet(path ="d", nested_facet = TermsFacet(field="d.value.keyword", label=_("d/value/keyword.label")))
 
 
 
-b = TermsFacet(field="b")
+b = TermsFacet(field="b", label=_("b.label"))
 
 
 
-c_language = NestedLabeledFacet(path ="c", nested_facet = TermsFacet(field="c.language"))
+c_language = NestedLabeledFacet(path ="c", nested_facet = TermsFacet(field="c.language", label=_("c/language.label")))
 
 
 
 c_cs_keyword = TermsFacet(field="c_cs.keyword")
 
 
 
 c_en_keyword = TermsFacet(field="c_en.keyword")
 
 
 
-c_value_keyword = NestedLabeledFacet(path ="c", nested_facet = TermsFacet(field="c.value.keyword"))
+c_value_keyword = NestedLabeledFacet(path ="c", nested_facet = TermsFacet(field="c.value.keyword", label=_("c/value/keyword.label")))
 
 
 
-a_lang = NestedLabeledFacet(path ="a", nested_facet = TermsFacet(field="a.lang"))
+a_lang = NestedLabeledFacet(path ="a", nested_facet = TermsFacet(field="a.lang", label=_("a/lang.label")))
 
 
 
 a_cs_keyword = TermsFacet(field="a_cs.keyword")
 
 
 
 a_en_keyword = TermsFacet(field="a_en.keyword")
 
 
 
-a_value_keyword = NestedLabeledFacet(path ="a", nested_facet = TermsFacet(field="a.value.keyword"))
+a_value_keyword = NestedLabeledFacet(path ="a", nested_facet = TermsFacet(field="a.value.keyword", label=_("a/value/keyword.label")))
 
 
 
-e_f = TermsFacet(field="e.f")
+e_f = TermsFacet(field="e.f", label=_("e/f.label"))
 
 
 
-e_g_lang = NestedLabeledFacet(path ="e.g", nested_facet = TermsFacet(field="e.g.lang"))
+e_g_lang = NestedLabeledFacet(path ="e.g", nested_facet = TermsFacet(field="e.g.lang", label=_("e/g/lang.label")))
 
 
 
 e_g_cs_keyword = TermsFacet(field="e.g_cs.keyword")
 
 
 
 e_g_en_keyword = TermsFacet(field="e.g_en.keyword")
 
 
 
-e_g_value_keyword = NestedLabeledFacet(path ="e.g", nested_facet = TermsFacet(field="e.g.value.keyword"))
+e_g_value_keyword = NestedLabeledFacet(path ="e.g", nested_facet = TermsFacet(field="e.g.value.keyword", label=_("e/g/value/keyword.label")))
 
 
 
-_id = TermsFacet(field="id")
+_id = TermsFacet(field="id", label=_("id.label"))
 
 
 
-created = TermsFacet(field="created")
+created = DateTimeFacet(field="created", label=_("created.label"))
 
 
 
-updated = TermsFacet(field="updated")
+updated = DateTimeFacet(field="updated", label=_("updated.label"))
 
 
 
-_schema = TermsFacet(field="$schema")
+_schema = TermsFacet(field="$schema", label=_("$schema.label"))
 
     """,
     )
```

### Comparing `oarepo-model-builder-multilingual-2.0.6/tests/test_runtime.py` & `oarepo-model-builder-multilingual-2.0.7/tests/test_runtime.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.6/tests/test_schema.py` & `oarepo-model-builder-multilingual-2.0.7/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.6/tests/test_ui.py` & `oarepo-model-builder-multilingual-2.0.7/tests/test_ui.py`

 * *Files identical despite different names*

