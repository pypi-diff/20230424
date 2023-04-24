# Comparing `tmp/libsql-client-0.1.2.tar.gz` & `tmp/libsql-client-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libsql-client-0.1.2.tar", max compression
+gzip compressed data, was "libsql-client-0.2.0.tar", max compression
```

## Comparing `libsql-client-0.1.2.tar` & `libsql-client-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,18 @@
--rw-r--r--   0        0        0     1069 2023-02-07 08:09:33.087822 libsql-client-0.1.2/LICENSE.md
--rw-r--r--   0        0        0     1160 2023-02-08 11:02:52.084090 libsql-client-0.1.2/README.md
--rw-r--r--   0        0        0      145 2023-02-09 12:48:13.632958 libsql-client-0.1.2/libsql_client/__init__.py
--rw-r--r--   0        0        0     2824 2023-02-07 08:09:33.087822 libsql-client-0.1.2/libsql_client/client.py
--rw-r--r--   0        0        0      483 2023-02-07 08:09:33.087822 libsql-client-0.1.2/libsql_client/driver.py
--rw-r--r--   0        0        0      380 2023-02-09 12:48:13.632958 libsql-client-0.1.2/libsql_client/errors.py
--rw-r--r--   0        0        0     3252 2023-02-09 12:48:13.632958 libsql-client-0.1.2/libsql_client/http_driver.py
--rw-r--r--   0        0        0     1492 2023-02-07 08:09:33.087822 libsql-client-0.1.2/libsql_client/result.py
--rw-r--r--   0        0        0     2118 2023-02-07 08:09:33.087822 libsql-client-0.1.2/libsql_client/sqlite_driver.py
--rw-r--r--   0        0        0      667 2023-02-09 12:48:13.632958 libsql-client-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1841 1970-01-01 00:00:00.000000 libsql-client-0.1.2/setup.py
--rw-r--r--   0        0        0     1773 1970-01-01 00:00:00.000000 libsql-client-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-02-27 08:58:08.764134 libsql-client-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0     2907 2023-04-19 12:23:21.137820 libsql-client-0.2.0/README.md
+-rw-r--r--   0        0        0      268 2023-04-19 10:43:28.755257 libsql-client-0.2.0/libsql_client/__init__.py
+-rw-r--r--   0        0        0     3039 2023-04-17 12:00:30.657316 libsql-client-0.2.0/libsql_client/client.py
+-rw-r--r--   0        0        0      993 2023-04-17 12:00:30.657316 libsql-client-0.2.0/libsql_client/config.py
+-rw-r--r--   0        0        0      801 2023-04-17 12:00:30.657316 libsql-client-0.2.0/libsql_client/create_client.py
+-rw-r--r--   0        0        0       85 2023-04-17 12:00:30.657316 libsql-client-0.2.0/libsql_client/hrana/__init__.py
+-rw-r--r--   0        0        0    13911 2023-04-17 12:00:30.657316 libsql-client-0.2.0/libsql_client/hrana/client.py
+-rw-r--r--   0        0        0     4816 2023-04-20 09:18:36.654076 libsql-client-0.2.0/libsql_client/hrana/convert.py
+-rw-r--r--   0        0        0     1610 2023-04-17 12:00:30.661316 libsql-client-0.2.0/libsql_client/hrana/id_alloc.py
+-rw-r--r--   0        0        0     3974 2023-04-17 12:00:30.661316 libsql-client-0.2.0/libsql_client/hrana/proto.py
+-rw-r--r--   0        0        0     3441 2023-04-17 12:00:30.661316 libsql-client-0.2.0/libsql_client/http.py
+-rw-r--r--   0        0        0     3048 2023-04-20 09:22:06.451040 libsql-client-0.2.0/libsql_client/result.py
+-rw-r--r--   0        0        0     4896 2023-04-20 09:19:13.406247 libsql-client-0.2.0/libsql_client/sqlite3.py
+-rw-r--r--   0        0        0     6347 2023-04-19 11:59:20.956756 libsql-client-0.2.0/libsql_client/sync.py
+-rw-r--r--   0        0        0      933 2023-04-24 11:57:58.823118 libsql-client-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3690 1970-01-01 00:00:00.000000 libsql-client-0.2.0/setup.py
+-rw-r--r--   0        0        0     3706 1970-01-01 00:00:00.000000 libsql-client-0.2.0/PKG-INFO
```

### Comparing `libsql-client-0.1.2/LICENSE.md` & `libsql-client-0.2.0/LICENSE.md`

 * *Files identical despite different names*

