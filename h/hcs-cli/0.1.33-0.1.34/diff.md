# Comparing `tmp/hcs-cli-0.1.33.tar.gz` & `tmp/hcs-cli-0.1.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcs-cli-0.1.33.tar", last modified: Mon Apr 24 20:30:23 2023, max compression
+gzip compressed data, was "hcs-cli-0.1.34.tar", last modified: Mon Apr 24 21:14:15 2023, max compression
```

## Comparing `hcs-cli-0.1.33.tar` & `hcs-cli-0.1.34.tar`

### file list

```diff
@@ -1,133 +1,141 @@
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 20:30:23.092853 hcs-cli-0.1.33/
--rw-r--r--   0 nanw       (501) staff       (20)     2820 2023-01-11 22:10:27.000000 hcs-cli-0.1.33/.gitignore
--rw-r--r--   0 nanw       (501) staff       (20)       82 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/CHANGELOG.md
--rw-r--r--   0 nanw       (501) staff       (20)      851 2023-04-24 20:30:04.000000 hcs-cli-0.1.33/Makefile
--rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-04-24 20:30:23.092163 hcs-cli-0.1.33/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)     1486 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/README.md
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 20:30:22.930924 hcs-cli-0.1.33/hcs_cli.egg-info/
--rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-04-24 20:30:22.000000 hcs-cli-0.1.33/hcs_cli.egg-info/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)     2873 2023-04-24 20:30:22.000000 hcs-cli-0.1.33/hcs_cli.egg-info/SOURCES.txt
--rw-r--r--   0 nanw       (501) staff       (20)        1 2023-04-24 20:30:22.000000 hcs-cli-0.1.33/hcs_cli.egg-info/dependency_links.txt
--rw-r--r--   0 nanw       (501) staff       (20)       43 2023-04-24 20:30:22.000000 hcs-cli-0.1.33/hcs_cli.egg-info/entry_points.txt
--rw-r--r--   0 nanw       (501) staff       (20)      127 2023-04-24 20:30:22.000000 hcs-cli-0.1.33/hcs_cli.egg-info/requires.txt
--rw-r--r--   0 nanw       (501) staff       (20)       11 2023-04-24 20:30:22.000000 hcs-cli-0.1.33/hcs_cli.egg-info/top_level.txt
--rw-r--r--   0 nanw       (501) staff       (20)       92 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/mypy.ini
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 20:30:22.884158 hcs-cli-0.1.33/payload/
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 20:30:22.932667 hcs-cli-0.1.33/payload/lcm/
--rw-r--r--   0 nanw       (501) staff       (20)      752 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/payload/lcm/zero.json
--rw-r--r--   0 nanw       (501) staff       (20)     1125 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/pyproject.toml
--rw-r--r--   0 nanw       (501) staff       (20)      194 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/requirements-dev.txt
--rw-r--r--   0 nanw       (501) staff       (20)      127 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/requirements.txt
--rw-r--r--   0 nanw       (501) staff       (20)       38 2023-04-24 20:30:23.093032 hcs-cli-0.1.33/setup.cfg
--rw-r--r--   0 nanw       (501) staff       (20)      545 2023-04-24 20:30:18.000000 hcs-cli-0.1.33/setup.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 20:30:22.937833 hcs-cli-0.1.33/tests/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/tests/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/tests/conftest.py
--rw-r--r--   0 nanw       (501) staff       (20)     2425 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/tests/test_utils.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 20:30:22.939701 hcs-cli-0.1.33/tests/vhcs/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/tests/vhcs/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 20:30:22.941078 hcs-cli-0.1.33/tests/vhcs/cli/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/tests/vhcs/cli/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 20:30:22.955471 hcs-cli-0.1.33/tests/vhcs/cli/cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/tests/vhcs/cli/cmds/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 20:30:22.959618 hcs-cli-0.1.33/tests/vhcs/cli/cmds/pki/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/tests/vhcs/cli/cmds/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/tests/vhcs/cli/cmds/pki/get_root_ca.py
--rw-r--r--   0 nanw       (501) staff       (20)      290 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/tests/vhcs/cli/cmds/test_auth.py
--rw-r--r--   0 nanw       (501) staff       (20)     1343 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/tests/vhcs/cli/cmds/test_context.py
--rw-r--r--   0 nanw       (501) staff       (20)      551 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/tests/vhcs/cli/cmds/test_profile.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 20:30:22.963721 hcs-cli-0.1.33/vhcs/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 21:25:27.000000 hcs-cli-0.1.33/vhcs/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)       87 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/__main__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 20:30:22.966623 hcs-cli-0.1.33/vhcs/cli/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.33/vhcs/cli/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 20:30:22.973699 hcs-cli-0.1.33/vhcs/cli/cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.33/vhcs/cli/cmds/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 20:30:22.974870 hcs-cli-0.1.33/vhcs/cli/cmds/admin/
--rw-r--r--   0 nanw       (501) staff       (20)       33 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/cli/cmds/admin/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 20:30:22.984562 hcs-cli-0.1.33/vhcs/cli/cmds/admin/edge/
--rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/cli/cmds/admin/edge/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      341 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/cli/cmds/admin/edge/get.py
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/cli/cmds/admin/edge/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 20:30:22.988719 hcs-cli-0.1.33/vhcs/cli/cmds/admin/template/
--rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/cli/cmds/admin/template/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      349 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/cli/cmds/admin/template/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1235 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/cli/cmds/admin/template/list.py
--rw-r--r--   0 nanw       (501) staff       (20)      375 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/cli/cmds/auth.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 20:30:22.991192 hcs-cli-0.1.33/vhcs/cli/cmds/lcm/
--rw-r--r--   0 nanw       (501) staff       (20)       31 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/cli/cmds/lcm/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 20:30:22.998494 hcs-cli-0.1.33/vhcs/cli/cmds/lcm/provider/
--rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/cli/cmds/lcm/provider/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      196 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/cli/cmds/lcm/provider/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      187 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/cli/cmds/lcm/provider/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      382 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/cli/cmds/lcm/provider/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 20:30:23.007565 hcs-cli-0.1.33/vhcs/cli/cmds/lcm/template/
--rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/cli/cmds/lcm/template/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1257 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/cli/cmds/lcm/template/create.py
--rw-r--r--   0 nanw       (501) staff       (20)      474 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/cli/cmds/lcm/template/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      235 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/cli/cmds/lcm/template/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      957 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/cli/cmds/lcm/template/list.py
--rw-r--r--   0 nanw       (501) staff       (20)     1656 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/cli/cmds/lcm/template/wait.py
--rw-r--r--   0 nanw       (501) staff       (20)      106 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/cli/cmds/lcm/test.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 20:30:23.026321 hcs-cli-0.1.33/vhcs/cli/cmds/pki/
--rw-r--r--   0 nanw       (501) staff       (20)       31 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/cli/cmds/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      551 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/cli/cmds/pki/delete_org_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      297 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/cli/cmds/pki/get_org_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      163 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/cli/cmds/pki/get_root_ca.py
--rw-r--r--   0 nanw       (501) staff       (20)     1220 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/cli/cmds/pki/sign_resource_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      106 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/cli/cmds/pki/test.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 20:30:23.028538 hcs-cli-0.1.33/vhcs/cli/cmds/profile/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.33/vhcs/cli/cmds/profile/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     3840 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/cli/cmds/profile/init.py
--rw-r--r--   0 nanw       (501) staff       (20)      171 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/cli/cmds/test.py
--rw-r--r--   0 nanw       (501) staff       (20)      332 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/cli/cmds/upgrade.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 20:30:23.032838 hcs-cli-0.1.33/vhcs/cli/cmds/vmhub/
--rw-r--r--   0 nanw       (501) staff       (20)       33 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/cli/cmds/vmhub/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      662 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/cli/cmds/vmhub/redeem-otp.py
--rw-r--r--   0 nanw       (501) staff       (20)      567 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/cli/cmds/vmhub/request-otp.py
--rw-r--r--   0 nanw       (501) staff       (20)      110 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/cli/cmds/vmhub/test.py
--rwxr-xr-x   0 nanw       (501) staff       (20)     2264 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/cli/main.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 20:30:23.034982 hcs-cli-0.1.33/vhcs/common/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.33/vhcs/common/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 20:30:23.051310 hcs-cli-0.1.33/vhcs/common/ctxp/
--rw-r--r--   0 nanw       (501) staff       (20)     1839 2023-04-06 02:05:21.000000 hcs-cli-0.1.33/vhcs/common/ctxp/README.md
--rw-r--r--   0 nanw       (501) staff       (20)      107 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/common/ctxp/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      611 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/common/ctxp/_init.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 20:30:23.057250 hcs-cli-0.1.33/vhcs/common/ctxp/built_in_cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.33/vhcs/common/ctxp/built_in_cmds/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1419 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/common/ctxp/built_in_cmds/context.py
--rw-r--r--   0 nanw       (501) staff       (20)     1819 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/common/ctxp/built_in_cmds/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)     4141 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/common/ctxp/cli_processor.py
--rw-r--r--   0 nanw       (501) staff       (20)      337 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/common/ctxp/config.py
--rw-r--r--   0 nanw       (501) staff       (20)     1656 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/common/ctxp/context.py
--rw-r--r--   0 nanw       (501) staff       (20)     5748 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/common/ctxp/fstore.py
--rw-r--r--   0 nanw       (501) staff       (20)      600 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/common/ctxp/init.py
--rw-r--r--   0 nanw       (501) staff       (20)     2162 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/common/ctxp/jsondot.py
--rw-r--r--   0 nanw       (501) staff       (20)     3974 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/common/ctxp/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)      899 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/common/ctxp/state.py
--rw-r--r--   0 nanw       (501) staff       (20)     2180 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/common/ctxp/util.py
--rw-r--r--   0 nanw       (501) staff       (20)     2656 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/common/ctxp/var_template.py
--rw-r--r--   0 nanw       (501) staff       (20)     4246 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/common/logger.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 20:30:23.067685 hcs-cli-0.1.33/vhcs/common/sglib/
--rw-r--r--   0 nanw       (501) staff       (20)       54 2023-04-06 02:05:21.000000 hcs-cli-0.1.33/vhcs/common/sglib/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     2504 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/common/sglib/auth.py
--rw-r--r--   0 nanw       (501) staff       (20)     3601 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/common/sglib/csp.py
--rw-r--r--   0 nanw       (501) staff       (20)     3870 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/common/sglib/ez_client.py
--rw-r--r--   0 nanw       (501) staff       (20)      549 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/common/sglib/hcs_client.py
--rw-r--r--   0 nanw       (501) staff       (20)      370 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/common/sglib/util.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 20:30:23.070718 hcs-cli-0.1.33/vhcs/config/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.33/vhcs/config/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     7771 2023-04-24 20:24:09.000000 hcs-cli-0.1.33/vhcs/config/hcs-deployments.yaml
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 20:30:23.083393 hcs-cli-0.1.33/vhcs/service/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/service/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      986 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/service/_util.py
--rw-r--r--   0 nanw       (501) staff       (20)      823 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/service/admin.py
--rw-r--r--   0 nanw       (501) staff       (20)     3217 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/service/lcm.py
--rw-r--r--   0 nanw       (501) staff       (20)      610 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/service/pki.py
--rw-r--r--   0 nanw       (501) staff       (20)      929 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/service/vmhub.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 20:30:23.090832 hcs-cli-0.1.33/vhcs/util/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.33/vhcs/util/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     2159 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/util/duration.py
--rw-r--r--   0 nanw       (501) staff       (20)     4688 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/util/pki_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     1160 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/util/query_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     1125 2023-04-24 20:24:05.000000 hcs-cli-0.1.33/vhcs/util/versions.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.908372 hcs-cli-0.1.34/
+-rw-r--r--   0 nanw       (501) staff       (20)     2820 2023-01-11 22:10:27.000000 hcs-cli-0.1.34/.gitignore
+-rw-r--r--   0 nanw       (501) staff       (20)       82 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/CHANGELOG.md
+-rw-r--r--   0 nanw       (501) staff       (20)      851 2023-04-24 20:31:20.000000 hcs-cli-0.1.34/Makefile
+-rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-04-24 21:14:15.907988 hcs-cli-0.1.34/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)     1486 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/README.md
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.720647 hcs-cli-0.1.34/hcs_cli.egg-info/
+-rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-04-24 21:14:15.000000 hcs-cli-0.1.34/hcs_cli.egg-info/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)     3039 2023-04-24 21:14:15.000000 hcs-cli-0.1.34/hcs_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 nanw       (501) staff       (20)        1 2023-04-24 21:14:15.000000 hcs-cli-0.1.34/hcs_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       43 2023-04-24 21:14:15.000000 hcs-cli-0.1.34/hcs_cli.egg-info/entry_points.txt
+-rw-r--r--   0 nanw       (501) staff       (20)      127 2023-04-24 21:14:15.000000 hcs-cli-0.1.34/hcs_cli.egg-info/requires.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       11 2023-04-24 21:14:15.000000 hcs-cli-0.1.34/hcs_cli.egg-info/top_level.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       92 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/mypy.ini
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.694623 hcs-cli-0.1.34/payload/
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.721841 hcs-cli-0.1.34/payload/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)      752 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/payload/lcm/zero.json
+-rw-r--r--   0 nanw       (501) staff       (20)     1125 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/pyproject.toml
+-rw-r--r--   0 nanw       (501) staff       (20)      194 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/requirements-dev.txt
+-rw-r--r--   0 nanw       (501) staff       (20)      127 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/requirements.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       38 2023-04-24 21:14:15.908471 hcs-cli-0.1.34/setup.cfg
+-rw-r--r--   0 nanw       (501) staff       (20)      545 2023-04-24 21:13:25.000000 hcs-cli-0.1.34/setup.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.723975 hcs-cli-0.1.34/tests/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/tests/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/tests/conftest.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2425 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/tests/test_utils.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.724607 hcs-cli-0.1.34/tests/vhcs/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/tests/vhcs/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.725193 hcs-cli-0.1.34/tests/vhcs/cli/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/tests/vhcs/cli/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.727697 hcs-cli-0.1.34/tests/vhcs/cli/cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/tests/vhcs/cli/cmds/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.728948 hcs-cli-0.1.34/tests/vhcs/cli/cmds/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/tests/vhcs/cli/cmds/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/tests/vhcs/cli/cmds/pki/get_root_ca.py
+-rw-r--r--   0 nanw       (501) staff       (20)      290 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/tests/vhcs/cli/cmds/test_auth.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1343 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/tests/vhcs/cli/cmds/test_context.py
+-rw-r--r--   0 nanw       (501) staff       (20)      551 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/tests/vhcs/cli/cmds/test_profile.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.729995 hcs-cli-0.1.34/vhcs/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 21:25:27.000000 hcs-cli-0.1.34/vhcs/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)       87 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/__main__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.731158 hcs-cli-0.1.34/vhcs/cli/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.34/vhcs/cli/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.733469 hcs-cli-0.1.34/vhcs/cli/cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.34/vhcs/cli/cmds/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.734065 hcs-cli-0.1.34/vhcs/cli/cmds/admin/
+-rw-r--r--   0 nanw       (501) staff       (20)       33 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/admin/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.735787 hcs-cli-0.1.34/vhcs/cli/cmds/admin/edge/
+-rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/admin/edge/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      341 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/admin/edge/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/admin/edge/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.737841 hcs-cli-0.1.34/vhcs/cli/cmds/admin/template/
+-rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/admin/template/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      349 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/admin/template/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1235 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/admin/template/list.py
+-rw-r--r--   0 nanw       (501) staff       (20)      375 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/auth.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.739081 hcs-cli-0.1.34/vhcs/cli/cmds/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)       31 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/lcm/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.741277 hcs-cli-0.1.34/vhcs/cli/cmds/lcm/provider/
+-rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/lcm/provider/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      196 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/lcm/provider/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      187 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/lcm/provider/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      382 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/lcm/provider/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.745041 hcs-cli-0.1.34/vhcs/cli/cmds/lcm/template/
+-rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/lcm/template/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1257 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/lcm/template/create.py
+-rw-r--r--   0 nanw       (501) staff       (20)      474 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/lcm/template/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      235 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/lcm/template/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      975 2023-04-24 21:13:51.000000 hcs-cli-0.1.34/vhcs/cli/cmds/lcm/template/list.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1656 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/lcm/template/wait.py
+-rw-r--r--   0 nanw       (501) staff       (20)      106 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/lcm/test.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.701395 hcs-cli-0.1.34/vhcs/cli/cmds/org/
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.746332 hcs-cli-0.1.34/vhcs/cli/cmds/org/datacenter/
+-rw-r--r--   0 nanw       (501) staff       (20)      249 2023-04-24 21:13:51.000000 hcs-cli-0.1.34/vhcs/cli/cmds/org/datacenter/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      410 2023-04-24 21:13:51.000000 hcs-cli-0.1.34/vhcs/cli/cmds/org/datacenter/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.747436 hcs-cli-0.1.34/vhcs/cli/cmds/org/detail/
+-rw-r--r--   0 nanw       (501) staff       (20)      310 2023-04-24 21:13:51.000000 hcs-cli-0.1.34/vhcs/cli/cmds/org/detail/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      605 2023-04-24 21:13:51.000000 hcs-cli-0.1.34/vhcs/cli/cmds/org/detail/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.750788 hcs-cli-0.1.34/vhcs/cli/cmds/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)       31 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      551 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/pki/delete_org_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      297 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/pki/get_org_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      163 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/pki/get_root_ca.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1220 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/pki/sign_resource_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      106 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/pki/test.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.751869 hcs-cli-0.1.34/vhcs/cli/cmds/profile/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.34/vhcs/cli/cmds/profile/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3840 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/profile/init.py
+-rw-r--r--   0 nanw       (501) staff       (20)      171 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/test.py
+-rw-r--r--   0 nanw       (501) staff       (20)      332 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/upgrade.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.753947 hcs-cli-0.1.34/vhcs/cli/cmds/vmhub/
+-rw-r--r--   0 nanw       (501) staff       (20)       33 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/vmhub/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      662 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/vmhub/redeem-otp.py
+-rw-r--r--   0 nanw       (501) staff       (20)      567 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/vmhub/request-otp.py
+-rw-r--r--   0 nanw       (501) staff       (20)      110 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/cmds/vmhub/test.py
+-rwxr-xr-x   0 nanw       (501) staff       (20)     2264 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/cli/main.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.755058 hcs-cli-0.1.34/vhcs/common/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.34/vhcs/common/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.762252 hcs-cli-0.1.34/vhcs/common/ctxp/
+-rw-r--r--   0 nanw       (501) staff       (20)     1839 2023-04-06 02:05:21.000000 hcs-cli-0.1.34/vhcs/common/ctxp/README.md
+-rw-r--r--   0 nanw       (501) staff       (20)      107 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/common/ctxp/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      611 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/common/ctxp/_init.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.763863 hcs-cli-0.1.34/vhcs/common/ctxp/built_in_cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.34/vhcs/common/ctxp/built_in_cmds/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1419 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/common/ctxp/built_in_cmds/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1819 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/common/ctxp/built_in_cmds/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4141 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/common/ctxp/cli_processor.py
+-rw-r--r--   0 nanw       (501) staff       (20)      337 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/common/ctxp/config.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1656 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/common/ctxp/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5748 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/common/ctxp/fstore.py
+-rw-r--r--   0 nanw       (501) staff       (20)      600 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/common/ctxp/init.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2162 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/common/ctxp/jsondot.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3974 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/common/ctxp/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)      899 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/common/ctxp/state.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2180 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/common/ctxp/util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2656 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/common/ctxp/var_template.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4246 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/common/logger.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.899474 hcs-cli-0.1.34/vhcs/common/sglib/
+-rw-r--r--   0 nanw       (501) staff       (20)       54 2023-04-06 02:05:21.000000 hcs-cli-0.1.34/vhcs/common/sglib/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2504 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/common/sglib/auth.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3601 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/common/sglib/csp.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3870 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/common/sglib/ez_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)      549 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/common/sglib/hcs_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)      370 2023-04-24 21:01:55.000000 hcs-cli-0.1.34/vhcs/common/sglib/util.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.900748 hcs-cli-0.1.34/vhcs/config/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.34/vhcs/config/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     7771 2023-04-24 20:24:09.000000 hcs-cli-0.1.34/vhcs/config/hcs-deployments.yaml
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.904693 hcs-cli-0.1.34/vhcs/service/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/service/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      986 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/service/_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)      823 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/service/admin.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3217 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/service/lcm.py
+-rw-r--r--   0 nanw       (501) staff       (20)      995 2023-04-24 21:13:51.000000 hcs-cli-0.1.34/vhcs/service/org_service.py
+-rw-r--r--   0 nanw       (501) staff       (20)      610 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/service/pki.py
+-rw-r--r--   0 nanw       (501) staff       (20)      929 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/service/vmhub.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-24 21:14:15.907268 hcs-cli-0.1.34/vhcs/util/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.34/vhcs/util/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2159 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/util/duration.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4688 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/util/pki_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1160 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/util/query_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1125 2023-04-24 20:24:05.000000 hcs-cli-0.1.34/vhcs/util/versions.py
```

### Comparing `hcs-cli-0.1.33/.gitignore` & `hcs-cli-0.1.34/.gitignore`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/Makefile` & `hcs-cli-0.1.34/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 test:
 	python3 -m unittest discover ./tests
 
 testinstall:
 	docker run --rm python /bin/bash -c "pip3 install hcs-cli && hcs profile"
 
 publish:
-	twine --repository hcs-cli upload dist/*
+	twine upload --repository hcs-cli dist/*
 
 install:
 	pip3 install hcs-cli
 
 wait:
 	sleep 30
```

