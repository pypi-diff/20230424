# Comparing `tmp/dff-0.3.2.tar.gz` & `tmp/dff-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dff-0.3.2.tar", last modified: Mon Feb 20 13:29:53 2023, max compression
+gzip compressed data, was "dff-0.4.1.tar", last modified: Mon Apr 24 14:28:32 2023, max compression
```

## Comparing `dff-0.3.2.tar` & `dff-0.4.1.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 13:29:53.390693 dff-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-02-20 13:29:40.000000 dff-0.3.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11434 2023-02-20 13:29:40.000000 dff-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-02-20 13:29:40.000000 dff-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7357 2023-02-20 13:29:53.390693 dff-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-02-20 13:29:40.000000 dff-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 13:29:53.374693 dff-0.3.2/dff/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-02-20 13:29:40.000000 dff-0.3.2/dff/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 13:29:53.378693 dff-0.3.2/dff/context_storages/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-02-20 13:29:40.000000 dff-0.3.2/dff/context_storages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-02-20 13:29:40.000000 dff-0.3.2/dff/context_storages/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-02-20 13:29:40.000000 dff-0.3.2/dff/context_storages/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-02-20 13:29:40.000000 dff-0.3.2/dff/context_storages/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-02-20 13:29:40.000000 dff-0.3.2/dff/context_storages/pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-02-20 13:29:40.000000 dff-0.3.2/dff/context_storages/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-02-20 13:29:40.000000 dff-0.3.2/dff/context_storages/protocols.json
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-02-20 13:29:40.000000 dff-0.3.2/dff/context_storages/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-02-20 13:29:40.000000 dff-0.3.2/dff/context_storages/shelve.py
--rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-02-20 13:29:40.000000 dff-0.3.2/dff/context_storages/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-02-20 13:29:40.000000 dff-0.3.2/dff/context_storages/ydb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 13:29:53.378693 dff-0.3.2/dff/messengers/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-20 13:29:40.000000 dff-0.3.2/dff/messengers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 13:29:53.382693 dff-0.3.2/dff/messengers/common/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-02-20 13:29:40.000000 dff-0.3.2/dff/messengers/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-02-20 13:29:40.000000 dff-0.3.2/dff/messengers/common/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-02-20 13:29:40.000000 dff-0.3.2/dff/messengers/common/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 13:29:53.382693 dff-0.3.2/dff/messengers/telegram/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-02-20 13:29:40.000000 dff-0.3.2/dff/messengers/telegram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8779 2023-02-20 13:29:40.000000 dff-0.3.2/dff/messengers/telegram/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-02-20 13:29:40.000000 dff-0.3.2/dff/messengers/telegram/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     9523 2023-02-20 13:29:40.000000 dff-0.3.2/dff/messengers/telegram/messenger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-02-20 13:29:40.000000 dff-0.3.2/dff/messengers/telegram/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 13:29:53.382693 dff-0.3.2/dff/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-02-20 13:29:40.000000 dff-0.3.2/dff/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-02-20 13:29:40.000000 dff-0.3.2/dff/pipeline/conditions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 13:29:53.382693 dff-0.3.2/dff/pipeline/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-20 13:29:40.000000 dff-0.3.2/dff/pipeline/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11296 2023-02-20 13:29:40.000000 dff-0.3.2/dff/pipeline/pipeline/component.py
--rw-r--r--   0 runner    (1001) docker     (123)    11778 2023-02-20 13:29:40.000000 dff-0.3.2/dff/pipeline/pipeline/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-02-20 13:29:40.000000 dff-0.3.2/dff/pipeline/pipeline/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 13:29:53.382693 dff-0.3.2/dff/pipeline/service/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-20 13:29:40.000000 dff-0.3.2/dff/pipeline/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-02-20 13:29:40.000000 dff-0.3.2/dff/pipeline/service/extra.py
--rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-02-20 13:29:40.000000 dff-0.3.2/dff/pipeline/service/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-02-20 13:29:40.000000 dff-0.3.2/dff/pipeline/service/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-02-20 13:29:40.000000 dff-0.3.2/dff/pipeline/service/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-02-20 13:29:40.000000 dff-0.3.2/dff/pipeline/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 13:29:53.386693 dff-0.3.2/dff/script/
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-02-20 13:29:40.000000 dff-0.3.2/dff/script/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 13:29:53.386693 dff-0.3.2/dff/script/conditions/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-02-20 13:29:40.000000 dff-0.3.2/dff/script/conditions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7711 2023-02-20 13:29:40.000000 dff-0.3.2/dff/script/conditions/std_conditions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 13:29:53.386693 dff-0.3.2/dff/script/core/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-20 13:29:40.000000 dff-0.3.2/dff/script/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19658 2023-02-20 13:29:40.000000 dff-0.3.2/dff/script/core/actor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-02-20 13:29:40.000000 dff-0.3.2/dff/script/core/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-02-20 13:29:40.000000 dff-0.3.2/dff/script/core/keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-02-20 13:29:40.000000 dff-0.3.2/dff/script/core/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-02-20 13:29:40.000000 dff-0.3.2/dff/script/core/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-02-20 13:29:40.000000 dff-0.3.2/dff/script/core/script.py
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-02-20 13:29:40.000000 dff-0.3.2/dff/script/core/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 13:29:53.386693 dff-0.3.2/dff/script/extras/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-20 13:29:40.000000 dff-0.3.2/dff/script/extras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 13:29:53.386693 dff-0.3.2/dff/script/extras/conditions/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-20 13:29:40.000000 dff-0.3.2/dff/script/extras/conditions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 13:29:53.386693 dff-0.3.2/dff/script/extras/slots/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-20 13:29:40.000000 dff-0.3.2/dff/script/extras/slots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 13:29:53.386693 dff-0.3.2/dff/script/labels/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-02-20 13:29:40.000000 dff-0.3.2/dff/script/labels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-02-20 13:29:40.000000 dff-0.3.2/dff/script/labels/std_labels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 13:29:53.386693 dff-0.3.2/dff/script/responses/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-02-20 13:29:40.000000 dff-0.3.2/dff/script/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-02-20 13:29:40.000000 dff-0.3.2/dff/script/responses/std_responses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 13:29:53.386693 dff-0.3.2/dff/stats/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-20 13:29:40.000000 dff-0.3.2/dff/stats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 13:29:53.386693 dff-0.3.2/dff/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-20 13:29:40.000000 dff-0.3.2/dff/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 13:29:53.390693 dff-0.3.2/dff/utils/parser/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-20 13:29:40.000000 dff-0.3.2/dff/utils/parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 13:29:53.390693 dff-0.3.2/dff/utils/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-02-20 13:29:40.000000 dff-0.3.2/dff/utils/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-02-20 13:29:40.000000 dff-0.3.2/dff/utils/testing/cleanup_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-02-20 13:29:40.000000 dff-0.3.2/dff/utils/testing/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-02-20 13:29:40.000000 dff-0.3.2/dff/utils/testing/response_comparers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12924 2023-02-20 13:29:40.000000 dff-0.3.2/dff/utils/testing/telegram.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-02-20 13:29:40.000000 dff-0.3.2/dff/utils/testing/toy_script.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 13:29:53.390693 dff-0.3.2/dff/utils/turn_caching/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-02-20 13:29:40.000000 dff-0.3.2/dff/utils/turn_caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-02-20 13:29:40.000000 dff-0.3.2/dff/utils/turn_caching/singleton_turn_caching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 13:29:53.390693 dff-0.3.2/dff/utils/viewer/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-20 13:29:40.000000 dff-0.3.2/dff/utils/viewer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 13:29:53.378693 dff-0.3.2/dff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7357 2023-02-20 13:29:53.000000 dff-0.3.2/dff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-02-20 13:29:53.000000 dff-0.3.2/dff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 13:29:53.000000 dff-0.3.2/dff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-02-20 13:29:53.000000 dff-0.3.2/dff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-20 13:29:53.000000 dff-0.3.2/dff.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 13:29:53.390693 dff-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-02-20 13:29:40.000000 dff-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.730352 dff-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-04-24 14:28:18.000000 dff-0.4.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11434 2023-04-24 14:28:18.000000 dff-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-24 14:28:18.000000 dff-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7341 2023-04-24 14:28:32.730352 dff-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-04-24 14:28:18.000000 dff-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.722352 dff-0.4.1/dff/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-24 14:28:18.000000 dff-0.4.1/dff/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.722352 dff-0.4.1/dff/context_storages/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-24 14:28:18.000000 dff-0.4.1/dff/context_storages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-04-24 14:28:18.000000 dff-0.4.1/dff/context_storages/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-24 14:28:18.000000 dff-0.4.1/dff/context_storages/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-04-24 14:28:18.000000 dff-0.4.1/dff/context_storages/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-24 14:28:18.000000 dff-0.4.1/dff/context_storages/pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-24 14:28:18.000000 dff-0.4.1/dff/context_storages/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-24 14:28:18.000000 dff-0.4.1/dff/context_storages/protocols.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-24 14:28:18.000000 dff-0.4.1/dff/context_storages/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-04-24 14:28:18.000000 dff-0.4.1/dff/context_storages/shelve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-04-24 14:28:18.000000 dff-0.4.1/dff/context_storages/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-04-24 14:28:18.000000 dff-0.4.1/dff/context_storages/ydb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.722352 dff-0.4.1/dff/messengers/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-24 14:28:18.000000 dff-0.4.1/dff/messengers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.726352 dff-0.4.1/dff/messengers/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-24 14:28:18.000000 dff-0.4.1/dff/messengers/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-04-24 14:28:18.000000 dff-0.4.1/dff/messengers/common/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-24 14:28:18.000000 dff-0.4.1/dff/messengers/common/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.726352 dff-0.4.1/dff/messengers/telegram/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-24 14:28:18.000000 dff-0.4.1/dff/messengers/telegram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9508 2023-04-24 14:28:18.000000 dff-0.4.1/dff/messengers/telegram/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-04-24 14:28:18.000000 dff-0.4.1/dff/messengers/telegram/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9544 2023-04-24 14:28:18.000000 dff-0.4.1/dff/messengers/telegram/messenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-24 14:28:18.000000 dff-0.4.1/dff/messengers/telegram/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.726352 dff-0.4.1/dff/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-24 14:28:18.000000 dff-0.4.1/dff/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-04-24 14:28:18.000000 dff-0.4.1/dff/pipeline/conditions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.726352 dff-0.4.1/dff/pipeline/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-24 14:28:18.000000 dff-0.4.1/dff/pipeline/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18667 2023-04-24 14:28:18.000000 dff-0.4.1/dff/pipeline/pipeline/actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11179 2023-04-24 14:28:18.000000 dff-0.4.1/dff/pipeline/pipeline/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17635 2023-04-24 14:28:18.000000 dff-0.4.1/dff/pipeline/pipeline/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-04-24 14:28:18.000000 dff-0.4.1/dff/pipeline/pipeline/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.726352 dff-0.4.1/dff/pipeline/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-24 14:28:18.000000 dff-0.4.1/dff/pipeline/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-04-24 14:28:18.000000 dff-0.4.1/dff/pipeline/service/extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-04-24 14:28:18.000000 dff-0.4.1/dff/pipeline/service/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8720 2023-04-24 14:28:18.000000 dff-0.4.1/dff/pipeline/service/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-24 14:28:18.000000 dff-0.4.1/dff/pipeline/service/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-04-24 14:28:18.000000 dff-0.4.1/dff/pipeline/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.726352 dff-0.4.1/dff/script/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-24 14:28:18.000000 dff-0.4.1/dff/script/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.726352 dff-0.4.1/dff/script/conditions/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-24 14:28:18.000000 dff-0.4.1/dff/script/conditions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-04-24 14:28:18.000000 dff-0.4.1/dff/script/conditions/std_conditions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.730352 dff-0.4.1/dff/script/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-24 14:28:18.000000 dff-0.4.1/dff/script/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11920 2023-04-24 14:28:18.000000 dff-0.4.1/dff/script/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-04-24 14:28:18.000000 dff-0.4.1/dff/script/core/keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-04-24 14:28:18.000000 dff-0.4.1/dff/script/core/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-04-24 14:28:18.000000 dff-0.4.1/dff/script/core/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-04-24 14:28:18.000000 dff-0.4.1/dff/script/core/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-24 14:28:18.000000 dff-0.4.1/dff/script/core/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.730352 dff-0.4.1/dff/script/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-24 14:28:18.000000 dff-0.4.1/dff/script/extras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.730352 dff-0.4.1/dff/script/extras/conditions/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-24 14:28:18.000000 dff-0.4.1/dff/script/extras/conditions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.730352 dff-0.4.1/dff/script/extras/slots/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-24 14:28:18.000000 dff-0.4.1/dff/script/extras/slots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.730352 dff-0.4.1/dff/script/labels/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-24 14:28:18.000000 dff-0.4.1/dff/script/labels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-04-24 14:28:18.000000 dff-0.4.1/dff/script/labels/std_labels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.730352 dff-0.4.1/dff/script/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-24 14:28:18.000000 dff-0.4.1/dff/script/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-24 14:28:18.000000 dff-0.4.1/dff/script/responses/std_responses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.730352 dff-0.4.1/dff/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-24 14:28:18.000000 dff-0.4.1/dff/stats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.730352 dff-0.4.1/dff/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-24 14:28:18.000000 dff-0.4.1/dff/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.730352 dff-0.4.1/dff/utils/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-24 14:28:18.000000 dff-0.4.1/dff/utils/parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.730352 dff-0.4.1/dff/utils/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-24 14:28:18.000000 dff-0.4.1/dff/utils/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-24 14:28:18.000000 dff-0.4.1/dff/utils/testing/cleanup_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-24 14:28:18.000000 dff-0.4.1/dff/utils/testing/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-24 14:28:18.000000 dff-0.4.1/dff/utils/testing/response_comparers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12929 2023-04-24 14:28:18.000000 dff-0.4.1/dff/utils/testing/telegram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-24 14:28:18.000000 dff-0.4.1/dff/utils/testing/toy_script.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.730352 dff-0.4.1/dff/utils/turn_caching/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-24 14:28:18.000000 dff-0.4.1/dff/utils/turn_caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-24 14:28:18.000000 dff-0.4.1/dff/utils/turn_caching/singleton_turn_caching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.730352 dff-0.4.1/dff/utils/viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-24 14:28:18.000000 dff-0.4.1/dff/utils/viewer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:32.722352 dff-0.4.1/dff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7341 2023-04-24 14:28:32.000000 dff-0.4.1/dff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-24 14:28:32.000000 dff-0.4.1/dff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 14:28:32.000000 dff-0.4.1/dff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-04-24 14:28:32.000000 dff-0.4.1/dff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-24 14:28:32.000000 dff-0.4.1/dff.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 14:28:32.730352 dff-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-04-24 14:28:18.000000 dff-0.4.1/setup.py
```

### Comparing `dff-0.3.2/CONTRIBUTING.md` & `dff-0.4.1/CONTRIBUTING.md`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,18 @@
 to annotate your modules and objects. You can easily build the Sphinx documentation for your module 
 by activating the virtual environment and then running
 
 ```bash
 make doc
 ```
 
-After that `docs/build` dir will be created and you can open index file `docs/build/index.html` in your browser of choice.
+After that `docs/build` dir will be created and you can open index file `docs/build/index.html` in your browser of choice.  
+WARNING! Because of the current patching solution, `make doc` modifies some of the source library code (`nbsphinx` and `autosummary`),
+so it is strongly advised to use it carefully and in virtual environment only.
+However, this behavior is likely to be changed in the future.
 
 ### Style
 For style supporting we propose `black`, which is a PEP 8 compliant opinionated formatter.
 It doesn't take previous formatting into account. See more about [black](https://github.com/psf/black). 
 To format your code, run
 
 ```bash
```

### Comparing `dff-0.3.2/LICENSE` & `dff-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dff-0.3.2/PKG-INFO` & `dff-0.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dff
-Version: 0.3.2
+Version: 0.4.1
 Summary: The Dialog Flow Framework (DFF) allows you to write conversational services.
 Home-page: https://github.com/deeppavlov/dialog_flow_framework
 Author: Denis Kuznetsov
 Author-email: kuznetsov.den.p@gmail.com
 Keywords: chatbots
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -27,15 +27,15 @@
 Provides-Extra: mysql
 Provides-Extra: postgresql
 Provides-Extra: ydb
 Provides-Extra: telegram
 Provides-Extra: full
 Provides-Extra: tests
 Provides-Extra: test_full
-Provides-Extra: examples
+Provides-Extra: tutorials
 Provides-Extra: devel
 Provides-Extra: doc
 Provides-Extra: devel_full
 License-File: LICENSE
 
 
 # Dialog Flow Framework
@@ -62,41 +62,45 @@
 pip install dff
 ```
 
 The above command will set the minimum dependencies to start working with DFF.
 The installation process allows the user to choose from different packages based on their dependencies, which are:
 ```bash
 pip install dff[core]  # minimal dependencies (by default)
+pip install dff[json]  # dependencies for using JSON
+pip install dff[pickle] # dependencies for using Pickle
 pip install dff[redis]  # dependencies for using Redis
 pip install dff[mongodb]  # dependencies for using MongoDB
 pip install dff[mysql]  # dependencies for using MySQL
 pip install dff[postgresql]  # dependencies for using PostgreSQL
 pip install dff[sqlite]  # dependencies for using SQLite
 pip install dff[ydb]  # dependencies for using Yandex Database
+pip install dff[telegram]  # dependencies for using Telegram
 pip install dff[full]  # full dependencies including all options above
 pip install dff[tests]  # dependencies for running tests
 pip install dff[test_full]  # full dependencies for running all tests (all options above)
-pip install dff[examples]  # dependencies for running examples (all options above)
+pip install dff[tutorials]  # dependencies for running tutorials (all options above)
 pip install dff[devel]  # dependencies for development
 pip install dff[doc]  # dependencies for documentation
 pip install dff[devel_full]  # full dependencies for development (all options above)
 ```
 
 For example, if you are going to use one of the database backends,
 you can specify the corresponding requirements yourself. Multiple dependencies can be installed at once, e.g.
 ```bash
 pip install dff[postgresql, mysql]
 ```
 
 ## Basic example
 
 ```python
-from dff.script import GLOBAL, TRANSITIONS, RESPONSE, Context, Actor, Message
+from dff.script import GLOBAL, TRANSITIONS, RESPONSE, Context, Message
+from dff.pipeline import Pipeline
 import dff.script.conditions.std_conditions as cnd
