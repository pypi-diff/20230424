# Comparing `tmp/scylla-driver-3.26.0.tar.gz` & `tmp/scylla-driver-3.26.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scylla-driver-3.26.0.tar", last modified: Thu Apr 13 14:29:15 2023, max compression
+gzip compressed data, was "scylla-driver-3.26.1.tar", last modified: Mon Apr 24 14:45:46 2023, max compression
```

## Comparing `scylla-driver-3.26.0.tar` & `scylla-driver-3.26.1.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:29:15.790249 scylla-driver-3.26.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-04-13 14:29:15.786249 scylla-driver-3.26.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:29:15.782249 scylla-driver-3.26.0/cassandra/
--rw-r--r--   0 runner    (1001) docker     (123)    19691 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10777 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/buffer.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/bytesio.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/bytesio.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/c_shard_info.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   239424 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     6516 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/cmurmur3.c
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)    69867 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:29:15.782249 scylla-driver-3.26.0/cassandra/cqlengine/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/cqlengine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33173 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/cqlengine/columns.py
--rw-r--r--   0 runner    (1001) docker     (123)    14372 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/cqlengine/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/cqlengine/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    23480 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/cqlengine/management.py
--rw-r--r--   0 runner    (1001) docker     (123)    38850 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/cqlengine/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/cqlengine/named.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/cqlengine/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)    56369 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/cqlengine/query.py
--rw-r--r--   0 runner    (1001) docker     (123)    29542 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/cqlengine/statements.py
--rw-r--r--   0 runner    (1001) docker     (123)     7432 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/cqlengine/usertype.py
--rw-r--r--   0 runner    (1001) docker     (123)    47427 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/cqltypes.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/cython_deps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/cython_marshal.pyx
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/cython_utils.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/cython_utils.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:29:15.782249 scylla-driver-3.26.0/cassandra/datastax/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/datastax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:29:15.782249 scylla-driver-3.26.0/cassandra/datastax/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/datastax/cloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:29:15.786249 scylla-driver-3.26.0/cassandra/datastax/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/datastax/graph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:29:15.786249 scylla-driver-3.26.0/cassandra/datastax/graph/fluent/
--rw-r--r--   0 runner    (1001) docker     (123)    12811 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/datastax/graph/fluent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/datastax/graph/fluent/_predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     7820 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/datastax/graph/fluent/_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/datastax/graph/fluent/_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/datastax/graph/fluent/predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/datastax/graph/fluent/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/datastax/graph/fluent/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)    35798 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/datastax/graph/graphson.py
--rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/datastax/graph/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/datastax/graph/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:29:15.786249 scylla-driver-3.26.0/cassandra/datastax/insights/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/datastax/insights/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/datastax/insights/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/datastax/insights/reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/datastax/insights/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/datastax/insights/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/deserializers.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    16917 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/deserializers.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:29:15.786249 scylla-driver-3.26.0/cassandra/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/graph/graphson.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/graph/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/graph/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:29:15.786249 scylla-driver-3.26.0/cassandra/io/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/io/asyncioreactor.py
--rw-r--r--   0 runner    (1001) docker     (123)    14418 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/io/asyncorereactor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/io/eventletreactor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/io/geventreactor.py
--rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/io/libevreactor.py
--rw-r--r--   0 runner    (1001) docker     (123)    22348 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/io/libevwrapper.c
--rw-r--r--   0 runner    (1001) docker     (123)    10333 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/io/twistedreactor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/ioutils.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/marshal.py
--rw-r--r--   0 runner    (1001) docker     (123)   136904 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/murmur3.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/numpyFlags.h
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/numpy_parser.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/obj_parser.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/parsing.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/parsing.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    43701 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/policies.py
--rw-r--r--   0 runner    (1001) docker     (123)    49766 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    48183 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)    42069 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/row_parser.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:29:15.786249 scylla-driver-3.26.0/cassandra/scylla/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/scylla/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/scylla/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/segment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/shard_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/timestamps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/tuple.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/type_codes.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/type_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)    65131 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/ez_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:29:15.786249 scylla-driver-3.26.0/scylla_driver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-04-13 14:29:15.000000 scylla-driver-3.26.0/scylla_driver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-13 14:29:15.000000 scylla-driver-3.26.0/scylla_driver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 14:29:15.000000 scylla-driver-3.26.0/scylla_driver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 14:29:15.000000 scylla-driver-3.26.0/scylla_driver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 14:29:15.000000 scylla-driver-3.26.0/scylla_driver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 14:29:15.790249 scylla-driver-3.26.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    17231 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:45:46.235679 scylla-driver-3.26.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-04-24 14:45:46.235679 scylla-driver-3.26.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:45:46.231678 scylla-driver-3.26.1/cassandra/
+-rw-r--r--   0 runner    (1001) docker     (123)    19691 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10777 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/buffer.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/bytesio.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/bytesio.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/c_shard_info.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   232919 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6516 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/cmurmur3.c
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69867 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:45:46.231678 scylla-driver-3.26.1/cassandra/cqlengine/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/cqlengine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33173 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/cqlengine/columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14372 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/cqlengine/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/cqlengine/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23480 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/cqlengine/management.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38850 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/cqlengine/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/cqlengine/named.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/cqlengine/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56369 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/cqlengine/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29542 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/cqlengine/statements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7432 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/cqlengine/usertype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47427 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/cqltypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/cython_deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/cython_marshal.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/cython_utils.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/cython_utils.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:45:46.231678 scylla-driver-3.26.1/cassandra/datastax/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/datastax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:45:46.231678 scylla-driver-3.26.1/cassandra/datastax/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/datastax/cloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:45:46.231678 scylla-driver-3.26.1/cassandra/datastax/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/datastax/graph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:45:46.231678 scylla-driver-3.26.1/cassandra/datastax/graph/fluent/
+-rw-r--r--   0 runner    (1001) docker     (123)    12811 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/datastax/graph/fluent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/datastax/graph/fluent/_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7820 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/datastax/graph/fluent/_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/datastax/graph/fluent/_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/datastax/graph/fluent/predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/datastax/graph/fluent/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/datastax/graph/fluent/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35798 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/datastax/graph/graphson.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/datastax/graph/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/datastax/graph/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:45:46.235679 scylla-driver-3.26.1/cassandra/datastax/insights/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/datastax/insights/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/datastax/insights/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/datastax/insights/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/datastax/insights/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/datastax/insights/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/deserializers.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    16917 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/deserializers.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:45:46.235679 scylla-driver-3.26.1/cassandra/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/graph/graphson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/graph/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/graph/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:45:46.235679 scylla-driver-3.26.1/cassandra/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/io/asyncioreactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14418 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/io/asyncorereactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/io/eventletreactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/io/geventreactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/io/libevreactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22348 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/io/libevwrapper.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10333 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/io/twistedreactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/ioutils.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/marshal.py
+-rw-r--r--   0 runner    (1001) docker     (123)   136904 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/murmur3.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/numpyFlags.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/numpy_parser.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/obj_parser.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/parsing.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/parsing.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    43701 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49766 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48183 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42069 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/row_parser.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:45:46.235679 scylla-driver-3.26.1/cassandra/scylla/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/scylla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/scylla/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/shard_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/timestamps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/tuple.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/type_codes.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/type_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65131 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/cassandra/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/ez_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:45:46.235679 scylla-driver-3.26.1/scylla_driver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-04-24 14:45:46.000000 scylla-driver-3.26.1/scylla_driver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-24 14:45:46.000000 scylla-driver-3.26.1/scylla_driver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 14:45:46.000000 scylla-driver-3.26.1/scylla_driver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-24 14:45:46.000000 scylla-driver-3.26.1/scylla_driver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-24 14:45:46.000000 scylla-driver-3.26.1/scylla_driver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 14:45:46.235679 scylla-driver-3.26.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    17231 2023-04-24 14:45:38.000000 scylla-driver-3.26.1/setup.py
```

### Comparing `scylla-driver-3.26.0/LICENSE` & `scylla-driver-3.26.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/PKG-INFO` & `scylla-driver-3.26.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scylla-driver
-Version: 3.26.0
+Version: 3.26.1
 Summary: Scylla Driver for Apache Cassandra
 Home-page: https://github.com/scylladb/python-driver
 Author: ScyllaDB
 Project-URL: Documentation, https://scylladb.github.io/python-driver/
 Project-URL: Source, https://github.com/scylladb/python-driver/
 Project-URL: Issues, https://github.com/scylladb/python-driver/issues
 Keywords: cassandra,cql,orm,dse,graph
