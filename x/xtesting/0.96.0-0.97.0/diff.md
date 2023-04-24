# Comparing `tmp/xtesting-0.96.0.tar.gz` & `tmp/xtesting-0.97.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtesting-0.96.0.tar", last modified: Fri Mar  4 10:11:15 2022, max compression
+gzip compressed data, was "xtesting-0.97.0.tar", last modified: Mon Apr 24 13:12:21 2023, max compression
```

## Comparing `xtesting-0.96.0.tar` & `xtesting-0.97.0.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2022-03-04 10:11:15.069116 xtesting-0.96.0/
-drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2022-03-04 10:11:15.057116 xtesting-0.96.0/.circleci/
--rw-r--r--   0 cedric    (1000) cedric    (1000)      449 2022-03-04 10:10:09.000000 xtesting-0.96.0/.circleci/config.yml
--rw-r--r--   0 cedric    (1000) cedric    (1000)       69 2021-02-20 08:02:47.000000 xtesting-0.96.0/.coveragerc
--rw-r--r--   0 cedric    (1000) cedric    (1000)       99 2018-03-23 21:18:00.000000 xtesting-0.96.0/.gitmodules
--rw-r--r--   0 cedric    (1000) cedric    (1000)     2321 2022-03-04 10:10:09.000000 xtesting-0.96.0/.travis.yml
--rw-r--r--   0 cedric    (1000) cedric    (1000)     4855 2022-03-04 10:11:11.000000 xtesting-0.96.0/AUTHORS
--rw-r--r--   0 cedric    (1000) cedric    (1000)   101556 2022-03-04 10:11:11.000000 xtesting-0.96.0/ChangeLog
--rw-r--r--   0 cedric    (1000) cedric    (1000)    11358 2018-02-26 20:08:32.000000 xtesting-0.96.0/LICENSE
--rw-r--r--   0 cedric    (1000) cedric    (1000)     1509 2022-03-04 10:11:15.069116 xtesting-0.96.0/PKG-INFO
--rw-r--r--   0 cedric    (1000) cedric    (1000)     5026 2021-02-17 22:59:47.000000 xtesting-0.96.0/README.md
--rw-r--r--   0 cedric    (1000) cedric    (1000)      854 2018-04-07 17:05:18.000000 xtesting-0.96.0/README.rst
-drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2022-03-04 10:11:15.057116 xtesting-0.96.0/ansible/
--rw-r--r--   0 cedric    (1000) cedric    (1000)      990 2022-03-04 10:10:09.000000 xtesting-0.96.0/ansible/site.gate.yml
--rw-r--r--   0 cedric    (1000) cedric    (1000)      340 2022-03-04 10:10:09.000000 xtesting-0.96.0/ansible/site.yml
-drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2022-03-04 10:11:15.061116 xtesting-0.96.0/api/
-drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2022-03-04 10:11:15.061116 xtesting-0.96.0/api/apidoc/
--rw-r--r--   0 cedric    (1000) cedric    (1000)       61 2018-02-28 14:23:15.000000 xtesting-0.96.0/api/apidoc/modules.rst
--rw-r--r--   0 cedric    (1000) cedric    (1000)      248 2018-02-28 14:23:15.000000 xtesting-0.96.0/api/apidoc/xtesting.ci.rst
--rw-r--r--   0 cedric    (1000) cedric    (1000)      160 2018-02-28 14:23:15.000000 xtesting-0.96.0/api/apidoc/xtesting.ci.run_tests.rst
--rw-r--r--   0 cedric    (1000) cedric    (1000)      169 2018-02-28 14:23:15.000000 xtesting-0.96.0/api/apidoc/xtesting.ci.tier_builder.rst
--rw-r--r--   0 cedric    (1000) cedric    (1000)      169 2018-02-28 14:23:15.000000 xtesting-0.96.0/api/apidoc/xtesting.ci.tier_handler.rst
--rw-r--r--   0 cedric    (1000) cedric    (1000)      182 2021-02-09 18:21:54.000000 xtesting-0.96.0/api/apidoc/xtesting.core.behaveframework.rst
--rw-r--r--   0 cedric    (1000) cedric    (1000)      158 2018-02-28 14:23:15.000000 xtesting-0.96.0/api/apidoc/xtesting.core.feature.rst
--rw-r--r--   0 cedric    (1000) cedric    (1000)      179 2018-02-28 14:23:15.000000 xtesting-0.96.0/api/apidoc/xtesting.core.robotframework.rst
--rw-r--r--   0 cedric    (1000) cedric    (1000)      332 2021-02-09 18:21:54.000000 xtesting-0.96.0/api/apidoc/xtesting.core.rst
--rw-r--r--   0 cedric    (1000) cedric    (1000)      161 2018-02-28 14:23:15.000000 xtesting-0.96.0/api/apidoc/xtesting.core.testcase.rst
--rw-r--r--   0 cedric    (1000) cedric    (1000)      149 2018-02-28 14:23:15.000000 xtesting-0.96.0/api/apidoc/xtesting.core.unit.rst
--rw-r--r--   0 cedric    (1000) cedric    (1000)      146 2018-02-28 14:23:15.000000 xtesting-0.96.0/api/apidoc/xtesting.core.vnf.rst
--rw-r--r--   0 cedric    (1000) cedric    (1000)      211 2021-02-20 08:02:47.000000 xtesting-0.96.0/api/apidoc/xtesting.rst
--rw-r--r--   0 cedric    (1000) cedric    (1000)      167 2018-02-28 14:23:15.000000 xtesting-0.96.0/api/apidoc/xtesting.utils.constants.rst
--rw-r--r--   0 cedric    (1000) cedric    (1000)      170 2018-02-28 14:23:15.000000 xtesting-0.96.0/api/apidoc/xtesting.utils.decorators.rst
--rw-r--r--   0 cedric    (1000) cedric    (1000)      149 2018-02-28 14:23:15.000000 xtesting-0.96.0/api/apidoc/xtesting.utils.env.rst
--rw-r--r--   0 cedric    (1000) cedric    (1000)      255 2018-02-28 14:23:15.000000 xtesting-0.96.0/api/apidoc/xtesting.utils.rst
--rw-r--r--   0 cedric    (1000) cedric    (1000)     9900 2018-04-04 05:01:05.000000 xtesting-0.96.0/api/conf.py
--rw-r--r--   0 cedric    (1000) cedric    (1000)     2158 2018-03-18 18:31:49.000000 xtesting-0.96.0/api/index.rst
--rw-r--r--   0 cedric    (1000) cedric    (1000)     1902 2022-03-04 10:10:09.000000 xtesting-0.96.0/build.sh
-drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2022-03-04 10:11:15.057116 xtesting-0.96.0/doc/
-drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2022-03-04 10:11:15.061116 xtesting-0.96.0/doc/cntt_rc_cookbook/
--rw-r--r--   0 cedric    (1000) cedric    (1000)     2412 2022-03-03 11:26:08.000000 xtesting-0.96.0/doc/cntt_rc_cookbook/cntt_rc_cookbook.md
--rw-r--r--   0 cedric    (1000) cedric    (1000)     1936 2022-03-03 11:26:08.000000 xtesting-0.96.0/doc/cntt_rc_cookbook/index.html
-drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2022-03-04 10:11:15.065116 xtesting-0.96.0/doc/ons2019/
--rw-r--r--   0 cedric    (1000) cedric    (1000)    95192 2021-02-20 08:02:47.000000 xtesting-0.96.0/doc/ons2019/chainedci.png
--rw-r--r--   0 cedric    (1000) cedric    (1000)   162001 2021-02-20 08:02:47.000000 xtesting-0.96.0/doc/ons2019/ftth.png
--rw-r--r--   0 cedric    (1000) cedric    (1000)     1933 2021-02-20 08:02:47.000000 xtesting-0.96.0/doc/ons2019/index.html
--rw-r--r--   0 cedric    (1000) cedric    (1000)     2639 2021-02-20 08:02:47.000000 xtesting-0.96.0/doc/ons2019/ons2019.md
-drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2022-03-04 10:11:15.065116 xtesting-0.96.0/doc/xtesting/
--rw-r--r--   0 cedric    (1000) cedric    (1000)    77673 2020-01-14 15:33:30.000000 xtesting-0.96.0/doc/xtesting/ONAP.png
--rw-r--r--   0 cedric    (1000) cedric    (1000)     1917 2020-01-14 15:33:30.000000 xtesting-0.96.0/doc/xtesting/index.html
--rw-r--r--   0 cedric    (1000) cedric    (1000)     6344 2020-01-14 15:33:30.000000 xtesting-0.96.0/doc/xtesting/xtesting.md
-drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2022-03-04 10:11:15.065116 xtesting-0.96.0/doc/xtesting2020/
--rw-r--r--   0 cedric    (1000) cedric    (1000)     1926 2022-03-03 11:26:08.000000 xtesting-0.96.0/doc/xtesting2020/index.html
--rw-r--r--   0 cedric    (1000) cedric    (1000)      800 2022-03-03 11:26:08.000000 xtesting-0.96.0/doc/xtesting2020/xtesting2020.md
-drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2022-03-04 10:11:15.057116 xtesting-0.96.0/docker/
-drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2022-03-04 10:11:15.065116 xtesting-0.96.0/docker/core/
--rw-r--r--   0 cedric    (1000) cedric    (1000)     1434 2022-03-04 10:10:09.000000 xtesting-0.96.0/docker/core/Dockerfile
--rw-r--r--   0 cedric    (1000) cedric    (1000)     2013 2022-03-04 10:10:09.000000 xtesting-0.96.0/docker/core/testcases.yaml
-drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2022-03-04 10:11:15.065116 xtesting-0.96.0/docker/mts/
--rw-r--r--   0 cedric    (1000) cedric    (1000)     1127 2022-03-04 10:10:09.000000 xtesting-0.96.0/docker/mts/Dockerfile
--rw-r--r--   0 cedric    (1000) cedric    (1000)       39 2021-02-09 18:31:06.000000 xtesting-0.96.0/docker/mts/mts-installer.properties
--rw-r--r--   0 cedric    (1000) cedric    (1000)      811 2022-03-04 10:10:09.000000 xtesting-0.96.0/docker/mts/testcases.yaml
--rw-r--r--   0 cedric    (1000) cedric    (1000)      665 2022-03-04 10:10:09.000000 xtesting-0.96.0/requirements.txt
--rw-r--r--   0 cedric    (1000) cedric    (1000)     1184 2022-03-04 10:11:15.069116 xtesting-0.96.0/setup.cfg
--rw-r--r--   0 cedric    (1000) cedric    (1000)      766 2022-03-03 11:26:08.000000 xtesting-0.96.0/setup.py
--rw-r--r--   0 cedric    (1000) cedric    (1000)      458 2022-03-04 10:10:09.000000 xtesting-0.96.0/test-requirements.txt
--rw-r--r--   0 cedric    (1000) cedric    (1000)     2141 2022-03-04 10:10:09.000000 xtesting-0.96.0/tox.ini
--rw-r--r--   0 cedric    (1000) cedric    (1000)      148 2022-03-04 10:10:09.000000 xtesting-0.96.0/upper-constraints.txt
-drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2022-03-04 10:11:15.065116 xtesting-0.96.0/xtesting/
--rw-r--r--   0 cedric    (1000) cedric    (1000)        0 2018-02-28 14:23:15.000000 xtesting-0.96.0/xtesting/__init__.py
-drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2022-03-04 10:11:15.065116 xtesting-0.96.0/xtesting/ci/
--rw-r--r--   0 cedric    (1000) cedric    (1000)        0 2018-02-28 14:23:15.000000 xtesting-0.96.0/xtesting/ci/__init__.py
--rw-r--r--   0 cedric    (1000) cedric    (1000)      935 2020-11-09 16:39:47.000000 xtesting-0.96.0/xtesting/ci/logging.debug.ini
--rw-r--r--   0 cedric    (1000) cedric    (1000)      886 2020-11-09 16:39:47.000000 xtesting-0.96.0/xtesting/ci/logging.ini
--rw-r--r--   0 cedric    (1000) cedric    (1000)    13944 2022-03-04 10:10:09.000000 xtesting-0.96.0/xtesting/ci/run_tests.py
--rw-r--r--   0 cedric    (1000) cedric    (1000)     2551 2022-03-04 10:02:45.000000 xtesting-0.96.0/xtesting/ci/testcases.yaml
--rw-r--r--   0 cedric    (1000) cedric    (1000)     4236 2022-03-04 10:10:09.000000 xtesting-0.96.0/xtesting/ci/tier_builder.py
--rw-r--r--   0 cedric    (1000) cedric    (1000)     3215 2022-03-04 10:10:09.000000 xtesting-0.96.0/xtesting/ci/tier_handler.py
-drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2022-03-04 10:11:15.069116 xtesting-0.96.0/xtesting/core/
--rw-r--r--   0 cedric    (1000) cedric    (1000)        0 2018-02-28 14:23:15.000000 xtesting-0.96.0/xtesting/core/__init__.py
--rw-r--r--   0 cedric    (1000) cedric    (1000)     2422 2022-03-03 13:43:25.000000 xtesting-0.96.0/xtesting/core/ansible.py
--rw-r--r--   0 cedric    (1000) cedric    (1000)     3909 2022-03-04 10:10:09.000000 xtesting-0.96.0/xtesting/core/behaveframework.py
--rw-r--r--   0 cedric    (1000) cedric    (1000)     9081 2022-03-04 10:10:09.000000 xtesting-0.96.0/xtesting/core/campaign.py
--rw-r--r--   0 cedric    (1000) cedric    (1000)     4268 2022-03-04 10:10:09.000000 xtesting-0.96.0/xtesting/core/feature.py
--rw-r--r--   0 cedric    (1000) cedric    (1000)    10253 2022-03-04 10:10:09.000000 xtesting-0.96.0/xtesting/core/mts.py
--rw-r--r--   0 cedric    (1000) cedric    (1000)     4499 2022-03-04 10:10:09.000000 xtesting-0.96.0/xtesting/core/robotframework.py
--rw-r--r--   0 cedric    (1000) cedric    (1000)    14047 2022-03-04 10:10:09.000000 xtesting-0.96.0/xtesting/core/testcase.py
--rw-r--r--   0 cedric    (1000) cedric    (1000)     4799 2022-03-04 10:10:09.000000 xtesting-0.96.0/xtesting/core/unit.py
--rw-r--r--   0 cedric    (1000) cedric    (1000)     5304 2022-03-04 10:10:09.000000 xtesting-0.96.0/xtesting/core/vnf.py
-drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2022-03-04 10:11:15.069116 xtesting-0.96.0/xtesting/samples/
--rw-r--r--   0 cedric    (1000) cedric    (1000)       58 2019-08-21 12:19:01.000000 xtesting-0.96.0/xtesting/samples/HelloWorld.robot
--rw-r--r--   0 cedric    (1000) cedric    (1000)        0 2018-02-28 14:23:15.000000 xtesting-0.96.0/xtesting/samples/__init__.py
-drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2022-03-04 10:11:15.069116 xtesting-0.96.0/xtesting/samples/features/
--rw-r--r--   0 cedric    (1000) cedric    (1000)      172 2021-02-09 18:21:54.000000 xtesting-0.96.0/xtesting/samples/features/hello.feature
-drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2022-03-04 10:11:15.069116 xtesting-0.96.0/xtesting/samples/features/steps/
--rw-r--r--   0 cedric    (1000) cedric    (1000)      362 2021-02-09 18:21:54.000000 xtesting-0.96.0/xtesting/samples/features/steps/hello.py
--rw-r--r--   0 cedric    (1000) cedric    (1000)      587 2022-03-04 10:10:09.000000 xtesting-0.96.0/xtesting/samples/first.py
--rw-r--r--   0 cedric    (1000) cedric    (1000)      523 2018-02-28 14:23:15.000000 xtesting-0.96.0/xtesting/samples/fourth.py
--rw-r--r--   0 cedric    (1000) cedric    (1000)      107 2022-03-03 13:43:25.000000 xtesting-0.96.0/xtesting/samples/helloworld.yml
-drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2022-03-04 10:11:15.069116 xtesting-0.96.0/xtesting/samples/mts/
--rw-r--r--   0 cedric    (1000) cedric    (1000)      348 2022-03-04 10:10:09.000000 xtesting-0.96.0/xtesting/samples/mts/pause.xml
--rw-r--r--   0 cedric    (1000) cedric    (1000)      447 2022-03-04 10:10:09.000000 xtesting-0.96.0/xtesting/samples/mts/test.xml
--rw-r--r--   0 cedric    (1000) cedric    (1000)      491 2022-03-04 10:10:09.000000 xtesting-0.96.0/xtesting/samples/second.py
-drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2022-03-04 10:11:15.069116 xtesting-0.96.0/xtesting/tests/
--rw-r--r--   0 cedric    (1000) cedric    (1000)        0 2018-02-28 14:23:15.000000 xtesting-0.96.0/xtesting/tests/__init__.py
-drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2022-03-04 10:11:15.069116 xtesting-0.96.0/xtesting/tests/unit/
--rw-r--r--   0 cedric    (1000) cedric    (1000)        0 2018-02-28 14:23:15.000000 xtesting-0.96.0/xtesting/tests/unit/__init__.py
-drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2022-03-04 10:11:15.069116 xtesting-0.96.0/xtesting/tests/unit/ci/
--rw-r--r--   0 cedric    (1000) cedric    (1000)        0 2018-02-28 14:23:15.000000 xtesting-0.96.0/xtesting/tests/unit/ci/__init__.py
--rw-r--r--   0 cedric    (1000) cedric    (1000)    13216 2022-03-04 10:10:09.000000 xtesting-0.96.0/xtesting/tests/unit/ci/test_run_tests.py
--rw-r--r--   0 cedric    (1000) cedric    (1000)     3703 2022-03-04 10:10:09.000000 xtesting-0.96.0/xtesting/tests/unit/ci/test_tier_builder.py
--rw-r--r--   0 cedric    (1000) cedric    (1000)     2778 2022-03-04 10:10:09.000000 xtesting-0.96.0/xtesting/tests/unit/ci/test_tier_handler.py
-drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2022-03-04 10:11:15.069116 xtesting-0.96.0/xtesting/tests/unit/core/
--rw-r--r--   0 cedric    (1000) cedric    (1000)        0 2018-02-28 14:23:15.000000 xtesting-0.96.0/xtesting/tests/unit/core/__init__.py
--rw-r--r--   0 cedric    (1000) cedric    (1000)     8155 2022-03-03 13:43:25.000000 xtesting-0.96.0/xtesting/tests/unit/core/test_ansible.py
--rw-r--r--   0 cedric    (1000) cedric    (1000)     6698 2022-03-04 10:10:09.000000 xtesting-0.96.0/xtesting/tests/unit/core/test_behaveframework.py
--rw-r--r--   0 cedric    (1000) cedric    (1000)    10548 2022-03-04 10:10:09.000000 xtesting-0.96.0/xtesting/tests/unit/core/test_feature.py
--rw-r--r--   0 cedric    (1000) cedric    (1000)    11775 2022-03-04 10:10:09.000000 xtesting-0.96.0/xtesting/tests/unit/core/test_robotframework.py
--rw-r--r--   0 cedric    (1000) cedric    (1000)    18739 2022-03-04 10:10:09.000000 xtesting-0.96.0/xtesting/tests/unit/core/test_testcase.py
--rw-r--r--   0 cedric    (1000) cedric    (1000)    10370 2022-03-04 10:10:09.000000 xtesting-0.96.0/xtesting/tests/unit/core/test_unit.py
--rw-r--r--   0 cedric    (1000) cedric    (1000)     5603 2018-02-28 14:23:15.000000 xtesting-0.96.0/xtesting/tests/unit/core/test_vnf.py
-drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2022-03-04 10:11:15.069116 xtesting-0.96.0/xtesting/tests/unit/utils/
--rw-r--r--   0 cedric    (1000) cedric    (1000)        0 2018-02-28 14:23:15.000000 xtesting-0.96.0/xtesting/tests/unit/utils/__init__.py
--rw-r--r--   0 cedric    (1000) cedric    (1000)     4616 2022-03-04 10:10:09.000000 xtesting-0.96.0/xtesting/tests/unit/utils/test_decorators.py
--rw-r--r--   0 cedric    (1000) cedric    (1000)     1479 2022-03-04 10:10:09.000000 xtesting-0.96.0/xtesting/tests/unit/utils/test_env.py
-drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2022-03-04 10:11:15.069116 xtesting-0.96.0/xtesting/utils/
--rw-r--r--   0 cedric    (1000) cedric    (1000)        0 2018-02-28 14:23:15.000000 xtesting-0.96.0/xtesting/utils/__init__.py
--rw-r--r--   0 cedric    (1000) cedric    (1000)      729 2022-03-04 10:02:45.000000 xtesting-0.96.0/xtesting/utils/config.py
--rw-r--r--   0 cedric    (1000) cedric    (1000)     1033 2022-03-04 10:02:45.000000 xtesting-0.96.0/xtesting/utils/constants.py
--rw-r--r--   0 cedric    (1000) cedric    (1000)     2001 2022-03-04 10:10:09.000000 xtesting-0.96.0/xtesting/utils/decorators.py
--rw-r--r--   0 cedric    (1000) cedric    (1000)     1171 2022-03-04 10:10:09.000000 xtesting-0.96.0/xtesting/utils/env.py
-drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2022-03-04 10:11:15.065116 xtesting-0.96.0/xtesting.egg-info/
--rw-r--r--   0 cedric    (1000) cedric    (1000)     1509 2022-03-04 10:11:11.000000 xtesting-0.96.0/xtesting.egg-info/PKG-INFO
--rw-r--r--   0 cedric    (1000) cedric    (1000)     3148 2022-03-04 10:11:15.000000 xtesting-0.96.0/xtesting.egg-info/SOURCES.txt
--rw-r--r--   0 cedric    (1000) cedric    (1000)        1 2022-03-04 10:11:11.000000 xtesting-0.96.0/xtesting.egg-info/dependency_links.txt
--rw-r--r--   0 cedric    (1000) cedric    (1000)      477 2022-03-04 10:11:11.000000 xtesting-0.96.0/xtesting.egg-info/entry_points.txt
--rw-r--r--   0 cedric    (1000) cedric    (1000)        1 2021-06-01 14:54:54.000000 xtesting-0.96.0/xtesting.egg-info/not-zip-safe
--rw-r--r--   0 cedric    (1000) cedric    (1000)       48 2022-03-04 10:11:11.000000 xtesting-0.96.0/xtesting.egg-info/pbr.json
--rw-r--r--   0 cedric    (1000) cedric    (1000)      342 2022-03-04 10:11:11.000000 xtesting-0.96.0/xtesting.egg-info/requires.txt
--rw-r--r--   0 cedric    (1000) cedric    (1000)        9 2022-03-04 10:11:11.000000 xtesting-0.96.0/xtesting.egg-info/top_level.txt
+drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2023-04-24 13:12:21.883233 xtesting-0.97.0/
+drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2023-04-24 13:12:21.871233 xtesting-0.97.0/.circleci/
+-rw-r--r--   0 cedric    (1000) cedric    (1000)      449 2023-04-18 13:03:00.000000 xtesting-0.97.0/.circleci/config.yml
+-rw-r--r--   0 cedric    (1000) cedric    (1000)       69 2021-02-20 08:02:47.000000 xtesting-0.97.0/.coveragerc
+-rw-r--r--   0 cedric    (1000) cedric    (1000)       99 2018-03-23 21:18:00.000000 xtesting-0.97.0/.gitmodules
+-rw-r--r--   0 cedric    (1000) cedric    (1000)      412 2023-04-18 13:03:00.000000 xtesting-0.97.0/.pre-commit-config.yaml
+-rw-r--r--   0 cedric    (1000) cedric    (1000)     1441 2023-04-24 13:10:15.000000 xtesting-0.97.0/.travis.yml
+-rw-r--r--   0 cedric    (1000) cedric    (1000)     4993 2023-04-24 13:12:21.000000 xtesting-0.97.0/AUTHORS
+-rw-r--r--   0 cedric    (1000) cedric    (1000)   102014 2023-04-24 13:12:21.000000 xtesting-0.97.0/ChangeLog
+-rw-r--r--   0 cedric    (1000) cedric    (1000)    11358 2018-02-26 20:08:32.000000 xtesting-0.97.0/LICENSE
+-rw-r--r--   0 cedric    (1000) cedric    (1000)     1472 2023-04-24 13:12:21.883233 xtesting-0.97.0/PKG-INFO
+-rw-r--r--   0 cedric    (1000) cedric    (1000)     5026 2021-02-17 22:59:47.000000 xtesting-0.97.0/README.md
+-rw-r--r--   0 cedric    (1000) cedric    (1000)      854 2018-04-07 17:05:18.000000 xtesting-0.97.0/README.rst
+drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2023-04-24 13:12:21.871233 xtesting-0.97.0/ansible/
+-rw-r--r--   0 cedric    (1000) cedric    (1000)      756 2023-04-24 13:10:15.000000 xtesting-0.97.0/ansible/site.gate.yml
+-rw-r--r--   0 cedric    (1000) cedric    (1000)      267 2023-04-18 13:03:00.000000 xtesting-0.97.0/ansible/site.yml
+drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2023-04-24 13:12:21.871233 xtesting-0.97.0/api/
+drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2023-04-24 13:12:21.875233 xtesting-0.97.0/api/apidoc/
+-rw-r--r--   0 cedric    (1000) cedric    (1000)       61 2022-04-22 20:48:17.000000 xtesting-0.97.0/api/apidoc/modules.rst
+-rw-r--r--   0 cedric    (1000) cedric    (1000)      248 2022-04-22 20:48:17.000000 xtesting-0.97.0/api/apidoc/xtesting.ci.rst
+-rw-r--r--   0 cedric    (1000) cedric    (1000)      160 2022-04-22 20:48:17.000000 xtesting-0.97.0/api/apidoc/xtesting.ci.run_tests.rst
+-rw-r--r--   0 cedric    (1000) cedric    (1000)      169 2022-04-22 20:48:17.000000 xtesting-0.97.0/api/apidoc/xtesting.ci.tier_builder.rst
+-rw-r--r--   0 cedric    (1000) cedric    (1000)      169 2022-04-22 20:48:17.000000 xtesting-0.97.0/api/apidoc/xtesting.ci.tier_handler.rst
+-rw-r--r--   0 cedric    (1000) cedric    (1000)      158 2023-04-13 11:05:30.000000 xtesting-0.97.0/api/apidoc/xtesting.core.ansible.rst
+-rw-r--r--   0 cedric    (1000) cedric    (1000)      182 2022-04-22 20:48:17.000000 xtesting-0.97.0/api/apidoc/xtesting.core.behaveframework.rst
+-rw-r--r--   0 cedric    (1000) cedric    (1000)      161 2023-04-13 11:05:30.000000 xtesting-0.97.0/api/apidoc/xtesting.core.campaign.rst
+-rw-r--r--   0 cedric    (1000) cedric    (1000)      158 2022-04-22 20:48:17.000000 xtesting-0.97.0/api/apidoc/xtesting.core.feature.rst
+-rw-r--r--   0 cedric    (1000) cedric    (1000)      155 2023-04-18 13:03:00.000000 xtesting-0.97.0/api/apidoc/xtesting.core.pytest.rst
+-rw-r--r--   0 cedric    (1000) cedric    (1000)      179 2022-04-22 20:48:17.000000 xtesting-0.97.0/api/apidoc/xtesting.core.robotframework.rst
+-rw-r--r--   0 cedric    (1000) cedric    (1000)      407 2023-04-18 13:03:00.000000 xtesting-0.97.0/api/apidoc/xtesting.core.rst
+-rw-r--r--   0 cedric    (1000) cedric    (1000)      161 2022-04-22 20:48:17.000000 xtesting-0.97.0/api/apidoc/xtesting.core.testcase.rst
+-rw-r--r--   0 cedric    (1000) cedric    (1000)      149 2022-04-22 20:48:17.000000 xtesting-0.97.0/api/apidoc/xtesting.core.unit.rst
+-rw-r--r--   0 cedric    (1000) cedric    (1000)      146 2022-04-22 20:48:17.000000 xtesting-0.97.0/api/apidoc/xtesting.core.vnf.rst
+-rw-r--r--   0 cedric    (1000) cedric    (1000)      211 2022-04-22 20:48:17.000000 xtesting-0.97.0/api/apidoc/xtesting.rst
+-rw-r--r--   0 cedric    (1000) cedric    (1000)      167 2022-04-22 20:48:17.000000 xtesting-0.97.0/api/apidoc/xtesting.utils.constants.rst
+-rw-r--r--   0 cedric    (1000) cedric    (1000)      170 2022-04-22 20:48:17.000000 xtesting-0.97.0/api/apidoc/xtesting.utils.decorators.rst
+-rw-r--r--   0 cedric    (1000) cedric    (1000)      149 2022-04-22 20:48:17.000000 xtesting-0.97.0/api/apidoc/xtesting.utils.env.rst
+-rw-r--r--   0 cedric    (1000) cedric    (1000)      255 2022-04-22 20:48:17.000000 xtesting-0.97.0/api/apidoc/xtesting.utils.rst
+-rw-r--r--   0 cedric    (1000) cedric    (1000)     9900 2022-04-22 20:48:17.000000 xtesting-0.97.0/api/conf.py
+-rw-r--r--   0 cedric    (1000) cedric    (1000)     2158 2022-04-22 20:48:17.000000 xtesting-0.97.0/api/index.rst
+-rw-r--r--   0 cedric    (1000) cedric    (1000)     1886 2023-04-24 13:10:15.000000 xtesting-0.97.0/build.sh
+drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2023-04-24 13:12:21.867233 xtesting-0.97.0/doc/
+drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2023-04-24 13:12:21.875233 xtesting-0.97.0/doc/cntt_rc_cookbook/
+-rw-r--r--   0 cedric    (1000) cedric    (1000)     2412 2022-04-12 08:13:45.000000 xtesting-0.97.0/doc/cntt_rc_cookbook/cntt_rc_cookbook.md
+-rw-r--r--   0 cedric    (1000) cedric    (1000)     1936 2022-04-12 08:13:45.000000 xtesting-0.97.0/doc/cntt_rc_cookbook/index.html
+drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2023-04-24 13:12:21.875233 xtesting-0.97.0/doc/ons2019/
+-rw-r--r--   0 cedric    (1000) cedric    (1000)    95192 2021-02-20 08:02:47.000000 xtesting-0.97.0/doc/ons2019/chainedci.png
+-rw-r--r--   0 cedric    (1000) cedric    (1000)   162001 2021-02-20 08:02:47.000000 xtesting-0.97.0/doc/ons2019/ftth.png
+-rw-r--r--   0 cedric    (1000) cedric    (1000)     1933 2021-02-20 08:02:47.000000 xtesting-0.97.0/doc/ons2019/index.html
+-rw-r--r--   0 cedric    (1000) cedric    (1000)     2639 2021-02-20 08:02:47.000000 xtesting-0.97.0/doc/ons2019/ons2019.md
+drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2023-04-24 13:12:21.875233 xtesting-0.97.0/doc/xtesting/
+-rw-r--r--   0 cedric    (1000) cedric    (1000)    77673 2020-01-14 15:33:30.000000 xtesting-0.97.0/doc/xtesting/ONAP.png
+-rw-r--r--   0 cedric    (1000) cedric    (1000)     1917 2020-01-14 15:33:30.000000 xtesting-0.97.0/doc/xtesting/index.html
+-rw-r--r--   0 cedric    (1000) cedric    (1000)     6344 2020-01-14 15:33:30.000000 xtesting-0.97.0/doc/xtesting/xtesting.md
+drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2023-04-24 13:12:21.875233 xtesting-0.97.0/doc/xtesting2020/
+-rw-r--r--   0 cedric    (1000) cedric    (1000)     1926 2022-04-12 08:13:45.000000 xtesting-0.97.0/doc/xtesting2020/index.html
+-rw-r--r--   0 cedric    (1000) cedric    (1000)      800 2022-04-12 08:13:45.000000 xtesting-0.97.0/doc/xtesting2020/xtesting2020.md
+drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2023-04-24 13:12:21.867233 xtesting-0.97.0/docker/
+drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2023-04-24 13:12:21.875233 xtesting-0.97.0/docker/core/
+-rw-r--r--   0 cedric    (1000) cedric    (1000)     1591 2023-04-24 13:10:15.000000 xtesting-0.97.0/docker/core/Dockerfile
+-rw-r--r--   0 cedric    (1000) cedric    (1000)     2320 2023-04-18 13:03:00.000000 xtesting-0.97.0/docker/core/testcases.yaml
+-rw-r--r--   0 cedric    (1000) cedric    (1000)      701 2023-04-18 13:03:00.000000 xtesting-0.97.0/requirements.txt
+-rw-r--r--   0 cedric    (1000) cedric    (1000)     1185 2023-04-24 13:12:21.883233 xtesting-0.97.0/setup.cfg
+-rw-r--r--   0 cedric    (1000) cedric    (1000)      766 2022-04-12 08:13:45.000000 xtesting-0.97.0/setup.py
+-rw-r--r--   0 cedric    (1000) cedric    (1000)      468 2023-04-18 13:03:00.000000 xtesting-0.97.0/test-requirements.txt
+-rw-r--r--   0 cedric    (1000) cedric    (1000)     2118 2023-04-24 13:10:15.000000 xtesting-0.97.0/tox.ini
+-rw-r--r--   0 cedric    (1000) cedric    (1000)      154 2023-04-18 13:03:00.000000 xtesting-0.97.0/upper-constraints.txt
+drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2023-04-24 13:12:21.875233 xtesting-0.97.0/xtesting/
+-rw-r--r--   0 cedric    (1000) cedric    (1000)        0 2018-02-28 14:23:15.000000 xtesting-0.97.0/xtesting/__init__.py
+drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2023-04-24 13:12:21.879233 xtesting-0.97.0/xtesting/ci/
+-rw-r--r--   0 cedric    (1000) cedric    (1000)        0 2018-02-28 14:23:15.000000 xtesting-0.97.0/xtesting/ci/__init__.py
+-rw-r--r--   0 cedric    (1000) cedric    (1000)      935 2020-11-09 16:39:47.000000 xtesting-0.97.0/xtesting/ci/logging.debug.ini
+-rw-r--r--   0 cedric    (1000) cedric    (1000)      886 2020-11-09 16:39:47.000000 xtesting-0.97.0/xtesting/ci/logging.ini
+-rw-r--r--   0 cedric    (1000) cedric    (1000)    14253 2023-04-18 13:03:00.000000 xtesting-0.97.0/xtesting/ci/run_tests.py
+-rw-r--r--   0 cedric    (1000) cedric    (1000)     2389 2023-04-18 13:03:00.000000 xtesting-0.97.0/xtesting/ci/testcases.yaml
+-rw-r--r--   0 cedric    (1000) cedric    (1000)     4236 2023-04-18 13:03:00.000000 xtesting-0.97.0/xtesting/ci/tier_builder.py
+-rw-r--r--   0 cedric    (1000) cedric    (1000)     3215 2023-04-18 13:03:00.000000 xtesting-0.97.0/xtesting/ci/tier_handler.py
+drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2023-04-24 13:12:21.879233 xtesting-0.97.0/xtesting/core/
+-rw-r--r--   0 cedric    (1000) cedric    (1000)        0 2018-02-28 14:23:15.000000 xtesting-0.97.0/xtesting/core/__init__.py
+-rw-r--r--   0 cedric    (1000) cedric    (1000)     2422 2022-04-12 08:13:45.000000 xtesting-0.97.0/xtesting/core/ansible.py
+-rw-r--r--   0 cedric    (1000) cedric    (1000)     3909 2023-04-18 13:03:00.000000 xtesting-0.97.0/xtesting/core/behaveframework.py
+-rw-r--r--   0 cedric    (1000) cedric    (1000)     9125 2023-04-18 13:03:00.000000 xtesting-0.97.0/xtesting/core/campaign.py
+-rw-r--r--   0 cedric    (1000) cedric    (1000)     4268 2023-04-24 13:10:29.000000 xtesting-0.97.0/xtesting/core/feature.py
+-rw-r--r--   0 cedric    (1000) cedric    (1000)     3203 2023-04-18 13:03:00.000000 xtesting-0.97.0/xtesting/core/pytest.py
+-rw-r--r--   0 cedric    (1000) cedric    (1000)     4661 2023-04-18 13:03:00.000000 xtesting-0.97.0/xtesting/core/robotframework.py
+-rw-r--r--   0 cedric    (1000) cedric    (1000)    14047 2023-04-18 13:03:00.000000 xtesting-0.97.0/xtesting/core/testcase.py
+-rw-r--r--   0 cedric    (1000) cedric    (1000)     4799 2023-04-18 13:03:00.000000 xtesting-0.97.0/xtesting/core/unit.py
+-rw-r--r--   0 cedric    (1000) cedric    (1000)     5304 2023-04-18 13:03:00.000000 xtesting-0.97.0/xtesting/core/vnf.py
+drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2023-04-24 13:12:21.879233 xtesting-0.97.0/xtesting/samples/
+-rw-r--r--   0 cedric    (1000) cedric    (1000)       58 2019-08-21 12:19:01.000000 xtesting-0.97.0/xtesting/samples/HelloWorld.robot
+-rw-r--r--   0 cedric    (1000) cedric    (1000)        0 2018-02-28 14:23:15.000000 xtesting-0.97.0/xtesting/samples/__init__.py
+drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2023-04-24 13:12:21.879233 xtesting-0.97.0/xtesting/samples/features/
+-rw-r--r--   0 cedric    (1000) cedric    (1000)      172 2021-02-09 18:21:54.000000 xtesting-0.97.0/xtesting/samples/features/hello.feature
+drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2023-04-24 13:12:21.879233 xtesting-0.97.0/xtesting/samples/features/steps/
+-rw-r--r--   0 cedric    (1000) cedric    (1000)      362 2021-02-09 18:21:54.000000 xtesting-0.97.0/xtesting/samples/features/steps/hello.py
+-rw-r--r--   0 cedric    (1000) cedric    (1000)      587 2023-04-18 13:03:00.000000 xtesting-0.97.0/xtesting/samples/first.py
+-rw-r--r--   0 cedric    (1000) cedric    (1000)      523 2018-02-28 14:23:15.000000 xtesting-0.97.0/xtesting/samples/fourth.py
+-rw-r--r--   0 cedric    (1000) cedric    (1000)      107 2022-04-12 08:13:45.000000 xtesting-0.97.0/xtesting/samples/helloworld.yml
+drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2023-04-24 13:12:21.879233 xtesting-0.97.0/xtesting/samples/mts/
+-rw-r--r--   0 cedric    (1000) cedric    (1000)      348 2023-04-18 13:03:00.000000 xtesting-0.97.0/xtesting/samples/mts/pause.xml
+-rw-r--r--   0 cedric    (1000) cedric    (1000)      447 2023-04-18 13:03:00.000000 xtesting-0.97.0/xtesting/samples/mts/test.xml
+-rw-r--r--   0 cedric    (1000) cedric    (1000)      491 2023-04-18 13:03:00.000000 xtesting-0.97.0/xtesting/samples/second.py
+drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2023-04-24 13:12:21.879233 xtesting-0.97.0/xtesting/tests/
+-rw-r--r--   0 cedric    (1000) cedric    (1000)        0 2018-02-28 14:23:15.000000 xtesting-0.97.0/xtesting/tests/__init__.py
+drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2023-04-24 13:12:21.879233 xtesting-0.97.0/xtesting/tests/unit/
+-rw-r--r--   0 cedric    (1000) cedric    (1000)        0 2018-02-28 14:23:15.000000 xtesting-0.97.0/xtesting/tests/unit/__init__.py
+drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2023-04-24 13:12:21.879233 xtesting-0.97.0/xtesting/tests/unit/ci/
+-rw-r--r--   0 cedric    (1000) cedric    (1000)        0 2018-02-28 14:23:15.000000 xtesting-0.97.0/xtesting/tests/unit/ci/__init__.py
+-rw-r--r--   0 cedric    (1000) cedric    (1000)    13216 2023-04-18 13:03:00.000000 xtesting-0.97.0/xtesting/tests/unit/ci/test_run_tests.py
+-rw-r--r--   0 cedric    (1000) cedric    (1000)     3703 2023-04-18 13:03:00.000000 xtesting-0.97.0/xtesting/tests/unit/ci/test_tier_builder.py
+-rw-r--r--   0 cedric    (1000) cedric    (1000)     2778 2023-04-18 13:03:00.000000 xtesting-0.97.0/xtesting/tests/unit/ci/test_tier_handler.py
+drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2023-04-24 13:12:21.883233 xtesting-0.97.0/xtesting/tests/unit/core/
+-rw-r--r--   0 cedric    (1000) cedric    (1000)        0 2018-02-28 14:23:15.000000 xtesting-0.97.0/xtesting/tests/unit/core/__init__.py
+-rw-r--r--   0 cedric    (1000) cedric    (1000)     8155 2022-04-12 08:13:45.000000 xtesting-0.97.0/xtesting/tests/unit/core/test_ansible.py
+-rw-r--r--   0 cedric    (1000) cedric    (1000)     6698 2023-04-18 13:03:00.000000 xtesting-0.97.0/xtesting/tests/unit/core/test_behaveframework.py
+-rw-r--r--   0 cedric    (1000) cedric    (1000)    10548 2023-04-24 13:10:29.000000 xtesting-0.97.0/xtesting/tests/unit/core/test_feature.py
+-rw-r--r--   0 cedric    (1000) cedric    (1000)    12738 2023-04-18 13:03:00.000000 xtesting-0.97.0/xtesting/tests/unit/core/test_robotframework.py
+-rw-r--r--   0 cedric    (1000) cedric    (1000)    18739 2023-04-18 13:03:00.000000 xtesting-0.97.0/xtesting/tests/unit/core/test_testcase.py
+-rw-r--r--   0 cedric    (1000) cedric    (1000)    10370 2023-04-18 13:03:00.000000 xtesting-0.97.0/xtesting/tests/unit/core/test_unit.py
+-rw-r--r--   0 cedric    (1000) cedric    (1000)     5603 2018-02-28 14:23:15.000000 xtesting-0.97.0/xtesting/tests/unit/core/test_vnf.py
+drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2023-04-24 13:12:21.883233 xtesting-0.97.0/xtesting/tests/unit/utils/
+-rw-r--r--   0 cedric    (1000) cedric    (1000)        0 2018-02-28 14:23:15.000000 xtesting-0.97.0/xtesting/tests/unit/utils/__init__.py
+-rw-r--r--   0 cedric    (1000) cedric    (1000)     4616 2023-04-18 13:03:00.000000 xtesting-0.97.0/xtesting/tests/unit/utils/test_decorators.py
+-rw-r--r--   0 cedric    (1000) cedric    (1000)     1479 2023-04-18 13:03:00.000000 xtesting-0.97.0/xtesting/tests/unit/utils/test_env.py
+drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2023-04-24 13:12:21.883233 xtesting-0.97.0/xtesting/utils/
+-rw-r--r--   0 cedric    (1000) cedric    (1000)        0 2018-02-28 14:23:15.000000 xtesting-0.97.0/xtesting/utils/__init__.py
+-rw-r--r--   0 cedric    (1000) cedric    (1000)      729 2022-03-04 14:04:55.000000 xtesting-0.97.0/xtesting/utils/config.py
+-rw-r--r--   0 cedric    (1000) cedric    (1000)     1033 2022-04-12 08:13:45.000000 xtesting-0.97.0/xtesting/utils/constants.py
+-rw-r--r--   0 cedric    (1000) cedric    (1000)     2001 2023-04-18 13:03:00.000000 xtesting-0.97.0/xtesting/utils/decorators.py
+-rw-r--r--   0 cedric    (1000) cedric    (1000)     1171 2023-04-18 13:03:00.000000 xtesting-0.97.0/xtesting/utils/env.py
+drwxr-xr-x   0 cedric    (1000) cedric    (1000)        0 2023-04-24 13:12:21.875233 xtesting-0.97.0/xtesting.egg-info/
+-rw-r--r--   0 cedric    (1000) cedric    (1000)     1472 2023-04-24 13:12:21.000000 xtesting-0.97.0/xtesting.egg-info/PKG-INFO
+-rw-r--r--   0 cedric    (1000) cedric    (1000)     3202 2023-04-24 13:12:21.000000 xtesting-0.97.0/xtesting.egg-info/SOURCES.txt
+-rw-r--r--   0 cedric    (1000) cedric    (1000)        1 2023-04-24 13:12:21.000000 xtesting-0.97.0/xtesting.egg-info/dependency_links.txt
+-rw-r--r--   0 cedric    (1000) cedric    (1000)      477 2023-04-24 13:12:21.000000 xtesting-0.97.0/xtesting.egg-info/entry_points.txt
+-rw-r--r--   0 cedric    (1000) cedric    (1000)        1 2021-06-01 14:54:54.000000 xtesting-0.97.0/xtesting.egg-info/not-zip-safe
+-rw-r--r--   0 cedric    (1000) cedric    (1000)       48 2023-04-24 13:12:21.000000 xtesting-0.97.0/xtesting.egg-info/pbr.json
+-rw-r--r--   0 cedric    (1000) cedric    (1000)      361 2023-04-24 13:12:21.000000 xtesting-0.97.0/xtesting.egg-info/requires.txt
+-rw-r--r--   0 cedric    (1000) cedric    (1000)        9 2023-04-24 13:12:21.000000 xtesting-0.97.0/xtesting.egg-info/top_level.txt
```

### Comparing `xtesting-0.96.0/.travis.yml` & `xtesting-0.97.0/.travis.yml`

 * *Files 17% similar despite different names*

```diff
@@ -39,37 +39,9 @@
         - amd64_dirs=""
         - arm64_dirs=""
         - arm_dirs="docker/core"
     - stage: publish xtesting manifests
       script: >
         sudo manifest-tool push from-args \
           --platforms linux/amd64,linux/arm,linux/arm64 \
