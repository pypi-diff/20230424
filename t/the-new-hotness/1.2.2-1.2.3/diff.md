# Comparing `tmp/the-new-hotness-1.2.2.tar.gz` & `tmp/the_new_hotness-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "the-new-hotness-1.2.2.tar", max compression
+gzip compressed data, was "the_new_hotness-1.2.3.tar", max compression
```

## Comparing `the-new-hotness-1.2.2.tar` & `the_new_hotness-1.2.3.tar`

### file list

```diff
@@ -1,58 +1,304 @@
--rw-r--r--   0        0        0    26530 2021-01-25 12:20:24.199782 the-new-hotness-1.2.2/LICENSE
--rw-r--r--   0        0        0     1369 2022-06-02 08:11:44.403651 the-new-hotness-1.2.2/README.rst
--rw-r--r--   0        0        0     5389 2023-02-08 12:56:22.400053 the-new-hotness-1.2.2/config/config.toml.example
--rw-r--r--   0        0        0      288 2022-10-06 09:37:29.077735 the-new-hotness-1.2.2/hotness/__init__.py
--rw-r--r--   0        0        0      849 2022-06-02 08:11:44.409651 the-new-hotness-1.2.2/hotness/builders/__init__.py
--rw-r--r--   0        0        0     1467 2022-06-02 08:11:44.409651 the-new-hotness-1.2.2/hotness/builders/builder.py
--rw-r--r--   0        0        0    18261 2023-02-08 12:56:22.400053 the-new-hotness-1.2.2/hotness/builders/koji.py
--rw-r--r--   0        0        0      804 2022-06-02 08:11:44.409651 the-new-hotness-1.2.2/hotness/common/__init__.py
--rw-r--r--   0        0        0     5876 2022-06-02 08:11:44.410651 the-new-hotness-1.2.2/hotness/common/rpm.py
--rw-r--r--   0        0        0     6329 2022-11-29 14:56:07.408454 the-new-hotness-1.2.2/hotness/config.py
--rw-r--r--   0        0        0      897 2022-06-02 08:11:44.411651 the-new-hotness-1.2.2/hotness/databases/__init__.py
--rw-r--r--   0        0        0     2511 2022-06-02 08:11:44.411651 the-new-hotness-1.2.2/hotness/databases/cache.py
--rw-r--r--   0        0        0     1803 2022-06-02 08:11:44.411651 the-new-hotness-1.2.2/hotness/databases/database.py
--rw-r--r--   0        0        0     3609 2022-06-02 10:34:33.536528 the-new-hotness-1.2.2/hotness/databases/redis.py
--rw-r--r--   0        0        0      812 2022-06-02 08:11:44.411651 the-new-hotness-1.2.2/hotness/domain/__init__.py
--rw-r--r--   0        0        0     2181 2022-06-02 08:11:44.412651 the-new-hotness-1.2.2/hotness/domain/package.py
--rw-r--r--   0        0        0     1140 2022-06-02 08:11:44.412651 the-new-hotness-1.2.2/hotness/exceptions/__init__.py
--rw-r--r--   0        0        0     1602 2022-06-02 08:11:44.412651 the-new-hotness-1.2.2/hotness/exceptions/base_exception.py
--rw-r--r--   0        0        0     2438 2022-06-02 08:11:44.413651 the-new-hotness-1.2.2/hotness/exceptions/builder_exception.py
--rw-r--r--   0        0        0     1223 2022-06-02 08:11:44.413651 the-new-hotness-1.2.2/hotness/exceptions/download_exception.py
--rw-r--r--   0        0        0     1513 2022-06-02 08:11:44.413651 the-new-hotness-1.2.2/hotness/exceptions/http_exception.py
--rw-r--r--   0        0        0     1253 2022-06-02 08:11:44.413651 the-new-hotness-1.2.2/hotness/exceptions/notifier_exception.py
--rw-r--r--   0        0        0     1219 2022-06-02 08:11:44.413651 the-new-hotness-1.2.2/hotness/exceptions/patcher_exception.py
--rw-r--r--   0        0        0    28244 2022-11-29 14:56:07.409454 the-new-hotness-1.2.2/hotness/hotness_consumer.py
--rw-r--r--   0        0        0      919 2022-06-02 08:11:44.414651 the-new-hotness-1.2.2/hotness/notifiers/__init__.py
--rw-r--r--   0        0        0    10095 2022-06-02 08:11:44.416651 the-new-hotness-1.2.2/hotness/notifiers/bugzilla.py
--rw-r--r--   0        0        0     3552 2022-06-02 08:11:44.416651 the-new-hotness-1.2.2/hotness/notifiers/fedora_messaging.py
--rw-r--r--   0        0        0     1663 2022-06-02 08:11:44.416651 the-new-hotness-1.2.2/hotness/notifiers/notifier.py
--rw-r--r--   0        0        0      857 2022-06-02 08:11:44.416651 the-new-hotness-1.2.2/hotness/patchers/__init__.py
--rw-r--r--   0        0        0     4008 2022-06-02 08:11:44.416651 the-new-hotness-1.2.2/hotness/patchers/bugzilla.py
--rw-r--r--   0        0        0     1607 2022-06-02 08:11:44.416651 the-new-hotness-1.2.2/hotness/patchers/patcher.py
--rw-r--r--   0        0        0     1181 2022-06-02 08:11:44.416651 the-new-hotness-1.2.2/hotness/requests/__init__.py
--rw-r--r--   0        0        0     1287 2022-06-02 08:11:44.416651 the-new-hotness-1.2.2/hotness/requests/build_request.py
--rw-r--r--   0        0        0     1256 2022-06-02 08:11:44.416651 the-new-hotness-1.2.2/hotness/requests/insert_data_request.py
--rw-r--r--   0        0        0     1394 2022-06-02 08:11:44.416651 the-new-hotness-1.2.2/hotness/requests/notify_request.py
--rw-r--r--   0        0        0     1234 2022-06-02 08:11:44.416651 the-new-hotness-1.2.2/hotness/requests/package_request.py
--rw-r--r--   0        0        0     1905 2022-06-02 08:11:44.416651 the-new-hotness-1.2.2/hotness/requests/request.py
--rw-r--r--   0        0        0     1152 2022-06-02 08:11:44.416651 the-new-hotness-1.2.2/hotness/requests/retrieve_data_request.py
--rw-r--r--   0        0        0     1389 2022-06-02 08:11:44.416651 the-new-hotness-1.2.2/hotness/requests/submit_patch_request.py
--rw-r--r--   0        0        0      934 2022-06-02 08:11:44.416651 the-new-hotness-1.2.2/hotness/responses/__init__.py
--rw-r--r--   0        0        0     1540 2022-06-02 08:11:44.416651 the-new-hotness-1.2.2/hotness/responses/response.py
--rw-r--r--   0        0        0     6212 2022-06-02 08:11:44.418651 the-new-hotness-1.2.2/hotness/responses/response_failure.py
--rw-r--r--   0        0        0     1623 2022-06-02 08:11:44.418651 the-new-hotness-1.2.2/hotness/responses/response_success.py
--rw-r--r--   0        0        0     1194 2022-06-02 08:11:44.418651 the-new-hotness-1.2.2/hotness/use_cases/__init__.py
--rw-r--r--   0        0        0     1992 2022-06-02 08:11:44.418651 the-new-hotness-1.2.2/hotness/use_cases/insert_data_use_case.py
--rw-r--r--   0        0        0     2033 2022-06-02 08:11:44.418651 the-new-hotness-1.2.2/hotness/use_cases/notify_user_use_case.py
--rw-r--r--   0        0        0     2011 2022-06-02 08:11:44.418651 the-new-hotness-1.2.2/hotness/use_cases/package_check_use_case.py
--rw-r--r--   0        0        0     1982 2022-06-02 08:11:44.418651 the-new-hotness-1.2.2/hotness/use_cases/package_scratch_build_use_case.py
--rw-r--r--   0        0        0     1991 2022-06-02 08:11:44.418651 the-new-hotness-1.2.2/hotness/use_cases/retrieve_data_use_case.py
--rw-r--r--   0        0        0     2061 2022-06-02 08:11:44.418651 the-new-hotness-1.2.2/hotness/use_cases/submit_patch_use_case.py
--rw-r--r--   0        0        0      931 2022-06-02 08:11:44.418651 the-new-hotness-1.2.2/hotness/validators/__init__.py
--rw-r--r--   0        0        0     5409 2022-06-02 08:11:44.418651 the-new-hotness-1.2.2/hotness/validators/mdapi.py
--rw-r--r--   0        0        0     5768 2022-06-02 08:11:44.418651 the-new-hotness-1.2.2/hotness/validators/pagure.py
--rw-r--r--   0        0        0     3597 2022-06-02 08:11:44.418651 the-new-hotness-1.2.2/hotness/validators/pdc.py
--rw-r--r--   0        0        0     1309 2022-06-02 08:11:44.419651 the-new-hotness-1.2.2/hotness/validators/validator.py
--rw-r--r--   0        0        0     2482 2023-02-08 13:25:52.634923 the-new-hotness-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     2586 2023-02-08 13:26:55.676781 the-new-hotness-1.2.2/setup.py
--rw-r--r--   0        0        0     2542 2023-02-08 13:26:55.677095 the-new-hotness-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0    26530 2021-01-25 12:20:24.199782 the_new_hotness-1.2.3/LICENSE
+-rw-r--r--   0        0        0     1369 2023-04-21 13:07:13.379253 the_new_hotness-1.2.3/README.rst
+-rw-r--r--   0        0        0     5389 2023-04-21 13:07:13.379253 the_new_hotness-1.2.3/config/config.toml.example
+-rw-r--r--   0        0        0      288 2023-04-21 13:07:13.383253 the_new_hotness-1.2.3/hotness/__init__.py
+-rw-r--r--   0        0        0      849 2022-06-02 08:11:44.409651 the_new_hotness-1.2.3/hotness/builders/__init__.py
+-rw-r--r--   0        0        0      230 2022-06-02 10:01:53.714952 the_new_hotness-1.2.3/hotness/builders/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      188 2021-10-06 15:16:54.694389 the_new_hotness-1.2.3/hotness/builders/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0      192 2021-10-06 15:19:39.044410 the_new_hotness-1.2.3/hotness/builders/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      228 2022-06-02 10:11:44.818772 the_new_hotness-1.2.3/hotness/builders/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      228 2022-06-02 10:11:58.409806 the_new_hotness-1.2.3/hotness/builders/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1093 2022-06-02 10:01:53.714952 the_new_hotness-1.2.3/hotness/builders/__pycache__/builder.cpython-310.pyc
+-rw-r--r--   0        0        0     1044 2021-10-06 15:16:54.695389 the_new_hotness-1.2.3/hotness/builders/__pycache__/builder.cpython-36.pyc
+-rw-r--r--   0        0        0     1048 2021-10-06 15:19:39.046410 the_new_hotness-1.2.3/hotness/builders/__pycache__/builder.cpython-37.pyc
+-rw-r--r--   0        0        0     1092 2022-06-02 10:11:44.819772 the_new_hotness-1.2.3/hotness/builders/__pycache__/builder.cpython-38.pyc
+-rw-r--r--   0        0        0     1092 2022-06-02 10:11:58.416806 the_new_hotness-1.2.3/hotness/builders/__pycache__/builder.cpython-39.pyc
+-rw-r--r--   0        0        0    11853 2023-04-21 13:39:35.515484 the_new_hotness-1.2.3/hotness/builders/__pycache__/koji.cpython-310.pyc
+-rw-r--r--   0        0        0    11623 2021-12-07 12:17:58.425775 the_new_hotness-1.2.3/hotness/builders/__pycache__/koji.cpython-36.pyc
+-rw-r--r--   0        0        0    11607 2021-12-07 12:18:07.200803 the_new_hotness-1.2.3/hotness/builders/__pycache__/koji.cpython-37.pyc
+-rw-r--r--   0        0        0    11754 2023-03-08 14:49:46.320328 the_new_hotness-1.2.3/hotness/builders/__pycache__/koji.cpython-38.pyc
+-rw-r--r--   0        0        0    11822 2023-03-08 14:49:56.474381 the_new_hotness-1.2.3/hotness/builders/__pycache__/koji.cpython-39.pyc
+-rw-r--r--   0        0        0     1467 2022-06-02 08:11:44.409651 the_new_hotness-1.2.3/hotness/builders/builder.py
+-rw-r--r--   0        0        0    18241 2023-04-24 10:44:45.364657 the_new_hotness-1.2.3/hotness/builders/koji.py
+-rw-r--r--   0        0        0      804 2022-06-02 08:11:44.409651 the_new_hotness-1.2.3/hotness/common/__init__.py
+-rw-r--r--   0        0        0      187 2022-06-02 10:01:54.135952 the_new_hotness-1.2.3/hotness/common/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      145 2021-10-06 15:16:55.442389 the_new_hotness-1.2.3/hotness/common/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0      149 2021-10-06 15:19:39.934411 the_new_hotness-1.2.3/hotness/common/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      185 2022-06-02 10:11:45.270773 the_new_hotness-1.2.3/hotness/common/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      185 2022-06-02 10:11:58.925807 the_new_hotness-1.2.3/hotness/common/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3220 2023-04-21 13:39:35.949486 the_new_hotness-1.2.3/hotness/common/__pycache__/rpm.cpython-310.pyc
+-rw-r--r--   0        0        0     3229 2021-10-06 15:16:55.443389 the_new_hotness-1.2.3/hotness/common/__pycache__/rpm.cpython-36.pyc
+-rw-r--r--   0        0        0     3213 2021-10-06 15:19:39.935411 the_new_hotness-1.2.3/hotness/common/__pycache__/rpm.cpython-37.pyc
+-rw-r--r--   0        0        0     3207 2022-06-02 10:11:45.272773 the_new_hotness-1.2.3/hotness/common/__pycache__/rpm.cpython-38.pyc
+-rw-r--r--   0        0        0     3205 2022-06-02 10:11:58.926807 the_new_hotness-1.2.3/hotness/common/__pycache__/rpm.cpython-39.pyc
+-rw-r--r--   0        0        0     5876 2023-04-21 13:07:13.384253 the_new_hotness-1.2.3/hotness/common/rpm.py
+-rw-r--r--   0        0        0     6329 2023-04-21 13:07:13.384253 the_new_hotness-1.2.3/hotness/config.py
+-rw-r--r--   0        0        0      897 2023-04-21 13:07:13.384253 the_new_hotness-1.2.3/hotness/databases/__init__.py
+-rw-r--r--   0        0        0      270 2023-04-21 13:39:35.596484 the_new_hotness-1.2.3/hotness/databases/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      193 2021-10-06 15:16:54.828389 the_new_hotness-1.2.3/hotness/databases/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0      197 2021-10-06 15:19:39.254410 the_new_hotness-1.2.3/hotness/databases/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      268 2022-06-02 10:11:44.921772 the_new_hotness-1.2.3/hotness/databases/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      268 2022-06-02 10:11:58.533806 the_new_hotness-1.2.3/hotness/databases/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2221 2023-04-21 13:39:35.598484 the_new_hotness-1.2.3/hotness/databases/__pycache__/cache.cpython-310.pyc
+-rw-r--r--   0        0        0     2141 2021-10-06 15:16:54.830389 the_new_hotness-1.2.3/hotness/databases/__pycache__/cache.cpython-36.pyc
+-rw-r--r--   0        0        0     2145 2021-10-06 15:19:39.257410 the_new_hotness-1.2.3/hotness/databases/__pycache__/cache.cpython-37.pyc
+-rw-r--r--   0        0        0     2228 2022-06-02 10:11:44.922772 the_new_hotness-1.2.3/hotness/databases/__pycache__/cache.cpython-38.pyc
+-rw-r--r--   0        0        0     2228 2022-06-02 10:11:58.534806 the_new_hotness-1.2.3/hotness/databases/__pycache__/cache.cpython-39.pyc
+-rw-r--r--   0        0        0     1464 2022-06-02 10:01:53.814952 the_new_hotness-1.2.3/hotness/databases/__pycache__/database.cpython-310.pyc
+-rw-r--r--   0        0        0     1434 2021-10-06 15:16:54.829389 the_new_hotness-1.2.3/hotness/databases/__pycache__/database.cpython-36.pyc
+-rw-r--r--   0        0        0     1438 2021-10-06 15:19:39.255411 the_new_hotness-1.2.3/hotness/databases/__pycache__/database.cpython-37.pyc
+-rw-r--r--   0        0        0     1484 2022-06-02 10:11:44.922772 the_new_hotness-1.2.3/hotness/databases/__pycache__/database.cpython-38.pyc
+-rw-r--r--   0        0        0     1484 2022-06-02 10:11:58.533806 the_new_hotness-1.2.3/hotness/databases/__pycache__/database.cpython-39.pyc
+-rw-r--r--   0        0        0     2828 2023-04-21 13:39:35.601484 the_new_hotness-1.2.3/hotness/databases/__pycache__/redis.cpython-310.pyc
+-rw-r--r--   0        0        0     2821 2022-10-05 13:45:56.825878 the_new_hotness-1.2.3/hotness/databases/__pycache__/redis.cpython-38.pyc
+-rw-r--r--   0        0        0     2815 2022-10-05 13:47:00.536070 the_new_hotness-1.2.3/hotness/databases/__pycache__/redis.cpython-39.pyc
+-rw-r--r--   0        0        0     2511 2023-04-21 13:07:13.384253 the_new_hotness-1.2.3/hotness/databases/cache.py
+-rw-r--r--   0        0        0     1803 2022-06-02 08:11:44.411651 the_new_hotness-1.2.3/hotness/databases/database.py
+-rw-r--r--   0        0        0     3609 2023-04-21 13:07:13.385253 the_new_hotness-1.2.3/hotness/databases/redis.py
+-rw-r--r--   0        0        0      812 2022-06-02 08:11:44.411651 the_new_hotness-1.2.3/hotness/domain/__init__.py
+-rw-r--r--   0        0        0      195 2022-06-02 10:01:53.713952 the_new_hotness-1.2.3/hotness/domain/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      153 2021-10-06 15:16:54.691389 the_new_hotness-1.2.3/hotness/domain/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0      157 2021-10-06 15:19:39.038411 the_new_hotness-1.2.3/hotness/domain/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      193 2022-06-02 10:11:44.817772 the_new_hotness-1.2.3/hotness/domain/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      193 2022-06-02 10:11:58.408806 the_new_hotness-1.2.3/hotness/domain/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1775 2023-04-21 13:39:35.512484 the_new_hotness-1.2.3/hotness/domain/__pycache__/package.cpython-310.pyc
+-rw-r--r--   0        0        0     1760 2021-10-06 15:16:54.693389 the_new_hotness-1.2.3/hotness/domain/__pycache__/package.cpython-36.pyc
+-rw-r--r--   0        0        0     1764 2021-10-06 15:19:39.041411 the_new_hotness-1.2.3/hotness/domain/__pycache__/package.cpython-37.pyc
+-rw-r--r--   0        0        0     1784 2022-06-02 10:11:44.817772 the_new_hotness-1.2.3/hotness/domain/__pycache__/package.cpython-38.pyc
+-rw-r--r--   0        0        0     1784 2022-06-02 10:11:58.409806 the_new_hotness-1.2.3/hotness/domain/__pycache__/package.cpython-39.pyc
+-rw-r--r--   0        0        0     2181 2023-04-21 13:07:13.385253 the_new_hotness-1.2.3/hotness/domain/package.py
+-rw-r--r--   0        0        0     1140 2023-04-21 13:07:13.385253 the_new_hotness-1.2.3/hotness/exceptions/__init__.py
+-rw-r--r--   0        0        0      507 2023-04-21 13:39:35.592484 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      497 2021-12-07 12:17:58.506775 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0      501 2021-12-07 12:18:07.281803 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      505 2022-06-02 10:11:44.917772 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      505 2022-06-02 10:11:58.527806 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1299 2023-04-21 13:39:35.592484 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/base_exception.cpython-310.pyc
+-rw-r--r--   0        0        0     1268 2021-12-07 12:17:58.507775 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/base_exception.cpython-36.pyc
+-rw-r--r--   0        0        0     1272 2021-12-07 12:18:07.282803 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/base_exception.cpython-37.pyc
+-rw-r--r--   0        0        0     1294 2022-06-02 10:11:44.918772 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/base_exception.cpython-38.pyc
+-rw-r--r--   0        0        0     1294 2022-06-02 10:11:58.528806 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/base_exception.cpython-39.pyc
+-rw-r--r--   0        0        0     1788 2023-04-21 13:39:35.593484 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/builder_exception.cpython-310.pyc
+-rw-r--r--   0        0        0     1736 2021-12-07 12:17:58.507775 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/builder_exception.cpython-36.pyc
+-rw-r--r--   0        0        0     1740 2021-12-07 12:18:07.283804 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/builder_exception.cpython-37.pyc
+-rw-r--r--   0        0        0     1779 2022-06-02 10:11:44.919772 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/builder_exception.cpython-38.pyc
+-rw-r--r--   0        0        0     1779 2022-06-02 10:11:58.529806 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/builder_exception.cpython-39.pyc
+-rw-r--r--   0        0        0      841 2023-04-21 13:39:35.594484 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/download_exception.cpython-310.pyc
+-rw-r--r--   0        0        0      825 2021-12-07 12:17:58.508775 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/download_exception.cpython-36.pyc
+-rw-r--r--   0        0        0      829 2021-12-07 12:18:07.283804 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/download_exception.cpython-37.pyc
+-rw-r--r--   0        0        0      839 2022-06-02 10:11:44.919772 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/download_exception.cpython-38.pyc
+-rw-r--r--   0        0        0      839 2022-06-02 10:11:58.530806 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/download_exception.cpython-39.pyc
+-rw-r--r--   0        0        0     1122 2021-04-12 11:42:23.041453 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/html_exception.cpython-39.pyc
+-rw-r--r--   0        0        0     1168 2023-04-21 13:39:35.595484 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/http_exception.cpython-310.pyc
+-rw-r--r--   0        0        0     1146 2021-12-07 12:17:58.508775 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/http_exception.cpython-36.pyc
+-rw-r--r--   0        0        0     1150 2021-12-07 12:18:07.284803 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/http_exception.cpython-37.pyc
+-rw-r--r--   0        0        0     1157 2022-06-02 10:11:44.920772 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/http_exception.cpython-38.pyc
+-rw-r--r--   0        0        0     1157 2022-06-02 10:11:58.531806 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/http_exception.cpython-39.pyc
+-rw-r--r--   0        0        0      876 2023-04-21 13:39:35.595484 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/notifier_exception.cpython-310.pyc
+-rw-r--r--   0        0        0      858 2021-12-07 12:17:58.509775 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/notifier_exception.cpython-36.pyc
+-rw-r--r--   0        0        0      862 2021-12-07 12:18:07.284803 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/notifier_exception.cpython-37.pyc
+-rw-r--r--   0        0        0      872 2022-06-02 10:11:44.920772 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/notifier_exception.cpython-38.pyc
+-rw-r--r--   0        0        0      872 2022-06-02 10:11:58.531806 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/notifier_exception.cpython-39.pyc
+-rw-r--r--   0        0        0      841 2023-04-21 13:39:35.596484 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/patcher_exception.cpython-310.pyc
+-rw-r--r--   0        0        0      823 2021-12-07 12:17:58.509775 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/patcher_exception.cpython-36.pyc
+-rw-r--r--   0        0        0      827 2021-12-07 12:18:07.285803 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/patcher_exception.cpython-37.pyc
+-rw-r--r--   0        0        0      837 2022-06-02 10:11:44.921772 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/patcher_exception.cpython-38.pyc
+-rw-r--r--   0        0        0      837 2022-06-02 10:11:58.532806 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/patcher_exception.cpython-39.pyc
+-rw-r--r--   0        0        0     1602 2023-04-21 13:07:13.386253 the_new_hotness-1.2.3/hotness/exceptions/base_exception.py
+-rw-r--r--   0        0        0     2438 2023-04-21 13:07:13.386253 the_new_hotness-1.2.3/hotness/exceptions/builder_exception.py
+-rw-r--r--   0        0        0     1223 2023-04-21 13:07:13.386253 the_new_hotness-1.2.3/hotness/exceptions/download_exception.py
+-rw-r--r--   0        0        0     1513 2023-04-21 13:07:13.387253 the_new_hotness-1.2.3/hotness/exceptions/http_exception.py
+-rw-r--r--   0        0        0     1253 2023-04-21 13:07:13.387253 the_new_hotness-1.2.3/hotness/exceptions/notifier_exception.py
+-rw-r--r--   0        0        0     1219 2023-04-21 13:07:13.387253 the_new_hotness-1.2.3/hotness/exceptions/patcher_exception.py
+-rw-r--r--   0        0        0    28765 2023-04-24 10:44:45.366658 the_new_hotness-1.2.3/hotness/hotness_consumer.py
+-rw-r--r--   0        0        0      919 2022-06-02 08:11:44.414651 the_new_hotness-1.2.3/hotness/notifiers/__init__.py
+-rw-r--r--   0        0        0      297 2022-06-02 10:01:53.841952 the_new_hotness-1.2.3/hotness/notifiers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      255 2021-10-06 15:16:54.831389 the_new_hotness-1.2.3/hotness/notifiers/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0      259 2021-10-06 15:19:39.259410 the_new_hotness-1.2.3/hotness/notifiers/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      295 2022-06-02 10:11:44.949772 the_new_hotness-1.2.3/hotness/notifiers/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      295 2022-06-02 10:11:58.570806 the_new_hotness-1.2.3/hotness/notifiers/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     7855 2023-04-21 13:39:35.637484 the_new_hotness-1.2.3/hotness/notifiers/__pycache__/bugzilla.cpython-310.pyc
+-rw-r--r--   0        0        0     8123 2021-11-23 15:45:23.344454 the_new_hotness-1.2.3/hotness/notifiers/__pycache__/bugzilla.cpython-36.pyc
+-rw-r--r--   0        0        0     7802 2022-02-10 13:19:26.228272 the_new_hotness-1.2.3/hotness/notifiers/__pycache__/bugzilla.cpython-37.pyc
+-rw-r--r--   0        0        0     7872 2022-06-02 10:11:44.951772 the_new_hotness-1.2.3/hotness/notifiers/__pycache__/bugzilla.cpython-38.pyc
+-rw-r--r--   0        0        0     7842 2022-06-02 10:11:58.572806 the_new_hotness-1.2.3/hotness/notifiers/__pycache__/bugzilla.cpython-39.pyc
+-rw-r--r--   0        0        0     2995 2023-04-21 13:39:35.645484 the_new_hotness-1.2.3/hotness/notifiers/__pycache__/fedora_messaging.cpython-310.pyc
+-rw-r--r--   0        0        0     2972 2021-11-23 15:45:23.352454 the_new_hotness-1.2.3/hotness/notifiers/__pycache__/fedora_messaging.cpython-36.pyc
+-rw-r--r--   0        0        0     2976 2021-11-23 15:45:33.176491 the_new_hotness-1.2.3/hotness/notifiers/__pycache__/fedora_messaging.cpython-37.pyc
+-rw-r--r--   0        0        0     2994 2022-06-02 10:11:44.960772 the_new_hotness-1.2.3/hotness/notifiers/__pycache__/fedora_messaging.cpython-38.pyc
+-rw-r--r--   0        0        0     3008 2022-06-02 10:11:58.585806 the_new_hotness-1.2.3/hotness/notifiers/__pycache__/fedora_messaging.cpython-39.pyc
+-rw-r--r--   0        0        0     1302 2022-06-02 10:01:53.841952 the_new_hotness-1.2.3/hotness/notifiers/__pycache__/notifier.cpython-310.pyc
+-rw-r--r--   0        0        0     1251 2021-10-06 15:16:54.832389 the_new_hotness-1.2.3/hotness/notifiers/__pycache__/notifier.cpython-36.pyc
+-rw-r--r--   0        0        0     1255 2021-10-06 15:19:39.261411 the_new_hotness-1.2.3/hotness/notifiers/__pycache__/notifier.cpython-37.pyc
+-rw-r--r--   0        0        0     1299 2022-06-02 10:11:44.949772 the_new_hotness-1.2.3/hotness/notifiers/__pycache__/notifier.cpython-38.pyc
+-rw-r--r--   0        0        0     1299 2022-06-02 10:11:58.571807 the_new_hotness-1.2.3/hotness/notifiers/__pycache__/notifier.cpython-39.pyc
+-rw-r--r--   0        0        0    10095 2023-04-21 13:07:13.388253 the_new_hotness-1.2.3/hotness/notifiers/bugzilla.py
+-rw-r--r--   0        0        0     3552 2023-04-21 13:07:13.388253 the_new_hotness-1.2.3/hotness/notifiers/fedora_messaging.py
+-rw-r--r--   0        0        0     1663 2022-06-02 08:11:44.416651 the_new_hotness-1.2.3/hotness/notifiers/notifier.py
+-rw-r--r--   0        0        0      857 2022-06-02 08:11:44.416651 the_new_hotness-1.2.3/hotness/patchers/__init__.py
+-rw-r--r--   0        0        0      238 2022-06-02 10:01:54.130952 the_new_hotness-1.2.3/hotness/patchers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      196 2021-10-06 15:16:55.434389 the_new_hotness-1.2.3/hotness/patchers/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0      200 2021-10-06 15:19:39.925411 the_new_hotness-1.2.3/hotness/patchers/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      236 2022-06-02 10:11:45.261773 the_new_hotness-1.2.3/hotness/patchers/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      236 2022-06-02 10:11:58.921807 the_new_hotness-1.2.3/hotness/patchers/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3249 2023-04-21 13:39:35.946486 the_new_hotness-1.2.3/hotness/patchers/__pycache__/bugzilla.cpython-310.pyc
+-rw-r--r--   0        0        0     3480 2021-11-23 15:45:23.640455 the_new_hotness-1.2.3/hotness/patchers/__pycache__/bugzilla.cpython-36.pyc
+-rw-r--r--   0        0        0     3176 2022-02-10 13:25:53.423747 the_new_hotness-1.2.3/hotness/patchers/__pycache__/bugzilla.cpython-37.pyc
+-rw-r--r--   0        0        0     3199 2022-06-02 10:11:45.265773 the_new_hotness-1.2.3/hotness/patchers/__pycache__/bugzilla.cpython-38.pyc
+-rw-r--r--   0        0        0     3234 2022-06-02 10:11:58.922807 the_new_hotness-1.2.3/hotness/patchers/__pycache__/bugzilla.cpython-39.pyc
+-rw-r--r--   0        0        0     5239 2022-04-14 10:12:40.509773 the_new_hotness-1.2.3/hotness/patchers/__pycache__/pagure.cpython-38.pyc
+-rw-r--r--   0        0        0     5451 2021-07-22 11:18:54.809605 the_new_hotness-1.2.3/hotness/patchers/__pycache__/pagure.cpython-39.pyc
+-rw-r--r--   0        0        0     1249 2022-06-02 10:01:54.131952 the_new_hotness-1.2.3/hotness/patchers/__pycache__/patcher.cpython-310.pyc
+-rw-r--r--   0        0        0     1198 2021-10-06 15:16:55.435389 the_new_hotness-1.2.3/hotness/patchers/__pycache__/patcher.cpython-36.pyc
+-rw-r--r--   0        0        0     1202 2021-10-06 15:19:39.926411 the_new_hotness-1.2.3/hotness/patchers/__pycache__/patcher.cpython-37.pyc
+-rw-r--r--   0        0        0     1246 2022-06-02 10:11:45.263773 the_new_hotness-1.2.3/hotness/patchers/__pycache__/patcher.cpython-38.pyc
+-rw-r--r--   0        0        0     1246 2022-06-02 10:11:58.921807 the_new_hotness-1.2.3/hotness/patchers/__pycache__/patcher.cpython-39.pyc
+-rw-r--r--   0        0        0     4008 2023-04-21 13:07:13.388253 the_new_hotness-1.2.3/hotness/patchers/bugzilla.py
+-rw-r--r--   0        0        0     1607 2022-06-02 08:11:44.416651 the_new_hotness-1.2.3/hotness/patchers/patcher.py
+-rw-r--r--   0        0        0     1181 2022-06-02 08:11:44.416651 the_new_hotness-1.2.3/hotness/requests/__init__.py
+-rw-r--r--   0        0        0      542 2022-06-02 10:01:54.142952 the_new_hotness-1.2.3/hotness/requests/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      500 2021-10-06 15:16:55.450389 the_new_hotness-1.2.3/hotness/requests/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0      504 2021-10-06 15:19:39.944411 the_new_hotness-1.2.3/hotness/requests/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      540 2022-06-02 10:11:45.283773 the_new_hotness-1.2.3/hotness/requests/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      540 2022-06-02 10:11:58.932807 the_new_hotness-1.2.3/hotness/requests/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      939 2022-06-02 10:01:54.143952 the_new_hotness-1.2.3/hotness/requests/__pycache__/build_request.cpython-310.pyc
+-rw-r--r--   0        0        0      887 2021-10-06 15:16:55.452389 the_new_hotness-1.2.3/hotness/requests/__pycache__/build_request.cpython-36.pyc
+-rw-r--r--   0        0        0      891 2021-10-06 15:19:39.950410 the_new_hotness-1.2.3/hotness/requests/__pycache__/build_request.cpython-37.pyc
+-rw-r--r--   0        0        0      933 2022-06-02 10:11:45.286773 the_new_hotness-1.2.3/hotness/requests/__pycache__/build_request.cpython-38.pyc
+-rw-r--r--   0        0        0      933 2022-06-02 10:11:58.934807 the_new_hotness-1.2.3/hotness/requests/__pycache__/build_request.cpython-39.pyc
+-rw-r--r--   0        0        0      897 2022-06-02 10:01:54.145952 the_new_hotness-1.2.3/hotness/requests/__pycache__/insert_data_request.cpython-310.pyc
+-rw-r--r--   0        0        0      845 2021-10-06 15:16:55.456389 the_new_hotness-1.2.3/hotness/requests/__pycache__/insert_data_request.cpython-36.pyc
+-rw-r--r--   0        0        0      849 2021-10-06 15:19:39.954411 the_new_hotness-1.2.3/hotness/requests/__pycache__/insert_data_request.cpython-37.pyc
+-rw-r--r--   0        0        0      891 2022-06-02 10:11:45.289773 the_new_hotness-1.2.3/hotness/requests/__pycache__/insert_data_request.cpython-38.pyc
+-rw-r--r--   0        0        0      891 2022-06-02 10:11:58.935807 the_new_hotness-1.2.3/hotness/requests/__pycache__/insert_data_request.cpython-39.pyc
+-rw-r--r--   0        0        0     1041 2022-06-02 10:01:54.144952 the_new_hotness-1.2.3/hotness/requests/__pycache__/notify_request.cpython-310.pyc
+-rw-r--r--   0        0        0      987 2021-10-06 15:16:55.453389 the_new_hotness-1.2.3/hotness/requests/__pycache__/notify_request.cpython-36.pyc
+-rw-r--r--   0        0        0      991 2021-10-06 15:19:39.951411 the_new_hotness-1.2.3/hotness/requests/__pycache__/notify_request.cpython-37.pyc
+-rw-r--r--   0        0        0     1033 2022-06-02 10:11:45.287773 the_new_hotness-1.2.3/hotness/requests/__pycache__/notify_request.cpython-38.pyc
+-rw-r--r--   0        0        0     1033 2022-06-02 10:11:58.934807 the_new_hotness-1.2.3/hotness/requests/__pycache__/notify_request.cpython-39.pyc
+-rw-r--r--   0        0        0      885 2022-06-02 10:01:54.143952 the_new_hotness-1.2.3/hotness/requests/__pycache__/package_request.cpython-310.pyc
+-rw-r--r--   0        0        0      835 2021-10-06 15:16:55.452389 the_new_hotness-1.2.3/hotness/requests/__pycache__/package_request.cpython-36.pyc
+-rw-r--r--   0        0        0      839 2021-10-06 15:19:39.949411 the_new_hotness-1.2.3/hotness/requests/__pycache__/package_request.cpython-37.pyc
+-rw-r--r--   0        0        0      881 2022-06-02 10:11:45.285773 the_new_hotness-1.2.3/hotness/requests/__pycache__/package_request.cpython-38.pyc
+-rw-r--r--   0        0        0      881 2022-06-02 10:11:58.933807 the_new_hotness-1.2.3/hotness/requests/__pycache__/package_request.cpython-39.pyc
+-rw-r--r--   0        0        0     1632 2023-04-21 13:39:35.955486 the_new_hotness-1.2.3/hotness/requests/__pycache__/request.cpython-310.pyc
+-rw-r--r--   0        0        0     1537 2021-10-06 15:16:55.451389 the_new_hotness-1.2.3/hotness/requests/__pycache__/request.cpython-36.pyc
+-rw-r--r--   0        0        0     1541 2021-10-06 15:19:39.947410 the_new_hotness-1.2.3/hotness/requests/__pycache__/request.cpython-37.pyc
+-rw-r--r--   0        0        0     1629 2022-06-02 10:11:45.284773 the_new_hotness-1.2.3/hotness/requests/__pycache__/request.cpython-38.pyc
+-rw-r--r--   0        0        0     1629 2022-06-02 10:11:58.933807 the_new_hotness-1.2.3/hotness/requests/__pycache__/request.cpython-39.pyc
+-rw-r--r--   0        0        0      805 2022-06-02 10:01:54.145952 the_new_hotness-1.2.3/hotness/requests/__pycache__/retrieve_data_request.cpython-310.pyc
+-rw-r--r--   0        0        0      755 2021-10-06 15:16:55.457389 the_new_hotness-1.2.3/hotness/requests/__pycache__/retrieve_data_request.cpython-36.pyc
+-rw-r--r--   0        0        0      759 2021-10-06 15:19:39.956411 the_new_hotness-1.2.3/hotness/requests/__pycache__/retrieve_data_request.cpython-37.pyc
+-rw-r--r--   0        0        0      801 2022-06-02 10:11:45.290773 the_new_hotness-1.2.3/hotness/requests/__pycache__/retrieve_data_request.cpython-38.pyc
+-rw-r--r--   0        0        0      801 2022-06-02 10:11:58.936807 the_new_hotness-1.2.3/hotness/requests/__pycache__/retrieve_data_request.cpython-39.pyc
+-rw-r--r--   0        0        0     1046 2022-06-02 10:01:54.144952 the_new_hotness-1.2.3/hotness/requests/__pycache__/submit_patch_request.cpython-310.pyc
+-rw-r--r--   0        0        0      992 2021-10-06 15:16:55.454389 the_new_hotness-1.2.3/hotness/requests/__pycache__/submit_patch_request.cpython-36.pyc
+-rw-r--r--   0        0        0      996 2021-10-06 15:19:39.953410 the_new_hotness-1.2.3/hotness/requests/__pycache__/submit_patch_request.cpython-37.pyc
+-rw-r--r--   0        0        0     1038 2022-06-02 10:11:45.288773 the_new_hotness-1.2.3/hotness/requests/__pycache__/submit_patch_request.cpython-38.pyc
+-rw-r--r--   0        0        0     1038 2022-06-02 10:11:58.935807 the_new_hotness-1.2.3/hotness/requests/__pycache__/submit_patch_request.cpython-39.pyc
+-rw-r--r--   0        0        0     1287 2022-06-02 08:11:44.416651 the_new_hotness-1.2.3/hotness/requests/build_request.py
+-rw-r--r--   0        0        0     1256 2022-06-02 08:11:44.416651 the_new_hotness-1.2.3/hotness/requests/insert_data_request.py
+-rw-r--r--   0        0        0     1394 2022-06-02 08:11:44.416651 the_new_hotness-1.2.3/hotness/requests/notify_request.py
+-rw-r--r--   0        0        0     1234 2022-06-02 08:11:44.416651 the_new_hotness-1.2.3/hotness/requests/package_request.py
+-rw-r--r--   0        0        0     1905 2023-04-21 13:07:13.388253 the_new_hotness-1.2.3/hotness/requests/request.py
+-rw-r--r--   0        0        0     1152 2022-06-02 08:11:44.416651 the_new_hotness-1.2.3/hotness/requests/retrieve_data_request.py
+-rw-r--r--   0        0        0     1389 2022-06-02 08:11:44.416651 the_new_hotness-1.2.3/hotness/requests/submit_patch_request.py
+-rw-r--r--   0        0        0      934 2022-06-02 08:11:44.416651 the_new_hotness-1.2.3/hotness/responses/__init__.py
+-rw-r--r--   0        0        0      312 2022-06-02 10:01:54.139952 the_new_hotness-1.2.3/hotness/responses/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      270 2021-10-06 15:16:55.461389 the_new_hotness-1.2.3/hotness/responses/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0      274 2021-10-06 15:19:39.960410 the_new_hotness-1.2.3/hotness/responses/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      310 2022-06-02 10:11:45.278773 the_new_hotness-1.2.3/hotness/responses/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      310 2022-06-02 10:11:58.929807 the_new_hotness-1.2.3/hotness/responses/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1204 2022-06-02 10:01:54.140952 the_new_hotness-1.2.3/hotness/responses/__pycache__/response.cpython-310.pyc
+-rw-r--r--   0        0        0     1168 2021-10-06 15:16:55.463389 the_new_hotness-1.2.3/hotness/responses/__pycache__/response.cpython-36.pyc
+-rw-r--r--   0        0        0     1172 2021-10-06 15:19:39.962411 the_new_hotness-1.2.3/hotness/responses/__pycache__/response.cpython-37.pyc
+-rw-r--r--   0        0        0     1216 2022-06-02 10:11:45.279773 the_new_hotness-1.2.3/hotness/responses/__pycache__/response.cpython-38.pyc
+-rw-r--r--   0        0        0     1216 2022-06-02 10:11:58.930807 the_new_hotness-1.2.3/hotness/responses/__pycache__/response.cpython-39.pyc
+-rw-r--r--   0        0        0     5684 2023-04-21 13:39:35.954486 the_new_hotness-1.2.3/hotness/responses/__pycache__/response_failure.cpython-310.pyc
+-rw-r--r--   0        0        0     5749 2021-12-07 12:17:58.828776 the_new_hotness-1.2.3/hotness/responses/__pycache__/response_failure.cpython-36.pyc
+-rw-r--r--   0        0        0     5753 2021-12-07 12:18:07.544804 the_new_hotness-1.2.3/hotness/responses/__pycache__/response_failure.cpython-37.pyc
+-rw-r--r--   0        0        0     5774 2022-06-02 10:11:45.282773 the_new_hotness-1.2.3/hotness/responses/__pycache__/response_failure.cpython-38.pyc
+-rw-r--r--   0        0        0     5770 2022-06-02 10:11:58.932807 the_new_hotness-1.2.3/hotness/responses/__pycache__/response_failure.cpython-39.pyc
+-rw-r--r--   0        0        0     1389 2022-06-02 10:01:54.140952 the_new_hotness-1.2.3/hotness/responses/__pycache__/response_success.cpython-310.pyc
+-rw-r--r--   0        0        0     1338 2021-10-06 15:16:55.464389 the_new_hotness-1.2.3/hotness/responses/__pycache__/response_success.cpython-36.pyc
+-rw-r--r--   0        0        0     1342 2021-10-06 15:19:39.964411 the_new_hotness-1.2.3/hotness/responses/__pycache__/response_success.cpython-37.pyc
+-rw-r--r--   0        0        0     1392 2022-06-02 10:11:45.280773 the_new_hotness-1.2.3/hotness/responses/__pycache__/response_success.cpython-38.pyc
+-rw-r--r--   0        0        0     1392 2022-06-02 10:11:58.931807 the_new_hotness-1.2.3/hotness/responses/__pycache__/response_success.cpython-39.pyc
+-rw-r--r--   0        0        0     1540 2022-06-02 08:11:44.416651 the_new_hotness-1.2.3/hotness/responses/response.py
+-rw-r--r--   0        0        0     6212 2023-04-21 13:07:13.388253 the_new_hotness-1.2.3/hotness/responses/response_failure.py
+-rw-r--r--   0        0        0     1623 2022-06-02 08:11:44.418651 the_new_hotness-1.2.3/hotness/responses/response_success.py
+-rw-r--r--   0        0        0     1194 2022-06-02 08:11:44.418651 the_new_hotness-1.2.3/hotness/use_cases/__init__.py
+-rw-r--r--   0        0        0      560 2022-06-02 10:01:54.146952 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      518 2021-10-06 15:16:55.458389 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0      522 2021-10-06 15:19:39.958411 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      558 2022-06-02 10:11:45.291773 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      558 2022-06-02 10:11:58.937807 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1628 2022-06-02 10:01:54.147952 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/insert_data_use_case.cpython-310.pyc
+-rw-r--r--   0        0        0     1564 2021-10-06 15:16:55.460389 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/insert_data_use_case.cpython-36.pyc
+-rw-r--r--   0        0        0     1570 2021-10-06 15:19:39.959411 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/insert_data_use_case.cpython-37.pyc
+-rw-r--r--   0        0        0     1626 2022-06-02 10:11:45.292773 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/insert_data_use_case.cpython-38.pyc
+-rw-r--r--   0        0        0     1624 2022-06-02 10:11:58.937807 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/insert_data_use_case.cpython-39.pyc
+-rw-r--r--   0        0        0     1643 2022-06-02 10:01:54.149952 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/notify_user_use_case.cpython-310.pyc
+-rw-r--r--   0        0        0     1577 2021-10-06 15:16:55.472389 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/notify_user_use_case.cpython-36.pyc
+-rw-r--r--   0        0        0     1583 2021-10-06 15:19:39.972411 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/notify_user_use_case.cpython-37.pyc
+-rw-r--r--   0        0        0     1645 2022-06-02 10:11:45.296773 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/notify_user_use_case.cpython-38.pyc
+-rw-r--r--   0        0        0     1639 2022-06-02 10:11:58.940807 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/notify_user_use_case.cpython-39.pyc
+-rw-r--r--   0        0        0     1656 2022-06-02 10:01:54.148952 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/package_check_use_case.cpython-310.pyc
+-rw-r--r--   0        0        0     1592 2021-10-06 15:16:55.469389 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/package_check_use_case.cpython-36.pyc
+-rw-r--r--   0        0        0     1598 2021-10-06 15:19:39.969411 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/package_check_use_case.cpython-37.pyc
+-rw-r--r--   0        0        0     1654 2022-06-02 10:11:45.294773 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/package_check_use_case.cpython-38.pyc
+-rw-r--r--   0        0        0     1652 2022-06-02 10:11:58.939808 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/package_check_use_case.cpython-39.pyc
+-rw-r--r--   0        0        0     1655 2022-06-02 10:01:54.148952 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/package_scratch_build_use_case.cpython-310.pyc
+-rw-r--r--   0        0        0     1591 2021-10-06 15:16:55.471389 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/package_scratch_build_use_case.cpython-36.pyc
+-rw-r--r--   0        0        0     1597 2021-10-06 15:19:39.970410 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/package_scratch_build_use_case.cpython-37.pyc
+-rw-r--r--   0        0        0     1653 2022-06-02 10:11:45.295773 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/package_scratch_build_use_case.cpython-38.pyc
+-rw-r--r--   0        0        0     1651 2022-06-02 10:11:58.939808 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/package_scratch_build_use_case.cpython-39.pyc
+-rw-r--r--   0        0        0     1635 2022-06-02 10:01:54.147952 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/retrieve_data_use_case.cpython-310.pyc
+-rw-r--r--   0        0        0     1571 2021-10-06 15:16:55.467389 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/retrieve_data_use_case.cpython-36.pyc
+-rw-r--r--   0        0        0     1577 2021-10-06 15:19:39.968411 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/retrieve_data_use_case.cpython-37.pyc
+-rw-r--r--   0        0        0     1633 2022-06-02 10:11:45.293773 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/retrieve_data_use_case.cpython-38.pyc
+-rw-r--r--   0        0        0     1631 2022-06-02 10:11:58.938807 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/retrieve_data_use_case.cpython-39.pyc
+-rw-r--r--   0        0        0     1673 2022-06-02 10:01:54.149952 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/submit_patch_use_case.cpython-310.pyc
+-rw-r--r--   0        0        0     1607 2021-10-06 15:16:55.474389 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/submit_patch_use_case.cpython-36.pyc
+-rw-r--r--   0        0        0     1613 2021-10-06 15:19:39.973410 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/submit_patch_use_case.cpython-37.pyc
+-rw-r--r--   0        0        0     1675 2022-06-02 10:11:45.297773 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/submit_patch_use_case.cpython-38.pyc
+-rw-r--r--   0        0        0     1669 2022-06-02 10:11:58.941807 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/submit_patch_use_case.cpython-39.pyc
+-rw-r--r--   0        0        0     1992 2022-06-02 08:11:44.418651 the_new_hotness-1.2.3/hotness/use_cases/insert_data_use_case.py
+-rw-r--r--   0        0        0     2033 2022-06-02 08:11:44.418651 the_new_hotness-1.2.3/hotness/use_cases/notify_user_use_case.py
+-rw-r--r--   0        0        0     2011 2022-06-02 08:11:44.418651 the_new_hotness-1.2.3/hotness/use_cases/package_check_use_case.py
+-rw-r--r--   0        0        0     1982 2022-06-02 08:11:44.418651 the_new_hotness-1.2.3/hotness/use_cases/package_scratch_build_use_case.py
+-rw-r--r--   0        0        0     1991 2022-06-02 08:11:44.418651 the_new_hotness-1.2.3/hotness/use_cases/retrieve_data_use_case.py
+-rw-r--r--   0        0        0     2061 2022-06-02 08:11:44.418651 the_new_hotness-1.2.3/hotness/use_cases/submit_patch_use_case.py
+-rw-r--r--   0        0        0      931 2022-06-02 08:11:44.418651 the_new_hotness-1.2.3/hotness/validators/__init__.py
+-rw-r--r--   0        0        0      306 2022-06-02 10:01:54.133952 the_new_hotness-1.2.3/hotness/validators/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      264 2021-10-06 15:16:55.438389 the_new_hotness-1.2.3/hotness/validators/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0      268 2021-10-06 15:19:39.929411 the_new_hotness-1.2.3/hotness/validators/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      304 2022-06-02 10:11:45.266773 the_new_hotness-1.2.3/hotness/validators/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      304 2022-06-02 10:11:58.923807 the_new_hotness-1.2.3/hotness/validators/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4391 2023-04-21 13:39:35.948486 the_new_hotness-1.2.3/hotness/validators/__pycache__/mdapi.cpython-310.pyc
+-rw-r--r--   0        0        0     3518 2021-10-06 15:16:55.440389 the_new_hotness-1.2.3/hotness/validators/__pycache__/mdapi.cpython-36.pyc
+-rw-r--r--   0        0        0     3517 2021-10-06 15:19:39.932411 the_new_hotness-1.2.3/hotness/validators/__pycache__/mdapi.cpython-37.pyc
+-rw-r--r--   0        0        0     4391 2022-06-02 10:11:45.269773 the_new_hotness-1.2.3/hotness/validators/__pycache__/mdapi.cpython-38.pyc
+-rw-r--r--   0        0        0     4391 2022-06-02 10:11:58.924807 the_new_hotness-1.2.3/hotness/validators/__pycache__/mdapi.cpython-39.pyc
+-rw-r--r--   0        0        0     3522 2023-04-21 13:39:35.951486 the_new_hotness-1.2.3/hotness/validators/__pycache__/pagure.cpython-310.pyc
+-rw-r--r--   0        0        0     2787 2021-10-06 15:16:55.447389 the_new_hotness-1.2.3/hotness/validators/__pycache__/pagure.cpython-36.pyc
+-rw-r--r--   0        0        0     2791 2021-10-06 15:19:39.941411 the_new_hotness-1.2.3/hotness/validators/__pycache__/pagure.cpython-37.pyc
+-rw-r--r--   0        0        0     3526 2022-06-02 10:11:45.275773 the_new_hotness-1.2.3/hotness/validators/__pycache__/pagure.cpython-38.pyc
+-rw-r--r--   0        0        0     3511 2022-06-02 10:11:58.928807 the_new_hotness-1.2.3/hotness/validators/__pycache__/pagure.cpython-39.pyc
+-rw-r--r--   0        0        0     2817 2023-04-21 13:39:35.952486 the_new_hotness-1.2.3/hotness/validators/__pycache__/pdc.cpython-310.pyc
+-rw-r--r--   0        0        0     2619 2021-10-06 15:16:55.449389 the_new_hotness-1.2.3/hotness/validators/__pycache__/pdc.cpython-36.pyc
+-rw-r--r--   0        0        0     2623 2021-10-06 15:19:39.942411 the_new_hotness-1.2.3/hotness/validators/__pycache__/pdc.cpython-37.pyc
+-rw-r--r--   0        0        0     2804 2022-06-02 10:11:45.276773 the_new_hotness-1.2.3/hotness/validators/__pycache__/pdc.cpython-38.pyc
+-rw-r--r--   0        0        0     2798 2022-06-02 10:11:58.929807 the_new_hotness-1.2.3/hotness/validators/__pycache__/pdc.cpython-39.pyc
+-rw-r--r--   0        0        0      938 2022-06-02 10:01:54.133952 the_new_hotness-1.2.3/hotness/validators/__pycache__/validator.cpython-310.pyc
+-rw-r--r--   0        0        0      891 2021-10-06 15:16:55.439389 the_new_hotness-1.2.3/hotness/validators/__pycache__/validator.cpython-36.pyc
+-rw-r--r--   0        0        0      895 2021-10-06 15:19:39.930410 the_new_hotness-1.2.3/hotness/validators/__pycache__/validator.cpython-37.pyc
+-rw-r--r--   0        0        0      939 2022-06-02 10:11:45.267773 the_new_hotness-1.2.3/hotness/validators/__pycache__/validator.cpython-38.pyc
+-rw-r--r--   0        0        0      939 2022-06-02 10:11:58.923807 the_new_hotness-1.2.3/hotness/validators/__pycache__/validator.cpython-39.pyc
+-rw-r--r--   0        0        0     5409 2023-04-21 13:07:13.389253 the_new_hotness-1.2.3/hotness/validators/mdapi.py
+-rw-r--r--   0        0        0     5768 2023-04-21 13:07:13.389253 the_new_hotness-1.2.3/hotness/validators/pagure.py
+-rw-r--r--   0        0        0     3597 2023-04-21 13:07:13.389253 the_new_hotness-1.2.3/hotness/validators/pdc.py
+-rw-r--r--   0        0        0     1309 2022-06-02 08:11:44.419651 the_new_hotness-1.2.3/hotness/validators/validator.py
+-rw-r--r--   0        0        0     2482 2023-04-24 14:30:13.547842 the_new_hotness-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2586 1970-01-01 00:00:00.000000 the_new_hotness-1.2.3/setup.py
+-rw-r--r--   0        0        0     2694 1970-01-01 00:00:00.000000 the_new_hotness-1.2.3/PKG-INFO
```

### Comparing `the-new-hotness-1.2.2/LICENSE` & `the_new_hotness-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/README.rst` & `the_new_hotness-1.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/config/config.toml.example` & `the_new_hotness-1.2.3/config/config.toml.example`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/builders/__init__.py` & `the_new_hotness-1.2.3/hotness/builders/__init__.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/builders/builder.py` & `the_new_hotness-1.2.3/hotness/builders/builder.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/builders/koji.py` & `the_new_hotness-1.2.3/hotness/builders/koji.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,14 +152,51 @@
                 std_err = ""
                 if exc.stdout:
                     std_out = exc.stdout.decode()
                 if exc.stderr:
                     std_err = exc.stderr.decode()
                 raise BuilderException(str(exc), std_out=std_out, std_err=std_err)
 
+            # Now, craft a patch to attach to the ticket
+            try:
+                sp.check_output(
+                    ["git", "config", "user.name", self.user_email[0]],
+                    cwd=tmp,
+                    stderr=sp.STDOUT,
+                )
+                sp.check_output(
+                    ["git", "config", "user.email", self.user_email[1]],
+                    cwd=tmp,
+                    stderr=sp.STDOUT,
+                )
+                sp.check_output(
+                    ["git", "commit", "-a", "-m", comment], cwd=tmp, stderr=sp.STDOUT
+                )
+                filename = sp.check_output(
+                    ["git", "format-patch", "HEAD^"], cwd=tmp, stderr=sp.STDOUT
+                )
+                filename_str = filename.decode("utf-8").strip()
+            except sp.CalledProcessError as exc:
+                std_out = ""
+                std_err = ""
+                if exc.stdout:
+                    std_out = exc.stdout.decode()
+                if exc.stderr:
+                    std_err = exc.stderr.decode()
+                raise BuilderException(
+                    str(exc), value=output, std_out=std_out, std_err=std_err
+                )
+
+            output["patch_filename"] = filename_str
+
+            # Copy the content of file to output
+            patch = os.path.join(tmp, filename_str)
+            with open(patch) as f:
+                output["patch"] = f.read()
+
             # We compare the old sources to the new ones to make sure we download
             # new sources from bumping the specfile version. Some packages don't
             # use macros in the source URL(s). We want to detect these and notify
             # the packager on the bug we filed about the new version.
             old_sources = self._dist_git_sources(tmp)
             new_sources = self._spec_sources(specfile, tmp)
             output["message"] = self._compare_sources(old_sources, new_sources)
@@ -193,51 +230,14 @@
             _logger.debug("Got srpm %r" % srpm)
 
             session = self._session_maker()
             if not session:
                 raise BuilderException("Can't authenticate with Koji!")
             output["build_id"] = self._scratch_build(session, package.name, srpm)
 
-            # Now, craft a patch to attach to the ticket
-            try:
-                sp.check_output(
-                    ["git", "config", "user.name", self.user_email[0]],
-                    cwd=tmp,
-                    stderr=sp.STDOUT,
-                )
-                sp.check_output(
-                    ["git", "config", "user.email", self.user_email[1]],
-                    cwd=tmp,
-                    stderr=sp.STDOUT,
-                )
-                sp.check_output(
-                    ["git", "commit", "-a", "-m", comment], cwd=tmp, stderr=sp.STDOUT
-                )
-                filename = sp.check_output(
-                    ["git", "format-patch", "HEAD^"], cwd=tmp, stderr=sp.STDOUT
-                )
-                filename_str = filename.decode("utf-8").strip()
-            except sp.CalledProcessError as exc:
-                std_out = ""
-                std_err = ""
-                if exc.stdout:
-                    std_out = exc.stdout.decode()
-                if exc.stderr:
-                    std_err = exc.stderr.decode()
-                raise BuilderException(
-                    str(exc), value=output, std_out=std_out, std_err=std_err
-                )
-
-            output["patch_filename"] = filename_str
-
-            # Copy the content of file to output
-            patch = os.path.join(tmp, filename_str)
-            with open(patch) as f:
-                output["patch"] = f.read()
-
             return output
 
     def _dist_git_sources(self, dist_git_path: str) -> list:
         """
         Retrieve sources from dist-git.
 
         Example:
@@ -297,16 +297,16 @@
                         os.path.realpath(os.path.join(target_dir, line.split()[-1]))
                     )
         except sp.CalledProcessError as e:
             # spectool passes the cURL exit codes back so see its manpage for the full list
             if e.returncode == 1:
                 # Unknown protocol (e.g. not ftp, http, or https)
                 msg = (
-                    "The specfile contains a Source URL with an unknown protocol; it should"
-                    'be "https", "http", or "ftp".'
+                    "There is a syntax error in updated specfile. "
+                    "See attached diff for the changes."
                 )
             elif e.returncode in (5, 6):
                 msg = "Unable to resolve the hostname for one of the package's Source URLs"
             elif e.returncode == 7:
                 # Failed to connect to the host
                 msg = (
                     "Unable to connect to the host for one of the package's Source URLs"
```