-from typing import Union
+from typing import Tuple
 
 # create a dialog script
 script = {
 GLOBAL: {
 TRANSITIONS: {
 ("flow", "node_hi"): cnd.exact_match(Message(text="Hi")),
 ("flow", "node_ok"): cnd.true()
@@ -104,36 +108,31 @@
 },
 "flow": {
 "node_hi": {RESPONSE: Message(text="Hi!!!")},
 "node_ok": {RESPONSE: Message(text="Okey")},
 },
 }
 
-# init actor
-actor = Actor(script, start_label=("flow", "node_hi"))
+# init pipeline
+pipeline = Pipeline.from_script(script, start_label=("flow", "node_hi"))
 
 
 # handler requests
-def turn_handler(in_request: Message, ctx: Union[Context, dict], actor: Actor):
-# Context.cast - gets an object type of [Context, str, dict] returns an object type of Context
-ctx = Context.cast(ctx)
-# Add in current context a next request of user
-ctx.add_request(in_request)
-# Pass the context into actor and it returns updated context with actor response
-ctx = actor(ctx)
+def turn_handler(in_request: Message, pipeline: Pipeline) -> Tuple[Message, Context]:
+# Pass the next request of user into pipeline and it returns updated context with actor response
+ctx = pipeline(in_request, 0)
 # Get last actor response from the context
 out_response = ctx.last_response
 # The next condition branching needs for testing
 return out_response, ctx
 
 
-ctx = {}
 while True:
 in_request = input("type your answer: ")
-out_response, ctx = turn_handler(Message(text=in_request), ctx, actor)
+out_response, ctx = turn_handler(Message(text=in_request), pipeline)
 print(out_response.text)
 ```
 
 When you run this code, you get similar output:
 ```
 type your answer: hi
 Okey
@@ -142,15 +141,15 @@
 type your answer: ok
 Okey
 type your answer: ok
 Okey
 ```
 
 To get more advanced examples, take a look at
-[examples](https://github.com/deeppavlov/dialog_flow_framework/tree/dev/examples) on GitHub.
+[tutorials](https://github.com/deeppavlov/dialog_flow_framework/tree/dev/tutorials) on GitHub.
 
 # Context Storages
 ## Description
 
 Context Storages allow you to save and retrieve user dialogue states
 (in the form of a `Context` object) using various database backends.
 
@@ -167,35 +166,30 @@
 
 Aside from this, we offer some interfaces for saving data to your local file system.
 These are not meant to be used in production, but can be helpful for prototyping your application.
 
 ## Basic example
 
 ```python
-from dff.script import Context, Actor
+from dff.script import Context
+from dff.pipeline import Pipeline
 from dff.context_storages import SQLContextStorage
 from .script import some_df_script
 
 db = SQLContextStorage("postgresql+asyncpg://user:password@host:port/dbname")
 
-actor = Actor(some_df_script, start_label=("root", "start"), fallback_label=("root", "fallback"))
+pipeline = Pipeline.from_script(some_df_script, start_label=("root", "start"), fallback_label=("root", "fallback"))
 
 
 def handle_request(request):
 user_id = request.args["user_id"]
-if user_id not in db:
-context = Context(id=user_id)
-else:
-context = db[user_id]
-new_context = actor(context)
-db[user_id] = new_context
-assert user_id in db
+new_context = pipeline(request, user_id)
 return new_context.last_response
 
 ```
 
 To get more advanced examples, take a look at
-[examples](https://github.com/deeppavlov/dialog_flow_framework/tree/dev/examples/context_storages) on GitHub.
+[tutorials](https://github.com/deeppavlov/dialog_flow_framework/tree/dev/tutorials/context_storages) on GitHub.
 
 # Contributing to the Dialog Flow Framework
 
 Please refer to [CONTRIBUTING.md](https://github.com/deeppavlov/dialog_flow_framework/blob/dev/CONTRIBUTING.md).
```

### Comparing `dff-0.3.2/README.md` & `dff-0.4.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -23,41 +23,45 @@
 pip install dff
 ```
 
 The above command will set the minimum dependencies to start working with DFF. 
 The installation process allows the user to choose from different packages based on their dependencies, which are:
 ```bash
 pip install dff[core]  # minimal dependencies (by default)
+pip install dff[json]  # dependencies for using JSON
+pip install dff[pickle] # dependencies for using Pickle
 pip install dff[redis]  # dependencies for using Redis
 pip install dff[mongodb]  # dependencies for using MongoDB
 pip install dff[mysql]  # dependencies for using MySQL
 pip install dff[postgresql]  # dependencies for using PostgreSQL
 pip install dff[sqlite]  # dependencies for using SQLite
 pip install dff[ydb]  # dependencies for using Yandex Database
+pip install dff[telegram]  # dependencies for using Telegram
 pip install dff[full]  # full dependencies including all options above
 pip install dff[tests]  # dependencies for running tests
 pip install dff[test_full]  # full dependencies for running all tests (all options above)
-pip install dff[examples]  # dependencies for running examples (all options above)
+pip install dff[tutorials]  # dependencies for running tutorials (all options above)
 pip install dff[devel]  # dependencies for development
 pip install dff[doc]  # dependencies for documentation
 pip install dff[devel_full]  # full dependencies for development (all options above)
 ```
 
 For example, if you are going to use one of the database backends,
 you can specify the corresponding requirements yourself. Multiple dependencies can be installed at once, e.g.
 ```bash
 pip install dff[postgresql, mysql]
 ```
 
 ## Basic example
 
 ```python
-from dff.script import GLOBAL, TRANSITIONS, RESPONSE, Context, Actor, Message
+from dff.script import GLOBAL, TRANSITIONS, RESPONSE, Context, Message
+from dff.pipeline import Pipeline
 import dff.script.conditions.std_conditions as cnd
-from typing import Union
+from typing import Tuple
 
 # create a dialog script
 script = {
     GLOBAL: {
         TRANSITIONS: {
             ("flow", "node_hi"): cnd.exact_match(Message(text="Hi")),
             ("flow", "node_ok"): cnd.true()
@@ -65,36 +69,31 @@
     },
     "flow": {
         "node_hi": {RESPONSE: Message(text="Hi!!!")},
         "node_ok": {RESPONSE: Message(text="Okey")},
     },
 }
 
-# init actor
-actor = Actor(script, start_label=("flow", "node_hi"))
+# init pipeline
+pipeline = Pipeline.from_script(script, start_label=("flow", "node_hi"))
 
 
 # handler requests
-def turn_handler(in_request: Message, ctx: Union[Context, dict], actor: Actor):
-    # Context.cast - gets an object type of [Context, str, dict] returns an object type of Context
-    ctx = Context.cast(ctx)
-    # Add in current context a next request of user
-    ctx.add_request(in_request)
-    # Pass the context into actor and it returns updated context with actor response
-    ctx = actor(ctx)
+def turn_handler(in_request: Message, pipeline: Pipeline) -> Tuple[Message, Context]:
+    # Pass the next request of user into pipeline and it returns updated context with actor response
+    ctx = pipeline(in_request, 0)
     # Get last actor response from the context
     out_response = ctx.last_response
     # The next condition branching needs for testing
     return out_response, ctx
 
 
-ctx = {}
 while True:
     in_request = input("type your answer: ")
-    out_response, ctx = turn_handler(Message(text=in_request), ctx, actor)
+    out_response, ctx = turn_handler(Message(text=in_request), pipeline)
     print(out_response.text)
 ```
 
 When you run this code, you get similar output:
 ```
 type your answer: hi
 Okey
@@ -103,15 +102,15 @@
 type your answer: ok
 Okey
 type your answer: ok
 Okey
 ```
 
 To get more advanced examples, take a look at
-[examples](https://github.com/deeppavlov/dialog_flow_framework/tree/dev/examples) on GitHub.
+[tutorials](https://github.com/deeppavlov/dialog_flow_framework/tree/dev/tutorials) on GitHub.
 
 # Context Storages
 ## Description
 
 Context Storages allow you to save and retrieve user dialogue states
 (in the form of a `Context` object) using various database backends. 
 
@@ -128,35 +127,30 @@
 
 Aside from this, we offer some interfaces for saving data to your local file system.
 These are not meant to be used in production, but can be helpful for prototyping your application.
 
 ## Basic example
 
 ```python
-from dff.script import Context, Actor
+from dff.script import Context
+from dff.pipeline import Pipeline
 from dff.context_storages import SQLContextStorage
 from .script import some_df_script
 
 db = SQLContextStorage("postgresql+asyncpg://user:password@host:port/dbname")
 
-actor = Actor(some_df_script, start_label=("root", "start"), fallback_label=("root", "fallback"))
+pipeline = Pipeline.from_script(some_df_script, start_label=("root", "start"), fallback_label=("root", "fallback"))
 
 
 def handle_request(request):
     user_id = request.args["user_id"]
-    if user_id not in db:
-        context = Context(id=user_id)
-    else:
-        context = db[user_id]
-    new_context = actor(context)
-    db[user_id] = new_context
-    assert user_id in db
+    new_context = pipeline(request, user_id)
     return new_context.last_response
 
 ```
 
 To get more advanced examples, take a look at
-[examples](https://github.com/deeppavlov/dialog_flow_framework/tree/dev/examples/context_storages) on GitHub.
+[tutorials](https://github.com/deeppavlov/dialog_flow_framework/tree/dev/tutorials/context_storages) on GitHub.
 
 # Contributing to the Dialog Flow Framework
 
-Please refer to [CONTRIBUTING.md](https://github.com/deeppavlov/dialog_flow_framework/blob/dev/CONTRIBUTING.md).
+Please refer to [CONTRIBUTING.md](https://github.com/deeppavlov/dialog_flow_framework/blob/dev/CONTRIBUTING.md).
```

### Comparing `dff-0.3.2/dff/context_storages/__init__.py` & `dff-0.4.1/dff/context_storages/__init__.py`

 * *Files identical despite different names*

### Comparing `dff-0.3.2/dff/context_storages/database.py` & `dff-0.4.1/dff/context_storages/database.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from typing import Callable, Hashable, Optional
 
 from .protocol import PROTOCOLS
 from ..script import Context
 
 
 class DBContextStorage(ABC):
-    """
+    r"""
     An abstract interface for `dff` DB context storages.
     It includes the most essential methods of the python `dict` class.
     Can not be instantiated.
 
     :param path: Parameter `path` should be set with the URI of the database.
         It includes a prefix and the required connection credentials.
         Example: postgresql+asyncpg://user:password@host:port/database
@@ -44,25 +44,25 @@
         """Threading for methods that require single thread access."""
 
     def __getitem__(self, key: Hashable) -> Context:
         """
         Synchronous method for accessing stored Context.
 
         :param key: Hashable key used to store Context instance.
-        :returns: The stored context, associated with the given key.
+        :return: The stored context, associated with the given key.
         """
         return asyncio.run(self.get_item_async(key))
 
     @abstractmethod
     async def get_item_async(self, key: Hashable) -> Context:
         """
         Asynchronous method for accessing stored Context.
 
         :param key: Hashable key used to store Context instance.
-        :returns: The stored context, associated with the given key.
+        :return: The stored context, associated with the given key.
         """
         raise NotImplementedError
 
     def __setitem__(self, key: Hashable, value: Context):
         """
         Synchronous method for storing Context.
 
@@ -99,62 +99,62 @@
         raise NotImplementedError
 
     def __contains__(self, key: Hashable) -> bool:
         """
         Synchronous method for finding whether any Context is stored with given key.
 
         :param key: Hashable key used to check if Context instance is stored.
-        :returns: True if there is Context accessible by given key, False otherwise.
+        :return: True if there is Context accessible by given key, False otherwise.
         """
         return asyncio.run(self.contains_async(key))
 
     @abstractmethod
     async def contains_async(self, key: Hashable) -> bool:
         """
         Asynchronous method for finding whether any Context is stored with given key.
 
         :param key: Hashable key used to check if Context instance is stored.
-        :returns: True if there is Context accessible by given key, False otherwise.
+        :return: True if there is Context accessible by given key, False otherwise.
         """
         raise NotImplementedError
 
     def __len__(self) -> int:
         """
         Synchronous method for retrieving number of stored Contexts.
 
-        :returns: The number of stored Contexts.
+        :return: The number of stored Contexts.
         """
         return asyncio.run(self.len_async())
 
     @abstractmethod
     async def len_async(self) -> int:
         """
         Asynchronous method for retrieving number of stored Contexts.
 
-        :returns: The number of stored Contexts.
+        :return: The number of stored Contexts.
         """
         raise NotImplementedError
 
     def get(self, key: Hashable, default: Optional[Context] = None) -> Context:
         """
         Synchronous method for accessing stored Context, returning default if no Context is stored with the given key.
 
         :param key: Hashable key used to store Context instance.
         :param default: Optional default value to be returned if no Context is found.
-        :returns: The stored context, associated with the given key or default value.
+        :return: The stored context, associated with the given key or default value.
         """
         return asyncio.run(self.get_async(key, default))
 
     async def get_async(self, key: Hashable, default: Optional[Context] = None) -> Context:
         """
         Asynchronous method for accessing stored Context, returning default if no Context is stored with the given key.
 
         :param key: Hashable key used to store Context instance.
         :param default: Optional default value to be returned if no Context is found.
-        :returns: The stored context, associated with the given key or default value.
+        :return: The stored context, associated with the given key or default value.
         """
         try:
             return await self.get_item_async(str(key))
         except KeyError:
             return default
 
     def clear(self):
```

### Comparing `dff-0.3.2/dff/context_storages/json.py` & `dff-0.4.1/dff/context_storages/json.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 JSON
 ----
 The JSON module provides a json-based version of the :py:class:`.DBContextStorage` class.
-This class is used to store and retrieve context data in a JSON. It allows the `DFF` to easily
+This class is used to store and retrieve context data in a JSON. It allows the DFF to easily
 store and retrieve context data.
 """
 import asyncio
 from typing import Hashable
 
 try:
     import aiofiles
@@ -31,15 +31,14 @@
 
 
 class JSONContextStorage(DBContextStorage):
     """
     Implements :py:class:`.DBContextStorage` with `json` as the storage format.
 
     :param path: Target file URI. Example: `json://file.json`.
-    :type path: str
     """
 
     def __init__(self, path: str):
         DBContextStorage.__init__(self, path)
         asyncio.run(self._load())
 
     @threadsafe_method
```

### Comparing `dff-0.3.2/dff/context_storages/mongo.py` & `dff-0.4.1/dff/context_storages/mongo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Mongo
 -----
 The Mongo module provides a MongoDB-based version of the :py:class:`.DBContextStorage` class.
 This class is used to store and retrieve context data in a MongoDB.
-It allows the `DFF` to easily store and retrieve context data in a format that is highly scalable
+It allows the DFF to easily store and retrieve context data in a format that is highly scalable
 and easy to work with.
 
 MongoDB is a widely-used, open-source NoSQL database that is known for its scalability and performance.
 It stores data in a format similar to JSON, making it easy to work with the data in a variety of programming languages
 and environments. Additionally, MongoDB is highly scalable and can handle large amounts of data
 and high levels of read and write traffic.
 """
```

### Comparing `dff-0.3.2/dff/context_storages/pickle.py` & `dff-0.4.1/dff/context_storages/pickle.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Pickle
 ------
 The Pickle module provides a pickle-based version of the :py:class:`.DBContextStorage` class.
 This class is used to store and retrieve context data in a pickle format.
-It allows the `DFF` to easily store and retrieve context data in a format that is efficient
+It allows the DFF to easily store and retrieve context data in a format that is efficient
 for serialization and deserialization and can be easily used in python.
 
 Pickle is a python library that allows to serialize and deserialize python objects.
 It is efficient and fast, but it is not recommended to use it to transfer data across
 different languages or platforms because it's not cross-language compatible.
 """
 import asyncio
```

### Comparing `dff-0.3.2/dff/context_storages/protocol.py` & `dff-0.4.1/dff/context_storages/protocol.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 """
 Protocol
 --------
-The Protocol module contains the base code for the different communication protocols used in the `DFF`.
-It defines the :py:data:`.PROTOCOLS` constant, which lists all the supported protocols in the `DFF`.
+The Protocol module contains the base code for the different communication protocols used in the DFF.
+It defines the :py:data:`.PROTOCOLS` constant, which lists all the supported protocols in the DFF.
 
 The module also includes a function :py:func:`.get_protocol_install_suggestion()` that is used to provide
 suggestions for installing the necessary dependencies for a specific protocol.
 This function takes the name of the desired protocol as an argument and returns
 a string containing the necessary installation commands for that protocol.
 
-The `DFF` supports a variety of communication protocols,
+The DFF supports a variety of communication protocols,
 which allows it to communicate with different types of databases.
 """
 import json
 import pathlib
 
 with open(pathlib.Path(__file__).parent / "protocols.json", "r", encoding="utf-8") as protocols:
     PROTOCOLS = json.load(protocols)
 _prtocol_keys = {"module", "class", "slug", "uri_example"}
 assert all(set(proc.keys()) == _prtocol_keys for proc in PROTOCOLS.values()), "Protocols are incomplete"
 
 
 def get_protocol_install_suggestion(protocol_name: str) -> str:
+    """
+    Provide suggestions for installing the necessary dependencies for a specific protocol.
+
+    :param protocol_name: Protocol name.
+    """
     protocol = PROTOCOLS.get(protocol_name, {})
     slug = protocol.get("slug")
     if slug:
         return f"Try to run `pip install dff[{slug}]`"
     return ""
```

### Comparing `dff-0.3.2/dff/context_storages/protocols.json` & `dff-0.4.1/dff/context_storages/protocols.json`

 * *Files identical despite different names*

### Comparing `dff-0.3.2/dff/context_storages/redis.py` & `dff-0.4.1/dff/context_storages/redis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Redis
 -----
 The Redis module provides a Redis-based version of the :py:class:`.DBContextStorage` class.
 This class is used to store and retrieve context data in a Redis.
-It allows the `DFF` to easily store and retrieve context data in a format that is highly scalable
+It allows the DFF to easily store and retrieve context data in a format that is highly scalable
 and easy to work with.
 
 Redis is an open-source, in-memory data structure store that is known for its
 high performance and scalability. It stores data in key-value pairs and supports a variety of data
 structures such as strings, hashes, lists, sets, and more.
 Additionally, Redis can be used as a cache, message broker, and database, making it a versatile
 and powerful choice for data storage and management.
@@ -29,15 +29,14 @@
 
 
 class RedisContextStorage(DBContextStorage):
     """
     Implements :py:class:`.DBContextStorage` with `redis` as the database backend.
 
     :param path: Database URI string. Example: `redis://user:password@host:port`.
-    :type path: str
     """
 
     def __init__(self, path: str):
         DBContextStorage.__init__(self, path)
         if not redis_available:
             install_suggestion = get_protocol_install_suggestion("redis")
             raise ImportError("`redis` package is missing.\n" + install_suggestion)
```

### Comparing `dff-0.3.2/dff/context_storages/shelve.py` & `dff-0.4.1/dff/context_storages/shelve.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Shelve
 ------
 The Shelve module provides a shelve-based version of the :py:class:`.DBContextStorage` class.
 This class is used to store and retrieve context data in a shelve format.
-It allows the `DFF` to easily store and retrieve context data in a format that is efficient
+It allows the DFF to easily store and retrieve context data in a format that is efficient
 for serialization and deserialization and can be easily used in python.
 
 Shelve is a python library that allows to store and retrieve python objects.
 It is efficient and fast, but it is not recommended to use it to transfer data across different languages
 or platforms because it's not cross-language compatible.
 It stores data in a dbm-style format in the file system, which is not as fast as the other serialization
 libraries like pickle or JSON.
```

### Comparing `dff-0.3.2/dff/context_storages/sql.py` & `dff-0.4.1/dff/context_storages/sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 SQL
 ---
 The SQL module provides a SQL-based version of the :py:class:`.DBContextStorage` class.
 This class is used to store and retrieve context data from SQL databases.
-It allows the `DFF` to easily store and retrieve context data in a format that is highly scalable
+It allows the DFF to easily store and retrieve context data in a format that is highly scalable
 and easy to work with.
 
 The SQL module provides the ability to choose the backend of your choice from
 MySQL, PostgreSQL, or SQLite. You can choose the one that is most suitable for your use case and environment.
 MySQL and PostgreSQL are widely used open-source relational databases that are known for their
 reliability and scalability. SQLite is a self-contained, high-reliability, embedded, full-featured,
 public-domain, SQL database engine.
```

### Comparing `dff-0.3.2/dff/context_storages/ydb.py` & `dff-0.4.1/dff/context_storages/ydb.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     """
     Version of the :py:class:`.DBContextStorage` for YDB.
 
     :param path: Standard sqlalchemy URI string.
         When using sqlite backend in Windows, keep in mind that you have to use double backslashes '\\'
         instead of forward slashes '/' in the file path.
     :param table_name: The name of the table to use.
-    :type table_name: str
     """
 
     def __init__(self, path: str, table_name: str = "contexts", timeout=5):
         DBContextStorage.__init__(self, path)
         protocol, netloc, self.database, _, _ = urlsplit(path)
         self.endpoint = "{}://{}".format(protocol, netloc)
         self.table_name = table_name
```

### Comparing `dff-0.3.2/dff/messengers/common/interface.py` & `dff-0.4.1/dff/messengers/common/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Message Interfaces
 ------------------
 The Message Interfaces module contains several basic classes that define the message interfaces.
-These classes provide a way to define the structure of the messengers that are used to communicate with the `DFF`.
+These classes provide a way to define the structure of the messengers that are used to communicate with the DFF.
 """
 import abc
 import asyncio
 import logging
 import uuid
 from typing import Optional, Any, List, Tuple, TextIO, Hashable
 
@@ -89,15 +89,15 @@
         self,
         pipeline_runner: PipelineRunnerFunction,
         loop: PollingInterfaceLoopFunction = lambda: True,
         timeout: float = 0,
     ):
         """
         Method, running a request - response cycle in a loop.
-        The looping behaviour is determined by `loop` and `timeout`,
+        The looping behavior is determined by `loop` and `timeout`,
         for most cases the loop itself shouldn't be overridden.
 
         :param pipeline_runner: A function that should return pipeline response to user request;
             usually it's a :py:meth:`~Pipeline._run_pipeline(request, ctx_id)` function.
         :type pipeline_runner: PipelineRunnerFunction
         :param loop: a function that determines whether polling should be continued;
             called in each cycle, should return `True` to continue polling or `False` to stop.
```

### Comparing `dff-0.3.2/dff/messengers/common/types.py` & `dff-0.4.1/dff/messengers/common/types.py`

 * *Files identical despite different names*

### Comparing `dff-0.3.2/dff/messengers/telegram/interface.py` & `dff-0.4.1/dff/messengers/telegram/interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -186,49 +186,67 @@
         Defaults to "/telegram-webhook".
     :param host:
         Host IP.
         Defaults to "localhost".
     :param port:
         Port of the app.
         Defaults to 8443.
+    :param debug:
+        Run the Flask app in debug mode.
+    :param load_dotenv:
+        Whether or not the .env file in the project folder
+        should be used to set environment variables.
     :param full_uri:
         Full public IP of your webhook that is accessible by https.
         Defaults to `"https://{host}:{port}{endpoint}"`.
+    :param wsgi_options:
+        Keyword arguments to forward to `Flask.run` method.
+        Use these to set `ssl_context` and other WSGI options.
     """
 
     def __init__(
         self,
         token: str,
         app: Optional[Flask] = None,
         host: str = "localhost",
         port: int = 8443,
+        debug: Optional[bool] = None,
+        load_dotenv: bool = True,
         endpoint: str = "/telegram-webhook",
         full_uri: Optional[str] = None,
         messenger: Optional[TelegramMessenger] = None,
+        **wsgi_options,
     ):
         if not flask_imported:
             raise ModuleNotFoundError("Flask is not installed. Install it with `pip install flask`.")
 
         self.messenger = messenger if messenger is not None else TelegramMessenger(token)
         self.app = app if app else Flask(__name__)
         self.host = host
         self.port = port
+        self.debug = debug
+        self.load_dotenv = load_dotenv
+        self.wsgi_options = wsgi_options
         self.endpoint = endpoint
         self.full_uri = full_uri if full_uri is not None else "".join([f"https://{host}:{port}", endpoint])
 
         async def endpoint():
             if not request.headers.get("content-type") == "application/json":
                 abort(403)
 
             json_string = request.get_data().decode("utf-8")
             update = types.Update.de_json(json_string)
-            return self.on_request(*extract_telegram_request_and_id(update, self.messenger))
+            resp = self.on_request(*extract_telegram_request_and_id(update, self.messenger))
+            self.messenger.send_response(resp.id, resp.last_response)
+            return ""
 
         self.app.route(self.endpoint, methods=["POST"])(endpoint)
 
     async def connect(self, callback: PipelineRunnerFunction):
         await super().connect(callback)
 
         self.messenger.remove_webhook()
         self.messenger.set_webhook(self.full_uri)
 
-        self.app.run(host=self.host, port=self.port)
+        self.app.run(
+            host=self.host, port=self.port, load_dotenv=self.load_dotenv, debug=self.debug, **self.wsgi_options
+        )
```

### Comparing `dff-0.3.2/dff/messengers/telegram/message.py` & `dff-0.4.1/dff/messengers/telegram/message.py`

 * *Files identical despite different names*

### Comparing `dff-0.3.2/dff/messengers/telegram/messenger.py` & `dff-0.4.1/dff/messengers/telegram/messenger.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 """
 from pathlib import Path
 from typing import Union, List, Optional, Callable
 from enum import Enum
 
 from telebot import types, TeleBot
 
-from dff.script import Context, Actor
+from dff.script import Context
+from dff.pipeline import Pipeline
 
 from .utils import batch_open_io
 from .message import TelegramMessage, TelegramUI, RemoveKeyboard
 
 from dff.script import Message
 from dff.script.core.message import Audio, Video, Image, Document
 
@@ -224,15 +225,15 @@
         regexp=regexp,
         func=func,
         content_types=content_types,
         chat_types=chat_types,
         **kwargs,
     )
 
-    def condition(ctx: Context, actor: Actor, *args, **kwargs):  # pragma: no cover
+    def condition(ctx: Context, _: Pipeline, *__, **___):  # pragma: no cover
         last_request = ctx.last_request
         if last_request is None:
             return False
         update = getattr(last_request, "update", None)
         request_update_type = getattr(last_request, "update_type", None)
         if update is None:
             return False
```

### Comparing `dff-0.3.2/dff/messengers/telegram/utils.py` & `dff-0.4.1/dff/messengers/telegram/utils.py`

 * *Files identical despite different names*

### Comparing `dff-0.3.2/dff/pipeline/__init__.py` & `dff-0.4.1/dff/pipeline/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,12 +24,12 @@
     ServiceFunction,
     ExtraHandlerBuilder,
     ServiceBuilder,
     ServiceGroupBuilder,
     PipelineBuilder,
 )
 