-          --template ${DOCKER_USERNAME}/xtesting:ARCH-xena \
-          --target ${DOCKER_USERNAME}/xtesting:xena
-    - stage: build xtesting-mts images
-      script: sudo -E bash build.sh
-      env:
-        - REPO="${DOCKER_USERNAME}"
-        - arch="amd64"
-        - amd64_dirs="docker/mts"
-        - arm64_dirs=""
-        - arm_dirs=""
-    - script: sudo -E bash build.sh
-      env:
-        - REPO="${DOCKER_USERNAME}"
-        - arch="arm64"
-        - amd64_dirs=""
-        - arm64_dirs="docker/mts"
-        - arm_dirs=""
-    - script: sudo -E bash build.sh
-      env:
-        - REPO="${DOCKER_USERNAME}"
-        - arch="arm"
-        - amd64_dirs=""
-        - arm64_dirs=""
-        - arm_dirs="docker/mts"
-    - stage: publish xtesting-mts manifests
-      script: >
-        sudo manifest-tool push from-args \
-          --platforms linux/amd64,linux/arm,linux/arm64 \
-          --template ${DOCKER_USERNAME}/xtesting-mts:ARCH-xena \
-          --target ${DOCKER_USERNAME}/xtesting-mts:xena
+          --template ${DOCKER_USERNAME}/xtesting:ARCH-zed \
+          --target ${DOCKER_USERNAME}/xtesting:zed
```

### Comparing `xtesting-0.96.0/AUTHORS` & `xtesting-0.97.0/AUTHORS`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Aimee Ukasick <aimeeu.opensource@gmail.com>
 Ajay Kumar <ajay4.kumar@orange.com>
 Alex Yang <yangyang1@zte.com.cn>
 Alexandru Avadanii <Alexandru.Avadanii@enea.com>
 AntonySilvester <antonysilvester@gmail.com>
 Aric Gardner <agardner@linuxfoundation.org>
 Ashish Singh <ashishsingh2k8@gmail.com>
+Bellengé Maxime <maxime.bellenge@orange.com>
 Benoit HERARD <benoit.herard@orange.com>
 Bertrand Souville <souville@docomolab-euro.com>
 Brady Johnson <brady.allen.johnson@ericsson.com>
 CNlucius <lukai1@huawei.com>
 CNlukai <lukai1@huawei.com>
 Calin Gherghe <calin.gherghe@intel.com>
 Carlos Goncalves <carlos.goncalves@neclab.eu>
@@ -23,20 +24,22 @@
 Cédric Ollivier <ollivier.cedric@gmail.com>
 Dan Radez <dradez@redhat.com>
 Daniel Farrell <dfarrell@redhat.com>
 David Blaisonneau <david.blaisonneau@orange.com>
 Deepak Chandella <deepak.chandella@orange.com>
 Delia Popescu <delia.popescu@enea.com>
 Dimitri Mazmanov <dimitri.mazmanov@ericsson.com>
+Edouard Hinard <edouard.hinard@orange.com>
 Ferenc Cserepkei <ferenc.cserepkei@ericsson.com>
 Francois Regis Menguy <francoisregis.menguy@orange.com>
 Frank Brockners <fbrockne@cisco.com>
 Georg Kunz <georg.kunz@ericsson.com>
 George Paraskevopoulos <geopar@intracom-telecom.com>
 Gerald Kunzmann <kunzmann@docomolab-euro.com>
+Guillaume Lambert <guillaume.lambert@orange.com>
 Helen Yao <yaohelan@huawei.com>
 Jamo Luhrsen <jluhrsen@redhat.com>
 Jose Lausuch <jalausuch@suse.com>
 Jose Lausuch <jose.lausuch@ericsson.com>
 Juan Vidal <juan.vidal.allende@ericsson.com>
 Juha Haapavirta <juha.haapavirta@nokia.com>
 Juha Kosonen <juha.kosonen@nokia.com>
```

