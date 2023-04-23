# Comparing `tmp/pyload-ng-0.5.0b3.dev54.tar.gz` & `tmp/pyload-ng-0.5.0b3.dev57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyload-ng-0.5.0b3.dev54.tar", last modified: Sat Mar 25 07:48:44 2023, max compression
+gzip compressed data, was "pyload-ng-0.5.0b3.dev57.tar", last modified: Sun Apr 23 23:23:14 2023, max compression
```

## Comparing `pyload-ng-0.5.0b3.dev54.tar` & `pyload-ng-0.5.0b3.dev57.tar`

### file list

```diff
@@ -1,862 +1,864 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.953760 pyload-ng-0.5.0b3.dev54/
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34277 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12610 2023-03-25 07:48:44.953760 pyload-ng-0.5.0b3.dev54/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10543 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/babel.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/poetry.toml
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-03-25 07:48:44.953760 pyload-ng-0.5.0b3.dev54/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.853756 pyload-ng-0.5.0b3.dev54/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.857756 pyload-ng-0.5.0b3.dev54/src/pyload/
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.857756 pyload-ng-0.5.0b3.dev54/src/pyload/core/
--rw-r--r--   0 runner    (1001) docker     (123)    16293 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.857756 pyload-ng-0.5.0b3.dev54/src/pyload/core/api/
--rw-r--r--   0 runner    (1001) docker     (123)    41788 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.857756 pyload-ng-0.5.0b3.dev54/src/pyload/core/config/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/config/default.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    12562 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/config/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.857756 pyload-ng-0.5.0b3.dev54/src/pyload/core/database/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14019 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/database/file_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/database/storage_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/database/user_database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.857756 pyload-ng-0.5.0b3.dev54/src/pyload/core/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/datatypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8365 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/datatypes/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/datatypes/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/datatypes/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7709 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/datatypes/pyfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/datatypes/pypackage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/log_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.861756 pyload-ng-0.5.0b3.dev54/src/pyload/core/managers/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/managers/account_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     9798 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/managers/addon_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/managers/captcha_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/managers/event_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    19441 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/managers/file_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    18965 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/managers/plugin_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    11705 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/managers/thread_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.861756 pyload-ng-0.5.0b3.dev54/src/pyload/core/network/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/network/browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/network/bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/network/cookie_jar.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/network/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.861756 pyload-ng-0.5.0b3.dev54/src/pyload/core/network/http/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/network/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/network/http/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13773 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/network/http/http_chunk.py
--rw-r--r--   0 runner    (1001) docker     (123)    12397 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/network/http/http_download.py
--rw-r--r--   0 runner    (1001) docker     (123)    13332 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/network/http/http_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/network/request_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.861756 pyload-ng-0.5.0b3.dev54/src/pyload/core/network/xdcc/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/network/xdcc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/network/xdcc/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.861756 pyload-ng-0.5.0b3.dev54/src/pyload/core/threads/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/threads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/threads/addon_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/threads/clicknload_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/threads/database_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/threads/decrypter_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/threads/download_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/threads/info_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/threads/plugin_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.865756 pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.865756 pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/old/
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/old/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/old/packagetools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/purge.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/seconds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.865756 pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/struct/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/struct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/struct/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/struct/info.py
--rw-r--r--   0 runner    (1001) docker     (123)    12495 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/struct/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/struct/style.py
--rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.865756 pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/web/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/web/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/web/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/web/format.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/web/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/web/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/web/purge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.865756 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.877757 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/AccioDebridCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/AlldebridCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/AniStreamCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/ArchiveOrg.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/BackinNet.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/CloudsharesNet.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/CloudsixMe.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/CloudzillaTo.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/CramitIn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/CzshareCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/DatoidCz.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/DdownloadCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/DebridItaliaCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/DebridlinkFr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/DebridplanetCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/DepositfilesCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/DownsterNet.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/EasybytezCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/EuroshareEu.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/ExashareCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/ExtmatrixCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/FastixRu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/FastshareCz.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/File4SafeCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/FileStoreTo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/FileboomMe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/FilecloudIo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/FilefactoryCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/FilejokerNet.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/FileomCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/FilerNet.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/FilerioCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/FilesMailRu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/FourSharedCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/FshareVn.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/Ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/GetTwentyFourOrg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/HellshareCz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/HighWayMe.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/Http.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/HugefilesNet.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/HundredEightyUploadCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/IronfilesNet.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/JunkyvideoCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/JunocloudMe.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/KatfileCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/Keep2ShareCc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/LeechThreeHundreedSixtyCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/LinkifierCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/LinksnappyCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/MegaCoNz.py
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/MegaDebridEu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/MegaRapidCz.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/MegaRapidoNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/MegasharesCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/MovReelCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/MultihostersCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/MultishareCz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/MyfastfileCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/NitrobitNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/NitroflareCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/NoPremiumPl.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/NosuploadCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/NovafileCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/NowVideoSx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/OneFichierCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/OpenloadCo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/OverLoadMe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/PorntrexCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/PremiumTo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/PremiumizeMe.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/PutdriveCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/QuickshareCz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/RPNetBiz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/RapideoPl.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/RapidfileshareNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/RapidgatorNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/RapiduNet.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/RarefileNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/RealdebridCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/RehostTo.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/SafesharingEu.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/SecureUploadEu.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/SendmywayCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/SharebeastCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/SimplyPremiumCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/SimplydebridCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/SmoozedCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/StreamcloudEu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/TbSevenPl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/TenluaVn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/TurbobitNet.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/TusfilesNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/TwojlimitPl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/UlozTo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/UpleaCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/UploadcCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/UploadgigCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/UploadheroCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/UpstoreNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/UptoboxCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/VidPlayNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/WebshareCz.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/WorldbytezCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/WrzucajplikiPl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/YibaishiwuCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/ZeveraCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.881757 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/AndroidPhoneNotify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/AntiCaptcha.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/AntiStandby.py
--rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/AntiVirus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/AppriseNotify.py
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/BypassCaptcha.py
--rw-r--r--   0 runner    (1001) docker     (123)    10335 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/Captcha9Kw.py
--rw-r--r--   0 runner    (1001) docker     (123)    15382 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/Checksum.py
--rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/ClickNLoad.py
--rw-r--r--   0 runner    (1001) docker     (123)    12908 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/CloudFlareDdos.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/DeathByCaptcha.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/DeleteFinished.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/DiscordNotifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/DownloadScheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/ExpertDecoders.py
--rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/ExternalScripts.py
--rw-r--r--   0 runner    (1001) docker     (123)    21628 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/ExtractArchive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/HotFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/IRC.py
--rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/ImageTyperz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/JustPremium.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/LinkFilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/LogMarker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/MergeFiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/MultiHome.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/PushBullet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/PushOver.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/RestartFailed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/SkipRev.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/TORRENT.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/TransmissionRPC.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/UnSkipOnFail.py
--rw-r--r--   0 runner    (1001) docker     (123)    14723 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/UpdateManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/UserAgentSwitcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/WindowsPhoneNotify.py
--rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/XFileSharing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/XMPP.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.885757 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/anticaptchas/
--rw-r--r--   0 runner    (1001) docker     (123)    30497 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/anticaptchas/CircleCaptcha.py
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/anticaptchas/CoinHive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/anticaptchas/HCaptcha.py
--rw-r--r--   0 runner    (1001) docker     (123)    17800 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/anticaptchas/ReCaptcha.py
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/anticaptchas/SolveMedia.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/anticaptchas/UlozTo.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/anticaptchas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.885757 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14832 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/addon.py
--rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/captcha.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/captcha_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/chat_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/dead_decrypter.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/dead_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/decrypter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16923 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)    15114 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/hoster.py
--rw-r--r--   0 runner    (1001) docker     (123)    14871 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/multi_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/multi_decrypter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/multi_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     9603 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)    12499 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/simple_decrypter.py
--rw-r--r--   0 runner    (1001) docker     (123)    17574 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/simple_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/xfs_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/xfs_decrypter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/xfs_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.889757 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/containers/
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/containers/CCF.py
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/containers/DLC.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/containers/RSDF.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/containers/TORRENT.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/containers/TXT.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/containers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.897758 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/
--rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/AlldebridComTorrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/ArchiveOrgFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/ChipDe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/CloudMailRuFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/CloudzillaToFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/CriptTo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/CryptCat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/CzshareComFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/DailymotionComFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/DataHuFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11645 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/DebridlinkFrTorrent.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/DepositfilesComFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/Dereferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/DevhostStFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/DlProtectCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/EasybytezComFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/EmbeduploadCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/FilecloudIoFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11287 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/FilecryptCc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/FilefactoryComFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/FilerNetFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/FilestubeCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/FiletramCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/FourChanOrg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/FreakhareComFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/FreetexthostCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/FshareVnFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/FurLy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/Go4UpCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/GofileIoFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/GooGl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/GoogledriveComDereferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/GoogledriveComFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/HearthisAtFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/HflixIn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/HoerbuchIn.py
--rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/ImgurCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/JDlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/LixIn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/MediafireComFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/MegaCoNzFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/MegaRapidCzFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/MegadyskPlFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/MirrorcreatorCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/MultiUpOrg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/MultiloadCz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/NitroflareComFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/NosvideoCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/PastebinCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/PastedCo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/QuickshareCzFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/RealdebridComTorrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/SafelinkingNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/SexuriaCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/ShSt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/TNTVillageScambioeticoOrg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/TenluaVnFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/TinyurlCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/TnyCz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/TurbobitNetFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/TusfilesNetFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/UlozToFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/XFileSharingFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/XupPl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/YoutubeComFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.921759 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/AccioDebridCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/AlfafileNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/AlldebridCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/AndroidfilehostCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/AnonfilesCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/ArchiveOrg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/BasketbuildCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/BayfilesCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/BezvadataCz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/ClicknuploadCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/CloudMailRu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/CloudzillaTo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/CosmoboxOrg.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/CramitIn.py
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/CzshareCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/DailymotionCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/DailyuploadsNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/DataHu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/DataportCz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/DatoidCz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/DdownloadCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/DebridItaliaCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/DebridlinkFr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/DebridplanetCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/DefaultPlugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/DepositfilesCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/DevhostSt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/DlFreeFr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/DownsterNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/DropDownload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/DropboxCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/EasybytezCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/EdiskCz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/EuroshareEu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/ExashareCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/ExtmatrixCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FastixRu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FastshareCz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FileAl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FileSharkPl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FileStoreTo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FileboomMe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FilecloudIo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FiledropperCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FilefactoryCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FilefoxCc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12929 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FilejokerNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FileomCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FilepupNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FilerNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FilerioCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FilesMailRu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FileuploadCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FileuploadNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FiregetCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FistfastNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FlyFilesNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FourSharedCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FshareVn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/Ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/GamefrontCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/GetTwentyFourOrg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/GigapetaCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/GofileIo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/GooIm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/GoogledriveCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/HearthisAt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/HellshareCz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/HighWayMe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/HitfileNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/HostujeNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/HotlinkCc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/Http.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/HugefilesNet.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/HundredEightyUploadCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/IfolderRu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/IronfilesNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/JumbofilesCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/JunocloudMe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/KatfileCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/Keep2ShareCc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/KingfilesNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/KrakenfilesCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/LeechThreeHundreedSixtyCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/LetsuploadCc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/LetsuploadCo.py
--rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/LibgenIo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/LinkifierCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/LinksnappyCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/LinksnappyComTorrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/LoadTo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/MediafireCom.py
--rw-r--r--   0 runner    (1001) docker     (123)    18129 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/MegaCoNz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/MegaDebridEu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/MegaRapidCz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/MegaRapidoNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/MegacrypterCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/MegadyskPl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/MegasharesCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/MegaupNet.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/MovReelCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/MultihostersCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/MultishareCz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/MyfastfileCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/MystoreTo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/NarodRu.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/NippyshareCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/NitrobitNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/NitroflareCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/NoPremiumPl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/NofileIo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/NosuploadCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/NovafileCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/NowVideoSx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/OneFichierCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/OnlineTvRecorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/OpenloadIo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/OverLoadMe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/PixeldrainCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/PornhostCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/PornhubCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/PornovkaCz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/PorntrexCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/PremiumTo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/PremiumizeMe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/PromptfileCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/PutdriveCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/QuickshareCz.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/RPNetBiz.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/RapideoPl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/RapidfileshareNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/RapidgatorNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/RapiduNet.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/RarefileNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/RealdebridCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/RedtubeCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/RehostTo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/RemixshareCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/RgHostNet.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/SafesharingEu.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/SecureUploadEu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/SenditCloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/SendspaceCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/Share4WebCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/ShareplaceCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/SimplyPremiumCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/SimplydebridCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/SizedriveCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/SmoozedCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/SmuleCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/SolidfilesCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/SoundcloudCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/SpeedyshareCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/StreamCz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/StreamcloudEu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/SuprafilesMe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/TbSevenPl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/TenluaVn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/TurbobitNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/TusfilesNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/TwoSharedCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/TwojlimitPl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10669 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/UlozTo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/UloziskoSk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/UnibytesCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/UpfileVn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/UpleaCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/UploadgigCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/UploadheroCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/UploadrocketNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/UploadshipCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/UpstoreNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/UptoboxCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/UserscloudCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/UseruploadNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/VeehdCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/VeohCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/VidPlayNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/VimeoCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/VkCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/WebshareCz.py
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/WetransferCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/WrzucTo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/WrzucajplikiPl.py
--rw-r--r--   0 runner    (1001) docker     (123)    36323 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/XDCC.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/XFileSharing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/XHamsterCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/XVideosCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/XdadevelopersCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/YadiSk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/YesPornPleaseCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/YibaishiwuCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/YoupornCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/YourfilesTo.py
--rw-r--r--   0 runner    (1001) docker     (123)    55150 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/YoutubeCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/ZDF.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/ZbigzCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/ZeveraCom.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/ZippyshareCom.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.921759 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/extractors/HjSplit.py
--rw-r--r--   0 runner    (1001) docker     (123)     9201 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/extractors/SevenZip.py
--rw-r--r--   0 runner    (1001) docker     (123)    10464 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/extractors/UnRar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/extractors/UnTar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/extractors/UnZip.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17225 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/plugins/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.921759 pyload-ng-0.5.0b3.dev54/src/pyload/webui/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.921759 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.925759 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/blueprints/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/blueprints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/blueprints/api_blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    14080 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/blueprints/app_blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/blueprints/cnl_blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    12181 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/blueprints/json_blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/processors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.853756 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.925759 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)    16227 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/css/base.css
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/css/logs.css
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/css/pathchooser.css
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/css/window.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.933760 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/add_folder.png
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/ajax-loader.gif
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/arrow-refresh.png
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/arrow-right.png
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/button.png
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/cog.png
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/control-add-blue.png
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/control-add.png
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/control-cancel-blue.png
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/control-cancel.png
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/control-pause-blue.png
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/control-pause.png
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/control-play-blue.png
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/control-play.png
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/control-stop-blue.png
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/control-stop.png
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/delete.png
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/dialog-close.png
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/dialog-question.png
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/error.png
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/folder.png
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/head-bg.png
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/head-login.png
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/head-menu-collector.png
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/head-menu-config.png
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/head-menu-development.png
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/head-menu-download.png
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/head-menu-home.png
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/head-menu-index.png
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/head-menu-news.png
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/head-menu-queue.png
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/head-menu-recent.png
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/head-menu-wiki.png
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/head-search-noshadow.png
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/images.png
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/notice.png
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/package-go.png
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/page-tools-backlinks.png
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/page-tools-edit.png
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/page-tools-revisions.png
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/parse-uri.png
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/pencil.png
--rw-r--r--   0 runner    (1001) docker     (123)    39315 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/pyload-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/reconnect.png
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/status-downloading.png
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/status-failed.png
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/status-finished.png
--rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/status-none.png
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/status-offline.png
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/status-proc.png
--rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/status-queue.png
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/status-waiting.png
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/success.png
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/tab-background.png
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/tabs-border-bottom.png
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/user-actions-logout.png
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/user-actions-profile.png
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/user-info.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.933760 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/js/captcha-interactive.user.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.853756 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.933760 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.933760 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/MooDialog/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Alert.js
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Confirm.js
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Error.js
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Fx.js
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.IFrame.js
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Prompt.js
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Request.js
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.js
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/MooDialog/Overlay.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.933760 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/MooDialog.css
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-close.png
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-error.png
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-question.png
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-warning.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.933760 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/MooDropMenu/
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/MooDropMenu/MooDropMenu.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.933760 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/MooDropMenu/css/
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/MooDropMenu/css/MooDropMenu.css
--rw-r--r--   0 runner    (1001) docker     (123)    89614 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/MooTools-Core.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   251703 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/MooTools-More.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.933760 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/Purr/
--rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/Purr/purr.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.933760 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/TinyTab/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/TinyTab/tinytab.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.937760 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/captcha.html
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/error.html
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/filemanager.html
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/files.html
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/folder.html
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/info.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.937760 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/js/
--rw-r--r--   0 runner    (1001) docker     (123)     6747 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/js/base.js
--rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/js/dashboard.js
--rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/js/filemanager.js
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/js/info.js
--rw-r--r--   0 runner    (1001) docker     (123)    13297 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/js/packages.js
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/js/pathchooser.js
--rw-r--r--   0 runner    (1001) docker     (123)     9042 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/js/settings.js
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/logout.html
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/logs.html
--rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/packages.html
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/pathchooser.html
--rw-r--r--   0 runner    (1001) docker     (123)    14003 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/settings.html
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/settings_item.html
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/window.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.853756 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.937760 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/info.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.853756 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.937760 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/css/base.css
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/css/dashboard.css
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/css/info.css
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/css/login.css
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/css/logout.css
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/css/logs.css
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/css/pathchooser.css
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/css/settings.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.941760 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/img/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/img/ajax-loader.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/img/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/img/pyload-banner.png
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/img/pyload-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/img/ui-icons_444444_256x240.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.853756 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.853756 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.941760 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/css/
--rw-r--r--   0 runner    (1001) docker     (123)   117150 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/css/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.941760 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 runner    (1001) docker     (123)   108738 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 runner    (1001) docker     (123)    45404 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    18028 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.941760 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/js/
--rw-r--r--   0 runner    (1001) docker     (123)    35452 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/js/bootstrap.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.941760 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/jQuery/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.941760 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.941760 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/
--rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_444444_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     7074 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_555555_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_777620_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_777777_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_cc0000_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)    16966 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/jquery-ui.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    73908 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/jquery-ui.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    86659 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jquery.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.853756 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/mdtoast/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.941760 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/mdtoast/css/
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/mdtoast/css/mdtoast.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.941760 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/mdtoast/js/
--rw-r--r--   0 runner    (1001) docker     (123)     9435 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/mdtoast/js/mdtoast.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.945760 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    12982 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/templates/captcha.html
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/templates/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/templates/error.html
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/templates/files.html
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/templates/info.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.945760 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/templates/js/
--rw-r--r--   0 runner    (1001) docker     (123)    18626 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/templates/js/base.js
--rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/templates/js/dashboard.js
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/templates/js/info.js
--rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/templates/js/packages.js
--rw-r--r--   0 runner    (1001) docker     (123)    13802 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/templates/js/settings.js
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/templates/logout.html
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/templates/logs.html
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/templates/packages.html
--rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/templates/pathchooser.html
--rw-r--r--   0 runner    (1001) docker     (123)    20067 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/templates/settings.html
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/templates/settings_item.html
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/templates/window.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.945760 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/info.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.853756 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.945760 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     9199 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/css/base.css
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/css/dashboard.css
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/css/info.css
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/css/login.css
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/css/logout.css
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/css/logs.css
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/css/pathchooser.css
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/css/settings.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.945760 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/img/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/img/ajax-loader.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/img/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/img/pyload-banner.png
--rw-r--r--   0 runner    (1001) docker     (123)     8602 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/img/pyload-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/img/ui-icons_444444_256x240.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.853756 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.853756 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.945760 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/css/
--rw-r--r--   0 runner    (1001) docker     (123)   117202 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/css/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.949760 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 runner    (1001) docker     (123)   108738 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 runner    (1001) docker     (123)    45404 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    18028 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.949760 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/js/
--rw-r--r--   0 runner    (1001) docker     (123)    35452 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/js/bootstrap.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.949760 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.949760 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.949760 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/
--rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_444444_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     7074 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_555555_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_777620_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_777777_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_cc0000_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)    16966 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/jquery-ui.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    73908 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/jquery-ui.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    86659 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jquery.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.853756 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/mdtoast/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.949760 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/mdtoast/css/
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/mdtoast/css/mdtoast.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.949760 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/mdtoast/js/
--rw-r--r--   0 runner    (1001) docker     (123)     9435 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/mdtoast/js/mdtoast.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.949760 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/templates/captcha.html
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/templates/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/templates/error.html
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/templates/files.html
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/templates/info.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.953760 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/templates/js/
--rw-r--r--   0 runner    (1001) docker     (123)    18626 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/templates/js/base.js
--rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/templates/js/dashboard.js
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/templates/js/info.js
--rw-r--r--   0 runner    (1001) docker     (123)    13329 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/templates/js/packages.js
--rw-r--r--   0 runner    (1001) docker     (123)    13265 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/templates/js/settings.js
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/templates/logout.html
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/templates/logs.html
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/templates/packages.html
--rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/templates/pathchooser.html
--rw-r--r--   0 runner    (1001) docker     (123)    20006 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/templates/settings.html
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/templates/settings_item.html
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/templates/window.html
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/src/pyload/webui/webserver_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.953760 pyload-ng-0.5.0b3.dev54/src/pyload_ng.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12610 2023-03-25 07:48:44.000000 pyload-ng-0.5.0b3.dev54/src/pyload_ng.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    36993 2023-03-25 07:48:44.000000 pyload-ng-0.5.0b3.dev54/src/pyload_ng.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 07:48:44.000000 pyload-ng-0.5.0b3.dev54/src/pyload_ng.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-25 07:48:44.000000 pyload-ng-0.5.0b3.dev54/src/pyload_ng.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 07:48:44.000000 pyload-ng-0.5.0b3.dev54/src/pyload_ng.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-03-25 07:48:44.000000 pyload-ng-0.5.0b3.dev54/src/pyload_ng.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-25 07:48:44.000000 pyload-ng-0.5.0b3.dev54/src/pyload_ng.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 07:48:44.953760 pyload-ng-0.5.0b3.dev54/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/tests/api_exerciser.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/tests/system_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/tests/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-25 07:48:40.000000 pyload-ng-0.5.0b3.dev54/tests/test_skeleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.921867 pyload-ng-0.5.0b3.dev57/
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34277 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12610 2023-04-23 23:23:14.921867 pyload-ng-0.5.0b3.dev57/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10543 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/babel.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/poetry.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-04-23 23:23:14.921867 pyload-ng-0.5.0b3.dev57/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.865868 pyload-ng-0.5.0b3.dev57/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.865868 pyload-ng-0.5.0b3.dev57/src/pyload/
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.869868 pyload-ng-0.5.0b3.dev57/src/pyload/core/
+-rw-r--r--   0 runner    (1001) docker     (123)    16485 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.869868 pyload-ng-0.5.0b3.dev57/src/pyload/core/api/
+-rw-r--r--   0 runner    (1001) docker     (123)    41788 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.869868 pyload-ng-0.5.0b3.dev57/src/pyload/core/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/config/default.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    12562 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/config/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.869868 pyload-ng-0.5.0b3.dev57/src/pyload/core/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14019 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/database/file_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/database/storage_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/database/user_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.869868 pyload-ng-0.5.0b3.dev57/src/pyload/core/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/datatypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8365 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/datatypes/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/datatypes/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/datatypes/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7709 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/datatypes/pyfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/datatypes/pypackage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/log_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.869868 pyload-ng-0.5.0b3.dev57/src/pyload/core/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/managers/account_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9798 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/managers/addon_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/managers/captcha_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/managers/event_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19441 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/managers/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18965 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/managers/plugin_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11705 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/managers/thread_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.869868 pyload-ng-0.5.0b3.dev57/src/pyload/core/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/network/browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/network/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/network/cookie_jar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/network/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.869868 pyload-ng-0.5.0b3.dev57/src/pyload/core/network/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/network/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/network/http/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13773 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/network/http/http_chunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12367 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/network/http/http_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13392 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/network/http/http_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/network/request_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.869868 pyload-ng-0.5.0b3.dev57/src/pyload/core/network/xdcc/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/network/xdcc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/network/xdcc/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.869868 pyload-ng-0.5.0b3.dev57/src/pyload/core/threads/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/threads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/threads/addon_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/threads/clicknload_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/threads/database_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/threads/decrypter_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/threads/download_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/threads/info_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/threads/plugin_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.869868 pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.873868 pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/old/
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/old/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/old/packagetools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/purge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/seconds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.873868 pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/struct/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/struct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/struct/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/struct/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12495 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/struct/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/struct/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.873868 pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/web/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/web/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/web/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/web/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/web/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/web/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/web/purge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.873868 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.881868 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/AccioDebridCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/AlldebridCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/AniStreamCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/ArchiveOrg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/BackinNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/CloudsharesNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/CloudsixMe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/CloudzillaTo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/CramitIn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/CzshareCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/DatoidCz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/DdownloadCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/DebridItaliaCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/DebridlinkFr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/DebridplanetCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/DepositfilesCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/DownsterNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/EasybytezCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/EuroshareEu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/ExashareCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/ExtmatrixCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/FastixRu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/FastshareCz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/File4SafeCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/FileStoreTo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/FileboomMe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/FilecloudIo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/FilefactoryCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/FilejokerNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/FileomCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/FilerNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/FilerioCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/FilesMailRu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/FourSharedCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/FshareVn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/Ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/GetTwentyFourOrg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/HellshareCz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/HighWayMe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/Http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/HugefilesNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/HundredEightyUploadCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/IronfilesNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/JunkyvideoCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/JunocloudMe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/KatfileCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/Keep2ShareCc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/LeechThreeHundreedSixtyCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/LinkifierCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/LinksnappyCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/MegaCoNz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/MegaDebridEu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/MegaRapidCz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/MegaRapidoNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/MegasharesCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/MovReelCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/MultihostersCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/MultishareCz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/MyfastfileCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/NitrobitNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/NitroflareCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/NoPremiumPl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/NosuploadCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/NovafileCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/NowVideoSx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/OneFichierCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/OpenloadCo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/OverLoadMe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/PorntrexCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/PremiumTo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/PremiumizeMe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/PutdriveCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/QuickshareCz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/RPNetBiz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/RapideoPl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/RapidfileshareNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/RapidgatorNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/RapiduNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/RarefileNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/RealdebridCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/RehostTo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/SafesharingEu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/SecureUploadEu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/SendmywayCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/SharebeastCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/SimplyPremiumCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/SimplydebridCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/SmoozedCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/StreamcloudEu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/TbSevenPl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/TenluaVn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/TurbobitNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/TusfilesNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/TwojlimitPl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/UlozTo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/UpleaCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/UploadcCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/UploadgigCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/UploadheroCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/UpstoreNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/UptoboxCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/VidPlayNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/WebshareCz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/WorldbytezCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/WrzucajplikiPl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/YibaishiwuCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/ZeveraCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.881868 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/AndroidPhoneNotify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/AntiCaptcha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/AntiStandby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/AntiVirus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/AppriseNotify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/BypassCaptcha.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10335 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/Captcha9Kw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15382 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/Checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/ClickNLoad.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12908 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/CloudFlareDdos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/DeathByCaptcha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/DeleteFinished.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/DiscordNotifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/DownloadScheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/ExpertDecoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/ExternalScripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21628 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/ExtractArchive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/HotFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/IRC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/ImageTyperz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/JustPremium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/LinkFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/LogMarker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/MergeFiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/MultiHome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/PushBullet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/PushOver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/RestartFailed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/SkipRev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/TORRENT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/TransmissionRPC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/UnSkipOnFail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14723 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/UpdateManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/UserAgentSwitcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/WindowsPhoneNotify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/XFileSharing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/XMPP.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.881868 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/anticaptchas/
+-rw-r--r--   0 runner    (1001) docker     (123)    30497 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/anticaptchas/CircleCaptcha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/anticaptchas/CoinHive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/anticaptchas/HCaptcha.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17858 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/anticaptchas/ReCaptcha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/anticaptchas/SolveMedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/anticaptchas/UlozTo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/anticaptchas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.885868 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14832 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/addon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/captcha.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/captcha_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/chat_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/dead_decrypter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/dead_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/decrypter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16923 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15114 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/hoster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14871 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/multi_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/multi_decrypter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/multi_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9603 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12499 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/simple_decrypter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17574 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/simple_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/xfs_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/xfs_decrypter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/xfs_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.885868 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/containers/CCF.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/containers/DLC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/containers/RSDF.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/containers/TORRENT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/containers/TXT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/containers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.889868 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/
+-rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/AlldebridComTorrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/ArchiveOrgFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/ChipDe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/CloudMailRuFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/CloudzillaToFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/CriptTo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/CryptCat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/CzshareComFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/DailymotionComFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/DataHuFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11645 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/DebridlinkFrTorrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/DepositfilesComFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/Dereferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/DevhostStFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/DlProtectCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/EasybytezComFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/EmbeduploadCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/FilecloudIoFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11287 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/FilecryptCc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/FilefactoryComFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/FilerNetFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/FilestubeCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/FiletramCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/FourChanOrg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/FreakhareComFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/FreetexthostCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/FshareVnFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/FurLy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/Go4UpCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/GofileIoFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/GooGl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/GoogledriveComDereferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/GoogledriveComFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/HearthisAtFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/HflixIn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/HoerbuchIn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/ImgurCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/JDlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/LixIn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/MediafireComFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/MegaCoNzFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/MegaRapidCzFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/MegadyskPlFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/MirrorcreatorCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/MultiUpOrg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/MultiloadCz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/NitroflareComFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/NosvideoCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/PastebinCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/PastedCo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/QuickshareCzFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/RealdebridComTorrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/SafelinkingNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/SexuriaCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/ShSt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/TNTVillageScambioeticoOrg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/TenluaVnFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/TinyurlCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/TnyCz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/TurbobitNetFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/TusfilesNetFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/UlozToFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/XFileSharingFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/XupPl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/YoutubeComFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.901867 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/AccioDebridCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/AlfafileNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/AlldebridCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/AndroidfilehostCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/AnonfilesCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/ArchiveOrg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/BasketbuildCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/BayfilesCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/BezvadataCz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/ClicknuploadCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/CloudMailRu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/CloudzillaTo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/CosmoboxOrg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/CramitIn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/CzshareCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/DailymotionCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/DailyuploadsNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/DataHu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/DataportCz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/DatoidCz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/DdownloadCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/DebridItaliaCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/DebridlinkFr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/DebridplanetCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/DefaultPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/DepositfilesCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/DevhostSt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/DlFreeFr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/DownsterNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/DropDownload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/DropboxCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/EasybytezCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/EasyuploadIo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/EdiskCz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/EuroshareEu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/ExashareCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/ExtmatrixCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FastixRu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FastshareCz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FikperCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FileAl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FileSharkPl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FileStoreTo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FileboomMe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FilecloudIo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FiledropperCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FilefactoryCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FilefoxCc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12929 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FilejokerNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FileomCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FilepupNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FilerNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FilerioCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FilesMailRu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FileuploadCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FileuploadNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FiregetCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FistfastNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FlyFilesNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FourSharedCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FshareVn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/Ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/GamefrontCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/GetTwentyFourOrg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/GigapetaCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/GofileIo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/GooIm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/GoogledriveCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/HearthisAt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/HellshareCz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/HighWayMe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/HitfileNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/HostujeNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/HotlinkCc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/Http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/HugefilesNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/HundredEightyUploadCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/IfolderRu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/IronfilesNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/JumbofilesCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/JunocloudMe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/KatfileCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/Keep2ShareCc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/KingfilesNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/KrakenfilesCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/LeechThreeHundreedSixtyCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/LetsuploadCc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/LetsuploadCo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/LibgenIo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/LinkifierCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/LinksnappyCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/LinksnappyComTorrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/LoadTo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/MediafireCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18129 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/MegaCoNz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/MegaDebridEu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/MegaRapidCz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/MegaRapidoNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/MegacrypterCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/MegadyskPl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/MegasharesCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/MegaupNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/MovReelCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/MultihostersCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/MultishareCz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/MyfastfileCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/MystoreTo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/NarodRu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/NippyshareCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/NitrobitNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/NitroflareCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/NoPremiumPl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/NofileIo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/NosuploadCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/NovafileCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/NowVideoSx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/OneFichierCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/OnlineTvRecorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/OpenloadIo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/OverLoadMe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/PixeldrainCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/PornhostCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/PornhubCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/PornovkaCz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/PorntrexCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/PremiumTo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/PremiumizeMe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/PromptfileCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/PutdriveCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/QuickshareCz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/RPNetBiz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/RapideoPl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/RapidfileshareNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/RapidgatorNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/RapiduNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/RarefileNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/RealdebridCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/RedtubeCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/RehostTo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/RemixshareCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/RgHostNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/SafesharingEu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/SecureUploadEu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/SenditCloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/SendspaceCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/Share4WebCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/ShareplaceCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/SimplyPremiumCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/SimplydebridCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/SizedriveCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/SmoozedCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/SmuleCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/SolidfilesCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/SoundcloudCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/SpeedyshareCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/StreamCz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/StreamcloudEu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/SuprafilesMe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/TbSevenPl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/TenluaVn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/TurbobitNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/TusfilesNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/TwoSharedCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/TwojlimitPl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10669 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/UlozTo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/UloziskoSk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/UnibytesCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/UpfileVn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/UpleaCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/UploadgigCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/UploadheroCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/UploadrocketNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/UploadshipCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/UpstoreNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/UptoboxCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/UserscloudCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/UseruploadNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/VeehdCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/VeohCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/VidPlayNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/VimeoCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/VkCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/WebshareCz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/WetransferCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/WrzucTo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/WrzucajplikiPl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36323 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/XDCC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/XFileSharing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/XHamsterCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/XVideosCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/XdadevelopersCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/YadiSk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/YesPornPleaseCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/YibaishiwuCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/YoupornCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/YourfilesTo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55150 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/YoutubeCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/ZDF.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/ZbigzCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/ZeveraCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/ZippyshareCom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.905868 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/extractors/HjSplit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9201 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/extractors/SevenZip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10464 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/extractors/UnRar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/extractors/UnTar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/extractors/UnZip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17225 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/plugins/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.905868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.905868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.905868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/blueprints/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/blueprints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/blueprints/api_blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14080 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/blueprints/app_blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/blueprints/cnl_blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12181 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/blueprints/json_blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/processors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.865868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.905868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    16227 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/css/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/css/logs.css
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/css/pathchooser.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/css/window.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.909868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/add_folder.png
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/ajax-loader.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/arrow-refresh.png
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/arrow-right.png
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/button.png
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/cog.png
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/control-add-blue.png
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/control-add.png
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/control-cancel-blue.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/control-cancel.png
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/control-pause-blue.png
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/control-pause.png
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/control-play-blue.png
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/control-play.png
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/control-stop-blue.png
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/control-stop.png
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/delete.png
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/dialog-close.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/dialog-question.png
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/error.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/folder.png
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/head-bg.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/head-login.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/head-menu-collector.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/head-menu-config.png
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/head-menu-development.png
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/head-menu-download.png
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/head-menu-home.png
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/head-menu-index.png
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/head-menu-news.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/head-menu-queue.png
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/head-menu-recent.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/head-menu-wiki.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/head-search-noshadow.png
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/images.png
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/notice.png
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/package-go.png
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/page-tools-backlinks.png
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/page-tools-edit.png
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/page-tools-revisions.png
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/parse-uri.png
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/pencil.png
+-rw-r--r--   0 runner    (1001) docker     (123)    39315 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/pyload-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/reconnect.png
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/status-downloading.png
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/status-failed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/status-finished.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/status-none.png
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/status-offline.png
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/status-proc.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/status-queue.png
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/status-waiting.png
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/success.png
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/tab-background.png
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/tabs-border-bottom.png
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/user-actions-logout.png
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/user-actions-profile.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/user-info.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.909868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/js/captcha-interactive.user.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.865868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.909868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.909868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/MooDialog/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Alert.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Confirm.js
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Error.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Fx.js
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.IFrame.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Prompt.js
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Request.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/MooDialog/Overlay.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.909868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/MooDialog.css
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-close.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-error.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-question.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-warning.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.909868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/MooDropMenu/
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/MooDropMenu/MooDropMenu.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.909868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/MooDropMenu/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/MooDropMenu/css/MooDropMenu.css
+-rw-r--r--   0 runner    (1001) docker     (123)    89614 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/MooTools-Core.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   251703 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/MooTools-More.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.909868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/Purr/
+-rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/Purr/purr.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.909868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/TinyTab/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/TinyTab/tinytab.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.913868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/captcha.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/error.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/filemanager.html
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/files.html
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/folder.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/info.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.913868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     6747 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/js/base.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/js/dashboard.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/js/filemanager.js
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/js/info.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13297 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/js/packages.js
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/js/pathchooser.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9042 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/js/settings.js
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/logout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/logs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/packages.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/pathchooser.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14003 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/settings.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/settings_item.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/window.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.865868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.913868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/info.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.865868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.913868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/css/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/css/dashboard.css
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/css/info.css
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/css/login.css
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/css/logout.css
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/css/logs.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/css/pathchooser.css
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/css/settings.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.913868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/img/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/img/ajax-loader.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/img/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/img/pyload-banner.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/img/pyload-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/img/ui-icons_444444_256x240.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.865868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.865868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.913868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   117150 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/css/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.913868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   108738 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45404 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    18028 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.913868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    35452 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/js/bootstrap.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.913868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/jQuery/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.913868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.913868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_444444_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7074 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_555555_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_777620_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_777777_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_cc0000_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16966 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/jquery-ui.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    73908 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/jquery-ui.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    86659 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jquery.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.865868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/mdtoast/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.913868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/mdtoast/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/mdtoast/css/mdtoast.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.913868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/mdtoast/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     9435 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/mdtoast/js/mdtoast.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.917868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    12982 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/templates/captcha.html
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/templates/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/templates/error.html
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/templates/files.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/templates/info.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.917868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/templates/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    18811 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/templates/js/base.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/templates/js/dashboard.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/templates/js/info.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/templates/js/packages.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13802 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/templates/js/settings.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/templates/logout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/templates/logs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/templates/packages.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/templates/pathchooser.html
+-rw-r--r--   0 runner    (1001) docker     (123)    20067 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/templates/settings.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/templates/settings_item.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/templates/window.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.917868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/info.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.865868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.917868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     9199 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/css/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/css/dashboard.css
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/css/info.css
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/css/login.css
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/css/logout.css
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/css/logs.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/css/pathchooser.css
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/css/settings.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.917868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/img/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/img/ajax-loader.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/img/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/img/pyload-banner.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8602 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/img/pyload-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/img/ui-icons_444444_256x240.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.865868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.865868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.917868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   117202 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/css/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.917868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   108738 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45404 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    18028 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.917868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    35452 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/js/bootstrap.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.917868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.917868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.917868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_444444_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7074 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_555555_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_777620_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_777777_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_cc0000_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16966 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/jquery-ui.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    73908 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/jquery-ui.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    86659 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jquery.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.865868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/mdtoast/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.917868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/mdtoast/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/mdtoast/css/mdtoast.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.917868 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/mdtoast/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     9435 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/mdtoast/js/mdtoast.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.921867 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/templates/captcha.html
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/templates/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/templates/error.html
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/templates/files.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/templates/info.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.921867 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/templates/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    18811 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/templates/js/base.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/templates/js/dashboard.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/templates/js/info.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13329 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/templates/js/packages.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13265 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/templates/js/settings.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/templates/logout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/templates/logs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/templates/packages.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/templates/pathchooser.html
+-rw-r--r--   0 runner    (1001) docker     (123)    20006 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/templates/settings.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/templates/settings_item.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/templates/window.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/src/pyload/webui/webserver_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.921867 pyload-ng-0.5.0b3.dev57/src/pyload_ng.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12610 2023-04-23 23:23:14.000000 pyload-ng-0.5.0b3.dev57/src/pyload_ng.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    37084 2023-04-23 23:23:14.000000 pyload-ng-0.5.0b3.dev57/src/pyload_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 23:23:14.000000 pyload-ng-0.5.0b3.dev57/src/pyload_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-23 23:23:14.000000 pyload-ng-0.5.0b3.dev57/src/pyload_ng.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 23:23:14.000000 pyload-ng-0.5.0b3.dev57/src/pyload_ng.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-23 23:23:14.000000 pyload-ng-0.5.0b3.dev57/src/pyload_ng.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 23:23:14.000000 pyload-ng-0.5.0b3.dev57/src/pyload_ng.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:23:14.921867 pyload-ng-0.5.0b3.dev57/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/tests/api_exerciser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/tests/system_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/tests/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-23 23:23:09.000000 pyload-ng-0.5.0b3.dev57/tests/test_skeleton.py
```

### Comparing `pyload-ng-0.5.0b3.dev54/AUTHORS.md` & `pyload-ng-0.5.0b3.dev57/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/CODE_OF_CONDUCT.md` & `pyload-ng-0.5.0b3.dev57/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/CONTRIBUTING.md` & `pyload-ng-0.5.0b3.dev57/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/LICENSE.md` & `pyload-ng-0.5.0b3.dev57/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/PKG-INFO` & `pyload-ng-0.5.0b3.dev57/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyload-ng
-Version: 0.5.0b3.dev54
+Version: 0.5.0b3.dev57
 Summary: The free and open-source Download Manager written in pure Python
 Home-page: https://pyload.net
 Download-URL: https://github.com/pyload/pyload/releases
 Author: pyLoad team
 Author-email: support@pyload.net
 Maintainer: Walter Purcaro
 Maintainer-email: vuolter@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyload-ng Version: 0.5.0b3.dev54 Summary: The free
