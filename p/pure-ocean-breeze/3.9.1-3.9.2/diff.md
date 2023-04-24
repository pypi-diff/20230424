# Comparing `tmp/pure_ocean_breeze-3.9.1.tar.gz` & `tmp/pure_ocean_breeze-3.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pure_ocean_breeze-3.9.1.tar", last modified: Sat Mar 25 11:42:00 2023, max compression
+gzip compressed data, was "pure_ocean_breeze-3.9.2.tar", last modified: Mon Apr 24 05:18:33 2023, max compression
```

## Comparing `pure_ocean_breeze-3.9.1.tar` & `pure_ocean_breeze-3.9.2.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 11:42:00.804481 pure_ocean_breeze-3.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-03-25 11:42:00.804481 pure_ocean_breeze-3.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 11:42:00.784481 pure_ocean_breeze-3.9.1/pure_ocean_breeze/
--rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 11:42:00.788481 pure_ocean_breeze-3.9.1/pure_ocean_breeze/data/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31550 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/data/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    29304 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    49960 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    49200 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 11:42:00.788481 pure_ocean_breeze-3.9.1/pure_ocean_breeze/future_version/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23637 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 11:42:00.788481 pure_ocean_breeze-3.9.1/pure_ocean_breeze/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 11:42:00.788481 pure_ocean_breeze-3.9.1/pure_ocean_breeze/labor/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12895 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)   215815 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 11:42:00.788481 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 11:42:00.788481 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v1/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)   192825 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 11:42:00.788481 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v1p10/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v1p10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v1p10/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)    85655 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 11:42:00.792481 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v2/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v2/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)   314704 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 11:42:00.792481 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 11:42:00.792481 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/data/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29395 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/data/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    43178 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 11:42:00.792481 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/future_version/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 11:42:00.792481 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 11:42:00.796481 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/labor/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)   138094 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 11:42:00.796481 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/mail/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 11:42:00.796481 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/state/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 11:42:00.796481 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/withs/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 11:42:00.796481 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/
--rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 11:42:00.800481 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/data/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29805 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/data/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    23214 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    29153 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    45478 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 11:42:00.800481 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/future_version/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 11:42:00.800481 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 11:42:00.800481 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/labor/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)   193541 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 11:42:00.800481 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/mail/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 11:42:00.800481 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/state/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 11:42:00.804481 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/withs/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 11:42:00.804481 pure_ocean_breeze-3.9.1/pure_ocean_breeze/mail/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 11:42:00.804481 pure_ocean_breeze-3.9.1/pure_ocean_breeze/state/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 11:42:00.804481 pure_ocean_breeze-3.9.1/pure_ocean_breeze/withs/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 11:42:00.784481 pure_ocean_breeze-3.9.1/pure_ocean_breeze.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-03-25 11:42:00.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-03-25 11:42:00.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 11:42:00.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-03-25 11:42:00.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-25 11:42:00.000000 pure_ocean_breeze-3.9.1/pure_ocean_breeze.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 11:42:00.804481 pure_ocean_breeze-3.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-03-25 11:41:46.000000 pure_ocean_breeze-3.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:18:33.108121 pure_ocean_breeze-3.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-04-24 05:18:33.108121 pure_ocean_breeze-3.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:18:33.092121 pure_ocean_breeze-3.9.2/pure_ocean_breeze/
+-rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:18:33.092121 pure_ocean_breeze-3.9.2/pure_ocean_breeze/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31550 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29530 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49960 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49330 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:18:33.092121 pure_ocean_breeze-3.9.2/pure_ocean_breeze/future_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23637 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:18:33.096121 pure_ocean_breeze-3.9.2/pure_ocean_breeze/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:18:33.096121 pure_ocean_breeze-3.9.2/pure_ocean_breeze/labor/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   225918 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:18:33.096121 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:18:33.096121 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v1/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)   192825 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:18:33.096121 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v1p10/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v1p10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v1p10/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85655 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:18:33.096121 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v2/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)   314704 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:18:33.100121 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:18:33.100121 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29395 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43178 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:18:33.100121 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/future_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:18:33.100121 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:18:33.100121 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/labor/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   138094 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:18:33.100121 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:18:33.104121 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:18:33.104121 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/withs/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:18:33.104121 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/
+-rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:18:33.104121 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29805 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23214 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29153 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45478 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:18:33.104121 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/future_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:18:33.104121 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:18:33.104121 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/labor/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   193541 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:18:33.108121 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:18:33.108121 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:18:33.108121 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/withs/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:18:33.108121 pure_ocean_breeze-3.9.2/pure_ocean_breeze/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:18:33.108121 pure_ocean_breeze-3.9.2/pure_ocean_breeze/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:18:33.108121 pure_ocean_breeze-3.9.2/pure_ocean_breeze/withs/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:18:33.092121 pure_ocean_breeze-3.9.2/pure_ocean_breeze.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-04-24 05:18:33.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-04-24 05:18:33.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 05:18:33.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-24 05:18:33.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-24 05:18:33.000000 pure_ocean_breeze-3.9.2/pure_ocean_breeze.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 05:18:33.108121 pure_ocean_breeze-3.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-24 05:18:18.000000 pure_ocean_breeze-3.9.2/setup.py
```

### Comparing `pure_ocean_breeze-3.9.1/LICENSE` & `pure_ocean_breeze-3.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/PKG-INFO` & `pure_ocean_breeze-3.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure_ocean_breeze
-Version: 3.9.1
+Version: 3.9.2
 Summary: stock factor test
 Home-page: https://github.com/chen-001/pure_ocean_breeze.git
 Author: chenzongwei
 Author-email: winterwinter999@163.com
 License: MIT
 Project-URL: Documentation, https://chen-001.github.io/pure_ocean_breeze/
 Requires-Python: >=3