### Comparing `xtesting-0.96.0/ChangeLog` & `xtesting-0.97.0/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 CHANGES
 =======
 
-0.96
+0.97
 ----
 
+* Remove MTS from Xtesting
+* Add pytest driver in Xtesting
+* Allow setting env vars via testcases.yaml
+* Add missing api docs
+* Run pre-commit in the Xtesting gates
+* Remove a useless duplicate when calling pytest
+* Prepare Xena containers
+* Set defaultbranch=stable/zed
+* Make robot driver even more generic
+* Add deny\_skipping parameter
+* Update to Alpine 3.16
+* Update to Alpine 3.15
+* Change working dir
+* Define xtesting user to harden security
 * Protect vs Bucket containing html chars
+* Complete previous commit
+* Rewrite last direct call to ci/testcases.yaml
+* Only erase the fallback config files
 * Search config files in tree
 * Allow overriding project\_name via env
-
-0.95
-----
-
 * Reset argv to prevent wrong usage
 * Protect if detail is returned as None
-
-0.94
-----
-
 * Fix incorrect f-string
 * Remove ansiblelint as tox entry
-
-0.93
-----
-
 * Leverage latest pylint features
 * Update robotframework to latest release
 * Update requirements
-* Update Xtesting to stable/xena
-* Update defaultbranch to stable/xena
 * Correct documented return values
 * Fix .circleci/config.yml (py39)
 * Update pylint to 2.9.6
 * Use python 3 super() style
 * Update container builds due to Alpine 3.14
 * Update to Alpine 3.14
 * Fix tag logics in behave
