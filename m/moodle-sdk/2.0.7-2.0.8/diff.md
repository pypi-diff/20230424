# Comparing `tmp/moodle-sdk-2.0.7.tar.gz` & `tmp/moodle-sdk-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/jun/Work/projects/mdk/dist/.tmp-isvk36by/moodle-sdk-2.0.7.tar", last modified: Mon Nov 28 03:02:34 2022, max compression
+gzip compressed data, was "moodle-sdk-2.0.8.tar", last modified: Mon Apr 24 01:39:10 2023, max compression
```

## Comparing `moodle-sdk-2.0.7.tar` & `moodle-sdk-2.0.8.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 jun        (501) staff       (20)        0 2022-11-28 03:02:34.000000 moodle-sdk-2.0.7/
--rw-r--r--   0 jun        (501) staff       (20)    10346 2022-11-28 02:57:42.000000 moodle-sdk-2.0.7/CHANGELOG.rst
--rw-r--r--   0 jun        (501) staff       (20)    35147 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/LICENSE.txt
--rw-r--r--   0 jun        (501) staff       (20)       79 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/MANIFEST.in
--rw-r--r--   0 jun        (501) staff       (20)    11153 2022-11-28 03:02:34.000000 moodle-sdk-2.0.7/PKG-INFO
--rw-r--r--   0 jun        (501) staff       (20)    10478 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/README.rst
-drwxr-xr-x   0 jun        (501) staff       (20)        0 2022-11-28 03:02:34.000000 moodle-sdk-2.0.7/mdk/
--rw-r--r--   0 jun        (501) staff       (20)        0 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/__init__.py
--rw-r--r--   0 jun        (501) staff       (20)     3969 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/__main__.py
--rw-r--r--   0 jun        (501) staff       (20)     7709 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/backup.py
--rw-r--r--   0 jun        (501) staff       (20)     4373 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/ci.py
--rw-r--r--   0 jun        (501) staff       (20)     4500 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/command.py
-drwxr-xr-x   0 jun        (501) staff       (20)        0 2022-11-28 03:02:34.000000 moodle-sdk-2.0.7/mdk/commands/
--rw-r--r--   0 jun        (501) staff       (20)     1379 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/commands/__init__.py
--rw-r--r--   0 jun        (501) staff       (20)     5729 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/commands/alias.py
--rw-r--r--   0 jun        (501) staff       (20)    10686 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/commands/backport.py
--rw-r--r--   0 jun        (501) staff       (20)     4613 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/commands/backup.py
--rw-r--r--   0 jun        (501) staff       (20)    13915 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/commands/behat.py
--rw-r--r--   0 jun        (501) staff       (20)     8909 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/commands/config.py
--rw-r--r--   0 jun        (501) staff       (20)     7939 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/commands/create.py
--rw-r--r--   0 jun        (501) staff       (20)     6005 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/commands/css.py
--rw-r--r--   0 jun        (501) staff       (20)    14808 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/commands/doctor.py
--rw-r--r--   0 jun        (501) staff       (20)     2955 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/commands/fix.py
--rw-r--r--   0 jun        (501) staff       (20)     4382 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/commands/info.py
--rw-r--r--   0 jun        (501) staff       (20)     7822 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/commands/init.py
--rw-r--r--   0 jun        (501) staff       (20)     3159 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/commands/install.py
--rw-r--r--   0 jun        (501) staff       (20)     8320 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/commands/js.py
--rw-r--r--   0 jun        (501) staff       (20)     6406 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/commands/phpunit.py
--rw-r--r--   0 jun        (501) staff       (20)    11039 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/commands/plugin.py
--rw-r--r--   0 jun        (501) staff       (20)     4594 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/commands/precheck.py
--rw-r--r--   0 jun        (501) staff       (20)     6280 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/commands/pull.py
--rw-r--r--   0 jun        (501) staff       (20)     2884 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/commands/purge.py
--rw-r--r--   0 jun        (501) staff       (20)     6466 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/commands/push.py
--rw-r--r--   0 jun        (501) staff       (20)     7004 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/commands/rebase.py
--rw-r--r--   0 jun        (501) staff       (20)     2156 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/commands/remove.py
--rw-r--r--   0 jun        (501) staff       (20)     3739 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/commands/run.py
--rw-r--r--   0 jun        (501) staff       (20)     6820 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/commands/tracker.py
--rw-r--r--   0 jun        (501) staff       (20)     1877 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/commands/uninstall.py
--rw-r--r--   0 jun        (501) staff       (20)     4145 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/commands/update.py
--rw-r--r--   0 jun        (501) staff       (20)     4130 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/commands/upgrade.py
--rw-r--r--   0 jun        (501) staff       (20)    12417 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/config-dist.json
--rw-r--r--   0 jun        (501) staff       (20)     8908 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/config.py
--rw-r--r--   0 jun        (501) staff       (20)     5997 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/css.py
--rw-r--r--   0 jun        (501) staff       (20)     8341 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/db.py
--rw-r--r--   0 jun        (501) staff       (20)     1269 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/exceptions.py
--rw-r--r--   0 jun        (501) staff       (20)     8005 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/fetch.py
--rw-r--r--   0 jun        (501) staff       (20)    10494 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/git.py
--rw-r--r--   0 jun        (501) staff       (20)    13701 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/jira.py
--rw-r--r--   0 jun        (501) staff       (20)     4183 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/js.py
--rw-r--r--   0 jun        (501) staff       (20)    32035 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/moodle.py
--rw-r--r--   0 jun        (501) staff       (20)     5002 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/phpunit.py
--rw-r--r--   0 jun        (501) staff       (20)    17107 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/plugins.py
-drwxr-xr-x   0 jun        (501) staff       (20)        0 2022-11-28 03:02:34.000000 moodle-sdk-2.0.7/mdk/scripts/
--rw-r--r--   0 jun        (501) staff       (20)      803 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/scripts/README.rst
--rw-r--r--   0 jun        (501) staff       (20)     2149 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/scripts/dev.php
--rw-r--r--   0 jun        (501) staff       (20)     2417 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/scripts/enrol.php
--rw-r--r--   0 jun        (501) staff       (20)     1529 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/scripts/external_functions.php
--rw-r--r--   0 jun        (501) staff       (20)     6891 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/scripts/jsconfig.php
--rw-r--r--   0 jun        (501) staff       (20)      215 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/scripts/less.sh
--rw-r--r--   0 jun        (501) staff       (20)      406 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/scripts/makecourse.sh
--rw-r--r--   0 jun        (501) staff       (20)     2279 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/scripts/mindev.php
--rw-r--r--   0 jun        (501) staff       (20)      519 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/scripts/setup.sh
--rw-r--r--   0 jun        (501) staff       (20)     1715 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/scripts/setupsecurity.sh
--rw-r--r--   0 jun        (501) staff       (20)      994 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/scripts/tokens.php
--rw-r--r--   0 jun        (501) staff       (20)     3227 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/scripts/undev.php
--rw-r--r--   0 jun        (501) staff       (20)     5484 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/scripts/users.php
--rw-r--r--   0 jun        (501) staff       (20)     1257 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/scripts/version.php
--rw-r--r--   0 jun        (501) staff       (20)     3530 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/scripts/webservices.php
--rw-r--r--   0 jun        (501) staff       (20)     5528 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/scripts.py
--rw-r--r--   0 jun        (501) staff       (20)     7364 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/tools.py
--rw-r--r--   0 jun        (501) staff       (20)      796 2022-11-28 02:56:46.000000 moodle-sdk-2.0.7/mdk/version.py
--rw-r--r--   0 jun        (501) staff       (20)    16046 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/mdk/workplace.py
-drwxr-xr-x   0 jun        (501) staff       (20)        0 2022-11-28 03:02:34.000000 moodle-sdk-2.0.7/moodle_sdk.egg-info/
--rw-r--r--   0 jun        (501) staff       (20)    11153 2022-11-28 03:02:34.000000 moodle-sdk-2.0.7/moodle_sdk.egg-info/PKG-INFO
--rw-r--r--   0 jun        (501) staff       (20)     1548 2022-11-28 03:02:34.000000 moodle-sdk-2.0.7/moodle_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 jun        (501) staff       (20)        1 2022-11-28 03:02:34.000000 moodle-sdk-2.0.7/moodle_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 jun        (501) staff       (20)       42 2022-11-28 03:02:34.000000 moodle-sdk-2.0.7/moodle_sdk.egg-info/entry_points.txt
--rw-r--r--   0 jun        (501) staff       (20)      113 2022-11-28 03:02:34.000000 moodle-sdk-2.0.7/moodle_sdk.egg-info/requires.txt
--rw-r--r--   0 jun        (501) staff       (20)        4 2022-11-28 03:02:34.000000 moodle-sdk-2.0.7/moodle_sdk.egg-info/top_level.txt
--rw-r--r--   0 jun        (501) staff       (20)      113 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/requirements.txt
--rw-r--r--   0 jun        (501) staff       (20)       38 2022-11-28 03:02:34.000000 moodle-sdk-2.0.7/setup.cfg
--rw-r--r--   0 jun        (501) staff       (20)     2390 2022-11-28 02:54:59.000000 moodle-sdk-2.0.7/setup.py
+drwxr-xr-x   0 jun        (501) staff       (20)        0 2023-04-24 01:39:10.851587 moodle-sdk-2.0.8/
+-rw-r--r--   0 jun        (501) staff       (20)    10405 2023-04-24 01:07:25.000000 moodle-sdk-2.0.8/CHANGELOG.rst
+-rw-r--r--   0 jun        (501) staff       (20)    35147 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/LICENSE.txt
+-rw-r--r--   0 jun        (501) staff       (20)       79 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/MANIFEST.in
+-rw-r--r--   0 jun        (501) staff       (20)    11153 2023-04-24 01:39:10.851366 moodle-sdk-2.0.8/PKG-INFO
+-rw-r--r--   0 jun        (501) staff       (20)    10478 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/README.rst
+drwxr-xr-x   0 jun        (501) staff       (20)        0 2023-04-24 01:39:10.843724 moodle-sdk-2.0.8/mdk/
+-rw-r--r--   0 jun        (501) staff       (20)        0 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/__init__.py
+-rw-r--r--   0 jun        (501) staff       (20)     3969 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/__main__.py
+-rw-r--r--   0 jun        (501) staff       (20)     7709 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/backup.py
+-rw-r--r--   0 jun        (501) staff       (20)     4373 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/ci.py
+-rw-r--r--   0 jun        (501) staff       (20)     4500 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/command.py
+drwxr-xr-x   0 jun        (501) staff       (20)        0 2023-04-24 01:39:10.848173 moodle-sdk-2.0.8/mdk/commands/
+-rw-r--r--   0 jun        (501) staff       (20)     1379 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/commands/__init__.py
+-rw-r--r--   0 jun        (501) staff       (20)     5729 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/commands/alias.py
+-rw-r--r--   0 jun        (501) staff       (20)    10686 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/commands/backport.py
+-rw-r--r--   0 jun        (501) staff       (20)     4613 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/commands/backup.py
+-rw-r--r--   0 jun        (501) staff       (20)    13915 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/commands/behat.py
+-rw-r--r--   0 jun        (501) staff       (20)     8909 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/commands/config.py
+-rw-r--r--   0 jun        (501) staff       (20)     7939 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/commands/create.py
+-rw-r--r--   0 jun        (501) staff       (20)     6005 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/commands/css.py
+-rw-r--r--   0 jun        (501) staff       (20)    14808 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/commands/doctor.py
+-rw-r--r--   0 jun        (501) staff       (20)     2955 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/commands/fix.py
+-rw-r--r--   0 jun        (501) staff       (20)     4382 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/commands/info.py
+-rw-r--r--   0 jun        (501) staff       (20)     7822 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/commands/init.py
+-rw-r--r--   0 jun        (501) staff       (20)     3159 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/commands/install.py
+-rw-r--r--   0 jun        (501) staff       (20)     8320 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/commands/js.py
+-rw-r--r--   0 jun        (501) staff       (20)     6406 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/commands/phpunit.py
+-rw-r--r--   0 jun        (501) staff       (20)    11039 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/commands/plugin.py
+-rw-r--r--   0 jun        (501) staff       (20)     4594 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/commands/precheck.py
+-rw-r--r--   0 jun        (501) staff       (20)     6280 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/commands/pull.py
+-rw-r--r--   0 jun        (501) staff       (20)     2884 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/commands/purge.py
+-rw-r--r--   0 jun        (501) staff       (20)     6466 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/commands/push.py
+-rw-r--r--   0 jun        (501) staff       (20)     7004 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/commands/rebase.py
+-rw-r--r--   0 jun        (501) staff       (20)     2156 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/commands/remove.py
+-rw-r--r--   0 jun        (501) staff       (20)     3739 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/commands/run.py
+-rw-r--r--   0 jun        (501) staff       (20)     6820 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/commands/tracker.py
+-rw-r--r--   0 jun        (501) staff       (20)     1877 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/commands/uninstall.py
+-rw-r--r--   0 jun        (501) staff       (20)     4145 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/commands/update.py
+-rw-r--r--   0 jun        (501) staff       (20)     4130 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/commands/upgrade.py
+-rw-r--r--   0 jun        (501) staff       (20)    12548 2023-04-24 01:02:17.000000 moodle-sdk-2.0.8/mdk/config-dist.json
+-rw-r--r--   0 jun        (501) staff       (20)     8908 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/config.py
+-rw-r--r--   0 jun        (501) staff       (20)     5997 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/css.py
+-rw-r--r--   0 jun        (501) staff       (20)     8341 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/db.py
+-rw-r--r--   0 jun        (501) staff       (20)     1269 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/exceptions.py
+-rw-r--r--   0 jun        (501) staff       (20)     8005 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/fetch.py
+-rw-r--r--   0 jun        (501) staff       (20)    10494 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/git.py
+-rw-r--r--   0 jun        (501) staff       (20)    13701 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/jira.py
+-rw-r--r--   0 jun        (501) staff       (20)     4183 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/js.py
+-rw-r--r--   0 jun        (501) staff       (20)    32035 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/moodle.py
+-rw-r--r--   0 jun        (501) staff       (20)     5002 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/phpunit.py
+-rw-r--r--   0 jun        (501) staff       (20)    17107 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/plugins.py
+drwxr-xr-x   0 jun        (501) staff       (20)        0 2023-04-24 01:39:10.850348 moodle-sdk-2.0.8/mdk/scripts/
+-rw-r--r--   0 jun        (501) staff       (20)      803 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/scripts/README.rst
+-rw-r--r--   0 jun        (501) staff       (20)     2149 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/scripts/dev.php
+-rw-r--r--   0 jun        (501) staff       (20)     2417 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/scripts/enrol.php
+-rw-r--r--   0 jun        (501) staff       (20)     1529 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/scripts/external_functions.php
+-rw-r--r--   0 jun        (501) staff       (20)     6891 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/scripts/jsconfig.php
+-rw-r--r--   0 jun        (501) staff       (20)      215 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/scripts/less.sh
+-rw-r--r--   0 jun        (501) staff       (20)      406 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/scripts/makecourse.sh
+-rw-r--r--   0 jun        (501) staff       (20)     2279 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/scripts/mindev.php
+-rw-r--r--   0 jun        (501) staff       (20)      519 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/scripts/setup.sh
+-rw-r--r--   0 jun        (501) staff       (20)     1715 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/scripts/setupsecurity.sh
+-rw-r--r--   0 jun        (501) staff       (20)      994 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/scripts/tokens.php
+-rw-r--r--   0 jun        (501) staff       (20)     3227 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/scripts/undev.php
+-rw-r--r--   0 jun        (501) staff       (20)     5484 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/scripts/users.php
+-rw-r--r--   0 jun        (501) staff       (20)     1257 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/scripts/version.php
+-rw-r--r--   0 jun        (501) staff       (20)     3530 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/scripts/webservices.php
+-rw-r--r--   0 jun        (501) staff       (20)     5528 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/scripts.py
+-rw-r--r--   0 jun        (501) staff       (20)     7364 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/tools.py
+-rw-r--r--   0 jun        (501) staff       (20)      796 2023-04-24 01:06:42.000000 moodle-sdk-2.0.8/mdk/version.py
+-rw-r--r--   0 jun        (501) staff       (20)    16046 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/mdk/workplace.py
+drwxr-xr-x   0 jun        (501) staff       (20)        0 2023-04-24 01:39:10.851139 moodle-sdk-2.0.8/moodle_sdk.egg-info/
+-rw-r--r--   0 jun        (501) staff       (20)    11153 2023-04-24 01:39:10.000000 moodle-sdk-2.0.8/moodle_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 jun        (501) staff       (20)     1548 2023-04-24 01:39:10.000000 moodle-sdk-2.0.8/moodle_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 jun        (501) staff       (20)        1 2023-04-24 01:39:10.000000 moodle-sdk-2.0.8/moodle_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 jun        (501) staff       (20)       42 2023-04-24 01:39:10.000000 moodle-sdk-2.0.8/moodle_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 jun        (501) staff       (20)      113 2023-04-24 01:39:10.000000 moodle-sdk-2.0.8/moodle_sdk.egg-info/requires.txt
+-rw-r--r--   0 jun        (501) staff       (20)        4 2023-04-24 01:39:10.000000 moodle-sdk-2.0.8/moodle_sdk.egg-info/top_level.txt
+-rw-r--r--   0 jun        (501) staff       (20)      113 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/requirements.txt
+-rw-r--r--   0 jun        (501) staff       (20)       38 2023-04-24 01:39:10.851638 moodle-sdk-2.0.8/setup.cfg
+-rw-r--r--   0 jun        (501) staff       (20)     2390 2022-11-28 02:54:59.000000 moodle-sdk-2.0.8/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `moodle-sdk-2.0.7/CHANGELOG.rst` & `moodle-sdk-2.0.8/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 Changelog
 =========
 
+v2.0.8
+------
+
+- Update config for Moodle 4.3 development
+
 v2.0.7
 ------
 
-- Update config for Moodle 4.1 development - Huong Nguyen
+- Update config for Moodle 4.2 development - Huong Nguyen
 
 v2.0.6
 ------
 
 - Make yes or no prompts equal - Adrian Perez
 - Add vscode script to generate jsconfig.json - Andrew Nicols
 - Tracker command argument to open Jira ticket in default browser - Dongsheng Cai
```

