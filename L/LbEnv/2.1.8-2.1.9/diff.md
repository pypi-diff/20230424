# Comparing `tmp/LbEnv-2.1.8.tar.gz` & `tmp/LbEnv-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "public/LbEnv-2.1.8.tar", last modified: Thu Dec  9 09:51:51 2021, max compression
+gzip compressed data, was "public/LbEnv-2.1.9.tar", last modified: Wed Feb 23 15:52:26 2022, max compression
```

## Comparing `LbEnv-2.1.8.tar` & `LbEnv-2.1.9.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-09 09:51:51.000000 LbEnv-2.1.8/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-09 09:51:51.000000 LbEnv-2.1.8/.ci/
--rwxr-xr-x   0 root         (0) root         (0)      636 2021-12-09 09:51:48.000000 LbEnv-2.1.8/.ci/run_tests.sh
--rw-r--r--   0 root         (0) root         (0)      128 2021-12-09 09:51:48.000000 LbEnv-2.1.8/.coveragerc
--rw-r--r--   0 root         (0) root         (0)      260 2021-12-09 09:51:48.000000 LbEnv-2.1.8/.gitignore
--rw-r--r--   0 root         (0) root         (0)     4706 2021-12-09 09:51:48.000000 LbEnv-2.1.8/.gitlab-ci.yml
--rw-r--r--   0 root         (0) root         (0)    32472 2021-12-09 09:51:48.000000 LbEnv-2.1.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1050 2021-12-09 09:51:51.000000 LbEnv-2.1.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      132 2021-12-09 09:51:48.000000 LbEnv-2.1.8/README.rst
--rw-r--r--   0 root         (0) root         (0)       44 2021-12-09 09:51:48.000000 LbEnv-2.1.8/always-include-coverage.pth
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-09 09:51:51.000000 LbEnv-2.1.8/python/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-09 09:51:51.000000 LbEnv-2.1.8/python/LbEnv/
--rw-r--r--   0 root         (0) root         (0)     2274 2021-12-09 09:51:48.000000 LbEnv-2.1.8/python/LbEnv/Banner.py
--rw-r--r--   0 root         (0) root         (0)    11089 2021-12-09 09:51:48.000000 LbEnv-2.1.8/python/LbEnv/Bootstrap.py
--rw-r--r--   0 root         (0) root         (0)      934 2021-12-09 09:51:48.000000 LbEnv-2.1.8/python/LbEnv/Info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-09 09:51:51.000000 LbEnv-2.1.8/python/LbEnv/ProjectEnv/
--rw-r--r--   0 root         (0) root         (0)     5850 2021-12-09 09:51:48.000000 LbEnv-2.1.8/python/LbEnv/ProjectEnv/__init__.py
--rw-r--r--   0 root         (0) root         (0)    94917 2021-12-09 09:51:48.000000 LbEnv-2.1.8/python/LbEnv/ProjectEnv/compatibility.py
--rw-r--r--   0 root         (0) root         (0)    27340 2021-12-09 09:51:48.000000 LbEnv-2.1.8/python/LbEnv/ProjectEnv/lookup.py
--rw-r--r--   0 root         (0) root         (0)    14460 2021-12-09 09:51:48.000000 LbEnv-2.1.8/python/LbEnv/ProjectEnv/options.py
--rw-r--r--   0 root         (0) root         (0)     9450 2021-12-09 09:51:48.000000 LbEnv-2.1.8/python/LbEnv/ProjectEnv/options_old.py
--rw-r--r--   0 root         (0) root         (0)     1912 2021-12-09 09:51:48.000000 LbEnv-2.1.8/python/LbEnv/ProjectEnv/profiling.py
--rw-r--r--   0 root         (0) root         (0)    43716 2021-12-09 09:51:48.000000 LbEnv-2.1.8/python/LbEnv/ProjectEnv/script.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-09 09:51:51.000000 LbEnv-2.1.8/python/LbEnv/ProjectEnv/tests/
--rw-r--r--   0 root         (0) root         (0)    24333 2021-12-09 09:51:48.000000 LbEnv-2.1.8/python/LbEnv/ProjectEnv/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-09 09:51:51.000000 LbEnv-2.1.8/python/LbEnv/ProjectEnv/tests/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-09 09:51:51.000000 LbEnv-2.1.8/python/LbEnv/ProjectEnv/tests/data/GAUDI/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-09 09:51:51.000000 LbEnv-2.1.8/python/LbEnv/ProjectEnv/tests/data/GAUDI/GAUDI_v24r0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-09 09:51:51.000000 LbEnv-2.1.8/python/LbEnv/ProjectEnv/tests/data/GAUDI/GAUDI_v24r0/InstallArea/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-09 09:51:51.000000 LbEnv-2.1.8/python/LbEnv/ProjectEnv/tests/data/GAUDI/GAUDI_v24r0/InstallArea/x86_64-slc6-gcc46-opt/
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-09 09:51:48.000000 LbEnv-2.1.8/python/LbEnv/ProjectEnv/tests/data/GAUDI/GAUDI_v24r0/InstallArea/x86_64-slc6-gcc46-opt/.empty
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-09 09:51:51.000000 LbEnv-2.1.8/python/LbEnv/ProjectEnv/tests/data/GAUDI/GAUDI_v24r1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-09 09:51:51.000000 LbEnv-2.1.8/python/LbEnv/ProjectEnv/tests/data/GAUDI/GAUDI_v24r1/InstallArea/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-09 09:51:51.000000 LbEnv-2.1.8/python/LbEnv/ProjectEnv/tests/data/GAUDI/GAUDI_v24r1/InstallArea/x86_64-slc6-gcc46-opt/
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-09 09:51:48.000000 LbEnv-2.1.8/python/LbEnv/ProjectEnv/tests/data/GAUDI/GAUDI_v24r1/InstallArea/x86_64-slc6-gcc46-opt/.empty
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-09 09:51:51.000000 LbEnv-2.1.8/python/LbEnv/ProjectEnv/tests/data/GAUDI/GAUDI_v25r0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-09 09:51:51.000000 LbEnv-2.1.8/python/LbEnv/ProjectEnv/tests/data/GAUDI/GAUDI_v25r0/InstallArea/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-09 09:51:51.000000 LbEnv-2.1.8/python/LbEnv/ProjectEnv/tests/data/GAUDI/GAUDI_v25r0/InstallArea/x86_64-slc6-gcc46-opt/
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-09 09:51:48.000000 LbEnv-2.1.8/python/LbEnv/ProjectEnv/tests/data/GAUDI/GAUDI_v25r0/InstallArea/x86_64-slc6-gcc46-opt/.empty
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-09 09:51:51.000000 LbEnv-2.1.8/python/LbEnv/ProjectEnv/tests/data/GAUDI/GAUDI_v26r0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-09 09:51:51.000000 LbEnv-2.1.8/python/LbEnv/ProjectEnv/tests/data/GAUDI/GAUDI_v26r0/InstallArea/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-09 09:51:51.000000 LbEnv-2.1.8/python/LbEnv/ProjectEnv/tests/data/GAUDI/GAUDI_v26r0/InstallArea/x86_64-slc6-gcc62-opt/
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-09 09:51:48.000000 LbEnv-2.1.8/python/LbEnv/ProjectEnv/tests/data/GAUDI/GAUDI_v26r0/InstallArea/x86_64-slc6-gcc62-opt/.empty
--rw-r--r--   0 root         (0) root         (0)     7926 2021-12-09 09:51:48.000000 LbEnv-2.1.8/python/LbEnv/ProjectEnv/tests/test_integration.py
--rw-r--r--   0 root         (0) root         (0)     3103 2021-12-09 09:51:48.000000 LbEnv-2.1.8/python/LbEnv/ProjectEnv/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-09 09:51:51.000000 LbEnv-2.1.8/python/LbEnv/Utils/
--rw-r--r--   0 root         (0) root         (0)     3562 2021-12-09 09:51:48.000000 LbEnv-2.1.8/python/LbEnv/Utils/Completion.py
--rw-r--r--   0 root         (0) root         (0)     4968 2021-12-09 09:51:48.000000 LbEnv-2.1.8/python/LbEnv/Utils/Temporary.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-09 09:51:48.000000 LbEnv-2.1.8/python/LbEnv/Utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2879 2021-12-09 09:51:48.000000 LbEnv-2.1.8/python/LbEnv/__init__.py
--rw-r--r--   0 root         (0) root         (0)      923 2021-12-09 09:51:48.000000 LbEnv-2.1.8/python/LbEnv/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-09 09:51:51.000000 LbEnv-2.1.8/python/LbEnv/data/
--rw-r--r--   0 root         (0) root         (0)     1488 2021-12-09 09:51:48.000000 LbEnv-2.1.8/python/LbEnv/data/aliases.csh
--rw-r--r--   0 root         (0) root         (0)     2794 2021-12-09 09:51:48.000000 LbEnv-2.1.8/python/LbEnv/data/aliases.sh
--rw-r--r--   0 root         (0) root         (0)      772 2021-12-09 09:51:48.000000 LbEnv-2.1.8/python/LbEnv/data/packages.txt
--rw-r--r--   0 root         (0) root         (0)      498 2021-12-09 09:51:48.000000 LbEnv-2.1.8/python/LbEnv/data/projects.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-09 09:51:51.000000 LbEnv-2.1.8/python/LbEnv/tests/
--rw-r--r--   0 root         (0) root         (0)     5686 2021-12-09 09:51:48.000000 LbEnv-2.1.8/python/LbEnv/tests/test_LbEnv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-09 09:51:51.000000 LbEnv-2.1.8/python/LbEnv.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1050 2021-12-09 09:51:50.000000 LbEnv-2.1.8/python/LbEnv.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1800 2021-12-09 09:51:51.000000 LbEnv-2.1.8/python/LbEnv.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-12-09 09:51:51.000000 LbEnv-2.1.8/python/LbEnv.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2021-12-09 09:51:51.000000 LbEnv-2.1.8/python/LbEnv.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-12-09 09:51:51.000000 LbEnv-2.1.8/python/LbEnv.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       38 2021-12-09 09:51:51.000000 LbEnv-2.1.8/python/LbEnv.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2021-12-09 09:51:51.000000 LbEnv-2.1.8/python/LbEnv.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      151 2021-12-09 09:51:51.000000 LbEnv-2.1.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     7915 2021-12-09 09:51:48.000000 LbEnv-2.1.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-09 09:51:51.000000 LbEnv-2.1.8/shell-completion/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-09 09:51:51.000000 LbEnv-2.1.8/shell-completion/bash/
--rw-r--r--   0 root         (0) root         (0)     1310 2021-12-09 09:51:48.000000 LbEnv-2.1.8/shell-completion/bash/LbEnv_helpers
--rw-r--r--   0 root         (0) root         (0)     2647 2021-12-09 09:51:48.000000 LbEnv-2.1.8/shell-completion/bash/_lb-run
--rw-r--r--   0 root         (0) root         (0)     1096 2021-12-09 09:51:48.000000 LbEnv-2.1.8/shell-completion/bash/_lb-set-platform
--rw-r--r--   0 root         (0) root         (0)     1561 2021-12-09 09:51:48.000000 LbEnv-2.1.8/shell-completion/bash_completion
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-09 09:51:51.000000 LbEnv-2.1.8/shell-completion/zsh/
--rw-r--r--   0 root         (0) root         (0)     3348 2021-12-09 09:51:48.000000 LbEnv-2.1.8/shell-completion/zsh/README.md
--rw-r--r--   0 root         (0) root         (0)     8702 2021-12-09 09:51:48.000000 LbEnv-2.1.8/shell-completion/zsh/_lb-run
--rw-r--r--   0 root         (0) root         (0)      780 2021-12-09 09:51:48.000000 LbEnv-2.1.8/shell-completion/zsh/_lb-set-platform
--rw-r--r--   0 root         (0) root         (0)     3680 2021-12-09 09:51:48.000000 LbEnv-2.1.8/shell-completion/zsh_completion
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-09 09:51:51.000000 LbEnv-2.1.8/utils/
--rwxr-xr-x   0 root         (0) root         (0)     2305 2021-12-09 09:51:48.000000 LbEnv-2.1.8/utils/list_gitlab_datapkgs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-23 15:52:26.000000 LbEnv-2.1.9/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-23 15:52:26.000000 LbEnv-2.1.9/.ci/
+-rwxr-xr-x   0 root         (0) root         (0)      636 2022-02-23 15:52:23.000000 LbEnv-2.1.9/.ci/run_tests.sh
+-rw-r--r--   0 root         (0) root         (0)      128 2022-02-23 15:52:23.000000 LbEnv-2.1.9/.coveragerc
+-rw-r--r--   0 root         (0) root         (0)      260 2022-02-23 15:52:23.000000 LbEnv-2.1.9/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     4706 2022-02-23 15:52:23.000000 LbEnv-2.1.9/.gitlab-ci.yml
+-rw-r--r--   0 root         (0) root         (0)    32472 2022-02-23 15:52:23.000000 LbEnv-2.1.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1050 2022-02-23 15:52:26.000000 LbEnv-2.1.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      132 2022-02-23 15:52:23.000000 LbEnv-2.1.9/README.rst
+-rw-r--r--   0 root         (0) root         (0)       44 2022-02-23 15:52:23.000000 LbEnv-2.1.9/always-include-coverage.pth
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-23 15:52:26.000000 LbEnv-2.1.9/python/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-23 15:52:26.000000 LbEnv-2.1.9/python/LbEnv/
+-rw-r--r--   0 root         (0) root         (0)     2274 2022-02-23 15:52:23.000000 LbEnv-2.1.9/python/LbEnv/Banner.py
+-rw-r--r--   0 root         (0) root         (0)    11138 2022-02-23 15:52:23.000000 LbEnv-2.1.9/python/LbEnv/Bootstrap.py
+-rw-r--r--   0 root         (0) root         (0)      934 2022-02-23 15:52:23.000000 LbEnv-2.1.9/python/LbEnv/Info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-23 15:52:26.000000 LbEnv-2.1.9/python/LbEnv/ProjectEnv/
+-rw-r--r--   0 root         (0) root         (0)     5850 2022-02-23 15:52:23.000000 LbEnv-2.1.9/python/LbEnv/ProjectEnv/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    94917 2022-02-23 15:52:23.000000 LbEnv-2.1.9/python/LbEnv/ProjectEnv/compatibility.py
+-rw-r--r--   0 root         (0) root         (0)    27340 2022-02-23 15:52:23.000000 LbEnv-2.1.9/python/LbEnv/ProjectEnv/lookup.py
+-rw-r--r--   0 root         (0) root         (0)    14460 2022-02-23 15:52:23.000000 LbEnv-2.1.9/python/LbEnv/ProjectEnv/options.py
+-rw-r--r--   0 root         (0) root         (0)     9450 2022-02-23 15:52:23.000000 LbEnv-2.1.9/python/LbEnv/ProjectEnv/options_old.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2022-02-23 15:52:23.000000 LbEnv-2.1.9/python/LbEnv/ProjectEnv/profiling.py
+-rw-r--r--   0 root         (0) root         (0)    43716 2022-02-23 15:52:23.000000 LbEnv-2.1.9/python/LbEnv/ProjectEnv/script.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-23 15:52:26.000000 LbEnv-2.1.9/python/LbEnv/ProjectEnv/tests/
+-rw-r--r--   0 root         (0) root         (0)    24333 2022-02-23 15:52:23.000000 LbEnv-2.1.9/python/LbEnv/ProjectEnv/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-23 15:52:26.000000 LbEnv-2.1.9/python/LbEnv/ProjectEnv/tests/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-23 15:52:26.000000 LbEnv-2.1.9/python/LbEnv/ProjectEnv/tests/data/GAUDI/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-23 15:52:26.000000 LbEnv-2.1.9/python/LbEnv/ProjectEnv/tests/data/GAUDI/GAUDI_v24r0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-23 15:52:26.000000 LbEnv-2.1.9/python/LbEnv/ProjectEnv/tests/data/GAUDI/GAUDI_v24r0/InstallArea/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-23 15:52:26.000000 LbEnv-2.1.9/python/LbEnv/ProjectEnv/tests/data/GAUDI/GAUDI_v24r0/InstallArea/x86_64-slc6-gcc46-opt/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-02-23 15:52:23.000000 LbEnv-2.1.9/python/LbEnv/ProjectEnv/tests/data/GAUDI/GAUDI_v24r0/InstallArea/x86_64-slc6-gcc46-opt/.empty
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-23 15:52:26.000000 LbEnv-2.1.9/python/LbEnv/ProjectEnv/tests/data/GAUDI/GAUDI_v24r1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-23 15:52:26.000000 LbEnv-2.1.9/python/LbEnv/ProjectEnv/tests/data/GAUDI/GAUDI_v24r1/InstallArea/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-23 15:52:26.000000 LbEnv-2.1.9/python/LbEnv/ProjectEnv/tests/data/GAUDI/GAUDI_v24r1/InstallArea/x86_64-slc6-gcc46-opt/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-02-23 15:52:23.000000 LbEnv-2.1.9/python/LbEnv/ProjectEnv/tests/data/GAUDI/GAUDI_v24r1/InstallArea/x86_64-slc6-gcc46-opt/.empty
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-23 15:52:26.000000 LbEnv-2.1.9/python/LbEnv/ProjectEnv/tests/data/GAUDI/GAUDI_v25r0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-23 15:52:26.000000 LbEnv-2.1.9/python/LbEnv/ProjectEnv/tests/data/GAUDI/GAUDI_v25r0/InstallArea/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-23 15:52:26.000000 LbEnv-2.1.9/python/LbEnv/ProjectEnv/tests/data/GAUDI/GAUDI_v25r0/InstallArea/x86_64-slc6-gcc46-opt/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-02-23 15:52:23.000000 LbEnv-2.1.9/python/LbEnv/ProjectEnv/tests/data/GAUDI/GAUDI_v25r0/InstallArea/x86_64-slc6-gcc46-opt/.empty
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-23 15:52:26.000000 LbEnv-2.1.9/python/LbEnv/ProjectEnv/tests/data/GAUDI/GAUDI_v26r0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-23 15:52:26.000000 LbEnv-2.1.9/python/LbEnv/ProjectEnv/tests/data/GAUDI/GAUDI_v26r0/InstallArea/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-23 15:52:26.000000 LbEnv-2.1.9/python/LbEnv/ProjectEnv/tests/data/GAUDI/GAUDI_v26r0/InstallArea/x86_64-slc6-gcc62-opt/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-02-23 15:52:23.000000 LbEnv-2.1.9/python/LbEnv/ProjectEnv/tests/data/GAUDI/GAUDI_v26r0/InstallArea/x86_64-slc6-gcc62-opt/.empty
+-rw-r--r--   0 root         (0) root         (0)     7926 2022-02-23 15:52:23.000000 LbEnv-2.1.9/python/LbEnv/ProjectEnv/tests/test_integration.py
+-rw-r--r--   0 root         (0) root         (0)     3103 2022-02-23 15:52:23.000000 LbEnv-2.1.9/python/LbEnv/ProjectEnv/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-23 15:52:26.000000 LbEnv-2.1.9/python/LbEnv/Utils/
+-rw-r--r--   0 root         (0) root         (0)     3562 2022-02-23 15:52:23.000000 LbEnv-2.1.9/python/LbEnv/Utils/Completion.py
+-rw-r--r--   0 root         (0) root         (0)     4968 2022-02-23 15:52:23.000000 LbEnv-2.1.9/python/LbEnv/Utils/Temporary.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-02-23 15:52:23.000000 LbEnv-2.1.9/python/LbEnv/Utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2879 2022-02-23 15:52:23.000000 LbEnv-2.1.9/python/LbEnv/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      923 2022-02-23 15:52:23.000000 LbEnv-2.1.9/python/LbEnv/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-23 15:52:26.000000 LbEnv-2.1.9/python/LbEnv/data/
+-rw-r--r--   0 root         (0) root         (0)     1488 2022-02-23 15:52:23.000000 LbEnv-2.1.9/python/LbEnv/data/aliases.csh
+-rw-r--r--   0 root         (0) root         (0)     2794 2022-02-23 15:52:23.000000 LbEnv-2.1.9/python/LbEnv/data/aliases.sh
+-rw-r--r--   0 root         (0) root         (0)      772 2022-02-23 15:52:23.000000 LbEnv-2.1.9/python/LbEnv/data/packages.txt
+-rw-r--r--   0 root         (0) root         (0)      498 2022-02-23 15:52:23.000000 LbEnv-2.1.9/python/LbEnv/data/projects.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-23 15:52:26.000000 LbEnv-2.1.9/python/LbEnv/tests/
+-rw-r--r--   0 root         (0) root         (0)     5686 2022-02-23 15:52:23.000000 LbEnv-2.1.9/python/LbEnv/tests/test_LbEnv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-23 15:52:26.000000 LbEnv-2.1.9/python/LbEnv.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1050 2022-02-23 15:52:26.000000 LbEnv-2.1.9/python/LbEnv.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1800 2022-02-23 15:52:26.000000 LbEnv-2.1.9/python/LbEnv.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-02-23 15:52:26.000000 LbEnv-2.1.9/python/LbEnv.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2022-02-23 15:52:26.000000 LbEnv-2.1.9/python/LbEnv.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-02-23 15:52:26.000000 LbEnv-2.1.9/python/LbEnv.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       38 2022-02-23 15:52:26.000000 LbEnv-2.1.9/python/LbEnv.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2022-02-23 15:52:26.000000 LbEnv-2.1.9/python/LbEnv.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      151 2022-02-23 15:52:26.000000 LbEnv-2.1.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     7915 2022-02-23 15:52:23.000000 LbEnv-2.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-23 15:52:26.000000 LbEnv-2.1.9/shell-completion/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-23 15:52:26.000000 LbEnv-2.1.9/shell-completion/bash/
+-rw-r--r--   0 root         (0) root         (0)     1310 2022-02-23 15:52:23.000000 LbEnv-2.1.9/shell-completion/bash/LbEnv_helpers
+-rw-r--r--   0 root         (0) root         (0)     2647 2022-02-23 15:52:23.000000 LbEnv-2.1.9/shell-completion/bash/_lb-run
+-rw-r--r--   0 root         (0) root         (0)     1096 2022-02-23 15:52:23.000000 LbEnv-2.1.9/shell-completion/bash/_lb-set-platform
+-rw-r--r--   0 root         (0) root         (0)     1561 2022-02-23 15:52:23.000000 LbEnv-2.1.9/shell-completion/bash_completion
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-23 15:52:26.000000 LbEnv-2.1.9/shell-completion/zsh/
+-rw-r--r--   0 root         (0) root         (0)     3348 2022-02-23 15:52:23.000000 LbEnv-2.1.9/shell-completion/zsh/README.md
+-rw-r--r--   0 root         (0) root         (0)     8702 2022-02-23 15:52:23.000000 LbEnv-2.1.9/shell-completion/zsh/_lb-run
+-rw-r--r--   0 root         (0) root         (0)      780 2022-02-23 15:52:23.000000 LbEnv-2.1.9/shell-completion/zsh/_lb-set-platform
+-rw-r--r--   0 root         (0) root         (0)     3680 2022-02-23 15:52:23.000000 LbEnv-2.1.9/shell-completion/zsh_completion
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-23 15:52:26.000000 LbEnv-2.1.9/utils/
+-rwxr-xr-x   0 root         (0) root         (0)     2305 2022-02-23 15:52:23.000000 LbEnv-2.1.9/utils/list_gitlab_datapkgs.py
```

### Comparing `LbEnv-2.1.8/.ci/run_tests.sh` & `LbEnv-2.1.9/.ci/run_tests.sh`

 * *Files identical despite different names*

### Comparing `LbEnv-2.1.8/.gitlab-ci.yml` & `LbEnv-2.1.9/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `LbEnv-2.1.8/LICENSE` & `LbEnv-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `LbEnv-2.1.8/PKG-INFO` & `LbEnv-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LbEnv
-Version: 2.1.8
+Version: 2.1.9
 Summary: LHCb Environment tools
 Home-page: https://gitlab.cern.ch/lhcb-core/LbEnv
 Author: CERN - LHCb Core Software
 Author-email: lhcb-core-soft@cern.ch
 License: UNKNOWN
 Description: LbEnv
         =====