-from .pipeline.pipeline import Pipeline
+from .pipeline.pipeline import Pipeline, ACTOR
 
 from .service.extra import BeforeHandler, AfterHandler
 from .service.group import ServiceGroup
 from .service.service import Service, to_service
```

### Comparing `dff-0.3.2/dff/pipeline/conditions.py` & `dff-0.4.1/dff/pipeline/conditions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,61 +1,63 @@
 """
 Conditions
 ----------
 The conditions module contains functions that can be used to determine whether the pipeline component to which they
 are attached should be executed or not.
 The standard set of them allows user to setup dependencies between pipeline components.
 """
-from typing import Optional
+from typing import Optional, ForwardRef
 
-from dff.script import Actor, Context
+from dff.script import Context
 
 from .types import (
     PIPELINE_STATE_KEY,
     StartConditionCheckerFunction,
     ComponentExecutionState,
     StartConditionCheckerAggregationFunction,
 )
 
+Pipeline = ForwardRef("Pipeline")
 
-def always_start_condition(_: Context, __: Actor) -> bool:
+
+def always_start_condition(_: Context, __: Pipeline) -> bool:
     """
     Condition that always allows service execution. It's the default condition for all services.
 
-    :param ctx: Current dialog context.
-    :param actor: Pipeline actor.
+    :param _: Current dialog context.
+    :param __: Pipeline.
     """
     return True
 
 
 def service_successful_condition(path: Optional[str] = None) -> StartConditionCheckerFunction:
     """
     Condition that allows service execution, only if the other service was executed successfully.
     Returns :py:data:`~.StartConditionCheckerFunction`.
 
     :param path: The path of the condition pipeline component.
     """
 
-    def check_service_state(ctx: Context, _: Actor):
+    def check_service_state(ctx: Context, _: Pipeline):
         state = ctx.framework_states[PIPELINE_STATE_KEY].get(path, ComponentExecutionState.NOT_RUN.name)
         return ComponentExecutionState[state] == ComponentExecutionState.FINISHED
 
     return check_service_state
 
 
 def not_condition(function: StartConditionCheckerFunction) -> StartConditionCheckerFunction:
     """
     Condition that returns opposite boolean value to the one returned by incoming function.
     Returns :py:data:`~.StartConditionCheckerFunction`.
 
     :param function: The function to return opposite of.
     """
 
-    def not_function(ctx: Context, actor: Actor):
-        return not function(ctx, actor)
+    def not_function(ctx: Context, pipeline: Pipeline):
+        return not function(ctx, pipeline)
 
     return not_function
 
 
 def aggregate_condition(
     aggregator: StartConditionCheckerAggregationFunction, *functions: StartConditionCheckerFunction
 ) -> StartConditionCheckerFunction:
@@ -63,16 +65,16 @@
     Condition that returns aggregated boolean value from all booleans returned by incoming functions.
     Returns :py:data:`~.StartConditionCheckerFunction`.
 
     :param aggregator: The function that accepts list of booleans and returns a single boolean.
     :param functions: Functions to aggregate.
     """
 
-    def aggregation_function(ctx: Context, actor: Actor):
-        return aggregator([function(ctx, actor) for function in functions])
+    def aggregation_function(ctx: Context, pipeline: Pipeline):
+        return aggregator([function(ctx, pipeline) for function in functions])
 
     return aggregation_function
 
 
 def all_condition(*functions: StartConditionCheckerFunction) -> StartConditionCheckerFunction:
     """
     Condition that returns `True` only if all incoming functions return `True`.
```

### Comparing `dff-0.3.2/dff/pipeline/pipeline/component.py` & `dff-0.4.1/dff/pipeline/pipeline/component.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 The PipelineComponent class can be a group or a service. It is designed to be reusable and composable,
 allowing developers to create complex processing pipelines by combining multiple components.
 """
 import logging
 import abc
 import asyncio
 import copy
-from typing import Optional, Union, Awaitable
+from typing import Optional, Union, Awaitable, ForwardRef
 
-from dff.script import Context, Actor
+from dff.script import Context
 
 from ..service.extra import BeforeHandler, AfterHandler
 from ..conditions import always_start_condition
 from ..types import (
     PIPELINE_STATE_KEY,
     StartConditionCheckerFunction,
     ComponentExecutionState,
@@ -27,14 +27,16 @@
     ExtraHandlerFunction,
     ExtraHandlerType,
     ExtraHandlerBuilder,
 )
 
 logger = logging.getLogger(__name__)
 
+Pipeline = ForwardRef("Pipeline")
+
 
 class PipelineComponent(abc.ABC):
     """
     This class represents a pipeline component, which is a service or a service group.
     It contains some fields that they have in common.
 
     :param before_handler: :py:class:`~.BeforeHandler`, associated with this component.
@@ -134,59 +136,57 @@
             it returns `False`.
         - | If component **can't** be asynchronous and :py:attr:`~requested_async_flag` is `True`,
             an Exception is thrown in constructor.
 
         """
         return self.calculated_async_flag if self.requested_async_flag is None else self.requested_async_flag
 
-    async def run_extra_handler(self, stage: ExtraHandlerType, ctx: Context, actor: Actor):
+    async def run_extra_handler(self, stage: ExtraHandlerType, ctx: Context, pipeline: Pipeline):
         extra_handler = None
         if stage == ExtraHandlerType.BEFORE:
             extra_handler = self.before_handler
         if stage == ExtraHandlerType.AFTER:
             extra_handler = self.after_handler
         if extra_handler is None:
             return
         try:
-            extra_handler_result = await extra_handler(ctx, actor, self._get_runtime_info(ctx))
+            extra_handler_result = await extra_handler(ctx, pipeline, self._get_runtime_info(ctx))
             if extra_handler.asynchronous and isinstance(extra_handler_result, Awaitable):
                 await extra_handler_result
         except asyncio.TimeoutError:
             logger.warning(f"{type(self).__name__} '{self.name}' {extra_handler.stage.name} extra handler timed out!")
 
     @abc.abstractmethod
-    async def _run(self, ctx: Context, actor: Optional[Actor] = None) -> Optional[Context]:
+    async def _run(self, ctx: Context, pipeline: Optional[Pipeline] = None) -> Optional[Context]:
         """
         A method for running pipeline component, it is overridden in all its children.
         This method is run after the component's timeout is set (if needed).
 
         :param ctx: Current dialog :py:class:`~.Context`.
-        :param actor: This :py:class:`~.Pipeline` :py:class:`~.Actor` or
-            `None` if this is a service, that wraps :py:class:`~.Actor`.
+        :param pipeline: This :py:class:`~.Pipeline`.
         :return: :py:class:`~.Context` if this is a synchronous service or `None`,
             asynchronous services shouldn't modify :py:class:`~.Context`.
         """
         raise NotImplementedError
 
-    async def __call__(self, ctx: Context, actor: Optional[Actor] = None) -> Optional[Union[Context, Awaitable]]:
+    async def __call__(self, ctx: Context, pipeline: Optional[Pipeline] = None) -> Optional[Union[Context, Awaitable]]:
         """
         A method for calling pipeline components.
         It sets up timeout if this component is asynchronous and executes it using :py:meth:`~._run` method.
 
         :param ctx: Current dialog :py:class:`~.Context`.
-        :param actor: This :py:class:`~.Pipeline` :py:class:`~.Actor` or
-            `None` if this is a service, that wraps :py:class:`~.Actor`.
+        :param pipeline: This :py:class:`~.Pipeline`.
         :return: :py:class:`~.Context` if this is a synchronous service or :py:class:`~.typing.const.Awaitable`,
             asynchronous services shouldn't modify :py:class:`~.Context`.
         """
         if self.asynchronous:
-            task = asyncio.create_task(self._run(ctx, actor))
+            task = asyncio.create_task(self._run(ctx, pipeline))
             return asyncio.wait_for(task, timeout=self.timeout)
         else:
-            return await self._run(ctx, actor)
+            return await self._run(ctx, pipeline)
 
     def add_extra_handler(self, global_extra_handler_type: GlobalExtraHandlerType, extra_handler: ExtraHandlerFunction):
         """
         Method for adding a global extra handler to this particular component.
 
         :param global_extra_handler_type: A type of extra handler to add.
         :param extra_handler: A :py:class:`~.GlobalExtraHandlerType` to add to the component as an extra handler.
```

### Comparing `dff-0.3.2/dff/pipeline/pipeline/utils.py` & `dff-0.4.1/dff/pipeline/pipeline/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 The Utils module contains several service functions that are commonly used throughout the framework.
 These functions provide a variety of utility functionality.
 """
 import collections
 from typing import Union, List, Callable
 from inspect import isfunction
 
-from dff.script import Actor
-
 from ..service.service import Service
 from ..service.group import ServiceGroup
 
 
 def pretty_format_component_info_dict(
     service: dict,
     show_extra_handlers: bool,
@@ -62,26 +60,26 @@
     service: Union[Service, ServiceGroup], collisions: List[Union[Service, ServiceGroup]]
 ) -> str:
     """
     Function for generating new name for a pipeline component,
     that has similar name with other components in the same group.
     The name is generated according to these rules:
 
-    - If service's handler is `Actor`, it is named `actor`.
+    - If service's handler is "ACTOR", it is named `actor`.
     - If service's handler is `Callable`, it is named after this `callable`.
     - If it's a service group, it is named `service_group`.
     - Otherwise, it is names `noname_service`.
     - | After that, `_[NUMBER]` is added to the resulting name,
         where `_[NUMBER]` is number of components with the same name in current service group.
 
     :param service: Service to be renamed.
     :param collisions: Services in the same service group as service.
     :return: Generated name
     """
-    if isinstance(service, Service) and isinstance(service.handler, Actor):
+    if isinstance(service, Service) and isinstance(service.handler, str) and service.handler == "ACTOR":
         base_name = "actor"
     elif isinstance(service, Service) and isinstance(service.handler, Callable):
         if isfunction(service.handler):
             base_name = service.handler.__name__
         else:
             base_name = service.handler.__class__.__name__
     elif isinstance(service, ServiceGroup):
@@ -91,38 +89,38 @@
 
     name_index = 0
     while f"{base_name}_{name_index}" in [component.name for component in collisions]:
         name_index += 1
     return f"{base_name}_{name_index}"
 
 
-def finalize_service_group(service_group: ServiceGroup, path: str = ".") -> Actor:
+def finalize_service_group(service_group: ServiceGroup, path: str = ".") -> bool:
     """
     Function that iterates through a service group (and all its subgroups),
     finalizing component's names and paths in it.
     Components are renamed only if user didn't set a name for them. Their paths are also generated here.
-    It also searches for :py:class:`~.Actor` in the group, throwing exception if no actor or multiple actors found.
+    It also searches for "ACTOR" in the group, throwing exception if no actor or multiple actors found.
 
     :param service_group: Service group to resolve name collisions in.
     """
-    actor = None
+    actor = False
     names_counter = collections.Counter([component.name for component in service_group.components])
     for component in service_group.components:
         if component.name is None:
             component.name = rename_component_incrementing(component, service_group.components)
         elif names_counter[component.name] > 1:
             raise Exception(f"User defined service name collision ({path})!")
         component.path = f"{path}.{component.name}"
 
-        if isinstance(component, Service) and isinstance(component.handler, Actor):
-            current_actor = component.handler
+        if isinstance(component, Service) and isinstance(component.handler, str) and component.handler == "ACTOR":
+            actor_found = True
         elif isinstance(component, ServiceGroup):
-            current_actor = finalize_service_group(component, f"{path}.{component.name}")
+            actor_found = finalize_service_group(component, f"{path}.{component.name}")
         else:
-            current_actor = None
+            actor_found = False
 
-        if current_actor is not None:
-            if actor is None:
-                actor = current_actor
+        if actor_found:
+            if not actor:
+                actor = actor_found
             else:
                 raise Exception(f"More than one actor found in group ({path})!")
     return actor
```

### Comparing `dff-0.3.2/dff/pipeline/service/extra.py` & `dff-0.4.1/dff/pipeline/service/extra.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 """
 Extra Handler
 -------------
 The Extra Handler module contains additional functionality that extends the capabilities of the system
 beyond the core functionality. Extra handlers is an input converting addition to :py:class:`.PipelineComponent`.
-For examples, it is used to grep statistics from components, timeing, logging, etc.
+For example, it is used to grep statistics from components, timing, logging, etc.
 """
 import asyncio
 import logging
 import inspect
-from typing import Optional, List
+from typing import Optional, List, ForwardRef
 
-from dff.script import Context, Actor
+from dff.script import Context
 
 from .utils import collect_defined_constructor_parameters_to_dict, _get_attrs_with_updates, wrap_sync_function_in_async
 from ..types import ServiceRuntimeInfo, ExtraHandlerType, ExtraHandlerBuilder, ExtraHandlerFunction
 
 logger = logging.getLogger(__name__)
 
+Pipeline = ForwardRef("Pipeline")
+
 
 class _ComponentExtraHandler:
     """
     Class, representing an extra pipeline component handler.
     A component extra handler is a set of functions, attached to pipeline component (before or after it).
     Extra handlers should execute supportive tasks (like time or resources measurement, minor data transformations).
-    Extra handlers should NOT edit context or actor, use services for that purpose instead.
+    Extra handlers should NOT edit context or pipeline, use services for that purpose instead.
 
     :param functions: An `ExtraHandlerBuilder` object, an `_ComponentExtraHandler` instance,
         a dict or a list of :py:data:`~.ExtraHandlerFunction`.
     :type functions: :py:data:`~.ExtraHandlerBuilder`
     :param stage: An :py:class:`~.ExtraHandlerType`, specifying whether this handler will be executed before or
         after pipeline component.
     :param timeout: (for asynchronous only!) Maximum component execution time (in seconds),
@@ -81,79 +83,79 @@
         - | If component **can't** be asynchronous and :py:attr:`~requested_async_flag` is `True`,
             an Exception is thrown in constructor.
 
         """
         return self.calculated_async_flag if self.requested_async_flag is None else self.requested_async_flag
 
     async def _run_function(
-        self, function: ExtraHandlerFunction, ctx: Context, actor: Actor, component_info: ServiceRuntimeInfo
+        self, function: ExtraHandlerFunction, ctx: Context, pipeline: Pipeline, component_info: ServiceRuntimeInfo
     ):
         handler_params = len(inspect.signature(function).parameters)
         if handler_params == 1:
             await wrap_sync_function_in_async(function, ctx)
         elif handler_params == 2:
-            await wrap_sync_function_in_async(function, ctx, actor)
+            await wrap_sync_function_in_async(function, ctx, pipeline)
         elif handler_params == 3:
             await wrap_sync_function_in_async(
                 function,
                 ctx,
-                actor,
+                pipeline,
                 {
                     "function": function,
                     "stage": self.stage,
                     "component": component_info,
                 },
             )
         else:
             raise Exception(
                 f"Too many parameters required for component {component_info['name']} {self.stage.name}"
                 f" wrapper handler '{function.__name__}': {handler_params}!"
             )
 
-    async def _run(self, ctx: Context, actor: Actor, component_info: ServiceRuntimeInfo):
+    async def _run(self, ctx: Context, pipeline: Pipeline, component_info: ServiceRuntimeInfo):
         """
         Method for executing one of the wrapper functions (before or after).
         If the function is not set, nothing happens.
 
         :param stage: current `WrapperStage` (before or after).
         :param ctx: current dialog context.
-        :param actor: actor, associated with current pipeline.
+        :param pipeline: the current pipeline.
         :param component_info: associated component's info dictionary.
         :return: `None`
         """
 
         if self.asynchronous:
-            futures = [self._run_function(function, ctx, actor, component_info) for function in self.functions]
+            futures = [self._run_function(function, ctx, pipeline, component_info) for function in self.functions]
             for function, future in zip(self.functions, asyncio.as_completed(futures)):
                 try:
                     await future
                 except asyncio.TimeoutError:
                     logger.warning(
                         f"Component {component_info['name']} {self.stage.name} wrapper '{function.__name__}' timed out!"
                     )
 
         else:
             for function in self.functions:
-                await self._run_function(function, ctx, actor, component_info)
+                await self._run_function(function, ctx, pipeline, component_info)
 
-    async def __call__(self, ctx: Context, actor: Actor, component_info: ServiceRuntimeInfo):
+    async def __call__(self, ctx: Context, pipeline: Pipeline, component_info: ServiceRuntimeInfo):
         """
         A method for calling pipeline components.
         It sets up timeout if this component is asynchronous and executes it using `_run` method.
 
         :param ctx: (required) Current dialog `Context`.
-        :param actor: This `Pipeline` `Actor` or `None` if this is a service, that wraps `Actor`.
+        :param pipeline: This `Pipeline`.
         :return: `Context` if this is a synchronous service or
             `Awaitable` if this is an asynchronous component or `None`.
         """
         if self.asynchronous:
-            task = asyncio.create_task(self._run(ctx, actor, component_info))
+            task = asyncio.create_task(self._run(ctx, pipeline, component_info))
             return await asyncio.wait_for(task, timeout=self.timeout)
         else:
-            return await self._run(ctx, actor, component_info)
+            return await self._run(ctx, pipeline, component_info)
 
     @property
     def info_dict(self) -> dict:
         """
         Property for retrieving info dictionary about this wrapper.
 
         :return: Info dict, containing its fields as well as its type.
@@ -164,24 +166,50 @@
             "timeout": self.timeout,
             "asynchronous": self.asynchronous,
             "functions": [function.__name__ for function in self.functions],
         }
 
 
 class BeforeHandler(_ComponentExtraHandler):
+    """
+    A handler for extra functions that are executed before the component's main function.
+
+    :param functions: A callable or a list of callables that will be executed
+        before the component's main function.
+    :type functions: ExtraHandlerBuilder
+    :param timeout: Optional timeout for the execution of the extra functions, in
+        seconds.
+    :param asynchronous: Optional flag that indicates whether the extra functions
+        should be executed asynchronously. The default value of the flag is True
+        if all the functions in this handler are asynchronous.
+    """
+
     def __init__(
         self,
         functions: ExtraHandlerBuilder,
         timeout: Optional[int] = None,
         asynchronous: Optional[bool] = None,
     ):
         super().__init__(functions, ExtraHandlerType.BEFORE, timeout, asynchronous)
 
 
 class AfterHandler(_ComponentExtraHandler):
+    """
+    A handler for extra functions that are executed after the component's main function.
+
+    :param functions: A callable or a list of callables that will be executed
+        after the component's main function.
+    :type functions: ExtraHandlerBuilder
+    :param timeout: Optional timeout for the execution of the extra functions, in
+        seconds.
+    :param asynchronous: Optional flag that indicates whether the extra functions
+        should be executed asynchronously. The default value of the flag is True
+        if all the functions in this handler are asynchronous.
+    """
+
     def __init__(
         self,
         functions: ExtraHandlerBuilder,
         timeout: Optional[int] = None,
         asynchronous: Optional[bool] = None,
     ):
         super().__init__(functions, ExtraHandlerType.AFTER, timeout, asynchronous)
```

### Comparing `dff-0.3.2/dff/pipeline/service/group.py` & `dff-0.4.1/dff/pipeline/service/group.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 :py:class:`~.ServiceGroup` class, which is used to represent a group of related services.
 This class provides a way to organize and manage multiple services as a single unit,
 allowing for easier management and organization of the services within the pipeline.
 The :py:class:`~.ServiceGroup` serves the important function of grouping services to work together in parallel.
 """
 import asyncio
 import logging
-from typing import Optional, List, Union, Awaitable
+from typing import Optional, List, Union, Awaitable, ForwardRef
 
-from dff.script import Actor, Context
+from dff.script import Context
 
 from .utils import collect_defined_constructor_parameters_to_dict, _get_attrs_with_updates
 from ..pipeline.component import PipelineComponent
 from ..types import (
     StartConditionCheckerFunction,
     ComponentExecutionState,
     ServiceGroupBuilder,
@@ -25,14 +25,16 @@
     ExtraHandlerBuilder,
     ExtraHandlerType,
 )
 from .service import Service
 
 logger = logging.getLogger(__name__)
 
+Pipeline = ForwardRef("Pipeline")
+
 
 class ServiceGroup(PipelineComponent):
     """
     A service group class.
     Service group can be included into pipeline as an object or a pipeline component list.
     Service group can be synchronous or asynchronous.
     Components in synchronous groups are executed consequently (no matter is they are synchronous or asynchronous).
@@ -91,76 +93,76 @@
             calc_async = all([service.asynchronous for service in self.components])
             super(ServiceGroup, self).__init__(
                 before_handler, after_handler, timeout, asynchronous, calc_async, start_condition, name
             )
         else:
             raise Exception(f"Unknown type for ServiceGroup {components}")
 
-    async def _run_services_group(self, ctx: Context, actor: Actor) -> Context:
+    async def _run_services_group(self, ctx: Context, pipeline: Pipeline) -> Context:
         """
         Method for running this service group.
         It doesn't include wrappers execution, start condition checking or error handling - pure execution only.
         Executes components inside the group based on its `asynchronous` property.
         Collects information about their execution state - group is finished successfully
         only if all components in it finished successfully.
 
         :param ctx: Current dialog context.
-        :param actor: Actor, associated with the pipeline.
+        :param pipeline: The current pipeline.
         :return: Current dialog context.
         """
         self._set_state(ctx, ComponentExecutionState.RUNNING)
 
         if self.asynchronous:
-            service_futures = [service(ctx, actor) for service in self.components]
+            service_futures = [service(ctx, pipeline) for service in self.components]
             for service, future in zip(self.components, asyncio.as_completed(service_futures)):
                 try:
                     service_result = await future
                     if service.asynchronous and isinstance(service_result, Awaitable):
                         await service_result
                 except asyncio.TimeoutError:
                     logger.warning(f"{type(service).__name__} '{service.name}' timed out!")
 
         else:
             for service in self.components:
-                service_result = await service(ctx, actor)
+                service_result = await service(ctx, pipeline)
                 if not service.asynchronous and isinstance(service_result, Context):
                     ctx = service_result
                 elif service.asynchronous and isinstance(service_result, Awaitable):
                     await service_result
 
         failed = any([service.get_state(ctx) == ComponentExecutionState.FAILED for service in self.components])
         self._set_state(ctx, ComponentExecutionState.FAILED if failed else ComponentExecutionState.FINISHED)
         return ctx
 
     async def _run(
         self,
         ctx: Context,
-        actor: Actor = None,
+        pipeline: Pipeline = None,
     ) -> Optional[Context]:
         """
         Method for handling this group execution.
         Executes before and after execution wrappers, checks start condition and catches runtime exceptions.
 
         :param ctx: Current dialog context.
-        :param actor: Actor, associated with the pipeline.
+        :param pipeline: The current pipeline.
         :return: Current dialog context if synchronous, else `None`.
         """
-        await self.run_extra_handler(ExtraHandlerType.BEFORE, ctx, actor)
+        await self.run_extra_handler(ExtraHandlerType.BEFORE, ctx, pipeline)
 
         try:
-            if self.start_condition(ctx, actor):
-                ctx = await self._run_services_group(ctx, actor)
+            if self.start_condition(ctx, pipeline):
+                ctx = await self._run_services_group(ctx, pipeline)
             else:
                 self._set_state(ctx, ComponentExecutionState.NOT_RUN)
 
         except Exception as e:
             self._set_state(ctx, ComponentExecutionState.FAILED)
             logger.error(f"ServiceGroup '{self.name}' execution failed!\n{e}")
 
-        await self.run_extra_handler(ExtraHandlerType.AFTER, ctx, actor)
+        await self.run_extra_handler(ExtraHandlerType.AFTER, ctx, pipeline)
         return ctx if not self.asynchronous else None
 
     def log_optimization_warnings(self):
         """
         Method for logging service group optimization warnings for all this groups inner components.
         (NOT this group itself!).
         Warnings are basically messages,
```

### Comparing `dff-0.3.2/dff/pipeline/service/service.py` & `dff-0.4.1/dff/pipeline/service/service.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,30 +10,32 @@
 Actor wrapping service can be synchronous only.
 """
 # TODO: change last sentence, when actor will be asynchronous
 
 import logging
 import asyncio
 import inspect
-from typing import Optional, Callable
+from typing import Optional, Callable, ForwardRef
 
-from dff.script import Actor, Context
+from dff.script import Context
 
 from .utils import wrap_sync_function_in_async, collect_defined_constructor_parameters_to_dict, _get_attrs_with_updates
 from ..types import (
     ServiceBuilder,
     StartConditionCheckerFunction,
     ComponentExecutionState,
     ExtraHandlerBuilder,
     ExtraHandlerType,
 )
 from ..pipeline.component import PipelineComponent
 
 logger = logging.getLogger(__name__)
 
+Pipeline = ForwardRef("Pipeline")
+
 
 class Service(PipelineComponent):
     """
     This class represents a service.
     Service can be included into pipeline as object or a dictionary.
     Service group can be synchronous or asynchronous.
     Service can be asynchronous only if its handler is a coroutine.
@@ -79,119 +81,119 @@
                         "calculated_async_flag",
                         "path",
                     ),
                     {"requested_async_flag": "asynchronous"},
                     overridden_parameters,
                 )
             )
-        elif isinstance(handler, Callable):
+        elif isinstance(handler, Callable) or isinstance(handler, str) and handler == "ACTOR":
             self.handler = handler
             super(Service, self).__init__(
                 before_handler,
                 after_handler,
                 timeout,
                 asynchronous,
                 asyncio.iscoroutinefunction(handler),
                 start_condition,
                 name,
             )
         else:
             raise Exception(f"Unknown type of service handler: {handler}")
 
-    async def _run_handler(self, ctx: Context, actor: Actor):
+    async def _run_handler(self, ctx: Context, pipeline: Pipeline):
         """
         Method for service `handler` execution.
         Handler has three possible signatures, so this method picks the right one to invoke.
         These possible signatures are:
 
         - (ctx: Context) - accepts current dialog context only.
-        - (ctx: Context, actor: Actor) - accepts context and actor, associated with the pipeline.
-        - | (ctx: Context, actor: Actor, info: ServiceRuntimeInfo) - accepts context,
-              actor and service runtime info dictionary.
+        - (ctx: Context, pipeline: Pipeline) - accepts context and current pipeline.
+        - | (ctx: Context, pipeline: Pipeline, info: ServiceRuntimeInfo) - accepts context,
+              pipeline and service runtime info dictionary.
 
         :param ctx: Current dialog context.
-        :param actor: Actor associated with the pipeline.
+        :param pipeline: The current pipeline.
         :return: `None`
         """
         handler_params = len(inspect.signature(self.handler).parameters)
         if handler_params == 1:
             await wrap_sync_function_in_async(self.handler, ctx)
         elif handler_params == 2:
-            await wrap_sync_function_in_async(self.handler, ctx, actor)
+            await wrap_sync_function_in_async(self.handler, ctx, pipeline)
         elif handler_params == 3:
-            await wrap_sync_function_in_async(self.handler, ctx, actor, self._get_runtime_info(ctx))
+            await wrap_sync_function_in_async(self.handler, ctx, pipeline, self._get_runtime_info(ctx))
         else:
             raise Exception(f"Too many parameters required for service '{self.name}' handler: {handler_params}!")
 
-    def _run_as_actor(self, ctx: Context):
+    def _run_as_actor(self, ctx: Context, pipeline: Pipeline):
         """
         Method for running this service if its handler is an `Actor`.
         Catches runtime exceptions.
 
         :param ctx: Current dialog context.
         :return: Context, mutated by actor.
         """
         try:
-            ctx = self.handler(ctx)
+            ctx = pipeline.actor(pipeline, ctx)
             self._set_state(ctx, ComponentExecutionState.FINISHED)
         except Exception as exc:
             self._set_state(ctx, ComponentExecutionState.FAILED)
             logger.error(f"Actor '{self.name}' execution failed!\n{exc}")
         return ctx
 
-    async def _run_as_service(self, ctx: Context, actor: Actor):
+    async def _run_as_service(self, ctx: Context, pipeline: Pipeline):
         """
         Method for running this service if its handler is not an Actor.
         Checks start condition and catches runtime exceptions.
 
         :param ctx: Current dialog context.
-        :param actor: Current pipeline's actor.
+        :param pipeline: Current pipeline.
         :return: `None`
         """
         try:
-            if self.start_condition(ctx, actor):
+            if self.start_condition(ctx, pipeline):
                 self._set_state(ctx, ComponentExecutionState.RUNNING)
-                await self._run_handler(ctx, actor)
+                await self._run_handler(ctx, pipeline)
                 self._set_state(ctx, ComponentExecutionState.FINISHED)
             else:
                 self._set_state(ctx, ComponentExecutionState.NOT_RUN)
         except Exception as e:
             self._set_state(ctx, ComponentExecutionState.FAILED)
             logger.error(f"Service '{self.name}' execution failed!\n{e}")
 
-    async def _run(self, ctx: Context, actor: Optional[Actor] = None) -> Optional[Context]:
+    async def _run(self, ctx: Context, pipeline: Optional[Pipeline] = None) -> Optional[Context]:
         """
         Method for handling this service execution.
         Executes before and after execution wrappers, launches `_run_as_actor` or `_run_as_service` method.
 
         :param ctx: (required) Current dialog context.
-        :param actor: Actor, associated with the pipeline.
+        :param pipeline: the current pipeline.
         :return: `Context` if this service's handler is an `Actor` else `None`.
         """
-        await self.run_extra_handler(ExtraHandlerType.BEFORE, ctx, actor)
+        await self.run_extra_handler(ExtraHandlerType.BEFORE, ctx, pipeline)
 
-        if isinstance(self.handler, Actor):
-            ctx = self._run_as_actor(ctx)
+        if isinstance(self.handler, str) and self.handler == "ACTOR":
+            ctx = self._run_as_actor(ctx, pipeline)
         else:
-            await self._run_as_service(ctx, actor)
+            await self._run_as_service(ctx, pipeline)
 
-        await self.run_extra_handler(ExtraHandlerType.AFTER, ctx, actor)
+        await self.run_extra_handler(ExtraHandlerType.AFTER, ctx, pipeline)
 
-        if isinstance(self.handler, Actor):
+        if isinstance(self.handler, str) and self.handler == "ACTOR":
             return ctx
 
     @property
     def info_dict(self) -> dict:
         """
         See `Component.info_dict` property.
         Adds `handler` key to base info dictionary.
         """
         representation = super(Service, self).info_dict
-        if isinstance(self.handler, Actor):
-            service_representation = f"Instance of {type(self.handler).__name__}"
+        if isinstance(self.handler, str) and self.handler == "ACTOR":
+            service_representation = "Instance of Actor"
         elif isinstance(self.handler, Callable):
             service_representation = f"Callable '{self.handler.__name__}'"
         else:
             service_representation = "[Unknown]"
         representation.update({"handler": service_representation})
         return representation
```

### Comparing `dff-0.3.2/dff/pipeline/service/utils.py` & `dff-0.4.1/dff/pipeline/service/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """
 Utility Functions
 -----------------
-The Utility Functions module contains several utility functions that are commonly used throughout the `DFF`.
+The Utility Functions module contains several utility functions that are commonly used throughout the DFF.
 These functions provide a variety of utility functionality.
 """
 import asyncio
 from typing import Callable, Any, Optional, Tuple, Mapping
 
 
 async def wrap_sync_function_in_async(function: Callable, *args, **kwargs) -> Any:
     """
     Utility function, that wraps both functions and coroutines in coroutines.
     Invokes `function` if it is just a callable and awaits, if this is a coroutine.
 
     :param function: Callable to wrap.
     :param \\*args: Function args.
     :param \\**kwargs: Function kwargs.
-    :return: What `function` returns.
+    :return: What function returns.
     """
     if asyncio.iscoroutinefunction(function):
         return await function(*args, **kwargs)
     else:
         return function(*args, **kwargs)
```

### Comparing `dff-0.3.2/dff/pipeline/types.py` & `dff-0.4.1/dff/pipeline/types.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,20 +6,22 @@
 data structures, and other types that are defined for type hinting.
 """
 from abc import ABC
 from enum import unique, Enum, auto
 from typing import Callable, Union, Awaitable, Dict, List, Optional, NewType, Iterable
 
 from dff.context_storages import DBContextStorage
-from dff.script import Context, Actor
+from dff.script import Context, ActorStage, NodeLabel2Type, Script
 from typing_extensions import NotRequired, TypedDict, TypeAlias
 
 
+_ForwardPipeline = NewType("Pipeline", None)
 _ForwardPipelineComponent = NewType("PipelineComponent", None)
 _ForwardService = NewType("Service", _ForwardPipelineComponent)
+_ForwardServiceBuilder = NewType("ServiceBuilder", None)
 _ForwardServiceGroup = NewType("ServiceGroup", _ForwardPipelineComponent)
 _ForwardComponentExtraHandler = NewType("_ComponentExtraHandler", None)
 _ForwardProvider = NewType("ABCProvider", ABC)
 _ForwardExtraHandlerFunction = NewType("ExtraHandlerFunction", None)
 
 
 @unique
@@ -78,18 +80,18 @@
 PIPELINE_STATE_KEY = "PIPELINE"
 """
 PIPELINE: storage for services and groups execution status.
 Should be used in `ctx.framework_keys[PIPELINE_STATE_KEY]`.
 """
 
 