### Comparing `the-new-hotness-1.2.2/hotness/common/__init__.py` & `the_new_hotness-1.2.3/hotness/common/__init__.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/common/rpm.py` & `the_new_hotness-1.2.3/hotness/common/rpm.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/config.py` & `the_new_hotness-1.2.3/hotness/config.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/databases/__init__.py` & `the_new_hotness-1.2.3/hotness/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/databases/cache.py` & `the_new_hotness-1.2.3/hotness/databases/cache.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/databases/database.py` & `the_new_hotness-1.2.3/hotness/databases/database.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/databases/redis.py` & `the_new_hotness-1.2.3/hotness/databases/redis.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/domain/__init__.py` & `the_new_hotness-1.2.3/hotness/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/domain/package.py` & `the_new_hotness-1.2.3/hotness/domain/package.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/exceptions/__init__.py` & `the_new_hotness-1.2.3/hotness/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/exceptions/base_exception.py` & `the_new_hotness-1.2.3/hotness/exceptions/base_exception.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/exceptions/builder_exception.py` & `the_new_hotness-1.2.3/hotness/exceptions/builder_exception.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/exceptions/download_exception.py` & `the_new_hotness-1.2.3/hotness/exceptions/download_exception.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/exceptions/http_exception.py` & `the_new_hotness-1.2.3/hotness/exceptions/http_exception.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/exceptions/notifier_exception.py` & `the_new_hotness-1.2.3/hotness/exceptions/notifier_exception.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/exceptions/patcher_exception.py` & `the_new_hotness-1.2.3/hotness/exceptions/patcher_exception.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/hotness_consumer.py` & `the_new_hotness-1.2.3/hotness/hotness_consumer.py`

 * *Files 5% similar despite different names*