```

### Comparing `xtesting-0.96.0/LICENSE` & `xtesting-0.97.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/PKG-INFO` & `xtesting-0.97.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: xtesting
-Version: 0.96.0
+Version: 0.97.0
 Summary: OPNFV reference testing framework
 Home-page: https://wiki.opnfv.org/display/functest
 Author: OPNFV
 Author-email: opnfv-tech-discuss@lists.opnfv.org
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -37,9 +35,7 @@
 To learn more about Xtesting:
 
   * Documentation: http://xtesting.readthedocs.io/en/latest/
   * Gerrit: https://gerrit.opnfv.org/gerrit/#/q/project:functest-xtesting
 
 Get in touch via `email <mailto:opnfv-tech-discuss@lists.opnfv.org>`_.
 
-
-
```

### Comparing `xtesting-0.96.0/README.md` & `xtesting-0.97.0/README.md`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/README.rst` & `xtesting-0.97.0/README.rst`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/ansible/site.gate.yml` & `xtesting-0.97.0/ansible/site.gate.yml`

 * *Files 24% similar despite different names*

```diff
@@ -4,37 +4,29 @@
     - role: collivier.xtesting
       use_gerrit: true
       gerrit_project: functest-xtesting
       git_url: https://gerrit.opnfv.org/gerrit/functest-xtesting
       docker_tags:
         - latest:
             branch: master