-StartConditionCheckerFunction: TypeAlias = Callable[[Context, Actor], bool]
+StartConditionCheckerFunction: TypeAlias = Callable[[Context, _ForwardPipeline], bool]
 """
 A function type for components `start_conditions`.
-Accepts context and actor (current pipeline state), returns boolean (whether service can be launched).
+Accepts context and pipeline, returns boolean (whether service can be launched).
 """
 
 
 StartConditionCheckerAggregationFunction: TypeAlias = Callable[[Iterable[bool]], bool]
 """
 A function type for creating aggregation `start_conditions` for components.
 Accepts list of functions (other start_conditions to aggregate), returns boolean (whether service can be launched).
@@ -136,34 +138,34 @@
 Contains current wrapper info (`name`, `stage`).
 Also contains `component` - runtime info dictionary of the component this wrapper is attached to.
 """
 
 
 ExtraHandlerFunction: TypeAlias = Union[
     Callable[[Context], None],
-    Callable[[Context, Actor], None],
-    Callable[[Context, Actor, ExtraHandlerRuntimeInfo], None],
+    Callable[[Context, _ForwardPipeline], None],
+    Callable[[Context, _ForwardPipeline, ExtraHandlerRuntimeInfo], None],
 ]
 """
 A function type for creating wrappers (before and after functions).
-Can accept current dialog context, actor, attached to the pipeline, and current wrapper info dictionary.
+Can accept current dialog context, pipeline, and current wrapper info dictionary.
 """
 
 
 ServiceFunction: TypeAlias = Union[
     Callable[[Context], None],
     Callable[[Context], Awaitable[None]],
-    Callable[[Context, Actor], None],
-    Callable[[Context, Actor], Awaitable[None]],
-    Callable[[Context, Actor, ServiceRuntimeInfo], None],
-    Callable[[Context, Actor, ServiceRuntimeInfo], Awaitable[None]],
+    Callable[[Context, _ForwardPipeline], None],
+    Callable[[Context, _ForwardPipeline], Awaitable[None]],
+    Callable[[Context, _ForwardPipeline, ServiceRuntimeInfo], None],
+    Callable[[Context, _ForwardPipeline, ServiceRuntimeInfo], Awaitable[None]],
 ]
 """
 A function type for creating service handlers.
-Can accept current dialog context, actor, attached to the pipeline, and current service info dictionary.
+Can accept current dialog context, pipeline, and current service info dictionary.
 Can be both synchronous and asynchronous.
 """
 
 
 ExtraHandlerBuilder: TypeAlias = Union[
     _ForwardComponentExtraHandler,
     TypedDict(
@@ -184,19 +186,19 @@
 - Dictionary, containing keys `timeout`, `asynchronous`, `functions`
 """
 
 
 ServiceBuilder: TypeAlias = Union[
     ServiceFunction,
     _ForwardService,
-    Actor,
+    str,
     TypedDict(
         "ServiceDict",
         {
-            "handler": "ServiceBuilder",
+            "handler": _ForwardServiceBuilder,
             "before_handler": NotRequired[Optional[ExtraHandlerBuilder]],
             "after_handler": NotRequired[Optional[ExtraHandlerBuilder]],
             "timeout": NotRequired[Optional[float]],
             "asynchronous": NotRequired[bool],
             "start_condition": NotRequired[StartConditionCheckerFunction],
             "name": Optional[str],
         },
@@ -204,15 +206,15 @@
 ]
 """
 A type, representing anything that can be transformed to service.
 It can be:
 
 - ServiceFunction (will become handler)
 - Service object (will be spread and recreated)
-- Actor (will be wrapped in a Service as a handler)
+- String 'ACTOR' - the pipeline Actor will be placed there
 - Dictionary, containing keys that are present in Service constructor parameters
 """
 
 
 ServiceGroupBuilder: TypeAlias = Union[
     List[Union[ServiceBuilder, List[ServiceBuilder], _ForwardServiceGroup]],
     _ForwardServiceGroup,
@@ -231,13 +233,21 @@
     {
         "messenger_interface": NotRequired[Optional[_ForwardProvider]],
         "context_storage": NotRequired[Optional[Union[DBContextStorage, Dict]]],
         "components": ServiceGroupBuilder,
         "before_handler": NotRequired[Optional[ExtraHandlerBuilder]],
         "after_handler": NotRequired[Optional[ExtraHandlerBuilder]],
         "optimization_warnings": NotRequired[bool],
+        "script": Union[Script, Dict],
+        "start_label": NodeLabel2Type,
+        "fallback_label": NotRequired[Optional[NodeLabel2Type]],
+        "label_priority": NotRequired[float],
+        "validation_stage": NotRequired[Optional[bool]],
+        "condition_handler": NotRequired[Optional[Callable]],
+        "verbose": NotRequired[bool],
+        "handlers": NotRequired[Optional[Dict[ActorStage, List[Callable]]]],
     },
 )
 """
 A type, representing anything that can be transformed to pipeline.
 It can be Dictionary, containing keys that are present in Pipeline constructor parameters.
 """
```

### Comparing `dff-0.3.2/dff/script/__init__.py` & `dff-0.4.1/dff/script/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # -*- coding: utf-8 -*-
 # flake8: noqa: F401
 
-from .core.actor import Actor
 from .core.context import Context
 from .core.keywords import (
     Keywords,
     GLOBAL,
     LOCAL,
     TRANSITIONS,
     RESPONSE,
```

### Comparing `dff-0.3.2/dff/script/conditions/std_conditions.py` & `dff-0.4.1/dff/script/conditions/std_conditions.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,31 +10,32 @@
 """
 from typing import Callable, Pattern, Union, Any, List, Optional
 import logging
 import re
 
 from pydantic import validate_arguments
 
-from dff.script import NodeLabel2Type, Actor, Context, Message
+from dff.pipeline import Pipeline
+from dff.script import NodeLabel2Type, Context, Message
 
 logger = logging.getLogger(__name__)
 
 
 @validate_arguments
 def exact_match(match: Message, skip_none: bool = True, *args, **kwargs) -> Callable[..., bool]:
     """
-    Returns function handler. This handler returns `True` only if the last user phrase
+    Return function handler. This handler returns `True` only if the last user phrase
     is the same Message as the :py:const:`match`.
     If :py:const:`skip_none` the handler will not compare `None` fields of :py:const:`match`.
 
     :param match: A Message variable to compare user request with.
     :param skip_none: Whether fields should be compared if they are `None` in :py:const:`match`.
     """
 
-    def exact_match_condition_handler(ctx: Context, actor: Actor, *args, **kwargs) -> bool:
+    def exact_match_condition_handler(ctx: Context, pipeline: Pipeline, *args, **kwargs) -> bool:
         request = ctx.last_request
         if request is None:
             return False
         for field in match.__fields__:
             match_value = match.__getattribute__(field)
             if skip_none and match_value is None:
                 continue
@@ -47,25 +48,25 @@
 
     return exact_match_condition_handler
 
 
 @validate_arguments
 def regexp(
     pattern: Union[str, Pattern], flags: Union[int, re.RegexFlag] = 0, *args, **kwargs
-) -> Callable[[Context, Actor, Any, Any], bool]:
+) -> Callable[[Context, Pipeline, Any, Any], bool]:
     """
-    Returns function handler. This handler returns `True` only if the last user phrase contains
+    Return function handler. This handler returns `True` only if the last user phrase contains
     :py:const:`pattern <Union[str, Pattern]>` with :py:const:`flags <Union[int, re.RegexFlag]>`.
 
     :param pattern: The `RegExp` pattern.
     :param flags: Flags for this pattern. Defaults to 0.
     """
     pattern = re.compile(pattern, flags)
 
-    def regexp_condition_handler(ctx: Context, actor: Actor, *args, **kwargs) -> bool:
+    def regexp_condition_handler(ctx: Context, pipeline: Pipeline, *args, **kwargs) -> bool:
         request = ctx.last_request
         if isinstance(request, Message):
             if request.text is None:
                 return False
             return bool(pattern.search(request.text))
         else:
             logger.error(f"request has to be str type, but got request={request}")
@@ -73,15 +74,15 @@
 
     return regexp_condition_handler
 
 
 @validate_arguments
 def check_cond_seq(cond_seq: list):
     """
-    Checks if the list consists only of Callables.
+    Check if the list consists only of Callables.
 
     :param cond_seq: List of conditions to check.
     """
     for cond in cond_seq:
         if not isinstance(cond, Callable):
             raise TypeError(f"{cond_seq} has to consist of callable objects")
 
@@ -95,140 +96,138 @@
 _all is an alias for all.
 """
 
 
 @validate_arguments
 def aggregate(
     cond_seq: list, aggregate_func: Callable = _any, *args, **kwargs
-) -> Callable[[Context, Actor, Any, Any], bool]:
+) -> Callable[[Context, Pipeline, Any, Any], bool]:
     """
-    Aggregates multiple functions into one by using aggregating function.
+    Aggregate multiple functions into one by using aggregating function.
 
     :param cond_seq: List of conditions to check.
     :param aggregate_func: Function to aggregate conditions. Defaults to :py:func:`_any`.
     """
     check_cond_seq(cond_seq)
 
-    def aggregate_condition_handler(ctx: Context, actor: Actor, *args, **kwargs) -> bool:
+    def aggregate_condition_handler(ctx: Context, pipeline: Pipeline, *args, **kwargs) -> bool:
         try:
-            return bool(aggregate_func([cond(ctx, actor, *args, **kwargs) for cond in cond_seq]))
+            return bool(aggregate_func([cond(ctx, pipeline, *args, **kwargs) for cond in cond_seq]))
         except Exception as exc:
             logger.error(f"Exception {exc} for {cond_seq}, {aggregate_func} and {ctx.last_request}", exc_info=exc)
             return False
 
     return aggregate_condition_handler
 
 
 @validate_arguments
-def any(cond_seq: list, *args, **kwargs) -> Callable[[Context, Actor, Any, Any], bool]:
+def any(cond_seq: list, *args, **kwargs) -> Callable[[Context, Pipeline, Any, Any], bool]:
     """
-    Returns function handler. This handler returns `True`
+    Return function handler. This handler returns `True`
     if any function from the list is `True`.
 
     :param cond_seq: List of conditions to check.
     """
     _agg = aggregate(cond_seq, _any)
 
-    def any_condition_handler(ctx: Context, actor: Actor, *args, **kwargs) -> bool:
-        return _agg(ctx, actor, *args, **kwargs)
+    def any_condition_handler(ctx: Context, pipeline: Pipeline, *args, **kwargs) -> bool:
+        return _agg(ctx, pipeline, *args, **kwargs)
 
     return any_condition_handler
 
 
 @validate_arguments
-def all(cond_seq: list, *args, **kwargs) -> Callable[[Context, Actor, Any, Any], bool]:
+def all(cond_seq: list, *args, **kwargs) -> Callable[[Context, Pipeline, Any, Any], bool]:
     """
-    Returns function handler. This handler returns `True` only
+    Return function handler. This handler returns `True` only
     if all functions from the list are `True`.
 
     :param cond_seq: List of conditions to check.
     """
     _agg = aggregate(cond_seq, _all)
 
-    def all_condition_handler(ctx: Context, actor: Actor, *args, **kwargs) -> bool:
-        return _agg(ctx, actor, *args, **kwargs)
+    def all_condition_handler(ctx: Context, pipeline: Pipeline, *args, **kwargs) -> bool:
+        return _agg(ctx, pipeline, *args, **kwargs)
 
     return all_condition_handler
 
 
 @validate_arguments
-def negation(condition: Callable, *args, **kwargs) -> Callable[[Context, Actor, Any, Any], bool]:
+def negation(condition: Callable, *args, **kwargs) -> Callable[[Context, Pipeline, Any, Any], bool]:
     """
-    Returns function handler. This handler returns negation of the :py:func:`~condition`: `False`
+    Return function handler. This handler returns negation of the :py:func:`~condition`: `False`
     if :py:func:`~condition` holds `True` and returns `True` otherwise.
 
     :param condition: Any :py:func:`~condition`.
     """
 
-    def negation_condition_handler(ctx: Context, actor: Actor, *args, **kwargs) -> bool:
-        return not condition(ctx, actor, *args, **kwargs)
+    def negation_condition_handler(ctx: Context, pipeline: Pipeline, *args, **kwargs) -> bool:
+        return not condition(ctx, pipeline, *args, **kwargs)
 
     return negation_condition_handler
 
 
 @validate_arguments
 def has_last_labels(
     flow_labels: Optional[List[str]] = None,
     labels: Optional[List[NodeLabel2Type]] = None,
     last_n_indices: int = 1,
     *args,
     **kwargs,
-) -> Callable[[Context, Actor, Any, Any], bool]:
+) -> Callable[[Context, Pipeline, Any, Any], bool]:
     """
-    Returns condition handler. This handler returns `True` if any label from
+    Return condition handler. This handler returns `True` if any label from
     last :py:const:`last_n_indices` context labels is in
     the :py:const:`flow_labels` list or in
     the :py:const:`~dff.script.NodeLabel2Type` list.
 
     :param flow_labels: List of labels to check. Every label has type `str`. Empty if not set.
     :param labels: List of labels corresponding to the nodes. Empty if not set.
     :param last_n_indices: Number of last utterances to check.
     """
     flow_labels = [] if flow_labels is None else flow_labels
     labels = [] if labels is None else labels
 
-    def has_last_labels_condition_handler(ctx: Context, actor: Actor, *args, **kwargs) -> bool:
+    def has_last_labels_condition_handler(ctx: Context, pipeline: Pipeline, *args, **kwargs) -> bool:
         label = list(ctx.labels.values())[-last_n_indices:]
         for label in list(ctx.labels.values())[-last_n_indices:]:
             label = label if label else (None, None)
             if label[0] in flow_labels or label in labels:
                 return True
         return False
 
     return has_last_labels_condition_handler
 
 
 @validate_arguments
-def true(*args, **kwargs) -> Callable[[Context, Actor, Any, Any], bool]:
+def true(*args, **kwargs) -> Callable[[Context, Pipeline, Any, Any], bool]:
     """
-    Returns function handler. This handler always returns `True`.
+    Return function handler. This handler always returns `True`.
     """
 
-    def true_handler(ctx: Context, actor: Actor, *args, **kwargs) -> bool:
+    def true_handler(ctx: Context, pipeline: Pipeline, *args, **kwargs) -> bool:
         return True
 
     return true_handler
 
 
 @validate_arguments
-def false(*args, **kwargs) -> Callable[[Context, Actor, Any, Any], bool]:
+def false(*args, **kwargs) -> Callable[[Context, Pipeline, Any, Any], bool]:
     """
-    Returns function handler. This handler always returns `False`.
+    Return function handler. This handler always returns `False`.
     """
 
-    def false_handler(ctx: Context, actor: Actor, *args, **kwargs) -> bool:
+    def false_handler(ctx: Context, pipeline: Pipeline, *args, **kwargs) -> bool:
         return False
 
     return false_handler
 
 
 # aliases
 agg = aggregate
 """
 :py:func:`~agg` is an alias for :py:func:`~aggregate`.
-:rtype:
 """
 neg = negation
 """
 :py:func:`~neg` is an alias for :py:func:`~negation`.
-:rtype:
 """
```

### Comparing `dff-0.3.2/dff/script/core/actor.py` & `dff-0.4.1/dff/pipeline/pipeline/actor.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,30 +14,30 @@
 for a transition to occur. The actor uses this information to navigate the graph
 and determine the next step in the conversation.
 
 Overall, the actor acts as a bridge between the user's input and the dialog graph,
 making sure that the conversation follows the expected flow and providing a personalized experience to the user.
 """
 import logging
-from typing import Union, Callable, Optional, Dict, List, Any
+from typing import Union, Callable, Optional, Dict, List, Any, ForwardRef
 import copy
 
-from pydantic import BaseModel, validate_arguments, Extra
-
 from dff.utils.turn_caching import cache_clear
-from .types import ActorStage, NodeLabel2Type, NodeLabel3Type, LabelType
-from .message import Message
+from dff.script.core.types import ActorStage, NodeLabel2Type, NodeLabel3Type, LabelType
+from dff.script.core.message import Message
 
-from .context import Context
-from .script import Script, Node
-from .normalization import normalize_label, normalize_response
-from .keywords import GLOBAL, LOCAL
+from dff.script.core.context import Context
+from dff.script.core.script import Script, Node
+from dff.script.core.normalization import normalize_label, normalize_response
+from dff.script.core.keywords import GLOBAL, LOCAL
 
 logger = logging.getLogger(__name__)
 
+Pipeline = ForwardRef("Pipeline")
+
 
 def error_handler(error_msgs: list, msg: str, exception: Optional[Exception] = None, logging_flag: bool = True):
     """
     This function handles errors during :py:class:`~dff.script.Script` validation.
 
     :param error_msgs: List that contains error messages. :py:func:`~dff.script.error_handler`
         adds every next error message to that list.
@@ -47,253 +47,200 @@
     :param logging_flag: The flag which defines whether logging is necessary. Defaults to `True`.
     """
     error_msgs.append(msg)
     if logging_flag:
         logger.error(msg, exc_info=exception)
 
 
-class Actor(BaseModel):
+class Actor:
     """
     The class which is used to process :py:class:`~dff.script.Context`
     according to the :py:class:`~dff.script.Script`.
-    """
-
-    class Config:
-        extra = Extra.allow
-
-    script: Union[Script, dict]
-    """
-    The dialog scenario: a graph described by the :py:class:~dff.script.Keywords.
-    While the graph is being initialized, it is validated and then used for the dialog.
-    """
-    start_label: NodeLabel3Type
-    """
-    The start node of :py:class:`~dff.script.Script`. The execution begins with it.
-    """
-    fallback_label: Optional[NodeLabel3Type] = None
-    """
-    The label of :py:class:`~dff.script.Script`.
-    Dialog comes into that label if all other transitions failed, or there was an error while executing the scenario.
-    Defaults to `None`.
-    """
-    label_priority: float = 1.0
-    """
-    Default priority value for all :py:const:`labels <dff.script.NodeLabel3Type>`
-    where there is no priority. Defaults to `1.0`.
-    """
-    validation_stage: Optional[bool] = None
-    """
-    This flag sets whether the validation stage is executed. It is executed by default. Defaults to `None`.
-    """
-    condition_handler: Optional[Callable] = None
-    """
-    Handler that processes a call of condition functions. Defaults to `None`.
-    """
-    verbose: bool = True
-    """
-    If it is `True`, logging is used. Defaults to `True`.
-    """
-    handlers: Dict[ActorStage, List[Callable]] = {}
-    """
-    This variable is responsible for the usage of external handlers on
-    the certain stages of work of :py:class:`~dff.script.Actor`.
 
-        - key: :py:class:`~dff.script.ActorStage` - Stage in which the handler is called.
-        - value: List[Callable] - The list of called handlers for each stage.
+    :param script: The dialog scenario: a graph described by the :py:class:`.Keywords`.
+        While the graph is being initialized, it is validated and then used for the dialog.
+    :param start_label: The start node of :py:class:`~dff.script.Script`. The execution begins with it.
+    :param fallback_label: The label of :py:class:`~dff.script.Script`.
+        Dialog comes into that label if all other transitions failed,
+        or there was an error while executing the scenario.
+        Defaults to `None`.
+    :param label_priority: Default priority value for all :py:const:`labels <dff.script.NodeLabel3Type>`
+        where there is no priority. Defaults to `1.0`.
+    :param condition_handler: Handler that processes a call of condition functions. Defaults to `None`.
+    :param handlers: This variable is responsible for the usage of external handlers on
+        the certain stages of work of :py:class:`~dff.script.Actor`.
 
-    Defaults to an empty `dict`.
+        - key (:py:class:`~dff.script.ActorStage`) - Stage in which the handler is called.
+        - value (List[Callable]) - The list of called handlers for each stage.  Defaults to an empty `dict`.
     """
 
-    @validate_arguments
     def __init__(
         self,
         script: Union[Script, dict],
         start_label: NodeLabel2Type,
         fallback_label: Optional[NodeLabel2Type] = None,
         label_priority: float = 1.0,
-        validation_stage: Optional[bool] = None,
         condition_handler: Optional[Callable] = None,
-        verbose: bool = True,
         handlers: Optional[Dict[ActorStage, List[Callable]]] = None,
-        *args,
-        **kwargs,
     ):
         # script validation
-        script = script if isinstance(script, Script) else Script(script=script)
+        self.script = script if isinstance(script, Script) else Script(script=script)
+        self.label_priority = label_priority
 
         # node labels validation
-        start_label = normalize_label(start_label)
-        if script.get(start_label[0], {}).get(start_label[1]) is None:
-            raise ValueError(f"Unkown start_label={start_label}")
+        self.start_label = normalize_label(start_label)
+        if self.script.get(self.start_label[0], {}).get(self.start_label[1]) is None:
+            raise ValueError(f"Unknown start_label={self.start_label}")
+
         if fallback_label is None:
-            fallback_label = start_label
+            self.fallback_label = self.start_label
         else:
-            fallback_label = normalize_label(fallback_label)
-            if script.get(fallback_label[0], {}).get(fallback_label[1]) is None:
-                raise ValueError(f"Unkown fallback_label={fallback_label}")
-        if condition_handler is None:
-            condition_handler = default_condition_handler
-
-        super(Actor, self).__init__(
-            script=script,
-            start_label=start_label,
-            fallback_label=fallback_label,
-            label_priority=label_priority,
-            validation_stage=validation_stage,
-            condition_handler=condition_handler,
-            verbose=verbose,
-            handlers={} if handlers is None else handlers,
-        )
+            self.fallback_label = normalize_label(fallback_label)
+            if self.script.get(self.fallback_label[0], {}).get(self.fallback_label[1]) is None:
+                raise ValueError(f"Unknown fallback_label={self.fallback_label}")
+        self.condition_handler = default_condition_handler if condition_handler is None else condition_handler
+
+        self.handlers = {} if handlers is None else handlers
 
         # NB! The following API is highly experimental and may be removed at ANY time WITHOUT FURTHER NOTICE!!
         self._clean_turn_cache = True
 
-        errors = self.validate_script(verbose) if validation_stage or validation_stage is None else []
-        if errors:
-            raise ValueError(
-                f"Found len(errors)={len(errors)} errors: " + " ".join([f"{i}) {er}" for i, er in enumerate(errors, 1)])
-            )
-
-    @validate_arguments
-    def __call__(self, ctx: Optional[Union[Context, dict, str]] = None, *args, **kwargs) -> Union[Context, dict, str]:
+    def __call__(
+        self, pipeline: Pipeline, ctx: Optional[Union[Context, dict, str]] = None, *args, **kwargs
+    ) -> Union[Context, dict, str]:
 
         # context init
         ctx = self._context_init(ctx, *args, **kwargs)
-        self._run_handlers(ctx, ActorStage.CONTEXT_INIT, *args, **kwargs)
+        self._run_handlers(ctx, pipeline, ActorStage.CONTEXT_INIT, *args, **kwargs)
 
         # get previous node
         ctx = self._get_previous_node(ctx, *args, **kwargs)
-        self._run_handlers(ctx, ActorStage.GET_PREVIOUS_NODE, *args, **kwargs)
+        self._run_handlers(ctx, pipeline, ActorStage.GET_PREVIOUS_NODE, *args, **kwargs)
 
         # rewrite previous node
         ctx = self._rewrite_previous_node(ctx, *args, **kwargs)
-        self._run_handlers(ctx, ActorStage.REWRITE_PREVIOUS_NODE, *args, **kwargs)
+        self._run_handlers(ctx, pipeline, ActorStage.REWRITE_PREVIOUS_NODE, *args, **kwargs)
 
         # run pre transitions processing
-        ctx = self._run_pre_transitions_processing(ctx, *args, **kwargs)
-        self._run_handlers(ctx, ActorStage.RUN_PRE_TRANSITIONS_PROCESSING, *args, **kwargs)
+        ctx = self._run_pre_transitions_processing(ctx, pipeline, *args, **kwargs)
+        self._run_handlers(ctx, pipeline, ActorStage.RUN_PRE_TRANSITIONS_PROCESSING, *args, **kwargs)
 
         # get true labels for scopes (GLOBAL, LOCAL, NODE)
-        ctx = self._get_true_labels(ctx, *args, **kwargs)
-        self._run_handlers(ctx, ActorStage.GET_TRUE_LABELS, *args, **kwargs)
+        ctx = self._get_true_labels(ctx, pipeline, *args, **kwargs)
+        self._run_handlers(ctx, pipeline, ActorStage.GET_TRUE_LABELS, *args, **kwargs)
 
         # get next node
         ctx = self._get_next_node(ctx, *args, **kwargs)
-        self._run_handlers(ctx, ActorStage.GET_NEXT_NODE, *args, **kwargs)
+        self._run_handlers(ctx, pipeline, ActorStage.GET_NEXT_NODE, *args, **kwargs)
 
         ctx.add_label(ctx.framework_states["actor"]["next_label"][:2])
 
         # rewrite next node
         ctx = self._rewrite_next_node(ctx, *args, **kwargs)
-        self._run_handlers(ctx, ActorStage.REWRITE_NEXT_NODE, *args, **kwargs)
+        self._run_handlers(ctx, pipeline, ActorStage.REWRITE_NEXT_NODE, *args, **kwargs)
 
         # run pre response processing
-        ctx = self._run_pre_response_processing(ctx, *args, **kwargs)
-        self._run_handlers(ctx, ActorStage.RUN_PRE_RESPONSE_PROCESSING, *args, **kwargs)
+        ctx = self._run_pre_response_processing(ctx, pipeline, *args, **kwargs)
+        self._run_handlers(ctx, pipeline, ActorStage.RUN_PRE_RESPONSE_PROCESSING, *args, **kwargs)
 
         # create response
         ctx.framework_states["actor"]["response"] = ctx.framework_states["actor"][
             "pre_response_processed_node"
-        ].run_response(ctx, self, *args, **kwargs)
-        self._run_handlers(ctx, ActorStage.CREATE_RESPONSE, *args, **kwargs)
+        ].run_response(ctx, pipeline, *args, **kwargs)
+        self._run_handlers(ctx, pipeline, ActorStage.CREATE_RESPONSE, *args, **kwargs)
         ctx.add_response(ctx.framework_states["actor"]["response"])
 
-        self._run_handlers(ctx, ActorStage.FINISH_TURN, *args, **kwargs)
+        self._run_handlers(ctx, pipeline, ActorStage.FINISH_TURN, *args, **kwargs)
         if self._clean_turn_cache:
             cache_clear()
 
         del ctx.framework_states["actor"]
         return ctx
 
-    @validate_arguments
     def _context_init(self, ctx: Optional[Union[Context, dict, str]] = None, *args, **kwargs) -> Context:
         ctx = Context.cast(ctx)
         if not ctx.requests:
             ctx.add_label(self.start_label[:2])
             ctx.add_request(Message())
         ctx.framework_states["actor"] = {}
         return ctx
 
-    @validate_arguments
     def _get_previous_node(self, ctx: Context, *args, **kwargs) -> Context:
         ctx.framework_states["actor"]["previous_label"] = (
             normalize_label(ctx.last_label) if ctx.last_label else self.start_label
         )
         ctx.framework_states["actor"]["previous_node"] = self.script.get(
             ctx.framework_states["actor"]["previous_label"][0], {}
         ).get(ctx.framework_states["actor"]["previous_label"][1], Node())
         return ctx
 
-    @validate_arguments
-    def _get_true_labels(self, ctx: Context, *args, **kwargs) -> Context:
+    def _get_true_labels(self, ctx: Context, pipeline: Pipeline, *args, **kwargs) -> Context:
         # GLOBAL
         ctx.framework_states["actor"]["global_transitions"] = (
             self.script.get(GLOBAL, {}).get(GLOBAL, Node()).transitions
         )
         ctx.framework_states["actor"]["global_true_label"] = self._get_true_label(
-            ctx.framework_states["actor"]["global_transitions"], ctx, GLOBAL, "global"
+            ctx.framework_states["actor"]["global_transitions"], ctx, pipeline, GLOBAL, "global"
         )
 
         # LOCAL
         ctx.framework_states["actor"]["local_transitions"] = (
             self.script.get(ctx.framework_states["actor"]["previous_label"][0], {}).get(LOCAL, Node()).transitions
         )
         ctx.framework_states["actor"]["local_true_label"] = self._get_true_label(
             ctx.framework_states["actor"]["local_transitions"],
             ctx,
+            pipeline,
             ctx.framework_states["actor"]["previous_label"][0],
             "local",
         )
 
         # NODE
         ctx.framework_states["actor"]["node_transitions"] = ctx.framework_states["actor"][
             "pre_transitions_processed_node"
         ].transitions
         ctx.framework_states["actor"]["node_true_label"] = self._get_true_label(
             ctx.framework_states["actor"]["node_transitions"],
             ctx,
+            pipeline,
             ctx.framework_states["actor"]["previous_label"][0],
             "node",
         )
         return ctx
 
-    @validate_arguments
     def _get_next_node(self, ctx: Context, *args, **kwargs) -> Context:
         # choose next label
         ctx.framework_states["actor"]["next_label"] = self._choose_label(
             ctx.framework_states["actor"]["node_true_label"], ctx.framework_states["actor"]["local_true_label"]
         )
         ctx.framework_states["actor"]["next_label"] = self._choose_label(
             ctx.framework_states["actor"]["next_label"], ctx.framework_states["actor"]["global_true_label"]
         )
         # get next node
         ctx.framework_states["actor"]["next_node"] = self.script.get(
             ctx.framework_states["actor"]["next_label"][0], {}
         ).get(ctx.framework_states["actor"]["next_label"][1])
         return ctx
 
-    @validate_arguments
     def _rewrite_previous_node(self, ctx: Context, *args, **kwargs) -> Context:
         node = ctx.framework_states["actor"]["previous_node"]
         flow_label = ctx.framework_states["actor"]["previous_label"][0]
         ctx.framework_states["actor"]["previous_node"] = self._overwrite_node(
             node,
             flow_label,
             only_current_node_transitions=True,
         )
         return ctx
 
-    @validate_arguments
     def _rewrite_next_node(self, ctx: Context, *args, **kwargs) -> Context:
         node = ctx.framework_states["actor"]["next_node"]
         flow_label = ctx.framework_states["actor"]["next_label"][0]
         ctx.framework_states["actor"]["next_node"] = self._overwrite_node(node, flow_label)
         return ctx
 
