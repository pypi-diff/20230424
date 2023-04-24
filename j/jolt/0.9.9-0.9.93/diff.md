# Comparing `tmp/jolt-0.9.9.tar.gz` & `tmp/jolt-0.9.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jolt-0.9.9.tar", last modified: Sun Feb  2 19:25:58 2020, max compression
+gzip compressed data, was "jolt-0.9.93.tar", last modified: Mon Apr 24 07:35:25 2023, max compression
```

## Comparing `jolt-0.9.9.tar` & `jolt-0.9.93.tar`

### file list

```diff
@@ -1,64 +1,86 @@
-drwxr-xr-x   0 rbrt      (1000) rbrt      (1000)        0 2020-02-02 19:25:58.000000 jolt-0.9.9/
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)     1128 2020-02-02 19:25:58.000000 jolt-0.9.9/PKG-INFO
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)      447 2018-12-26 14:39:48.000000 jolt-0.9.9/README.rst
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)     3798 2020-02-02 19:25:27.000000 jolt-0.9.9/setup.py
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)       38 2020-02-02 19:25:58.000000 jolt-0.9.9/setup.cfg
-drwxr-xr-x   0 rbrt      (1000) rbrt      (1000)        0 2020-02-02 19:25:58.000000 jolt-0.9.9/jolt/
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)    33811 2019-11-02 12:37:23.000000 jolt-0.9.9/jolt/tasks.py
-drwxr-xr-x   0 rbrt      (1000) rbrt      (1000)        0 2020-02-02 19:25:58.000000 jolt-0.9.9/jolt/plugins/
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)     6506 2019-10-31 19:39:05.000000 jolt-0.9.9/jolt/plugins/ftp.py
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)     9922 2019-09-08 17:00:52.000000 jolt-0.9.9/jolt/plugins/jenkins.py
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)     3178 2020-01-30 21:22:23.000000 jolt-0.9.9/jolt/plugins/selfdeploy.py
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)     1245 2019-09-29 09:53:13.000000 jolt-0.9.9/jolt/plugins/autoweight.py
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)        0 2018-12-23 13:37:15.000000 jolt-0.9.9/jolt/plugins/__init__.py
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)     1641 2019-09-29 09:53:13.000000 jolt-0.9.9/jolt/plugins/logstash.py
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)     3593 2019-10-31 19:39:05.000000 jolt-0.9.9/jolt/plugins/volume.py
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)     1901 2019-12-21 20:35:23.000000 jolt-0.9.9/jolt/plugins/yamltask.py
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)     1383 2019-04-22 15:38:27.000000 jolt-0.9.9/jolt/plugins/strings.py
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)     1080 2019-10-31 19:39:05.000000 jolt-0.9.9/jolt/plugins/symlinks.py
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)    30127 2020-02-01 10:45:43.000000 jolt-0.9.9/jolt/plugins/amqp.py
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)     1858 2019-10-31 19:39:05.000000 jolt-0.9.9/jolt/plugins/ninja-cache.py
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)     2649 2019-09-29 09:53:13.000000 jolt-0.9.9/jolt/plugins/cxxinfo.py
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)     1554 2019-10-31 19:39:05.000000 jolt-0.9.9/jolt/plugins/gerrit.py
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)     4163 2020-02-01 16:37:19.000000 jolt-0.9.9/jolt/plugins/artifactory.py
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)     2882 2019-09-29 09:53:13.000000 jolt-0.9.9/jolt/plugins/python.py
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)    39062 2020-01-30 21:22:23.000000 jolt-0.9.9/jolt/plugins/ninja.py
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)     8937 2019-04-22 17:15:44.000000 jolt-0.9.9/jolt/plugins/repo.py
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)    11483 2020-01-30 21:22:23.000000 jolt-0.9.9/jolt/plugins/git.py
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)     2809 2019-09-29 09:53:13.000000 jolt-0.9.9/jolt/plugins/environ.py
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)     7280 2019-10-31 19:39:05.000000 jolt-0.9.9/jolt/plugins/ninjacli.py
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)     1630 2019-09-08 17:00:52.000000 jolt-0.9.9/jolt/hooks.py
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)      654 2019-09-09 17:48:33.000000 jolt-0.9.9/jolt/colors.py
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)    37939 2020-01-30 21:22:23.000000 jolt-0.9.9/jolt/tools.py
-drwxr-xr-x   0 rbrt      (1000) rbrt      (1000)        0 2020-02-02 19:25:58.000000 jolt-0.9.9/jolt/tps/
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)        0 2018-12-23 11:08:44.000000 jolt-0.9.9/jolt/tps/__init__.py
-drwxr-xr-x   0 rbrt      (1000) rbrt      (1000)        0 2020-02-02 19:25:58.000000 jolt-0.9.9/jolt/tps/pkg/
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)       34 2018-12-23 11:08:44.000000 jolt-0.9.9/jolt/tps/pkg/__init__.py
-drwxr-xr-x   0 rbrt      (1000) rbrt      (1000)        0 2020-02-02 19:25:58.000000 jolt-0.9.9/jolt/tps/jenkins/
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)    76881 2019-04-19 07:41:39.000000 jolt-0.9.9/jolt/tps/jenkins/__init__.py
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)      786 2018-12-23 11:08:44.000000 jolt-0.9.9/jolt/tps/jenkins/version.py
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)     3819 2018-12-23 11:08:44.000000 jolt-0.9.9/jolt/tps/jenkins/plugins.py
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)      879 2019-06-21 13:10:30.000000 jolt-0.9.9/jolt/__init__.py
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)    17255 2020-02-01 17:18:02.000000 jolt-0.9.9/jolt/scheduler.py
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)     4043 2019-10-31 19:39:05.000000 jolt-0.9.9/jolt/config.py
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)    32651 2019-10-31 19:39:05.000000 jolt-0.9.9/jolt/cache.py
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)      839 2019-09-29 09:53:13.000000 jolt-0.9.9/jolt/__main__.py
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)     6433 2019-10-31 19:39:05.000000 jolt-0.9.9/jolt/manifest.py
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)     9151 2019-10-31 19:39:05.000000 jolt-0.9.9/jolt/influence.py
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)     1483 2019-09-29 09:53:13.000000 jolt-0.9.9/jolt/error.py
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)     7530 2019-09-28 11:37:53.000000 jolt-0.9.9/jolt/log.py
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)      351 2019-10-31 19:39:05.000000 jolt-0.9.9/jolt/options.py
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)     2330 2019-04-22 15:38:27.000000 jolt-0.9.9/jolt/expires.py
--rwxr-xr-x   0 rbrt      (1000) rbrt      (1000)    19758 2019-12-17 18:06:03.000000 jolt-0.9.9/jolt/cli.py
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)     2767 2019-12-17 18:06:03.000000 jolt-0.9.9/jolt/filesystem.py
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)     5399 2019-10-31 19:39:05.000000 jolt-0.9.9/jolt/xmldom.py
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)    17863 2020-02-01 17:09:28.000000 jolt-0.9.9/jolt/graph.py
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)     7065 2020-01-30 21:22:36.000000 jolt-0.9.9/jolt/loader.py
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)     8840 2019-10-31 19:39:05.000000 jolt-0.9.9/jolt/utils.py
-drwxr-xr-x   0 rbrt      (1000) rbrt      (1000)        0 2020-02-02 19:25:58.000000 jolt-0.9.9/jolt.egg-info/
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)     1128 2020-02-02 19:25:58.000000 jolt-0.9.9/jolt.egg-info/PKG-INFO
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)        5 2020-02-02 19:25:58.000000 jolt-0.9.9/jolt.egg-info/top_level.txt
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)        1 2020-02-02 19:25:58.000000 jolt-0.9.9/jolt.egg-info/dependency_links.txt
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)      196 2020-02-02 19:25:58.000000 jolt-0.9.9/jolt.egg-info/requires.txt
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)     1144 2020-02-02 19:25:58.000000 jolt-0.9.9/jolt.egg-info/SOURCES.txt
--rw-r--r--   0 rbrt      (1000) rbrt      (1000)       45 2020-02-02 19:25:58.000000 jolt-0.9.9/jolt.egg-info/entry_points.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 07:35:25.837291 jolt-0.9.93/
+-rw-r--r--   0 root         (0) root         (0)     4189 2023-04-24 07:35:25.837291 jolt-0.9.93/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3130 2023-04-24 07:35:25.000000 jolt-0.9.93/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 07:35:25.805291 jolt-0.9.93/jolt/
+-rw-r--r--   0 root         (0) root         (0)     1437 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1393 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    59840 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/cache.py
+-rwxr-xr-x   0 root         (0) root         (0)    39083 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/cli.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/colors.py
+-rw-r--r--   0 root         (0) root         (0)     8543 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/config.py
+-rw-r--r--   0 root         (0) root         (0)     2110 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/error.py
+-rw-r--r--   0 root         (0) root         (0)     2330 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/expires.py
+-rw-r--r--   0 root         (0) root         (0)     5969 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/filesystem.py
+-rw-r--r--   0 root         (0) root         (0)    22861 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/graph.py
+-rw-r--r--   0 root         (0) root         (0)     9979 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/hooks.py
+-rw-r--r--   0 root         (0) root         (0)    15426 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/influence.py
+-rw-r--r--   0 root         (0) root         (0)     3931 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/inspection.py
+-rw-r--r--   0 root         (0) root         (0)    10264 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/loader.py
+-rw-r--r--   0 root         (0) root         (0)    11117 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/log.py
+-rw-r--r--   0 root         (0) root         (0)     7639 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/manifest.py
+-rw-r--r--   0 root         (0) root         (0)      371 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 07:35:25.809291 jolt-0.9.93/jolt/pkgs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/pkgs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1153 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/pkgs/golang.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/pkgs/nodejs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 07:35:25.837291 jolt-0.9.93/jolt/plugins/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      313 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/plugins/alias.py
+-rw-r--r--   0 root         (0) root         (0)    10151 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/plugins/allure.py
+-rw-r--r--   0 root         (0) root         (0)    32129 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/plugins/amqp.py
+-rw-r--r--   0 root         (0) root         (0)     1245 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/plugins/autoweight.py
+-rw-r--r--   0 root         (0) root         (0)     2687 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/plugins/cmake.py
+-rw-r--r--   0 root         (0) root         (0)     7654 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/plugins/conan.py
+-rw-r--r--   0 root         (0) root         (0)     2398 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/plugins/cxxinfo.py
+-rw-r--r--   0 root         (0) root         (0)      641 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/plugins/dashboard.py
+-rw-r--r--   0 root         (0) root         (0)    11569 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/plugins/debian.py
+-rw-r--r--   0 root         (0) root         (0)    19171 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/plugins/docker.py
+-rw-r--r--   0 root         (0) root         (0)     3356 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/plugins/email.py
+-rw-r--r--   0 root         (0) root         (0)     7200 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/plugins/email.xslt
+-rw-r--r--   0 root         (0) root         (0)     3371 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/plugins/environ.py
+-rw-r--r--   0 root         (0) root         (0)     6545 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/plugins/ftp.py
+-rw-r--r--   0 root         (0) root         (0)     5727 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/plugins/gdb.py
+-rw-r--r--   0 root         (0) root         (0)     1420 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/plugins/gerrit.py
+-rw-r--r--   0 root         (0) root         (0)    14483 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/plugins/git.py
+-rw-r--r--   0 root         (0) root         (0)     2049 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/plugins/golang.py
+-rw-r--r--   0 root         (0) root         (0)      191 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/plugins/googletest.py
+-rw-r--r--   0 root         (0) root         (0)     4002 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/plugins/http.py
+-rw-r--r--   0 root         (0) root         (0)     1342 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/plugins/junit.py
+-rw-r--r--   0 root         (0) root         (0)     1788 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/plugins/logstash.py
+-rw-r--r--   0 root         (0) root         (0)     8212 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/plugins/ninja-compdb.py
+-rw-r--r--   0 root         (0) root         (0)    73139 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/plugins/ninja.py
+-rw-r--r--   0 root         (0) root         (0)     1879 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/plugins/nodejs.py
+-rw-r--r--   0 root         (0) root         (0)     1686 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/plugins/paths.py
+-rw-r--r--   0 root         (0) root         (0)    20101 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/plugins/podman.py
+-rw-r--r--   0 root         (0) root         (0)     3073 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/plugins/python.py
+-rw-r--r--   0 root         (0) root         (0)     8947 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/plugins/repo.py
+-rw-r--r--   0 root         (0) root         (0)     2179 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/plugins/report.py
+-rw-r--r--   0 root         (0) root         (0)     5994 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/plugins/selfdeploy.py
+-rw-r--r--   0 root         (0) root         (0)     1538 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/plugins/strings.py
+-rw-r--r--   0 root         (0) root         (0)     1921 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/plugins/symlinks.py
+-rw-r--r--   0 root         (0) root         (0)     3461 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/plugins/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)     1620 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/plugins/timeline.py
+-rw-r--r--   0 root         (0) root         (0)     3583 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/plugins/volume.py
+-rw-r--r--   0 root         (0) root         (0)     3060 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/plugins/yaml-ninja.py
+-rw-r--r--   0 root         (0) root         (0)     3528 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/plugins/yamltask.py
+-rw-r--r--   0 root         (0) root         (0)    18464 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/scheduler.py
+-rw-r--r--   0 root         (0) root         (0)    85933 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 07:35:25.837291 jolt-0.9.93/jolt/templates/
+-rw-r--r--   0 root         (0) root         (0)     1720 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/templates/cxxexecutable.cmake.template
+-rw-r--r--   0 root         (0) root         (0)     1750 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/templates/cxxlibrary.cmake.template
+-rw-r--r--   0 root         (0) root         (0)     1778 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/templates/export.sh.template
+-rw-r--r--   0 root         (0) root         (0)     1410 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/templates/timeline.html.template
+-rw-r--r--   0 root         (0) root         (0)    68277 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/tools.py
+-rw-r--r--   0 root         (0) root         (0)    12977 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/utils.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/version.py
+-rw-r--r--   0 root         (0) root         (0)     3900 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/version_utils.py
+-rw-r--r--   0 root         (0) root         (0)     5543 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt/xmldom.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 07:35:25.805291 jolt-0.9.93/jolt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4189 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1702 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      618 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-04-24 07:35:25.000000 jolt-0.9.93/jolt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 07:35:25.841291 jolt-0.9.93/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3015 2023-04-24 07:35:25.000000 jolt-0.9.93/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `jolt-0.9.9/jolt/plugins/ftp.py` & `jolt-0.9.93/jolt/plugins/ftp.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 CONNECT_TIMEOUT = 3.5
 
 
 def catch(func, *args, **kwargs):
     try:
         val = func(*args, **kwargs)
         return val if val is not None else True
-    except:
+    except Exception:
+        log.exception()
         return False
 
 
 class FtpStorage(cache.StorageProvider):
     def __init__(self, cache):
         super(FtpStorage, self).__init__()
         self._cache = cache
@@ -40,21 +41,20 @@
     def _get_auth(self):
         service = config.get(NAME, "keyring.service")
         if not service:
             return None, None
 
         username = config.get(NAME, "keyring.username")
         if not username:
-            username = raw_input(NAME + " username: ")
+            username = input(NAME + " username: ")
             raise_error_if(not username, "no username configured for " + NAME)
             config.set(NAME, "keyring.username", username)
             config.save()
 
-        password = config.get(NAME, "keyring.password") or \
-                   keyring.get_password(NAME, username)
+        password = config.get(NAME, "keyring.password") or keyring.get_password(NAME, username)
         if not password:
             password = getpass.getpass(NAME + " password: ")
             raise_error_if(not password, "no password in keyring for " + NAME)
             keyring.set_password(service, username, password)
         return username, password
 
     def _get_ftp(self):
@@ -72,15 +72,15 @@
                     ftp.cwd("/")
                 components = self._path.split("/")
                 for component in components:
                     if not catch(ftp.cwd, component):
                         ftp.mkd(component)
                         ftp.cwd(component)
             return ftp
-        except:
+        except Exception:
             log.exception()
             log.warning("[FTP] failed to establish server connection, disabled")
             self._disabled = True
         return None
 
     @utils.retried.on_exception((RequestException))
     def download(self, node, force=False):
@@ -93,15 +93,15 @@
             if ftp is None:
                 return False
             pathname = artifact.get_archive_path()
             name = fs.path.basename(pathname)
             try:
                 ftp.cwd(node.canonical_name)
                 size = ftp.size(name)
-            except:
+            except Exception:
                 return False
             with log.progress("Downloading {0}".format(name), size, "B") as pbar:
                 with open(pathname, 'wb') as out_file:
                     def _write(block):
                         out_file.write(block)
                         pbar.update(len(block))
                     return catch(ftp.retrbinary,
@@ -164,15 +164,15 @@
                         user=username,
                         uri=self._uri,
                         path=self._path,
                         taskname=node.canonical_name,
                         archive=name)
                     log.debug("[FTP] {0}", url)
                     return url
-            except:
+            except Exception:
                 return False
         return False
 
 
 @cache.RegisterStorage
 class FtpStorageFactory(cache.StorageProviderFactory):
     @staticmethod
```

### Comparing `jolt-0.9.9/jolt/plugins/autoweight.py` & `jolt-0.9.93/jolt/plugins/autoweight.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.9/jolt/plugins/logstash.py` & `jolt-0.9.93/jolt/plugins/logstash.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,53 +1,54 @@
+from contextlib import contextmanager
 from datetime import datetime
 
-from jolt import *
 from jolt import config
 from jolt import filesystem as fs
 from jolt import log
-from jolt import utils
 from jolt.error import raise_error_if
 from jolt.hooks import TaskHook, TaskHookFactory
 
 
 log.verbose("[LogStash] Loaded")
 
 
 class LogStashHooks(TaskHook):
     def __init__(self):
         self._uri = config.get("logstash", "http.uri")
-        self._failed_enabled = config.get("logstash", "failed", False)
-        self._finished_enabled = config.get("logstash", "finished", False)
+        self._failed_enabled = config.getboolean("logstash", "failed", False)
+        self._finished_enabled = config.getboolean("logstash", "finished", False)
         raise_error_if(not self._uri, "logstash.http.uri not configured")
 
     def _get_uri(self, task):
         return "{}/{}-{}.txt".format(
             self._uri,
             datetime.now().strftime("%Y-%m-%d_%H%M%S.%f"),
             task.canonical_name)
 
-    def _stash_log(self, task):
+    def _stash_log(self, task, logbuffer):
         with task.tools.tmpdir("logstash") as t:
             filepath = fs.path.join(t.path, "log")
             with open(filepath, "w") as f:
-                f.write(task.logsink_buffer.getvalue())
-            task.tools.upload(filepath, self._get_uri(task))
-
-    def task_started(self, task):
-        task.logsink = log.threadsink()
-        task.logsink_buffer = task.logsink.__enter__()
-
-    def task_failed(self, task):
-        task.logsink.__exit__(None, None, None)
-        if self._failed_enabled:
-            self._stash_log(task)
-
-    def task_finished(self, task):
-        task.logsink.__exit__(None, None, None)
-        if self._finished_enabled:
-            self._stash_log(task)
-
-
-@TaskHookFactory.register
+                f.write(logbuffer)
+            task.logstash = self._get_uri(task)
+            task.tools.upload(filepath, task.logstash, exceptions=False)
+
+    @contextmanager
+    def task_run(self, task):
+        with log.threadsink() as logsink:
+            try:
+                yield
+            except Exception as e:
+                if self._failed_enabled:
+                    self._stash_log(task, logsink.getvalue())
+                raise e
+            else:
+                if self._finished_enabled:
+                    self._stash_log(task, logsink.getvalue())
+
+
+# Must run before other plugins which depend on the
+# logstash_uri TaskProxy attribute.
+@TaskHookFactory.register_with_prio(10)
 class LogStashFactory(TaskHookFactory):
     def create(self, env):
         return LogStashHooks()
```

### Comparing `jolt-0.9.9/jolt/plugins/volume.py` & `jolt-0.9.93/jolt/plugins/volume.py`

 * *Files 11% similar despite different names*

```diff
@@ -53,15 +53,15 @@
                 return True
             except OSError as e:
                 if e.errno == errno.ESTALE:
                     log.verbose("[VOLUME] got stale file handle, retrying...")
                     raise StaleFileHandleError(e)
                 else:
                     log.exception()
-            except Exception as e:
+            except Exception:
                 log.exception()
 
         return False
 
     def download_enabled(self):
         return self._download
 
@@ -80,15 +80,15 @@
                 else:
                     fs.unlink(temp)
                 return True
             except OSError as e:
                 if e.errno != errno.EEXIST:
                     log.verbose("[VOLUME] Failed to copy artifact, errno={}", os.strerror(e.errno))
                 return e.errno == errno.EEXIST
-            except Exception as e:
+            except Exception:
                 log.exception()
             finally:
                 fs.unlink(temp, ignore_errors=True)
         return False
 
     def upload_enabled(self):
         return self._upload
```

### Comparing `jolt-0.9.9/jolt/plugins/strings.py` & `jolt-0.9.93/jolt/plugins/strings.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 from jolt.cache import ArtifactAttributeSet
 from jolt.cache import ArtifactAttributeSetProvider
 from jolt.cache import ArtifactStringAttribute
 
 
 class StringVariable(ArtifactStringAttribute):
-    def __init__(self, name):
-        super(StringVariable, self).__init__(name)
+    def __init__(self, artifact, name):
+        super(StringVariable, self).__init__(artifact, name)
         self._old_value = None
 
     def apply(self, task, artifact):
         pass
 
     def unapply(self, task, artifact):
         pass
 
 
 class StringVariableSet(ArtifactAttributeSet):
-    def __init__(self):
+    def __init__(self, artifact):
         super(StringVariableSet, self).__init__()
+        super(ArtifactAttributeSet, self).__setattr__("_artifact", artifact)
 
     def create(self, name):
-        return StringVariable(name)
+        return StringVariable(self._artifact, name)
 
 
 @ArtifactAttributeSetProvider.Register
 class StringVariableSetProvider(ArtifactAttributeSetProvider):
     def create(self, artifact):
-        setattr(artifact, "strings", StringVariableSet())
+        setattr(artifact, "strings", StringVariableSet(artifact))
 
     def parse(self, artifact, content):
         if "strings" not in content:
             return
 
         for key, value in content["strings"].items():
-            setattr(artifact.strings, key, value)
+            getattr(artifact.strings, key).set_value(value, expand=False)
 
     def format(self, artifact, content):
         if "strings" not in content:
             content["strings"] = {}
 
         for key, value in artifact.strings.items():
             content["strings"][key] = str(value)
```

### Comparing `jolt-0.9.9/jolt/plugins/amqp.py` & `jolt-0.9.93/jolt/plugins/amqp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 import click
 import functools
 import getpass
 import keyring
 import os
-import pika
-from pika.exceptions import AMQPConnectionError
-from pika.adapters.utils.connection_workflow import AMQPConnectorStackTimeout
+try:
+    import pika
+    from pika.exceptions import AMQPConnectionError
+    from pika.adapters.utils.connection_workflow import AMQPConnectorStackTimeout
+except ImportError:
+    from jolt import log
+    log.error("AMQP plugin enabled but not installed. Install it with: pip install jolt[amqp]")
+    os._exit(1)
+
 import threading
 import time
-import uuid
 
 from jolt.cli import cli
 from jolt import config
 from jolt import filesystem as fs
+from jolt import hooks
 from jolt import log
 from jolt import scheduler
 from jolt import utils
 from jolt.manifest import JoltManifest
 from jolt.tools import Tools
 from jolt.error import JoltCommandError
 from jolt.error import raise_error
@@ -30,16 +36,15 @@
 def _get_auth():
     service = config.get(NAME, "keyring.service", NAME)
 
     username = config.get(NAME, "keyring.username")
     if not username:
         return "guest", "guest"
 
-    password = config.get(NAME, "keyring.password") or \
-               keyring.get_password(NAME, username)
+    password = config.get(NAME, "keyring.password") or keyring.get_password(NAME, username)
     if not password:
         password = getpass.getpass(NAME + " password: ")
         assert password, "no password in keyring for " + NAME
         keyring.set_password(service, username, password)
     return username, password
 
 
@@ -96,14 +101,15 @@
         # for higher consumer throughput
         self._prefetch_count = 1
         self._job = None
         self._routing_key = self.ROUTING_KEY_PREFIX + config.get(
             "amqp", "routing_key",
             os.getenv("RABBITMQ_ROUTING_KEY", self.ROUTING_KEY_REQUEST))
         self._queue = self.QUEUE + "_" + self._routing_key
+        self._max_priority = config.getint("amqp", "max-priority", 1)
 
     def connect(self):
         """This method connects to RabbitMQ, returning the connection handle.
         When the connection is established, the on_connection_open method
         will be invoked by pika.
 
         :rtype: pika.SelectConnection
@@ -254,15 +260,18 @@
         :param str|unicode queue_name: The name of the queue to declare.
 
         """
         log.info('Declaring queue {}', queue_name)
         cb = functools.partial(self.on_queue_declareok, userdata=queue_name)
         self._channel.queue_declare(
             queue=queue_name, callback=cb,
-            arguments={"x-message-deduplication": True})
+            arguments={
+                "x-message-deduplication": True,
+                "x-max-priority": self._max_priority
+            })
 
     def on_queue_declareok(self, _unused_frame, userdata):
         """Method invoked by pika when the Queue.Declare RPC call made in
         setup_queue has completed. In this method we will bind the queue
         and exchange together with the routing key by issuing the Queue.Bind
         RPC command. When this command is complete, the on_bindok method will
         be invoked by pika.
@@ -276,14 +285,20 @@
                  self.EXCHANGE, queue_name, self._routing_key)
         cb = functools.partial(self.on_bindok, userdata=queue_name)
         self._channel.queue_bind(
             queue_name,
             self.EXCHANGE,
             routing_key=self._routing_key,
             callback=cb)
+        log.info('Binding {} to {} with jolt_{}',
+                 self.EXCHANGE, queue_name, self._routing_key)
+        self._channel.queue_bind(
+            queue_name,
+            self.EXCHANGE,
+            routing_key="jolt_" + self._routing_key)
 
     def on_bindok(self, _unused_frame, userdata):
         """Invoked by pika when the Queue.Bind method has completed. At this
         point we will set the prefetch count for the channel.
 
         :param pika.frame.Method _unused_frame: The Queue.BindOk response frame
         :param str|unicode userdata: Extra user data (queue name)
@@ -400,22 +415,24 @@
                         try:
                             fs.makedirs(src)
                             tools.run("curl {} | tar zx -C {}", url, src)
                             tools.run("virtualenv {}", env)
                             tools.run(". {}/bin/activate && pip install -e {}", env, src)
                             if requires:
                                 tools.run(". {}/bin/activate && pip install {}", env, requires)
+                            if "autocompletion=" in tools.read_file(f"{src}/jolt/cli.py"):
+                                tools.run(". {}/bin/activate && pip install 'click<8.1'", env, src)
                         except Exception as e:
                             tools.rmtree("build/selfdeploy/{}", ident, ignore_errors=True)
                             raise e
 
                     return ". {}/bin/activate && jolt".format(env)
-                except:
+                except Exception as e:
                     log.exception()
-                return "jolt"
+                    raise e
 
             def run(self):
                 with open("default.joltxmanifest", "wb") as f:
                     f.write(self.body)
 
                 log.info("Manifest written")
 
@@ -434,48 +451,48 @@
                               jolt, config_file, output_stdio=True)
                 except JoltCommandError as e:
                     self.response = ""
                     try:
                         manifest = JoltManifest()
                         try:
                             manifest.parse("result.joltxmanifest")
-                        except:
+                        except Exception:
                             manifest.duration = "0"
                         manifest.result = "FAILED"
                         manifest.stdout = "\n".join(e.stdout)
                         manifest.stderr = "\n".join(e.stderr)
                         self.response = manifest.format()
-                    except:
+                    except Exception:
                         log.exception()
                     log.error("Task failed")
-                except Exception as e:
+                except Exception:
                     log.exception()
                     self.response = ""
                     try:
                         manifest = JoltManifest()
                         try:
                             manifest.parse("result.joltxmanifest")
-                        except:
+                        except Exception:
                             manifest.duration = "0"
                         manifest.result = "FAILED"
                         self.response = manifest.format()
-                    except:
+                    except Exception:
                         log.exception()
                     log.error("Task failed")
                 else:
                     self.response = ""
                     try:
                         manifest = JoltManifest()
                         try:
                             manifest.parse("result.joltxmanifest")
-                        except:
+                        except Exception:
                             manifest.duration = "0"
                         manifest.result = "SUCCESS"
                         self.response = manifest.format()
-                    except:
+                    except Exception:
                         log.exception()
                     log.info("Task succeeded")
 
                 utils.call_and_catch(tools.unlink, "result.joltxmanifest")
                 self.consumer.add_on_job_completed_callback(self)
 
         self._job = Job(self, channel, basic_deliver, properties, body)
@@ -631,89 +648,99 @@
 
 
 class AmqpExecutor(scheduler.NetworkExecutor):
 
     def __init__(self, factory, task):
         super(AmqpExecutor, self).__init__(factory)
         self.factory = factory
-        self.task = task
         self.callback_queue = None
+        self.connection = None
+        self.priority = config.getint("amqp", "priority", 0)
+        self.task = task
 
     def _create_manifest(self):
         manifest = JoltManifest.export(self.task)
         build = manifest.create_build()
 
         tasks = [self.task.qualified_name]
         tasks += [t.qualified_name for t in self.task.extensions]
 
         for task in tasks:
             mt = build.create_task()
             mt.name = task
 
-        for task in self.factory.options.default:
-            default = build.create_default()
-            default.name = task
-
         registry = scheduler.ExecutorRegistry.get()
         for key, value in registry.get_network_parameters(self.task).items():
             param = manifest.create_parameter()
             param.key = key
             param.value = value
 
         routing_key = WorkerTaskConsumer.ROUTING_KEY_PREFIX
         routing_key += getattr(self.task.task, "routing_key", WorkerTaskConsumer.ROUTING_KEY_REQUEST)
 
         return manifest.format(), routing_key
 
     def _run(self, env):
+        timeout = int(config.getint("amqp", "timeout", 300))
         manifest, routing_key = self._create_manifest()
 
         self.connect()
         self.publish_request(manifest, routing_key)
 
         log.debug("[AMQP] Queued {0}", self.task.short_qualified_name)
 
         self.task.running()
         for extension in self.task.extensions:
             extension.running()
 
         while self.response is None:
             try:
-                self.connection.process_data_events(None)
+                self.connection.process_data_events(time_limit=timeout)
+                if self.response is None:
+                    self.task.info("Remote execution still in progress after {}",
+                                   self.task.duration_queued)
             except (ConnectionError, AMQPConnectionError):
                 log.warning("[AMQP] Lost server connection")
                 self.connect()
 
         log.debug("[AMQP] Finished {0}", self.task.short_qualified_name)
 
         manifest = JoltManifest()
         with raise_task_error_on_exception(self.task, "failed to parse build result manifest"):
             manifest.parsestring(self.response)
 
         self.task.running(utils.duration() - float(manifest.duration))
 
         if manifest.result != "SUCCESS":
             output = []
-            output.extend(manifest.stdout.split("\n"))
-            output.extend(manifest.stderr.split("\n"))
+            if manifest.stdout:
+                output.extend(manifest.stdout.split("\n"))
+            if manifest.stderr:
+                output.extend(manifest.stderr.split("\n"))
             for line in output:
                 log.transfer(line, self.task.identity[:8])
