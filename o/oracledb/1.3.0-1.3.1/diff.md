# Comparing `tmp/oracledb-1.3.0.tar.gz` & `tmp/oracledb-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oracledb-1.3.0.tar", last modified: Thu Mar 30 22:59:12 2023, max compression
+gzip compressed data, was "oracledb-1.3.1.tar", last modified: Mon Apr 24 20:03:36 2023, max compression
```

## Comparing `oracledb-1.3.0.tar` & `oracledb-1.3.1.tar`

### file list

```diff
@@ -1,179 +1,179 @@
-drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-03-30 22:59:12.833833 oracledb-1.3.0/
--rw-r--r--   0 anthony   (1030) users      (100)    12570 2022-05-20 21:47:15.000000 oracledb-1.3.0/LICENSE.txt
--rw-r--r--   0 anthony   (1030) users      (100)      398 2022-05-20 21:47:15.000000 oracledb-1.3.0/MANIFEST.in
--rw-r--r--   0 anthony   (1030) users      (100)       56 2022-05-20 21:47:15.000000 oracledb-1.3.0/NOTICE.txt
--rw-rw-r--   0 anthony   (1030) users      (100)     5062 2023-03-30 22:59:12.833833 oracledb-1.3.0/PKG-INFO
--rw-r--r--   0 anthony   (1030) users      (100)      167 2022-05-20 21:47:15.000000 oracledb-1.3.0/README.txt
--rw-r--r--   0 anthony   (1030) users      (100)    28104 2022-05-20 21:47:15.000000 oracledb-1.3.0/THIRD_PARTY_LICENSES.txt
--rw-r--r--   0 anthony   (1030) users      (100)      110 2022-05-20 21:47:15.000000 oracledb-1.3.0/pyproject.toml
--rw-r--r--   0 anthony   (1030) users      (100)     1603 2023-03-30 22:59:12.833833 oracledb-1.3.0/setup.cfg
--rw-r--r--   0 anthony   (1030) users      (100)     3990 2022-08-27 22:13:47.000000 oracledb-1.3.0/setup.py
-drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-03-30 22:59:12.818833 oracledb-1.3.0/src/
-drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-03-30 22:59:12.822833 oracledb-1.3.0/src/oracledb/
--rw-rw-r--   0 anthony   (1030) users      (100)     5922 2023-03-27 21:56:43.000000 oracledb-1.3.0/src/oracledb/__init__.py
--rw-rw-r--   0 anthony   (1030) users      (100)    19013 2023-03-27 21:56:43.000000 oracledb-1.3.0/src/oracledb/aq.py
--rw-rw-r--   0 anthony   (1030) users      (100)    14703 2023-03-21 21:27:13.000000 oracledb-1.3.0/src/oracledb/base_impl.pxd
--rw-r--r--   0 anthony   (1030) users      (100)     5404 2022-08-27 17:10:23.000000 oracledb-1.3.0/src/oracledb/base_impl.pyx
--rw-rw-r--   0 anthony   (1030) users      (100)    31296 2023-03-27 21:31:03.000000 oracledb-1.3.0/src/oracledb/connect_params.py
--rw-rw-r--   0 anthony   (1030) users      (100)    49238 2023-03-27 21:57:19.000000 oracledb-1.3.0/src/oracledb/connection.py
--rw-r--r--   0 anthony   (1030) users      (100)     4070 2023-01-18 17:02:00.000000 oracledb-1.3.0/src/oracledb/constants.py
--rw-r--r--   0 anthony   (1030) users      (100)     2909 2022-05-20 21:47:15.000000 oracledb-1.3.0/src/oracledb/constructors.py
--rw-rw-r--   0 anthony   (1030) users      (100)    35219 2023-03-27 21:57:07.000000 oracledb-1.3.0/src/oracledb/cursor.py
--rw-rw-r--   0 anthony   (1030) users      (100)    11850 2023-03-27 21:56:43.000000 oracledb-1.3.0/src/oracledb/dbobject.py
--rw-r--r--   0 anthony   (1030) users      (100)     1827 2022-05-20 21:47:15.000000 oracledb-1.3.0/src/oracledb/defaults.py
--rw-r--r--   0 anthony   (1030) users      (100)     5403 2022-09-28 15:14:10.000000 oracledb-1.3.0/src/oracledb/driver_mode.py
--rw-r--r--   0 anthony   (1030) users      (100)     3130 2022-05-20 21:47:15.000000 oracledb-1.3.0/src/oracledb/dsn.py
--rw-rw-r--   0 anthony   (1030) users      (100)    21982 2023-03-29 03:54:03.000000 oracledb-1.3.0/src/oracledb/errors.py
--rw-r--r--   0 anthony   (1030) users      (100)     1811 2022-06-10 02:53:08.000000 oracledb-1.3.0/src/oracledb/exceptions.py
-drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-03-30 22:59:12.819833 oracledb-1.3.0/src/oracledb/impl/
-drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-03-30 22:59:12.823833 oracledb-1.3.0/src/oracledb/impl/base/
--rw-r--r--   0 anthony   (1030) users      (100)     7341 2022-05-20 21:47:15.000000 oracledb-1.3.0/src/oracledb/impl/base/bind_var.pyx
--rw-rw-r--   0 anthony   (1030) users      (100)    37428 2023-03-27 21:31:03.000000 oracledb-1.3.0/src/oracledb/impl/base/connect_params.pyx
--rw-r--r--   0 anthony   (1030) users      (100)    11765 2022-11-01 20:32:06.000000 oracledb-1.3.0/src/oracledb/impl/base/connection.pyx
--rw-r--r--   0 anthony   (1030) users      (100)    18951 2022-07-29 21:22:34.000000 oracledb-1.3.0/src/oracledb/impl/base/cursor.pyx
--rw-r--r--   0 anthony   (1030) users      (100)     4808 2022-11-01 20:32:06.000000 oracledb-1.3.0/src/oracledb/impl/base/dbobject.pyx
--rw-r--r--   0 anthony   (1030) users      (100)     2741 2022-05-20 21:47:15.000000 oracledb-1.3.0/src/oracledb/impl/base/lob.pyx
--rw-r--r--   0 anthony   (1030) users      (100)     4215 2022-05-20 21:47:15.000000 oracledb-1.3.0/src/oracledb/impl/base/pool.pyx
--rw-r--r--   0 anthony   (1030) users      (100)     4420 2022-08-02 17:00:32.000000 oracledb-1.3.0/src/oracledb/impl/base/pool_params.pyx
--rw-r--r--   0 anthony   (1030) users      (100)     6379 2022-08-27 21:55:16.000000 oracledb-1.3.0/src/oracledb/impl/base/queue.pyx
--rw-r--r--   0 anthony   (1030) users      (100)     4657 2022-05-20 21:47:15.000000 oracledb-1.3.0/src/oracledb/impl/base/soda.pyx
--rw-r--r--   0 anthony   (1030) users      (100)     1933 2022-05-20 21:47:15.000000 oracledb-1.3.0/src/oracledb/impl/base/subscr.pyx
--rw-rw-r--   0 anthony   (1030) users      (100)     8439 2023-03-21 21:27:13.000000 oracledb-1.3.0/src/oracledb/impl/base/types.pyx
--rw-r--r--   0 anthony   (1030) users      (100)     8646 2022-05-20 21:47:15.000000 oracledb-1.3.0/src/oracledb/impl/base/utils.pyx
--rw-r--r--   0 anthony   (1030) users      (100)    12993 2023-01-18 23:20:15.000000 oracledb-1.3.0/src/oracledb/impl/base/var.pyx
-drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-03-30 22:59:12.824833 oracledb-1.3.0/src/oracledb/impl/thick/
--rw-r--r--   0 anthony   (1030) users      (100)     2256 2022-05-20 21:47:15.000000 oracledb-1.3.0/src/oracledb/impl/thick/buffer.pyx
--rw-r--r--   0 anthony   (1030) users      (100)    25954 2022-11-07 17:33:47.000000 oracledb-1.3.0/src/oracledb/impl/thick/connection.pyx
--rw-r--r--   0 anthony   (1030) users      (100)    19732 2022-08-02 15:15:52.000000 oracledb-1.3.0/src/oracledb/impl/thick/cursor.pyx
--rw-r--r--   0 anthony   (1030) users      (100)    13927 2022-11-01 20:32:06.000000 oracledb-1.3.0/src/oracledb/impl/thick/dbobject.pyx
--rw-r--r--   0 anthony   (1030) users      (100)     9330 2022-05-20 21:47:15.000000 oracledb-1.3.0/src/oracledb/impl/thick/json.pyx
--rw-r--r--   0 anthony   (1030) users      (100)     7534 2022-05-20 21:47:15.000000 oracledb-1.3.0/src/oracledb/impl/thick/lob.pyx
-drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-03-30 22:59:12.819833 oracledb-1.3.0/src/oracledb/impl/thick/odpi/
-drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-03-30 22:59:12.824833 oracledb-1.3.0/src/oracledb/impl/thick/odpi/embed/
--rw-r--r--   0 anthony   (1030) users      (100)     2569 2022-05-20 22:11:04.000000 oracledb-1.3.0/src/oracledb/impl/thick/odpi/embed/dpi.c
-drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-03-30 22:59:12.825833 oracledb-1.3.0/src/oracledb/impl/thick/odpi/include/
--rw-rw-r--   0 anthony   (1030) users      (100)    82859 2023-03-30 22:40:58.000000 oracledb-1.3.0/src/oracledb/impl/thick/odpi/include/dpi.h
-drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-03-30 22:59:12.828833 oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/
--rw-rw-r--   0 anthony   (1030) users      (100)   113814 2023-03-30 22:40:58.000000 oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiConn.c
--rw-rw-r--   0 anthony   (1030) users      (100)    16638 2023-03-30 22:40:58.000000 oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiContext.c
--rw-r--r--   0 anthony   (1030) users      (100)    34806 2022-05-20 22:11:04.000000 oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiData.c
--rw-r--r--   0 anthony   (1030) users      (100)     7443 2022-05-20 22:11:04.000000 oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiDebug.c
--rw-r--r--   0 anthony   (1030) users      (100)    15574 2022-05-20 22:11:04.000000 oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiDeqOptions.c
--rw-r--r--   0 anthony   (1030) users      (100)     7552 2022-05-20 22:11:04.000000 oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiEnqOptions.c
--rw-r--r--   0 anthony   (1030) users      (100)     9569 2022-05-20 22:11:04.000000 oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiEnv.c
--rw-r--r--   0 anthony   (1030) users      (100)    12063 2022-05-20 22:11:04.000000 oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiError.c
--rw-rw-r--   0 anthony   (1030) users      (100)     9018 2023-03-30 22:40:58.000000 oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiErrorMessages.h
--rw-r--r--   0 anthony   (1030) users      (100)    13052 2022-05-20 22:11:04.000000 oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiGen.c
--rw-r--r--   0 anthony   (1030) users      (100)    15039 2022-11-07 17:19:09.000000 oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiGlobal.c
--rw-r--r--   0 anthony   (1030) users      (100)     5184 2022-05-20 22:11:04.000000 oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiHandleList.c
--rw-r--r--   0 anthony   (1030) users      (100)     5399 2022-05-20 22:11:04.000000 oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiHandlePool.c
--rw-rw-r--   0 anthony   (1030) users      (100)   107983 2023-03-30 22:40:58.000000 oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiImpl.h
--rw-rw-r--   0 anthony   (1030) users      (100)    35246 2023-03-30 22:40:58.000000 oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiJson.c
--rw-r--r--   0 anthony   (1030) users      (100)    19751 2022-05-20 22:11:04.000000 oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiLob.c
--rw-r--r--   0 anthony   (1030) users      (100)    23232 2022-08-27 21:56:08.000000 oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiMsgProps.c
--rw-r--r--   0 anthony   (1030) users      (100)    40061 2022-05-20 22:11:04.000000 oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiObject.c
--rw-r--r--   0 anthony   (1030) users      (100)     4894 2022-05-20 22:11:04.000000 oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiObjectAttr.c
--rw-rw-r--   0 anthony   (1030) users      (100)    14713 2023-03-30 22:40:58.000000 oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiObjectType.c
--rw-r--r--   0 anthony   (1030) users      (100)   179729 2022-05-20 22:11:04.000000 oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiOci.c
--rw-r--r--   0 anthony   (1030) users      (100)    26914 2022-11-01 20:30:53.000000 oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiOracleType.c
--rw-r--r--   0 anthony   (1030) users      (100)    32638 2022-08-02 17:00:34.000000 oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiPool.c
--rw-r--r--   0 anthony   (1030) users      (100)    23678 2022-08-27 21:56:08.000000 oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiQueue.c
--rw-r--r--   0 anthony   (1030) users      (100)     5712 2022-05-20 22:11:04.000000 oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiRowid.c
--rw-rw-r--   0 anthony   (1030) users      (100)    39581 2023-03-30 22:40:58.000000 oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiSodaColl.c
--rw-r--r--   0 anthony   (1030) users      (100)     6131 2022-05-20 22:11:04.000000 oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiSodaCollCursor.c
--rw-r--r--   0 anthony   (1030) users      (100)    17459 2022-05-20 22:11:04.000000 oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiSodaDb.c
--rw-r--r--   0 anthony   (1030) users      (100)     9371 2022-05-20 22:11:04.000000 oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiSodaDoc.c
--rw-r--r--   0 anthony   (1030) users      (100)     6134 2022-05-20 22:11:04.000000 oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiSodaDocCursor.c
--rw-r--r--   0 anthony   (1030) users      (100)    78753 2022-05-20 22:11:04.000000 oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiStmt.c
--rw-r--r--   0 anthony   (1030) users      (100)    29091 2022-05-20 22:11:04.000000 oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiSubscr.c
--rw-r--r--   0 anthony   (1030) users      (100)    23589 2022-11-01 20:30:53.000000 oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiUtils.c
--rw-r--r--   0 anthony   (1030) users      (100)    78379 2022-06-09 19:44:20.000000 oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiVar.c
--rw-r--r--   0 anthony   (1030) users      (100)    39137 2022-11-01 20:23:41.000000 oracledb-1.3.0/src/oracledb/impl/thick/odpi.pxd
--rw-r--r--   0 anthony   (1030) users      (100)    13694 2022-11-18 03:37:36.000000 oracledb-1.3.0/src/oracledb/impl/thick/pool.pyx
--rw-r--r--   0 anthony   (1030) users      (100)    21424 2022-10-18 22:30:30.000000 oracledb-1.3.0/src/oracledb/impl/thick/queue.pyx
--rw-r--r--   0 anthony   (1030) users      (100)    24041 2022-12-01 00:47:06.000000 oracledb-1.3.0/src/oracledb/impl/thick/soda.pyx
--rw-r--r--   0 anthony   (1030) users      (100)     7249 2022-12-01 00:47:47.000000 oracledb-1.3.0/src/oracledb/impl/thick/subscr.pyx
--rw-rw-r--   0 anthony   (1030) users      (100)    21952 2023-03-21 21:27:13.000000 oracledb-1.3.0/src/oracledb/impl/thick/utils.pyx
--rw-r--r--   0 anthony   (1030) users      (100)    11462 2022-11-01 20:34:31.000000 oracledb-1.3.0/src/oracledb/impl/thick/var.pyx
-drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-03-30 22:59:12.829833 oracledb-1.3.0/src/oracledb/impl/thin/
--rw-rw-r--   0 anthony   (1030) users      (100)    49673 2023-03-29 03:54:03.000000 oracledb-1.3.0/src/oracledb/impl/thin/buffer.pyx
--rw-rw-r--   0 anthony   (1030) users      (100)     5330 2023-03-27 21:55:41.000000 oracledb-1.3.0/src/oracledb/impl/thin/capabilities.pyx
--rw-rw-r--   0 anthony   (1030) users      (100)    16804 2023-03-27 21:46:22.000000 oracledb-1.3.0/src/oracledb/impl/thin/connection.pyx
--rw-rw-r--   0 anthony   (1030) users      (100)    23238 2023-03-29 03:54:03.000000 oracledb-1.3.0/src/oracledb/impl/thin/constants.pxi
--rw-r--r--   0 anthony   (1030) users      (100)     7681 2022-10-18 22:29:50.000000 oracledb-1.3.0/src/oracledb/impl/thin/conversions.pyx
--rw-r--r--   0 anthony   (1030) users      (100)     6194 2022-10-18 22:33:19.000000 oracledb-1.3.0/src/oracledb/impl/thin/crypto.pyx
--rw-rw-r--   0 anthony   (1030) users      (100)     8773 2023-03-21 23:24:10.000000 oracledb-1.3.0/src/oracledb/impl/thin/cursor.pyx
--rw-r--r--   0 anthony   (1030) users      (100)    23713 2022-05-20 21:47:15.000000 oracledb-1.3.0/src/oracledb/impl/thin/data_types.pyx
--rw-rw-r--   0 anthony   (1030) users      (100)    41584 2023-03-21 23:24:10.000000 oracledb-1.3.0/src/oracledb/impl/thin/dbobject.pyx
--rw-rw-r--   0 anthony   (1030) users      (100)     7553 2023-03-21 23:24:10.000000 oracledb-1.3.0/src/oracledb/impl/thin/lob.pyx
--rw-rw-r--   0 anthony   (1030) users      (100)    97981 2023-03-30 17:50:57.000000 oracledb-1.3.0/src/oracledb/impl/thin/messages.pyx
--rw-rw-r--   0 anthony   (1030) users      (100)    26238 2023-03-29 03:53:29.000000 oracledb-1.3.0/src/oracledb/impl/thin/oson.pyx
--rw-rw-r--   0 anthony   (1030) users      (100)    27772 2023-03-21 23:24:10.000000 oracledb-1.3.0/src/oracledb/impl/thin/packet.pyx
--rw-rw-r--   0 anthony   (1030) users      (100)    20664 2023-03-21 23:07:43.000000 oracledb-1.3.0/src/oracledb/impl/thin/pool.pyx
--rw-rw-r--   0 anthony   (1030) users      (100)    20265 2023-03-21 21:27:13.000000 oracledb-1.3.0/src/oracledb/impl/thin/protocol.pyx
--rw-rw-r--   0 anthony   (1030) users      (100)     9973 2023-03-29 03:49:45.000000 oracledb-1.3.0/src/oracledb/impl/thin/statement.pyx
--rw-r--r--   0 anthony   (1030) users      (100)     5869 2023-01-18 23:19:35.000000 oracledb-1.3.0/src/oracledb/impl/thin/utils.pyx
--rw-r--r--   0 anthony   (1030) users      (100)     5445 2022-10-18 22:29:50.000000 oracledb-1.3.0/src/oracledb/impl/thin/var.pyx
--rw-rw-r--   0 anthony   (1030) users      (100)     6078 2023-03-27 21:56:43.000000 oracledb-1.3.0/src/oracledb/lob.py
--rw-rw-r--   0 anthony   (1030) users      (100)    35074 2023-03-27 21:31:03.000000 oracledb-1.3.0/src/oracledb/pool.py
--rw-r--r--   0 anthony   (1030) users      (100)    31290 2022-09-28 15:08:47.000000 oracledb-1.3.0/src/oracledb/pool_params.py
--rw-r--r--   0 anthony   (1030) users      (100)        0 2022-05-20 21:47:15.000000 oracledb-1.3.0/src/oracledb/py.typed
--rw-rw-r--   0 anthony   (1030) users      (100)    27454 2023-03-27 21:56:43.000000 oracledb-1.3.0/src/oracledb/soda.py
--rw-r--r--   0 anthony   (1030) users      (100)    11078 2022-12-01 00:48:14.000000 oracledb-1.3.0/src/oracledb/subscr.py
--rw-r--r--   0 anthony   (1030) users      (100)     3130 2022-05-20 21:47:15.000000 oracledb-1.3.0/src/oracledb/thick_impl.pyx
--rw-rw-r--   0 anthony   (1030) users      (100)     3758 2023-03-21 23:24:10.000000 oracledb-1.3.0/src/oracledb/thin_impl.pyx
--rw-r--r--   0 anthony   (1030) users      (100)     3382 2022-05-20 21:47:15.000000 oracledb-1.3.0/src/oracledb/utils.py
--rw-rw-r--   0 anthony   (1030) users      (100)     6393 2023-03-27 21:56:43.000000 oracledb-1.3.0/src/oracledb/var.py
--rw-rw-r--   0 anthony   (1030) users      (100)     1533 2023-03-30 22:58:14.000000 oracledb-1.3.0/src/oracledb/version.py
-drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-03-30 22:59:12.822833 oracledb-1.3.0/src/oracledb.egg-info/
--rw-r--r--   0 anthony   (1030) users      (100)     5062 2023-03-30 22:59:12.000000 oracledb-1.3.0/src/oracledb.egg-info/PKG-INFO
--rw-r--r--   0 anthony   (1030) users      (100)     5443 2023-03-30 22:59:12.000000 oracledb-1.3.0/src/oracledb.egg-info/SOURCES.txt
--rw-r--r--   0 anthony   (1030) users      (100)        1 2023-03-30 22:59:12.000000 oracledb-1.3.0/src/oracledb.egg-info/dependency_links.txt
--rw-r--r--   0 anthony   (1030) users      (100)        1 2023-01-19 17:26:29.000000 oracledb-1.3.0/src/oracledb.egg-info/not-zip-safe
--rw-r--r--   0 anthony   (1030) users      (100)       20 2023-03-30 22:59:12.000000 oracledb-1.3.0/src/oracledb.egg-info/requires.txt
--rw-r--r--   0 anthony   (1030) users      (100)        9 2023-03-30 22:59:12.000000 oracledb-1.3.0/src/oracledb.egg-info/top_level.txt
-drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-03-30 22:59:12.833833 oracledb-1.3.0/tests/
--rw-r--r--   0 anthony   (1030) users      (100)     2205 2022-11-10 17:47:01.000000 oracledb-1.3.0/tests/create_schema.py
--rw-r--r--   0 anthony   (1030) users      (100)     1928 2022-05-20 21:47:15.000000 oracledb-1.3.0/tests/drop_schema.py
--rw-r--r--   0 anthony   (1030) users      (100)     7093 2022-05-20 21:47:15.000000 oracledb-1.3.0/tests/test_1000_module.py
--rw-rw-r--   0 anthony   (1030) users      (100)    25465 2023-03-27 21:31:03.000000 oracledb-1.3.0/tests/test_1100_connection.py
--rw-r--r--   0 anthony   (1030) users      (100)    13329 2022-11-01 20:34:31.000000 oracledb-1.3.0/tests/test_1300_cursor_var.py
--rw-r--r--   0 anthony   (1030) users      (100)    11560 2022-05-20 21:47:15.000000 oracledb-1.3.0/tests/test_1400_datetime_var.py
--rw-rw-r--   0 anthony   (1030) users      (100)     9367 2023-03-21 21:27:13.000000 oracledb-1.3.0/tests/test_1500_types.py
--rw-rw-r--   0 anthony   (1030) users      (100)    19283 2023-03-29 03:49:45.000000 oracledb-1.3.0/tests/test_1600_dml_returning.py
--rw-r--r--   0 anthony   (1030) users      (100)     3768 2022-05-20 21:47:15.000000 oracledb-1.3.0/tests/test_1700_error.py
--rw-r--r--   0 anthony   (1030) users      (100)     8251 2022-05-20 21:47:15.000000 oracledb-1.3.0/tests/test_1800_interval_var.py
--rw-r--r--   0 anthony   (1030) users      (100)    20023 2022-08-02 17:00:32.000000 oracledb-1.3.0/tests/test_1900_lob_var.py
--rw-r--r--   0 anthony   (1030) users      (100)     5306 2022-05-20 21:47:15.000000 oracledb-1.3.0/tests/test_2000_long_var.py
--rw-r--r--   0 anthony   (1030) users      (100)    11357 2022-05-20 21:47:15.000000 oracledb-1.3.0/tests/test_2100_nchar_var.py
--rw-r--r--   0 anthony   (1030) users      (100)    21431 2022-11-01 21:30:49.000000 oracledb-1.3.0/tests/test_2200_number_var.py
--rw-rw-r--   0 anthony   (1030) users      (100)    25954 2023-03-21 21:27:13.000000 oracledb-1.3.0/tests/test_2300_object_var.py
--rw-rw-r--   0 anthony   (1030) users      (100)    35040 2023-03-21 21:27:13.000000 oracledb-1.3.0/tests/test_2400_pool.py
--rw-r--r--   0 anthony   (1030) users      (100)    21339 2022-11-07 17:27:30.000000 oracledb-1.3.0/tests/test_2500_string_var.py
--rw-r--r--   0 anthony   (1030) users      (100)     7896 2022-05-20 21:47:15.000000 oracledb-1.3.0/tests/test_2600_timestamp_var.py
--rw-rw-r--   0 anthony   (1030) users      (100)    24023 2023-03-27 21:30:23.000000 oracledb-1.3.0/tests/test_2700_aq.py
--rw-r--r--   0 anthony   (1030) users      (100)     7672 2022-08-27 21:55:16.000000 oracledb-1.3.0/tests/test_2800_bulk_aq.py
--rw-r--r--   0 anthony   (1030) users      (100)     7813 2022-10-18 22:31:58.000000 oracledb-1.3.0/tests/test_2900_rowid.py
--rw-r--r--   0 anthony   (1030) users      (100)     7971 2022-05-20 21:47:15.000000 oracledb-1.3.0/tests/test_3000_subscription.py
--rw-r--r--   0 anthony   (1030) users      (100)     3943 2023-01-18 17:02:49.000000 oracledb-1.3.0/tests/test_3100_boolean_var.py
--rw-rw-r--   0 anthony   (1030) users      (100)    24868 2023-03-21 21:27:13.000000 oracledb-1.3.0/tests/test_3200_features_12_1.py
--rw-r--r--   0 anthony   (1030) users      (100)     5670 2022-05-20 21:47:15.000000 oracledb-1.3.0/tests/test_3300_soda_database.py
--rw-r--r--   0 anthony   (1030) users      (100)    21475 2022-09-29 00:05:59.000000 oracledb-1.3.0/tests/test_3400_soda_collection.py
--rw-rw-r--   0 anthony   (1030) users      (100)    10520 2023-03-21 23:24:10.000000 oracledb-1.3.0/tests/test_3500_json.py
--rw-rw-r--   0 anthony   (1030) users      (100)    25036 2023-03-21 21:27:13.000000 oracledb-1.3.0/tests/test_3600_outputtypehandler.py
--rw-rw-r--   0 anthony   (1030) users      (100)    20995 2023-03-21 23:24:10.000000 oracledb-1.3.0/tests/test_3700_var.py
--rw-r--r--   0 anthony   (1030) users      (100)    10197 2022-05-20 21:47:15.000000 oracledb-1.3.0/tests/test_3800_typehandler.py
--rw-r--r--   0 anthony   (1030) users      (100)    16426 2022-05-20 21:47:15.000000 oracledb-1.3.0/tests/test_3900_cursor_execute.py
--rw-r--r--   0 anthony   (1030) users      (100)    13808 2022-07-29 21:22:34.000000 oracledb-1.3.0/tests/test_4000_cursor_executemany.py
--rw-r--r--   0 anthony   (1030) users      (100)     6304 2022-05-20 21:47:15.000000 oracledb-1.3.0/tests/test_4100_cursor_callproc.py
--rw-r--r--   0 anthony   (1030) users      (100)    10122 2022-05-20 21:47:15.000000 oracledb-1.3.0/tests/test_4200_cursor_scrollable.py
--rw-rw-r--   0 anthony   (1030) users      (100)    40520 2023-03-21 23:25:18.000000 oracledb-1.3.0/tests/test_4300_cursor_other.py
--rw-r--r--   0 anthony   (1030) users      (100)     5200 2022-11-07 16:22:37.000000 oracledb-1.3.0/tests/test_4400_tpc.py
--rw-rw-r--   0 anthony   (1030) users      (100)    30813 2023-03-27 21:31:03.000000 oracledb-1.3.0/tests/test_4500_connect_params.py
--rw-r--r--   0 anthony   (1030) users      (100)     9049 2022-05-20 21:47:15.000000 oracledb-1.3.0/tests/test_4600_type_changes.py
--rw-r--r--   0 anthony   (1030) users      (100)     2746 2022-08-27 17:02:29.000000 oracledb-1.3.0/tests/test_4700_pool_params.py
--rw-r--r--   0 anthony   (1030) users      (100)     7681 2022-06-06 16:50:09.000000 oracledb-1.3.0/tests/test_4800_timestamp_ltz_var.py
--rw-r--r--   0 anthony   (1030) users      (100)     7315 2022-06-10 16:31:07.000000 oracledb-1.3.0/tests/test_4900_timestamp_tz_var.py
--rw-r--r--   0 anthony   (1030) users      (100)    11969 2022-08-02 17:00:32.000000 oracledb-1.3.0/tests/test_5000_externalauth.py
--rw-r--r--   0 anthony   (1030) users      (100)    15451 2022-11-10 17:47:01.000000 oracledb-1.3.0/tests/test_env.py
--rw-r--r--   0 anthony   (1030) users      (100)      593 2022-12-01 16:31:07.000000 oracledb-1.3.0/tox.ini
+drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-04-24 20:03:36.231150 oracledb-1.3.1/
+-rw-rw-r--   0 anthony   (1030) users      (100)    12570 2023-04-21 18:03:32.000000 oracledb-1.3.1/LICENSE.txt
+-rw-r--r--   0 anthony   (1030) users      (100)      398 2022-05-20 21:47:15.000000 oracledb-1.3.1/MANIFEST.in
+-rw-r--r--   0 anthony   (1030) users      (100)       56 2022-05-20 21:47:15.000000 oracledb-1.3.1/NOTICE.txt
+-rw-rw-r--   0 anthony   (1030) users      (100)     5062 2023-04-24 20:03:36.231150 oracledb-1.3.1/PKG-INFO
+-rw-r--r--   0 anthony   (1030) users      (100)      167 2022-05-20 21:47:15.000000 oracledb-1.3.1/README.txt
+-rw-r--r--   0 anthony   (1030) users      (100)    28104 2022-05-20 21:47:15.000000 oracledb-1.3.1/THIRD_PARTY_LICENSES.txt
+-rw-r--r--   0 anthony   (1030) users      (100)      110 2022-05-20 21:47:15.000000 oracledb-1.3.1/pyproject.toml
+-rw-r--r--   0 anthony   (1030) users      (100)     1603 2023-04-24 20:03:36.231150 oracledb-1.3.1/setup.cfg
+-rw-r--r--   0 anthony   (1030) users      (100)     3990 2022-08-27 22:13:47.000000 oracledb-1.3.1/setup.py
+drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-04-24 20:03:36.216151 oracledb-1.3.1/src/
+drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-04-24 20:03:36.220151 oracledb-1.3.1/src/oracledb/
+-rw-rw-r--   0 anthony   (1030) users      (100)     5922 2023-03-27 21:56:43.000000 oracledb-1.3.1/src/oracledb/__init__.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    19013 2023-03-27 21:56:43.000000 oracledb-1.3.1/src/oracledb/aq.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    14703 2023-03-21 21:27:13.000000 oracledb-1.3.1/src/oracledb/base_impl.pxd
+-rw-r--r--   0 anthony   (1030) users      (100)     5404 2022-08-27 17:10:23.000000 oracledb-1.3.1/src/oracledb/base_impl.pyx
+-rw-rw-r--   0 anthony   (1030) users      (100)    31296 2023-03-27 21:31:03.000000 oracledb-1.3.1/src/oracledb/connect_params.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    49238 2023-03-27 21:57:19.000000 oracledb-1.3.1/src/oracledb/connection.py
+-rw-r--r--   0 anthony   (1030) users      (100)     4070 2023-01-18 17:02:00.000000 oracledb-1.3.1/src/oracledb/constants.py
+-rw-r--r--   0 anthony   (1030) users      (100)     2909 2022-05-20 21:47:15.000000 oracledb-1.3.1/src/oracledb/constructors.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    35219 2023-03-27 21:57:07.000000 oracledb-1.3.1/src/oracledb/cursor.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    11850 2023-03-27 21:56:43.000000 oracledb-1.3.1/src/oracledb/dbobject.py
+-rw-r--r--   0 anthony   (1030) users      (100)     1827 2022-05-20 21:47:15.000000 oracledb-1.3.1/src/oracledb/defaults.py
+-rw-r--r--   0 anthony   (1030) users      (100)     5403 2022-09-28 15:14:10.000000 oracledb-1.3.1/src/oracledb/driver_mode.py
+-rw-r--r--   0 anthony   (1030) users      (100)     3130 2022-05-20 21:47:15.000000 oracledb-1.3.1/src/oracledb/dsn.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    21982 2023-03-29 03:54:03.000000 oracledb-1.3.1/src/oracledb/errors.py
+-rw-r--r--   0 anthony   (1030) users      (100)     1811 2022-06-10 02:53:08.000000 oracledb-1.3.1/src/oracledb/exceptions.py
+drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-04-24 20:03:36.217151 oracledb-1.3.1/src/oracledb/impl/
+drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-04-24 20:03:36.222151 oracledb-1.3.1/src/oracledb/impl/base/
+-rw-r--r--   0 anthony   (1030) users      (100)     7341 2022-05-20 21:47:15.000000 oracledb-1.3.1/src/oracledb/impl/base/bind_var.pyx
+-rw-rw-r--   0 anthony   (1030) users      (100)    37428 2023-03-27 21:31:03.000000 oracledb-1.3.1/src/oracledb/impl/base/connect_params.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)    11765 2022-11-01 20:32:06.000000 oracledb-1.3.1/src/oracledb/impl/base/connection.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)    18951 2022-07-29 21:22:34.000000 oracledb-1.3.1/src/oracledb/impl/base/cursor.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)     4808 2022-11-01 20:32:06.000000 oracledb-1.3.1/src/oracledb/impl/base/dbobject.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)     2741 2022-05-20 21:47:15.000000 oracledb-1.3.1/src/oracledb/impl/base/lob.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)     4215 2022-05-20 21:47:15.000000 oracledb-1.3.1/src/oracledb/impl/base/pool.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)     4420 2022-08-02 17:00:32.000000 oracledb-1.3.1/src/oracledb/impl/base/pool_params.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)     6379 2022-08-27 21:55:16.000000 oracledb-1.3.1/src/oracledb/impl/base/queue.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)     4657 2022-05-20 21:47:15.000000 oracledb-1.3.1/src/oracledb/impl/base/soda.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)     1933 2022-05-20 21:47:15.000000 oracledb-1.3.1/src/oracledb/impl/base/subscr.pyx
+-rw-rw-r--   0 anthony   (1030) users      (100)     8439 2023-03-21 21:27:13.000000 oracledb-1.3.1/src/oracledb/impl/base/types.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)     8646 2022-05-20 21:47:15.000000 oracledb-1.3.1/src/oracledb/impl/base/utils.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)    12993 2023-01-18 23:20:15.000000 oracledb-1.3.1/src/oracledb/impl/base/var.pyx
+drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-04-24 20:03:36.223151 oracledb-1.3.1/src/oracledb/impl/thick/
+-rw-r--r--   0 anthony   (1030) users      (100)     2256 2022-05-20 21:47:15.000000 oracledb-1.3.1/src/oracledb/impl/thick/buffer.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)    25954 2022-11-07 17:33:47.000000 oracledb-1.3.1/src/oracledb/impl/thick/connection.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)    19732 2022-08-02 15:15:52.000000 oracledb-1.3.1/src/oracledb/impl/thick/cursor.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)    13927 2022-11-01 20:32:06.000000 oracledb-1.3.1/src/oracledb/impl/thick/dbobject.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)     9330 2022-05-20 21:47:15.000000 oracledb-1.3.1/src/oracledb/impl/thick/json.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)     7534 2022-05-20 21:47:15.000000 oracledb-1.3.1/src/oracledb/impl/thick/lob.pyx
+drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-04-24 20:03:36.217151 oracledb-1.3.1/src/oracledb/impl/thick/odpi/
+drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-04-24 20:03:36.223151 oracledb-1.3.1/src/oracledb/impl/thick/odpi/embed/
+-rw-r--r--   0 anthony   (1030) users      (100)     2569 2022-05-20 22:11:04.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/embed/dpi.c
+drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-04-24 20:03:36.223151 oracledb-1.3.1/src/oracledb/impl/thick/odpi/include/
+-rw-rw-r--   0 anthony   (1030) users      (100)    82859 2023-03-30 22:40:58.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/include/dpi.h
+drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-04-24 20:03:36.226151 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/
+-rw-rw-r--   0 anthony   (1030) users      (100)   113814 2023-03-30 22:40:58.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiConn.c
+-rw-rw-r--   0 anthony   (1030) users      (100)    16638 2023-03-30 22:40:58.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiContext.c
+-rw-r--r--   0 anthony   (1030) users      (100)    34806 2022-05-20 22:11:04.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiData.c
+-rw-r--r--   0 anthony   (1030) users      (100)     7443 2022-05-20 22:11:04.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiDebug.c
+-rw-r--r--   0 anthony   (1030) users      (100)    15574 2022-05-20 22:11:04.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiDeqOptions.c
+-rw-r--r--   0 anthony   (1030) users      (100)     7552 2022-05-20 22:11:04.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiEnqOptions.c
+-rw-r--r--   0 anthony   (1030) users      (100)     9569 2022-05-20 22:11:04.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiEnv.c
+-rw-r--r--   0 anthony   (1030) users      (100)    12063 2022-05-20 22:11:04.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiError.c
+-rw-rw-r--   0 anthony   (1030) users      (100)     9018 2023-03-30 22:40:58.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiErrorMessages.h
+-rw-r--r--   0 anthony   (1030) users      (100)    13052 2022-05-20 22:11:04.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiGen.c
+-rw-r--r--   0 anthony   (1030) users      (100)    15039 2022-11-07 17:19:09.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiGlobal.c
+-rw-r--r--   0 anthony   (1030) users      (100)     5184 2022-05-20 22:11:04.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiHandleList.c
+-rw-r--r--   0 anthony   (1030) users      (100)     5399 2022-05-20 22:11:04.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiHandlePool.c
+-rw-rw-r--   0 anthony   (1030) users      (100)   107983 2023-03-30 22:40:58.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiImpl.h
+-rw-rw-r--   0 anthony   (1030) users      (100)    35246 2023-03-30 22:40:58.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiJson.c
+-rw-r--r--   0 anthony   (1030) users      (100)    19751 2022-05-20 22:11:04.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiLob.c
+-rw-r--r--   0 anthony   (1030) users      (100)    23232 2022-08-27 21:56:08.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiMsgProps.c
+-rw-r--r--   0 anthony   (1030) users      (100)    40061 2022-05-20 22:11:04.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiObject.c
+-rw-r--r--   0 anthony   (1030) users      (100)     4894 2022-05-20 22:11:04.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiObjectAttr.c
+-rw-rw-r--   0 anthony   (1030) users      (100)    14713 2023-03-30 22:40:58.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiObjectType.c
+-rw-r--r--   0 anthony   (1030) users      (100)   179729 2022-05-20 22:11:04.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiOci.c
+-rw-r--r--   0 anthony   (1030) users      (100)    26914 2022-11-01 20:30:53.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiOracleType.c
+-rw-r--r--   0 anthony   (1030) users      (100)    32638 2022-08-02 17:00:34.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiPool.c
+-rw-r--r--   0 anthony   (1030) users      (100)    23678 2022-08-27 21:56:08.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiQueue.c
+-rw-r--r--   0 anthony   (1030) users      (100)     5712 2022-05-20 22:11:04.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiRowid.c
+-rw-rw-r--   0 anthony   (1030) users      (100)    39581 2023-03-30 22:40:58.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiSodaColl.c
+-rw-r--r--   0 anthony   (1030) users      (100)     6131 2022-05-20 22:11:04.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiSodaCollCursor.c
+-rw-r--r--   0 anthony   (1030) users      (100)    17459 2022-05-20 22:11:04.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiSodaDb.c
+-rw-r--r--   0 anthony   (1030) users      (100)     9371 2022-05-20 22:11:04.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiSodaDoc.c
+-rw-r--r--   0 anthony   (1030) users      (100)     6134 2022-05-20 22:11:04.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiSodaDocCursor.c
+-rw-r--r--   0 anthony   (1030) users      (100)    78753 2022-05-20 22:11:04.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiStmt.c
+-rw-r--r--   0 anthony   (1030) users      (100)    29091 2022-05-20 22:11:04.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiSubscr.c
+-rw-r--r--   0 anthony   (1030) users      (100)    23589 2022-11-01 20:30:53.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiUtils.c
+-rw-r--r--   0 anthony   (1030) users      (100)    78379 2022-06-09 19:44:20.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiVar.c
+-rw-r--r--   0 anthony   (1030) users      (100)    39137 2022-11-01 20:23:41.000000 oracledb-1.3.1/src/oracledb/impl/thick/odpi.pxd
+-rw-r--r--   0 anthony   (1030) users      (100)    13694 2022-11-18 03:37:36.000000 oracledb-1.3.1/src/oracledb/impl/thick/pool.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)    21424 2022-10-18 22:30:30.000000 oracledb-1.3.1/src/oracledb/impl/thick/queue.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)    24041 2022-12-01 00:47:06.000000 oracledb-1.3.1/src/oracledb/impl/thick/soda.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)     7249 2022-12-01 00:47:47.000000 oracledb-1.3.1/src/oracledb/impl/thick/subscr.pyx
+-rw-rw-r--   0 anthony   (1030) users      (100)    21952 2023-03-21 21:27:13.000000 oracledb-1.3.1/src/oracledb/impl/thick/utils.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)    11462 2022-11-01 20:34:31.000000 oracledb-1.3.1/src/oracledb/impl/thick/var.pyx
+drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-04-24 20:03:36.228150 oracledb-1.3.1/src/oracledb/impl/thin/
+-rw-rw-r--   0 anthony   (1030) users      (100)    49673 2023-03-29 03:54:03.000000 oracledb-1.3.1/src/oracledb/impl/thin/buffer.pyx
+-rw-rw-r--   0 anthony   (1030) users      (100)     5330 2023-03-27 21:55:41.000000 oracledb-1.3.1/src/oracledb/impl/thin/capabilities.pyx
+-rw-rw-r--   0 anthony   (1030) users      (100)    16804 2023-03-27 21:46:22.000000 oracledb-1.3.1/src/oracledb/impl/thin/connection.pyx
+-rw-rw-r--   0 anthony   (1030) users      (100)    23238 2023-03-29 03:54:03.000000 oracledb-1.3.1/src/oracledb/impl/thin/constants.pxi
+-rw-r--r--   0 anthony   (1030) users      (100)     7681 2022-10-18 22:29:50.000000 oracledb-1.3.1/src/oracledb/impl/thin/conversions.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)     6194 2022-10-18 22:33:19.000000 oracledb-1.3.1/src/oracledb/impl/thin/crypto.pyx
+-rw-rw-r--   0 anthony   (1030) users      (100)     8773 2023-04-21 18:03:32.000000 oracledb-1.3.1/src/oracledb/impl/thin/cursor.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)    23713 2022-05-20 21:47:15.000000 oracledb-1.3.1/src/oracledb/impl/thin/data_types.pyx
+-rw-rw-r--   0 anthony   (1030) users      (100)    41584 2023-03-21 23:24:10.000000 oracledb-1.3.1/src/oracledb/impl/thin/dbobject.pyx
+-rw-rw-r--   0 anthony   (1030) users      (100)     7553 2023-03-21 23:24:10.000000 oracledb-1.3.1/src/oracledb/impl/thin/lob.pyx
+-rw-rw-r--   0 anthony   (1030) users      (100)    98072 2023-04-21 18:03:32.000000 oracledb-1.3.1/src/oracledb/impl/thin/messages.pyx
+-rw-rw-r--   0 anthony   (1030) users      (100)    26238 2023-03-29 03:53:29.000000 oracledb-1.3.1/src/oracledb/impl/thin/oson.pyx
+-rw-rw-r--   0 anthony   (1030) users      (100)    27772 2023-03-21 23:24:10.000000 oracledb-1.3.1/src/oracledb/impl/thin/packet.pyx
+-rw-rw-r--   0 anthony   (1030) users      (100)    20678 2023-04-21 18:03:32.000000 oracledb-1.3.1/src/oracledb/impl/thin/pool.pyx
+-rw-rw-r--   0 anthony   (1030) users      (100)    20265 2023-03-21 21:27:13.000000 oracledb-1.3.1/src/oracledb/impl/thin/protocol.pyx
+-rw-rw-r--   0 anthony   (1030) users      (100)    10891 2023-04-21 18:03:32.000000 oracledb-1.3.1/src/oracledb/impl/thin/statement.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)     5869 2023-01-18 23:19:35.000000 oracledb-1.3.1/src/oracledb/impl/thin/utils.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)     5445 2022-10-18 22:29:50.000000 oracledb-1.3.1/src/oracledb/impl/thin/var.pyx
+-rw-rw-r--   0 anthony   (1030) users      (100)     6078 2023-03-27 21:56:43.000000 oracledb-1.3.1/src/oracledb/lob.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    35074 2023-03-27 21:31:03.000000 oracledb-1.3.1/src/oracledb/pool.py
+-rw-r--r--   0 anthony   (1030) users      (100)    31290 2022-09-28 15:08:47.000000 oracledb-1.3.1/src/oracledb/pool_params.py
+-rw-r--r--   0 anthony   (1030) users      (100)        0 2022-05-20 21:47:15.000000 oracledb-1.3.1/src/oracledb/py.typed
+-rw-rw-r--   0 anthony   (1030) users      (100)    27454 2023-03-27 21:56:43.000000 oracledb-1.3.1/src/oracledb/soda.py
+-rw-r--r--   0 anthony   (1030) users      (100)    11078 2022-12-01 00:48:14.000000 oracledb-1.3.1/src/oracledb/subscr.py
+-rw-r--r--   0 anthony   (1030) users      (100)     3130 2022-05-20 21:47:15.000000 oracledb-1.3.1/src/oracledb/thick_impl.pyx
+-rw-rw-r--   0 anthony   (1030) users      (100)     3758 2023-03-21 23:24:10.000000 oracledb-1.3.1/src/oracledb/thin_impl.pyx
+-rw-r--r--   0 anthony   (1030) users      (100)     3382 2022-05-20 21:47:15.000000 oracledb-1.3.1/src/oracledb/utils.py
+-rw-rw-r--   0 anthony   (1030) users      (100)     6393 2023-03-27 21:56:43.000000 oracledb-1.3.1/src/oracledb/var.py
+-rw-rw-r--   0 anthony   (1030) users      (100)     1533 2023-04-21 18:03:32.000000 oracledb-1.3.1/src/oracledb/version.py
+drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-04-24 20:03:36.220151 oracledb-1.3.1/src/oracledb.egg-info/
+-rw-r--r--   0 anthony   (1030) users      (100)     5062 2023-04-24 20:03:36.000000 oracledb-1.3.1/src/oracledb.egg-info/PKG-INFO
+-rw-r--r--   0 anthony   (1030) users      (100)     5443 2023-04-24 20:03:36.000000 oracledb-1.3.1/src/oracledb.egg-info/SOURCES.txt
+-rw-r--r--   0 anthony   (1030) users      (100)        1 2023-04-24 20:03:36.000000 oracledb-1.3.1/src/oracledb.egg-info/dependency_links.txt
+-rw-r--r--   0 anthony   (1030) users      (100)        1 2023-01-19 17:26:29.000000 oracledb-1.3.1/src/oracledb.egg-info/not-zip-safe
+-rw-r--r--   0 anthony   (1030) users      (100)       20 2023-04-24 20:03:36.000000 oracledb-1.3.1/src/oracledb.egg-info/requires.txt
+-rw-r--r--   0 anthony   (1030) users      (100)        9 2023-04-24 20:03:36.000000 oracledb-1.3.1/src/oracledb.egg-info/top_level.txt
+drwxrwxr-x   0 anthony   (1030) users      (100)        0 2023-04-24 20:03:36.231150 oracledb-1.3.1/tests/
+-rw-rw-r--   0 anthony   (1030) users      (100)     2368 2023-04-21 18:03:32.000000 oracledb-1.3.1/tests/create_schema.py
+-rw-r--r--   0 anthony   (1030) users      (100)     1928 2022-05-20 21:47:15.000000 oracledb-1.3.1/tests/drop_schema.py
+-rw-r--r--   0 anthony   (1030) users      (100)     7093 2022-05-20 21:47:15.000000 oracledb-1.3.1/tests/test_1000_module.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    25407 2023-04-21 18:03:32.000000 oracledb-1.3.1/tests/test_1100_connection.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    13372 2023-04-21 18:03:32.000000 oracledb-1.3.1/tests/test_1300_cursor_var.py
+-rw-r--r--   0 anthony   (1030) users      (100)    11560 2022-05-20 21:47:15.000000 oracledb-1.3.1/tests/test_1400_datetime_var.py
+-rw-rw-r--   0 anthony   (1030) users      (100)     9367 2023-03-21 21:27:13.000000 oracledb-1.3.1/tests/test_1500_types.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    19283 2023-03-29 03:49:45.000000 oracledb-1.3.1/tests/test_1600_dml_returning.py
+-rw-rw-r--   0 anthony   (1030) users      (100)     3785 2023-04-21 18:03:32.000000 oracledb-1.3.1/tests/test_1700_error.py
+-rw-r--r--   0 anthony   (1030) users      (100)     8251 2022-05-20 21:47:15.000000 oracledb-1.3.1/tests/test_1800_interval_var.py
+-rw-r--r--   0 anthony   (1030) users      (100)    20023 2022-08-02 17:00:32.000000 oracledb-1.3.1/tests/test_1900_lob_var.py
+-rw-r--r--   0 anthony   (1030) users      (100)     5306 2022-05-20 21:47:15.000000 oracledb-1.3.1/tests/test_2000_long_var.py
+-rw-r--r--   0 anthony   (1030) users      (100)    11357 2022-05-20 21:47:15.000000 oracledb-1.3.1/tests/test_2100_nchar_var.py
+-rw-r--r--   0 anthony   (1030) users      (100)    21431 2022-11-01 21:30:49.000000 oracledb-1.3.1/tests/test_2200_number_var.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    25820 2023-04-21 18:03:32.000000 oracledb-1.3.1/tests/test_2300_object_var.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    35040 2023-03-21 21:27:13.000000 oracledb-1.3.1/tests/test_2400_pool.py
+-rw-r--r--   0 anthony   (1030) users      (100)    21339 2022-11-07 17:27:30.000000 oracledb-1.3.1/tests/test_2500_string_var.py
+-rw-r--r--   0 anthony   (1030) users      (100)     7896 2022-05-20 21:47:15.000000 oracledb-1.3.1/tests/test_2600_timestamp_var.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    23955 2023-04-21 18:03:32.000000 oracledb-1.3.1/tests/test_2700_aq.py
+-rw-r--r--   0 anthony   (1030) users      (100)     7672 2022-08-27 21:55:16.000000 oracledb-1.3.1/tests/test_2800_bulk_aq.py
+-rw-r--r--   0 anthony   (1030) users      (100)     7813 2022-10-18 22:31:58.000000 oracledb-1.3.1/tests/test_2900_rowid.py
+-rw-r--r--   0 anthony   (1030) users      (100)     7971 2022-05-20 21:47:15.000000 oracledb-1.3.1/tests/test_3000_subscription.py
+-rw-r--r--   0 anthony   (1030) users      (100)     3943 2023-01-18 17:02:49.000000 oracledb-1.3.1/tests/test_3100_boolean_var.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    24905 2023-04-21 18:03:32.000000 oracledb-1.3.1/tests/test_3200_features_12_1.py
+-rw-r--r--   0 anthony   (1030) users      (100)     5670 2022-05-20 21:47:15.000000 oracledb-1.3.1/tests/test_3300_soda_database.py
+-rw-r--r--   0 anthony   (1030) users      (100)    21475 2022-09-29 00:05:59.000000 oracledb-1.3.1/tests/test_3400_soda_collection.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    10520 2023-03-21 23:24:10.000000 oracledb-1.3.1/tests/test_3500_json.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    25036 2023-03-21 21:27:13.000000 oracledb-1.3.1/tests/test_3600_outputtypehandler.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    20995 2023-03-21 23:24:10.000000 oracledb-1.3.1/tests/test_3700_var.py
+-rw-r--r--   0 anthony   (1030) users      (100)    10197 2022-05-20 21:47:15.000000 oracledb-1.3.1/tests/test_3800_typehandler.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    16463 2023-04-21 18:03:32.000000 oracledb-1.3.1/tests/test_3900_cursor_execute.py
+-rw-r--r--   0 anthony   (1030) users      (100)    13808 2022-07-29 21:22:34.000000 oracledb-1.3.1/tests/test_4000_cursor_executemany.py
+-rw-r--r--   0 anthony   (1030) users      (100)     6304 2022-05-20 21:47:15.000000 oracledb-1.3.1/tests/test_4100_cursor_callproc.py
+-rw-r--r--   0 anthony   (1030) users      (100)    10122 2022-05-20 21:47:15.000000 oracledb-1.3.1/tests/test_4200_cursor_scrollable.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    43164 2023-04-21 18:03:32.000000 oracledb-1.3.1/tests/test_4300_cursor_other.py
+-rw-r--r--   0 anthony   (1030) users      (100)     5200 2022-11-07 16:22:37.000000 oracledb-1.3.1/tests/test_4400_tpc.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    30813 2023-03-27 21:31:03.000000 oracledb-1.3.1/tests/test_4500_connect_params.py
+-rw-r--r--   0 anthony   (1030) users      (100)     9049 2022-05-20 21:47:15.000000 oracledb-1.3.1/tests/test_4600_type_changes.py
+-rw-r--r--   0 anthony   (1030) users      (100)     2746 2022-08-27 17:02:29.000000 oracledb-1.3.1/tests/test_4700_pool_params.py
+-rw-rw-r--   0 anthony   (1030) users      (100)     7614 2023-04-21 18:03:32.000000 oracledb-1.3.1/tests/test_4800_timestamp_ltz_var.py
+-rw-r--r--   0 anthony   (1030) users      (100)     7315 2022-06-10 16:31:07.000000 oracledb-1.3.1/tests/test_4900_timestamp_tz_var.py
+-rw-r--r--   0 anthony   (1030) users      (100)    11969 2022-08-02 17:00:32.000000 oracledb-1.3.1/tests/test_5000_externalauth.py
+-rw-rw-r--   0 anthony   (1030) users      (100)    15525 2023-04-21 18:03:32.000000 oracledb-1.3.1/tests/test_env.py
+-rw-r--r--   0 anthony   (1030) users      (100)      593 2022-12-01 16:31:07.000000 oracledb-1.3.1/tox.ini
```

### Comparing `oracledb-1.3.0/LICENSE.txt` & `oracledb-1.3.1/LICENSE.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2016, 2022 Oracle and/or its affiliates.
+Copyright (c) 2016, 2023 Oracle and/or its affiliates.
 
 This software is dual-licensed to you under the Universal Permissive License
 (UPL) 1.0 as shown at https://oss.oracle.com/licenses/upl and Apache License
 2.0 as shown at http://www.apache.org/licenses/LICENSE-2.0. You may choose
 either license.
 
 If you elect to accept the software under the Apache License, Version 2.0,