```

### Comparing `pure_ocean_breeze-3.9.1/README.md` & `pure_ocean_breeze-3.9.2/README.md`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/__init__.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 一个量化多因子研究的框架，包含数据、回测、因子加工等方面的功能
 """
 
-__updated__ = "2023-03-23 19:09:31"
-__version__ = "3.9.1"
+__updated__ = "2023-03-27 22:53:46"
+__version__ = "3.9.2"
 __author__ = "chenzongwei"
 __author_email__ = "winterwinter999@163.com"
 __url__ = "https://github.com/chen-001/pure_ocean_breeze"
 __all__ = [
     "data",
     "labor",
     "state",
```

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/data/database.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/data/dicts.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/data/read_data.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/data/read_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -350,14 +350,16 @@
         读取最低点数, by default 0
     start : int, optional
         读取的起始日期, by default STATES["START"]
     every_stock : bool, optional
         是否修改为index是时间，columns是每只股票代码，每一列值都相同的形式, by default 1
     market_code : str, optional
         选用哪个指数作为市场指数，默认使用中证全指
+    questdb_host: str, optional
+        questdb的host，使用NAS时改为'192.168.1.3', by default '127.0.0.1'
 
     Returns
     -------
     Union[pd.DataFrame,pd.Series]
         中证全指每天的指数
 
     Raises
@@ -497,14 +499,16 @@
 def read_index_single(code: str,questdb_host:str='127.0.0.1') -> pd.Series:
     """读取某个指数的日行情收盘价数据
 
     Parameters
     ----------
     code : str
         指数的wind代码
+    questdb_host: str, optional
+        questdb的host，使用NAS时改为'192.168.1.3', by default '127.0.0.1'
 
     Returns
     -------
     pd.Series
         日行情数据
     """
     try:
```

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/data/tools.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/data/tools.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/data/write_data.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/data/write_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__updated__ = "2023-03-23 11:58:16"
+__updated__ = "2023-03-26 22:29:53"
 
 import time
 
 try:
     import rqdatac
 
     rqdatac.init()
@@ -315,14 +315,18 @@
                 "close",
                 "volume",
                 "adjopen",
                 "adjclose",
                 "adjhigh",
                 "adjlow",
                 "tradestatus",
+                "adjfactor",
+                "limit",
+                "stopping",
+                "avgprice",
             ],
         )
         # 换手率，流通股本，换手率要除以100，流通股本要乘以10000
         df2 = pro.daily_basic(
             trade_date=day,
             fields=[
                 "ts_code",
@@ -465,21 +469,21 @@
         # 复权最低价
         dilows = to_mat(part1, "adjlow", "lows")
         # 复权收盘价
         dicloses = to_mat(part1, "adjclose", "closes")
         # 交易状态
         status = to_mat(part1, "tradestatus", "states")
         # 平均价格
-        vwaps = to_mat(part1, "adjprice", "vwaps")
+        vwaps = to_mat(part1, "avgprice", "vwaps")
         # 复权因子
         adjfactors = to_mat(part1, "adjfactor", "adjfactors")
         # 涨停价
         stop_ups = to_mat(part1, "limit", "stop_ups")
         # 跌停价
-        stop_downs = to_mat(part1, "stop", "stop_downs")
+        stop_downs = to_mat(part1, "stopping", "stop_downs")
 
         # 换手率
         part2 = df2s[["date", "code", "turnover_rate_f"]].pivot(
             index="date", columns="code", values="turnover_rate_f"
         )
         part2 = part2 / 100
         part2_old = pd.read_parquet(homeplace.daily_data_file + "trs.parquet")
@@ -511,15 +515,15 @@
             columns="code", index="date", values="total_share"
         )
         part3a = part3a * 10000
         part3_olda = pd.read_parquet(
             homeplace.daily_data_file + "total_sharenums.parquet"
         )
         part3_newa = pd.concat([part3_olda, part3a]).drop_duplicates()
-        part3_newa = part3_newa[closes.columns]
+        part3_newa = part3_newa.reindex(columns=closes.columns)
         part3_newa = drop_duplicates_index(part3_newa)
         part3_newa = part3_newa[sorted(list(part3_newa.columns))]
         part3_newa.to_parquet(homeplace.daily_data_file + "total_sharenums.parquet")
         logger.success("总股数更新完成")
 
         # pb
         partpb = df2s[["date", "code", "pb"]].pivot(
```

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/future_version/half_way.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/future_version/in_thoughts.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/initialize/initialize.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/labor/comment.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/labor/comment.py`

 * *Files 6% similar despite different names*

```diff
@@ -142,14 +142,15 @@
 @do_on_dfs
 def make_relative_comments(
     ret_fac: pd.Series,
     hs300: bool = 0,
     zz500: bool = 0,
     zz1000: bool = 0,
     gz2000: bool = 0,
+    all_a: bool = 0,
     day: int = None,
     show_nets: bool = 0,
 ) -> pd.Series:
     """对于一个给定的收益率序列，计算其相对于某个指数的超额表现
 
     Parameters
     ----------
@@ -159,14 +160,16 @@
         为1则相对沪深300指数行情, by default 0
     zz500 : bool, optional
         为1则相对中证500指数行情, by default 0
     zz1000 : bool, optional
         为1则相对中证1000指数行情, by default 0
     gz2000 : bool, optional
         为1则相对国证2000指数行情, by default 0
+    all_a : bool, optional
+        为1则相对中证全指指数行情, by default 0
     day : int, optional
         起始日期，形如20130101, by default None
     show_nets : bool, optional
         返回值中包括超额净值数据, by default 0
 
     Returns
     -------
@@ -196,15 +199,19 @@
             net_index = read_index_single("000852.SH").resample("M").last()
             net_indexs.append(net_index)
             weights.append(1000)
         if gz2000:
             net_index = read_index_single("399303.SZ").resample("M").last()
             net_indexs.append(net_index)
             weights.append(2000)
-        if (hs300 + zz500 + zz1000 + gz2000) == 0:
+        if all_a:
+            net_index = read_index_single("000985.SH").resample("M").last()
+            net_indexs.append(net_index)
+            weights.append(5000)
+        if (hs300 + zz500 + zz1000 + gz2000+ all_a) == 0:
             raise IOError("你总得指定一个股票池吧？")
         net_index = pd.concat(net_indexs, axis=1)
     ret_index = net_index.pct_change()
     if isinstance(ret_index, pd.DataFrame):
         ret_index = sum(
             [ret_index.iloc[:, i] * weights[i] for i in range(len(weights))]
         ) / sum(weights)
@@ -227,14 +234,15 @@
 @do_on_dfs
 def make_relative_comments_plot(
     ret_fac: pd.Series,
     hs300: bool = 0,
     zz500: bool = 0,
     zz1000: bool = 0,
     gz2000: bool = 0,
+    all_a: bool = 0,
     day: int = None,
 ) -> pd.Series:
     """对于一个给定的收益率序列，计算其相对于某个指数的超额表现，然后绘图，并返回超额净值序列
 
     Parameters
     ----------
     ret_fac : pd.Series