-            dependency: '3.14'
+            dependency: '3.16'
       builds:
         dependency:
           repo: _
           dport:
           container: alpine
         steps:
           - name: opnfv/xtesting
             containers:
               - name: xtesting
                 ref_arg: BRANCH
                 path: docker/core
-          - name: opnfv/xtesting-mts
-            containers:
-              - name: xtesting-mts
-                ref_arg: BRANCH
-                path: docker/mts
       suites:
         - container: xtesting
           tests:
             - first
             - second
             - third
             - fourth
             - fifth
             - sixth
             - eighth
-        - container: xtesting-mts
-          tests:
-            - seventh
```

### Comparing `xtesting-0.96.0/api/conf.py` & `xtesting-0.97.0/api/conf.py`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/api/index.rst` & `xtesting-0.97.0/api/index.rst`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/build.sh` & `xtesting-0.97.0/build.sh`

 * *Files 4% similar despite different names*

```diff
@@ -9,36 +9,35 @@
 
 repo=${REPO:-opnfv}
 arch=${arch-"\
 amd64 \
 arm64 \
 arm"}
 amd64_dirs=${amd64_dirs-"\
-docker/core \
-docker/mts"}
+docker/core"}
 arm_dirs=${arm_dirs-${amd64_dirs}}
 arm64_dirs=${arm64_dirs-${amd64_dirs}}