### Comparing `hcs-cli-0.1.33/PKG-INFO` & `hcs-cli-0.1.34/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-cli
-Version: 0.1.33
+Version: 0.1.34
 Summary: Horizon Cloud Service CLI
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/nanw1103/hcs-cli
 Project-URL: Bug Tracker, https://github.com/nanw1103/hcs-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/nanw1103/hcs-cli
 Project-URL: changelog, https://github.com/nanw1103/hcs-cli/blob/master/CHANGELOG.md
```

### Comparing `hcs-cli-0.1.33/README.md` & `hcs-cli-0.1.34/README.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/hcs_cli.egg-info/PKG-INFO` & `hcs-cli-0.1.34/hcs_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-cli
-Version: 0.1.33
+Version: 0.1.34
 Summary: Horizon Cloud Service CLI
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/nanw1103/hcs-cli
 Project-URL: Bug Tracker, https://github.com/nanw1103/hcs-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/nanw1103/hcs-cli
 Project-URL: changelog, https://github.com/nanw1103/hcs-cli/blob/master/CHANGELOG.md
```

### Comparing `hcs-cli-0.1.33/hcs_cli.egg-info/SOURCES.txt` & `hcs-cli-0.1.34/hcs_cli.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -48,14 +48,18 @@
 vhcs/cli/cmds/lcm/provider/list.py
 vhcs/cli/cmds/lcm/template/__init__.py
 vhcs/cli/cmds/lcm/template/create.py
 vhcs/cli/cmds/lcm/template/delete.py
 vhcs/cli/cmds/lcm/template/get.py
 vhcs/cli/cmds/lcm/template/list.py
 vhcs/cli/cmds/lcm/template/wait.py