```

### Comparing `scylla-driver-3.26.0/README.rst` & `scylla-driver-3.26.1/README.rst`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/__init__.py` & `scylla-driver-3.26.1/cassandra/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 class NullHandler(logging.Handler):
 
     def emit(self, record):
         pass
 
 logging.getLogger('cassandra').addHandler(NullHandler())
 
-__version_info__ = (3, 26, 0)
+__version_info__ = (3, 26, 1)
 __version__ = '.'.join(map(str, __version_info__))
 
 
 class ConsistencyLevel(object):
     """
     Spcifies how many replicas must respond for an operation to be considered
     a success.  By default, ``ONE`` is used for all operations.
```

### Comparing `scylla-driver-3.26.0/cassandra/auth.py` & `scylla-driver-3.26.1/cassandra/auth.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/buffer.pxd` & `scylla-driver-3.26.1/cassandra/buffer.pxd`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/bytesio.pxd` & `scylla-driver-3.26.1/cassandra/bytesio.pxd`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/bytesio.pyx` & `scylla-driver-3.26.1/cassandra/bytesio.pyx`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/c_shard_info.pyx` & `scylla-driver-3.26.1/cassandra/c_shard_info.pyx`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/cluster.py` & `scylla-driver-3.26.1/cassandra/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -3779,146 +3779,14 @@
         if not agreed:
             log.debug("Skipping schema refresh due to lack of schema agreement")
             return False
 
         self._cluster.metadata.refresh(connection, self._timeout, fetch_size=self._schema_meta_page_size, **kwargs)
 
         return True