+            for task in [self.task] + self.task.extensions:
+                with task.task.report() as report:
+                    remote_report = manifest.find_task(task.qualified_name)
+                    if remote_report:
+                        for error in remote_report.errors:
+                            report.manifest.append(error)
             raise_error("[AMQP] remote build failed with status: {0}".format(manifest.result))
 
         raise_task_error_if(
-            not env.cache.is_available_remotely(self.task), self.task,
+            self.task.has_artifact() and not env.cache.is_available_remotely(self.task), self.task,
             "no task artifact available in any cache, check configuration")
 
         raise_task_error_if(
-            not env.cache.download(self.task) and env.cache.download_enabled(),
+            self.task.has_artifact() and not env.cache.download(self.task) and env.cache.download_enabled(),
             self.task, "failed to download task artifact")
 
         for extension in self.task.extensions:
             raise_task_error_if(
-                not env.cache.download(extension) and env.cache.download_enabled(),
+                self.task.has_artifact() and not env.cache.download(extension) and env.cache.download_enabled(),
                 self.task, "failed to download task artifact")
 
         return self.task
 
     @utils.retried.on_exception((ConnectionError, AMQPConnectionError, AMQPConnectorStackTimeout))
     def connect(self):
         self.connection = pika.BlockingConnection(
@@ -744,43 +771,52 @@
             channel.basic_ack(basic_deliver.delivery_tag)
         else:
             channel.basic_ack(basic_deliver.delivery_tag)
 
     def publish_request(self, manifest, routing_key):
         props = pika.BasicProperties(
             correlation_id=self.corr_id,
+            priority=self.priority,
             headers={"x-deduplication-header": self.task.identity})
         self.response = None
         self.channel.basic_publish(
             exchange=WorkerTaskConsumer.EXCHANGE,
             routing_key=routing_key,
             properties=props,
             body=manifest)
 
     def run(self, env):
         try:
             self.task.started(TYPE)
+            hooks.task_started_execution(self.task)
             for extension in self.task.extensions:
                 extension.started(TYPE)
-            self._run(env)
+                hooks.task_started_execution(extension)
+            with hooks.task_run([self.task] + self.task.extensions):
+                self._run(env)
             for extension in self.task.extensions:
+                hooks.task_finished_execution(extension)
                 extension.finished(TYPE)
+            hooks.task_finished_execution(self.task)
             self.task.finished(TYPE)
-        except (ConnectionError, AMQPConnectionError) as e:
+        except (ConnectionError, AMQPConnectionError):
             log.exception()
             for extension in self.task.extensions:
                 extension.failed(TYPE)
             self.task.failed(TYPE)
             raise_error("Lost connection to AMQP server")
         except Exception as e:
             log.exception()
             for extension in self.task.extensions:
                 extension.failed(TYPE)
             self.task.failed(TYPE)
             raise e
+        finally:
+            if self.connection is not None:
+                utils.call_and_catch(self.connection.close)
         return self.task
 
 
 @scheduler.ExecutorFactory.Register
 class AmqpExecutorFactory(scheduler.NetworkExecutorFactory):
     def __init__(self, options):
         workers = config.getint(NAME, "workers", 16)
```

### Comparing `jolt-0.9.9/jolt/plugins/cxxinfo.py` & `jolt-0.9.93/jolt/plugins/python.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,87 +1,100 @@
+import sys
+
 from jolt import filesystem as fs
 from jolt.cache import ArtifactStringAttribute
 from jolt.cache import ArtifactAttributeSet
 from jolt.cache import ArtifactAttributeSetProvider
 
 
-class CppInfoVariable(ArtifactStringAttribute):
-    def __init__(self, name):
-        super(CppInfoVariable, self).__init__(name)
+class PythonVariable(ArtifactStringAttribute):
+    def __init__(self, artifact, name):
+        super(PythonVariable, self).__init__(artifact, name)
 
     def apply(self, task, artifact):
         pass
 
     def unapply(self, task, artifact):
         pass
 
 
-class CppInfoListVariable(CppInfoVariable):
-    def __init__(self, name):
-        super(CppInfoListVariable, self).__init__(name)
+class PythonListVariable(PythonVariable):
+    def __init__(self, artifact, name):
+        super(PythonListVariable, self).__init__(artifact, name)
 
     def append(self, value):
         if self.get_value():
             self.set_value(self.get_value() + ":" + value)
         else:
             self.set_value(value)
 
     def items(self):
         value = self.get_value()
         return value.split(":") if value is not None else []
 
 
-class CppInfoDictVariable(CppInfoListVariable):
-    def __init__(self, name):
-        super(CppInfoDictVariable, self).__init__(name)
+class PythonPathVariable(PythonListVariable):
+    def __init__(self, artifact, name):
+        super(PythonPathVariable, self).__init__(artifact, name)
+
+    def append(self, value):
+        if self.get_value():
+            self.set_value(self.get_value() + ":" + value)
+        else:
+            self.set_value(value)
+
+    def items(self):
+        value = self.get_value()
+        return value.split(":") if value is not None else []
+
+    def apply(self, task, artifact):
+        paths = [fs.path.join(artifact.path, path) for path in self.items()]
+        sys.path.extend(paths)
+
+    def unapply(self, task, artifact):
+        paths = [fs.path.join(artifact.path, path) for path in self.items()]
+        for path in paths:
+            sys.path.remove(path)
+
+
+class PythonDictVariable(PythonListVariable):
+    def __init__(self, artifact, name):
+        super(PythonDictVariable, self).__init__(artifact, name)
 
     def __setitem__(self, key, value=None):
         item = "{0}={1}".format(key, value) if value is not None else key
         self.append(item)
 
 
-class CppInfo(ArtifactAttributeSet):
-    def __init__(self):
-        super(CppInfo, self).__init__()
+class Python(ArtifactAttributeSet):
+    def __init__(self, artifact):
+        super(Python, self).__init__()
+        super(ArtifactAttributeSet, self).__setattr__("_artifact", artifact)
 
     def create(self, name):
-        if name == "asflags":
-            return CppInfoListVariable("asflags")
-        if name == "cflags":
-            return CppInfoListVariable("cflags")
-        if name == "cxxflags":
-            return CppInfoListVariable("cxxflags")
-        if name == "incpaths":
-            return CppInfoListVariable("incpaths")
-        if name == "ldflags":
-            return CppInfoListVariable("ldflags")
-        if name == "libpaths":
-            return CppInfoListVariable("libpaths")
-        if name == "libraries":
-            return CppInfoListVariable("libraries")
-        if name == "macros":
-            return CppInfoDictVariable("macros")
-        assert False, "no such cxxinfo attribute: {0}".format(name)
+        if name.lower() == "path":
+            return PythonPathVariable(self._artifact, "PATH")
+        assert False, "No such python attribute: {0}".format(name)
 
 
 @ArtifactAttributeSetProvider.Register
-class CppInfoProvider(ArtifactAttributeSetProvider):
+class PythonProvider(ArtifactAttributeSetProvider):
     def create(self, artifact):
-        setattr(artifact, "cxxinfo", CppInfo())
+        setattr(artifact, "python", Python(artifact))
 
     def parse(self, artifact, content):
-        if "cxxinfo" not in content:
+        if "python" not in content:
             return
-        for key, value in content["cxxinfo"].items():
-            setattr(artifact.cxxinfo, key, value)
+        for key, value in content["python"].items():
+            setattr(artifact.python, key, value)
 
     def format(self, artifact, content):
-        if "cxxinfo" not in content:
-            content["cxxinfo"] = {}
-        for key, value in artifact.cxxinfo.items():
-            content["cxxinfo"][key] = str(value)
+        if "python" not in content:
+            content["python"] = {}
+        for key, value in artifact.python.items():
+            content["python"][key] = str(value)
 
     def apply(self, task, artifact):
-        pass
+        artifact.python.apply(task, artifact)
 
     def unapply(self, task, artifact):
-        pass
+        artifact.python.unapply(task, artifact)
```

### Comparing `jolt-0.9.9/jolt/plugins/gerrit.py` & `jolt-0.9.93/jolt/plugins/gerrit.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,27 +11,25 @@
     name = "gerrit-src"
     url = Parameter(help="URL to the Gerrit git repo to be cloned. Required.")
     sha = Parameter(required=False, help="Specific commit or tag to be checked out. Optional.")
     path = Parameter(required=False, help="Local path where the repository should be cloned.")
     _revision = Export(value=lambda self: self._get_revision() or self.git.head())
 
     def __init__(self, *args, **kwargs):
-        refspec1 = '+refs/heads/*:refs/remotes/gerrit/*'
-        refspec2 = '+refs/changes/*:refs/remotes/gerrit/changes/*'
-        super(GerritSrc, self).__init__(*args, refspecs=[refspec1, refspec2], **kwargs)
+        refspec1 = '+refs/changes/*:refs/remotes/origin/changes/*'
+        super(GerritSrc, self).__init__(*args, refspecs=[refspec1], **kwargs)
 
 
 class Gerrit(git.Git):
     name = "gerrit"
     url = Parameter(help="URL to the Gerrit git repo to be cloned. Required.")
     sha = Parameter(required=False, help="Specific commit or tag to be checked out. Optional.")
     path = Parameter(required=False, help="Local path where the repository should be cloned.")
     _revision = Export(value=lambda self: self._get_revision() or self.git.head())
 
     def __init__(self, *args, **kwargs):
-        refspec1 = '+refs/heads/*:refs/remotes/gerrit/*'
-        refspec2 = '+refs/changes/*:refs/remotes/gerrit/changes/*'
-        super(Gerrit, self).__init__(*args, refspecs=[refspec1, refspec2], **kwargs)
+        refspec1 = '+refs/changes/*:refs/remotes/origin/changes/*'
+        super(Gerrit, self).__init__(*args, refspecs=[refspec1], **kwargs)
 
 
 TaskRegistry.get().add_task_class(GerritSrc)
 TaskRegistry.get().add_task_class(Gerrit)
```

### Comparing `jolt-0.9.9/jolt/plugins/artifactory.py` & `jolt-0.9.93/jolt/plugins/http.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,34 @@
-import requests
 from requests.auth import HTTPBasicAuth
 from requests.exceptions import ConnectTimeout, RequestException
 import keyring
 import getpass
 
 
 from jolt import utils
 from jolt import cache
 from jolt import log
 from jolt import config
 from jolt import filesystem as fs
 from jolt.error import raise_error_if, JoltError
 
 
-NAME = "artifactory"
+NAME = "http"
 TIMEOUT = (3.5, 27)
 TIMEOUT_HEAD = (27, 27)
 
 
-class Artifactory(cache.StorageProvider):
+class Http(cache.StorageProvider):
     def __init__(self, cache):
-        super(Artifactory, self).__init__()
+        super(Http, self).__init__()
         self._cache = cache
         self._uri = config.get(NAME, "uri")
-        raise_error_if(not self._uri, "artifactory URI not configured")
+        raise_error_if(not self._uri, "HTTP URI not configured")
         if self._uri[-1] != "/":
             self._uri += "/"
-        self._repository = config.get(NAME, "repository", "jolt")
         self._upload = config.getboolean(NAME, "upload", True)
         self._download = config.getboolean(NAME, "download", True)
         self._disabled = False
 
     def _get_auth(self):
         service = config.get(NAME, "keyring.service")
         if not service:
@@ -39,38 +37,37 @@
         username = config.get(NAME, "keyring.username")
         if not username:
             username = utils.read_input(NAME + " username: ")
             raise_error_if(not username, "no username configured for " + NAME)
             config.set(NAME, "keyring.username", username)
             config.save()
 
-        password = config.get(NAME, "keyring.password") or \
-                   keyring.get_password(NAME, username)
+        password = config.get(NAME, "keyring.password") or keyring.get_password(NAME, username)
         if not password:
             password = getpass.getpass(NAME + " password: ")
             raise_error_if(not password, "no password in keyring for " + NAME)
             keyring.set_password(service, username, password)
+
         return HTTPBasicAuth(username, password)
 
     def _get_url(self, node, artifact):
-        return "{uri}{repository}/{name}/{file}".format(
+        return "{uri}/{name}/{file}".format(
             uri=self._uri,
-            repository=self._repository,
             name=node.name,
             file=fs.path.basename(artifact.get_archive_path()))
 
     @utils.retried.on_exception((RequestException, JoltError))
     def download(self, node, force=False):
         if self._disabled:
             return False
         if not self._download and not force:
             return False
         with self._cache.get_artifact(node) as artifact:
             url = self._get_url(node, artifact)
-            if node.tools.download(url, artifact.get_archive_path(), exceptions=True, timeout=TIMEOUT):
+            if node.tools.download(url, artifact.get_archive_path(), exceptions=False, timeout=TIMEOUT):
                 return True
         return False
 
     def download_enabled(self):
         return not self._disabled and self._download
 
     @utils.retried.on_exception((RequestException))
@@ -78,39 +75,44 @@
         if self._disabled:
             return True
         if not self._upload and not force:
             return True
         with self._cache.get_artifact(node) as artifact:
             url = self._get_url(node, artifact)
             archive = artifact.get_archive()
-            return node.tools.upload(archive, url, exceptions=True,
-                                     auth=self._get_auth(), timeout=TIMEOUT)
+            return node.tools.upload(
+                archive, url,
+                exceptions=False,
+                auth=self._get_auth(),
+                timeout=TIMEOUT)
         return False
 
     def upload_enabled(self):
         return not self._disabled and self._upload
 
     @utils.retried.on_exception((RequestException))
     def location(self, node):
         if self._disabled:
             return False
         with self._cache.get_artifact(node) as artifact:
+            from requests.api import head
+
             url = self._get_url(node, artifact)
             try:
-                response = requests.head(url, stream=True, timeout=TIMEOUT_HEAD)
+                response = head(url, stream=True, timeout=TIMEOUT_HEAD)
             except ConnectTimeout:
                 self._disabled = True
-                log.warning("[ARTIFACTORY] failed to establish server connection, disabled")
+                log.warning("[HTTP] failed to establish server connection, disabled")
                 return False
 
-            log.debug("[ARTIFACTORY] Head: {0}", url)
-            log.debug("[ARTIFACTORY] Response: {0}", response.status_code)
+            log.debug("[HTTP] Head: {0}", url)
+            log.debug("[HTTP] Response: {0}", response.status_code)
             return url if response.status_code == 200 else ''
         return False
 
 
 @cache.RegisterStorage
-class ArtifactoryFactory(cache.StorageProviderFactory):
+class HttpFactory(cache.StorageProviderFactory):
     @staticmethod
     def create(cache):
-        log.verbose("[Artifactory] Loaded")
-        return Artifactory(cache)
+        log.verbose("[Http] Loaded")
+        return Http(cache)
```

### Comparing `jolt-0.9.9/jolt/plugins/python.py` & `jolt-0.9.93/jolt/plugins/paths.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,99 +1,57 @@
-import sys
-
-from jolt import filesystem as fs
-from jolt.cache import ArtifactStringAttribute
 from jolt.cache import ArtifactAttributeSet
 from jolt.cache import ArtifactAttributeSetProvider
+from jolt.cache import ArtifactStringAttribute
+
+from jolt import filesystem as fs
 
 
-class PythonVariable(ArtifactStringAttribute):
-    def __init__(self, name):
-        super(PythonVariable, self).__init__(name)
+class PathVariable(ArtifactStringAttribute):
+    def __init__(self, artifact, name):
+        super(PathVariable, self).__init__(artifact, name)
+        self._old_value = None
 
     def apply(self, task, artifact):
         pass
 
     def unapply(self, task, artifact):
         pass
 
+    def __str__(self):
+        if self._value is None:
+            return ""
+        return fs.path.join(self._artifact.path, self._value)
 
-class PythonListVariable(PythonVariable):
-    def __init__(self, name):
-        super(PythonListVariable, self).__init__(name)
-
-    def append(self, value):
-        if self.get_value():
-            self.set_value(self.get_value() + ":" + value)
-        else:
-            self.set_value(value)
-
-    def items(self):
-        value = self.get_value()
-        return value.split(":") if value is not None else []
-
-
-class PythonPathVariable(PythonListVariable):
-    def __init__(self, name):
-        super(PythonPathVariable, self).__init__(name)
-
-    def append(self, value):
-        if self.get_value():
-            self.set_value(self.get_value() + ":" + value)
-        else:
-            self.set_value(value)
-
-    def items(self):
-        value = self.get_value()
-        return value.split(":") if value is not None else []
-
-    def apply(self, task, artifact):
-        paths = [fs.path.join(artifact.path, path) for path in self.items()]
-        sys.path.extend(paths)
-
-    def unapply(self, task, artifact):
-        paths = [fs.path.join(artifact.path, path) for path in self.items()]
-        for path in paths:
-            sys.path.remove(path)
-
-
-class PythonDictVariable(PythonListVariable):
-    def __init__(self, name):
-        super(PythonDictVariable, self).__init__(name)
 
-    def __setitem__(self, key, value=None):
-        item = "{0}={1}".format(key, value) if value is not None else key
-        self.append(item)
-
-
-class Python(ArtifactAttributeSet):
-    def __init__(self):
-        super(Python, self).__init__()
+class PathVariableSet(ArtifactAttributeSet):
+    def __init__(self, artifact):
+        super(PathVariableSet, self).__init__()
+        super(ArtifactAttributeSet, self).__setattr__("_artifact", artifact)
 
     def create(self, name):
-        if name.lower() == "path":
-            return PythonPathVariable("PATH")
-        assert False, "no such python attribute: {0}".format(name)
+        return PathVariable(self._artifact, name)
 
 
 @ArtifactAttributeSetProvider.Register
-class PythonProvider(ArtifactAttributeSetProvider):
+class PathVariableSetProvider(ArtifactAttributeSetProvider):
     def create(self, artifact):
-        setattr(artifact, "python", Python())
+        setattr(artifact, "paths", PathVariableSet(artifact))
 
     def parse(self, artifact, content):
-        if "python" not in content:
+        if "paths" not in content:
             return
-        for key, value in content["python"].items():
-            setattr(artifact.python, key, value)
+
+        for key, value in content["paths"].items():
+            getattr(artifact.paths, key).set_value(value, expand=False)
 
     def format(self, artifact, content):
-        if "python" not in content:
-            content["python"] = {}
-        for key, value in artifact.python.items():
-            content["python"][key] = str(value)
+        if "paths" not in content:
+            content["paths"] = {}
+
+        for key, value in artifact.paths.items():
+            content["paths"][key] = value.get_value()
 
     def apply(self, task, artifact):
-        artifact.python.apply(task, artifact)
+        artifact.paths.apply(task, artifact)
 
     def unapply(self, task, artifact):
-        artifact.python.unapply(task, artifact)
+        artifact.paths.unapply(task, artifact)
```

### Comparing `jolt-0.9.9/jolt/plugins/ninja.py` & `jolt-0.9.93/jolt/plugins/ninja.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,76 +1,318 @@
 import copy
 import ninja_syntax as ninja
-import platform
 import os
 import sys
 
-from jolt.tasks import Task
+from jolt.tasks import Task, attributes as task_attributes
 from jolt import config
-from jolt import influence
+from jolt.influence import attribute as influence_attribute
+from jolt.influence import DirectoryInfluence, FileInfluence
+from jolt.influence import HashInfluenceProvider, TaskAttributeInfluence
 from jolt import log
 from jolt import utils
 from jolt import filesystem as fs
 from jolt.error import raise_task_error_if
+from jolt.error import JoltError, JoltCommandError
 
 
-class Variable(object):
+class CompileError(JoltError):
+    def __init__(self):
+        super().__init__("Compilation failed")
+
+
+class attributes:
+    @staticmethod
+    def asflags(attrib, prepend=False):
+        """
+        Decorates a task with an alternative ``asflags`` attribute.
+
+        The new attribute will be concatenated with the regular
+        ``asflags`` attribute.
+
+        Args:
+            attrib (str): Name of alternative attribute.
+                Keywords are expanded.
+            prepend (boolean): Prepend the value of the alternative
+                attribute. Default: false (append).
+        """
+        return utils.concat_attributes("asflags", attrib, prepend)
+
+    @staticmethod
+    def cflags(attrib, prepend=False):
+        """
+        Decorates a task with an alternative ``cflags`` attribute.
+
+        The new attribute will be concatenated with the regular
+        ``asflags`` attribute.
+
+        Args:
+            attrib (str): Name of alternative attribute.
+                Keywords are expanded.
+            prepend (boolean): Prepend the value of the alternative
+                attribute. Default: false (append).
+        """
+        return utils.concat_attributes("cflags", attrib, prepend)
+
+    @staticmethod
+    def cxxflags(attrib, prepend=False):
+        """
+        Decorates a task with an alternative ``cxxflags`` attribute.
+
+        The new attribute will be concatenated with the regular
+        ``cxxflags`` attribute.
+
+        Args:
+            attrib (str): Name of alternative attribute.
+                Keywords are expanded.
+            prepend (boolean): Prepend the value of the alternative
+                attribute. Default: false (append).
+        """
+        return utils.concat_attributes("cxxflags", attrib, prepend)
+
+    @staticmethod
+    def incpaths(attrib, prepend=False):
+        """
+        Decorates a task with an alternative ``incpaths`` attribute.
+
+        The new attribute will be concatenated with the regular
+        ``incpaths`` attribute.
+
+        Args:
+            attrib (str): Name of alternative attribute.
+                Keywords are expanded.
+            prepend (boolean): Prepend the value of the alternative
+                attribute. Default: false (append).
+        """
+        return utils.concat_attributes("incpaths", attrib, prepend)
+
+    @staticmethod
+    def ldflags(attrib, prepend=False):
+        """
+        Decorates a task with an alternative ``ldflags`` attribute.
+
+        The new attribute will be concatenated with the regular
+        ``ldflags`` attribute.
+
+        Args:
+            attrib (str): Name of alternative attribute.
+                Keywords are expanded.
+            prepend (boolean): Prepend the value of the alternative
+                attribute. Default: false (append).
+        """
+        return utils.concat_attributes("ldflags", attrib, prepend)
+
+    @staticmethod
+    def libpaths(attrib, prepend=False):
+        """
+        Decorates a task with an alternative ``libpaths`` attribute.
+
+        The new attribute will be concatenated with the regular
+        ``libpaths`` attribute.
+
+        Args:
+            attrib (str): Name of alternative attribute.
+                Keywords are expanded.
+            prepend (boolean): Prepend the value of the alternative
+                attribute. Default: false (append).
+        """
+        return utils.concat_attributes("libpaths", attrib, prepend)
+
+    @staticmethod
+    def libraries(attrib, prepend=False):
+        """
+        Decorates a task with an alternative ``libraries`` attribute.
+
+        The new attribute will be concatenated with the regular
+        ``libraries`` attribute.
+
+        Args:
+            attrib (str): Name of alternative attribute.
+                Keywords are expanded.
+            prepend (boolean): Prepend the value of the alternative
+                attribute. Default: false (append).
+        """
+        return utils.concat_attributes("libraries", attrib, prepend)
+
+    @staticmethod
+    def macros(attrib, prepend=False):
+        """
+        Decorates a task with an alternative ``macros`` attribute.
+
+        The new attribute will be concatenated with the regular
+        ``macros`` attribute.
+
+        Args:
+            attrib (str): Name of alternative attribute.
+                Keywords are expanded.
+            prepend (boolean): Prepend the value of the alternative
+                attribute. Default: false (append).
+        """
+        return utils.concat_attributes("macros", attrib, prepend)
+
+    @staticmethod
+    def sources(attrib, prepend=False):
+        """
+        Decorates a task with an alternative ``sources`` attribute.
+
+        The new attribute will be concatenated with the regular
+        ``sources`` attribute.
+
+        Args:
+            attrib (str): Name of alternative attribute.
+                Keywords are expanded.
+            prepend (boolean): Prepend the value of the alternative
+                attribute. Default: false (append).
+        """
+        return utils.concat_attributes("sources", attrib, prepend)
+
+
+class influence:
+    @staticmethod
+    def incpaths(type=DirectoryInfluence):
+        return influence_attribute("_incpaths", type=type)
+
+    @staticmethod
+    def libpaths(type=DirectoryInfluence):
+        return influence_attribute("_libpaths", type=type)
+
+    @staticmethod
+    def sources(type=FileInfluence):
+        return influence_attribute("_sources", type=type)
+
+
+class Variable(HashInfluenceProvider):
     def __init__(self, value=None):
         self._value = value
 
+    @staticmethod
+    def __get_variables__(obj):
+        variables = {}
+        for mro in reversed(obj.__class__.__mro__):
+            for key, variable in getattr(mro, "__variable_list", {}).items():
+                attr = getattr(obj.__class__, key)
+                if isinstance(attr, Variable):
+                    variables[key] = attr
+        return variables
+
+    def __set_name__(self, owner, name):
+        self.name = name
+        if "__variable_list" not in owner.__dict__:
+            setattr(owner, "__variable_list", {})
+        getattr(owner, "__variable_list")[name] = self
+
     def create(self, project, writer, deps, tools):
         writer.variable(self.name, self._value)
 
+    @utils.cached.instance
+    def get_influence(self, task):
+        return "V: value={}".format(self._value)
+
+
+class HostVariable(Variable):
+    def __init__(self, value=None):
+        self._value = value
+
+    def create(self, project, writer, deps, tools):
+        writer.variable(self.name, self._value[os.name])
+
+    @utils.cached.instance
+    def get_influence(self, task):
+        return "HV: value={}".format(self._value)
+
 
 class EnvironmentVariable(Variable):
     def __init__(self, name=None, default=None, envname=None, prefix=None):
         self.name = name
         self._default = default or ''
         self._envname = envname
         self._prefix = prefix or ""
 
     def create(self, project, writer, deps, tools):
         envname = self._envname or self.name
         self.value = tools.getenv(envname.upper(), self._default)
         writer.variable(self.name, self._prefix + self.value)
 
+    @utils.cached.instance
+    def get_influence(self, task):
+        return "EV: default={},envname={},prefix={}".format(
+            self._default, self._envname, self._prefix)
 
-class ToolEnvironmentVariable(EnvironmentVariable):
+
+class ToolVariable(Variable):
     def create(self, project, writer, deps, tools):
-        super(ToolEnvironmentVariable, self).create(project, writer, deps, tools)
-        if not self.value:
-            return
-        value = self.value.split()[0]
-        executable_path = tools.which(value)
+        super().create(project, writer, deps, tools)
+        executable = self._value.split()[0]
+        executable_path = tools.which(executable)
         if executable_path:
             writer.variable(self.name + "_path", executable_path)
 
+    @utils.cached.instance
+    def get_influence(self, task):
+        return "TV"
+
+
+class ToolEnvironmentVariable(Variable):
+    def __init__(self, name=None, default=None, envname=None, prefix=None, abspath=False):
+        self.name = name
+        self._default = default or ''
+        self._envname = envname
+        self._prefix = prefix or ""
+        self._abspath = abspath
+
+    def create(self, project, writer, deps, tools):
+        envname = self._envname or self.name
+        value = tools.getenv(envname.upper(), self._default)
+        executable_and_args = value.split(maxsplit=1) or [""]
+        executable = executable_and_args[0]
+        executable_path = tools.which(executable)
+
+        if executable_path:
+            writer.variable(self.name + "_path", executable_path)
+            if self._abspath:
+                executable_and_args[0] = utils.quote_path(executable_path)
+
+        writer.variable(self.name, self._prefix + " ".join(executable_and_args))
+
+    @utils.cached.instance
+    def get_influence(self, task):
+        return "ToolEnvironment: default={},envname={},prefix={},abspath={}".format(
+            self._default, self._envname, self._prefix, self._abspath)
+
 
 class ProjectVariable(Variable):
     def __init__(self, name=None, default=None, attrib=None):
         self.name = name
         self._default = default or ''
         self._attrib = attrib
 
     def create(self, project, writer, deps, tools):
         value = getattr(project, self._attrib or self.name, "")
         if type(value) == list:
             value = " ".join(value)
         writer.variable(self.name, str(value))
 
+    @utils.cached.instance
+    def get_influence(self, task):
+        return "PV: default={},attrib={}".format(self._default, self._attrib)
+
 
 class SharedLibraryVariable(Variable):
     def __init__(self, name=None, default=None):
         self.name = name
         self._default = default
 
     def create(self, project, writer, deps, tools):
         value = self._default if isinstance(project, CXXLibrary) and project.shared else ""
         writer.variable(self.name, str(value))
 
+    @utils.cached.instance
+    def get_influence(self, task):
+        return "SLV: default={}".format(self._default)
+
 
 class GNUPCHVariables(Variable):
     pch_ext = ".pch"
     gch_ext = ".gch"
 
     def __init__(self):
         pass
@@ -79,26 +321,30 @@
         pch = [src for src in project.sources if src.endswith(self.pch_ext)]
 
         raise_task_error_if(
             len(pch) > 1, project,
             "multiple precompiled headers found, only one is allowed")
 
         if len(pch) <= 0:
-            writer.variable("pch_out", ".")
+            writer.variable("pch_out", "$binary.dir/")
             return
 
         project._pch = fs.path.basename(pch[0])
-        project._pch_out = project._pch + self.gch_ext
+        project._pch_out = "$binary.dir/" + project._pch + self.gch_ext
 
         writer.variable("pch", project._pch)
-        writer.variable("pch_flags", "-include $pch")
+        writer.variable("pch_flags", "")
         writer.variable("pch_out", project._pch_out)
 
+    @utils.cached.instance
+    def get_influence(self, task):
+        return "PCHV"
 
-class Rule(object):
+
+class Rule(HashInfluenceProvider):
     """ A source transformation rule.
 
     Rules are used to transform files from one type to another.
     An example is the rule that compiles a C/C++ file to an object file.
     Ninja tasks can be extended with additional rules beyond those
     already builtin and the builtin rules may also be overridden.
 
@@ -122,15 +368,15 @@
     a corresponding moc source file, ``myqtproject_moc.cpp``.
     The moc source file will then automatically be fed to the builtin
     compiler rule from which the output is an object file,
     ``myqtproject_moc.o``.
 
     """
 
-    def __init__(self, command=None, infiles=None, outfiles=None, depfile=None, deps=None, variables=None, implicit=None, order_only=None):
+    def __init__(self, command=None, infiles=None, outfiles=None, depfile=None, deps=None, variables=None, implicit=None, order_only=None, aggregate=False, phony=None):
         """
         Creates a new rule.
 
         Args:
             command (str, optional):
                 The command that will be execute by the rule.
                 It can use any of the `variables` created below.
@@ -156,322 +402,615 @@
 
                 Example:
 
                   .. code-block:: python
 
                     Rule(command="echo $extension", variables={"extension": "{in_ext}"}, ...)
 
+            aggregate (boolean, optional):
+                When this attribute is set, the Rule will aggregate all input
+                files and transform them with a single command. This is
+                useful, for example, when creating linking and archiving rules.
+                In aggregating rules the ``$in`` Ninja variable expands to all
+                matched input files, while the ``outfiles`` / ``$out`` variable
+                is expanded using the first input in the set, if the ``in_*``
+                keywords are used at all.
+
+                By default, a rule is applied once for each matched input file
+                for improved parallelism.
+
+                Example:
+
+                  In this example, the rule concatenates all header files into
+                  a single precompiled header.
+
+                  .. code-block:: python
+
+                    pch = Rule(
+                       command="cat $in > $out",
+                       infiles=["*.h"],
+                       outfiles=["{outdir}/all.pch"],
+                       aggregate=True)
+
+             phony (boolean, optional):
+                 Emit a phony build target depending on all files generated by
+                 this rule. The phony build target becomes an implicit dependency
+                 in downstream rules that pick up the output from this rule.
+
+                 An example use-case is the compilation of protobuffers into C++
+                 headers and source files. The C++ header files must be available
+                 before they can be included from other static C++ source files.
+                 With the phony target enabled, all protobuffers are compiled
+                 before any C++ file is compiled.
         """
         self.command = command
         self.variables = variables or {}
         self.depfile = depfile
         self.deps = deps
         self.infiles = infiles or []
         self.outfiles = utils.as_list(outfiles or [])
-        self.implicit = implicit
-        self.order_only = order_only
+        self.implicit = implicit or []
+        self.order_only = order_only or []
+        self.aggregate = aggregate
+        self.phony = phony
+
+    @staticmethod
+    def __get_rules__(obj):
+        rules = {}
+        for mro in reversed(obj.__class__.__mro__):
+            for key, rule in getattr(mro, "__rule_list", {}).items():
+                attr = getattr(obj.__class__, key)
+                if isinstance(attr, Rule):
+                    rules[key] = attr
+        return rules
+
+    def __set_name__(self, owner, name):
+        self.name = name
+        if self.phony:
+            self.phony = name
+        if "__rule_list" not in owner.__dict__:
+            setattr(owner, "__rule_list", {})
+        getattr(owner, "__rule_list")[name] = self
 
     def _out(self, project, infile):
+        in_dirname_outdir = None
         in_dirname, in_basename = fs.path.split(infile)
         in_base, in_ext = fs.path.splitext(in_basename)
 
-        if in_dirname:
+        if in_dirname and fs.path.isabs(in_dirname):
+            in_dirname_outdir = fs.path.relpath(in_dirname, project.outdir)
             in_dirname = fs.path.relpath(in_dirname, project.joltdir)
 
         result_files = []
         for outfile in self.outfiles:
             outfile = project.tools.expand(
                 outfile,
                 in_path=in_dirname,
+                in_path_outdir=in_dirname_outdir,
                 in_base=in_base,
                 in_ext=in_ext)
 
             if outfile.startswith(project.joltdir) and not outfile.startswith(project.outdir):
-                outfile = outfile[len(project.joltdir)+1:]
+                outfile = outfile[len(project.joltdir) + 1:]
                 outfile = fs.path.join(project.outdir, outfile)
 
-            result_files.append(outfile)
+            result_files.append(outfile.replace("..", "__"))
 
         result_vars = {}
         for key, val in self.variables.items():
             result_vars[key] = project.tools.expand(
                 val,
                 in_path=in_dirname,
+                in_path_outdir=in_dirname_outdir,
                 in_base=in_base,
                 in_ext=in_ext)
 
         return result_files, result_vars
 
     def create(self, project, writer, deps, tools):
         if self.command is not None:
-            writer.rule(self.name, tools.expand(self.command), depfile=self.depfile, deps=self.deps, description="$desc")
+            command = utils.as_list(self.command)
+            command = ["cmd /c " + c for c in command] if os.name == "nt" else command
+            command = " && ".join(command)
+            writer.rule(self.name, tools.expand(command), depfile=self.depfile, deps=self.deps, description="$desc")
             writer.newline()
 
-    def build(self, project, writer, infiles, implicit=None):
+    def output(self, project, infiles):
+        outfiles, _ = self._out(project, utils.as_list(infiles)[0])
+        return outfiles
+
+    def build(self, project, writer, infiles, implicit=None, order_only=None):
         result = []
-        for infile in utils.as_list(infiles):
-            infile_rel = fs.path.relpath(infile, project.outdir)
-            outfiles, variables = self._out(project, infile)
+        infiles = utils.as_list(infiles)
+        infiles_rel = [fs.path.relpath(infile, project.outdir) for infile in infiles]
+        implicit = (self.implicit or []) + (implicit or [])
+        order_only = (self.order_only or []) + (order_only or [])
+
+        if self.aggregate:
+            outfiles, variables = self._out(project, infiles[0])
             outfiles_rel = [fs.path.relpath(outfile, project.outdir) for outfile in outfiles]
-            implicit = (self.implicit or []) + (implicit or [])
-            writer.build(outfiles_rel, self.name, infile_rel, variables=variables, implicit=implicit, order_only=self.order_only)
+            writer.build(outfiles_rel, self.name, infiles_rel, variables=variables, implicit=implicit, order_only=self.order_only + order_only)
             result.extend(outfiles)
+        else:
+            for infile, infile_rel in zip(infiles, infiles_rel):
+                outfiles, variables = self._out(project, infile)
+                outfiles_rel = [fs.path.relpath(outfile, project.outdir) for outfile in outfiles]
+                writer.build(outfiles_rel, self.name, infile_rel, variables=variables, implicit=implicit, order_only=order_only)
+                result.extend(outfiles)
+        if self.phony:
+            writer.build(self.phony, "phony", outfiles_rel)
         return result
 
+    @utils.cached.instance
+    def get_influence(self, task):
+        return "R: cmd={},var={},in={},out={},impl={},order={},dep={}.{}".format(
+            self.command, utils.as_stable_string_list(self.variables),
+            self.infiles, self.outfiles, self.implicit,
+            self.order_only, self.deps, self.depfile)
+
+
+class ProtobufCompiler(Rule):
+    def __init__(
+            self,
+            command="$protoc_path -I$in_path_outdir $incpaths $protoflags $task_protoflags --dependency_out=$out_depfile --${{generator}}_out=$outdir_proto $in",
+            infiles=[".proto"],
+            deps="gcc",
+            depfile="$out_depfile",
+            generator="cpp",
+            implicit=["$protoc_path"],
+            outfiles=[
+                "{outdir}/{binary}.dir/{in_base}.pb.h",
+                "{outdir}/{binary}.dir/{in_base}.pb.cc",
+            ],
+            phony=True,
+            variables=None,
+            **kwargs):
+        variables_final = {
+            "desc": "[PROTOC] {in_base}{in_ext}",
+            "out_depfile": "{binary}.dir/{in_base}.pb.d",
+            "outdir_proto": os.path.dirname(outfiles[0]),
+            "in_path_outdir": "{in_path_outdir}",
+        }
+        variables_final.update(variables or {})
+        super().__init__(
+            command=command,
+            infiles=infiles,
+            deps=deps,
+            depfile=depfile,
+            implicit=implicit,
+            outfiles=outfiles,
+            phony=phony,
+            variables=variables_final,
+            **kwargs)
+        self.generator = generator
+
+    def _out(self, project, infile):
+        outfiles, variables = super()._out(project, infile)
+        variables["generator"] = project.tools.expand(self.generator)
+        return outfiles, variables
+
+    @utils.cached.instance
+    def get_influence(self, task):
+        return "ProtoC" + super().get_influence(task)
+
+
+class GRPCProtobufCompiler(ProtobufCompiler):
+    def __init__(
+            self,
+            command=[
+                "$protoc_path -I$in_path_outdir $incpaths $protoflags $task_protoflags --dependency_out=$out_depfile --${{generator}}_out=$outdir_proto $in",
+                "$protoc_path -I$in_path_outdir $incpaths $protoflags $task_protoflags --dependency_out=$out_depfile_grpc --grpc_out=$outdir_proto --plugin=protoc-gen-grpc=`which grpc_${{generator}}_plugin` $in",
+            ],
+            depfile=["$out_depfile", "$out_depfile_grpc"],
+            outfiles=[
+                "{outdir}/{binary}.dir/{in_base}.pb.h",
+                "{outdir}/{binary}.dir/{in_base}.pb.cc",
+                "{outdir}/{binary}.dir/{in_base}.grpc.pb.h",
+                "{outdir}/{binary}.dir/{in_base}.grpc.pb.cc",
+            ],
+            variables=None,
+            **kwargs):
+        variables_final = {
+            "out_depfile": "{binary}.dir/{in_base}.pb.d",
+            "out_depfile_grpc": "{binary}.dir/{in_base}.grpc.pb.d",
+        }
+        variables_final.update(variables or {})
+        super().__init__(command=command, depfile=depfile, outfiles=outfiles, variables=variables_final, **kwargs)
+
+
+class FlatbufferCompiler(Rule):
+    def __init__(
+            self,
+            command=[
+                "$flatc_path --${{generator}} $fbflags $task_fbflags $fbincpaths -o $outdir_fb $in",
+                "$flatc_path -M --${{generator}} $fbflags $task_fbflags $fbincpaths -o $outdir_fb $in > $out.d",
+            ],
+            infiles=[".fbs"],
+            deps="gcc",
+            depfile="$out.d",
+            generator="cpp",
+            implicit=["$flatc_path"],
+            outfiles=["{outdir}/{binary}.dir/{in_base}_generated.h"],
+            phony=True,
+            variables=None,
+            **kwargs):
+        variables_final = {
+            "desc": "[FLATC] {in_base}{in_ext}",
+            "outdir_fb": os.path.dirname(outfiles[0]),
+        }
+        variables_final.update(variables or {})
+        super().__init__(
+            command=command,
+            infiles=infiles,
+            deps=deps,
+            depfile=depfile,
+            implicit=implicit,
+            outfiles=outfiles,
+            phony=phony,
+            variables=variables_final,
+            **kwargs)
+        self.generator = generator
+
+    def _out(self, project, infile):
+        outfiles, variables = super()._out(project, infile)
+        variables["generator"] = project.tools.expand(self.generator)
+        return outfiles, variables
+
+    @utils.cached.instance
+    def get_influence(self, task):
+        return "FlatC" + super().get_influence(task)
+
 
 class Skip(Rule):
     def __init__(self, *args, **kwargs):
         super(Skip, self).__init__(*args, **kwargs)
         self.command = None
 
     def create(self, project, writer, deps, tools):
         pass
 
-    def build(self, project, writer, infiles):
+    def build(self, project, writer, infiles, implicit=None, order_only=None):
         return None
 
+    @utils.cached.instance
+    def get_influence(self, task):
+        return "S" + super().get_influence(task)
 
-class Objects(Rule):
-    def __init__(self, *args, **kwargs):
-        super(Objects, self).__init__(*args, **kwargs)
-        self.command = None
+
+@task_attributes.system
+class MakeDirectory(Rule):
+    command_linux = "mkdir -p $out"
+    command_windows = "if not exist $out mkdir $out"
+
+    def __init__(self, name):
+        super(MakeDirectory, self).__init__(
+            command=getattr(self, "command_" + self.system))
+        self.dirname = name
 
     def create(self, project, writer, deps, tools):
-        pass
+        super().create(project, writer, deps, tools)
+        writer.build(fs.path.normpath(self.dirname), self.name, [], variables={"desc": "[MKDIR] " + self.dirname})
 
-    def build(self, project, writer, infiles):
-        project.objects.extend(utils.as_list(infiles))
+    def build(self, project, writer, infiles, implicit=None, order_only=None):
         return None
 
+    @utils.cached.instance
+    def get_influence(self, task):
+        return "MD" + super().get_influence(task)
+
 
 class GNUCompiler(Rule):
     def __init__(self, *args, **kwargs):
         super(GNUCompiler, self).__init__(*args, **kwargs)
 
-    def build(self, project, writer, infiles, implicit=None):
+    def create(self, project, writer, deps, tools):
+        super().create(project, writer, deps, tools)
+
+    def build(self, project, writer, infiles, implicit=None, order_only=None):
         implicit = implicit or []
         if GNUPCHVariables.pch_ext not in self.infiles and project._pch_out is not None:
             implicit.append(project._pch_out)
-        return super(GNUCompiler, self).build(project, writer, infiles, implicit)
+        return super().build(project, writer, infiles, implicit, order_only)
+
+    @utils.cached.instance
+    def get_influence(self, task):
+        return "GC" + super().get_influence(task)
 
 
 class FileListWriter(Rule):
-    def __init__(self, name):
+    def __init__(self, name, posix=False):
         self.name = name
+        self.posix = posix
 
     def _write(self, flp, flhp, data, digest):
         with open(flp, "w") as f:
             f.write(data)
         with open(flhp, "w") as f:
             f.write(digest)
 
     def _identical(self, flp, flhp, data, digest):
         if not fs.path.exists(flp) or not fs.path.exists(flhp):
             return False
 
         try:
             with open(flhp, "r") as f:
                 disk_digest = f.read()
-        except:
+        except Exception:
             return False
 
         return digest == disk_digest
 
-    def _data(self, files):
+    def _data(self, project, files):
         data = "\n".join(files)
         return data, utils.sha1(data)
 
-    def build(self, project, writer, infiles):
+    def build(self, project, writer, infiles, implicit=None, order_only=None):
+        infiles = [fs.as_posix(infile) for infile in infiles] if self.posix else infiles
         file_list_path = fs.path.join(project.outdir, "{0}.list".format(self.name))
         file_list_hash_path = fs.path.join(project.outdir, "{0}.hash".format(self.name))
-        data, digest = self._data(infiles)
+        data, digest = self._data(project, infiles)
         if not self._identical(file_list_path, file_list_hash_path, data, digest):
             self._write(file_list_path, file_list_hash_path, data, digest)
-        project.depimports.append(file_list_path)
+        writer.depimports.append(file_list_path)
+
+    @utils.cached.instance
+    def get_influence(self, task):
+        return "FL" + super().get_influence(task)
+
+
+class GNUMRIWriter(FileListWriter):
+    """
+    Creates an AR instruction script.
+
+    All input object files and libraries are be added to the target libary.
+
+    """
+
+    def __init__(self, name, outfiles):
+        super().__init__(name)
+        self.outfiles = outfiles
+
+    def _data(self, project, infiles):
+        data = "create {}\n".format(self.outfiles[0])
+        for infile in infiles:
+            _, ext = fs.path.splitext(infile)
+            if ext == ".a":
+                data += "addlib {}\n".format(infile)
+            else:
+                data += "addmod {}\n".format(infile)
+        data += "save\nend\n"
+        return data, utils.sha1(data)
+
+    @utils.cached.instance
+    def get_influence(self, task):
+        return "MRI" + super().get_influence(task)
 
 
 class GNULinker(Rule):
     def __init__(self, *args, **kwargs):
-        super(GNULinker, self).__init__(*args, **kwargs)
-
-    def build(self, project, writer, infiles):
-        file_list = FileListWriter("objects")
-        file_list.build(project, writer, infiles)
+        super(GNULinker, self).__init__(*args, aggregate=True, **kwargs)
 
-        infiles_rel = [fs.path.relpath(infile, project.outdir) for infile in infiles]
-        outfiles, variables = self._out(project, project.binary)
-        outfiles_rel = [fs.path.relpath(outfile, project.outdir) for outfile in outfiles]
-        writer.build(outfiles_rel, self.name, infiles_rel, implicit=project.depimports, variables=variables)
-        return outfiles
+    def build(self, project, writer, infiles, implicit=None, order_only=None):
+        writer._objects = infiles
+        project._binaries, _ = self._out(project, project.binary)
+        file_list = FileListWriter("objects", posix=True)
+        file_list.build(project, writer, infiles, implicit=None)
+        return super().build(project, writer, infiles, implicit=writer.depimports, order_only=order_only)
+
+    @utils.cached.instance
+    def get_influence(self, task):
+        return "L" + super().get_influence(task)
 
 
 class GNUArchiver(Rule):
     def __init__(self, *args, **kwargs):
-        super(GNUArchiver, self).__init__(*args, **kwargs)
+        super(GNUArchiver, self).__init__(*args, aggregate=True, **kwargs)
 
-    def build(self, project, writer, infiles):
-        file_list = FileListWriter("objects")
+    def build(self, project, writer, infiles, implicit=None, order_only=None):
+        writer._objects = infiles
+        project._binaries, _ = self._out(project, project.binary)
+        file_list = GNUMRIWriter("objects", project._binaries)
         file_list.build(project, writer, infiles)
+        super().build(project, writer, infiles, implicit=writer.depimports, order_only=order_only)
 
-        infiles_rel = [fs.path.relpath(infile, project.outdir) for infile in infiles]
-        outfiles, variables = self._out(project, project.binary)
-        outfiles_rel = [fs.path.relpath(outfile, project.outdir) for outfile in outfiles]
-        writer.build(outfiles_rel, self.name, infiles_rel, implicit=project.depimports, variables=variables)
-        return outfiles
+    def get_influence(self, task):
+        return "GA" + super().get_influence(task)
 
 
 class GNUDepImporter(Rule):
     def __init__(self, prefix=None, suffix=None):
+        super().__init__()
         self.prefix = prefix
         self.suffix = suffix
         self.infiles = []
         self.command = None
 
     def _build_archives(self, project, writer, deps):
         archives = []
         for name, artifact in deps.items():
-             for lib in artifact.cxxinfo.libraries.items():
-                 name = "{0}{1}{2}".format(self.prefix, lib, self.suffix)
-                 for path in artifact.cxxinfo.libpaths.items():
-                     archive = fs.path.join(artifact.path, path, name)
-                     if fs.path.exists(archive):
-                         archives.append(archive)
+            if artifact.cxxinfo.libpaths.items():
+                sandbox = project.tools.sandbox(artifact, project.incremental)
+            for lib in artifact.cxxinfo.libraries.items():
+                name = "{0}{1}{2}".format(self.prefix, lib, self.suffix)
+                for path in artifact.cxxinfo.libpaths.items():
+                    archive = fs.path.join(sandbox, path, name)
+                    if fs.path.exists(archive):
+                        archives.append(archive)
         return archives
 
-    def build(self, project, writer, deps):
+    def build(self, project, writer, deps, implicit=None, order_only=None):
         imports = []
         if isinstance(project, CXXExecutable):
             imports += self._build_archives(project, writer, deps)
+        if isinstance(project, CXXLibrary):
+            imports += self._build_archives(project, writer, deps)
+            if not project.shared and project.selfsustained:
+                writer.sources.extend(imports)
         return imports
 
+    def get_influence(self, task):
+        return "GD" + super().get_influence(task)
+
 
 class Toolchain(object):
     def __init__(self):
-        self._rule_map = self.build_rule_map(self)
-        self.build_variables(self)
+        self._rules_by_ext = self.build_rules_and_vars(self)
 
     @staticmethod
-    def build_rule_map(cls):
+    def build_rules_and_vars(obj):
         rule_map = {}
-        for name, rule in Toolchain.all_rules(cls):
+        rules, vars = Toolchain.all_rules_and_vars(obj)
+        for name, rule in rules.items():
             rule.name = name
             for ext in rule.infiles:
                 rule_map[ext] = rule
-        return rule_map
-
-    @staticmethod
-    def build_variables(cls):
-        for name, var in Toolchain.all_variables(cls):
+        for name, var in vars.items():
             var.name = name
-
-    @staticmethod
-    def all_rules(cls):
-        return [(key, getattr(cls, key)) for key in dir(cls)
-                if isinstance(utils.getattr_safe(cls, key), Rule)]
+        return rule_map
 
     def find_rule(self, ext):
-        return self._rule_map.get(ext)
+        return self._rules_by_ext.get(ext)
 
     @staticmethod
-    def all_variables(cls):
-        return [(key, getattr(cls, key)) for key in dir(cls)
-                if isinstance(utils.getattr_safe(cls, key), Variable)]
+    def all_rules_and_vars(obj):
+        return Rule.__get_rules__(obj), Variable.__get_variables__(obj)
 
     def __str__(self):
         return self.__class__.__name__
 
 
 class Macros(Variable):
-    def __init__(self, prefix=None):
+    def __init__(self, prefix=None, attrib="macros", imported=True):
         self.prefix = prefix or ''
+        self.attrib = attrib
+        self.imported = imported
 
     def create(self, project, writer, deps, tools):
-        macros = [tools.expand(macro) for macro in project.macros]
-        for name, artifact in deps.items():
-            macros += artifact.cxxinfo.macros.items()
+        macros = []
+        if self.attrib:
+            macros = [tools.expand(macro) for macro in getattr(project, self.attrib)]
+        if self.imported:
+            for _, artifact in deps.items():
+                macros += artifact.cxxinfo.macros.items()
         macros = ["{0}{1}".format(self.prefix, macro) for macro in macros]
         writer.variable(self.name, " ".join(macros))
 
+    @utils.cached.instance
+    def get_influence(self, task):
+        return "Macros: prefix={}".format(self.prefix)
+
 
 class ImportedFlags(Variable):
     def create(self, project, writer, deps, tools):
         asflags = []
         cflags = []
         cxxflags = []
         ldflags = []
-        for name, artifact in deps.items():
+        for _, artifact in deps.items():
             asflags += artifact.cxxinfo.asflags.items()
             cflags += artifact.cxxinfo.cflags.items()
             cxxflags += artifact.cxxinfo.cxxflags.items()
             ldflags += artifact.cxxinfo.ldflags.items()
         writer.variable("imported_asflags", " ".join(asflags))
         writer.variable("imported_cflags", " ".join(cflags))
         writer.variable("imported_cxxflags", " ".join(cxxflags))
         writer.variable("imported_ldflags", " ".join(ldflags))
 
 
 class IncludePaths(Variable):
-    def __init__(self, prefix=None):
+    def __init__(self, prefix=None, attrib="incpaths", imported=True, outdir=True):
         self.prefix = prefix or ''
+        self.outdir = outdir
+        self.attrib = attrib
+        self.imported = imported
 
     def create(self, project, writer, deps, tools):
         def expand(path):
             if path[0] in ['=', fs.sep]:
                 return tools.expand(path)
             if path[0] in ['-']:
-                return tools.expand(path[1:])
+                path = tools.expand_path(path[1:])
             return tools.expand_relpath(path, project.outdir)
 
         def expand_artifact(sandbox, path):
             if path[0] in ['=', fs.sep]:
                 return path
             if path[0] in ['-']:
-                return path[1:]
+                path = fs.path.join(project.joltdir, path[1:])
             return tools.expand_relpath(fs.path.join(sandbox, path), project.outdir)
 
-        incpaths = [expand(path) for path in project.incpaths] + ["."]
-        for name, artifact in deps.items():
-            incs = [path for path in artifact.cxxinfo.incpaths.items()]
-            if incs:
-                sandbox = tools.sandbox(artifact, project.incremental)
-                incpaths += [expand_artifact(sandbox, path) for path in incs]
+        incpaths = []
+        if self.outdir:
+            incpaths += ["$binary.dir"]
+        if self.attrib:
+            incpaths += [expand(path) for path in getattr(project, self.attrib)]
+        if self.imported:
+            for _, artifact in deps.items():
+                incs = artifact.cxxinfo.incpaths.items()
+                if incs:
+                    sandbox = tools.sandbox(artifact, project.incremental)
+                    incpaths += [expand_artifact(sandbox, path) for path in incs]
 
         incpaths = ["{0}{1}".format(self.prefix, path) for path in incpaths]
         writer.variable(self.name, " ".join(incpaths))
 
+    @utils.cached.instance
+    def get_influence(self, task):
+        return "IncludePaths: prefix={}".format(self.prefix)
+
 
 class LibraryPaths(Variable):
-    def __init__(self, prefix=None):
+    def __init__(self, prefix=None, attrib="libpaths", imported=True):
         self.prefix = prefix or ''
+        self.attrib = attrib
+        self.imported = imported
 
     def create(self, project, writer, deps, tools):
         if isinstance(project, CXXLibrary) and not project.shared:
             return
-        libpaths = [tools.expand_relpath(path, project.outdir) for path in project.libpaths]
-        for name, artifact in deps.items():
-            libpaths += [fs.path.join(artifact.path, path)
-                         for path in artifact.cxxinfo.libpaths.items()]
+        libpaths = []
+        if self.attrib:
+            libpaths = [tools.expand_relpath(path, project.outdir) for path in getattr(project, self.attrib)]
+        if self.imported:
+            for _, artifact in deps.items():
+                libs = artifact.cxxinfo.libpaths.items()
+                if libs:
+                    sandbox = tools.sandbox(artifact, project.incremental)
+                    libpaths += [fs.path.join(sandbox, path) for path in libs]
         libpaths = ["{0}{1}".format(self.prefix, path) for path in libpaths]
         writer.variable(self.name, " ".join(libpaths))
 
+    @utils.cached.instance
+    def get_influence(self, task):
+        return "LibraryPaths: prefix={}".format(self.prefix)
+
 
 class Libraries(Variable):
-    def __init__(self, prefix=None, suffix=None):
+    def __init__(self, prefix=None, suffix=None, attrib="libraries", imported=True):
         self.prefix = prefix or ''
         self.suffix = suffix or ''
+        self.attrib = attrib
+        self.imported = imported
 
     def create(self, project, writer, deps, tools):
         if isinstance(project, CXXLibrary) and not project.shared:
             return
-        libraries = [tools.expand(lib) for lib in project._libraries()]
-        for name, artifact in deps.items():
-            libraries += artifact.cxxinfo.libraries.items()
+        libraries = []
+        if self.attrib:
+            libraries = [tools.expand(lib) for lib in getattr(project, self.attrib)]
+        if self.imported:
+            for _, artifact in deps.items():
+                libraries += artifact.cxxinfo.libraries.items()
         libraries = ["{0}{1}{2}".format(self.prefix, path, self.suffix) for path in libraries]
         writer.variable(self.name, " ".join(libraries))
 
+    @utils.cached.instance
+    def get_influence(self, task):
+        return "Libraries: prefix={},suffix={}".format(self.prefix, self.suffix)
+
 
 class GNUFlags(object):
     @staticmethod
     def set(flags, flag, fixup=None):
         flags = flags.split(" ")
         fixup = fixup or []
         flags_out = [flag_out for flag_out in flags if flag_out not in fixup]
@@ -490,209 +1029,266 @@
     @staticmethod
     def set_debug(flags):
         return GNUOptFlags.set(flags, GNUOptFlags.DEBUG)
 
 
 class GNUToolchain(Toolchain):
     hh = Skip(infiles=[".h", ".hh", ".hpp", ".hxx", GNUPCHVariables.gch_ext])
-    obj = Objects(infiles=[".o", ".obj", ".a"])
+    bin = Skip(infiles=[".dll", ".elf", ".exe", ".out", ".so"])
 
     joltdir = ProjectVariable()
     outdir = ProjectVariable()
     binary = ProjectVariable()
 
-    ar = ToolEnvironmentVariable(default="ar")
-    cc = ToolEnvironmentVariable(default="gcc")
-    cxx = ToolEnvironmentVariable(default="g++")
-    ld = ToolEnvironmentVariable(default="g++", envname="CXX")
-    objcopy = ToolEnvironmentVariable(default="objcopy")
-
+    ar = ToolEnvironmentVariable(default="ar", abspath=True)
+    cc = ToolEnvironmentVariable(default="gcc", abspath=True)
+    cxx = ToolEnvironmentVariable(default="g++", abspath=True)
+    ld = ToolEnvironmentVariable(default="g++", envname="CXX", abspath=True)
+    objcopy = ToolEnvironmentVariable(default="objcopy", abspath=True)
+    ranlib = ToolEnvironmentVariable(default="ranlib", abspath=True)
     ccwrap = EnvironmentVariable(default="")
     cxxwrap = EnvironmentVariable(default="")
+    flatc = ToolEnvironmentVariable(default="flatc", envname="FLATC", abspath=True)
+    protoc = ToolEnvironmentVariable(default="protoc", envname="PROTOC", abspath=True)
 
     asflags = EnvironmentVariable(default="")
     cflags = EnvironmentVariable(default="")
     cxxflags = EnvironmentVariable(default="")
+    fbflags = EnvironmentVariable(default="")
     ldflags = EnvironmentVariable(default="")
+    protoflags = EnvironmentVariable(default="")
 
     shared_flags = SharedLibraryVariable(default="-fPIC")
     pch_flags = GNUPCHVariables()
 
     extra_asflags = ProjectVariable(attrib="asflags")
     extra_cflags = ProjectVariable(attrib="cflags")
     extra_cxxflags = ProjectVariable(attrib="cxxflags")
     extra_ldflags = ProjectVariable(attrib="ldflags")
 
+    task_fbflags = ProjectVariable(attrib="fbflags")
+    task_protoflags = ProjectVariable(attrib="protoflags")
+
+    fbincpaths = IncludePaths("-I ")
     flags = ImportedFlags()
-    macros = Macros(prefix="-D")
     incpaths = IncludePaths(prefix="-I")
+    macros = Macros(prefix="-D")
     libpaths = LibraryPaths(prefix="-L")
     libraries = Libraries(prefix="-l")
 
+    mkdir_debug = MakeDirectory(name=".debug")
+
     compile_pch = GNUCompiler(
         command="$cxxwrap $cxx -x c++-header $cxxflags $shared_flags $imported_cxxflags $extra_cxxflags $macros $incpaths -MMD -MF $out.d -c $in -o $out",
         deps="gcc",
         depfile="$out.d",
         infiles=[GNUPCHVariables.pch_ext],
-        outfiles=["{outdir}/{in_base}{in_ext}" + GNUPCHVariables.gch_ext],
+        outfiles=["{outdir}/{binary}.dir/{in_base}{in_ext}" + GNUPCHVariables.gch_ext],
         variables={"desc": "[PCH] {in_base}{in_ext}"})
 
     compile_c = GNUCompiler(
         command="$ccwrap $cc -x c $pch_flags $cflags $shared_flags $imported_cflags $extra_cflags $macros $incpaths -MMD -MF $out.d -c $in -o $out",
         deps="gcc",
         depfile="$out.d",
         infiles=[".c"],
-        outfiles=["{outdir}/{in_path}/{in_base}.o"],
+        outfiles=["{outdir}/{binary}.dir/{in_path}/{in_base}{in_ext}.o"],
         variables={"desc": "[C] {in_base}{in_ext}"},
         implicit=["$cc_path"])
 
     compile_cxx = GNUCompiler(
         command="$cxxwrap $cxx -x c++ $pch_flags $cxxflags $shared_flags $imported_cxxflags $extra_cxxflags $macros $incpaths -MMD -MF $out.d -c $in -o $out",
         deps="gcc",
         depfile="$out.d",
         infiles=[".cc", ".cpp", ".cxx"],
-        outfiles=["{outdir}/{in_path}/{in_base}.o"],
+        outfiles=["{outdir}/{binary}.dir/{in_path}/{in_base}{in_ext}.o"],
         variables={"desc": "[CXX] {in_base}{in_ext}"},
         implicit=["$cxx_path"])
 
     compile_asm = GNUCompiler(
         command="$ccwrap $cc -x assembler $pch_flags $asflags $shared_flags $imported_asflags $extra_asflags -MMD -MF $out.d -c $in -o $out",
         deps="gcc",
         depfile="$out.d",
         infiles=[".s", ".asm"],
-        outfiles=["{outdir}/{in_path}/{in_base}.o"],
+        outfiles=["{outdir}/{binary}.dir/{in_path}/{in_base}{in_ext}.o"],
         variables={"desc": "[ASM] {in_base}{in_ext}"},
         implicit=["$cc_path"])
 
     compile_asm_with_cpp = GNUCompiler(
-        "$ccwrap $cc -x assembler-with-cpp $pch_flags $asflags $shared_flags $imported_asflags $extra_asflags $macros $incpaths -MMD -MF $out.d -c $in -o $out",
+        command="$ccwrap $cc -x assembler-with-cpp $pch_flags $asflags $shared_flags $imported_asflags $extra_asflags $macros $incpaths -MMD -MF $out.d -c $in -o $out",
         deps="gcc",
         depfile="$out.d",
         infiles=[".S"],
-        outfiles=["{outdir}/{in_path}/{in_base}.o"],
+        outfiles=["{outdir}/{binary}.dir/{in_path}/{in_base}{in_ext}.o"],
         variables={"desc": "[ASM] {in_base}{in_ext}"},
         implicit=["$cc_path"])
 
+    compile_fbs = FlatbufferCompiler(generator="cpp")
+
+    compile_proto = ProtobufCompiler(generator="cpp")
+
     linker = GNULinker(
         command=" && ".join([
             "$ld $ldflags $imported_ldflags $extra_ldflags $libpaths -Wl,--start-group @objects.list -Wl,--end-group -o $out -Wl,--start-group $libraries -Wl,--end-group",
-            "mkdir -p .debug",
-            "$objcopy --only-keep-debug $out .debug/$binary",
-            "$objcopy --strip-all $out",
-            "$objcopy --add-gnu-debuglink=.debug/$binary $out"
+            "$objcopy_path --only-keep-debug $out .debug/$binary",
+            "$objcopy_path --strip-all $out",
+            "$objcopy_path --add-gnu-debuglink=.debug/$binary $out"
         ]),
+        infiles=[".o", ".obj", ".a"],
         outfiles=["{outdir}/{binary}"],
         variables={"desc": "[LINK] {binary}"},
-        implicit=["$ld_path", "$objcopy_path"])
+        implicit=["$ld_path", "$objcopy_path", ".debug"])
 
     dynlinker = GNULinker(
         command=" && ".join([
             "$ld $ldflags -shared $imported_ldflags $extra_ldflags $libpaths -Wl,--start-group @objects.list -Wl,--end-group -o $out -Wl,--start-group $libraries -Wl,--end-group",
-            "mkdir -p $outdir/.debug",
-            "$objcopy --only-keep-debug $out $outdir/.debug/$binary",
-            "$objcopy --strip-all $out",
-            "$objcopy --add-gnu-debuglink=$outdir/.debug/$binary $out"
+            "$objcopy_path --only-keep-debug $out .debug/lib$binary.so",
+            "$objcopy_path --strip-all $out",
+            "$objcopy_path --add-gnu-debuglink=.debug/lib$binary.so $out"
         ]),
+        infiles=[".o", ".obj", ".a"],
         outfiles=["{outdir}/lib{binary}.so"],
         variables={"desc": "[LINK] {binary}"},
-        implicit=["$ld_path", "$objcopy_path"])
+        implicit=["$ld_path", "$objcopy_path", ".debug"])
 
     archiver = GNUArchiver(
-        command="rm -f $out && $ar cr $out @objects.list",
+        command="$ar -M < objects.list && $ranlib $out",
+        infiles=[".o", ".obj", ".a"],
         outfiles=["{outdir}/lib{binary}.a"],
         variables={"desc": "[AR] lib{binary}.a"},
         implicit=["$ld_path", "$ar_path"])
 
     depimport = GNUDepImporter(
         prefix="lib",
         suffix=".a")
 
 