-    @validate_arguments
     def _overwrite_node(
         self,
         current_node: Node,
         flow_label: LabelType,
         *args,
         only_current_node_transitions: bool = False,
         **kwargs,
@@ -307,41 +254,47 @@
             overwritten_node.misc.update(node.misc)
             if not only_current_node_transitions:
                 overwritten_node.transitions.update(node.transitions)
         if only_current_node_transitions:
             overwritten_node.transitions = current_node.transitions
         return overwritten_node
 
-    @validate_arguments
-    def _run_pre_transitions_processing(self, ctx: Context, *args, **kwargs) -> Context:
+    def _run_pre_transitions_processing(self, ctx: Context, pipeline: Pipeline, *args, **kwargs) -> Context:
         ctx.framework_states["actor"]["processed_node"] = copy.deepcopy(ctx.framework_states["actor"]["previous_node"])
-        ctx = ctx.framework_states["actor"]["previous_node"].run_pre_transitions_processing(ctx, self, *args, **kwargs)
+        ctx = ctx.framework_states["actor"]["previous_node"].run_pre_transitions_processing(
+            ctx, pipeline, *args, **kwargs
+        )
         ctx.framework_states["actor"]["pre_transitions_processed_node"] = ctx.framework_states["actor"][
             "processed_node"
         ]
         del ctx.framework_states["actor"]["processed_node"]
         return ctx
 
-    @validate_arguments
-    def _run_pre_response_processing(self, ctx: Context, *args, **kwargs) -> Context:
+    def _run_pre_response_processing(self, ctx: Context, pipeline: Pipeline, *args, **kwargs) -> Context:
         ctx.framework_states["actor"]["processed_node"] = copy.deepcopy(ctx.framework_states["actor"]["next_node"])
-        ctx = ctx.framework_states["actor"]["next_node"].run_pre_response_processing(ctx, self, *args, **kwargs)
+        ctx = ctx.framework_states["actor"]["next_node"].run_pre_response_processing(ctx, pipeline, *args, **kwargs)
         ctx.framework_states["actor"]["pre_response_processed_node"] = ctx.framework_states["actor"]["processed_node"]
         del ctx.framework_states["actor"]["processed_node"]
         return ctx
 
-    @validate_arguments
     def _get_true_label(
-        self, transitions: dict, ctx: Context, flow_label: LabelType, transition_info: str = "", *args, **kwargs
+        self,
+        transitions: dict,
+        ctx: Context,
+        pipeline: Pipeline,
+        flow_label: LabelType,
+        transition_info: str = "",
+        *args,
+        **kwargs,
     ) -> Optional[NodeLabel3Type]:
         true_labels = []
         for label, condition in transitions.items():
-            if self.condition_handler(condition, ctx, self, *args, **kwargs):
+            if self.condition_handler(condition, ctx, pipeline, *args, **kwargs):
                 if isinstance(label, Callable):
-                    label = label(ctx, self, *args, **kwargs)
+                    label = label(ctx, pipeline, *args, **kwargs)
                     # TODO: explicit handling of errors
                     if label is None:
                         continue
                 label = normalize_label(label, flow_label)
                 true_labels += [label]
         true_labels = [
             ((label[0] if label[0] else flow_label),)
@@ -350,52 +303,48 @@
             for label in true_labels
         ]
         true_labels.sort(key=lambda label: -label[2])
         true_label = true_labels[0] if true_labels else None
         logger.debug(f"{transition_info} transitions sorted by priority = {true_labels}")
         return true_label
 
-    @validate_arguments
-    def _run_handlers(self, ctx, actor_stade: ActorStage, *args, **kwargs):
-        [handler(ctx, self, *args, **kwargs) for handler in self.handlers.get(actor_stade, [])]
+    def _run_handlers(self, ctx, pipeline: Pipeline, actor_stade: ActorStage, *args, **kwargs):
+        [handler(ctx, pipeline, *args, **kwargs) for handler in self.handlers.get(actor_stade, [])]
 
-    @validate_arguments
     def _choose_label(
         self, specific_label: Optional[NodeLabel3Type], general_label: Optional[NodeLabel3Type]
     ) -> NodeLabel3Type:
         if all([specific_label, general_label]):
             chosen_label = specific_label if specific_label[2] >= general_label[2] else general_label
         elif any([specific_label, general_label]):
             chosen_label = specific_label if specific_label else general_label
         else:
             chosen_label = self.fallback_label
         return chosen_label
 
-    @validate_arguments
-    def validate_script(self, verbose: bool = True):
+    def validate_script(self, pipeline: Pipeline, verbose: bool = True):
         # TODO: script has to not contain priority == -inf, because it uses for miss values
         flow_labels = []
         node_labels = []
         labels = []
         conditions = []
         for flow_name, flow in self.script.items():
             for node_name, node in flow.items():
                 flow_labels += [flow_name] * len(node.transitions)
                 node_labels += [node_name] * len(node.transitions)
                 labels += list(node.transitions.keys())
                 conditions += list(node.transitions.values())
 
-        actor = self.copy(deep=True)
         error_msgs = []
         for flow_label, node_label, label, condition in zip(flow_labels, node_labels, labels, conditions):
             ctx = Context()
             ctx.validation = True
             ctx.add_request(Message(text="text"))
 
-            label = label(ctx, actor) if isinstance(label, Callable) else normalize_label(label, flow_label)
+            label = label(ctx, pipeline) if isinstance(label, Callable) else normalize_label(label, flow_label)
 
             # validate labeling
             try:
                 node = self.script[label[0]][label[1]]
             except Exception as exc:
                 msg = (
                     f"Could not find node with label={label}, "
@@ -403,15 +352,15 @@
                 )
                 error_handler(error_msgs, msg, exc, verbose)
                 break
 
             # validate responsing
             response_func = normalize_response(node.response)
             try:
-                response_result = response_func(ctx, actor)
+                response_result = response_func(ctx, pipeline)
                 if not isinstance(response_result, Message):
                     msg = (
                         "Expected type of response_result is `Message`.\n"
                         + f"Got type(response_result)={type(response_result)}"
                         f" for label={label} , error was found in (flow_label, node_label)={(flow_label, node_label)}"
                     )
                     error_handler(error_msgs, msg, None, verbose)
@@ -423,29 +372,28 @@
                     f", error was found in (flow_label, node_label)={(flow_label, node_label)}"
                 )
                 error_handler(error_msgs, msg, exc, verbose)
                 continue
 
             # validate conditioning
             try:
-                condition_result = condition(ctx, actor)
-                if not isinstance(condition(ctx, actor), bool):
+                condition_result = condition(ctx, pipeline)
+                if not isinstance(condition(ctx, pipeline), bool):
                     raise Exception(f"Returned condition_result={condition_result}, but expected bool type")
             except Exception as exc:
                 msg = f"Got exception '''{exc}''' during condition execution for label={label}"
                 error_handler(error_msgs, msg, exc, verbose)
                 continue
         return error_msgs
 
 
-@validate_arguments()
 def default_condition_handler(
-    condition: Callable, ctx: Context, actor: Actor, *args, **kwargs
-) -> Callable[[Context, Actor, Any, Any], bool]:
+    condition: Callable, ctx: Context, pipeline: Pipeline, *args, **kwargs
+) -> Callable[[Context, Pipeline, Any, Any], bool]:
     """
     The simplest and quickest condition handler for trivial condition handling returns the callable condition:
 
     :param condition: Condition to copy.
     :param ctx: Context of current condition.
-    :param actor: Actor we use in this condition.
+    :param pipeline: Pipeline we use in this condition.
     """
-    return condition(ctx, actor, *args, **kwargs)
+    return condition(ctx, pipeline, *args, **kwargs)
```

### Comparing `dff-0.3.2/dff/script/core/context.py` & `dff-0.4.1/dff/script/core/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             "last_response": "set_last_response",
             "last_request": "set_last_request",
         }
 
     id: Union[UUID, int, str] = Field(default_factory=uuid4)
     """
     `id` is the unique context identifier. By default, randomly generated using `uuid4` `id` is used.
-    `id` can be used to trace the user behaviour, e.g while collecting the statistical data.
+    `id` can be used to trace the user behavior, e.g while collecting the statistical data.
     """
     labels: Dict[int, NodeLabel2Type] = {}
     """
     `labels` stores the history of all passed `labels`
 
         - key - `id` of the turn.
         - value - `label` on this turn.
@@ -97,28 +97,28 @@
     so storage of any data won't reflect on the work on the internal Dialog Flow Scripting functions.
 
         - key - Arbitrary data name.
         - value - Arbitrary data.
     """
     validation: bool = False
     """
-    `validation` is a flag that signals that :py:class:`~dff.script.Actor`,
+    `validation` is a flag that signals that :py:class:`~dff.script.Pipeline`,
     while being initialized, checks the :py:class:`~dff.script.Script`.
-    The functions that can give not validable data
+    The functions that can give not valid data
     while being validated must use this flag to take the validation mode into account.
     Otherwise the validation will not be passed.
     """
     framework_states: Dict[ModuleName, Dict[str, Any]] = {}
     """
     `framework_states` is used for addons states or for
-    :py:class:`~dff.script.Actor`'s states.
-    :py:class:`~dff.script.Actor`
+    :py:class:`~dff.script.Pipeline`'s states.
+    :py:class:`~dff.script.Pipeline`
     records all its intermediate conditions into the `framework_states`.
     After :py:class:`~dff.script.Context` processing is finished,
-    :py:class:`~dff.script.Actor` resets `framework_states` and
+    :py:class:`~dff.script.Pipeline` resets `framework_states` and
     returns :py:class:`~dff.script.Context`.
 
         - key - Temporary variable name.
         - value - Temporary variable data.
     """
 
     # validators
```

### Comparing `dff-0.3.2/dff/script/core/keywords.py` & `dff-0.4.1/dff/script/core/keywords.py`

 * *Files identical despite different names*

### Comparing `dff-0.3.2/dff/script/core/message.py` & `dff-0.4.1/dff/script/core/message.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,74 @@
 """
 Message
 -------
 The :py:class:`.Message` class is a universal data model for representing a message that should be supported by
-`DFF`. It only contains types and properties that are compatible with most messaging services.
+DFF. It only contains types and properties that are compatible with most messaging services.
 """
 from typing import Any, Optional, List, Union
 from enum import Enum, auto
 from pathlib import Path
 from urllib.request import urlopen
 
 from pydantic import Extra, Field, ValidationError, FilePath, HttpUrl, BaseModel
 from pydantic import validator, root_validator
 
 
 class Session(Enum):
+    """
+    An enumeration that defines two possible states of a session.
+    """
+
     ACTIVE = auto()
     FINISHED = auto()
 
 
 class DataModel(BaseModel):
+    """
+    This class is a Pydantic BaseModel that serves as a base class for all DFF models.
+    """
+
     class Config:
         extra = Extra.allow
         arbitrary_types_allowed = True
 
 
 class Command(DataModel):
+    """
+    This class is a subclass of DataModel and represents
+    a command that can be executed in response to a user input.
+    """
+
     ...
 
 
 class Location(DataModel):
+    """
+    This class is a data model that represents a geographical
+    location on the Earth's surface.
+    It has two attributes, longitude and latitude, both of which are float values.
+    If the absolute difference between the latitude and longitude values of the two
+    locations is less than 0.00004, they are considered equal.
+    """
+
     longitude: float
     latitude: float
 
     def __eq__(self, other):
         if isinstance(other, Location):
             return abs(self.latitude - other.latitude) + abs(self.longitude - other.longitude) < 0.00004
         return NotImplemented
 
 
 class Attachment(DataModel):
+    """
+    This class represents an attachment that can be either
+    a file or a URL, along with an optional ID and title.
+    """
+
     source: Optional[Union[HttpUrl, FilePath]] = None
     id: Optional[str] = None  # id field is made separate to simplify type validation
     title: Optional[str] = None
 
     def get_bytes(self) -> Optional[bytes]:
         if self.source is None:
             return None
@@ -72,48 +98,65 @@
     def validate_source(cls, value):
         if isinstance(value, Path):
             return Path(value)
         return value
 
 
 class Audio(Attachment):
+    """Represents an audio file attachment."""
+
     pass
 
 
 class Video(Attachment):
+    """Represents a video file attachment."""
+
     pass
 
 
 class Image(Attachment):
+    """Represents an image file attachment."""
+
     pass
 
 
 class Document(Attachment):
+    """Represents a document file attachment."""
+
     pass
 
 
 class Attachments(DataModel):
+    """This class is a data model that represents a list of attachments."""
+
     files: List[Attachment] = Field(default_factory=list)
 
     def __eq__(self, other):
         if isinstance(other, Attachments):
             return self.files == other.files
         return NotImplemented
 
 
 class Link(DataModel):
+    """This class is a DataModel representing a hyperlink."""
+
     source: HttpUrl
     title: Optional[str] = None
 
     @property
     def html(self):
         return f'<a href="{self.source}">{self.title if self.title else self.source}</a>'
 
 
 class Button(DataModel):
+    """
+    This class allows for the creation of a button object
+    with a source URL, a text description, and a payload.
+    """
+
     source: Optional[HttpUrl] = None
     text: str
     payload: Optional[Any] = None
 
     def __eq__(self, other):
         if isinstance(other, Button):
             if self.source != other.source:
@@ -123,25 +166,31 @@
             first_payload = bytes(self.payload, encoding="utf-8") if isinstance(self.payload, str) else self.payload
             second_payload = bytes(other.payload, encoding="utf-8") if isinstance(other.payload, str) else other.payload
             return first_payload == second_payload
         return NotImplemented
 
 
 class Keyboard(DataModel):
+    """
+    This class is a DataModel that represents a keyboard object
+    that can be used for a chatbot or messaging application.
+    """
+
     buttons: List[Button] = Field(default_factory=list, min_items=1)
 
     def __eq__(self, other):
         if isinstance(other, Keyboard):
             return self.buttons == other.buttons
         return NotImplemented
 
 
 class Message(DataModel):
     """
-    Class representing a message and contains several class level variables to store message information.
+    Class representing a message and contains several
+    class level variables to store message information.
     """
 
     text: Optional[str] = None
     commands: Optional[List[Command]] = None
     attachments: Optional[Attachments] = None
     annotations: Optional[dict] = None
     misc: Optional[dict] = None
@@ -161,8 +210,10 @@
         return NotImplemented
 
     def __repr__(self) -> str:
         return " ".join([f"{key}='{value}'" for key, value in self.dict(exclude_none=True).items()])
 
 
 class MultiMessage(Message):
+    """This class represents a message that contains multiple sub-messages."""
+
     messages: Optional[List[Message]] = None
```

### Comparing `dff-0.3.2/dff/script/core/normalization.py` & `dff-0.4.1/dff/script/core/normalization.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,52 +3,50 @@
 -------------
 Normalization module is used to normalize all python objects and functions to a format
 that is suitable for script and actor execution process.
 This module contains a basic set of functions for normalizing data in a dialog script.
 """
 import logging
 
-from typing import Union, Callable, Any, Dict, Optional
+from typing import Union, Callable, Any, Dict, Optional, ForwardRef
 
 from .keywords import GLOBAL, Keywords
 from .context import Context
 from .types import NodeLabel3Type, NodeLabelType, ConditionType, LabelType
 from .message import Message
 
-from pydantic import validate_arguments, BaseModel
+from pydantic import validate_arguments
 
 logger = logging.getLogger(__name__)
 
-Actor = BaseModel
+Pipeline = ForwardRef("Pipeline")
 
 
 @validate_arguments
 def normalize_label(label: NodeLabelType, default_flow_label: LabelType = "") -> Union[Callable, NodeLabel3Type]:
     """
     The function that is used for normalization of
     :py:const:`default_flow_label <dff.script.NodeLabelType>`.
 
-    :param label: If `label` is `Callable` the function is wrapped into try/except
-        and normalization is used on the result of the function call with the name `label`.
-    :param default_flow_label: `flow_label` is used if `label` does not contain `flow_label`.
-
-    :return: Result of the `label` normalization,
-        if `Callable` is returned, the normalized result is returned.
+    :param label: If label is Callable the function is wrapped into try/except
+        and normalization is used on the result of the function call with the name label.
+    :param default_flow_label: flow_label is used if label does not contain flow_label.
+    :return: Result of the label normalization,
+        if Callable is returned, the normalized result is returned.
     """
     if isinstance(label, Callable):
 
-        @validate_arguments
-        def get_label_handler(ctx: Context, actor: Actor, *args, **kwargs) -> NodeLabel3Type:
+        def get_label_handler(ctx: Context, pipeline: Pipeline, *args, **kwargs) -> NodeLabel3Type:
             try:
-                new_label = label(ctx, actor, *args, **kwargs)
+                new_label = label(ctx, pipeline, *args, **kwargs)
                 new_label = normalize_label(new_label, default_flow_label)
                 flow_label, node_label, _ = new_label
-                node = actor.script.get(flow_label, {}).get(node_label)
+                node = pipeline.script.get(flow_label, {}).get(node_label)
                 if not node:
-                    raise Exception(f"Unknown transitions {new_label} for actor.script={actor.script}")
+                    raise Exception(f"Unknown transitions {new_label} for pipeline.script={pipeline.script}")
             except Exception as exc:
                 new_label = None
                 logger.error(f"Exception {exc} of function {label}", exc_info=exc)
             return new_label
 
         return get_label_handler  # create wrap to get uniq key for dictionary
     elif isinstance(label, str) or isinstance(label, Keywords):
@@ -62,89 +60,86 @@
         flow_label = label[0] or default_flow_label
         return (flow_label, label[1], label[2])
 
 
 @validate_arguments
 def normalize_condition(condition: ConditionType) -> Callable:
     """
-    The functon that is used to normalize `condition`
+    The function that is used to normalize `condition`
 
-    :param condition: `condition` to normalize.
-    :return: The function `condition` wrapped into the try/except.
+    :param condition: Condition to normalize.
+    :return: The function condition wrapped into the try/except.
     """
     if isinstance(condition, Callable):
 
-        @validate_arguments
-        def callable_condition_handler(ctx: Context, actor: Actor, *args, **kwargs) -> bool:
+        def callable_condition_handler(ctx: Context, pipeline: Pipeline, *args, **kwargs) -> bool:
             try:
-                return condition(ctx, actor, *args, **kwargs)
+                return condition(ctx, pipeline, *args, **kwargs)
             except Exception as exc:
                 logger.error(f"Exception {exc} of function {condition}", exc_info=exc)
                 return False
 
         return callable_condition_handler
 
 
 @validate_arguments
 def normalize_transitions(
     transitions: Dict[NodeLabelType, ConditionType]
 ) -> Dict[Union[Callable, NodeLabel3Type], Callable]:
     """
-    The function which is used to normalize `transitions` and returns normalized `dict`.
+    The function which is used to normalize transitions and returns normalized dict.
 
-    :param transitions: `transitions` to normalize.
-    :return: `transitions` with normalized `label` and `condition`.
+    :param transitions: Transitions to normalize.
+    :return: Transitions with normalized label and condition.
     """
     transitions = {normalize_label(label): normalize_condition(condition) for label, condition in transitions.items()}
     return transitions
 
 
 @validate_arguments
 def normalize_response(response: Optional[Union[Message, Callable[..., Message]]]) -> Callable[..., Message]:
     """
-    This function is used to normalize `response`, if `response` Callable, it is returned, otherwise
-    `response` is wrapped to the function and this function is returned.
+    This function is used to normalize response, if response Callable, it is returned, otherwise
+    response is wrapped to the function and this function is returned.
 
-    :param response: `response` to normalize.
+    :param response: Response to normalize.
     :return: Function that returns callable response.
     """
     if isinstance(response, Callable):
         return response
     else:
         if response is None:
             result = Message()
         elif isinstance(response, Message):
             result = response
         else:
             raise TypeError(type(response))
 
-        @validate_arguments
-        def response_handler(ctx: Context, actor: Actor, *args, **kwargs):
+        def response_handler(ctx: Context, pipeline: Pipeline, *args, **kwargs):
             return result
 
         return response_handler
 
 
 @validate_arguments
 def normalize_processing(processing: Dict[Any, Callable]) -> Callable:
     """
-    This function is used to normalize `processing`.
-    It returns function that consecutively applies all preprocessing stages from `dict`.
+    This function is used to normalize processing.
+    It returns function that consecutively applies all preprocessing stages from dict.
 
-    :param processing: `processing` which contains all preprocessing stages in a format "PROC_i" -> proc_func_i.
-    :return: Function that consequentially applies all preprocessing stages from `dict`.
+    :param processing: Processing which contains all preprocessing stages in a format "PROC_i" -> proc_func_i.
+    :return: Function that consequentially applies all preprocessing stages from dict.
     """
     if isinstance(processing, dict):
 
-        @validate_arguments
-        def processing_handler(ctx: Context, actor: Actor, *args, **kwargs) -> Context:
+        def processing_handler(ctx: Context, pipeline: Pipeline, *args, **kwargs) -> Context:
             for processing_name, processing_func in processing.items():
                 try:
                     if processing_func is not None:
-                        ctx = processing_func(ctx, actor, *args, **kwargs)
+                        ctx = processing_func(ctx, pipeline, *args, **kwargs)
                 except Exception as exc:
                     logger.error(
                         f"Exception {exc} for processing_name={processing_name} and processing_func={processing_func}",
                         exc_info=exc,
                     )
             return ctx
 
@@ -171,16 +166,16 @@
 @validate_arguments
 def normalize_keywords(
     script: Dict[LabelType, Dict[LabelType, Dict[Keywords, Any]]]
 ) -> Dict[LabelType, Dict[LabelType, Dict[str, Any]]]:
     """
     This function is used to normalize keywords in the script.
 
-    :param script: `Script`, containing all transitions between states based in the keywords.
-    :return: `Script` with the normalized keywords.
+    :param script: :py:class:`.Script`, containing all transitions between states based in the keywords.
+    :return: :py:class:`.Script` with the normalized keywords.
     """
 
     script = {
         flow_label: {
             node_label: {map_deprecated_key(key.name.lower()): val for key, val in node.items()}
             for node_label, node in flow.items()
         }
@@ -188,19 +183,19 @@
     }
     return script
 
 
 @validate_arguments
 def normalize_script(script: Dict[LabelType, Any]) -> Dict[LabelType, Dict[LabelType, Dict[str, Any]]]:
     """
-    This function normalizes `Script`: it returns `dict` where the `GLOBAL` node is moved
-    into the flow with the `GLOBAL` name. The function returns the structure
+    This function normalizes :py:class:`.Script`: it returns dict where the GLOBAL node is moved
+    into the flow with the GLOBAL name. The function returns the structure
 
     `{GLOBAL: {...NODE...}, ...}` -> `{GLOBAL: {GLOBAL: {...NODE...}}, ...}`.
 
-    :param script: `Script` that describes the dialog scenario.
-    :return: Normalized `Script`.
+    :param script: :py:class:`.Script` that describes the dialog scenario.
+    :return: Normalized :py:class:`.Script`.
     """
     if isinstance(script, dict):
         if GLOBAL in script and all([isinstance(item, Keywords) for item in script[GLOBAL].keys()]):
             script[GLOBAL] = {GLOBAL: script[GLOBAL]}
     return normalize_keywords(script)
```

### Comparing `dff-0.3.2/dff/script/core/script.py` & `dff-0.4.1/dff/script/core/script.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,58 +16,60 @@
 from .message import Message
 from .normalization import normalize_response, normalize_processing, normalize_transitions, normalize_script
 from typing import ForwardRef
 
 logger = logging.getLogger(__name__)
 
 
-Actor = ForwardRef("Actor")
+Pipeline = ForwardRef("Pipeline")
 Context = ForwardRef("Context")
 
 
 class Node(BaseModel, extra=Extra.forbid):
     """
     The class for the `Node` object.
     """
 
     transitions: Dict[NodeLabelType, ConditionType] = {}
-    response: Optional[Union[Message, Callable[[Context, Actor], Message]]] = None
+    response: Optional[Union[Message, Callable[[Context, Pipeline], Message]]] = None
     pre_transitions_processing: Dict[Any, Callable] = {}
     pre_response_processing: Dict[Any, Callable] = {}
     misc: dict = {}
 
     _normalize_transitions = validator("transitions", allow_reuse=True)(normalize_transitions)
 
-    def run_response(self, ctx: Context, actor: Actor, *args, **kwargs) -> Context:
+    def run_response(self, ctx: Context, pipeline: Pipeline, *args, **kwargs) -> Context:
         """
         Executes the normalized response.
         See details in the :py:func:`~normalize_response` function of `normalization.py`.
         """
         response = normalize_response(self.response)
-        return response(ctx, actor, *args, **kwargs)
+        return response(ctx, pipeline, *args, **kwargs)
 
-    def run_pre_response_processing(self, ctx: Context, actor: Actor, *args, **kwargs) -> Context:
+    def run_pre_response_processing(self, ctx: Context, pipeline: Pipeline, *args, **kwargs) -> Context:
         """
         Executes pre-processing of responses.
         """
-        return self.run_processing(self.pre_response_processing, ctx, actor, *args, **kwargs)
+        return self.run_processing(self.pre_response_processing, ctx, pipeline, *args, **kwargs)
 
-    def run_pre_transitions_processing(self, ctx: Context, actor: Actor, *args, **kwargs) -> Context:
+    def run_pre_transitions_processing(self, ctx: Context, pipeline: Pipeline, *args, **kwargs) -> Context:
         """
         Executes pre-processing of transitions.
         """
-        return self.run_processing(self.pre_transitions_processing, ctx, actor, *args, **kwargs)
+        return self.run_processing(self.pre_transitions_processing, ctx, pipeline, *args, **kwargs)
 
-    def run_processing(self, processing: Dict[Any, Callable], ctx: Context, actor: Actor, *args, **kwargs) -> Context:
+    def run_processing(
+        self, processing: Dict[Any, Callable], ctx: Context, pipeline: Pipeline, *args, **kwargs
+    ) -> Context:
         """
         Executes the normalized processing.
         See details in the :py:func:`~normalize_processing` function of `normalization.py`.
         """
         processing = normalize_processing(processing)
-        return processing(ctx, actor, *args, **kwargs)
+        return processing(ctx, pipeline, *args, **kwargs)
 
 
 class Script(BaseModel, extra=Extra.forbid):
     """
     The class for the `Script` object.
     """
```

### Comparing `dff-0.3.2/dff/script/labels/std_labels.py` & `dff-0.4.1/dff/script/labels/std_labels.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,168 +6,170 @@
 They are used to identify the next step in the conversation.
 Labels can also be used in combination with other conditions,
 such as the current context or user data, to create more complex and dynamic conversations.
 
 This module contains a standard set of scripting :py:const:`labels <dff.script.NodeLabelType>` that
 can be used by developers to define the conversation flow.
 """