```diff
@@ -620,27 +620,19 @@
             repo_version=current_version,
             repo_release=current_release,
             url=project_homepage,
             explanation_url=self.explanation_url,
             projectid=project_id,
             dist_git_url=dist_git_url,
         )
-        if len(retrieved_versions) > 1:
-            if latest_upstream in retrieved_versions:
-                short_desc = self.short_desc_template % dict(
-                    name=package.name, retrieved_version=latest_upstream
-                )
-            else:
-                short_desc = self.short_desc_template_more_versions % dict(
-                    name=package.name
-                )
-        elif retrieved_versions:
-            short_desc = self.short_desc_template % dict(
-                name=package.name, retrieved_version=retrieved_versions[0]
-            )
+        # Don't change the title of bug if the new version received is
+        # older than the latest upstream
+        short_desc = self.short_desc_template % dict(
+            name=package.name, retrieved_version=latest_upstream
+        )
         notify_request = NotifyRequest(
             package=package,
             message=description,
             opts={"bz_short_desc": short_desc},
         )
         notifier_bugzilla_use_case = NotifyUserUseCase(self.notifier_bugzilla)
         response = notifier_bugzilla_use_case.notify(notify_request)
@@ -681,22 +673,44 @@
                 package=package,
                 message=message,
                 opts={"bz_id": bz_id},
             )
             notifier_bugzilla_use_case = NotifyUserUseCase(self.notifier_bugzilla)
             notifier_bugzilla_use_case.notify(notify_request)
 
+            # Read the values from use case when available
+            build_id = None
+            patch = None
+            patch_filename = None
+            if response.use_case_value:
+                build_id = response.use_case_value.get("build_id", None)
+                patch = response.use_case_value.get("patch", None)
+                patch_filename = response.use_case_value.get("patch_filename", None)
+
             # Insert the build_id to redis if available
-            if response.use_case_value and "build_id" in response.use_case_value:
-                build_id = response.use_case_value["build_id"]
+            if build_id:
                 insert_data_request = InsertDataRequest(
                     key=str(build_id), value=str(bz_id)
                 )
                 insert_data_redis_use_case = InsertDataUseCase(self.database_redis)
                 response = insert_data_redis_use_case.insert(insert_data_request)
+
+            # Attach patch to Bugzilla
+            if patch and patch_filename:
+                submit_patch_request = SubmitPatchRequest(
+                    package=package,
+                    patch=patch,
+                    opts={"bz_id": bz_id, "patch_filename": patch_filename},
+                )
+                submit_patch_bugzilla_use_case = SubmitPatchUseCase(
+                    self.patcher_bugzilla
+                )
+                response = submit_patch_bugzilla_use_case.submit_patch(
+                    submit_patch_request
+                )
             return
 
         build_id = response.value["build_id"]
         patch = response.value["patch"]
         patch_filename = response.value["patch_filename"]
         message = response.value["message"]
         if message:
```