+Metadata-Version: 2.1 Name: pyload-ng Version: 0.5.0b3.dev57 Summary: The free
 and open-source Download Manager written in pure Python Home-page: https://
 pyload.net Download-URL: https://github.com/pyload/pyload/releases Author:
 pyLoad team Author-email: support@pyload.net Maintainer: Walter Purcaro
 Maintainer-email: vuolter@gmail.com License: agpl3 Project-URL: Source Code
 (mirror), https://gitlab.com/pyload/pyload Project-URL: Source Code, https://
 github.com/pyload/pyload Project-URL: Bug Tracker, https://github.com/pyload/
 pyload/issues Project-URL: Documentation, https://github.com/pyload/pyload/wiki
```

### Comparing `pyload-ng-0.5.0b3.dev54/README.md` & `pyload-ng-0.5.0b3.dev57/README.md`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/SECURITY.md` & `pyload-ng-0.5.0b3.dev57/SECURITY.md`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/pyproject.toml` & `pyload-ng-0.5.0b3.dev57/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/setup.cfg` & `pyload-ng-0.5.0b3.dev57/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/setup.py` & `pyload-ng-0.5.0b3.dev57/setup.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/__init__.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/__init__.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/__main__.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/__main__.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/__init__.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,18 +191,17 @@
             )
 
     def _init_managers(self):
         from .managers.account_manager import AccountManager
         from .managers.addon_manager import AddonManager
         from .managers.captcha_manager import CaptchaManager
         from .managers.event_manager import EventManager