### Comparing `moodle-sdk-2.0.7/LICENSE.txt` & `moodle-sdk-2.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/PKG-INFO` & `moodle-sdk-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moodle-sdk
-Version: 2.0.7
+Version: 2.0.8
 Summary: Moodle Development Kit
 Home-page: https://github.com/FMCorz/mdk
 Author: Frédéric Massart
 Author-email: fred@fmcorz.net
 License: MIT
 Keywords: mdk moodle moodle-sdk
 Classifier: Development Status :: 6 - Mature
```

### Comparing `moodle-sdk-2.0.7/README.rst` & `moodle-sdk-2.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/__main__.py` & `moodle-sdk-2.0.8/mdk/__main__.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/backup.py` & `moodle-sdk-2.0.8/mdk/backup.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/ci.py` & `moodle-sdk-2.0.8/mdk/ci.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/command.py` & `moodle-sdk-2.0.8/mdk/command.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/commands/__init__.py` & `moodle-sdk-2.0.8/mdk/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/commands/alias.py` & `moodle-sdk-2.0.8/mdk/commands/alias.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/commands/backport.py` & `moodle-sdk-2.0.8/mdk/commands/backport.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/commands/backup.py` & `moodle-sdk-2.0.8/mdk/commands/backup.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/commands/behat.py` & `moodle-sdk-2.0.8/mdk/commands/behat.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/commands/config.py` & `moodle-sdk-2.0.8/mdk/commands/config.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/commands/create.py` & `moodle-sdk-2.0.8/mdk/commands/create.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/commands/css.py` & `moodle-sdk-2.0.8/mdk/commands/css.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/commands/doctor.py` & `moodle-sdk-2.0.8/mdk/commands/doctor.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/commands/fix.py` & `moodle-sdk-2.0.8/mdk/commands/fix.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/commands/info.py` & `moodle-sdk-2.0.8/mdk/commands/info.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/commands/init.py` & `moodle-sdk-2.0.8/mdk/commands/init.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/commands/install.py` & `moodle-sdk-2.0.8/mdk/commands/install.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/commands/js.py` & `moodle-sdk-2.0.8/mdk/commands/js.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/commands/phpunit.py` & `moodle-sdk-2.0.8/mdk/commands/phpunit.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/commands/plugin.py` & `moodle-sdk-2.0.8/mdk/commands/plugin.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/commands/precheck.py` & `moodle-sdk-2.0.8/mdk/commands/precheck.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/commands/pull.py` & `moodle-sdk-2.0.8/mdk/commands/pull.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/commands/purge.py` & `moodle-sdk-2.0.8/mdk/commands/purge.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/commands/push.py` & `moodle-sdk-2.0.8/mdk/commands/push.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/commands/rebase.py` & `moodle-sdk-2.0.8/mdk/commands/rebase.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/commands/remove.py` & `moodle-sdk-2.0.8/mdk/commands/remove.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/commands/run.py` & `moodle-sdk-2.0.8/mdk/commands/run.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/commands/tracker.py` & `moodle-sdk-2.0.8/mdk/commands/tracker.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/commands/uninstall.py` & `moodle-sdk-2.0.8/mdk/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/commands/update.py` & `moodle-sdk-2.0.8/mdk/commands/update.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/commands/upgrade.py` & `moodle-sdk-2.0.8/mdk/commands/upgrade.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/config-dist.json` & `moodle-sdk-2.0.8/mdk/config-dist.json`

 * *Files 1% similar despite different names*

```diff
@@ -162,14 +162,18 @@
                 "branch" : "Pull 4.0 Branch",
                 "diffurl" : "Pull 4.0 Diff URL"
             },
             "401" : {
                 "branch" : "Pull 4.1 Branch",
                 "diffurl" : "Pull 4.1 Diff URL"
             },