-    
-    # Three functions below (_refresh_schema_async, _refresh_schema_async_inner, _wait_for_schema_agreement_async) are async
-    # versions of the functions without _async in name - instead of blocking and returning result, their first argument
-    # is a callback that will receive either a result or an exception.
-    # Purpose of those functions is to avoid filling whole thread pool and deadlocking.
-    def _refresh_schema_async(self, callback, force=False, **kwargs):
-        def new_callback(e):
-            if isinstance(e, ReferenceError):
-                # our weak reference to the Cluster is no good
-                callback(False)
-                return
-            elif isinstance(e, Exception):
-                log.debug("[control connection] Error refreshing schema", exc_info=True)
-                self._signal_error()
-                callback(False)
-                return
-            else:
-                callback(e)
-        if self._connection:
-            self._refresh_schema_async_inner(new_callback, self._connection, force=force, **kwargs)
-        else:
-            callback(False)
-
-    def _refresh_schema_async_inner(self, callback, connection, preloaded_results=None, schema_agreement_wait=None, force=False, **kwargs):
-        if self._cluster.is_shutdown:
-            callback(False)
-            return
-        
-        def new_callback(e):
-            if not self._schema_meta_enabled and not force:
-                log.debug("[control connection] Skipping schema refresh because schema metadata is disabled")
-                callback(False)
-                return
-
-            if not e:
-                log.debug("Skipping schema refresh due to lack of schema agreement")
-                callback(False)
-                return
-            self._cluster.metadata.refresh(connection, self._timeout, fetch_size=self._schema_meta_page_size, **kwargs)
-        
-        self._wait_for_schema_agreement_async(new_callback,
-                                                connection=self._connection,
-                                                preloaded_results=preloaded_results,
-                                                wait_time=schema_agreement_wait)
-
-    # INTENDED ONLY FOR INTERNAL USE
-    def _wait_for_schema_agreement_async(self, callback, connection=None, preloaded_results=None, wait_time=None):
-        total_timeout = wait_time if wait_time is not None else self._cluster.max_schema_agreement_wait
-        if total_timeout <= 0:
-            callback(True)
-            return
-
-        # Each schema change typically generates two schema refreshes, one
-        # from the response type and one from the pushed notification. Holding
-        # a lock is just a simple way to cut down on the number of schema queries
-        # we'll make.
-        if not self._schema_agreement_lock.acquire(blocking=False):
-            self._cluster.scheduler.schedule_unique(0.2, self._wait_for_schema_agreement_async, callback, connection, preloaded_results, wait_time)
-            return
-        
-        try:
-            if self._is_shutdown:
-                self._schema_agreement_lock.release()
-                callback(None)
-                return
-
-            if not connection:
-                connection = self._connection
-
-            if preloaded_results:
-                log.debug("[control connection] Attempting to use preloaded results for schema agreement")
-
-                peers_result = preloaded_results[0]
-                local_result = preloaded_results[1]
-                schema_mismatches = self._get_schema_mismatches(peers_result, local_result, connection.endpoint)
-                if schema_mismatches is None:
-                    self._schema_agreement_lock.release()
-                    callback(True)
-                    return
-
-            log.debug("[control connection] Waiting for schema agreement")
-            start = self._time.time()
-            elapsed = 0
-            cl = ConsistencyLevel.ONE
-            schema_mismatches = None
-            select_peers_query = self._get_peers_query(self.PeersQueryType.PEERS_SCHEMA, connection)
-        except Exception as e:
-            self._schema_agreement_lock.release()
-            callback(e)
-            return
-
-        def inner(first_iter):
-            try:
-                elapsed = self._time.time() - start
-                if elapsed < total_timeout or first_iter:
-                    peers_query = QueryMessage(query=select_peers_query, consistency_level=cl)
-                    local_query = QueryMessage(query=self._SELECT_SCHEMA_LOCAL, consistency_level=cl)
-                    try:
-                        timeout = min(self._timeout, total_timeout - elapsed)
-                        peers_result, local_result = connection.wait_for_responses(
-                            peers_query, local_query, timeout=timeout)
-                    except OperationTimedOut as timeout:
-                        log.debug("[control connection] Timed out waiting for "
-                                    "response during schema agreement check: %s", timeout)
-                        self._cluster.scheduler.schedule_unique(0.2, inner, False)
-                        return
-                    except ConnectionShutdown as e:
-                        if self._is_shutdown:
-                            log.debug("[control connection] Aborting wait for schema match due to shutdown")
-                            self._schema_agreement_lock.release()
-                            callback(None)
-                            return
-                        else:
-                            raise
-
-                    schema_mismatches = self._get_schema_mismatches(peers_result, local_result, connection.endpoint)
-                    if schema_mismatches is None:
-                        self._schema_agreement_lock.release()
-                        callback(True)
-                        return
-
-                    log.debug("[control connection] Schemas mismatched, trying again")
-                    self._cluster.scheduler.schedule_unique(0.2, inner, False)
-                else:
-                    log.warning("Node %s is reporting a schema disagreement: %s",
-                                connection.endpoint, schema_mismatches)
-                    self._schema_agreement_lock.release()
-                    callback(False)
-            except Exception as e:
-                self._schema_agreement_lock.release()
-                callback(e)
-        inner(True)
 
     def refresh_node_list_and_token_map(self, force_token_rebuild=False):
         try:
             if self._connection:
                 self._refresh_node_list_and_token_map(self._connection, force_token_rebuild=force_token_rebuild)
                 return True
         except ReferenceError:
@@ -4167,15 +4035,15 @@
                 # this will be run by the scheduler
                 self._cluster.on_down(host, is_host_addition=False)
 
     def _handle_schema_change(self, event):
         if self._schema_event_refresh_window < 0:
             return
         delay = self._delay_for_event_type('schema_change', self._schema_event_refresh_window)
-        self._cluster.scheduler.schedule_unique(delay, self._refresh_schema_async, lambda *a, **k: None, **event)
+        self._cluster.scheduler.schedule_unique(delay, self.refresh_schema, **event)
 
     def wait_for_schema_agreement(self, connection=None, preloaded_results=None, wait_time=None):
 
         total_timeout = wait_time if wait_time is not None else self._cluster.max_schema_agreement_wait
         if total_timeout <= 0:
             return True
```

### Comparing `scylla-driver-3.26.0/cassandra/cmurmur3.c` & `scylla-driver-3.26.1/cassandra/cmurmur3.c`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/compat.py` & `scylla-driver-3.26.1/cassandra/compat.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/concurrent.py` & `scylla-driver-3.26.1/cassandra/concurrent.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/connection.py` & `scylla-driver-3.26.1/cassandra/connection.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/cqlengine/__init__.py` & `scylla-driver-3.26.1/cassandra/cqlengine/__init__.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/cqlengine/columns.py` & `scylla-driver-3.26.1/cassandra/cqlengine/columns.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/cqlengine/connection.py` & `scylla-driver-3.26.1/cassandra/cqlengine/connection.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/cqlengine/functions.py` & `scylla-driver-3.26.1/cassandra/cqlengine/functions.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/cqlengine/management.py` & `scylla-driver-3.26.1/cassandra/cqlengine/management.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/cqlengine/models.py` & `scylla-driver-3.26.1/cassandra/cqlengine/models.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/cqlengine/named.py` & `scylla-driver-3.26.1/cassandra/cqlengine/named.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/cqlengine/operators.py` & `scylla-driver-3.26.1/cassandra/cqlengine/operators.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/cqlengine/query.py` & `scylla-driver-3.26.1/cassandra/cqlengine/query.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/cqlengine/statements.py` & `scylla-driver-3.26.1/cassandra/cqlengine/statements.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/cqlengine/usertype.py` & `scylla-driver-3.26.1/cassandra/cqlengine/usertype.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/cqltypes.py` & `scylla-driver-3.26.1/cassandra/cqltypes.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/cython_marshal.pyx` & `scylla-driver-3.26.1/cassandra/cython_marshal.pyx`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/cython_utils.pyx` & `scylla-driver-3.26.1/cassandra/cython_utils.pyx`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/datastax/__init__.py` & `scylla-driver-3.26.1/cassandra/datastax/__init__.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/datastax/cloud/__init__.py` & `scylla-driver-3.26.1/cassandra/datastax/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/datastax/graph/__init__.py` & `scylla-driver-3.26.1/cassandra/datastax/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/datastax/graph/fluent/__init__.py` & `scylla-driver-3.26.1/cassandra/datastax/graph/fluent/__init__.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/datastax/graph/fluent/_predicates.py` & `scylla-driver-3.26.1/cassandra/datastax/graph/fluent/_predicates.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/datastax/graph/fluent/_query.py` & `scylla-driver-3.26.1/cassandra/datastax/graph/fluent/_query.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/datastax/graph/fluent/_serializers.py` & `scylla-driver-3.26.1/cassandra/datastax/graph/fluent/_serializers.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/datastax/graph/fluent/predicates.py` & `scylla-driver-3.26.1/cassandra/datastax/graph/fluent/predicates.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/datastax/graph/fluent/query.py` & `scylla-driver-3.26.1/cassandra/datastax/graph/fluent/query.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/datastax/graph/fluent/serializers.py` & `scylla-driver-3.26.1/cassandra/datastax/graph/fluent/serializers.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/datastax/graph/graphson.py` & `scylla-driver-3.26.1/cassandra/datastax/graph/graphson.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/datastax/graph/query.py` & `scylla-driver-3.26.1/cassandra/datastax/graph/query.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/datastax/graph/types.py` & `scylla-driver-3.26.1/cassandra/datastax/graph/types.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/datastax/insights/__init__.py` & `scylla-driver-3.26.1/cassandra/datastax/insights/__init__.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/datastax/insights/registry.py` & `scylla-driver-3.26.1/cassandra/datastax/insights/registry.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/datastax/insights/reporter.py` & `scylla-driver-3.26.1/cassandra/datastax/insights/reporter.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/datastax/insights/serializers.py` & `scylla-driver-3.26.1/cassandra/datastax/insights/serializers.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/datastax/insights/util.py` & `scylla-driver-3.26.1/cassandra/datastax/insights/util.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/deserializers.pxd` & `scylla-driver-3.26.1/cassandra/deserializers.pxd`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/deserializers.pyx` & `scylla-driver-3.26.1/cassandra/deserializers.pyx`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/encoder.py` & `scylla-driver-3.26.1/cassandra/encoder.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/graph/__init__.py` & `scylla-driver-3.26.1/cassandra/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/graph/graphson.py` & `scylla-driver-3.26.1/cassandra/graph/graphson.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/graph/query.py` & `scylla-driver-3.26.1/cassandra/graph/query.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/graph/types.py` & `scylla-driver-3.26.1/cassandra/graph/types.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/io/__init__.py` & `scylla-driver-3.26.1/cassandra/io/__init__.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/io/asyncioreactor.py` & `scylla-driver-3.26.1/cassandra/io/asyncioreactor.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/io/asyncorereactor.py` & `scylla-driver-3.26.1/cassandra/io/asyncorereactor.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/io/eventletreactor.py` & `scylla-driver-3.26.1/cassandra/io/eventletreactor.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/io/geventreactor.py` & `scylla-driver-3.26.1/cassandra/io/geventreactor.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/io/libevreactor.py` & `scylla-driver-3.26.1/cassandra/io/libevreactor.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/io/libevwrapper.c` & `scylla-driver-3.26.1/cassandra/io/libevwrapper.c`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/io/twistedreactor.py` & `scylla-driver-3.26.1/cassandra/io/twistedreactor.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/ioutils.pyx` & `scylla-driver-3.26.1/cassandra/ioutils.pyx`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/marshal.py` & `scylla-driver-3.26.1/cassandra/marshal.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/metadata.py` & `scylla-driver-3.26.1/cassandra/metadata.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/metrics.py` & `scylla-driver-3.26.1/cassandra/metrics.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/murmur3.py` & `scylla-driver-3.26.1/cassandra/murmur3.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/numpy_parser.pyx` & `scylla-driver-3.26.1/cassandra/numpy_parser.pyx`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/obj_parser.pyx` & `scylla-driver-3.26.1/cassandra/obj_parser.pyx`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/parsing.pxd` & `scylla-driver-3.26.1/cassandra/parsing.pxd`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/parsing.pyx` & `scylla-driver-3.26.1/cassandra/parsing.pyx`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/policies.py` & `scylla-driver-3.26.1/cassandra/policies.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/pool.py` & `scylla-driver-3.26.1/cassandra/pool.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/protocol.py` & `scylla-driver-3.26.1/cassandra/protocol.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/query.py` & `scylla-driver-3.26.1/cassandra/query.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/row_parser.pyx` & `scylla-driver-3.26.1/cassandra/row_parser.pyx`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/scylla/cloud.py` & `scylla-driver-3.26.1/cassandra/scylla/cloud.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/segment.py` & `scylla-driver-3.26.1/cassandra/segment.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/shard_info.py` & `scylla-driver-3.26.1/cassandra/shard_info.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/timestamps.py` & `scylla-driver-3.26.1/cassandra/timestamps.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/tuple.pxd` & `scylla-driver-3.26.1/cassandra/tuple.pxd`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/type_codes.pxd` & `scylla-driver-3.26.1/cassandra/type_codes.pxd`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/type_codes.py` & `scylla-driver-3.26.1/cassandra/type_codes.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/cassandra/util.py` & `scylla-driver-3.26.1/cassandra/util.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/ez_setup.py` & `scylla-driver-3.26.1/ez_setup.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/scylla_driver.egg-info/PKG-INFO` & `scylla-driver-3.26.1/scylla_driver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scylla-driver
-Version: 3.26.0
+Version: 3.26.1
 Summary: Scylla Driver for Apache Cassandra
 Home-page: https://github.com/scylladb/python-driver
 Author: ScyllaDB
 Project-URL: Documentation, https://scylladb.github.io/python-driver/
 Project-URL: Source, https://github.com/scylladb/python-driver/
 Project-URL: Issues, https://github.com/scylladb/python-driver/issues
 Keywords: cassandra,cql,orm,dse,graph
```

### Comparing `scylla-driver-3.26.0/scylla_driver.egg-info/SOURCES.txt` & `scylla-driver-3.26.1/scylla_driver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.26.0/setup.py` & `scylla-driver-3.26.1/setup.py`

 * *Files identical despite different names*