+class MinGWToolchain(GNUToolchain):
+    linker = GNULinker(
+        command=" && ".join([
+            "$ld $ldflags $imported_ldflags $extra_ldflags $libpaths -Wl,--start-group @objects.list -Wl,--end-group -o $out -Wl,--start-group $libraries -Wl,--end-group",
+            "$objcopy --only-keep-debug $out .debug/$binary.exe",
+            "$objcopy --strip-all $out",
+            "$objcopy --add-gnu-debuglink=.debug/$binary.exe $out"
+        ]),
+        outfiles=["{outdir}/{binary}.exe"],
+        variables={"desc": "[LINK] {binary}"},
+        implicit=["$ld_path", "$objcopy_path", ".debug"])
+
+
+class MSVCArchiver(Rule):
+    def __init__(self, *args, **kwargs):
+        super(MSVCArchiver, self).__init__(*args, aggregate=True, **kwargs)
+
+    def build(self, project, writer, infiles, implicit=None, order_only=None):
+        writer._objects = infiles
+        project._binaries, _ = self._out(project, project.binary)
+        file_list = FileListWriter("objects", project._binaries)
+        file_list.build(project, writer, infiles)
+        super().build(project, writer, infiles, implicit=writer.depimports, order_only=order_only)
+
+    def get_influence(self, task):
+        return "MSVCArchiver" + super().get_influence(task)
+
+
 MSVCCompiler = GNUCompiler
-MSVCArchiver = GNUArchiver
 MSVCLinker = GNULinker
 MSVCDepImporter = GNUDepImporter
 
 
 class MSVCToolchain(Toolchain):
     hh = Skip(infiles=[".h", ".hh", ".hpp", ".hxx"])
-    obj = Objects(infiles=[".o", ".obj", ".a"])
+    bin = Skip(infiles=[".dll", ".exe"])
 
     joltdir = ProjectVariable()
     outdir = ProjectVariable()
     binary = ProjectVariable()
 
-    cl = EnvironmentVariable(default="cl", envname="cl_exe")
-    lib = EnvironmentVariable(default="lib", envname="lib_exe")
-    link = EnvironmentVariable(default="link", envname="link_exe")
+    cl = ToolEnvironmentVariable(default="cl", envname="cl_exe", abspath=True)
+    lib = ToolEnvironmentVariable(default="lib", envname="lib_exe", abspath=True)
+    link = ToolEnvironmentVariable(default="link", envname="link_exe", abspath=True)
+    flatc = ToolEnvironmentVariable(default="flatc", envname="FLATC", abspath=True)
+    protoc = ToolEnvironmentVariable(default="protoc", envname="PROTOC", abspath=True)
 
     asflags = EnvironmentVariable(default="")
     cflags = EnvironmentVariable(default="/EHsc")
     cxxflags = EnvironmentVariable(default="/EHsc")
+    fbflags = EnvironmentVariable(default="")
     ldflags = EnvironmentVariable(default="")
+    protoflags = EnvironmentVariable(default="")
 
     extra_asflags = ProjectVariable(attrib="asflags")
     extra_cflags = ProjectVariable(attrib="cflags")
     extra_cxxflags = ProjectVariable(attrib="cxxflags")
     extra_ldflags = ProjectVariable(attrib="ldflags")
+
+    task_fbflags = ProjectVariable(attrib="fbflags")
+    task_protoflags = ProjectVariable(attrib="protoflags")
+
     macros = Macros(prefix="/D")
     incpaths = IncludePaths(prefix="/I")
     libpaths = LibraryPaths(prefix="/LIBPATH:")
     libraries = Libraries(suffix=".lib")
 
     compile_asm = MSVCCompiler(
         command="$cl /nologo /showIncludes $asflags $extra_asflags $macros $incpaths /c /Tc$in /Fo$out",
         deps="msvc",
         infiles=[".asm", ".s", ".S"],
-        outfiles=["{outdir}/{in_path}/{in_base}.obj"])
+        outfiles=["{outdir}/{binary}.dir/{in_path}/{in_base}.obj"],
+        variables={"desc": "[ASM] {in_base}{in_ext}"},
+        implicit=["$cl_path"])
 
     compile_c = MSVCCompiler(
         command="$cl /nologo /showIncludes $cxxflags $extra_cxxflags $macros $incpaths /c /Tc$in /Fo$out",
         deps="msvc",
         infiles=[".c"],
-        outfiles=["{outdir}/{in_path}/{in_base}.obj"])
+        outfiles=["{outdir}/{binary}.dir/{in_path}/{in_base}.obj"],
+        variables={"desc": "[C] {in_base}{in_ext}"},
+        implicit=["$cl_path"])
 
     compile_cxx = MSVCCompiler(
         command="$cl /nologo /showIncludes $cxxflags $extra_cxxflags $macros $incpaths /c /Tp$in /Fo$out",
         deps="msvc",
         infiles=[".cc", ".cpp", ".cxx"],
-        outfiles=["{outdir}/{in_path}/{in_base}.obj"])
+        outfiles=["{outdir}/{binary}.dir/{in_path}/{in_base}.obj"],
+        variables={"desc": "[CXX] {in_base}{in_ext}"},
+        implicit=["$cl_path"])
+
+    compile_fbs = FlatbufferCompiler(generator="cpp")
+    compile_proto = ProtobufCompiler(generator="cpp")
 
     linker = MSVCLinker(
         command="$link /nologo $ldflags $extra_ldflags $libpaths @objects.list $libraries /out:$out",
-        outfiles=["{outdir}/{binary}.exe"])
+        infiles=[".o", ".obj", ".lib"],
+        outfiles=["{outdir}/{binary}.exe"],
+        variables={"desc": "[LINK] {binary}"},
+        implicit=["$link_path"])
 
     archiver = MSVCArchiver(
         command="$lib /nologo /out:$out @objects.list",
-        outfiles=["{outdir}/{binary}.lib"])
+        infiles=[".o", ".obj", ".lib"],
+        outfiles=["{outdir}/{binary}.lib"],
+        variables={"desc": "[LIB] {binary}"},
+        implicit=["$lib_path"])
 
     depimport = MSVCDepImporter(
         prefix="",
         suffix=".lib")
 
 
+_toolchains = {
+    GNUToolchain: GNUToolchain(),
+    MSVCToolchain: MSVCToolchain(),
+}
+
 if os.name == "nt":
-    toolchain = MSVCToolchain()
+    toolchain = _toolchains[MSVCToolchain]
 else:
-    toolchain = GNUToolchain()
+    toolchain = _toolchains[GNUToolchain]
 
 
-@influence.attribute("asflags")
-@influence.attribute("cflags")
-@influence.attribute("cxxflags")
-@influence.attribute("depimports")
-@influence.attribute("incpaths")
-@influence.attribute("ldflags")
-@influence.attribute("libpaths")
-@influence.attribute("libraries")
-@influence.attribute("macros")
-@influence.attribute("sources")
-@influence.attribute("binary")
-@influence.attribute("publishdir")
-@influence.attribute("toolchain")
 class CXXProject(Task):
     """
 
     The task recognizes these source file types:
     .asm, .c, .cc, .cpp, .cxx, .h, .hh, .hpp, .hxx, .pch, .s, .S
 
     Other file types can be supported through additional rules,
@@ -787,84 +1383,154 @@
 
     abstract = True
     toolchain = None
 
     def __init__(self, *args, **kwargs):
         super(CXXProject, self).__init__(*args, **kwargs)
         self._init_sources()
-        self.toolchain = self.__class__.toolchain() if self.__class__.toolchain else toolchain
-        self.binary = self.expand(self.__class__.binary or self.canonical_name)
+        if self.__class__.toolchain:
+            if self.__class__.toolchain not in _toolchains:
+                _toolchains[self.__class__.toolchain] = self.__class__.toolchain()
+            self.toolchain = _toolchains[self.__class__.toolchain]
+        else:
+            self.toolchain = toolchain
+        self.binary = self.expand(utils.call_or_return(self, self.__class__._binary))
 
         self.asflags = self.expand(utils.as_list(utils.call_or_return(self, self.__class__._asflags)))
         self.cflags = self.expand(utils.as_list(utils.call_or_return(self, self.__class__._cflags)))
         self.cxxflags = self.expand(utils.as_list(utils.call_or_return(self, self.__class__._cxxflags)))
         self.ldflags = self.expand(utils.as_list(utils.call_or_return(self, self.__class__._ldflags)))
 
         self.depimports = utils.as_list(utils.call_or_return(self, self.__class__._depimports))
         self.incpaths = utils.as_list(utils.call_or_return(self, self.__class__._incpaths))
         self.libpaths = utils.as_list(utils.call_or_return(self, self.__class__._libpaths))
         self.libraries = utils.as_list(utils.call_or_return(self, self.__class__._libraries))
         self.macros = utils.as_list(utils.call_or_return(self, self.__class__._macros))
         self._pch_out = None
         self.publishdir = self.expand(self.__class__.publishdir or '')
+
+        self.influence.append(TaskAttributeInfluence("asflags"))
+        self.influence.append(TaskAttributeInfluence("cflags"))
+        self.influence.append(TaskAttributeInfluence("cxxflags"))
+        self.influence.append(TaskAttributeInfluence("depimports"))
+        self.influence.append(TaskAttributeInfluence("incpaths"))
+        self.influence.append(TaskAttributeInfluence("ldflags"))
+        self.influence.append(TaskAttributeInfluence("libpaths"))
+        self.influence.append(TaskAttributeInfluence("libraries"))
+        self.influence.append(TaskAttributeInfluence("macros"))
+        self.influence.append(TaskAttributeInfluence("sources"))
+        self.influence.append(TaskAttributeInfluence("binary"))
+        self.influence.append(TaskAttributeInfluence("publishdir"))
+        self.influence.append(TaskAttributeInfluence("toolchain"))
+
         if self.source_influence:
             for source in self.sources:
-                self.influence.append(influence.FileInfluence(source))
-        else:
-            self._verify_influence()
-        self._init_variables()
-        self._init_rules()
-        self._rule_map = Toolchain.build_rule_map(self)
+                self.influence.append(FileInfluence(source))
+        self._init_rules_and_vars()
 
-    def _init_variables(self):
-        for name, var in Toolchain.all_variables(self):
+    def _init_rules_and_vars(self):
+        self._rules_by_ext = {}
+        self._rules = []
+        self._variables = []
+
+        linker = None
+        if isinstance(self, CXXExecutable):
+            linker = self.toolchain.linker
+        elif isinstance(self, CXXLibrary):
+            if self.shared:
+                linker = self.toolchain.dynlinker
+            else:
+                linker = self.toolchain.archiver
+
+        default_rules, default_vars = [], []
+        rules, variables = Toolchain.all_rules_and_vars(self)
+        if linker:
+            default_rules.append(("__linker", linker))
+        for name, var in default_vars + list(variables.items()):
             var = copy.copy(var)
-            setattr(self, name, var)
             var.name = name
-
-    def _init_rules(self):
-        for name, rule in Toolchain.all_rules(self):
+            setattr(self, var.name, var)
+            self._variables.append(var)
+            self.influence.append(var)
+        for name, rule in default_rules + list(rules.items()):
             rule = copy.copy(rule)
-            setattr(self, name, rule)
+            rule.name = name
+            setattr(self, rule.name, rule)
+            for ext in rule.infiles:
+                self._rules_by_ext[ext] = rule
+            self._rules.append(rule)
+            self.influence.append(rule)
 
     def _init_sources(self):
         self.sources = utils.as_list(utils.call_or_return(self, self.__class__._sources))
 
-    def _verify_influence(self):
-        sources = set(self.sources)
-        for ip in self.influence:
-            if not isinstance(ip, influence.FileInfluence):
-                continue
-            ok = [source for source in sources
-                  if self.expand(source).startswith(self.expand(ip.path))]
-            sources.difference_update(ok)
-        for source in sources:
-            log.warning("Missing influence: {} ({})", source, self.name)
-            self.influence.append(influence.FileInfluence(source))
+    def _verify_influence(self, deps, artifact, tools):
+        # Verify that listed sources and their dependencies are influencing
+        sources = set(self.sources + getattr(self, "headers", []))
+        with tools.cwd(self.outdir):
+            depfiles = [obj + ".d" for obj in getattr(self._writer, "_objects", [])]
+            for depfile in depfiles:
+                try:
+                    data = tools.read_file(depfile)
+                except Exception:
+                    continue
+                data = data.split(":", 1)
+                if len(data) <= 1:
+                    continue
+
+                depsrcs = data[1]
+                depsrcs = depsrcs.split()
+                depsrcs = [f.rstrip("\\").strip() for f in depsrcs]
+                depsrcs = [tools.expand_relpath(dep, self.joltdir) for dep in filter(lambda n: n, depsrcs)]
+                sources = sources.union(depsrcs)
+        super()._verify_influence(deps, artifact, tools, sources)
+
+    def _expand_headers(self):
+        headers = []
+        for header in getattr(self, "headers", []):
+            list = self.tools.glob(header)
+            raise_task_error_if(
+                not list and not ('*' in header or '?' in header), self,
+                "header file '{0}' not found", fs.path.basename(header))
+            headers += list
+        self.headers = headers
+
+    def _expand_sources(self, deps, tools):
+        imported_sources = []
+        for _, artifact in deps.items():
+            sources = artifact.cxxinfo.sources.items()
+            if sources:
+                sandbox = tools.sandbox(artifact, self.incremental)
+                imported_sources += [
+                    tools.expand_relpath(fs.path.join(sandbox, path), self.joltdir)
+                    for path in sources
+                ]
 
-    def _expand_sources(self):
         sources = []
-        for source in self.sources:
-            l = self.tools.glob(source)
+        for source in self.sources + imported_sources:
+            list = self.tools.glob(source)
             raise_task_error_if(
-                not l and not ('*' in source or '?' in source), self,
-                "source file '{0}' not found", fs.path.basename(source))
-            sources += l
+                not list and not ('*' in source or '?' in source), self,
+                "listed source file '{0}' not found in workspace", fs.path.basename(source))
+            sources += list
         self.sources = sources
 
-    def _write_ninja_file(self, basedir, deps, tools):
-        with open(fs.path.join(basedir, "build.ninja"), "w") as fobj:
+    def _write_ninja_file(self, basedir, deps, tools, filename="build.ninja"):
+        with open(fs.path.join(basedir, filename), "w") as fobj:
             writer = ninja.Writer(fobj)
-            self._populate_variables(writer, deps, tools)
-            self._populate_rules(writer, deps, tools)
+            writer.depimports = [tools.expand_relpath(dep, self.outdir)
+                                 for dep in self.depimports]
+            writer.objects = []
+            writer.sources = copy.copy(self.sources)
+            self._populate_rules_and_variables(writer, deps, tools)
             self._populate_inputs(writer, deps, tools)
-            self._populate_project(writer, deps, tools)
             writer.close()
+            return writer
 
-    def _write_shell_file(self, basedir, deps, tools):
+    def _write_shell_file(self, basedir, deps, tools, writer):
         filepath = fs.path.join(basedir, "compile")
         with open(filepath, "w") as fobj:
             data = """#!{executable}
 import sys
 import subprocess
 
 objects = {objects}