### Comparing `the-new-hotness-1.2.2/hotness/notifiers/__init__.py` & `the_new_hotness-1.2.3/hotness/notifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/notifiers/bugzilla.py` & `the_new_hotness-1.2.3/hotness/notifiers/bugzilla.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/notifiers/fedora_messaging.py` & `the_new_hotness-1.2.3/hotness/notifiers/fedora_messaging.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/notifiers/notifier.py` & `the_new_hotness-1.2.3/hotness/notifiers/notifier.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/patchers/__init__.py` & `the_new_hotness-1.2.3/hotness/patchers/__init__.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/patchers/bugzilla.py` & `the_new_hotness-1.2.3/hotness/patchers/bugzilla.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/patchers/patcher.py` & `the_new_hotness-1.2.3/hotness/patchers/patcher.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/requests/__init__.py` & `the_new_hotness-1.2.3/hotness/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/requests/build_request.py` & `the_new_hotness-1.2.3/hotness/requests/build_request.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/requests/insert_data_request.py` & `the_new_hotness-1.2.3/hotness/requests/insert_data_request.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/requests/notify_request.py` & `the_new_hotness-1.2.3/hotness/requests/notify_request.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/requests/package_request.py` & `the_new_hotness-1.2.3/hotness/requests/package_request.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/requests/request.py` & `the_new_hotness-1.2.3/hotness/requests/request.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/requests/retrieve_data_request.py` & `the_new_hotness-1.2.3/hotness/requests/retrieve_data_request.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/requests/submit_patch_request.py` & `the_new_hotness-1.2.3/hotness/requests/submit_patch_request.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/responses/__init__.py` & `the_new_hotness-1.2.3/hotness/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/responses/response.py` & `the_new_hotness-1.2.3/hotness/responses/response.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/responses/response_failure.py` & `the_new_hotness-1.2.3/hotness/responses/response_failure.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/responses/response_success.py` & `the_new_hotness-1.2.3/hotness/responses/response_success.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/use_cases/__init__.py` & `the_new_hotness-1.2.3/hotness/use_cases/__init__.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/use_cases/insert_data_use_case.py` & `the_new_hotness-1.2.3/hotness/use_cases/insert_data_use_case.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/use_cases/notify_user_use_case.py` & `the_new_hotness-1.2.3/hotness/use_cases/notify_user_use_case.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/use_cases/package_check_use_case.py` & `the_new_hotness-1.2.3/hotness/use_cases/package_check_use_case.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/use_cases/package_scratch_build_use_case.py` & `the_new_hotness-1.2.3/hotness/use_cases/package_scratch_build_use_case.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/use_cases/retrieve_data_use_case.py` & `the_new_hotness-1.2.3/hotness/use_cases/retrieve_data_use_case.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/use_cases/submit_patch_use_case.py` & `the_new_hotness-1.2.3/hotness/use_cases/submit_patch_use_case.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/validators/__init__.py` & `the_new_hotness-1.2.3/hotness/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/validators/mdapi.py` & `the_new_hotness-1.2.3/hotness/validators/mdapi.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/validators/pagure.py` & `the_new_hotness-1.2.3/hotness/validators/pagure.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/validators/pdc.py` & `the_new_hotness-1.2.3/hotness/validators/pdc.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/hotness/validators/validator.py` & `the_new_hotness-1.2.3/hotness/validators/validator.py`

 * *Files identical despite different names*