+        from .managers.file_manager import FileManager
         from .managers.plugin_manager import PluginManager
         from .managers.thread_manager import ThreadManager
-        from .managers.file_manager import FileManager
-
         from .scheduler import Scheduler
 
         self.files = self.file_manager = FileManager(self)
         self.scheduler = Scheduler(self)
 
         self.pgm = self.plugin_manager = PluginManager(self)
         self.evm = self.event_manager = EventManager(self)
@@ -365,14 +364,15 @@
     #     except Exception as exc:
     #         self.log.debug(exc, exc_info=self.debug > 1, stack_info=self.debug > 2)
 
     def start(self):
         try:
             try:
                 signal.signal(signal.SIGQUIT, self.sigquit)
+                signal.signal(signal.SIGTERM, self.sigterm)
             except Exception:
                 pass
 
             self.log.debug("Starting core...")
 
             if self.debug:
                 debug_level = reversemap(self.DEBUG_LEVEL_MAP)[self.debug].upper()
@@ -459,14 +459,19 @@
         sys.exit()
 
     def sigquit(self, a, b):
         self.log.info(self._("Received Quit signal"))
         self.terminate()
         sys.exit()
 
+    def sigterm(self, a, b):
+        self.log.info(self._("Received Terminate signal"))
+        self.terminate()
+        sys.exit()
+
     def terminate(self):
         if self.running:
             self.stop()
             self.log.info(self._("Exiting core..."))
             # self.tsm.exit()
             # self.db.exit()  # NOTE: Why here?
             self.logfactory.shutdown()