-from typing import Optional, Callable
-from dff.script import Actor, Context, NodeLabel3Type
+from typing import Optional, Callable, ForwardRef
+from dff.script import Context, NodeLabel3Type
+
+Pipeline = ForwardRef("Pipeline")
 
 
 def repeat(priority: Optional[float] = None, *args, **kwargs) -> Callable:
     """
     Returns transition handler that takes :py:class:`.Context`,
-    :py:class:`.Actor` and :py:const:`priority <float>`.
+    :py:class:`~dff.pipeline.Pipeline` and :py:const:`priority <float>`.
     This handler returns a :py:const:`label <NodeLabelType>`
     to the last node with a given :py:const:`priority <float>`.
-    If the priority is not given, `Actor.label_priority` is used as default.
+    If the priority is not given, `Pipeline.actor.label_priority` is used as default.
 
-    :param priority: Priority of transition. Uses `Actor.label_priority` if priority not defined.
+    :param priority: Priority of transition. Uses `Pipeline.actor.label_priority` if priority not defined.
     """
 
-    def repeat_transition_handler(ctx: Context, actor: Actor, *args, **kwargs) -> NodeLabel3Type:
-        current_priority = actor.label_priority if priority is None else priority
+    def repeat_transition_handler(ctx: Context, pipeline: Pipeline, *args, **kwargs) -> NodeLabel3Type:
+        current_priority = pipeline.actor.label_priority if priority is None else priority
         if len(ctx.labels) >= 1:
             flow_label, label = list(ctx.labels.values())[-1]
         else:
-            flow_label, label = actor.fallback_label[:2]
+            flow_label, label = pipeline.actor.fallback_label[:2]
         return (flow_label, label, current_priority)
 
     return repeat_transition_handler
 
 
 def previous(priority: Optional[float] = None, *args, **kwargs) -> Callable:
     """
     Returns transition handler that takes :py:class:`~dff.script.Context`,
-    :py:class:`~dff.script.Actor` and :py:const:`priority <float>`.
+    :py:class:`~dff.pipeline.Pipeline` and :py:const:`priority <float>`.
     This handler returns a :py:const:`label <dff.script.NodeLabelType>`
     to the previous node with a given :py:const:`priority <float>`.
-    If the priority is not given, `Actor.label_priority` is used as default.
+    If the priority is not given, `Pipeline.actor.label_priority` is used as default.
 
-    :param priority: Priority of transition. Uses `Actor.label_priority` if priority not defined.
+    :param priority: Priority of transition. Uses `Pipeline.actor.label_priority` if priority not defined.
     """
 
-    def previous_transition_handler(ctx: Context, actor: Actor, *args, **kwargs) -> NodeLabel3Type:
-        current_priority = actor.label_priority if priority is None else priority
+    def previous_transition_handler(ctx: Context, pipeline: Pipeline, *args, **kwargs) -> NodeLabel3Type:
+        current_priority = pipeline.actor.label_priority if priority is None else priority
         if len(ctx.labels) >= 2:
             flow_label, label = list(ctx.labels.values())[-2]
         else:
-            flow_label, label = actor.fallback_label[:2]
+            flow_label, label = pipeline.actor.fallback_label[:2]
         return (flow_label, label, current_priority)
 
     return previous_transition_handler
 
 
 def to_start(priority: Optional[float] = None, *args, **kwargs) -> Callable:
     """
     Returns transition handler that takes :py:class:`~dff.script.Context`,
-    :py:class:`~dff.script.Actor` and :py:const:`priority <float>`.
+    :py:class:`~dff.pipeline.Pipeline` and :py:const:`priority <float>`.
     This handler returns a :py:const:`label <dff.script.NodeLabelType>`
     to the start node with a given :py:const:`priority <float>`.
-    If the priority is not given, `Actor.label_priority` is used as default.
+    If the priority is not given, `Pipeline.actor.label_priority` is used as default.
 
-    :param priority: Priority of transition. Uses `Actor.label_priority` if priority not defined.
+    :param priority: Priority of transition. Uses `Pipeline.actor.label_priority` if priority not defined.
     """
 
-    def to_start_transition_handler(ctx: Context, actor: Actor, *args, **kwargs) -> NodeLabel3Type:
-        current_priority = actor.label_priority if priority is None else priority
-        return (*actor.start_label[:2], current_priority)
+    def to_start_transition_handler(ctx: Context, pipeline: Pipeline, *args, **kwargs) -> NodeLabel3Type:
+        current_priority = pipeline.actor.label_priority if priority is None else priority
+        return (*pipeline.actor.start_label[:2], current_priority)
 
     return to_start_transition_handler
 
 
 def to_fallback(priority: Optional[float] = None, *args, **kwargs) -> Callable:
     """
     Returns transition handler that takes :py:class:`~dff.script.Context`,
-    :py:class:`~dff.script.Actor` and :py:const:`priority <float>`.
+    :py:class:`~dff.pipeline.Pipeline` and :py:const:`priority <float>`.
     This handler returns a :py:const:`label <dff.script.NodeLabelType>`
     to the fallback node with a given :py:const:`priority <float>`.
-    If the priority is not given, `Actor.label_priority` is used as default.
+    If the priority is not given, `Pipeline.actor.label_priority` is used as default.
 
-    :param priority: Priority of transition. Uses `Actor.label_priority` if priority not defined.
+    :param priority: Priority of transition. Uses `Pipeline.actor.label_priority` if priority not defined.
     """
 
-    def to_fallback_transition_handler(ctx: Context, actor: Actor, *args, **kwargs) -> NodeLabel3Type:
-        current_priority = actor.label_priority if priority is None else priority
-        return (*actor.fallback_label[:2], current_priority)
+    def to_fallback_transition_handler(ctx: Context, pipeline: Pipeline, *args, **kwargs) -> NodeLabel3Type:
+        current_priority = pipeline.actor.label_priority if priority is None else priority
+        return (*pipeline.actor.fallback_label[:2], current_priority)
 
     return to_fallback_transition_handler
 
 
 def _get_label_by_index_shifting(
     ctx: Context,
-    actor: Actor,
+    pipeline: Pipeline,
     priority: Optional[float] = None,
     increment_flag: bool = True,
     cyclicality_flag: bool = True,
     *args,
     **kwargs,
 ) -> NodeLabel3Type:
     """
-    Function that returns node label from the context and actor after shifting the index.
+    Function that returns node label from the context and pipeline after shifting the index.
 
     :param ctx: Dialog context.
-    :param actor: Dialog actor.
-    :param priority: Priority of transition. Uses `Actor.label_priority` if priority not defined.
+    :param pipeline: Dialog pipeline.
+    :param priority: Priority of transition. Uses `Pipeline.actor.label_priority` if priority not defined.
     :param increment_flag: If it is `True`, label index is incremented by `1`,
         otherwise it is decreased by `1`. Defaults to `True`.
     :param cyclicality_flag: If it is `True` the iteration over the label list is going cyclically
         (e.g the element with `index = len(labels)` has `index = 0`). Defaults to `True`.
     :return: The tuple that consists of `(flow_label, label, priority)`.
         If fallback is executed `(flow_fallback_label, fallback_label, priority)` are returned.
     """
-    flow_label, node_label, current_priority = repeat(priority, *args, **kwargs)(ctx, actor, *args, **kwargs)
-    labels = list(actor.script.get(flow_label, {}))
+    flow_label, node_label, current_priority = repeat(priority, *args, **kwargs)(ctx, pipeline, *args, **kwargs)
+    labels = list(pipeline.script.get(flow_label, {}))
 
     if node_label not in labels:
-        return (*actor.fallback_label[:2], current_priority)
+        return (*pipeline.actor.fallback_label[:2], current_priority)
 
     label_index = labels.index(node_label)
     label_index = label_index + 1 if increment_flag else label_index - 1
     if not (cyclicality_flag or (0 <= label_index < len(labels))):
-        return (*actor.fallback_label[:2], current_priority)
+        return (*pipeline.actor.fallback_label[:2], current_priority)
     label_index %= len(labels)
 
     return (flow_label, labels[label_index], current_priority)
 
 
 def forward(priority: Optional[float] = None, cyclicality_flag: bool = True, *args, **kwargs) -> Callable:
     """
     Returns transition handler that takes :py:class:`~dff.script.Context`,
-    :py:class:`~dff.script.Actor` and :py:const:`priority <float>`.
+    :py:class:`~dff.pipeline.Pipeline` and :py:const:`priority <float>`.
     This handler returns a :py:const:`label <dff.script.NodeLabelType>`
     to the forward node with a given :py:const:`priority <float>` and :py:const:`cyclicality_flag <bool>`.
-    If the priority is not given, `Actor.label_priority` is used as default.
+    If the priority is not given, `Pipeline.actor.label_priority` is used as default.
 
-    :param priority: Float priority of transition. Uses `Actor.label_priority` if priority not defined.
+    :param priority: Float priority of transition. Uses `Pipeline.actor.label_priority` if priority not defined.
     :param cyclicality_flag: If it is `True`, the iteration over the label list is going cyclically
         (e.g the element with `index = len(labels)` has `index = 0`). Defaults to `True`.
     """
 
-    def forward_transition_handler(ctx: Context, actor: Actor, *args, **kwargs) -> NodeLabel3Type:
+    def forward_transition_handler(ctx: Context, pipeline: Pipeline, *args, **kwargs) -> NodeLabel3Type:
         return _get_label_by_index_shifting(
-            ctx, actor, priority, increment_flag=True, cyclicality_flag=cyclicality_flag
+            ctx, pipeline, priority, increment_flag=True, cyclicality_flag=cyclicality_flag
         )
 
     return forward_transition_handler
 
 
 def backward(priority: Optional[float] = None, cyclicality_flag: bool = True, *args, **kwargs) -> Callable:
     """
     Returns transition handler that takes :py:class:`~dff.script.Context`,
-    :py:class:`~dff.script.Actor` and :py:const:`priority <float>`.
+    :py:class:`~dff.pipeline.Pipeline` and :py:const:`priority <float>`.
     This handler returns a :py:const:`label <dff.script.NodeLabelType>`
     to the backward node with a given :py:const:`priority <float>` and :py:const:`cyclicality_flag <bool>`.
-    If the priority is not given, `Actor.label_priority` is used as default.
+    If the priority is not given, `Pipeline.actor.label_priority` is used as default.
 
-    :param priority: Float priority of transition. Uses `Actor.label_priority` if priority not defined.
+    :param priority: Float priority of transition. Uses `Pipeline.actor.label_priority` if priority not defined.
     :param cyclicality_flag: If it is `True`, the iteration over the label list is going cyclically
         (e.g the element with `index = len(labels)` has `index = 0`). Defaults to `True`.
     """
 
-    def back_transition_handler(ctx: Context, actor: Actor, *args, **kwargs) -> NodeLabel3Type:
+    def back_transition_handler(ctx: Context, pipeline: Pipeline, *args, **kwargs) -> NodeLabel3Type:
         return _get_label_by_index_shifting(
-            ctx, actor, priority, increment_flag=False, cyclicality_flag=cyclicality_flag
+            ctx, pipeline, priority, increment_flag=False, cyclicality_flag=cyclicality_flag
         )
 
     return back_transition_handler
```

### Comparing `dff-0.3.2/dff/script/responses/std_responses.py` & `dff-0.4.1/dff/script/responses/std_responses.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,22 +7,23 @@
 
 This module provides only one predefined response function that can be used to quickly
 respond to the user and keep the conversation flowing.
 """
 import random
 from typing import List
 
-from dff.script import Context, Actor, Message
+from dff.pipeline import Pipeline
+from dff.script import Context, Message
 
 
 def choice(responses: List[Message]):
     """
     Function wrapper that takes the list of responses as an input
     and returns handler which outputs a response randomly chosen from that list.
 
     :param responses: A list of responses for random sampling.
     """
 
-    def choice_response_handler(ctx: Context, actor: Actor, *args, **kwargs):
+    def choice_response_handler(ctx: Context, pipeline: Pipeline, *args, **kwargs):
         return random.choice(responses)
 
     return choice_response_handler
```

### Comparing `dff-0.3.2/dff/utils/testing/common.py` & `dff-0.4.1/dff/utils/testing/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,24 @@
+"""
+Common
+------
+This module contains several functions which are used to run demonstrations in tutorials.
+"""
 from os import getenv
 from typing import Callable, Tuple, Any, Optional
 from uuid import uuid4
 
 from dff.script import Context, Message
 from dff.pipeline import Pipeline
 from dff.utils.testing.response_comparers import default_comparer
 
 
-def is_interactive_mode() -> bool:
+def is_interactive_mode() -> bool:  # pragma: no cover
     """
-    Checking whether the example code should be run in interactive mode.
+    Checking whether the tutorial code should be run in interactive mode.
 
     :return: `True` if it's being executed by Jupyter kernel and DISABLE_INTERACTIVE_MODE env variable isn't set,
         `False` otherwise.
     """
 
     shell = None
     try:
@@ -28,15 +33,15 @@
     pipeline: Pipeline,
     happy_path: Tuple[Tuple[Any, Any], ...],
     # This optional argument is used for additional processing of candidate responses and reference responses
     response_comparer: Callable[[Any, Any, Context], Optional[str]] = default_comparer,
     printout_enable: bool = True,
 ):
     """
-    Running example with provided pipeline for provided requests, comparing responses with correct expected responses.
+    Running tutorial with provided pipeline for provided requests, comparing responses with correct expected responses.
     In cases when additional processing of responses is needed (e.g. in case of response being an HTML string),
     a special function (response comparer) is used.
 
     :param pipeline: The Pipeline instance, that will be used for checking.
     :param happy_path: A tuple of (request, response) tuples, so-called happy path,
         its requests are passed to pipeline and the pipeline responses are compared to its responses.
     :param response_comparer: A special comparer function that accepts received response, true response and context;
@@ -62,15 +67,15 @@
                 f"reference_response = {repr(reference_response)}\n"
                 "candidate_response != reference_response"
             )
 
 
 def run_interactive_mode(pipeline: Pipeline):  # pragma: no cover
     """
-    Running example with provided pipeline in interactive mode, just like with CLI messenger interface.
+    Running tutorial with provided pipeline in interactive mode, just like with CLI messenger interface.
     The dialog won't be stored anywhere, it will only be outputted to STDOUT.
 
     :param pipeline: The Pipeline instance, that will be used for running.
     """
 
     ctx_id = uuid4()  # Random UID
     print("Start a dialogue with the bot")
```

### Comparing `dff-0.3.2/dff/utils/testing/response_comparers.py` & `dff-0.4.1/dff/utils/testing/response_comparers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+Response comparer
+-----------------
+This module defines function used to compare two response objects.
+"""
 from typing import Any, Optional
 
 from dff.script import Context, Message
 
 
 def default_comparer(candidate: Message, reference: Message, _: Context) -> Optional[Any]:
     """
```

### Comparing `dff-0.3.2/dff/utils/testing/telegram.py` & `dff-0.4.1/dff/utils/testing/telegram.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from contextlib import asynccontextmanager, nullcontext
 import logging
 import asyncio
 from tempfile import TemporaryDirectory
 from pathlib import Path
 from copy import deepcopy
 
-import telethon.tl.types
+from telethon.tl.types import ReplyKeyboardHide
 from telethon import TelegramClient
 from telethon.types import User
 from telethon.custom import Message as TlMessage
 from telebot import types
 
 from dff.pipeline.pipeline.pipeline import Pipeline
 from dff.script.core.message import Message, Attachments, Attachment, Button, Location
@@ -161,15 +161,15 @@
                                 text=button.text,
                                 payload=button.data,
                             )
                         )
                 if msg.ui is not None:
                     raise RuntimeError(f"Several messages with ui:\n{msg.ui}\n{TelegramUI(buttons=buttons)}")
                 msg.ui = TelegramUI(buttons=buttons)
-            if isinstance(response.reply_markup, telethon.tl.types.ReplyKeyboardHide):
+            if isinstance(response.reply_markup, ReplyKeyboardHide):
                 if msg.ui is not None:
                     raise RuntimeError(f"Several messages with ui:\n{msg.ui}\n{types.ReplyKeyboardRemove()}")
                 msg.ui = RemoveKeyboard()
             if response.geo is not None:
                 location = Location(latitude=response.geo.lat, longitude=response.geo.long)
                 if msg.location is not None:
                     raise RuntimeError(f"Several messages with location:\n{msg.location}\n{location}")