### Comparing `the-new-hotness-1.2.2/pyproject.toml` & `the_new_hotness-1.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     | dist
   )/
 )
 '''
 
 [tool.poetry]
 name = "the-new-hotness"
-version = "1.2.2"
+version = "1.2.3"
 description = "A fedora messaging consumer that files bugzilla bugs for upstream releases"
 authors = ["Ralph Bean <rbean@redhat.com>"]
 maintainers = ["Michal Konecny <mkonecny@redhat.com>"]
 readme = "README.rst"
 homepage = "https://github.com/fedora-infra/the-new-hotness"
 documentation = "https://the-new-hotness.readthedocs.io"
 repository = "https://github.com/fedora-infra/the-new-hotness"
```

### Comparing `the-new-hotness-1.2.2/setup.py` & `the_new_hotness-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
  'koji>=1.30.0,<2.0.0',
  'python-bugzilla>=3.2.0,<4.0.0',
  'redis>=4.3.4,<5.0.0',
  'requests>=2.28.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'the-new-hotness',
-    'version': '1.2.2',
+    'version': '1.2.3',
     'description': 'A fedora messaging consumer that files bugzilla bugs for upstream releases',
     'long_description': ".. image:: https://img.shields.io/pypi/v/the-new-hotness.svg\n  :target: https://pypi.org/project/the-new-hotness/\n\n.. image:: https://readthedocs.org/projects/the-new-hotness/badge/?version=latest\n  :alt: Documentation Status\n  :target: https://the-new-hotness.readthedocs.io/en/latest/?badge=latest\n\nthe-new-hotness\n---------------\n\n`Fedora-messaging <https://github.com/fedora-infra/fedora-messaging>`_ consumer that listens to `release-monitoring.org\n<http://release-monitoring.org>`_ and files bugzilla bugs in response (to\nnotify packagers that they can update their packages).\n\nFor additional information see `documentation <https://the-new-hotness.readthedocs.io/en/stable/>`_.\n\nSeeing it in action\n^^^^^^^^^^^^^^^^^^^\n\nTo see recent messages from the-new-hotness:\n\n* Check Fedora's `datagrepper\n  <https://apps.fedoraproject.org/datagrepper/raw?category=hotness&delta=2592000>`_\n\n* Or join #fedora-fedmsg IRC channel on `libera <https://libera.chat/>`_ and watch for ``hotness``\n  messages.\n\nTo see recent koji builds started by the-new-hotness:\n\n* Check Fedora's `koji builds\n  <https://koji.fedoraproject.org/koji/tasks?owner=the-new-hotness/release-monitoring.org&state=all>`_\n\nDevelopment\n^^^^^^^^^^^\n\nContributions are welcome, check out `contribution guidelines <https://the-new-hotness.readthedocs.io/en/stable/dev-guide.html#contribution-guidelines>`_.\n",
     'author': 'Ralph Bean',
     'author_email': 'rbean@redhat.com',
     'maintainer': 'Michal Konecny',
     'maintainer_email': 'mkonecny@redhat.com',
     'url': 'https://github.com/fedora-infra/the-new-hotness',
```

### Comparing `the-new-hotness-1.2.2/PKG-INFO` & `the_new_hotness-1.2.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: the-new-hotness
-Version: 1.2.2
+Version: 1.2.3
 Summary: A fedora messaging consumer that files bugzilla bugs for upstream releases
 Home-page: https://github.com/fedora-infra/the-new-hotness
 License: GPL-2.0-or-later
 Author: Ralph Bean
 Author-email: rbean@redhat.com
 Maintainer: Michal Konecny
 Maintainer-email: mkonecny@redhat.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: anitya-schema (>=2.0.1,<3.0.0)
 Requires-Dist: fedora-messaging (>=3.1.0,<4.0.0)
 Requires-Dist: fedora-messaging-the-new-hotness-schema (>=1.1.2,<2.0.0)
 Requires-Dist: koji (>=1.30.0,<2.0.0)
```