```

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/api/__init__.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/config/default.cfg` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/config/default.cfg`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/config/parser.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/config/parser.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/database/__init__.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/database/__init__.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/database/file_database.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/database/file_database.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/database/storage_database.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/database/storage_database.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/database/user_database.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/database/user_database.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/datatypes/data.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/datatypes/data.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/datatypes/enums.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/datatypes/enums.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/datatypes/exceptions.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/datatypes/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/datatypes/pyfile.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/datatypes/pyfile.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/datatypes/pypackage.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/datatypes/pypackage.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/log_factory.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/log_factory.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/managers/account_manager.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/managers/account_manager.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/managers/addon_manager.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/managers/addon_manager.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/managers/captcha_manager.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/managers/captcha_manager.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/managers/event_manager.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/managers/event_manager.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/managers/file_manager.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/managers/file_manager.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/managers/plugin_manager.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/managers/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/managers/thread_manager.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/managers/thread_manager.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/network/browser.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/network/browser.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/network/bucket.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/network/bucket.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/network/cookie_jar.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/network/cookie_jar.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/network/http/exceptions.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/network/http/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/network/http/http_chunk.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/network/http/http_chunk.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/network/http/http_download.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/network/http/http_download.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,23 +59,23 @@
             self.info = ChunkInfo(filename)
 
         self.chunk_support = None
         self.m = self.manager = pycurl.CurlMulti()
 
         #: needed for speed calculation
         self.last_arrived = []
-        self.last_speeds = [0, 0]
+        self.last_speeds = []
 
         #: notifications callback
         self.status_notify = status_notify
 
     @property
     def speed(self):
-        speeds = [sum(x) for x in self.last_speeds if x]
-        return sum(speeds) // len(speeds)  #: average
+        #: bytes per second
+        return sum(self.last_speeds) // len(self.last_speeds)  #: average
 
     @property
     def arrived(self):
         return sum(c.arrived for c in self.chunks)
 
     @property
     def percent(self):
@@ -215,30 +215,29 @@
 
             #: reduce these calls
             while last_finish_check + 0.5 < t:
                 #: list of failed curl handles
                 failed = []
                 ex = None  #: save only last exception, we can only raise one anyway
 
-                num_q, ok_list, err_list = self.m.info_read()
+                num_queued, ok_list, err_list = self.m.info_read()
                 for c in ok_list:
                     chunk = self.find_chunk(c)
                     try:  #: check if the header implies success, else add it to failed list
                         chunk.verify_header()
                     except BadHeader as exc:
                         self.log.debug(f"Chunk {chunk.id + 1} failed: {exc}")
                         failed.append(chunk)
                         ex = exc
                     else:
                         self.log.debug(f"Chunk {chunk.id + 1} download finished")
                         chunks_done.add(c)
 
-                for c in err_list:
-                    curl, errno, msg = c
-                    chunk = self.find_chunk(curl)
+                for c, errno, msg in err_list:
+                    chunk = self.find_chunk(c)
                     #: test if chunk was finished
                     if errno != pycurl.E_WRITE_ERROR or not chunk.aborted:
                         failed.append(chunk)
                         ex = pycurl.error(errno, msg)
                         self.log.debug(f"Chunk {chunk.id + 1} failed: {ex}")
                         continue
 
@@ -246,18 +245,18 @@
                         chunk.verify_header()
                     except BadHeader as exc:
                         self.log.debug(f"Chunk {chunk.id + 1} failed: {exc}")
                         failed.append(chunk)
                         ex = exc
                     else:
                         self.log.debug(f"Chunk {chunk.id + 1} download finished")
-                        chunks_done.add(curl)
-                if not num_q:  #: no more infos to get
+                        chunks_done.add(c)
+                if not num_queued:  #: no more infos to get
 
-                    #: check if init is not finished so we reset download connections
+                    #: check if init is not finished, so we reset download connections
                     #: note that other chunks are closed and downloaded with init too
                     if failed and init not in failed and init.c not in chunks_done:
                         self.log.error(
                             f"Download chunks failed, fallback to single connection | {ex}"
                         )
 
                         #: list of chunks to clean and os.remove
@@ -287,20 +286,20 @@
                     break
 
             if done:
                 break  #: all chunks loaded
 
             #: calc speed once per second, averaging over 3 seconds
             if last_time_check + 1 < t:
-                arrived_delta = [
+                arrived_delta = (
                     chunk.arrived - (self.last_arrived[i] if len(self.last_arrived) > i else 0)
                     for i, chunk in enumerate(self.chunks)
-                ]
+                )
                 self.last_speeds = [
-                    list(float(a) / (t - last_time_check) for a in arrived_delta)
+                    sum(float(delta) / (t - last_time_check) for delta in arrived_delta)
                 ] + self.last_speeds[:2]
 
                 self.last_arrived = [c.arrived for c in self.chunks]
                 last_time_check = t
                 self.update_progress()
 
             if self.abort:
```

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/network/http/http_request.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/network/http/http_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 import mimetypes
 import os
 from itertools import chain
 from logging import getLogger
 from urllib.parse import quote, urlencode
 
 import certifi
-
 import pycurl
+
 from pyload import APPID
 
+from ...utils.check import is_mapping
 from ...utils.convert import to_bytes, to_str
 from ..exceptions import Abort
 from .exceptions import BadHeader
 
 if not hasattr(pycurl, "PROXYTYPE_HTTPS"):
     pycurl.PROXYTYPE_HTTPS = 2
 
@@ -227,21 +228,23 @@
         self.c.setopt(pycurl.URL, url)
         self.c.last_url = url
 
         if post:
             self.c.setopt(pycurl.POST, 1)
             if not multipart:
                 if post is True:
-                    pass
+                    post = b""
                 elif isinstance(post, str):
                     post = post.encode()
-                    self.c.setopt(pycurl.POSTFIELDS, post)
-                else:  # TODO: check if mapping
+                elif is_mapping(post):
                     post = myurlencode(post)
-                    self.c.setopt(pycurl.POSTFIELDS, post)
+                else:
+                    raise ValueError("Invalid value for 'post'")
+
+                self.c.setopt(pycurl.POSTFIELDS, post)
 
             else:
                 multipart_post = []
                 for k, v in post.items():
                     if isinstance(v, (str, bool, int)):
                         multipart_post.append((k, to_str(v)))
```

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/network/request_factory.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/network/request_factory.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/network/xdcc/request.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/network/xdcc/request.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/scheduler.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/scheduler.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/threads/addon_thread.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/threads/addon_thread.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/threads/clicknload_thread.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/threads/clicknload_thread.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/threads/database_thread.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/threads/database_thread.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/threads/decrypter_thread.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/threads/decrypter_thread.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/threads/download_thread.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/threads/download_thread.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/threads/info_thread.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/threads/info_thread.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/threads/plugin_thread.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/threads/plugin_thread.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/check.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/check.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 # -*- coding: utf-8 -*-
 
 import imp
 from collections.abc import Iterable, Mapping
 
 
-def bitset(bits, bset):
-    """Checks if all bits are set in bset or bits is zero."""
-    return bits == (bits & bset)
+def is_bits_set(value, bits):
+    """Checks if all bits are set in value or some bits are zero."""
+    return bits == (value & bits)
 
 
 def cmp(x, y):
     """Compare the two objects x and y and return an integer according to the
     outcome."""
     return (x > y) - (x < y)
 
 
-def hasmethod(obj, name):
+def has_method(obj, name):
     """Check if method `name` was defined in obj."""
     return callable(getattr(obj, name, None))
 
 
-def haspropriety(obj, name):
+def has_propriety(obj, name):
     """Check if propriety `name` was defined in obj."""
     attr = getattr(obj, name, None)
     return attr and not callable(attr)
 
 
 def methods(obj):
     """List all the methods declared in obj."""
-    return [name for name in dir(obj) if hasmethod(obj, name)]
+    return [name for name in dir(obj) if has_method(obj, name)]
 
 
 def proprieties(obj):
     """List all the propriety attribute declared in obj."""
-    return [name for name in dir(obj) if haspropriety(obj, name)]
+    return [name for name in dir(obj) if has_propriety(obj, name)]
 
 
 def is_iterable(obj, strict=False):
     """Check if object is iterable (`<type 'str'>` excluded if
     strict=False)."""
     return isinstance(obj, Iterable) and (
         strict or not isinstance(obj, str) or not isinstance(obj, bytes)
@@ -57,12 +57,13 @@
             fp.close()
         return True
     except ImportError:
         return False
 
 
 def missing(iterable, start=None, end=None):
+    """List all the values between 'start' and 'stop' that are missing from 'iterable'."""
     iter_seq = set(map(int, iterable))
     min_val = start or min(iter_seq)
     max_val = end or max(iter_seq)
     full_seq = set(range(min_val, max_val + 1))
     return sorted(full_seq - iter_seq)
```

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/convert.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/convert.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/debug.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/debug.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/format.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/format.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/fs.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/fs.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/misc.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/misc.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/old/__init__.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/old/__init__.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/old/packagetools.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/old/packagetools.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/parse.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/parse.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/purge.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/purge.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/seconds.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/seconds.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/struct/base.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/struct/base.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/struct/info.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/struct/info.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/struct/lock.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/struct/lock.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/struct/style.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/struct/style.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/system.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/system.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/web/check.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/web/check.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/web/convert.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/web/convert.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/web/format.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/web/format.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/web/parse.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/web/parse.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/core/utils/web/purge.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/core/utils/web/purge.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/AccioDebridCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/AccioDebridCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/AlldebridCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/AlldebridCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/ArchiveOrg.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/ArchiveOrg.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/CloudzillaTo.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/CloudzillaTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/CzshareCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/CzshareCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/DatoidCz.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/DatoidCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/DdownloadCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/DdownloadCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/DebridItaliaCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/DebridItaliaCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/DebridlinkFr.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/DebridlinkFr.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/DebridplanetCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/DebridplanetCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/DepositfilesCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/DepositfilesCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/DownsterNet.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/DownsterNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/EuroshareEu.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/EuroshareEu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/ExtmatrixCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/ExtmatrixCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/FastixRu.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/FastixRu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/FastshareCz.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/FastshareCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/FileStoreTo.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/FileStoreTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/FileboomMe.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/FileboomMe.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/FilecloudIo.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/FilecloudIo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/FilefactoryCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/FilefactoryCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/FilejokerNet.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/FilejokerNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/FilerNet.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/FilerNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/FilesMailRu.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/FilesMailRu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/FourSharedCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/FourSharedCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/FshareVn.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/FshareVn.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/GetTwentyFourOrg.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/GetTwentyFourOrg.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/HellshareCz.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/HellshareCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/HighWayMe.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/HighWayMe.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/IronfilesNet.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/IronfilesNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/KatfileCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/KatfileCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/Keep2ShareCc.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/Keep2ShareCc.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/LeechThreeHundreedSixtyCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/LeechThreeHundreedSixtyCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/LinkifierCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/LinkifierCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/LinksnappyCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/LinksnappyCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/MegaCoNz.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/MegaCoNz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/MegaDebridEu.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/MegaDebridEu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/MegaRapidCz.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/MegaRapidCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/MegaRapidoNet.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/MegaRapidoNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/MegasharesCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/MegasharesCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/MultishareCz.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/MultishareCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/MyfastfileCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/MyfastfileCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/NitrobitNet.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/NitrobitNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/NitroflareCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/NitroflareCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/NoPremiumPl.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/NoPremiumPl.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/NowVideoSx.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/NowVideoSx.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/OneFichierCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/OneFichierCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/OverLoadMe.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/OverLoadMe.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/PorntrexCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/PorntrexCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/PremiumTo.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/PremiumTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/PremiumizeMe.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/PremiumizeMe.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/QuickshareCz.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/QuickshareCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/RPNetBiz.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/RPNetBiz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/RapideoPl.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/RapideoPl.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/RapidfileshareNet.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/RapidfileshareNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/RapidgatorNet.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/RapidgatorNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/RapiduNet.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/RapiduNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/RealdebridCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/RealdebridCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/RehostTo.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/RehostTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/SimplyPremiumCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/SimplyPremiumCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/SimplydebridCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/SimplydebridCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/SmoozedCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/SmoozedCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/TbSevenPl.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/TbSevenPl.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/TenluaVn.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/TenluaVn.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/TurbobitNet.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/TurbobitNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/TusfilesNet.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/TusfilesNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/TwojlimitPl.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/TwojlimitPl.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/UlozTo.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/UlozTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/UpleaCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/UpleaCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/UploadgigCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/UploadgigCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/UploadheroCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/UploadheroCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/UpstoreNet.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/UpstoreNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/UptoboxCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/UptoboxCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/WebshareCz.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/WebshareCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/WrzucajplikiPl.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/WrzucajplikiPl.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/YibaishiwuCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/YibaishiwuCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/accounts/ZeveraCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/accounts/ZeveraCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/AndroidPhoneNotify.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/AndroidPhoneNotify.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/AntiCaptcha.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/AntiCaptcha.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/AntiStandby.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/AntiStandby.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/AntiVirus.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/AntiVirus.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/AppriseNotify.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/AppriseNotify.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/BypassCaptcha.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/BypassCaptcha.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/Captcha9Kw.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/Captcha9Kw.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/Checksum.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/Checksum.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/ClickNLoad.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/ClickNLoad.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/CloudFlareDdos.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/CloudFlareDdos.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/DeathByCaptcha.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/DeathByCaptcha.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/DeleteFinished.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/DeleteFinished.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/DiscordNotifier.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/DiscordNotifier.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/DownloadScheduler.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/DownloadScheduler.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/ExpertDecoders.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/ExpertDecoders.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/ExternalScripts.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/ExternalScripts.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/ExtractArchive.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/ExtractArchive.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/HotFolder.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/HotFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/IRC.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/IRC.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/ImageTyperz.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/ImageTyperz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/JustPremium.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/JustPremium.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/LinkFilter.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/LinkFilter.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/LogMarker.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/LogMarker.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/MergeFiles.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/MergeFiles.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/MultiHome.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/MultiHome.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/PushBullet.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/PushBullet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/PushOver.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/PushOver.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/RestartFailed.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/RestartFailed.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/SkipRev.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/SkipRev.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/TORRENT.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/TORRENT.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/TransmissionRPC.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/TransmissionRPC.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/UnSkipOnFail.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/UnSkipOnFail.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/UpdateManager.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/UpdateManager.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/UserAgentSwitcher.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/UserAgentSwitcher.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/WindowsPhoneNotify.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/WindowsPhoneNotify.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/XFileSharing.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/XFileSharing.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/addons/XMPP.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/addons/XMPP.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/anticaptchas/CircleCaptcha.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/anticaptchas/CircleCaptcha.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/anticaptchas/CoinHive.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/anticaptchas/CoinHive.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/anticaptchas/HCaptcha.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/anticaptchas/HCaptcha.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/anticaptchas/ReCaptcha.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/anticaptchas/ReCaptcha.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from ..base.captcha_service import CaptchaService
 
 
 class ReCaptcha(CaptchaService):
     __name__ = "ReCaptcha"
     __type__ = "anticaptcha"