-tag=${BRANCH:-stable/xena}
+tag=${BRANCH:-stable/yoga}
 image="xtesting"
 build_opts=(--pull=true --no-cache --force-rm=true)
 
 for arch in ${arch}; do
     if [[ ${arch} == arm64 ]]; then
         find . -name Dockerfile -exec sed -i \
-            -e "s|alpine:3.14|arm64v8/alpine:3.14|g" {} +
+            -e "s|alpine:3.16|arm64v8/alpine:3.16|g" {} +
         find . -name Dockerfile -exec sed -i \
-            -e "s|opnfv/xtesting:xena|${repo}/xtesting:arm64-${tag}|g" {} +
+            -e "s|opnfv/xtesting:zed|${repo}/xtesting:arm64-${tag}|g" {} +
     elif [[ ${arch} == arm ]]; then
         find . -name Dockerfile -exec sed -i \
-            -e "s|alpine:3.14|arm32v6/alpine:3.14|g" {} +
+            -e "s|alpine:3.16|arm32v6/alpine:3.16|g" {} +
         find . -name Dockerfile -exec sed -i \
-            -e "s|opnfv/xtesting:xena|${repo}/xtesting:arm-${tag}|g" {} +
+            -e "s|opnfv/xtesting:zed|${repo}/xtesting:arm-${tag}|g" {} +
     else
         find . -name Dockerfile -exec sed -i \
-            -e "s|opnfv/xtesting:xena|${repo}/xtesting:amd64-${tag}|g" {} +
+            -e "s|opnfv/xtesting:zed|${repo}/xtesting:amd64-${tag}|g" {} +
     fi
     dirs=${arch}_dirs
     for dir in ${!dirs}; do
         if [[ ${dir} == docker/core ]]; then
             image=xtesting
         else
             image=xtesting-${dir##**/}
```

### Comparing `xtesting-0.96.0/doc/cntt_rc_cookbook/cntt_rc_cookbook.md` & `xtesting-0.97.0/doc/cntt_rc_cookbook/cntt_rc_cookbook.md`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/doc/cntt_rc_cookbook/index.html` & `xtesting-0.97.0/doc/cntt_rc_cookbook/index.html`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/doc/ons2019/chainedci.png` & `xtesting-0.97.0/doc/ons2019/chainedci.png`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/doc/ons2019/ftth.png` & `xtesting-0.97.0/doc/ons2019/ftth.png`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/doc/ons2019/index.html` & `xtesting-0.97.0/doc/ons2019/index.html`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/doc/ons2019/ons2019.md` & `xtesting-0.97.0/doc/ons2019/ons2019.md`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/doc/xtesting/ONAP.png` & `xtesting-0.97.0/doc/xtesting/ONAP.png`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/doc/xtesting/index.html` & `xtesting-0.97.0/doc/xtesting/index.html`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/doc/xtesting/xtesting.md` & `xtesting-0.97.0/doc/xtesting/xtesting.md`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/doc/xtesting2020/index.html` & `xtesting-0.97.0/doc/xtesting2020/index.html`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/doc/xtesting2020/xtesting2020.md` & `xtesting-0.97.0/doc/xtesting2020/xtesting2020.md`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/docker/core/Dockerfile` & `xtesting-0.97.0/docker/core/Dockerfile`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,32 @@
-FROM alpine:3.14
+FROM alpine:3.16
 
-ARG BRANCH=stable/xena
-ARG OPENSTACK_TAG=stable/xena
+ARG BRANCH=stable/zed
+ARG OPENSTACK_TAG=stable/zed
 
 RUN apk -U upgrade && \
     apk --no-cache add --update python3 py3-pip py3-wheel bash git mailcap libxml2 libxslt ansible && \
     apk --no-cache add --virtual .build-deps --update \
         python3-dev build-base libxml2-dev libxslt-dev linux-headers && \
     wget -q -O- https://opendev.org/openstack/requirements/raw/branch/$OPENSTACK_TAG/upper-constraints.txt > upper-constraints.txt && \
-    sed -i -E /^PyYAML==+.*$/d upper-constraints.txt && \
-    sed -i -E /^six==+.*$/d upper-constraints.txt && \
+    sed -i -E /^packaging==+.*$/d upper-constraints.txt && \
     case $(uname -m) in aarch*|arm*) CFLAGS="-O0" \
         pip3 install --no-cache-dir \
             -cupper-constraints.txt \
             -chttps://git.opnfv.org/functest-xtesting/plain/upper-constraints.txt?h=$BRANCH \
             lxml ;; esac && \
     git init /src/functest-xtesting && \
     (cd /src/functest-xtesting && \
         git fetch --tags https://gerrit.opnfv.org/gerrit/functest-xtesting $BRANCH && \
         git checkout FETCH_HEAD) && \
     pip3 install --no-cache-dir --src /src \
         -cupper-constraints.txt \
         -chttps://git.opnfv.org/functest-xtesting/plain/upper-constraints.txt?h=$BRANCH \
         /src/functest-xtesting && \
     rm -r /src/functest-xtesting upper-constraints.txt && \
+    addgroup -g 1000 xtesting && adduser -u 1000 -G xtesting -D xtesting && \
+    mkdir -p /var/lib/xtesting/results && chown -R xtesting: /var/lib/xtesting && \
     apk del .build-deps
-COPY testcases.yaml /usr/lib/python3.9/site-packages/xtesting/ci/testcases.yaml
+COPY testcases.yaml /usr/lib/python3.10/site-packages/xtesting/ci/testcases.yaml
+USER xtesting
+WORKDIR /var/lib/xtesting/results
 CMD ["run_tests", "-t", "all"]
```

### Comparing `xtesting-0.96.0/docker/core/testcases.yaml` & `xtesting-0.97.0/xtesting/ci/testcases.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -37,44 +37,58 @@
         description: ''
         run:
           name: unit
           args:
             name: xtesting.samples.fourth
       - case_name: fifth
         project_name: xtesting
+        enabled: false
         criteria: 100
         blocking: true
         clean_flag: false
         description: ''
         run:
           name: robotframework
           args:
             suites:
               - >-
-                /usr/lib/python3.9/site-packages/xtesting/samples/HelloWorld.robot
+                /usr/lib/python3.10/site-packages/xtesting/samples/HelloWorld.robot
             variable:
               - 'var01:foo'
               - 'var02:bar'
       - case_name: sixth
         project_name: xtesting
+        enabled: false
         criteria: 100
         blocking: true
         clean_flag: false
         description: ''
         run:
           name: behaveframework
           args:
             suites:
-              - /usr/lib/python3.9/site-packages/xtesting/samples/features
+              - /usr/lib/python3.10/site-packages/xtesting/samples/features
             tags:
               - foo
       - case_name: eighth
         project_name: xtesting
+        enabled: false
         criteria: 100
         blocking: true
         clean_flag: false
         description: ''
         run:
           name: ansible
           args:
-            private_data_dir: /usr/lib/python3.9/site-packages/xtesting/samples
+            private_data_dir: /usr/lib/python3.10/site-packages/xtesting/samples
             playbook: helloworld.yml
+      - case_name: nineth
+        project_name: xtesting
+        enabled: true
+        criteria: 100
+        blocking: true
+        clean_flag: false
+        description: ''
+        run:
+          name: pytest
+          args:
+            dir: /usr/lib/python3.10/site-packages/xtesting/samples/fourth.py
```

### Comparing `xtesting-0.96.0/requirements.txt` & `xtesting-0.97.0/requirements.txt`

 * *Files 12% similar despite different names*

```diff
@@ -13,7 +13,9 @@
 PrettyTable # BSD
 python-subunit # Apache-2.0/BSD
 os-testr # Apache-2.0
 junitxml
 boto3 # Apache-2.0
 lxml!=3.7.0 # BSD
 ansible-runner!=1.3.5 # Apache 2.0
+pytest  # MIT
+pytest-html  #MPL-2.0
```

### Comparing `xtesting-0.96.0/setup.cfg` & `xtesting-0.97.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 xtesting.testcase = 
 	bashfeature = xtesting.core.feature:BashFeature
 	robotframework = xtesting.core.robotframework:RobotFramework
 	behaveframework = xtesting.core.behaveframework:BehaveFramework
 	unit = xtesting.core.unit:Suite
 	first = xtesting.samples.first:Test
 	second = xtesting.samples.second:Test