```

### Comparing `oracledb-1.3.0/PKG-INFO` & `oracledb-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oracledb
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python interface to Oracle Database
 Home-page: https://oracle.github.io/python-oracledb
 Author: Anthony Tuininga
 Author-email: anthony.tuininga@oracle.com
 License: Apache and/or UPL
 Project-URL: Installation, https://python-oracledb.readthedocs.io/en/latest/user_guide/installation.html
 Project-URL: Samples, https://github.com/oracle/python-oracledb/tree/main/samples
```

### Comparing `oracledb-1.3.0/THIRD_PARTY_LICENSES.txt` & `oracledb-1.3.1/THIRD_PARTY_LICENSES.txt`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/setup.cfg` & `oracledb-1.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/setup.py` & `oracledb-1.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/__init__.py` & `oracledb-1.3.1/src/oracledb/__init__.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/aq.py` & `oracledb-1.3.1/src/oracledb/aq.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/base_impl.pxd` & `oracledb-1.3.1/src/oracledb/base_impl.pxd`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/base_impl.pyx` & `oracledb-1.3.1/src/oracledb/base_impl.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/connect_params.py` & `oracledb-1.3.1/src/oracledb/connect_params.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/connection.py` & `oracledb-1.3.1/src/oracledb/connection.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/constants.py` & `oracledb-1.3.1/src/oracledb/constants.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/constructors.py` & `oracledb-1.3.1/src/oracledb/constructors.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/cursor.py` & `oracledb-1.3.1/src/oracledb/cursor.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/dbobject.py` & `oracledb-1.3.1/src/oracledb/dbobject.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/defaults.py` & `oracledb-1.3.1/src/oracledb/defaults.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/driver_mode.py` & `oracledb-1.3.1/src/oracledb/driver_mode.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/dsn.py` & `oracledb-1.3.1/src/oracledb/dsn.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/errors.py` & `oracledb-1.3.1/src/oracledb/errors.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/exceptions.py` & `oracledb-1.3.1/src/oracledb/exceptions.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/base/bind_var.pyx` & `oracledb-1.3.1/src/oracledb/impl/base/bind_var.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/base/connect_params.pyx` & `oracledb-1.3.1/src/oracledb/impl/base/connect_params.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/base/connection.pyx` & `oracledb-1.3.1/src/oracledb/impl/base/connection.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/base/cursor.pyx` & `oracledb-1.3.1/src/oracledb/impl/base/cursor.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/base/dbobject.pyx` & `oracledb-1.3.1/src/oracledb/impl/base/dbobject.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/base/lob.pyx` & `oracledb-1.3.1/src/oracledb/impl/base/lob.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/base/pool.pyx` & `oracledb-1.3.1/src/oracledb/impl/base/pool.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/base/pool_params.pyx` & `oracledb-1.3.1/src/oracledb/impl/base/pool_params.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/base/queue.pyx` & `oracledb-1.3.1/src/oracledb/impl/base/queue.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/base/soda.pyx` & `oracledb-1.3.1/src/oracledb/impl/base/soda.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/base/subscr.pyx` & `oracledb-1.3.1/src/oracledb/impl/base/subscr.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/base/types.pyx` & `oracledb-1.3.1/src/oracledb/impl/base/types.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/base/utils.pyx` & `oracledb-1.3.1/src/oracledb/impl/base/utils.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/base/var.pyx` & `oracledb-1.3.1/src/oracledb/impl/base/var.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/buffer.pyx` & `oracledb-1.3.1/src/oracledb/impl/thick/buffer.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/connection.pyx` & `oracledb-1.3.1/src/oracledb/impl/thick/connection.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/cursor.pyx` & `oracledb-1.3.1/src/oracledb/impl/thick/cursor.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/dbobject.pyx` & `oracledb-1.3.1/src/oracledb/impl/thick/dbobject.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/json.pyx` & `oracledb-1.3.1/src/oracledb/impl/thick/json.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/lob.pyx` & `oracledb-1.3.1/src/oracledb/impl/thick/lob.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/odpi/embed/dpi.c` & `oracledb-1.3.1/src/oracledb/impl/thick/odpi/embed/dpi.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/odpi/include/dpi.h` & `oracledb-1.3.1/src/oracledb/impl/thick/odpi/include/dpi.h`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiConn.c` & `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiConn.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiContext.c` & `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiContext.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiData.c` & `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiData.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiDebug.c` & `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiDebug.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiDeqOptions.c` & `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiDeqOptions.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiEnqOptions.c` & `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiEnqOptions.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiEnv.c` & `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiEnv.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiError.c` & `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiError.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiErrorMessages.h` & `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiErrorMessages.h`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiGen.c` & `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiGen.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiGlobal.c` & `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiGlobal.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiHandleList.c` & `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiHandleList.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiHandlePool.c` & `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiHandlePool.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiImpl.h` & `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiImpl.h`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiJson.c` & `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiJson.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiLob.c` & `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiLob.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiMsgProps.c` & `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiMsgProps.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiObject.c` & `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiObject.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiObjectAttr.c` & `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiObjectAttr.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiObjectType.c` & `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiObjectType.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiOci.c` & `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiOci.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiOracleType.c` & `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiOracleType.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiPool.c` & `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiPool.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiQueue.c` & `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiQueue.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiRowid.c` & `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiRowid.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiSodaColl.c` & `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiSodaColl.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiSodaCollCursor.c` & `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiSodaCollCursor.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiSodaDb.c` & `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiSodaDb.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiSodaDoc.c` & `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiSodaDoc.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiSodaDocCursor.c` & `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiSodaDocCursor.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiStmt.c` & `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiStmt.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiSubscr.c` & `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiSubscr.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiUtils.c` & `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiUtils.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/odpi/src/dpiVar.c` & `oracledb-1.3.1/src/oracledb/impl/thick/odpi/src/dpiVar.c`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/odpi.pxd` & `oracledb-1.3.1/src/oracledb/impl/thick/odpi.pxd`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/pool.pyx` & `oracledb-1.3.1/src/oracledb/impl/thick/pool.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/queue.pyx` & `oracledb-1.3.1/src/oracledb/impl/thick/queue.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/soda.pyx` & `oracledb-1.3.1/src/oracledb/impl/thick/soda.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/subscr.pyx` & `oracledb-1.3.1/src/oracledb/impl/thick/subscr.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/utils.pyx` & `oracledb-1.3.1/src/oracledb/impl/thick/utils.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thick/var.pyx` & `oracledb-1.3.1/src/oracledb/impl/thick/var.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thin/buffer.pyx` & `oracledb-1.3.1/src/oracledb/impl/thin/buffer.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thin/capabilities.pyx` & `oracledb-1.3.1/src/oracledb/impl/thin/capabilities.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thin/connection.pyx` & `oracledb-1.3.1/src/oracledb/impl/thin/connection.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thin/constants.pxi` & `oracledb-1.3.1/src/oracledb/impl/thin/constants.pxi`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thin/conversions.pyx` & `oracledb-1.3.1/src/oracledb/impl/thin/conversions.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thin/crypto.pyx` & `oracledb-1.3.1/src/oracledb/impl/thin/crypto.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thin/cursor.pyx` & `oracledb-1.3.1/src/oracledb/impl/thin/cursor.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #------------------------------------------------------------------------------
-# Copyright (c) 2020, 2022, Oracle and/or its affiliates.
+# Copyright (c) 2020, 2023, Oracle and/or its affiliates.
 #
 # This software is dual-licensed to you under the Universal Permissive License
 # (UPL) 1.0 as shown at https://oss.oracle.com/licenses/upl and Apache License
 # 2.0 as shown at http://www.apache.org/licenses/LICENSE-2.0. You may choose
 # either license.
 #
 # If you elect to accept the software under the Apache License, Version 2.0,