+vhcs/cli/cmds/org/datacenter/get.py
+vhcs/cli/cmds/org/datacenter/list.py
+vhcs/cli/cmds/org/detail/get.py
+vhcs/cli/cmds/org/detail/list.py
 vhcs/cli/cmds/pki/__init__.py
 vhcs/cli/cmds/pki/delete_org_cert.py
 vhcs/cli/cmds/pki/get_org_cert.py
 vhcs/cli/cmds/pki/get_root_ca.py
 vhcs/cli/cmds/pki/sign_resource_cert.py
 vhcs/cli/cmds/pki/test.py
 vhcs/cli/cmds/profile/__init__.py
@@ -90,14 +94,15 @@
 vhcs/common/sglib/util.py
 vhcs/config/__init__.py
 vhcs/config/hcs-deployments.yaml
 vhcs/service/__init__.py
 vhcs/service/_util.py
 vhcs/service/admin.py
 vhcs/service/lcm.py
+vhcs/service/org_service.py
 vhcs/service/pki.py
 vhcs/service/vmhub.py
 vhcs/util/__init__.py
 vhcs/util/duration.py
 vhcs/util/pki_util.py
 vhcs/util/query_util.py
 vhcs/util/versions.py
```

### Comparing `hcs-cli-0.1.33/payload/lcm/zero.json` & `hcs-cli-0.1.34/payload/lcm/zero.json`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/pyproject.toml` & `hcs-cli-0.1.34/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/setup.py` & `hcs-cli-0.1.34/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools_scm import get_version
 import os
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
-VERSION = "0.1.33"
+VERSION = "0.1.34"
 
 
 def get_version():
     version = VERSION
     local_version = os.environ.get("SCM_REV")
     if local_version:
         version += "+" + local_version
```