+            "402" : {
+                "branch" : "Pull 4.2 Branch",
+                "diffurl" : "Pull 4.2 Diff URL"
+            },
             "master" : {
                 "branch" : "Pull Master Branch",
                 "diffurl" : "Pull Master Diff URL"
             }
         }
     },
     // The base for diff URLs, you can use the following wildcards:
@@ -312,15 +316,15 @@
     // Clones the cached repository with the option --shared, which drastically reduces the
     // size of the .git/ folder in each of the Moodle instances. Git reports this as a possible
     // dangerous operation (https://git-scm.com/docs/git-clone) so it is not enabled by default.
     // This requires the useCacheAsUpstreamRemote to be enabled.
     "useCacheAsSharedClone": false,
 
     // You should not edit this, this is the branch that is considered as master by developers.
-    "masterBranch": 402,
+    "masterBranch": 403,
 
     // Aliases for MDK commands.
     // An alias starting with a ! will be executed through the command line. Those also
     // can use placeholders for arguments: $1, $2, ...
     // Examples:
     //   "upall": "update --all". `mdk upall` will execute `mdk update --all`
     //   "ls": "!ls -al". `mdk ls` will execute `ls -al`
```

### Comparing `moodle-sdk-2.0.7/mdk/config.py` & `moodle-sdk-2.0.8/mdk/config.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/css.py` & `moodle-sdk-2.0.8/mdk/css.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/db.py` & `moodle-sdk-2.0.8/mdk/db.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/exceptions.py` & `moodle-sdk-2.0.8/mdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/fetch.py` & `moodle-sdk-2.0.8/mdk/fetch.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/git.py` & `moodle-sdk-2.0.8/mdk/git.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/jira.py` & `moodle-sdk-2.0.8/mdk/jira.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/js.py` & `moodle-sdk-2.0.8/mdk/js.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/moodle.py` & `moodle-sdk-2.0.8/mdk/moodle.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/phpunit.py` & `moodle-sdk-2.0.8/mdk/phpunit.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/plugins.py` & `moodle-sdk-2.0.8/mdk/plugins.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/scripts/README.rst` & `moodle-sdk-2.0.8/mdk/scripts/README.rst`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/scripts/dev.php` & `moodle-sdk-2.0.8/mdk/scripts/dev.php`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/scripts/enrol.php` & `moodle-sdk-2.0.8/mdk/scripts/enrol.php`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/scripts/external_functions.php` & `moodle-sdk-2.0.8/mdk/scripts/external_functions.php`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/scripts/jsconfig.php` & `moodle-sdk-2.0.8/mdk/scripts/jsconfig.php`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/scripts/mindev.php` & `moodle-sdk-2.0.8/mdk/scripts/mindev.php`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/scripts/setup.sh` & `moodle-sdk-2.0.8/mdk/scripts/setup.sh`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/scripts/setupsecurity.sh` & `moodle-sdk-2.0.8/mdk/scripts/setupsecurity.sh`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/scripts/tokens.php` & `moodle-sdk-2.0.8/mdk/scripts/tokens.php`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/scripts/undev.php` & `moodle-sdk-2.0.8/mdk/scripts/undev.php`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/scripts/users.php` & `moodle-sdk-2.0.8/mdk/scripts/users.php`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/scripts/version.php` & `moodle-sdk-2.0.8/mdk/scripts/version.php`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/scripts/webservices.php` & `moodle-sdk-2.0.8/mdk/scripts/webservices.php`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/scripts.py` & `moodle-sdk-2.0.8/mdk/scripts.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/tools.py` & `moodle-sdk-2.0.8/mdk/tools.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/mdk/version.py` & `moodle-sdk-2.0.8/mdk/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 http://github.com/FMCorz/mdk
 """
 
-__version__ = "2.0.7"
+__version__ = "2.0.8"
```

### Comparing `moodle-sdk-2.0.7/mdk/workplace.py` & `moodle-sdk-2.0.8/mdk/workplace.py`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/moodle_sdk.egg-info/PKG-INFO` & `moodle-sdk-2.0.8/moodle_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moodle-sdk
-Version: 2.0.7
+Version: 2.0.8
 Summary: Moodle Development Kit
 Home-page: https://github.com/FMCorz/mdk
 Author: Frédéric Massart
 Author-email: fred@fmcorz.net
 License: MIT
 Keywords: mdk moodle moodle-sdk
 Classifier: Development Status :: 6 - Mature
```

### Comparing `moodle-sdk-2.0.7/moodle_sdk.egg-info/SOURCES.txt` & `moodle-sdk-2.0.8/moodle_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moodle-sdk-2.0.7/setup.py` & `moodle-sdk-2.0.8/setup.py`

 * *Files identical despite different names*