@@ -243,14 +251,16 @@
         为1则相对沪深300指数行情, by default 0
     zz500 : bool, optional
         为1则相对中证500指数行情, by default 0
     zz1000 : bool, optional
         为1则相对中证1000指数行情, by default 0
     gz2000 : bool, optional
         为1则相对国证2000指数行情, by default 0
+    all_a : bool, optional
+        为1则相对中证全指指数行情, by default 0
     day : int, optional
         起始日期，形如20130101, by default None
 
     Returns
     -------
     `pd.Series`
         超额净值序列
@@ -277,15 +287,19 @@
             net_index = read_index_single("000852.SH").resample("M").last()
             net_indexs.append(net_index)
             weights.append(1000)
         if gz2000:
             net_index = read_index_single("399303.SZ").resample("M").last()
             net_indexs.append(net_index)
             weights.append(2000)
-        if (hs300 + zz500 + zz1000 + gz2000) == 0:
+        if all_a:
+            net_index = read_index_single("000985.SH").resample("M").last()
+            net_indexs.append(net_index)
+            weights.append(5000)
+        if (hs300 + zz500 + zz1000 + gz2000+ all_a) == 0:
             raise IOError("你总得指定一个股票池吧？")
         net_index = pd.concat(net_indexs, axis=1)
     ret_index = net_index.pct_change()
     if isinstance(ret_index, pd.DataFrame):
         ret_index = sum(
             [ret_index.iloc[:, i] * weights[i] for i in range(len(weights))]
         ) / sum(weights)