### Comparing `hcs-cli-0.1.33/tests/test_utils.py` & `hcs-cli-0.1.34/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/tests/vhcs/cli/cmds/test_context.py` & `hcs-cli-0.1.34/tests/vhcs/cli/cmds/test_context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/tests/vhcs/cli/cmds/test_profile.py` & `hcs-cli-0.1.34/tests/vhcs/cli/cmds/test_profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/vhcs/cli/cmds/admin/template/list.py` & `hcs-cli-0.1.34/vhcs/cli/cmds/admin/template/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/vhcs/cli/cmds/lcm/template/create.py` & `hcs-cli-0.1.34/vhcs/cli/cmds/lcm/template/create.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/vhcs/cli/cmds/lcm/template/list.py` & `hcs-cli-0.1.34/vhcs/cli/cmds/lcm/template/list.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import click
 from vhcs.service import lcm
 from vhcs.common.sglib.util import option_org_id, get_org_id
 from vhcs.common.ctxp.util import option_id_only
 
 
 @click.command("list")
-@click.option("--limit", "-l", type=int, required=False, default=20, help="Optionally, specify cloud provider type.")
+@click.option(
+    "--limit", "-l", type=int, required=False, default=20, help="Optionally, specify the number of records to return."
+)
 @option_org_id
 @option_id_only
 @click.option("--type", "-t", type=str, required=False, help="Optionally, specify cloud provider type.")
 @click.option("--name", "-n", type=str, required=False, help="Optionally, specify name pattern to find.")
 def list_templates(limit: int, org: str, id_only: bool, type: str, name: str):
     """List templates"""
     if org == "all":