```

### Comparing `oracledb-1.3.0/src/oracledb/impl/thin/data_types.pyx` & `oracledb-1.3.1/src/oracledb/impl/thin/data_types.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thin/dbobject.pyx` & `oracledb-1.3.1/src/oracledb/impl/thin/dbobject.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thin/lob.pyx` & `oracledb-1.3.1/src/oracledb/impl/thin/lob.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thin/messages.pyx` & `oracledb-1.3.1/src/oracledb/impl/thin/messages.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -248,23 +248,21 @@
         else:
             msg = f"Unhandled server side piggyback opcode: {opcode}"
             raise Exception(msg)
 
     cdef int _process_warning_info(self, ReadBuffer buf) except -1:
         cdef:
             _OracleErrorInfo info = self.error_info
-            const char_type *ptr
             uint16_t num_bytes, temp16
         buf.read_ub2(&temp16)               # error number
         info.num = temp16
         buf.read_ub2(&num_bytes)            # length of error message
         buf.skip_ub2()                      # flags
         if info.num != 0 and num_bytes > 0:
-            ptr = buf.read_raw_bytes(num_bytes)
-            info.message = ptr[:num_bytes].decode().rstrip()
+            info.message = buf.read_str(TNS_CS_IMPLICIT).rstrip()
         info.is_warning = True
 
     cdef int _write_function_code(self, WriteBuffer buf) except -1:
         buf.write_uint8(self.message_type)
         buf.write_uint8(self.function_code)
         buf.write_seq_num()
         if buf._caps.ttc_field_version >= TNS_CCAP_FIELD_VERSION_23_1_EXT_1:
@@ -452,14 +450,15 @@
         # variables in order to take the new type handler into account
         conn = self.cursor.connection
         type_handler = cursor_impl._get_output_type_handler()
         if type_handler is not statement._last_output_type_handler:
             for i, var_impl in enumerate(cursor_impl.fetch_var_impls):
                 cursor_impl._create_fetch_var(conn, self.cursor, type_handler,
                                               i, var_impl._fetch_info)
+            cursor_impl._statement._adjust_requires_define()
             statement._last_output_type_handler = type_handler
 
         # the list of output variables is equivalent to the fetch variables
         self.out_var_impls = cursor_impl.fetch_var_impls
 
         # resize fetch variables, if necessary, to allow room in each variable
         # for the fetch array size
@@ -715,14 +714,15 @@
         for i in range(cursor_impl._num_columns):
             fetch_info = self._process_column_info(buf, cursor_impl)
             if prev_fetch_var_impls is not None \
                     and i < len(prev_fetch_var_impls):
                 self._adjust_fetch_info(prev_fetch_var_impls[i], fetch_info)
             cursor_impl._create_fetch_var(conn, self.cursor, type_handler, i,
                                           fetch_info)
+        cursor_impl._statement._adjust_requires_define()
         buf.read_ub4(&num_bytes)
         if num_bytes > 0:
             buf.skip_raw_bytes_chunked()    # current date
         buf.skip_ub4()                      # dcbflag
         buf.skip_ub4()                      # dcbmdbz
         buf.skip_ub4()                      # dcbmnpr
         buf.skip_ub4()                      # dcbmxpr