@@ -898,60 +1564,105 @@
 if __name__ == "__main__":
     main()
 
 """
             fobj.write(
                 data.format(
                     executable=sys.executable,
-                    objects=[fs.path.relpath(o, self.outdir) for o in self.objects]))
+                    objects=[fs.path.relpath(o, self.outdir) for o in writer.objects]))
         tools.chmod(filepath, 0o777)
 
     def find_rule(self, ext):
-        rule = self._rule_map.get(ext)
+        if not ext:
+            return Skip()
+        rule = self._rules_by_ext.get(ext)
         if rule is None:
-            rule = toolchain.find_rule(ext)
+            rule = self.toolchain.find_rule(ext)
         raise_task_error_if(
             not rule, self,
             "no build rule available for files with extension '{0}'", ext)
         return rule
 
-    def _populate_variables(self, writer, deps, tools):
+    def _populate_rules_and_variables(self, writer, deps, tools):
+        tc_rules, tc_vars = Toolchain.all_rules_and_vars(self.toolchain)
+
         variables = set()
-        for name, var in Toolchain.all_variables(self):
+        for var in self._variables:
             var.create(self, writer, deps, tools)
-            variables.add(name)
-        for name, var in Toolchain.all_variables(self.toolchain):
+            variables.add(var.name)
+        for name, var in tc_vars.items():
             if name not in variables:
                 var.create(self, writer, deps, tools)
         writer.newline()
 
-    def _populate_rules(self, writer, deps, tools):
         rules = set()
-        for name, rule in Toolchain.all_rules(self):
+        for rule in self._rules:
             rule.create(self, writer, deps, tools)
-            rules.add(name)
-        for name, rule in Toolchain.all_rules(self.toolchain):
+            rules.add(rule.name)
+        for name, rule in tc_rules.items():
             if name not in rules:
                 rule.create(self, writer, deps, tools)
         writer.newline()
 
-    def _populate_inputs(self, writer, deps, tools):
-        self.objects = []
-        sources = copy.copy(self.sources)
+    def _populate_inputs(self, writer, deps, tools, sources=None):
+        # Source process queue
+        sources = sources or writer.sources
+        if not sources:
+            return
+
+        sources = list(zip(copy.copy(sources), [None] * len(sources)))
+        sources = [(tools.expand_path(source), origin) for source, origin in sources]
+
+        # Aggregated list of sources for each rule
+        rule_source_list = {}
         while sources:
-            source = sources.pop()
+            source, origin = sources.pop()
             _, ext = fs.path.splitext(source)
             rule = self.find_rule(ext)
-            output = rule.build(self, writer, tools.expand_path(source))
-            sources.extend(output or [])
+
+            if rule is origin:
+                # Don't feed sources back to rules from where they originated,
+                # as it may cause dependency cycles.
+                continue
+
+            try:
+                rule_source_list[rule].append((source, origin))
+                # Aggregating rules only have one set of outputs
+                # while regular rules produce one set of outputs
+                # for each input.
+                if not rule.aggregate:
+                    output = rule.output(self, source)
+                    if output:
+                        writer.objects.extend(output)
+                        sources.extend(zip(output, [rule] * len(output)))
+            except KeyError:
+                rule_source_list[rule] = [(source, origin)]
+                output = rule.output(self, source)
+                if output:
+                    writer.objects.extend(output)
+                    sources.extend(zip(output, [rule] * len(output)))
+
+        # No more inputs/outputs to process, now emit all build rules
+        for rule, source_list_origin in rule_source_list.items():
+            source_list, origins = [], set()
+            for source, origin in source_list_origin:
+                source_list.append(source)
+                origins.add(origin)
+            source_list = list(map(tools.expand_path, source_list))
+            rule.build(self, writer, source_list, order_only=[origin.phony for origin in origins if origin and origin.phony])
+
+        # Done
         writer.newline()
 
     def _populate_project(self, writer, deps, tools):
         pass
 
+    def _binary(self):
+        return utils.call_or_return(self, self.__class__.binary) or self.canonical_name
+
     def _incpaths(self):
         return utils.call_or_return(self, self.__class__.incpaths)
 
     def _ldflags(self):
         return utils.call_or_return(self, self.__class__.ldflags)
 
     def _libpaths(self):
@@ -978,109 +1689,263 @@
     def _depimports(self):
         return utils.call_or_return(self, self.__class__.depimports)
 
     def clean(self, tools):
         self.outdir = tools.builddir("ninja", self.incremental)
         tools.rmtree(self.outdir, ignore_errors=True)
 
+    def _get_keepdepfile(self, tools):
+        try:
+            tools.run("ninja -d list", output=False)
+        except JoltCommandError as e:
+            return " -d keepdepfile" if "keepdepfile" in "".join(e.stdout) else ""
+        return ""
+
     def run(self, deps, tools):
-        self._expand_sources()
+        """
+        Generates a Ninja build file and invokes Ninja to build the project.
+
+        The build file and all intermediate files are written to a build
+        directory within the workspace. By default, the directory persists
+        between different invokations of Jolt to allow projects to be built
+        incrementally. The behavior can be changed with the ``incremental``
+        class attribute.
+        """
+
         self.outdir = tools.builddir("ninja", self.incremental)
-        self._write_ninja_file(self.outdir, deps, tools)
-        verbose = "-v" if log.is_verbose() else ""
+        self._expand_headers()
+        self._expand_sources(deps, tools)
+        self._writer = self._write_ninja_file(self.outdir, deps, tools)
+        verbose = " -v" if log.is_verbose() else ""
         threads = config.get("jolt", "threads", tools.getenv("JOLT_THREADS", None))
-        threads = "-j " + threads if threads else ""
-        tools.run("ninja -d keepdepfile {2} -C {0} {1}", self.outdir, verbose, threads)
+        threads = " -j" + threads if threads else ""
+        depsfile = self._get_keepdepfile(tools)
+        try:
+            tools.run("ninja{3}{2} -C {0} {1}", self.outdir, verbose, threads, depsfile)
+        except JoltCommandError as e:
+            with utils.ignore_exception(), self.report() as report:
+                self._report_errors(report, "\n".join(e.stdout))
+            raise CompileError()
 
     def shell(self, deps, tools):
-        self._expand_sources()
+        """
+        Invoked to start a debug shell.
+
+        The method prepares the environment with attributes exported by task requirement
+        artifacts. The shell is entered by passing the ``-g`` flag to the build command.
+
+        For Ninja tasks, a special ``compile`` command is made available inside
+        the shell. The command can be used to compile individual source files which
+        is useful when troubleshooting compilation errors. Run ``compile -h`` for
+        help.
+
+        Task execution resumes normally when exiting the shell.
+        """
+        self._expand_headers()
+        self._expand_sources(deps, tools)
         self.outdir = tools.builddir("ninja", self.incremental)
-        self._write_ninja_file(self.outdir, deps, tools)
-        self._write_shell_file(self.outdir, deps, tools)
+        writer = self._write_ninja_file(self.outdir, deps, tools)
+        self._write_shell_file(self.outdir, deps, tools, writer)
         pathenv = self.outdir + os.pathsep + tools.getenv("PATH")
         with tools.cwd(self.outdir), tools.environ(PATH=pathenv):
             print()
             print("Use the 'compile' command to build individual compilation targets")
             super(CXXProject, self).shell(deps, tools)
 
+    def _report_errors(self, report, logbuffer):
+        # GCC style errors
+        report.add_regex_errors_with_file(
+            "Compiler Error",
+            r"(?P<location>(?P<file>.*?):(?P<line>[0-9]+):(?P<col>[0-9]+)): (?P<message>.*)",
+            logbuffer,
+            self.outdir,
+            lambda err: not err["message"].startswith("note:"))
+
+        # other compiler errors
+        report.add_regex_errors_with_file(
+            "Compiler Error",
+            r"(?P<location>(?P<file>.*?)\((?P<line>[0-9]+)\)): (?P<message>error: .*)",
+            logbuffer,
+            self.outdir)
+
+        # Linker errors
+        report.add_regex_errors(
+            "Linker Error",
+            r"(?P<location>(?P<file>.*?):(.*?)): (?P<message>(undefined reference|multiple definition).*)",
+            logbuffer)
+        report.add_regex_errors(
+            "Linker Error",
+            r"(?P<location>ld): (error|warning): (?P<message>.*)",
+            logbuffer)
+
 
-@influence.attribute("shared")
 class CXXLibrary(CXXProject):
     """
     Builds a C/C++ library.
     """
 
     abstract = True
     shared = False
 
+    headers = []
+    """ List of public headers to be published with the artifact """
+
+    publishapi = "include/"
+    """ The artifact path where public headers are published. """
+
     publishdir = "lib/"
     """ The artifact path where the library is published. """
 
+    selfsustained = False
+    """ Consume this library independently from its requirements.
+
+    When self-sustained, all static libraries listed as requirements are merged
+    into the final library. Merging can also be achieved by listing libraries
+    as source files.
+
+    See :func:`Task.selfsustained <jolt.Task.selfsustained>` for general information.
+    """
+
+    strip = True
+    """
+    Remove debug information from binary.
+
+    When using the GNU toolchain, debug information is kept in a separate binary
+    which is either published or not depending on the value of this attribute.
+    It's found in a .debug directory if present.
+
+    Only applicable to shared libraries.
+    """
+
     def __init__(self, *args, **kwargs):
         super(CXXLibrary, self).__init__(*args, **kwargs)
+        self.headers = utils.as_list(utils.call_or_return(self, self.__class__._headers))
+        self.publishlib = self.publishdir
+        if self.source_influence:
+            for header in self.headers:
+                self.influence.append(FileInfluence(header))
+        self.influence.append(TaskAttributeInfluence("headers"))
+        self.influence.append(TaskAttributeInfluence("publishapi"))
+        self.influence.append(TaskAttributeInfluence("shared"))
+
+    def _headers(self):
+        return utils.call_or_return(self, self.__class__.headers)
 
     def _populate_inputs(self, writer, deps, tools):
-        self.depimports += self.toolchain.depimport.build(self, writer, deps)
+        writer.depimports += self.toolchain.depimport.build(self, writer, deps)
         super(CXXLibrary, self)._populate_inputs(writer, deps, tools)
 
-    def _populate_project(self, writer, deps, tools):
-        if self.shared:
-            self.outfiles = self.toolchain.dynlinker.build(self, writer, self.objects)
-        else:
-            self.outfiles = self.toolchain.archiver.build(self, writer, self.objects)
-
     def publish(self, artifact, tools):
+        """
+        Publishes the library.
+
+        By default, the library is collected into a directory as specified
+        by the ``publishdir`` class attribute. Library path metadata
+        for this directory as well as linking metadata is automatically exported.
+        The relative path of the library within the artifact is also exported as
+        a metadata string. It can be read by consumers by accessing
+        ``artifact.strings.library``.
+
+        Public headers listed in the ``headers`` class attribute are collected into
+        a directory as specified by the ``publishapi`` class attribute.
+        Include path metadata for this directory is automatically exported.
+
+        """
+
         with tools.cwd(self.outdir):
-            artifact.collect("*{binary}.a", self.publishdir)
-            artifact.collect("*{binary}.dll", self.publishdir)
-            artifact.collect("*{binary}.lib", self.publishdir)
-            artifact.collect("*{binary}.so", self.publishdir)
-        artifact.cxxinfo.libpaths.append(self.publishdir)
-        artifact.cxxinfo.libraries.append(self.binary)
-        artifact.strings.library = fs.path.join(
-            self.publishdir, fs.path.basename(self.outfiles[0]))
+            if not self.shared:
+                artifact.collect("*{binary}.a", self.publishlib)
+                artifact.collect("*{binary}.lib", self.publishlib)
+            else:
+                artifact.collect("*{binary}.dll", self.publishlib)
+                artifact.collect("*{binary}.so", self.publishlib)
+            if self.shared and not self.strip:
+                artifact.collect(".debug/*{binary}.so", self.publishdir)
+
+        if self.headers:
+            for header in self.headers:
+                artifact.collect(header, self.publishapi)
+            artifact.cxxinfo.incpaths.append(self.publishapi)
+
+        if hasattr(self, "_binaries"):
+            artifact.cxxinfo.libpaths.append(self.publishlib)
+            artifact.cxxinfo.libraries.append(self.binary)
+            artifact.strings.library = fs.path.join(
+                self.publishdir, fs.path.basename(self._binaries[0]))
+
 
 CXXLibrary.__doc__ += CXXProject.__doc__
 
 
-@influence.attribute("strip")
 class CXXExecutable(CXXProject):
     """
     Builds a C/C++ executable.
     """
 
     abstract = True
+
     selfsustained = True
+    """ Consume this executable independently from its requirements.
+
+    When self-sustained, all shared libraries listed as requirements are
+    published toghether with the executable.
+
+    See :func:`Task.selfsustained <jolt.Task.selfsustained>` for general information.
+    """
 
     publishdir = "bin/"
     """ The artifact path where the binary is published. """
 
     strip = True
-    """ Strip binary from debug information. """
+    """
+    Remove debug information from binary.
+
+    When using the GNU toolchain, debug information is kept in a separate binary
+    which is either published or not depending on the value of this attribute.
+    It's found in a .debug directory if present.
+
+    Only applicable to shared libraries.
+    """
 
     def __init__(self, *args, **kwargs):
         super(CXXExecutable, self).__init__(*args, **kwargs)
         self.strip = utils.call_or_return(self, self.__class__._strip)
+        self.influence.append(TaskAttributeInfluence("strip"))
 
     def _populate_inputs(self, writer, deps, tools):
-        self.depimports += self.toolchain.depimport.build(self, writer, deps)
+        writer.depimports += self.toolchain.depimport.build(self, writer, deps)
         super(CXXExecutable, self)._populate_inputs(writer, deps, tools)
 
     def _populate_project(self, writer, deps, tools):
-        self.toolchain.linker.build(self, writer, [o for o in reversed(self.objects)])
+        outputs = self.toolchain.linker.build(self, writer, [o for o in reversed(writer.objects)])
+        super(CXXExecutable, self)._populate_inputs(writer, deps, tools, outputs)
 
     def _strip(self):
         return utils.call_or_return(self, self.__class__.strip)
 
     def publish(self, artifact, tools):
+        """
+        Publishes the linked executable.
+
+        By default, the executable is collected into a directory as specified
+        by the ``publishdir`` class attribute. The relative path of the executable
+        within the artifact is exported as a metadata string. It can be read by
+        consumers by accessing ``artifact.strings.executable``.
+
+        The method appends the ``PATH`` environment variable with the path to
+        the executable to allow consumers to run it easily.
+
+        """
+
         with tools.cwd(self.outdir):
             if os.name == "nt":
                 artifact.collect(self.binary + '.exe', self.publishdir)
             else:
                 artifact.collect(self.binary, self.publishdir)
-                if not self.strip:
-                    artifact.collect(".debug", self.publishdir)
+            if not self.strip:
+                artifact.collect(".debug", self.publishdir)
         artifact.environ.PATH.append(self.publishdir)
         artifact.strings.executable = fs.path.join(
             self.publishdir, self.binary)
 
+
 CXXExecutable.__doc__ += CXXProject.__doc__
```

### Comparing `jolt-0.9.9/jolt/plugins/repo.py` & `jolt-0.9.93/jolt/plugins/repo.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             return result.splitlines()
         assert False, "git command failed"
 
     def has_local_ref(self, ref):
         with self.tools.cwd(self.path_or_name):
             try:
                 return True if self.tools.run("git show-ref {0}", ref, output=False) else False
-            except:
+            except Exception:
                 return False
 
     def get_remote_ref(self, commit, remote, pattern=None):
         with self.tools.cwd(self.path_or_name):
             result = self.tools.run(
                 "git ls-remote {0}{1}",
                 remote,
```

### Comparing `jolt-0.9.9/jolt/plugins/git.py` & `jolt-0.9.93/jolt/plugins/git.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,298 +1,378 @@
-import copy
+import os
+import pygit2
+import re
 
-from jolt.tasks import Resource, WorkspaceResource, Parameter, BooleanParameter, Export, TaskRegistry
-from jolt.influence import HashInfluenceProvider, HashInfluenceRegistry, FileInfluence
+from jolt.tasks import BooleanParameter, Export, Parameter, TaskRegistry, WorkspaceResource
+from jolt.influence import FileInfluence, HashInfluenceRegistry
 from jolt.tools import Tools
 from jolt.loader import JoltLoader
+from jolt import config
 from jolt import filesystem as fs
 from jolt import log
 from jolt import utils
 from jolt.error import JoltCommandError
 from jolt.error import raise_error
 from jolt.error import raise_error_if
 from jolt.error import raise_task_error_if
 
 
 log.verbose("[Git] Loaded")
 
 
-_tree = {}
-_tree_hash_cache = {}
-
-
-
 class GitRepository(object):
     def __init__(self, url, path, relpath, refspecs=None):
         self.path = path
         self.relpath = relpath
+        self.gitpath = None
         self.tools = Tools()
         self.url = url
-        self.refspecs = utils.as_list(refspecs or [])
+        self.default_refspecs = [
+            '+refs/heads/*:refs/remotes/origin/*',
+            '+refs/tags/*:refs/remotes/origin/*',
+        ]
+        self.refspecs = refspecs or []
+        self._tree_hash = {}
+        self._original_head = True
+        self._init_repo()
+
+    def _init_repo(self):
+        gitpath = os.path.join(self.path, ".git")
+        if os.path.isdir(os.path.join(self.path, ".git")):
+            self.gitpath = gitpath
+            self.repository = pygit2.Repository(self.gitpath)
+        elif os.path.exists(gitpath):
+            with self.tools.cwd(self.path):
+                path = self.tools.run("git rev-parse --git-dir", output=False)
+            self.gitpath = os.path.join(self.path, path)
+            self.repository = pygit2.Repository(self.gitpath)
+        else:
+            self.repository = None
+
+    @utils.cached.instance
+    def _git_folder(self):
+        return self.gitpath
 
     @utils.cached.instance
-    def _get_git_folder(self):
-        return fs.path.join(self.path, ".git")
+    def _git_index(self):
+        return fs.path.join(self.gitpath, "index")
 
     @utils.cached.instance
-    def _get_git_index(self):
-        return fs.path.join(self.path, ".git", "index")
+    def _git_jolt_index(self):
+        return fs.path.join(self.gitpath, "jolt-index")
 
     def is_cloned(self):
-        return fs.path.exists(self._get_git_folder())
+        return self.gitpath is not None
 
     def is_indexed(self):
-        return fs.path.exists(self._get_git_index())
-
-    def _is_synced(self):
-        with self.tools.cwd(self.path):
-            return True if self.tools.run("git branch -r --contains HEAD", output_on_error=True) else False
-        return True
+        return self.is_cloned() and fs.path.exists(self._git_index())
 
     def clone(self):
         log.info("Cloning into {0}", self.path)
         if fs.path.exists(self.path):
             with self.tools.cwd(self.path):
                 self.tools.run("git init && git remote add origin {} && git fetch",
                                self.url, output_on_error=True)
         else:
             self.tools.run("git clone {0} {1}", self.url, self.path, output_on_error=True)
+        self._init_repo()
         raise_error_if(
-            not fs.path.exists(self._get_git_folder()),
+            self.repository is None,
             "git: failed to clone repository '{0}'", self.relpath)
 
     @utils.cached.instance
-    def _diff(self, path="/"):
+    def diff_unchecked(self):
+        if not self.is_indexed():
+            return ""
+
+        # Build the jolt index file
         self.write_tree()
-        with self.tools.cwd(self.path):
-            index = fs.path.join(self.path, ".git", "jolt-index")
-            with self.tools.environ(GIT_INDEX_FILE=index):
-                return self.tools.run("git diff --binary --no-ext-diff HEAD .{0}".format(path),
-                                      output_on_error=True,
-                                      output_rstrip=False)
 
-    def diff(self, path="/"):
-        return self._diff(path) if self.is_indexed() else ""
+        # Diff against the jolt index
+        with self.tools.environ(GIT_INDEX_FILE=self._git_jolt_index()), self.tools.cwd(self.path):
+            return self.tools.run("git diff --binary --no-ext-diff HEAD ./",
+                                  output_on_error=True,
+                                  output_rstrip=False)
+
+    def diff(self):
+        diff = self.diff_unchecked()
+        dlim = config.getsize("git", "maxdiffsize", "1M")
+        raise_error_if(
+            len(diff) > dlim,
+            "Repository '{}' has uncommitted changes. Size of patch exceeds configured transfer limit ({} > {} bytes)."
+            .format(self.relpath, len(diff), dlim))
+        return diff
 
     def patch(self, patch):
         if not patch:
             return
         with self.tools.cwd(self.path), self.tools.tmpdir("git") as t:
             patchfile = fs.path.join(t.path, "jolt.diff")
             with open(patchfile, "wb") as f:
                 f.write(patch.encode())
             log.info("Applying patch to {0}", self.path)
             self.tools.run("git apply --whitespace=nowarn {patchfile}", patchfile=patchfile)
 
-    @utils.cached.instance
-    def _head(self):
-        with self.tools.cwd(self.path):
-            return self.tools.run("git rev-parse HEAD", output_on_error=True)
-
     def head(self):
-        return self._head() if self.is_cloned() else ""
+        if not self.is_cloned():
+            return None
+        return str(self.repository.head.target)
 
     def is_head(self, rev):
         return self.is_indexed() and self.head() == rev
 
+    def is_original_head(self):
+        return self._original_head
+
+    def is_valid_sha(self, rev):
+        return re.match(r"[0-9a-f]{40}", rev)
+
     def rev_parse(self, rev):
+        if self.is_valid_sha(rev):
+            return rev
         with self.tools.cwd(self.path):
-            return self.tools.run("git rev-parse {rev}", rev=rev, output_on_error=True)
+            try:
+                commit = self.repository.revparse_single(rev)
+            except KeyError:
+                self.fetch()
+                try:
+                    commit = self.repository.revparse_single(rev)
+                except Exception:
+                    raise_error("invalid git reference: {}", rev)
+            try:
+                return str(commit.id)
+            except Exception:
+                return str(commit)
 
     @utils.cached.instance
     def write_tree(self):
         tools = Tools()
-        index = fs.path.join(self.path, ".git", "jolt-index")
-        gitpath = fs.path.dirname(index)
-
-        tree = _tree.get(gitpath)
-        if tree is not None:
-            return tree
-
-        with tools.environ(GIT_INDEX_FILE=index):
-            with tools.cwd(gitpath):
-                tools.copy("index", "jolt-index")
-            with tools.cwd(fs.path.dirname(gitpath)):
-                _tree[gitpath] = tree = tools.run(
-                    "git -c core.safecrlf=false add -A && git write-tree",
-                    output_on_error=True)
-
+        with tools.cwd(self._git_folder()):
+            tools.copy("index", "jolt-index")
+        with tools.environ(GIT_INDEX_FILE=self._git_jolt_index()), tools.cwd(self.path):
+            tree = tools.run(
+                "git -c core.safecrlf=false add -A && git write-tree",
+                output_on_error=True)
         return tree
 
-    def tree_hash(self, sha="HEAD", path="/"):
-        full_path = fs.path.join(self.path, path)
-        value = _tree_hash_cache.get((full_path, sha))
-        if value is None:
-            if sha == "HEAD":
-                tree = self.write_tree()
+    def tree_hash(self, sha=None, path="/"):
+        # When sha is None, the caller want the tree hash of the repository's
+        # current workspace state. If no checkout has been made, that would be the
+        # tree that was written upon initialization of the repository as it
+        # includes any uncommitted changes. If a checkout has been made since
+        # the repo was initialized, make this an explicit request for the current
+        # head - there can be no local changes.
+        if sha is None:
+            if self.is_original_head():
+                tree = self.repository.get(self.write_tree())
             else:
-                try:
-                    with self.tools.cwd(self.path):
-                        tree = self.tools.run("git rev-parse {0}^{{tree}}", sha, output=False)
-                except:
-                    with self.tools.cwd(self.path):
-                        self.fetch()
-                        tree = self.tools.run("git rev-parse {0}^{{tree}}", sha, output=False)
-            if path == "/":
-                return tree
-            with self.tools.cwd(self.path):
-                _tree_hash_cache[(full_path, sha)] = value = self.tools.run(
-                    "git rev-parse {0}:{1}".format(tree, path), output=False)
+                sha = self.head()
+
+        path = fs.path.normpath(path)
+        full_path = fs.path.join(self.path, path) if path != "/" else self.path
+
+        # Lookup tree hash value in cache
+        value = self._tree_hash.get((full_path, sha))
+        if value is not None:
+            return value
+
+        # Translate explicit sha to tree
+        if sha is not None:
+            commit = self.rev_parse(sha)
+            obj = self.repository.get(commit)
+            try:
+                tree = obj.tree
+            except AttributeError:
+                tree = obj.get_object().tree
+
+        # Traverse tree from root to requested path
+        if path != "/":
+            tree = tree[fs.as_posix(path)]
+
+        # Update tree hash cache
+        self._tree_hash[(full_path, sha)] = value = tree.id
+
         return value
 
     def clean(self):
         with self.tools.cwd(self.path):
             return self.tools.run("git clean -dfx", output_on_error=True)
 
     def reset(self):
         with self.tools.cwd(self.path):
             return self.tools.run("git reset --hard", output_on_error=True)
 
     def fetch(self):
-        refspecs = self.refspecs or []
-        for refspec in [''] + refspecs:
+        refspec = " ".join(self.default_refspecs + self.refspecs)
+        with self.tools.cwd(self.path):
+            log.info("Fetching {0} from {1}", refspec or 'commits', self.url)
             self.tools.run("git fetch {url} {refspec}",
                            url=self.url,
-                           refspec=refspec or '')
+                           refspec=refspec or '',
+                           output_on_error=True)
 
     def checkout(self, rev):
         log.info("Checking out {0} in {1}", rev, self.path)
         with self.tools.cwd(self.path):
             try:
                 return self.tools.run("git checkout -f {rev}", rev=rev, output=False)
-            except:
+            except Exception:
                 self.fetch()
                 return self.tools.run("git checkout -f {rev}", rev=rev, output_on_error=True)
+        self._original_head = False
 
 
-class LocalGitRepository(GitRepository):
-    def fetch(self):
-        pass
+_gits = {}
 
-    def clone(self):
-        raise_error("attempt to clone local git repository at '{}'", self.relpath)
+
+def new_git(url, path, relpath, refspecs=None):
+    refspecs = utils.as_list(refspecs or [])
+    try:
+        git = _gits[path]
+        raise_error_if(git.url != url, "multiple git repositories required at {}", relpath)
+        raise_error_if(git.refspecs != refspecs,
+                       "conflicting refspecs detected for git repository at  {}", relpath)
+        return git
+    except Exception:
+        git = _gits[path] = GitRepository(url, path, relpath, refspecs)
+        return git
 
 
 class GitInfluenceProvider(FileInfluence):
     name = "Git"
 
     def __init__(self, path):
         super(GitInfluenceProvider, self).__init__(path)
-        self.path = path
+        self.path = path.rstrip(fs.sep)
         self.name = GitInfluenceProvider.name
 
     @property
     def joltdir(self):
         return JoltLoader.get().joltdir
 
     def _find_dotgit(self, path):
-        while path != self.joltdir:
-            if fs.path.isdir(fs.path.join(path, ".git")):
+        ppath = None
+        while path != ppath:
+            if fs.path.exists(fs.path.join(path, ".git")):
                 return path
+            ppath = path
             path = fs.path.dirname(path)
         raise_error("no git repository found at '{}'", self.path)
 
     @utils.cached.instance
     def get_influence(self, task):
-        tools = Tools(task)
-        path = tools.expand_path(fs.path.join(task.joltdir, self.path))
+        tools = Tools(task, task.joltdir)
+        path = tools.expand_path(self.path)
         git_abs = self._find_dotgit(path)
-        git_rel = git_abs[len(self.joltdir)+1:]
-        relpath = path[len(git_abs)+1:]
+        git_rel = git_abs[len(self.joltdir) + 1:]
+        relpath = path[len(git_abs) + 1:]
+        relpath = fs.as_posix(relpath) if relpath else relpath
 
         if not fs.path.exists(path):
             return "{0}/{1}: N/A".format(git_rel, relpath)
         try:
-            git = LocalGitRepository(None, git_abs, git_rel)
-
+            git = new_git(None, git_abs, git_rel)
             return "{0}/{1}: {2}".format(git_rel, relpath, git.tree_hash(path=relpath or "/"))
+        except KeyError:
+            return "{0}/{1}: N/A".format(git_rel, relpath)
         except JoltCommandError as e:
             stderr = "\n".join(e.stderr)
             if "exists on disk, but not in" in stderr:
                 return "{0}/{1}: N/A".format(git_rel, relpath)
-            #for line in e.stderr:
-            #    log.stderr(line)
             raise e
 
+    def is_influenced_by(self, task, path):
+        tools = Tools(task, task.joltdir)
+        gitpath = tools.expand_path(self.path)
+        return fs.is_relative_to(path, gitpath)
+
+
 def global_influence(path, cls=GitInfluenceProvider):
     HashInfluenceRegistry.get().register(cls(path))
 
 
 def influence(path, git_cls=GitInfluenceProvider):
     def _decorate(cls):
         _old_influence = cls._influence
+
         def _influence(self, *args, **kwargs):
             influence = _old_influence(self, *args, **kwargs)
             influence.append(git_cls(path=path))
             return influence
+
         cls._influence = _influence
         return cls
     return _decorate
 
 
-class GitSrc(WorkspaceResource):
+class GitSrc(WorkspaceResource, FileInfluence):
     """ Clones a Git repo.
     """
 
     name = "git-src"
     url = Parameter(help="URL to the git repo to be cloned. Required.")
     sha = Parameter(required=False, help="Specific commit or tag to be checked out. Optional.")
     path = Parameter(required=False, help="Local path where the repository should be cloned.")
     defer = BooleanParameter(False, help="Defer cloning until a consumer task must be built.")
-    _revision = Export(value=lambda self: self._get_revision() or self.git.head())
-    _diff = Export(value=lambda self: self.git.diff(), encoded=True)
+    _revision = Export(value=lambda t: t._export_revision())
+    _diff = Export(value=lambda t: t.git.diff(), encoded=True)
 
     def __init__(self, *args, **kwargs):
         super(GitSrc, self).__init__(*args, **kwargs)
         self.joltdir = JoltLoader.get().joltdir
         self.relpath = str(self.path) or self._get_name()
         self.abspath = fs.path.join(self.joltdir, self.relpath)
         self.refspecs = kwargs.get("refspecs", [])
-        self.git = GitRepository(self.url, self.abspath, self.relpath, self.refspecs)
-        self.influence.append(self)
+        self.git = new_git(self.url, self.abspath, self.relpath, self.refspecs)
 
     @utils.cached.instance
     def _get_name(self):
         repo = fs.path.basename(self.url.get_value())
         name, _ = fs.path.splitext(repo)
         return name
 
+    def _export_revision(self):
+        return self.sha.value or self.git.head()
+
     def _get_revision(self):
-        if self._revision.value is not None:
+        if self._revision.is_imported:
             return self._revision.value
         if not self.sha.is_unset():
             return self.sha.get_value()
         return None
 
-    def _get_diff(self):
-        return self._diff.value
-
-    def acquire(self, artifact, env, tools):
-        self.acquire_ws()
+    def acquire(self, **kwargs):
+        self._acquire_ws()
 
     def acquire_ws(self):
+        if self.defer is None or self.defer.is_false:
+            self._acquire_ws()
+
+    def _acquire_ws(self):
         if not self.git.is_cloned():
             self.git.clone()
+        if not self._revision.is_imported:
+            self.git.diff_unchecked()
         rev = self._get_revision()
         if rev is not None:
             raise_task_error_if(
-                self._revision.value is None and not self.sha.is_unset() and self.git.diff(), self,
+                not self._revision.is_imported and not self.sha.is_unset() and self.git.diff(), self,
                 "explicit sha requested but git repo '{0}' has local changes", self.git.relpath)
             # Should be safe to do this now
             rev = self.git.rev_parse(rev)
-            if not self.git.is_head(rev) or self._revision.value is not None:
+            if not self.git.is_head(rev) or self._revision.is_imported:
                 self.git.checkout(rev)
                 self.git.clean()
-                self.git.patch(self._get_diff())
+                self.git.patch(self._diff.value)
 
-    @utils.cached.instance
     def get_influence(self, task):
-        if self.defer.is_false and not self.git.is_cloned():
-            self.git.clone()
-        return "Enabled"
+        return None
+
+    def is_influenced_by(self, task, path):
+        return fs.is_relative_to(path, self.abspath) and self.sha.is_set()
 
 
 TaskRegistry.get().add_task_class(GitSrc)
 
 
 class Git(GitSrc):
     """ Clones a Git repo.