```

### Comparing `hcs-cli-0.1.33/vhcs/cli/cmds/lcm/template/wait.py` & `hcs-cli-0.1.34/vhcs/cli/cmds/lcm/template/wait.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/vhcs/cli/cmds/pki/delete_org_cert.py` & `hcs-cli-0.1.34/vhcs/cli/cmds/pki/delete_org_cert.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/vhcs/cli/cmds/pki/sign_resource_cert.py` & `hcs-cli-0.1.34/vhcs/cli/cmds/pki/sign_resource_cert.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/vhcs/cli/cmds/profile/init.py` & `hcs-cli-0.1.34/vhcs/cli/cmds/profile/init.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/vhcs/cli/cmds/vmhub/redeem-otp.py` & `hcs-cli-0.1.34/vhcs/cli/cmds/vmhub/redeem-otp.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/vhcs/cli/cmds/vmhub/request-otp.py` & `hcs-cli-0.1.34/vhcs/cli/cmds/vmhub/request-otp.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/vhcs/cli/main.py` & `hcs-cli-0.1.34/vhcs/cli/main.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/vhcs/common/ctxp/README.md` & `hcs-cli-0.1.34/vhcs/common/ctxp/README.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/vhcs/common/ctxp/_init.py` & `hcs-cli-0.1.34/vhcs/common/ctxp/_init.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/vhcs/common/ctxp/built_in_cmds/context.py` & `hcs-cli-0.1.34/vhcs/common/ctxp/built_in_cmds/context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/vhcs/common/ctxp/built_in_cmds/profile.py` & `hcs-cli-0.1.34/vhcs/common/ctxp/built_in_cmds/profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/vhcs/common/ctxp/cli_processor.py` & `hcs-cli-0.1.34/vhcs/common/ctxp/cli_processor.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/vhcs/common/ctxp/context.py` & `hcs-cli-0.1.34/vhcs/common/ctxp/context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/vhcs/common/ctxp/fstore.py` & `hcs-cli-0.1.34/vhcs/common/ctxp/fstore.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/vhcs/common/ctxp/init.py` & `hcs-cli-0.1.34/vhcs/common/ctxp/init.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/vhcs/common/ctxp/jsondot.py` & `hcs-cli-0.1.34/vhcs/common/ctxp/jsondot.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/vhcs/common/ctxp/profile.py` & `hcs-cli-0.1.34/vhcs/common/ctxp/profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/vhcs/common/ctxp/state.py` & `hcs-cli-0.1.34/vhcs/common/ctxp/state.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/vhcs/common/ctxp/util.py` & `hcs-cli-0.1.34/vhcs/common/ctxp/util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/vhcs/common/ctxp/var_template.py` & `hcs-cli-0.1.34/vhcs/common/ctxp/var_template.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/vhcs/common/logger.py` & `hcs-cli-0.1.34/vhcs/common/logger.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/vhcs/common/sglib/auth.py` & `hcs-cli-0.1.34/vhcs/common/sglib/auth.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/vhcs/common/sglib/csp.py` & `hcs-cli-0.1.34/vhcs/common/sglib/csp.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/vhcs/common/sglib/ez_client.py` & `hcs-cli-0.1.34/vhcs/common/sglib/ez_client.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/vhcs/common/sglib/hcs_client.py` & `hcs-cli-0.1.34/vhcs/common/sglib/hcs_client.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/vhcs/config/hcs-deployments.yaml` & `hcs-cli-0.1.34/vhcs/config/hcs-deployments.yaml`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/vhcs/service/_util.py` & `hcs-cli-0.1.34/vhcs/service/_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/vhcs/service/admin.py` & `hcs-cli-0.1.34/vhcs/service/admin.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/vhcs/service/lcm.py` & `hcs-cli-0.1.34/vhcs/service/lcm.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/vhcs/service/pki.py` & `hcs-cli-0.1.34/vhcs/service/pki.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/vhcs/service/vmhub.py` & `hcs-cli-0.1.34/vhcs/service/vmhub.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/vhcs/util/duration.py` & `hcs-cli-0.1.34/vhcs/util/duration.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/vhcs/util/pki_util.py` & `hcs-cli-0.1.34/vhcs/util/pki_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/vhcs/util/query_util.py` & `hcs-cli-0.1.34/vhcs/util/query_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.33/vhcs/util/versions.py` & `hcs-cli-0.1.34/vhcs/util/versions.py`

 * *Files identical despite different names*