@@ -1772,18 +1772,16 @@
             int i
 
         # write character set and capabilities
         buf.write_uint8(TNS_MSG_TYPE_DATA_TYPES)
         buf.write_uint16(TNS_CHARSET_UTF8, BYTE_ORDER_LSB)
         buf.write_uint16(TNS_CHARSET_UTF8, BYTE_ORDER_LSB)
         buf.write_uint8(TNS_ENCODING_MULTI_BYTE | TNS_ENCODING_CONV_LENGTH)
-        buf.write_uint8(len(buf._caps.compile_caps))
-        buf.write_bytes(bytes(buf._caps.compile_caps))
-        buf.write_uint8(len(buf._caps.runtime_caps))
-        buf.write_bytes(bytes(buf._caps.runtime_caps))
+        buf.write_bytes_with_length(bytes(buf._caps.compile_caps))
+        buf.write_bytes_with_length(bytes(buf._caps.runtime_caps))
 
         # write data types
         i = 0
         while True:
             data_type = &DATA_TYPES[i]
             if data_type.data_type == 0:
                 break
@@ -1848,17 +1846,17 @@
                 if self.cursor_impl.prefetchrows > 0:
                     options |= TNS_EXEC_OPTION_FETCH
                 if stmt._cursor_id == 0 or stmt._requires_define:
                     num_iters = self.cursor_impl.prefetchrows
                     self.cursor_impl._fetch_array_size = num_iters
                 else:
                     num_iters = self.cursor_impl._fetch_array_size