@@ -302,25 +382,37 @@
 
     """
     name = "git"
     url = Parameter(help="URL to the git repo to be cloned. Required.")
     sha = Parameter(required=False, help="Specific commit or tag to be checked out. Optional.")
     path = Parameter(required=False, help="Local path where the repository should be cloned.")
     defer = None
-    _revision = Export(value=lambda self: self._get_revision())
-    _diff = Export(value=lambda self: self.git.diff(), encoded=True)
+    _revision = Export(value=lambda t: t._export_revision())
+    _diff = Export(value=lambda t: t.git.diff(), encoded=True)
 
     def __init__(self, *args, **kwargs):
         super(Git, self).__init__(*args, **kwargs)
+        self.influence.append(self)
 
     @utils.cached.instance
     def get_influence(self, task):
         if not self.git.is_cloned():
             self.git.clone()
+        if not self._revision.is_imported:
+            self.git.diff_unchecked()
         rev = self._get_revision()
-        if rev is not None:
-            return self.git.tree_hash(rev)
-        return "{0}: {1}".format(
-            self.git.relpath,
-            self.git.tree_hash())
+
+        try:
+            if rev is not None:
+                th = self.git.tree_hash(rev)
+            else:
+                th = self.git.tree_hash()
+        except KeyError:
+            th = "N/A"
+
+        return "{0}: {1}".format(self.git.relpath, th)
+
+    def is_influenced_by(self, task, path):
+        return path.startswith(self.abspath + fs.sep)
+
 
 TaskRegistry.get().add_task_class(Git)
```

### Comparing `jolt-0.9.9/jolt/plugins/environ.py` & `jolt-0.9.93/jolt/plugins/environ.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 from jolt import filesystem as fs
+from jolt import utils
 from jolt.cache import ArtifactStringAttribute
 from jolt.cache import ArtifactAttributeSet
 from jolt.cache import ArtifactAttributeSetProvider
 
 
 class EnvironmentVariable(ArtifactStringAttribute):
-    def __init__(self, name):
-        super(EnvironmentVariable, self).__init__(name)
+    def __init__(self, artifact, name):
+        super(EnvironmentVariable, self).__init__(artifact, name)
         self._old_value = None
 
     def apply(self, task, artifact):
         self._old_value = task.tools.getenv(self.get_name())
         task.tools.setenv(self.get_name(), self.get_value())
 
     def unapply(self, task, artifact):
         if self._old_value:
             task.tools.setenv(self.get_name(), self._old_value)
         else:
             task.tools.setenv(self.get_name())
         self._old_value = None
 
+    def visit(self, task, artifact, visitor):
+        visitor.setenv(self.get_name(), self.get_value())
+
 
 class PathEnvironmentVariable(EnvironmentVariable):
-    def __init__(self, name="PATH"):
-        super(PathEnvironmentVariable, self).__init__(name)
+    def __init__(self, artifact, name="PATH"):
+        super(PathEnvironmentVariable, self).__init__(artifact, name)
+
+    def set_value(self, value, expand=True):
+        values = utils.as_list(value)
+        super(PathEnvironmentVariable, self).set_value(fs.pathsep.join(values), expand)
 
     def append(self, value):
         if self.get_value():
             self.set_value(self.get_value() + fs.pathsep + value)
         else:
             self.set_value(value)
 
@@ -36,48 +44,51 @@
         paths = self.get_value().split(fs.pathsep)
         paths = [fs.path.join(artifact.path, path) for path in paths]
         new_val = fs.pathsep.join(paths)
         if self._old_value:
             new_val = new_val + fs.pathsep + task.tools.getenv(self.get_name())
         task.tools.setenv(self.get_name(), new_val)
 
+    def visit(self, task, artifact, visitor):
+        paths = self.get_value().split(fs.pathsep)
+        paths = [fs.path.join(artifact.path, path) for path in paths]
+        visitor.setenv(self.get_name(), paths)
+
 
 class EnvironmentVariableSet(ArtifactAttributeSet):
-    def __init__(self):
+    def __init__(self, artifact):
         super(EnvironmentVariableSet, self).__init__()
+        super(ArtifactAttributeSet, self).__setattr__("_artifact", artifact)
 
     def create(self, name):
-        if name == "PATH":
-            return PathEnvironmentVariable(name)
-        if name == "PYTHONPATH":
-            return PathEnvironmentVariable(name)
-        if name == "LD_LIBRARY_PATH":
-            return PathEnvironmentVariable(name)
-        if name == "PKG_CONFIG_PATH":
-            return PathEnvironmentVariable(name)
-        return EnvironmentVariable(name)
+        if "PATH" in name:
+            return PathEnvironmentVariable(self._artifact, name)
+        return EnvironmentVariable(self._artifact, name)
 
 
 @ArtifactAttributeSetProvider.Register
 class EnvironmentVariableSetProvider(ArtifactAttributeSetProvider):
     def create(self, artifact):
-        setattr(artifact, "environ", EnvironmentVariableSet())
+        setattr(artifact, "environ", EnvironmentVariableSet(artifact))
 
     def parse(self, artifact, content):
         if "environ" not in content:
             return
 
         for key, value in content["environ"].items():
-            setattr(artifact.environ, key, value)
+            getattr(artifact.environ, key).set_value(value, expand=False)
 
     def format(self, artifact, content):
         if "environ" not in content:
             content["environ"] = {}
 
-        for key, value in artifact.environ.items():
-            content["environ"][key] = str(value)
+        for key, attrib in artifact.environ.items():
+            content["environ"][key] = attrib.get_value()
 
     def apply(self, task, artifact):
         artifact.environ.apply(task, artifact)
 
     def unapply(self, task, artifact):
         artifact.environ.unapply(task, artifact)
+
+    def visit(self, task, artifact, visitor):
+        artifact.environ.visit(task, artifact, visitor)
```

### Comparing `jolt-0.9.9/jolt/colors.py` & `jolt-0.9.93/jolt/colors.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,24 +2,34 @@
 
 from colorama import Fore, Style
 from jolt import config
 
 
 _tty = sys.stdout.isatty() and sys.stderr.isatty()
 
+
 def enabled():
     return _tty and config.getboolean("jolt", "colors", True)
 
+
 def red(s):
     return Fore.RED + Style.BRIGHT + s + Style.RESET_ALL if enabled() else s
 
+
 def yellow(s):
     return Fore.YELLOW + Style.BRIGHT + s + Style.RESET_ALL if enabled() else s
 
+
 def green(s):
     return Fore.GREEN + Style.BRIGHT + s + Style.RESET_ALL if enabled() else s
 
+
 def blue(s):
     return Fore.BLUE + Style.BRIGHT + s + Style.RESET_ALL if enabled() else s
 
+
 def bright(s):
     return Style.BRIGHT + s + Style.RESET_ALL if enabled() else s
+
+
+def dim(s):
+    return Style.DIM + s + Style.RESET_ALL if enabled() else s
```

### Comparing `jolt-0.9.9/jolt/tools.py` & `jolt-0.9.93/jolt/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,1081 +1,1052 @@
+import atexit
+import click
 import subprocess
-import os
 import sys
-import threading
-if os.name != "nt":
-    import termios
-import glob
-import multiprocessing
-import shutil
-import requests
-import tarfile
-import zipfile
-import bz2file
-from contextlib import contextmanager
-
+import datetime
+import uuid
+import webbrowser
+from os import _exit, environ, getcwd
+
+from jolt.tasks import Task, TaskRegistry, Parameter
+from jolt import scheduler
+from jolt import graph
 from jolt import cache
+from jolt import colors
 from jolt import filesystem as fs
 from jolt import log
-from jolt import utils
+from jolt import __version__
+from jolt.log import logfile
 from jolt import config
-from jolt.error import JoltCommandError
+from jolt.loader import JoltLoader
+from jolt import tools
+from jolt import utils
+from jolt.influence import HashInfluenceRegistry
+from jolt.options import JoltOptions
+from jolt import hooks
+from jolt.manifest import JoltManifest
+from jolt.error import JoltError
+from jolt.error import raise_error
 from jolt.error import raise_error_if
-from jolt.error import raise_task_error, raise_task_error_if
-
-
-def stdout_write(line):
-    sys.stdout.write(line + "\n")
-    sys.stdout.flush()
-
-
-def stderr_write(line):
-    sys.stderr.write(line + "\n")
-    sys.stderr.flush()
-
-
-def _run(cmd, cwd, env, *args, **kwargs):
-    output = kwargs.get("output")
-    output_on_error = kwargs.get("output_on_error")
-    output_rstrip = kwargs.get("output_rstrip", True)
-    output_stdio = kwargs.get("output_stdio", False)
-    output = output if output is not None else True
-    output = False if output_on_error else output
-    shell = kwargs.get("shell", True)
-
-    log.debug("Running: '{0}' (CWD: {1})", cmd, cwd)
-
-    p = subprocess.Popen(
-        cmd,
-        stdin=subprocess.PIPE,
-        stdout=subprocess.PIPE,
-        stderr=subprocess.PIPE,
-        shell=shell,
-        cwd=cwd,
-        env=env)
-
-    class Reader(threading.Thread):
-        def __init__(self, parent, stream, output=None):
-            super(Reader, self).__init__()
-            self.output = output
-            self.parent = parent
-            self.stream = stream
-            self.buffer = []
-            self.start()
+from jolt.error import raise_task_error_if
+from jolt.plugins import report
 
-        def run(self):
-            line = ""
-            try:
-                with log.map_thread(self, self.parent):
-                    for line in iter(self.stream.readline, b''):
-                        if output_rstrip:
-                            line = line.rstrip()
-                        line = line.decode(errors='ignore')
-                        if self.output:
-                            self.output(line)
-                        self.buffer.append(line)
-            except Exception as e:
-                if self.output:
-                    self.output("{0}", str(e))
-                    self.output(line)
-                self.buffer.append(line)
+debug_enabled = False
+workdir = getcwd()
 
-    stdout_func = log.stdout if not output_stdio else stdout_write
-    stderr_func = log.stderr if not output_stdio else stderr_write
 
-    stdout = Reader(threading.current_thread(), p.stdout, output=stdout_func if output else None)
-    stderr = Reader(threading.current_thread(), p.stderr, output=stderr_func if output else None)
-    p.wait()
-    stdout.join()
-    stderr.join()
+class ArgRequiredUnless(click.Argument):
+    def __init__(self, *args, **kwargs):
+        self.required_unless = kwargs.pop('required_unless')
+        assert self.required_unless, "'required_unless' parameter required"
+        super(ArgRequiredUnless, self).__init__(*args, **kwargs)
+
+    def handle_parse_result(self, ctx, opts, args):
+        if self.required_unless not in opts:
+            if not opts.get(self.name, None):
+                self.required = True
+        return super(ArgRequiredUnless, self).handle_parse_result(
+            ctx, opts, args)
+
+
+class PluginGroup(click.Group):
+    def get_command(self, ctx, cmd_name):
+        if cmd_name == "info":
+            cmd_name = "inspect"
+
+        if cmd_name in ["export", "inspect"]:
+            log.set_level(log.SILENCE)
+        elif ctx.params.get("verbose", False):
+            log.set_level(log.VERBOSE)
+        elif ctx.params.get("extra_verbose", False):
+            log.set_level(log.DEBUG)
+
+        config_files = ctx.params.get("config_file") or []
+        for config_file in config_files:
+            log.verbose("Config: {0}", config_file)
+            config.load_or_set(config_file)
+
+        # Load configured plugins
+        JoltLoader.get().load_plugins()
+
+        return click.Group.get_command(self, ctx, cmd_name)
+
+
+@click.group(cls=PluginGroup, invoke_without_command=True)
+@click.version_option(__version__)
+@click.option("-v", "--verbose", is_flag=True, help="Verbose output.")
+@click.option("-vv", "--extra-verbose", is_flag=True, help="Extra verbose output.")
+@click.option("-c", "--config", "config_file", multiple=True, type=str,
+              help="Load a configuration file or set a configuration key.")
+@click.option("-d", "--debugger", is_flag=True,
+              help="Attach debugger on exception.")
+@click.option("-p", "--profile", is_flag=True, hidden=True,
+              help="Profile code while running")
+@click.option("-f", "--force", is_flag=True, default=False, hidden=True,
+              help="Force rebuild of target tasks.")
+@click.option("-s", "--salt", type=str, hidden=True,
+              help="Add salt as task influence.")
+@click.option("-g", "--debug", is_flag=True, default=False, hidden=True,
+              help="Start debug shell before executing task.")
+@click.option("-n", "--network", is_flag=True, default=False, hidden=True,
+              help="Build on network.")
+@click.option("-l", "--local", is_flag=True, default=False, hidden=True,
+              help="Disable all network operations.")
+@click.option("-k", "--keep-going", is_flag=True, default=False, hidden=True,
+              help="Build as many tasks as possible, don't abort on first failure.")
+@click.option("-j", "--jobs", type=int, default=1, hidden=True,
+              help="Number of tasks allowed to execute in parallel (1). ")
+@click.option("-h", "--help", is_flag=True, help="Show this message and exit.")
+@click.pass_context
+def cli(ctx, verbose, extra_verbose, config_file, debugger, profile,
+        force, salt, debug, network, local, keep_going, jobs, help):
+    """
+    A task execution tool.
 
-    if p.returncode != 0 and output_on_error:
-        log.stdout("STDOUT:")
-        for line in stdout.buffer:
-            log.stdout(line)
-        log.stderr("STDERR:\r\n")
-        for line in stderr.buffer:
-            log.stderr(line)
+    When invoked without any commands and arguments, Jolt by default tries
+    to execute and build the artifact of a task called `default`. To build
+    artifacts of other tasks use the build subcommand.
+
+    The Jolt command line interface is hierarchical. One set of options
+    can be passed to the top-level command and a different set of options
+    to the subcommands, simultaneously. For example, verbose output is
+    a top-level option while forced rebuild is a build command option.
+    They may combined like this:
 
-    if p.returncode != 0:
-        raise JoltCommandError(
-            "command failed: {0}".format(
-                " ".join(cmd) if type(cmd) == list else cmd.format(*args, **kwargs)),
-            stdout.buffer, stderr.buffer, p.returncode)
-    return "\n".join(stdout.buffer) if output_rstrip else "".join(stdout.buffer)
+      $ jolt --verbose build --force taskname
 
+    Most build command options are available also at the top-level when
+    build is invoked implicitly for the default task.
 
-class _String(object):
-    def __init__(self, s=None):
-        self._str = s or ''
+    """
 
-    def __enter__(self):
-        return self
+    global debug_enabled
+    debug_enabled = debugger
 
-    def __exit__(self, type, value, tb):
-        pass
+    log.verbose("Jolt command: {}", " ".join([fs.path.basename(sys.argv[0])] + sys.argv[1:]))
+    log.verbose("Jolt host: {}", environ.get("HOSTNAME", "localhost"))
+    log.verbose("Jolt install path: {}", fs.path.dirname(__file__))
+
+    if ctx.invoked_subcommand in ["config"]:
+        # Don't attempt to load any task recipes as they might require
+        # plugins that are not yet configured.
+        return
+
+    if ctx.invoked_subcommand is None:
+        build = ctx.command.get_command(ctx, "build")
+
+    if help:
+        print(ctx.get_help())
+        sys.exit(0)
+
+    manifest = JoltManifest()
+    utils.call_and_catch(manifest.parse)
+    manifest.process_import()
+    ctx.obj["manifest"] = manifest
+
+    if manifest.version:
+        from jolt.version_utils import requirement, version
+        req = requirement(manifest.version)
+        ver = version(__version__)
+        raise_error_if(not req.satisfied(ver),
+                       "This project requires Jolt version {} (running {})",
+                       req, __version__)
+
+    loader = JoltLoader.get()
+    tasks = loader.load()
+    for cls in tasks:
+        TaskRegistry.get().add_task_class(cls)
+
+    if ctx.invoked_subcommand in ["build", "clean"] and loader.joltdir:
+        ctx.obj["workspace_lock"] = utils.LockFile(
+            fs.path.join(loader.joltdir, "build"),
+            log.info, "Workspace is locked by another process, please wait...")
+        atexit.register(ctx.obj["workspace_lock"].close)
+
+    # If no command is given, we default to building the default task.
+    # If the default task doesn't exist, help is printed inside build().
+    if ctx.invoked_subcommand is None:
+        task = config.get("jolt", "default", "default")
+        taskname, _ = utils.parse_task_name(task)
+        if TaskRegistry.get().get_task_class(taskname) is not None:
+            ctx.invoke(build, task=[task], force=force, salt=salt, debug=debug,
+                       network=network, local=local, keep_going=keep_going, jobs=jobs)
+        else:
+            print(cli.get_help(ctx))
+            sys.exit(1)
 
-    def __str__(self):
-        return self._str
 
-    def __get__(self):
-        return self._str
+def _autocomplete_tasks(ctx, args, incomplete):
+    manifest = JoltManifest()
+    utils.call_and_catch(manifest.parse)
+    manifest.process_import()
+
+    tasks = JoltLoader.get().load()
+    tasks = [task.name for task in tasks if task.name.startswith(incomplete or '')]
+    return sorted(tasks)
+
+
+@cli.command()
+@click.argument("task", type=str, nargs=-1, shell_complete=_autocomplete_tasks, cls=ArgRequiredUnless, required_unless="worker")
+@click.option("-c", "--copy", type=click.Path(),
+              help="Copy artifact content to directory PATH.")
+@click.option("-d", "--default", type=str, multiple=True, help="Override default parameter values.", metavar="DEFAULT")
+@click.option("-f", "--force", is_flag=True, default=False, help="Force rebuild of TASK artifact.")
+@click.option("-g", "--debug", is_flag=True, default=False,
+              help="Start debug shell before executing TASK.")
+@click.option("-j", "--jobs", type=int, default=1, help="Number of tasks allowed to execute in parallel [1]. ", metavar="JOBS")
+@click.option("-k", "--keep-going", is_flag=True, default=False, help="Build as many task artifacts as possible.")
+@click.option("-l", "--local", is_flag=True, default=False, help="Disable remote cache access.")
+@click.option("-n", "--network", is_flag=True, default=False, help="Distribute tasks to network workers.")
+@click.option("-s", "--salt", type=str, help="Add salt as hash influence for all tasks in dependency tree.", metavar="SALT")
+@click.option("--result", type=click.Path(), hidden=True,
+              help="Write result manifest to this file.")
+@click.option("--no-download", is_flag=True, default=False,
+              help="Don't download artifacts from remote storage")
+@click.option("--no-upload", is_flag=True, default=False,
+              help="Don't upload artifacts to remote storage")
+@click.option("--download", is_flag=True, default=False,
+              help="Do download artifacts from remote storage")
+@click.option("--upload", is_flag=True, default=False,
+              help="Do upload artifacts to remote storage")
+@click.option("--no-prune", is_flag=True, default=False,
+              help="Don't prune cached artifacts from the build graph. This option can be used to populate the local cache with remotely cached dependency artifacts.")
+@click.option("--worker", is_flag=True, default=False,
+              help="Run with the worker build strategy", hidden=True)
+@click.pass_context
+@hooks.cli_build
+def build(ctx, task, network, keep_going, default, local,
+          no_download, no_upload, download, upload, worker, force,
+          salt, copy, debug, result, jobs, no_prune):
+    """
+    Build task artifact.
 
-    def __add__(self, s):
-        return self._str + s
+    TASK is the name of the task to execute. It is optionally followed by a colon and
+    parameter value assignments. Assignments are separated by commas. Example:
 
-    def __iadd__(self, s):
-        self._str += s
-        return self
+       taskname:param1=value1,param2=value2
 
-    def endswith(self, substr):
-        return self._str.endswith(substr)
+    Default parameter values can be overridden for any task in the dependency tree
+    with --default. DEFAULT is a qualified task name, just like TASK, but parameter
+    assignments change default values.
+
+    By default, a task is executed locally and the resulting artifact is stored
+    in the local artifact cache. If an artifact is already available in the cache,
+    no execution takes place. Artifacts are identified with a hash digest,
+    constructed from hashing task attributes.
+
+    When remote cache providers are configured, artifacts may be downloaded from and/or
+    uploaded to the remote cache as execution progresses. Several options exist to control
+    the behavior, such as --local which disables all remote caches.
+
+    Distributed task execution is enabled by passing the --network option. Tasks are then
+    distributed to and executed by a pool of workers, if one has been configured.
+
+    Rebuilds can be forced with either --force or --salt. --force rebuilds the requested
+    task, but not its dependencies. --salt affects the entire dependency tree. Both add
+    an extra attribute to the task hash calculation in order to taint the identity and
+    induce a cache miss. In both cases, existing intermediate files in build directories
+    are removed before execution starts.
 
-    def startswith(self, substr):
-        return self._str.startswith(substr)
+    """
+    raise_error_if(network and local,
+                   "The -n and -l flags are mutually exclusive")
 
+    raise_error_if(network and debug,
+                   "The -g and -n flags are mutually exclusive")
 
-class _tmpdir(object):
-    def __init__(self, name, cwd=None):
-        self._name = name
-        self._path = None
-        self._cwd = cwd or os.getcwd()
+    raise_error_if(no_download and download,
+                   "The --download and --no-download flags are mutually exclusive")
 
-    def __enter__(self):
+    raise_error_if(no_upload and upload,
+                   "The --upload and --no-upload flags are mutually exclusive")
+
+    duration = utils.duration()
+
+    task = list(task)
+    task = [utils.stable_task_name(t) for t in task]
+
+    if network:
+        _download = config.getboolean("network", "download", True)
+        _upload = config.getboolean("network", "upload", True)
+    else:
+        _download = config.getboolean("jolt", "download", True)
+        _upload = config.getboolean("jolt", "upload", True)
+
+    if local:
+        _download = False
+        _upload = False
+    else:
+        if no_download:
+            _download = False
+        if no_upload:
+            _upload = False
+        if download:
+            _download = True
+        if upload:
+            _upload = True
+
+    options = JoltOptions(network=network,
+                          local=local,
+                          download=_download,
+                          upload=_upload,
+                          keep_going=keep_going,
+                          default=default,
+                          worker=worker,
+                          debug=debug,
+                          salt=salt,
+                          jobs=jobs)
+
+    acache = cache.ArtifactCache.get(options)
+
+    executors = scheduler.ExecutorRegistry.get(options)
+    if worker:
+        log.set_worker()
+        log.verbose("Local build as a worker")
+        strategy = scheduler.WorkerStrategy(executors, acache)
+    elif network:
+        log.verbose("Distributed build as a user")
+        strategy = scheduler.DistributedStrategy(executors, acache)
+    else:
+        log.verbose("Local build as a user")
+        strategy = scheduler.LocalStrategy(executors, acache)
+
+    hooks.TaskHookRegistry.get(options)
+    registry = TaskRegistry.get(options)
+
+    for params in default:
+        registry.set_default_parameters(params)
+
+    manifest = ctx.obj["manifest"]
+
+    for mb in manifest.builds:
+        for mt in mb.tasks:
+            task.append(mt.name)
+        for mt in mb.defaults:
+            registry.set_default_parameters(mt.name)
+
+    if force:
+        for goal in task:
+            registry.get_task(goal, manifest=manifest).taint = uuid.uuid4()
+
+    log.info("Started: {}", datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S"))
+
+    gb = graph.GraphBuilder(registry, manifest, options, progress=True)
+    dag = gb.build(task)
+
+    if not no_prune:
+        gp = graph.GraphPruner(strategy)
+        dag = gp.prune(dag)
+
+    goal_tasks = dag.goals
+    goal_task_duration = 0
+
+    queue = scheduler.TaskQueue(strategy)
+
+    try:
+        if not dag.has_tasks():
+            return
+
+        progress = log.progress(
+            "Progress",
+            dag.number_of_tasks(filterfn=lambda t: not t.is_resource()),
+            " tasks",
+            estimates=False,
+            debug=debug)
+
+        with progress:
+            while dag.has_tasks() or not queue.empty():
+                # Find all tasks ready to be executed
+                leafs = dag.select(lambda graph, task: task.is_ready())
+
+                # Order the tasks by their weights to improve build times
+                leafs.sort(key=lambda x: x.weight)
+
+                while leafs:
+                    task = leafs.pop()
+                    queue.submit(acache, task)
+
+                task, error = queue.wait()
+
+                if not task:
+                    dag.debug()
+                    break
+                elif task.is_goal() and task.duration_running:
+                    goal_task_duration += task.duration_running.seconds
+
+                if not task.is_resource():
+                    if no_prune and task.task.unpack.__func__ is not Task.unpack:
+                        with acache.get_context(task):
+                            pass
+
+                    progress.update(1)
+
+                if not keep_going and error is not None:
+                    queue.abort()
+                    raise error
+
+        if dag.failed:
+            log.error("List of failed tasks")
+            for failed in dag.failed:
+                log.error("- {}", failed.log_name.strip("()"))
+            raise_error("No more tasks could be executed")
+
+        for goal in goal_tasks:
+            if acache.is_available_locally(goal):
+                with acache.get_artifact(goal) as artifact:
+                    log.info("Location: {0}", artifact.path)
+                    if copy:
+                        artifact.copy("*", utils.as_dirpath(fs.path.join(workdir, click.format_filename(copy))), symlinks=True)
+    except KeyboardInterrupt:
+        print()
+        log.warning("Interrupted by user")
         try:
-            dirname = self._cwd
-            fs.makedirs(fs.path.join(dirname, fs.path.dirname(self._name)))
-            self._path = fs.mkdtemp(prefix=self._name + "-", dir=dirname)
-        except KeyboardInterrupt as e:
-            raise e
-        except:
-            raise
-        raise_error_if(not self._path, "failed to create temporary directory")
-        return self
-
-    def __exit__(self, type, value, tb):
-        if self._path:
-            fs.rmtree(self._path, ignore_errors=True)
-
-    @property
-    def path(self):
-        return self.get_path()
-
-    def get_path(self):
-        return self._path
-
-
-class _CMake(object):
-    def __init__(self, deps, tools):
-        self.deps = deps
-        self.tools = tools
-        self.builddir = self.tools.builddir()
-        self.installdir = self.tools.builddir("install")
-
-    def configure(self, sourcedir, *args, **kwargs):
-        sourcedir = self.tools.expand_path(sourcedir)
-
-        extra_args = ["-D{0}={1}".format(key, self.tools.expand(val))
-                      for key, val in kwargs.items()]
-        extra_args = " ".join(extra_args)
-
-        with self.tools.cwd(self.builddir):
-            self.tools.run("cmake {0} -DCMAKE_INSTALL_PREFIX={1} {2}",
-                           sourcedir, self.installdir, extra_args,
-                           output=True)
+            queue.abort()
+            sys.exit(1)
+        except KeyboardInterrupt:
+            print()
+            log.warning("Interrupted again, exiting")
+            _exit(1)
+    finally:
+        log.info("Ended: {}", datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S"))
+        log.info("Total execution time: {0} {1}",
+                 str(duration),
+                 str(queue.duration_acc) if network else '')
+        if result:
+            with report.update() as manifest:
+                manifest.duration = str(goal_task_duration)
+                manifest.write(result)
+
+
+@cli.command()
+@click.argument("task", type=str, nargs=-1, required=False, shell_complete=_autocomplete_tasks)
+@click.option("-d", "--deps", is_flag=True, help="Clean all task dependencies.")
+@click.option("-e", "--expired", is_flag=True, help="Only clean expired tasks.")
+@click.pass_context
+@hooks.cli_clean
+def clean(ctx, task, deps, expired):
+    """
+    Delete task artifacts and intermediate files.
 
-    def build(self, release=True, *args, **kwargs):
-        threading_args = ''
+    When run without arguments, this command removes all task artifacts
+    from the local cache, but no intermediate files are removed.
+
+    When TASK is specified, the task clean() method is invoked to remove
+    any intermediate files still present in persistent build directories.
+    Secondly, the task artifact will be removed from the local cache.
+    Global caches are not affected. The --deps parameter can be used to also
+    clean all dependencies of the specified TASK.
+
+    By default, task artifacts are removed without considering any
+    artifact expiration metadata. To only remove artifact which have expired,
+    use the --expired parameter. Artifacts typically expire immediately after
+    creation unless explicitly configured not to.
+    """
+    acache = cache.ArtifactCache.get()
+    if task:
+        task = [utils.stable_task_name(t) for t in task]
+        registry = TaskRegistry.get()
+        dag = graph.GraphBuilder(registry, ctx.obj["manifest"]).build(task)
+        if deps:
+            tasks = dag.tasks
+        else:
+            tasks = dag.goals
+        for task in tasks:
+            task.clean(acache, expired)
+    else:
+        acache.discard_all(expired, onerror=fs.onerror_warning)
         try:
-            threading_args = ' -j {}'.format(kwargs.get("threads", self.tools.thread_count())) \
-                if "--parallel" in self.tools.run("cmake --help-manual cmake 2>&1", output=False) \
-                   else ''
-        except:
+            # May not be in a workspace when running the command
+            t = tools.Tools()
+            fs.rmtree(t.buildroot, onerror=fs.onerror_warning)
+        except AssertionError:
             pass
 
-        with self.tools.cwd(self.builddir):
-            release = "--config Release" if release else ""
-            self.tools.run("cmake --build . {0}{1}", release, threading_args, output=True)
-
-    def install(self, release=True, *args, **kwargs):
-        with self.tools.cwd(self.builddir):
-            release = "--config Release" if release else ""
-            self.tools.run("cmake --build . --target install {0}", release, output=True)
-
-    def publish(self, artifact, files='*', *args, **kwargs):
-        with self.tools.cwd(self.installdir):
-            artifact.collect(files, *args, **kwargs)
-
-
-class _Meson(object):
-    def __init__(self, deps, tools):
-        self.deps = deps
-        self.tools = tools
-        self.builddir = self.tools.builddir()
-        self.installdir = self.tools.builddir("install")
-
-    def configure(self, sourcedir, *args, **kwargs):
-        sourcedir = self.tools.expand_path(sourcedir)
-        self.tools.run("meson --prefix=/ {0} {1}", sourcedir, self.builddir,
-                       output=True)
-
-    def build(self, *args, **kwargs):
-        self.tools.run("ninja -C {0} ", self.builddir, output=True)
-
-    def install(self, *args, **kwargs):
-        self.tools.run("DESTDIR={0} ninja -C {1} install",
-                       self.installdir, self.builddir,
-                       output=True)
-
-    def publish(self, artifact, files='*', *args, **kwargs):
-        with self.tools.cwd(self.installdir):
-            artifact.collect(files, *args, **kwargs)
-
-
-class _AutoTools(object):
-    def __init__(self, deps, tools):
-        self.deps = deps
-        self.tools = tools
-        self.builddir = self.tools.builddir()
-        self.installdir = self.tools.builddir("install")
-
-    def configure(self, sourcedir, *args, **kwargs):
-        sourcedir = self.tools.expand_path(sourcedir)
-
-        if not fs.path.exists(fs.path.join(sourcedir, "configure")):
-            with self.tools.cwd(sourcedir):
-                self.tools.run("autoreconf -visf", output=True)
-
-        with self.tools.cwd(self.builddir):
-            self.tools.run("{0}/configure --prefix={1} {2}",
-                           sourcedir, self.installdir,
-                           self.tools.getenv("CONFIGURE_FLAGS"),
-                           output=True)
-
-    def build(self, *args, **kwargs):
-        with self.tools.cwd(self.builddir):
-            self.tools.run("make VERBOSE=yes Q= V=1 -j{0}",
-                           self.tools.cpu_count(), output=True)
-
-    def install(self, target="install", **kwargs):
-        with self.tools.cwd(self.builddir):
-            self.tools.run("make {}", target, output=True)
-
-    def publish(self, artifact, files='*', *args, **kwargs):
-        with self.tools.cwd(self.installdir):
-            artifact.collect(files, *args, **kwargs)
-
-
-class Tools(object):
-    """ A collection of useful tools.
-
-    Any {keyword} arguments, or macros, found in strings passed to
-    tool functions are automatically expanded to the value of the
-    associated task's parameters and properties. Relative paths are
-    made absolute by prepending the current working directory.
-    """
-
-    def __init__(self, task=None, cwd=None):
-        self._cwd = cwd or os.getcwd()
-        self._env = {key: value for key, value in os.environ.items()}
-        self._task = task
-        self._builddir = {}
-
-    def __enter__(self):
-        return self
-
-    def __exit__(self, type, value, tb):
-        for dir in self._builddir.values():
-            fs.rmtree(dir, ignore_errors=True)
-        return False
-
-    def append_file(self, pathname, content):
-        """ Appends data at the end of a file.
-
-        Args:
-            pathname (str): Path to file. The file must exist.
-            content (str): Data to be appended at the end of the file.
-        """
-
-        pathname = self.expand_path(pathname)
-        content = self.expand(content)
-        with open(pathname, "ab") as f:
-            f.write(content.encode())
-
-    def archive(self, pathname, filename):
-        """ Creates a (compressed) archive.
-
-        The type of archive to create is determined by the filename extension.
-        Supported formats are:
-
-        - tar
-        - tar.bz2
-        - tar.gz
-        - tar.xz
-        - zip
-
-        Args:
-            pathname (str): Directory path of files to be archived.
-            filename (str): Name/path of created archive.
-        """
-        filename = self.expand_path(filename)
-        pathname = self.expand_path(pathname)
-
-        fmt = None
-        if filename.endswith(".zip"):
-            fmt = "zip"
-            basename = filename[:-4]
-        elif filename.endswith(".tar"):
-            fmt = "tar"
-            basename = filename[:-4]
-        elif filename.endswith(".tar.gz"):
-            if shutil.which("tar") and shutil.which("pigz"):
-                self.run("tar -I pigz -cf {} -C {} .", filename, pathname)
-                return filename
-            fmt = "gztar"
-            basename = filename[:-7]
-        elif filename.endswith(".tgz"):
-            if shutil.which("tar") and shutil.which("pigz"):
-                self.run("tar -I pigz -cf {} -C {} .", filename, pathname)
-                return filename
-            fmt = "gztar"
-            basename = filename[:-4]
-        elif filename.endswith(".tar.bz2"):
-            fmt = "bztar"
-            basename = filename[:-8]
-        elif filename.endswith(".tar.xz"):
-            fmt = "xztar"
-            basename = filename[:-7]
-        raise_task_error_if(
-            not fmt, self._task,
-            "unknown archive type '{0}'", fs.path.basename(filename))
-        try:
-            outfile = shutil.make_archive(basename, fmt, root_dir=pathname)
-            if outfile != filename:
-                shutil.move(outfile, filename)
-            return filename
-        except Exception:
-            raise_task_error(self._task, "failed to create archive from directory '{0}'", pathname)
-
-    def autotools(self, deps=None):
-        """ Creates an AutoTools invokation helper """
-        return _AutoTools(deps, self)
-
-    def builddir(self, name=None, incremental=False, unique=True):
-        """ Creates a temporary build directory.
-
-        The build directory will persist for the duration of a task's
-        execution. It is automatically removed afterwards.
-
-        Args:
-            name (str): Name prefix for the directory. A unique
-                autogenerated suffix will also be appended to the
-                final name.
-            incremental (boolean): If false, the created directory is
-                deleted upon completion of the task.
-
-        Returns:
-            Path to the created directory.
-        """
-        default_name = "builddir" if self._task is None else self._task.canonical_name
-        name = self.expand(name or default_name)
-        name = fs.path.join("build", name)
-
-        if incremental and self._task is not None:
-            if unique:
-                task_hash = utils.sha1(utils.format_task_name(
-                    self._task.name,
-                    self._task._get_parameters()))
-                dirname = fs.path.join(self.getcwd(), "{0}-{1}-{2}".format(
-                    name, self._task.canonical_name, task_hash[:8]))
-            else:
-                dirname = fs.path.join(self.getcwd(), name)
 
-            if self._task.taint is not None:
-                meta = fs.path.join(dirname, ".taint")
-                if not fs.path.exists(meta) or self.read_file(meta) != self._task.taint:
-                    fs.rmtree(dirname, ignore_errors=True)
-                    fs.makedirs(dirname)
-                    self.write_file(meta, self._task.taint)
-            else:
-                fs.makedirs(dirname)
-            return dirname
+@cli.command(name="config")
+@click.option("-l", "--list", is_flag=True,
+              help="List all configuration keys and values.")
+@click.option("-d", "--delete", is_flag=True,
+              help="Delete configuration key.")
+@click.option("-g", "--global", "global_", is_flag=True,
+              help="List, set or get configuration keys in the global config.")
+@click.option("-u", "--user", is_flag=True,
+              help="List, set or get configuration keys in the user config.")
+@click.argument("key", type=str, nargs=1, required=False)
+@click.argument("value", type=str, nargs=1, required=False)
+@click.pass_context
+def _config(ctx, list, delete, global_, user, key, value):
+    """
+    Configure Jolt.
 
-        if name not in self._builddir:
-            dirname = self.getcwd()
-            fs.makedirs(fs.path.join(dirname, fs.path.dirname(name)))
-            self._builddir[name] = fs.mkdtemp(prefix=name+"-", dir=dirname)
-
-        return self._builddir[name]
-
-    def chmod(self, pathname, mode):
-        """ Changes permissions of files and directories.
-
-        Args:
-            pathname (str): Path to a file or directory to change
-                permissions for.
-            mode (int): Requested permission bits.
-        """
-        pathname = self.expand_path(pathname)
-        return os.chmod(pathname, mode)
-
-    def cmake(self, deps=None):
-        """ Creates a CMake invokation helper """
-        return _CMake(deps, self)
-
-    def copy(self, src, dst, symlinks=False):
-        """ Copies file and directories (recursively).
-
-        The directory tree structure is retained when copying directories.
-
-        Args:
-            src (str): Path to a file or directory to be copied.
-            dest (str): Destination path. If the string ends with a
-                path separator a new directory will
-                be created and source files/directories will be copied into
-                the new directory. A destination without trailing path
-                separator can be used to rename single files, one at a time.
-            symlinks (boolean, optional): If True, symlinks are copied.
-                The default is False, i.e. the symlink target is copied.
-        """
-        src = self.expand_path(src)
-        dst = self.expand_path(dst)
-        return fs.copy(src, dst, symlinks=symlinks)
-
-    def cpu_count(self):
-        """ The number of CPUs on the host.
-
-        Returns:
-            int: The number of CPUs on the host.
-        """
-
-        return multiprocessing.cpu_count()
-
-    def thread_count(self):
-        """ Number of threads to use for a task.
-
-        Returns:
-            int: number of threads to use.
-        """
-        threads = config.get("jolt", "threads", self.getenv("JOLT_THREADS", None))
-        return int(threads) if threads else self.cpu_count()
-
-    @contextmanager
-    def cwd(self, pathname, *args):
-        """ Change the current working directory to the specified path.
-
-        This function doesn't change the working directory of the Jolt
-        process. It only changes the working directory for tools within
-        the tools object.
-
-        Args:
-            pathname (str): Path to change to.
-
-        Example:
-
-            .. code-block:: python
-
-                with tools.cwd("subdir") as cwd:
-                    print(cwd)
-        """
-        path = self.expand_path(fs.path.join(pathname, *args))
-        prev = self._cwd
-        try:
-            raise_task_error_if(
-                not fs.path.exists(self._cwd) or not fs.path.isdir(self._cwd),
-                self._task,
-                "failed to change directory to '{0}'", self._cwd)
-            self._cwd = path
-            yield fs.path.normpath(self._cwd)
-        finally:
-            self._cwd = prev
-
-    def download(self, url, pathname, exceptions=False, **kwargs):
-        """ Downloads a file using HTTP.
-
-        Args:
-           url (str): URL to the file to be downloaded.
-           pathname (str): Name/path of destination file.
-           exceptions (boolean): Raise exception if connection fails. Default: false.
-           kwargs (optional): Addidional keyword arguments passed on
-               directly ``requests.get()``.
-
-        """
-        url = self.expand(url)
-        pathname = self.expand_path(pathname)
-        try:
-            response = requests.get(url, stream=True, **kwargs)
-            name = fs.path.basename(pathname)
-            size = int(response.headers.get('content-length', 0))
-            with log.progress("Downloading {0}".format(name), size, "B") as pbar:
-                with open(pathname, 'wb') as out_file:
-                    chunk_size = 4096
-                    for data in response.iter_content(chunk_size=chunk_size):
-                        out_file.write(data)
-                        pbar.update(len(data))
-                actual_size = self.file_size(pathname)
-                raise_error_if(
-                    size != 0 and size != actual_size,
-                    "downloaded file was truncated to {actual_size}/{size} bytes: {name}".format(
-                        actual_size=actual_size, size=size, name=name))
-            if response.status_code not in [200, 404]:
-                log.verbose("Server response {} for {}", response.status_code, url)
-            return response.status_code == 200
-        except KeyboardInterrupt as e:
-            raise e
-        except Exception as e:
-            log.exception()
-            if exceptions:
-                raise e
-            return False
-
-    @contextmanager
-    def environ(self, **kwargs):
-        """ Set/get environment variables.
-
-        Only child processes spawned by the same tools object will be affected
-        by the changed environment.
-
-        The changed environment is only valid within a context and it is
-        restored immediately upon leaving the context.
-
-        Args:
-            kwargs (optinal): A list of keyword arguments assigning values to
-                environment variable.
-
-        Example:
-
-            .. code-block:: python
-
-                with tools.environ(CC="clang"):
-                    tools.run("make all")
-        """
-        for key, value in kwargs.items():
-            kwargs[key] = self.expand(value)
-
-        restore = {key: value for key, value in self._env.items()}
-        self._env.update(kwargs)
-        yield self._env
-        for key, value in kwargs.items():
-            if key not in restore:
-                del self._env[key]
-        self._env.update(restore)
-
-    def expand(self, string, *args, **kwargs):
-        """ Expands keyword arguments/macros in a format string.
-
-        This function is identical to ``str.format()`` but it
-        automatically collects keyword arguments from a task's parameters
-        and properties.
-
-        Args:
-            string (str): The string to be expanded.
-            args (str, optional): Additional positional values required
-                by the format string.
-            kwargs (str, optional): Additional keyword values required by
-                the format string.
-
-        Returns:
-            str: Expanded string.
-
-        Example:
-
-            .. code-block:: python
-
-                target = Parameter(default="all")
-                verbose = "yes"
-
-                def run(self, deps, tools):
-                    print(tools.expand("make {target} VERBOSE={verbose}"))  # "make all VERBOSE=yes"
-
-        """
-        return self._task.expand(string, *args, **kwargs) \
-            if self._task is not None \
-            else utils.expand(string, *args, **kwargs)
-
-    def expand_path(self, pathname, *args, **kwargs):
-        """ Expands keyword arguments/macros in a pathname format string.
-
-        This function is identical to ``str.format()`` but it
-        automatically collects keyword arguments from a task's parameters
-        and properties.
-
-        The function also makes relative paths absolute by prepending the
-        current working directory.
-
-        Args:
-            pathname (str): The pathname to be expanded.
-            args (str, optional): Additional positional values required
-                by the format pathname.
-            kwargs (str, optional): Additional keyword values required by
-                the format pathname.
-
-        Return
-            str: Expanded string.
-        """
-
-        return fs.path.join(self.getcwd(), self.expand(pathname, *args, **kwargs))
-
-    def expand_relpath(self, pathname, relpath, *args, **kwargs):
-        """ Expands keyword arguments/macros in a pathname format string.
-
-        This function is identical to ``str.format()`` but it
-        automatically collects keyword arguments from a task's parameters
-        and properties.
-
-        The function also makes absolute paths relative to a specified
-        directory.
-
-        Args:
-            pathname (str): The pathname to be expanded.
-            relpath (str): Directory to which the returned path will be relative.
-            args (str, optional): Additional positional values required
-                by the format pathname.
-            kwargs (str, optional): Additional keyword values required by
-                the format pathname.
-
-        Return
-            str: Expanded string.
-        """
-
-        pathname = self.expand(pathname, *args, **kwargs)
-        relpath = self.expand(relpath, *args, **kwargs)
-        pathname = fs.path.join(self.getcwd(), pathname)
-        return fs.path.relpath(pathname, relpath)
-
-    def extract(self, filename, pathname, files=None):
-        """ Extracts files in an archive.
-
-        Supported formats are:
-
-        - tar
-        - tar.bz2
-        - tar.gz
-        - tar.xz
-        - zip
-
-        Args:
-            filename (str): Name/path of archive file to be extracted.
-            pathname (str): Destination path for extracted files.
-            files (list, optional): List of files the be extracted
-                from the archive. If not provided, all files are
-                extracted.
-
-        """
-        filename = self.expand_path(filename)
-        filepath = self.expand_path(pathname)
-        try:
-            fs.makedirs(filepath)
-            if filename.endswith(".zip"):
-                with zipfile.ZipFile(filename, 'r') as zip:
-                    if files:
-                        zip.extract(files, filepath)
-                    else:
-                        zip.extractall(filepath)
-            elif filename.endswith(".tar"):
-                with tarfile.open(filename, 'r') as tar:
-                    if files:
-                        tar.extract(files, filepath)
-                    else:
-                        tar.extractall(filepath)
-            elif filename.endswith(".tar.gz") or filename.endswith(".tgz"):
-                if shutil.which("tar") and shutil.which("pigz"):
-                    self.run("tar -I pigz -xf {} -C {} {}", filename, filepath, files or "")
-                    return
-                with tarfile.open(filename, 'r:gz') as tar:
-                    if files:
-                        tar.extract(files, filepath)
-                    else:
-                        tar.extractall(filepath)
-            elif filename.endswith(".tar.bz2"):
-                # bz2file module for multistream support
-                with bz2file.open(filename) as bz2:
-                    with tarfile.open(fileobj=bz2) as tar:
-                        if files:
-                            tar.extract(files, filepath)
-                        else:
-                            tar.extractall(filepath)
-            elif filename.endswith(".tar.xz"):
-                with tarfile.open(filename, 'r:xz') as tar:
-                    if files:
-                        tar.extract(files, filepath)
-                    else:
-                        tar.extractall(filepath)
-            else:
-                raise_task_error(self._task, "unknown archive type '{0}'", fs.path.basename(filename))
-        except Exception:
-            log.exception()
-            raise_task_error(self._task, "failed to extract archive '{0}'", filename)
-
-    def file_size(self, pathname):
-        """ Determines the size of a file.
-
-        Args:
-            pathname (str): Name/path of file for which the size is requested.
-
-        Returns:
-            int: The size of the file in bytes.
-        """
-        pathname = self.expand_path(pathname)
-        try:
-            stat = os.stat(pathname)
-        except KeyboardInterrupt as e:
-            raise e
-        except:
-            raise_task_error(self._task, "file not found '{0}'", pathname)
-        else:
-            return stat.st_size
+    You can query/set/replace/unset configuration keys with this command.
+    Key strings are constructed from the configuration section and the
+    option separated by a dot.
+
+    There are tree different configuration sources:
+
+       - A global configuration file
+
+       - A user configuration file
 