-	mts = xtesting.core.mts:MTSLauncher
 	ansible = xtesting.core.ansible:Ansible
+	pytest = xtesting.core.pytest:Pytest
 
 [build_sphinx]
 all_files = 1
 build-dir = api/build/
 source-dir = api
 
 [wheel]
```

### Comparing `xtesting-0.96.0/setup.py` & `xtesting-0.97.0/setup.py`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/tox.ini` & `xtesting-0.97.0/tox.ini`

 * *Files 17% similar despite different names*

```diff
@@ -1,82 +1,81 @@
 [tox]
-envlist = docs,pep8,pylint,yamllint,bashate,py39,cover,perm
+envlist = docs,pep8,pylint,yamllint,bashate,py310,cover,perm,pre-commit
 skipsdist = True
 
 [testenv]
 pip_version = pip==20.2.4
 usedevelop = True
 deps =
   -c{toxinidir}/upper-constraints.txt
-  -chttps://opendev.org/openstack/requirements/raw/branch/stable/xena/upper-constraints.txt
+  -chttps://opendev.org/openstack/requirements/raw/branch/stable/zed/upper-constraints.txt
   -r{toxinidir}/requirements.txt
   -r{toxinidir}/test-requirements.txt
 install_command = pip install {opts} {packages}
-commands = nosetests --with-xunit \
-  --with-coverage \
-  --cover-tests \
-  --cover-package=xtesting \
-  --cover-xml \
-  --cover-html \
-  xtesting/tests/unit
+commands =
+  pytest \
+    --junit-xml=junit.xml \
+    --html=report.html --self-contained-html \
+    --cov=xtesting --cov-reset --cov-report html \
+    xtesting/tests/unit
 
 [testenv:docs]
-basepython = python3.9
+basepython = python3.10
 commands =
   doc8 README.rst api --ignore-path api/build
   sphinx-build -W -b html api/ api/build
 
 [testenv:pep8]
-basepython = python3.9
+basepython = python3.10
 commands = flake8
 
 [testenv:pylint]
-basepython = python3.9
+basepython = python3.10
 whitelist_externals = bash
 commands =
   pylint --min-similarity-lines=10 \
     --disable=locally-disabled --ignore-imports=y --reports=n --extension-pkg-whitelist=lxml xtesting
 
 [testenv:yamllint]
-basepython = python3.9
+basepython = python3.10
 files =
   .travis.yml
   ansible
   xtesting/ci
 commands =
   yamllint -s {[testenv:yamllint]files}
 
-[testenv:py38]
-commands = nosetests xtesting/tests/unit
-
 [testenv:bashate]
-basepython = python3.9
+basepython = python3.10
 files =
   build.sh
 commands = bashate {[testenv:bashate]files}
 
 [testenv:bandit]
-basepython = python3.9
+basepython = python3.10
 commands = bandit -r xtesting -x tests -n 5 -ll -s B602
 
 [testenv:cover]
-basepython = python3.9
+basepython = python3.10
 dirs =
   xtesting/tests/unit/ci
   xtesting/tests/unit/core
   xtesting/tests/unit/utils/test_decorators.py
-commands = nosetests --with-coverage --cover-tests \
-  --cover-package xtesting.core \
-  --cover-package xtesting.tests.unit \
-  --cover-package xtesting.utils.decorators \
-  --cover-min-percentage 100 {[testenv:cover]dirs}
+commands =
+  pytest --cov=xtesting --cov-reset --cov-report html --cov-fail-under=100 \
+    {[testenv:cover]dirs}
 
 [testenv:perm]
-basepython = python3.9
+basepython = python3.10
 whitelist_externals = bash
 path=. -not -path './.tox/*' -not -path './.git/*' -not -path './doc/reveal.js/*'
 commands =
   bash -c "\
     find {[testenv:perm]path} \( -type f -not -perm 644 -o -type d -not -perm 755 \) \
     -exec ls -l \{\} + | grep '.' && exit 1 || exit 0"
   bash -c "\
     find {[testenv:perm]path} -exec file \{\} + | grep CRLF && exit 1 || exit 0"
+
+[testenv:pre-commit]
+basepython = python3.10
+commands =
+    pre-commit run --all-files --show-diff-on-failure
```

### Comparing `xtesting-0.96.0/xtesting/ci/logging.debug.ini` & `xtesting-0.97.0/xtesting/ci/logging.debug.ini`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/xtesting/ci/logging.ini` & `xtesting-0.97.0/xtesting/ci/logging.ini`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/xtesting/ci/run_tests.py` & `xtesting-0.97.0/xtesting/ci/run_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,14 +139,15 @@
             return None
         except Exception:  # pylint: disable=broad-except
             LOGGER.exception("Cannot get %s's config options", testname)
             return None
 
     def run_test(self, test):
         """Run one test case"""
+        # pylint: disable=too-many-branches
         if not test.is_enabled() or test.is_skipped():
             msg = prettytable.PrettyTable(
                 header_style='upper', padding_width=5,
                 field_names=['test case', 'project', 'duration',
                              'result'])
             msg.add_row([test.get_name(), test.get_project(), "00:00", "SKIP"])
             LOGGER.info("Test result:\n\n%s\n", msg)
@@ -164,14 +165,19 @@
                     invoke_kwds=test_dict).driver
                 self.executed_test_cases[test.get_name()] = test_case
                 test_case.check_requirements()
                 if test_case.is_skipped:
                     LOGGER.info("Skipping test case '%s'...", test.get_name())
                     LOGGER.info("Test result:\n\n%s\n", test_case)
                     return testcase.TestCase.EX_TESTCASE_SKIPPED
+                if 'env' in run_dict:
+                    LOGGER.info(
+                        "Setting env for test case '%s'...", test.get_name())
+                    for key, value in run_dict['env'].items():
+                        os.environ[key] = str(value)
                 LOGGER.info("Running test case '%s'...", test.get_name())
                 try:
                     kwargs = run_dict['args']
                     test_case.run(**kwargs)
                 except KeyError:
                     test_case.run()
                 result = test_case.is_successful()
```

### Comparing `xtesting-0.96.0/xtesting/ci/tier_builder.py` & `xtesting-0.97.0/xtesting/ci/tier_builder.py`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/xtesting/ci/tier_handler.py` & `xtesting-0.97.0/xtesting/ci/tier_handler.py`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/xtesting/core/ansible.py` & `xtesting-0.97.0/xtesting/core/ansible.py`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/xtesting/core/behaveframework.py` & `xtesting-0.97.0/xtesting/core/behaveframework.py`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/xtesting/core/campaign.py` & `xtesting-0.97.0/xtesting/core/campaign.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,8 +222,9 @@
     if env.get('DEBUG').lower() == 'true':
         logging.config.fileConfig(config.get_xtesting_config(
             'logging.debug.ini', constants.DEBUG_INI_PATH_DEFAULT))
     else:
         logging.config.fileConfig(config.get_xtesting_config(
             'logging.ini', constants.INI_PATH_DEFAULT))
     logging.captureWarnings(True)
+    os.chdir(testcase.TestCase.dir_results)
     Campaign.zip_campaign_files()
```

### Comparing `xtesting-0.96.0/xtesting/core/feature.py` & `xtesting-0.97.0/xtesting/core/feature.py`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/xtesting/core/robotframework.py` & `xtesting-0.97.0/xtesting/core/robotframework.py`

 * *Files 9% similar despite different names*

```diff
@@ -52,24 +52,31 @@
     """RobotFramework runner."""
 
     __logger = logging.getLogger(__name__)
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.xml_file = os.path.join(self.res_dir, 'output.xml')
+        self.deny_skipping = kwargs.get("deny_skipping", False)
 
     def parse_results(self):
         """Parse output.xml and get the details in it."""
         result = robot.api.ExecutionResult(self.xml_file)
         visitor = ResultVisitor()
         result.visit(visitor)
         try:
-            self.result = 100 * (
-                result.suite.statistics.passed /
-                result.suite.statistics.total)
+            if self.deny_skipping:
+                self.result = 100 * (
+                    result.suite.statistics.passed /
+                    result.suite.statistics.total)
+            else:
+                self.result = 100 * ((
+                    result.suite.statistics.passed +
+                    result.suite.statistics.skipped) /
+                    result.suite.statistics.total)
         except ZeroDivisionError:
             self.__logger.error("No test has been run")
         self.start_time = timestamp_to_secs(result.suite.starttime)
         self.stop_time = timestamp_to_secs(result.suite.endtime)
         self.details = {}
         self.details['description'] = result.suite.name
         self.details['tests'] = visitor.get_data()
@@ -95,31 +102,30 @@
             kwargs: Arbitrary keyword arguments.
 
         Returns:
             EX_OK if all suites ran well.
             EX_RUN_ERROR otherwise.
         """
         try:
-            suites = kwargs["suites"]
-            variable = kwargs.get("variable", [])
-            variablefile = kwargs.get("variablefile", [])
-            include = kwargs.get("include", [])
+            suites = kwargs.pop("suites")
         except KeyError:
             self.__logger.exception("Mandatory args were not passed")
             return self.EX_RUN_ERROR
         if not os.path.exists(self.res_dir):
             try:
                 os.makedirs(self.res_dir)
             except Exception:  # pylint: disable=broad-except
                 self.__logger.exception("Cannot create %s", self.res_dir)
                 return self.EX_RUN_ERROR
         stream = StringIO()
-        robot.run(*suites, variable=variable, variablefile=variablefile,
-                  include=include, output=self.xml_file, log='NONE',
-                  report='NONE', stdout=stream)
+        kwargs["output"] = self.xml_file
+        kwargs["log"] = "NONE"
+        kwargs["report"] = "NONE"
+        kwargs["stdout"] = stream
+        robot.run(*suites, **kwargs)
         self.__logger.info("\n%s", stream.getvalue())
         try:
             self.parse_results()
             self.__logger.info("Results were successfully parsed")
             self.generate_report()
             self.__logger.info("Results were successfully generated")
         except RobotError as ex:
```