-    __version__ = '0.48'
+    __version__ = '0.50'
     __status__ = "testing"
 
     __description__ = "ReCaptcha captcha service plugin"
     __license__ = "GPLv3"
     __authors__ = [
         ("Walter Purcaro", "vuolter@gmail.com"),
         ("zapp-brannigan", "fuerst.reinje@web.de"),
@@ -29,21 +29,21 @@
     ]
 
     KEY_V2_PATTERN = r'(?:data-sitekey=["\']|["\']sitekey["\']\s*:\s*["\'])((?:[\w\-]|%[0-9a-fA-F]{2})+)'
     KEY_FORMAT_V2_PATTERN = r'^6L[\w-]{6}AAAAA[\w-]{27}$'
     INVISIBLE_V2_PATTERN = r'data-size\s*=\s*(["\'])\s*invisible\s*\1'
     STOKEN_V2_PATTERN = r'data-stoken=["\']([\w\-]+)'
 
-    RECAPTCHA_INTERACTIVE_SIG = "7b99386315b3e035285946b842049575fc69a88ccc219e1bc96a9afd0f3c4b7456f09d36bf3dc530" + \
-                                "a08cd50f1b3128716cf727b30f7de4ab1513f15bb82776e84404089a764c6305d9c6033c99f8514e" + \
-                                "249bc3fd5530b475c00059797ce5a45d131adb626a440366af9acc9a50a3a7327b9d3dc28b59f83f" + \
-                                "32129feb89e0cfb74521c306e8ac0b9fff9df31d453eedc54a17d41528c2d866363fc13cb524ad77" + \
-                                "60483b28bf4a347de4a8b2b1480f83f66c4408ad9dbfec78f6f1525b8507b6e52cdd13e13f8e3bfc" + \
-                                "0bb5dd1860e6fc5db99ef0c915fd626c3aaec0bb5ead3a668ebb31dd2a08eacaefffdf51e3a0ba31" + \
-                                "cb636da134c24633f2b2b38f56dfbb92"
+    RECAPTCHA_INTERACTIVE_SIG = "661a94a7eeb590d8d0f20d8d6e7aefa474918af01cc573da7101bc53df6ebd4ccf62df44c0bf3171" + \
+                                "fa389cf9ed8e9bb9b684621e2a1d1a3bd5bd1d5450ba5350d26f63c119477fcc3f53c5a4e784a5b9" + \
+                                "7a013cbc4e802325df4a693de112bc8fe72e8d64ec6e14d14b907290c0db04e139283733a7981daf" + \
+                                "b05a00785d1ed32c9dcd2ae9aa10f2c058ecb7667c3d000adfc1372d6a161e348ba1170e4211737f" + \
+                                "1f54518bf9f50197bba1bb336ceb17be220245f1554dfad7af1e2b996d65419d259e98a1f468dfc2" + \
+                                "ce492fa359f7489184786ea9d02f595101910d711d2c93978a81e9a573a27720f2e81c5d636b2483" + \
+                                "0c85257db01aeaf58474b00190fb702f"
 
     RECAPTCHA_INTERACTIVE_JS = """
 			while(document.children[0].childElementCount > 0) {
 				document.children[0].removeChild(document.children[0].children[0]);
 			}
 			document.children[0].innerHTML = '<html><head></head><body style="display:inline-block;"><div id="captchadiv" style="display: inline-block;"></div></body></html>';
 
@@ -80,31 +80,32 @@
 						var recaptchaResponse = grecaptcha.getResponse(); // get captcha response
 						gpyload.submitResponse(recaptchaResponse);
 					 }}
 				);
 				gpyload.activated();
 			};
 
+			delete window.grecaptcha;
 			if(typeof grecaptcha !== 'undefined' && grecaptcha) {
 				window.pyloadCaptchaOnLoadCallback();
 			} else {
 				var js_script = document.createElement('script');
 				js_script.type = "text/javascript";
 				js_script.src = "//www.google.com/recaptcha/api.js?onload=pyloadCaptchaOnLoadCallback&render=explicit";
 				js_script.async = true;
 				document.getElementsByTagName('head')[0].appendChild(js_script);
 			}"""
 