-        if not stmt._is_plsql:
+        if not stmt._is_plsql and not self.parse_only:
             options |= TNS_EXEC_OPTION_NOT_PLSQL
-        elif num_params > 0:
+        elif stmt._is_plsql and num_params > 0:
             options |= TNS_EXEC_OPTION_PLSQL_BIND
         if num_params > 0:
             options |= TNS_EXEC_OPTION_BIND
         if self.batcherrors:
             options |= TNS_EXEC_OPTION_BATCH_ERRORS
         if self.arraydmlrowcounts:
             dml_options = TNS_EXEC_OPTION_DML_ROWCOUNTS
@@ -2000,16 +1998,19 @@
         """
         Write the execute message to the buffer. Two types of execute messages
         are possible: one for a full execute and the second, simpler message,
         for when an existing cursor is being re-executed.
         """
         cdef:
             Statement stmt = self.cursor_impl._statement
-        if stmt._cursor_id != 0 and not stmt._requires_full_execute \
-                and not self.parse_only and not stmt._is_ddl \
+        if stmt._cursor_id != 0 \
+                and not stmt._requires_full_execute \
+                and not stmt._always_full_execute \
+                and not self.parse_only \
+                and not stmt._is_ddl \
                 and not self.batcherrors:
             if stmt._is_query and not stmt._requires_define \
                     and self.cursor_impl.prefetchrows > 0:
                 self.function_code = TNS_FUNC_REEXECUTE_AND_FETCH
             else:
                 self.function_code = TNS_FUNC_REEXECUTE
             self._write_reexecute_message(buf)