```

### Comparing `LbEnv-2.1.8/python/LbEnv/Banner.py` & `LbEnv-2.1.9/python/LbEnv/Banner.py`

 * *Files identical despite different names*

### Comparing `LbEnv-2.1.8/python/LbEnv/Bootstrap.py` & `LbEnv-2.1.9/python/LbEnv/Bootstrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,15 +175,16 @@
     args = parser.parse_args()
 
     if os.environ.get("LBENV_SOURCED"):
         # LbEnv already called, do not run again
         return
 
     # Check if the existing MANPATH ends with ":" (which has a very special meaning)
-    manpath_with_default = os.environ.get("MANPATH", ":").endswith(":")
+    manpath = os.environ.get("MANPATH", ":")
+    manpath_with_default = manpath.endswith(":") or manpath.startswith(":")
 
     import LbEnv
     import LbPlatformUtils
     from xenv.Control import Environment
 
     control = Environment()
     control.presetFromSystem()
```

### Comparing `LbEnv-2.1.8/python/LbEnv/Info.py` & `LbEnv-2.1.9/python/LbEnv/Info.py`

 * *Files identical despite different names*

### Comparing `LbEnv-2.1.8/python/LbEnv/ProjectEnv/__init__.py` & `LbEnv-2.1.9/python/LbEnv/ProjectEnv/__init__.py`

 * *Files identical despite different names*

### Comparing `LbEnv-2.1.8/python/LbEnv/ProjectEnv/compatibility.py` & `LbEnv-2.1.9/python/LbEnv/ProjectEnv/compatibility.py`

 * *Files identical despite different names*

### Comparing `LbEnv-2.1.8/python/LbEnv/ProjectEnv/lookup.py` & `LbEnv-2.1.9/python/LbEnv/ProjectEnv/lookup.py`

 * *Files identical despite different names*

### Comparing `LbEnv-2.1.8/python/LbEnv/ProjectEnv/options.py` & `LbEnv-2.1.9/python/LbEnv/ProjectEnv/options.py`

 * *Files identical despite different names*

### Comparing `LbEnv-2.1.8/python/LbEnv/ProjectEnv/options_old.py` & `LbEnv-2.1.9/python/LbEnv/ProjectEnv/options_old.py`

 * *Files identical despite different names*

### Comparing `LbEnv-2.1.8/python/LbEnv/ProjectEnv/profiling.py` & `LbEnv-2.1.9/python/LbEnv/ProjectEnv/profiling.py`

 * *Files identical despite different names*

### Comparing `LbEnv-2.1.8/python/LbEnv/ProjectEnv/script.py` & `LbEnv-2.1.9/python/LbEnv/ProjectEnv/script.py`

 * *Files identical despite different names*

### Comparing `LbEnv-2.1.8/python/LbEnv/ProjectEnv/tests/__init__.py` & `LbEnv-2.1.9/python/LbEnv/ProjectEnv/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `LbEnv-2.1.8/python/LbEnv/ProjectEnv/tests/test_integration.py` & `LbEnv-2.1.9/python/LbEnv/ProjectEnv/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `LbEnv-2.1.8/python/LbEnv/ProjectEnv/version.py` & `LbEnv-2.1.9/python/LbEnv/ProjectEnv/version.py`

 * *Files identical despite different names*

### Comparing `LbEnv-2.1.8/python/LbEnv/Utils/Completion.py` & `LbEnv-2.1.9/python/LbEnv/Utils/Completion.py`

 * *Files identical despite different names*

### Comparing `LbEnv-2.1.8/python/LbEnv/Utils/Temporary.py` & `LbEnv-2.1.9/python/LbEnv/Utils/Temporary.py`

 * *Files identical despite different names*

### Comparing `LbEnv-2.1.8/python/LbEnv/__init__.py` & `LbEnv-2.1.9/python/LbEnv/__init__.py`

 * *Files identical despite different names*

### Comparing `LbEnv-2.1.8/python/LbEnv/__main__.py` & `LbEnv-2.1.9/python/LbEnv/__main__.py`

 * *Files identical despite different names*

### Comparing `LbEnv-2.1.8/python/LbEnv/data/aliases.csh` & `LbEnv-2.1.9/python/LbEnv/data/aliases.csh`

 * *Files identical despite different names*

### Comparing `LbEnv-2.1.8/python/LbEnv/data/aliases.sh` & `LbEnv-2.1.9/python/LbEnv/data/aliases.sh`

 * *Files identical despite different names*

### Comparing `LbEnv-2.1.8/python/LbEnv/data/packages.txt` & `LbEnv-2.1.9/python/LbEnv/data/packages.txt`

 * *Files identical despite different names*

### Comparing `LbEnv-2.1.8/python/LbEnv/tests/test_LbEnv.py` & `LbEnv-2.1.9/python/LbEnv/tests/test_LbEnv.py`

 * *Files identical despite different names*

### Comparing `LbEnv-2.1.8/python/LbEnv.egg-info/PKG-INFO` & `LbEnv-2.1.9/python/LbEnv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LbEnv
-Version: 2.1.8
+Version: 2.1.9
 Summary: LHCb Environment tools
 Home-page: https://gitlab.cern.ch/lhcb-core/LbEnv
 Author: CERN - LHCb Core Software
 Author-email: lhcb-core-soft@cern.ch
 License: UNKNOWN
 Description: LbEnv
         =====