### Comparing `xtesting-0.96.0/xtesting/core/testcase.py` & `xtesting-0.97.0/xtesting/core/testcase.py`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/xtesting/core/unit.py` & `xtesting-0.97.0/xtesting/core/unit.py`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/xtesting/core/vnf.py` & `xtesting-0.97.0/xtesting/core/vnf.py`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/xtesting/samples/first.py` & `xtesting-0.97.0/xtesting/samples/first.py`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/xtesting/samples/fourth.py` & `xtesting-0.97.0/xtesting/samples/fourth.py`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/xtesting/tests/unit/ci/test_run_tests.py` & `xtesting-0.97.0/xtesting/tests/unit/ci/test_run_tests.py`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/xtesting/tests/unit/ci/test_tier_builder.py` & `xtesting-0.97.0/xtesting/tests/unit/ci/test_tier_builder.py`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/xtesting/tests/unit/ci/test_tier_handler.py` & `xtesting-0.97.0/xtesting/tests/unit/ci/test_tier_handler.py`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/xtesting/tests/unit/core/test_ansible.py` & `xtesting-0.97.0/xtesting/tests/unit/core/test_ansible.py`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/xtesting/tests/unit/core/test_behaveframework.py` & `xtesting-0.97.0/xtesting/tests/unit/core/test_behaveframework.py`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/xtesting/tests/unit/core/test_feature.py` & `xtesting-0.97.0/xtesting/tests/unit/core/test_feature.py`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/xtesting/tests/unit/core/test_robotframework.py` & `xtesting-0.97.0/xtesting/tests/unit/core/test_robotframework.py`

 * *Files 11% similar despite different names*

```diff
@@ -82,33 +82,50 @@
                              timestamp_to_secs(config['starttime']))
             self.assertEqual(self.test.stop_time,
                              timestamp_to_secs(config['endtime']))
             self.assertEqual(self.test.details,
                              {'description': config['name'], 'tests': []})
 
     def test_null_passed(self):
-        self._config.update({'statistics.passed': 0,
+        self._config.update({'statistics.skipped': 0,
+                             'statistics.passed': 0,
                              'statistics.total': 20})
         self._test_result(self._config, 0)
 
     def test_no_test(self):
-        self._config.update({'statistics.passed': 20,
+        self._config.update({'statistics.skipped': 0,
+                             'statistics.passed': 20,
                              'statistics.total': 0})
         self._test_result(self._config, 0)
 
     def test_half_success(self):
-        self._config.update({'statistics.passed': 10,
+        self._config.update({'statistics.skipped': 0,
+                             'statistics.passed': 10,
                              'statistics.total': 20})
         self._test_result(self._config, 50)
 
     def test_success(self):
-        self._config.update({'statistics.passed': 20,
+        self._config.update({'statistics.skipped': 0,
+                             'statistics.passed': 20,
                              'statistics.total': 20})
         self._test_result(self._config, 100)
 
+    def test_skip_excluded(self):
+        self.test.deny_skipping = True
+        self._config.update({'statistics.skipped': 1,
+                             'statistics.passed': 4,
+                             'statistics.total': 5})
+        self._test_result(self._config, 80)
+
+    def test_skip_included(self):
+        self._config.update({'statistics.skipped': 1,
+                             'statistics.passed': 4,
+                             'statistics.total': 5})
+        self._test_result(self._config, 100)
+
 
 class GenerateReportTesting(unittest.TestCase):
 
     """The class testing RobotFramework.generate_report()."""
     # pylint: disable=missing-docstring
 
     def setUp(self):
@@ -194,19 +211,24 @@
     def test_makedirs_exc(self, *args):
         self._test_makedirs_exc()
         args[0].assert_called_once_with(self.test.res_dir)
         args[1].assert_called_once_with(self.test.res_dir)
 
     @mock.patch('robot.run')
     def _test_makedirs(self, *args):
+        kwargs = {
+            'variable': self.variable,
+            'variablefile': self.variablefile,
+            'include': self.include
+        }
         with mock.patch.object(self.test, 'parse_results') as mock_method, \
                 mock.patch.object(self.test, 'generate_report',
                                   return_value=0) as mmethod:
             self.assertEqual(
-                self.test.run(suites=self.suites, variable=self.variable),
+                self.test.run(suites=self.suites, **kwargs),
                 self.test.EX_OK)
             args[0].assert_called_once_with(
                 *self.suites, log='NONE', output=self.test.xml_file,
                 report='NONE', stdout=mock.ANY, variable=self.variable,
                 variablefile=self.variablefile, include=self.include)
             mock_method.assert_called_once_with()
             mmethod.assert_called_once_with()
@@ -224,18 +246,21 @@
         self._test_makedirs()
         args[0].assert_called_once_with(self.test.res_dir)
         args[1].assert_called_once_with(self.test.res_dir)
 
     @mock.patch('os.makedirs')
     @mock.patch('robot.run')
     def _test_parse_results(self, status, *args):
+        kwargs = {
+            'variable': self.variable,
+            'variablefile': self.variablefile,
+            'include': self.include
+        }
         self.assertEqual(
-            self.test.run(
-                suites=self.suites, variable=self.variable,
-                variablefile=self.variablefile, include=self.include),
+            self.test.run(suites=self.suites, **kwargs),
             status)
         args[0].assert_called_once_with(
             *self.suites, log='NONE', output=self.test.xml_file,
             report='NONE', stdout=mock.ANY, variable=self.variable,
             variablefile=self.variablefile, include=self.include)
         args[1].assert_called_once_with(self.test.res_dir)
 
@@ -254,19 +279,22 @@
             self._test_parse_results(self.test.EX_RUN_ERROR)
             mock_method.assert_called_once_with()
             mmethod.assert_not_called()
 
     @mock.patch('os.makedirs')
     @mock.patch('robot.run')
     def _test_generate_report(self, status, *args):
+        kwargs = {
+            'variable': self.variable,
+            'variablefile': self.variablefile,
+            'include': self.include
+        }
         with mock.patch.object(self.test, 'parse_results') as mock_method:
             self.assertEqual(
-                self.test.run(
-                    suites=self.suites, variable=self.variable,
-                    variablefile=self.variablefile, include=self.include),
+                self.test.run(suites=self.suites, **kwargs),
                 status)
         args[0].assert_called_once_with(
             *self.suites, log='NONE', output=self.test.xml_file,
             report='NONE', stdout=mock.ANY, variable=self.variable,
             variablefile=self.variablefile, include=self.include)
         args[1].assert_called_once_with(self.test.res_dir)
         mock_method.assert_called_once_with()
```

### Comparing `xtesting-0.96.0/xtesting/tests/unit/core/test_testcase.py` & `xtesting-0.97.0/xtesting/tests/unit/core/test_testcase.py`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/xtesting/tests/unit/core/test_unit.py` & `xtesting-0.97.0/xtesting/tests/unit/core/test_unit.py`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/xtesting/tests/unit/core/test_vnf.py` & `xtesting-0.97.0/xtesting/tests/unit/core/test_vnf.py`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/xtesting/tests/unit/utils/test_decorators.py` & `xtesting-0.97.0/xtesting/tests/unit/utils/test_decorators.py`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/xtesting/tests/unit/utils/test_env.py` & `xtesting-0.97.0/xtesting/tests/unit/utils/test_env.py`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/xtesting/utils/config.py` & `xtesting-0.97.0/xtesting/utils/config.py`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/xtesting/utils/constants.py` & `xtesting-0.97.0/xtesting/utils/constants.py`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/xtesting/utils/decorators.py` & `xtesting-0.97.0/xtesting/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/xtesting/utils/env.py` & `xtesting-0.97.0/xtesting/utils/env.py`

 * *Files identical despite different names*

### Comparing `xtesting-0.96.0/xtesting.egg-info/PKG-INFO` & `xtesting-0.97.0/xtesting.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: xtesting
-Version: 0.96.0
+Version: 0.97.0
 Summary: OPNFV reference testing framework
 Home-page: https://wiki.opnfv.org/display/functest
 Author: OPNFV
 Author-email: opnfv-tech-discuss@lists.opnfv.org
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -37,9 +35,7 @@
 To learn more about Xtesting:
 
   * Documentation: http://xtesting.readthedocs.io/en/latest/
   * Gerrit: https://gerrit.opnfv.org/gerrit/#/q/project:functest-xtesting
 
 Get in touch via `email <mailto:opnfv-tech-discuss@lists.opnfv.org>`_.
 
-
-
```

### Comparing `xtesting-0.96.0/xtesting.egg-info/SOURCES.txt` & `xtesting-0.97.0/xtesting.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .coveragerc
 .gitmodules
+.pre-commit-config.yaml
 .travis.yml
 AUTHORS
 ChangeLog
 LICENSE
 README.md
 README.rst
 build.sh
@@ -19,16 +20,19 @@
 api/conf.py
 api/index.rst
 api/apidoc/modules.rst
 api/apidoc/xtesting.ci.rst
 api/apidoc/xtesting.ci.run_tests.rst
 api/apidoc/xtesting.ci.tier_builder.rst
 api/apidoc/xtesting.ci.tier_handler.rst
+api/apidoc/xtesting.core.ansible.rst
 api/apidoc/xtesting.core.behaveframework.rst
+api/apidoc/xtesting.core.campaign.rst
 api/apidoc/xtesting.core.feature.rst
+api/apidoc/xtesting.core.pytest.rst
 api/apidoc/xtesting.core.robotframework.rst
 api/apidoc/xtesting.core.rst
 api/apidoc/xtesting.core.testcase.rst
 api/apidoc/xtesting.core.unit.rst
 api/apidoc/xtesting.core.vnf.rst
 api/apidoc/xtesting.rst
 api/apidoc/xtesting.utils.constants.rst
@@ -45,17 +49,14 @@
 doc/xtesting/ONAP.png
 doc/xtesting/index.html
 doc/xtesting/xtesting.md
 doc/xtesting2020/index.html
 doc/xtesting2020/xtesting2020.md
 docker/core/Dockerfile
 docker/core/testcases.yaml
-docker/mts/Dockerfile
-docker/mts/mts-installer.properties
-docker/mts/testcases.yaml
 xtesting/__init__.py
 xtesting.egg-info/PKG-INFO
 xtesting.egg-info/SOURCES.txt
 xtesting.egg-info/dependency_links.txt
 xtesting.egg-info/entry_points.txt
 xtesting.egg-info/not-zip-safe
 xtesting.egg-info/pbr.json
@@ -69,15 +70,15 @@
 xtesting/ci/tier_builder.py
 xtesting/ci/tier_handler.py
 xtesting/core/__init__.py
 xtesting/core/ansible.py
 xtesting/core/behaveframework.py
 xtesting/core/campaign.py
 xtesting/core/feature.py
-xtesting/core/mts.py
+xtesting/core/pytest.py
 xtesting/core/robotframework.py
 xtesting/core/testcase.py
 xtesting/core/unit.py
 xtesting/core/vnf.py
 xtesting/samples/HelloWorld.robot
 xtesting/samples/__init__.py
 xtesting/samples/first.py
```