-    def getcwd(self):
-        """ Returns the current working directory. """
-        return fs.path.normpath(self._cwd)
+       - Temporary configuration passed on the command line.
 
-    def getenv(self, key, default=""):
-        """ Returns the value of an environment variable.
+    When reading, the values are read from all configuration sources.
+    The options --global and --user can be used to tell the command to read
+    from only one of the sources. If a configuration key is available from
+    multiple sources, temporary CLI configuration has priority followed by
+    the user configuration file and lastly the global configuration file.
 
-        Only child processes spawned by the same tools object can see
-        the environment variables and their values returned by this method.
-        Don't assume the same variables are set in the Jolt process' environment.
-        """
-        return self._env.get(key, default)
+    When writing, the new values are written to the user configuration by default.
+    The options --global and --user can be used to tell the command to write
+    to only one of the sources.
 
-    def glob(self, pathname):
-        """ Enumerates files and directories.
+    When removing keys, the values are removed from all sources.
+    The options --global and --user can be used to restrict removal to one of
+    the sources.
 
-        Args:
-            pathname (str): A pathname pattern used to match files to be
-                included in the returned list of files and directories.
-                The pattern may contain simple shell-style
-                wildcards such as '*' and '?'. Note: files starting with a
-                dot are not matched by these wildcards.
+    To assign a value to a key:
 
-        Returns:
-            A list of file and directory pathnames. The pathnames are relative
-            to the current working directory unless the ``pathname`` argument
-            was absolute.
+      $ jolt config jolt.default all   # Change name of the default task
 
-        Example:
+    To list existing keys:
 
-            .. code-block:: python
+      $ jolt config -l                 # List all existing keys
 
-                textfiles = tools.glob("*.txt")
-        """
-        path = self.expand_path(pathname)
-        files = utils.as_list(glob.glob(path, recursive=True))
-        if not fs.path.isabs(pathname):
-            files = [file[len(self.getcwd())+1:] for file in files]
-        return files
+      $ jolt config -l -g              # List keys in the global config file
 
-    def map_consecutive(self, callable, iterable):
-        """ Same as ``map()``. """
-        return utils.map_consecutive(callable, iterable)
+      $ jolt config jolt.colors        # Display the value of a key.
 
-    def map_concurrent(self, callable, iterable, max_workers=None):
-        """ Concurrent `~map()`.
+    To delete an existing key:
 
-        Args:
-            callable: A callable object to be executed for each item in
-                the collection.
-            iterable: An iterable collection of items.
-            max_workers (optional): The maximum number of worker threads
-                allowed to be spawned when performing the work. The
-                default is the value returned by
-                :func:`jolt.Tools.cpu_count()`.
+      $ jolt config -d jolt.colors
+
+    To pass temporary configuration:
+
+      $ jolt -c jolt.colors=true config -l
+
+    """
 
-        Returns:
-            list: List of return values.
+    if delete and not key:
+        raise click.UsageError("--delete requires KEY")
 
+    if not key and not list and not key:
+        print(ctx.get_help())
+        sys.exit(1)
+
+    if global_ and user:
+        raise click.UsageError("--global and --user are mutually exclusive")
+
+    alias = None
+
+    if global_:
+        alias = "global"
+    if user:
+        alias = "user"
+
+    def _print_key(section, opt):
+        value = config.get(section, opt, alias=alias)
+        raise_error_if(value is None, "No such key: {}".format(key))
+        print("{} = {}".format(key, value))
+
+    def _print_section(section):
+        print("{}".format(section))
+
+    if list:
+        for section, option, value in config.items(alias):
+            if option:
+                print("{}.{} = {}".format(section, option, value))
+            else:
+                print(section)
+    elif delete:
+        raise_error_if(config.delete(key, alias) <= 0,
+                       "No such key: {}", key)
+        config.save()
+    elif key:
+        section, opt = config.split(key)
+        if value:
+            raise_error_if(opt is None, "Invalid configuration key: {}".format(key))
+            config.set(section, opt, value, alias)
+            try:
+                config.save()
+            except Exception as e:
+                log.exception()
+                raise_error("Failed to write configuration file: {}".format(e))
+        else:
+            if opt:
+                _print_key(section, opt)
+            else:
+                _print_section(section)
 
-        Example:
 
-            .. code-block:: python
+@cli.command()
+@click.argument("task", type=str, nargs=-1, required=False, shell_complete=_autocomplete_tasks)
+@click.option("-c", "--cached", "show_cache", is_flag=True, help="Highlight cache presence with colors.")
+@click.option("-r", "--reverse", type=str, help="Display consumers of REVERSE if TASK is executed.")
+@click.option("-p", "--prune", "prune", is_flag=True, help="Do not repeat tasks. An already visited task's name is printed inside [square brackets] and its deps are omitted.")
+@click.pass_context
+def display(ctx, task, reverse=None, show_cache=False, prune=False):
+    """
+    Display a task and its dependencies visually.
 
-                def compile(self, srcfile):
-                    objfile = srcfile + ".o"
-                    tools.run("gcc -c {0} -o {1}", srcfile, objfile)
-                    return objfile
+    """
+    registry = TaskRegistry.get()
+    gb = graph.GraphBuilder(registry, ctx.obj["manifest"])
+    dag = gb.build(task, influence=show_cache)
+
+    options = JoltOptions()
+    acache = cache.ArtifactCache.get(options)
+
+    if reverse:
+        def iterator(task):
+            return list(dag.predecessors(task))
+        reverse = utils.as_list(reverse)
+        tasklist = dag.select(
+            lambda graph, node:
+            node.short_qualified_name in reverse or node.qualified_name in reverse)
+    else:
+        def iterator(task):
+            return task.children
+        tasklist = dag.requested_goals
+
+    if dag.has_tasks():
+        processed = set()
+
+        def _display(task, indent=0, last=None):
+            header = ""
+            if indent > 0:
+                for pipe in last[:-1]:
+                    if pipe:
+                        header += "\u2502 "
+                    else:
+                        header += "  "
+                if last[-1]:
+                    header += "\u251c\u2574"
+                else:
+                    header += "\u2514\u2574"
+
+            if not show_cache:
+                colorize = str
+            elif task.is_cacheable() and not acache.is_available(task):
+                colorize = colors.red
+            else:
+                colorize = colors.green
 
-                srcfiles = ["test.c", "main.c"]
-                objfiles = tools.map_concurrent(compile, srcfiles)
+            if prune and task.short_qualified_name in processed:
+                def prune_marker(n):
+                    return "[" + n + "]"
+            else:
+                def prune_marker(n):
+                    return n
 
-        """
-        return utils.map_concurrent(callable, iterable, max_workers)
+            print(header + colorize(prune_marker(task.short_qualified_name)))
+            children = iterator(task)
+            if not prune or task.short_qualified_name not in processed:
+                for i in range(0, len(children)):
+                    _display(children[i], indent + 1, last=(last or []) + [i + 1 != len(children)])
+
+            if prune:
+                processed.add(task.short_qualified_name)
+
+        for task in tasklist:
+            _display(task)
+    else:
+        log.info("no tasks to display")
 
-    def meson(self, deps=None):
-        """ Creates a Meson invokation helper """
-        return _Meson(deps, self)
 
-    def replace_in_file(self, pathname, search, replace):
-        """ Replaces all occurrences of a substring in a file.
+@cli.command()
+def docs():
+    """
+    Opens the Jolt documentation in the default webbrowser.
+    """
+    webbrowser.open(config.get("jolt", "docs", "http://jolt.readthedocs.io/"))
 
-        Args:
-            pathname (str): Name/path of file to modify.
-            search (str): Substring to be replaced.
-            replace (str): Replacement substring.
 
-        Example:
+@cli.command()
+@click.argument("task", type=str, nargs=-1, required=True, shell_complete=_autocomplete_tasks)
+@click.option("-c", "--copy", type=click.Path(),
+              help="Copy artifact content to directory PATH.")
+@click.option("-ca", "--copy-all", type=click.Path(), help="Copy artifacts, including dependency artifacts, to directory PATH. Implies --deps.")
+@click.option("-d", "--deps", is_flag=True, help="Download dependencies.")
+@click.pass_context
+@hooks.cli_download
+def download(ctx, task, deps, copy, copy_all):
+    """
+    Download task artifacts from remote caches.
 
-            .. code-block:: python
+    No attempt to build the artifact is made if it is not present
+    in configured remote caches.
 
-                version = Parameter(default="1.0")
+    Task dependencies may optionally be downloaded by passing the -d option.
+    """
 
-                def run(self, deps, tools):
-                    tools.replace_in_file("Makefile", "VERSION := 0.9", "VERSION := {version}")
-        """
-        pathname = self.expand_path(pathname)
-        search = self.expand(search)
-        replace = self.expand(replace)
-        try:
-            with open(pathname, "rb") as f:
-                data = f.read()
-            data = data.replace(search.encode(), replace.encode())
-            with open(pathname, "wb") as f:
-                f.write(data)
-        except KeyboardInterrupt as e:
-            raise e
-        except:
-            raise_task_error(self._task, "failed to replace string in file '{0}'", pathname)
-
-    def rmtree(self, pathname, *args, **kwargs):
-        """Removes a directory tree from disk.
-
-        Args:
-            pathname (str): Path to the file or directory to be removed.
-            ignore_errors (boolean, optional): Ignore files that can't be deleted.
-                The default is ``False``.
-
-        """
-        pathname = self.expand_path(pathname, *args, **kwargs)
-        return fs.rmtree(pathname, **kwargs)
-
-    def run(self, cmd, *args, **kwargs):
-        """ Runs a command in a shell interpreter.
-
-        Args:
-            cmd (str): Command format string.
-            args: Positional arguments for the command format string.
-            kwargs: Keyword arguments for the command format string.
-            output (boolean, optional): By default, the executed command's
-                output will be written to the console. Set to ``False`` to
-                disable all output.
-            output_on_error (boolean, optional): If ``True``, no output is
-                written to the console unless the command fails.
-                The default is ``False``.
-            output_rstrip (boolean, optional): By default, output written
-                to stdout is stripped from whitespace at the end of the
-                string. This can be disabled by setting this argument to False.
-            shell (boolean, optional): Use a shell to run the command.
-                Default: True.
-
-        Example:
-
-            .. code-block:: python
-
-                target = Parameter(default="all")
-                verbose = "yes"
-
-                def run(self, deps, tools):
-                    tools.run("make {target} VERBOSE={verbose} JOBS={0}", tools.cpu_count())
-
-        """
-        cmd = self.expand(cmd, *args, **kwargs)
-        stdi, stdo, stde = None, None, None
+    raise_error_if(copy and copy_all, "--copy and --copy-all are mutually exclusive")
+    if copy_all:
+        deps = True
+
+    manifest = ctx.obj["manifest"]
+    options = JoltOptions()
+    acache = cache.ArtifactCache.get(options)
+    hooks.TaskHookRegistry.get(options)
+    executors = scheduler.ExecutorRegistry.get(options)
+    registry = TaskRegistry.get()
+    strategy = scheduler.DownloadStrategy(executors, acache)
+    queue = scheduler.TaskQueue(strategy)
+    gb = graph.GraphBuilder(registry, manifest, options, progress=True)
+    dag = gb.build(task)
+
+    if not deps:
+        for task in dag.tasks:
+            if not task.is_goal():
+                task.pruned()
+
+    all_tasks = dag.tasks
+    goal_tasks = dag.goals
+
+    try:
+        with log.progress("Progress", dag.number_of_tasks(), " tasks", estimates=False, debug=False) as p:
+            while dag.has_tasks() or not queue.empty():
+                leafs = dag.select(lambda graph, task: task.is_ready())
+
+                while leafs:
+                    task = leafs.pop()
+                    queue.submit(acache, task)
+
+                task, error = queue.wait()
+                p.update(1)
+
+        copy_tasks = goal_tasks if not copy_all else all_tasks
+        for goal in copy_tasks:
+            if acache.is_available_locally(goal):
+                with acache.get_artifact(goal) as artifact:
+                    if copy:
+                        log.info("Copying: {0}", artifact.path)
+                        artifact.copy("*", utils.as_dirpath(fs.path.join(workdir, click.format_filename(copy))), symlinks=True)
+                    elif copy_all:
+                        log.info("Copying: {0}", artifact.path)
+                        artifact.copy("*", utils.as_dirpath(fs.path.join(workdir, click.format_filename(copy_all))), symlinks=True)
+                    elif goal.is_goal():
+                        log.info("Location: {0}", artifact.path)
+
+    except KeyboardInterrupt:
+        print()
+        log.warning("Interrupted by user")
         try:
-            stdi, stdo, stde = None, None, None
-            try:
-                stdi = termios.tcgetattr(sys.stdin.fileno())
-                stdo = termios.tcgetattr(sys.stdout.fileno())
-                stde = termios.tcgetattr(sys.stderr.fileno())
-            except KeyboardInterrupt as e:
-                raise e
-            except:
-                pass
-            return _run(cmd, self._cwd, self._env, *args, **kwargs)
-        finally:
-            if stdi:
-                termios.tcsetattr(sys.stdin.fileno(), termios.TCSANOW, stdi)
-            if stdo:
-                termios.tcsetattr(sys.stdout.fileno(), termios.TCSANOW, stdo)
-            if stde:
-                termios.tcsetattr(sys.stderr.fileno(), termios.TCSANOW, stde)
-
-    def sandbox(self, artifact, incremental=False):
-        """ Creates a temporary build directory populated with the contents of an artifact.
-
-        Files are copied using rsync.
-
-        Args:
-            artifact (cache.Artifact): A task artifact to be copied
-                into the sandbox.
-            incremental (boolean): If false, the created directory is
-                deleted upon completion of the task.
-
-        Returns:
-            str: Path to the build directory..
-
-        Example:
-
-            .. code-block:: python
-
-              def run(self, deps, tools):
-                 sandbox = tools.sandbox(deps["boost"], incremental=True)
-        """
-
-        raise_error_if(
-            type(artifact) is not cache.Artifact,
-            "non-artifact passed as argument to Tools.sandbox()")
-
-        canon_name = fs.path.basename(fs.path.dirname(artifact.path))
-        sandbox_name = "sandbox-1-{0}-{1}".format(
-            canon_name, utils.sha1(artifact.get_name())[:8])
-        path = self.builddir(sandbox_name, incremental=incremental, unique=False)
-        meta = fs.path.join(self.getcwd(), path, ".artifact")
-
-        if not fs.path.exists(meta) or self.read_file(meta) != artifact.path:
-            if shutil.which("rsync"):
-                self.run("rsync --delete -c -r {0}/ {1}", artifact.path, path, output_on_error=True)
-            else:
-                fs.rmtree(path)
-                fs.copytree(artifact.path, path)
-            self.write_file(meta, artifact.path)
+            queue.abort()
+            sys.exit(1)
+        except KeyboardInterrupt:
+            print()
+            log.warning("Interrupted again, exiting")
+            _exit(1)
+    except Exception as e:
+        log.set_interactive(True)
+        raise e
+
+
+@cli.command(hidden=True)
+@click.argument("task", type=str, nargs=-1, required=True)
+@click.option("-r", "--remove", is_flag=True, help="Remove tasks from existing manifest.")
+@click.option("-d", "--default", type=str, multiple=True, help="Override default parameter values.")
+@click.option("-o", "--output", type=str, default="default.joltxmanifest", help="Manifest filename.")
+@click.pass_context
+def freeze(ctx, task, default, output, remove):
+    """
+    Freeze the identity of a task.
+
+    <WIP>
+    """
+    manifest = ctx.obj["manifest"]
 
-        return path
+    options = JoltOptions(default=default)
+    acache = cache.ArtifactCache.get(options)
+    scheduler.ExecutorRegistry.get(options)
+    registry = TaskRegistry.get()
 
-    def setenv(self, key, value=None):
-        """ Sets or unset an environment variable.
+    for params in default:
+        registry.set_default_parameters(params)
 
-        Only child processes spawned by the same tools object can see
-        the set environment variable and its value.
-        Don't assume the same variable is set in the Jolt process' environment.
+    gb = graph.GraphBuilder(registry, manifest)
+    dag = gb.build(task)
 
-        Args:
-            key (str): Name of variable to set.
-            value (str): Value of the variable or ``None`` to unset it.
+    available_in_cache = [
+        (t.is_available_locally(acache) or (
+            t.is_available_remotely(acache) and acache.download_enabled()), t)
+        for t in dag.tasks if t.is_cacheable()]
 
-        """
-        if value is None:
-            try:
-                del self._env[key]
-            except KeyboardInterrupt as e:
-                raise e
-            except:
-                pass
-        else:
-            self._env[key] = self.expand(value)
+    for available, task in available_in_cache:
+        raise_task_error_if(
+            not remove and not available, task,
+            "Task artifact is not available in any cache, build it first")
 
-    def symlink(self, src, dst, replace=True, relative=True):
-        """ Creates a symbolic link.
+    for task in dag.tasks:
+        if task.is_resource() or not task.is_cacheable():
+            continue
+        manifest_task = manifest.find_task(task)
+        if remove and manifest_task:
+            manifest.remove_task(manifest_task)
+            continue
+        if not remove:
+            if not manifest_task:
+                manifest_task = manifest.create_task()
+            manifest_task.name = task.qualified_name
+            manifest_task.identity = task.identity
+
+    manifest.write(fs.path.join(JoltLoader.get().joltdir, output))
+
+
+@cli.command(name="list")
+@click.argument("task", type=str, nargs=-1, required=False, shell_complete=_autocomplete_tasks)
+@click.option("-a", "--all", is_flag=True, help="List all direct and indirect dependencies of TASK.")
+@click.option("-r", "--reverse", type=str, help="Only list dependencies of TASK that are also reverse dependencies of REVERSE.", metavar="REVERSE")
+@click.pass_context
+def _list(ctx, task=None, all=False, reverse=None):
+    """
+    List all tasks, or dependencies of a task.
 
-        Args:
-            src (str): Path to target file or directory.
-            dst (str): Name/path of symbolic link.
-            replace (boolean): Replace existing file or link. Default: false.
-            relative (boolean): Create link using relative path to target.
-                Default: false (absolute path).
-        """
-        src = self.expand_path(src) if not relative else self.expand(src)
-        dst = self.expand_path(dst)
-        if replace and fs.path.lexists(dst):
-            self.unlink(dst)
-        fs.symlink(src, dst)
+    By default, when no TASK is specified, all known task names
+    are listed in alphabetical order.
 
-    def tmpdir(self, name):
-        """ Creates a temporary directory.
+    When a TASK is specified, only direct dependencies of that task
+    are listed. Use -a to also list its indirect dependencies.
 
-        The directory is only valid within a context and it is removed
-        immediately upon leaving the context.
+    Multiple TASK names are allowed.
+    """
 
-        Args:
-            name (str): Name prefix for the directory. A unique
-                autogenerated suffix will also be appended to the
-                final name.
+    raise_error_if(not task and reverse, "TASK required with --reverse")
 
-        Example:
+    registry = TaskRegistry.get()
 
-            .. code-block:: python
+    if not task:
+        classes = registry.get_task_classes()
+        for task in sorted(classes, key=lambda x: x.name):
+            if task.name:
+                print(task.name)
+        return
+
+    task = [utils.stable_task_name(t) for t in task]
+    reverse = [utils.stable_task_name(t) for t in utils.as_list(reverse or [])]
+
+    try:
+        dag = graph.GraphBuilder(registry, ctx.obj["manifest"]).build(task, influence=False)
+    except JoltError as e:
+        raise e
+    except Exception:
+        raise_error("An exception occurred during task dependency evaluation, see log for details")
+
+    task = reverse or task
+    nodes = dag.select(
+        lambda graph, node:
+        node.short_qualified_name in task or node.qualified_name in task)
+    nodes = list(nodes)
+    iterator = dag.predecessors if reverse else dag.successors
+
+    tasklist = set()
+    while nodes:
+        node = nodes.pop()
+        for task in iterator(node):
+            if all and task.short_qualified_name not in tasklist:
+                new_node = dag.get_task(task.qualified_name)
+                nodes.append(new_node)
+            tasklist.add(task.short_qualified_name)
+
+    for task in sorted(list(tasklist)):
+        print(task)
+
+
+@cli.command(name="log")
+@click.option("-f", "--follow", is_flag=True, help="Display log output as it appears")
+@click.option("-d", "--delete", is_flag=True, help="Delete the log file")
+def _log(follow, delete):
+    """
+    Display the Jolt log file.
 
-                with tools.tmpdir("temp") as tmp, tools.cwd(tmp.path):
-                    tools.write_file("tempfile", "tempdata")
+    """
+    if follow:
+        subprocess.call("tail -f {0}".format(logfile), shell=True)
+    elif delete:
+        fs.unlink(logfile)
+    else:
+        t = tools.Tools()
+        configured_pager = config.get("jolt", "pager", environ.get("PAGER", None))
+        for pager in [configured_pager, "less", "more", "cat"]:
+            if pager and t.which(pager):
+                return subprocess.call("{1} {0}".format(logfile, pager), shell=True)
+        print(t.read_file(logfile))
+
+
+@cli.command()
+@click.argument("task", shell_complete=_autocomplete_tasks)
+@click.option("-i", "--influence", is_flag=True, help="Print influence attributes and values.")
+@click.option("-a", "--artifact", is_flag=True, help="Print artifact cache status.")
+@click.option("-s", "--salt", type=str, help="Add salt as task influence.", metavar="SALT")
+@click.pass_context
+def inspect(ctx, task, influence=False, artifact=False, salt=None):
+    """
+    View information about a task.
 
-        """
-        return _tmpdir(name, cwd=self._cwd)
+    This command displays information about a task, such as its class
+    documentation, parameters and their accepted values, requirements,
+    task class origin (file/line), influence attributes, artifact identity,
+    cache status, and more. Default parameter values, if any, are highlighted.
 
-    def unlink(self, pathname, *args, **kwargs):
-        """Removes a file from disk.
+    """
+    task_name = task
+    task_cls_name, task_params = utils.parse_task_name(task_name)
+    task_registry = TaskRegistry.get()
+    task = task_registry.get_task_class(task_cls_name)
+    raise_task_error_if(not task, task_name, "No such task")
+
+    from jolt import inspection
+
+    print()
+    print("  {0}".format(task.name))
+    print()
+    if task.__doc__:
+        print("  {0}".format(task.__doc__.strip()))
+        print()
+    print("  Parameters")
+    has_param = False
+    params = {key: getattr(task, key) for key in dir(task)
+              if isinstance(utils.getattr_safe(task, key), Parameter)}
+    for item, param in params.items():
+        has_param = True
+        print("    {0:<15}   {1}".format(item, param.help or ""))
+    if not has_param:
+        print("    None")
+
+    print()
+    print("  Definition")
+    print("    {0:<15}   {1} ({2})".format(
+        "File", fs.path.relpath(inspection.getfile(task), JoltLoader.get().joltdir),
+        inspection.getlineno(task)))
+
+    print()
+    print("  Requirements")
+    manifest = ctx.obj["manifest"]
+    try:
+        task = task_registry.get_task(task_name, manifest=manifest)
+        for req in sorted(utils.as_list(utils.call_or_return(task, task.requires))):
+            print("    {0}".format(task.tools.expand(req)))
+        if not task.requires:
+            print("    None")
+        print()
+    except Exception as e:
+        log.exception()
+        if "has not been set" in str(e):
+            print("    Unavailable (parameters must be set)")
+            print()
+            return
+        print("    Unavailable (exception during evaluation)")
+        print()
+        return
+
+    if salt:
+        task.taint = salt
+
+    if artifact:
+        acache = cache.ArtifactCache.get()
+        builder = graph.GraphBuilder(task_registry, manifest)
+        dag = builder.build([task.qualified_name])
+        tasks = dag.select(lambda graph, node: node.task is task)
+        assert len(tasks) == 1, "graph produced multiple tasks, one expected"
+        proxy = tasks[0]
+        task = proxy.task
+
+        print("  Cache")
+        print("    Identity          {0}".format(proxy.identity))
+        if acache.is_available_locally(proxy):
+            with acache.get_artifact(proxy) as artifact:
+                print("    Location          {0}".format(artifact.path))
+            print("    Local             True ({0})".format(
+                utils.as_human_size(acache.get_artifact(proxy).get_size())))
+        else:
+            print("    Local             False")
+        print("    Remote            {0}".format(acache.is_available_remotely(proxy)))
+        print()
+
+    if influence:
+        print("  Influence")
+        for string in HashInfluenceRegistry.get().get_strings(task):
+            string = string.split(":", 1)
+            print("    {:<18}{}".format(string[0][10:], string[1].strip()))
 
-        To remove directories, use :func:`~jolt.Tools.rmtree`.
 
-        Args:
-            pathname (str): Path to the file to be removed.
+@cli.command()
+@click.argument("task", type=str, nargs=-1, required=True, shell_complete=_autocomplete_tasks)
+@click.pass_context
+def export(ctx, task):
+    """
+    Export task artifact metadata into shell environment.
 
-        """
-        pathname = self.expand_path(pathname, *args, **kwargs)
-        return fs.unlink(pathname)
+    When running the command, a shell script is printed to stdout.
+    It can be redirected to a file and executed separately, or sourced
+    directly in the shell by running:
 
-    def upload(self, pathname, url, exceptions=False, auth=None, **kwargs):
-        """ Uploads a file using HTTP (PUT).
+      source <(jolt export <task>)
 
-        Args:
-           pathname (str): Name/path of file to be uploaded.
-           url (str): Destination URL.
-           exceptions (boolean): Raise exception if connection fails. Default: false.
-           auth (requests.auth.AuthBase, optional): Authentication helper.
-               See requests.auth for details.
-           kwargs (optional): Addidional keyword arguments passed on
-               directly to `~requests.put()`.
+    The script creates a virtual environment that is identical
+    to the environment that would be setup when the specified task
+    artifact is consumed by another task. This enables packaged
+    applications, such as compilers, to be run directly from the shell.
 
-        """
+    The command will fail if the task artifact or any dependency
+    artifact is missing in the local cache. Build the task to
+    populate the cache and then try again.
 