```

### Comparing `LbEnv-2.1.8/python/LbEnv.egg-info/SOURCES.txt` & `LbEnv-2.1.9/python/LbEnv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LbEnv-2.1.8/setup.py` & `LbEnv-2.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `LbEnv-2.1.8/shell-completion/bash/LbEnv_helpers` & `LbEnv-2.1.9/shell-completion/bash/LbEnv_helpers`

 * *Files identical despite different names*

### Comparing `LbEnv-2.1.8/shell-completion/bash/_lb-run` & `LbEnv-2.1.9/shell-completion/bash/_lb-run`

 * *Files identical despite different names*

### Comparing `LbEnv-2.1.8/shell-completion/bash/_lb-set-platform` & `LbEnv-2.1.9/shell-completion/bash/_lb-set-platform`

 * *Files identical despite different names*

### Comparing `LbEnv-2.1.8/shell-completion/bash_completion` & `LbEnv-2.1.9/shell-completion/bash_completion`

 * *Files identical despite different names*

### Comparing `LbEnv-2.1.8/shell-completion/zsh/README.md` & `LbEnv-2.1.9/shell-completion/zsh/README.md`

 * *Files identical despite different names*

### Comparing `LbEnv-2.1.8/shell-completion/zsh/_lb-run` & `LbEnv-2.1.9/shell-completion/zsh/_lb-run`

 * *Files identical despite different names*

### Comparing `LbEnv-2.1.8/shell-completion/zsh/_lb-set-platform` & `LbEnv-2.1.9/shell-completion/zsh/_lb-set-platform`

 * *Files identical despite different names*

### Comparing `LbEnv-2.1.8/shell-completion/zsh_completion` & `LbEnv-2.1.9/shell-completion/zsh_completion`

 * *Files identical despite different names*

### Comparing `LbEnv-2.1.8/utils/list_gitlab_datapkgs.py` & `LbEnv-2.1.9/utils/list_gitlab_datapkgs.py`

 * *Files identical despite different names*

