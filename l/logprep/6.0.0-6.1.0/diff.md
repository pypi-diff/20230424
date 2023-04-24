# Comparing `tmp/logprep-6.0.0.tar.gz` & `tmp/logprep-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logprep-6.0.0.tar", last modified: Thu Mar 23 12:51:53 2023, max compression
+gzip compressed data, was "logprep-6.1.0.tar", last modified: Mon Apr 24 10:09:11 2023, max compression
```

## Comparing `logprep-6.0.0.tar` & `logprep-6.1.0.tar`

### file list

```diff
@@ -1,440 +1,479 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.809565 logprep-6.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-03-23 12:51:50.000000 logprep-6.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-23 12:51:50.000000 logprep-6.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-03-23 12:51:53.813565 logprep-6.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16889 2023-03-23 12:51:50.000000 logprep-6.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.813565 logprep-6.0.0/logprep/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-23 12:51:53.813565 logprep-6.0.0/logprep/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.781565 logprep-6.0.0/logprep/abc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/abc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/abc/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/abc/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/abc/getter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15656 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/abc/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/abc/output.py
--rw-r--r--   0 runner    (1001) docker     (123)    11396 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/abc/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.781565 logprep-6.0.0/logprep/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/connector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.781565 logprep-6.0.0/logprep/connector/confluent_kafka/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/connector/confluent_kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/connector/confluent_kafka/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/connector/confluent_kafka/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.781565 logprep-6.0.0/logprep/connector/console/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/connector/console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/connector/console/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.781565 logprep-6.0.0/logprep/connector/dummy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/connector/dummy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/connector/dummy/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/connector/dummy/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.781565 logprep-6.0.0/logprep/connector/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/connector/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13270 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/connector/elasticsearch/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.781565 logprep-6.0.0/logprep/connector/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/connector/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/connector/file/input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.781565 logprep-6.0.0/logprep/connector/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/connector/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/connector/http/input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.781565 logprep-6.0.0/logprep/connector/json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/connector/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/connector/json/input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.781565 logprep-6.0.0/logprep/connector/jsonl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/connector/jsonl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/connector/jsonl/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/connector/jsonl/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.785565 logprep-6.0.0/logprep/connector/opensearch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/connector/opensearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/connector/opensearch/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/factory_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.785565 logprep-6.0.0/logprep/filter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/filter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.785565 logprep-6.0.0/logprep/filter/expression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/filter/expression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11322 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/filter/expression/filter_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/filter/lucene_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.785565 logprep-6.0.0/logprep/framework/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21761 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/framework/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/framework/pipeline_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.785565 logprep-6.0.0/logprep/framework/rule_tree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/framework/rule_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/framework/rule_tree/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    22374 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/framework/rule_tree/rule_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/framework/rule_tree/rule_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.785565 logprep-6.0.0/logprep/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/metrics/metric_exposer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/metrics/metric_targets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.785565 logprep-6.0.0/logprep/processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.785565 logprep-6.0.0/logprep/processor/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12030 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/base/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.785565 logprep-6.0.0/logprep/processor/calculator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/calculator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/calculator/fourFn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/calculator/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/calculator/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.785565 logprep-6.0.0/logprep/processor/clusterer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/clusterer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/clusterer/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/clusterer/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/clusterer/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.785565 logprep-6.0.0/logprep/processor/clusterer/signature_calculation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/clusterer/signature_calculation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.785565 logprep-6.0.0/logprep/processor/clusterer/signature_calculation/rules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/clusterer/signature_calculation/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/clusterer/signature_calculation/rules/rule_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/clusterer/signature_calculation/signature_phase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.785565 logprep-6.0.0/logprep/processor/concatenator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/concatenator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/concatenator/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/concatenator/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.785565 logprep-6.0.0/logprep/processor/datetime_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/datetime_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/datetime_extractor/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/datetime_extractor/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.785565 logprep-6.0.0/logprep/processor/deleter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/deleter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/deleter/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/deleter/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.789565 logprep-6.0.0/logprep/processor/dissector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/dissector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/dissector/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/dissector/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.789565 logprep-6.0.0/logprep/processor/domain_label_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/domain_label_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/domain_label_extractor/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/domain_label_extractor/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.789565 logprep-6.0.0/logprep/processor/domain_resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/domain_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8796 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/domain_resolver/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/domain_resolver/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.789565 logprep-6.0.0/logprep/processor/dropper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/dropper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/dropper/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/dropper/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.789565 logprep-6.0.0/logprep/processor/field_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/field_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/field_manager/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/field_manager/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.789565 logprep-6.0.0/logprep/processor/generic_adder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/generic_adder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/generic_adder/mysql_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    10641 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/generic_adder/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9198 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/generic_adder/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.789565 logprep-6.0.0/logprep/processor/generic_resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/generic_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/generic_resolver/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/generic_resolver/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.789565 logprep-6.0.0/logprep/processor/geoip_enricher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/geoip_enricher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/geoip_enricher/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/geoip_enricher/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.789565 logprep-6.0.0/logprep/processor/hyperscan_resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/hyperscan_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/hyperscan_resolver/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/hyperscan_resolver/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.789565 logprep-6.0.0/logprep/processor/ip_informer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/ip_informer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/ip_informer/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/ip_informer/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.789565 logprep-6.0.0/logprep/processor/key_checker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/key_checker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/key_checker/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/key_checker/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.789565 logprep-6.0.0/logprep/processor/labeler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/labeler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/labeler/labeling_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/labeler/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/labeler/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.789565 logprep-6.0.0/logprep/processor/list_comparison/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/list_comparison/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/list_comparison/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/list_comparison/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.789565 logprep-6.0.0/logprep/processor/normalizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/normalizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16306 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/normalizer/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    28522 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/normalizer/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.793565 logprep-6.0.0/logprep/processor/pre_detector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/pre_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/pre_detector/ip_alerter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/pre_detector/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/pre_detector/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/processor_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.793565 logprep-6.0.0/logprep/processor/pseudonymizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/pseudonymizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/pseudonymizer/encrypter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15975 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/pseudonymizer/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/pseudonymizer/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.793565 logprep-6.0.0/logprep/processor/requester/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/requester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/requester/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/requester/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.793565 logprep-6.0.0/logprep/processor/selective_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/selective_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/selective_extractor/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/selective_extractor/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.793565 logprep-6.0.0/logprep/processor/string_splitter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/string_splitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/string_splitter/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/string_splitter/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.793565 logprep-6.0.0/logprep/processor/template_replacer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/template_replacer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/template_replacer/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/template_replacer/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.793565 logprep-6.0.0/logprep/processor/timestamp_differ/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/timestamp_differ/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/timestamp_differ/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/processor/timestamp_differ/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/run_logprep.py
--rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.793565 logprep-6.0.0/logprep/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/util/aggregating_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.797565 logprep-6.0.0/logprep/util/auto_rule_tester/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/util/auto_rule_tester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17190 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/util/auto_rule_tester/auto_rule_corpus_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)    26978 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/util/auto_rule_tester/auto_rule_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     8167 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/util/auto_rule_tester/grok_pattern_replacer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/util/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    19307 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/util/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/util/getter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/util/grok_pattern_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/util/hasher.py
--rw-r--r--   0 runner    (1001) docker     (123)     9204 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/util/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/util/json_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/util/log_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/util/multiprocessing_log_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/util/pipeline_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12537 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/util/pre_detector_rule_matching_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/util/processor_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/util/prometheus_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/util/rule_dry_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/util/schema_and_rule_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/util/time_measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-03-23 12:51:50.000000 logprep-6.0.0/logprep/util/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.781565 logprep-6.0.0/logprep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-03-23 12:51:53.000000 logprep-6.0.0/logprep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14517 2023-03-23 12:51:53.000000 logprep-6.0.0/logprep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 12:51:53.000000 logprep-6.0.0/logprep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-23 12:51:53.000000 logprep-6.0.0/logprep.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-03-23 12:51:53.000000 logprep-6.0.0/logprep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-23 12:51:53.000000 logprep-6.0.0/logprep.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-23 12:51:50.000000 logprep-6.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-03-23 12:51:53.813565 logprep-6.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-03-23 12:51:50.000000 logprep-6.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.797565 logprep-6.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.797565 logprep-6.0.0/tests/acceptance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/acceptance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/acceptance/test_config_refresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/acceptance/test_file_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     9171 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/acceptance/test_full_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/acceptance/test_http_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5199 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/acceptance/test_multiple_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19060 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/acceptance/test_pre_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/acceptance/test_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/acceptance/test_selective_extractor_full_pipeline_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/acceptance/test_wineventlog_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/acceptance/test_wineventlog_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/acceptance/test_wineventlog_pseudonymization.py
--rw-r--r--   0 runner    (1001) docker     (123)    10367 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/acceptance/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.797565 logprep-6.0.0/tests/ci/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/ci/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.797565 logprep-6.0.0/tests/ci/runner-image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/ci/runner-image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.797565 logprep-6.0.0/tests/ci/runner-image/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/ci/runner-image/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/ci/runner-image/scripts/compare_json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.797565 logprep-6.0.0/tests/testdata/
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/testdata/ConfigurationForTest.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/testdata/FilledTempFile.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/testdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/testdata/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/testdata/ruledata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.797565 logprep-6.0.0/tests/testdata/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/testdata/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.797565 logprep-6.0.0/tests/testdata/unit/clusterer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/testdata/unit/clusterer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12733 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/testdata/unit/clusterer/test_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.797565 logprep-6.0.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.801565 logprep-6.0.0/tests/unit/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22045 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/connector/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/connector/test_confluent_kafka_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/connector/test_confluent_kafka_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/connector/test_confluent_kafka_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/connector/test_console_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/connector/test_dummy_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/connector/test_dummy_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     9075 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/connector/test_elasticsearch_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     9926 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/connector/test_file_input_default_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/connector/test_file_input_not_tailing_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/connector/test_file_input_start_at_end_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/connector/test_http_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/connector/test_json_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/connector/test_jsonl_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/connector/test_jsonl_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     9869 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/connector/test_opensearch_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.801565 logprep-6.0.0/tests/unit/filter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17640 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/filter/test_filter_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/filter/test_lucene_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.801565 logprep-6.0.0/tests/unit/framework/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.801565 logprep-6.0.0/tests/unit/framework/rule_tree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/framework/rule_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/framework/rule_tree/test_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    25387 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/framework/rule_tree/test_rule_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    19943 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/framework/rule_tree/test_rule_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    38431 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/framework/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/framework/test_pipeline_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.801565 logprep-6.0.0/tests/unit/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/metrics/test_metric_exposer.py
--rw-r--r--   0 runner    (1001) docker     (123)    22193 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/metrics/test_metric_targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/metrics/test_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.801565 logprep-6.0.0/tests/unit/processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14462 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.801565 logprep-6.0.0/tests/unit/processor/calculator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/calculator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11619 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/calculator/test_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/calculator/test_calculator_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.801565 logprep-6.0.0/tests/unit/processor/clusterer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/clusterer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/clusterer/test_clusterer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/clusterer/test_clusterer_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/clusterer/test_clusterer_signature_phase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.801565 logprep-6.0.0/tests/unit/processor/concatenator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/concatenator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/concatenator/test_concatenator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11216 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/concatenator/test_concatenator_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.801565 logprep-6.0.0/tests/unit/processor/datetime_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/datetime_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/datetime_extractor/test_datetime_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/datetime_extractor/test_datetime_extractor_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.801565 logprep-6.0.0/tests/unit/processor/deleter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/deleter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/deleter/test_deleter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/deleter/test_deleter_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.805565 logprep-6.0.0/tests/unit/processor/dissector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/dissector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19593 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/dissector/test_dissector.py
--rw-r--r--   0 runner    (1001) docker     (123)    17681 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/dissector/test_dissector_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.805565 logprep-6.0.0/tests/unit/processor/domain_label_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/domain_label_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13354 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.805565 logprep-6.0.0/tests/unit/processor/domain_resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/domain_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12028 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/domain_resolver/test_domain_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/domain_resolver/test_domain_resolver_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.805565 logprep-6.0.0/tests/unit/processor/dropper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/dropper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/dropper/test_dropper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/dropper/test_dropper_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.805565 logprep-6.0.0/tests/unit/processor/field_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/field_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13469 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/field_manager/test_field_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/field_manager/test_field_manager_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.805565 logprep-6.0.0/tests/unit/processor/generic_adder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/generic_adder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30415 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/generic_adder/test_generic_adder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/generic_adder/test_generic_adder_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.805565 logprep-6.0.0/tests/unit/processor/generic_resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/generic_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/generic_resolver/test_generic_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/generic_resolver/test_generic_resolver_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.805565 logprep-6.0.0/tests/unit/processor/geoip_enricher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/geoip_enricher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/geoip_enricher/test_geoip_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/geoip_enricher/test_geoip_enricher_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.805565 logprep-6.0.0/tests/unit/processor/hyperscan_resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/hyperscan_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23067 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.805565 logprep-6.0.0/tests/unit/processor/ip_informer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/ip_informer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13575 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/ip_informer/test_ip_informer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/ip_informer/test_ip_informer_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.805565 logprep-6.0.0/tests/unit/processor/labeler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/labeler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/labeler/test_labeler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/labeler/test_labeler_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    12544 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/labeler/test_labeling_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.805565 logprep-6.0.0/tests/unit/processor/list_comparison/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/list_comparison/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11280 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/list_comparison/test_list_comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/list_comparison/test_list_comparison_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.805565 logprep-6.0.0/tests/unit/processor/normalizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/normalizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38697 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/normalizer/test_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/normalizer/test_normalizer_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.809565 logprep-6.0.0/tests/unit/processor/pre_detector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/pre_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/pre_detector/test_ip_alerter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/pre_detector/test_pre_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/pre_detector/test_pre_detector_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.809565 logprep-6.0.0/tests/unit/processor/pseudonymizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/pseudonymizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/pseudonymizer/test_encrypter.py
--rw-r--r--   0 runner    (1001) docker     (123)    29603 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/pseudonymizer/test_pseudonymizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/pseudonymizer/test_pseudonymizer_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.809565 logprep-6.0.0/tests/unit/processor/requester/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/requester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12218 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/requester/test_requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/requester/test_requester_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.809565 logprep-6.0.0/tests/unit/processor/selective_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/selective_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/selective_extractor/test_selective_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/selective_extractor/test_selective_extractor_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.809565 logprep-6.0.0/tests/unit/processor/string_splitter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/string_splitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/string_splitter/test_string_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/string_splitter/test_string_splitter_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.809565 logprep-6.0.0/tests/unit/processor/template_replacer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/template_replacer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/template_replacer/test_template_replacer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/test_processor_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/test_processor_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.809565 logprep-6.0.0/tests/unit/processor/timestamp_differ/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/timestamp_differ/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17227 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/timestamp_differ/test_timestamp_differ.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/processor/timestamp_differ/test_timestamp_differ_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/test_run_logprep.py
--rw-r--r--   0 runner    (1001) docker     (123)    18858 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/test_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.809565 logprep-6.0.0/tests/unit/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17223 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/util/test_auto_rule_corpus_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/util/test_auto_rule_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/util/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    39375 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/util/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    16251 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/util/test_getter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/util/test_grok_pattern_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/util/test_hasher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/util/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/util/test_helper_add_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/util/test_log_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/util/test_processor_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/util/test_prometheus_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7685 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/util/test_rule_dry_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/util/test_schema_and_rule_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/util/test_time_measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)    16746 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/util/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/unit/util/tests_json_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:53.809565 logprep-6.0.0/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-03-23 12:51:50.000000 logprep-6.0.0/tests/util/testhelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    81000 2023-03-23 12:51:50.000000 logprep-6.0.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.092395 logprep-6.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-04-24 10:09:06.000000 logprep-6.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-24 10:09:06.000000 logprep-6.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-04-24 10:09:11.092395 logprep-6.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16889 2023-04-24 10:09:06.000000 logprep-6.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.092395 logprep-6.1.0/logprep/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-24 10:09:11.092395 logprep-6.1.0/logprep/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.056394 logprep-6.1.0/logprep/abc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/abc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/abc/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/abc/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/abc/getter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16468 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/abc/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/abc/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12024 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/abc/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.056394 logprep-6.1.0/logprep/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.056394 logprep-6.1.0/logprep/connector/confluent_kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/confluent_kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12736 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/confluent_kafka/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8002 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/confluent_kafka/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.056394 logprep-6.1.0/logprep/connector/console/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/console/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.056394 logprep-6.1.0/logprep/connector/dummy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/dummy/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/dummy/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.056394 logprep-6.1.0/logprep/connector/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13442 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/elasticsearch/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.060394 logprep-6.1.0/logprep/connector/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/file/input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.060394 logprep-6.1.0/logprep/connector/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/http/input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.060394 logprep-6.1.0/logprep/connector/json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/json/input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.060394 logprep-6.1.0/logprep/connector/jsonl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/jsonl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/jsonl/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/jsonl/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.060394 logprep-6.1.0/logprep/connector/opensearch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/opensearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/opensearch/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.060394 logprep-6.1.0/logprep/connector/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11760 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/s3/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/factory_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.060394 logprep-6.1.0/logprep/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/filter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.060394 logprep-6.1.0/logprep/filter/expression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/filter/expression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11681 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/filter/expression/filter_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14986 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/filter/lucene_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.060394 logprep-6.1.0/logprep/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19708 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/framework/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/framework/pipeline_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.060394 logprep-6.1.0/logprep/framework/rule_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/framework/rule_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/framework/rule_tree/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22708 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/framework/rule_tree/rule_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/framework/rule_tree/rule_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.060394 logprep-6.1.0/logprep/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/metrics/metric_exposer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/metrics/metric_targets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.060394 logprep-6.1.0/logprep/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.060394 logprep-6.1.0/logprep/processor/amides/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/amides/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/amides/detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/amides/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/amides/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11157 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/amides/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/amides/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.060394 logprep-6.1.0/logprep/processor/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/base/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.064394 logprep-6.1.0/logprep/processor/calculator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/calculator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/calculator/fourFn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/calculator/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/calculator/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.064394 logprep-6.1.0/logprep/processor/clusterer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/clusterer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/clusterer/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/clusterer/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/clusterer/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.064394 logprep-6.1.0/logprep/processor/clusterer/signature_calculation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/clusterer/signature_calculation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.064394 logprep-6.1.0/logprep/processor/clusterer/signature_calculation/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/clusterer/signature_calculation/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/clusterer/signature_calculation/rules/rule_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/clusterer/signature_calculation/signature_phase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.064394 logprep-6.1.0/logprep/processor/concatenator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/concatenator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/concatenator/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/concatenator/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.064394 logprep-6.1.0/logprep/processor/datetime_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/datetime_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/datetime_extractor/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/datetime_extractor/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.064394 logprep-6.1.0/logprep/processor/deleter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/deleter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/deleter/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/deleter/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.064394 logprep-6.1.0/logprep/processor/dissector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/dissector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/dissector/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8710 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/dissector/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.064394 logprep-6.1.0/logprep/processor/domain_label_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/domain_label_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/domain_label_extractor/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/domain_label_extractor/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.064394 logprep-6.1.0/logprep/processor/domain_resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/domain_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8276 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/domain_resolver/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/domain_resolver/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.064394 logprep-6.1.0/logprep/processor/dropper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/dropper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/dropper/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/dropper/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.064394 logprep-6.1.0/logprep/processor/field_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/field_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/field_manager/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/field_manager/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.064394 logprep-6.1.0/logprep/processor/generic_adder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/generic_adder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/generic_adder/mysql_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/generic_adder/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9198 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/generic_adder/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.064394 logprep-6.1.0/logprep/processor/generic_resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/generic_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/generic_resolver/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/generic_resolver/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.068394 logprep-6.1.0/logprep/processor/geoip_enricher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/geoip_enricher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/geoip_enricher/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/geoip_enricher/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.068394 logprep-6.1.0/logprep/processor/grokker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/grokker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/grokker/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/grokker/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.068394 logprep-6.1.0/logprep/processor/hyperscan_resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/hyperscan_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/hyperscan_resolver/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/hyperscan_resolver/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.068394 logprep-6.1.0/logprep/processor/ip_informer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/ip_informer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/ip_informer/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/ip_informer/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.068394 logprep-6.1.0/logprep/processor/key_checker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/key_checker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/key_checker/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/key_checker/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.068394 logprep-6.1.0/logprep/processor/labeler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/labeler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/labeler/labeling_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/labeler/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/labeler/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.068394 logprep-6.1.0/logprep/processor/list_comparison/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/list_comparison/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/list_comparison/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/list_comparison/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.068394 logprep-6.1.0/logprep/processor/normalizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/normalizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16548 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/normalizer/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28741 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/normalizer/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.068394 logprep-6.1.0/logprep/processor/pre_detector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/pre_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/pre_detector/ip_alerter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/pre_detector/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/pre_detector/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/processor_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.068394 logprep-6.1.0/logprep/processor/pseudonymizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/pseudonymizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/pseudonymizer/encrypter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16129 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/pseudonymizer/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/pseudonymizer/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.068394 logprep-6.1.0/logprep/processor/requester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/requester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/requester/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/requester/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.068394 logprep-6.1.0/logprep/processor/selective_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/selective_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/selective_extractor/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/selective_extractor/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.072394 logprep-6.1.0/logprep/processor/string_splitter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/string_splitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/string_splitter/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/string_splitter/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.072394 logprep-6.1.0/logprep/processor/template_replacer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/template_replacer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/template_replacer/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/template_replacer/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.072394 logprep-6.1.0/logprep/processor/timestamp_differ/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/timestamp_differ/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/timestamp_differ/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/timestamp_differ/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/run_logprep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.072394 logprep-6.1.0/logprep/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/aggregating_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.072394 logprep-6.1.0/logprep/util/auto_rule_tester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/auto_rule_tester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17268 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/auto_rule_tester/auto_rule_corpus_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26980 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/auto_rule_tester/auto_rule_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/auto_rule_tester/grok_pattern_replacer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19307 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/getter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.072394 logprep-6.1.0/logprep/util/grok/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/grok/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/grok/grok.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/grok_pattern_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/hasher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9641 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/json_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/log_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/multiprocessing_log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/pipeline_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12543 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/pre_detector_rule_matching_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/processor_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/prometheus_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/rule_dry_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/schema_and_rule_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/time_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.056394 logprep-6.1.0/logprep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-04-24 10:09:11.000000 logprep-6.1.0/logprep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15686 2023-04-24 10:09:11.000000 logprep-6.1.0/logprep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 10:09:11.000000 logprep-6.1.0/logprep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-24 10:09:11.000000 logprep-6.1.0/logprep.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-24 10:09:11.000000 logprep-6.1.0/logprep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-24 10:09:11.000000 logprep-6.1.0/logprep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-24 10:09:06.000000 logprep-6.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-24 10:09:11.092395 logprep-6.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-24 10:09:06.000000 logprep-6.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.072394 logprep-6.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.076394 logprep-6.1.0/tests/acceptance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/acceptance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/acceptance/test_amides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/acceptance/test_config_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/acceptance/test_file_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/acceptance/test_full_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/acceptance/test_http_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/acceptance/test_multiple_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19060 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/acceptance/test_pre_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/acceptance/test_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/acceptance/test_selective_extractor_full_pipeline_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/acceptance/test_wineventlog_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/acceptance/test_wineventlog_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/acceptance/test_wineventlog_pseudonymization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10368 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/acceptance/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.076394 logprep-6.1.0/tests/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/ci/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.076394 logprep-6.1.0/tests/ci/runner-image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/ci/runner-image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.076394 logprep-6.1.0/tests/ci/runner-image/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/ci/runner-image/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/ci/runner-image/scripts/compare_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.076394 logprep-6.1.0/tests/testdata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/testdata/ConfigurationForTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/testdata/FilledTempFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/testdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/testdata/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/testdata/ruledata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.076394 logprep-6.1.0/tests/testdata/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/testdata/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.076394 logprep-6.1.0/tests/testdata/unit/clusterer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/testdata/unit/clusterer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12733 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/testdata/unit/clusterer/test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.076394 logprep-6.1.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.076394 logprep-6.1.0/tests/unit/component/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/component/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.080394 logprep-6.1.0/tests/unit/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21571 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/connector/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/connector/test_confluent_kafka_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/connector/test_confluent_kafka_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/connector/test_confluent_kafka_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/connector/test_console_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/connector/test_dummy_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/connector/test_dummy_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/connector/test_elasticsearch_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9926 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/connector/test_file_input_default_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/connector/test_file_input_not_tailing_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/connector/test_file_input_start_at_end_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/connector/test_http_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/connector/test_json_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/connector/test_jsonl_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/connector/test_jsonl_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9239 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/connector/test_opensearch_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10222 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/connector/test_s3_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.080394 logprep-6.1.0/tests/unit/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.080394 logprep-6.1.0/tests/unit/exceptions/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/exceptions/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/exceptions/processor/test_processing_warning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.080394 logprep-6.1.0/tests/unit/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19683 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/filter/test_filter_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20548 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/filter/test_lucene_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.080394 logprep-6.1.0/tests/unit/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.080394 logprep-6.1.0/tests/unit/framework/rule_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/framework/rule_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/framework/rule_tree/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27846 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/framework/rule_tree/test_rule_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19943 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/framework/rule_tree/test_rule_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39696 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/framework/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/framework/test_pipeline_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.080394 logprep-6.1.0/tests/unit/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/metrics/test_metric_exposer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22193 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/metrics/test_metric_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/metrics/test_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.080394 logprep-6.1.0/tests/unit/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.080394 logprep-6.1.0/tests/unit/processor/amides/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/amides/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/amides/test_amides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/amides/test_amides_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/amides/test_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/amides/test_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/amides/test_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.080394 logprep-6.1.0/tests/unit/processor/calculator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/calculator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/calculator/test_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/calculator/test_calculator_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.084395 logprep-6.1.0/tests/unit/processor/clusterer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/clusterer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/clusterer/test_clusterer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/clusterer/test_clusterer_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/clusterer/test_clusterer_signature_phase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.084395 logprep-6.1.0/tests/unit/processor/concatenator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/concatenator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/concatenator/test_concatenator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11216 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/concatenator/test_concatenator_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.084395 logprep-6.1.0/tests/unit/processor/datetime_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/datetime_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8165 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/datetime_extractor/test_datetime_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/datetime_extractor/test_datetime_extractor_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.084395 logprep-6.1.0/tests/unit/processor/deleter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/deleter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/deleter/test_deleter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/deleter/test_deleter_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.084395 logprep-6.1.0/tests/unit/processor/dissector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/dissector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19625 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/dissector/test_dissector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17681 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/dissector/test_dissector_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.084395 logprep-6.1.0/tests/unit/processor/domain_label_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/domain_label_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13265 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.084395 logprep-6.1.0/tests/unit/processor/domain_resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/domain_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11812 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/domain_resolver/test_domain_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/domain_resolver/test_domain_resolver_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.084395 logprep-6.1.0/tests/unit/processor/dropper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/dropper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/dropper/test_dropper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/dropper/test_dropper_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.084395 logprep-6.1.0/tests/unit/processor/field_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/field_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13374 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/field_manager/test_field_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/field_manager/test_field_manager_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.084395 logprep-6.1.0/tests/unit/processor/generic_adder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/generic_adder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29997 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/generic_adder/test_generic_adder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/generic_adder/test_generic_adder_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.084395 logprep-6.1.0/tests/unit/processor/generic_resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/generic_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14079 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/generic_resolver/test_generic_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/generic_resolver/test_generic_resolver_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.084395 logprep-6.1.0/tests/unit/processor/geoip_enricher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/geoip_enricher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14996 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/geoip_enricher/test_geoip_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/geoip_enricher/test_geoip_enricher_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.088394 logprep-6.1.0/tests/unit/processor/grokker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/grokker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/grokker/test_grok.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12078 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/grokker/test_grokker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10893 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/grokker/test_grokker_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.088394 logprep-6.1.0/tests/unit/processor/hyperscan_resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/hyperscan_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23145 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.088394 logprep-6.1.0/tests/unit/processor/ip_informer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/ip_informer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/ip_informer/test_ip_informer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/ip_informer/test_ip_informer_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.088394 logprep-6.1.0/tests/unit/processor/labeler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/labeler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/labeler/test_labeler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/labeler/test_labeler_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12544 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/labeler/test_labeling_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.088394 logprep-6.1.0/tests/unit/processor/list_comparison/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/list_comparison/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11202 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/list_comparison/test_list_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/list_comparison/test_list_comparison_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.088394 logprep-6.1.0/tests/unit/processor/normalizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/normalizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38308 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/normalizer/test_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/normalizer/test_normalizer_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.088394 logprep-6.1.0/tests/unit/processor/pre_detector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/pre_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/pre_detector/test_ip_alerter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/pre_detector/test_pre_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/pre_detector/test_pre_detector_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.088394 logprep-6.1.0/tests/unit/processor/pseudonymizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/pseudonymizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/pseudonymizer/test_encrypter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29770 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/pseudonymizer/test_pseudonymizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/pseudonymizer/test_pseudonymizer_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.088394 logprep-6.1.0/tests/unit/processor/requester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/requester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12431 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/requester/test_requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/requester/test_requester_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.088394 logprep-6.1.0/tests/unit/processor/selective_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/selective_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/selective_extractor/test_selective_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/selective_extractor/test_selective_extractor_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.088394 logprep-6.1.0/tests/unit/processor/string_splitter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/string_splitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/string_splitter/test_string_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/string_splitter/test_string_splitter_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.088394 logprep-6.1.0/tests/unit/processor/template_replacer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/template_replacer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/template_replacer/test_template_replacer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/test_processor_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/test_processor_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.092395 logprep-6.1.0/tests/unit/processor/timestamp_differ/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/timestamp_differ/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17368 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/timestamp_differ/test_timestamp_differ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/timestamp_differ/test_timestamp_differ_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/test_run_logprep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18858 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/test_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.092395 logprep-6.1.0/tests/unit/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/util/test_auto_rule_corpus_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/util/test_auto_rule_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/util/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39375 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/util/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16243 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/util/test_getter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/util/test_grok_pattern_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/util/test_hasher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/util/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/util/test_helper_add_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/util/test_log_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/util/test_processor_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/util/test_prometheus_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/util/test_rule_dry_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/util/test_schema_and_rule_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/util/test_time_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16746 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/util/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/util/tests_json_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.092395 logprep-6.1.0/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/util/testhelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81000 2023-04-24 10:09:06.000000 logprep-6.1.0/versioneer.py
```

### Comparing `logprep-6.0.0/LICENSE` & `logprep-6.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/PKG-INFO` & `logprep-6.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logprep
-Version: 6.0.0
+Version: 6.1.0
 Summary: Logprep allows to collect, process and forward log messages from various data sources.
 Home-page: https://github.com/fkie-cad/Logprep
 Author: Logprep Team
 License: LGPL-2.1 license
 Project-URL: Homepage, https://github.com/fkie-cad/Logprep
 Project-URL: Documentation, https://logprep.readthedocs.io/en/latest/
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: logprep Version: 6.0.0 Summary: Logprep allows to
+Metadata-Version: 2.1 Name: logprep Version: 6.1.0 Summary: Logprep allows to
 collect, process and forward log messages from various data sources. Home-page:
 https://github.com/fkie-cad/Logprep Author: Logprep Team License: LGPL-2.1
 license Project-URL: Homepage, https://github.com/fkie-cad/Logprep Project-URL:
 Documentation, https://logprep.readthedocs.io/en/latest/ Platform: UNKNOWN
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

### Comparing `logprep-6.0.0/README.md` & `logprep-6.1.0/README.md`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/abc/connector.py` & `logprep-6.1.0/logprep/abc/connector.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/abc/getter.py` & `logprep-6.1.0/logprep/abc/getter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/abc/input.py` & `logprep-6.1.0/logprep/abc/input.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,52 +1,67 @@
 """This module provides the abstract base class for all input endpoints.
 New input endpoint types are created by implementing it.
 """
 
 import base64
 import hashlib
-import json
 import zlib
 from abc import abstractmethod
 from functools import partial
 from hmac import HMAC
-from typing import Tuple, Optional
+from typing import Optional, Tuple
 
 import arrow
 from attrs import define, field, validators
 
 from logprep.abc.connector import Connector
 from logprep.util.helper import add_field_to, get_dotted_field_value
 from logprep.util.time_measurement import TimeMeasurement
 from logprep.util.validators import dict_structure_validator
 
 
 class InputError(BaseException):
     """Base class for Input related exceptions."""
 
+    def __init__(self, input_connector: "Input", message: str) -> None:
+        super().__init__(f"{self.__class__.__name__} in {input_connector.describe()}: {message}")
+
 
 class CriticalInputError(InputError):
     """A significant error occurred - log and don't process the event."""
 
-    def __init__(self, message, raw_input):
+    def __init__(self, input_connector: "Input", message, raw_input):
         self.raw_input = raw_input
-        super().__init__(message)
+        input_connector.metrics.number_of_errors += 1
+        super().__init__(input_connector, f"{message} -> {raw_input}")
 
 
 class FatalInputError(InputError):
     """Must not be catched."""
 
+    def __init__(self, input_connector: "Input", message: str) -> None:
+        input_connector.metrics.number_of_errors += 1
+        super().__init__(input_connector, message)
+
 
 class WarningInputError(InputError):
     """May be catched but must be displayed to the user/logged."""
 
+    def __init__(self, input_connector: "Input", message: str) -> None:
+        input_connector.metrics.number_of_warnings += 1
+        super().__init__(input_connector, message)
+
 
 class SourceDisconnectedError(WarningInputError):
     """Lost (or failed to establish) contact with the source."""
 
+    def __init__(self, input_connector: "Input", message: str) -> None:
+        input_connector.metrics.number_of_errors += 1
+        super().__init__(input_connector, message)
+
 
 class InfoInputError(InputError):
     """Informational exceptions, e.g. to inform that a timeout occurred"""
 
 
 @define(kw_only=True)
 class HmacConfig:
@@ -246,15 +261,15 @@
             After timeout (usually a fraction of seconds) if no input data was available by then.
         """
         event, raw_event = self._get_event(timeout)
         non_critical_error_msg = None
         if event is None:
             return None, None
         if event is not None and not isinstance(event, dict):
-            raise CriticalInputError("not a dict", event)
+            raise CriticalInputError(self, "not a dict", event)
         if self._add_hmac:
             event, non_critical_error_msg = self._add_hmac_to(event, raw_event)
         if self._add_version_info:
             self._add_version_information_to_event(event)
         if self._add_log_arrival_time_information:
             self._add_arrival_time_information_to_event(event)
         if self._add_log_arrival_timedelta_information:
@@ -315,15 +330,15 @@
             field, which was used to calculate the hmac.
         """
         hmac_options = self._config.preprocessing.get("hmac", {})
         hmac_target_field_name = hmac_options.get("target")
         non_critical_error_msg = None
 
         if raw_event is None:
-            raw_event = json.dumps(event_dict).encode("utf-8")
+            raw_event = self._encoder.encode(event_dict)
 
         if hmac_target_field_name == "<RAW_MSG>":
             received_orig_message = raw_event
         else:
             received_orig_message = get_dotted_field_value(event_dict, hmac_target_field_name)
 
         if received_orig_message is None:
```

### Comparing `logprep-6.0.0/logprep/abc/output.py` & `logprep-6.1.0/logprep/abc/output.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,35 +5,49 @@
 from abc import abstractmethod
 from logging import Logger
 from typing import Optional
 
 from attrs import define, field, validators
 
 from logprep.abc.connector import Connector
+from logprep.abc.input import Input
 
 
 class OutputError(BaseException):
     """Base class for Output related exceptions."""
 
+    def __init__(self, output: "Output", message: str) -> None:
+        super().__init__(f"{self.__class__.__name__} in {output.describe()}: {message}")
+
 
 class CriticalOutputError(OutputError):
     """A significant error occurred - log and don't process the event."""
 
-    def __init__(self, message, raw_input):
-        self.raw_input = raw_input
-        super().__init__(message)
+    def __init__(self, output, message, raw_input):
+        if raw_input:
+            output.store_failed(str(self), raw_input, {})
+        output.metrics.number_of_errors += 1
+        super().__init__(output, f"{message} for event: {raw_input}")
 
 
 class FatalOutputError(OutputError):
     """Must not be catched."""
 
+    def __init__(self, output, message) -> None:
+        output.metrics.number_of_errors += 1
+        super().__init__(output, message)
+
 
 class WarningOutputError(OutputError):
     """May be catched but must be displayed to the user/logged."""
 
+    def __init__(self, output, message) -> None:
+        output.metrics.number_of_warnings += 1
+        super().__init__(output, message)
+
 
 class Output(Connector):
     """Connect to a output destination."""
 
     @define(kw_only=True)
     class Config(Connector.Config):
         """output config parameters"""
@@ -41,15 +55,15 @@
         default: bool = field(validator=validators.instance_of(bool), default=True)
         """ (Optional) if :code:`false` the event are not delivered to this output.
         But this output can be called as output for extra_data.
         """
 
     __slots__ = {"input_connector"}
 
-    input_connector: Connector
+    input_connector: Optional[Input]
 
     def __init__(self, name: str, configuration: "Connector.Config", logger: Logger):
         super().__init__(name, configuration, logger)
         self.input_connector = None
 
     @property
     def default(self):
```

### Comparing `logprep-6.0.0/logprep/abc/processor.py` & `logprep-6.1.0/logprep/abc/processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 """Abstract module for processors"""
 import copy
 from abc import abstractmethod
 from logging import DEBUG, Logger
 from multiprocessing import current_process
 from pathlib import Path
-from typing import List, Optional, TYPE_CHECKING
+from typing import TYPE_CHECKING, List, Optional
 
 from attr import define, field, validators
 
 from logprep.abc.component import Component
 from logprep.framework.rule_tree.rule_tree import RuleTree
 from logprep.metrics.metric import Metric, calculate_new_average
-from logprep.processor.base.exceptions import DuplicationError, ProcessingWarning
+from logprep.processor.base.exceptions import (
+    FieldExistsWarning,
+    ProcessingCriticalError,
+    ProcessingWarning,
+)
 from logprep.processor.processor_strategy import SpecificGenericProcessStrategy
 from logprep.util import getter
 from logprep.util.helper import (
+    add_and_overwrite,
     add_field_to,
-    pop_dotted_field_value,
     get_dotted_field_value,
-    add_and_overwrite,
+    pop_dotted_field_value,
 )
 from logprep.util.json_handling import list_json_files_in_directory
 from logprep.util.time_measurement import TimeMeasurement
 
 if TYPE_CHECKING:
     from logprep.processor.base.rule import Rule  # pragma: no cover
 
@@ -55,14 +59,19 @@
         For valid URI formats see :ref:`getters`.
         """
         tree_config: Optional[str] = field(
             default=None, validator=[validators.optional(validators.instance_of(str))]
         )
         """Path to a JSON file with a valid rule tree configuration.
         For string format see :ref:`getters`"""
+        apply_multiple_times: Optional[bool] = field(
+            default=False, validator=[validators.optional(validators.instance_of(bool))]
+        )
+        """Set if the processor should be applied multiple times. This enables further processing
+        of an output with the same processor."""
 
     @define(kw_only=True)
     class ProcessorMetrics(Metric):
         """Tracks statistics about this processor"""
 
         _prefix: str = "logprep_processor_"
 
@@ -103,19 +112,19 @@
     rule_class: "Rule"
     has_custom_tests: bool
     metrics: ProcessorMetrics
     metric_labels: dict
     _event: dict
     _specific_tree: RuleTree
     _generic_tree: RuleTree
-
-    _strategy = SpecificGenericProcessStrategy()
+    _strategy = None
 
     def __init__(self, name: str, configuration: "Processor.Config", logger: Logger):
         super().__init__(name, configuration, logger)
+        self._strategy = SpecificGenericProcessStrategy(self._config.apply_multiple_times)
         self.metric_labels, specific_tree_labels, generic_tree_labels = self._create_metric_labels()
         self._specific_tree = RuleTree(
             config_path=self._config.tree_config, metric_labels=specific_tree_labels
         )
         self._generic_tree = RuleTree(
             config_path=self._config.tree_config, metric_labels=generic_tree_labels
         )
@@ -192,14 +201,16 @@
         )
 
     def _apply_rules_wrapper(self, event, rule):
         try:
             self._apply_rules(event, rule)
         except ProcessingWarning as error:
             self._handle_warning_error(event, rule, error)
+        except BaseException as error:
+            raise ProcessingCriticalError(self, str(error), event) from error
         if not hasattr(rule, "delete_source_fields"):
             return
         if rule.delete_source_fields:
             for dotted_field in rule.source_fields:
                 pop_dotted_field_value(event, dotted_field)
 
     @abstractmethod
@@ -262,36 +273,38 @@
         for field_ in fields:
             if field_ in dict_ and isinstance(dict_, dict):
                 dict_ = dict_[field_]
             else:
                 return False
         return True
 
-    @staticmethod
-    def _handle_warning_error(event, rule, error):
+    def _handle_warning_error(self, event, rule, error):
         tags = get_dotted_field_value(event, "tags")
         if tags is None:
             add_and_overwrite(event, "tags", sorted(list({*rule.failure_tags})))
         else:
             add_and_overwrite(event, "tags", sorted(list({*tags, *rule.failure_tags})))
         if isinstance(error, ProcessingWarning):
-            raise error
-        raise ProcessingWarning(str(error)) from error
+            self._logger.warning(str(error))
+        else:
+            self._logger.warning(str(ProcessingWarning(self, str(error), rule, event)))
 
-    def _check_for_missing_values(self, event, rule, source_field_dict):
+    def _has_missing_values(self, event, rule, source_field_dict):
         missing_fields = list(
             dict(filter(lambda x: x[1] in [None, ""], source_field_dict.items())).keys()
         )
         if missing_fields:
             error = BaseException(f"{self.name}: no value for fields: {missing_fields}")
             self._handle_warning_error(event, rule, error)
+            return True
+        return False
 
     def _write_target_field(self, event: dict, rule: "Rule", result: any) -> None:
         add_successful = add_field_to(
             event,
             output_field=rule.target_field,
             content=result,
             extends_lists=rule.extend_target_list,
             overwrite_output_field=rule.overwrite_target,
         )
         if not add_successful:
-            raise DuplicationError(self.name, [rule.target_field])
+            raise FieldExistsWarning(self, rule, event, [rule.target_field])
```

### Comparing `logprep-6.0.0/logprep/configuration.py` & `logprep-6.1.0/logprep/configuration.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/connector/confluent_kafka/input.py` & `logprep-6.1.0/logprep/connector/confluent_kafka/input.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,24 +22,25 @@
         bootstrapservers: [127.0.0.1:9092]
         topic: consumer
         group: cgroup
         auto_commit: true
         session_timeout: 6000
         offset_reset_policy: smallest
 """
-import json
 from functools import cached_property, partial
 from logging import Logger
 from socket import getfqdn
-from typing import Any, List, Tuple, Union
+from typing import Any, List, Optional, Tuple, Union
 
+import msgspec
 from attrs import define, field, validators
-from confluent_kafka import Consumer
+from confluent_kafka import Consumer, KafkaException
 
 from logprep.abc.input import CriticalInputError, Input
+from logprep.abc.output import FatalOutputError
 from logprep.util.validators import dict_with_keys_validator
 
 
 class ConfluentKafkaInput(Input):
     """A kafka input connector."""
 
     @define(kw_only=True, slots=False)
@@ -114,14 +115,29 @@
         consumer starts by reading the newest log messages of a partition if a valid offset is
         missing. Thus, old log messages from that partition will not be processed. This setting can
         therefore lead to a loss of log messages. A value of earliest/smallest causes the Kafka
         consumer to read all log messages from a partition, which can lead to a duplication of log
         messages. Currently, the deprecated value smallest is used, which should be later changed
         to earliest. The default value of librdkafka is largest."""
 
+        kafka_config: Optional[dict] = field(
+            validator=[
+                validators.instance_of(dict),
+                validators.deep_mapping(
+                    key_validator=validators.instance_of(str),
+                    value_validator=validators.instance_of((str, dict)),
+                ),
+            ],
+            factory=dict,
+        )
+        """ (Optional) Additional kafka configuration for the kafka client. 
+        This is for advanced usage only. For possible configuration options see: 
+        <https://github.com/edenhill/librdkafka/blob/master/CONFIGURATION.md>
+        """
+
     current_offset: int
 
     _record: Any
 
     _last_valid_records: dict
 
     __slots__ = [
@@ -180,15 +196,15 @@
         if self._record is None:
             return None
         self._last_valid_records[self._record.partition()] = self._record
         self.current_offset = self._record.offset()
         record_error = self._record.error()
         if record_error:
             raise CriticalInputError(
-                f"A confluent-kafka record contains an error code: ({record_error})", None
+                self, "A confluent-kafka record contains an error code", record_error
             )
         return self._record.value()
 
     def _get_event(self, timeout: float) -> Union[Tuple[None, None], Tuple[dict, dict]]:
         """Parse the raw document from Kafka into a json.
 
         Parameters
@@ -208,21 +224,23 @@
         CriticalInputError
             Raises if an input is invalid or if it causes an error.
         """
         raw_event = self._get_raw_event(timeout)
         if raw_event is None:
             return None, None
         try:
-            event_dict = json.loads(raw_event.decode("utf-8"))
-        except ValueError as error:
+            event_dict = self._decoder.decode(raw_event)
+        except msgspec.DecodeError as error:
             raise CriticalInputError(
-                "Input record value is not a valid json string", raw_event
+                self, "Input record value is not a valid json string", raw_event
             ) from error
         if not isinstance(event_dict, dict):
-            raise CriticalInputError("Input record value could not be parsed as dict", event_dict)
+            raise CriticalInputError(
+                self, "Input record value could not be parsed as dict", event_dict
+            )
         return event_dict, raw_event
 
     @cached_property
     def _confluent_settings(self) -> dict:
         """Generate confluence settings, mapped from the given kafka logprep configuration.
 
         Returns
@@ -245,24 +263,31 @@
                     "security.protocol": "SSL",
                     "ssl.ca.location": self._config.ssl["cafile"],
                     "ssl.certificate.location": self._config.ssl["certfile"],
                     "ssl.key.location": self._config.ssl["keyfile"],
                     "ssl.key.password": self._config.ssl["password"],
                 }
             )
-        return configuration
+        return self._config.kafka_config | configuration
 
     def batch_finished_callback(self):
         """Store offsets for each kafka partition.
         Should be called by output connectors if they are finished processing a batch of records.
         This is only used if automatic offest storing is disabled in the kafka input.
         The last valid record for each partition is be used by this method to update all offsets.
         """
         if not self._config.enable_auto_offset_store:
             if self._last_valid_records:
                 for last_valid_records in self._last_valid_records.values():
                     self._consumer.store_offsets(message=last_valid_records)
 
+    def setup(self):
+        super().setup()
+        try:
+            _ = self._consumer
+        except (KafkaException, ValueError) as error:
+            raise FatalOutputError(self, str(error)) from error
+
     def shut_down(self):
         """Close consumer, which also commits kafka offsets."""
         if self._consumer is not None:
             self._consumer.close()
```

### Comparing `logprep-6.0.0/logprep/connector/confluent_kafka/output.py` & `logprep-6.1.0/logprep/connector/confluent_kafka/output.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,18 +28,19 @@
 
 import json
 from datetime import datetime
 from functools import cached_property, partial
 from socket import getfqdn
 from typing import List, Optional
 
+import msgspec
 from attrs import define, field, validators
-from confluent_kafka import Producer
+from confluent_kafka import KafkaException, Producer
 
-from logprep.abc.output import CriticalOutputError, Output
+from logprep.abc.output import CriticalOutputError, FatalOutputError, Output
 from logprep.util.validators import dict_with_keys_validator
 
 
 class ConfluentKafkaOutput(Output):
     """A kafka connector that serves as output connector."""
 
     @define(kw_only=True, slots=False)
@@ -75,14 +76,28 @@
                 partial(
                     dict_with_keys_validator,
                     expected_keys=["cafile", "certfile", "keyfile", "password"],
                 ),
             ],
             default={"cafile": None, "certfile": None, "keyfile": None, "password": None},
         )
+        kafka_config: Optional[dict] = field(
+            validator=[
+                validators.instance_of(dict),
+                validators.deep_mapping(
+                    key_validator=validators.instance_of(str),
+                    value_validator=validators.instance_of((str, dict)),
+                ),
+            ],
+            factory=dict,
+        )
+        """ (Optional) Additional kafka configuration for the kafka client. 
+        This is for advanced usage only. For possible configuration options see: 
+        <https://github.com/edenhill/librdkafka/blob/master/CONFIGURATION.md>
+        """
 
     @cached_property
     def _client_id(self):
         return getfqdn()
 
     @cached_property
     def _producer(self):
@@ -111,15 +126,15 @@
                     "security.protocol": "SSL",
                     "ssl.ca.location": self._config.ssl["cafile"],
                     "ssl.certificate.location": self._config.ssl["certfile"],
                     "ssl.key.location": self._config.ssl["keyfile"],
                     "ssl.key.password": self._config.ssl["password"],
                 }
             )
-        return configuration
+        return self._config.kafka_config | configuration
 
     def describe(self) -> str:
         """Get name of Kafka endpoint with the bootstrap server.
 
         Returns
         -------
         kafka : ConfluentKafka
@@ -159,24 +174,22 @@
         Raises
         ------
         CriticalOutputError
             Raises if any error except a BufferError occurs while writing into Kafka.
 
         """
         try:
-            self._producer.produce(
-                target, value=json.dumps(document, separators=(",", ":")).encode("utf-8")
-            )
+            self._producer.produce(target, value=self._encoder.encode(document))
             self._producer.poll(self._config.send_timeout)
         except BufferError:
             # block program until buffer is empty
             self._producer.flush(timeout=self._config.flush_timeout)
         except BaseException as error:
             raise CriticalOutputError(
-                f"Error storing output document: ({error})", document
+                self, f"Error storing output document -> {error}", document
             ) from error
 
     def store_failed(
         self, error_message: str, document_received: dict, document_processed: dict
     ) -> None:
         """Write errors into error topic for documents that failed processing.
 
@@ -202,11 +215,18 @@
                 value=json.dumps(value, separators=(",", ":")).encode("utf-8"),
             )
             self._producer.poll(self._config.send_timeout)
         except BufferError:
             # block program until buffer is empty
             self._producer.flush(timeout=self._config.flush_timeout)
 
+    def setup(self):
+        super().setup()
+        try:
+            _ = self._producer
+        except (KafkaException, ValueError) as error:
+            raise FatalOutputError(self, str(error)) from error
+
     def shut_down(self) -> None:
         """ensures that all messages are flushed"""
         if self._producer is not None:
             self._producer.flush(self._config.flush_timeout)
```

### Comparing `logprep-6.0.0/logprep/connector/console/output.py` & `logprep-6.1.0/logprep/connector/console/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/connector/dummy/input.py` & `logprep-6.1.0/logprep/connector/dummy/input.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 
     input:
       mydummyinput:
         type: dummy_input
         documents: [{"document":"one"}, "Exception", {"document":"two"}]
 """
 from typing import List, Union
+
 from attrs import define
+
 from logprep.abc.input import Input, SourceDisconnectedError
 
 
 class DummyInput(Input):
     """DummyInput Connector"""
 
     @define(kw_only=True)
@@ -36,14 +38,14 @@
     @property
     def _documents(self):
         return self._config.documents
 
     def _get_event(self, timeout: float) -> tuple:
         """Retriev next document from configuration and raise error if found"""
         if not self._documents:
-            raise SourceDisconnectedError
+            raise SourceDisconnectedError(self, "no documents left")
 
         document = self._documents.pop(0)
 
         if (document.__class__ == type) and issubclass(document, BaseException):
             raise document
         return document, None
```

### Comparing `logprep-6.0.0/logprep/connector/dummy/output.py` & `logprep-6.1.0/logprep/connector/dummy/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/connector/elasticsearch/output.py` & `logprep-6.1.0/logprep/connector/elasticsearch/output.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,29 +23,31 @@
         default_index: default_index
         error_index: error_index
         message_backlog_size: 10000
         timeout: 10000
         max_retries:
         user:
         secret:
-        cert: /path/to/cert.crt
+        ca_cert: /path/to/cert.crt
 """
 
 import json
 import re
 import ssl
 from functools import cached_property
 from logging import Logger
 from typing import List, Optional
 
 import arrow
-import elasticsearch
+import elasticsearch as search
 from attr import define, field
 from attrs import validators
-from elasticsearch import helpers, ElasticsearchException
+from elasticsearch import ElasticsearchException, helpers
+from opensearchpy import OpenSearchException
+from urllib3.exceptions import TimeoutError
 
 from logprep.abc.output import FatalOutputError, Output
 
 
 class ElasticsearchOutput(Output):
     """An Elasticsearch output connector."""
 
@@ -66,42 +68,36 @@
         default_index: str = field(validator=validators.instance_of(str))
         """Default index to write to if no index was set in the document or the document could not
         be indexed. The document will be transformed into a string to prevent rejections by the
         default index."""
         error_index: str = field(validator=validators.instance_of(str))
         """Index to write documents to that could not be processed."""
         message_backlog_size: int = field(validator=validators.instance_of(int))
-        """Amount of documents to store before sending them to Elasticsearch."""
+        """Amount of documents to store before sending them."""
         timeout: int = field(validator=validators.instance_of(int), default=500)
-        """Timeout for Elasticsearch connection (default is 500ms)"""
+        """(Optional) Timeout for the connection (default is 500ms)."""
         max_retries: int = field(validator=validators.instance_of(int), default=0)
-        """Maximum number of retries for documents rejected with code 429 (default is 0).
+        """(Optional) Maximum number of retries for documents rejected with code 429 (default is 0).
         Increases backoff time by 2 seconds per try, but never exceeds 600 seconds."""
         user: Optional[str] = field(validator=validators.instance_of(str), default="")
-        """The user used for authentication (optional)."""
+        """(Optional) User used for authentication."""
         secret: Optional[str] = field(validator=validators.instance_of(str), default="")
-        """The secret used for authentication (optional)."""
+        """(Optional) Secret used for authentication."""
         ca_cert: Optional[str] = field(validator=validators.instance_of(str), default="")
-        """The path to a SSL ca certificate to verify the ssl context (optional)"""
+        """(Optional) Path to a SSL ca certificate to verify the ssl context."""
+        flush_timeout: Optional[int] = field(validator=validators.instance_of(int), default=60)
+        """(Optional) Timout after :code:`message_backlog` is flushed if :code:`message_backlog_size` is not reached."""
 
-    __slots__ = ["_message_backlog", "_processed_cnt", "_index_cache"]
+    __slots__ = ["_message_backlog"]
 
     _message_backlog: List
 
-    _processed_cnt: int
-
-    _index_cache: dict
-
     def __init__(self, name: str, configuration: "ElasticsearchOutput.Config", logger: Logger):
         super().__init__(name, configuration, logger)
-        self._message_backlog = [
-            {"_index": self._config.default_index}
-        ] * self._config.message_backlog_size
-        self._processed_cnt = 0
-        self._index_cache = {}
+        self._message_backlog = []
 
     @cached_property
     def ssl_context(self) -> ssl.SSLContext:
         """Returns the ssl context
 
         Returns
         -------
@@ -137,23 +133,23 @@
         return (
             (self._config.user, self._config.secret)
             if self._config.user and self._config.secret
             else None
         )
 
     @cached_property
-    def _search_context(self) -> elasticsearch.Elasticsearch:
+    def _search_context(self) -> search.Elasticsearch:
         """Returns a elasticsearch context
 
         Returns
         -------
         elasticsearch.Elasticsearch
             the eleasticsearch context
         """
-        return elasticsearch.Elasticsearch(
+        return search.Elasticsearch(
             self._config.hosts,
             scheme=self.schema,
             http_auth=self.http_auth,
             ssl_context=self.ssl_context,
             timeout=self._config.timeout,
         )
 
@@ -187,35 +183,29 @@
            Document to store.
 
         Returns
         -------
         Returns True to inform the pipeline to call the batch_finished_callback method in the
         configured input
         """
-        self._message_backlog[self._processed_cnt] = document
-        currently_processed_cnt = self._processed_cnt + 1
-        if currently_processed_cnt == self._config.message_backlog_size:
-            try:
-                helpers.bulk(
-                    self._search_context,
-                    self._message_backlog,
-                    max_retries=self._config.max_retries,
-                    chunk_size=self._config.message_backlog_size,
-                )
-            except elasticsearch.SerializationError as error:
-                self._handle_serialization_error(error)
-            except elasticsearch.ConnectionError as error:
-                self._handle_connection_error(error)
-            except helpers.BulkIndexError as error:
-                self._handle_bulk_index_error(error)
-            self._processed_cnt = 0
-            if self.input_connector:
-                self.input_connector.batch_finished_callback()
-        else:
-            self._processed_cnt = currently_processed_cnt
+        self._message_backlog.append(document)
+        if len(self._message_backlog) >= self._config.message_backlog_size:
+            self._write_backlog()
+
+    def _write_backlog(self):
+        if not self._message_backlog:
+            return
+
+        self._bulk(
+            self._search_context,
+            self._message_backlog,
+            max_retries=self._config.max_retries,
+            chunk_size=len(self._message_backlog),
+        )
+        self._message_backlog.clear()
 
     def _handle_bulk_index_error(self, error: helpers.BulkIndexError):
         """Handle bulk indexing error for elasticsearch bulk indexing.
 
         Documents that could not be sent to elastiscsearch due to index errors are collected and
         sent into an error index that should always accept all documents.
         This can lead to a rebuild of the pipeline if this causes another exception.
@@ -232,17 +222,29 @@
             data = error_info.get("data") if "data" in error_info else None
             error_type = error_info.get("error").get("type")
             error_reason = error_info.get("error").get("reason")
             reason = f"{error_type}: {error_reason}"
             error_document = self._build_failed_index_document(data, reason)
             self._add_dates(error_document)
             error_documents.append(error_document)
-        helpers.bulk(self._search_context, error_documents)
+        self._bulk(self._search_context, error_documents)
+
+    def _bulk(self, *args, **kwargs):
+        try:
+            helpers.bulk(*args, **kwargs)
+        except search.SerializationError as error:
+            self._handle_serialization_error(error)
+        except search.ConnectionError as error:
+            self._handle_connection_error(error)
+        except helpers.BulkIndexError as error:
+            self._handle_bulk_index_error(error)
+        if self.input_connector:
+            self.input_connector.batch_finished_callback()
 
-    def _handle_connection_error(self, error: elasticsearch.ConnectionError):
+    def _handle_connection_error(self, error: search.ConnectionError):
         """Handle connection error for elasticsearch bulk indexing.
 
         No documents will be sent if there is no connection to begin with.
         Therefore, it won't result in duplicates once the the data is resent.
         If the connection is lost during indexing, duplicate documents could be sent.
 
         Parameters
@@ -252,17 +254,17 @@
 
         Raises
         ------
         FatalOutputError
             This causes a pipeline rebuild and gives an appropriate error log message.
 
         """
-        raise FatalOutputError(error.error)
+        raise FatalOutputError(self, error.error)
 
-    def _handle_serialization_error(self, error: elasticsearch.SerializationError):
+    def _handle_serialization_error(self, error: search.SerializationError):
         """Handle serialization error for elasticsearch bulk indexing.
 
         If at least one document in a chunk can't be serialized, no events will be sent.
         The chunk size is thus set to be the same size as the message backlog size.
         Therefore, it won't result in duplicates once the the data is resent.
 
         Parameters
@@ -272,15 +274,15 @@
 
         Raises
         ------
         FatalOutputError
             This causes a pipeline rebuild and gives an appropriate error log message.
 
         """
-        raise FatalOutputError(f"{error.args[1]} in document {error.args[0]}")
+        raise FatalOutputError(self, f"{error.args[1]} in document {error.args[0]}")
 
     def store(self, document: dict) -> bool:
         """Store a document in the index.
 
         Parameters
         ----------
         document : dict
@@ -359,11 +361,13 @@
             now = arrow.now()
             for date_format_match in date_format_matches:
                 formatted_date = now.format(date_format_match[2:-1])
                 document["_index"] = re.sub(date_format_match, formatted_date, document["_index"])
 
     def setup(self):
         super().setup()
+        flush_timeout = self._config.flush_timeout
+        self._schedule_task(task=self._write_backlog, seconds=flush_timeout)
         try:
             self._search_context.info()
-        except ElasticsearchException as error:
-            raise FatalOutputError(error) from error
+        except (ElasticsearchException, OpenSearchException, TimeoutError) as error:
+            raise FatalOutputError(self, error) from error
```

### Comparing `logprep-6.0.0/logprep/connector/file/input.py` & `logprep-6.1.0/logprep/connector/file/input.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,22 +16,23 @@
         type: file_input
         logfile_path: path/to/a/document
         start: begin
         interval: 1
         watch_file: True
 """
 import queue
-import zlib
 import threading
-from typing import Callable, TextIO
+import zlib
 from logging import Logger
+from typing import Callable, TextIO
+
 from attrs import define, field, validators
+
+from logprep.abc.input import FatalInputError, Input
 from logprep.util.validators import file_validator
-from logprep.abc.input import Input
-from logprep.abc.input import FatalInputError
 
 
 def threadsafe_wrapper(func: Callable):
     """Decorator making sure that the decorated function is thread safe"""
     lock = threading.Lock()
 
     def func_wrapper(*args, **kwargs):
@@ -45,17 +46,19 @@
 def runtime_file_exceptions(func: Callable):
     """Decorator to wrap and catch file related errors that can occur during runtime"""
 
     def func_wrapper(*args, **kwargs):
         try:
             func_wrapper = func(*args, **kwargs)
         except FileNotFoundError:
-            return FatalInputError("File that was used in config doesn't exist anymore.")
+            return FatalInputError(args[0], "File that was used in config doesn't exist anymore.")
         except PermissionError:
-            return FatalInputError("The Permissions changed of the File that was used in config.")
+            return FatalInputError(
+                args[0], "The Permissions changed of the File that was used in config."
+            )
         return func_wrapper
 
     return func_wrapper
 
 
 class RepeatedTimerThread(threading.Thread):
     """This class is a minimal Thread Wrapper that runs a given function for a given time interval.
@@ -320,15 +323,15 @@
     def setup(self):
         """Creates and starts the Thread that continously monitors the given logfile.
         Right now this input connector is only started in the first process.
         It needs the class attribute pipeline_index before running setup in Pipeline
         Initiation"""
         if not hasattr(self, "pipeline_index"):
             raise FatalInputError(
-                "Necessary instance attribute `pipeline_index` could not be found."
+                self, "Necessary instance attribute `pipeline_index` could not be found."
             )
         if self.pipeline_index == 1:
             initial_file_pointer: int = self._get_initial_file_offset(self._config.logfile_path)
             self._fileinfo_util.add_offset(self._config.logfile_path, initial_file_pointer)
             self.rthread = RepeatedTimerThread(
                 self._config.interval,
                 self._file_input_handler,
```

### Comparing `logprep-6.0.0/logprep/connector/http/input.py` & `logprep-6.1.0/logprep/connector/http/input.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,20 +19,20 @@
         endpoints:
             /firstendpoint: json
             /seccondendpoint: plaintext
             /thirdendpoint: jsonl
 """
 import contextlib
 import inspect
-import json
 import queue
 import threading
 from abc import ABC, abstractmethod
 from typing import Mapping, Tuple, Union
 
+import msgspec
 import uvicorn
 from attrs import define, field, validators
 from fastapi import FastAPI, Request
 from pydantic import BaseModel  # pylint: disable=no-name-in-module
 
 from logprep.abc.input import Input
 
@@ -68,22 +68,24 @@
         """json endpoint method"""
         self.messages.put(dict(event))
 
 
 class JSONLHttpEndpoint(HttpEndpoint):
     """:code:`jsonl` endpoint to get jsonl from request"""
 
+    _decoder = msgspec.json.Decoder()
+
     async def endpoint(self, request: Request):  # pylint: disable=arguments-differ
         """jsonl endpoint method"""
         data = await request.body()
         data = data.decode("utf8")
         for line in data.splitlines():
             line = line.strip()
             if line:
-                event = json.loads(line)
+                event = self._decoder.decode(line)
                 self.messages.put(event)
 
 
 class PlaintextHttpEndpoint(HttpEndpoint):
     """:code:`plaintext` endpoint to get the body from request and put it in :code:`message` field"""
 
     async def endpoint(self, request: Request):  # pylint: disable=arguments-differ
```

### Comparing `logprep-6.0.0/logprep/connector/json/input.py` & `logprep-6.1.0/logprep/connector/json/input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/connector/jsonl/input.py` & `logprep-6.1.0/logprep/connector/jsonl/input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/connector/jsonl/output.py` & `logprep-6.1.0/logprep/connector/jsonl/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/factory.py` & `logprep-6.1.0/logprep/factory.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/factory_error.py` & `logprep-6.1.0/logprep/factory_error.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/filter/expression/filter_expression.py` & `logprep-6.1.0/logprep/filter/expression/filter_expression.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,15 +80,28 @@
         if not isinstance(other, type(self)):
             return False
         if not self.__dict__ == other.__dict__:
             return False
         return True
 
     @staticmethod
-    def _as_dotted_string(key_list: List[str]) -> str:
+    def as_dotted_string(key_list: List[str]) -> str:
+        """Converts list of keys to dotted string.
+
+        Parameters
+        ----------
+        key_list : List[str]
+            List of keys.
+
+        Returns
+        -------
+        str
+            Returns dotted string.
+
+        """
         return ".".join([str(i) for i in key_list])
 
 
 class Always(FilterExpression):
     """Filter expression that can be set to match always or never."""
 
     def __init__(self, value: Any):
@@ -146,45 +159,45 @@
         return any((expression.matches(document) for expression in self.expressions))
 
 
 class KeyValueBasedFilterExpression(FilterExpression):
     """Base class of filter expressions that match a certain value on a given key."""
 
     def __init__(self, key: List[str], expected_value: Any):
-        self._key = key
+        self.key = key
         self._expected_value = expected_value
 
     def __repr__(self) -> str:
-        return f"{self._as_dotted_string(self._key)}:{str(self._expected_value)}"
+        return f"{self.as_dotted_string(self.key)}:{str(self._expected_value)}"
 
     def does_match(self, document):
         raise NotImplementedError
 
 
 class StringFilterExpression(KeyValueBasedFilterExpression):
     """Key value filter expression that matches for a string."""
 
     def does_match(self, document: dict) -> bool:
-        value = self._get_value(self._key, document)
+        value = self._get_value(self.key, document)
 
         if isinstance(value, list):
             return self._expected_value in value
         return str(value) == self._expected_value
 
     def __repr__(self) -> str:
-        return f'{self._as_dotted_string(self._key)}:"{str(self._expected_value)}"'
+        return f'{self.as_dotted_string(self.key)}:"{str(self._expected_value)}"'
 
 
 class WildcardStringFilterExpression(KeyValueBasedFilterExpression):
     """Key value filter expression that matches for a string with wildcard support."""
 
     flags = 0
 
-    wc = re.compile(r".*?((?:\\)*\*).*?")
-    wq = re.compile(r".*?((?:\\)*\?).*?")
+    wc = re.compile(r"((?:\\)*\*)")
+    wq = re.compile(r"((?:\\)*\?)")
 
     def __init__(self, key: List[str], expected_value: Any):
         super().__init__(key, expected_value)
         new_string = re.escape(str(self._expected_value))
 
         matches = self.wq.findall(new_string)
         new_string = self._replace_wildcard(new_string, matches, r"\?", ".?")
@@ -196,15 +209,15 @@
         self._matcher = re.compile(self.escaped_expected, flags=self.flags)
 
     @staticmethod
     def _normalize_regex(regex: str) -> str:
         return f"^{regex}$"
 
     def does_match(self, document: dict) -> bool:
-        value = self._get_value(self._key, document)
+        value = self._get_value(self.key, document)
 
         if isinstance(value, list):
             return any(filter(self._matcher.match, (str(val) for val in value)))
 
         match_result = self._matcher.match(str(value))
 
         return match_result is not None
@@ -219,114 +232,117 @@
                 matches[idx] = match[:-4] + symbol
             elif length > 2:
                 matches[idx] = match[:-4] + wildcard
         split = re.split(r"(?:\\)*" + symbol, expected)
         return "".join([x for x in chain.from_iterable(zip_longest(split, matches)) if x])
 
     def __repr__(self) -> str:
-        return f'{self._as_dotted_string(self._key)}:"{self._expected_value}"'
+        return f'{self.as_dotted_string(self.key)}:"{self._expected_value}"'
 
 
 class SigmaFilterExpression(WildcardStringFilterExpression):
     """Key value filter expression for strings with wildcard support that is case-insensitive."""
 
     flags = re.IGNORECASE
 
 
 class IntegerFilterExpression(KeyValueBasedFilterExpression):
     """Key value filter expression that matches for an integer."""
 
     def does_match(self, document: dict) -> bool:
-        value = self._get_value(self._key, document)
+        value = self._get_value(self.key, document)
 
         return value == self._expected_value
 
 
 class FloatFilterExpression(KeyValueBasedFilterExpression):
     """Key value filter expression that matches for a float."""
 
     def does_match(self, document: dict) -> bool:
-        value = self._get_value(self._key, document)
+        value = self._get_value(self.key, document)
 
         return value == self._expected_value
 
 
 class RangeBasedFilterExpression(FilterExpression):
     """Base class of filter expressions that match for a range of values."""
 
     def __init__(self, key: List[str], lower_bound: float, upper_bound: float):
-        self._key = key
+        self.key = key
         self._lower_bound = lower_bound
         self._upper_bound = upper_bound
 
     def __repr__(self) -> str:
-        return f"{self._as_dotted_string(self._key)}:[{self._lower_bound} TO {self._upper_bound}]"
+        return f"{self.as_dotted_string(self.key)}:[{self._lower_bound} TO {self._upper_bound}]"
 
     def does_match(self, document: dict):
         raise NotImplementedError
 
 
 class IntegerRangeFilterExpression(RangeBasedFilterExpression):
     """Range based filter expression that matches for integers."""
 
     def does_match(self, document: dict) -> bool:
-        value = self._get_value(self._key, document)
+        value = self._get_value(self.key, document)
 
         return self._lower_bound <= value <= self._upper_bound
 
 
 class FloatRangeFilterExpression(RangeBasedFilterExpression):
     """Range based filter expression that matches for floats."""
 
     def does_match(self, document: dict) -> bool:
-        value = self._get_value(self._key, document)
+        value = self._get_value(self.key, document)
 
         return self._lower_bound <= value <= self._upper_bound
 
 
 class RegExFilterExpression(FilterExpression):
     """Filter expression that matches a value using regex."""
 
+    match_escaping_pattern = re.compile(r".*?(?P<escaping>\\*)\$$")
+    match_parts_pattern = re.compile(r"^(?P<flag>\(\?\w\))?(?P<start>\^)?(?P<pattern>.*)")
+
     def __init__(self, key: List[str], regex: str):
-        self._key = key
+        self.key = key
         self._regex = self._normalize_regex(regex)
         self._matcher = re.compile(self._regex)
 
     def __repr__(self) -> str:
-        return f"{self._as_dotted_string(self._key)}:r/{self._regex}/"
+        return f"{self.as_dotted_string(self.key)}:r/{self._regex}/"
 
     @staticmethod
     def _normalize_regex(regex: str) -> str:
-        match = re.match(r".*?(?P<escaping>\\*)\$$", regex)
+        match = RegExFilterExpression.match_escaping_pattern.match(regex)
         if match and len(match.group("escaping")) % 2 == 0:
             end_token = ""
         else:
             end_token = "$"
-        match = re.match(r"^(?P<flag>\(\?\w\))?(?P<start>\^)?(?P<pattern>.*)", regex)
+        match = RegExFilterExpression.match_parts_pattern.match(regex)
         flag, _, pattern = match.groups()
         flag = "" if flag is None else flag
         pattern = "" if pattern is None else pattern
         return rf"{flag}^{pattern}{end_token}"
 
     def does_match(self, document: dict) -> bool:
-        value = self._get_value(self._key, document)
+        value = self._get_value(self.key, document)
 
         if isinstance(value, list):
             return any(filter(self._matcher.match, value))
         return self._matcher.match(str(value)) is not None
 
 
 class Exists(FilterExpression):
     """Filter expression that returns true if a given field exists."""
 
     def __init__(self, value: list):
         self.split_field = value
 
     def __repr__(self) -> str:
-        return f'"{self._as_dotted_string(self.split_field)}"'
+        return f'"{self.as_dotted_string(self.split_field)}"'
 
     def does_match(self, document: dict) -> bool:
         if not self.split_field:
             return False
 
         try:
             current = document
@@ -345,15 +361,15 @@
         return True
 
 
 class Null(FilterExpression):
     """Filter expression that returns true if a given field is set to null."""
 
     def __init__(self, key: List[str]):
-        self._key = key
+        self.key = key
 
     def __repr__(self) -> str:
-        return f"{self._as_dotted_string(self._key)}:{None}"
+        return f"{self.as_dotted_string(self.key)}:{None}"
 
     def does_match(self, document: dict) -> bool:
-        value = self._get_value(self._key, document)
+        value = self._get_value(self.key, document)
         return value is None
```

### Comparing `logprep-6.0.0/logprep/filter/lucene_filter.py` & `logprep-6.1.0/logprep/processor/generic_adder/processor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,313 +1,264 @@
 """
-Filter
-======
-
-The filters are based on the Lucene query language, but contain some additional enhancements.
-It is possible to filter for keys and values in log messages.
-**Dot notation** is used to access subfields in log messages.
-A filter for :code:`{'field': {'subfield': 'value'}}` can be specified by
-:code:`field.subfield': 'value`.
-
-If a key without a value is given it is filtered for the existence of the key.
-The existence of a specific field can therefore be checked by a key without a value.
-The filter :code:`filter: field.subfield` would match for every value :code:`subfield` in
-:code:`{'field': {'subfield': 'value'}}`.
-The special key :code:`*` can be used to always match on any input.
-Thus, the filter :code:`filter: *` would match any input document.
-
-The filter in the following example would match fields :code:`ip_address` with the
-value :code:`192.168.0.1`.
-Meaning all following transformations done by this rule would be applied only
-on log messages that match this criterion.
-This example is not complete, since rules are specific to processors and require additional options.
-
-
-..  code-block:: json
-    :linenos:
-    :caption: Example
-
-    { "filter": "ip_address: 192.168.0.1" }
-
-It is possible to use filters with field names that contain white spaces or use special symbols
-of the Lucene syntax. However, this has to be escaped.
-The filter :code:`filter: 'field.a subfield(test): value'` must be escaped as
-:code:`filter: 'field.a\ subfield\(test\): value'`.
-Other references to this field do not require such escaping.
-This is *only* necessary for the filter.
-It is necessary to escape twice if the file is in the JSON format - once for
-the filter itself and once for JSON.
-
-Operators
----------
-
-A subset of Lucene query operators is supported:
-
-- **NOT**: Condition is not true.
-- **AND**: Connects two conditions. Both conditions must be true.
-- **OR**: Connects two conditions. At least one them must be true.
-
-In the following example log messages are filtered for which :code:`event_id: 1` is true and
-:code:`ip_address: 192.168.0.1` is false.
-This example is not complete, since rules are specific to processors and require additional options.
-
-
-..  code-block:: json
-    :linenos:
-    :caption: Example
-
-    { "filter": "event_id: 1 AND NOT ip_address: 192.168.0.1" }
-
-RegEx-Filter
+GenericAdder
 ------------
-
-It is possible use regex expressions to match values.
-For this, the field with the regex pattern must be added to the optional field
-:code:`regex_fields` in the rule definition.
-
-In the following example the field :code:`ip_address` is defined as regex field.
-It would be filtered for log messages in which the value :code:`ip_address` starts with
-:code:`192.168.0.`.
-This example is not complete, since rules are specific to processors and
-require additional options.
+The `generic_adder` is a processor that adds new fields and values to documents based on a list.
+The list can reside inside a rule, inside a file or retrieved from an sql database.
 
 
+Example
+^^^^^^^
 ..  code-block:: yaml
     :linenos:
-    :caption: Example
 
-    filter: 'ip_address: "192\.168\.0\..*"'
-    regex_fields:
-    - ip_address
+    - genericaddername:
+        type: generic_adder
+        specific_rules:
+            - tests/testdata/rules/specific/
+        generic_rules:
+            - tests/testdata/rules/generic/
+        sql_config:
+            user: example_user
+            password: example_password
+            host: "127.0.0.1
+            database: example_db
+            table: example_table
+            target_column: example_column
+            add_target_column: True
+            timer: 0.1
 """
-
-from typing import List, Union, Optional
+import json
+import os
 import re
-from itertools import chain, zip_longest
+import time
+from logging import Logger
+from typing import Optional
+
+from attr import define, field, validators
+from filelock import FileLock
+
+from logprep.abc.processor import Processor
+from logprep.factory_error import InvalidConfigurationError
+from logprep.processor.base.exceptions import FieldExistsWarning
+from logprep.processor.generic_adder.mysql_connector import MySQLConnector
+from logprep.processor.generic_adder.rule import GenericAdderRule
+from logprep.util.helper import add_field_to, get_dotted_field_value
+
+
+class GenericAdderError(BaseException):
+    """Base class for GenericAdder related exceptions."""
+
+    def __init__(self, name: str, message: str):
+        super().__init__(f"GenericAdder ({name}): {message}")
+
+
+def sql_config_validator(_, attribute, value):
+    """validate if a subfield of a dict is valid"""
+    if attribute.name == "sql_config" and isinstance(value, dict):
+        table = value.get("table")
+        if table and re.search(r"\s", table):
+            raise InvalidConfigurationError("Table in 'sql_config' contains whitespaces!")
+        if table and not re.search(r"^[a-zA-Z0-9_]+$", table):
+            raise InvalidConfigurationError(
+                "Table in 'sql_config' may only contain alphanumeric characters and underscores!"
+            )
 
-import luqum
-from luqum.parser import parser, ParseSyntaxError, IllegalCharacterError
-from luqum.tree import OrOperation, AndOperation, Group, FieldGroup, SearchField, Phrase, Word, Not
-
-from logprep.filter.expression.filter_expression import (
-    Or,
-    And,
-    StringFilterExpression,
-    WildcardStringFilterExpression,
-    SigmaFilterExpression,
-    RegExFilterExpression,
-    Not as NotExpression,
-    Exists,
-    Null,
-    Always,
-    FilterExpression,
-)
-
-
-class LuceneFilterError(BaseException):
-    """Base class for LuceneFilter related exceptions."""
-
-
-class LuceneFilter:
-    """A filter that allows using lucene query strings."""
-
-    @staticmethod
-    def create(query_string: str, special_fields: dict = None) -> FilterExpression:
-        """Create a FilterExpression from a lucene query string.
 
-        Parameters
-        ----------
-        query_string : str
-           A lucene query string.
-        special_fields : list, optional
-           Determines if query_string should be processed as regex-query or sigma-query.
-
-        Returns
-        -------
-        filter : FilterExpression
-            A lucene query parsed into a FilterExpression.
-
-        Raises
-        ------
-        LuceneFilterError
-            Raises if lucene filter could not be built.
+class GenericAdder(Processor):
+    """Resolve values in documents by referencing a mapping list."""
 
+    @define(kw_only=True)
+    class Config(Processor.Config):
+        """GenericAdder config"""
+
+        sql_config: Optional[dict] = field(
+            default=None,
+            validator=[
+                validators.optional(validator=validators.instance_of(dict)),
+                sql_config_validator,
+            ],
+        )
+        """
+        Configuration of the connection to a MySQL database and settings on how to add data from
+        the database.
+        This field is optional. The database feature will not be used if `sql_config` is omitted.
+        Has following subfields:
+
+        - `user` - The user to use when connecting to the MySQL database.
+        - `password` - The password to use when connecting to the MySQL database.
+        - `host` - The host to use when connecting to the MySQL database.
+        - `database` - The database name to use when connecting to the MySQL database.
+        - `table` - The table name to use when connecting to the MySQL database.
+        - `target_column` - The name of the column whose values are being matched against a value
+          from an event.
+          If a value matches, the remaining values of the row with the match are being added to
+          the event.
+        - `add_target_column` - Determines if the target column itself will be added to the event.
+          This is set to false per default.
+        - `timer` - Period how long to wait (in seconds) before the database table is being checked
+          for changes.
+          If there is a change, the table is reloaded by Logprep.
+        - `file_lock_path` - Path to a file lock used by the adder when updating the SQL table
+          (default: ./sql_update.lock).
+        - `db_file_path` - Path to a file used to store the SQL table obtained by the generic adder
+          (default: ./sql_db_table.json).
         """
-        query_string = LuceneFilter._add_lucene_escaping(query_string)
-
-        try:
-            tree = parser.parse(query_string)
-            transformer = LuceneTransformer(tree, special_fields)
-        except (ParseSyntaxError, IllegalCharacterError) as error:
-            raise LuceneFilterError(error)
-
-        return transformer.build_filter()
-
-    @staticmethod
-    def _add_lucene_escaping(query_string):
-        """Ignore all escaping and escape only double quotes so that lucene can be parsed."""
-        matches = re.findall(r'.*?((?:\\)+").*?', query_string)
-        for idx, match in enumerate(matches):
-            length = len(match) - 1
-            if length > 1:
-                matches[idx] = "\\" + matches[idx]
-        split = re.split(r'(?:\\)+"', query_string)
-        query_string = "".join([x for x in chain.from_iterable(zip_longest(split, matches)) if x])
-
-        query_string = re.sub(r'((?:\\)+"[\s\)]*(?:AND|OR|NOT|$))', r"\\\g<1>", query_string)
-        return query_string
-
-
-class LuceneTransformer:
-    """A transformer that converts a luqum tree into a FilterExpression."""
-
-    _special_fields_map = {
-        "regex_fields": RegExFilterExpression,
-        "sigma_fields": SigmaFilterExpression,
-    }
-
-    def __init__(self, tree: luqum.tree, special_fields: dict = None):
-        self._tree = tree
-
-        self._special_fields = dict()
-
-        special_fields = special_fields if special_fields else dict()
-        for key in self._special_fields_map.keys():
-            self._special_fields[key] = (
-                special_fields.get(key) if special_fields.get(key) else list()
-            )
-
-        self._last_search_field = None
-
-    def build_filter(self) -> FilterExpression:
-        """Transform luqum tree into FilterExpression
 
-        Returns
-        -------
-        filter : FilterExpression
-            A luqum.tree parsed into a FilterExpression.
+    rule_class = GenericAdderRule
 
+    __slots__ = [
+        "_db_connector",
+        "_db_table",
+        "_file_lock_path",
+        "_db_file_path",
+        "_file_check_interval",
+    ]
+
+    _db_table: Optional[dict]
+    """Dict containing table from SQL database"""
+
+    _db_connector: MySQLConnector
+    """Connector for MySQL database"""
+
+    _file_check_interval: Optional[float]
+    """Time that has to pass for the database file to become stale"""
+
+    _file_lock_path: Optional[str]
+    """Path to file lock for database update"""
+
+    _db_file_path: Optional[str]
+    """Path to file containing table from SQL database"""
+
+    def __init__(self, name: str, configuration: Processor.Config, logger: Logger):
+        """Initialize a generic adder instance.
+        Performs a basic processor initialization. Furthermore, a SQL database and a SQL table are
+        being initialized if a SQL configuration exists.
+        Parameters
+        ----------
+        name : str
+           Name for the generic adder.
+        configuration : Processor.Config
+           Configuration for SQL adding and rule loading.
+        logger : logging.Logger
+           Logger to use.
         """
-        return self._parse_tree(self._tree)
-
-    def _parse_tree(self, tree: luqum.tree) -> FilterExpression:
-        if isinstance(tree, OrOperation):
-            return Or(*self._collect_children(tree))
-        if isinstance(tree, AndOperation):
-            return And(*self._collect_children(tree))
-        if isinstance(tree, Not):
-            return NotExpression(
-                *self._collect_children(tree)
-            )  # pylint: disable=no-value-for-parameter
-        if isinstance(tree, Group):
-            return self._parse_tree(tree.children[0])
-        if isinstance(tree, SearchField):
-            if isinstance(tree.expr, FieldGroup):
-                self._last_search_field = tree.name
-                parsed = self._parse_tree(tree.expr.children[0])
-                self._last_search_field = None
-                return parsed
-            else:
-                return self._create_field(tree)
-        if isinstance(tree, Word):
-            if self._last_search_field:
-                return self._create_field_group_expression(tree)
-            else:
-                return self._create_value_expression(tree)
-        if isinstance(tree, Phrase):
-            if self._last_search_field:
-                return self._create_field_group_expression(tree)
-            else:
-                return self._create_value_expression(tree)
-        raise LuceneFilterError('The expression "{}" is invalid!'.format(str(tree)))
+        super().__init__(name, configuration, logger)
 
-    def _create_field_group_expression(self, tree: luqum.tree) -> FilterExpression:
-        """Creates filter expression that is resulting from a field group.
+        self._db_table = None
+        sql_config = configuration.sql_config
+        if sql_config:
+            self._initialize_sql(sql_config)
+
+    def _initialize_sql(self, sql_config):
+        self._db_connector = MySQLConnector(sql_config, self._logger) if sql_config else None
+        if self._db_connector:
+            self._file_lock_path = sql_config.get("file_lock_path", "sql_update.lock")
+            self._db_file_path = sql_config.get("db_file_path", "sql_db_table.json")
+            self._file_check_interval = sql_config.get("timer", 60 * 3)
+
+            self._check_connection()
+            self._update_db_table()
+
+    def _check_connection(self):
+        """Check connections with lock to prevent a sudden spike of connections to the database.
+
+        Checking at initialization prevents error documents caused by a wrong connection
+        configuration when starting Logprep"""
+        with FileLock(self._file_lock_path):  # pylint: disable=abstract-class-instantiated
+            self._db_connector.connect()
+            self._db_connector.disconnect()
+
+    def _update_db_table(self):
+        if self._db_connector.time_to_check_for_change():
+            with FileLock(self._file_lock_path):  # pylint: disable=abstract-class-instantiated
+                now = time.time()
+                if self._check_if_file_not_exists_or_stale(now):
+                    self._update_from_db_and_write_to_file()
+                else:
+                    self._load_from_file()
+
+    def _load_from_file(self):
+        with open(self._db_file_path, "r", encoding="utf8") as db_file:
+            self._db_table = json.load(db_file)
 
+    def _update_from_db_and_write_to_file(self):
+        self._db_connector.connect()
+        try:
+            if self._db_connector.has_changed():
+                self._db_table = self._db_connector.get_data()
+                with open(self._db_file_path, "w", encoding="utf8") as db_file:
+                    json.dump(self._db_table, db_file)
+        finally:
+            self._db_connector.disconnect()
+
+    def _check_if_file_not_exists_or_stale(self, now):
+        if not os.path.isfile(self._db_file_path):
+            return True
+        if now - os.path.getmtime(self._db_file_path) > self._file_check_interval:
+            return True
+        return False
+
+    def _apply_rules(self, event: dict, rule: GenericAdderRule):
+        """Apply a matching generic adder rule to the event.
+         Add fields and values to the event according to the rules it matches for.
+        Additions can come from the rule definition, from a file or from a SQL table.
+        The SQL table is initially loaded from the database and then reloaded if it changes.
+        At first it checks if a SQL table exists and if it will be used. If it does, it adds all
+        values from a matching row in the table to the event. To determine if a row matches, a
+        pattern is used on a defined value of the event to extract a subvalue that is then matched
+        against a value in a defined column of the SQL table. A dotted path prefix can be applied to
+        add the new fields into a shared nested location.
+        If no table exists, fields defined withing the rule itself or in a rule file are being added
+        to the event.
         Parameters
         ----------
-        tree : luqum.tree
-            luqum.tree to create field group expression from.
+        event : dict
+           Name of the event to add keys and values to.
+        rule : GenericAdderRule
+           A matching generic adder rule.
+        Raises
+        ------
+        FieldExistsWarning
+            Raises if an addition would overwrite an existing field or value.
+        """
+        conflicting_fields = []
+
+        use_db = rule.db_target and self._db_table
+        if use_db:
+            self._update_db_table()
+
+        items_to_add = [] if use_db else rule.add.items()
+        if use_db and rule.db_pattern:
+            self._try_adding_from_db(event, items_to_add, rule)
+
+        # Add the items to the event
+        for dotted_field, value in items_to_add:
+            add_successful = add_field_to(
+                event,
+                output_field=dotted_field,
+                content=value,
+                extends_lists=rule.extend_target_list,
+                overwrite_output_field=rule.overwrite_target,
+            )
+            if not add_successful:
+                conflicting_fields.append(dotted_field)
 
-        Returns
-        -------
-        FilterExpression
-            Parsed filter expression.
+        if conflicting_fields:
+            raise FieldExistsWarning(self, rule, event, conflicting_fields)
 
-        """
-        key = self._last_search_field.split(".")
-        value = self._strip_quote_from_string(tree.value)
-        value = self._remove_lucene_escaping(value)
-        return self._get_filter_expression(key, value)
-
-    def _collect_children(self, tree: luqum.tree) -> List[FilterExpression]:
-        expressions = []
-        for child in tree.children:
-            expressions.append(self._parse_tree(child))
-        return expressions
-
-    def _create_field(self, tree: luqum.tree) -> Optional[FilterExpression]:
-        if isinstance(tree.expr, (Phrase, Word)):
-            key = tree.name.replace("\\", "")
-            key = key.split(".")
-            if tree.expr.value == "null":
-                return Null(key)
-
-            value = self._strip_quote_from_string(tree.expr.value)
-            value = self._remove_lucene_escaping(value)
-            return self._get_filter_expression(key, value)
-        return None
-
-    def _get_filter_expression(
-        self, key: List[str], value
-    ) -> Union[RegExFilterExpression, StringFilterExpression]:
-        key_and_modifier = key[-1].split("|")
-        if len(key_and_modifier) == 2:
-            if key_and_modifier[-1] == "re":
-                return RegExFilterExpression(key[:-1] + key_and_modifier[:-1], value)
-
-        dotted_field = ".".join(key)
-        if self._special_fields.items():
-            for sf_key, sf_value in self._special_fields.items():
-                if sf_value is True or dotted_field in sf_value:
-                    return self._special_fields_map[sf_key](key, value)
-        return StringFilterExpression(key, value)
-
-    @staticmethod
-    def _create_value_expression(word: luqum.tree) -> Union[Exists, Always]:
-        value = word.value.replace("\\", "")
-        value = value.split(".")
-        if value == ["*"]:
-            return Always(True)
-        else:
-            return Exists(value)
-
-    @staticmethod
-    def _strip_quote_from_string(string: str) -> str:
-        if (string[0] == string[-1]) and (string[0] in ["'", '"']):
-            return string[1:-1]
-        return string
-
-    @staticmethod
-    def _remove_lucene_escaping(string):
-        """Remove previously added lucene escaping so that double quotes will be
-        interpreted correctly by wildcard parser."""
-        matches = re.findall(r'.*?((?:\\)*").*?', string)
-        for idx, match in enumerate(matches):
-            length = len(match) - 1
-            matches[idx] = "\\" * (length // 2 - 1) + '"'
-
-        split = re.split(r'(?:\\)*"', string)
-        string = "".join([x for x in chain.from_iterable(zip_longest(split, matches)) if x])
-
-        backslashes = 0
-        for x in range(len(string)):
-            chara = string[len(string) - 1 - x]
-            if chara == "\\":
-                backslashes += 1
-            else:
-                break
+    def _try_adding_from_db(self, event: dict, items_to_add: list, rule: GenericAdderRule):
+        """Get the sub part of the value from the event using a regex pattern"""
 
-        if backslashes > 0:
-            string = string[:-backslashes] + "\\" * (backslashes // 2 - 2)
+        value_to_check_in_db = get_dotted_field_value(event, rule.db_target)
+        match_with_value_in_db = rule.db_pattern.match(value_to_check_in_db)
+        if match_with_value_in_db:
+            # Get values to add from db table using the sub part
+            value_to_map = match_with_value_in_db.group(1).upper()
+            add_from_db = self._db_table.get(value_to_map, [])
+
+            if rule.db_destination_prefix:
+                for idx, _ in enumerate(add_from_db):
+                    if not add_from_db[idx][0].startswith(rule.db_destination_prefix):
+                        add_from_db[idx][0] = f"{rule.db_destination_prefix}.{add_from_db[idx][0]}"
 
-        return string
+            for item in add_from_db:
+                items_to_add.append(item)
```

### Comparing `logprep-6.0.0/logprep/framework/pipeline.py` & `logprep-6.1.0/logprep/framework/pipeline.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,48 @@
 """This module contains all Pipeline functionality.
 
 Pipelines contain a list of processors that can be executed in order to process input log data.
 They can be multi-processed.
 
 """
 # pylint: disable=logging-fstring-interpolation
-import json
 import queue
 import warnings
 from ctypes import c_bool, c_double, c_ulonglong
 from functools import cached_property
 from logging import INFO, NOTSET, Handler, Logger
 from multiprocessing import Lock, Process, Value, current_process
 from time import time
-from typing import List, Tuple
+from typing import Any, List, Tuple
 
 import attrs
+import msgspec
 import numpy as np
 
 from logprep._version import get_versions
+from logprep.abc.component import Component
 from logprep.abc.connector import Connector
 from logprep.abc.input import (
     CriticalInputError,
     FatalInputError,
     Input,
     SourceDisconnectedError,
     WarningInputError,
 )
-from logprep.abc.output import CriticalOutputError, FatalOutputError, WarningOutputError, Output
+from logprep.abc.output import (
+    CriticalOutputError,
+    FatalOutputError,
+    Output,
+    WarningOutputError,
+)
 from logprep.abc.processor import Processor
 from logprep.factory import Factory
-from logprep.metrics.metric import Metric, calculate_new_average, MetricTargets
+from logprep.metrics.metric import Metric, MetricTargets, calculate_new_average
 from logprep.metrics.metric_exposer import MetricExposer
-from logprep.processor.base.exceptions import ProcessingWarning, ProcessingWarningCollection
+from logprep.processor.base.exceptions import ProcessingCriticalError, ProcessingWarning
 from logprep.util.multiprocessing_log_handler import MultiprocessingLogHandler
 from logprep.util.pipeline_profiler import PipelineProfiler
 from logprep.util.time_measurement import TimeMeasurement
 
 
 class PipelineError(BaseException):
     """Base class for Pipeline related exceptions."""
@@ -105,14 +111,39 @@
                         )
                     if self._logger:
                         self._logger.info(msg)
                     self._val.value = 0
                     self._timer.value = time() + self._period
 
 
+def _handle_pipeline_error(func):
+    def _inner(self: "Pipeline") -> Any:
+        try:
+            return func(self)
+        except SourceDisconnectedError as error:
+            self.logger.warning(str(error))
+            self.stop()
+        except (WarningOutputError, WarningInputError) as error:
+            self.logger.warning(str(error))
+        except CriticalOutputError as error:
+            self.logger.error(str(error))
+        except (FatalOutputError, FatalInputError) as error:
+            self.logger.error(str(error))
+            self.stop()
+        except CriticalInputError as error:
+            if raw_input := error.raw_input and self._output:  # pylint: disable=protected-access
+                for _, output in self._output.items():  # pylint: disable=protected-access
+                    if output.default:
+                        output.store_failed(str(self), raw_input, {})
+            self.logger.error(str(error))
+        return None
+
+    return _inner
+
+
 class Pipeline:
     """Pipeline of processors to be processed."""
 
     # pylint: disable=logging-not-lazy
     # Would require too much change in the tests.
 
     @attrs.define(kw_only=True)
@@ -192,23 +223,26 @@
         shared_dict: dict = None,
         used_server_ports: dict = None,
         metric_targets: MetricTargets = None,
     ) -> None:
         if log_handler and not isinstance(log_handler, Handler):
             raise MustProvideALogHandlerError
         self._logprep_config = config
+        self._timeout = config.get("timeout")
         self._log_handler = log_handler
         self._continue_iterating = Value(c_bool)
 
         self._lock = lock
         self._shared_dict = shared_dict
         self._processing_counter = counter
         self._used_server_ports = used_server_ports
         self._metric_targets = metric_targets
         self.pipeline_index = pipeline_index
+        self._encoder = msgspec.msgpack.Encoder()
+        self._decoder = msgspec.msgpack.Decoder()
 
     @cached_property
     def _process_name(self) -> str:
         return current_process().name
 
     @cached_property
     def _event_version_information(self) -> dict:
@@ -224,15 +258,15 @@
     @cached_property
     def _metrics_exposer(self) -> MetricExposer:
         return MetricExposer(
             self._logprep_config.get("metrics", {}),
             self._metric_targets,
             self._shared_dict,
             self._lock,
-            self._logger,
+            self.logger,
         )
 
     @cached_property
     def metrics(self) -> PipelineMetrics:
         """The pipeline metrics object"""
         if self._metric_targets is None:
             return None
@@ -240,102 +274,101 @@
             input=self._input.metrics,
             output=[self._output.get(output).metrics for output in self._output],
             labels=self._metric_labels,
         )
 
     @cached_property
     def _pipeline(self) -> tuple:
-        self._logger.debug(f"Building '{self._process_name}'")
-        pipeline = tuple(
-            (self._create_processor(entry) for entry in self._logprep_config.get("pipeline"))
-        )
-        self._logger.debug(f"Finished building pipeline ({self._process_name})")
+        self.logger.debug(f"Building '{self._process_name}'")
+        pipeline = [self._create_processor(entry) for entry in self._logprep_config.get("pipeline")]
+        self.logger.debug(f"Finished building pipeline ({self._process_name})")
         return pipeline
 
     @cached_property
     def _output(self) -> dict[str, Output]:
         output_configs = self._logprep_config.get("output")
         if not output_configs:
             return None
         output_names = list(output_configs.keys())
         outputs = {}
         for output_name in output_names:
             output_configs[output_name]["metric_labels"] = self._metric_labels
             output_config = output_configs.get(output_name)
-            outputs |= {output_name: Factory.create({output_name: output_config}, self._logger)}
+            outputs |= {output_name: Factory.create({output_name: output_config}, self.logger)}
         return outputs
 
     @cached_property
     def _input(self) -> Input:
         input_connector_config = self._logprep_config.get("input")
         if input_connector_config is None:
             return None
         connector_name = list(input_connector_config.keys())[0]
         input_connector_config[connector_name]["metric_labels"] = self._metric_labels
         input_connector_config[connector_name].update(
             {"version_information": self._event_version_information}
         )
-        return Factory.create(input_connector_config, self._logger)
+        return Factory.create(input_connector_config, self.logger)
 
     @cached_property
-    def _logger(self) -> Logger:
+    def logger(self) -> Logger:
+        """the pipeline logger"""
         if self._log_handler is None:
             return Logger("Pipeline")
         if self._log_handler.level == NOTSET:
             self._log_handler.level = INFO
         logger = Logger("Pipeline", level=self._log_handler.level)
         for handler in logger.handlers:
             logger.removeHandler(handler)
         logger.addHandler(self._log_handler)
 
         return logger
 
+    @_handle_pipeline_error
     def _setup(self):
-        self._logger.debug(f"Creating connectors ({self._process_name})")
+        self.logger.debug(f"Creating connectors ({self._process_name})")
         for _, output in self._output.items():
             output.input_connector = self._input
-        self._logger.debug(
+        self.logger.debug(
             f"Created connectors -> input: '{self._input.describe()}',"
             f" output -> '{[output.describe() for _, output in self._output.items()]}' ({self._process_name})"
         )
         self._input.pipeline_index = self.pipeline_index
         self._input.setup()
         for _, output in self._output.items():
-            try:
-                output.setup()
-            except FatalOutputError as error:
-                self._logger.error(f"Output {output.describe()} failed: {error}")
-                output.metrics.number_of_errors += 1
-                self.stop()
+            output.setup()
+
         if hasattr(self._input, "server"):
             while self._input.server.config.port in self._used_server_ports:
                 self._input.server.config.port += 1
             self._used_server_ports.update({self._input.server.config.port: self._process_name})
-        self._logger.debug(f"Finished creating connectors ({self._process_name})")
+        self.logger.debug(f"Finished creating connectors ({self._process_name})")
+        self.logger.info(f"Start building pipeline ({self._process_name})")
+        _ = self._pipeline
+        self.logger.info(f"Finished building pipeline ({self._process_name})")
 
     def _create_processor(self, entry: dict) -> "Processor":
         processor_name = list(entry.keys())[0]
         entry[processor_name]["metric_labels"] = self._metric_labels
-        processor = Factory.create(entry, self._logger)
+        processor = Factory.create(entry, self.logger)
         processor.setup()
         if self.metrics:
             self.metrics.pipeline.append(processor.metrics)
-        self._logger.debug(f"Created '{processor}' processor ({self._process_name})")
+        self.logger.debug(f"Created '{processor}' processor ({self._process_name})")
         return processor
 
     def run(self) -> None:
         """Start processing processors in the Pipeline."""
         self._enable_iteration()
         assert self._input, "Pipeline should not be run without input connector"
         assert self._output, "Pipeline should not be run without output connector"
         with self._lock:
             with warnings.catch_warnings():
                 warnings.simplefilter("default")
                 self._setup()
-        self._logger.debug(f"Start iterating ({self._process_name})")
+        self.logger.debug(f"Start iterating ({self._process_name})")
         if hasattr(self._input, "server"):
             with self._input.server.run_in_thread():
                 while self._iterate():
                     self.process_pipeline()
         else:
             while self._iterate():
                 self.process_pipeline()
@@ -344,138 +377,74 @@
     def _iterate(self) -> bool:
         return self._continue_iterating.value
 
     def _enable_iteration(self) -> None:
         with self._continue_iterating.get_lock():
             self._continue_iterating.value = True
 
+    @_handle_pipeline_error
     def process_pipeline(self) -> Tuple[dict, list]:
         """Retrieve next event, process event with full pipeline and store or return results"""
         assert self._input, "Run process_pipeline only with an valid input connector"
         self._metrics_exposer.expose(self.metrics)
-        event = self._get_event()
+        Component.run_pending_tasks()
         extra_outputs = []
-        if event:
+        if event := self._get_event():
             extra_outputs = self.process_event(event)
         if event and self._output:
             self._store_event(event)
         return event, extra_outputs
 
     def _store_event(self, event: dict) -> None:
         for output_name, output in self._output.items():
             if output.default:
-                try:
-                    output.store(event)
-                    self._logger.debug(f"Stored output in {output_name}")
-                except WarningOutputError as error:
-                    self._logger.warning(
-                        f"An error occurred for output {output.describe()}: {error}"
-                    )
-                    output.metrics.number_of_warnings += 1
-                except CriticalOutputError as error:
-                    msg = f"A critical error occurred for output " f"{output.describe()}: {error}"
-                    self._logger.error(msg)
-                    if error.raw_input:
-                        output.store_failed(msg, error.raw_input, {})
-                    output.metrics.number_of_errors += 1
-                except FatalOutputError as error:
-                    self._logger.error(f"Output {output.describe()} failed: {error}")
-                    output.metrics.number_of_errors += 1
-                    self.stop()
+                output.store(event)
+                self.logger.debug(f"Stored output in {output_name}")
 
     def _get_event(self) -> dict:
+        event, non_critical_error_msg = self._input.get_next(self._timeout)
+        if non_critical_error_msg and self._output:
+            for _, output in self._output.items():
+                if output.default:
+                    output.store_failed(non_critical_error_msg, event, None)
         try:
-            event, non_critical_error_msg = self._input.get_next(
-                self._logprep_config.get("timeout")
-            )
-            if non_critical_error_msg and self._output:
-                for _, output in self._output.items():
-                    if output.default:
-                        output.store_failed(non_critical_error_msg, event, None)
-            try:
-                self.metrics.kafka_offset = self._input.current_offset
-            except AttributeError:
-                pass
-            return event
-        except SourceDisconnectedError:
-            self._logger.warning(
-                f"Lost or failed to establish connection to {self._input.describe()}"
-            )
-            self.stop()
-        except FatalInputError as error:
-            self._logger.error(f"Input {self._input.describe()} failed: {error}")
-            self._input.metrics.number_of_errors += 1
-            self.stop()
-        except WarningInputError as error:
-            self._logger.warning(f"An error occurred for input {self._input.describe()}: {error}")
-            self._input.metrics.number_of_warnings += 1
-        except CriticalInputError as error:
-            msg = f"A critical error occurred for input {self._input.describe()}: {error}"
-            self._logger.error(msg)
-            if error.raw_input:
-                for _, output in self._output.items():
-                    if output.default:
-                        output.store_failed(msg, error.raw_input, {})
-            self._input.metrics.number_of_errors += 1
-        return {}
+            self.metrics.kafka_offset = self._input.current_offset
+        except AttributeError:
+            pass
+        return event
 
     @TimeMeasurement.measure_time("pipeline")
     def process_event(self, event: dict):
-        event_received = json.dumps(event, separators=(",", ":"))
+        """process all processors for one event"""
+        event_received = self._encoder.encode(event)
         extra_outputs = []
         for processor in self._pipeline:
             try:
-                extra_data = processor.process(event)
-                if extra_data and self._output:
-                    self._store_extra_data(extra_data)
-                if extra_data:
+                if extra_data := processor.process(event):
+                    if self._output:
+                        self._store_extra_data(extra_data)
                     extra_outputs.append(extra_data)
             except ProcessingWarning as error:
-                self._handle_processing_warning(processor, error)
-            except ProcessingWarningCollection as error:
-                for warning in error.processing_warnings:
-                    self._handle_processing_warning(processor, warning)
-            except BaseException as error:  # pylint: disable=broad-except
-                msg = self._handle_fatal_processing_error(processor, error)
-                if self._output:
-                    for _, output in self._output.items():
-                        if output.default:
-                            output.store_failed(msg, json.loads(event_received), event)
-                processor.metrics.number_of_errors += 1
-                event.clear()  # 'delete' the event, i.e. no regular output
+                self.logger.warning(str(error))
+            except ProcessingCriticalError as error:
+                self.logger.error(str(error))
+                for _, output in self._output.items():
+                    if output.default:
+                        output.store_failed(str(error), self._decoder.decode(event_received), event)
             if not event:
-                self._logger.debug(f"Event deleted by processor {processor}")
                 break
         if self._processing_counter:
             self._processing_counter.increment()
             self._processing_counter.print_if_ready()
         if self.metrics:
             self.metrics.number_of_processed_events += 1
         return extra_outputs
 
-    def _handle_fatal_processing_error(self, processor: Processor, error: Exception) -> str:
-        original_error_msg = type(error).__name__
-        if str(error):
-            original_error_msg += f": {error}"
-        msg = (
-            f"A critical error occurred for processor {processor.describe()} when "
-            f"processing an event, processing was aborted: ({original_error_msg})"
-        )
-        self._logger.error(msg)
-        return msg
-
-    def _handle_processing_warning(self, processor: Processor, error: Exception) -> None:
-        self._logger.warning(
-            f"A non-fatal error occurred for processor {processor.describe()} "
-            f"when processing an event: {error}"
-        )
-        processor.metrics.number_of_warnings += 1
-
     def _store_extra_data(self, extra_data: List[tuple]) -> None:
-        self._logger.debug("Storing extra data")
+        self.logger.debug("Storing extra data")
         if isinstance(extra_data, tuple):
             documents, outputs = extra_data
             for document in documents:
                 for output in outputs:
                     for output_name, topic in output.items():
                         self._output[output_name].store_custom(document, topic)
             return
```

### Comparing `logprep-6.0.0/logprep/framework/pipeline_manager.py` & `logprep-6.1.0/logprep/framework/pipeline_manager.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/framework/rule_tree/node.py` & `logprep-6.1.0/logprep/framework/rule_tree/node.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/framework/rule_tree/rule_parser.py` & `logprep-6.1.0/logprep/framework/rule_tree/rule_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 behavior, allowing a simpler construction of the rule tree.
 
 """
 
 from typing import Union
 
 from logprep.filter.expression.filter_expression import (
-    Or,
-    CompoundFilterExpression,
-    Not,
+    Always,
     And,
+    CompoundFilterExpression,
     Exists,
-    StringFilterExpression,
     FilterExpression,
-    Always,
+    Not,
+    Or,
+    StringFilterExpression,
 )
+from logprep.util.helper import get_dotted_field_list
 
 
 class RuleParserException(Exception):
     """Raise if rule parser encounters a problem."""
 
 
 class RuleParser:
@@ -99,27 +100,27 @@
         """
         if RuleParser._has_unresolved_not_expression(rule):
             if isinstance(rule, Not):
                 exp = rule.expression
 
                 if isinstance(exp, StringFilterExpression):
                     return rule
-                elif isinstance(exp, Or):
+                if isinstance(exp, Or):
                     result_segments = ()
 
                     for or_segment in exp.expressions:
                         result_segments = result_segments + (Not(or_segment),)
 
                     result = And(*result_segments)
 
                     if RuleParser._has_unresolved_not_expression(result):
                         result = RuleParser._parse_not_expression(result)
 
                     return result
-                elif isinstance(exp, And):
+                if isinstance(exp, And):
                     result_segments = ()
 
                     for and_segment in exp.expressions:
                         result_segments = result_segments + (Not(and_segment),)
 
                     result = Or(*result_segments)
 
@@ -147,15 +148,15 @@
 
                 result = Or(*result_segments)
                 return result
         else:
             return rule
 
     @staticmethod
-    def _has_unresolved_not_expression(rule: FilterExpression):
+    def _has_unresolved_not_expression(rule: FilterExpression) -> bool:
         """Check if given filter expression contains NOT-expressions.
 
         This function checks if the given filter expression contains any unresolved NOT-expressions.
         Simple NOT(field: value) expressions do not count as unresolved expression since it cannot
         be resolved.
 
         Parameters
@@ -172,83 +173,86 @@
         if isinstance(rule, Not):
             if isinstance(rule.expression, CompoundFilterExpression):
                 return True
         elif isinstance(rule, CompoundFilterExpression):
             for expression in rule.expressions:
                 if RuleParser._has_unresolved_not_expression(expression):
                     return True
+        return False
 
     @staticmethod
-    def _parse_or_expression(rule: FilterExpression) -> Union[list, tuple, FilterExpression]:
+    def _parse_or_expression(rule: FilterExpression) -> Union[list, tuple, FilterExpression, None]:
         """Parse filters with OR-expressions.
 
         This function parses filter expressions with OR-expressions recursively by splitting them
         into separate filter expressions using the distributive property of the logical operators
         AND and OR. During the recursive parsing process, different types are returned.
         Hence, different cases have to be handled when constructing the results.
 
         Parameters
         ----------
         rule: FilterExpression
             Filter expression with OR-expressions to be parsed.
 
         Returns
         -------
-        result: Union[list, tuple, FilterExpression]
+        result: Union[list, tuple, FilterExpression, None]
             Resulting filter expression created by resolving OR- and AND-expressions in the given
             filter expression. The return type may differ depending on the level of recursion.
 
         """
         if RuleParser._has_or_expression(rule):
             # If expression is OR-expression, parse it
             if isinstance(rule, Or):
                 result_list = []
 
                 for exp in rule.expressions:
                     # Recursively parse subexpressions of current expressions
                     loop_result = RuleParser._parse_or_expression(exp)
 
-                    # Differentiate between different loop_result types and construct result_list accordingly
+                    # Differentiate between different loop_result types
+                    # and construct result_list accordingly
                     if not isinstance(loop_result, list):
                         if isinstance(loop_result, tuple):
                             loop_result = list(loop_result)
                         else:
                             loop_result = [loop_result]
                     if isinstance(loop_result, list) and isinstance(loop_result[0], list):
                         for element in loop_result:
                             result_list.append(element)
                     else:
                         result_list.append(loop_result)
 
                 return result_list
-            # Else, if expression is AND-expression, parse it and continue to parse OR-expression afterwards
-            elif isinstance(rule, And):
+            # Else, if expression is AND-expression,
+            # parse it and continue to parse OR-expression afterwards
+            if isinstance(rule, And):
                 loop_results = []
 
                 for exp in rule.expressions:
                     # Recursively parse subexpressions of current expressions
                     loop_results.append(RuleParser._parse_or_expression(exp))
 
                 # Iterate through loop_results and resolve tuples
                 for loop_result in loop_results:
                     if isinstance(loop_result, tuple):
                         tuple_segment = loop_result
-                        loop_results.remove(tuple_segment)
+                        loop_results.remove(tuple_segment)  # pylint: disable=W4701
 
                         for tuple_element in tuple_segment:
                             loop_results.insert(0, tuple_element)
 
                 # Continue to parse OR-expressions in already parsed subexpressions
                 return RuleParser._parse_or(loop_results)
         else:
             # Handle cases that may occur in recursive parsing process
             if isinstance(rule, And):
                 return tuple(RuleParser._parse_and_expression(rule))
-            else:
-                return rule
+            return rule
+        return None
 
     @staticmethod
     def _parse_or(loop_results: list):
         """Parse OR-expressions.
 
         This function handles the parsing of OR-subexpressions in AND-expression filters in a
         recursive manner.
@@ -273,15 +277,16 @@
         for or_element in or_segment:
             result_list.append(loop_results + or_element)
 
         # Recursively resolve elements in result_list
         for parsed_rule in result_list.copy():
             for segment in parsed_rule:
                 if isinstance(segment, list):
-                    result_list.remove(parsed_rule)
+                    if parsed_rule in result_list:
+                        result_list.remove(parsed_rule)
                     rule_list = RuleParser._parse_or(parsed_rule)
 
                     for rule in rule_list:
                         result_list.append(rule)
 
         return result_list
 
@@ -326,15 +331,15 @@
         -------
         has_or_expression: bool
             Decision if given expression has OR-expression.
 
         """
         if isinstance(expression, Or):
             return True
-        elif isinstance(expression, CompoundFilterExpression):
+        if isinstance(expression, CompoundFilterExpression):
             for exp in expression.expressions:
                 if RuleParser._has_or_expression(exp):
                     return True
 
         if isinstance(expression, Not):
             return RuleParser._has_or_expression(expression.expression)
 
@@ -360,58 +365,59 @@
             Dictionary with sorting priority information (key -> field name; value -> priority).
 
         """
         for parsed_rule in parsed_rule_list:
             parsed_rule.sort(key=lambda r: RuleParser._sort(r, priority_dict))
 
     @staticmethod
-    def _sort(r: StringFilterExpression, priority_dict: dict) -> Union[dict, str]:
+    def _sort(expr: StringFilterExpression, priority_dict: dict) -> Union[dict, str, None]:
         """Helper function for _sort_rule_segments.
 
         This function is used by the _sort_rule_segments() function in the sorting key.
         It includes various cases to cover all the different expression classes. For every class it
         tries to get a priority value from the priority dict. If the field name used in the
         expression does not exist in the priority dict, the field name itself is returned to use an
         alphabetical sort.
 
         Parameters
         ----------
-        r: StringFilterExpression
+        expr: StringFilterExpression
             Filter expression to get comparison value for.
         priority_dict: dict
             Dictionary with sorting priority information (key -> field name; value -> priority).
 
         Returns
         -------
-        comparison_value: str
+        comparison_value: Union[dict, str, None]
             Comparison value to use for sorting.
 
         """
-        if isinstance(r, Always):
-            return
-        elif isinstance(r, Not):
+        if isinstance(expr, Always):
+            return None
+        if isinstance(expr, Not):
             try:
-                if isinstance(r.expression, Exists):
-                    return priority_dict[r.expression._as_dotted_string(r.expression.split_field)]
-                elif isinstance(r.expression, Not):
-                    return priority_dict[r.expression.expression.split_field[0]]
-                else:
-                    return priority_dict[r._as_dotted_string(r.expression._key)]
+                if isinstance(expr.expression, Exists):
+                    return priority_dict[
+                        expr.expression.as_dotted_string(expr.expression.split_field)
+                    ]
+                if isinstance(expr.expression, Not):
+                    return priority_dict[expr.expression.expression.split_field[0]]
+                return priority_dict[expr.as_dotted_string(expr.expression.key)]
             except KeyError:
-                return RuleParser._sort(r.expression, priority_dict)
-        elif isinstance(r, Exists):
+                return RuleParser._sort(expr.expression, priority_dict)
+        elif isinstance(expr, Exists):
             try:
-                return priority_dict[r._as_dotted_string(r.split_field)]
+                return priority_dict[expr.as_dotted_string(expr.split_field)]
             except KeyError:
-                return r.__repr__()[1:-1]
+                return repr(expr)[1:-1]
         else:
             try:
-                return priority_dict[r._as_dotted_string(r._key)]
+                return priority_dict[expr.as_dotted_string(expr.key)]
             except KeyError:
-                return r.__repr__()
+                return repr(expr)
 
     @staticmethod
     def _parse_and_expression(expression: FilterExpression) -> list:
         """Parse AND-expression.
 
         This function parses AND-(sub)expressions in the given filter expression to a list of
         filter expressions.
@@ -432,16 +438,16 @@
         if isinstance(expression, And):
             for segment in expression.expressions:
                 if not isinstance(segment, And):
                     rule_list.append(segment)
                 else:
                     looped_result = RuleParser._parse_and_expression(segment)
 
-                    for s in looped_result:
-                        rule_list.append(s)
+                    for looped_segment in looped_result:
+                        rule_list.append(looped_segment)
 
         return rule_list
 
     @staticmethod
     def _add_special_tags(parsed_rules: list, tag_map: dict):
         """Add tags to rule filter.
 
@@ -476,22 +482,22 @@
                         if segment.split_field[0] in tag_map.keys():
                             RuleParser._add_tag(rule, tag_map[segment.split_field[0]])
                     elif isinstance(segment, Not):
                         expression = segment.expression
                         if isinstance(expression, Exists):
                             if expression.split_field[0] in tag_map.keys():
                                 RuleParser._add_tag(rule, tag_map[expression.split_field[0]])
-                        elif expression._key[0] in tag_map.keys():
-                            RuleParser._add_tag(rule, tag_map[expression._key[0]])
+                        elif expression.key[0] in tag_map.keys():
+                            RuleParser._add_tag(rule, tag_map[expression.key[0]])
                     # Always Expressions do not need tags
                     elif isinstance(segment, Always):
                         continue
                     else:
-                        if segment._key[0] in tag_map.keys():
-                            RuleParser._add_tag(rule, tag_map[segment._key[0]])
+                        if segment.key[0] in tag_map.keys():
+                            RuleParser._add_tag(rule, tag_map[segment.key[0]])
 
     @staticmethod
     def _add_tag(rule, tag_map_value: str):
         """Add tag helper function.
 
         This function implements the functionality to add a tag for _add_special_tags().
 
@@ -510,20 +516,20 @@
 
         """
         if RuleParser._tag_exists(rule[0], tag_map_value):
             return
 
         if ":" in tag_map_value:
             key, value = tag_map_value.split(":")
-            rule.insert(0, StringFilterExpression(key.split("."), value))
+            rule.insert(0, StringFilterExpression(get_dotted_field_list(key), value))
         else:
             rule.insert(0, Exists(tag_map_value.split(".")))
 
     @staticmethod
-    def _tag_exists(segment, tag):
+    def _tag_exists(segment: Union[Exists, StringFilterExpression], tag: str) -> bool:
         """Helper function for _add_tag.
 
         Checks if the given segment is equal to the given tag.
 
         Parameters
         ----------
         segment: Union[Exists, StringFilterExpression]
@@ -534,19 +540,20 @@
         Returns
         -------
         tag_exists: bool
             Decision if the given tag already exists as the given segment.
 
         """
         if isinstance(segment, Exists):
-            if segment.__repr__()[1:-1] == tag:
+            if repr(segment)[1:-1] == tag:
                 return True
         elif isinstance(segment, StringFilterExpression):
-            if segment.__repr__().replace('"', "") == tag:
+            if repr(segment).replace('"', "") == tag:
                 return True
+        return False
 
     @staticmethod
     def _add_exists_filter(parsed_rules: list):
         """Add Exists filter expression.
 
         In order to achieve better performances, this function adds Exists filter expression to
         the rule. E.g., before checking if a specific field "field" has values "a", "b" or "c" it
@@ -560,24 +567,23 @@
             List of parsed rules. Each rule is a list of filter expressions.
 
         """
         for parsed_rule in parsed_rules:
             temp_parsed_rule = parsed_rule.copy()
             skipped_counter = 0
 
-            for segment_index in range(len(temp_parsed_rule)):
-                segment = temp_parsed_rule[segment_index]
+            for segment_index, segment in enumerate(temp_parsed_rule):
                 # Skip Always()-, Exists()- and Not()-expressions when adding Exists()-filter
                 # Not()-expressions need to be skipped for cases where the field does not exist
                 if (
                     not isinstance(segment, Exists)
                     and not isinstance(segment, Not)
                     and not isinstance(segment, Always)
                 ):
-                    exists_filter = Exists(segment._key)
+                    exists_filter = Exists(segment.key)
 
                     # Skip if Exists()-filter already exists in Rule. No need to add it twice
                     if exists_filter in parsed_rule:
                         skipped_counter += 1
                     else:
                         # Insert Exists filter at the right place in the rule
                         parsed_rule.insert(segment_index * 2 - skipped_counter, exists_filter)
```

### Comparing `logprep-6.0.0/logprep/framework/rule_tree/rule_tree.py` & `logprep-6.1.0/logprep/framework/rule_tree/rule_tree.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/metrics/metric.py` & `logprep-6.1.0/logprep/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/metrics/metric_exposer.py` & `logprep-6.1.0/logprep/metrics/metric_exposer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/metrics/metric_targets.py` & `logprep-6.1.0/logprep/metrics/metric_targets.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/processor/base/exceptions.py` & `logprep-6.1.0/logprep/processor/base/exceptions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 """This module contains exceptions for rules."""
 
-from typing import Any, List
+from typing import TYPE_CHECKING, Any, List
 
 from logprep.factory_error import FactoryError
 
+if TYPE_CHECKING:
+    from logprep.abc.processor import Processor
+    from logprep.processor.base.rule import Rule
+
 
 class RuleError(BaseException):
     """Base class for Rule related exceptions."""
 
 
 class InvalidRuleDefinitionError(RuleError):
     """Raise if defined rule is invalid."""
@@ -41,39 +45,51 @@
     def __init__(self, processor_type=None):  # pragma: no cover
         if processor_type:
             super().__init__(f"Processor type '{processor_type}' can't be imported")
         else:
             super().__init__("Processor can't be imported")
 
 
-class ProcessingError(BaseException):
+class ProcessingError(Exception):
     """Base class for exceptions related to processing events."""
 
-    def __init__(self, name: str, message: str):
-        super().__init__(f"{name}: ({message})")
+    def __init__(self, processor: "Processor", message: str):
+        super().__init__(f"{self.__class__.__name__} in {processor.describe()}: {message}")
 
 
-class ProcessingWarning(ProcessingError):
-    """An minor error occurred - log the error but continue processing the event."""
+class ProcessingCriticalError(ProcessingError):
+    """A critical error occurred - stop processing of this event"""
 
-    def __init__(self, message: str):
-        super().__init__("ProcessingWarning", message)
+    def __init__(self, processor: "Processor", message: str, event: dict):
+        event.clear()
+        processor.metrics.number_of_errors += 1
+        super().__init__(processor, f"{message} -> event was deleted")
 
 
-class ProcessingWarningCollection(ProcessingError):
-    """A collection of ProcessingWarnings."""
+class ProcessingWarning(Warning):
+    """A minor error occurred - log the error, but continue processing the event."""
 
-    def __init__(self, name: str, message: str, processing_warnings):
-        super().__init__(name, message)
-        self.processing_warnings = processing_warnings
+    def __init__(self, processor: "Processor", message: str, rule: "Rule", event: dict):
+        processor.metrics.number_of_warnings += 1
+        message = f"""{message}
+Rule: {rule},
+Event: {event}
+        """
+        super().__init__(f"{self.__class__.__name__} in {processor.describe()}: {message}")
 
 
-class DuplicationError(ProcessingWarning):
-    """Raise if field already exists."""
+class FieldExistsWarning(ProcessingWarning):
+    """Raised if field already exists."""
 
-    def __init__(self, name: str, skipped_fields: List[str]):
+    def __init__(
+        self,
+        processor: "Processor",
+        rule: "Rule",
+        event: dict,
+        skipped_fields: List[str],
+    ):
         message = (
-            f"{name} - The following fields could not be written, because "
+            "The following fields could not be written, because "
             "one or more subfields existed and could not be extended: "
+            f"{', '.join(skipped_fields)}"
         )
-        message += " ".join(skipped_fields)
-        super().__init__(message)
+        super().__init__(processor, message, rule, event)
```

### Comparing `logprep-6.0.0/logprep/processor/base/rule.py` & `logprep-6.1.0/logprep/processor/base/rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
    The dotted field notation is available in all processors, the use of indices to access list
    elements is though not available in the :code:`Clusterer`, :code:`Labeler` and the
    :code:`Pseudonymizer`.
 """
 
 import json
 from os.path import basename, splitext
-from typing import List, Set, Optional, Dict
+from typing import Dict, List, Optional, Set
 
 from attrs import define, field, validators
 from ruamel.yaml import YAML
 
 from logprep.filter.expression.filter_expression import FilterExpression
 from logprep.filter.lucene_filter import LuceneFilter
 from logprep.metrics.metric import Metric, calculate_new_average
@@ -227,15 +227,15 @@
         return all([other.filter == self._filter, other._config == self._config])
 
     def __hash__(self) -> int:  # pylint: disable=function-redefined
         return id(self)
 
     def __repr__(self) -> str:
         if hasattr(self, "_config"):
-            return f"filter={self.filter}, {self._config}"
+            return f"filename={self.file_name}, filter={self.filter}, {self._config}"
         return super().__repr__()
 
     # pylint: disable=C0111
     @property
     def filter(self):
         return self._filter
```

### Comparing `logprep-6.0.0/logprep/processor/calculator/fourFn.py` & `logprep-6.1.0/logprep/processor/calculator/fourFn.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/processor/calculator/processor.py` & `logprep-6.1.0/logprep/processor/calculator/processor.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,32 +22,33 @@
 from functools import cached_property
 
 from pyparsing import ParseException
 
 from logprep.abc.processor import Processor
 from logprep.processor.calculator.fourFn import BNF
 from logprep.processor.calculator.rule import CalculatorRule
-from logprep.util.helper import get_source_fields_dict
 from logprep.util.decorators import timeout
+from logprep.util.helper import get_source_fields_dict
 
 
 class Calculator(Processor):
     """A Processor to calculate with and without field values"""
 
     rule_class = CalculatorRule
 
     def _apply_rules(self, event, rule):
         source_field_dict = get_source_fields_dict(event, rule)
-        self._check_for_missing_values(event, rule, source_field_dict)
-        expression = self._template(rule.calc, source_field_dict)
-        try:
-            result = self._calculate(event, rule, expression)
-        except TimeoutError as error:
-            self._handle_warning_error(event, rule, error)
-        self._write_target_field(event, rule, result)
+        if not self._has_missing_values(event, rule, source_field_dict):
+            expression = self._template(rule.calc, source_field_dict)
+            try:
+                result = self._calculate(event, rule, expression)
+                if result is not None:
+                    self._write_target_field(event, rule, result)
+            except TimeoutError as error:
+                self._handle_warning_error(event, rule, error)
 
     @cached_property
     def bnf(self) -> BNF:
         """Holds the Backus-Naur Form definition
 
         Returns
         -------
@@ -65,20 +66,20 @@
         return string
 
     def _calculate(self, event, rule, expression):
         @timeout(seconds=rule.timeout)
         def calculate(event, rule, expression):
             try:
                 _ = self.bnf.parseString(expression, parseAll=True)
-                result = self.bnf.evaluate_stack()
+                return self.bnf.evaluate_stack()
             except ParseException as error:
                 error.msg = f"({self.name}): expression '{error.line}' could not be parsed"
                 self._handle_warning_error(event, rule, error)
             except ArithmeticError as error:
                 error.args = [
                     f"({self.name}): expression '{rule.calc}' => '{expression}' results in "
                     + f"{error.args[0]}"
                 ]
                 self._handle_warning_error(event, rule, error)
-            return result
+            return None
 
         return calculate(event, rule, expression)
```

### Comparing `logprep-6.0.0/logprep/processor/calculator/rule.py` & `logprep-6.1.0/logprep/processor/calculator/rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,17 +82,17 @@
 * :code:`all(1,1,1,1,1,0)` => :code:`False`
 
 The calc expression is not whitespace sensitive.
 
 """
 import re
 
-from attrs import field, define, validators
+from attrs import define, field, validators
 
-from logprep.processor.field_manager.rule import FieldManagerRule, FIELD_PATTERN
+from logprep.processor.field_manager.rule import FIELD_PATTERN, FieldManagerRule
 
 
 class CalculatorRule(FieldManagerRule):
     """CalculatorRule"""
 
     @define(kw_only=True)
     class Config(FieldManagerRule.Config):
@@ -109,14 +109,15 @@
         of the source fields.
         """
         timeout: int = field(validator=validators.instance_of(int), converter=int, default=1)
         """The maximum time in seconds for the calculation. Defaults to :code:`1`"""
 
         def __attrs_post_init__(self):
             self.source_fields = re.findall(FIELD_PATTERN, self.calc)
+            super().__attrs_post_init__()
 
     @property
     def calc(self):
         """Returns the calculation expression"""
         return self._config.calc
 
     @property
```

### Comparing `logprep-6.0.0/logprep/processor/clusterer/processor.py` & `logprep-6.1.0/logprep/processor/clusterer/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/processor/clusterer/rule.py` & `logprep-6.1.0/logprep/processor/clusterer/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/processor/clusterer/signature_calculation/signature_phase.py` & `logprep-6.1.0/logprep/processor/clusterer/signature_calculation/signature_phase.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/processor/concatenator/processor.py` & `logprep-6.1.0/logprep/processor/concatenator/processor.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,17 +16,16 @@
         type: concatenator
         specific_rules:
             - tests/testdata/rules/specific/
         generic_rules:
             - tests/testdata/rules/generic/
 """
 from logprep.abc.processor import Processor
-from logprep.processor.base.exceptions import DuplicationError
 from logprep.processor.concatenator.rule import ConcatenatorRule
-from logprep.util.helper import add_field_to, get_dotted_field_value
+from logprep.util.helper import get_dotted_field_value
 
 
 class ConcatenatorError(BaseException):
     """Base class for Concatenator related exceptions."""
 
     def __init__(self, name: str, message: str):
         super().__init__(f"Concatenator ({name}): {message}")
@@ -55,12 +54,8 @@
         for source_field in rule.source_fields:
             field_value = get_dotted_field_value(event, source_field)
             source_field_values.append(field_value)
 
         source_field_values = [field for field in source_field_values if field is not None]
         target_value = f"{rule.separator}".join(source_field_values)
 
-        adding_was_successful = add_field_to(
-            event, rule.target_field, target_value, overwrite_output_field=rule.overwrite_target
-        )
-        if not adding_was_successful:
-            raise DuplicationError(self.name, [rule.target_field])
+        self._write_target_field(event, rule, target_value)
```

### Comparing `logprep-6.0.0/logprep/processor/concatenator/rule.py` & `logprep-6.1.0/logprep/processor/concatenator/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/processor/datetime_extractor/processor.py` & `logprep-6.1.0/logprep/processor/datetime_extractor/processor.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,17 +22,16 @@
 from datetime import datetime
 from logging import Logger
 
 from dateutil.parser import parse
 from dateutil.tz import tzlocal
 
 from logprep.abc.processor import Processor
-from logprep.processor.base.exceptions import DuplicationError
 from logprep.processor.datetime_extractor.rule import DatetimeExtractorRule
-from logprep.util.helper import add_field_to, get_dotted_field_value
+from logprep.util.helper import get_dotted_field_value
 
 
 class DateTimeExtractorError(BaseException):
     """Base class for DateTimeExtractor related exceptions."""
 
     def __init__(self, name: str, message: str):
         super().__init__(f"DateTimeExtractor ({name}): {message}")
@@ -78,15 +77,8 @@
                 "second": parsed_timestamp.second,
                 "microsecond": parsed_timestamp.microsecond,
                 "weekday": parsed_timestamp.strftime("%A"),
                 "timezone": self._local_timezone_name,
             }
 
             if split_timestamp:
-                adding_was_successful = add_field_to(
-                    event,
-                    rule.target_field,
-                    split_timestamp,
-                    overwrite_output_field=rule.overwrite_target,
-                )
-                if not adding_was_successful:
-                    raise DuplicationError(self.name, [rule.target_field])
+                self._write_target_field(event, rule, split_timestamp)
```

### Comparing `logprep-6.0.0/logprep/processor/datetime_extractor/rule.py` & `logprep-6.1.0/logprep/processor/datetime_extractor/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/processor/deleter/processor.py` & `logprep-6.1.0/logprep/processor/deleter/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/processor/deleter/rule.py` & `logprep-6.1.0/logprep/processor/deleter/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/processor/dissector/processor.py` & `logprep-6.1.0/logprep/processor/dissector/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
                 current_field = source_field
                 loop_content = get_dotted_field_value(event, current_field)
                 if loop_content is None:
                     error = BaseException(
                         f"dissector: mapping field '{source_field}' does not exist"
                     )
                     self._handle_warning_error(event, rule, error)
-            if delimeter is not None:
+            if delimeter is not None and loop_content is not None:
                 content, _, loop_content = loop_content.partition(delimeter)
             else:
                 content = loop_content
             if target_field.startswith("?"):
                 target_field_mapping[target_field.lstrip("?")] = content
                 target_field = content
                 content = ""
```

### Comparing `logprep-6.0.0/logprep/processor/dissector/rule.py` & `logprep-6.1.0/logprep/processor/dissector/rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,19 +77,19 @@
 .. datatemplate:import-module:: tests.unit.processor.dissector.test_dissector
    :template: testcase-renderer.tmpl
 
 """
 import re
 from typing import Callable, List, Tuple
 
-from attrs import define, validators, field, Factory
+from attrs import define, field, validators
 
 from logprep.filter.expression.filter_expression import FilterExpression
 from logprep.processor.field_manager.rule import FieldManagerRule
-from logprep.util.helper import append, add_and_overwrite
+from logprep.util.helper import add_and_overwrite, append
 
 START = r"%\{"
 END = r"\}"
 VALID_TARGET_FIELD = r"[^\}\%\{\}\+\/\|]*"
 APPEND_WITH_SEPERATOR = r"(\+\([^%]+\))"
 APPEND_WITHOUT_SEPERATOR = r"(\+(?!\([^%]))"
 INDIRECT_FIELD_NOTATION = r"([&\?]))"
@@ -104,14 +104,16 @@
 TARGET_FIELD = r"(?P<target_field>[^\/\|]*)"
 POSITION = r"(\/(?P<position>\d*))?"
 DATATYPE = r"(\|(?P<datatype>int|float|bool))?"
 SECTION_MATCH = (
     rf"{START}{ACTION}{SEPERATOR}{TARGET_FIELD}{POSITION}{DATATYPE}{END}(?P<delimeter>.*)"
 )
 
+MAPPING_VALIDATION_REGEX = re.compile(rf"^({DELIMETER})?({DISSECT}{DELIMETER})+({DISSECT})?$")
+
 
 def _do_nothing(*_):
     return
 
 
 def str_to_bool(input_str: str) -> bool:
     """converts an input string to bool by meaning"""
@@ -127,48 +129,47 @@
 class DissectorRule(FieldManagerRule):
     """dissector rule"""
 
     @define(kw_only=True)
     class Config(FieldManagerRule.Config):
         """Config for Dissector"""
 
-        source_fields: list = field(factory=list)
-        target_field: str = field(default="")
+        source_fields: list = field(factory=list, init=False)
+        target_field: str = field(default="", init=False)
 
         mapping: dict = field(
             validator=[
                 validators.instance_of(dict),
                 validators.deep_mapping(
                     key_validator=validators.instance_of(str),
-                    value_validator=validators.matches_re(
-                        rf"^({DELIMETER})?({DISSECT}{DELIMETER})+({DISSECT})?$"
-                    ),
+                    value_validator=validators.matches_re(MAPPING_VALIDATION_REGEX),
                 ),
             ],
-            default=Factory(dict),
+            factory=dict,
         )
         """A mapping from source fields to a dissect pattern [optional].
         Dotted field notation is possible in key and in the dissect pattern.
         """
         convert_datatype: dict = field(
             validator=[
                 validators.instance_of(dict),
                 validators.deep_mapping(
                     key_validator=validators.instance_of(str),
                     value_validator=validators.in_(["float", "int", "bool", "string"]),
                 ),
             ],
-            default=Factory(dict),
+            factory=dict,
         )
         """A mapping from source field and desired datatype [optional].
         The datatypes could be :code:`float`, :code:`int`, :code:`bool`, :code:`string`
         """
 
         def __attrs_post_init__(self):
             self.source_fields = list(self.mapping.keys())  # pylint: disable=no-member
+            super().__attrs_post_init__()
 
     _actions_mapping: dict = {
         None: add_and_overwrite,
         "+": append,
     }
 
     _converter_mapping: dict = {"int": int, "float": float, "string": str, "bool": str_to_bool}
```

### Comparing `logprep-6.0.0/logprep/processor/domain_label_extractor/processor.py` & `logprep-6.1.0/logprep/processor/domain_label_extractor/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from pathlib import Path
 from typing import Optional
 
 from attr import define, field, validators
 from tldextract import TLDExtract
 
 from logprep.abc.processor import Processor
-from logprep.processor.base.exceptions import DuplicationError
+from logprep.processor.base.exceptions import FieldExistsWarning
 from logprep.processor.domain_label_extractor.rule import DomainLabelExtractorRule
 from logprep.util.getter import GetterFactory
 from logprep.util.helper import add_field_to, get_dotted_field_value
 from logprep.util.validators import list_of_urls_validator
 
 
 class DomainLabelExtractor(Processor):
@@ -124,15 +124,15 @@
             for label, value in labels_dict.items():
                 output_field = f"{rule.target_field}.{label}"
                 add_successful = add_field_to(
                     event, output_field, value, overwrite_output_field=rule.overwrite_target
                 )
 
                 if not add_successful:
-                    raise DuplicationError(self.name, [output_field])
+                    raise FieldExistsWarning(self, rule, event, [output_field])
         else:
             tagging_field.append(f"invalid_domain_in_{rule.source_fields[0].replace('.', '_')}")
             event[self._config.tagging_field_name] = tagging_field
 
     @staticmethod
     def _is_valid_ip(domain):
         try:
```

### Comparing `logprep-6.0.0/logprep/processor/domain_label_extractor/rule.py` & `logprep-6.1.0/logprep/processor/domain_label_extractor/rule.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,15 +46,13 @@
             "registered_domain": "domain.de",
             "top_level_domain": "de",
             "subdomain": "www.sub"
         }
     }
 
 """
-import warnings
 
 from logprep.processor.field_manager.rule import FieldManagerRule
-from logprep.util.helper import pop_dotted_field_value, add_and_overwrite
 
 
 class DomainLabelExtractorRule(FieldManagerRule):
     """Check if documents match a filter."""
```

### Comparing `logprep-6.0.0/logprep/processor/domain_resolver/processor.py` & `logprep-6.1.0/logprep/processor/domain_resolver/processor.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,32 +22,31 @@
         max_cached_domains: 20000
         max_caching_days: 1
         hash_salt: secure_salt
         cache_enabled: true
         debug_cache: false
 """
 import datetime
-from pathlib import Path
 import socket
 from functools import cached_property
 from logging import Logger
 from multiprocessing import context, current_process
 from multiprocessing.pool import ThreadPool
+from pathlib import Path
 from typing import Optional
 
 from attr import define, field, validators
 from tldextract import TLDExtract
 
 from logprep.abc.processor import Processor
-from logprep.processor.base.exceptions import DuplicationError
 from logprep.processor.domain_resolver.rule import DomainResolverRule
 from logprep.util.cache import Cache
 from logprep.util.getter import GetterFactory
 from logprep.util.hasher import SHA256Hasher
-from logprep.util.helper import add_field_to, get_dotted_field_value
+from logprep.util.helper import get_dotted_field_value
 from logprep.util.validators import list_of_urls_validator
 
 
 class DomainResolver(Processor):
     """Resolve domains."""
 
     @define(kw_only=True)
@@ -151,16 +150,14 @@
                 list_path.write_bytes(GetterFactory.from_string(tld_list).get_raw())
                 downloaded_tld_lists_paths.append(f"file://{str(list_path.absolute())}")
             self._config.tld_lists = downloaded_tld_lists_paths
             self._logger.debug("finished tldlists download...")
 
     def _apply_rules(self, event, rule):
         source_field = rule.source_fields[0]
-        target_field = rule.target_field
-        overwrite_target = rule.overwrite_target
         domain_or_url_str = get_dotted_field_value(event, source_field)
         if not domain_or_url_str:
             return
         domain = self._tld_extractor(domain_or_url_str).fqdn
         if not domain:
             return
         self.metrics.total_urls += 1
@@ -170,33 +167,24 @@
             if requires_storing:
                 resolved_ip = self._resolve_ip(domain, hash_string)
                 self._domain_ip_map.update({hash_string: resolved_ip})
                 self.metrics.resolved_new += 1
             else:
                 resolved_ip = self._domain_ip_map.get(hash_string)
                 self.metrics.resolved_cached += 1
-            self._add_resolve_infos_to_event(
-                event, rule, target_field, resolved_ip, overwrite_target
-            )
+            self._add_resolve_infos_to_event(event, rule, resolved_ip)
             if self._config.debug_cache:
                 self._store_debug_infos(event, requires_storing)
         else:
             resolved_ip = self._resolve_ip(domain)
-            self._add_resolve_infos_to_event(
-                event, rule, target_field, resolved_ip, overwrite_target
-            )
+            self._add_resolve_infos_to_event(event, rule, resolved_ip)
 
-    def _add_resolve_infos_to_event(self, event, _, output_field, resolved_ip, overwrite_target):
+    def _add_resolve_infos_to_event(self, event, rule, resolved_ip):
         if resolved_ip:
-            adding_was_successful = add_field_to(
-                event, output_field, resolved_ip, overwrite_output_field=overwrite_target
-            )
-
-            if not adding_was_successful:
-                raise DuplicationError(self.name, [output_field])
+            self._write_target_field(event, rule, resolved_ip)
 
     def _resolve_ip(self, domain, hash_string=None):
         try:
             result = self._thread_pool.apply_async(socket.gethostbyname, (domain,))
             resolved_ip = result.get(timeout=self._config.timeout)
             return resolved_ip
         except (context.TimeoutError, OSError):
```

### Comparing `logprep-6.0.0/logprep/processor/domain_resolver/rule.py` & `logprep-6.1.0/logprep/processor/domain_resolver/rule.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,18 +17,17 @@
     :caption: Example
 
       filter: url
       domain_resolver:
         source_fields: [url]
       description: '...'
 """
-import warnings
 from attrs import define, field, fields
+
 from logprep.processor.field_manager.rule import FieldManagerRule
-from logprep.util.helper import pop_dotted_field_value, add_and_overwrite
 
 
 class DomainResolverRule(FieldManagerRule):
     """Check if documents match a filter."""
 
     @define(kw_only=True)
     class Config(FieldManagerRule.Config):
```

### Comparing `logprep-6.0.0/logprep/processor/dropper/processor.py` & `logprep-6.1.0/logprep/processor/dropper/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/processor/dropper/rule.py` & `logprep-6.1.0/logprep/processor/dropper/rule.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,33 +39,38 @@
         "keep_me": {
             "keep_me_too": "something"
         }
     }]
 """
 
 from typing import List
-import warnings
+
 from attrs import define, field, validators
 
 from logprep.processor.base.rule import Rule
-from logprep.util.helper import pop_dotted_field_value, add_and_overwrite
+from logprep.util.helper import get_dotted_field_value
 
 
 class DropperRule(Rule):
     """Check if documents match a filter."""
 
     @define(kw_only=True)
     class Config(Rule.Config):
         """RuleConfig for DropperRule"""
 
         drop: list = field(validator=validators.instance_of(list))
         """List of fields to drop"""
         drop_full: bool = field(validator=validators.instance_of(bool), default=True)
         """Drop recursive? defaults to [True]"""
 
+        def __attrs_post_init__(self):
+            # to ensure no split operations during processing
+            for dotted_field in self.drop:  # pylint: disable=not-an-iterable
+                get_dotted_field_value({}, dotted_field)
+
     @property
     def fields_to_drop(self) -> List[str]:
         """Returns fields_to_drop"""
         return self._config.drop
 
     @property
     def drop_full(self) -> bool:
```

### Comparing `logprep-6.0.0/logprep/processor/field_manager/processor.py` & `logprep-6.1.0/logprep/processor/field_manager/processor.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,51 +16,52 @@
     - fieldmanagername:
         type: field_manager
         specific_rules:
             - tests/testdata/rules/specific/
         generic_rules:
             - tests/testdata/rules/generic/
 """
-from typing import List, Tuple, Any
+from typing import Any, List, Tuple
 
 from logprep.abc.processor import Processor
-from logprep.processor.base.exceptions import DuplicationError
+from logprep.processor.base.exceptions import FieldExistsWarning
 from logprep.processor.field_manager.rule import FieldManagerRule
-from logprep.util.helper import get_dotted_field_value, add_field_to, add_and_overwrite
+from logprep.util.helper import add_and_overwrite, add_field_to, get_dotted_field_value
 
 
 class FieldManager(Processor):
     """A processor that copies, moves or merges source fields to one target field"""
 
     rule_class = FieldManagerRule
 
     def _apply_rules(self, event, rule):
         source_fields = rule.source_fields
         target_field = rule.target_field
         field_values = self._get_field_values(event, rule)
-        self._check_for_missing_fields(event, rule, source_fields, field_values)
+        if self._has_missing_fields(event, rule, source_fields, field_values):
+            return
         extend_target_list = rule.extend_target_list
         overwrite_target = rule.overwrite_target
         args = (event, target_field, field_values)
         if extend_target_list and overwrite_target:
             self._overwrite_with_list_from_source_field_values(*args)
         if extend_target_list and not overwrite_target:
             self._overwrite_with_list_from_source_field_values_include_target_field_value(*args)
         if not extend_target_list and overwrite_target:
             self._overwrite_target_with_source_field_values(*args)
         if not extend_target_list and not overwrite_target:
-            self._add_field_to(*args)
+            self._add_field_to(*args, rule=rule)
 
-    def _add_field_to(self, *args):
+    def _add_field_to(self, *args, rule):
         event, target_field, field_values = args
         if len(field_values) == 1:
             field_values = field_values.pop()
         successful = add_field_to(event, target_field, field_values, False, False)
         if not successful:
-            raise DuplicationError(self.name, [target_field])
+            raise FieldExistsWarning(self, rule, event, [target_field])
 
     def _overwrite_target_with_source_field_values(self, event, target_field, field_values):
         if len(field_values) == 1:
             field_values = field_values.pop()
         add_and_overwrite(event, target_field, field_values)
 
     def _overwrite_with_list_from_source_field_values_include_target_field_value(self, *args):
@@ -72,18 +73,20 @@
 
     def _overwrite_with_list_from_source_field_values(self, *args):
         event, target_field, field_values = args
         lists, other = self._separate_lists_form_other_types(field_values)
         target_field_value = self._get_deduplicated_sorted_flatten_list(lists, other)
         add_and_overwrite(event, target_field, target_field_value)
 
-    def _check_for_missing_fields(self, event, rule, source_fields, field_values):
+    def _has_missing_fields(self, event, rule, source_fields, field_values):
         if None in field_values:
             error = self._get_missing_fields_error(source_fields, field_values)
             self._handle_warning_error(event, rule, error)
+            return True
+        return False
 
     def _get_field_values(self, event, rule):
         return [get_dotted_field_value(event, source_field) for source_field in rule.source_fields]
 
     def _get_missing_fields_error(self, source_fields, field_values):
         missing_fields = [key for key, value in zip(source_fields, field_values) if value is None]
         error = BaseException(f"{self.name}: missing source_fields: {missing_fields}")
```

### Comparing `logprep-6.0.0/logprep/processor/field_manager/rule.py` & `logprep-6.1.0/logprep/processor/field_manager/rule.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,15 +76,17 @@
 ------------------------------------------------
 
 .. datatemplate:import-module:: tests.unit.processor.field_manager.test_field_manager
    :template: testcase-renderer.tmpl
 
 """
 from attrs import define, field, validators
+
 from logprep.processor.base.rule import Rule
+from logprep.util.helper import get_dotted_field_value
 
 FIELD_PATTERN = r"\$\{([+&?]?[^${}]*)\}"
 
 
 class FieldManagerRule(Rule):
     """Interface for a simple Rule with source_fields and target_field"""
 
@@ -109,14 +111,20 @@
         extend_target_list: bool = field(validator=validators.instance_of(bool), default=False)
         """If the target field exists and is a list, the list will be extended with the values
         of the source fields. If the source field is a list, the lists will be merged.
         If the target field does not exist, a new field will be added with the
         source field value as list. Defaults to :code:`False`.
         """
 
+        def __attrs_post_init__(self):
+            # ensures no split operations during processing
+            for dotted_field in self.source_fields:  # pylint: disable=not-an-iterable
+                get_dotted_field_value({}, dotted_field)
+            get_dotted_field_value({}, self.target_field)
+
     # pylint: disable=missing-function-docstring
     @property
     def delete_source_fields(self):
         if hasattr(self, "_config"):
             return self._config.delete_source_fields
         return False
```

### Comparing `logprep-6.0.0/logprep/processor/generic_adder/mysql_connector.py` & `logprep-6.1.0/logprep/processor/generic_adder/mysql_connector.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/processor/generic_adder/rule.py` & `logprep-6.1.0/logprep/processor/generic_adder/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/processor/generic_resolver/processor.py` & `logprep-6.1.0/logprep/processor/generic_resolver/processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         generic_rules:
             - tests/testdata/rules/generic/
 """
 import re
 from logging import Logger
 
 from logprep.abc.processor import Processor
-from logprep.processor.base.exceptions import DuplicationError
+from logprep.processor.base.exceptions import FieldExistsWarning
 from logprep.processor.generic_resolver.rule import GenericResolverRule
 from logprep.util.getter import GetterFactory
 from logprep.util.helper import get_dotted_field_value
 
 
 class GenericResolverError(BaseException):
     """Base class for GenericResolver related exceptions."""
@@ -109,15 +109,15 @@
                         if isinstance(event[key], dict):
                             event = event[key]
                         else:
                             conflicting_fields.append(keys[idx])
                     break
 
         if conflicting_fields:
-            raise DuplicationError(self.name, conflicting_fields)
+            raise FieldExistsWarning(self, rule, event, conflicting_fields)
 
     def ensure_rules_from_file(self, rule):
         """loads rules from file"""
         if rule.resolve_from_file:
             if rule.resolve_from_file["path"] not in self._replacements_from_file:
                 try:
                     add_dict = GetterFactory.from_string(rule.resolve_from_file["path"]).get_yaml()
```

### Comparing `logprep-6.0.0/logprep/processor/generic_resolver/rule.py` & `logprep-6.1.0/logprep/processor/generic_resolver/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/processor/geoip_enricher/processor.py` & `logprep-6.1.0/logprep/processor/geoip_enricher/processor.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,26 +14,26 @@
             - tests/testdata/geoip_enricher/rules/
         generic_rules:
             - tests/testdata/geoip_enricher/rules/
         db_path: /path/to/GeoLite2-City.mmdb
 """
 from functools import cached_property
 from ipaddress import ip_address
-from pathlib import Path
 from multiprocessing import current_process
+from pathlib import Path
 
 from attr import define, field, validators
 from geoip2 import database
 from geoip2.errors import AddressNotFoundError
 
 from logprep.abc.processor import Processor
-from logprep.processor.base.exceptions import DuplicationError
-from logprep.processor.geoip_enricher.rule import GeoipEnricherRule, GEOIP_DATA_STUBS
-from logprep.util.helper import add_field_to, get_dotted_field_value
+from logprep.processor.base.exceptions import FieldExistsWarning, ProcessingWarning
+from logprep.processor.geoip_enricher.rule import GEOIP_DATA_STUBS, GeoipEnricherRule
 from logprep.util.getter import GetterFactory
+from logprep.util.helper import add_field_to, get_dotted_field_value
 
 
 class GeoipEnricher(Processor):
     """Resolve values in documents by referencing a mapping list."""
 
     @define(kw_only=True)
     class Config(Processor.Config):
@@ -66,38 +66,50 @@
             self._logger.debug("finished geoip database download.")
             self._config.db_path = str(db_path_file.absolute())
 
     def _try_getting_geoip_data(self, ip_string):
         try:
             ip_addr = str(ip_address(ip_string))
             ip_data = self._city_db.city(ip_addr)
+
             geoip_data = GEOIP_DATA_STUBS.copy()
-            geoip_data.update(
-                {
-                    "geometry.coordinates": [
-                        ip_data.location.longitude,
-                        ip_data.location.latitude,
-                    ],
-                    "properties.accuracy_radius": ip_data.location.accuracy_radius,
-                    "properties.continent": ip_data.continent.name,
-                    "properties.continent_code": ip_data.continent.code,
-                    "properties.country": ip_data.country.name,
-                    "properties.country_iso_code": ip_data.country.iso_code,
-                    "properties.time_zone": ip_data.location.time_zone,
-                    "properties.city": ip_data.city.name,
-                    "properties.postal_code": ip_data.postal.code,
-                    "properties.subdivision": ip_data.subdivisions.most_specific.name,
-                }
-            )
+
+            geoip_data |= {
+                "properties.accuracy_radius": ip_data.location.accuracy_radius,
+                "properties.continent": ip_data.continent.name,
+                "properties.continent_code": ip_data.continent.code,
+                "properties.country": ip_data.country.name,
+                "properties.country_iso_code": ip_data.country.iso_code,
+                "properties.time_zone": ip_data.location.time_zone,
+                "properties.city": ip_data.city.name,
+                "properties.postal_code": ip_data.postal.code,
+                "properties.subdivision": ip_data.subdivisions.most_specific.name,
+            }
+
+            if ip_data.location.longitude and ip_data.location.latitude:
+                geoip_data.update(
+                    {
+                        "geometry.type": "Point",
+                        "geometry.coordinates": [
+                            ip_data.location.longitude,
+                            ip_data.location.latitude,
+                        ],
+                    }
+                )
+
             return geoip_data
         except (ValueError, AddressNotFoundError):
             return {}
 
     def _apply_rules(self, event, rule):
         ip_string = get_dotted_field_value(event, rule.source_fields[0])
+        if ip_string is None:
+            raise ProcessingWarning(
+                self, f"Value of IP field '{rule.source_fields[0]}' is 'None'", rule, event
+            )
         geoip_data = self._try_getting_geoip_data(ip_string)
         if not geoip_data:
             return
         for target_subfield, value in geoip_data.items():
             if value is None:
                 continue
             full_output_field = f"{rule.target_field}.{target_subfield}"
@@ -107,8 +119,8 @@
                 event=event,
                 output_field=full_output_field,
                 content=value,
                 extends_lists=False,
                 overwrite_output_field=rule.overwrite_target,
             )
             if not adding_was_successful:
-                raise DuplicationError(self.name, [full_output_field])
+                raise FieldExistsWarning(self, rule, event, [full_output_field])
```

### Comparing `logprep-6.0.0/logprep/processor/geoip_enricher/rule.py` & `logprep-6.1.0/logprep/processor/geoip_enricher/rule.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,26 +15,22 @@
     :caption: Example
 
     filter: client.ip
     geoip:
       source_fields: [client.ip]
     description: '...'
 """
-
-import warnings
-
 from attr import Factory
 from attrs import define, field, validators
 
 from logprep.processor.field_manager.rule import FieldManagerRule
-from logprep.util.helper import add_and_overwrite, pop_dotted_field_value
 
 GEOIP_DATA_STUBS = {
     "type": "Feature",
-    "geometry.type": "Point",
+    "geometry.type": None,
     "geometry.coordinates": None,
     "properties.accuracy_radius": None,
     "properties.continent": None,
     "properties.continent_code": None,
     "properties.country": None,
     "properties.country_iso_code": None,
     "properties.time_zone": None,
```

### Comparing `logprep-6.0.0/logprep/processor/hyperscan_resolver/processor.py` & `logprep-6.1.0/logprep/processor/hyperscan_resolver/processor.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,32 +19,27 @@
         generic_rules:
             - tests/testdata/rules/generic/
         hyperscan_db_path: tmp/path/scan.db
 """
 
 import errno
 from logging import Logger
-from os import path, makedirs
-from typing import Tuple, Any, Dict
+from os import makedirs, path
+from typing import Any, Dict, Tuple
+
 from attr import define, field
 
 from logprep.abc.processor import Processor
-from logprep.processor.base.exceptions import SkipImportError, DuplicationError
-from logprep.util.validators import directory_validator
+from logprep.processor.base.exceptions import FieldExistsWarning, SkipImportError
 from logprep.util.helper import get_dotted_field_value
+from logprep.util.validators import directory_validator
 
 # pylint: disable=no-name-in-module
 try:
-    from hyperscan import (
-        Database,
-        HS_FLAG_SINGLEMATCH,
-        HS_FLAG_CASELESS,
-        loadb,
-        dumpb,
-    )
+    from hyperscan import HS_FLAG_CASELESS, HS_FLAG_SINGLEMATCH, Database, dumpb, loadb
 except ModuleNotFoundError as error:  # pragma: no cover
     raise SkipImportError("hyperscan_resolver") from error
 
 # pylint: enable=no-name-in-module
 
 # pylint: disable=ungrouped-imports
 from logprep.processor.hyperscan_resolver.rule import HyperscanResolverRule
@@ -133,15 +128,15 @@
                         has_conflict = self._try_adding_value_to_existing_field(
                             dict_, dotted_key_part, resolved_value, rule
                         )
 
                     if has_conflict:
                         conflicting_fields.append(split_dotted_keys[idx])
         if conflicting_fields:
-            raise DuplicationError(self.name, conflicting_fields)
+            raise FieldExistsWarning(self, rule, event, conflicting_fields)
 
     @staticmethod
     def _try_adding_value_to_existing_field(
         dict_: dict, dotted_key_part: str, resolved_value: str, rule: HyperscanResolverRule
     ) -> bool:
         current_value = dict_[dotted_key_part]
         if rule.append_to_list and isinstance(current_value, list):
```

### Comparing `logprep-6.0.0/logprep/processor/hyperscan_resolver/rule.py` & `logprep-6.1.0/logprep/processor/hyperscan_resolver/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/processor/ip_informer/processor.py` & `logprep-6.1.0/logprep/processor/ip_informer/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,20 +13,20 @@
     - myipinformer:
         type: ip_informer
         specific_rules:
             - tests/testdata/rules/specific/
         generic_rules:
             - tests/testdata/rules/generic/
 """
-from functools import partial
 import ipaddress
+from functools import partial
 from itertools import chain
 from typing import Iterable
-from logprep.processor.base.exceptions import ProcessingWarning
 
+from logprep.processor.base.exceptions import ProcessingWarning
 from logprep.processor.field_manager.processor import FieldManager
 from logprep.processor.ip_informer.rule import IpInformerRule, get_ip_property_names
 from logprep.util.helper import get_dotted_field_value
 
 
 class IpInformer(FieldManager):
     """A processor that enriches ip information"""
@@ -40,15 +40,15 @@
     def _apply_rules(self, event: dict, rule: IpInformerRule) -> None:
         self._processing_warnings = []
         ip_address_list = self._get_flat_ip_address_list(event, rule)
         results = self._get_results(ip_address_list, rule)
         if results:
             self._write_target_field(event, rule, results)
         for msg, error in self._processing_warnings:
-            raise ProcessingWarning(msg) from error
+            raise ProcessingWarning(self, msg, rule, event) from error
 
     def _get_results(self, ip_address_list: Iterable, rule: IpInformerRule) -> dict:
         results = [(ip, self._ip_properties(ip, rule)) for ip in ip_address_list]
         return dict(filter(lambda x: bool(x[1]), results))
 
     def _get_flat_ip_address_list(self, event: dict, rule: IpInformerRule) -> Iterable:
         source_field_values = list(map(partial(get_dotted_field_value, event), rule.source_fields))
```

### Comparing `logprep-6.0.0/logprep/processor/ip_informer/rule.py` & `logprep-6.1.0/logprep/processor/ip_informer/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/processor/key_checker/processor.py` & `logprep-6.1.0/logprep/processor/key_checker/processor.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,19 +16,19 @@
             - tests/testdata/rules/specific/
         generic_rules:
             - tests/testdata/rules/generic/
 
 """
 
 from typing import Iterable
+
 from logprep.abc.processor import Processor
 from logprep.processor.base.rule import Rule
 from logprep.processor.key_checker.rule import KeyCheckerRule
-from logprep.util.helper import add_field_to, get_dotted_field_value
-from logprep.processor.base.exceptions import DuplicationError
+from logprep.util.helper import get_dotted_field_value
 
 
 class KeyChecker(Processor):
     """Checks if all keys of a given List are in the event"""
 
     rule_class: Rule = KeyCheckerRule
 
@@ -47,17 +47,8 @@
         output_value = get_dotted_field_value(event, rule.target_field)
 
         if isinstance(output_value, Iterable):
             output_value = list({*not_existing_fields, *output_value})
         else:
             output_value = not_existing_fields
 
-        add_successful = add_field_to(
-            event,
-            rule.target_field,
-            sorted(output_value),
-            extends_lists=False,
-            overwrite_output_field=rule.overwrite_target,
-        )
-
-        if not add_successful:
-            raise DuplicationError(self.name, [rule.target_field])
+        self._write_target_field(event, rule, sorted(output_value))
```

### Comparing `logprep-6.0.0/logprep/processor/key_checker/rule.py` & `logprep-6.1.0/logprep/processor/key_checker/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/processor/labeler/labeling_schema.py` & `logprep-6.1.0/logprep/processor/labeler/labeling_schema.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/processor/labeler/processor.py` & `logprep-6.1.0/logprep/processor/labeler/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/processor/labeler/rule.py` & `logprep-6.1.0/logprep/processor/labeler/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/processor/list_comparison/processor.py` & `logprep-6.1.0/logprep/processor/list_comparison/processor.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         list_search_base_path: /path/to/list/dir
 """
 from logging import Logger
 
 from attr import define, field, validators
 
 from logprep.abc.processor import Processor
-from logprep.processor.base.exceptions import DuplicationError
+from logprep.processor.base.exceptions import FieldExistsWarning
 from logprep.processor.list_comparison.rule import ListComparisonRule
 from logprep.util.helper import add_field_to, get_dotted_field_value
 
 
 class ListComparisonError(BaseException):
     """Base class for ListComparison related exceptions."""
 
@@ -78,15 +78,15 @@
 
         comparison_result, comparison_key = self._list_comparison(rule, event)
 
         if comparison_result is not None:
             output_field = f"{ rule.target_field }.{ comparison_key }"
             field_possible = add_field_to(event, output_field, comparison_result, True)
             if not field_possible:
-                raise DuplicationError(self.name, [output_field])
+                raise FieldExistsWarning(self, rule, event, [output_field])
 
     def _list_comparison(self, rule: ListComparisonRule, event: dict):
         """
         Check if field value violates block or allow list.
         Returns the result of the comparison (res_key), as well as a dictionary containing
         the result (key) and a list of filenames pertaining to said result (value).
         """
```

### Comparing `logprep-6.0.0/logprep/processor/list_comparison/rule.py` & `logprep-6.1.0/logprep/processor/list_comparison/rule.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,23 +33,21 @@
 .. note::
 
     Currently it is not possible to check in more than one source_field per rule
 
 """
 import os.path
 from string import Template
-import warnings
 from typing import List, Optional
 
 from attrs import define, field, validators
 
 from logprep.filter.expression.filter_expression import FilterExpression
 from logprep.processor.field_manager.rule import FieldManagerRule
 from logprep.util.getter import GetterFactory
-from logprep.util.helper import pop_dotted_field_value, add_and_overwrite
 
 
 class ListComparisonRule(FieldManagerRule):
     """Check if documents match a filter."""
 
     _compare_sets: dict
```

### Comparing `logprep-6.0.0/logprep/processor/normalizer/processor.py` & `logprep-6.1.0/logprep/processor/normalizer/processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,33 +32,35 @@
 from functools import reduce
 from logging import Logger
 from pathlib import Path
 from time import time
 from typing import List, Optional, Tuple, Union
 
 import arrow
+import msgspec
 from attr import define, field, validators
 from dateutil import parser
 from filelock import FileLock
 from pytz import timezone
 
 from logprep.abc.processor import Processor
-from logprep.processor.base.exceptions import DuplicationError
+from logprep.processor.base.exceptions import FieldExistsWarning, ProcessingWarning
 from logprep.processor.normalizer.rule import NormalizerRule
 from logprep.util.getter import GetterFactory
-from logprep.util.helper import add_field_to, get_dotted_field_value
+from logprep.util.helper import (
+    add_field_to,
+    get_dotted_field_list,
+    get_dotted_field_value,
+)
 from logprep.util.validators import directory_validator
 
 
-class NormalizerError(BaseException):
+class NormalizerError(ProcessingWarning):
     """Base class for Normalizer related exceptions."""
 
-    def __init__(self, name: str, message: str):
-        super().__init__(f"Normalizer ({name}): {message}")
-
 
 class Normalizer(Processor):
     """Normalize log events by copying specific values to standardized fields."""
 
     @define(kw_only=True)
     class Config(Processor.Config):
         """config description for Normalizer"""
@@ -105,14 +107,16 @@
     _regex_mapping: str
 
     _html_replace_fields: str
 
     _conflicting_fields: list
 
     rule_class = NormalizerRule
+    _encoder = msgspec.json.Encoder()
+    _decoder = msgspec.json.Decoder()
 
     def __init__(self, name: str, configuration: Processor.Config, logger: Logger):
         self._event = None
         self._conflicting_fields = []
 
         self._regex_mapping = configuration.regex_mapping
         self._html_replace_fields = configuration.html_replace_fields
@@ -159,15 +163,15 @@
         file_name = f"{current_date}_{weekday}.json"
         file_path = os.path.join(self._grok_matches_path, file_name)
         Path(self._grok_matches_path).mkdir(parents=True, exist_ok=True)
         with FileLock(self._file_lock_path):
             json_dict = {}
             if os.path.isfile(file_path):
                 with open(file_path, "r", encoding="utf8") as grok_json_file:
-                    json_dict = json.load(grok_json_file)
+                    json_dict = self._decoder.decode(grok_json_file.read())
 
             for key, value in self._grok_pattern_matches.items():
                 json_dict[key] = json_dict.get(key, 0) + value
                 self._grok_pattern_matches[key] = 0
 
             with open(file_path, "w", encoding="utf8") as grok_json_file:
                 json_dict = dict(reversed(sorted(json_dict.items(), key=lambda items: items[1])))
@@ -188,49 +192,48 @@
             if matching_pattern:
                 substitution_pattern = target[2]
                 value = re.sub(matching_pattern, substitution_pattern, value)
             target = target[0]
         return target, value
 
     def _add_field(self, event: dict, dotted_field: str, value: Union[str, int]):
-        fields = dotted_field.split(".")
-        missing_fields = json.loads(json.dumps(fields))
-        for field in fields:
-            if isinstance(event, dict) and field in event:
-                event = event[field]
+        fields = get_dotted_field_list(dotted_field)
+        missing_fields = self._decoder.decode(self._encoder.encode(fields))
+        for event_field in fields:
+            if isinstance(event, dict) and event_field in event:
+                event = event[event_field]
                 missing_fields.pop(0)
             else:
                 break
         if not isinstance(event, dict):
             self._conflicting_fields.append(dotted_field)
             return
-        for field in missing_fields[:-1]:
-            event[field] = {}
-            event = event[field]
+        for event_field in missing_fields[:-1]:
+            event[event_field] = {}
+            event = event[event_field]
         event[missing_fields[-1]] = value
 
         if self._html_replace_fields and dotted_field in self._html_replace_fields:
             if self._has_html_entity(value):
                 event[missing_fields[-1] + "_decodiert"] = html.unescape(value)
 
     @staticmethod
     def _has_html_entity(value):
         return re.search("&#[0-9]{2,4};", value)
 
     @staticmethod
     def _replace_field(event: dict, dotted_field: str, value: str):
-        fields = dotted_field.split(".")
+        fields = get_dotted_field_list(dotted_field)
         reduce(lambda dict_, key: dict_[key], fields[:-1], event)[fields[-1]] = value
 
     def process(self, event: dict):
         self._conflicting_fields.clear()
         super().process(event)
         if self._count_grok_pattern_matches:
             self._write_grok_matches()
-        self._raise_warning_if_fields_already_existed()
 
     def _apply_rules(self, event, rule):
         """Normalizes Windows Event Logs.
 
         The rules in this function are applied on a first-come, first-serve basis: If a rule copies
         a source field to a normalized field and a subsequent rule tries to write the same
         normalized field, it will not be overwritten and a ProcessingWarning will be raised
@@ -239,14 +242,15 @@
         be written in a way that no such warnings are produced during normal operation because each
         warning should be an indicator of incorrect rules or unexpected/changed events.
         """
         self._apply_grok(event, rule)
         self._apply_timestamp_normalization(event, rule)
         for source_field, target_field in rule.substitutions.items():
             self._apply_field_copy(event, source_field, target_field)
+        self._raise_warning_if_fields_already_existed(rule, event)
 
     def _apply_grok(self, event: dict, rule: NormalizerRule):
         """
         Applies the grok pattern of a given NormalizerRule to a given event, by matching the field
         value against the grok pattern. If no pattern matches a grok failure field is written to the
         event (if configured).
         """
@@ -305,20 +309,22 @@
         """
         for source_field, normalization in rule.timestamps.items():
             source_timestamp = get_dotted_field_value(event, source_field)
             if source_timestamp is None:
                 continue
 
             timestamp_normalization = normalization.get("timestamp")
-            timestamp = self._transform_timestamp(source_timestamp, timestamp_normalization)
+            timestamp = self._transform_timestamp(
+                source_timestamp, timestamp_normalization, rule, event
+            )
             timestamp = self._convert_timezone(timestamp, timestamp_normalization)
             iso_timestamp = timestamp.isoformat().replace("+00:00", "Z")
             self._write_normalized_timestamp(event, iso_timestamp, timestamp_normalization)
 
-    def _transform_timestamp(self, source_timestamp, timestamp_normalization):
+    def _transform_timestamp(self, source_timestamp, timestamp_normalization, rule, event):
         source_timezone = timestamp_normalization["source_timezone"]
         timestamp = None
         format_parsed = False
         source_formats = timestamp_normalization["source_formats"]
         for source_format in source_formats:
             try:
                 if source_format == "ISO8601":
@@ -340,15 +346,15 @@
             except ValueError:
                 pass
         if not format_parsed:
             error_message = (
                 f"Could not parse source timestamp "
                 f"{source_timestamp}' with formats '{source_formats}'"
             )
-            raise NormalizerError(self.name, error_message)
+            raise NormalizerError(self, error_message, rule, event)
         return timestamp
 
     def _convert_timezone(self, timestamp, timestamp_normalization):
         source_timezone = timestamp_normalization["source_timezone"]
         destination_timezone = timestamp_normalization["destination_timezone"]
         time_zone = timezone(source_timezone)
         if not timestamp.tzinfo:
@@ -367,17 +373,17 @@
             self._try_add_field(event, normalization_target, iso_timestamp)
 
     def _apply_field_copy(self, event: dict, source_field: str, target_field: str):
         if self._field_exists(event, source_field):
             source_value = get_dotted_field_value(event, source_field)
             self._try_add_field(event, target_field, source_value)
 
-    def _raise_warning_if_fields_already_existed(self):
+    def _raise_warning_if_fields_already_existed(self, rule, event):
         if self._conflicting_fields:
-            raise DuplicationError(self.name, self._conflicting_fields)
+            raise FieldExistsWarning(self, rule, event, self._conflicting_fields)
 
     def shut_down(self):
         """
         Stop processing of this processor and finish outstanding actions.
         Optional: Called when stopping the pipeline
         """
         if self._count_grok_pattern_matches:
```

### Comparing `logprep-6.0.0/logprep/processor/normalizer/rule.py` & `logprep-6.1.0/logprep/processor/normalizer/rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+# pylint: disable=anomalous-backslash-in-string
 """
 Normalizer
 ==========
 
 The normalizer requires the additional field :code:`normalize`.
 It contains key-value pairs that define if and how fields gets normalized.
-The keys describe fields that are going to be normalized and the values describe the new normalized fields.
-Through normalizing, old fields are being copied to new fields, but the old fields are not deleted.
+The keys describe fields that are going to be normalized and the values describe the new
+normalized fields. Through normalizing, old fields are being copied to new fields, but the old
+fields are not deleted.
 
-In the following example the field :code:`event_data.ClientAddress` is normalized to :code:`client.ip`.
+In the following example the field :code:`event_data.ClientAddress` is normalized to
+:code:`client.ip`.
 
 ..  code-block:: yaml
     :linenos:
     :caption: Example
 
     filter: 'event_data.ClientAddress'
     normalize:
@@ -19,20 +22,23 @@
     description: '...'
 
 Extraction and Replacement
 --------------------------
 
 Instead of copying a whole field, it is possible to copy only parts of it via regex capture groups.
 These can be then extracted and rearranged in a new field.
-The groups are defined in a configurable file as keywords and can be referenced from within the rules via the Python regex syntax.
+The groups are defined in a configurable file as keywords and can be referenced from within the
+rules via the Python regex syntax.
 
 Instead of specifying a target field, a list with three elements has to be used.
-The first element is the target field, the second element is a regex keyword and the third field is a regex expression that defines how the value should be inserted into the new field.
+The first element is the target field, the second element is a regex keyword and the third field is
+a regex expression that defines how the value should be inserted into the new field.
 
-In the following example :code:`event_data.address_text: "The IP is 1.2.3.4 and the port is 1234!"` is normalized to :code:`address: "1.2.3.4:1234"`.
+In the following example :code:`event_data.address_text: "The IP is 1.2.3.4 and the port is 1234!"`
+is normalized to :code:`address: "1.2.3.4:1234"`.
 
 ..  code-block:: json
     :linenos:
     :caption: Example - Definition of regex keywords in the regex mapping file
 
     {
       "RE_IP_PORT_CAP": ".*(?P<IP>[\\d.]+).*(?P<PORT>\\d+).*",
@@ -58,17 +64,17 @@
 instead of them.
 By combining both types of normalization it is possible to perform transformations on results of
 Grok that can not be achieved by Grok alone.
 All Grok normalizations are always performed before other normalizations.
 An example for this is the creation of nested fields.
 
 The following example would normalize
-:code:`event_data.ip_and_port: "Linus has the address 1.2.3.4 1234", event_data.address_text: "This is an address: 1.2.3.4:1234"` to
-:code:`address.ip: "1.2.3.4"`, :code:`address.port: 1234`, :code:`name: Linus` and
-:code:`address.combined: 1.2.3.4 and 1234`.
+:code:`event_data.ip_and_port: "Linus has the address 1.2.3.4 1234", event_data.address_text:
+"This is an address: 1.2.3.4:1234"` to :code:`address.ip: "1.2.3.4"`, :code:`address.port: 1234`,
+:code:`name: Linus` and :code:`address.combined: 1.2.3.4 and 1234`.
 
 ..  code-block:: yaml
     :linenos:
     :caption: Example - Grok normalization and subsequent normalization of a result
 
       filter: event_id
       normalize:
@@ -96,16 +102,16 @@
         some_field_with_an_ip:
           grok:
             - '%{IP:ip_foo} %{NUMBER:port_foo:int} foo'
             - '%{IP:ip} %{NUMBER:port:int}'
 
 As Grok pattern are only applied when they match a given input string it is sometimes desired to
 know when none of the given pattern matches.
-This is helpful in identifying new, unknown or reconfigured log sources that are not correctly covered by the current
-rule set.
+This is helpful in identifying new, unknown or reconfigured log sources that are not correctly
+covered by the current rule set.
 To activate the output of this information it is required to add the field
 :code:`failure_target_field` to the grok rule.
 This will describe the output field where the grok failure should be written to.
 It can be a dotted field path.
 An example rule would look like:
 
 ..  code-block:: yaml
@@ -171,29 +177,30 @@
       }
     }
 
 Normalization of Timestamps
 ---------------------------
 
 There is a special functionality that allows to normalize timestamps.
-With this functionality different timestamp formats can be converted to ISO8601 and timezones can be adapted.
-Instead of giving a target field, the special field `timestamp` is used.
+With this functionality different timestamp formats can be converted to ISO8601 and timezones can
+be adapted. Instead of giving a target field, the special field `timestamp` is used.
 Under this field additional configurations for the normalization can be specified.
-Under `timestamp.source_formats` a list of possible source formats for the timestamp must be defined.
-The original timezone of the timestamp must be specified in `timestamp.source_timezone`.
+Under `timestamp.source_formats` a list of possible source formats for the timestamp must be
+defined. The original timezone of the timestamp must be specified in `timestamp.source_timezone`.
 Furthermore, in `timestamp.destination_timezone` the new timestamp must be specified.
-Finally, `timestamp.destination` defines the target field to which the new timestamp should be written.
-Optionally, it can be defined if the normalization is allowed to override existing values by setting `timestamp.allow_override` to `true` or `false`.
-It is allowed to override by default.
+Finally, `timestamp.destination` defines the target field to which the new timestamp should be
+written. Optionally, it can be defined if the normalization is allowed to override existing values
+by setting `timestamp.allow_override` to `true` or `false`. It is allowed to override by default.
 
 Valid formats for timestamps are defined by the notation of the Python datetime module.
-Additionally, the value `ISO8601` and `UNIX` can be used for the `source_formats` field. The former can be used if the
-timestamp already exists in the ISO98601 format, such that only a timezone conversion should be applied. And the latter
-can be used if the timestamp is given in the UNIX Epoch Time. This supports the Unix timestamps in seconds and
-milliseconds.
+Additionally, the value `ISO8601` and `UNIX` can be used for the `source_formats` field.
+The former can be used if the
+timestamp already exists in the ISO98601 format, such that only a timezone conversion should be
+applied. And the latter can be used if the timestamp is given in the UNIX Epoch Time. This supports
+the Unix timestamps in seconds and milliseconds.
 
 Valid timezones are defined in the pytz module:
 
 .. raw:: html
 
    <details>
    <summary><a>List of all timezones</a></summary>
@@ -779,15 +786,16 @@
    Zulu
 
 .. raw:: html
 
    </details>
    <br/>
 
-In the following example :code:`@timestamp: 2000 12 31 - 22:59:59` would be normalized to :code:`@timestamp: 2000-12-31T23:59:59+01:00`.
+In the following example :code:`@timestamp: 2000 12 31 - 22:59:59` would be normalized to
+:code:`@timestamp: 2000-12-31T23:59:59+01:00`.
 
 ..  code-block:: yaml
     :linenos:
     :caption: Example - Normalization of a timestamp
 
     filter: '@timestamp'
     normalize:
@@ -796,25 +804,27 @@
           destination: '@timestamp'
           source_formats:
           - '%Y %m %d - %H:%M:%S'
           source_timezone: 'UTC'
           destination_timezone: 'Europe/Berlin'
     description: 'Test-rule with matching auto-test'
 
-If Grok and a timestamp normalization is being used in the same rule, then Grok is being applied first,
-so that a time normalization can be performed on the Grok results.
+If Grok and a timestamp normalization is being used in the same rule,
+then Grok is being applied first, so that a time normalization can be performed
+on the Grok results.
 """
+# pylint: enable=anomalous-backslash-in-string
 
 import re
-from typing import Union, Dict, List
+from typing import Dict, List, Union
 
 from pygrok import Grok
 
 from logprep.filter.expression.filter_expression import FilterExpression
-from logprep.processor.base.rule import Rule, InvalidRuleDefinitionError
+from logprep.processor.base.rule import InvalidRuleDefinitionError, Rule
 
 GROK_DELIMITER = "__________________"
 
 
 class NormalizerRuleError(InvalidRuleDefinitionError):
     """Base class for Normalizer rule related exceptions."""
 
@@ -858,16 +868,16 @@
             patterns = [f"^{pattern}$" for pattern in patterns]
             self._grok_list = [Grok(pattern_item, **kwargs) for pattern_item in patterns]
 
         self._match_cnt_initialized = False
         self.failure_target_field = failure_target_field
 
     def __eq__(self, other: "GrokWrapper") -> bool:
-        return set([grok_item.regex_obj for grok_item in self._grok_list]) == set(
-            [grok_item.regex_obj for grok_item in other._grok_list]
+        return set(grok_item.regex_obj for grok_item in self._grok_list) == set(
+            grok_item.regex_obj for grok_item in other._grok_list
         )
 
     def match(self, text: str, pattern_matches: dict = None) -> Dict[str, str]:
         """Match string via grok using delimiter and count matches if enabled."""
         if pattern_matches is not None and not self._match_cnt_initialized:
             for grok in self._grok_list:
                 pattern_matches[grok.pattern] = 0
@@ -887,14 +897,15 @@
 
 class NormalizerRule(Rule):
     """Check if documents match a filter."""
 
     additional_grok_patterns = None
     extract_field_pattern = re.compile(r"%{(\w+):([\w\[\]]+)(?::\w+)?}")
     sub_fields_pattern = re.compile(r"(\[(\w+)\])")
+    failure_tags = ["_normalizer_failure"]
 
     # pylint: disable=super-init-not-called
     # TODO: this is not refactored, because this processor should be dissected
     def __init__(
         self, filter_rule: FilterExpression, normalizations: dict, description: str = None
     ):
         self.__class__.__hash__ = Rule.__hash__
@@ -925,24 +936,27 @@
     def _extract_grok_pattern(self, normalization, source_field):
         """Checks the rule file for grok pattern, reformats them and adds them to self._grok"""
         if isinstance(normalization["grok"], str):
             normalization["grok"] = [normalization["grok"]]
         for idx, grok in enumerate(normalization["grok"]):
             patterns = self.extract_field_pattern.findall(grok)
             self._reformat_grok_pattern(idx, normalization, patterns)
-            failure_target_field = normalization.get("failure_target_field")
-            self._grok.update(
-                {
-                    source_field: GrokWrapper(
-                        patterns=normalization["grok"],
-                        custom_patterns_dir=NormalizerRule.additional_grok_patterns,
-                        failure_target_field=failure_target_field,
-                    )
-                }
-            )
+        self._add_grok_patterns(normalization, source_field)
+
+    def _add_grok_patterns(self, normalization, source_field):
+        failure_target_field = normalization.get("failure_target_field")
+        self._grok.update(
+            {
+                source_field: GrokWrapper(
+                    patterns=normalization["grok"],
+                    custom_patterns_dir=NormalizerRule.additional_grok_patterns,
+                    failure_target_field=failure_target_field,
+                )
+            }
+        )
 
     def _reformat_grok_pattern(self, idx, normalization, patterns):
         """
         Changes the grok pattern format by removing the square brackets and introducing
         the GROK_DELIMITER.
         """
         for pattern in patterns:
```

### Comparing `logprep-6.0.0/logprep/processor/pre_detector/ip_alerter.py` & `logprep-6.1.0/logprep/processor/pre_detector/ip_alerter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/processor/pre_detector/processor.py` & `logprep-6.1.0/logprep/processor/pre_detector/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/processor/pre_detector/rule.py` & `logprep-6.1.0/logprep/processor/pre_detector/rule.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,15 @@
       mitre:
       - some_tag
       case_condition: directly
     description: Some malicous event.
     ip_fields:
     - some_ip_field
 """
-
+from functools import cached_property
 from typing import Union, Optional
 from attrs import define, field, validators, asdict
 
 from logprep.processor.base.rule import Rule
 
 
 class PreDetectorRule(Rule):
@@ -91,15 +91,15 @@
             [
                 super().__eq__(other),
                 self.ip_fields == other.ip_fields,
             ]
         )
 
     # pylint: disable=C0111
-    @property
+    @cached_property
     def detection_data(self) -> dict:
         detection_data = asdict(self._config)
         if self._config.link is None:
             del detection_data["link"]
         for special_field in Rule.special_field_types:
             detection_data.pop(special_field)
         return detection_data
```

### Comparing `logprep-6.0.0/logprep/processor/processor_strategy.py` & `logprep-6.1.0/logprep/processor/processor_strategy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 processor strategies module
 
 processor strategies are used to implement in one point how rules are processed in processors
 this could be the order of specific or generic rules
 """
 from abc import ABC, abstractmethod
+from functools import reduce
 from time import time
-from typing import Callable, TYPE_CHECKING
-
+from typing import TYPE_CHECKING, Callable
 
 if TYPE_CHECKING:  # pragma: no cover
     from logprep.abc.processor import Processor
     from logprep.framework.rule_tree.rule_tree import RuleTree
 
 
 class ProcessStrategy(ABC):
@@ -27,22 +27,25 @@
 
 class SpecificGenericProcessStrategy(ProcessStrategy):
     """
     Strategy to process rules in rule trees in the following order:
     specific_rules >> generic_rules
     """
 
+    def __init__(self, apply_multiple_times=False):
+        self._apply_multiple_times = apply_multiple_times
+
     def process(self, event: dict, **kwargs):
         specific_tree = kwargs.get("specific_tree")
         generic_tree = kwargs.get("generic_tree")
         callback = kwargs.get("callback")
         processor_metrics = kwargs.get("processor_metrics")
+        processor_metrics.number_of_processed_events += 1
         self._process_specific(event, specific_tree, callback, processor_metrics)
         self._process_generic(event, generic_tree, callback, processor_metrics)
-        processor_metrics.number_of_processed_events += 1
 
     def _process_specific(
         self,
         event: dict,
         specific_tree: "RuleTree",
         callback: Callable,
         processor_metrics: "Processor.ProcessorMetrics",
@@ -64,20 +67,25 @@
         self,
         event: dict,
         tree: "RuleTree",
         callback: Callable,
         processor_metrics: "Processor.ProcessorMetrics",
     ):
         applied_rules = set()
-        matching_rules = tree.get_matching_rules(event)
-        while True:
-            for rule in matching_rules:
-                begin = time()
-                callback(event, rule)
-                processing_time = time() - begin
-                rule.metrics._number_of_matches += 1
-                rule.metrics.update_mean_processing_time(processing_time)
-                processor_metrics.update_mean_processing_time_per_event(processing_time)
-                applied_rules.add(rule)
+
+        def _process_rule(event, rule):
+            begin = time()
+            callback(event, rule)
+            processing_time = time() - begin
+            rule.metrics._number_of_matches += 1
+            rule.metrics.update_mean_processing_time(processing_time)
+            processor_metrics.update_mean_processing_time_per_event(processing_time)
+            applied_rules.add(rule)
+            return event
+
+        if self._apply_multiple_times:
             matching_rules = tree.get_matching_rules(event)
-            if not set(matching_rules).difference(applied_rules):
-                break
+            while matching_rules:
+                reduce(_process_rule, (event, *matching_rules))
+                matching_rules = set(tree.get_matching_rules(event)).difference(applied_rules)
+        else:
+            reduce(_process_rule, (event, *tree.get_matching_rules(event)))
```

### Comparing `logprep-6.0.0/logprep/processor/pseudonymizer/encrypter.py` & `logprep-6.1.0/logprep/processor/pseudonymizer/encrypter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/processor/pseudonymizer/processor.py` & `logprep-6.1.0/logprep/processor/pseudonymizer/processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,27 +28,28 @@
         tld_lists:
             -/path/to/tld_list.dat
 """
 import datetime
 import re
 from functools import cached_property
 from logging import Logger
-from typing import Any, List, Optional, Tuple, Union
+from typing import Any, List, Optional, Tuple, Union, Pattern
 from urllib.parse import parse_qs
 
 from attr import define, field, validators
 from tldextract import TLDExtract
 from urlextract import URLExtract
 
 from logprep.abc.processor import Processor
 from logprep.processor.pseudonymizer.encrypter import DualPKCS1HybridEncrypter
 from logprep.processor.pseudonymizer.rule import PseudonymizerRule
 from logprep.util.cache import Cache
 from logprep.util.getter import GetterFactory
 from logprep.util.hasher import SHA256Hasher
+from logprep.util.helper import get_dotted_field_list
 from logprep.util.validators import list_of_urls_validator
 
 
 class Pseudonymizer(Processor):
     """Pseudonymize log events to conform to EU privacy laws."""
 
     @define(kw_only=True)
@@ -86,15 +87,15 @@
 
         * /var/git/depseudo_pub.pem
         """
         hash_salt: str = field(validator=validators.instance_of(str))
         """A salt that is used for hashing."""
         regex_mapping: str = field(validator=validators.instance_of(str))
         """
-        Path to a file (for string format see :ref:`getters`) with a regex mapping for 
+        Path to a file (for string format see :ref:`getters`) with a regex mapping for
         pseudonymization, i.e.:
 
         * /var/git/logprep-rules/pseudonymizer_rules/regex_mapping.json
         """
         max_cached_pseudonyms: int = field(validator=validators.instance_of(int))
         """
         The maximum number of cached pseudonyms. One cache entry requires ~250 Byte, thus 10
@@ -138,14 +139,16 @@
 
     pseudonyms: list
     pseudonymized_fields: set
 
     HASH_PREFIX = "<pseudonym:"
     HASH_SUFFIX = ">"
 
+    URL_SPLIT_PATTERN = re.compile("(://)")
+
     rule_class = PseudonymizerRule
 
     def __init__(self, name: str, configuration: Processor.Config, logger: Logger):
         super().__init__(name=name, configuration=configuration, logger=logger)
         self.metrics = self.PseudonymizerMetrics(
             labels=self.metric_labels,
             generic_rule_tree=self._generic_tree.metrics,
@@ -223,21 +226,21 @@
 
         if "@timestamp" in event:
             for pseudonym in self.pseudonyms:
                 pseudonym["@timestamp"] = event["@timestamp"]
 
     @staticmethod
     def _innermost_field(dotted_field: str, event: dict) -> Tuple[Union[dict, Any], str]:
-        keys = dotted_field.split(".")
+        keys = get_dotted_field_list(dotted_field)
         for i in range(len(keys) - 1):
             event = event[keys[i]]
         return event, keys[-1]
 
     def _pseudonymize_field(
-        self, pattern: str, field_: Union[str, List[str]]
+        self, pattern: Pattern, field_: Union[str, List[str]]
     ) -> Tuple[Union[str, List[str]], Optional[list], bool]:
         new_pseudonyms = []
 
         if isinstance(field_, list):
             values = [str(value) for value in field_]
             matches_list = [re.match(pattern, value) for value in values]
             if not any(matches_list):
@@ -250,15 +253,15 @@
                     new_field.append(
                         self._get_field_with_pseudonymized_capture_groups(matches, new_pseudonyms)
                     )
                 else:
                     new_field.append(field_[idx])
         else:
             new_field = str(field_)
-            matches = re.match(pattern, new_field)
+            matches = pattern.match(new_field)
 
             # No matches, no change
             if matches is None:
                 return new_field, None, False
 
             # Replace capture groups if there are any, else pseudonymize whole match (group(0))
             if any(matches.groups()):
@@ -280,15 +283,15 @@
         return field_
 
     def _get_field_with_pseudonymized_urls(self, field_: str, pseudonyms: List[dict]) -> str:
         pseudonyms = pseudonyms if pseudonyms else []
         for url_string in self._url_extractor.gen_urls(field_):
             url_parts = self._parse_url_parts(self._tld_extractor, url_string)
             pseudonym_map = self._get_pseudonym_map(pseudonyms, url_parts)
-            url_split = re.split("(://)", url_string)
+            url_split = self.URL_SPLIT_PATTERN.split(url_string)
 
             replacements = self._get_parts_to_replace_in_correct_order(pseudonym_map)
 
             do_not_replace_pattern = (
                 rf"(<pseudonym:[a-z0-9]*>|\?\w+=|&\w+=|"
                 rf"{url_parts['domain']}\.{url_parts['suffix']})"
             )
@@ -383,15 +386,15 @@
             pseudonyms.append({"pseudonym": hash_string, "origin": encrypted_origin})
         return self._wrap_hash(hash_string)
 
     def _replace_regex_keywords_by_regex_expression(self):
         for rule in self._specific_rules:
             for dotted_field, regex_keyword in rule.pseudonyms.items():
                 if regex_keyword in self._regex_mapping:
-                    rule.pseudonyms[dotted_field] = self._regex_mapping[regex_keyword]
+                    rule.pseudonyms[dotted_field] = re.compile(self._regex_mapping[regex_keyword])
         for rule in self._generic_rules:
             for dotted_field, regex_keyword in rule.pseudonyms.items():
                 if regex_keyword in self._regex_mapping:
-                    rule.pseudonyms[dotted_field] = self._regex_mapping[regex_keyword]
+                    rule.pseudonyms[dotted_field] = re.compile(self._regex_mapping[regex_keyword])
 
     def _wrap_hash(self, hash_string: str) -> str:
         return self.HASH_PREFIX + hash_string + self.HASH_SUFFIX
```

### Comparing `logprep-6.0.0/logprep/processor/pseudonymizer/rule.py` & `logprep-6.1.0/logprep/processor/pseudonymizer/rule.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,18 +36,17 @@
       "RE_DOMAIN_BACKSLASH_USERNAME": "\\w+\\\\(.*)",
       "RE_IP4_COLON_PORT": "([\\d.]+):\\d+"
     }
 
 """
 
 from typing import List
-import warnings
+
 from attrs import define, field, validators
 
-from logprep.util.helper import pop_dotted_field_value, add_and_overwrite
 from logprep.processor.base.rule import Rule
 
 
 class PseudonymizerRule(Rule):
     """Check if documents match a filter."""
 
     @define(kw_only=True)
```

### Comparing `logprep-6.0.0/logprep/processor/requester/processor.py` & `logprep-6.1.0/logprep/processor/requester/processor.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,36 +18,43 @@
             - tests/testdata/rules/specific/
         generic_rules:
             - tests/testdata/rules/generic/
 
 """
 import json
 import re
+
 import requests
 
 from logprep.abc.processor import Processor
-from logprep.processor.base.exceptions import DuplicationError
+from logprep.processor.base.exceptions import FieldExistsWarning
 from logprep.processor.requester.rule import RequesterRule
-from logprep.util.helper import add_field_to, get_dotted_field_value, get_source_fields_dict
+from logprep.util.helper import (
+    add_field_to,
+    get_dotted_field_value,
+    get_source_fields_dict,
+)
 
 TEMPLATE_KWARGS = ("url", "json", "data", "params")
 
 
 class Requester(Processor):
     """A processor to invoke http requests with field data
     and parses response data to field values"""
 
     rule_class = RequesterRule
 
     def _apply_rules(self, event, rule):
         source_field_dict = get_source_fields_dict(event, rule)
-        self._check_for_missing_values(event, rule, source_field_dict)
+        if self._has_missing_values(event, rule, source_field_dict):
+            return
         kwargs = self._template_kwargs(rule.kwargs, source_field_dict)
         response = self._request(event, rule, kwargs)
-        self._handle_response(event, rule, response)
+        if response is not None:
+            self._handle_response(event, rule, response)
 
     def _handle_response(self, event, rule, response):
         conflicting_fields = []
         if rule.target_field:
             result = self._get_result(response)
             successful = add_field_to(
                 event,
@@ -68,25 +75,26 @@
                     source_field_value,
                     rule.extend_target_list,
                     rule.overwrite_target,
                 )
                 if not successful:
                     conflicting_fields.append(rule.target_field)
         if conflicting_fields:
-            raise DuplicationError(self.name, [rule.target_field])
+            raise FieldExistsWarning(self, rule, event, [rule.target_field])
 
     def _request(self, event, rule, kwargs):
         try:
             response = requests.request(**kwargs)
             response.raise_for_status()
+            return response
         except requests.exceptions.HTTPError as error:
             self._handle_warning_error(event, rule, error)
         except requests.exceptions.ConnectTimeout as error:
             self._handle_warning_error(event, rule, error)
-        return response
+        return None
 
     @staticmethod
     def _get_result(response):
         try:
             result = json.loads(response.content)
         except json.JSONDecodeError:
             result = response.content.decode("utf-8")
```

### Comparing `logprep-6.0.0/logprep/processor/requester/rule.py` & `logprep-6.1.0/logprep/processor/requester/rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 import inspect
 import json
 import re
 
 import requests
 from attrs import define, field, validators
 
-from logprep.processor.field_manager.rule import FieldManagerRule, FIELD_PATTERN
+from logprep.processor.field_manager.rule import FIELD_PATTERN, FieldManagerRule
 
 parameter_keys = inspect.signature(requests.Request).parameters.keys()
 REQUEST_CONFIG_KEYS = [
     parameter for parameter in parameter_keys if parameter not in ["hooks", "cookies", "files"]
 ] + ["timeout", "proxies", "verify", "cert"]
 URL_REGEX_PATTERN = r"(http|https):\/\/.+"
 HTTP_METHODS = ["GET", "OPTIONS", "HEAD", "POST", "PUT", "PATCH", "DELETE"]
@@ -173,14 +173,15 @@
 
         def __attrs_post_init__(self):
             url_fields = re.findall(FIELD_PATTERN, self.url)
             json_fields = re.findall(FIELD_PATTERN, json.dumps(self.json))
             data_fields = re.findall(FIELD_PATTERN, self.data)
             params_fields = re.findall(FIELD_PATTERN, json.dumps(self.params))
             self.source_fields = list({*url_fields, *json_fields, *data_fields, *params_fields})
+            super().__attrs_post_init__()
 
     # pylint: disable=missing-docstring
     @property
     def kwargs(self):
         kwargs = {
             key: getattr(self._config, key)
             for key in REQUEST_CONFIG_KEYS
```

### Comparing `logprep-6.0.0/logprep/processor/selective_extractor/processor.py` & `logprep-6.1.0/logprep/processor/selective_extractor/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/processor/selective_extractor/rule.py` & `logprep-6.1.0/logprep/processor/selective_extractor/rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,15 @@
     field1
     field2
     field3
 
 """
 
 from typing import List
+
 from attrs import define, field, validators
 
 from logprep.processor.base.rule import InvalidRuleDefinitionError
 from logprep.processor.field_manager.rule import FieldManagerRule
 from logprep.util.getter import GetterFactory
 
 
@@ -155,14 +156,15 @@
         target_field: str = field(default="", init=False)
 
         overwrite_target: bool = field(default=False, init=False)
 
         extend_target_list: bool = field(default=False, init=False)
 
         def __attrs_post_init__(self):
+            super().__attrs_post_init__()
             if not self.extract_from_file:
                 return
             try:
                 content = GetterFactory.from_string(self.extract_from_file).get()
             except FileNotFoundError as error:
                 raise SelectiveExtractorRuleError(
                     "extract_from_file is not a valid file handle"
```

### Comparing `logprep-6.0.0/logprep/processor/string_splitter/processor.py` & `logprep-6.1.0/logprep/processor/string_splitter/processor.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,36 +15,36 @@
         type: string_splitter
         specific_rules:
             - tests/testdata/rules/specific/
         generic_rules:
             - tests/testdata/rules/generic/
 """
 
+from logprep.processor.base.exceptions import FieldExistsWarning, ProcessingWarning
 from logprep.processor.field_manager.processor import FieldManager
 from logprep.processor.string_splitter.rule import StringSplitterRule
 from logprep.util.helper import add_field_to, get_dotted_field_value
-from logprep.processor.base.exceptions import DuplicationError, ProcessingWarning
 
 
 class StringSplitter(FieldManager):
     """A processor that splits strings"""
 
     rule_class = StringSplitterRule
 
     def _apply_rules(self, event: dict, rule: StringSplitterRule):
         target_field = rule.target_field
         source_field = rule.source_fields[0]
         source_field_content = get_dotted_field_value(event, source_field)
         if not isinstance(source_field_content, str):
             raise ProcessingWarning(
-                f"{ self.describe() }: source_field '{source_field}' is not a string"
+                self, f"source_field '{source_field}' is not a string", rule, event
             )
         result = source_field_content.split(rule.delimeter)
         successful = add_field_to(
             event=event,
             output_field=target_field,
             content=result,
             extends_lists=rule.extend_target_list,
             overwrite_output_field=rule.overwrite_target,
         )
         if not successful:
-            raise DuplicationError(self.describe(), target_field)
+            raise FieldExistsWarning(self, rule, event, [target_field])
```

### Comparing `logprep-6.0.0/logprep/processor/string_splitter/rule.py` & `logprep-6.1.0/logprep/processor/string_splitter/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/processor/template_replacer/processor.py` & `logprep-6.1.0/logprep/processor/template_replacer/processor.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,17 +28,18 @@
 """
 from logging import Logger
 from typing import Optional
 
 from attr import define, field, validators
 
 from logprep.abc.processor import Processor
+from logprep.processor.base.exceptions import FieldExistsWarning
 from logprep.processor.template_replacer.rule import TemplateReplacerRule
 from logprep.util.getter import GetterFactory
-from logprep.util.helper import get_dotted_field_value
+from logprep.util.helper import get_dotted_field_list, get_dotted_field_value
 
 
 class TemplateReplacerError(BaseException):
     """Base class for TemplateReplacer related exceptions."""
 
     def __init__(self, name: str, message: str):
         super().__init__(f"TemplateReplacer ({name}): {message}")
@@ -81,15 +82,15 @@
     rule_class = TemplateReplacerRule
 
     def __init__(self, name: str, configuration: Processor.Config, logger: Logger):
         super().__init__(name=name, configuration=configuration, logger=logger)
         pattern = configuration.pattern
         template_path = configuration.template
         self._target_field = pattern["target_field"]
-        self._target_field_split = self._target_field.split(".")
+        self._target_field_split = get_dotted_field_list(self._target_field)
         self._fields = pattern["fields"]
         delimiter = pattern["delimiter"]
         allow_delimiter_field = pattern["allowed_delimiter_field"]
         allow_delimiter_index = self._fields.index(allow_delimiter_field)
 
         self._mapping = {}
         template = GetterFactory.from_string(template_path).get_yaml()
@@ -124,38 +125,33 @@
                 raise TemplateReplacerError(
                     self.name, "template_replacer template is invalid!"
                 ) from error
 
     def _apply_rules(self, event, rule):
         replacement = self._get_replacement_value(event)
         if replacement is not None:
-            self._perform_replacement(event, replacement)
+            self._perform_replacement(event, replacement, rule)
 
     def _get_replacement_value(self, event: dict) -> Optional[str]:
         replacement = self._mapping
         for field_ in self._fields:
             dotted_field_value = get_dotted_field_value(event, field_)
             if dotted_field_value is None:
                 return None
 
             value = str(dotted_field_value)
             replacement = replacement.get(value, None)
             if replacement is None:
                 return None
         return replacement
 
-    def _perform_replacement(self, event: dict, replacement: str):
-        _event = event
+    def _perform_replacement(self, event: dict, replacement: str, rule: TemplateReplacerRule):
         for subfield in self._target_field_split[:-1]:
-            event_sub = _event.get(subfield)
+            event_sub = event.get(subfield)
             if isinstance(event_sub, dict):
-                _event = event_sub
+                event = event_sub
             elif event_sub is None:
-                _event[subfield] = {}
-                _event = _event[subfield]
+                event[subfield] = {}
+                event = event[subfield]
             else:
-                raise TemplateReplacerError(
-                    self.name,
-                    f"Parent field '{subfield}' of target field '{self._target_field}' "
-                    f"exists and is not a dict!",
-                )
-        _event[self._target_field_split[-1]] = replacement
+                raise FieldExistsWarning(self, event, rule, [subfield])
+        event[self._target_field_split[-1]] = replacement
```

### Comparing `logprep-6.0.0/logprep/processor/template_replacer/rule.py` & `logprep-6.1.0/logprep/processor/template_replacer/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/processor/timestamp_differ/processor.py` & `logprep-6.1.0/logprep/processor/timestamp_differ/processor.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,49 +18,52 @@
             - tests/testdata/rules/generic/
 """
 from functools import reduce
 
 import arrow
 
 from logprep.abc.processor import Processor
-from logprep.processor.base.exceptions import DuplicationError
+from logprep.processor.base.exceptions import FieldExistsWarning
 from logprep.processor.timestamp_differ.rule import TimestampDifferRule
 from logprep.util.helper import add_field_to, get_source_fields_dict
 
 
 class TimestampDiffer(Processor):
     """A processor that calculates the time difference between two timestamps"""
 
     rule_class = TimestampDifferRule
 
     def _apply_rules(self, event, rule):
         source_field_formats = rule.source_field_formats
         source_field_dict = get_source_fields_dict(event, rule)
-        self._check_for_missing_values(event, rule, source_field_dict)
+        if self._has_missing_values(event, rule, source_field_dict):
+            return
+        diff = None
         try:
             timestamp_objects = map(
                 self._create_timestamp_object, source_field_dict.values(), source_field_formats
             )
             diff = reduce(lambda a, b: a - b, timestamp_objects)
         except arrow.parser.ParserError as error:
             error.args = [
                 f"{error.args[0]} Corresponding source fields and values are: {source_field_dict}."
             ]
             self._handle_warning_error(event, rule, error)
 
-        diff = self._apply_output_format(diff, rule)
-        add_successful = add_field_to(
-            event,
-            output_field=rule.target_field,
-            content=diff,
-            extends_lists=rule.extend_target_list,
-            overwrite_output_field=rule.overwrite_target,
-        )
-        if not add_successful:
-            raise DuplicationError(self.name, [rule.target_field])
+        if diff is not None:
+            diff = self._apply_output_format(diff, rule)
+            add_successful = add_field_to(
+                event,
+                output_field=rule.target_field,
+                content=diff,
+                extends_lists=rule.extend_target_list,
+                overwrite_output_field=rule.overwrite_target,
+            )
+            if not add_successful:
+                raise FieldExistsWarning(self, rule, event, [rule.target_field])
 
     @staticmethod
     def _create_timestamp_object(timestamp_str, timestamp_format):
         if timestamp_format is None:
             return arrow.get(timestamp_str)
         return arrow.get(timestamp_str, timestamp_format)
```

### Comparing `logprep-6.0.0/logprep/processor/timestamp_differ/rule.py` & `logprep-6.1.0/logprep/processor/timestamp_differ/rule.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,15 @@
    :template: testcase-renderer.tmpl
 """
 import re
 
 from attr import field
 from attrs import define, validators
 
-from logprep.processor.field_manager.rule import FieldManagerRule, FIELD_PATTERN
+from logprep.processor.field_manager.rule import FIELD_PATTERN, FieldManagerRule
 
 
 class TimestampDifferRule(FieldManagerRule):
     """TimestampDifferRule"""
 
     @define(kw_only=True)
     class Config(FieldManagerRule.Config):
@@ -86,14 +86,15 @@
         def __attrs_post_init__(self):
             field_format_str = re.findall(FIELD_PATTERN, self.diff)
             field_format_tuple = map(lambda s: s.split(":", maxsplit=1), field_format_str)
             field_format_tuple = map(lambda x: x + [None] if len(x) == 1 else x, field_format_tuple)
             source_fields, source_field_formats = list(map(list, zip(*field_format_tuple)))
             self.source_fields = source_fields
             self.source_field_formats = source_field_formats
+            super().__attrs_post_init__()
 
     # pylint: disable=missing-function-docstring
     @property
     def output_format(self):
         return self._config.output_format
 
     @property
```

### Comparing `logprep-6.0.0/logprep/registry.py` & `logprep-6.1.0/logprep/registry.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,36 +5,39 @@
 
 from logprep.connector.confluent_kafka.input import ConfluentKafkaInput
 from logprep.connector.confluent_kafka.output import ConfluentKafkaOutput
 from logprep.connector.console.output import ConsoleOutput
 from logprep.connector.dummy.input import DummyInput
 from logprep.connector.dummy.output import DummyOutput
 from logprep.connector.elasticsearch.output import ElasticsearchOutput
+from logprep.connector.file.input import FileInput
 from logprep.connector.http.input import HttpConnector
 from logprep.connector.json.input import JsonInput
 from logprep.connector.jsonl.input import JsonlInput
 from logprep.connector.jsonl.output import JsonlOutput
-from logprep.connector.file.input import FileInput
 from logprep.connector.opensearch.output import OpensearchOutput
+from logprep.connector.s3.output import S3Output
+from logprep.processor.amides.processor import Amides
 from logprep.processor.calculator.processor import Calculator
 from logprep.processor.clusterer.processor import Clusterer
 from logprep.processor.concatenator.processor import Concatenator
 from logprep.processor.datetime_extractor.processor import DatetimeExtractor
 from logprep.processor.deleter.processor import Deleter
 from logprep.processor.dissector.processor import Dissector
 from logprep.processor.domain_label_extractor.processor import DomainLabelExtractor
 from logprep.processor.domain_resolver.processor import DomainResolver
 from logprep.processor.dropper.processor import Dropper
 from logprep.processor.field_manager.processor import FieldManager
 from logprep.processor.generic_adder.processor import GenericAdder
 from logprep.processor.generic_resolver.processor import GenericResolver
 from logprep.processor.geoip_enricher.processor import GeoipEnricher
+from logprep.processor.grokker.processor import Grokker
 from logprep.processor.hyperscan_resolver.processor import HyperscanResolver
-from logprep.processor.key_checker.processor import KeyChecker
 from logprep.processor.ip_informer.processor import IpInformer
+from logprep.processor.key_checker.processor import KeyChecker
 from logprep.processor.labeler.processor import Labeler
 from logprep.processor.list_comparison.processor import ListComparison
 from logprep.processor.normalizer.processor import Normalizer
 from logprep.processor.pre_detector.processor import PreDetector
 from logprep.processor.pseudonymizer.processor import Pseudonymizer
 from logprep.processor.requester.processor import Requester
 from logprep.processor.selective_extractor.processor import SelectiveExtractor
@@ -44,27 +47,29 @@
 
 
 class Registry:
     """Component Registry"""
 
     mapping = {
         # Processors
+        "amides": Amides,
         "calculator": Calculator,
         "clusterer": Clusterer,
         "concatenator": Concatenator,
         "datetime_extractor": DatetimeExtractor,
         "deleter": Deleter,
         "dissector": Dissector,
         "domain_label_extractor": DomainLabelExtractor,
         "domain_resolver": DomainResolver,
         "dropper": Dropper,
         "field_manager": FieldManager,
         "generic_adder": GenericAdder,
         "generic_resolver": GenericResolver,
         "geoip_enricher": GeoipEnricher,
+        "grokker": Grokker,
         "hyperscan_resolver": HyperscanResolver,
         "ip_informer": IpInformer,
         "key_checker": KeyChecker,
         "labeler": Labeler,
         "list_comparison": ListComparison,
         "normalizer": Normalizer,
         "pre_detector": PreDetector,
@@ -83,14 +88,15 @@
         "confluentkafka_input": ConfluentKafkaInput,
         "confluentkafka_output": ConfluentKafkaOutput,
         "console_output": ConsoleOutput,
         "elasticsearch_output": ElasticsearchOutput,
         "jsonl_output": JsonlOutput,
         "opensearch_output": OpensearchOutput,
         "http_input": HttpConnector,
+        "s3_output": S3Output,
     }
 
     @classmethod
     def get_class(cls, component_type):
         """return the processor class for a given type
 
         Parameters
```

### Comparing `logprep-6.0.0/logprep/run_logprep.py` & `logprep-6.1.0/logprep/run_logprep.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/runner.py` & `logprep-6.1.0/logprep/runner.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/util/aggregating_logger.py` & `logprep-6.1.0/logprep/util/aggregating_logger.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/util/auto_rule_tester/auto_rule_corpus_tester.py` & `logprep-6.1.0/logprep/util/auto_rule_tester/auto_rule_corpus_tester.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,14 +183,15 @@
     def _run_pipeline_per_test_case(self):
         """
         For each test case the logprep connector files are rewritten (only the current test case
         will be added to the input file), the pipline is run and the outputs are compared.
         """
         print(Style.BRIGHT + "# Test Cases Summary:" + Style.RESET_ALL)
         for test_case_id, test_case in self._test_cases.items():
+            _ = [processor.setup() for processor in self._pipeline._pipeline]
             parsed_event, extra_outputs = self._pipeline.process_pipeline()
             extra_outputs = self._align_extra_output_formats(extra_outputs)
             test_case.generated_output = parsed_event
             test_case.generated_extra_output = extra_outputs
             self._compare_logprep_outputs(test_case_id, parsed_event)
             self._compare_extra_data_output(test_case_id, extra_outputs)
             self._print_pass_fail_statements(test_case_id)
```

### Comparing `logprep-6.0.0/logprep/util/auto_rule_tester/auto_rule_tester.py` & `logprep-6.1.0/logprep/util/auto_rule_tester/auto_rule_tester.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,44 +48,40 @@
 (see :doc:`configuration/configurationdata`).
 
 Auto-testing does also perform a verification of the pipeline section of the Logprep configuration.
 """
 
 import hashlib
 import json
+import re
 import sys
 import tempfile
 import traceback
 from collections import OrderedDict, defaultdict
 from contextlib import redirect_stdout
 from difflib import ndiff
 from io import StringIO
 from logging import getLogger
 from os import path, walk
 from pprint import pprint
-from typing import TYPE_CHECKING, Tuple, TextIO
+from typing import TYPE_CHECKING, TextIO, Tuple
 
-import regex as re
 from colorama import Fore
 from ruamel.yaml import YAML, YAMLError
-from typing.io import TextIO
 
 from logprep.factory import Factory
 from logprep.framework.rule_tree.rule_tree import RuleTree
 from logprep.processor.pre_detector.processor import PreDetector
 from logprep.util.auto_rule_tester.grok_pattern_replacer import GrokPatternReplacer
 from logprep.util.helper import print_fcolor, remove_file_if_exists
 
 if TYPE_CHECKING:
     from logprep.abc.processor import Processor
 
 
-logger = getLogger()
-logger.disabled = True
-
 yaml = YAML(typ="safe", pure=True)
 
 
 # pylint: disable=protected-access
 class AutoRuleTesterException(BaseException):
     """Base class for AutoRuleTester related exceptions."""
 
@@ -177,14 +173,17 @@
 
         self._gpr = GrokPatternReplacer(self._config_yml)
 
         self._custom_tests_output = ""
         self._custom_tests = []
         self._missing_custom_tests = []
 
+        self._logger = getLogger()
+        self._logger.disabled = True
+
     def run(self):
         """Perform auto-tests."""
         rules_dirs = self._get_rule_dirs_by_processor_name()
         rules_pn = self._get_rules_per_processor_name(rules_dirs)
         self._run_if_any_rules_exist(rules_pn)
 
     def _run_if_any_rules_exist(self, rules_pn: dict):
@@ -242,26 +241,26 @@
         return False
 
     def _get_processors_split_by_custom_tests_existence(self) -> Tuple[OrderedDict, OrderedDict]:
         processors_with_custom_test = OrderedDict()
         processors_without_custom_test = OrderedDict()
         for processor_in_pipeline in self._config_yml["pipeline"]:
             name, processor_cfg = next(iter(processor_in_pipeline.items()))
-            processor = self._get_processor_instance(name, processor_cfg, logger)
+            processor = self._get_processor_instance(name, processor_cfg, self._logger)
             if processor.has_custom_tests:
                 processors_with_custom_test[processor] = name
             else:
                 processors_without_custom_test[processor] = name
         return processors_with_custom_test, processors_without_custom_test
 
     def _get_custom_test_mapping(self) -> dict:
         processor_uses_own_tests = {}
         for processor_in_pipeline in self._config_yml["pipeline"]:
             name, processor_cfg = next(iter(processor_in_pipeline.items()))
-            processor = self._get_processor_instance(name, processor_cfg, logger)
+            processor = self._get_processor_instance(name, processor_cfg, self._logger)
             processor_uses_own_tests[processor_cfg["type"]] = processor.has_custom_tests
         return processor_uses_own_tests
 
     @staticmethod
     def _get_rules(processor: "Processor", rule_test: dict) -> dict:
         if rule_test.get("rules"):
             return {"rules": rule_test.get("rules", [])}
```

### Comparing `logprep-6.0.0/logprep/util/auto_rule_tester/grok_pattern_replacer.py` & `logprep-6.1.0/logprep/util/auto_rule_tester/grok_pattern_replacer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/python3
 """This module implements a grok pattern replacer for the auto tester."""
 
+import re
 from pprint import pprint
 from typing import Any
 
-import regex as re
-
 from logprep.util.grok_pattern_loader import GrokPatternLoader as gpl
 from logprep.util.helper import get_dotted_field_value
 
 
 # pylint: disable=protected-access
 class GrokPatternReplacer:
     """Used to replace strings with pre-defined grok patterns."""
```

### Comparing `logprep-6.0.0/logprep/util/cache.py` & `logprep-6.1.0/logprep/util/cache.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/util/configuration.py` & `logprep-6.1.0/logprep/util/configuration.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/util/decorators.py` & `logprep-6.1.0/logprep/util/decorators.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/util/getter.py` & `logprep-6.1.0/logprep/util/getter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/util/grok_pattern_loader.py` & `logprep-6.1.0/logprep/util/grok_pattern_loader.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/util/hasher.py` & `logprep-6.1.0/logprep/util/hasher.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/util/helper.py` & `logprep-6.1.0/logprep/util/helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """This module contains helper functions that are shared by different modules."""
 import re
-from functools import partial, reduce
+from functools import lru_cache, partial, reduce
 from os import remove
 from typing import Optional, Union
 
-from colorama import Fore, Back
-from colorama.ansi import AnsiFore, AnsiBack
+from colorama import Back, Fore
+from colorama.ansi import AnsiBack, AnsiFore
 
 
 def color_print_line(
     back: Optional[Union[str, AnsiBack]], fore: Optional[Union[str, AnsiBack]], message: str
 ):
     """Print string with colors and reset the color afterwards."""
     color = ""
@@ -71,37 +71,36 @@
     This method returns true if no conflicting fields were found during the process of the creation
     of the dotted subfields. If conflicting fields were found False is returned.
     """
 
     assert not (
         extends_lists and overwrite_output_field
     ), "An output field can't be overwritten and extended at the same time"
-
-    output_field_path = [event, *output_field.split(".")]
+    output_field_path = [event, *get_dotted_field_list(output_field)]
     target_key = output_field_path.pop()
 
     if overwrite_output_field:
         target_field = reduce(_add_and_overwrite_key, output_field_path)
-        target_field.update({target_key: content})
+        target_field |= {target_key: content}
         return True
 
     try:
         target_field = reduce(_add_and_not_overwrite_key, output_field_path)
     except KeyError:
         return False
 
     target_field_value = target_field.get(target_key)
     if target_field_value is None:
-        target_field.update({target_key: content})
+        target_field |= {target_key: content}
         return True
     if extends_lists:
         if not isinstance(target_field_value, list):
             return False
         if isinstance(content, list):
-            target_field.update({target_key: [*target_field_value, *content]})
+            target_field |= {target_key: [*target_field_value, *content]}
         else:
             target_field_value.append(content)
         return True
     return False
 
 
 def _get_slice_arg(slice_item):
@@ -133,28 +132,41 @@
         The dotted field name which identifies the requested value
 
     Returns
     -------
     dict_: dict, list, str
         The value of the requested dotted field.
     """
-
-    fields = [event, *dotted_field.split(".")]
     try:
-        return reduce(_get_item, fields)
-    except KeyError:
-        return None
-    except ValueError:
-        return None
-    except TypeError:
-        return None
-    except IndexError:
+        for field in get_dotted_field_list(dotted_field):
+            event = _get_item(event, field)
+        return event
+    except (KeyError, ValueError, TypeError, IndexError):
         return None
 
 
+@lru_cache(maxsize=None)
+def get_dotted_field_list(dotted_field: str) -> list[str]:
+    """make lookup of dotted field in the dotted_field_lookup_table and ensures
+    it is added if not found. Additionally the string will be interned for faster
+    followup lookups.
+
+    Parameters
+    ----------
+    dotted_field : str
+        the dotted field input
+
+    Returns
+    -------
+    list[str]
+        a list with keys for dictionary iteration
+    """
+    return dotted_field.split(".")
+
+
 def pop_dotted_field_value(event: dict, dotted_field: str) -> Optional[Union[dict, list, str]]:
     """
     Remove and return dotted field. Returns None is field does not exist.
 
     Parameters
     ----------
     event: dict
```

### Comparing `logprep-6.0.0/logprep/util/json_handling.py` & `logprep-6.1.0/logprep/util/json_handling.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/util/log_aggregator.py` & `logprep-6.1.0/logprep/util/log_aggregator.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/util/multiprocessing_log_handler.py` & `logprep-6.1.0/logprep/util/multiprocessing_log_handler.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/util/pipeline_profiler.py` & `logprep-6.1.0/logprep/util/pipeline_profiler.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/util/pre_detector_rule_matching_tester.py` & `logprep-6.1.0/logprep/util/pre_detector_rule_matching_tester.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 #!/usr/bin/python3
 """This module is used to test if PreDetector rules match depending on a naming scheme."""
 
 import json
 import logging
+import re
 import sys
 import tempfile
 from argparse import ArgumentParser
 from os import path, sep, walk
 from typing import Any, List, Tuple
 
-import regex as re
 from colorama import Fore
 from ruamel.yaml import YAML, YAMLError
+
+from logprep.factory import Factory
 from logprep.framework.rule_tree.rule_tree import RuleTree
 from logprep.processor.pre_detector.processor import PreDetector
 from logprep.processor.pre_detector.rule import PreDetectorRule
-from logprep.factory import Factory
 from logprep.util.helper import print_fcolor
 
-logger = logging.getLogger()
-logger.disabled = True
-
 yaml = YAML(typ="safe", pure=True)
 
 
 # pylint: disable=protected-access
 class MatchingRuleTesterException(BaseException):
     """Base class for MatchingRuleTester related exceptions."""
 
@@ -130,15 +128,16 @@
         processor_cfg = {
             "type": "pre_detector",
             "generic_rules": [],
             "specific_rules": [],
             "tree_config": "",
             "pre_detector_topic": "",
         }
-
+        logger = logging.getLogger()
+        logger.disabled = True
         processor = Factory.create(processor_cfg, logger)
         return processor
 
     def _print_results(self):
         print_fcolor(Fore.RED, "---- Failed tests ----")
         for failed_test, values in self._failed_tests.items():
             print_fcolor(Fore.RED, "Rule:")
```

### Comparing `logprep-6.0.0/logprep/util/processor_generator.py` & `logprep-6.1.0/logprep/util/processor_generator.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/util/prometheus_exporter.py` & `logprep-6.1.0/logprep/util/prometheus_exporter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/util/rule_dry_runner.py` & `logprep-6.1.0/logprep/util/rule_dry_runner.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,25 +42,21 @@
 import json
 import shutil
 import tempfile
 from copy import deepcopy
 from difflib import ndiff
 from functools import cached_property
 
-from colorama import Fore, Back
+from colorama import Back, Fore
 from ruamel.yaml import YAML
 
 from logprep.framework.pipeline import Pipeline
 from logprep.util.configuration import Configuration
 from logprep.util.getter import GetterFactory
-from logprep.util.helper import (
-    color_print_line,
-    recursive_compare,
-    color_print_title,
-)
+from logprep.util.helper import color_print_line, color_print_title, recursive_compare
 
 yaml = YAML(typ="safe", pure=True)
 
 
 class DryRunner:
     """Used to run pipeline with given events and show changes made by processing."""
```

### Comparing `logprep-6.0.0/logprep/util/schema_and_rule_checker.py` & `logprep-6.1.0/logprep/util/schema_and_rule_checker.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/util/time_measurement.py` & `logprep-6.1.0/logprep/util/time_measurement.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep/util/validators.py` & `logprep-6.1.0/logprep/util/validators.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/logprep.egg-info/PKG-INFO` & `logprep-6.1.0/logprep.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logprep
-Version: 6.0.0
+Version: 6.1.0
 Summary: Logprep allows to collect, process and forward log messages from various data sources.
 Home-page: https://github.com/fkie-cad/Logprep
 Author: Logprep Team
 License: LGPL-2.1 license
 Project-URL: Homepage, https://github.com/fkie-cad/Logprep
 Project-URL: Documentation, https://logprep.readthedocs.io/en/latest/
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: logprep Version: 6.0.0 Summary: Logprep allows to
+Metadata-Version: 2.1 Name: logprep Version: 6.1.0 Summary: Logprep allows to
 collect, process and forward log messages from various data sources. Home-page:
 https://github.com/fkie-cad/Logprep Author: Logprep Team License: LGPL-2.1
 license Project-URL: Homepage, https://github.com/fkie-cad/Logprep Project-URL:
 Documentation, https://logprep.readthedocs.io/en/latest/ Platform: UNKNOWN
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

### Comparing `logprep-6.0.0/logprep.egg-info/SOURCES.txt` & `logprep-6.1.0/logprep.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -44,14 +44,16 @@
 logprep/connector/json/__init__.py
 logprep/connector/json/input.py
 logprep/connector/jsonl/__init__.py
 logprep/connector/jsonl/input.py
 logprep/connector/jsonl/output.py
 logprep/connector/opensearch/__init__.py
 logprep/connector/opensearch/output.py
+logprep/connector/s3/__init__.py
+logprep/connector/s3/output.py
 logprep/filter/__init__.py
 logprep/filter/lucene_filter.py
 logprep/filter/expression/__init__.py
 logprep/filter/expression/filter_expression.py
 logprep/framework/__init__.py
 logprep/framework/pipeline.py
 logprep/framework/pipeline_manager.py
@@ -61,14 +63,20 @@
 logprep/framework/rule_tree/rule_tree.py
 logprep/metrics/__init__.py
 logprep/metrics/metric.py
 logprep/metrics/metric_exposer.py
 logprep/metrics/metric_targets.py
 logprep/processor/__init__.py
 logprep/processor/processor_strategy.py
+logprep/processor/amides/__init__.py
+logprep/processor/amides/detection.py
+logprep/processor/amides/features.py
+logprep/processor/amides/normalize.py
+logprep/processor/amides/processor.py
+logprep/processor/amides/rule.py
 logprep/processor/base/__init__.py
 logprep/processor/base/exceptions.py
 logprep/processor/base/rule.py
 logprep/processor/calculator/__init__.py
 logprep/processor/calculator/fourFn.py
 logprep/processor/calculator/processor.py
 logprep/processor/calculator/rule.py
@@ -110,14 +118,17 @@
 logprep/processor/generic_adder/rule.py
 logprep/processor/generic_resolver/__init__.py
 logprep/processor/generic_resolver/processor.py
 logprep/processor/generic_resolver/rule.py
 logprep/processor/geoip_enricher/__init__.py
 logprep/processor/geoip_enricher/processor.py
 logprep/processor/geoip_enricher/rule.py
+logprep/processor/grokker/__init__.py
+logprep/processor/grokker/processor.py
+logprep/processor/grokker/rule.py
 logprep/processor/hyperscan_resolver/__init__.py
 logprep/processor/hyperscan_resolver/processor.py
 logprep/processor/hyperscan_resolver/rule.py
 logprep/processor/ip_informer/__init__.py
 logprep/processor/ip_informer/processor.py
 logprep/processor/ip_informer/rule.py
 logprep/processor/key_checker/__init__.py
@@ -176,16 +187,19 @@
 logprep/util/schema_and_rule_checker.py
 logprep/util/time_measurement.py
 logprep/util/validators.py
 logprep/util/auto_rule_tester/__init__.py
 logprep/util/auto_rule_tester/auto_rule_corpus_tester.py
 logprep/util/auto_rule_tester/auto_rule_tester.py
 logprep/util/auto_rule_tester/grok_pattern_replacer.py
+logprep/util/grok/__init__.py
+logprep/util/grok/grok.py
 tests/__init__.py
 tests/acceptance/__init__.py
+tests/acceptance/test_amides.py
 tests/acceptance/test_config_refresh.py
 tests/acceptance/test_file_input.py
 tests/acceptance/test_full_configuration.py
 tests/acceptance/test_http_input.py
 tests/acceptance/test_multiple_outputs.py
 tests/acceptance/test_pre_detection.py
 tests/acceptance/test_preprocessing.py
@@ -207,14 +221,16 @@
 tests/testdata/unit/clusterer/__init__.py
 tests/testdata/unit/clusterer/test_data.py
 tests/unit/__init__.py
 tests/unit/test_configuration.py
 tests/unit/test_factory.py
 tests/unit/test_run_logprep.py
 tests/unit/test_runner.py
+tests/unit/component/__init__.py
+tests/unit/component/base.py
 tests/unit/connector/__init__.py
 tests/unit/connector/base.py
 tests/unit/connector/test_confluent_kafka_common.py
 tests/unit/connector/test_confluent_kafka_input.py
 tests/unit/connector/test_confluent_kafka_output.py
 tests/unit/connector/test_console_output.py
 tests/unit/connector/test_dummy_input.py
@@ -224,14 +240,18 @@
 tests/unit/connector/test_file_input_not_tailing_config.py
 tests/unit/connector/test_file_input_start_at_end_config.py
 tests/unit/connector/test_http_input.py
 tests/unit/connector/test_json_input.py
 tests/unit/connector/test_jsonl_input.py
 tests/unit/connector/test_jsonl_output.py
 tests/unit/connector/test_opensearch_output.py
+tests/unit/connector/test_s3_output.py
+tests/unit/exceptions/__init__.py
+tests/unit/exceptions/processor/__init__.py
+tests/unit/exceptions/processor/test_processing_warning.py
 tests/unit/filter/__init__.py
 tests/unit/filter/test_filter_expression.py
 tests/unit/filter/test_lucene_filter.py
 tests/unit/framework/__init__.py
 tests/unit/framework/test_pipeline.py
 tests/unit/framework/test_pipeline_manager.py
 tests/unit/framework/rule_tree/__init__.py
@@ -242,14 +262,20 @@
 tests/unit/metrics/test_metric_exposer.py
 tests/unit/metrics/test_metric_targets.py
 tests/unit/metrics/test_metrics.py
 tests/unit/processor/__init__.py
 tests/unit/processor/base.py
 tests/unit/processor/test_processor_rule.py
 tests/unit/processor/test_processor_strategy.py
+tests/unit/processor/amides/__init__.py
+tests/unit/processor/amides/test_amides.py
+tests/unit/processor/amides/test_amides_rule.py
+tests/unit/processor/amides/test_detection.py
+tests/unit/processor/amides/test_normalize.py
+tests/unit/processor/amides/test_tokenizer.py
 tests/unit/processor/calculator/__init__.py
 tests/unit/processor/calculator/test_calculator.py
 tests/unit/processor/calculator/test_calculator_rule.py
 tests/unit/processor/clusterer/__init__.py
 tests/unit/processor/clusterer/test_clusterer.py
 tests/unit/processor/clusterer/test_clusterer_rule.py
 tests/unit/processor/clusterer/test_clusterer_signature_phase.py
@@ -282,14 +308,18 @@
 tests/unit/processor/generic_adder/test_generic_adder_rule.py
 tests/unit/processor/generic_resolver/__init__.py
 tests/unit/processor/generic_resolver/test_generic_resolver.py
 tests/unit/processor/generic_resolver/test_generic_resolver_rule.py
 tests/unit/processor/geoip_enricher/__init__.py
 tests/unit/processor/geoip_enricher/test_geoip_enricher.py
 tests/unit/processor/geoip_enricher/test_geoip_enricher_rule.py
+tests/unit/processor/grokker/__init__.py
+tests/unit/processor/grokker/test_grok.py
+tests/unit/processor/grokker/test_grokker.py
+tests/unit/processor/grokker/test_grokker_rule.py
 tests/unit/processor/hyperscan_resolver/__init__.py
 tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver.py
 tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver_rule.py
 tests/unit/processor/ip_informer/__init__.py
 tests/unit/processor/ip_informer/test_ip_informer.py
 tests/unit/processor/ip_informer/test_ip_informer_rule.py
 tests/unit/processor/labeler/__init__.py
```

### Comparing `logprep-6.0.0/setup.py` & `logprep-6.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/acceptance/test_config_refresh.py` & `logprep-6.1.0/tests/acceptance/test_config_refresh.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # pylint: disable=missing-docstring
 import json
 from pathlib import Path
+
 from ruamel.yaml import YAML
-from tests.acceptance.util import (
-    start_logprep,
-    stop_logprep,
-    wait_for_output,
-)
+
 from logprep.util.configuration import Configuration
+from tests.acceptance.util import start_logprep, stop_logprep, wait_for_output
 
 yaml = YAML(typ="safe", pure=True)
 
 
 def teardown_function():
     Path("generated_config.yml").unlink(missing_ok=True)
     stop_logprep()
@@ -38,9 +36,9 @@
     config_path = tmp_path / "generated_config.yml"
     config_path.write_text(json.dumps(config))
     proc = start_logprep(config_path)
     wait_for_output(proc, "Config refresh interval is set to: 5 seconds", test_timeout=5)
     wait_for_output(
         proc,
         "Configuration version didn't change. Continue running with current version.",
-        test_timeout=5,
+        test_timeout=7,
     )
```

### Comparing `logprep-6.0.0/tests/acceptance/test_file_input.py` & `logprep-6.1.0/tests/acceptance/test_file_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/acceptance/test_full_configuration.py` & `logprep-6.1.0/tests/acceptance/test_full_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 import tempfile
 from pathlib import Path
 
 import requests
 
 from logprep.util.json_handling import dump_config_as_file
 from tests.acceptance.util import (
-    get_full_pipeline,
+    HTTPServerForTesting,
+    convert_to_http_config,
     get_default_logprep_config,
+    get_full_pipeline,
     start_logprep,
     stop_logprep,
-    convert_to_http_config,
-    HTTPServerForTesting,
 )
 
 
 def teardown_function():
     Path("generated_config.yml").unlink(missing_ok=True)
     stop_logprep()
 
@@ -149,15 +149,15 @@
                 "type": "console_output",
             },
         },
     }
     config_path = str(tmp_path / "generated_config.yml")
     dump_config_as_file(config_path, config)
     proc = start_logprep(config_path, env={"PROMETHEUS_MULTIPROC_DIR": tmp_path})
-    input_file_path.write_text("test event\n", encoding="utf8")
+    input_file_path.write_text("user root logged in\n", encoding="utf8")
     while True:
         output = proc.stdout.readline().decode("utf8")
         assert "error" not in output.lower(), "error message"
         assert "critical" not in output.lower(), "error message"
         assert "exception" not in output.lower(), "error message"
         assert "error" not in output.lower(), "error message"
         if "Started exposing metrics" in output:
```

### Comparing `logprep-6.0.0/tests/acceptance/test_http_input.py` & `logprep-6.1.0/tests/acceptance/test_http_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import pytest
 import requests
 
 from logprep.util.json_handling import dump_config_as_file
 from tests.acceptance.util import (
     get_default_logprep_config,
     start_logprep,
-    wait_for_output,
     stop_logprep,
+    wait_for_output,
 )
 
 basicConfig(level=DEBUG, format="%(asctime)-15s %(name)-5s %(levelname)-8s: %(message)s")
 logger = getLogger("Logprep-Test")
 
 
 @pytest.fixture(name="config")
@@ -57,30 +57,30 @@
 @pytest.mark.filterwarnings("ignore:Unverified HTTPS request is being made to host '127.0.0.1'")
 def test_http_input_accepts_message_for_single_pipeline(tmp_path, config):
     output_path = tmp_path / "output.jsonl"
     config["output"] = {"testoutput": {"type": "jsonl_output", "output_file": str(output_path)}}
     config_path = str(tmp_path / "generated_config.yml")
     dump_config_as_file(config_path, config)
     proc = start_logprep(config_path)
-    wait_for_output(proc, "Uvicorn running on https://127.0.0.1:9000")
+    wait_for_output(proc, "Uvicorn running on https://127.0.0.1:9000", test_timeout=15)
     # nosemgrep
     requests.post("https://127.0.0.1:9000/plaintext", data="my message", verify=False, timeout=5)
     time.sleep(0.5)  # nosemgrep
     assert "my message" in output_path.read_text()
 
 
 @pytest.mark.filterwarnings("ignore:Unverified HTTPS request is being made to host '127.0.0.1'")
 def test_http_input_accepts_message_for_two_pipelines(tmp_path, config):
     config["process_count"] = 2
     output_path = tmp_path / "output.jsonl"
     config["output"] = {"testoutput": {"type": "jsonl_output", "output_file": str(output_path)}}
     config_path = str(tmp_path / "generated_config.yml")
     dump_config_as_file(config_path, config)
     proc = start_logprep(config_path)
-    wait_for_output(proc, "Uvicorn running on https://127.0.0.1:9001")
+    wait_for_output(proc, "Uvicorn running on https://127.0.0.1:9001", test_timeout=15)
     # nosemgrep
     requests.post(
         "https://127.0.0.1:9000/plaintext",
         data="my first message",
         verify=False,
         timeout=5,
     )
@@ -101,15 +101,15 @@
 def test_http_input_accepts_message_for_three_pipelines(tmp_path, config):
     config["process_count"] = 3
     output_path = tmp_path / "output.jsonl"
     config["output"] = {"testoutput": {"type": "jsonl_output", "output_file": str(output_path)}}
     config_path = str(tmp_path / "generated_config.yml")
     dump_config_as_file(config_path, config)
     proc = start_logprep(config_path)
-    wait_for_output(proc, "Uvicorn running on https://127.0.0.1:9002", test_timeout=10)
+    wait_for_output(proc, "Uvicorn running on https://127.0.0.1:9002", test_timeout=15)
     # nosemgrep
     requests.post(
         "https://127.0.0.1:9000/plaintext",
         data="my first message",
         verify=False,
         timeout=5,
     )
```

### Comparing `logprep-6.0.0/tests/acceptance/test_multiple_outputs.py` & `logprep-6.1.0/tests/acceptance/test_multiple_outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import time
 
 import pytest
 
 from logprep.util.json_handling import dump_config_as_file
 from tests.acceptance.util import start_logprep, stop_logprep, wait_for_output
 
-
 CHECK_INTERVAL = 0.1
 
 
 def wait_for_interval(interval):
     time.sleep(2 * interval)
 
 
@@ -116,15 +115,15 @@
             },
         },
     }
     config |= output
     config_path = str(tmp_path / "generated_config.yml")
     dump_config_as_file(config_path, config)
     proc = start_logprep(config_path)
-    wait_for_output(proc, "Lost or failed to establish connection to JsonlInput")
+    wait_for_output(proc, "no documents left")
     stop_logprep(proc)
     assert output_path1.read_text(), "output is not empty"
     assert (
         output_path1.read_text() == output_path2.read_text()
     ), "stored output in both default outputs"
     assert output_path_custom1.read_text(), "stored custom output in output with name 'jsonl'"
     assert (
```

### Comparing `logprep-6.0.0/tests/acceptance/test_pre_detection.py` & `logprep-6.1.0/tests/acceptance/test_pre_detection.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/acceptance/test_preprocessing.py` & `logprep-6.1.0/tests/acceptance/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/acceptance/test_selective_extractor_full_pipeline_pass.py` & `logprep-6.1.0/tests/acceptance/test_selective_extractor_full_pipeline_pass.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/acceptance/test_wineventlog_normalization.py` & `logprep-6.1.0/tests/acceptance/test_wineventlog_processing.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,51 +1,94 @@
 # pylint: disable=missing-docstring
-# pylint: disable=line-too-long
-#!/usr/bin/python3
-from os import path
+import logging
+import os
 
 import pytest
 
 from logprep.util.json_handling import dump_config_as_file, parse_jsonl
 from tests.acceptance.util import (
     get_default_logprep_config,
+    get_difference,
     get_test_output,
     store_latest_test_output,
-    get_difference,
 )
 
+logging.basicConfig(
+    level=logging.DEBUG, format="%(asctime)-15s %(name)-5s %(levelname)-8s: %(message)s"
+)
+logger = logging.getLogger("Logprep-Test")
 
-@pytest.fixture(name="config")
-def create_config():
+
+@pytest.fixture(name="config_template")
+def fixture_config_template():
     pipeline = [
         {
-            "normalizername": {
-                "type": "normalizer",
-                "specific_rules": ["tests/testdata/acceptance/normalizer/rules_static/specific"],
-                "generic_rules": ["tests/testdata/acceptance/normalizer/rules_static/generic"],
-                "regex_mapping": "tests/testdata/acceptance/normalizer/rules_static/regex_mapping.yml",
+            "labelername": {
+                "type": "labeler",
+                "schema": "",
+                "include_parent_labels": True,
+                "specific_rules": None,
+                "generic_rules": None,
             }
         }
     ]
     return get_default_logprep_config(pipeline, with_hmac=False)
 
 
-def test_events_normalized_correctly(tmp_path, config):
-    expected_output = "normalized_win_event_log.jsonl"
-    expected_output_path = path.join("tests/testdata/acceptance/expected_result", expected_output)
-    config["input"]["jsonl"][
+@pytest.mark.parametrize(
+    "specific_rules, generic_rules, schema, expected_output",
+    [
+        (
+            ["acceptance/labeler/rules_static/rules/specific"],
+            ["acceptance/labeler/rules_static/rules/generic"],
+            "acceptance/labeler/rules_static/labeling/schema.json",
+            "labeled_win_event_log.jsonl",
+        ),
+        (
+            [
+                "acceptance/labeler/rules_static/rules/specific",
+                "acceptance/labeler/rules_static_only_regex/rules/specific",
+            ],
+            [
+                "acceptance/labeler/rules_static/rules/generic",
+                "acceptance/labeler/rules_static_only_regex/rules/generic",
+            ],
+            "acceptance/labeler/rules_static_only_regex/labeling/schema.json",
+            "labeled_win_event_log_with_regex.jsonl",
+        ),
+    ],
+)
+def test_events_labeled_correctly(
+    tmp_path, config_template, specific_rules, generic_rules, schema, expected_output
+):  # pylint: disable=too-many-arguments
+    expected_output_path = os.path.join(
+        "tests/testdata/acceptance/expected_result", expected_output
+    )
+
+    set_config(config_template, specific_rules, generic_rules, schema)
+    config_template["input"]["jsonl"][
         "documents_path"
     ] = "tests/testdata/input_logdata/wineventlog_raw.jsonl"
     config_path = str(tmp_path / "generated_config.yml")
-    dump_config_as_file(config_path, config)
+    dump_config_as_file(config_path, config_template)
 
     test_output, _, _ = get_test_output(config_path)
     assert test_output, "should not be empty"
     store_latest_test_output(expected_output, test_output)
 
     expected_output = parse_jsonl(expected_output_path)
 
     result = get_difference(test_output, expected_output)
 
     assert (
         result["difference"][0] == result["difference"][1]
     ), f"Missmatch in event at line {result['event_line_no']}!"
+
+
+def set_config(config_template, specific_rules, generic_rules, schema):
+    config_template["pipeline"][0]["labelername"]["schema"] = os.path.join("tests/testdata", schema)
+    config_template["pipeline"][0]["labelername"]["specific_rules"] = [
+        os.path.join("tests/testdata", rule) for rule in specific_rules
+    ]
+    config_template["pipeline"][0]["labelername"]["generic_rules"] = [
+        os.path.join("tests/testdata", rule) for rule in generic_rules
+    ]
```

### Comparing `logprep-6.0.0/tests/acceptance/test_wineventlog_pseudonymization.py` & `logprep-6.1.0/tests/acceptance/test_wineventlog_pseudonymization.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/acceptance/util.py` & `logprep-6.1.0/tests/acceptance/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,19 +258,19 @@
     )
 
 
 def wait_for_output(proc, expected_output, test_timeout=10):
     @timeout(test_timeout)
     def wait_for_output_inner(proc, expected_output):
         output = proc.stdout.readline()
-        while expected_output not in output.decode("utf8"):
+        while not re.search(expected_output, output.decode("utf8")):
             output = proc.stdout.readline()
-            time.sleep(0.1)  # nosemgrep
 
     wait_for_output_inner(proc, expected_output)
+    time.sleep(0.1)  # nosemgrep
 
 
 def stop_logprep(proc=None):
     if proc:
         proc.send_signal(signal.SIGINT)
         try:
             wait_for_output(proc, "Shutdown complete", test_timeout=10)
```

### Comparing `logprep-6.0.0/tests/ci/runner-image/scripts/compare_json.py` & `logprep-6.1.0/tests/ci/runner-image/scripts/compare_json.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/testdata/ConfigurationForTest.py` & `logprep-6.1.0/tests/testdata/ConfigurationForTest.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/testdata/FilledTempFile.py` & `logprep-6.1.0/tests/testdata/FilledTempFile.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/testdata/metadata.py` & `logprep-6.1.0/tests/testdata/metadata.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/testdata/ruledata.py` & `logprep-6.1.0/tests/testdata/ruledata.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/testdata/unit/clusterer/test_data.py` & `logprep-6.1.0/tests/testdata/unit/clusterer/test_data.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/connector/base.py` & `logprep-6.1.0/tests/unit/connector/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,51 +1,38 @@
 # pylint: disable=missing-docstring
 # pylint: disable=protected-access
 import base64
 import json
 import zlib
-from abc import ABC
 from copy import deepcopy
 from logging import getLogger
-from typing import Iterable
 from unittest import mock
 
 import arrow
 
 from logprep.abc.connector import Connector
 from logprep.abc.input import Input
 from logprep.abc.output import Output
 from logprep.factory import Factory
-from logprep.util.helper import camel_to_snake
 from logprep.util.time_measurement import TimeMeasurement
+from tests.unit.component.base import BaseComponentTestCase
 
 
-class BaseConnectorTestCase(ABC):
+class BaseConnectorTestCase(BaseComponentTestCase):
     CONFIG: dict = {}
     object: Connector = None
     logger = getLogger()
 
     def setup_method(self) -> None:
         config = {"Test Instance Name": self.CONFIG}
         self.object = Factory.create(configuration=config, logger=self.logger)
 
     def test_is_a_connector_implementation(self):
         assert isinstance(self.object, Connector)
 
-    def test_uses_python_slots(self):
-        assert isinstance(self.object.__slots__, Iterable)
-
-    def test_describe(self):
-        describe_string = self.object.describe()
-        expected_base_description = f"{self.object.__class__.__name__} (Test Instance Name)"
-        assert describe_string.startswith(expected_base_description)
-
-    def test_snake_type(self):
-        assert str(self.object) == camel_to_snake(self.object.__class__.__name__)
-
 
 class BaseInputTestCase(BaseConnectorTestCase):
     def test_is_input_instance(self):
         assert isinstance(self.object, Input)
 
     def test_get_next_returns_event(self):
         return_value = ({"message": "test message"}, b'{"message": "test message"}')
@@ -113,19 +100,19 @@
         processed_event, non_critical_error_msg = connector._add_hmac_to(
             {"message": "test message"}, None
         )
         assert non_critical_error_msg is None
         assert processed_event.get("Hmac")
         calculated_hmac = processed_event.get("Hmac").get("hmac")
         assert (
-            calculated_hmac == "142454394037b655ec0663867172738319dbdbe669dedb7ccf8a69875f9fcd08"
+            calculated_hmac == "8b2d75efcba66476e5551d44065128bacff2f090db5b08d7a0201c33e3f651f5"
         ), f"Wrong hmac: '{calculated_hmac}'"
         calculated_compression = processed_event.get("Hmac").get("compressed_base64")
         assert (
-            calculated_compression == "eJyrVspNLS5OTE9VslJQKkktLlGA8WsBg/YJhQ=="
+            calculated_compression == "eJyrVspNLS5OTE9VslIqSS0uUYBxawF+Fwll"
         ), f"Wrong compression: {calculated_compression}"
 
     def test_get_next_with_hmac_of_raw_message(self):
         connector_config = deepcopy(self.CONFIG)
         connector_config.update(
             {
                 "preprocessing": {
```

### Comparing `logprep-6.0.0/tests/unit/connector/test_confluent_kafka_common.py` & `logprep-6.1.0/tests/unit/connector/test_confluent_kafka_common.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/connector/test_confluent_kafka_input.py` & `logprep-6.1.0/tests/unit/connector/test_confluent_kafka_input.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,18 +5,21 @@
 # pylint: disable=attribute-defined-outside-init
 # pylint: disable=no-self-use
 from copy import deepcopy
 from unittest import mock
 
 import pytest
 
-from logprep.factory import Factory
 from logprep.abc.input import CriticalInputError
+from logprep.abc.output import FatalOutputError
+from logprep.factory import Factory
 from tests.unit.connector.base import BaseInputTestCase
-from tests.unit.connector.test_confluent_kafka_common import CommonConfluentKafkaTestCase
+from tests.unit.connector.test_confluent_kafka_common import (
+    CommonConfluentKafkaTestCase,
+)
 
 
 class TestConfluentKafkaInput(BaseInputTestCase, CommonConfluentKafkaTestCase):
     CONFIG = {
         "type": "confluentkafka_input",
         "bootstrapservers": ["testserver:9092"],
         "topic": "test_input_raw",
@@ -61,16 +64,20 @@
     def test_get_next_raises_critical_input_exception_for_invalid_confluent_kafka_record(self, _):
         mock_record = mock.MagicMock()
         mock_record.error = mock.MagicMock(return_value="An arbitrary confluent-kafka error")
         mock_record.value = mock.MagicMock(return_value=None)
         self.object._consumer.poll = mock.MagicMock(return_value=mock_record)
         with pytest.raises(
             CriticalInputError,
-            match=r"A confluent-kafka record contains an error code: "
-            r"\(An arbitrary confluent-kafka error\)",
+            match=(
+                r"CriticalInputError in ConfluentKafkaInput \(Test Instance Name\) - "
+                r"Kafka Input: testserver:9092: "
+                r"A confluent-kafka record contains an error code -> "
+                r"An arbitrary confluent-kafka error"
+            ),
         ):
             _, _ = self.object.get_next(1)
 
     @mock.patch("logprep.connector.confluent_kafka.input.Consumer")
     def test_shut_down_calls_consumer_close(self, _):
         kafka_consumer = self.object._consumer
         self.object.shut_down()
@@ -131,7 +138,22 @@
         mock_record.error = mock.MagicMock()
         mock_record.error.return_value = None
         self.object._consumer.poll = mock.MagicMock(return_value=mock_record)
         mock_record.value = mock.MagicMock()
         mock_record.value.return_value = '{"element":"in list"}'.encode("utf8")
         result = self.object._get_raw_event(0.001)
         assert result
+
+    @mock.patch("logprep.connector.confluent_kafka.input.Consumer")
+    def test_logprep_config_has_precedence(self, mock_consumer):
+        kafka_config = deepcopy(self.object._confluent_settings)
+        config = {"bootstrap.servers": "bootstrap1, myprivatebootstrap"}
+        self.object._config.kafka_config = config
+        self.object._consumer.clear()
+        _ = self.object._consumer
+        mock_consumer.assert_called_with(kafka_config)
+
+    def test_setup_raises_fatal_output_error_on_invalid_config(self):
+        config = {"myconfig": "the config"}
+        self.object._config.kafka_config = config
+        with pytest.raises(FatalOutputError, match="No such configuration property"):
+            self.object.setup()
```

### Comparing `logprep-6.0.0/tests/unit/connector/test_confluent_kafka_output.py` & `logprep-6.1.0/tests/unit/connector/test_confluent_kafka_output.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,22 +2,25 @@
 # pylint: disable=protected-access
 # pylint: disable=wrong-import-position
 # pylint: disable=wrong-import-order
 # pylint: disable=attribute-defined-outside-init
 # pylint: disable=no-self-use
 
 import json
+from copy import deepcopy
 from unittest import mock
 
 import pytest
 
-from logprep.abc.output import CriticalOutputError
+from logprep.abc.output import CriticalOutputError, FatalOutputError
 from logprep.factory import Factory
 from tests.unit.connector.base import BaseOutputTestCase
-from tests.unit.connector.test_confluent_kafka_common import CommonConfluentKafkaTestCase
+from tests.unit.connector.test_confluent_kafka_common import (
+    CommonConfluentKafkaTestCase,
+)
 
 
 class TestConfluentKafkaOutput(BaseOutputTestCase, CommonConfluentKafkaTestCase):
     CONFIG = {
         "type": "confluentkafka_output",
         "bootstrapservers": ["testserver:9092"],
         "topic": "test_input_raw",
@@ -109,23 +112,50 @@
     @mock.patch("logprep.connector.confluent_kafka.output.Producer")
     def test_shut_down_calls_producer_flush(self, _):
         kafka_producer = self.object._producer
         self.object.shut_down()
         kafka_producer.flush.assert_called()
 
     @mock.patch("logprep.connector.confluent_kafka.output.Producer")
-    def test_create_confluent_settings_contains_expected_values2(self, _):
-        self.object._producer.produce.side_effect = BaseException
-        with pytest.raises(CriticalOutputError, match=r"Error storing output document:"):
+    def test_raises_critical_output_on_any_exception(self, _):
+        self.object._producer.produce.side_effect = [
+            BaseException("bad things happened"),
+            None,
+            None,
+        ]
+        self.object.store_failed = mock.MagicMock()
+        with pytest.raises(
+            CriticalOutputError,
+            match=r"CriticalOutputError in ConfluentKafkaOutput"
+            r" \(Test Instance Name\) - Kafka Output: testserver:9092: "
+            r"Error storing output document -> bad things happened for event: "
+            r"\{'message': 'test message'\}",
+        ):
             self.object.store({"message": "test message"})
+        self.object.store_failed.assert_called()
 
     @mock.patch("logprep.connector.confluent_kafka.output.Producer")
     def test_store_counts_processed_events(self, _):  # pylint: disable=arguments-differ
         assert self.object.metrics.number_of_processed_events == 0
         self.object.store({"message": "my event message"})
         assert self.object.metrics.number_of_processed_events == 1
 
     @mock.patch("logprep.connector.confluent_kafka.output.Producer")
     def test_store_calls_batch_finished_callback(self, _):  # pylint: disable=arguments-differ
         self.object.input_connector = mock.MagicMock()
         self.object.store({"message": "my event message"})
         self.object.input_connector.batch_finished_callback.assert_called()
+
+    @mock.patch("logprep.connector.confluent_kafka.output.Producer")
+    def test_logprep_config_has_precedence(self, mock_producer):
+        kafka_config = deepcopy(self.object._confluent_settings)
+        config = {"bootstrap.servers": "bootstrap1, myprivatebootstrap"}
+        self.object._config.kafka_config = config
+        self.object._producer.clear()
+        _ = self.object._producer
+        mock_producer.assert_called_with(kafka_config)
+
+    def test_setup_raises_fatal_output_error_on_invalid_config(self):
+        config = {"myconfig": "the config"}
+        self.object._config.kafka_config = config
+        with pytest.raises(FatalOutputError, match="No such configuration property"):
+            self.object.setup()
```

### Comparing `logprep-6.0.0/tests/unit/connector/test_console_output.py` & `logprep-6.1.0/tests/unit/connector/test_console_output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/connector/test_dummy_input.py` & `logprep-6.1.0/tests/unit/connector/test_dummy_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/connector/test_dummy_output.py` & `logprep-6.1.0/tests/unit/connector/test_dummy_output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/connector/test_elasticsearch_output.py` & `logprep-6.1.0/tests/unit/connector/test_opensearch_output.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,67 +1,55 @@
 # pylint: disable=missing-docstring
 # pylint: disable=protected-access
 # pylint: disable=wrong-import-position
 # pylint: disable=wrong-import-order
 # pylint: disable=attribute-defined-outside-init
 # pylint: disable=no-self-use
-from copy import deepcopy
 import json
 import re
-import pytest
 from datetime import datetime
-from json import loads, dumps
 from math import isclose
 from unittest import mock
 
 import arrow
-import elasticsearch
-import elasticsearch.helpers
+import opensearchpy as search
+import pytest
+from opensearchpy import OpenSearchException as SearchException
+from opensearchpy import helpers
 
-from logprep.factory import Factory
-from logprep.abc.output import CriticalOutputError, FatalOutputError
+from logprep.abc.component import Component
+from logprep.abc.output import FatalOutputError
 from tests.unit.connector.base import BaseOutputTestCase
 
 
 class NotJsonSerializableMock:
     pass
 
 
-def mock_bulk(
-    _, documents: list, max_retries: int = 0, chunk_size: int = 500
-):  # pylint: disable=unused-argument
-    for document in documents:
-        try:
-            loads(dumps(document))
-        except TypeError as error:
-            raise CriticalOutputError(
-                "Error storing output document: Serialization Error", document
-            ) from error
-
+helpers.bulk = mock.MagicMock()
 
-elasticsearch.helpers.bulk = mock_bulk
 
-
-class TestElasticsearchOutput(BaseOutputTestCase):
+class TestOpenSearchOutput(BaseOutputTestCase):
     CONFIG = {
-        "type": "elasticsearch_output",
+        "type": "opensearch_output",
         "hosts": ["host:123"],
         "default_index": "default_index",
         "error_index": "error_index",
         "message_backlog_size": 1,
         "timeout": 5000,
     }
 
-    def test_describe_returns_elasticsearch_output(self):
+    def test_describe_returns_output(self):
         assert (
             self.object.describe()
-            == "ElasticsearchOutput (Test Instance Name) - ElasticSearch Output: ['host:123']"
+            == "OpensearchOutput (Test Instance Name) - Opensearch Output: ['host:123']"
         )
 
     def test_store_sends_to_default_index(self):
+        self.object._config.message_backlog_size = 2
         event = {"field": "content"}
         expected = {
             "_index": "default_index",
             "message": '{"field": "content"}',
             "reason": "Missing index in document",
         }
         self.object.store(event)
@@ -76,26 +64,26 @@
         formatted_date = arrow.now().format("YYYY-MM-DD")
         expected_index = re.sub(r"%{YYYY-MM-DD}", formatted_date, default_index)
         expected = {
             "_index": expected_index,
             "message": '{"field": "content"}',
             "reason": "Missing index in document",
         }
-        es_config = deepcopy(self.CONFIG)
-        es_config.update({"default_index": default_index})
-        es_output = Factory.create({"elasticsearch": es_config}, self.logger)
-        es_output.store(event)
+        self.object._config.default_index = default_index
+        self.object._config.message_backlog_size = 2
+        self.object.store(event)
 
-        assert es_output._message_backlog[0].pop("@timestamp")
-        assert es_output._message_backlog[0] == expected
+        assert self.object._message_backlog[0].pop("@timestamp")
+        assert self.object._message_backlog[0] == expected
 
     def test_store_custom_sends_event_to_expected_index(self):
         custom_index = "custom_index"
         event = {"field": "content"}
         expected = {"field": "content", "_index": custom_index}
+        self.object._config.message_backlog_size = 2
         self.object.store_custom(event, custom_index)
         assert self.object._message_backlog[0] == expected
 
     def test_store_failed(self):
         error_index = "error_index"
         event_received = {"field": "received"}
         event = {"field": "content"}
@@ -104,14 +92,15 @@
             "error": error_message,
             "original": event_received,
             "processed": event,
             "_index": error_index,
             "@timestamp": str(datetime.now()),
         }
 
+        self.object._config.message_backlog_size = 2
         self.object.store_failed(error_message, event_received, event)
 
         error_document = self.object._message_backlog[0]
         # timestamp is compared to be approximately the same,
         # since it is variable and then removed to compare the rest
         error_time = datetime.timestamp(arrow.get(error_document["@timestamp"]).datetime)
         expected_time = datetime.timestamp(arrow.get(error_document["@timestamp"]).datetime)
@@ -143,57 +132,60 @@
         failed_document = self.object._build_failed_index_document(
             {"foo": "bar"}, "A reason for failed indexing"
         )
         assert failed_document.pop("@timestamp")
         assert failed_document == expected
 
     @mock.patch(
-        "logprep.connector.elasticsearch.output.helpers.bulk",
-        side_effect=elasticsearch.SerializationError,
+        "opensearchpy.helpers.bulk",
+        side_effect=search.SerializationError,
     )
     def test_write_to_search_context_calls_handle_serialization_error_if_serialization_error(
         self, _
     ):
+        self.object._config.message_backlog_size = 1
         self.object._handle_serialization_error = mock.MagicMock()
         self.object._write_to_search_context({"dummy": "event"})
         self.object._handle_serialization_error.assert_called()
 
     @mock.patch(
-        "logprep.connector.elasticsearch.output.helpers.bulk",
-        side_effect=elasticsearch.ConnectionError,
+        "opensearchpy.helpers.bulk",
+        side_effect=search.ConnectionError,
     )
     def test_write_to_search_context_calls_handle_connection_error_if_connection_error(self, _):
+        self.object._config.message_backlog_size = 1
         self.object._handle_connection_error = mock.MagicMock()
         self.object._write_to_search_context({"dummy": "event"})
         self.object._handle_connection_error.assert_called()
 
     @mock.patch(
-        "logprep.connector.elasticsearch.output.helpers.bulk",
-        side_effect=elasticsearch.helpers.BulkIndexError,
+        "opensearchpy.helpers.bulk",
+        side_effect=helpers.BulkIndexError,
     )
     def test_write_to_search_context_calls_handle_bulk_index_error_if_bulk_index_error(self, _):
+        self.object._config.message_backlog_size = 1
         self.object._handle_bulk_index_error = mock.MagicMock()
         self.object._write_to_search_context({"dummy": "event"})
         self.object._handle_bulk_index_error.assert_called()
 
-    @mock.patch("logprep.connector.elasticsearch.output.helpers.bulk")
+    @mock.patch("opensearchpy.helpers.bulk")
     def test__handle_bulk_index_error_calls_bulk(self, fake_bulk):
         mock_bulk_index_error = mock.MagicMock()
         mock_bulk_index_error.errors = [
             {
                 "index": {
                     "data": {"my": "document"},
                     "error": {"type": "myerrortype", "reason": "myreason"},
                 }
             }
         ]
         self.object._handle_bulk_index_error(mock_bulk_index_error)
         fake_bulk.assert_called()
 
-    @mock.patch("logprep.connector.elasticsearch.output.helpers.bulk")
+    @mock.patch("opensearchpy.helpers.bulk")
     def test_handle_bulk_index_error_calls_bulk_with_error_documents(self, fake_bulk):
         mock_bulk_index_error = mock.MagicMock()
         mock_bulk_index_error.errors = [
             {
                 "index": {
                     "data": {"my": "document"},
                     "error": {"type": "myerrortype", "reason": "myreason"},
@@ -206,28 +198,40 @@
         assert "reason" in error_document
         assert "@timestamp" in error_document
         assert "_index" in error_document
         assert "message" in error_document
         assert error_document.get("reason") == "myerrortype: myreason"
         assert error_document.get("message") == json.dumps({"my": "document"})
 
-    def test_write_to_search_context_sets_processed_cnt(self):
-        es_config = deepcopy(self.CONFIG)
-        es_config.update({"message_backlog_size": 2})
-        es_output = Factory.create({"elasticsearch": es_config}, self.logger)
-        current_proccessed_cnt = es_output._processed_cnt
-        es_output._write_to_search_context({"dummy": "event"})
-        assert current_proccessed_cnt < es_output._processed_cnt
-
     def test_handle_connection_error_raises_fatal_output_error(self):
         with pytest.raises(FatalOutputError):
             self.object._handle_connection_error(mock.MagicMock())
 
     def test_handle_serialization_error_raises_fatal_output_error(self):
         with pytest.raises(FatalOutputError):
             self.object._handle_serialization_error(mock.MagicMock())
 
-    def test_setup_raises_fatal_output_error_if_unauthenticated(self):
+    def test_setup_raises_fatal_output_error_if_opensearch_error_is_raised(self):
         self.object._search_context.info = mock.MagicMock()
-        self.object._search_context.info.side_effect = elasticsearch.AuthenticationException
+        self.object._search_context.info.side_effect = SearchException
+        with pytest.raises(FatalOutputError):
+            self.object.setup()
+
+    def test_setup_registers_flush_timout_tasks(self):
+        job_count = len(Component._scheduler.jobs)
         with pytest.raises(FatalOutputError):
             self.object.setup()
+        assert len(Component._scheduler.jobs) == job_count + 1
+
+    def test_message_backlog_is_not_written_if_message_backlog_size_not_reached(self):
+        self.object._config.message_backlog_size = 2
+        assert len(self.object._message_backlog) == 0
+        with mock.patch(
+            "logprep.connector.opensearch.output.OpensearchOutput._write_backlog"
+        ) as mock_write_backlog:
+            self.object.store({"test": "event"})
+        mock_write_backlog.assert_not_called()
+
+    def test_message_backlog_is_cleared_after_it_was_written(self):
+        self.object._config.message_backlog_size = 1
+        self.object.store({"event": "test_event"})
+        assert len(self.object._message_backlog) == 0
```

### Comparing `logprep-6.0.0/tests/unit/connector/test_file_input_default_config.py` & `logprep-6.1.0/tests/unit/connector/test_file_input_default_config.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/connector/test_file_input_not_tailing_config.py` & `logprep-6.1.0/tests/unit/connector/test_file_input_not_tailing_config.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/connector/test_file_input_start_at_end_config.py` & `logprep-6.1.0/tests/unit/connector/test_file_input_start_at_end_config.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/connector/test_http_input.py` & `logprep-6.1.0/tests/unit/connector/test_http_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/connector/test_json_input.py` & `logprep-6.1.0/tests/unit/connector/test_json_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/connector/test_jsonl_input.py` & `logprep-6.1.0/tests/unit/connector/test_jsonl_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/connector/test_jsonl_output.py` & `logprep-6.1.0/tests/unit/connector/test_jsonl_output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/connector/test_opensearch_output.py` & `logprep-6.1.0/tests/unit/connector/test_elasticsearch_output.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,79 +1,55 @@
 # pylint: disable=missing-docstring
 # pylint: disable=protected-access
 # pylint: disable=wrong-import-position
 # pylint: disable=wrong-import-order
 # pylint: disable=attribute-defined-outside-init
 # pylint: disable=no-self-use
-from copy import deepcopy
 import json
 import re
-import pytest
 from datetime import datetime
-from json import loads, dumps
 from math import isclose
 from unittest import mock
 
 import arrow
-import opensearchpy
-import opensearchpy.helpers
+import elasticsearch as search
+import pytest
+from elasticsearch import ElasticsearchException as SearchException
+from elasticsearch import helpers
 
-from logprep.abc.output import CriticalOutputError, FatalOutputError
-from logprep.factory import Factory
+from logprep.abc.component import Component
+from logprep.abc.output import FatalOutputError
 from tests.unit.connector.base import BaseOutputTestCase
 
 
 class NotJsonSerializableMock:
     pass
 
 
-def mock_bulk(
-    _, documents: list, max_retries: int = 0, chunk_size: int = 500
-):  # pylint: disable=unused-argument
-    for document in documents:
-        try:
-            loads(dumps(document))
-        except TypeError as error:
-            raise CriticalOutputError(
-                "Error storing output document: Serialization Error", document
-            ) from error
-
-
-opensearchpy.helpers.bulk = mock_bulk
-
-
-class TestOpenSearchOutput(BaseOutputTestCase):
-    # def setup_method(self, _):
-    #     self.os_output = OpenSearchOutput(
-    #         ["host:123"], "default_index", "error_index", 1, 5000, 0, None, None, None, None
-    #     )
+helpers.bulk = mock.MagicMock()
 
+
+class TestElasticsearchOutput(BaseOutputTestCase):
     CONFIG = {
-        "type": "opensearch_output",
+        "type": "elasticsearch_output",
         "hosts": ["host:123"],
         "default_index": "default_index",
         "error_index": "error_index",
         "message_backlog_size": 1,
         "timeout": 5000,
     }
 
-    def test_describe_returns_opensearch_output(self):
-        assert (
-            self.object.describe()
-            == "OpensearchOutput (Test Instance Name) - Opensearch Output: ['host:123']"
-        )
-
-    def test_store_sends_event_to_expected_index_if_index_missing_in_event(self):
+    def test_store_sends_to_default_index(self):
+        self.object._config.message_backlog_size = 2
         event = {"field": "content"}
         expected = {
             "_index": "default_index",
             "message": '{"field": "content"}',
             "reason": "Missing index in document",
         }
-
         self.object.store(event)
 
         assert self.object._message_backlog[0].pop("@timestamp")
         assert self.object._message_backlog[0] == expected
 
     def test_store_sends_event_to_expected_index_with_date_pattern_if_index_missing_in_event(self):
         default_index = "default_index-%{YYYY-MM-DD}"
@@ -82,58 +58,57 @@
         formatted_date = arrow.now().format("YYYY-MM-DD")
         expected_index = re.sub(r"%{YYYY-MM-DD}", formatted_date, default_index)
         expected = {
             "_index": expected_index,
             "message": '{"field": "content"}',
             "reason": "Missing index in document",
         }
-        os_config = deepcopy(self.CONFIG)
-        os_config.update({"default_index": default_index})
-        os_output = Factory.create({"elasticsearch": os_config}, self.logger)
-        os_output.store(event)
-        assert os_output._message_backlog[0].pop("@timestamp")
-        assert os_output._message_backlog[0] == expected
+        self.object._config.default_index = default_index
+        self.object._config.message_backlog_size = 2
+        self.object.store(event)
+
+        assert self.object._message_backlog[0].pop("@timestamp")
+        assert self.object._message_backlog[0] == expected
 
     def test_store_custom_sends_event_to_expected_index(self):
         custom_index = "custom_index"
         event = {"field": "content"}
-
         expected = {"field": "content", "_index": custom_index}
+        self.object._config.message_backlog_size = 2
         self.object.store_custom(event, custom_index)
-
         assert self.object._message_backlog[0] == expected
 
     def test_store_failed(self):
         error_index = "error_index"
         event_received = {"field": "received"}
         event = {"field": "content"}
         error_message = "error message"
-
         expected = {
             "error": error_message,
             "original": event_received,
             "processed": event,
             "_index": error_index,
             "@timestamp": str(datetime.now()),
         }
 
+        self.object._config.message_backlog_size = 2
         self.object.store_failed(error_message, event_received, event)
 
         error_document = self.object._message_backlog[0]
         # timestamp is compared to be approximately the same,
         # since it is variable and then removed to compare the rest
         error_time = datetime.timestamp(arrow.get(error_document["@timestamp"]).datetime)
         expected_time = datetime.timestamp(arrow.get(error_document["@timestamp"]).datetime)
         assert isclose(error_time, expected_time)
         del error_document["@timestamp"]
         del expected["@timestamp"]
 
         assert error_document == expected
 
-    def test_create_os_output_settings_contains_expected_values(self):
+    def test_create_es_output_settings_contains_expected_values(self):
         expected = {
             "reason": "A reason for failed indexing",
             "_index": "default_index",
         }
         failed_document = self.object._build_failed_index_document(
             {"invalid_json": NotJsonSerializableMock(), "something_valid": "im_valid!"},
             "A reason for failed indexing",
@@ -144,80 +119,68 @@
 
     def test_build_failed_index_document(self):
         expected = {
             "reason": "A reason for failed indexing",
             "message": '{"foo": "bar"}',
             "_index": "default_index",
         }
-
         failed_document = self.object._build_failed_index_document(
             {"foo": "bar"}, "A reason for failed indexing"
         )
         assert failed_document.pop("@timestamp")
         assert failed_document == expected
 
     @mock.patch(
-        "logprep.connector.opensearch.output.opensearch.helpers.bulk",
-        side_effect=opensearchpy.SerializationError,
+        "elasticsearch.helpers.bulk",
+        side_effect=search.SerializationError,
     )
     def test_write_to_search_context_calls_handle_serialization_error_if_serialization_error(
         self, _
     ):
+        self.object._config.message_backlog_size = 1
         self.object._handle_serialization_error = mock.MagicMock()
         self.object._write_to_search_context({"dummy": "event"})
         self.object._handle_serialization_error.assert_called()
 
     @mock.patch(
-        "logprep.connector.opensearch.output.opensearch.helpers.bulk",
-        side_effect=opensearchpy.ConnectionError,
+        "elasticsearch.helpers.bulk",
+        side_effect=search.ConnectionError,
     )
     def test_write_to_search_context_calls_handle_connection_error_if_connection_error(self, _):
+        self.object._config.message_backlog_size = 1
         self.object._handle_connection_error = mock.MagicMock()
         self.object._write_to_search_context({"dummy": "event"})
         self.object._handle_connection_error.assert_called()
 
     @mock.patch(
-        "logprep.connector.opensearch.output.opensearch.helpers.bulk",
-        side_effect=opensearchpy.helpers.BulkIndexError,
+        "elasticsearch.helpers.bulk",
+        side_effect=helpers.BulkIndexError,
     )
     def test_write_to_search_context_calls_handle_bulk_index_error_if_bulk_index_error(self, _):
+        self.object._config.message_backlog_size = 1
         self.object._handle_bulk_index_error = mock.MagicMock()
         self.object._write_to_search_context({"dummy": "event"})
         self.object._handle_bulk_index_error.assert_called()
 
-    @mock.patch("logprep.connector.opensearch.output.opensearch.helpers.bulk")
+    @mock.patch("elasticsearch.helpers.bulk")
     def test__handle_bulk_index_error_calls_bulk(self, fake_bulk):
         mock_bulk_index_error = mock.MagicMock()
         mock_bulk_index_error.errors = [
             {
                 "index": {
                     "data": {"my": "document"},
                     "error": {"type": "myerrortype", "reason": "myreason"},
                 }
             }
         ]
         self.object._handle_bulk_index_error(mock_bulk_index_error)
         fake_bulk.assert_called()
 
-    @mock.patch("logprep.connector.opensearch.output.opensearch.helpers.bulk")
-    def test__handle_bulk_index_error_calls_bulk_for_special_op_type(self, fake_bulk):
-        mock_bulk_index_error = mock.MagicMock()
-        mock_bulk_index_error.errors = [
-            {
-                "create": {
-                    "data": {"my": "document"},
-                    "error": {"type": "myerrortype", "reason": "myreason"},
-                }
-            }
-        ]
-        self.object._handle_bulk_index_error(mock_bulk_index_error)
-        fake_bulk.assert_called()
-
-    @mock.patch("logprep.connector.opensearch.output.opensearch.helpers.bulk")
-    def test__handle_bulk_index_error_calls_bulk_with_error_documents(self, fake_bulk):
+    @mock.patch("elasticsearch.helpers.bulk")
+    def test_handle_bulk_index_error_calls_bulk_with_error_documents(self, fake_bulk):
         mock_bulk_index_error = mock.MagicMock()
         mock_bulk_index_error.errors = [
             {
                 "index": {
                     "data": {"my": "document"},
                     "error": {"type": "myerrortype", "reason": "myreason"},
                 }
@@ -229,28 +192,40 @@
         assert "reason" in error_document
         assert "@timestamp" in error_document
         assert "_index" in error_document
         assert "message" in error_document
         assert error_document.get("reason") == "myerrortype: myreason"
         assert error_document.get("message") == json.dumps({"my": "document"})
 
-    def test_write_to_es_sets_processed_cnt(self):
-        os_config = deepcopy(self.CONFIG)
-        os_config.update({"message_backlog_size": 2})
-        os_output = Factory.create({"opensearch": os_config}, self.logger)
-        current_proccessed_cnt = os_output._processed_cnt
-        os_output._write_to_search_context({"dummy": "event"})
-        assert current_proccessed_cnt < os_output._processed_cnt
-
     def test_handle_connection_error_raises_fatal_output_error(self):
         with pytest.raises(FatalOutputError):
             self.object._handle_connection_error(mock.MagicMock())
 
     def test_handle_serialization_error_raises_fatal_output_error(self):
         with pytest.raises(FatalOutputError):
             self.object._handle_serialization_error(mock.MagicMock())
 
-    def test_setup_raises_fatal_output_error_if_unauthenticated(self):
+    def test_setup_raises_fatal_output_error_if_elastic_error_is_raised(self):
         self.object._search_context.info = mock.MagicMock()
-        self.object._search_context.info.side_effect = opensearchpy.AuthenticationException
+        self.object._search_context.info.side_effect = SearchException
         with pytest.raises(FatalOutputError):
             self.object.setup()
+
+    def test_setup_registers_flush_timout_tasks(self):
+        job_count = len(Component._scheduler.jobs)
+        with pytest.raises(FatalOutputError):
+            self.object.setup()
+        assert len(Component._scheduler.jobs) == job_count + 1
+
+    def test_message_backlog_is_not_written_if_message_backlog_size_not_reached(self):
+        self.object._config.message_backlog_size = 2
+        assert len(self.object._message_backlog) == 0
+        with mock.patch(
+            "logprep.connector.elasticsearch.output.ElasticsearchOutput._write_backlog"
+        ) as mock_write_backlog:
+            self.object.store({"test": "event"})
+        mock_write_backlog.assert_not_called()
+
+    def test_message_backlog_is_cleared_after_it_was_written(self):
+        self.object._config.message_backlog_size = 1
+        self.object.store({"event": "test_event"})
+        assert len(self.object._message_backlog) == 0
```

### Comparing `logprep-6.0.0/tests/unit/filter/test_filter_expression.py` & `logprep-6.1.0/tests/unit/filter/test_filter_expression.py`

 * *Files 3% similar despite different names*

```diff
@@ -404,14 +404,41 @@
                 {
                     "key1": {
                         "key2": "start" + "".join(sample(digits + ascii_letters, length)) + "end"
                     }
                 }
             )
 
+    @pytest.mark.parametrize(
+        "filter_expression, expected_expression",
+        [
+            (r"*", r"^.*$"),
+            (r"?", r"^.?$"),
+            (r"(*)", r"^\(.*\)$"),
+            (r"(?)", r"^\(.?\)$"),
+            (r"**", r"^.*.*$"),
+            (r"??", r"^.?.?$"),
+            (r"start*end", r"^start.*end$"),
+            (r"start**end", r"^start.*.*end$"),
+            (r"start?end", r"^start.?end$"),
+            (r"\\", r"^\\\\$"),
+            (r"\\\\", r"^\\\\\\\\$"),
+            (r"\*", r"^\*$"),
+            (r"\\*", r"^\\.*$"),
+            (r"\\\*", r"^\\\\.*$"),
+            (r"\\\\*", r"^\\\\\\.*$"),
+            (r'"', r'^"$'),
+            (r"\"", r'^\\"$'),
+            (r'\\"', r'^\\\\"$'),
+        ],
+    )
+    def test_escaped_expected(self, filter_expression, expected_expression):
+        _filter = WildcardStringFilterExpression(["key1", "key2"], filter_expression)
+        assert _filter.escaped_expected == expected_expression
+
 
 class TestSigmaFilterExpression(ValueBasedFilterExpressionTest):
     def setup_method(self, _):
         self.value = "start*end"
         self.filter = SigmaFilterExpression(["key1", "key2"], self.value)
         self.filter_identical = SigmaFilterExpression(["key1", "key2"], self.value)
 
@@ -460,7 +487,37 @@
             assert not self.filter.matches(
                 {
                     "key1": {
                         "key2": "start" + "".join(sample(digits + ascii_letters, length)) + "end"
                     }
                 }
             )
+
+    @pytest.mark.parametrize(
+        "filter_expression, expected_expression",
+        [
+            (r"*", r"^.*$"),
+            (r"?", r"^.?$"),
+            (r"(*)", r"^\(.*\)$"),
+            (r"(?)", r"^\(.?\)$"),
+            (r"**", r"^.*.*$"),
+            (r"??", r"^.?.?$"),
+            (r"start*end", r"^start.*end$"),
+            (r"start**end", r"^start.*.*end$"),
+            (r"start?end", r"^start.?end$"),
+            (r"\\", r"^\\\\$"),
+            (r"\\\\", r"^\\\\\\\\$"),
+            (r"\*", r"^\*$"),
+            (r"\\*", r"^\\.*$"),
+            (r"\\\*", r"^\\\\.*$"),
+            (r"\\\\*", r"^\\\\\\.*$"),
+            (r'"', r'^"$'),
+            (r"\"", r'^\\"$'),
+            (r'\\"', r'^\\\\"$'),
+            (r'te"st', r'^te"st$'),
+            (r'te\\"st', r'^te\\\\"st$'),
+            (r'te\\"st"', r'^te\\\\"st"$'),
+        ],
+    )
+    def test_escaped_expected(self, filter_expression, expected_expression):
+        _filter = SigmaFilterExpression(["key1", "key2"], filter_expression)
+        assert _filter.escaped_expected == expected_expression
```

### Comparing `logprep-6.0.0/tests/unit/framework/rule_tree/test_node.py` & `logprep-6.1.0/tests/unit/framework/rule_tree/test_node.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/framework/rule_tree/test_rule_parser.py` & `logprep-6.1.0/tests/unit/framework/rule_tree/test_rule_parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,20 @@
-import pytest
+# pylint: disable=protected-access
+# pylint: disable=missing-docstring
+# pylint: disable=line-too-long
+# pylint: disable=too-many-statements
 
-pytest.importorskip("logprep.processor.pre_detector")
+import pytest
 
 from logprep.filter.expression.filter_expression import And, Or, StringFilterExpression, Not, Exists
 from logprep.framework.rule_tree.rule_parser import RuleParser as RP
 from logprep.processor.pre_detector.rule import PreDetectorRule
 
+pytest.importorskip("logprep.processor.pre_detector")
+
 str1 = StringFilterExpression(["key1"], "value1")
 str2 = StringFilterExpression(["key2"], "value2")
 str3 = StringFilterExpression(["key3"], "value3")
 str4 = StringFilterExpression(["key4"], "value4")
 str5 = StringFilterExpression(["key5", "subkey5"], "value5")
 
 ex1 = Exists(["ABC.def"])
@@ -460,14 +465,55 @@
                 Not(Not(Exists(["AImphash"]))),
                 Exists(["EventID"]),
                 StringFilterExpression(["EventID"], "15"),
                 Not(StringFilterExpression(["Imphash"], "000")),
             ]
         ]
 
+        rule = PreDetectorRule._create_from_dict(
+            {
+                "filter": "(A1 OR A2) AND (B1 OR B2) AND (C1 OR C2) AND (D1 OR D2)",
+                "pre_detector": {
+                    "id": 1,
+                    "title": "1",
+                    "severity": "0",
+                    "case_condition": "directly",
+                    "mitre": [],
+                },
+            }
+        )
+
+        parsed_rule = RP.parse_rule(rule, {}, {})
+        assert parsed_rule == [
+            [Exists(["A1"]), Exists(["B1"]), Exists(["C1"]), Exists(["D1"])],
+            [Exists(["A1"]), Exists(["B1"]), Exists(["C1"]), Exists(["D2"])],
+            [Exists(["A1"]), Exists(["B1"]), Exists(["C2"]), Exists(["D1"])],
+            [Exists(["A1"]), Exists(["B1"]), Exists(["C2"]), Exists(["D2"])],
+            [Exists(["A1"]), Exists(["B2"]), Exists(["C1"]), Exists(["D1"])],
+            [Exists(["A1"]), Exists(["B2"]), Exists(["C1"]), Exists(["D2"])],
+            [Exists(["A1"]), Exists(["B2"]), Exists(["C2"]), Exists(["D1"])],
+            [Exists(["A1"]), Exists(["B2"]), Exists(["C2"]), Exists(["D2"])],
+            [Exists(["A1"]), Exists(["C1"]), Exists(["D1"])],
+            [Exists(["A1"]), Exists(["C1"]), Exists(["D2"])],
+            [Exists(["A1"]), Exists(["C2"]), Exists(["D1"])],
+            [Exists(["A1"]), Exists(["C2"]), Exists(["D2"])],
+            [Exists(["A2"]), Exists(["B1"]), Exists(["C1"]), Exists(["D1"])],
+            [Exists(["A2"]), Exists(["B1"]), Exists(["C1"]), Exists(["D2"])],
+            [Exists(["A2"]), Exists(["B1"]), Exists(["C2"]), Exists(["D1"])],
+            [Exists(["A2"]), Exists(["B1"]), Exists(["C2"]), Exists(["D2"])],
+            [Exists(["A2"]), Exists(["B2"]), Exists(["C1"]), Exists(["D1"])],
+            [Exists(["A2"]), Exists(["B2"]), Exists(["C1"]), Exists(["D2"])],
+            [Exists(["A2"]), Exists(["B2"]), Exists(["C2"]), Exists(["D1"])],
+            [Exists(["A2"]), Exists(["B2"]), Exists(["C2"]), Exists(["D2"])],
+            [Exists(["A2"]), Exists(["C1"]), Exists(["D1"])],
+            [Exists(["A2"]), Exists(["C1"]), Exists(["D2"])],
+            [Exists(["A2"]), Exists(["C2"]), Exists(["D1"])],
+            [Exists(["A2"]), Exists(["C2"]), Exists(["D2"])],
+        ]
+
     def test_has_unresolved_not_expression(self):
         exp = And(str1, str2)
         assert not RP._has_unresolved_not_expression(exp)
 
         exp = Not(str1)
         assert not RP._has_unresolved_not_expression(exp)
 
@@ -482,14 +528,15 @@
 
         exp = Not(And(str1, str2))
         assert RP._has_unresolved_not_expression(exp)
 
         exp = Or(Not(And(str1, str2)), str3)
         assert RP._has_unresolved_not_expression(exp)
 
+    # pylint: disable=invalid-name
     def test_parse_NOT(self):
         exp = Not(str1)
         assert RP._parse_not_expression(exp) == exp
 
         exp = Not(Or(str1, str2))
         assert RP._parse_not_expression(exp) == And(Not(str1), Not(str2))
 
@@ -564,14 +611,16 @@
             [str2, str3],
             [str2, str4],
         ]
 
         exp = Or(And(str1, Or(str2, str3)), str4)
         assert RP._parse_or_expression(exp) == [[str1, str2], [str1, str3], [str4]]
 
+    # pylint: enable=invalid-name
+
     def test_has_or_expression(self):
         exp = And(str1, str2)
         assert not RP._has_or_expression(exp)
 
         exp = Or(str1, str2)
         assert RP._has_or_expression(exp)
```

### Comparing `logprep-6.0.0/tests/unit/framework/rule_tree/test_rule_tree.py` & `logprep-6.1.0/tests/unit/framework/rule_tree/test_rule_tree.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/framework/test_pipeline.py` & `logprep-6.1.0/tests/unit/framework/test_pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # pylint: disable=missing-docstring
 # pylint: disable=protected-access
 # pylint: disable=attribute-defined-outside-init
-import re
 from copy import deepcopy
 from logging import DEBUG, WARNING, getLogger
 from multiprocessing import Lock, active_children
 from unittest import mock
 
 import pytest
 import requests
@@ -14,26 +13,35 @@
 
 from logprep.abc.input import (
     CriticalInputError,
     FatalInputError,
     SourceDisconnectedError,
     WarningInputError,
 )
-from logprep.abc.output import CriticalOutputError, FatalOutputError, Output, WarningOutputError
+from logprep.abc.output import (
+    CriticalOutputError,
+    FatalOutputError,
+    Output,
+    WarningOutputError,
+)
 from logprep.abc.processor import Processor
 from logprep.factory import Factory
 from logprep.framework.pipeline import (
     MultiprocessingPipeline,
     MustProvideALogHandlerError,
     MustProvideAnMPLogHandlerError,
     Pipeline,
     SharedCounter,
 )
 from logprep.metrics.metric import MetricTargets
-from logprep.processor.base.exceptions import ProcessingWarning, ProcessingWarningCollection
+from logprep.processor.base.exceptions import (
+    ProcessingCriticalError,
+    ProcessingError,
+    ProcessingWarning,
+)
 from logprep.processor.deleter.rule import DeleterRule
 from logprep.util.getter import GetterFactory
 from logprep.util.multiprocessing_log_handler import MultiprocessingLogHandler
 
 original_create = Factory.create
 
 
@@ -136,15 +144,15 @@
         }
         deleter_processor = original_create(deleter_config, mock.MagicMock())
         deleter_rule = DeleterRule._create_from_dict(
             {"filter": "delete_me", "deleter": {"delete": True}}
         )
         deleter_processor._specific_tree.add_rule(deleter_rule)
         self.pipeline._pipeline = [mock.MagicMock(), deleter_processor, mock.MagicMock()]
-        self.pipeline._logger.setLevel(DEBUG)
+        self.pipeline.logger.setLevel(DEBUG)
         while self.pipeline._input._documents:
             self.pipeline.process_pipeline()
         assert len(input_data) == 0, "all events were processed"
         assert self.pipeline._pipeline[0].process.call_count == 3, "called for all events"
         assert self.pipeline._pipeline[2].process.call_count == 2, "not called for deleted event"
         assert {"delete_me": "2"} not in self.pipeline._output["dummy"].events
         assert len(self.pipeline._output["dummy"].events) == 2
@@ -183,19 +191,27 @@
         self.pipeline._shut_down()
         for _, output in self.pipeline._output.items():
             output.shut_down.assert_called()
 
     @mock.patch("logging.Logger.warning")
     def test_logs_source_disconnected_error_as_warning(self, mock_warning, _):
         self.pipeline._setup()
-        self.pipeline._input.get_next.side_effect = SourceDisconnectedError
+
+        def raise_source_disconnected_error(event):
+            raise SourceDisconnectedError(self.pipeline._input, "error occured")
+
+        self.pipeline._input = original_create(
+            {"dummy": {"type": "dummy_input", "documents": []}}, getLogger()
+        )
+        self.pipeline._input.get_next = raise_source_disconnected_error
+        assert self.pipeline._input.metrics.number_of_errors == 0
         self.pipeline.run()
-        mock_warning.assert_called()
-        assert re.search(
-            r"Lost or failed to establish connection to ", mock_warning.call_args[0][0]
+        assert self.pipeline._input.metrics.number_of_errors == 1
+        mock_warning.assert_called_with(
+            str(SourceDisconnectedError(self.pipeline._input, "error occured"))
         )
 
     def test_all_events_provided_by_input_arrive_at_output(self, _):
         self.pipeline._setup()
         self.pipeline._setup = mock.MagicMock()
         input_data = [{"test": "1"}, {"test": "2"}, {"test": "3"}]
         expected_output_data = deepcopy(input_data)
@@ -213,232 +229,238 @@
         self.pipeline._enable_iteration()
         assert self.pipeline._iterate()
 
         self.pipeline.stop()
         assert not self.pipeline._iterate()
 
     @mock.patch("logging.Logger.error")
-    def test_critical_input_error_is_logged_and_stored_as_failed(self, mock_error, _):
-        def raise_critical_input_error(event):
-            raise CriticalInputError("An error message", event)
-
-        self.pipeline._setup()
-        self.pipeline._input.get_next.side_effect = raise_critical_input_error
-        self.pipeline._output = {
-            "dummy": original_create({"dummy": {"type": "dummy_output"}}, mock.MagicMock())
-        }
-        self.pipeline.process_pipeline()
-        assert len(self.pipeline._output["dummy"].events) == 0
-        mock_error.assert_called()
-        assert re.search(
-            "A critical error occurred for input .*: An error message", mock_error.call_args[0][0]
-        )
-        assert len(self.pipeline._output["dummy"].failed_events) == 1
-
-    @mock.patch("logging.Logger.error")
     def test_critical_output_error_is_logged_and_stored_as_failed(self, mock_error, _):
-        def raise_critical_output_error(event):
-            raise CriticalOutputError("An error message", event)
-
         self.pipeline._setup()
         self.pipeline._input.get_next.return_value = ({"order": 1}, None)
-        self.pipeline._output["dummy"].store.side_effect = raise_critical_output_error
+        raised_error = CriticalOutputError(
+            self.pipeline._output["dummy"], "An error message", {"failed": "event"}
+        )
+        self.pipeline._output["dummy"].store.side_effect = raised_error
         self.pipeline.process_pipeline()
         self.pipeline._output["dummy"].store_failed.assert_called()
-        mock_error.assert_called()
-        assert re.search(
-            r"A critical error occurred for output .*: An error message", mock_error.call_args[0][0]
-        )
+        mock_error.assert_called_with(str(raised_error))
 
     @mock.patch("logging.Logger.warning")
     def test_input_warning_error_is_logged_but_processing_continues(self, mock_warning, _):
         self.pipeline._setup()
+
+        def raise_warning_error(_):
+            raise WarningInputError(self.pipeline._input, "i warn you")
+
         self.pipeline._input.metrics = mock.MagicMock()
         self.pipeline._input.metrics.number_of_warnings = 0
         self.pipeline._input.get_next.return_value = ({"order": 1}, None)
         self.pipeline.process_pipeline()
-        self.pipeline._input.get_next.side_effect = WarningInputError
+        self.pipeline._input.get_next.side_effect = raise_warning_error
         self.pipeline.process_pipeline()
         self.pipeline._input.get_next.side_effect = None
         self.pipeline.process_pipeline()
         assert self.pipeline._input.get_next.call_count == 3
-        assert mock_warning.call_count == 1
-        assert self.pipeline._output["dummy"].store.call_count == 2
         assert self.pipeline._input.metrics.number_of_warnings == 1
+        mock_warning.assert_called_with(str(WarningInputError(self.pipeline._input, "i warn you")))
+        assert self.pipeline._output["dummy"].store.call_count == 2
 
     @mock.patch("logging.Logger.warning")
     def test_output_warning_error_is_logged_but_processing_continues(self, mock_warning, _):
         self.pipeline._setup()
         self.pipeline._input.get_next.return_value = ({"order": 1}, None)
         self.pipeline._output["dummy"].metrics = mock.MagicMock()
         self.pipeline._output["dummy"].metrics.number_of_warnings = 0
         self.pipeline.process_pipeline()
-        self.pipeline._output["dummy"].store.side_effect = WarningOutputError
+        self.pipeline._output["dummy"].store.side_effect = WarningOutputError(
+            self.pipeline._output["dummy"], ""
+        )
         self.pipeline.process_pipeline()
         self.pipeline._output["dummy"].store.side_effect = None
         self.pipeline.process_pipeline()
         assert self.pipeline._input.get_next.call_count == 3
         assert mock_warning.call_count == 1
         assert self.pipeline._output["dummy"].store.call_count == 3
         assert self.pipeline._output["dummy"].metrics.number_of_warnings == 1
 
     @mock.patch("logging.Logger.warning")
     def test_processor_warning_error_is_logged_but_processing_continues(self, mock_warning, _):
         self.pipeline._setup()
         self.pipeline._input.get_next.return_value = ({"message": "test"}, None)
-        self.pipeline._pipeline[1].process.side_effect = ProcessorWarningMockError
-        self.pipeline.process_pipeline()
-        self.pipeline._input.get_next.return_value = ({"message": "test"}, None)
-        self.pipeline.process_pipeline()
-        mock_warning.assert_called()
-        assert (
-            "ProcessorWarningMockError" in mock_warning.call_args[0][0]
-        ), "the log message was written"
-        assert self.pipeline._output["dummy"].store.call_count == 2, "all events are processed"
+        processing_warning = ProcessingWarning(
+            self.pipeline._pipeline[1], "not so bad", None, {"message": "test"}
+        )
 
-    @mock.patch("logging.Logger.warning")
-    def test_processor_warning_error_is_logged_for_processingwarningcollection(
-        self, mock_warning, _
-    ):
-        class ProcessingWarningMockCollection(ProcessingWarningCollection):
-            def __init__(self):
-                super().__init__(
-                    "name",
-                    "message",
-                    [ProcessingWarning("warning1"), ProcessingWarning("warning2")],
-                )
+        def raise_processing_warning(_):
+            raise processing_warning
 
-        self.pipeline._setup()
+        self.pipeline._pipeline[1].process.side_effect = raise_processing_warning
+        self.pipeline.process_pipeline()
         self.pipeline._input.get_next.return_value = ({"message": "test"}, None)
-        self.pipeline._pipeline[0].process.side_effect = ProcessingWarningMockCollection
         self.pipeline.process_pipeline()
-        assert mock_warning.call_count == 4, "called 2 times for 2 processors in pipeline"
-        assert self.pipeline._output["dummy"].store.call_count == 1, "the event is processed"
+        mock_warning.assert_called_with(str(processing_warning))
+        assert self.pipeline._output["dummy"].store.call_count == 2, "all events are processed"
 
     @mock.patch("logging.Logger.error")
     def test_processor_critical_error_is_logged_event_is_stored_in_error_output(
         self, mock_error, _
     ):
         self.pipeline._setup()
-        self.pipeline._input.get_next.return_value = ({"message": "test"}, None)
-        self.pipeline._pipeline[1].process.side_effect = Exception
+        input_event1 = {"message": "first event"}
+        input_event2 = {"message": "second event"}
+        self.pipeline._input.get_next.return_value = (input_event1, None)
+
+        def raise_critical_processing_error(event):
+            raise ProcessingCriticalError(
+                self.pipeline._pipeline[1], "really bad things happened", event
+            )
+
+        self.pipeline._pipeline[1].process.side_effect = raise_critical_processing_error
         self.pipeline.process_pipeline()
-        self.pipeline._input.get_next.return_value = ({"message": "test"}, None)
+        self.pipeline._input.get_next.return_value = (input_event2, None)
         self.pipeline.process_pipeline()
         assert self.pipeline._input.get_next.call_count == 2, "2 events gone into processing"
         assert mock_error.call_count == 2, "two errors occured"
-        assert (
-            "A critical error occurred for processor" in mock_error.call_args[0][0]
-        ), "the log error message was written"
+        mock_error.assert_called_with(
+            str(
+                ProcessingCriticalError(
+                    self.pipeline._pipeline[1], "really bad things happened", input_event1
+                )
+            )
+        )
+        mock_error.assert_called_with(
+            str(
+                ProcessingCriticalError(
+                    self.pipeline._pipeline[1], "really bad things happened", input_event2
+                )
+            )
+        )
         assert self.pipeline._output["dummy"].store.call_count == 0, "no event in output"
         assert (
             self.pipeline._output["dummy"].store_failed.call_count == 2
         ), "errored events are gone to connector error output handler"
 
     @mock.patch("logging.Logger.error")
     def test_critical_input_error_is_logged_error_is_stored_in_failed_events(self, mock_error, _):
-        def raise_critical(args):
-            raise CriticalInputError("mock input error", args)
-
         self.pipeline._setup()
+        input_event = {"message": "test"}
+
+        def raise_critical(timeout):
+            raise CriticalInputError(self.pipeline._input, "mock input error", input_event)
+
         self.pipeline._input.metrics = mock.MagicMock()
         self.pipeline._input.metrics.number_of_errors = 0
-        self.pipeline._input.get_next.return_value = ({"message": "test"}, None)
+        self.pipeline._input.get_next.return_value = (input_event, None)
         self.pipeline._input.get_next.side_effect = raise_critical
         self.pipeline.process_pipeline()
         self.pipeline._input.get_next.assert_called()
-        mock_error.assert_called()
-        assert re.search(
-            r"A critical error occurred for input .*: mock input error", mock_error.call_args[0][0]
-        ), "error message is logged"
+        assert self.pipeline._input.metrics.number_of_errors == 1, "counts error metric"
+        mock_error.assert_called_with(
+            str(CriticalInputError(self.pipeline._input, "mock input error", input_event))
+        )
         assert self.pipeline._output["dummy"].store_failed.call_count == 1, "one error is stored"
         assert self.pipeline._output["dummy"].store.call_count == 0, "no event is stored"
-        assert self.pipeline._input.metrics.number_of_errors == 1, "counts error metric"
 
     @mock.patch("logging.Logger.warning")
     def test_input_warning_is_logged(self, mock_warning, _):
-        def raise_warning(args):
-            raise WarningInputError("mock input warning", args)
+        def raise_warning(_):
+            raise WarningInputError(self.pipeline._input, "mock input warning")
 
         self.pipeline._setup()
         self.pipeline._input.get_next.side_effect = raise_warning
         self.pipeline.process_pipeline()
         self.pipeline._input.get_next.assert_called()
-        mock_warning.assert_called()
-        assert re.search(
-            r"An error occurred for input .*:", mock_warning.call_args[0][0]
-        ), "error message is logged"
+        mock_warning.assert_called_with(
+            str(WarningInputError(self.pipeline._input, "mock input warning"))
+        )
 
     @mock.patch("logging.Logger.error")
-    def test_critical_output_error_is_logged(self, mock_error, _):
-        def raise_critical(args):
-            raise CriticalOutputError("mock output error", args)
-
-        self.pipeline._setup()
-        self.pipeline._input.get_next.return_value = ({"test": "message"}, None)
-        self.pipeline._output["dummy"].metrics = mock.MagicMock()
-        self.pipeline._output["dummy"].metrics.number_of_errors = 0
-        self.pipeline._output["dummy"].store.side_effect = raise_critical
-        self.pipeline.process_pipeline()
-        self.pipeline._output["dummy"].store_failed.assert_called()
-        mock_error.assert_called()
-        assert re.search(
-            r"A critical error occurred for output .*: mock output error",
-            mock_error.call_args[0][0],
-        ), "error message is logged"
-        assert self.pipeline._output["dummy"].metrics.number_of_errors == 1, "counts error metric"
+    def test_critical_output_error_is_logged_and_counted(self, mock_log_error, _):
+        dummy_output = original_create({"dummy_output": {"type": "dummy_output"}}, mock.MagicMock())
+        dummy_output.store_failed = mock.MagicMock()
+
+        def raise_critical(event):
+            raise CriticalOutputError(dummy_output, "mock output error", event)
+
+        input_event = {"test": "message"}
+        dummy_output.store = raise_critical
+        dummy_output.metrics.number_of_errors = 0
+        self.pipeline._setup()
+        self.pipeline._output["dummy"] = dummy_output
+        self.pipeline._input.get_next.return_value = (input_event, None)
+        self.pipeline.process_pipeline()
+        dummy_output.store_failed.assert_called()
+        assert dummy_output.metrics.number_of_errors == 1, "counts error metric"
+        mock_log_error.assert_called_with(
+            str(CriticalOutputError(dummy_output, "mock output error", input_event))
+        )
 
     @mock.patch("logging.Logger.warning")
-    def test_warning_output_error_is_logged(self, mock_warning, _):
-        self.pipeline._setup()
-        self.pipeline._input.get_next.return_value = ({"some": "event"}, None)
-        self.pipeline._output["dummy"].store.side_effect = WarningOutputError("mock output warning")
-        self.pipeline.process_pipeline()
-        self.pipeline._output["dummy"].store.assert_called()
-        mock_warning.assert_called()
-        assert mock_warning.call_args[0][0].startswith(
-            "An error occurred for output"
-        ), "error message is logged"
+    def test_warning_output_error_is_logged_and_counted(self, mock_warning, _):
+        dummy_output = original_create({"dummy_output": {"type": "dummy_output"}}, mock.MagicMock())
+
+        def raise_warning(event):
+            raise WarningOutputError(self.pipeline._output["dummy"], "mock output warning")
+
+        input_event = {"test": "message"}
+        dummy_output.store = raise_warning
+        dummy_output.metrics.number_of_warnings = 0
+        self.pipeline._setup()
+        self.pipeline._output["dummy"] = dummy_output
+        self.pipeline._input.get_next.return_value = (input_event, None)
+        self.pipeline.process_pipeline()
+        assert dummy_output.metrics.number_of_warnings == 1
+        mock_warning.assert_called_with(
+            str(WarningOutputError(self.pipeline._output["dummy"], "mock output warning"))
+        )
 
-    @mock.patch("logprep.framework.pipeline.Pipeline._shut_down")
     @mock.patch("logging.Logger.error")
-    def test_processor_fatal_input_error_is_logged_pipeline_is_rebuilt(
-        self, mock_error, mock_shut_down, _
-    ):
+    def test_processor_fatal_input_error_is_logged_pipeline_is_rebuilt(self, mock_error, _):
         self.pipeline._setup()
-        self.pipeline._input.get_next.side_effect = FatalInputError
+
+        def raise_fatal_input_error(event):
+            raise FatalInputError(self.pipeline._input, "fatal input error")
+
+        self.pipeline._input = original_create(
+            {"dummy": {"type": "dummy_input", "documents": []}}, getLogger()
+        )
+        self.pipeline._input.get_next = mock.MagicMock(side_effect=raise_fatal_input_error)
+        self.pipeline._shut_down = mock.MagicMock()
+        assert self.pipeline._input.metrics.number_of_errors == 0
         self.pipeline.run()
         self.pipeline._input.get_next.assert_called()
-        mock_error.assert_called()
-        assert re.search(r"Input .* failed:", mock_error.call_args[0][0]), "error message is logged"
-        mock_shut_down.assert_called()
+        self.pipeline._shut_down.assert_called()
+        assert self.pipeline._input.metrics.number_of_errors == 1
+        mock_error.assert_called_with(
+            str(FatalInputError(self.pipeline._input, "fatal input error"))
+        )
 
     @mock.patch("logprep.framework.pipeline.Pipeline._shut_down")
     @mock.patch("logging.Logger.error")
     def test_processor_fatal_output_error_is_logged_pipeline_is_rebuilt(
-        self, mock_error, mock_shut_down, _
+        self, mock_log_error, mock_shut_down, _
     ):
         self.pipeline._setup()
         self.pipeline._input.get_next.return_value = ({"some": "event"}, None)
-        self.pipeline._output["dummy"].store.side_effect = FatalOutputError
+        raised_error = FatalOutputError(mock.MagicMock(), "fatal output error")
+        self.pipeline._output["dummy"].store.side_effect = raised_error
         self.pipeline.run()
         self.pipeline._output["dummy"].store.assert_called()
-        mock_error.assert_called()
-        assert re.search("Output .* failed:", mock_error.call_args[0][0]), "error message is logged"
+        mock_log_error.assert_called_with(str(raised_error))
         mock_shut_down.assert_called()
 
     @mock.patch("logging.Logger.error")
     def test_processor_fatal_output_error_in_setup_is_logged_pipeline_is_rebuilt(
-        self, mock_error, _
+        self, mock_log_error, _
     ):
         self.pipeline._output = {"dummy": mock.MagicMock()}
-        self.pipeline._output["dummy"].setup.side_effect = FatalOutputError
+        raised_error = FatalOutputError(mock.MagicMock(), "bad things happened")
+        self.pipeline._output["dummy"].setup.side_effect = raised_error
         self.pipeline.run()
-        mock_error.assert_called()
-        assert re.search("Output .* failed:", mock_error.call_args[0][0]), "error message is logged"
+        mock_log_error.assert_called_with(str(raised_error))
 
     def test_extra_data_tuple_is_passed_to_store_custom(self, _):
         self.pipeline._setup()
         self.pipeline._input.get_next.return_value = ({"some": "event"}, None)
         processor_with_extra_data = mock.MagicMock()
         processor_with_extra_data.process = mock.MagicMock()
         processor_with_extra_data.process.return_value = ([{"foo": "bar"}], ({"dummy": "target"},))
@@ -636,14 +658,30 @@
         with mock.patch("logprep.factory.Factory.create", original_create):
             output = self.pipeline._output
             assert isinstance(output, dict)
             for output_connector in output.items():
                 assert isinstance(output_connector[1], Output)
         assert not self.pipeline._output["dummy1"].default
 
+    def test_process_pipeline_runs_scheduled_tasks(self, _):
+        self.pipeline._logprep_config["output"] = {
+            "dummy": {"type": "dummy_output"},
+        }
+        with mock.patch("logprep.factory.Factory.create", original_create):
+            output = self.pipeline._output
+
+        mock_task = mock.MagicMock()
+        self.pipeline._get_event = mock.MagicMock()
+        self.pipeline._store_event = mock.MagicMock()
+        self.pipeline.process_event = mock.MagicMock()
+        output["dummy"]._schedule_task(task=mock_task, seconds=30)
+        with mock.patch("schedule.Job.should_run", return_value=True):
+            self.pipeline.process_pipeline()
+        mock_task.assert_called()
+
 
 class TestPipelineWithActualInput:
     def setup_method(self):
         self.config = GetterFactory.from_string("tests/testdata/config/config.yml").get_yaml()
         del self.config["output"]
         self.config["process_count"] = 1
         self.config["input"] = {
@@ -807,51 +845,61 @@
             log_handler=self.log_handler,
             lock=self.lock,
             used_server_ports=mock.MagicMock(),
             shared_dict=self.shared_dict,
         )
         pipeline._input = mock.MagicMock()
         pipeline._input.get_next = mock.MagicMock()
-        pipeline._input.get_next.side_effect = SourceDisconnectedError()
+
+        def raise_source_disconnected_error(_):
+            raise SourceDisconnectedError(pipeline._input, "source was disconnected")
+
+        pipeline._input.get_next.side_effect = raise_source_disconnected_error
         pipeline.start()
         pipeline.stop()
         pipeline.join()
-        out, err = capfd.readouterr()
+        _, err = capfd.readouterr()
         assert "AttributeError: 'bool' object has no attribute 'get_lock'" not in err
 
     def test_graceful_shutdown_of_pipeline_on_fata_input_error(self, capfd):
         pipeline = MultiprocessingPipeline(
             pipeline_index=1,
             config=self.logprep_config,
             log_handler=self.log_handler,
             lock=self.lock,
             used_server_ports=mock.MagicMock(),
             shared_dict=self.shared_dict,
         )
         pipeline._input = mock.MagicMock()
         pipeline._input.get_next = mock.MagicMock()
-        pipeline._input.get_next.side_effect = FatalInputError()
+
+        def raise_fatal_input_error(_):
+            raise FatalInputError(pipeline._input, "realy bad things happened")
+
+        pipeline._input.get_next.side_effect = raise_fatal_input_error
         pipeline.start()
         pipeline.stop()
         pipeline.join()
-        out, err = capfd.readouterr()
+        _, err = capfd.readouterr()
         assert "AttributeError: 'bool' object has no attribute 'get_lock'" not in err
 
     def test_graceful_shutdown_of_pipeline_on_fatal_output_error(self, capfd):
         pipeline = MultiprocessingPipeline(
             pipeline_index=1,
             config=self.logprep_config,
             log_handler=self.log_handler,
             lock=self.lock,
             used_server_ports=mock.MagicMock(),
             shared_dict=self.shared_dict,
         )
         pipeline._output = mock.MagicMock()
         pipeline._output.store = mock.MagicMock()
-        pipeline._output.store.side_effect = FatalOutputError()
+        pipeline._output.store.side_effect = FatalOutputError(
+            pipeline._output, "bad things happened"
+        )
         pipeline.start()
         pipeline.stop()
         pipeline.join()
         out, err = capfd.readouterr()
         assert "AttributeError: 'bool' object has no attribute 'get_lock'" not in err
 
     @staticmethod
```

### Comparing `logprep-6.0.0/tests/unit/framework/test_pipeline_manager.py` & `logprep-6.1.0/tests/unit/framework/test_pipeline_manager.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/metrics/test_metric_exposer.py` & `logprep-6.1.0/tests/unit/metrics/test_metric_exposer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/metrics/test_metric_targets.py` & `logprep-6.1.0/tests/unit/metrics/test_metric_targets.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/metrics/test_metrics.py` & `logprep-6.1.0/tests/unit/metrics/test_metrics.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/processor/base.py` & `logprep-6.1.0/tests/unit/processor/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 # pylint: disable=missing-module-docstring
 # pylint: disable=protected-access
 
 import json
-from abc import ABC
 from copy import deepcopy
 from logging import getLogger
 from pathlib import Path
-from typing import Iterable
 from unittest import mock
 
 import pytest
-import responses
 import requests
+import responses
 from ruamel.yaml import YAML
 
 from logprep.abc.processor import Processor
 from logprep.factory import Factory
 from logprep.framework.rule_tree.rule_tree import RuleTree
 from logprep.processor.base.exceptions import ProcessingWarning
 from logprep.processor.processor_strategy import ProcessStrategy
 from logprep.util.helper import camel_to_snake
 from logprep.util.json_handling import list_json_files_in_directory
 from logprep.util.time_measurement import TimeMeasurement
+from tests.unit.component.base import BaseComponentTestCase
 
 yaml = YAML(typ="safe", pure=True)
 
 
-class BaseProcessorTestCase(ABC):
+class BaseProcessorTestCase(BaseComponentTestCase):
     mocks: dict = {}
 
     CONFIG: dict = {}
 
     logger = getLogger()
 
     object: Processor = None
@@ -114,24 +113,14 @@
             "message": "user root logged in",
         }
         count = self.object.metrics.number_of_processed_events
         self.object.process(document)
 
         assert self.object.metrics.number_of_processed_events == count + 1
 
-    def test_uses_python_slots(self):
-        assert isinstance(self.object.__slots__, Iterable)
-
-    def test_describe(self):
-        describe_string = self.object.describe()
-        assert f"{self.object.__class__.__name__} (Test Instance Name)" == describe_string
-
-    def test_snake_type(self):
-        assert str(self.object) == camel_to_snake(self.object.__class__.__name__)
-
     def test_generic_specific_rule_trees(self):
         assert isinstance(self.object._generic_tree, RuleTree)
         assert isinstance(self.object._specific_tree, RuleTree)
 
     def test_generic_specific_rule_trees_not_empty(self):
         assert self.object._generic_tree.get_size() > 0
         assert self.object._specific_tree.get_size() > 0
```

### Comparing `logprep-6.0.0/tests/unit/processor/calculator/test_calculator.py` & `logprep-6.1.0/tests/unit/processor/calculator/test_calculator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # pylint: disable=missing-docstring
+import logging
 import math
+import re
 
 import pytest
 
-from logprep.processor.base.exceptions import ProcessingWarning
 from logprep.processor.calculator.fourFn import BNF
 from tests.unit.processor.base import BaseProcessorTestCase
 
 test_cases = [  # testcase, rule, event, expected
     (
         "sums integers",
         {
@@ -173,15 +174,15 @@
         {"field1": "not parsable", "field2": "4", "field3": 2},
         {
             "field1": "not parsable",
             "field2": "4",
             "field3": 2,
             "tags": ["_calculator_failure"],
         },
-        r"expression 'not parsable \+ 4 \* 2' could not be parsed",
+        r"ProcessingWarning.*expression 'not parsable \+ 4 \* 2' could not be parsed",
     ),
     (
         "Tags failure if target_field exist",
         {
             "filter": "field1 AND field2 AND field3",
             "calculator": {
                 "calc": "${field1} + ${field2} * ${field3}",
@@ -192,15 +193,15 @@
         {
             "field1": "5",
             "field2": "4",
             "field3": 2,
             "result": "exists",
             "tags": ["_calculator_failure"],
         },
-        "one or more subfields existed and could not be extended: result",
+        "FieldExistsWarning.*one or more subfields existed and could not be extended: result",
     ),
     (
         "Tags failure if source_field missing",
         {
             "filter": "field2 AND field3",
             "calculator": {
                 "calc": "${field1} + ${field2} * ${field3}",
@@ -209,15 +210,15 @@
         },
         {"field2": "4", "field3": 2},
         {
             "field2": "4",
             "field3": 2,
             "tags": ["_calculator_failure"],
         },
-        r"no value for fields: \['field1'\]",
+        r"ProcessingWarning.*no value for fields: \['field1'\]",
     ),
     (
         "Tags failure if source_field is empty",
         {
             "filter": "field2 AND field3",
             "calculator": {
                 "calc": "${field1} + ${field2} * ${field3}",
@@ -227,15 +228,15 @@
         {"field1": "", "field2": "4", "field3": 2},
         {
             "field1": "",
             "field2": "4",
             "field3": 2,
             "tags": ["_calculator_failure"],
         },
-        r"no value for fields: \['field1'\]",
+        r"ProcessingWarning.*no value for fields: \['field1'\]",
     ),
     (
         "Tags failure try to escape",
         {
             "filter": "field2 AND field3",
             "calculator": {
                 "calc": "${field1} + ${field2} * ${field3}",
@@ -245,15 +246,15 @@
         {"field1": "\"; print('escaped');\"", "field2": "4", "field3": 2},
         {
             "field1": "\"; print('escaped');\"",
             "field2": "4",
             "field3": 2,
             "tags": ["_calculator_failure"],
         },
-        r"could not be parsed",
+        r"ProcessingWarning.*could not be parsed",
     ),
     (
         "division by zero",
         {
             "filter": "message",
             "calculator": {
                 "calc": "3/0",
@@ -263,15 +264,15 @@
         {"message": "This is a message", "field1": "1.2", "field2": 4.5},
         {
             "message": "This is a message",
             "field1": "1.2",
             "field2": 4.5,
             "tags": ["_calculator_failure"],
         },
-        r"'3/0' => '3/0' results in division by zero",
+        r"ProcessingWarning.*'3/0' => '3/0' results in division by zero",
     ),
     (
         "raises timout",
         {
             "filter": "message",
             "calculator": {
                 "calc": " 9^9^9",
@@ -279,15 +280,15 @@
             },
         },
         {"message": "This is a message"},
         {
             "message": "This is a message",
             "tags": ["_calculator_failure"],
         },
-        r"Timer expired",
+        r"ProcessingWarning.*Timer expired",
     ),
 ]
 
 
 class TestCalculator(BaseProcessorTestCase):
     CONFIG: dict = {
         "type": "calculator",
@@ -298,18 +299,21 @@
     @pytest.mark.parametrize("testcase, rule, event, expected", test_cases)
     def test_testcases(self, testcase, rule, event, expected):  # pylint: disable=unused-argument
         self._load_specific_rule(rule)
         self.object.process(event)
         assert event == expected
 
     @pytest.mark.parametrize("testcase, rule, event, expected, error_message", failure_test_cases)
-    def test_testcases_failure_handling(self, testcase, rule, event, expected, error_message):
+    def test_testcases_failure_handling(
+        self, caplog, testcase, rule, event, expected, error_message
+    ):
         self._load_specific_rule(rule)
-        with pytest.raises(ProcessingWarning, match=error_message):
+        with caplog.at_level(logging.WARNING):
             self.object.process(event)
+            assert re.match(rf".*{error_message}", caplog.text)
         assert event == expected, testcase
 
     @pytest.mark.parametrize(
         "expression, expected",
         [
             ("9", 9),
             ("-9", -9),
```

### Comparing `logprep-6.0.0/tests/unit/processor/calculator/test_calculator_rule.py` & `logprep-6.1.0/tests/unit/processor/calculator/test_calculator_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/processor/clusterer/test_clusterer.py` & `logprep-6.1.0/tests/unit/processor/clusterer/test_clusterer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/processor/clusterer/test_clusterer_rule.py` & `logprep-6.1.0/tests/unit/processor/clusterer/test_clusterer_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/processor/clusterer/test_clusterer_signature_phase.py` & `logprep-6.1.0/tests/unit/processor/clusterer/test_clusterer_signature_phase.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/processor/concatenator/test_concatenator.py` & `logprep-6.1.0/tests/unit/processor/concatenator/test_concatenator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # pylint: disable=missing-docstring
 # pylint: disable=protected-access
+import logging
+import re
+
 import pytest
 
-from logprep.processor.base.exceptions import ProcessingWarning
 from tests.unit.processor.base import BaseProcessorTestCase
 
 
 class TestConcatenator(BaseProcessorTestCase):
     CONFIG = {
         "type": "concatenator",
         "specific_rules": ["tests/testdata/unit/concatenator/rules/specific"],
@@ -145,31 +147,27 @@
     )
     def test_for_expected_output(self, test_case, rule, document, expected_output):
         self._load_specific_rule(rule)
         self.object.process(document)
         assert document == expected_output, test_case
 
     def test_process_raises_duplication_error_if_target_field_exists_and_should_not_be_overwritten(
-        self,
+        self, caplog
     ):
         rule = {
             "filter": "field.a",
             "concatenator": {
                 "source_fields": ["field.a", "field.b"],
                 "target_field": "target_field",
                 "separator": "-",
                 "overwrite_target": False,
                 "delete_source_fields": False,
             },
         }
         self._load_specific_rule(rule)
         document = {"field": {"a": "first", "b": "second"}, "target_field": "has already content"}
-        with pytest.raises(
-            ProcessingWarning,
-            match=r"ProcessingWarning: \(Test Instance Name - The following fields could not be "
-            r"written, because one or more subfields existed and could not be extended: "
-            r"target_field\)",
-        ):
+        with caplog.at_level(logging.WARNING):
             self.object.process(document)
+        assert re.match(".*FieldExistsWarning.*", caplog.text)
         assert "target_field" in document
         assert document.get("target_field") == "has already content"
         assert document.get("tags") == ["_concatenator_failure"]
```

### Comparing `logprep-6.0.0/tests/unit/processor/concatenator/test_concatenator_rule.py` & `logprep-6.1.0/tests/unit/processor/concatenator/test_concatenator_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/processor/datetime_extractor/test_datetime_extractor.py` & `logprep-6.1.0/tests/unit/processor/datetime_extractor/test_datetime_extractor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # pylint: disable=protected-access
 # pylint: disable=missing-module-docstring
 # pylint: disable=wrong-import-position
 # pylint: disable=wrong-import-order
-import pytest
-
+import logging
+import re
 from datetime import datetime
-from dateutil.tz import tzlocal, tzutc
+
 from dateutil.parser import parse
+from dateutil.tz import tzlocal, tzutc
 
-from logprep.processor.base.exceptions import ProcessingWarning
 from logprep.processor.datetime_extractor.processor import DatetimeExtractor
 from tests.unit.processor.base import BaseProcessorTestCase
 
 
 class TestDatetimeExtractor(BaseProcessorTestCase):
     CONFIG = {
         "type": "datetime_extractor",
@@ -193,33 +193,29 @@
                 "microsecond": 861000,
                 "weekday": "Tuesday",
                 "timezone": "UTC",
             },
         }
         assert document == expected
 
-    def test_existing_target_raises_if_not_overwrite_target(self):
+    def test_existing_target_raises_if_not_overwrite_target(self, caplog):
         document = {"@timestamp": "2019-07-30T14:37:42.861+00:00", "winlog": {"event_id": 123}}
         rule = {
             "filter": "@timestamp",
             "datetime_extractor": {
                 "source_fields": ["@timestamp"],
                 "target_field": "@timestamp",
                 "overwrite_target": False,
             },
             "description": "",
         }
         self._load_specific_rule(rule)
-        with pytest.raises(
-            ProcessingWarning,
-            match=r"ProcessingWarning: \(Test Instance Name - The following fields could not be "
-            r"written, because one or more subfields existed and could not be extended: "
-            r"@timestamp\)",
-        ):
+        with caplog.at_level(logging.WARNING):
             self.object.process(document)
+        assert re.match(".*FieldExistsWarning.*", caplog.text)
 
     @staticmethod
     def _parse_local_tz(tz_local_name):
         sign = tz_local_name[:1]
         hour = tz_local_name[1:-2]
         minute = tz_local_name[3:]
         timezone_utc = f"UTC{sign}{hour}:{minute}" if hour != "00" or minute != "00" else "UTC"
```

### Comparing `logprep-6.0.0/tests/unit/processor/datetime_extractor/test_datetime_extractor_rule.py` & `logprep-6.1.0/tests/unit/processor/datetime_extractor/test_datetime_extractor_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/processor/deleter/test_deleter.py` & `logprep-6.1.0/tests/unit/processor/deleter/test_deleter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/processor/deleter/test_deleter_rule.py` & `logprep-6.1.0/tests/unit/processor/deleter/test_deleter_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/processor/dissector/test_dissector.py` & `logprep-6.1.0/tests/unit/processor/dissector/test_dissector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # pylint: disable=missing-docstring
+import logging
+import re
+
 import pytest
 
-from logprep.processor.base.exceptions import ProcessingWarning
 from tests.unit.processor.base import BaseProcessorTestCase
 
 test_cases = [  # testcase, rule, event, expected
     (
         "writes new fields with same separator",
         {
             "filter": "message",
@@ -579,12 +581,13 @@
     @pytest.mark.parametrize("testcase, rule, event, expected", test_cases)
     def test_testcases(self, testcase, rule, event, expected):  # pylint: disable=unused-argument
         self._load_specific_rule(rule)
         self.object.process(event)
         assert event == expected
 
     @pytest.mark.parametrize("testcase, rule, event, expected", failure_test_cases)
-    def test_testcases_failure_handling(self, testcase, rule, event, expected):
+    def test_testcases_failure_handling(self, caplog, testcase, rule, event, expected):
         self._load_specific_rule(rule)
-        with pytest.raises(ProcessingWarning):
+        with caplog.at_level(logging.WARNING):
             self.object.process(event)
+        assert re.match(".*ProcessingWarning.*", caplog.text)
         assert event == expected, testcase
```

### Comparing `logprep-6.0.0/tests/unit/processor/dissector/test_dissector_rule.py` & `logprep-6.1.0/tests/unit/processor/dissector/test_dissector_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor.py` & `logprep-6.1.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # pylint: disable=protected-access
 # pylint: disable=missing-docstring
 
 import hashlib
+import logging
+import re
 from multiprocessing import current_process
 from pathlib import Path
-import pytest
+
 import responses
 
-from logprep.processor.base.exceptions import ProcessingWarning
 from logprep.factory import Factory
+from logprep.processor.base.exceptions import ProcessingWarning
 from tests.unit.processor.base import BaseProcessorTestCase
 
 
 class TestDomainLabelExtractor(BaseProcessorTestCase):
     CONFIG = {
         "type": "domain_label_extractor",
         "generic_rules": ["tests/testdata/unit/domain_label_extractor/rules/generic"],
@@ -246,24 +248,20 @@
             "url": {"domain": "2001:0db8:85a3:0000:0000:8a2e:0370:7334"},
             "tags": ["ip_in_url_domain"],
         }
 
         self.object.process(document)
         assert document == expected_output
 
-    def test_domain_extraction_with_existing_output_field(self):
+    def test_domain_extraction_with_existing_output_field(self, caplog):
         document = {"url": {"domain": "test.domain.de", "subdomain": "exists already"}}
 
-        with pytest.raises(
-            ProcessingWarning,
-            match=r"ProcessingWarning: \(Test Instance Name - The following fields could not be "
-            r"written, because one or more subfields existed and could not be extended: "
-            r"url.subdomain\)",
-        ):
+        with caplog.at_level(logging.WARNING):
             self.object.process(document)
+        assert re.match(".*FieldExistsWarning.*", caplog.text)
 
     def test_domain_extraction_overwrites_target_field(self):
         document = {"url": {"domain": "test.domain.de", "subdomain": "exists already"}}
         expected = {
             "url": {
                 "domain": "test.domain.de",
                 "registered_domain": "domain.de",
@@ -320,15 +318,15 @@
             },
             "description": "",
         }
         self._load_specific_rule(rule_dict)
         self.object.process(document)
         assert document == expected
 
-    def test_raises_duplication_error_if_target_field_exits(self):
+    def test_raises_duplication_error_if_target_field_exits(self, caplog):
         document = {"url": {"domain": "test.domain.de", "subdomain": "exists already"}}
         expected = {
             "tags": ["_domain_label_extractor_failure"],
             "url": {
                 "domain": "test.domain.de",
                 "subdomain": "exists already",
                 "registered_domain": "domain.de",
@@ -341,16 +339,17 @@
             "domain_label_extractor": {
                 "source_fields": ["url.domain"],
                 "target_field": "url",
             },
             "description": "",
         }
         self._load_specific_rule(rule_dict)
-        with pytest.raises(ProcessingWarning):
+        with caplog.at_level(logging.WARNING):
             self.object.process(document)
+        assert re.match(".*FieldExistsWarning.*", caplog.text)
         assert document == expected
 
     @responses.activate
     def test_setup_downloads_tld_lists_to_separate_process_file(self):
         tld_list = "http://db-path-target/list.dat"
         tld_list_path = Path("/usr/bin/ls") if Path("/usr/bin/ls").exists() else Path("/bin/ls")
         tld_list_content = tld_list_path.read_bytes()
```

### Comparing `logprep-6.0.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor_rule.py` & `logprep-6.1.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/processor/domain_resolver/test_domain_resolver.py` & `logprep-6.1.0/tests/unit/processor/domain_resolver/test_domain_resolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # pylint: disable=missing-docstring
 # pylint: disable=protected-access
-from copy import deepcopy
 import hashlib
+import logging
+import re
+from copy import deepcopy
 from multiprocessing import current_process
 from os.path import exists
 from pathlib import Path
 from unittest import mock
 
 import pytest
 import responses
 
-from logprep.processor.base.exceptions import ProcessingWarning
 from logprep.factory import Factory
+from logprep.processor.base.exceptions import ProcessingWarning
 from tests.unit.processor.base import BaseProcessorTestCase
 
 REL_TLD_LIST_PATH = "tests/testdata/external/public_suffix_list.dat"
 TLD_LIST = f"file://{Path().absolute().joinpath(REL_TLD_LIST_PATH).as_posix()}"
 
 
 class TestDomainResolver(BaseProcessorTestCase):
@@ -215,25 +217,20 @@
     def test_configured_dotted_subfield(self, _):
         document = {"source": "google.de"}
         expected = {"source": "google.de", "resolved": {"ip": "1.2.3.4"}}
         self.object.process(document)
         assert document == expected
 
     @mock.patch("socket.gethostbyname", return_value="1.2.3.4")
-    def test_duplication_error(self, _):
+    def test_duplication_error(self, _, caplog):
         document = {"client": "google.de"}
 
-        # Due to duplication error logprep raises an ProcessingWarning
-        with pytest.raises(
-            ProcessingWarning,
-            match=r"ProcessingWarning: \(Test Instance Name - The following fields could not be "
-            r"written, because one or more subfields existed and could not be extended: "
-            r"resolved_ip\)",
-        ):
+        with caplog.at_level(logging.WARNING):
             self.object.process(document)
+        assert re.match(".*FieldExistsWarning.*", caplog.text)
 
     @mock.patch("socket.gethostbyname", return_value="1.2.3.4")
     def test_no_duplication_error(self, _):
         document = {"client_2": "google.de"}
         expected = {"client_2": "google.de", "resolved_ip": "1.2.3.4"}
 
         # Rules have same effect, but are equal and thus one is ignored
```

### Comparing `logprep-6.0.0/tests/unit/processor/domain_resolver/test_domain_resolver_rule.py` & `logprep-6.1.0/tests/unit/processor/domain_resolver/test_domain_resolver_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/processor/dropper/test_dropper.py` & `logprep-6.1.0/tests/unit/processor/dropper/test_dropper.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/processor/dropper/test_dropper_rule.py` & `logprep-6.1.0/tests/unit/processor/dropper/test_dropper_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/processor/field_manager/test_field_manager.py` & `logprep-6.1.0/tests/unit/processor/field_manager/test_field_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # pylint: disable=missing-docstring
+import logging
+import re
+
 import pytest
-from logprep.processor.base.exceptions import ProcessingWarning
-from tests.unit.processor.base import BaseProcessorTestCase
 
+from tests.unit.processor.base import BaseProcessorTestCase
 
 test_cases = [  # testcase, rule, event, expected
     (
         "copies single field to non existing target field",
         {
             "filter": "message",
             "field_manager": {
@@ -332,54 +334,50 @@
     @pytest.mark.parametrize("testcase, rule, event, expected", test_cases)
     def test_testcases(self, testcase, rule, event, expected):  # pylint: disable=unused-argument
         self._load_specific_rule(rule)
         self.object.process(event)
         assert event == expected
 
     @pytest.mark.parametrize("testcase, rule, event, expected", failure_test_cases)
-    def test_testcases_failure_handling(self, testcase, rule, event, expected):
+    def test_testcases_failure_handling(self, testcase, rule, event, expected, caplog):
         self._load_specific_rule(rule)
-        with pytest.raises(ProcessingWarning):
+        with caplog.at_level(logging.WARNING):
             self.object.process(event)
+        assert re.match(".*ProcessingWarning.*", caplog.text)
         assert event == expected, testcase
 
     def test_process_raises_duplication_error_if_target_field_exists_and_should_not_be_overwritten(
-        self,
+        self, caplog
     ):
         rule = {
             "filter": "field.a",
             "field_manager": {
                 "source_fields": ["field.a", "field.b"],
                 "target_field": "target_field",
                 "overwrite_target": False,
                 "delete_source_fields": False,
             },
         }
         self._load_specific_rule(rule)
         document = {"field": {"a": "first", "b": "second"}, "target_field": "has already content"}
-        with pytest.raises(
-            ProcessingWarning,
-            match=r"ProcessingWarning: \(Test Instance Name - The following fields could not be "
-            r"written, because one or more subfields existed and could not be extended: "
-            r"target_field\)",
-        ):
+        with caplog.at_level(logging.WARNING):
             self.object.process(document)
+        assert re.match(".*FieldExistsWarning.*", caplog.text)
         assert "target_field" in document
         assert document.get("target_field") == "has already content"
         assert document.get("tags") == ["_field_manager_failure"]
 
-    def test_process_raises_processing_warning_with_missing_fields(
-        self,
-    ):
+    def test_process_raises_processing_warning_with_missing_fields(self, caplog):
         rule = {
             "filter": "field.a",
             "field_manager": {
                 "source_fields": ["does.not.exists"],
                 "target_field": "target_field",
             },
         }
         self._load_specific_rule(rule)
         document = {"field": {"a": "first", "b": "second"}}
-        with pytest.raises(
-            ProcessingWarning, match=r"missing source_fields: \['does.not.exists'\]"
-        ):
+        with caplog.at_level(logging.WARNING):
             self.object.process(document)
+        assert re.match(
+            r".*ProcessingWarning.*missing source_fields: \['does.not.exists'\]", caplog.text
+        )
```

### Comparing `logprep-6.0.0/tests/unit/processor/field_manager/test_field_manager_rule.py` & `logprep-6.1.0/tests/unit/processor/field_manager/test_field_manager_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/processor/generic_adder/test_generic_adder.py` & `logprep-6.1.0/tests/unit/processor/generic_adder/test_generic_adder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # pylint: disable=protected-access
 # pylint: disable=missing-docstring
 # pylint: disable=unused-argument
 # pylint: disable=too-many-arguments
 import json
+import logging
 import os
 import re
 import tempfile
 import time
 from copy import deepcopy
 from unittest import mock
 
 import pytest
 
-from logprep.processor.base.exceptions import InvalidRuleDefinitionError, ProcessingWarning
 from logprep.factory import Factory
 from logprep.factory_error import InvalidConfigurationError
+from logprep.processor.base.exceptions import (
+    InvalidRuleDefinitionError,
+)
 from tests.unit.processor.base import BaseProcessorTestCase
 
 RULES_DIR_MISSING = "tests/testdata/unit/generic_adder/rules_missing"
 RULES_DIR_INVALID = "tests/testdata/unit/generic_adder/rules_invalid"
 RULES_DIR_FIRST_EXISTING = "tests/testdata/unit/generic_adder/rules_first_existing"
 
 
@@ -306,19 +309,15 @@
                 "add_generic_test": "Test",
                 "event_id": 123,
                 "some_added_field": "some_non_dict",
                 "another_added_field": "another_value",
                 "dotted": {"added": {"field": "yet_another_value"}},
                 "tags": ["_generic_adder_failure"],
             },
-            re.escape(
-                "ProcessingWarning: (Test Instance Name - The following fields could not be "
-                + "written, because one or more subfields existed and could not be extended: "
-                + "some_added_field)"
-            ),
+            r"subfields existed and could not be extended: some_added_field",
         ),
         (
             "Extend list field with 'extend_target_list' disabled",
             {
                 "filter": "extend_generic_test",
                 "generic_adder": {
                     "add": {
@@ -334,19 +333,15 @@
                 "extend_generic_test": "Test",
                 "event_id": 123,
                 "some_added_field": [],
                 "another_added_field": "another_value",
                 "dotted": {"added": {"field": "yet_another_value"}},
                 "tags": ["_generic_adder_failure"],
             },
-            re.escape(
-                "ProcessingWarning: (Test Instance Name - The following fields could not be "
-                + "written, because one or more subfields existed and could not be extended: "
-                + "some_added_field)"
-            ),
+            r"subfields existed and could not be extended: some_added_field",
         ),
         (
             "Extend list field with 'extend_target_list' enabled, but non-list target",
             {
                 "filter": "extend_generic_test",
                 "generic_adder": {
                     "add": {
@@ -362,19 +357,15 @@
                 "extend_generic_test": "Test",
                 "event_id": 123,
                 "some_added_field": "not_a_list",
                 "another_added_field": "another_value",
                 "dotted": {"added": {"field": "yet_another_value"}},
                 "tags": ["_generic_adder_failure"],
             },
-            re.escape(
-                "ProcessingWarning: (Test Instance Name - The following fields could not be "
-                + "written, because one or more subfields existed and could not be extended: "
-                + "some_added_field)"
-            ),
+            r"subfields existed and could not be extended: some_added_field",
         ),
     ]
 
     CONFIG = {
         "type": "generic_adder",
         "generic_rules": ["tests/testdata/unit/generic_adder/rules/generic"],
         "specific_rules": ["tests/testdata/unit/generic_adder/rules/specific"],
@@ -397,19 +388,20 @@
     ):  # pylint: disable=unused-argument
         self._load_specific_rule(rule)
         self.object.process(event)
         assert event == expected
 
     @pytest.mark.parametrize("testcase, rule, event, expected, error_message", failure_test_cases)
     def test_generic_adder_testcases_failure_handling(
-        self, testcase, rule, event, expected, error_message
+        self, testcase, rule, event, expected, error_message, caplog
     ):
         self._load_specific_rule(rule)
-        with pytest.raises(ProcessingWarning, match=error_message):
+        with caplog.at_level(logging.WARNING):
             self.object.process(event)
+        assert re.match(rf".*FieldExistsWarning.*{error_message}", caplog.text)
         assert event == expected, testcase
 
     def test_add_generic_fields_from_file_missing_and_existing_with_all_required(self):
         with pytest.raises(InvalidRuleDefinitionError, match=r"files do not exist"):
             config = deepcopy(self.CONFIG)
             config["specific_rules"] = [RULES_DIR_MISSING]
             configuration = {"test_instance_name": config}
@@ -588,26 +580,27 @@
         self.object.process(document_1)
         mock_simulate_table_change()
         self.object.process(document_2)
 
         assert document_1 == expected
         assert document_2 == expected
 
-    def test_sql_database_raises_exception_on_duplicate(self):
+    def test_sql_database_raises_exception_on_duplicate(self, caplog):
         expected = {
             "add_from_sql_db_table": "Test",
             "source": "TEST_0.test.123",
             "db": {"test": {"b": "foo", "c": "bar"}},
             "tags": ["_generic_adder_failure"],
         }
         document = {"add_from_sql_db_table": "Test", "source": "TEST_0.test.123"}
 
         self.object.process(document)
-        with pytest.raises(ProcessingWarning):
+        with caplog.at_level(logging.WARNING):
             self.object.process(document)
+        assert re.match(".*FieldExistsWarning.*", caplog.text)
 
         assert document == expected
 
     def test_time_to_check_for_change_not_read_for_change(self):
         self.object._file_check_interval = 9999999
         assert self.object._db_connector.time_to_check_for_change() is False
```

### Comparing `logprep-6.0.0/tests/unit/processor/generic_adder/test_generic_adder_rule.py` & `logprep-6.1.0/tests/unit/processor/generic_adder/test_generic_adder_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/processor/generic_resolver/test_generic_resolver.py` & `logprep-6.1.0/tests/unit/processor/generic_resolver/test_generic_resolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # pylint: disable=duplicate-code
 # pylint: disable=protected-access
 # pylint: disable=missing-docstring
 # pylint: disable=wrong-import-position
+import logging
+import re
 from collections import OrderedDict
 
 import pytest
 
-from logprep.processor.base.exceptions import ProcessingWarning
-from logprep.processor.generic_resolver.processor import GenericResolver, GenericResolverError
+from logprep.processor.base.exceptions import ProcessingCriticalError
+from logprep.processor.generic_resolver.processor import GenericResolver
 from tests.unit.processor.base import BaseProcessorTestCase
 
 
 class TestGenericResolver(BaseProcessorTestCase):
     CONFIG = {
         "type": "generic_resolver",
         "specific_rules": ["tests/testdata/unit/generic_resolver/rules/specific/"],
@@ -290,15 +292,15 @@
                 "resolve_list": {"FOO": "BAR"},
             },
         }
         self._load_specific_rule(rule)
         document = {"to_resolve": "ab"}
 
         with pytest.raises(
-            GenericResolverError,
+            ProcessingCriticalError,
             match=r"GenericResolver \(Test Instance Name\)\: Mapping group is missing in mapping "
             r"file pattern!",
         ):
             self.object.process(document)
 
     def test_resolve_generic_match_from_file_and_file_does_not_exist(self):
         rule = {
@@ -309,15 +311,15 @@
             },
         }
         self._load_specific_rule(rule)
 
         document = {"to": {"resolve": "something HELLO1"}}
 
         with pytest.raises(
-            GenericResolverError,
+            ProcessingCriticalError,
             match=r"GenericResolver \(Test Instance Name\)\: Additions file \'foo\' not found!",
         ):
             self.object.process(document)
 
     def test_resolve_dotted_field_no_conflict_no_match(self):
         rule = {
             "filter": "to.resolve",
@@ -384,17 +386,15 @@
         expected = {"to": {"resolve": "something HELLO1"}, "re": {"solved": "Greeting"}}
         document = {"to": {"resolve": "something HELLO1"}}
 
         self.object.process(document)
 
         assert document == expected
 
-    def test_resolve_dotted_src_and_dest_field_and_conflict_match(
-        self,
-    ):
+    def test_resolve_dotted_src_and_dest_field_and_conflict_match(self, caplog):
         rule = {
             "filter": "to.resolve",
             "generic_resolver": {
                 "field_mapping": {"to.resolve": "re.solved"},
                 "resolve_list": {".*HELLO\\d": "Greeting"},
             },
         }
@@ -405,16 +405,17 @@
             "re": {"solved": "I already exist!"},
         }
         expected = {
             "tags": ["_generic_resolver_failure"],
             "to": {"resolve": "something HELLO1"},
             "re": {"solved": "I already exist!"},
         }
-        with pytest.raises(ProcessingWarning):
+        with caplog.at_level(logging.WARNING):
             self.object.process(document)
+        assert re.match(".*FieldExistsWarning.*", caplog.text)
 
         assert document == expected
 
     def test_resolve_generic_and_multiple_match_first_only(self):
         rule = {
             "filter": "to.resolve",
             "generic_resolver": {
```

### Comparing `logprep-6.0.0/tests/unit/processor/generic_resolver/test_generic_resolver_rule.py` & `logprep-6.1.0/tests/unit/processor/generic_resolver/test_generic_resolver_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/processor/geoip_enricher/test_geoip_enricher.py` & `logprep-6.1.0/tests/unit/processor/geoip_enricher/test_geoip_enricher.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # pylint: disable=missing-docstring
 # pylint: disable=no-member
 # pylint: disable=protected-access
+# pylint: disable=too-many-statements
 import hashlib
+import logging
+import re
 from multiprocessing import current_process
 from pathlib import Path
 from unittest import mock
 
 import pytest
 import responses
 from geoip2.errors import AddressNotFoundError
@@ -52,14 +55,33 @@
             city.country.name = None
             city.country.iso_code = None
             city.city.name = None
             city.postal.code = None
             city.subdivisions.most_specific = mock.MagicMock()
             city.subdivisions.most_specific.name = None
             return city
+        if any(ip in ip_list for ip in ["55.55.55.51", "55.55.55.52", "55.55.55.53"]):
+            city = City()
+            city.location.accuracy_radius = 1337
+            city.location.time_zone = None
+            city.continent.name = None
+            city.continent.code = None
+            city.country.name = None
+            city.country.iso_code = None
+            city.city.name = None
+            city.postal.code = None
+            city.subdivisions.most_specific = mock.MagicMock()
+            city.subdivisions.most_specific.name = None
+            city.location.longitude = None
+            city.location.latitude = None
+            if "55.55.55.52" in ip_list:
+                city.location.latitude = 1.1
+            if "55.55.55.53" in ip_list:
+                city.location.longitude = 2.2
+            return city
         return mock.MagicMock()
 
 
 class TestGeoipEnricher(BaseProcessorTestCase):
     mocks = {"geoip2.database.Reader": {"new": ReaderMock()}}
 
     CONFIG = {
@@ -80,22 +102,42 @@
 
     def test_geoip_data_added(self):
         assert self.object.metrics.number_of_processed_events == 0
         document = {"client": {"ip": "1.2.3.4"}}
 
         self.object.process(document)
 
+        assert document.get("geoip")
+
     def test_geoip_data_added_not_exists(self):
         assert self.object.metrics.number_of_processed_events == 0
         document = {"client": {"ip": "127.0.0.1"}}
 
         self.object.process(document)
 
         assert document.get("geoip") is None
 
+    def test_no_geoip_data_added_if_source_field_is_none(self):
+        assert self.object.metrics.number_of_processed_events == 0
+        document = {"client": {"ip": None}}
+
+        self.object.process(document)
+
+        assert document.get("geoip") is None
+
+    def test_source_field_is_none_raises_processing_warning(self):
+        assert self.object.metrics.number_of_processed_events == 0
+        document = {"client": {"ip": None}}
+
+        with pytest.raises(
+            ProcessingWarning,
+            match=re.escape("Value of IP field 'client.ip' is 'None'"),
+        ):
+            self.object._apply_rules(document, self.object.rules[0])
+
     def test_nothing_to_enrich(self):
         assert self.object.metrics.number_of_processed_events == 0
         document = {"something": {"something": "1.2.3.4"}}
 
         self.object.process(document)
         assert "geoip" not in document
 
@@ -122,24 +164,21 @@
         assert geoip["geometry"]["coordinates"][0] == 1.1
         assert geoip["geometry"]["coordinates"][1] == 2.2
         assert isinstance(geoip.get("properties"), dict)
         assert geoip["properties"].get("continent") == "MyContinent"
         assert geoip["properties"].get("country") == "MyCountry"
         assert geoip["properties"].get("accuracy_radius") == 1337
 
-    def test_enrich_an_event_geoip_with_existing_differing_geoip(self):
+    def test_enrich_an_event_geoip_with_existing_differing_geoip(self, caplog):
         assert self.object.metrics.number_of_processed_events == 0
         document = {"client": {"ip": "8.8.8.8"}, "geoip": {"type": "Feature"}}
 
-        with pytest.raises(
-            ProcessingWarning,
-            match=r"The following fields could not be written, because one or more subfields "
-            r"existed and could not be extended: geoip.type",
-        ):
+        with caplog.at_level(logging.WARNING):
             self.object.process(document)
+        assert re.match(".*FieldExistsWarning.*geoip.type", caplog.text)
 
     def test_configured_dotted_output_field(self):
         assert self.object.metrics.number_of_processed_events == 0
         document = {"source": {"ip": "8.8.8.8"}}
 
         self.object.process(document)
         assert document.get("source", {}).get("geo", {}).get("ip") is not None
@@ -280,15 +319,15 @@
                 },
             },
             "description": "",
         }
         with pytest.raises(ValueError, match=r"\'customize_target_subfields\' must be in"):
             self._load_specific_rule(rule_dict)
 
-    def test_geoip_db_returns_only_limited_data(self):
+    def test_geoip_db_returns_only_limited_data_without_missing_coordinates(self):
         document = {"client": {"ip": "13.21.21.37"}}
         rule_dict = {
             "filter": "client",
             "geoip_enricher": {
                 "source_fields": ["client.ip"],
             },
             "description": "",
@@ -301,14 +340,38 @@
                 "geometry": {"coordinates": [1.1, 2.2], "type": "Point"},
                 "properties": {"accuracy_radius": 1337},
                 "type": "Feature",
             },
         }
         assert document == expected_event
 
+    @pytest.mark.parametrize(
+        "source_ip",
+        ["55.55.55.51", "55.55.55.52", "55.55.55.53"],
+    )
+    def test_geoip_db_returns_only_limited_data_with_missing_coordinates(self, source_ip):
+        document = {"client": {"ip": source_ip}}
+        rule_dict = {
+            "filter": "client",
+            "geoip_enricher": {
+                "source_fields": ["client.ip"],
+            },
+            "description": "",
+        }
+        self._load_specific_rule(rule_dict)
+        self.object.process(document)
+        expected_event = {
+            "client": {"ip": source_ip},
+            "geoip": {
+                "properties": {"accuracy_radius": 1337},
+                "type": "Feature",
+            },
+        }
+        assert document == expected_event
+
     @responses.activate
     def test_setup_downloads_geoip_database_if_not_exits(self):
         geoip_database_path = "http://db-path-target/db_file.mmdb"
         db_path = Path("/usr/bin/ls") if Path("/usr/bin/ls").exists() else Path("/bin/ls")
         db_path_content = db_path.read_bytes()
         expected_checksum = hashlib.md5(db_path_content).hexdigest()  # nosemgrep
         responses.add(responses.GET, geoip_database_path, db_path_content)
```

### Comparing `logprep-6.0.0/tests/unit/processor/geoip_enricher/test_geoip_enricher_rule.py` & `logprep-6.1.0/tests/unit/processor/geoip_enricher/test_geoip_enricher_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver.py` & `logprep-6.1.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 # pylint: disable=protected-access
 # pylint: disable=missing-docstring
 # pylint: disable=wrong-import-position
 # pylint: disable=wrong-import-order
+import logging
+import re
 from collections import OrderedDict
 from copy import deepcopy
 
 import pytest
 
-from logprep.processor.base.exceptions import ProcessingWarning
+from logprep.processor.base.exceptions import ProcessingCriticalError
 
 pytest.importorskip("hyperscan")
 
-from tests.unit.processor.base import BaseProcessorTestCase
-
 # pylint: disable=ungrouped-imports
-from logprep.processor.hyperscan_resolver.rule import (
-    InvalidHyperscanResolverDefinition,
-)
+from logprep.processor.hyperscan_resolver.rule import InvalidHyperscanResolverDefinition
+from tests.unit.processor.base import BaseProcessorTestCase
 
 # pylint: enable=ungrouped-imports
 
 pytest.importorskip("logprep.processor.hyperscan_resolver")
 
-from logprep.processor.hyperscan_resolver.processor import HyperscanResolver, HyperscanResolverError
+from logprep.processor.hyperscan_resolver.processor import (
+    HyperscanResolver,
+)
 
 
 class TestHyperscanResolverProcessor(BaseProcessorTestCase):
     CONFIG = {
         "type": "hyperscan_resolver",
         "specific_rules": ["tests/testdata/unit/hyperscan_resolver/rules/specific/"],
         "generic_rules": ["tests/testdata/unit/hyperscan_resolver/rules/generic/"],
@@ -338,15 +339,15 @@
         expected = {"to": {"resolve": "something HELLO1"}, "re": {"solved": "Greeting"}}
         document = {"to": {"resolve": "something HELLO1"}}
 
         self.object.process(document)
 
         assert document == expected
 
-    def test_resolve_dotted_and_dest_field_with_conflict_match(self):
+    def test_resolve_dotted_and_dest_field_with_conflict_match(self, caplog):
         rule = {
             "filter": "to.resolve",
             "hyperscan_resolver": {
                 "field_mapping": {"to.resolve": "re.solved"},
                 "resolve_list": {".*HELLO\\d": "Greeting"},
             },
         }
@@ -356,16 +357,17 @@
         document = {"to": {"resolve": "something HELLO1"}, "re": {"solved": "I already exist!"}}
         expected = {
             "to": {"resolve": "something HELLO1"},
             "re": {"solved": "I already exist!"},
             "tags": ["_hyperscan_resolver_failure"],
         }
 
-        with pytest.raises(ProcessingWarning):
+        with caplog.at_level(logging.WARNING):
             self.object.process(document)
+        assert re.match(".*FieldExistsWarning.*", caplog.text)
 
         assert document == expected
 
     def test_resolve_with_multiple_match_first_only(self):
         rule = {
             "filter": "to.resolve",
             "hyperscan_resolver": {
@@ -621,15 +623,15 @@
         }
 
         self._load_specific_rule(rule)
 
         document = {"to_resolve": "12ab34"}
 
         with pytest.raises(
-            HyperscanResolverError, match=r"No patter to compile for hyperscan database!"
+            ProcessingCriticalError, match=r"No patter to compile for hyperscan database!"
         ):
             self.object.process(document)
 
     def test_resolve_no_conflict_from_file_and_list_has_conflict(
         self,
     ):
         rule = {
```

### Comparing `logprep-6.0.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver_rule.py` & `logprep-6.1.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/processor/ip_informer/test_ip_informer.py` & `logprep-6.1.0/tests/unit/processor/ip_informer/test_ip_informer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # pylint: disable=missing-docstring
 # pylint: disable=line-too-long
+import logging
+import re
+
 import pytest
-from logprep.processor.base.exceptions import ProcessingWarning
-from tests.unit.processor.base import BaseProcessorTestCase
 
+from tests.unit.processor.base import BaseProcessorTestCase
 
 test_cases = [
     (
         "single field with ipv4 address",
         {
             "filter": "ip",
             "ip_informer": {
@@ -375,12 +377,13 @@
     @pytest.mark.parametrize("testcase, rule, event, expected", test_cases)
     def test_testcases(self, testcase, rule, event, expected):
         self._load_specific_rule(rule)
         self.object.process(event)
         assert event == expected, testcase
 
     @pytest.mark.parametrize("testcase, rule, event, expected", failure_test_cases)
-    def test_testcases_failure_handling(self, testcase, rule, event, expected):
+    def test_testcases_failure_handling(self, testcase, rule, event, expected, caplog):
         self._load_specific_rule(rule)
-        with pytest.raises(ProcessingWarning):
+        with caplog.at_level(logging.WARNING):
             self.object.process(event)
+        assert re.match(".*ProcessingWarning.*", caplog.text)
         assert event == expected, testcase
```

### Comparing `logprep-6.0.0/tests/unit/processor/ip_informer/test_ip_informer_rule.py` & `logprep-6.1.0/tests/unit/processor/ip_informer/test_ip_informer_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/processor/labeler/test_labeler.py` & `logprep-6.1.0/tests/unit/processor/labeler/test_labeler.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/processor/labeler/test_labeler_rule.py` & `logprep-6.1.0/tests/unit/processor/labeler/test_labeler_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/processor/labeler/test_labeling_schema.py` & `logprep-6.1.0/tests/unit/processor/labeler/test_labeling_schema.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/processor/list_comparison/test_list_comparison.py` & `logprep-6.1.0/tests/unit/processor/list_comparison/test_list_comparison.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # pylint: disable=missing-docstring
 # pylint: disable=protected-access
-import pytest
+import logging
+import re
+
 import responses
 
 from logprep.factory import Factory
-from logprep.processor.base.exceptions import ProcessingWarning
 from tests.unit.processor.base import BaseProcessorTestCase
 
 
 class TestListComparison(BaseProcessorTestCase):
     CONFIG = {
         "type": "list_comparison",
         "specific_rules": ["tests/testdata/unit/list_comparison/rules/specific"],
@@ -137,15 +138,15 @@
 
         assert document.get("dotted", {}).get("user_results", {}).get("not_in_list") is None
         assert len(document.get("dotted", {}).get("user_results", {}).get("in_list")) == 1
         assert (
             len(document.get("dotted", {}).get("preexistent_output_field", {}).get("in_list")) == 1
         )
 
-    def test_target_field_exists_and_cant_be_extended(self):
+    def test_target_field_exists_and_cant_be_extended(self, caplog):
         assert self.object.metrics.number_of_processed_events == 0
         document = {"dot_channel": "test", "user": "Franz", "dotted": "dotted_Franz"}
         expected = {
             "dot_channel": "test",
             "user": "Franz",
             "dotted": "dotted_Franz",
             "tags": ["_list_comparison_failure"],
@@ -158,19 +159,20 @@
                 "target_field": "dotted.user_results",
                 "list_file_paths": ["../lists/user_list.txt"],
             },
             "description": "",
         }
         self._load_specific_rule(rule_dict)
         self.object.setup()
-        with pytest.raises(ProcessingWarning):
+        with caplog.at_level(logging.WARNING):
             self.object.process(document)
+        assert re.match(".*FieldExistsWarning.*", caplog.text)
         assert document == expected
 
-    def test_intermediate_output_field_is_wrong_type(self):
+    def test_intermediate_output_field_is_wrong_type(self, caplog):
         assert self.object.metrics.number_of_processed_events == 0
         document = {
             "dot_channel": "test",
             "user": "Franz",
             "dotted": {"user_results": ["do_not_look_here"]},
         }
         expected = {
@@ -187,16 +189,17 @@
                 "target_field": "dotted.user_results.do_not_look_here",
                 "list_file_paths": ["../lists/user_list.txt"],
             },
             "description": "",
         }
         self._load_specific_rule(rule_dict)
         self.object.setup()
-        with pytest.raises(ProcessingWarning):
+        with caplog.at_level(logging.WARNING):
             self.object.process(document)
+        assert re.match(".*FieldExistsWarning.*", caplog.text)
         assert document == expected
 
     def test_check_in_dotted_subfield(self):
         assert self.object.metrics.number_of_processed_events == 0
         document = {"channel": {"type": "fast"}}
 
         self.object.process(document)
@@ -229,36 +232,32 @@
         }
         expected = {"user_results": {"in_list": ["user_list.txt"]}}
         self._load_specific_rule(rule_dict)
         self.object.setup()
         self.object.process(document)
         assert document == expected
 
-    def test_overwrite_target_field(self):
+    def test_overwrite_target_field(self, caplog):
         document = {"user": "Franz"}
         expected = {"user": "Franz", "tags": ["_list_comparison_failure"]}
         rule_dict = {
             "filter": "user",
             "list_comparison": {
                 "source_fields": ["user"],
                 "target_field": "user",
                 "list_file_paths": ["../lists/user_list.txt"],
                 "overwrite_target": True,
             },
             "description": "",
         }
         self._load_specific_rule(rule_dict)
         self.object.setup()
-        match = (
-            r"ProcessingWarning: \(Test Instance Name - The following fields could not be written, "
-            r"because one or more subfields existed and could not be extended: user\.in_list\)"
-        )
-        with pytest.raises(ProcessingWarning, match=match):
+        with caplog.at_level(logging.WARNING):
             self.object.process(document)
-
+        assert re.match(".*FieldExistsWarning.*", caplog.text)
         assert document == expected
 
     @responses.activate
     def test_list_comparison_loads_rule_with_http_template_in_list_search_base_path(self):
         responses.add(
             responses.GET,
             "http://localhost/tests/testdata/bad_users.list?ref=bla",
```

### Comparing `logprep-6.0.0/tests/unit/processor/list_comparison/test_list_comparison_rule.py` & `logprep-6.1.0/tests/unit/processor/list_comparison/test_list_comparison_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/processor/normalizer/test_normalizer.py` & `logprep-6.1.0/tests/unit/processor/normalizer/test_normalizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # pylint: disable=missing-docstring
 # pylint: disable=protected-access
 # pylint: disable=too-many-lines
 # pylint: disable=line-too-long
 import calendar
 import copy
 import json
+import logging
 import os
+import re
 import tempfile
 from copy import deepcopy
 
 import arrow
 import pytest
+
+from logprep.factory import Factory
 from logprep.processor.base.exceptions import ProcessingWarning
-from logprep.processor.normalizer.processor import NormalizerError
 from logprep.processor.normalizer.rule import (
     InvalidGrokDefinition,
     InvalidNormalizationDefinition,
     NormalizerRule,
 )
-from logprep.factory import Factory
 from tests.unit.processor.base import BaseProcessorTestCase
 
 
 class TestNormalizer(BaseProcessorTestCase):
     CONFIG = {
         "type": "normalizer",
         "specific_rules": ["tests/testdata/unit/normalizer/rules/specific/"],
@@ -57,30 +59,26 @@
             )
 
         assert (
             document["test_normalized"]["something"]
             == "Existing and normalized have the same value"
         )
 
-    def test_process_normalized_field_already_exists_with_different_content(self):
+    def test_process_normalized_field_already_exists_with_different_content(self, caplog):
         document = {
             "winlog": {
                 "api": "wineventlog",
                 "event_id": 1234,
                 "event_data": {"test_normalize": "I am new and want to be normalized!"},
             },
             "test_normalized": {"something": "I already exist but I am different!"},
         }
-        with pytest.raises(
-            ProcessingWarning,
-            match=r"ProcessingWarning: \(Test Instance Name - The following fields could not be "
-            r"written, because one or more subfields existed and could not be extended: "
-            r"test_normalized\.something\)",
-        ):
+        with caplog.at_level(logging.WARNING):
             self.object.process(document)
+        assert re.match(".*FieldExistsWarning.*", caplog.text)
 
         assert document["test_normalized"]["something"] == "I already exist but I am different!"
 
     def test_apply_windows_rules_catch_all(self):
         document = {
             "winlog": {
                 "api": "wineventlog",
@@ -621,15 +619,15 @@
         assert event.get("port_1") is None
         assert event.get("some_ip_2") is None
         assert event.get("port_2") is None
         assert event.get("winlog", {}).get("event_data", {}).get("grok_failure") == {
             "winlog>event_data>normalize me!": "123.123.123.123 1234"
         }
 
-    def test_normalization_from_grok_onto_existing(self):
+    def test_normalization_from_grok_onto_existing(self, caplog):
         event = {
             "winlog": {
                 "api": "wineventlog",
                 "event_id": 123456789,
                 "event_data": {"normalize me!": "123.123.123.123 1234"},
             }
         }
@@ -639,21 +637,17 @@
             "normalize": {
                 "winlog.event_data.normalize me!": {"grok": "%{IP:winlog} %{NUMBER:port:int}"}
             },
         }
 
         self._load_specific_rule(rule)
 
-        with pytest.raises(
-            ProcessingWarning,
-            match=r"ProcessingWarning: \(Test Instance Name - The following fields could not be "
-            r"written, because one or more subfields existed and could not be extended: "
-            r"winlog\)",
-        ):
+        with caplog.at_level(logging.WARNING):
             self.object.process(event)
+        assert re.match(".*FieldExistsWarning.*", caplog.text)
 
     def test_incorrect_grok_identifier_definition(self):
         rule = {
             "filter": "winlog.event_id: 123456789",
             "normalize": {
                 "winlog.event_data.normalize me!": {"groks": "%{IP:some_ip} %{NUMBER:port:int}"}
             },
@@ -968,24 +962,25 @@
         }
 
         self._load_specific_rule(rule)
         self.object.process(event)
 
         assert event == expected
 
-    def test_normalization_from_timestamp_with_non_matching_patterns(self):
+    def test_normalization_from_timestamp_with_non_matching_patterns(self, caplog):
         event = {
             "winlog": {
                 "api": "wineventlog",
                 "event_id": 123456789,
                 "event_data": {"some_timestamp_utc": "1999 12 12 - 12:12:22 UTC"},
             }
         }
 
         expected = copy.deepcopy(event)
+        expected.update({"tags": ["_normalizer_failure"]})
 
         rule = {
             "filter": "winlog.event_id: 123456789",
             "normalize": {
                 "winlog.event_data.some_timestamp_utc": {
                     "timestamp": {
                         "destination": "@timestamp",
@@ -994,17 +989,17 @@
                         "destination_timezone": "Europe/Berlin",
                     }
                 }
             },
         }
 
         self._load_specific_rule(rule)
-        with pytest.raises(NormalizerError):
+        with caplog.at_level(logging.WARNING):
             self.object.process(event)
-
+        assert re.match(".*NormalizerError.*", caplog.text)
         assert event == expected
 
     def test_normalization_from_timestamp_with_collision(self):
         expected = {
             "@timestamp": "1999-12-12T11:12:22Z",
             "winlog": {
                 "api": "wineventlog",
@@ -1037,27 +1032,26 @@
         }
 
         self._load_specific_rule(rule)
         self.object.process(event)
 
         assert event == expected
 
-    def test_normalization_from_timestamp_with_collision_without_allow_override_fails(
-        self,
-    ):
+    def test_normalization_from_timestamp_with_collision_without_allow_override_fails(self, caplog):
         event = {
             "@timestamp": "2200-02-01T16:19:22Z",
             "winlog": {
                 "api": "wineventlog",
                 "event_id": 123456789,
                 "event_data": {"some_timestamp_utc": "1999 12 12 - 12:12:22"},
             },
         }
 
         expected = copy.deepcopy(event)
+        expected.update({"tags": ["_normalizer_failure"]})
 
         rule = {
             "filter": "winlog.event_id: 123456789",
             "normalize": {
                 "winlog.event_data.some_timestamp_utc": {
                     "timestamp": {
                         "destination": "@timestamp",
@@ -1067,22 +1061,17 @@
                         "allow_override": False,
                     }
                 }
             },
         }
 
         self._load_specific_rule(rule)
-        with pytest.raises(
-            ProcessingWarning,
-            match=r"ProcessingWarning: \(Test Instance Name - The following fields could not be "
-            r"written, because one or more subfields existed and could not be extended: "
-            r"@timestamp\)",
-        ):
+        with caplog.at_level(logging.WARNING):
             self.object.process(event)
-
+        assert re.match(".*FieldExistsWarning.*", caplog.text)
         assert event == expected
 
     def test_normalization_with_replace_html_entity(self):
         event = {
             "tags": ["testtag"],
             "message": "replace=MAX&#43;&#8364;MORITZ&amp;dont_replace=FOO&#43;BAR&amp;id=5",
         }
```

### Comparing `logprep-6.0.0/tests/unit/processor/pre_detector/test_ip_alerter.py` & `logprep-6.1.0/tests/unit/processor/pre_detector/test_ip_alerter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/processor/pre_detector/test_pre_detector.py` & `logprep-6.1.0/tests/unit/processor/pre_detector/test_pre_detector.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/processor/pre_detector/test_pre_detector_rule.py` & `logprep-6.1.0/tests/unit/processor/pre_detector/test_pre_detector_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/processor/pseudonymizer/test_encrypter.py` & `logprep-6.1.0/tests/unit/processor/pseudonymizer/test_encrypter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/processor/pseudonymizer/test_pseudonymizer.py` & `logprep-6.1.0/tests/unit/processor/pseudonymizer/test_pseudonymizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # pylint: disable=missing-docstring
 # pylint: disable=protected-access
+# pylint: disable=attribute-defined-outside-init
+# pylint: disable=too-many-public-methods
 import datetime
+import re
 import time
 from copy import deepcopy
 from pathlib import Path
 
 import pytest
 
 from logprep.factory import Factory
@@ -775,10 +778,11 @@
     def test_replace_regex_keywords_by_regex_expression_can_be_called_multiple_times(self):
         rule_dict = {
             "filter": "event_id: 1234",
             "pseudonymizer": {"pseudonyms": {"something": "RE_WHOLE_FIELD"}},
             "description": "description content irrelevant for these tests",
         }
         self._load_specific_rule(rule_dict)  # First call
-        assert self.object._specific_tree.rules[0].pseudonyms == {"something": "(.*)"}
+        expected_pattern = re.compile("(.*)")
+        assert self.object._specific_tree.rules[0].pseudonyms == {"something": expected_pattern}
         self.object._replace_regex_keywords_by_regex_expression()  # Second Call
-        assert self.object._specific_tree.rules[0].pseudonyms == {"something": "(.*)"}
+        assert self.object._specific_tree.rules[0].pseudonyms == {"something": expected_pattern}
```

### Comparing `logprep-6.0.0/tests/unit/processor/pseudonymizer/test_pseudonymizer_rule.py` & `logprep-6.1.0/tests/unit/processor/pseudonymizer/test_pseudonymizer_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/processor/requester/test_requester.py` & `logprep-6.1.0/tests/unit/processor/requester/test_requester.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # pylint: disable=missing-docstring
+import logging
+import re
 
 import pytest
 import responses
 from requests import ConnectTimeout, HTTPError
 from responses import matchers
 
-from logprep.processor.base.exceptions import ProcessingWarning
 from tests.unit.processor.base import BaseProcessorTestCase
 
 test_cases = [
     (
         "simple request",
         {"filter": "message", "requester": {"url": "http://mock-mock", "method": "GET"}},
         {"message": "the message"},
@@ -267,14 +268,15 @@
         {
             "method": "GET",
             "url": "http://failure_mock",
             "body": HTTPError("404"),
             "content_type": "text/plain",
             "status": 404,
         },
+        ".*ProcessingWarning.*",
     ),
     (
         "timout error",
         {
             "filter": "message",
             "requester": {"url": "http://failure_mock", "method": "GET", "timeout": 0.2},
         },
@@ -283,14 +285,15 @@
         {
             "method": "GET",
             "url": "http://failure_mock",
             "body": ConnectTimeout(),
             "content_type": "text/plain",
             "status": 200,
         },
+        ".*ProcessingWarning.*",
     ),
     (
         "does not overwrite if not permitted",
         {
             "filter": "message",
             "requester": {
                 "url": "http://failure_mock",
@@ -303,26 +306,28 @@
         {
             "method": "GET",
             "url": "http://failure_mock",
             "body": "the body",
             "content_type": "text/plain",
             "status": 200,
         },
+        ".*FieldExistsWarning.*",
     ),
     (
         "errors on missing fields",
         {
             "filter": "message",
             "requester": {"url": "http://${missingfield}", "method": "GET"},
         },
         {"message": "the message"},
         {"message": "the message", "tags": ["_requester_failure"]},
         {},
+        ".*ProcessingWarning.*",
     ),
-]  # testcase, rule, event, expected, mock
+]  # testcase, rule, event, expected, mock, error_message
 
 
 class TestRequester(BaseProcessorTestCase):
     CONFIG: dict = {
         "type": "requester",
         "specific_rules": ["tests/testdata/unit/requester/specific_rules"],
         "generic_rules": ["tests/testdata/unit/requester/generic_rules"],
@@ -333,23 +338,26 @@
     def test_testcases(self, testcase, rule, event, expected, response_kwargs):
         responses.add(responses.Response(**response_kwargs))
         self._load_specific_rule(rule)
         self.object.process(event)
         assert event == expected, testcase
 
     @responses.activate
-    @pytest.mark.parametrize("testcase, rule, event, expected, response_kwargs", failure_test_cases)
+    @pytest.mark.parametrize(
+        "testcase, rule, event, expected, response_kwargs, error_message", failure_test_cases
+    )
     def test_requester_testcases_failure_handling(
-        self, testcase, rule, event, expected, response_kwargs
+        self, testcase, rule, event, expected, response_kwargs, error_message, caplog
     ):
         if response_kwargs:
             responses.add(responses.Response(**response_kwargs))
         self._load_specific_rule(rule)
-        with pytest.raises(ProcessingWarning):
+        with caplog.at_level(logging.WARNING):
             self.object.process(event)
+        assert re.match(error_message, caplog.text)
         assert event == expected, testcase
 
     @responses.activate
     def test_process(self):
         responses.add(
             responses.Response(
                 **{
```

### Comparing `logprep-6.0.0/tests/unit/processor/requester/test_requester_rule.py` & `logprep-6.1.0/tests/unit/processor/requester/test_requester_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/processor/selective_extractor/test_selective_extractor.py` & `logprep-6.1.0/tests/unit/processor/selective_extractor/test_selective_extractor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/processor/selective_extractor/test_selective_extractor_rule.py` & `logprep-6.1.0/tests/unit/processor/selective_extractor/test_selective_extractor_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/processor/string_splitter/test_string_splitter.py` & `logprep-6.1.0/tests/unit/processor/string_splitter/test_string_splitter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # pylint: disable=missing-docstring
+import logging
+import re
+
 import pytest
-from logprep.processor.base.exceptions import ProcessingWarning
-from tests.unit.processor.base import BaseProcessorTestCase
 
+from tests.unit.processor.base import BaseProcessorTestCase
 
 test_cases = [
     (
         "splits without delimeter on whitespace",
         {
             "filter": "message",
             "string_splitter": {"source_fields": ["message"], "target_field": "result"},
@@ -34,25 +36,27 @@
         "splits without delimeter on whitespace",
         {
             "filter": "message",
             "string_splitter": {"source_fields": ["message"], "target_field": "result"},
         },
         {"message": ["this", "is", "the", "message"]},
         {"message": ["this", "is", "the", "message"], "tags": ["_string_splitter_failure"]},
+        ".*ProcessingWarning.*",
     ),
     (
         "splits without delimeter on whitespace",
         {
             "filter": "message",
             "string_splitter": {"source_fields": ["message"], "target_field": "message"},
         },
         {"message": "this is the message"},
         {"message": "this is the message", "tags": ["_string_splitter_failure"]},
+        ".*FieldExistsWarning.*",
     ),
-]  # testcase, rule, event, expected
+]  # testcase, rule, event, expected, error_message
 
 
 class TestStringSplitter(BaseProcessorTestCase):
     CONFIG: dict = {
         "type": "string_splitter",
         "specific_rules": ["tests/testdata/unit/string_splitter/specific/"],
         "generic_rules": ["tests/testdata/unit/string_splitter/generic/"],
@@ -60,13 +64,16 @@
 
     @pytest.mark.parametrize("testcase, rule, event, expected", test_cases)
     def test_testcases(self, testcase, rule, event, expected):  # pylint: disable=unused-argument
         self._load_specific_rule(rule)
         self.object.process(event)
         assert event == expected
 
-    @pytest.mark.parametrize("testcase, rule, event, expected", failure_test_cases)
-    def test_testcases_failure_handling(self, testcase, rule, event, expected):
+    @pytest.mark.parametrize("testcase, rule, event, expected, error_message", failure_test_cases)
+    def test_testcases_failure_handling(
+        self, testcase, rule, event, expected, error_message, caplog
+    ):
         self._load_specific_rule(rule)
-        with pytest.raises(ProcessingWarning):
+        with caplog.at_level(logging.WARNING):
             self.object.process(event)
+        assert re.match(error_message, caplog.text)
         assert event == expected, testcase
```

### Comparing `logprep-6.0.0/tests/unit/processor/string_splitter/test_string_splitter_rule.py` & `logprep-6.1.0/tests/unit/processor/string_splitter/test_string_splitter_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/processor/template_replacer/test_template_replacer.py` & `logprep-6.1.0/tests/unit/processor/template_replacer/test_template_replacer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # pylint: disable=missing-module-docstring
+import logging
+import re
 from copy import deepcopy
 
 import pytest
 
 from logprep.factory import Factory
 from logprep.processor.template_replacer.processor import TemplateReplacerError
 from tests.unit.processor.base import BaseProcessorTestCase
@@ -139,30 +141,27 @@
 
         self.object.process(document)
 
         assert document.get("dotted")
         assert document["dotted"].get("message")
         assert document["dotted"]["message"] == "Test %1 Test %2"
 
-    def test_replace_incompatible_existing_dotted_message_parent_via_template(self):
+    def test_replace_incompatible_existing_dotted_message_parent_via_template(self, caplog):
         config = deepcopy(self.CONFIG)
         config.get("pattern").update({"target_field": "dotted.message"})
         self.object = Factory.create({"test instance": config}, self.logger)
         assert self.object.metrics.number_of_processed_events == 0
         document = {
             "winlog": {"channel": "System", "provider_name": "Test", "event_id": 123},
             "dotted": "foo",
         }
 
-        with pytest.raises(
-            TemplateReplacerError,
-            match="Parent field 'dotted' of target field 'dotted.message' exists "
-            "and is not a dict!",
-        ):
+        with caplog.at_level(logging.WARNING):
             self.object.process(document)
+        assert re.match(".*FieldExistsWarning.*", caplog.text)
 
     def test_replace_fails_with_invalid_template(self):
         config = deepcopy(self.CONFIG)
         config.update(
             {"template": "tests/testdata/unit/template_replacer/replacer_template_invalid.yml"}
         )
         with pytest.raises(TemplateReplacerError, match="Not enough delimiters"):
```

### Comparing `logprep-6.0.0/tests/unit/processor/test_processor_rule.py` & `logprep-6.1.0/tests/unit/processor/test_processor_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/processor/timestamp_differ/test_timestamp_differ.py` & `logprep-6.1.0/tests/unit/processor/timestamp_differ/test_timestamp_differ.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # pylint: disable=missing-docstring
+import logging
+import re
 
 import pytest
 
-from logprep.processor.base.exceptions import ProcessingWarning
 from tests.unit.processor.base import BaseProcessorTestCase
 
 test_cases = [  # testcase, rule, event, expected
     (
         "Time difference between two timestamps",
         {
             "filter": "field1 AND field2",
@@ -355,15 +356,15 @@
         },
         {"field1": "non-timestamp", "subfield": {"field2": "2022-12-05 12:00:00"}},
         {
             "field1": "non-timestamp",
             "subfield": {"field2": "2022-12-05 12:00:00"},
             "tags": ["_timestamp_differ_failure"],
         },
-        r"Could not match input 'non-timestamp' to any of the following formats",
+        r".*ProcessingWarning.*Could not match input 'non-timestamp' to any of the following formats",
     ),
     (
         "diff between two timestamps with partial timestamp format match",
         {
             "filter": "field1 AND subfield.field2",
             "timestamp_differ": {
                 "diff": "${subfield.field2:YYYY-MM-DD HH:mm:ss} - ${field1:YYYY-MM-DD HH:mm:ss}",
@@ -372,15 +373,15 @@
         },
         {"field1": "2022-12-05", "subfield": {"field2": "2022-12-05 12:00:00"}},
         {
             "field1": "2022-12-05",
             "subfield": {"field2": "2022-12-05 12:00:00"},
             "tags": ["_timestamp_differ_failure"],
         },
-        "Failed to match 'YYYY-MM-DD HH:mm:ss' when parsing",
+        ".*ProcessingWarning.*Failed to match 'YYYY-MM-DD HH:mm:ss' when parsing",
     ),
     (
         "diff between two timestamps with one empty field",
         {
             "filter": "field1 AND subfield.field2",
             "timestamp_differ": {
                 "diff": "${subfield.field2:YYYY-MM-DD HH:mm:ss} - ${field1:YYYY-MM-DD HH:mm:ss}",
@@ -389,15 +390,15 @@
         },
         {"field1": "2022-12-05", "subfield": {"field2": ""}},
         {
             "field1": "2022-12-05",
             "subfield": {"field2": ""},
             "tags": ["_timestamp_differ_failure"],
         },
-        r"no value for fields: \['subfield.field2'\]",
+        r".*ProcessingWarning.*no value for fields: \['subfield.field2'\]",
     ),
     (
         "diff between two timestamps with one non existing field",
         {
             "filter": "field1",
             "timestamp_differ": {
                 "diff": "${subfield.field2:YYYY-MM-DD HH:mm:ss} - ${field1:YYYY-MM-DD HH:mm:ss}",
@@ -405,15 +406,15 @@
             },
         },
         {"field1": "2022-12-05"},
         {
             "field1": "2022-12-05",
             "tags": ["_timestamp_differ_failure"],
         },
-        r"no value for fields: \['subfield.field2'\]",
+        r".*ProcessingWarning.*no value for fields: \['subfield.field2'\]",
     ),
     (
         "diff between two timestamps with non existing fields",
         {
             "filter": "some_field",
             "timestamp_differ": {
                 "diff": "${subfield.field2:YYYY-MM-DD HH:mm:ss} - ${field1:YYYY-MM-DD HH:mm:ss}",
@@ -421,15 +422,15 @@
             },
         },
         {"some_field": "some value"},
         {
             "some_field": "some value",
             "tags": ["_timestamp_differ_failure"],
         },
-        r"no value for fields: \['subfield.field2', 'field1'\]",
+        r".*ProcessingWarning.*no value for fields: \['subfield.field2', 'field1'\]",
     ),
     (
         "diff between two timestamps with already existing output field",
         {
             "filter": "field1 AND field2",
             "timestamp_differ": {
                 "diff": "${field2:YYYY-MM-DD HH:mm:ss} - ${field1:YYYY-MM-DD HH:mm:ss}",
@@ -439,15 +440,15 @@
         {"field1": "2022-12-05 11:38:42", "field2": "2022-12-05 12:00:00", "time_diff": "1278"},
         {
             "field1": "2022-12-05 11:38:42",
             "field2": "2022-12-05 12:00:00",
             "time_diff": "1278",
             "tags": ["_timestamp_differ_failure"],
         },
-        "The following fields could not be written, because one or more subfields existed and could not be extended: time_diff",
+        ".*FieldExistsWarning.*The following fields could not be written, because one or more subfields existed and could not be extended: time_diff",
     ),
 ]
 
 
 class TestTimestampDiffer(BaseProcessorTestCase):
     CONFIG: dict = {
         "type": "timestamp_differ",
@@ -458,12 +459,15 @@
     @pytest.mark.parametrize("testcase, rule, event, expected", test_cases)
     def test_testcases(self, testcase, rule, event, expected):
         self._load_specific_rule(rule)
         self.object.process(event)
         assert event == expected, testcase
 
     @pytest.mark.parametrize("testcase, rule, event, expected, error_message", failure_test_cases)
-    def test_testcases_failure_handling(self, testcase, rule, event, expected, error_message):
+    def test_testcases_failure_handling(
+        self, testcase, rule, event, expected, error_message, caplog
+    ):
         self._load_specific_rule(rule)
-        with pytest.raises(ProcessingWarning, match=error_message):
+        with caplog.at_level(logging.WARNING):
             self.object.process(event)
+        assert re.match(error_message, caplog.text)
         assert event == expected, testcase
```

### Comparing `logprep-6.0.0/tests/unit/processor/timestamp_differ/test_timestamp_differ_rule.py` & `logprep-6.1.0/tests/unit/processor/timestamp_differ/test_timestamp_differ_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/test_configuration.py` & `logprep-6.1.0/tests/unit/test_configuration.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/test_factory.py` & `logprep-6.1.0/tests/unit/test_factory.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/test_run_logprep.py` & `logprep-6.1.0/tests/unit/test_run_logprep.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/test_runner.py` & `logprep-6.1.0/tests/unit/test_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from copy import deepcopy
 from functools import partial
 from logging import ERROR, INFO, Logger
 from os.path import join, split
 from unittest import mock
 
 from pytest import raises
-from requests.exceptions import SSLError, HTTPError
+from requests.exceptions import HTTPError, SSLError
 
 from logprep.processor.labeler.labeling_schema import LabelingSchemaError
 from logprep.runner import (
     CannotReloadWhenConfigIsUnsetError,
     MustConfigureALoggerError,
     MustConfigureBeforeRunningError,
     MustNotConfigureTwiceError,
```

### Comparing `logprep-6.0.0/tests/unit/util/test_auto_rule_corpus_tester.py` & `logprep-6.1.0/tests/unit/util/test_auto_rule_corpus_tester.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # pylint: disable=missing-docstring
 # pylint: disable=protected-access
+# pylint: disable=too-many-arguments
 import json
 import os
 from json import JSONDecodeError
 from unittest import mock
 
 import pytest
 
@@ -15,24 +16,27 @@
 def fixture_auto_rule_corpus_tester():
     config_path = "tests/testdata/config/config.yml"
     data_dir = "will be overwritten in test cases"
     corpus_tester = RuleCorpusTester(config_path, data_dir)
     return corpus_tester
 
 
-def prepare_corpus_tester(corpus_tester, tmp_path, test_data):
-    case_name = "rule_auto_corpus_test"
-    test_data_dir = tmp_path / "test_data"
-    os.makedirs(test_data_dir, exist_ok=True)
-    input_data_path = test_data_dir / f"{case_name}_in.json"
+def write_test_case_data_tmp_files(test_data_dir, test_case_name, test_data):
+    input_data_path = test_data_dir / f"{test_case_name}_in.json"
     input_data_path.write_text(json.dumps(test_data.get("input")))
-    expected_output_data_path = test_data_dir / f"{case_name}_out.json"
+    expected_output_data_path = test_data_dir / f"{test_case_name}_out.json"
     expected_output_data_path.write_text(json.dumps(test_data.get("expected_output")))
-    expected_extra_output_data_path = test_data_dir / f"{case_name}_out_extra.json"
+    expected_extra_output_data_path = test_data_dir / f"{test_case_name}_out_extra.json"
     expected_extra_output_data_path.write_text(json.dumps(test_data.get("expected_extra_output")))
+
+
+def prepare_corpus_tester(corpus_tester, tmp_path, test_data):
+    test_data_dir = tmp_path / "test_data"
+    os.makedirs(test_data_dir, exist_ok=True)
+    write_test_case_data_tmp_files(test_data_dir, "rule_auto_corpus_test", test_data)
     corpus_tester._input_test_data_path = test_data_dir
     corpus_tester._tmp_dir = tmp_path
 
 
 class TestAutoRuleTester:
     @pytest.mark.parametrize(
         "test_case, test_data, mock_output, expected_prints, exit_code",
@@ -314,20 +318,21 @@
                 "logprep.util.auto_rule_tester.auto_rule_corpus_tester.Pipeline.process_pipeline"
             ) as mock_process_pipeline:
                 mock_process_pipeline.return_value = mock_output
                 corpus_tester.run()
         else:
             corpus_tester.run()
         console_output, console_error = capsys.readouterr()
+        assert console_error == ""
         for expected_print in expected_prints:
             assert expected_print in console_output, test_case
         mock_exit.assert_called_with(exit_code)
 
     @mock.patch("logprep.util.auto_rule_tester.auto_rule_corpus_tester.parse_json")
-    def test_run_logs_json_decoding_error(self, mock_parse_json, tmp_path, corpus_tester, capsys):
+    def test_run_logs_json_decoding_error(self, mock_parse_json, tmp_path, corpus_tester):
         test_data = {"input": {}, "expected_output": {}, "expected_extra_output": []}
         prepare_corpus_tester(corpus_tester, tmp_path, test_data)
         mock_parse_json.side_effect = JSONDecodeError("Some Error", "in doc", 0)
         with pytest.raises(ValueError, match="Following parsing errors were found"):
             corpus_tester.run()
 
     def test_run_raises_if_case_misses_input_file(self, tmp_path, corpus_tester):
@@ -352,14 +357,15 @@
             "Total test cases: 1",
             "Success rate: 100.00%",
         ]
         prepare_corpus_tester(corpus_tester, tmp_path, test_data)
         os.remove(tmp_path / "test_data" / "rule_auto_corpus_test_out.json")
         corpus_tester.run()
         console_output, console_error = capsys.readouterr()
+        assert console_error == ""
         for expected_print in expected_prints:
             assert expected_print in console_output
         mock_exit.assert_called_with(0)
 
     @mock.patch("logprep.util.auto_rule_tester.auto_rule_corpus_tester.shutil.rmtree")
     @mock.patch("logprep.util.auto_rule_tester.auto_rule_corpus_tester.sys.exit")
     def test_run_removes_test_tmp_dir(self, _, mock_shutil, corpus_tester):
@@ -410,10 +416,52 @@
             "PASSED",
             "Total test cases: 1",
             "Success rate: 100.00%",
         ]
         prepare_corpus_tester(corpus_tester, tmp_path, test_data)
         corpus_tester.run()
         console_output, console_error = capsys.readouterr()
+        assert console_error == ""
+        for expected_print in expected_prints:
+            assert expected_print in console_output
+        mock_exit.assert_called_with(0)
+
+    @mock.patch("logprep.util.auto_rule_tester.auto_rule_corpus_tester.sys.exit")
+    def test_corpus_tests_dont_share_cache_between_runs_by_resetting_processors(
+        self, mock_exit, tmp_path, capsys
+    ):
+        test_case_data = {
+            "input": {
+                "winlog": {"event_id": "2222", "event_data": {"IpAddress": "1.2.3.4"}},
+            },
+            "expected_output": {
+                "winlog": {"event_id": "2222", "event_data": {"IpAddress": "<IGNORE_VALUE>"}},
+            },
+            "expected_extra_output": [
+                {
+                    "({'kafka_output': 'pseudonyms'},)": {
+                        "origin": "<IGNORE_VALUE>",
+                        "pseudonym": "<IGNORE_VALUE>",
+                    }
+                },
+            ],
+        }
+        test_data_dir = tmp_path / "test_data"
+        os.makedirs(test_data_dir, exist_ok=True)
+        # run one test case two times to trigger the pseudonymizer cache.
+        # Without reinitializing the processors the second test wouldn't create an extra output, as
+        # the cache realizes it as an existing pseudonym already.
+        write_test_case_data_tmp_files(test_data_dir, "test_case_one", test_case_data)
+        write_test_case_data_tmp_files(test_data_dir, "test_case_two", test_case_data)
+        config_path = "tests/testdata/config/config.yml"
+        corpus_tester = RuleCorpusTester(config_path, test_data_dir)
+        corpus_tester.run()
+        console_output, console_error = capsys.readouterr()
+        assert console_error == ""
+        expected_prints = [
+            "PASSED",
+            "Total test cases: 2",
+            "Success rate: 100.00%",
+        ]
         for expected_print in expected_prints:
             assert expected_print in console_output
         mock_exit.assert_called_with(0)
```

### Comparing `logprep-6.0.0/tests/unit/util/test_auto_rule_tester.py` & `logprep-6.1.0/tests/unit/util/test_auto_rule_tester.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/util/test_cache.py` & `logprep-6.1.0/tests/unit/util/test_cache.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/util/test_configuration.py` & `logprep-6.1.0/tests/unit/util/test_configuration.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/util/test_getter.py` & `logprep-6.1.0/tests/unit/util/test_getter.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
 
     def test_factory_returns_file_getter_with_protocol(self):
         file_getter = GetterFactory.from_string("file:///my/file")
         assert isinstance(file_getter, FileGetter)
 
     def test_get_returns_content(self):
         file_getter = GetterFactory.from_string("/my/file")
-        with mock.patch("pathlib.Path.open", mock.mock_open(read_data=b"my content")) as mock_open:
+        with mock.patch("pathlib.Path.open", mock.mock_open(read_data=b"my content")) as _:
             content = file_getter.get()
             assert content == "my content"
 
     def test_get_returns_binary_content(self):
         file_getter = GetterFactory.from_string("/my/file")
         with mock.patch("pathlib.Path.open", mock.mock_open(read_data=b"my content")) as mock_open:
             content = file_getter.get_raw()
```

### Comparing `logprep-6.0.0/tests/unit/util/test_grok_pattern_loader.py` & `logprep-6.1.0/tests/unit/util/test_grok_pattern_loader.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/util/test_helper.py` & `logprep-6.1.0/tests/unit/util/test_helper.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/util/test_helper_add_field.py` & `logprep-6.1.0/tests/unit/util/test_helper_add_field.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/util/test_log_aggregator.py` & `logprep-6.1.0/tests/unit/util/test_log_aggregator.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/util/test_processor_generator.py` & `logprep-6.1.0/tests/unit/util/test_processor_generator.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/util/test_prometheus_exporter.py` & `logprep-6.1.0/tests/unit/util/test_prometheus_exporter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/util/test_rule_dry_runner.py` & `logprep-6.1.0/tests/unit/util/test_rule_dry_runner.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # pylint: disable=missing-docstring
 # pylint: disable=attribute-defined-outside-init
 import json
 import logging
 import os
-import re
 import tempfile
-from unittest import mock
 
 from logprep.util.rule_dry_runner import DryRunner
 
 
 class TestRunLogprep:
     def setup_method(self):
         config = """
@@ -168,31 +166,7 @@
         )
         dry_runner.run()
 
         captured = capsys.readouterr()
         assert "------ PROCESSED EVENT ------" in captured.out
         assert "------ TRANSFORMED EVENTS: 1/1 ------" in captured.out
         assert "------ CUSTOM OUTPUTS ------" in captured.out
-
-    @mock.patch("logprep.processor.labeler.processor.Labeler.process", side_effect=BaseException)
-    def test_dry_run_prints_errors(self, _, tmp_path, capsys):
-        test_json = {
-            "winlog": {
-                "event_id": 123,
-                "event_data": {"ServiceName": "VERY BAD"},
-            }
-        }
-        input_json_file = os.path.join(tmp_path, "test_input.json")
-        with open(input_json_file, "w", encoding="utf8") as input_file:
-            json.dump(test_json, input_file)
-
-        dry_runner = DryRunner(
-            input_file_path=input_json_file,
-            config_path=self.config_path,
-            full_output=True,
-            use_json=True,
-            logger=logging.getLogger("test-logger"),
-        )
-        dry_runner.run()
-
-        captured = capsys.readouterr()
-        assert not re.match(r".*A critical error occured for processor Labeler", captured.err)
```

### Comparing `logprep-6.0.0/tests/unit/util/test_time_measurement.py` & `logprep-6.1.0/tests/unit/util/test_time_measurement.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/util/test_validators.py` & `logprep-6.1.0/tests/unit/util/test_validators.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/unit/util/tests_json_handling.py` & `logprep-6.1.0/tests/unit/util/tests_json_handling.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/tests/util/testhelpers.py` & `logprep-6.1.0/tests/util/testhelpers.py`

 * *Files identical despite different names*

### Comparing `logprep-6.0.0/versioneer.py` & `logprep-6.1.0/versioneer.py`

 * *Files identical despite different names*