-        pathname = self.expand_path(pathname)
-        try:
-            name = fs.path.basename(pathname)
-            size = self.file_size(pathname)
-            with log.progress("Uploading " + name, size, "B") as pbar, \
-                 open(pathname, 'rb') as fileobj:
-                def read():
-                    data = fileobj.read(4096)
-                    pbar.update(len(data))
-                    return data
-                response = requests.put(url, data=iter(read, b''), auth=auth, **kwargs)
-                if response.status_code not in [201, 204]:
-                    log.verbose("Server response {} for {}", response.status_code, url)
-                return response.status_code in [201, 204]
-        except KeyboardInterrupt as e:
-            raise e
-        except Exception as e:
-            log.exception()
-            if exceptions:
-                raise e
-        return False
-
-    def read_file(self, pathname, binary=False):
-        """ Reads a file. """
-        pathname = self.expand_path(pathname)
-        with open(pathname, "rb" if binary else "r") as f:
-            return f.read()
-
-    def which(self, executable):
-        """ Find executable in PATH.
-
-        Args:
-            executable (str): Name of executable to be found.
-
-        Returns:
-            str: Full path to the executable.
-        """
-        executable = self.expand(executable)
-        return shutil.which(executable, path=self._env.get("PATH"))
-
-    def write_file(self, pathname, content=None):
-        """ Creates a file.
-
-        Note:
-            Existing files are overwritten.
-
-        Args:
-            pathname (str): Name/path of file to be created.
-            content (str, optional): Data to be written to the file.
-        """
-        pathname = self.expand_path(pathname)
-        content = self.expand(content) if content is not None else ''
-        with open(pathname, "wb") as f:
-            f.write(content.encode())
+    Run ``deactivate-jolt`` to leave the virtual environment. All
+    environment variables will be restored to their original values.
+    """
+    try:
+        _export(ctx, task)
+    finally:
+        log.set_level(log.INFO)
+
+
+def _export(ctx, task):
+    acache = cache.ArtifactCache.get()
+    task = [utils.stable_task_name(t) for t in task]
+    registry = TaskRegistry.get()
+    executors = scheduler.ExecutorRegistry.get()
+    strategy = scheduler.LocalStrategy(executors, acache)
+
+    dag = graph.GraphBuilder(registry, ctx.obj["manifest"])
+    dag = dag.build(task)
+
+    gp = graph.GraphPruner(strategy)
+    dag = gp.prune(dag)
+
+    class Export(object):
+        def __init__(self):
+            self.environ = {}
+            self.prepend_environ = {}
+
+        def setenv(self, name, value):
+            self.environ[name] = value
+
+    class Context(object):
+        def __init__(self, tasks):
+            self.tasks = tasks
+            self.environ = set()
+            self.exports = {}
+
+        def add_export(self, task, visitor):
+            self.exports[task] = visitor
+            self.environ.update(set(visitor.environ.keys()))
+
+    tasks = list(filter(lambda t: t.is_cacheable(), reversed(dag.topological_nodes)))
+    context = Context(tasks)
+
+    for task in context.tasks:
+        artifact = acache.get_artifact(task)
+        raise_task_error_if(
+            artifact.is_temporary(), task,
+            "Task artifact not found in local cache, build it first")
+
+        visitor = Export()
+        cache.visit_artifact(task, artifact, visitor)
+        context.add_export(task, visitor)
+
+    script = utils.render(
+        "export.sh.template",
+        ctx=context)
+
+    print(script)
```

### Comparing `jolt-0.9.9/jolt/__init__.py` & `jolt-0.9.93/jolt/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,63 @@
-name = "jolt"
-
 from .tasks import Alias
+from .tasks import BooleanParameter
+from .tasks import Download
+from .tasks import EnvironExport
+from .tasks import Export
+from .tasks import ListParameter
+from .tasks import MultiTask
+from .tasks import Parameter
+from .tasks import Resource
+from .tasks import Script
 from .tasks import Task
 from .tasks import TaskGenerator
 from .tasks import Test
-from .tasks import Resource
-from .tasks import Export
-from .tasks import Parameter
-from .tasks import BooleanParameter
+from .tasks import attributes
 
 from .cache import Artifact
 from .cache import Context
 
 from .tools import Tools
 
+from .version import __version__
 from . import expires
+from . import influence
+
+__all__ = (
+    "Alias",
+    "Artifact",
+    "BooleanParameter",
+    "Context",
+    "Download",
+    "EnvironExport",
+    "Export",
+    "ListParameter",
+    "MultiTask",
+    "Parameter",
+    "Resource",
+    "Script",
+    "Task",
+    "TaskGenerator",
+    "Test",
+    "Tools",
+    "__version__",
+    "attributes",
+    "expires",
+    "influence",
+)
+
+name = "jolt"
 
 
 def include(joltfile):
     """ Include another Python file """
     try:
         from os import path
         from sys import _getframe
         from jolt.loader import JoltLoader
         filepath = _getframe().f_back.f_code.co_filename
         filepath = path.dirname(filepath)
         filepath = path.join(filepath, joltfile)
         JoltLoader.get()._load_file(filepath)
     except Exception as e:
-        log.exception()
         from jolt.error import raise_error
-        raise_error("failed to load '{0}': {1}", joltfile, str(e))
+        raise_error("Failed to load '{0}': {1}", joltfile, str(e))
```

### Comparing `jolt-0.9.9/jolt/scheduler.py` & `jolt-0.9.93/jolt/scheduler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from concurrent.futures import ThreadPoolExecutor, as_completed, Future
-from functools import partial
+import os
 import queue
-try:
-    import asyncio
-    has_asyncio = True
-except:
-    has_asyncio = False
-
 
+from jolt import config
+from jolt import hooks
 from jolt import log
 from jolt import utils
+from jolt import tools
 from jolt.error import raise_error
+from jolt.error import raise_task_error
 from jolt.error import raise_task_error_if
 from jolt.graph import PruneStrategy
 from jolt.manifest import ManifestExtension
 from jolt.manifest import ManifestExtensionRegistry
 from jolt.options import JoltOptions
 
 
@@ -70,14 +68,17 @@
 
     def is_aborted(self):
         return self._aborted
 
     def in_progress(self, task):
         return task in self.futures.values()
 
+    def empty(self):
+        return len(self.futures) == 0
+
 
 class Executor(object):
     def __init__(self, factory):
         self.factory = factory
 
     def submit(self, env):
         return self.factory.submit(self, env)
@@ -95,29 +96,28 @@
         self.task = task
         self.force_build = force_build
         self.force_upload = force_upload
 
     def run(self, env):
         if self.is_aborted():
             return
-        if has_asyncio:
-            loop = asyncio.SelectorEventLoop()
-            asyncio.set_event_loop(loop)
-
         try:
             self.task.started()
-            self.task.run(
-                env.cache,
-                force_build=self.force_build,
-                force_upload=self.force_upload)
+            hooks.task_started_execution(self.task)
+            with hooks.task_run(self.task):
+                self.task.run(
+                    env.cache,
+                    force_build=self.force_build,
+                    force_upload=self.force_upload)
         except Exception as e:
             log.exception()
             self.task.failed()
             raise e
         else:
+            hooks.task_finished_execution(self.task)
             self.task.finished()
         return self.task
 
 
 class NetworkExecutor(Executor):
     pass
 
@@ -138,23 +138,29 @@
     def __init__(self, factory, task, *args, **kwargs):
         super(Downloader, self).__init__(factory, *args, **kwargs)
         self.task = task
 
     def _download(self, env, task):
         if self.is_aborted():
             return
+        if not task.is_downloadable():
+            return
         try:
             task.started("Download")
+            hooks.task_started_download(task)
             raise_task_error_if(
                 not env.cache.download(task),
-                task, "failed to download task artifact")
+                task, "Failed to download task artifact")
         except Exception as e:
+            with task.task.report() as report:
+                report.add_exception(e)
             task.failed("Download")
             raise e
         else:
+            hooks.task_finished_download(task)
             task.finished("Download")
 
     def run(self, env):
         self._download(env, self.task)
         for ext in self.task.extensions:
             self._download(env, ext)
         return self.task
@@ -166,21 +172,25 @@
         self.task = task
 
     def _upload(self, env, task):
         if self.is_aborted():
             return
         try:
             task.started("Upload")
+            hooks.task_started_upload(task)
             raise_task_error_if(
                 not env.cache.upload(task),
-                task, "failed to upload task artifact")
+                task, "Failed to upload task artifact")
         except Exception as e:
+            with task.task.report() as report:
+                report.add_exception(e)
             task.failed("Upload")
             raise e
         else:
+            hooks.task_finished_upload(task)
             task.finished("Upload")
 
     def run(self, env):
         self._upload(env, self.task)
         for ext in self.task.extensions:
             self._upload(env, ext)
 
@@ -206,29 +216,31 @@
         self._concurrent_factory.shutdown()
 
     def create_skipper(self, task):
         return SkipTask(self._concurrent_factory, task)
 
     def create_downloader(self, task):
         # TODO: Switch to concurrent factory once the progress bar can handle it
-        return Downloader(self._local_factory, task)
+        return Downloader(self._concurrent_factory, task)
 
     def create_uploader(self, task):
         # TODO: Switch to concurrent factory once the progress bar can handle it
-        return Uploader(self._local_factory, task)
+        return Uploader(self._concurrent_factory, task)
 
     def create_local(self, task, force=False):
+        task.set_locally_executed()
         return self._local_factory.create(task, force=force)
 
     def create_network(self, task):
         for factory in self._factories:
             executor = factory.create(task)
             if executor is not None:
+                task.set_remotely_executed()
                 return executor
-        return self._local_factory.create(task)
+        return self.create_local(task)
 
     def get_network_parameters(self, task):
         parameters = {}
         for extension in self._extensions:
             parameters.update(extension.get_parameters(task))
         return parameters
 
@@ -236,15 +248,15 @@
 class NetworkExecutorExtensionFactory(object):
     @staticmethod
     def Register(cls):
         ExecutorRegistry.extension_factories.insert(0, cls)
         return cls
 
     def create(self):
-        raise NotImplemented()
+        raise NotImplementedError()
 
 
 class NetworkExecutorExtension(object):
     def get_parameters(self, task):
         return {}
 
 
@@ -290,15 +302,15 @@
         return self._options.keep_going
 
     def shutdown(self):
         self._aborted = True
         self.pool.shutdown()
 
     def create(self, task):
-        raise NotImplemented()
+        raise NotImplementedError()
 
     def _run(self):
         job = self._queue.get(False)
         self._queue.task_done()
         try:
             if not self.is_aborted():
                 job.executor.run(job.env)
@@ -318,36 +330,44 @@
         self._queue.put(Job(-executor.task.weight, future, executor, env))
         self.pool.submit(self._run)
         return future
 
 
 class LocalExecutorFactory(ExecutorFactory):
     def __init__(self, options=None):
-        super(LocalExecutorFactory, self).__init__(options=options, max_workers=1)
+        max_workers = config.getint(
+            "jolt", "parallel_tasks",
+            os.getenv("JOLT_PARALLEL_TASKS", 1 if options is None else options.jobs))
+        super(LocalExecutorFactory, self).__init__(
+            options=options,
+            max_workers=max_workers)
 
     def create(self, task, force=False):
         return LocalExecutor(self, task, force_build=force)
 
 
 class ConcurrentLocalExecutorFactory(ExecutorFactory):
     def __init__(self, options=None):
-        super(ConcurrentLocalExecutorFactory, self).__init__(options=options)
+        max_workers = tools.Tools().thread_count()
+        super(ConcurrentLocalExecutorFactory, self).__init__(
+            options=options,
+            max_workers=max_workers)
 
     def create(self, task):
         raise NotImplementedError()
 
 
 class NetworkExecutorFactory(ExecutorFactory):
     def __init__(self, *args, **kwargs):
         super(NetworkExecutorFactory, self).__init__(*args, **kwargs)
 
 
 class ExecutionStrategy(object):
     def create_executor(self, task):
-        raise NotImplemented()
+        raise NotImplementedError()
 
 
 class LocalStrategy(ExecutionStrategy, PruneStrategy):
     def __init__(self, executors, cache):
         self.executors = executors
         self.cache = cache
 
@@ -368,106 +388,75 @@
         if task.is_available_locally(self.cache):
             return True
         if self.cache.download_enabled() and task.is_available_remotely(self.cache):
             return True
         return False
 
 
-class CollaborativeDistributedStrategy(ExecutionStrategy, PruneStrategy):
+class DownloadStrategy(ExecutionStrategy, PruneStrategy):
     def __init__(self, executors, cache):
         self.executors = executors
         self.cache = cache
 
     def create_executor(self, task):
-        if task.is_resource():
-            return self.executors.create_local(task)
-
         if task.is_alias():
             return self.executors.create_skipper(task)
-
+        if task.is_resource():
+            return self.executors.create_local(task)
         if not task.is_cacheable():
-            return self.executors.create_network(task)
-
-        # Check remote availability first so that the availability of
-        # remote storage providers is made known when checking if
-        # artifacts can be downloaded or not.
-        remote = task.is_available_remotely(self.cache)
-
-        if not self.cache.download_enabled():
-            if not task.is_available_locally(self.cache):
-                return self.executors.create_local(task)
-            else:
-                return self.executors.create_skipper(task)
-
-        if remote:
-            if not task.is_available_locally(self.cache):
-                return self.executors.create_downloader(task)
-            else:
-                return self.executors.create_skipper(task)
-
+            return self.executors.create_skipper(task)
         if task.is_available_locally(self.cache):
-            if self.cache.upload_enabled():
-                if task.is_uploadable(self.cache):
-                    return self.executors.create_uploader(task)
-                else:
-                    return self.executors.create_network(task)
-            else:
-                return self.executors.create_skipper(task)
-
-        if task.is_fast():
-            if not self.cache.upload_enabled():
-                return self.executors.create_network(task)
-            else:
-                return self.executors.create_local(task)
-
-        return self.executors.create_network(task)
+            return self.executors.create_skipper(task)
+        if self.cache.download_enabled() and task.is_available_remotely(self.cache):
+            return self.executors.create_downloader(task)
+        raise_task_error(task, "Task must be built first")
 
     def should_prune_requirements(self, task):
-        if task.is_alias() or not task.is_cacheable():
-            return False
-        if self.cache.upload_enabled() and task.is_available_locally(self.cache):
-            return True
-        if self.cache.download_enabled() and task.is_available_remotely(self.cache):
-            return True
         return False
 
 
 class DistributedStrategy(ExecutionStrategy, PruneStrategy):
     def __init__(self, executors, cache):
         self.executors = executors
         self.cache = cache
 
     def create_executor(self, task):
         if task.is_alias():
             return self.executors.create_skipper(task)
 
         if task.is_resource():
-            return self.executors.create_local(task)
+            if task.deps_available_locally(self.cache):
+                return self.executors.create_local(task)
+            else:
+                return self.executors.create_skipper(task)
 
         if not task.is_cacheable():
             return self.executors.create_network(task)
 
         if not self.cache.upload_enabled():
             return self.executors.create_network(task)
 
+        if not task.is_goal(with_extensions=False):
+            task.disable_download()
+        for extension in task.extensions:
+            if not extension.is_goal(with_extensions=False):
+                extension.disable_download()
+
         remote = task.is_available_remotely(self.cache)
         if remote:
             if task.is_goal() and self.cache.download_enabled() and \
                not task.is_available_locally(self.cache):
                 return self.executors.create_downloader(task)
             return self.executors.create_skipper(task)
         else:
             if task.is_available_locally(self.cache) and task.is_uploadable(self.cache):
                 return self.executors.create_uploader(task)
-            if task.deps_available_locally(self.cache) and task.is_fast():
+            if task.is_fast() and task.deps_available_locally(self.cache):
                 return self.executors.create_local(task)
 
-        if not task.is_goal():
-            task.disable_download()
-
         return self.executors.create_network(task)
 
     def should_prune_requirements(self, task):
         if task.is_alias() or not task.is_cacheable():
             return False
         if task.is_available_remotely(self.cache):
             return True
@@ -491,15 +480,18 @@
             "artifact upload must be enabled for workers, fix configuration")
 
         if not task.is_cacheable():
             return self.executors.create_local(task)
 
         if task.is_available_locally(self.cache):
             if task.is_goal() and not task.is_available_remotely(self.cache):
-                if task.is_uploadable(self.cache):
+                # Unpacked artifacts may become unpacked before we manage to upload.
+                # To keep the implementation simple we take the easy road and rebuild
+                # all artifacts that have not been unpacked, even if they are uploadable.
+                if task.is_unpacked(self.cache) and task.is_uploadable(self.cache):
                     return self.executors.create_uploader(task)
                 else:
                     return self.executors.create_local(task, force=True)
             return self.executors.create_skipper(task)
 
         if not self.cache.download_enabled():
             return self.executors.create_local(task)
@@ -509,38 +501,59 @@
 
         return self.executors.create_local(task)
 
     def should_prune_requirements(self, task):
         if task.is_alias() or not task.is_cacheable():
             return False
         if task.is_available_locally(self.cache):
-            return True
-        if task.is_available_remotely(self.cache):
+            # Unpacked artifacts may become unpacked before we manage to upload.
+            # To keep the implementation simple we take the easy road and rebuild
+            # all artifacts that have not been unpacked, even if they are uploadable.
+            if task.is_unpacked(self.cache) and task.is_uploadable(self.cache):
+                return True
+        if not task.is_goal() and task.task.selfsustained:
             return True
         return False
 
 
 class TaskIdentityExtension(ManifestExtension):
     def export_manifest(self, manifest, task):
         for child in [task] + task.extensions + task.descendants:
             manifest_task = manifest.find_task(child.qualified_name)
             if manifest_task is None:
                 manifest_task = manifest.create_task()
                 manifest_task.name = child.qualified_name
             manifest_task.identity = child.identity
 
+
 ManifestExtensionRegistry.add(TaskIdentityExtension())
 
 
 class TaskExportExtension(ManifestExtension):
     def export_manifest(self, manifest, task):
-        for child in [task] + task.children:
+        short_task_names = set()
+        for child in [task] + task.extensions + task.descendants:
             manifest_task = manifest.find_task(child.qualified_name)
             if manifest_task is None:
                 manifest_task = manifest.create_task()
                 manifest_task.name = child.qualified_name
             for key, export in child.task._get_export_objects().items():
                 attrib = manifest_task.create_attribute()
                 attrib.name = key
                 attrib.value = export.export(child.task)
+            short_task_names.add(child.name)
+
+        # Figure out if any task with an overridden default parameter
+        # value was included in the manifest. If so, add info about it.
+        default_task_names = set()
+        for task in task.options.default:
+            short_name, _ = utils.parse_task_name(task)
+            if short_name in short_task_names:
+                default_task_names.add(task)
+        if default_task_names:
+            build = manifest.create_build()
+            for task in default_task_names:
+                default = build.create_default()
+                default.name = task
+
 
 ManifestExtensionRegistry.add(TaskExportExtension())
```

### Comparing `jolt-0.9.9/jolt/manifest.py` & `jolt-0.9.93/jolt/manifest.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from xml.dom import minidom
+from xml.etree import ElementTree as ET
 import os
 
-from jolt.xmldom import Attribute, Composition, SubElement, Element, ElementTree, ET
+from jolt.xmldom import Attribute, Composition, SubElement, Element, ElementTree
 from jolt import filesystem as fs
 from jolt import log
 
 
 @Attribute('name')
 @Attribute('value', child=True)
 class _JoltAttribute(SubElement):
@@ -30,31 +31,53 @@
 @Attribute('src')
 @Attribute('joltdir')
 class _JoltProjectRecipe(SubElement):
     def __init__(self, elem=None):
         super(_JoltProjectRecipe, self).__init__('recipe', elem=elem)
 
 
+@Attribute('src')
+class _JoltProjectModule(SubElement):
+    def __init__(self, elem=None):
+        super(_JoltProjectModule, self).__init__('module', elem=elem)
+
+
 @Attribute('name')
 class _JoltProjectResource(SubElement):
     def __init__(self, elem=None):
         super(_JoltProjectResource, self).__init__('resource', elem=elem)
 
 
 @Attribute('name')
 @Composition(_JoltProjectLink, "link")
+@Composition(_JoltProjectModule, "module")
 @Composition(_JoltProjectRecipe, "recipe")
 @Composition(_JoltProjectResource, "resource")
 class _JoltProject(SubElement):
     def __init__(self, elem=None):
         super(_JoltProject, self).__init__('project', elem=elem)
 
+
+@Attribute('type', child=True)
+@Attribute('location', child=True)
+@Attribute('message', child=True)
+@Attribute('details', child=True)
+class _JoltTaskError(SubElement):
+    def __init__(self, elem=None):
+        super(_JoltTaskError, self).__init__('error', elem=elem)
+
+
 @Attribute('name')
+@Attribute('duration', child=True)
+@Attribute('goal', child=True)
 @Attribute('identity', child=True)
+@Attribute('logstash', child=True)
+@Attribute('result', child=True)
 @Composition(_JoltAttribute, "attribute")
+@Composition(_JoltTaskError, "error")
 class _JoltTask(SubElement):
     def __init__(self, elem=None):
         super(_JoltTask, self).__init__('task', elem=elem)
 
 
 @Attribute('name')
 class _JoltDefault(SubElement):
@@ -78,14 +101,15 @@
 
 @Attribute("config", child=True, zlib=True)
 @Attribute("stdout", child=True, zlib=True)
 @Attribute("stderr", child=True, zlib=True)
 @Attribute("result", child=True)
 @Attribute("duration", child=True)
 @Attribute("workspace")
+@Attribute("version")
 @Composition(_JoltRecipe, "recipe")
 @Composition(_JoltTask, "task")
 @Composition(_JoltBuild, "build")
 @Composition(_JoltNetworkParameter, "parameter")
 @Composition(_JoltProject, "project")
 class JoltManifest(ElementTree):
     def __init__(self):
@@ -147,21 +171,34 @@
         self._setroot(root)
         self._elem = root
         return self
 
     def format(self):
         return minidom.parseString(ET.tostring(self.getroot())).toprettyxml(indent="  ")
 
+    def transform(self, xsltfile):
+        from lxml import etree as lxmlET
+        manifest = lxmlET.fromstring(self.format())
+        xslt = lxmlET.parse(xsltfile)
+        transform = lxmlET.XSLT(xslt)
+        document = transform(manifest)
+        return minidom.parseString(lxmlET.tostring(document)).toprettyxml(indent="  ")
+
     def write(self, filename):
         with open(filename, 'w') as f:
             f.write(self.format())
 
     def has_task(self, task):
         return self.find("./task[@identity='{}']".format(task.identity)) is not None
 
+    def has_failure(self):
+        if self.result and self.result == "FAILED":
+            return True
+        return self.find("./task[result='FAILED']") is not None
+
     def find_task(self, task):
         match = self.find("./task[@name='{0}']".format(task))
         if match is None:
             return None
         return _JoltTask(elem=match)
 
     def get_parameter(self, key):
```

### Comparing `jolt-0.9.9/jolt/influence.py` & `jolt-0.9.93/jolt/influence.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import datetime
 import hashlib
 import os
-import uuid
-
+from pathlib import Path, PurePath
 
+from jolt import inspection
 from jolt import utils
-from jolt import log
 from jolt import filesystem as fs
 from jolt import tools
+from jolt import version
 
 
 _providers = []
 
+
 @utils.Singleton
 class HashInfluenceRegistry(object):
     @staticmethod
     def Register(cls):
         _providers.append(cls)
 
     def __init__(self):
@@ -23,28 +24,28 @@
 
     def register(self, provider):
         self._providers.append(provider)
 
     def apply_all(self, task, sha):
         for influence in self.get_strings(task):
             sha.update(influence.encode())
-            log.debug("{0}: {1}", task.name, influence)
 
     def get_strings(self, task):
         content = []
         for provider in self._providers + task.influence:
             for line in str(provider.get_influence(task)).splitlines():
                 content.append("Influence-{0}: {1}".format(provider.name, line))
         return content
 
 
 class HashInfluenceProvider(object):
     name = "X"
+
     def get_influence(self, task):
-        raise NotImplemented()
+        raise NotImplementedError()
 
 
 class TaintInfluenceProvider(object):
     name = "Taint"
 
     def get_influence(self, task):
         return str(task.taint)
@@ -53,61 +54,120 @@
 class TaskAttributeInfluence(HashInfluenceProvider):
     def __init__(self, attrib, sort=False):
         self._attrib = attrib
         self._sort = sort
         self.name = attrib.title()
 
     def get_influence(self, task):
-        value = utils.getattr_safe(task, tools.Tools(task).expand(self._attrib), "N/A")
+        value = getattr(task, tools.Tools(task).expand(self._attrib), "N/A")
         try:
             value = value.__get__(task)
             if type(value) == list and self._sort:
                 value.sort()
         except AttributeError:
             pass
         return value
 
 
-def attribute(name, sort=False):
+def attribute(name, type=None, sort=False):
     """ Add task attribute value as hash influence.
 
     Args:
         name (str): Name of task class attribute/property.
+        type (InfluenceProvider, optional): Alternative
+            HashInfluenceProvider implementation used to interpret
+            the value of the attribute. If the attribute is a list,
+            the provider will be instantiated once for each item in
+            the list. For example, if the attribute is a list of
+            filesystem paths, the FileInfluence class could be passed
+            as argument to automatically monitor files at those paths.
+        sort (boolean, optional): Optionally sort the value. Always sort
+            values that are unstable, such as dictionaries.
 
     Example:
 
     .. code-block:: python
 
         from jolt import influence
 
-        @influence.source("attribute")
+        @influence.attribute("attribute")
         class Example(Task):
             attribute = False
+
+    .. code-block:: python
+
+        from jolt import influence
+
+        @influence.attribute("sources", type=influence.FileInfluence)
+        class Example(Task):
+            sources = [
+                "main.cpp",
+                "utils.cpp",
+            ]
     """
 
     def _decorate(cls):
         _old_influence = cls._influence
+
         def _influence(self, *args, **kwargs):
             influence = _old_influence(self, *args, **kwargs)
-            influence.append(TaskAttributeInfluence(name, sort))
+            if type:
+                items = getattr(self, name, [])
+                if callable(items):
+                    items = items()
+                if sort:
+                    items = sorted(items)
+                for item in items:
+                    influence.append(type(item))
+            else:
+                influence.append(TaskAttributeInfluence(name, sort))
             return influence
+
         cls._influence = _influence
         return cls
     return _decorate
 
 
 class TaskSourceInfluence(HashInfluenceProvider):
     def __init__(self, funcname, obj=None):
-        self.name = "Source:" + funcname
+        self.name = "Source"
         self.funcname = funcname
         self.obj = obj
 
+    @staticmethod
+    def _default_func():
+        pass
+
     def get_influence(self, task):
         obj = self.obj or task
-        return utils.sha1(task._get_source(getattr(obj, self.funcname)))
+        try:
+            funcname = self.funcname
+            funcname = obj.expand(funcname)
+        except Exception:
+            pass
+
+        # Collect all functions from the class hierarchy
+        if type(obj) == type:
+            funcs = [utils.getattr_safe(mro, funcname, TaskSourceInfluence._default_func)
+                     for mro in obj.mro()]
+        else:
+            funcs = [utils.getattr_safe(mro, funcname, TaskSourceInfluence._default_func)
+                     for mro in obj.__class__.mro()]
+
+        # Calculate sha1 sum for all functions
+        shasum = hashlib.sha1()
+        for func in funcs:
+            try:
+                func.__influence
+            except AttributeError:
+                func.__influence = utils.sha1(inspection.getfuncsource(func))
+            finally:
+                shasum.update(func.__influence.encode())
+
+        return shasum.hexdigest() + ": " + funcname
 
 
 def source(name, obj=None):
     """ Add function source code as hash influence.
 
     Args:
         name (str): Name of function in task class.
@@ -122,40 +182,106 @@
         class Example(Task):
             def method(self):
                 return False
 
     """
     def _decorate(cls):
         _old_influence = cls._influence
+
         def _influence(self, *args, **kwargs):
             influence = _old_influence(self, *args, **kwargs)
             influence.append(TaskSourceInfluence(name, obj))
             return influence
+
         cls._influence = _influence
         return cls
     return _decorate
 
 
+class TaskClassSourceInfluence(HashInfluenceProvider):
+    name = "Source"
+
+    def get_influence(self, task):
+        # Calculate sha1 sum for classes in hierarchy
+        result = ""
+        for cls in reversed(task.__class__.mro()):
+            if cls is object:
+                continue
+            try:
+                cls.__dict__["_TaskClassSourceInfluence__influence"]
+            except KeyError:
+                try:
+                    cls.__influence = utils.sha1(inspection.getclasssource(cls))
+                except TypeError:
+                    continue
+            result += cls.__dict__["_TaskClassSourceInfluence__influence"] + \
+                ": " + cls.__name__ + "\n"
+        return result
+
+
+class TaskRequirementInfluence(HashInfluenceProvider):
+    name = "Requirement"
+
+    def __init__(self, proxy):
+        self._identity = proxy.identity
+        self._name = proxy.short_qualified_name
+
+    def get_influence(self, task):
+        return "{}: {}".format(self._identity, self._name)
+
+
 @HashInfluenceRegistry.Register
 class TaskNameInfluence(HashInfluenceProvider):
     name = "Name"
+
     def get_influence(self, task):
         return task.name
 
 
 @HashInfluenceRegistry.Register
 class TaskParameterInfluence(HashInfluenceProvider):
     name = "Parameters"
+
     def get_influence(self, task):
         return ",".join(
             sorted(["{0}={1}".format(key, value)
                     for key, value in task._get_parameter_objects().items()
                     if value.is_influencer()]))
 
 
+class InstanceInfluence(HashInfluenceProvider):
+    name = "Instance"
+
+    def get_influence(self, task):
+        return task._instance.value
+
+
+def always(cls):
+    """ Always execute the task.
+
+    Example:
+
+      .. code-block:: python
+
+        from jolt import influence
+
+        @influence.always
+        class Example(Task):
+
+    """
+    _old_influence = cls._influence
+
+    def _influence(self, *args, **kwargs):
+        influence = _old_influence(self, *args, **kwargs)
+        influence.append(InstanceInfluence())
+        return influence
+
+    cls._influence = _influence
+    return cls
+
 
 class TaskDateInfluence(HashInfluenceProvider):
     name = "Date"
 
     def __init__(self, fmt):
         self.fmt = fmt
 
@@ -163,18 +289,20 @@
         now = datetime.datetime.now()
         return now.strftime(self.fmt)
 
 
 def _date_influence(fmt):
     def _decorate(cls):
         _old_influence = cls._influence
+
         def _influence(self, *args, **kwargs):
             influence = _old_influence(self, *args, **kwargs)
             influence.append(TaskDateInfluence(fmt))
             return influence
+
         cls._influence = _influence
         return cls
     return _decorate
 
 
 yearly = _date_influence("%Y")
 """ Add yearly hash influence.
@@ -188,14 +316,15 @@
         from jolt import influence
 
         @influence.yearly
         class Example(Task):
 
 """
 
+
 weekly = _date_influence("%Y-%w")
 """ Add weekly hash influence.
 
 If nothing else changes, the task is re-executed once every week.
 
 Example:
 
@@ -204,14 +333,15 @@
         from jolt import influence
 
         @influence.weekly
         class Example(Task):
 
 """
 
+
 monthly = _date_influence("%Y-%m")
 """ Add monthly hash influence.
 
 If nothing else changes, the task is re-executed once every month.
 
 Example:
 
@@ -220,14 +350,15 @@
         from jolt import influence
 
         @influence.monthly
         class Example(Task):
 
 """
 
+
 daily = _date_influence("%Y-%m-%d")
 """ Add daily hash influence.
 
 If nothing else changes, the task is re-executed once every day.
 
 Example:
 
@@ -236,14 +367,15 @@
         from jolt import influence
 
         @influence.daily
         class Example(Task):
 
 """
 
+
 hourly = _date_influence("%Y-%m-%d %H")
 """ Add hourly hash influence.
 
 If nothing else changes, the task is re-executed once every hour.
 
 Example:
 
@@ -253,15 +385,14 @@
 
         @influence.hourly
         class Example(Task):
 
 """
 
 
-
 class TaskEnvironmentInfluence(HashInfluenceProvider):
     name = "Environment"
 
     def __init__(self, variable):
         self.variable = variable
 
     def get_influence(self, task):
@@ -283,59 +414,81 @@
 
         @influence.environ("CFLAGS")
         class Example(Task):
 
     """
     def _decorate(cls):
         _old_influence = cls._influence
+
         def _influence(self, *args, **kwargs):
             influence = _old_influence(self, *args, **kwargs)
             influence.append(TaskEnvironmentInfluence(variable))
             return influence
+
         cls._influence = _influence
         return cls
 
     return _decorate
 
 
 _fi_files = {}
 
 
 class FileInfluence(HashInfluenceProvider):
     def __init__(self, path):
-        self.path = path
+        self.path = path.rstrip(fs.sep)
         self.name = "File"
+        self._files = {}
 
     def get_file_influence(self, path):
-        sha = hashlib.sha1()
-        with open(path, "rb") as f:
-            for data in iter(lambda: f.read(0x10000), b''):
-                sha.update(data)
-        return sha.hexdigest()
+        return utils.filesha1(str(path))
+
+    def get_filelist(self, task):
+        try:
+            return self._files[task]
+        except KeyError:
+            if fs.path.isdir(task.tools.expand_path(self.path)):
+                path = self.path + fs.sep + "**"
+            else:
+                path = self.path
+
+            filelist = task.tools.glob(path, expand=True)
+            filelist.sort()
+            filelist = [Path(fname) for fname in filelist]
+            self._files[task] = filelist
+            return filelist
 
     def get_influence(self, task):
         result = []
-        files = task.tools.glob(self.path)
-        files.sort()
-        for f in files:
-            f = task.tools.expand_path(f)
-            if fs.path.isdir(f):
+        for f in self.get_filelist(task):
+            if f.is_dir():
                 continue
             value = _fi_files.get(f)
             if value:
                 result.append(value)
-            elif fs.path.exists(f):
-                _fi_files[f] = value = fs.path.basename(f) + ":" + self.get_file_influence(f)
+            elif f.exists():
+                _fi_files[f] = value = self.get_file_influence(f) + ": " + f.name
                 result.append(value)
-            elif fs.path.lexists(f):
-                _fi_files[f] = value = fs.path.basename(f) + ": Symlink (broken)"
+            elif fs.path.lexists(str(f)):
+                _fi_files[f] = value = "Symlink (broken): " + f.name
                 result.append(value)
-
         return "\n".join(result)
 
+    def is_influenced_by(self, task, path):
+        """
+        Return True if the path influences the task.
+        """
+        path = task.tools.expand_path(path)
+        return PurePath(path) in self.get_filelist(task)
+
+
+class DirectoryInfluence(FileInfluence):
+    def __init__(self, path):
+        super().__init__(path.rstrip(os.sep) + "/**")
+
 
 def files(pathname):
     """ Add file content hash influence.
 
     Args:
         pathname (str): A pathname pattern used to find files that will
                 influence the hash of the task
@@ -351,34 +504,105 @@
 
         @influence.files("*.cpp")
         class Example(Task):
 
     """
     def _decorate(cls):
         _old_influence = cls._influence
+
         def _influence(self, *args, **kwargs):
             influence = _old_influence(self, *args, **kwargs)
             influence.append(FileInfluence(pathname))
             return influence
+
         cls._influence = _influence
         return cls
 
     return _decorate
 
 
 def global_files(pathname, cls=FileInfluence):
     HashInfluenceRegistry.get().register(cls(pathname))
 
 
+class WhitelistInfluence(FileInfluence):
+    def __init__(self, path):
+        self.path = path.rstrip(fs.sep)
+        self.name = "Whitelist"
+
+    def get_influence(self, task):
+        return self.path
+
+    def is_influenced_by(self, task, path):
+        path = task.tools.expand_path(path)
+        pattern = task.tools.expand_path(self.path)
+        return utils.pathmatch(path, pattern)
+
+
+def whitelist(pathname):
+    """
+    Whitelist files published by a task, but don't let them influence
+    the hash.
+
+    This is typically used to whitelist files in the workspace. It
+    should only be used for files produced by the task, not for files
+    used as input. If possible, consider writing files to build
+    directories instead.
+
+    This decorator cannot be used to exclude influencing files matched
+    by another influence decorator. If there is an overlap of files
+    between decorators, some or all of the overlapping files files may
+    influence the hash.
+
+    Args:
+        pathname (str): A pathname pattern used to match whitelisted files.
+                The pattern may contain simple shell-style
+                wildcards such as '*' and '?'. Note: files starting with a
+                dot are not matched by these wildcards.
+
+    Example:
+
+    .. code-block:: python
+
+        from jolt import influence
+
+        @influence.whitelist("build/")
+        class Example(Task):
+
+    """
+    def _decorate(cls):
+        _old_influence = cls._influence
+
+        def _influence(self, *args, **kwargs):
+            influence = _old_influence(self, *args, **kwargs)
+            influence.append(WhitelistInfluence(pathname))
+            return influence
+
+        cls._influence = _influence
+        return cls
+
+    return _decorate
+
 
 class StringInfluence(HashInfluenceProvider):
     name = "String"
 
     def __init__(self, value):
         self.value = value
 
     def get_influence(self, task):
         return self.value
 
 
 def global_string(string):
     HashInfluenceRegistry.get().register(StringInfluence(string))
+
+
+class VersionInfluence(HashInfluenceProvider):
+    name = "Version"
+
+    def get_influence(self, task):
+        return version.__version__
+
+
+def global_version():
+    HashInfluenceRegistry.get().register(VersionInfluence())
```

### Comparing `jolt-0.9.9/jolt/error.py` & `jolt-0.9.93/jolt/error.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,41 @@
+from jolt import inspection
+from jolt import utils
 
 
 class JoltError(Exception):
     def __init__(self, *args, **kwargs):
         super(JoltError, self).__init__(*args, **kwargs)
 
 
 class JoltCommandError(JoltError):
-    def __init__(self, what, stdout, stderr, returncode, *args, **kwargs):
+    def __init__(self, what, stdout=[], stderr=[], returncode=None, *args, **kwargs):
         super(JoltCommandError, self).__init__(what, *args, **kwargs)
         self.stdout = stdout
         self.stderr = stderr
         self.returncode = returncode
 
 
 def raise_error(msg, *args, **kwargs):
     raise JoltError(msg.format(*args, **kwargs))
 
 
 def raise_task_error(task, msg, *args, **kwargs):
     if task:
+        with utils.ignore_exception():
+            with task.report() as report:
+                report.add_error("Error", inspection.getfile(task.__class__),
+                                 msg.format(*args, **kwargs))
+        raise_error(msg + " (" + str(task) + ")", *args, **kwargs)
+    else:
+        raise_error(msg, *args, **kwargs)
+
+
+def raise_unreported_task_error(task, msg, *args, **kwargs):
+    if task:
         raise_error(msg + " (" + str(task) + ")", *args, **kwargs)
     else:
         raise_error(msg, *args, **kwargs)
 
 
 def raise_error_if(condition, *args, **kwargs):
     if condition:
@@ -30,14 +43,19 @@
 
 
 def raise_task_error_if(condition, task, *args, **kwargs):
     if condition:
         raise_task_error(task, *args, **kwargs)
 
 
+def raise_unreported_task_error_if(condition, task, *args, **kwargs):
+    if condition:
+        raise_unreported_task_error(task, *args, **kwargs)
+
+
 class raise_error_on_exception(object):
     def __init__(self, message):
         self.message = message
 
     def __enter__(self):
         return self
```

### Comparing `jolt-0.9.9/jolt/log.py` & `jolt-0.9.93/jolt/log.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 from __future__ import print_function
 import os
+import re
 import sys
 import tqdm
+if os.name == "nt":
+    # FIXME: Workaround to make tqdm behave correctly on Windows
+    import colorama
+    colorama.deinit()  # Undo the work of tqdm
+    os.system("")      # Hack to enable vt100
 import traceback
 from datetime import datetime
 import threading
 import logging
 import logging.handlers
 from contextlib import contextmanager
 try:
     from StringIO import StringIO
-except:
+except Exception:
     from io import StringIO
 
 from jolt import config
+from jolt.error import JoltError
 from jolt import filesystem as fs
 from jolt import colors
 
 
 default_path = fs.path.join(config.get_logpath(), "jolt.log")
 logfile = config.get("jolt", "logfile", default_path)
-logsize = config.getsize("jolt", "logsize", os.environ.get("JOLT_LOGSIZE", 10*1024**2))  # 10MiB
+logsize = config.getsize("jolt", "logsize", os.environ.get("JOLT_LOGSIZE", 10 * 1024 ** 2))  # 10MiB
 logcount = config.getint("jolt", "logcount", os.environ.get("JOLT_LOGCOUNT", 1))
 
 dirpath = fs.path.dirname(logfile)
 if not fs.path.exists(dirpath):
     fs.makedirs(dirpath)
 with open(logfile, "a") as f:
     f.write("--------------------------------------------------------------------------------\n")
@@ -35,14 +42,15 @@
 WARNING = logging.WARNING
 INFO = logging.INFO
 VERBOSE = 15
 DEBUG = logging.DEBUG
 EXCEPTION = logging.DEBUG + 1
 STDOUT = logging.INFO + 1
 STDERR = logging.ERROR + 1
+SILENCE = STDERR + 1
 logging.addLevelName(VERBOSE, "VERBOSE")
 logging.addLevelName(STDOUT, "STDOUT")
 logging.addLevelName(STDERR, "STDERR")
 logging.addLevelName(EXCEPTION, "EXCEPT")
 
 logging.raiseExceptions = False
 
@@ -51,68 +59,108 @@
     def __init__(self, fmt, *args, **kwargs):
         super(Formatter, self).__init__(*args, **kwargs)
         self.fmt = fmt
 
     def format(self, record):
         try:
             record.message = record.msg.format(*record.args)
-        except:
+        except Exception:
             record.message = record.msg
         record.asctime = datetime.fromtimestamp(record.created).strftime("%Y-%m-%d %H:%M:%S.%f")
         return self.fmt.format(
             levelname=record.levelname,
             message=record.message,
             asctime=record.asctime
         )
 
 
 class ConsoleFormatter(logging.Formatter):
-    def __init__(self, fmt, *args, **kwargs):
+    def __init__(self, fmt_prefix, fmt_noprefix, *args, **kwargs):
         super(ConsoleFormatter, self).__init__(*args, **kwargs)
-        self.fmt = fmt
+        self.fmt_prefix = fmt_prefix
+        self.fmt_noprefix = fmt_noprefix
+        self.always_prefix = False
+
+    def enable_prefixes(self):
+        self.always_prefix = True
+
+    def enable_gdb(self):
+        self.always_prefix = True
+        self.fmt_prefix = "~\"" + self.fmt_prefix + "\\n\""
 
     def format(self, record):
         try:
             msg = record.msg.format(*record.args)
-        except:
+        except Exception:
             msg = record.msg
         if sys.stdout.isatty() and sys.stderr.isatty():
             if record.levelno >= ERROR:
                 msg = colors.red(msg)
             elif record.levelno >= WARNING:
                 msg = colors.yellow(msg)
         record.message = msg
         record.asctime = datetime.fromtimestamp(record.created).strftime("%Y-%m-%d %H:%M:%S.%f")