-    RECAPTCHA_INVISIBLE_SIG = "7a51902e14a4afd9cd6f09e6e4dab3ec7c44f3d901693e9fcd06ff915decfb942e60fc18752cfe72" + \
-                              "5a6e0017e26bab86d385cab9f3ebf49a7b3c1791bdde5754790852b695d28b4b304e7f14948c87f7" + \
-                              "6962fed3d18ed02e69d4f90aaa8f41b0e760355815220baeb9f696fa4ebde41ffb64cbdf774a84b5" + \
-                              "5e48e87eebea2237a9d196fe6bb2ecdf5e369581398ed489b1bc571cdae84d4724b4d7f7ab8f6e70" + \
-                              "a17cd0f85b4eca338c07b34b13bdf18242abd0dd7d0b85257013a5267af98381157eb855ee145506" + \
-                              "6759e37feee3e64cab997c0ed12063b2a00bd8ebc34d898463d97540d2538e41be1946e94202b445" + \
-                              "99c646544f79711f5ee1ee03a9b816b1"
+    RECAPTCHA_INVISIBLE_SIG = "6c6fb9970fdeac68b95809ce45a344f1225d2284e2c08507261f3506dbeebe9f0e1d9040df64191e" + \
+                              "938f578b52009c31d0da920e1a9616d73ff7b7eb1e964477fac169e412fd1e325992c1783c4664e8" + \
+                              "ba207986af12939fcc50bed642f8c26136cc8656a22be2fc51651437d1e0d356ae19a8c33d569f4d" + \
+                              "7d11d3d794a074caf06f58bd2e2e339d31968967ad78c955ea36c707a8524ba3933509525a22e3ba" + \
+                              "56ad3e71770700e6a1d18158db33f65f47d6558f16d2db5c75ab8b1be8595846a27f4aa514a98d7c" + \
+                              "b13d6a557a1273ca5a06b1251f7481d787e3eca77523a8733be179318f46baaa1d99112daaf08c4f" + \
+                              "86e067931f593c0f1941d9a8414fa1a4"
 
     RECAPTCHA_INVISIBLE_JS = """
 			while(document.children[0].childElementCount > 0) {
 				document.children[0].removeChild(document.children[0].children[0]);
 			}
 			document.children[0].innerHTML = '<html><head></head><body style="display:inline-block;"><div id="captchadiv" style="display: inline-block;"></div></body></html>';
 
@@ -119,14 +120,15 @@
 						var recaptchaResponse = grecaptcha.getResponse(); // get captcha response
 						gpyload.submitResponse(recaptchaResponse);
 					 }}
 				);
 				grecaptcha.execute();
 			};
 
+			delete window.grecaptcha;
 			if(typeof grecaptcha !== 'undefined' && grecaptcha) {
 				window.pyloadCaptchaOnLoadCallback();
 			} else {
 				var js_script = document.createElement('script');
 				js_script.type = "text/javascript";
 				js_script.src = "//www.google.com/recaptcha/api.js?onload=pyloadCaptchaOnLoadCallback&render=explicit";
 				js_script.async = true;
```

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/anticaptchas/SolveMedia.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/anticaptchas/SolveMedia.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/anticaptchas/UlozTo.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/anticaptchas/UlozTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/account.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/account.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/addon.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/addon.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/captcha.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/captcha.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/captcha_service.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/captcha_service.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/chat_bot.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/chat_bot.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/container.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/container.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/dead_decrypter.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/dead_decrypter.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/dead_downloader.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/dead_downloader.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/decrypter.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/decrypter.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/downloader.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/downloader.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/extractor.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/extractor.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/hoster.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/hoster.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/multi_account.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/multi_account.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/multi_decrypter.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/multi_decrypter.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/multi_downloader.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/multi_downloader.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/notifier.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/notifier.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/ocr.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/ocr.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/plugin.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/plugin.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/simple_decrypter.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/simple_decrypter.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/simple_downloader.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/simple_downloader.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/xfs_account.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/xfs_account.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/xfs_decrypter.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/xfs_decrypter.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/base/xfs_downloader.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/base/xfs_downloader.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/containers/CCF.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/containers/CCF.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/containers/DLC.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/containers/DLC.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/containers/RSDF.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/containers/RSDF.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/containers/TORRENT.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/containers/TORRENT.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/containers/TXT.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/containers/TXT.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/AlldebridComTorrent.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/AlldebridComTorrent.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/ArchiveOrgFolder.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/ArchiveOrgFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/ChipDe.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/ChipDe.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/CloudMailRuFolder.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/CloudMailRuFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/CloudzillaToFolder.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/CloudzillaToFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/CriptTo.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/CriptTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/CryptCat.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/CryptCat.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/CzshareComFolder.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/CzshareComFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/DailymotionComFolder.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/DailymotionComFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/DataHuFolder.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/DataHuFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/DebridlinkFrTorrent.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/DebridlinkFrTorrent.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/DepositfilesComFolder.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/DepositfilesComFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/Dereferer.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/Dereferer.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/DevhostStFolder.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/DevhostStFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/DlProtectCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/DlProtectCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/EasybytezComFolder.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/EasybytezComFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/EmbeduploadCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/EmbeduploadCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/FilecloudIoFolder.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/FilecloudIoFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/FilecryptCc.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/FilecryptCc.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/FilefactoryComFolder.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/FilefactoryComFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/FilerNetFolder.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/FilerNetFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/FilestubeCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/FilestubeCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/FiletramCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/FiletramCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/FourChanOrg.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/FourChanOrg.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/FreakhareComFolder.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/FreakhareComFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/FreetexthostCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/FreetexthostCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/FshareVnFolder.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/FshareVnFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/FurLy.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/FurLy.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/Go4UpCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/Go4UpCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/GofileIoFolder.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/GofileIoFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/GooGl.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/GooGl.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/GoogledriveComDereferer.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/GoogledriveComDereferer.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/GoogledriveComFolder.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/GoogledriveComFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/HearthisAtFolder.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/HearthisAtFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/HflixIn.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/HflixIn.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/HoerbuchIn.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/HoerbuchIn.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/ImgurCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/ImgurCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/JDlist.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/JDlist.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/LixIn.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/LixIn.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/MediafireComFolder.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/MediafireComFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/MegaCoNzFolder.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/MegaCoNzFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/MegaRapidCzFolder.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/MegaRapidCzFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/MegadyskPlFolder.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/MegadyskPlFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/MirrorcreatorCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/MirrorcreatorCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/MultiUpOrg.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/MultiUpOrg.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/MultiloadCz.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/MultiloadCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/NitroflareComFolder.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/NitroflareComFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/NosvideoCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/NosvideoCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/PastebinCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/PastebinCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/PastedCo.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/PastedCo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/QuickshareCzFolder.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/QuickshareCzFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/RealdebridComTorrent.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/RealdebridComTorrent.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/SafelinkingNet.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/SafelinkingNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/SexuriaCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/SexuriaCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/ShSt.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/ShSt.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/TNTVillageScambioeticoOrg.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/TNTVillageScambioeticoOrg.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/TenluaVnFolder.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/TenluaVnFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/TinyurlCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/TinyurlCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/TnyCz.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/TnyCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/TurbobitNetFolder.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/TurbobitNetFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/TusfilesNetFolder.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/TusfilesNetFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/UlozToFolder.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/UlozToFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/XFileSharingFolder.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/XFileSharingFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/XupPl.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/XupPl.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/decrypters/YoutubeComFolder.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/decrypters/YoutubeComFolder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/AccioDebridCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/AccioDebridCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/AlfafileNet.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/AlfafileNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/AlldebridCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/AlldebridCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/AndroidfilehostCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/AndroidfilehostCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/AnonfilesCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/AnonfilesCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/ArchiveOrg.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/ArchiveOrg.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/BasketbuildCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/BasketbuildCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/BayfilesCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/BayfilesCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/BezvadataCz.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/BezvadataCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/ClicknuploadCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FiregetCom.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,36 @@
 # -*- coding: utf-8 -*-
 
 from ..base.xfs_downloader import XFSDownloader
 
 
-class ClicknuploadCom(XFSDownloader):
-    __name__ = "ClicknuploadCom"
+class FiregetCom(XFSDownloader):
+    __name__ = "FiregetCom"
     __type__ = "downloader"
-    __version__ = "0.07"
+    __version__ = "0.04"
     __status__ = "testing"
 
-    __pattern__ = r"https?://(?:www\.)?clicknupload\.(?:com|org|cc|to|me|link|club)/(?P<ID>\w{12})"
+    __pattern__ = r"http://(?:www\.)?fireget\.com/(?P<ID>\w{12})/.+"
     __config__ = [
         ("enabled", "bool", "Activated", True),
         ("use_premium", "bool", "Use premium account if available", True),
         ("fallback", "bool", "Fallback to free download if premium fails", True),
         ("chk_filesize", "bool", "Check file size", True),
         ("max_wait", "int", "Reconnect if waiting time is greater than minutes", 10),
     ]
 
-    __description__ = """Clicknupload.com downloader plugin"""
+    __description__ = """Fireget.com downloader plugin"""
     __license__ = "GPLv3"
-    __authors__ = [
-        ("tbsn", "tbsnpy_github@gmx.de"),
-        ("GammaC0de", "nitzo2001[AT]yahoo[DOT]com"),
-    ]
-
-    PLUGIN_DOMAIN = "clicknupload.to"
-
-    URL_REPLACEMENTS = [(__pattern__ + ".*", r"https://clicknupload.to/\g<ID>")]
+    __authors__ = [("GammaC0de", "nitzo2001[AT]yahoo[DOT]com")]
 
-    LINK_PATTERN = r"onClick=\"window.open\('(.+?)'\);"
+    NAME_PATTERN = r'name="fname" value="(?P<N>.+?)"'
+    SIZE_PATTERN = r">You have requested .+?> \((?P<S>[\d.,]+) (?P<U>[\w^_]+)\)"
 
-    NAME_PATTERN = r'name="fname" value="(?P<N>.+?)">'
-    SIZE_PATTERN = r">size</span>\s*<span>(?P<S>[\d.,]+) (?P<U>[\w^_]+)</span>"
+    WAIT_PATTERN = r'<span id="countdown_str">.+?<span .+?>(\d+)</span>'
+    DL_LIMIT_PATTERN = r">You have to wait (.+?) till next download<"
 
-    OFFLINE_PATTERN = r"File Not Found"
-    ERROR_PATTERN = ""
+    OFFLINE_PATTERN = r"File Not Found|No such file with this filename"
+    TEMP_OFFLINE_PATTERN = (
+        r"Connection limit reached|Server error|You have reached the download limit"
+    )
 
-    WAIT_PATTERN = r'<span class="seconds">(\d+)</span>'
+    PLUGIN_DOMAIN = "fireget.com"
```

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/CloudMailRu.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/CloudMailRu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/CloudzillaTo.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/CloudzillaTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/CosmoboxOrg.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/CosmoboxOrg.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/CramitIn.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/CramitIn.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/CzshareCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/CzshareCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/DailymotionCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/DailymotionCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/DailyuploadsNet.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/DailyuploadsNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/DataHu.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/DataHu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/DataportCz.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/DataportCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/DatoidCz.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/DatoidCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/DdownloadCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/DdownloadCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/DebridItaliaCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/DebridItaliaCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/DebridlinkFr.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/DebridlinkFr.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/DebridplanetCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/DebridplanetCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/DefaultPlugin.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/DefaultPlugin.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/DepositfilesCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/DepositfilesCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/DevhostSt.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/DevhostSt.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/DlFreeFr.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/DlFreeFr.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/DownsterNet.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/DownsterNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/DropDownload.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/DropDownload.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/DropboxCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/DropboxCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/EasybytezCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/EasybytezCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/EdiskCz.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/EdiskCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/EuroshareEu.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/EuroshareEu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/ExashareCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/ExashareCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/ExtmatrixCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/ExtmatrixCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FastixRu.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FastixRu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FastshareCz.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FastshareCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FileAl.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FileAl.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FileSharkPl.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FileSharkPl.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FileStoreTo.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FileStoreTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FileboomMe.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FileboomMe.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FilecloudIo.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FilecloudIo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FiledropperCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FiledropperCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FilefactoryCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FilefactoryCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FilefoxCc.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FilefoxCc.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FilejokerNet.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FilejokerNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FileomCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FileomCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FilepupNet.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FilepupNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FilerNet.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FilerNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FilerioCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FilerioCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FilesMailRu.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FilesMailRu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FileuploadCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FileuploadCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FileuploadNet.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FileuploadNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FiregetCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/NofileIo.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,30 @@
 # -*- coding: utf-8 -*-
 
-from ..base.xfs_downloader import XFSDownloader
+from ..base.simple_downloader import SimpleDownloader
 
 
-class FiregetCom(XFSDownloader):
-    __name__ = "FiregetCom"
+class NofileIo(SimpleDownloader):
+    __name__ = "NofileIo"
     __type__ = "downloader"
-    __version__ = "0.04"
+    __version__ = "0.01"
     __status__ = "testing"
 
-    __pattern__ = r"http://(?:www\.)?fireget\.com/(?P<ID>\w{12})/.+"
+    __pattern__ = r"https?://(?:www\.)?nofile\.io/f/[\w^_]+"
     __config__ = [
         ("enabled", "bool", "Activated", True),
         ("use_premium", "bool", "Use premium account if available", True),
         ("fallback", "bool", "Fallback to free download if premium fails", True),
         ("chk_filesize", "bool", "Check file size", True),
         ("max_wait", "int", "Reconnect if waiting time is greater than minutes", 10),
     ]
 
-    __description__ = """Fireget.com downloader plugin"""
+    __description__ = """Nofile.io downloader plugin"""
     __license__ = "GPLv3"
     __authors__ = [("GammaC0de", "nitzo2001[AT]yahoo[DOT]com")]
 
-    NAME_PATTERN = r'name="fname" value="(?P<N>.+?)"'
-    SIZE_PATTERN = r">You have requested .+?> \((?P<S>[\d.,]+) (?P<U>[\w^_]+)\)"
-
-    WAIT_PATTERN = r'<span id="countdown_str">.+?<span .+?>(\d+)</span>'
-    DL_LIMIT_PATTERN = r">You have to wait (.+?) till next download<"
-
-    OFFLINE_PATTERN = r"File Not Found|No such file with this filename"
-    TEMP_OFFLINE_PATTERN = (
-        r"Connection limit reached|Server error|You have reached the download limit"
+    NAME_PATTERN = r'<span id="filename">(?P<N>.+?)</span>'
+    SIZE_PATTERN = (
+        r"<strong>File size</strong><br/>\s*(?P<S>[\d\.,]+) (?P<U>[\w^_]+)\s*<"
     )
 
-    PLUGIN_DOMAIN = "fireget.com"
+    LINK_PATTERN = r'data-url="(https://\w+\.nofilecdn\.io/g/.+?)"'
```

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FistfastNet.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FistfastNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FlyFilesNet.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FlyFilesNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FourSharedCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FourSharedCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/FshareVn.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/FshareVn.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/Ftp.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/Ftp.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/GamefrontCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/GamefrontCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/GetTwentyFourOrg.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/GetTwentyFourOrg.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/GigapetaCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/GigapetaCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/GofileIo.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/GofileIo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/GooIm.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/GooIm.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/GoogledriveCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/GoogledriveCom.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from ..base.downloader import BaseDownloader
 
 
 class GoogledriveCom(BaseDownloader):
     __name__ = "GoogledriveCom"
     __type__ = "downloader"
-    __version__ = "0.33"
+    __version__ = "0.34"
     __status__ = "testing"
 
     __pattern__ = r"https?://(?:www\.)?(?:drive|docs)\.google\.com/(?:file/d/|uc\?.*id=)(?P<ID>[-\w]+)"
     __config__ = [
         ("enabled", "bool", "Activated", True),
         ("use_premium", "bool", "Use premium account if available", True),
         ("fallback", "bool", "Fallback to free download if premium fails", True),
@@ -71,47 +71,49 @@
                     "API Error: {}".format(cmd),
                     exc,
                     "ID: {}".format(self.info["pattern"]["ID"]),
                     "Error code: {}".format(exc.code),
                 )
             return None
 
-    def api_download(self):
+    def api_download(self, disposition):
         try:
             self.download(
                 "{}{}/{}".format(self.API_URL, "files", self.info["pattern"]["ID"]),
                 get={
                     "alt": "media",
-                    # 'acknowledgeAbuse': "true",
+                    "acknowledgeAbuse": "true",
+                    "supportsAllDrives": "true",
                     "key": self.API_KEY,
                 },
+                disposition=disposition
             )
 
         except BadHeader as exc:
             if exc.code == 404:
                 self.offline()
 
             elif exc.code == 403:
                 self.temp_offline()
 
             else:
                 raise
 
     def process(self, pyfile):
         disposition = False
-        self.data = self.load(pyfile.url)
         json_data = self.api_request(
             "files/" + self.info["pattern"]["ID"],
             fields="md5Checksum,name,size",
             supportsAllDrives="true",
         )
 
         if json_data is None:
             self.fail("API error")
 
+        self.data = self.load(pyfile.url, ref=False)
         if "error" in json_data:
             if json_data["error"]["code"] == 404:
                 if "Virus scan warning" not in self.data:
                     self.offline()
 
                 else:
                     m = re.search(self.INFO_PATTERN, self.data)
@@ -126,15 +128,15 @@
 
         else:
             pyfile.size = int(json_data["size"])
             pyfile.name = json_data["name"]
             self.info["md5"] = json_data["md5Checksum"]
 
         # Somehow, API downloads are significantly slow compared to "normal" download :(
-        # self.api_download()
+        # self.api_download(disposition)
 
         for _i in range(2):
             m = re.search(r'"([^"]+uc\?.*?)"', self.data)
             if m is None:
                 if "Quota exceeded" in self.data:
                     self.temp_offline()
                 else:
```

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/HearthisAt.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/HearthisAt.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/HellshareCz.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/HellshareCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/HighWayMe.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/HighWayMe.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/HitfileNet.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/HitfileNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/HostujeNet.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/HostujeNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/HotlinkCc.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/HotlinkCc.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/Http.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/Http.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # -*- coding: utf-8 -*-
 
+import fnmatch
 import re
 import urllib.parse
 
 from pyload.core.network.http.exceptions import BadHeader
 
 from ..base.downloader import BaseDownloader
 
 
 class Http(BaseDownloader):
     __name__ = "Http"
     __type__ = "downloader"
-    __version__ = "0.13"
+    __version__ = "0.14"
     __status__ = "testing"
 
     __pattern__ = r"(?:jd|pys?)://.+"
     __config__ = [("enabled", "bool", "Activated", True)]
 
     __description__ = """Download simple http link"""
     __license__ = "GPLv3"
@@ -52,17 +53,20 @@
             else:
                 if self.account:
                     logins = dict((x['login'], x['password'])
                                   for x in self.account.get_all_accounts())
                 else:
                     logins = {}
 
-                if netloc in logins:
-                    auth = logins[netloc]
-                    self.log_debug(f"Logging on to {netloc} using the account plugin")
+                for pattern, auth in logins.items():
+                    if fnmatch.fnmatch(netloc, pattern):
+                        self.log_debug(f"Logging on to {netloc} using the account plugin")
+                        break
+                else:
+                    auth = None
 
             if auth is not None:
                 self.req.add_auth(auth)
 
         else:
             self.log_debug(f"Logging on to {netloc} using credentials specified in the URL")
```

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/HugefilesNet.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/HugefilesNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/HundredEightyUploadCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/HundredEightyUploadCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/IfolderRu.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/IfolderRu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/IronfilesNet.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/IronfilesNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/JumbofilesCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/JumbofilesCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/JunocloudMe.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/JunocloudMe.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/KatfileCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/KatfileCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/Keep2ShareCc.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/Keep2ShareCc.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/KingfilesNet.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/KingfilesNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/KrakenfilesCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/KrakenfilesCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/LeechThreeHundreedSixtyCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/LeechThreeHundreedSixtyCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/LetsuploadCc.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/LetsuploadCc.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/LetsuploadCo.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/LetsuploadCo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/LibgenIo.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/LibgenIo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/LinkifierCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/LinkifierCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/LinksnappyCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/LinksnappyCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/LinksnappyComTorrent.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/LinksnappyComTorrent.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/LoadTo.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/LoadTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/MediafireCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/MediafireCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/MegaCoNz.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/MegaCoNz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/MegaDebridEu.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/MegaDebridEu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/MegaRapidCz.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/MegaRapidCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/MegaRapidoNet.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/MegaRapidoNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/MegacrypterCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/MegacrypterCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/MegadyskPl.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/MegadyskPl.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/MegasharesCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/MegasharesCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/MegaupNet.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/MegaupNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/MovReelCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/MovReelCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/MultihostersCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/MultihostersCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/MultishareCz.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/MultishareCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/MyfastfileCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/MyfastfileCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/MystoreTo.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/MystoreTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/NarodRu.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/NarodRu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/NippyshareCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/NippyshareCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/NitrobitNet.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/NitrobitNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/NitroflareCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/NitroflareCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/NoPremiumPl.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/NoPremiumPl.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/NofileIo.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/VidPlayNet.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # -*- coding: utf-8 -*-
 
-from ..base.simple_downloader import SimpleDownloader
+#
+# Test links:
+# BigBuckBunny_320x180.mp4 - 61.7 Mb - http://vidplay.net/38lkev0h3jv0
 
+from ..base.xfs_downloader import XFSDownloader
 
-class NofileIo(SimpleDownloader):
-    __name__ = "NofileIo"
+
+class VidPlayNet(XFSDownloader):
+    __name__ = "VidPlayNet"
     __type__ = "downloader"
-    __version__ = "0.01"
+    __version__ = "0.11"
     __status__ = "testing"
 
-    __pattern__ = r"https?://(?:www\.)?nofile\.io/f/[\w^_]+"
+    __pattern__ = r"https?://(?:www\.)?vidplay\.net/\w{12}"
     __config__ = [
         ("enabled", "bool", "Activated", True),
         ("use_premium", "bool", "Use premium account if available", True),
         ("fallback", "bool", "Fallback to free download if premium fails", True),
         ("chk_filesize", "bool", "Check file size", True),
         ("max_wait", "int", "Reconnect if waiting time is greater than minutes", 10),
     ]
 
-    __description__ = """Nofile.io downloader plugin"""
+    __description__ = """VidPlay.net downloader plugin"""
     __license__ = "GPLv3"
-    __authors__ = [("GammaC0de", "nitzo2001[AT]yahoo[DOT]com")]
+    __authors__ = [("t4skforce", "t4skforce1337[AT]gmail[DOT]com")]
 
-    NAME_PATTERN = r'<span id="filename">(?P<N>.+?)</span>'
-    SIZE_PATTERN = (
-        r"<strong>File size</strong><br/>\s*(?P<S>[\d\.,]+) (?P<U>[\w^_]+)\s*<"
-    )
+    PLUGIN_DOMAIN = "vidplay.net"
 
-    LINK_PATTERN = r'data-url="(https://\w+\.nofilecdn\.io/g/.+?)"'
+    NAME_PATTERN = r"<b>Password:</b></div>\s*<h[1-6]>(?P<N>.+?)</h[1-6]>"
```

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/NosuploadCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/NosuploadCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/NovafileCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/NovafileCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/NowVideoSx.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/NowVideoSx.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/OneFichierCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/OneFichierCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/OnlineTvRecorder.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/OnlineTvRecorder.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/OpenloadIo.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/OpenloadIo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/OverLoadMe.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/OverLoadMe.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/PixeldrainCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/PixeldrainCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/PornhostCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/PornhostCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/PornhubCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/PornhubCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/PornovkaCz.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/PornovkaCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/PorntrexCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/PorntrexCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/PremiumTo.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/PremiumTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/PremiumizeMe.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/PremiumizeMe.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/PromptfileCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/PromptfileCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/PutdriveCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/PutdriveCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/QuickshareCz.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/QuickshareCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/RPNetBiz.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/RPNetBiz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/RapideoPl.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/RapideoPl.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/RapidfileshareNet.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/RapidfileshareNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/RapidgatorNet.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/RapidgatorNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/RapiduNet.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/RapiduNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/RarefileNet.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/RarefileNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/RealdebridCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/RealdebridCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/RedtubeCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/RedtubeCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/RehostTo.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/RehostTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/RemixshareCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/RemixshareCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/RgHostNet.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/RgHostNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/SafesharingEu.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/SafesharingEu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/SecureUploadEu.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/SecureUploadEu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/SenditCloud.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/SenditCloud.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/SendspaceCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/SendspaceCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/ShareplaceCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/ShareplaceCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/SimplyPremiumCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/SimplyPremiumCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/SimplydebridCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/SimplydebridCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/SizedriveCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/SizedriveCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/SmoozedCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/SmoozedCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/SmuleCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/SmuleCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/SolidfilesCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/SolidfilesCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/SoundcloudCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/SoundcloudCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/SpeedyshareCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/SpeedyshareCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/StreamCz.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/StreamCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/StreamcloudEu.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/StreamcloudEu.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/SuprafilesMe.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/SuprafilesMe.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/TbSevenPl.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/TbSevenPl.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/TenluaVn.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/TenluaVn.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/TurbobitNet.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/TurbobitNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/TusfilesNet.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/TusfilesNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/TwoSharedCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/TwoSharedCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/TwojlimitPl.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/TwojlimitPl.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/UlozTo.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/UlozTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/UloziskoSk.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/UloziskoSk.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/UnibytesCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/UnibytesCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/UpfileVn.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/UpfileVn.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/UpleaCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/UpleaCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/UploadgigCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/UploadgigCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/UploadheroCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/UploadheroCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/UploadrocketNet.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/UploadrocketNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/UploadshipCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/UploadshipCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/UpstoreNet.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/UpstoreNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/UptoboxCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/UptoboxCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/UserscloudCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/UserscloudCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/UseruploadNet.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/UseruploadNet.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/VeehdCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/VeehdCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/VeohCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/VeohCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/VidPlayNet.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/WrzucajplikiPl.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 # -*- coding: utf-8 -*-
 
-#
-# Test links:
-# BigBuckBunny_320x180.mp4 - 61.7 Mb - http://vidplay.net/38lkev0h3jv0
+import re
 
 from ..base.xfs_downloader import XFSDownloader
 
 
-class VidPlayNet(XFSDownloader):
-    __name__ = "VidPlayNet"
+class WrzucajplikiPl(XFSDownloader):
+    __name__ = "WrzucajplikiPl"
     __type__ = "downloader"
-    __version__ = "0.11"
+    __version__ = "0.03"
     __status__ = "testing"
 
-    __pattern__ = r"https?://(?:www\.)?vidplay\.net/\w{12}"
+    __pattern__ = r"https?://(?:www\.)?wrzucajpliki\.pl/(?P<ID>\w{12})"
     __config__ = [
         ("enabled", "bool", "Activated", True),
         ("use_premium", "bool", "Use premium account if available", True),
         ("fallback", "bool", "Fallback to free download if premium fails", True),
         ("chk_filesize", "bool", "Check file size", True),
         ("max_wait", "int", "Reconnect if waiting time is greater than minutes", 10),
     ]
 
-    __description__ = """VidPlay.net downloader plugin"""
+    __description__ = """Wrzucajpliki.pl downloader plugin"""
     __license__ = "GPLv3"
-    __authors__ = [("t4skforce", "t4skforce1337[AT]gmail[DOT]com")]
+    __authors__ = [("GammaC0de", "nitzo2001[AT]yahoo[DOT]com")]
 
-    PLUGIN_DOMAIN = "vidplay.net"
+    NAME_PATTERN = r'name="fname" value="(?P<N>.+?)"'
+    SIZE_PATTERN = r">You have requested .+?> \((?P<S>[\d.,]+) (?P<U>[\w^_]+)\)"
 
-    NAME_PATTERN = r"<b>Password:</b></div>\s*<h[1-6]>(?P<N>.+?)</h[1-6]>"
+    WAIT_PATTERN = r'<span class="seconds">(\d+)</span>'
+    DL_LIMIT_PATTERN = r">You have to wait (.+?) till next download<"
+
+    OFFLINE_PATTERN = r"File Not Found|No such file with this filename"
+    TEMP_OFFLINE_PATTERN = (
+        r"Connection limit reached|Server error|You have reached the download limit"
+    )
+
+    PLUGIN_DOMAIN = "wrzucajpliki.pl"
```

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/VimeoCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/VimeoCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/VkCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/VkCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/WebshareCz.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/WebshareCz.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/WetransferCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/WetransferCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/WrzucTo.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/WrzucTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/WrzucajplikiPl.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/XVideosCom.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,31 @@
 # -*- coding: utf-8 -*-
 
 import re
+import urllib.parse
 
-from ..base.xfs_downloader import XFSDownloader
+from ..base.downloader import BaseDownloader
 
 
-class WrzucajplikiPl(XFSDownloader):
-    __name__ = "WrzucajplikiPl"
+class XVideosCom(BaseDownloader):
+    __name__ = "XVideos.com"
     __type__ = "downloader"
-    __version__ = "0.03"
+    __version__ = "0.17"
     __status__ = "testing"
 
-    __pattern__ = r"https?://(?:www\.)?wrzucajpliki\.pl/(?P<ID>\w{12})"
-    __config__ = [
-        ("enabled", "bool", "Activated", True),
-        ("use_premium", "bool", "Use premium account if available", True),
-        ("fallback", "bool", "Fallback to free download if premium fails", True),
-        ("chk_filesize", "bool", "Check file size", True),
-        ("max_wait", "int", "Reconnect if waiting time is greater than minutes", 10),
-    ]
+    __pattern__ = r"https?://(?:www\.)?xvideos\.com/video(\d+)"
+    __config__ = [("enabled", "bool", "Activated", True)]
 
-    __description__ = """Wrzucajpliki.pl downloader plugin"""
+    __description__ = """XVideos.com downloader plugin"""
     __license__ = "GPLv3"
-    __authors__ = [("GammaC0de", "nitzo2001[AT]yahoo[DOT]com")]
+    __authors__ = []
 
-    NAME_PATTERN = r'name="fname" value="(?P<N>.+?)"'
-    SIZE_PATTERN = r">You have requested .+?> \((?P<S>[\d.,]+) (?P<U>[\w^_]+)\)"
-
-    WAIT_PATTERN = r'<span class="seconds">(\d+)</span>'
-    DL_LIMIT_PATTERN = r">You have to wait (.+?) till next download<"
-
-    OFFLINE_PATTERN = r"File Not Found|No such file with this filename"
-    TEMP_OFFLINE_PATTERN = (
-        r"Connection limit reached|Server error|You have reached the download limit"
-    )
-
-    PLUGIN_DOMAIN = "wrzucajpliki.pl"
+    def process(self, pyfile):
+        site = self.load(pyfile.url)
+        title_search = re.search(r'<meta\s+property="og:title"\s+content="(.+?)"', site)
+        id_search = re.search(self.__pattern__, pyfile.url)
+        pyfile.name = "{} ({}).mp4".format(title_search.group(1), id_search.group(1))
+        self.download(
+            urllib.parse.unquote(
+                re.search(r"html5player\.setVideoUrlHigh\(\'(.+?)\'\)", site).group(1)
+            )
+        )
```

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/XDCC.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/XDCC.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/XFileSharing.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/XFileSharing.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/XHamsterCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/XHamsterCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/XVideosCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/XdadevelopersCom.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,41 @@
-# -*- coding: utf-8 -*-
+# -*- coding: utf-8 -*
 
-import re
-import urllib.parse
+#
+# Test links:
+#   http://forum.xda-developers.com/devdb/project/dl/?id=10885
 
-from ..base.downloader import BaseDownloader
 
+from ..base.simple_downloader import SimpleDownloader
 
-class XVideosCom(BaseDownloader):
-    __name__ = "XVideos.com"
+
+class XdadevelopersCom(SimpleDownloader):
+    __name__ = "XdadevelopersCom"
     __type__ = "downloader"
-    __version__ = "0.17"
+    __version__ = "0.08"
     __status__ = "testing"
 
-    __pattern__ = r"https?://(?:www\.)?xvideos\.com/video(\d+)"
-    __config__ = [("enabled", "bool", "Activated", True)]
+    __pattern__ = r"https?://(?:www\.)?forum\.xda-developers\.com/devdb/project/dl/\?id=\d+"
+    __config__ = [
+        ("enabled", "bool", "Activated", True),
+        ("use_premium", "bool", "Use premium account if available", True),
+        ("fallback", "bool", "Fallback to free download if premium fails", True),
+        ("chk_filesize", "bool", "Check file size", True),
+        ("max_wait", "int", "Reconnect if waiting time is greater than minutes", 10),
+    ]
 
-    __description__ = """XVideos.com downloader plugin"""
+    __description__ = """Xda-developers.com downloader plugin"""
     __license__ = "GPLv3"
-    __authors__ = []
+    __authors__ = [("zapp-brannigan", "fuerst.reinje@web.de")]
 
-    def process(self, pyfile):
-        site = self.load(pyfile.url)
-        title_search = re.search(r'<meta\s+property="og:title"\s+content="(.+?)"', site)
-        id_search = re.search(self.__pattern__, pyfile.url)
-        pyfile.name = "{} ({}).mp4".format(title_search.group(1), id_search.group(1))
-        self.download(
-            urllib.parse.unquote(
-                re.search(r"html5player\.setVideoUrlHigh\(\'(.+?)\'\)", site).group(1)
-            )
-        )
+    NAME_PATTERN = r"<label>Filename:</label>\s*<div>\s*(?P<N>.*?)\n"
+    SIZE_PATTERN = r"<label>Size:</label>\s*<div>\s*(?P<S>[\d.,]+)(?P<U>[\w^_]+)"
+    OFFLINE_PATTERN = r"</i> Device Filter</h3>"
+
+    def setup(self):
+        self.multi_dl = True
+        self.resume_download = True
+        self.chunk_limit = 1
+
+    def handle_free(self, pyfile):
+        # TODO: Revert to `get={'task': "get"}` in 0.6.x
+        self.link = pyfile.url + "&task=get"
```

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/YadiSk.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/YadiSk.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/YesPornPleaseCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/YesPornPleaseCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/YibaishiwuCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/YibaishiwuCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/YoupornCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/YoupornCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/YourfilesTo.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/YourfilesTo.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/YoutubeCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/YoutubeCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/ZDF.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/ZDF.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/ZbigzCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/ZbigzCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/ZeveraCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/ZeveraCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/downloaders/ZippyshareCom.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/downloaders/ZippyshareCom.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/extractors/HjSplit.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/extractors/HjSplit.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/extractors/SevenZip.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/extractors/SevenZip.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/extractors/UnRar.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/extractors/UnRar.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/extractors/UnTar.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/extractors/UnTar.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/extractors/UnZip.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/extractors/UnZip.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/plugins/helpers.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/plugins/helpers.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/__init__.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/__init__.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/blueprints/__init__.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/blueprints/__init__.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/blueprints/api_blueprint.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/blueprints/api_blueprint.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/blueprints/app_blueprint.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/blueprints/app_blueprint.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/blueprints/cnl_blueprint.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/blueprints/cnl_blueprint.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/blueprints/json_blueprint.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/blueprints/json_blueprint.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/config.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/config.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/extensions.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/extensions.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/filters.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/filters.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/handlers.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/handlers.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/helpers.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/helpers.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/processors.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/processors.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/css/base.css` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/css/base.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/css/logs.css` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/css/logs.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/css/pathchooser.css` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/css/pathchooser.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/css/window.css` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/css/window.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/add_folder.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/add_folder.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/arrow-refresh.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/arrow-refresh.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/cog.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/cog.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/control-add-blue.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/control-add-blue.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/control-cancel-blue.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/control-cancel-blue.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/control-cancel.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/control-cancel.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/control-pause-blue.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/control-pause-blue.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/control-pause.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/control-pause.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/control-play-blue.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/control-play-blue.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/control-play.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/control-play.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/control-stop-blue.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/control-stop-blue.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/delete.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/delete.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/dialog-close.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/dialog-close.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/dialog-question.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/dialog-question.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/error.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/error.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/favicon.ico` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/folder.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/folder.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/head-login.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/head-login.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/head-menu-collector.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/head-menu-collector.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/head-menu-config.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/head-menu-config.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/head-menu-development.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/head-menu-development.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/head-menu-download.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/head-menu-download.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/head-menu-home.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/head-menu-home.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/head-menu-news.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/head-menu-news.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/head-menu-queue.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/head-menu-queue.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/head-menu-recent.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/head-menu-recent.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/head-menu-wiki.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/head-menu-wiki.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/head-search-noshadow.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/head-search-noshadow.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/images.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/images.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/notice.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/notice.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/package-go.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/package-go.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/page-tools-backlinks.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/page-tools-backlinks.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/page-tools-edit.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/page-tools-edit.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/page-tools-revisions.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/page-tools-revisions.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/parse-uri.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/parse-uri.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/pyload-logo.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/pyload-logo.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/reconnect.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/reconnect.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/status-downloading.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/status-downloading.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/status-failed.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/status-failed.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/status-finished.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/status-finished.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/status-none.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/status-none.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/status-offline.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/status-offline.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/status-proc.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/status-proc.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/status-queue.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/status-queue.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/status-waiting.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/status-waiting.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/success.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/success.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/user-actions-logout.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/user-actions-logout.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/user-actions-profile.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/user-actions-profile.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/img/user-info.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/img/user-info.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/js/captcha-interactive.user.js` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/js/captcha-interactive.user.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Alert.js` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Alert.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Confirm.js` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Confirm.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Fx.js` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Fx.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.IFrame.js` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.IFrame.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Prompt.js` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Prompt.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Request.js` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.Request.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.js` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/MooDialog/MooDialog.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/MooDialog/Overlay.js` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/MooDialog/Overlay.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/MooDialog.css` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/MooDialog.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-close.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-close.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-error.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-error.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-question.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-question.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-warning.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/MooDialog/css/dialog-warning.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/MooDropMenu/MooDropMenu.js` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/MooDropMenu/MooDropMenu.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/MooDropMenu/css/MooDropMenu.css` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/MooDropMenu/css/MooDropMenu.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/MooTools-Core.min.js` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/MooTools-Core.min.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/MooTools-More.min.js` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/MooTools-More.min.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/Purr/purr.js` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/Purr/purr.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/static/vendor/MooTools/TinyTab/tinytab.js` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/static/vendor/MooTools/TinyTab/tinytab.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/base.html` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/base.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/captcha.html` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/captcha.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/dashboard.html` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/dashboard.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/filemanager.html` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/filemanager.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/files.html` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/files.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/folder.html` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/folder.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/info.html` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/info.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/js/base.js` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/js/base.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/js/dashboard.js` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/js/dashboard.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/js/filemanager.js` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/js/filemanager.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/js/packages.js` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/js/packages.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/js/settings.js` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/js/settings.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/login.html` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/login.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/logs.html` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/logs.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/packages.html` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/packages.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/pathchooser.html` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/pathchooser.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/settings.html` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/settings.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/settings_item.html` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/settings_item.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/templates/window.html` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/templates/window.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/css/base.css` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/css/base.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/css/logs.css` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/css/logs.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/css/pathchooser.css` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/css/pathchooser.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/css/settings.css` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/css/settings.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/img/favicon.ico` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/img/pyload-banner.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/img/pyload-banner.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/img/pyload-logo.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/img/pyload-logo.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/img/ui-icons_444444_256x240.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/img/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/css/bootstrap.min.css` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.eot` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.svg` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.ttf` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff2` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/js/bootstrap.min.js` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/Bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_444444_256x240.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_555555_256x240.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_777620_256x240.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_777777_256x240.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_cc0000_256x240.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_ffffff_256x240.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/jquery-ui.min.css` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/jquery-ui.min.js` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jQuery UI/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jquery.min.js` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/jQuery/jquery.min.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/mdtoast/css/mdtoast.min.css` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/mdtoast/css/mdtoast.min.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/static/vendor/mdtoast/js/mdtoast.min.js` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/static/vendor/mdtoast/js/mdtoast.min.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/templates/base.html` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/templates/base.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/templates/captcha.html` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/templates/captcha.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/templates/dashboard.html` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/templates/dashboard.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/templates/files.html` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/templates/files.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/templates/info.html` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/templates/info.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/templates/js/base.js` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/templates/js/base.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -522,17 +522,26 @@
 
     this._params = params;
 
     $("#" + this._iframeId).attr("src", url);
 };
 
 // This function listens to messages from the TamperMonkey script in the iframe
-interactiveCaptchaHandler.prototype.windowEventListener = function(e) {
-    var interactiveHandlerInstance = e.data;
-    var requestMessage = JSON.parse(e.originalEvent.data);
+interactiveCaptchaHandler.prototype.windowEventListener = function(event) {
+    var requestMessage;
+    try {
+        requestMessage = JSON.parse(event.originalEvent.data);
+    } catch (e) {
+        if (e instanceof SyntaxError) {
+            return
+        } else {
+            console.error(e)
+        }
+    }
+    var interactiveHandlerInstance = event.data;
 
     if (requestMessage.actionCode === interactiveHandlerInstance.actionCodes.submitResponse) {
         // We got the response! pass it to the callback function
         interactiveHandlerInstance._captchaResponseCallback(requestMessage.params.response);
         interactiveHandlerInstance.clearEventlisteners();
 
     } else if (requestMessage.actionCode === interactiveHandlerInstance.actionCodes.activated) {
```

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/templates/js/dashboard.js` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/templates/js/dashboard.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/templates/js/info.js` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/templates/js/info.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/templates/js/packages.js` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/templates/js/packages.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/templates/js/settings.js` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/templates/js/settings.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/templates/login.html` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/templates/login.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/templates/logs.html` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/templates/logs.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/templates/packages.html` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/templates/packages.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/templates/pathchooser.html` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/templates/pathchooser.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/templates/settings.html` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/templates/settings.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/templates/settings_item.html` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/templates/settings_item.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/modern/templates/window.html` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/modern/templates/window.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/css/base.css` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/css/base.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/css/logs.css` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/css/logs.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/css/pathchooser.css` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/css/pathchooser.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/css/settings.css` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/css/settings.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/img/favicon.ico` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/img/pyload-banner.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/img/pyload-banner.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/img/pyload-logo.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/img/pyload-logo.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/img/ui-icons_444444_256x240.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/img/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/css/bootstrap.min.css` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.eot` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.svg` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.ttf` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff2` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/js/bootstrap.min.js` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/Bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_444444_256x240.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_555555_256x240.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_777620_256x240.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_777777_256x240.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_cc0000_256x240.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_ffffff_256x240.png` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/jquery-ui.min.css` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/jquery-ui.min.js` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jQuery UI/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jquery.min.js` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/jQuery/jquery.min.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/mdtoast/css/mdtoast.min.css` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/mdtoast/css/mdtoast.min.css`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/static/vendor/mdtoast/js/mdtoast.min.js` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/static/vendor/mdtoast/js/mdtoast.min.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/templates/base.html` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/templates/base.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/templates/captcha.html` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/templates/captcha.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/templates/dashboard.html` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/templates/dashboard.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/templates/files.html` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/templates/files.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/templates/info.html` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/templates/info.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/templates/js/base.js` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/templates/js/base.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -522,17 +522,26 @@
 
     this._params = params;
 
     $("#" + this._iframeId).attr("src", url);
 };
 
 // This function listens to messages from the TamperMonkey script in the iframe
-interactiveCaptchaHandler.prototype.windowEventListener = function(e) {
-    var interactiveHandlerInstance = e.data;
-    var requestMessage = JSON.parse(e.originalEvent.data);
+interactiveCaptchaHandler.prototype.windowEventListener = function(event) {
+    var requestMessage;
+    try {
+        requestMessage = JSON.parse(event.originalEvent.data);
+    } catch (e) {
+        if (e instanceof SyntaxError) {
+            return
+        } else {
+            console.error(e)
+        }
+    }
+    var interactiveHandlerInstance = event.data;
 
     if (requestMessage.actionCode === interactiveHandlerInstance.actionCodes.submitResponse) {
         // We got the response! pass it to the callback function
         interactiveHandlerInstance._captchaResponseCallback(requestMessage.params.response);
         interactiveHandlerInstance.clearEventlisteners();
 
     } else if (requestMessage.actionCode === interactiveHandlerInstance.actionCodes.activated) {
```

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/templates/js/dashboard.js` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/templates/js/dashboard.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/templates/js/info.js` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/templates/js/info.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/templates/js/packages.js` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/templates/js/packages.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/templates/js/settings.js` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/templates/js/settings.js`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/templates/login.html` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/templates/login.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/templates/logs.html` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/templates/logs.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/templates/packages.html` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/templates/packages.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/templates/pathchooser.html` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/templates/pathchooser.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/templates/settings.html` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/templates/settings.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/templates/settings_item.html` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/templates/settings_item.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/app/themes/pyplex/templates/window.html` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/app/themes/pyplex/templates/window.html`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload/webui/webserver_thread.py` & `pyload-ng-0.5.0b3.dev57/src/pyload/webui/webserver_thread.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload_ng.egg-info/PKG-INFO` & `pyload-ng-0.5.0b3.dev57/src/pyload_ng.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyload-ng
-Version: 0.5.0b3.dev54
+Version: 0.5.0b3.dev57
 Summary: The free and open-source Download Manager written in pure Python
 Home-page: https://pyload.net
 Download-URL: https://github.com/pyload/pyload/releases
 Author: pyLoad team
 Author-email: support@pyload.net
 Maintainer: Walter Purcaro
 Maintainer-email: vuolter@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyload-ng Version: 0.5.0b3.dev54 Summary: The free
+Metadata-Version: 2.1 Name: pyload-ng Version: 0.5.0b3.dev57 Summary: The free
 and open-source Download Manager written in pure Python Home-page: https://
 pyload.net Download-URL: https://github.com/pyload/pyload/releases Author:
 pyLoad team Author-email: support@pyload.net Maintainer: Walter Purcaro
 Maintainer-email: vuolter@gmail.com License: agpl3 Project-URL: Source Code
 (mirror), https://gitlab.com/pyload/pyload Project-URL: Source Code, https://
 github.com/pyload/pyload Project-URL: Bug Tracker, https://github.com/pyload/
 pyload/issues Project-URL: Documentation, https://github.com/pyload/pyload/wiki
```

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload_ng.egg-info/SOURCES.txt` & `pyload-ng-0.5.0b3.dev57/src/pyload_ng.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -363,20 +363,22 @@
 src/pyload/plugins/downloaders/DepositfilesCom.py
 src/pyload/plugins/downloaders/DevhostSt.py
 src/pyload/plugins/downloaders/DlFreeFr.py
 src/pyload/plugins/downloaders/DownsterNet.py
 src/pyload/plugins/downloaders/DropDownload.py
 src/pyload/plugins/downloaders/DropboxCom.py
 src/pyload/plugins/downloaders/EasybytezCom.py
+src/pyload/plugins/downloaders/EasyuploadIo.py
 src/pyload/plugins/downloaders/EdiskCz.py
 src/pyload/plugins/downloaders/EuroshareEu.py
 src/pyload/plugins/downloaders/ExashareCom.py
 src/pyload/plugins/downloaders/ExtmatrixCom.py
 src/pyload/plugins/downloaders/FastixRu.py
 src/pyload/plugins/downloaders/FastshareCz.py
+src/pyload/plugins/downloaders/FikperCom.py
 src/pyload/plugins/downloaders/FileAl.py
 src/pyload/plugins/downloaders/FileSharkPl.py
 src/pyload/plugins/downloaders/FileStoreTo.py
 src/pyload/plugins/downloaders/FileboomMe.py
 src/pyload/plugins/downloaders/FilecloudIo.py
 src/pyload/plugins/downloaders/FiledropperCom.py
 src/pyload/plugins/downloaders/FilefactoryCom.py
```

### Comparing `pyload-ng-0.5.0b3.dev54/src/pyload_ng.egg-info/requires.txt` & `pyload-ng-0.5.0b3.dev57/src/pyload_ng.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/tests/api_exerciser.py` & `pyload-ng-0.5.0b3.dev57/tests/api_exerciser.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/tests/system_check.py` & `pyload-ng-0.5.0b3.dev57/tests/system_check.py`

 * *Files identical despite different names*

### Comparing `pyload-ng-0.5.0b3.dev54/tests/test_json.py` & `pyload-ng-0.5.0b3.dev57/tests/test_json.py`

 * *Files identical despite different names*