```

### Comparing `dff-0.3.2/dff/utils/turn_caching/singleton_turn_caching.py` & `dff-0.4.1/dff/utils/turn_caching/singleton_turn_caching.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,19 +4,15 @@
 
 USED_CACHES: List[Callable] = list()
 """Cache singleton, it is common for all actors and pipelines in current environment."""
 
 
 def cache_clear():
     """
-    Function for cache singleton clearing, it is called in the end of:
-
-    1. Actor execution turn (except for actor inside pipeline)
-
-    2. Pipeline execution turn
+    Function for cache singleton clearing, it is called in the end of pipeline execution turn.
     """
     for used_cache in USED_CACHES:
         used_cache.cache_clear()
 
 
 def lru_cache(maxsize: Optional[int] = None, typed: bool = False) -> Callable:
     """
```

### Comparing `dff-0.3.2/dff.egg-info/PKG-INFO` & `dff-0.4.1/dff.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dff
-Version: 0.3.2
+Version: 0.4.1
 Summary: The Dialog Flow Framework (DFF) allows you to write conversational services.
 Home-page: https://github.com/deeppavlov/dialog_flow_framework
 Author: Denis Kuznetsov
 Author-email: kuznetsov.den.p@gmail.com
 Keywords: chatbots
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -27,15 +27,15 @@
 Provides-Extra: mysql
 Provides-Extra: postgresql
 Provides-Extra: ydb
 Provides-Extra: telegram
 Provides-Extra: full
 Provides-Extra: tests
 Provides-Extra: test_full
-Provides-Extra: examples
+Provides-Extra: tutorials
 Provides-Extra: devel
 Provides-Extra: doc
 Provides-Extra: devel_full
 License-File: LICENSE
 
 
 # Dialog Flow Framework
@@ -62,41 +62,45 @@
 pip install dff
 ```
 
 The above command will set the minimum dependencies to start working with DFF.
 The installation process allows the user to choose from different packages based on their dependencies, which are:
 ```bash
 pip install dff[core]  # minimal dependencies (by default)
+pip install dff[json]  # dependencies for using JSON
+pip install dff[pickle] # dependencies for using Pickle
 pip install dff[redis]  # dependencies for using Redis
 pip install dff[mongodb]  # dependencies for using MongoDB
 pip install dff[mysql]  # dependencies for using MySQL
 pip install dff[postgresql]  # dependencies for using PostgreSQL
 pip install dff[sqlite]  # dependencies for using SQLite
 pip install dff[ydb]  # dependencies for using Yandex Database
+pip install dff[telegram]  # dependencies for using Telegram
 pip install dff[full]  # full dependencies including all options above
 pip install dff[tests]  # dependencies for running tests
 pip install dff[test_full]  # full dependencies for running all tests (all options above)
-pip install dff[examples]  # dependencies for running examples (all options above)
+pip install dff[tutorials]  # dependencies for running tutorials (all options above)
 pip install dff[devel]  # dependencies for development
 pip install dff[doc]  # dependencies for documentation
 pip install dff[devel_full]  # full dependencies for development (all options above)
 ```
 
 For example, if you are going to use one of the database backends,
 you can specify the corresponding requirements yourself. Multiple dependencies can be installed at once, e.g.
 ```bash
 pip install dff[postgresql, mysql]
 ```
 
 ## Basic example
 
 ```python
-from dff.script import GLOBAL, TRANSITIONS, RESPONSE, Context, Actor, Message
+from dff.script import GLOBAL, TRANSITIONS, RESPONSE, Context, Message
+from dff.pipeline import Pipeline
 import dff.script.conditions.std_conditions as cnd
-from typing import Union
+from typing import Tuple
 
 # create a dialog script
 script = {
 GLOBAL: {
 TRANSITIONS: {
 ("flow", "node_hi"): cnd.exact_match(Message(text="Hi")),
 ("flow", "node_ok"): cnd.true()
@@ -104,36 +108,31 @@
 },
 "flow": {
 "node_hi": {RESPONSE: Message(text="Hi!!!")},
 "node_ok": {RESPONSE: Message(text="Okey")},
 },
 }
 
-# init actor
-actor = Actor(script, start_label=("flow", "node_hi"))
+# init pipeline
+pipeline = Pipeline.from_script(script, start_label=("flow", "node_hi"))
 
 
 # handler requests
-def turn_handler(in_request: Message, ctx: Union[Context, dict], actor: Actor):
-# Context.cast - gets an object type of [Context, str, dict] returns an object type of Context
-ctx = Context.cast(ctx)
-# Add in current context a next request of user
-ctx.add_request(in_request)
-# Pass the context into actor and it returns updated context with actor response
-ctx = actor(ctx)
+def turn_handler(in_request: Message, pipeline: Pipeline) -> Tuple[Message, Context]:
+# Pass the next request of user into pipeline and it returns updated context with actor response
+ctx = pipeline(in_request, 0)
 # Get last actor response from the context
 out_response = ctx.last_response
 # The next condition branching needs for testing
 return out_response, ctx
 
 
-ctx = {}
 while True:
 in_request = input("type your answer: ")
-out_response, ctx = turn_handler(Message(text=in_request), ctx, actor)
+out_response, ctx = turn_handler(Message(text=in_request), pipeline)
 print(out_response.text)
 ```
 
 When you run this code, you get similar output:
 ```
 type your answer: hi
 Okey
@@ -142,15 +141,15 @@
 type your answer: ok
 Okey
 type your answer: ok
 Okey
 ```
 
 To get more advanced examples, take a look at
-[examples](https://github.com/deeppavlov/dialog_flow_framework/tree/dev/examples) on GitHub.
+[tutorials](https://github.com/deeppavlov/dialog_flow_framework/tree/dev/tutorials) on GitHub.
 
 # Context Storages
 ## Description
 
 Context Storages allow you to save and retrieve user dialogue states
 (in the form of a `Context` object) using various database backends.
 
@@ -167,35 +166,30 @@
 
 Aside from this, we offer some interfaces for saving data to your local file system.
 These are not meant to be used in production, but can be helpful for prototyping your application.
 
 ## Basic example
 
 ```python
-from dff.script import Context, Actor
+from dff.script import Context
+from dff.pipeline import Pipeline
 from dff.context_storages import SQLContextStorage
 from .script import some_df_script
 
 db = SQLContextStorage("postgresql+asyncpg://user:password@host:port/dbname")
 
-actor = Actor(some_df_script, start_label=("root", "start"), fallback_label=("root", "fallback"))
+pipeline = Pipeline.from_script(some_df_script, start_label=("root", "start"), fallback_label=("root", "fallback"))
 
 
 def handle_request(request):
 user_id = request.args["user_id"]
-if user_id not in db:
-context = Context(id=user_id)
-else:
-context = db[user_id]
-new_context = actor(context)
-db[user_id] = new_context
-assert user_id in db
+new_context = pipeline(request, user_id)
 return new_context.last_response
 
 ```
 
 To get more advanced examples, take a look at
-[examples](https://github.com/deeppavlov/dialog_flow_framework/tree/dev/examples/context_storages) on GitHub.
+[tutorials](https://github.com/deeppavlov/dialog_flow_framework/tree/dev/tutorials/context_storages) on GitHub.
 
 # Contributing to the Dialog Flow Framework
 
 Please refer to [CONTRIBUTING.md](https://github.com/deeppavlov/dialog_flow_framework/blob/dev/CONTRIBUTING.md).
```

### Comparing `dff-0.3.2/dff.egg-info/SOURCES.txt` & `dff-0.4.1/dff.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -29,27 +29,27 @@
 dff/messengers/telegram/message.py
 dff/messengers/telegram/messenger.py
 dff/messengers/telegram/utils.py
 dff/pipeline/__init__.py
 dff/pipeline/conditions.py
 dff/pipeline/types.py
 dff/pipeline/pipeline/__init__.py
+dff/pipeline/pipeline/actor.py
 dff/pipeline/pipeline/component.py
 dff/pipeline/pipeline/pipeline.py
 dff/pipeline/pipeline/utils.py
 dff/pipeline/service/__init__.py
 dff/pipeline/service/extra.py
 dff/pipeline/service/group.py
 dff/pipeline/service/service.py
 dff/pipeline/service/utils.py
 dff/script/__init__.py
 dff/script/conditions/__init__.py
 dff/script/conditions/std_conditions.py
 dff/script/core/__init__.py
-dff/script/core/actor.py
 dff/script/core/context.py
 dff/script/core/keywords.py
 dff/script/core/message.py
 dff/script/core/normalization.py
 dff/script/core/script.py
 dff/script/core/types.py
 dff/script/extras/__init__.py
```

### Comparing `dff-0.3.2/dff.egg-info/requires.txt` & `dff-0.4.1/dff.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -9,180 +9,215 @@
 
 [devel]
 bump2version>=1.0.1
 build==0.7.0
 twine==4.0.0
 
 [devel_full]
+sphinx<6
+aioredis>=2.0.1
+isort<6.0.0,>=5.0.6
+sphinxcontrib-httpdomain>=1.8.0
+sqlalchemy[asyncio]>=1.4.27
+aiosqlite>=0.18.0
+mypy==0.950
+fastapi>=0.95.1
+pytest-asyncio<0.15.0,>=0.14.0
+jupyter>=1.0.0
+pytest<8.0.0,>=7.2.1
+sphinx-favicon>=1.0.1
+sphinx_gallery==0.7.0
+ydb~=2.5.0
+pytest-cov<5.0.0,>=4.0.0
+uvicorn>=0.21.1
+flake8<4.0.0,>=3.8.3
+starlette>=0.26.1
+psutil>=5.9.1
+sphinxcontrib-katex==0.9.0
+sphinxcontrib-apidoc==0.3.0
+sphinx_copybutton>=0.5
+asyncpg>=0.27.0
 aiofiles>=22.1.0
+idna>=3.4
+requests>=2.28.1
+pydata_sphinx_theme>=0.12.0
+flask[async]>=2.1.2
+pydantic>=1.8.2
+websockets>=11.0
+h11>=0.14.0
+nbsphinx>=0.8.9
+sniffio>=1.3.0
 black==20.8b1
-psutil>=5.9.1
-sphinx_gallery==0.7.0
 sphinx-autodoc-typehints>=1.19.4
-mypy==0.950
-nbsphinx>=0.8.9
-ydb>=2.5.0
-aioredis>=2.0.1
-telethon<2.0,>=1.27.0
-sphinxcontrib-apidoc==0.3.0
-sphinx<6
-flake8<4.0.0,>=3.8.3
+twine==4.0.0
+click<=8.0.4
 asyncmy>=0.2.5
 motor>=3.1.1
-jupyter>=1.0.0
-requests>=2.28.1
-flask[async]>=2.1.2
-nest_asyncio>=1.5.5
-pytest<8.0.0,>=7.2.1
-pydata_sphinx_theme>=0.12.0
+six>=1.16.0
 bump2version>=1.0.1
-click<=8.0.4
+typing_extensions>=4.0.0
+telethon<2.0,>=1.27.0
 cryptography>=36.0.2
-pytest-asyncio<0.15.0,>=0.14.0
-sqlalchemy[asyncio]>=1.4.27
-asyncpg>=0.27.0
-sphinxcontrib-httpdomain>=1.8.0
-sphinx_copybutton>=0.5
-pytelegrambotapi==4.5.1
-sqlalchemy[asyncio]>=2.0.2
-sphinxcontrib-katex==0.9.0
-pydantic>=1.8.2
-aiosqlite>=0.18.0
+nest_asyncio>=1.5.5
 build==0.7.0
+sqlalchemy[asyncio]>=2.0.2
+pytelegrambotapi==4.5.1
+anyio>=3.6.2
 jupytext>=1.14.1
-isort<6.0.0,>=5.0.6
-typing_extensions>=4.0.0
-twine==4.0.0
-six>=1.16.0
-pytest-cov<5.0.0,>=4.0.0
 
 [doc]
 sphinx<6
-pydata_sphinx_theme>=0.12.0
-sphinxcontrib-apidoc==0.3.0
-sphinxcontrib-httpdomain>=1.8.0
 sphinxcontrib-katex==0.9.0
+sphinxcontrib-apidoc==0.3.0
 sphinx_copybutton>=0.5
+jupyter>=1.0.0
+sphinx-favicon>=1.0.1
+requests>=2.28.1
+sphinxcontrib-httpdomain>=1.8.0
+pydata_sphinx_theme>=0.12.0
 sphinx_gallery==0.7.0
-sphinx-autodoc-typehints>=1.19.4
 nbsphinx>=0.8.9
+sphinx-autodoc-typehints>=1.19.4
 jupytext>=1.14.1
-jupyter>=1.0.0
 
-[examples]
-aiofiles>=22.1.0
-black==20.8b1
-psutil>=5.9.1
-ydb>=2.5.0
-aioredis>=2.0.1
-telethon<2.0,>=1.27.0
-flake8<4.0.0,>=3.8.3
-six>=1.16.0
+[full]
 asyncmy>=0.2.5
 motor>=3.1.1
-requests>=2.28.1
-nest_asyncio>=1.5.5
-flask[async]>=2.1.2
-pytest<8.0.0,>=7.2.1
-click<=8.0.4
-cryptography>=36.0.2
-pytest-asyncio<0.15.0,>=0.14.0
-sqlalchemy[asyncio]>=1.4.27
+aioredis>=2.0.1
+six>=1.16.0
 asyncpg>=0.27.0
-pytelegrambotapi==4.5.1
-pydantic>=1.8.2
-aiosqlite>=0.18.0
-isort<6.0.0,>=5.0.6
 typing_extensions>=4.0.0
-sqlalchemy[asyncio]>=2.0.2
-pytest-cov<5.0.0,>=4.0.0
-
-[full]
 aiofiles>=22.1.0
-pydantic>=1.8.2
-aiosqlite>=0.18.0
-typing_extensions>=4.0.0
+pytelegrambotapi==4.5.1
 cryptography>=36.0.2
-ydb>=2.5.0
-six>=1.16.0
-asyncmy>=0.2.5
-motor>=3.1.1
-sqlalchemy[asyncio]>=1.4.27
-asyncpg>=0.27.0
-sqlalchemy[asyncio]>=2.0.2
 nest_asyncio>=1.5.5
-aioredis>=2.0.1
-pytelegrambotapi==4.5.1
+ydb~=2.5.0
+pydantic>=1.8.2
+sqlalchemy[asyncio]>=2.0.2
+sqlalchemy[asyncio]>=1.4.27
+aiosqlite>=0.18.0
 
 [json]
 aiofiles>=22.1.0
 
 [mongodb]
 motor>=3.1.1
 
 [mysql]
-sqlalchemy[asyncio]>=2.0.2
-asyncmy>=0.2.5
 cryptography>=36.0.2
+asyncmy>=0.2.5
+sqlalchemy[asyncio]>=2.0.2
 
 [pickle]
 aiofiles>=22.1.0
 
 [postgresql]
-sqlalchemy[asyncio]>=2.0.2
 asyncpg>=0.27.0
+sqlalchemy[asyncio]>=2.0.2
 
 [redis]
 aioredis>=2.0.1
 
 [sqlite]
-sqlalchemy[asyncio]>=2.0.2
-aiosqlite>=0.18.0
 sqlalchemy[asyncio]>=1.4.27
+aiosqlite>=0.18.0
+sqlalchemy[asyncio]>=2.0.2
 
 [telegram]
 pytelegrambotapi==4.5.1
 
 [test_full]
-aiofiles>=22.1.0
-black==20.8b1
-psutil>=5.9.1
-ydb>=2.5.0
 aioredis>=2.0.1
-telethon<2.0,>=1.27.0
+isort<6.0.0,>=5.0.6
+sqlalchemy[asyncio]>=1.4.27
+aiosqlite>=0.18.0
+fastapi>=0.95.1
+pytest-asyncio<0.15.0,>=0.14.0
+pytest<8.0.0,>=7.2.1
+ydb~=2.5.0
+pytest-cov<5.0.0,>=4.0.0
+uvicorn>=0.21.1
 flake8<4.0.0,>=3.8.3
-six>=1.16.0
-asyncmy>=0.2.5
-motor>=3.1.1
+starlette>=0.26.1
+psutil>=5.9.1
+asyncpg>=0.27.0
+aiofiles>=22.1.0
+idna>=3.4
 requests>=2.28.1
-nest_asyncio>=1.5.5
 flask[async]>=2.1.2
-pytest<8.0.0,>=7.2.1
-click<=8.0.4
-cryptography>=36.0.2
-pytest-asyncio<0.15.0,>=0.14.0
-sqlalchemy[asyncio]>=1.4.27
-asyncpg>=0.27.0
-pytelegrambotapi==4.5.1
 pydantic>=1.8.2
-aiosqlite>=0.18.0
-isort<6.0.0,>=5.0.6
+websockets>=11.0
+h11>=0.14.0
+sniffio>=1.3.0
+black==20.8b1
+click<=8.0.4
+asyncmy>=0.2.5
+motor>=3.1.1
+six>=1.16.0
 typing_extensions>=4.0.0
+telethon<2.0,>=1.27.0
+cryptography>=36.0.2
+nest_asyncio>=1.5.5
 sqlalchemy[asyncio]>=2.0.2
-pytest-cov<5.0.0,>=4.0.0
+pytelegrambotapi==4.5.1
+anyio>=3.6.2
 
 [tests]
+isort<6.0.0,>=5.0.6
+fastapi>=0.95.1
+pytest-asyncio<0.15.0,>=0.14.0
 pytest<8.0.0,>=7.2.1
 pytest-cov<5.0.0,>=4.0.0
-pytest-asyncio<0.15.0,>=0.14.0
+uvicorn>=0.21.1
 flake8<4.0.0,>=3.8.3
-click<=8.0.4
+starlette>=0.26.1
+psutil>=5.9.1
+idna>=3.4
+requests>=2.28.1
+flask[async]>=2.1.2
+websockets>=11.0
+h11>=0.14.0
+sniffio>=1.3.0
 black==20.8b1
+click<=8.0.4
+telethon<2.0,>=1.27.0
+anyio>=3.6.2
+
+[tutorials]
+aioredis>=2.0.1
 isort<6.0.0,>=5.0.6
-flask[async]>=2.1.2
+sqlalchemy[asyncio]>=1.4.27
+aiosqlite>=0.18.0
+fastapi>=0.95.1
+pytest-asyncio<0.15.0,>=0.14.0
+pytest<8.0.0,>=7.2.1
+ydb~=2.5.0
+pytest-cov<5.0.0,>=4.0.0
+uvicorn>=0.21.1
+flake8<4.0.0,>=3.8.3
+starlette>=0.26.1
 psutil>=5.9.1
+asyncpg>=0.27.0
+aiofiles>=22.1.0
+idna>=3.4
 requests>=2.28.1
+flask[async]>=2.1.2
+pydantic>=1.8.2
+websockets>=11.0
+h11>=0.14.0
+sniffio>=1.3.0
+black==20.8b1
+click<=8.0.4
+asyncmy>=0.2.5
+motor>=3.1.1
+six>=1.16.0
+typing_extensions>=4.0.0
 telethon<2.0,>=1.27.0
+cryptography>=36.0.2
+nest_asyncio>=1.5.5
+sqlalchemy[asyncio]>=2.0.2
+pytelegrambotapi==4.5.1
+anyio>=3.6.2
 
 [ydb]
-ydb>=2.5.0
+ydb~=2.5.0
 six>=1.16.0
```

### Comparing `dff-0.3.2/setup.py` & `dff-0.4.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import pathlib
-from typing import Iterable, List
+from typing import List
 
 from setuptools import setup, find_packages
 
 
 LOCATION = pathlib.Path(__file__).parent.resolve()
 
 
@@ -14,15 +14,15 @@
 readme_file = LOCATION / "README.md"
 
 readme_lines = [line.strip() for line in readme_file.open(encoding="utf-8").readlines()]
 description = [line for line in readme_lines if line and not line.startswith("#")][0]
 long_description = "\n".join(readme_lines)
 
 
-def merge_req_lists(req_lists: Iterable[List[str]]) -> List[str]:
+def merge_req_lists(*req_lists: List[str]) -> List[str]:
     result: set[str] = set()
     for req_list in req_lists:
         for req in req_list:
             result.add(req)
     return list(result)
 
 
@@ -45,117 +45,123 @@
 ]
 
 _sql_dependencies = [
     "sqlalchemy[asyncio]>=2.0.2",
 ]
 
 sqlite_dependencies = merge_req_lists(
+    _sql_dependencies,
     [
-        _sql_dependencies,
-        [
-            "aiosqlite>=0.18.0",
-            "sqlalchemy[asyncio]>=1.4.27",
-        ],
-    ]
+        "aiosqlite>=0.18.0",
+        "sqlalchemy[asyncio]>=1.4.27",
+    ],
 )
 
 mysql_dependencies = merge_req_lists(
+    _sql_dependencies,
     [
-        _sql_dependencies,
-        [
-            "asyncmy>=0.2.5",
-            "cryptography>=36.0.2",
-        ],
-    ]
+        "asyncmy>=0.2.5",
+        "cryptography>=36.0.2",
+    ],
 )
 
 postgresql_dependencies = merge_req_lists(
+    _sql_dependencies,
     [
-        _sql_dependencies,
-        [
-            "asyncpg>=0.27.0",
-        ],
-    ]
+        "asyncpg>=0.27.0",
+    ],
 )
 
 ydb_dependencies = [
-    "ydb>=2.5.0",
+    "ydb~=2.5.0",
     "six>=1.16.0",
 ]
 
 telegram_dependencies = [
     "pytelegrambotapi==4.5.1",
 ]
 
 full = merge_req_lists(
-    [
-        core,
-        async_files_dependencies,
-        sqlite_dependencies,
-        redis_dependencies,
-        mongodb_dependencies,
-        mysql_dependencies,
-        postgresql_dependencies,
-        ydb_dependencies,
-        telegram_dependencies,
-    ]
-)
-
-test_requirements = [
-    "pytest >=7.2.1,<8.0.0",
-    "pytest-cov >=4.0.0,<5.0.0",
-    "pytest-asyncio >=0.14.0,<0.15.0",
-    "flake8 >=3.8.3,<4.0.0",
-    "click<=8.0.4",
-    "black ==20.8b1",
-    "isort >=5.0.6,<6.0.0",
-    "flask[async]>=2.1.2",
-    "psutil>=5.9.1",
+    core,
+    async_files_dependencies,
+    sqlite_dependencies,
+    redis_dependencies,
+    mongodb_dependencies,
+    mysql_dependencies,
+    postgresql_dependencies,
+    ydb_dependencies,
+    telegram_dependencies,
+)
+
+requests_requirements = [
     "requests>=2.28.1",
-    "telethon>=1.27.0,<2.0",
 ]
 
+test_requirements = merge_req_lists(
+    [
+        "pytest >=7.2.1,<8.0.0",
+        "pytest-cov >=4.0.0,<5.0.0",
+        "pytest-asyncio >=0.14.0,<0.15.0",
+        "flake8 >=3.8.3,<4.0.0",
+        "click<=8.0.4",
+        "black ==20.8b1",
+        "isort >=5.0.6,<6.0.0",
+        "flask[async]>=2.1.2",
+        "psutil>=5.9.1",
+        "telethon>=1.27.0,<2.0",
+        "anyio>=3.6.2",
+        "fastapi>=0.95.1",
+        "idna>=3.4",
+        "sniffio>=1.3.0",
+        "starlette>=0.26.1",
+        "h11>=0.14.0",
+        "uvicorn>=0.21.1",
+        "websockets>=11.0",
+    ],
+    requests_requirements,
+)
+
 tests_full = merge_req_lists(
+    full,
+    test_requirements,
+)
+
+doc = merge_req_lists(
     [
-        full,
-        test_requirements,
-    ]
-)
-
-doc = [
-    "sphinx<6",
-    "pydata_sphinx_theme>=0.12.0",
-    "sphinxcontrib-apidoc==0.3.0",
-    "sphinxcontrib-httpdomain>=1.8.0",
-    "sphinxcontrib-katex==0.9.0",
-    "sphinx_copybutton>=0.5",
-    "sphinx_gallery==0.7.0",
-    "sphinx-autodoc-typehints>=1.19.4",
-    "nbsphinx>=0.8.9",
-    "jupytext>=1.14.1",
-    "jupyter>=1.0.0",
-]
+        "sphinx<6",
+        "pydata_sphinx_theme>=0.12.0",
+        "sphinxcontrib-apidoc==0.3.0",
+        "sphinxcontrib-httpdomain>=1.8.0",
+        "sphinxcontrib-katex==0.9.0",
+        "sphinx-favicon>=1.0.1",
+        "sphinx_copybutton>=0.5",
+        "sphinx_gallery==0.7.0",
+        "sphinx-autodoc-typehints>=1.19.4",
+        "nbsphinx>=0.8.9",
+        "jupytext>=1.14.1",
+        "jupyter>=1.0.0",
+    ],
+    requests_requirements,
+)
 
 devel = [
     "bump2version>=1.0.1",
     "build==0.7.0",
     "twine==4.0.0",
 ]
 
 mypy_dependencies = [
     "mypy==0.950",
 ]
 
 devel_full = merge_req_lists(
-    [
-        tests_full,
-        doc,
-        devel,
-        mypy_dependencies,
-    ]
+    tests_full,
+    doc,
+    devel,
+    mypy_dependencies,
 )
 
 EXTRA_DEPENDENCIES = {
     "core": core,  # minimal dependencies (by default)
     "json": async_files_dependencies,  # dependencies for using JSON
     "pickle": async_files_dependencies,  # dependencies for using Pickle
     "sqlite": sqlite_dependencies,  # dependencies for using SQLite
@@ -164,23 +170,23 @@
     "mysql": mysql_dependencies,  # dependencies for using MySQL
     "postgresql": postgresql_dependencies,  # dependencies for using PostgreSQL
     "ydb": ydb_dependencies,  # dependencies for using Yandex Database
     "telegram": telegram_dependencies,  # dependencies for using Telegram
     "full": full,  # full dependencies including all options above
     "tests": test_requirements,  # dependencies for running tests
     "test_full": tests_full,  # full dependencies for running all tests (all options above)
-    "examples": tests_full,  # dependencies for running examples (all options above)
+    "tutorials": tests_full,  # dependencies for running tutorials (all options above)
     "devel": devel,  # dependencies for development
     "doc": doc,  # dependencies for documentation
     "devel_full": devel_full,  # full dependencies for development (all options above)
 }
 
 setup(
     name="dff",
-    version="0.3.2",
+    version="0.4.1",
     description=description,
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/deeppavlov/dialog_flow_framework",
     author="Denis Kuznetsov",
     author_email="kuznetsov.den.p@gmail.com",
     classifiers=[  # Optional
```