-        return self.fmt.format(
+        record.prefix = True if record.__dict__.get("prefix", False) else False
+
+        if not record.prefix and \
+           not self.always_prefix and \
+           record.levelno in [STDOUT, STDERR]:
+            fmt = self.fmt_noprefix
+        else:
+            fmt = self.fmt_prefix
+
+        return fmt.format(
             levelname=record.levelname,
             message=record.message,
             asctime=record.asctime
         )
 
 
 class Filter(logging.Filter):
     def __init__(self, filterfn):
         self.filterfn = filterfn
 
     def filter(self, record):
         return self.filterfn(record)
 
 
-# create logger
+class TqdmStream(object):
+    def __init__(self, stream):
+        self.stream = stream
+
+    def write(self, msg):
+        with tqdm.tqdm.external_write_mode(file=self.stream, nolock=False):
+            self.stream.write(msg)
+
+    def flush(self):
+        getattr(self.stream, 'flush', lambda: None)()
+
+
+# silence root logger
+_root = logging.getLogger()
+_root.setLevel(logging.CRITICAL)
+
+# create jolt logger
 _logger = logging.getLogger('jolt')
 _logger.setLevel(logging.DEBUG)
 
-_console_formatter = ConsoleFormatter('[{levelname:>7}] {message}')
+_console_formatter = ConsoleFormatter('[{levelname:>7}] {message}', '{message}')
 
-_stdout = logging.StreamHandler(sys.stdout)
+if sys.stdout.isatty() and sys.stderr.isatty():
+    _stdout = logging.StreamHandler(TqdmStream(sys.stdout))
+else:
+    _stdout = logging.StreamHandler(sys.stdout)
 _stdout.setLevel(INFO)
 _stdout.setFormatter(_console_formatter)
 _stdout.addFilter(Filter(lambda r: r.levelno < ERROR))
 
-_stderr = logging.StreamHandler(sys.stderr)
+if sys.stdout.isatty() and sys.stderr.isatty():
+    _stderr = logging.StreamHandler(TqdmStream(sys.stdout))
+else:
+    _stderr = logging.StreamHandler(sys.stderr)
 _stderr.setLevel(INFO)
 _stderr.setFormatter(_console_formatter)
 _stderr.addFilter(Filter(lambda r: r.levelno >= ERROR))
 _stderr.addFilter(Filter(lambda r: r.levelno != EXCEPTION))
 
 _file = logging.handlers.RotatingFileHandler(logfile, maxBytes=logsize, backupCount=logcount)
 _file.setLevel(logging.DEBUG)
@@ -120,48 +168,77 @@
 _file.setFormatter(_file_formatter)
 
 _logger.addHandler(_stdout)
 _logger.addHandler(_stderr)
 _logger.addHandler(_file)
 
 
-
 def info(fmt, *args, **kwargs):
     _logger.info(fmt, *args, **kwargs)
 
+
 def warning(fmt, *args, **kwargs):
     _logger.warning(fmt, *args, **kwargs)
 
+
 def verbose(fmt, *args, **kwargs):
     _logger.log(VERBOSE, fmt, *args, **kwargs)
 
+
 def debug(fmt, *args, **kwargs):
     _logger.debug(fmt, *args, **kwargs)
 
+
 def error(fmt, *args, **kwargs):
     _logger.error(fmt, *args, **kwargs)
 
-def stdout(line):
+
+def stdout(line, **kwargs):
     line = line.replace("{", "{{")
     line = line.replace("}", "}}")
-    _logger.log(STDOUT, line)
+    _logger.log(STDOUT, line, extra=kwargs)
+
 
-def stderr(line):
+def stderr(line, **kwargs):
     line = line.replace("{", "{{")
     line = line.replace("}", "}}")
-    _logger.log(STDERR, line)
+    _logger.log(STDERR, line, extra=kwargs)
+
 
 def exception(exc=None):
     if exc:
-        _logger.error(str(exc))
-    backtrace = traceback.format_exc()
-    for line in backtrace.splitlines():
+        te = traceback.TracebackException.from_exception(exc)
+        if isinstance(exc, JoltError):
+            _logger.error("{}", str(exc))
+        elif isinstance(exc, SyntaxError):
+            filename = fs.path.relpath(
+                te.filename,
+                fs.path.commonprefix([os.getcwd(), te.filename]))
+            _logger.error("SyntaxError: {} ({}, line {})",
+                          te.text.strip(),
+                          filename,
+                          te.lineno)
+        else:
+            filename = fs.path.relpath(
+                te.stack[-1].filename,
+                fs.path.commonprefix([os.getcwd(), te.stack[-1].filename]))
+            _logger.error("{}: {} ({}, line {}, in {})",
+                          type(exc).__name__,
+                          str(exc) or te.stack[-1].line,
+                          filename,
+                          te.stack[-1].lineno,
+                          te.stack[-1].name)
+        backtrace = traceback.format_exc().splitlines()
+    else:
+        backtrace = traceback.format_exc().splitlines()
+    for line in backtrace:
         line = line.replace("{", "{{")
         line = line.replace("}", "}}")
-        _logger.log(EXCEPTION, line)
+        _logger.log(EXCEPTION, line.strip())
+
 
 def transfer(line, context):
     context = "[{}] ".format(context)
     outline1 = context + line[10:]
     outline2 = context + line
     if line.startswith("[  ERROR]"):
         error(outline1)
@@ -172,19 +249,27 @@
     elif line.startswith("[   INFO]"):
         info(outline1)
     elif line.startswith("[ EXCEPT]"):
         outline1 = outline1.replace("{", "{{")
         outline1 = outline1.replace("}", "}}")
         _logger.log(EXCEPTION, outline1)
     elif line.startswith("[ STDERR]"):
-        stderr(outline1)
+        stderr(outline1, prefix=True)
     elif line.startswith("[ STDOUT]"):
-        stdout(outline1)
+        stdout(outline1, prefix=True)
     else:
-        stdout(outline2)
+        stdout(outline2, prefix=True)
+
+
+def decompose(line):
+    match = re.match(r"(?P<timestamp>[0-9]{4}-[0-9]{1,2}-[0-9]{1,2} [0-9]{1,2}:[0-9]{1,2}:[0-9]{1,2}.[0-9]{6}) \[(?P<loglevel>.*?)\]( \[(?P<context>.*?)\])? (?P<message>.*)", line)
+    if not match:
+        return line
+    match = match.groupdict()
+    return match["timestamp"], match["loglevel"].strip(), match.get("context"), match["message"]
 
 
 class _Progress(object):
     def __init__(self, msg):
         verbose(msg)
 
     def __enter__(self):
@@ -197,68 +282,97 @@
         pass
 
 
 def progress_log(desc, count, unit):
     return _Progress(desc)
 
 
-def progress(desc, count, unit):
-    if sys.stdout.isatty() and sys.stderr.isatty() and not is_verbose():
-        p = tqdm.tqdm(total=count, unit=unit, unit_scale=True)
+def progress(desc, count, unit, estimates=True, debug=False):
+    bar_format = '{l_bar}{bar}| {n_fmt}/{total_fmt} [{elapsed}]' \
+                 if not estimates else None
+    if not debug and is_interactive() and not is_verbose():
+        p = tqdm.tqdm(total=count, unit=unit, unit_scale=True, bar_format=bar_format, dynamic_ncols=True)
         p.set_description("[   INFO] " + desc)
         return p
     return progress_log(desc, count, unit)
 
 
 def set_level(level):
     _stdout.setLevel(level)
     _stderr.setLevel(level)
 
 
+def set_worker():
+    _console_formatter.enable_prefixes()
+
+
+def enable_gdb():
+    set_interactive(False)
+    _console_formatter.enable_gdb()
+
+
 def is_verbose():
     return _stdout.level <= VERBOSE
 
 
+_interactive = True
+
+
+def is_interactive():
+    global _interactive
+    return _interactive and sys.stdout.isatty() and sys.stderr.isatty()
+
+
+def set_interactive(value):
+    global _interactive
+    _interactive = value
+
+
 class _ThreadMapper(Filter):
     def __init__(self):
         self.thread_map = {}
 
     def map(self, fr, to):
         self.thread_map[fr] = to
 
     def unmap(self, fr):
         del self.thread_map[fr]
 
     def filter(self, record):
         record.thread = self.thread_map.get(record.thread, record.thread)
         return True
 
+
 _thread_map = _ThreadMapper()
 
 
 @contextmanager
-def threadsink():
+def threadsink(level=DEBUG):
     threadid = threading.get_ident()
     stringbuf = StringIO()
     handler = logging.StreamHandler(stringbuf)
-    handler.setLevel(DEBUG)
+    handler.setLevel(level)
     handler.setFormatter(_file_formatter)
     handler.addFilter(_thread_map)
     handler.addFilter(Filter(lambda record: record.thread == threadid))
     _logger.addHandler(handler)
-    yield stringbuf
-    _logger.removeHandler(handler)
+    try:
+        yield stringbuf
+    finally:
+        _logger.removeHandler(handler)
 
 
 @contextmanager
 def map_thread(thread_from, thread_to):
     tid = thread_from.ident
     _thread_map.map(tid, thread_to.ident)
-    yield
-    _thread_map.unmap(tid)
+    try:
+        yield
+    finally:
+        _thread_map.unmap(tid)
 
 
 class _LogStream(object):
     def __init__(self):
         self.buf = ""
 
     def write(self, data):
```

### Comparing `jolt-0.9.9/jolt/expires.py` & `jolt-0.9.93/jolt/expires.py`

 * *Files identical despite different names*

### Comparing `jolt-0.9.9/jolt/xmldom.py` & `jolt-0.9.93/jolt/xmldom.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from base64 import decodestring as base64_decodestring
-from base64 import encodestring as base64_encodestring
+from base64 import decodebytes as base64_decodebytes
+from base64 import encodebytes as base64_encodebytes
 import codecs
 from xml.etree.ElementTree import Element
 from xml.etree.ElementTree import ElementTree
-from xml.etree import ElementTree as ET
 
 
 class SubElement(object):
     def __init__(self, tag='', elem=None):
         super(SubElement, self).__init__()
         self._elem = elem if elem is not None else Element(tag)
 
@@ -70,63 +69,67 @@
                     raise ValueError('{0} is not one of {1}'.format(value, values))
 
             def attr_get(self):
                 if attribute not in self.attrib:
                     return ''
                 value = self.get(attribute)
                 if base64:
-                    value = base64_decodestring(value.encode())
+                    value = base64_decodebytes(value.encode())
                     if zlib:
                         value = codecs.decode(value, "zlib")
                     value = value.decode()
                 return value
 
             def attr_set(self, value):
                 if value is None:
                     try:
                         self.attrib.pop(attribute)
-                    except:
+                    except Exception:
                         pass
                     finally:
                         return
                 _check_value(value, values)
                 if base64:
                     value = value.encode()
                     if zlib:
                         value = codecs.encode(value, "zlib")
-                    value = base64_encodestring(value).decode()
+                    value = base64_encodebytes(value).decode()
                 return self.set(attribute, value)
 
             def child_get(self):
-                if not hasattr(self, '_'+varname):
+                if not hasattr(self, '_' + varname):
                     e = SubElement(attribute, elem=self._elem.find(attribute))
-                    setattr(self, '_'+varname, e)
-                value = getattr(self, '_'+varname).text
+                    setattr(self, '_' + varname, e)
+                value = getattr(self, '_' + varname).text
                 if value is None:
                     return None
                 if base64:
-                    value = base64_decodestring(value.encode())
-                    if zlib:
-                        value = codecs.decode(value, "zlib")
-                    value = value.decode()
+                    try:
+                        value = base64_decodebytes(value.encode())
+                        if zlib:
+                            value = codecs.decode(value, "zlib")
+                        value = value.decode()
+                    except Exception:
+                        value = getattr(self, '_' + varname).text
                 return str(value)
 
             def child_set(self, value):
                 _check_value(value, values)
-                if not value: return
-                if not hasattr(self, '_'+varname):
+                if value is None:
+                    return
+                if not hasattr(self, '_' + varname):
                     e = SubElement(attribute)
                     self.append(e)
-                    setattr(self, '_'+varname, e)
+                    setattr(self, '_' + varname, e)
                 if base64:
                     value = value.encode()
                     if zlib:
                         value = codecs.encode(value, "zlib")
-                    value = base64_encodestring(value).decode()
-                getattr(self,'_'+varname).text = value
+                    value = base64_encodebytes(value).decode()
+                getattr(self, '_' + varname).text = value
 
             if not child:
                 setattr(cls, varname, property(attr_get, attr_set))
             else:
                 setattr(cls, varname, property(child_get, child_set))
             return cls
         return decorate(cls, self.attribute, self.varname, self.child, self.values)
```

### Comparing `jolt-0.9.9/jolt/graph.py` & `jolt-0.9.93/jolt/graph.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 from contextlib import contextmanager
+import copy
 import hashlib
-import networkx as nx
 from os import getenv
 from threading import RLock
+from collections import OrderedDict
 import uuid
 
-from jolt.tasks import Alias, Resource, Export
-#from jolt.utils import *
-from jolt.influence import HashInfluenceRegistry
+from jolt.tasks import Alias, Resource, WorkspaceResource, Task
+from jolt.influence import HashInfluenceRegistry, TaskRequirementInfluence
 from jolt import log
 from jolt import utils
 from jolt import colors
 from jolt import hooks
-from jolt import tools
 from jolt import filesystem as fs
 from jolt.error import raise_error_if
 from jolt.error import raise_task_error_if
 from jolt.options import JoltOptions
 
 
 class TaskProxy(object):
     def __init__(self, task, graph, options):
         self.task = task
         self.graph = graph
         self.options = options
 
         self.children = []
-        self.ancestors = []
+        self.ancestors = set()
+        self.descendants = set()
         self.neighbors = []
         self.extensions = []
         self.duration_queued = None
         self.duration_running = None
+        self.requirement_aliases = {}
 
         self._extended_task = None
         self._in_progress = False
         self._completed = False
         self._goal = False
         self._download = True
+        self._local = False
+        self._network = False
         hooks.task_created(self)
 
     def __hash__(self):
         return id(self)
 
     @property
     def tools(self):
@@ -67,81 +70,72 @@
         return "({0} {1})".format(self.short_qualified_name, self.identity[:8])
 
     @property
     def identity(self):
         if self.task.identity is not None:
             return self.task.identity
 
-        sha = hashlib.sha1()
+        # Acquire workspace resources before calculating the identity
+        for c in self.children:
+            if c.is_workspace_resource():
+                c.task.acquire_ws()
 
+        sha = hashlib.sha1()
         HashInfluenceRegistry.get().apply_all(self.task, sha)
-
-        # print("{}: {}".format(self.name, [n.name for n in self.children]))
-        for node in self.children:
-            sha.update(node.identity.encode())
-
-        if self._extended_task:
-            sha.update(self._extended_task.identity.encode())
-
         self.task.identity = sha.hexdigest()
+
         return str(self.task.identity)
 
     @identity.setter
     def identity(self, value):
         self.task.identity = value
 
     @property
+    def instance(self):
+        return self.task._instance.value
+
+    @property
     def weight(self):
         return self.task.weight
 
     @weight.setter
     def weight(self, weight):
-        self.task.weight =  weight
+        self.task.weight = weight
 
     def __str__(self):
         return "{0}{1}".format(self.short_qualified_name, "*" if self.is_extension() else '')
 
     def info(self, fmt, *args, **kwargs):
         self.task.info(fmt + " " + self.log_name, *args, **kwargs)
 
+    def verbose(self, fmt, *args, **kwargs):
+        log.verbose(fmt + " " + self.log_name, *args, **kwargs)
+
     def warning(self, fmt, *args, **kwargs):
         self.task.warning(fmt + " " + self.log_name, *args, **kwargs)
 
     def error(self, fmt, *args, **kwargs):
         self.task.error(fmt + " " + self.log_name, *args, **kwargs)
 
     def has_children(self):
         return len(self.children) > 0
 
     def has_ancestors(self):
         return len(self.ancestors) > 0
 
-    def is_cacheable(self):
-        return self.task.is_cacheable()
-
-    def is_alias(self):
-        return isinstance(self.task, Alias)
-
-    def is_resource(self):
-        return isinstance(self.task, Resource)
-
     def has_artifact(self):
         return self.is_cacheable() and not self.is_resource() and not self.is_alias()
 
     def has_extensions(self):
         return len(self.extensions) > 0
 
     def add_extension(self, task):
         if self.is_extension():
-            self._extended_task.add_extension(task)
-        else:
-            self.extensions.append(task)
-
-    def is_extension(self):
-        return self._extended_task is not None
+            self.get_extended_task().add_extension(task)
+        self.extensions.append(task)
 
     def set_extended_task(self, task):
         self._extended_task = task
 
     def get_extended_task(self):
         if self.is_extension():
             return self._extended_task.get_extended_task()
@@ -151,84 +145,126 @@
         for c in self.children:
             if c.is_resource() or c.is_alias():
                 continue
             if not c.is_available_locally(cache):
                 return False
         return True
 
+    def is_alias(self):
+        return isinstance(self.task, Alias)
+
     def is_available_locally(self, cache):
         tasks = [self] + self.extensions
         return all(map(cache.is_available_locally, tasks))
 
     def is_available_remotely(self, cache):
         tasks = [self] + self.extensions
         return all(map(cache.is_available_remotely, tasks))
 
-    def is_uploadable(self, cache):
-        tasks = [self] + self.extensions
-        return all(map(cache.is_uploadable, tasks))
+    def is_cacheable(self):
+        return self.task.is_cacheable()
+
+    def is_completed(self):
+        return self._completed
 
     def is_downloadable(self):
         return self._download
 
-    def disable_download(self):
-        self._download = False
-        for extension in self.extensions:
-            extension.disable_download()
+    def is_extension(self):
+        return self._extended_task is not None
 
     def is_fast(self):
         tasks = [self.task] + [e.task for e in self.extensions]
         return all([task.fast for task in tasks])
 
+    def is_identified(self):
+        return self.task.identity is not None
+
+    def is_goal(self, with_extensions=True):
+        return self._goal or (with_extensions and any([e.is_goal() for e in self.extensions]))
+
     def in_progress(self):
         return self._in_progress
 
     def is_ready(self):
         if self.in_progress():
             return False
 
         if self.is_extension():
             return False
 
         return self.graph.is_leaf(self)
 
-    def is_completed(self):
-        return self._completed
+    def is_locally_executed(self):
+        return self._local
+
+    def is_remotely_executed(self):
+        return self._network
+
+    def is_resource(self):
+        return isinstance(self.task, Resource)
+
+    def is_unpackable(self):
+        return self.task.unpack.__func__ is not Task.unpack
+
+    def is_unpacked(self, cache):
+        tasks = [self] + self.extensions
+        return any(map(cache.is_unpacked, tasks))
+
+    def is_uploadable(self, cache):
+        tasks = [self] + self.extensions
+        return all(map(cache.is_uploadable, tasks))
+
+    def is_workspace_resource(self):
+        return isinstance(self.task, WorkspaceResource)
+
+    def disable_download(self):
+        self._download = False
+
+    def resolve_requirement_alias(self, name):
+        return self.requirement_aliases.get(name)
 
     def set_in_progress(self):
         self._in_progress = True
 
-    def is_goal(self):
-        return self._goal or any([e.is_goal() for e in self.extensions])
+    def set_locally_executed(self):
+        self._local = True
+
+    def set_remotely_executed(self):
+        self._network = True
 
     def set_goal(self):
         self._goal = True
 
     def finalize(self, dag, manifest):
         log.debug("Finalizing: " + self.short_qualified_name)
         self.manifest = manifest
 
         # Find all direct and transitive dependencies
-        self.descendants = sorted(
-            nx.descendants(dag, self),
-            key=lambda t: t.qualified_name)
-
-        # Find all direct dependencies
-        self.neighbors = list(
-            filter(lambda n: dag.are_neighbors(self, n), self.descendants))
+        self.ancestors = set()
+        self.descendants = set()
+
+        self.neighbors = copy.copy(self.children)
+        self.neighbors = sorted(self.neighbors, key=lambda n: n.qualified_name)
+
+        for n in self.neighbors:
+            self.descendants.add(n)
+            self.descendants = self.descendants.union(n.descendants)
+            if not n.task.selfsustained:
+                self.children.extend(n.children)
+            n.ancestors.add(self)
 
         # Exclude transitive alias and resources dependencies
         self.children = list(
-            filter(lambda n: not n.is_alias() and (not n.is_resource() or \
-                   dag.are_neighbors(self, n)),
-                   self.descendants))
-
-        self.ancestors = list(nx.ancestors(dag, self))
-        self.direct_ancestors = list(
-            filter(lambda n: dag.are_neighbors(n, self), self.ancestors))
+            filter(lambda n: not n.is_alias() and (not n.is_resource() or dag.are_neighbors(self, n)),
+                   utils.unique_list(self.children)))
+
+        self.descendants = list(self.descendants)
+
+        self.task.influence += [TaskRequirementInfluence(n) for n in self.neighbors]
 
         return self.identity
 
     def taint(self, salt=None):
         self.task.taint = salt or uuid.uuid4()
         if salt is None:
             # Only recalculate identity when build is forced, not when salted
@@ -244,43 +280,58 @@
     def running(self, when=None):
         self.duration_running = utils.duration() if not when else when
 
     def failed(self, what="Execution"):
         self.error("{0} failed after {1} {2}", what,
                    self.duration_running,
                    self.duration_queued.diff(self.duration_running))
+        self.graph.add_failed(self)
         hooks.task_failed(self)
 
+    def passed(self, what="Execution"):
+        hooks.task_passed(self)
+
     def finished(self, what="Execution"):
-        assert not self._completed, "task has already been completed"
+        raise_task_error_if(
+            self.is_completed() and not self.is_extension(),
+            self, "task has already been completed")
         self._completed = True
         try:
             self.graph.remove_node(self)
-        except:
+        except KeyError:
             self.warning("Pruned task was executed")
         self.task.info(colors.green(what + " finished after {0} {1}" + self.log_name),
                        self.duration_running,
                        self.duration_queued.diff(self.duration_running))
         hooks.task_finished(self)
 
     def skipped(self):
         self._completed = True
         try:
             self.graph.remove_node(self)
-        except:
-            self.warning("Pruned task was executed")
+        except KeyError:
+            pass
+        hooks.task_skipped(self)
+
+    def pruned(self):
+        self._completed = True
+        try:
+            self.graph.remove_node(self)
+        except KeyError:
+            self.warning("Pruned task was already pruned")
+        hooks.task_pruned(self)
 
-    def clean(self, cache, expired):
+    def clean(self, cache, if_expired, onerror=None):
         with self.tools:
             self.task.clean(self.tools)
-            discarded = cache.discard(self, expired)
+            discarded = cache.discard(self, if_expired, onerror=fs.onerror_warning)
             if discarded:
-                log.verbose("Discarded: {} ({})", self.short_qualified_name, self.identity[:8])
+                log.debug("Discarded: {} ({})", self.short_qualified_name, self.identity[:8])
             else:
-                log.verbose(" Retained: {} ({})", self.short_qualified_name, self.identity[:8])
+                log.debug(" Retained: {} ({})", self.short_qualified_name, self.identity[:8])
 
     def run(self, cache, force_upload=False, force_build=False):
         with self.tools:
             tasks = [self] + self.extensions
             available_locally = available_remotely = False
 
             for child in self.children:
@@ -291,66 +342,152 @@
                         not cache.download(child),
                         child, "failed to download task artifact")
 
             if not force_build:
                 available_locally = all(map(cache.is_available_locally, tasks))
                 if available_locally and not force_upload:
                     return
-                available_remotely = all(map(cache.is_available_remotely, tasks))
+                available_remotely = cache.download_enabled() and \
+                    all(map(cache.is_available_remotely, tasks))
                 if not available_locally and available_remotely:
                     available_locally = cache.download(self)
 
             if force_build or not available_locally:
                 with log.threadsink() as buildlog:
                     if self.task.is_runnable():
                         log.verbose("Host: {0}", getenv("HOSTNAME", "localhost"))
 
-                    with cache.get_context(self) as context:
-                        self.running()
-                        with self.tools.cwd(self.task.joltdir):
-                            if self.is_goal() and self.options.debug:
-                                log.info("Entering debug shell")
-                                self.task.shell(context, self.tools)
-                            self.task.run(context, self.tools)
-
-                    if cache.is_available_locally(self):
-                        with cache.get_artifact(self) as artifact:
-                            artifact.discard()
-
-                    with cache.get_artifact(self) as artifact:
-                        with self.tools.cwd(self.task.joltdir):
-                            self.task.publish(artifact, self.tools)
-                        with open(fs.path.join(artifact.path, ".build.log"), "w") as f:
-                            f.write(buildlog.getvalue())
-                        artifact.commit()
-
-            if force_build or force_upload or not available_remotely:
+                    with cache.get_locked_artifact(self, discard=force_build) as artifact:
+                        if not cache.is_available_locally(self) or self.has_extensions():
+                            with cache.get_context(self) as context:
+                                self.running()
+                                with self.tools.cwd(self.task.joltdir):
+                                    hooks.task_prerun(self, context, self.tools)
+                                    if self.is_goal() and self.options.debug:
+                                        log.info("Entering debug shell")
+                                        self.task.shell(context, self.tools)
+                                    self.task.run(context, self.tools)
+                                    hooks.task_postrun(self, context, self.tools)
+
+                                if not cache.is_available_locally(self):
+                                    with self.tools.cwd(self.task.joltdir):
+                                        hooks.task_prepublish(self, artifact, self.tools)
+                                        self.task.publish(artifact, self.tools)
+                                        self.task._verify_influence(context, artifact, self.tools)
+                                        hooks.task_postpublish(self, artifact, self.tools)
+                                    with open(fs.path.join(artifact.path, ".build.log"), "w") as f:
+                                        f.write(buildlog.getvalue())
+                                    cache.commit(artifact)
+                                else:
+                                    self.info("Publication skipped, already in local cache")
+                        else:
+                            self.info("Execution skipped, already in local cache")
+
+                        # Must upload the artifact while still holding its lock, otherwise the
+                        # artifact may become unpack():ed before we have a chance to.
+                        if force_upload or force_build or not available_remotely:
+                            raise_task_error_if(
+                                not cache.upload(self, force=force_upload, locked=False) and cache.upload_enabled(),
+                                self, "failed to upload task artifact")
+            elif force_upload or not available_remotely:
                 raise_task_error_if(
                     not cache.upload(self, force=force_upload) and cache.upload_enabled(),
                     self, "failed to upload task artifact")
 
             for extension in self.extensions:
                 try:
                     extension.started()
-                    extension.run(cache, force_upload, force_build)
+                    with hooks.task_run(extension):
+                        extension.run(cache, force_upload, force_build)
                 except Exception as e:
                     extension.failed()
                     raise e
                 else:
                     extension.finished()
 
+    def report(self):
+        return self.task.report()
+
 
-class Graph(nx.DiGraph):
+class Graph(object):
     def __init__(self):
-        super(Graph, self).__init__()
         self._mutex = RLock()
+        self._failed = []
+        self._children = OrderedDict()
+        self._parents = OrderedDict()
+
+    def add_node(self, node):
+        with self._mutex:
+            self._children[node] = OrderedDict()
+            self._parents[node] = OrderedDict()
 
     def remove_node(self, node):
         with self._mutex:
-            super(Graph, self).remove_node(node)
+            parents = self._parents[node].keys()
+            for child in self._children[node]:
+                del self._parents[child][node]
+            for parent in parents:
+                del self._children[parent][node]
+            del self._children[node]
+            del self._parents[node]
+
+    def add_edges_from(self, edges):
+        with self._mutex:
+            for src, dst in edges:
+                self._children[src][dst] = None
+                self._parents[dst][src] = None
+
+    def successors(self, node):
+        return self._children[node].keys()
+
+    def predecessors(self, node):
+        return self._parents[node].keys()
+
+    @property
+    def topological_nodes(self):
+        with self._mutex:
+            G = self.clone()
+            S = G.roots
+            L = []
+            while S:
+                for n in S:
+                    L.append(n)
+                    G.remove_node(n)
+                S = G.roots
+            if len(G.nodes) > 0:
+                log.debug("[GRAPH] Graph has cycles between these nodes:")
+                for node in G.nodes:
+                    log.debug("[GRAPH]   " + node.short_qualified_name)
+                raise_error_if(len(G.nodes) > 0, "graph has cycles")
+            return L
+
+    def clone(self):
+        g = Graph()
+        g._children = OrderedDict()
+        g._parents = OrderedDict()
+        for k, v in self._children.items():
+            g._children[k] = copy.copy(v)
+        for k, v in self._parents.items():
+            g._parents[k] = copy.copy(v)
+        return g
+
+    @property
+    def nodes(self):
+        with self._mutex:
+            return self._children.keys()
+
+    def number_of_tasks(self, filterfn=None):
+        return len(list(filter(filterfn, self.nodes)) if filterfn else self.nodes)
+
+    @property
+    def failed(self):
+        return self._failed
+
+    def add_failed(self, task):
+        self._failed.append(task)
 
     @property
     def tasks(self):
         with self._mutex:
             return [n for n in self.nodes]
 
     @property
@@ -362,92 +499,94 @@
         with self._mutex:
             return len(self.nodes) > 0
 
     def get_task(self, qualified_name):
         with self._mutex:
             return self._nodes_by_name.get(qualified_name)
 
-    def prune(self, func):
-        with self._mutex:
-            for node in nx.topological_sort(self):
-                if func(self, node):
-                    log.debug("[GRAPH] Pruned {0}", node.short_qualified_name)
-                    self.remove_node(node)
-
-            for node in self.nodes:
-                log.debug("[GRAPH] Keeping {0} ({1})", node.qualified_name, node.identity)
-
     def select(self, func):
         with self._mutex:
             return [n for n in self.nodes if func(self, n)]
 
     def debug(self):
         with self._mutex:
-            log.verbose("[GRAPH] Listing all nodes")
-            for node in nx.topological_sort(self):
-                log.verbose("[GRAPH]   " + node.qualified_name + " ({})", self.out_degree(node))
+            log.debug("[GRAPH] Listing all nodes")
+            for node in self.topological_nodes:
+                log.debug("[GRAPH]   " + node.qualified_name + " ({})", len(self._children[node].keys()))
 
     def is_leaf(self, node):
         with self._mutex:
-            return self.out_degree(node) == 0
+            return len(self._children[node].keys()) == 0
 
     def is_root(self, node):
         with self._mutex:
-            return self.in_degree(node) == 0
+            return len(self._parents[node].keys()) == 0
 
     def is_orphan(self, node):
         with self._mutex:
             return self.is_root(node) and self.is_leaf(node)
 
     def are_neighbors(self, n1, n2):
         with self._mutex:
-            return n2 in self[n1]
+            return n2 in self._children[n1]
 
 
 class GraphBuilder(object):
     def __init__(self, registry, manifest, options=None, progress=False):
         self.graph = Graph()
         self.nodes = {}
         self.registry = registry
         self.manifest = manifest
         self.progress = progress
         self.options = options or JoltOptions()
 
     def _get_node(self, progress, name):
+        name = utils.stable_task_name(name)
         node = self.nodes.get(name)
         if not node:
             task = self.registry.get_task(name, manifest=self.manifest)
-            node = self.nodes[name] = TaskProxy(task, self.graph, self.options)
+            node = self.nodes.get(task.qualified_name, None)
+            if node is not None:
+                return node
+            node = TaskProxy(task, self.graph, self.options)
+            self.nodes[node.short_qualified_name] = node
+            self.nodes[node.qualified_name] = node
             if self.options.salt:
                 node.taint(self.options.salt)
             self._build_node(progress, node)
             progress.update(1)
         return node
 
     def _build_node(self, progress, node):
         self.graph.add_node(node)
 
         if node.task.extends:
             extended_node = self._get_node(progress, node.task.extends)
             self.graph.add_edges_from([(node, extended_node)])
             node.set_extended_task(extended_node)
             extended_node.add_extension(node)
+            node.children.append(extended_node)
             parent = extended_node.get_extended_task()
         else:
             parent = node
 
         for requirement in node.task.requires:
-            child = self._get_node(progress, requirement)
+            alias, task, name = utils.parse_aliased_task_name(requirement)
+            child = self._get_node(progress, utils.format_task_name(task, name))
             # Create direct edges from alias parents to alias children
             if child.is_alias():
                 for child_child in child.children:
                     self.graph.add_edges_from([(parent, child_child)])
-            else:
-                self.graph.add_edges_from([(parent, child)])
+                    node.children.append(child_child)
+            self.graph.add_edges_from([(parent, child)])
             node.children.append(child)
+            if alias:
+                node.requirement_aliases[alias] = requirement
+
+        node.children = utils.unique_list(node.children)
 
         return node
 
     @contextmanager
     def _progress(self, *args, **kwargs):
         if self.progress:
             with log.progress(*args, **kwargs) as p:
@@ -455,56 +594,46 @@
         else:
             with log.progress_log(*args, **kwargs) as p:
                 yield p
 
     def build(self, task_list, influence=True):
         with self._progress("Building graph", len(self.graph.tasks), "tasks") as progress:
             goals = [self._get_node(progress, task) for task in task_list]
-            raise_error_if(not nx.is_directed_acyclic_graph(self.graph),
-                           "there are cyclic task dependencies")
             self.graph._nodes_by_name = self.nodes
 
         if influence:
-            topological_nodes = list(nx.topological_sort(self.graph))
+            topological_nodes = self.graph.topological_nodes
             with self._progress("Collecting task influence", len(self.graph.tasks), "tasks") as p:
                 for node in reversed(topological_nodes):
                     node.finalize(self.graph, self.manifest)
                     p.update(1)
 
             max_time = 0
             min_time = 0
             for node in topological_nodes:
                 max_time += node.task.weight
-                node.task.weight += max([a.weight for a in node.direct_ancestors] + [0])
+                node.task.weight += max([a.weight for a in node.ancestors] + [0])
                 min_time = max(node.task.weight, min_time)
 
             log.verbose("Time estimate: {}- {}",
                         utils.duration_diff(min_time),
                         utils.duration_diff(max_time))
 
+        self.graph.requested_goals = goals
         self.graph.goals = []
         for goal in goals:
             goal.set_goal()
             self.graph.goals.append(goal)
             if goal.is_alias():
                 for goal_alias in goal.neighbors:
                     goal_alias.set_goal()
                     self.graph.goals.append(goal_alias)
 
         return self.graph
 
-    def display(self):
-        from networkx.drawing.nx_agraph import write_dot
-
-        t = tools.Tools()
-        with t.tmpdir("dot") as tmpdir, t.cwd(tmpdir.get_path()):
-            write_dot(self.graph, fs.path.join(t.getcwd(), 'graph.dot'))
-            t.run('dot -Tsvg graph.dot -o graph.svg')
-            t.run('eog graph.svg')
-
 
 class PruneStrategy(object):
     def should_prune_requirements(self, task):
         raise NotImplementedError()
 
 
 class GraphPruner(object):
@@ -512,37 +641,37 @@
         self.strategy = strategy
         self.retained = set()
         self.visited = set()
 
     def _check_node(self, node):
         if node in self.visited:
             return
+        self._progress.update(1)
         self.visited.add(node)
         self.retained.add(node)
 
         prune = self.strategy.should_prune_requirements(node)
         if not node.task.selfsustained or not prune or node.is_extension():
-            for child in node.neighbors:
-                self._check_node(child)
+            utils.map_concurrent(self._check_node, node.neighbors)
 
     def prune(self, graph):
-        for root in graph.roots:
-            self._check_node(root)
+        with log.progress("Checking availability", 0, " tasks") as p:
+            self._progress = p
+            for root in graph.roots:
+                self._check_node(root)
 
-        pruned = []
+        for node in graph.goals:
+            self.retained.add(node)
 
-        for node in graph:
-            if node.is_goal():
-                self.retained.add(node)
-
-        for node in graph:
+        pruned = []
+        for node in graph.nodes:
             if node not in self.retained:
                 pruned.append(node)
             else:
-                log.verbose("Retained: {}", node.log_name)
+                log.debug("Retained: {}", node.log_name)
                 node.children = [c for c in node.children if c in self.retained]
 
         for node in pruned:
-            log.verbose("Excluded: {}", node.log_name)
-            graph.remove_node(node)
+            log.debug("Excluded: {}", node.log_name)
+            node.pruned()
 
         return graph
```

### Comparing `jolt-0.9.9/jolt.egg-info/SOURCES.txt` & `jolt-0.9.93/jolt.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -8,48 +8,71 @@
 jolt/config.py
 jolt/error.py
 jolt/expires.py
 jolt/filesystem.py
 jolt/graph.py
 jolt/hooks.py
 jolt/influence.py
+jolt/inspection.py
 jolt/loader.py
 jolt/log.py
 jolt/manifest.py
 jolt/options.py
 jolt/scheduler.py
 jolt/tasks.py
 jolt/tools.py
 jolt/utils.py
+jolt/version.py
+jolt/version_utils.py
 jolt/xmldom.py
 jolt.egg-info/PKG-INFO
 jolt.egg-info/SOURCES.txt
 jolt.egg-info/dependency_links.txt
 jolt.egg-info/entry_points.txt
 jolt.egg-info/requires.txt
 jolt.egg-info/top_level.txt
+jolt/pkgs/__init__.py
+jolt/pkgs/golang.py
+jolt/pkgs/nodejs.py
 jolt/plugins/__init__.py
+jolt/plugins/alias.py
+jolt/plugins/allure.py
 jolt/plugins/amqp.py
-jolt/plugins/artifactory.py
 jolt/plugins/autoweight.py
+jolt/plugins/cmake.py
+jolt/plugins/conan.py
 jolt/plugins/cxxinfo.py
+jolt/plugins/dashboard.py
+jolt/plugins/debian.py
+jolt/plugins/docker.py
+jolt/plugins/email.py
+jolt/plugins/email.xslt
 jolt/plugins/environ.py
 jolt/plugins/ftp.py
+jolt/plugins/gdb.py
 jolt/plugins/gerrit.py
 jolt/plugins/git.py
-jolt/plugins/jenkins.py
+jolt/plugins/golang.py
+jolt/plugins/googletest.py
+jolt/plugins/http.py
+jolt/plugins/junit.py
 jolt/plugins/logstash.py
-jolt/plugins/ninja-cache.py
+jolt/plugins/ninja-compdb.py
 jolt/plugins/ninja.py
-jolt/plugins/ninjacli.py
+jolt/plugins/nodejs.py
+jolt/plugins/paths.py
+jolt/plugins/podman.py
 jolt/plugins/python.py
 jolt/plugins/repo.py
+jolt/plugins/report.py
 jolt/plugins/selfdeploy.py
 jolt/plugins/strings.py
 jolt/plugins/symlinks.py
+jolt/plugins/telemetry.py
+jolt/plugins/timeline.py
 jolt/plugins/volume.py
+jolt/plugins/yaml-ninja.py
 jolt/plugins/yamltask.py
-jolt/tps/__init__.py
-jolt/tps/jenkins/__init__.py
-jolt/tps/jenkins/plugins.py
-jolt/tps/jenkins/version.py
-jolt/tps/pkg/__init__.py
+jolt/templates/cxxexecutable.cmake.template
+jolt/templates/cxxlibrary.cmake.template
+jolt/templates/export.sh.template
+jolt/templates/timeline.html.template
```