```

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/labor/process.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/labor/process.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__updated__ = "2023-03-25 19:33:26"
+__updated__ = "2023-04-03 01:16:24"
 
 import warnings
 
 warnings.filterwarnings("ignore")
 import numpy as np
 import pandas as pd
 import knockknock as kk
@@ -3022,15 +3022,15 @@
 
     def __init__(
         self,
         factor_file: str,
         project: str = None,
         startdate: int = None,
         enddate: int = None,
-        questdb_host: str = '127.0.0.1',
+        questdb_host: str = "127.0.0.1",
         kind: str = "stock",
         clickhouse: bool = 0,
         questdb: bool = 0,
         questdb_web_port: str = "9001",
         ignore_history_in_questdb: bool = 0,
         groupby_target: list = ["date", "code"],
     ) -> None:
@@ -3042,14 +3042,16 @@
             用于保存因子值的文件名，需为parquet文件，以'.parquet'结尾
         project : str, optional
             该因子所属项目，即子文件夹名称, by default None
         startdate : int, optional
             起始时间，形如20121231，为开区间, by default None
         enddate : int, optional
             截止时间，形如20220814，为闭区间，为空则计算到最近数据, by default None
+        questdb_host: str, optional
+            questdb的host，使用NAS时改为'192.168.1.3', by default '127.0.0.1'
         kind : str, optional
             类型为股票还是指数，指数为'index', by default "stock"
         clickhouse : bool, optional
             使用clickhouse作为数据源，如果postgresql与本参数都为0，将依然从clickhouse中读取, by default 0
         questdb : bool, optional
             使用questdb作为数据源, by default 0
         questdb_web_port : str, optional
@@ -3068,21 +3070,21 @@
         self.clickhouse = clickhouse
         self.questdb = questdb
         self.questdb_web_port = questdb_web_port
         if clickhouse == 1:
             # 连接clickhouse
             self.chc = ClickHouseClient("minute_data")
         elif questdb == 1:
-            self.chc = Questdb(host=questdb_host,web_port=questdb_web_port)
+            self.chc = Questdb(host=questdb_host, web_port=questdb_web_port)
         # 将计算到一半的因子，存入questdb中，避免中途被打断后重新计算，表名即为因子文件名的汉语拼音
         pinyin = Pinyin()
         self.factor_file_pinyin = pinyin.get_pinyin(
             factor_file.replace(".parquet", ""), ""
         )
-        self.factor_steps = Questdb(host=questdb_host,web_port=questdb_web_port)
+        self.factor_steps = Questdb(host=questdb_host, web_port=questdb_web_port)
         if project is not None:
             if not os.path.exists(homeplace.factor_data_file + project):
                 os.makedirs(homeplace.factor_data_file + project)
             else:
                 logger.info(f"当前正在{project}项目中……")
         else:
             logger.warning("当前因子不属于任何项目，这将造成因子数据文件夹的混乱，不便于管理，建议指定一个项目名称")
@@ -4413,14 +4415,240 @@
     # 买3只超额表现
     rets = long_test_on_industry(
         fac, nums, pos=pos, neg=neg, swindustry=swindustry, zxindustry=zxindustry
     )
     logger.success("因子后续的必要测试全部完成")
 
 
+def test_on_index_four_out(
+    fac: pd.DataFrame,
+    trade_cost_double_side_list: float = [0.001, 0.002, 0.003, 0.004, 0.005],
+    group_num: int = 10,
+    boxcox: bool = 1,
+    comments_writer: pd.ExcelWriter = None,
+    net_values_writer: pd.ExcelWriter = None,
+    opens_average_first_day: bool = 0,
+):
+    if comments_writer is None:
+        from pure_ocean_breeze.state.states import COMMENTS_WRITER
+
+        comments_writer = COMMENTS_WRITER
+    if net_values_writer is None:
+        from pure_ocean_breeze.state.states import NET_VALUES_WRITER
+
+        net_values_writer = NET_VALUES_WRITER
+
+    shen = pure_moonnight(
+        fac,
+        opens_average_first_day=opens_average_first_day,
+    )
+    if (
+        shen.shen.group_net_values.group1.iloc[-1]
+        > shen.shen.group_net_values10.iloc[-1]
+    ):
+        neg = 1
+        pos = 0
+    else:
+        pos = 1
+        neg = 0
+
+    """3510多空和多头"""
+    # 300
+    fi300 = daily_factor_on300500(fac, hs300=1)
+    shen = pure_moonnight(
+        fi300,
+        groups_num=group_num,
+        boxcox=boxcox,
+        comments_writer=comments_writer,
+        net_values_writer=net_values_writer,
+        sheetname="300多空",
+        opens_average_first_day=opens_average_first_day,
+    )
+    if pos:
+        if comments_writer is not None:
+            make_relative_comments(
+                shen.shen.group_rets[f"group{group_num}"], hs300=1
+            ).to_excel(comments_writer, sheet_name="300超额")
+            for i in trade_cost_double_side_list:
+                make_relative_comments(
+                    shen.shen.group_rets[f"group{group_num}"]
+                    - shen.shen.factor_turnover_rates[f"group{group_num}"] * i,
+                    hs300=1,
+                ).to_excel(comments_writer, sheet_name=f"300超额双边费率{i}")
+        else:
+            make_relative_comments(shen.shen.group_rets[f"group{group_num}"], hs300=1)
+        if net_values_writer is not None:
+            make_relative_comments_plot(
+                shen.shen.group_rets[f"group{group_num}"], hs300=1
+            ).to_excel(net_values_writer, sheet_name="300超额")
+            for i in trade_cost_double_side_list:
+                make_relative_comments_plot(
+                    shen.shen.group_rets[f"group{group_num}"]
+                    - shen.shen.factor_turnover_rates[f"group{group_num}"] * i,
+                    hs300=1,
+                ).to_excel(net_values_writer, sheet_name=f"300超额双边费率{i}")
+        else:
+            make_relative_comments_plot(
+                shen.shen.group_rets[f"group{group_num}"], hs300=1
+            )
+    elif neg:
+        if comments_writer is not None:
+            make_relative_comments(shen.shen.group_rets.group1, hs300=1).to_excel(
+                comments_writer, sheet_name="300超额"
+            )
+            for i in trade_cost_double_side_list:
+                make_relative_comments(
+                    shen.shen.group_rets.group1
+                    - shen.shen.factor_turnover_rates.group1 * i,
+                    hs300=1,
+                ).to_excel(comments_writer, sheet_name=f"300超额双边费率{i}")
+        else:
+            make_relative_comments(shen.shen.group_rets.group1, hs300=1)
+        if net_values_writer is not None:
+            make_relative_comments_plot(shen.shen.group_rets.group1, hs300=1).to_excel(
+                net_values_writer, sheet_name="300超额"
+            )
+            for i in trade_cost_double_side_list:
+                make_relative_comments_plot(
+                    shen.shen.group_rets.group1
+                    - shen.shen.factor_turnover_rates.group1 * i,
+                    hs300=1,
+                ).to_excel(net_values_writer, sheet_name=f"300超额双边费率{i}")
+        else:
+            make_relative_comments_plot(shen.shen.group_rets.group1, hs300=1)
+    else:
+        raise IOError("请指定因子的方向是正是负🤒")
+    # 500
+    fi500 = daily_factor_on300500(fac, zz500=1)
+    shen = pure_moonnight(
+        fi500,
+        groups_num=group_num,
+        boxcox=boxcox,
+        comments_writer=comments_writer,
+        net_values_writer=net_values_writer,
+        sheetname="500多空",
+        opens_average_first_day=opens_average_first_day,
+    )
+    if pos:
+        if comments_writer is not None:
+            make_relative_comments(
+                shen.shen.group_rets[f"group{group_num}"], zz500=1
+            ).to_excel(comments_writer, sheet_name="500超额")
+            for i in trade_cost_double_side_list:
+                make_relative_comments(
+                    shen.shen.group_rets[f"group{group_num}"]
+                    - shen.shen.factor_turnover_rates[f"group{group_num}"] * i,
+                    zz500=1,
+                ).to_excel(comments_writer, sheet_name=f"500超额双边费率{i}")
+        else:
+            make_relative_comments(shen.shen.group_rets[f"group{group_num}"], zz500=1)
+        if net_values_writer is not None:
+            make_relative_comments_plot(
+                shen.shen.group_rets[f"group{group_num}"], zz500=1
+            ).to_excel(net_values_writer, sheet_name="500超额")
+            for i in trade_cost_double_side_list:
+                make_relative_comments_plot(
+                    shen.shen.group_rets[f"group{group_num}"]
+                    - shen.shen.factor_turnover_rates[f"group{group_num}"] * i,
+                    zz500=1,
+                ).to_excel(net_values_writer, sheet_name=f"500超额双边费率{i}")
+        else:
+            make_relative_comments_plot(
+                shen.shen.group_rets[f"group{group_num}"], zz500=1
+            )
+    else:
+        if comments_writer is not None:
+            make_relative_comments(shen.shen.group_rets.group1, zz500=1).to_excel(
+                comments_writer, sheet_name="500超额"
+            )
+            for i in trade_cost_double_side_list:
+                make_relative_comments(
+                    shen.shen.group_rets.group1
+                    - shen.shen.factor_turnover_rates.group1 * i,
+                    zz500=1,
+                ).to_excel(comments_writer, sheet_name=f"500超额双边费率{i}")
+        else:
+            make_relative_comments(shen.shen.group_rets.group1, zz500=1)
+        if net_values_writer is not None:
+            make_relative_comments_plot(shen.shen.group_rets.group1, zz500=1).to_excel(
+                net_values_writer, sheet_name="500超额"
+            )
+            for i in trade_cost_double_side_list:
+                make_relative_comments_plot(
+                    shen.shen.group_rets.group1
+                    - shen.shen.factor_turnover_rates.group1 * i,
+                    zz500=1,
+                ).to_excel(net_values_writer, sheet_name=f"500超额双边费率{i}")
+        else:
+            make_relative_comments_plot(shen.shen.group_rets.group1, zz500=1)
+    # 1000
+    fi1000 = daily_factor_on300500(fac, zz1000=1)
+    shen = pure_moonnight(
+        fi1000,
+        groups_num=group_num,
+        boxcox=boxcox,
+        comments_writer=comments_writer,
+        net_values_writer=net_values_writer,
+        sheetname="1000多空",
+        opens_average_first_day=opens_average_first_day,
+    )
+    if pos:
+        if comments_writer is not None:
+            make_relative_comments(
+                shen.shen.group_rets[f"group{group_num}"], zz1000=1
+            ).to_excel(comments_writer, sheet_name="1000超额")
+            for i in trade_cost_double_side_list:
+                make_relative_comments(
+                    shen.shen.group_rets[f"group{group_num}"]
+                    - shen.shen.factor_turnover_rates[f"group{group_num}"] * i,
+                    zz1000=1,
+                ).to_excel(comments_writer, sheet_name=f"1000超额双边费率{i}")
+        else:
+            make_relative_comments(shen.shen.group_rets[f"group{group_num}"], zz1000=1)
+        if net_values_writer is not None:
+            make_relative_comments_plot(
+                shen.shen.group_rets[f"group{group_num}"], zz1000=1
+            ).to_excel(net_values_writer, sheet_name="1000超额")
+            for i in trade_cost_double_side_list:
+                make_relative_comments_plot(
+                    shen.shen.group_rets[f"group{group_num}"]
+                    - shen.shen.factor_turnover_rates[f"group{group_num}"] * i,
+                    zz1000=1,
+                ).to_excel(net_values_writer, sheet_name=f"1000超额双边费率{i}")
+        else:
+            make_relative_comments_plot(
+                shen.shen.group_rets[f"group{group_num}"], zz1000=1
+            )
+    else:
+        if comments_writer is not None:
+            make_relative_comments(shen.shen.group_rets.group1, zz1000=1).to_excel(
+                comments_writer, sheet_name="1000超额"
+            )
+            for i in trade_cost_double_side_list:
+                make_relative_comments(
+                    shen.shen.group_rets.group1
+                    - shen.shen.factor_turnover_rates.group1 * i,
+                    zz1000=1,
+                ).to_excel(comments_writer, sheet_name=f"1000超额双边费率{i}")
+        else:
+            make_relative_comments(shen.shen.group_rets.group1, zz1000=1)
+        if net_values_writer is not None:
+            make_relative_comments_plot(shen.shen.group_rets.group1, zz1000=1).to_excel(
+                net_values_writer, sheet_name="1000超额"
+            )
+            for i in trade_cost_double_side_list:
+                make_relative_comments_plot(
+                    shen.shen.group_rets.group1
+                    - shen.shen.factor_turnover_rates.group1 * i,
+                    zz1000=1,
+                ).to_excel(net_values_writer, sheet_name=f"1000超额双边费率{i}")
+        else:
+            make_relative_comments_plot(shen.shen.group_rets.group1, zz1000=1)
+
+
 class pure_helper(object):
     def __init__(
         self,
         df_main: pd.DataFrame,
         df_helper: pd.DataFrame,
         func: Callable = None,
         group: int = 10,
@@ -4817,14 +5045,15 @@
 
 
 @do_on_dfs
 def test_on_300500(
     df: pd.DataFrame,
     trade_cost_double_side: float = 0,
     group_num: int = 10,
+    boxcox: bool = 0,
     hs300: bool = 0,
     zz500: bool = 0,
     zz1000: bool = 0,
     gz2000: bool = 0,
     iplot: bool = 1,
     opens_average_first_day: bool = 0,
 ) -> pd.Series:
@@ -4859,14 +5088,15 @@
     fi300 = daily_factor_on300500(
         df, hs300=hs300, zz500=zz500, zz1000=zz1000, gz2000=gz2000
     )
     shen = pure_moonnight(
         fi300,
         groups_num=group_num,
         trade_cost_double_side=trade_cost_double_side,
+        boxcox=boxcox,
         iplot=iplot,
         opens_average_first_day=opens_average_first_day,
     )
     if (
         shen.shen.group_net_values.group1.iloc[-1]
         > shen.shen.group_net_values[f"group{group_num}"].iloc[-1]
     ):
@@ -5156,15 +5386,15 @@
         fac: pd.Series,
         code: str = None,
         price_opens: pd.Series = None,
         iplot: bool = 1,
         comments_writer: pd.ExcelWriter = None,
         net_values_writer: pd.ExcelWriter = None,
         sheetname: str = None,
-        questdb_host: str='127.0.0.1',
+        questdb_host: str = "127.0.0.1",
     ):
         """择时回测框架，输入仓位比例或信号值，依据信号买入对应的股票或指数，并考察绝对收益、超额收益和基准收益
         回测方式为，t日收盘时获得信号，t+1日开盘时以开盘价买入，t+2开盘时以开盘价卖出
 
         Parameters
         ----------
         fac : pd.Series
@@ -5177,14 +5407,16 @@
             使用cufflinks呈现回测绩效和走势图, by default 1
         comments_writer : pd.ExcelWriter, optional
             绩效评价的存储文件, by default None
         net_values_writer : pd.ExcelWriter, optional
             净值序列的存储文件, by default None
         sheetname : str, optional
             存储文件的工作表的名字, by default None
+        questdb_host: str, optional
+            questdb的host，使用NAS时改为'192.168.1.3', by default '127.0.0.1'
         """
         if code is not None:
             x1 = code.split(".")[0]
             x2 = code.split(".")[1]
             if (x1[0] == "0" or x1[:2] == "30") and x2 == "SZ":
                 kind = "stock"
             elif x1[0] == "6" and x2 == "SH":
```

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v1/initialize.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v1/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v1p10/initialize.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v1p10/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v2/initialize.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v2/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/__init__.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/data/database.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/data/tools.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/data/tools.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/labor/process.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/labor/process.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/mail/email.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/__init__.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/data/database.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/data/tools.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/data/tools.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/labor/process.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/labor/process.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/mail/email.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/state/states.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/state/states.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/mail/email.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/state/decorators.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/state/homeplace.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/state/states.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/state/states.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze/withs/requires.py` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze.egg-info/PKG-INFO` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure-ocean-breeze
-Version: 3.9.1
+Version: 3.9.2
 Summary: stock factor test
 Home-page: https://github.com/chen-001/pure_ocean_breeze.git
 Author: chenzongwei
 Author-email: winterwinter999@163.com
 License: MIT
 Project-URL: Documentation, https://chen-001.github.io/pure_ocean_breeze/
 Requires-Python: >=3
```

### Comparing `pure_ocean_breeze-3.9.1/pure_ocean_breeze.egg-info/SOURCES.txt` & `pure_ocean_breeze-3.9.2/pure_ocean_breeze.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.1/setup.py` & `pure_ocean_breeze-3.9.2/setup.py`

 * *Files identical despite different names*