```

### Comparing `oracledb-1.3.0/src/oracledb/impl/thin/oson.pyx` & `oracledb-1.3.1/src/oracledb/impl/thin/oson.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thin/packet.pyx` & `oracledb-1.3.1/src/oracledb/impl/thin/packet.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thin/pool.pyx` & `oracledb-1.3.1/src/oracledb/impl/thin/pool.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -324,17 +324,18 @@
         Helper method which checks the free and used connection lists before
         acquiring to drop off timed out connections
         """
         cdef ThinConnImpl conn_impl
         current_time = time.monotonic()
         while self.get_open_count() > self.min and conn_impls_to_check:
             conn_impl = conn_impls_to_check[0]
-            if current_time - conn_impl._time_in_pool > self._timeout:
-                conn_impls_to_check.pop(0)
-                self._drop_conn_impl(conn_impl)
+            if current_time - conn_impl._time_in_pool < self._timeout:
+                break
+            conn_impls_to_check.pop(0)
+            self._drop_conn_impl(conn_impl)
 
     def acquire(self, ConnectParamsImpl params):
         """
         Internal method for acquiring a connection from the pool.
         """
         cdef:
             ThinConnImpl conn_impl
```

### Comparing `oracledb-1.3.0/src/oracledb/impl/thin/protocol.pyx` & `oracledb-1.3.1/src/oracledb/impl/thin/protocol.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thin/statement.pyx` & `oracledb-1.3.1/src/oracledb/impl/thin/statement.pyx`

 * *Files 10% similar despite different names*

```diff
@@ -34,20 +34,26 @@
 # 1. Quoted and non-quoted bind names are allowed.
 # 2. Quoted binds can contain any characters.
 # 3. Non-quoted binds must begin with an alphabet character.
 # 4. Non-quoted binds can only contain alphanumeric characters, the underscore,
 #    the dollar sign and the pound sign.
 # 5. Non-quoted binds cannot be Oracle Database Reserved Names (Server handles
 #    this case and returns an appropriate error)
-BIND_PATTERN = r'(?<!"\:)(?<=\:)\s*("[^\"]*"|[^\W\d_][\w\$#]*|\d+)'
+BIND_PATTERN = r':\s*((?:".*?")|(?:[^\W\d_][\w\$#]*)|\d+)'
 
 # pattern used for detecting a DML returning clause; bind variables in the
-# first group are input variables; bind variables in the second group are
-# output only variables
-DML_RETURNING_PATTERN = r'(?si)([)\s]RETURNING[(\s][\s\S]+[)\s]INTO\s+)(.*?$)'
+# SQL prior to the INTO keyword are input variables; bind varibles in the SQL
+# after the INTO keyword are output variables
+DML_RETURNING_PATTERN = r'(?si)(?<=\bRETURNING\b)(.*?)(?=\bINTO\b)'
+
+# patterns for identifying comments and quoted strings
+SINGLE_LINE_COMMENT_PATTERN = r'--.*'
+MULTI_LINE_COMMENT_PATTERN = r'(?s)/\*.*?\*/'
+CONSTANT_STRING_PATTERN = r"(?s)'.*?'"
+QUOTED_NAME_PATTERN = r'(:\s*)?(".*?")'
 
 cdef class BindInfo:
 
     cdef:
         uint32_t num_elements
         bint _is_return_bind
         uint8_t ora_type_num
@@ -84,14 +90,15 @@
         list _bind_info_list
         list _fetch_vars
         list _fetch_var_impls
         object _bind_info_dict
         object _last_output_type_handler
         uint32_t _num_columns
         bint _requires_full_execute
+        bint _always_full_execute
         bint _requires_define
         bint _return_to_cache
         bint _in_use
 
     cdef Statement copy(self):
         cdef:
             Statement copied_statement = Statement()
@@ -135,14 +142,26 @@
             info = BindInfo(name, is_return_bind)
             self._bind_info_list.append(info)
             if info._bind_name in self._bind_info_dict:
                 self._bind_info_dict[info._bind_name].append(info)
             else:
                 self._bind_info_dict[info._bind_name] = [info]
 
+    cdef int _adjust_requires_define(self) except -1:
+        """
+        The define step is only supposed to be done once for each cursor, but a
+        full execute is required if a define was ever performed, so perform
+        that adjustment here, if needed.
+        """
+        if self._requires_define:
+            if self._always_full_execute:
+                self._requires_define = False
+            else:
+                self._always_full_execute = True
+
     cdef _determine_statement_type(self, str sql):
         """
         Determine the type of the SQL statement by examining the first keyword
         found in the statement.
         """
         tokens = sql.strip().lstrip("(")[:10].split()
         if tokens:
@@ -173,36 +192,38 @@
         self._sql_bytes = self._sql.encode()
         self._sql_length = <uint32_t> len(self._sql_bytes)
 
         # create empty list (bind by position) and dict (bind by name)
         self._bind_info_dict = collections.OrderedDict()
         self._bind_info_list = []
 
-        # Strip single/multiline comments and strings from the sql statement to
-        # ease searching for bind variables.
-        sql = re.sub(r"/\*[\S\n ]+?\*/", "", sql)
-        sql = re.sub(r"\--.*(\n|$)", "", sql)
-        sql = re.sub(r"""'[^']*'(?=(?:[^']*[^']*')*[^']*$)*""", "", sql,
-                     flags=re.MULTILINE)
-        sql = re.sub(r'(:\s*)?("([^"]*)")',
-                    lambda m: m.group(0) if sql[m.start(0)] == ":" else "",
+        # Strip single/multiline comments and replace constant strings and
+        # quoted names with single characters in order to facilitate detection
+        # of bind variables; note that bind variables can be quoted so a check
+        # must be made to ensure that a quoted string doesn't refer to a bind
+        # variable first before it can be replaced
+        sql = re.sub(MULTI_LINE_COMMENT_PATTERN, "", sql)
+        sql = re.sub(SINGLE_LINE_COMMENT_PATTERN, "", sql)
+        sql = re.sub(CONSTANT_STRING_PATTERN, "S", sql)
+        sql = re.sub(QUOTED_NAME_PATTERN,
+                    lambda m: m.group(0) if sql[m.start(0)] == ":" else "Q",
                     sql)
 
         # determine statement type
         self._determine_statement_type(sql)
 
         # bind variables can only be found in queries, DML and PL/SQL
         if self._is_query or self._is_dml or self._is_plsql:
             input_sql = sql
-            if not self._is_plsql:
+            if self._is_dml:
                 match = re.search(DML_RETURNING_PATTERN, sql)
                 if match is not None:
-                    pos = match.start(2)
+                    pos = match.end()
                     input_sql = sql[:pos]
-                    returning_sql = sql[pos:]
+                    returning_sql = sql[pos + 4:]
             self._add_binds(input_sql, is_return_bind=False)
             if returning_sql is not None:
                 self._is_returning = True
                 self._add_binds(returning_sql, is_return_bind=True)
 
     cdef int _set_var(self, BindInfo bind_info, ThinVarImpl var_impl,
                       ThinCursorImpl cursor_impl) except -1:
```

### Comparing `oracledb-1.3.0/src/oracledb/impl/thin/utils.pyx` & `oracledb-1.3.1/src/oracledb/impl/thin/utils.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/impl/thin/var.pyx` & `oracledb-1.3.1/src/oracledb/impl/thin/var.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/lob.py` & `oracledb-1.3.1/src/oracledb/lob.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/pool.py` & `oracledb-1.3.1/src/oracledb/pool.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/pool_params.py` & `oracledb-1.3.1/src/oracledb/pool_params.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/soda.py` & `oracledb-1.3.1/src/oracledb/soda.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/subscr.py` & `oracledb-1.3.1/src/oracledb/subscr.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/thick_impl.pyx` & `oracledb-1.3.1/src/oracledb/thick_impl.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/thin_impl.pyx` & `oracledb-1.3.1/src/oracledb/thin_impl.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/utils.py` & `oracledb-1.3.1/src/oracledb/utils.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/var.py` & `oracledb-1.3.1/src/oracledb/var.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/src/oracledb/version.py` & `oracledb-1.3.1/src/oracledb/version.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #------------------------------------------------------------------------------
-# Copyright (c) 2021, 2022, Oracle and/or its affiliates.
+# Copyright (c) 2021, 2023, Oracle and/or its affiliates.
 #
 # This software is dual-licensed to you under the Universal Permissive License
 # (UPL) 1.0 as shown at https://oss.oracle.com/licenses/upl and Apache License
 # 2.0 as shown at http://www.apache.org/licenses/LICENSE-2.0. You may choose
 # either license.
 #
 # If you elect to accept the software under the Apache License, Version 2.0,
@@ -26,8 +26,8 @@
 # version.py
 #
 # Defines the version of the package. This is the only place where this is
 # found. The setup.cfg configuration file and the documentation configuration
 # file doc/src/conf.py both reference this file directly.
 #------------------------------------------------------------------------------
 
-__version__ = "1.3.0"
+__version__ = "1.3.1"
```

### Comparing `oracledb-1.3.0/src/oracledb.egg-info/PKG-INFO` & `oracledb-1.3.1/src/oracledb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oracledb
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python interface to Oracle Database
 Home-page: https://oracle.github.io/python-oracledb
 Author: Anthony Tuininga
 Author-email: anthony.tuininga@oracle.com
 License: Apache and/or UPL
 Project-URL: Installation, https://python-oracledb.readthedocs.io/en/latest/user_guide/installation.html
 Project-URL: Samples, https://github.com/oracle/python-oracledb/tree/main/samples
```

### Comparing `oracledb-1.3.0/src/oracledb.egg-info/SOURCES.txt` & `oracledb-1.3.1/src/oracledb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/tests/create_schema.py` & `oracledb-1.3.1/tests/create_schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #------------------------------------------------------------------------------
-# Copyright (c) 2020, 2022, Oracle and/or its affiliates.
+# Copyright (c) 2020, 2023, Oracle and/or its affiliates.
 #
 # This software is dual-licensed to you under the Universal Permissive License
 # (UPL) 1.0 as shown at https://oss.oracle.com/licenses/upl and Apache License
 # 2.0 as shown at http://www.apache.org/licenses/LICENSE-2.0. You may choose
 # either license.
 #
 # If you elect to accept the software under the Apache License, Version 2.0,
@@ -43,11 +43,14 @@
 # create test schemas
 print("Creating test schemas...")
 test_env.run_sql_script(conn, "create_schema",
                         main_user=test_env.get_main_user(),
                         main_password=test_env.get_main_password(),
                         proxy_user=test_env.get_proxy_user(),
                         proxy_password=test_env.get_proxy_password())
+if test_env.get_server_version() >= (21, 0):
+    test_env.run_sql_script(conn, "create_schema_21",
+                            main_user=test_env.get_main_user())
 if test_env.is_on_oracle_cloud(conn):
     test_env.run_sql_script(conn, "create_schema_cloud",
                             main_user=test_env.get_main_user())
 print("Done.")
```

### Comparing `oracledb-1.3.0/tests/drop_schema.py` & `oracledb-1.3.1/tests/drop_schema.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/tests/test_1000_module.py` & `oracledb-1.3.1/tests/test_1000_module.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/tests/test_1100_connection.py` & `oracledb-1.3.1/tests/test_1100_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,16 +134,15 @@
         cursor.execute("insert into TestTempTable (IntCol) values (2)")
         other_cursor.execute("select IntCol from TestTempTable order by IntCol")
         rows = other_cursor.fetchall()
         self.assertEqual(rows, [(1,), (2,)])
 
     def test_1105_bad_connect_string(self):
         "1105 - connection to database with bad connect string"
-        errors = "^DPY-4000:|^DPY-4001:|^DPY-4026:|^DPY-4027:|^ORA-12154:"
-        self.assertRaisesRegex(oracledb.DatabaseError, errors,
+        self.assertRaisesRegex(oracledb.DatabaseError, "^DPY-4001:|ORA-12547:",
                                oracledb.connect, test_env.get_main_user())
         self.assertRaisesRegex(oracledb.DatabaseError, "^DPY-4000:|^DPY-4001:",
                                oracledb.connect, test_env.get_main_user() + \
                                "@" + test_env.get_connect_string())
         errors = "^DPY-4000:|^DPY-4001:|^DPY-4017:|^ORA-12154:|^ORA-12521:"
         self.assertRaisesRegex(oracledb.DatabaseError, errors,
                                oracledb.connect, test_env.get_main_user() + \
```

### Comparing `oracledb-1.3.0/tests/test_1300_cursor_var.py` & `oracledb-1.3.1/tests/test_1300_cursor_var.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #------------------------------------------------------------------------------
-# Copyright (c) 2020, 2022, Oracle and/or its affiliates.
+# Copyright (c) 2020, 2023, Oracle and/or its affiliates.
 #
 # This software is dual-licensed to you under the Universal Permissive License
 # (UPL) 1.0 as shown at https://oss.oracle.com/licenses/upl and Apache License
 # 2.0 as shown at http://www.apache.org/licenses/LICENSE-2.0. You may choose
 # either license.
 #
 # If you elect to accept the software under the Apache License, Version 2.0,
@@ -203,16 +203,17 @@
                         open :cursor for
                             select user
                             from dual;
                     end if;
                 end;""",
                 cursor=ref_cursor_var)
         ref_cursor = ref_cursor_var.getvalue()
-        self.assertRaisesRegex(oracledb.DatabaseError, "^DPY-4025:",
-                               ref_cursor.fetchall)
+        if ref_cursor is not None:
+            self.assertRaisesRegex(oracledb.DatabaseError, "^DPY-4025:",
+                                   ref_cursor.fetchall)
 
     def test_1311_fetch_cursor_uses_custom_class(self):
         "1311 - test fetching a cursor with a custom class"
         class Counter:
             num_cursors_created = 0
             @classmethod
             def cursor_created(cls):
```

### Comparing `oracledb-1.3.0/tests/test_1400_datetime_var.py` & `oracledb-1.3.1/tests/test_1400_datetime_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/tests/test_1500_types.py` & `oracledb-1.3.1/tests/test_1500_types.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/tests/test_1600_dml_returning.py` & `oracledb-1.3.1/tests/test_1600_dml_returning.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/tests/test_1700_error.py` & `oracledb-1.3.1/tests/test_1700_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #------------------------------------------------------------------------------
-# Copyright (c) 2020, 2022, Oracle and/or its affiliates.
+# Copyright (c) 2020, 2023, Oracle and/or its affiliates.
 #
 # This software is dual-licensed to you under the Universal Permissive License
 # (UPL) 1.0 as shown at https://oss.oracle.com/licenses/upl and Apache License
 # 2.0 as shown at http://www.apache.org/licenses/LICENSE-2.0. You may choose
 # either license.
 #
 # If you elect to accept the software under the Apache License, Version 2.0,
@@ -60,24 +60,25 @@
         self.assertTrue(new_error_obj.code == error_obj.code)
         self.assertTrue(new_error_obj.offset == error_obj.offset)
         self.assertTrue(new_error_obj.context == error_obj.context)
         self.assertTrue(new_error_obj.isrecoverable == error_obj.isrecoverable)
 
     def test_1702_error_full_code(self):
         "1702 - test generation of full_code for ORA, DPI and DPY errors"
+        cursor = self.connection.cursor()
         with self.assertRaises(oracledb.Error) as cm:
-            self.cursor.execute(None)
+            cursor.execute(None)
         error_obj, = cm.exception.args
         self.assertEqual(error_obj.full_code, "DPY-2001")
         if not self.connection.thin:
             with self.assertRaises(oracledb.Error) as cm:
-                self.cursor.execute("truncate table TestTempTable")
-                int_var = self.cursor.var(int)
-                str_var = self.cursor.var(str, 2)
-                self.cursor.execute("""
+                cursor.execute("truncate table TestTempTable")
+                int_var = cursor.var(int)
+                str_var = cursor.var(str, 2)
+                cursor.execute("""
                         insert into TestTempTable (IntCol, StringCol1)
                         values (1, 'Longer than two chars')
                         returning IntCol, StringCol1
                         into :int_var, :str_var""",
                         int_var=int_var, str_var=str_var)
             error_obj, = cm.exception.args
             self.assertEqual(error_obj.full_code, "DPI-1037")
```

### Comparing `oracledb-1.3.0/tests/test_1800_interval_var.py` & `oracledb-1.3.1/tests/test_1800_interval_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/tests/test_1900_lob_var.py` & `oracledb-1.3.1/tests/test_1900_lob_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/tests/test_2000_long_var.py` & `oracledb-1.3.1/tests/test_2000_long_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/tests/test_2100_nchar_var.py` & `oracledb-1.3.1/tests/test_2100_nchar_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/tests/test_2200_number_var.py` & `oracledb-1.3.1/tests/test_2200_number_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/tests/test_2300_object_var.py` & `oracledb-1.3.1/tests/test_2300_object_var.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,14 @@
         "2303 - test getting an empty collection as a list"
         type_obj = self.connection.gettype("UDT_ARRAY")
         obj = type_obj.newobject()
         self.assertEqual(obj.aslist(), [])
 
     def test_2304_fetch_data(self):
         "2304 - test fetching objects"
-        self.cursor.execute("alter session set time_zone = 'UTC'")
         self.cursor.execute("""
                 select IntCol, ObjectCol, ArrayCol
                 from TestObjects
                 order by IntCol""")
         expected_value = [
             ('INTCOL', oracledb.DB_TYPE_NUMBER, 10, None, 9, 0, False),
             ('OBJECTCOL', oracledb.DB_TYPE_OBJECT, None, None, None, None,
@@ -252,15 +251,14 @@
         obj, = self.cursor.fetchone()
         self.assertEqual(obj.type.schema, self.connection.username.upper())
         self.assertEqual(obj.type.name, "UDT_OBJECT")
         self.assertEqual(obj.type.attributes[0].name, "NUMBERVALUE")
 
     def test_2307_round_trip_object(self):
         "2307 - test inserting and then querying object with all data types"
-        self.cursor.execute("alter session set time_zone = 'UTC'")
         self.cursor.execute("truncate table TestClobs")
         self.cursor.execute("truncate table TestNClobs")
         self.cursor.execute("truncate table TestBlobs")
         self.cursor.execute("""
                 insert into TestClobs
                 (IntCol, ClobCol)
                 values (1, 'A short CLOB')""")
```

### Comparing `oracledb-1.3.0/tests/test_2400_pool.py` & `oracledb-1.3.1/tests/test_2400_pool.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/tests/test_2500_string_var.py` & `oracledb-1.3.1/tests/test_2500_string_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/tests/test_2600_timestamp_var.py` & `oracledb-1.3.1/tests/test_2600_timestamp_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/tests/test_2700_aq.py` & `oracledb-1.3.1/tests/test_2700_aq.py`

 * *Files 0% similar despite different names*

```diff
@@ -518,15 +518,14 @@
         random_string = "This is a string message"
         props = self.connection.msgproperties(payload=random_string)
         self.assertRaisesRegex(oracledb.DatabaseError, "^DPI-1071:",
                                queue.enqone, props)
 
     def test_2723_enqtime(self):
         "2723 - test message props enqtime"
-        self.cursor.execute("alter session set time_zone = '0:00'")
         queue = self.get_and_clear_queue(self.book_queue_name,
                                          self.book_type_name)
         book = queue.payload_type.newobject()
         self.cursor.execute("select sysdate from dual")
         start_date, = self.cursor.fetchone()
         props = self.connection.msgproperties(payload=book)
         queue.enqone(props)
```

### Comparing `oracledb-1.3.0/tests/test_2800_bulk_aq.py` & `oracledb-1.3.1/tests/test_2800_bulk_aq.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/tests/test_2900_rowid.py` & `oracledb-1.3.1/tests/test_2900_rowid.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/tests/test_3000_subscription.py` & `oracledb-1.3.1/tests/test_3000_subscription.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/tests/test_3100_boolean_var.py` & `oracledb-1.3.1/tests/test_3100_boolean_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/tests/test_3200_features_12_1.py` & `oracledb-1.3.1/tests/test_3200_features_12_1.py`

 * *Files 1% similar despite different names*

```diff
@@ -395,16 +395,17 @@
         self.assertEqual([n for n, in results[0]],
                          [2924207, None, 59797108943])
         self.assertEqual([n for n, in results[1]],
                          [1222791080775407, None, 25004854810776297743, None])
 
     def test_3221_implicit_results_no_statement(self):
         "3221 - test getimplicitresults() without executing a statement"
+        cursor = self.connection.cursor()
         self.assertRaisesRegex(oracledb.InterfaceError, "^DPY-1004:",
-                               self.cursor.getimplicitresults)
+                               cursor.getimplicitresults)
 
     def test_3222_insert_with_batch_error(self):
         "3222 - test executing insert with multiple distinct batch errors"
         self.cursor.execute("truncate table TestArrayDML")
         rows = [
             (1, "First", 100),
             (2, "Second", 200),
```

### Comparing `oracledb-1.3.0/tests/test_3300_soda_database.py` & `oracledb-1.3.1/tests/test_3300_soda_database.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/tests/test_3400_soda_collection.py` & `oracledb-1.3.1/tests/test_3400_soda_collection.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/tests/test_3500_json.py` & `oracledb-1.3.1/tests/test_3500_json.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/tests/test_3600_outputtypehandler.py` & `oracledb-1.3.1/tests/test_3600_outputtypehandler.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/tests/test_3700_var.py` & `oracledb-1.3.1/tests/test_3700_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/tests/test_3800_typehandler.py` & `oracledb-1.3.1/tests/test_3800_typehandler.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/tests/test_3900_cursor_execute.py` & `oracledb-1.3.1/tests/test_3900_cursor_execute.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #------------------------------------------------------------------------------
-# Copyright (c) 2020, 2022, Oracle and/or its affiliates.
+# Copyright (c) 2020, 2023, Oracle and/or its affiliates.
 #
 # This software is dual-licensed to you under the Universal Permissive License
 # (UPL) 1.0 as shown at https://oss.oracle.com/licenses/upl and Apache License
 # 2.0 as shown at http://www.apache.org/licenses/LICENSE-2.0. You may choose
 # either license.
 #
 # If you elect to accept the software under the Apache License, Version 2.0,
@@ -34,16 +34,17 @@
     def test_3900_execute_no_args(self):
         "3900 - test executing a statement without any arguments"
         result = self.cursor.execute("begin null; end;")
         self.assertEqual(result, None)
 
     def test_3901_execute_no_statement_with_args(self):
         "3901 - test executing a None statement with bind variables"
+        cursor = self.connection.cursor()
         self.assertRaisesRegex(oracledb.ProgrammingError, "^DPY-2001:",
-                               self.cursor.execute, None, x=5)
+                               cursor.execute, None, x=5)
 
     def test_3902_execute_empty_keyword_args(self):
         "3902 - test executing a statement with args and empty keyword args"
         simple_var = self.cursor.var(oracledb.NUMBER)
         args = [simple_var]
         kwargs = {}
         result = self.cursor.execute("begin :1 := 25; end;", args, **kwargs)
```

### Comparing `oracledb-1.3.0/tests/test_4000_cursor_executemany.py` & `oracledb-1.3.1/tests/test_4000_cursor_executemany.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/tests/test_4100_cursor_callproc.py` & `oracledb-1.3.1/tests/test_4100_cursor_callproc.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/tests/test_4200_cursor_scrollable.py` & `oracledb-1.3.1/tests/test_4200_cursor_scrollable.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/tests/test_4300_cursor_other.py` & `oracledb-1.3.1/tests/test_4300_cursor_other.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,25 +32,26 @@
 import oracledb
 import test_env
 
 class TestCase(test_env.BaseTestCase):
 
     def test_4300_prepare(self):
         "4300 - test preparing a statement and executing it multiple times"
-        self.assertEqual(self.cursor.statement, None)
+        cursor = self.connection.cursor()
+        self.assertEqual(cursor.statement, None)
         statement = "begin :value := :value + 5; end;"
-        self.cursor.prepare(statement)
-        var = self.cursor.var(oracledb.NUMBER)
-        self.assertEqual(self.cursor.statement, statement)
+        cursor.prepare(statement)
+        var = cursor.var(oracledb.NUMBER)
+        self.assertEqual(cursor.statement, statement)
         var.setvalue(0, 2)
-        self.cursor.execute(None, value = var)
+        cursor.execute(None, value = var)
         self.assertEqual(var.getvalue(), 7)
-        self.cursor.execute(None, value = var)
+        cursor.execute(None, value = var)
         self.assertEqual(var.getvalue(), 12)
-        self.cursor.execute("begin :value2 := 3; end;", value2 = var)
+        cursor.execute("begin :value2 := 3; end;", value2 = var)
         self.assertEqual(var.getvalue(), 3)
 
     def test_4301_exception_on_close(self):
         "4301 - confirm an exception is raised after closing a cursor"
         self.cursor.close()
         self.assertRaisesRegex(oracledb.InterfaceError, "^DPY-1006:",
                                self.cursor.execute, "select 1 from dual")
@@ -77,32 +78,33 @@
         value, = next(test_iter)
         self.cursor.execute("insert into TestTempTable (IntCol) values (1)")
         self.assertRaisesRegex(oracledb.InterfaceError, "^DPY-1003:", next,
                                test_iter)
 
     def test_4304_bind_names(self):
         "4304 - test that bindnames() works correctly."
+        cursor = self.connection.cursor()
         self.assertRaisesRegex(oracledb.ProgrammingError, "^DPY-2002:",
-                               self.cursor.bindnames)
-        self.cursor.prepare("begin null; end;")
-        self.assertEqual(self.cursor.bindnames(), [])
-        self.cursor.prepare("begin :retval := :inval + 5; end;")
-        self.assertEqual(self.cursor.bindnames(), ["RETVAL", "INVAL"])
-        self.cursor.prepare("begin :retval := :a * :a + :b * :b; end;")
-        self.assertEqual(self.cursor.bindnames(), ["RETVAL", "A", "B"])
-        self.cursor.prepare("begin :a := :b + :c + :d + :e + :f + :g + " + \
-                            ":h + :i + :j + :k + :l; end;")
+                               cursor.bindnames)
+        cursor.prepare("begin null; end;")
+        self.assertEqual(cursor.bindnames(), [])
+        cursor.prepare("begin :retval := :inval + 5; end;")
+        self.assertEqual(cursor.bindnames(), ["RETVAL", "INVAL"])
+        cursor.prepare("begin :retval := :a * :a + :b * :b; end;")
+        self.assertEqual(cursor.bindnames(), ["RETVAL", "A", "B"])
+        cursor.prepare("begin :a := :b + :c + :d + :e + :f + :g + " + \
+                       ":h + :i + :j + :k + :l; end;")
         names = ["A", "B", "C", "D", "E", "F", "G", "H", "I", "J", "K", "L"]
-        self.assertEqual(self.cursor.bindnames(), names)
-        self.cursor.prepare("select :a * :a + :b * :b from dual")
-        self.assertEqual(self.cursor.bindnames(), ["A", "B"])
-        self.cursor.prepare("select :value1 + :VaLue_2 from dual")
-        self.assertEqual(self.cursor.bindnames(), ["VALUE1", "VALUE_2"])
-        self.cursor.prepare("select :élevé, :fenêtre from dual")
-        self.assertEqual(self.cursor.bindnames(), ["ÉLEVÉ", "FENÊTRE"])
+        self.assertEqual(cursor.bindnames(), names)
+        cursor.prepare("select :a * :a + :b * :b from dual")
+        self.assertEqual(cursor.bindnames(), ["A", "B"])
+        cursor.prepare("select :value1 + :VaLue_2 from dual")
+        self.assertEqual(cursor.bindnames(), ["VALUE1", "VALUE_2"])
+        cursor.prepare("select :élevé, :fenêtre from dual")
+        self.assertEqual(cursor.bindnames(), ["ÉLEVÉ", "FENÊTRE"])
 
     def test_4305_set_input_sizes_negative(self):
         "4305 - test cursor.setinputsizes() with invalid parameters"
         val = decimal.Decimal(5)
         self.assertRaisesRegex(oracledb.ProgrammingError, "^DPY-2005:",
                                self.cursor.setinputsizes, val, x=val)
         self.assertRaisesRegex(oracledb.ProgrammingError, "^DPY-2007:",
@@ -899,17 +901,83 @@
             (1, data, 5),
             (2, data, 6)
         ]
         self.cursor.execute(sql, rows[0])
         plsql = f"begin {sql}; end;"
         self.cursor.execute(plsql, rows[1])
         self.connection.commit()
-        oracledb.defaults.fetch_lobs = False
-        self.cursor.execute("""
-            select IntCol, CLOBCol, ExtraNumCol1
-            from TestCLOBs
-            order by IntCol""")
-        fetched_rows = self.cursor.fetchall()
-        self.assertEqual(fetched_rows, rows)
+        with test_env.FetchLobsContextManager(False):
+            self.cursor.execute("""
+                select IntCol, CLOBCol, ExtraNumCol1
+                from TestCLOBs
+                order by IntCol""")
+            fetched_rows = self.cursor.fetchall()
+            self.assertEqual(fetched_rows, rows)
+
+    def test_4370_rebuild_table_with_lob_in_cached_query(self):
+        "4370 - test rebuild of table with LOB in cached query (as string)"
+        table_name = "test_4370"
+        drop_sql = f"drop table {table_name} purge"
+        create_sql = f"""
+            create table {table_name} (
+                Col1 number(9) not null,
+                Col2 clob not null
+            )"""
+        insert_sql = f"insert into {table_name} values (:1, :2)"
+        query_sql = f"select * from {table_name} order by Col1"
+        data = [
+            (1, "CLOB value 1"),
+            (2, "CLOB value 2")
+        ]
+        try:
+            self.cursor.execute(drop_sql)
+        except:
+            pass
+        with test_env.FetchLobsContextManager(False):
+            self.cursor.execute(create_sql)
+            self.cursor.executemany(insert_sql, data)
+            self.cursor.execute(query_sql)
+            self.assertEqual(self.cursor.fetchall(), data)
+            self.cursor.execute(query_sql)
+            self.assertEqual(self.cursor.fetchall(), data)
+            self.cursor.execute(drop_sql)
+            self.cursor.execute(create_sql)
+            self.cursor.executemany(insert_sql, data)
+            self.cursor.execute(query_sql)
+            self.assertEqual(self.cursor.fetchall(), data)
+
+    def test_4371_rebuild_table_with_lob_in_cached_query(self):
+        "4371 - test rebuild of table with LOB in cached query (as LOB)"
+        table_name = "test_4371"
+        drop_sql = f"drop table {table_name} purge"
+        create_sql = f"""
+            create table {table_name} (
+                Col1 number(9) not null,
+                Col2 clob not null
+            )"""
+        insert_sql = f"insert into {table_name} values (:1, :2)"
+        query_sql = f"select * from {table_name} order by Col1"
+        data = [
+            (1, "CLOB value 1"),
+            (2, "CLOB value 2")
+        ]
+        try:
+            self.cursor.execute(drop_sql)
+        except:
+            pass
+        self.cursor.execute(create_sql)
+        self.cursor.executemany(insert_sql, data)
+        self.cursor.execute(query_sql)
+        fetched_data = [(n, c.read()) for n, c in self.cursor]
+        self.assertEqual(fetched_data, data)
+        self.cursor.execute(query_sql)
+        fetched_data = [(n, c.read()) for n, c in self.cursor]
+        self.assertEqual(fetched_data, data)
+        self.cursor.execute(drop_sql)
+        self.cursor.execute(create_sql)
+        self.cursor.executemany(insert_sql, data)
+        self.cursor.execute(query_sql)
+        fetched_data = [(n, c.read()) for n, c in self.cursor]
+        self.assertEqual(fetched_data, data)
 
 if __name__ == "__main__":
     test_env.run_test_cases()
```

### Comparing `oracledb-1.3.0/tests/test_4400_tpc.py` & `oracledb-1.3.1/tests/test_4400_tpc.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/tests/test_4500_connect_params.py` & `oracledb-1.3.1/tests/test_4500_connect_params.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/tests/test_4600_type_changes.py` & `oracledb-1.3.1/tests/test_4600_type_changes.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/tests/test_4700_pool_params.py` & `oracledb-1.3.1/tests/test_4700_pool_params.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/tests/test_4800_timestamp_ltz_var.py` & `oracledb-1.3.1/tests/test_4800_timestamp_ltz_var.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 class TestCase(test_env.BaseTestCase):
 
     def setUp(self):
         super().setUp()
         self.raw_data = []
         self.data_by_key = {}
         base_date = datetime.datetime(2022, 6, 2)
-        self.cursor.execute("alter session set time_zone = 'UTC'")
         for i in range(1, 11):
             if i % 4 == 0:
                 tz_hours = i
             elif i % 2 == 0:
                 tz_hours = i + 0.5
             else:
                 tz_hours = -(i + 0.5)
```

### Comparing `oracledb-1.3.0/tests/test_4900_timestamp_tz_var.py` & `oracledb-1.3.1/tests/test_4900_timestamp_tz_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/tests/test_5000_externalauth.py` & `oracledb-1.3.1/tests/test_5000_externalauth.py`

 * *Files identical despite different names*

### Comparing `oracledb-1.3.0/tests/test_env.py` & `oracledb-1.3.1/tests/test_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -395,14 +395,15 @@
             connection = self.connection
         return is_on_oracle_cloud(connection)
 
     def setUp(self):
         if self.requires_connection:
             self.connection = get_connection()
             self.cursor = self.connection.cursor()
+            self.cursor.execute("alter session set time_zone = '+00:00'")
 
     def setup_parse_count_checker(self):
         self.parse_count_info = ParseCountInfo(self.connection)
 
     def setup_round_trip_checker(self):
         self.round_trip_info = RoundTripInfo(self.connection)
```

### Comparing `oracledb-1.3.0/tox.ini` & `oracledb-1.3.1/tox.ini`

 * *Files identical despite different names*

