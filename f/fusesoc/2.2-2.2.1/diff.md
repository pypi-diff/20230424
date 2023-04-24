# Comparing `tmp/fusesoc-2.2.tar.gz` & `tmp/fusesoc-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusesoc-2.2.tar", last modified: Tue Apr 18 10:07:46 2023, max compression
+gzip compressed data, was "fusesoc-2.2.1.tar", last modified: Mon Apr 24 13:26:51 2023, max compression
```

## Comparing `fusesoc-2.2.tar` & `fusesoc-2.2.1.tar`

### file list

```diff
@@ -1,265 +1,265 @@
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.593973 fusesoc-2.2/
--rw-r--r--   0 olof      (1000) olof      (1000)      421 2023-02-28 12:23:16.000000 fusesoc-2.2/.editorconfig
--rw-r--r--   0 olof      (1000) olof      (1000)       30 2023-02-28 12:28:34.000000 fusesoc-2.2/.flake8
--rw-r--r--   0 olof      (1000) olof      (1000)       85 2023-02-28 12:23:16.000000 fusesoc-2.2/.git-blame-ignore-revs
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.530973 fusesoc-2.2/.github/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.544973 fusesoc-2.2/.github/workflows/
--rw-r--r--   0 olof      (1000) olof      (1000)     1461 2023-02-28 12:28:15.000000 fusesoc-2.2/.github/workflows/ci.yml
--rw-r--r--   0 olof      (1000) olof      (1000)      226 2022-09-29 19:36:09.000000 fusesoc-2.2/.github/workflows/lint.yml
--rw-r--r--   0 olof      (1000) olof      (1000)      227 2022-09-29 19:36:09.000000 fusesoc-2.2/.gitignore
--rw-r--r--   0 olof      (1000) olof      (1000)     1182 2023-02-28 12:32:13.000000 fusesoc-2.2/.pre-commit-config.yaml
--rw-r--r--   0 olof      (1000) olof      (1000)      444 2023-02-28 12:23:16.000000 fusesoc-2.2/.readthedocs.yml
--rw-r--r--   0 olof      (1000) olof      (1000)     1315 2022-09-29 19:36:09.000000 fusesoc-2.2/LICENSE
--rw-r--r--   0 olof      (1000) olof      (1000)    17659 2023-04-18 10:07:10.000000 fusesoc-2.2/NEWS
--rw-r--r--   0 olof      (1000) olof      (1000)     6131 2023-04-18 10:07:46.592973 fusesoc-2.2/PKG-INFO
--rw-r--r--   0 olof      (1000) olof      (1000)     5491 2023-02-28 12:32:13.000000 fusesoc-2.2/README.md
--rw-r--r--   0 olof      (1000) olof      (1000)      259 2023-02-28 12:28:15.000000 fusesoc-2.2/dev-requirements.txt
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.544973 fusesoc-2.2/doc/
--rw-r--r--   0 olof      (1000) olof      (1000)       59 2023-02-28 12:23:16.000000 fusesoc-2.2/doc/requirements.txt
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.545973 fusesoc-2.2/doc/source/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.545973 fusesoc-2.2/doc/source/_static/
--rw-r--r--   0 olof      (1000) olof      (1000)      365 2022-09-29 19:36:09.000000 fusesoc-2.2/doc/source/_static/theme_overrides.css
--rw-r--r--   0 olof      (1000) olof      (1000)     6282 2023-02-28 12:28:15.000000 fusesoc-2.2/doc/source/conf.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.545973 fusesoc-2.2/doc/source/dev/
--rw-r--r--   0 olof      (1000) olof      (1000)     4668 2023-02-28 12:28:15.000000 fusesoc-2.2/doc/source/dev/devsetup.rst
--rw-r--r--   0 olof      (1000) olof      (1000)      143 2022-09-29 19:36:09.000000 fusesoc-2.2/doc/source/dev/index.rst
--rw-r--r--   0 olof      (1000) olof      (1000)      839 2022-09-29 19:36:09.000000 fusesoc-2.2/doc/source/index.rst
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.546973 fusesoc-2.2/doc/source/ref/
--rw-r--r--   0 olof      (1000) olof      (1000)    15496 2023-02-28 12:23:16.000000 fusesoc-2.2/doc/source/ref/capi1.rst
--rw-r--r--   0 olof      (1000) olof      (1000)     1723 2023-02-28 12:28:15.000000 fusesoc-2.2/doc/source/ref/glossary.rst
--rw-r--r--   0 olof      (1000) olof      (1000)      175 2023-02-28 12:28:15.000000 fusesoc-2.2/doc/source/ref/index.rst
--rw-r--r--   0 olof      (1000) olof      (1000)    10054 2023-02-28 12:23:16.000000 fusesoc-2.2/doc/source/ref/migrations.rst
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.548973 fusesoc-2.2/doc/source/user/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.550973 fusesoc-2.2/doc/source/user/build_system/
--rw-r--r--   0 olof      (1000) olof      (1000)    12263 2023-02-28 12:28:15.000000 fusesoc-2.2/doc/source/user/build_system/core_files.rst
--rw-r--r--   0 olof      (1000) olof      (1000)     7514 2023-02-28 12:23:16.000000 fusesoc-2.2/doc/source/user/build_system/dependencies.rst
--rw-r--r--   0 olof      (1000) olof      (1000)     1603 2023-02-28 12:32:13.000000 fusesoc-2.2/doc/source/user/build_system/eda_flows.rst
--rw-r--r--   0 olof      (1000) olof      (1000)     7507 2023-02-28 12:28:34.000000 fusesoc-2.2/doc/source/user/build_system/flags.rst
--rw-r--r--   0 olof      (1000) olof      (1000)     2978 2023-02-28 12:32:13.000000 fusesoc-2.2/doc/source/user/build_system/flow_options.rst
--rw-r--r--   0 olof      (1000) olof      (1000)    12067 2023-02-28 12:32:13.000000 fusesoc-2.2/doc/source/user/build_system/generators.rst
--rw-r--r--   0 olof      (1000) olof      (1000)      129 2022-09-29 19:36:09.000000 fusesoc-2.2/doc/source/user/build_system/hooks.rst
--rw-r--r--   0 olof      (1000) olof      (1000)     1902 2023-02-28 12:32:13.000000 fusesoc-2.2/doc/source/user/build_system/index.rst
--rw-r--r--   0 olof      (1000) olof      (1000)     2267 2023-02-28 12:32:13.000000 fusesoc-2.2/doc/source/user/build_system/tool_options.rst
--rw-r--r--   0 olof      (1000) olof      (1000)       87 2022-09-29 19:36:09.000000 fusesoc-2.2/doc/source/user/build_system/vpi.rst
--rw-r--r--   0 olof      (1000) olof      (1000)     1502 2023-02-28 12:28:34.000000 fusesoc-2.2/doc/source/user/cli.rst
--rw-r--r--   0 olof      (1000) olof      (1000)     1149 2022-09-29 19:36:09.000000 fusesoc-2.2/doc/source/user/index.rst
--rw-r--r--   0 olof      (1000) olof      (1000)     4013 2023-04-17 12:12:08.000000 fusesoc-2.2/doc/source/user/installation.rst
--rw-r--r--   0 olof      (1000) olof      (1000)     2015 2022-09-29 19:36:09.000000 fusesoc-2.2/doc/source/user/introduction.rst
--rw-r--r--   0 olof      (1000) olof      (1000)     1381 2022-09-29 19:36:09.000000 fusesoc-2.2/doc/source/user/knowledgebase.rst
--rw-r--r--   0 olof      (1000) olof      (1000)     6678 2023-02-28 12:28:34.000000 fusesoc-2.2/doc/source/user/overview.rst
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.551973 fusesoc-2.2/doc/source/user/package_manager/
--rw-r--r--   0 olof      (1000) olof      (1000)     2888 2023-02-28 12:32:13.000000 fusesoc-2.2/doc/source/user/package_manager/index.rst
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.551973 fusesoc-2.2/extras/
--rw-r--r--   0 olof      (1000) olof      (1000)      766 2022-09-29 19:36:09.000000 fusesoc-2.2/extras/bash-completion
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.553973 fusesoc-2.2/fusesoc/
--rw-r--r--   0 olof      (1000) olof      (1000)      250 2022-09-29 19:36:09.000000 fusesoc-2.2/fusesoc/__init__.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.557973 fusesoc-2.2/fusesoc/capi2/
--rw-r--r--   0 olof      (1000) olof      (1000)      141 2022-09-29 19:36:09.000000 fusesoc-2.2/fusesoc/capi2/__init__.py
--rw-r--r--   0 olof      (1000) olof      (1000)    21425 2023-04-18 10:07:10.000000 fusesoc-2.2/fusesoc/capi2/core.py
--rw-r--r--   0 olof      (1000) olof      (1000)     5895 2023-04-18 10:07:10.000000 fusesoc-2.2/fusesoc/capi2/coredata.py
--rw-r--r--   0 olof      (1000) olof      (1000)      720 2023-04-17 12:12:08.000000 fusesoc-2.2/fusesoc/capi2/coreparser.py
--rw-r--r--   0 olof      (1000) olof      (1000)     5825 2023-04-17 12:12:08.000000 fusesoc-2.2/fusesoc/capi2/exprs.py
--rw-r--r--   0 olof      (1000) olof      (1000)     2046 2023-04-17 12:12:08.000000 fusesoc-2.2/fusesoc/capi2/generator.py
--rw-r--r--   0 olof      (1000) olof      (1000)    22016 2023-04-18 10:07:10.000000 fusesoc-2.2/fusesoc/capi2/json_schema.py
--rw-r--r--   0 olof      (1000) olof      (1000)     6424 2023-02-28 12:32:13.000000 fusesoc-2.2/fusesoc/config.py
--rw-r--r--   0 olof      (1000) olof      (1000)      340 2023-02-28 12:28:15.000000 fusesoc-2.2/fusesoc/core.py
--rw-r--r--   0 olof      (1000) olof      (1000)    14081 2023-04-17 12:12:08.000000 fusesoc-2.2/fusesoc/coremanager.py
--rw-r--r--   0 olof      (1000) olof      (1000)    25699 2023-04-17 12:20:14.000000 fusesoc-2.2/fusesoc/edalizer.py
--rw-r--r--   0 olof      (1000) olof      (1000)     2870 2023-02-28 12:32:13.000000 fusesoc-2.2/fusesoc/librarymanager.py
--rw-r--r--   0 olof      (1000) olof      (1000)    22647 2023-04-17 12:12:08.000000 fusesoc-2.2/fusesoc/main.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.557973 fusesoc-2.2/fusesoc/parser/
--rw-r--r--   0 olof      (1000) olof      (1000)      141 2023-04-17 12:12:08.000000 fusesoc-2.2/fusesoc/parser/__init__.py
--rw-r--r--   0 olof      (1000) olof      (1000)     2335 2023-04-17 12:12:08.000000 fusesoc-2.2/fusesoc/parser/coreparser.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.559973 fusesoc-2.2/fusesoc/provider/
--rw-r--r--   0 olof      (1000) olof      (1000)      279 2023-02-28 12:28:15.000000 fusesoc-2.2/fusesoc/provider/__init__.py
--rw-r--r--   0 olof      (1000) olof      (1000)     2253 2023-02-28 12:53:14.000000 fusesoc-2.2/fusesoc/provider/git.py
--rw-r--r--   0 olof      (1000) olof      (1000)     1364 2023-02-28 12:28:15.000000 fusesoc-2.2/fusesoc/provider/github.py
--rw-r--r--   0 olof      (1000) olof      (1000)      602 2023-02-28 12:28:15.000000 fusesoc-2.2/fusesoc/provider/local.py
--rw-r--r--   0 olof      (1000) olof      (1000)     1188 2022-09-29 19:36:09.000000 fusesoc-2.2/fusesoc/provider/opencores.py
--rw-r--r--   0 olof      (1000) olof      (1000)     2673 2023-02-28 12:28:34.000000 fusesoc-2.2/fusesoc/provider/provider.py
--rw-r--r--   0 olof      (1000) olof      (1000)     1852 2023-02-28 12:28:15.000000 fusesoc-2.2/fusesoc/provider/url.py
--rw-r--r--   0 olof      (1000) olof      (1000)     5521 2023-04-17 12:12:08.000000 fusesoc-2.2/fusesoc/utils.py
--rw-r--r--   0 olof      (1000) olof      (1000)      171 2023-04-18 10:07:46.000000 fusesoc-2.2/fusesoc/version.py
--rw-r--r--   0 olof      (1000) olof      (1000)     5135 2023-02-28 12:28:15.000000 fusesoc-2.2/fusesoc/vlnv.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.554973 fusesoc-2.2/fusesoc.egg-info/
--rw-r--r--   0 olof      (1000) olof      (1000)     6131 2023-04-18 10:07:46.000000 fusesoc-2.2/fusesoc.egg-info/PKG-INFO
--rw-r--r--   0 olof      (1000) olof      (1000)     6624 2023-04-18 10:07:46.000000 fusesoc-2.2/fusesoc.egg-info/SOURCES.txt
--rw-r--r--   0 olof      (1000) olof      (1000)        1 2023-04-18 10:07:46.000000 fusesoc-2.2/fusesoc.egg-info/dependency_links.txt
--rw-r--r--   0 olof      (1000) olof      (1000)       46 2023-04-18 10:07:46.000000 fusesoc-2.2/fusesoc.egg-info/entry_points.txt
--rw-r--r--   0 olof      (1000) olof      (1000)       64 2023-04-18 10:07:46.000000 fusesoc-2.2/fusesoc.egg-info/requires.txt
--rw-r--r--   0 olof      (1000) olof      (1000)        8 2023-04-18 10:07:46.000000 fusesoc-2.2/fusesoc.egg-info/top_level.txt
--rw-r--r--   0 olof      (1000) olof      (1000)       38 2023-04-18 10:07:46.593973 fusesoc-2.2/setup.cfg
--rw-r--r--   0 olof      (1000) olof      (1000)     1689 2023-04-17 12:12:08.000000 fusesoc-2.2/setup.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.562973 fusesoc-2.2/tests/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.533973 fusesoc-2.2/tests/capi2_cores/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.564973 fusesoc-2.2/tests/capi2_cores/deptree/
--rw-r--r--   0 olof      (1000) olof      (1000)      375 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/deptree/child1.core
--rw-r--r--   0 olof      (1000) olof      (1000)      338 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/deptree/child2.core
--rw-r--r--   0 olof      (1000) olof      (1000)      338 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/deptree/child3.core
--rw-r--r--   0 olof      (1000) olof      (1000)      304 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/deptree/child4.core
--rw-r--r--   0 olof      (1000) olof      (1000)     1288 2023-02-28 12:23:16.000000 fusesoc-2.2/tests/capi2_cores/deptree/generated_child_a.core
--rw-r--r--   0 olof      (1000) olof      (1000)      444 2023-02-28 12:23:16.000000 fusesoc-2.2/tests/capi2_cores/deptree/generated_child_a.py
--rw-r--r--   0 olof      (1000) olof      (1000)      802 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/deptree/root.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.564973 fusesoc-2.2/tests/capi2_cores/files_out_of_hierarchy/
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2023-02-28 12:23:16.000000 fusesoc-2.2/tests/capi2_cores/files_out_of_hierarchy/bad.sv
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.565973 fusesoc-2.2/tests/capi2_cores/files_out_of_hierarchy/subdir/
--rw-r--r--   0 olof      (1000) olof      (1000)      533 2023-02-28 12:23:16.000000 fusesoc-2.2/tests/capi2_cores/files_out_of_hierarchy/subdir/files_out_of_hierarchy.core
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2023-02-28 12:23:16.000000 fusesoc-2.2/tests/capi2_cores/files_out_of_hierarchy/subdir/good.sv
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.572973 fusesoc-2.2/tests/capi2_cores/misc/
--rw-r--r--   0 olof      (1000) olof      (1000)      493 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/misc/append.core
--rw-r--r--   0 olof      (1000) olof      (1000)      646 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/misc/depends.core
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/misc/dontpickthisfile
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/misc/dummy.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/misc/empty.core
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/misc/f1
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/misc/f2
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/misc/f3
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/misc/f4
--rw-r--r--   0 olof      (1000) olof      (1000)     1496 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/misc/files.core
--rw-r--r--   0 olof      (1000) olof      (1000)      447 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/capi2_cores/misc/flags.core
--rw-r--r--   0 olof      (1000) olof      (1000)      502 2023-02-28 12:28:43.000000 fusesoc-2.2/tests/capi2_cores/misc/flow.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.573973 fusesoc-2.2/tests/capi2_cores/misc/generate/
--rw-r--r--   0 olof      (1000) olof      (1000)       10 2023-02-28 12:32:13.000000 fusesoc-2.2/tests/capi2_cores/misc/generate/file_cachetest
--rw-r--r--   0 olof      (1000) olof      (1000)      914 2023-02-28 12:32:13.000000 fusesoc-2.2/tests/capi2_cores/misc/generate/generate.core
--rw-r--r--   0 olof      (1000) olof      (1000)      375 2023-02-28 12:32:13.000000 fusesoc-2.2/tests/capi2_cores/misc/generate/generators.core
--rw-r--r--   0 olof      (1000) olof      (1000)      553 2023-02-28 12:23:16.000000 fusesoc-2.2/tests/capi2_cores/misc/generate/testgen.py
--rw-r--r--   0 olof      (1000) olof      (1000)      886 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/misc/hooks.core
--rw-r--r--   0 olof      (1000) olof      (1000)     1471 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/misc/parameters.core
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/misc/scriptfile
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.574973 fusesoc-2.2/tests/capi2_cores/misc/subdir/
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/misc/subdir/dummy.extra
--rw-r--r--   0 olof      (1000) olof      (1000)      356 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/misc/targets.core
--rw-r--r--   0 olof      (1000) olof      (1000)      301 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/misc/toplevel.core
--rw-r--r--   0 olof      (1000) olof      (1000)      609 2023-02-28 12:28:34.000000 fusesoc-2.2/tests/capi2_cores/misc/typecheck.core
--rw-r--r--   0 olof      (1000) olof      (1000)      244 2023-04-17 12:12:08.000000 fusesoc-2.2/tests/capi2_cores/misc/uncachable.core
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/misc/vhdlfile
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/misc/vlogfile
--rw-r--r--   0 olof      (1000) olof      (1000)      562 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/misc/vpi.core
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/misc/vpifile
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.574973 fusesoc-2.2/tests/capi2_cores/parser/
--rw-r--r--   0 olof      (1000) olof      (1000)      334 2023-04-17 12:12:08.000000 fusesoc-2.2/tests/capi2_cores/parser/no_additional_properties.core
--rw-r--r--   0 olof      (1000) olof      (1000)      482 2023-04-17 12:12:08.000000 fusesoc-2.2/tests/capi2_cores/parser/with_additional_properties.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.576973 fusesoc-2.2/tests/capi2_cores/providers/
--rw-r--r--   0 olof      (1000) olof      (1000)      309 2023-02-28 12:28:43.000000 fusesoc-2.2/tests/capi2_cores/providers/url_simple.core
--rw-r--r--   0 olof      (1000) olof      (1000)      348 2023-02-28 12:28:43.000000 fusesoc-2.2/tests/capi2_cores/providers/url_simple_with_user_agent.core
--rw-r--r--   0 olof      (1000) olof      (1000)      308 2023-02-28 12:28:43.000000 fusesoc-2.2/tests/capi2_cores/providers/url_tar.core
--rw-r--r--   0 olof      (1000) olof      (1000)      305 2023-02-28 12:28:43.000000 fusesoc-2.2/tests/capi2_cores/providers/url_zip.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.577973 fusesoc-2.2/tests/capi2_cores/virtual/
--rw-r--r--   0 olof      (1000) olof      (1000)      325 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/capi2_cores/virtual/impl1.core
--rw-r--r--   0 olof      (1000) olof      (1000)      325 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/capi2_cores/virtual/impl2.core
--rw-r--r--   0 olof      (1000) olof      (1000)      349 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/capi2_cores/virtual/user.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.539973 fusesoc-2.2/tests/cores/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.577973 fusesoc-2.2/tests/cores/adv_debug_sys/
--rw-r--r--   0 olof      (1000) olof      (1000)     1225 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/adv_debug_sys/adv_debug_sys.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.577973 fusesoc-2.2/tests/cores/atlys/
--rw-r--r--   0 olof      (1000) olof      (1000)     2269 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/atlys/atlys.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.578973 fusesoc-2.2/tests/cores/atlys/data/
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/atlys/data/atlys.ucf
--rw-r--r--   0 olof      (1000) olof      (1000)      176 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/atlys/data/dummy_backend_tcl_file.tcl
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.579973 fusesoc-2.2/tests/cores/elf-loader/
--rwxr-xr-x   0 olof      (1000) olof      (1000)      184 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/elf-loader/check_libelf.sh
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/elf-loader/elf-loader.c
--rw-r--r--   0 olof      (1000) olof      (1000)     1458 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/elf-loader/elf-loader.core
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/elf-loader/vpi_wrapper.c
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.579973 fusesoc-2.2/tests/cores/gpio/
--rw-r--r--   0 olof      (1000) olof      (1000)      379 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/gpio/gpio.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.579973 fusesoc-2.2/tests/cores/jtag_tap/
--rw-r--r--   0 olof      (1000) olof      (1000)      474 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/jtag_tap/jtag_tap-1.13.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.580973 fusesoc-2.2/tests/cores/libstorage/
--rw-r--r--   0 olof      (1000) olof      (1000)      529 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/libstorage/libstorage-1.0.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.583973 fusesoc-2.2/tests/cores/misc/
--rw-r--r--   0 olof      (1000) olof      (1000)     1051 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/misc/c3demo.core
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/misc/c3demo.pcf
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.583973 fusesoc-2.2/tests/cores/misc/copytocore/
--rw-r--r--   0 olof      (1000) olof      (1000)      421 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/misc/copytocore/copytocore.core
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/misc/copytocore/dummy.tcl
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.583973 fusesoc-2.2/tests/cores/misc/copytocore/subdir/
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/misc/copytocore/subdir/dummy.extra
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/misc/dummy.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/misc/dummy.xci
--rw-r--r--   0 olof      (1000) olof      (1000)      854 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/misc/filetypes.core
--rw-r--r--   0 olof      (1000) olof      (1000)     1391 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/misc/ghdltest.core
--rw-r--r--   0 olof      (1000) olof      (1000)      356 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/misc/gitcore.core
--rw-r--r--   0 olof      (1000) olof      (1000)      698 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/misc/no_exe_script.core
--rw-r--r--   0 olof      (1000) olof      (1000)      234 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/misc/nomain.core
--rw-r--r--   0 olof      (1000) olof      (1000)      399 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/misc/opencorescore.core
--rw-r--r--   0 olof      (1000) olof      (1000)     2482 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/misc/paramtest.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.584973 fusesoc-2.2/tests/cores/misc/scripts/
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/misc/scripts/no_exe_script
--rwxr-xr-x   0 olof      (1000) olof      (1000)      192 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/misc/scripts/post_build_script
--rwxr-xr-x   0 olof      (1000) olof      (1000)      173 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/misc/scripts/post_run_script
--rwxr-xr-x   0 olof      (1000) olof      (1000)      191 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/misc/scripts/pre_build_script
--rwxr-xr-x   0 olof      (1000) olof      (1000)      172 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/misc/scripts/pre_run_script
--rw-r--r--   0 olof      (1000) olof      (1000)     1474 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/misc/scriptscore.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.584973 fusesoc-2.2/tests/cores/misc/subdir/
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/misc/subdir/dummy.extra
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.585973 fusesoc-2.2/tests/cores/mor1kx/
--rw-r--r--   0 olof      (1000) olof      (1000)     2807 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/mor1kx/mor1kx-3.1.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.585973 fusesoc-2.2/tests/cores/mor1kx-arty/
--rw-r--r--   0 olof      (1000) olof      (1000)      702 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/mor1kx-arty/mor1kx-arty.core
--rw-r--r--   0 olof      (1000) olof      (1000)      337 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/mor1kx-arty/mor1kx-arty.system
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.585973 fusesoc-2.2/tests/cores/mor1kx-generic/
--rw-r--r--   0 olof      (1000) olof      (1000)     3024 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/mor1kx-generic/mor1kx-generic.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.586973 fusesoc-2.2/tests/cores/mor1kx-generic/scripts/
--rwxr-xr-x   0 olof      (1000) olof      (1000)      173 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/mor1kx-generic/scripts/post_run_script
--rwxr-xr-x   0 olof      (1000) olof      (1000)      174 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/mor1kx-generic/scripts/pre_build_script
--rwxr-xr-x   0 olof      (1000) olof      (1000)      172 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/mor1kx-generic/scripts/pre_run_script
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.586973 fusesoc-2.2/tests/cores/sockit/
--rw-r--r--   0 olof      (1000) olof      (1000)     1596 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/sockit/sockit.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.586973 fusesoc-2.2/tests/cores/uart16550/
--rw-r--r--   0 olof      (1000) olof      (1000)      920 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/uart16550/uart16550-1.5.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.587973 fusesoc-2.2/tests/cores/verilator_tb_utils/
--rw-r--r--   0 olof      (1000) olof      (1000)      715 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/verilator_tb_utils/verilator_tb_utils.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.587973 fusesoc-2.2/tests/cores/verilog-arbiter/
--rw-r--r--   0 olof      (1000) olof      (1000)      761 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/verilog-arbiter/verilog-arbiter-r1.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.588973 fusesoc-2.2/tests/cores/verilog_utils/
--rw-r--r--   0 olof      (1000) olof      (1000)      573 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/verilog_utils/verilog_utils.core
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/verilog_utils/verilog_utils.vh
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.588973 fusesoc-2.2/tests/cores/vga_lcd/
--rw-r--r--   0 olof      (1000) olof      (1000)     1200 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/vga_lcd/vga_lcd.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.588973 fusesoc-2.2/tests/cores/vlog_tb_utils/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.588973 fusesoc-2.2/tests/cores/vlog_tb_utils/files/
--rw-r--r--   0 olof      (1000) olof      (1000)      554 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/vlog_tb_utils/files/0001-testpatch.patch
--rw-r--r--   0 olof      (1000) olof      (1000)     1456 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/vlog_tb_utils/vlog_tb_utils-1.1.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.589973 fusesoc-2.2/tests/cores/wb_common/
--rw-r--r--   0 olof      (1000) olof      (1000)      655 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/wb_common/wb_common.core
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/wb_common/wb_common.v
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/wb_common/wb_common_params.v
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.589973 fusesoc-2.2/tests/cores/wb_intercon/
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/wb_intercon/dummy_icarus.v
--rw-r--r--   0 olof      (1000) olof      (1000)     1329 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/wb_intercon/wb_intercon-1.0.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.590973 fusesoc-2.2/tests/test_capi2/
--rw-r--r--   0 olof      (1000) olof      (1000)       90 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/test_capi2/generators.info
--rw-r--r--   0 olof      (1000) olof      (1000)      207 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/test_capi2/targets.info
--rw-r--r--   0 olof      (1000) olof      (1000)    21205 2023-04-17 12:27:19.000000 fusesoc-2.2/tests/test_capi2.py
--rw-r--r--   0 olof      (1000) olof      (1000)      335 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/test_common.py
--rw-r--r--   0 olof      (1000) olof      (1000)     2230 2023-02-28 12:28:34.000000 fusesoc-2.2/tests/test_config.py
--rw-r--r--   0 olof      (1000) olof      (1000)     7657 2023-03-23 19:51:07.000000 fusesoc-2.2/tests/test_coremanager.py
--rw-r--r--   0 olof      (1000) olof      (1000)     3988 2023-03-23 19:51:07.000000 fusesoc-2.2/tests/test_edalizer.py
--rw-r--r--   0 olof      (1000) olof      (1000)     1619 2023-03-23 19:51:07.000000 fusesoc-2.2/tests/test_exprs.py
--rw-r--r--   0 olof      (1000) olof      (1000)     1484 2023-02-28 12:28:34.000000 fusesoc-2.2/tests/test_ignored_dirs.py
--rw-r--r--   0 olof      (1000) olof      (1000)     5516 2023-02-28 12:32:13.000000 fusesoc-2.2/tests/test_libraries.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.590973 fusesoc-2.2/tests/test_provider/
--rw-r--r--   0 olof      (1000) olof      (1000)      114 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/test_provider/file.tar.gz
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/test_provider/file.v
--rw-r--r--   0 olof      (1000) olof      (1000)      162 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/test_provider/file.zip
--rw-r--r--   0 olof      (1000) olof      (1000)     1141 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/test_provider/vlog_functions.v
--rw-r--r--   0 olof      (1000) olof      (1000)     3000 2023-04-17 12:12:08.000000 fusesoc-2.2/tests/test_provider.py
--rw-r--r--   0 olof      (1000) olof      (1000)     2177 2023-02-28 12:23:16.000000 fusesoc-2.2/tests/test_vlnv.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.540973 fusesoc-2.2/tests/userguide/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.591973 fusesoc-2.2/tests/userguide/blinky/
--rw-r--r--   0 olof      (1000) olof      (1000)     1743 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/userguide/blinky/blinky.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.591973 fusesoc-2.2/tests/userguide/blinky/data/
--rw-r--r--   0 olof      (1000) olof      (1000)      458 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/userguide/blinky/data/nexys_video.xdc
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.591973 fusesoc-2.2/tests/userguide/blinky/rtl/
--rw-r--r--   0 olof      (1000) olof      (1000)      636 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/userguide/blinky/rtl/blinky.sv
--rw-r--r--   0 olof      (1000) olof      (1000)      153 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/userguide/blinky/rtl/macros.svh
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.592973 fusesoc-2.2/tests/userguide/blinky/tb/
--rw-r--r--   0 olof      (1000) olof      (1000)     1031 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/userguide/blinky/tb/blinky_tb.sv
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.592973 fusesoc-2.2/tests/userguide/dualblinky/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.592973 fusesoc-2.2/tests/userguide/dualblinky/data/
--rw-r--r--   0 olof      (1000) olof      (1000)      574 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/userguide/dualblinky/data/nexys_video.xdc
--rw-r--r--   0 olof      (1000) olof      (1000)      792 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/userguide/dualblinky/dualblinky.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.592973 fusesoc-2.2/tests/userguide/dualblinky/rtl/
--rw-r--r--   0 olof      (1000) olof      (1000)      665 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/userguide/dualblinky/rtl/dualblinky.sv
--rw-r--r--   0 olof      (1000) olof      (1000)     3014 2023-02-28 12:32:13.000000 fusesoc-2.2/tox.ini
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.449414 fusesoc-2.2.1/
+-rw-r--r--   0 olof      (1000) olof      (1000)      421 2023-02-28 12:23:16.000000 fusesoc-2.2.1/.editorconfig
+-rw-r--r--   0 olof      (1000) olof      (1000)       30 2023-02-28 12:28:34.000000 fusesoc-2.2.1/.flake8
+-rw-r--r--   0 olof      (1000) olof      (1000)       85 2023-02-28 12:23:16.000000 fusesoc-2.2.1/.git-blame-ignore-revs
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.411413 fusesoc-2.2.1/.github/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.418413 fusesoc-2.2.1/.github/workflows/
+-rw-r--r--   0 olof      (1000) olof      (1000)     1461 2023-02-28 12:28:15.000000 fusesoc-2.2.1/.github/workflows/ci.yml
+-rw-r--r--   0 olof      (1000) olof      (1000)      226 2022-09-29 19:36:09.000000 fusesoc-2.2.1/.github/workflows/lint.yml
+-rw-r--r--   0 olof      (1000) olof      (1000)      227 2022-09-29 19:36:09.000000 fusesoc-2.2.1/.gitignore
+-rw-r--r--   0 olof      (1000) olof      (1000)     1182 2023-02-28 12:32:13.000000 fusesoc-2.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 olof      (1000) olof      (1000)      444 2023-02-28 12:23:16.000000 fusesoc-2.2.1/.readthedocs.yml
+-rw-r--r--   0 olof      (1000) olof      (1000)     1315 2022-09-29 19:36:09.000000 fusesoc-2.2.1/LICENSE
+-rw-r--r--   0 olof      (1000) olof      (1000)    17714 2023-04-24 13:24:59.000000 fusesoc-2.2.1/NEWS
+-rw-r--r--   0 olof      (1000) olof      (1000)     6133 2023-04-24 13:26:51.448414 fusesoc-2.2.1/PKG-INFO
+-rw-r--r--   0 olof      (1000) olof      (1000)     5491 2023-02-28 12:32:13.000000 fusesoc-2.2.1/README.md
+-rw-r--r--   0 olof      (1000) olof      (1000)      259 2023-02-28 12:28:15.000000 fusesoc-2.2.1/dev-requirements.txt
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.419413 fusesoc-2.2.1/doc/
+-rw-r--r--   0 olof      (1000) olof      (1000)       59 2023-02-28 12:23:16.000000 fusesoc-2.2.1/doc/requirements.txt
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.419413 fusesoc-2.2.1/doc/source/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.419413 fusesoc-2.2.1/doc/source/_static/
+-rw-r--r--   0 olof      (1000) olof      (1000)      365 2022-09-29 19:36:09.000000 fusesoc-2.2.1/doc/source/_static/theme_overrides.css
+-rw-r--r--   0 olof      (1000) olof      (1000)     6282 2023-02-28 12:28:15.000000 fusesoc-2.2.1/doc/source/conf.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.420414 fusesoc-2.2.1/doc/source/dev/
+-rw-r--r--   0 olof      (1000) olof      (1000)     4668 2023-02-28 12:28:15.000000 fusesoc-2.2.1/doc/source/dev/devsetup.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)      143 2022-09-29 19:36:09.000000 fusesoc-2.2.1/doc/source/dev/index.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)      839 2022-09-29 19:36:09.000000 fusesoc-2.2.1/doc/source/index.rst
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.421414 fusesoc-2.2.1/doc/source/ref/
+-rw-r--r--   0 olof      (1000) olof      (1000)    15496 2023-02-28 12:23:16.000000 fusesoc-2.2.1/doc/source/ref/capi1.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)     1723 2023-02-28 12:28:15.000000 fusesoc-2.2.1/doc/source/ref/glossary.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)      175 2023-02-28 12:28:15.000000 fusesoc-2.2.1/doc/source/ref/index.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)    10054 2023-02-28 12:23:16.000000 fusesoc-2.2.1/doc/source/ref/migrations.rst
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.423414 fusesoc-2.2.1/doc/source/user/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.425413 fusesoc-2.2.1/doc/source/user/build_system/
+-rw-r--r--   0 olof      (1000) olof      (1000)    12263 2023-02-28 12:28:15.000000 fusesoc-2.2.1/doc/source/user/build_system/core_files.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)     7514 2023-02-28 12:23:16.000000 fusesoc-2.2.1/doc/source/user/build_system/dependencies.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)     1603 2023-02-28 12:32:13.000000 fusesoc-2.2.1/doc/source/user/build_system/eda_flows.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)     7507 2023-02-28 12:28:34.000000 fusesoc-2.2.1/doc/source/user/build_system/flags.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)     2978 2023-02-28 12:32:13.000000 fusesoc-2.2.1/doc/source/user/build_system/flow_options.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)    12067 2023-02-28 12:32:13.000000 fusesoc-2.2.1/doc/source/user/build_system/generators.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)      129 2022-09-29 19:36:09.000000 fusesoc-2.2.1/doc/source/user/build_system/hooks.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)     1902 2023-02-28 12:32:13.000000 fusesoc-2.2.1/doc/source/user/build_system/index.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)     2267 2023-02-28 12:32:13.000000 fusesoc-2.2.1/doc/source/user/build_system/tool_options.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)       87 2022-09-29 19:36:09.000000 fusesoc-2.2.1/doc/source/user/build_system/vpi.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)     1502 2023-02-28 12:28:34.000000 fusesoc-2.2.1/doc/source/user/cli.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)     1149 2022-09-29 19:36:09.000000 fusesoc-2.2.1/doc/source/user/index.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)     4013 2023-04-17 12:12:08.000000 fusesoc-2.2.1/doc/source/user/installation.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)     2015 2022-09-29 19:36:09.000000 fusesoc-2.2.1/doc/source/user/introduction.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)     1381 2022-09-29 19:36:09.000000 fusesoc-2.2.1/doc/source/user/knowledgebase.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)     6678 2023-02-28 12:28:34.000000 fusesoc-2.2.1/doc/source/user/overview.rst
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.426414 fusesoc-2.2.1/doc/source/user/package_manager/
+-rw-r--r--   0 olof      (1000) olof      (1000)     2888 2023-02-28 12:32:13.000000 fusesoc-2.2.1/doc/source/user/package_manager/index.rst
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.426414 fusesoc-2.2.1/extras/
+-rw-r--r--   0 olof      (1000) olof      (1000)      766 2022-09-29 19:36:09.000000 fusesoc-2.2.1/extras/bash-completion
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.427414 fusesoc-2.2.1/fusesoc/
+-rw-r--r--   0 olof      (1000) olof      (1000)      250 2022-09-29 19:36:09.000000 fusesoc-2.2.1/fusesoc/__init__.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.429414 fusesoc-2.2.1/fusesoc/capi2/
+-rw-r--r--   0 olof      (1000) olof      (1000)      141 2022-09-29 19:36:09.000000 fusesoc-2.2.1/fusesoc/capi2/__init__.py
+-rw-r--r--   0 olof      (1000) olof      (1000)    21425 2023-04-18 10:07:10.000000 fusesoc-2.2.1/fusesoc/capi2/core.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     5908 2023-04-24 13:23:55.000000 fusesoc-2.2.1/fusesoc/capi2/coredata.py
+-rw-r--r--   0 olof      (1000) olof      (1000)      720 2023-04-17 12:12:08.000000 fusesoc-2.2.1/fusesoc/capi2/coreparser.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     5825 2023-04-23 19:51:22.000000 fusesoc-2.2.1/fusesoc/capi2/exprs.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     2046 2023-04-17 12:12:08.000000 fusesoc-2.2.1/fusesoc/capi2/generator.py
+-rw-r--r--   0 olof      (1000) olof      (1000)    22016 2023-04-24 13:10:01.000000 fusesoc-2.2.1/fusesoc/capi2/json_schema.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     6424 2023-02-28 12:32:13.000000 fusesoc-2.2.1/fusesoc/config.py
+-rw-r--r--   0 olof      (1000) olof      (1000)      340 2023-02-28 12:28:15.000000 fusesoc-2.2.1/fusesoc/core.py
+-rw-r--r--   0 olof      (1000) olof      (1000)    14081 2023-04-17 12:12:08.000000 fusesoc-2.2.1/fusesoc/coremanager.py
+-rw-r--r--   0 olof      (1000) olof      (1000)    25699 2023-04-17 12:20:14.000000 fusesoc-2.2.1/fusesoc/edalizer.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     2870 2023-02-28 12:32:13.000000 fusesoc-2.2.1/fusesoc/librarymanager.py
+-rw-r--r--   0 olof      (1000) olof      (1000)    22647 2023-04-17 12:12:08.000000 fusesoc-2.2.1/fusesoc/main.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.430414 fusesoc-2.2.1/fusesoc/parser/
+-rw-r--r--   0 olof      (1000) olof      (1000)      141 2023-04-17 12:12:08.000000 fusesoc-2.2.1/fusesoc/parser/__init__.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     2335 2023-04-17 12:12:08.000000 fusesoc-2.2.1/fusesoc/parser/coreparser.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.430414 fusesoc-2.2.1/fusesoc/provider/
+-rw-r--r--   0 olof      (1000) olof      (1000)      279 2023-02-28 12:28:15.000000 fusesoc-2.2.1/fusesoc/provider/__init__.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     2253 2023-02-28 12:53:14.000000 fusesoc-2.2.1/fusesoc/provider/git.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     1364 2023-02-28 12:28:15.000000 fusesoc-2.2.1/fusesoc/provider/github.py
+-rw-r--r--   0 olof      (1000) olof      (1000)      602 2023-02-28 12:28:15.000000 fusesoc-2.2.1/fusesoc/provider/local.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     1188 2022-09-29 19:36:09.000000 fusesoc-2.2.1/fusesoc/provider/opencores.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     2673 2023-02-28 12:28:34.000000 fusesoc-2.2.1/fusesoc/provider/provider.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     1852 2023-02-28 12:28:15.000000 fusesoc-2.2.1/fusesoc/provider/url.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     5521 2023-04-17 12:12:08.000000 fusesoc-2.2.1/fusesoc/utils.py
+-rw-r--r--   0 olof      (1000) olof      (1000)      176 2023-04-24 13:26:51.000000 fusesoc-2.2.1/fusesoc/version.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     5135 2023-02-28 12:28:15.000000 fusesoc-2.2.1/fusesoc/vlnv.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.428413 fusesoc-2.2.1/fusesoc.egg-info/
+-rw-r--r--   0 olof      (1000) olof      (1000)     6133 2023-04-24 13:26:51.000000 fusesoc-2.2.1/fusesoc.egg-info/PKG-INFO
+-rw-r--r--   0 olof      (1000) olof      (1000)     6624 2023-04-24 13:26:51.000000 fusesoc-2.2.1/fusesoc.egg-info/SOURCES.txt
+-rw-r--r--   0 olof      (1000) olof      (1000)        1 2023-04-24 13:26:51.000000 fusesoc-2.2.1/fusesoc.egg-info/dependency_links.txt
+-rw-r--r--   0 olof      (1000) olof      (1000)       46 2023-04-24 13:26:51.000000 fusesoc-2.2.1/fusesoc.egg-info/entry_points.txt
+-rw-r--r--   0 olof      (1000) olof      (1000)       64 2023-04-24 13:26:51.000000 fusesoc-2.2.1/fusesoc.egg-info/requires.txt
+-rw-r--r--   0 olof      (1000) olof      (1000)        8 2023-04-24 13:26:51.000000 fusesoc-2.2.1/fusesoc.egg-info/top_level.txt
+-rw-r--r--   0 olof      (1000) olof      (1000)       38 2023-04-24 13:26:51.449414 fusesoc-2.2.1/setup.cfg
+-rw-r--r--   0 olof      (1000) olof      (1000)     1689 2023-04-17 12:12:08.000000 fusesoc-2.2.1/setup.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.432414 fusesoc-2.2.1/tests/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.413413 fusesoc-2.2.1/tests/capi2_cores/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.433414 fusesoc-2.2.1/tests/capi2_cores/deptree/
+-rw-r--r--   0 olof      (1000) olof      (1000)      375 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/capi2_cores/deptree/child1.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      338 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/capi2_cores/deptree/child2.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      338 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/capi2_cores/deptree/child3.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      304 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/capi2_cores/deptree/child4.core
+-rw-r--r--   0 olof      (1000) olof      (1000)     1288 2023-02-28 12:23:16.000000 fusesoc-2.2.1/tests/capi2_cores/deptree/generated_child_a.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      444 2023-02-28 12:23:16.000000 fusesoc-2.2.1/tests/capi2_cores/deptree/generated_child_a.py
+-rw-r--r--   0 olof      (1000) olof      (1000)      802 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/capi2_cores/deptree/root.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.433414 fusesoc-2.2.1/tests/capi2_cores/files_out_of_hierarchy/
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2023-02-28 12:23:16.000000 fusesoc-2.2.1/tests/capi2_cores/files_out_of_hierarchy/bad.sv
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.433414 fusesoc-2.2.1/tests/capi2_cores/files_out_of_hierarchy/subdir/
+-rw-r--r--   0 olof      (1000) olof      (1000)      533 2023-02-28 12:23:16.000000 fusesoc-2.2.1/tests/capi2_cores/files_out_of_hierarchy/subdir/files_out_of_hierarchy.core
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2023-02-28 12:23:16.000000 fusesoc-2.2.1/tests/capi2_cores/files_out_of_hierarchy/subdir/good.sv
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.436414 fusesoc-2.2.1/tests/capi2_cores/misc/
+-rw-r--r--   0 olof      (1000) olof      (1000)      493 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/capi2_cores/misc/append.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      646 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/capi2_cores/misc/depends.core
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/capi2_cores/misc/dontpickthisfile
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/capi2_cores/misc/dummy.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/capi2_cores/misc/empty.core
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/capi2_cores/misc/f1
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/capi2_cores/misc/f2
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/capi2_cores/misc/f3
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/capi2_cores/misc/f4
+-rw-r--r--   0 olof      (1000) olof      (1000)     1496 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/capi2_cores/misc/files.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      447 2023-02-28 12:28:15.000000 fusesoc-2.2.1/tests/capi2_cores/misc/flags.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      502 2023-02-28 12:28:43.000000 fusesoc-2.2.1/tests/capi2_cores/misc/flow.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.437414 fusesoc-2.2.1/tests/capi2_cores/misc/generate/
+-rw-r--r--   0 olof      (1000) olof      (1000)       10 2023-02-28 12:32:13.000000 fusesoc-2.2.1/tests/capi2_cores/misc/generate/file_cachetest
+-rw-r--r--   0 olof      (1000) olof      (1000)      914 2023-02-28 12:32:13.000000 fusesoc-2.2.1/tests/capi2_cores/misc/generate/generate.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      375 2023-02-28 12:32:13.000000 fusesoc-2.2.1/tests/capi2_cores/misc/generate/generators.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      553 2023-02-28 12:23:16.000000 fusesoc-2.2.1/tests/capi2_cores/misc/generate/testgen.py
+-rw-r--r--   0 olof      (1000) olof      (1000)      886 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/capi2_cores/misc/hooks.core
+-rw-r--r--   0 olof      (1000) olof      (1000)     1471 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/capi2_cores/misc/parameters.core
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/capi2_cores/misc/scriptfile
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.437414 fusesoc-2.2.1/tests/capi2_cores/misc/subdir/
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/capi2_cores/misc/subdir/dummy.extra
+-rw-r--r--   0 olof      (1000) olof      (1000)      356 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/capi2_cores/misc/targets.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      301 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/capi2_cores/misc/toplevel.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      609 2023-02-28 12:28:34.000000 fusesoc-2.2.1/tests/capi2_cores/misc/typecheck.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      244 2023-04-17 12:12:08.000000 fusesoc-2.2.1/tests/capi2_cores/misc/uncachable.core
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/capi2_cores/misc/vhdlfile
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/capi2_cores/misc/vlogfile
+-rw-r--r--   0 olof      (1000) olof      (1000)      562 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/capi2_cores/misc/vpi.core
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/capi2_cores/misc/vpifile
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.437414 fusesoc-2.2.1/tests/capi2_cores/parser/
+-rw-r--r--   0 olof      (1000) olof      (1000)      334 2023-04-17 12:12:08.000000 fusesoc-2.2.1/tests/capi2_cores/parser/no_additional_properties.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      482 2023-04-17 12:12:08.000000 fusesoc-2.2.1/tests/capi2_cores/parser/with_additional_properties.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.438414 fusesoc-2.2.1/tests/capi2_cores/providers/
+-rw-r--r--   0 olof      (1000) olof      (1000)      309 2023-02-28 12:28:43.000000 fusesoc-2.2.1/tests/capi2_cores/providers/url_simple.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      348 2023-02-28 12:28:43.000000 fusesoc-2.2.1/tests/capi2_cores/providers/url_simple_with_user_agent.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      308 2023-02-28 12:28:43.000000 fusesoc-2.2.1/tests/capi2_cores/providers/url_tar.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      305 2023-02-28 12:28:43.000000 fusesoc-2.2.1/tests/capi2_cores/providers/url_zip.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.438414 fusesoc-2.2.1/tests/capi2_cores/virtual/
+-rw-r--r--   0 olof      (1000) olof      (1000)      325 2023-02-28 12:28:15.000000 fusesoc-2.2.1/tests/capi2_cores/virtual/impl1.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      325 2023-02-28 12:28:15.000000 fusesoc-2.2.1/tests/capi2_cores/virtual/impl2.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      349 2023-02-28 12:28:15.000000 fusesoc-2.2.1/tests/capi2_cores/virtual/user.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.416413 fusesoc-2.2.1/tests/cores/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.438414 fusesoc-2.2.1/tests/cores/adv_debug_sys/
+-rw-r--r--   0 olof      (1000) olof      (1000)     1225 2023-02-28 12:28:15.000000 fusesoc-2.2.1/tests/cores/adv_debug_sys/adv_debug_sys.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.438414 fusesoc-2.2.1/tests/cores/atlys/
+-rw-r--r--   0 olof      (1000) olof      (1000)     2269 2023-02-28 12:28:15.000000 fusesoc-2.2.1/tests/cores/atlys/atlys.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.439414 fusesoc-2.2.1/tests/cores/atlys/data/
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/cores/atlys/data/atlys.ucf
+-rw-r--r--   0 olof      (1000) olof      (1000)      176 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/cores/atlys/data/dummy_backend_tcl_file.tcl
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.439414 fusesoc-2.2.1/tests/cores/elf-loader/
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      184 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/cores/elf-loader/check_libelf.sh
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/cores/elf-loader/elf-loader.c
+-rw-r--r--   0 olof      (1000) olof      (1000)     1458 2023-02-28 12:28:15.000000 fusesoc-2.2.1/tests/cores/elf-loader/elf-loader.core
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/cores/elf-loader/vpi_wrapper.c
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.439414 fusesoc-2.2.1/tests/cores/gpio/
+-rw-r--r--   0 olof      (1000) olof      (1000)      379 2023-02-28 12:28:15.000000 fusesoc-2.2.1/tests/cores/gpio/gpio.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.440414 fusesoc-2.2.1/tests/cores/jtag_tap/
+-rw-r--r--   0 olof      (1000) olof      (1000)      474 2023-02-28 12:28:15.000000 fusesoc-2.2.1/tests/cores/jtag_tap/jtag_tap-1.13.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.440414 fusesoc-2.2.1/tests/cores/libstorage/
+-rw-r--r--   0 olof      (1000) olof      (1000)      529 2023-02-28 12:28:15.000000 fusesoc-2.2.1/tests/cores/libstorage/libstorage-1.0.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.442414 fusesoc-2.2.1/tests/cores/misc/
+-rw-r--r--   0 olof      (1000) olof      (1000)     1051 2023-02-28 12:28:15.000000 fusesoc-2.2.1/tests/cores/misc/c3demo.core
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/cores/misc/c3demo.pcf
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.442414 fusesoc-2.2.1/tests/cores/misc/copytocore/
+-rw-r--r--   0 olof      (1000) olof      (1000)      421 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/cores/misc/copytocore/copytocore.core
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/cores/misc/copytocore/dummy.tcl
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.442414 fusesoc-2.2.1/tests/cores/misc/copytocore/subdir/
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/cores/misc/copytocore/subdir/dummy.extra
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/cores/misc/dummy.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/cores/misc/dummy.xci
+-rw-r--r--   0 olof      (1000) olof      (1000)      854 2023-02-28 12:28:15.000000 fusesoc-2.2.1/tests/cores/misc/filetypes.core
+-rw-r--r--   0 olof      (1000) olof      (1000)     1391 2023-02-28 12:28:15.000000 fusesoc-2.2.1/tests/cores/misc/ghdltest.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      356 2023-02-28 12:28:15.000000 fusesoc-2.2.1/tests/cores/misc/gitcore.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      698 2023-02-28 12:28:15.000000 fusesoc-2.2.1/tests/cores/misc/no_exe_script.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      234 2023-02-28 12:28:15.000000 fusesoc-2.2.1/tests/cores/misc/nomain.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      399 2023-02-28 12:28:15.000000 fusesoc-2.2.1/tests/cores/misc/opencorescore.core
+-rw-r--r--   0 olof      (1000) olof      (1000)     2482 2023-02-28 12:28:15.000000 fusesoc-2.2.1/tests/cores/misc/paramtest.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.443414 fusesoc-2.2.1/tests/cores/misc/scripts/
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/cores/misc/scripts/no_exe_script
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      192 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/cores/misc/scripts/post_build_script
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      173 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/cores/misc/scripts/post_run_script
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      191 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/cores/misc/scripts/pre_build_script
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      172 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/cores/misc/scripts/pre_run_script
+-rw-r--r--   0 olof      (1000) olof      (1000)     1474 2023-02-28 12:28:15.000000 fusesoc-2.2.1/tests/cores/misc/scriptscore.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.443414 fusesoc-2.2.1/tests/cores/misc/subdir/
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/cores/misc/subdir/dummy.extra
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.443414 fusesoc-2.2.1/tests/cores/mor1kx/
+-rw-r--r--   0 olof      (1000) olof      (1000)     2807 2023-02-28 12:28:15.000000 fusesoc-2.2.1/tests/cores/mor1kx/mor1kx-3.1.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.444414 fusesoc-2.2.1/tests/cores/mor1kx-arty/
+-rw-r--r--   0 olof      (1000) olof      (1000)      702 2023-02-28 12:28:15.000000 fusesoc-2.2.1/tests/cores/mor1kx-arty/mor1kx-arty.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      337 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/cores/mor1kx-arty/mor1kx-arty.system
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.444414 fusesoc-2.2.1/tests/cores/mor1kx-generic/
+-rw-r--r--   0 olof      (1000) olof      (1000)     3024 2023-02-28 12:28:15.000000 fusesoc-2.2.1/tests/cores/mor1kx-generic/mor1kx-generic.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.444414 fusesoc-2.2.1/tests/cores/mor1kx-generic/scripts/
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      173 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/cores/mor1kx-generic/scripts/post_run_script
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      174 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/cores/mor1kx-generic/scripts/pre_build_script
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      172 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/cores/mor1kx-generic/scripts/pre_run_script
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.444414 fusesoc-2.2.1/tests/cores/sockit/
+-rw-r--r--   0 olof      (1000) olof      (1000)     1596 2023-02-28 12:28:15.000000 fusesoc-2.2.1/tests/cores/sockit/sockit.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.445414 fusesoc-2.2.1/tests/cores/uart16550/
+-rw-r--r--   0 olof      (1000) olof      (1000)      920 2023-02-28 12:28:15.000000 fusesoc-2.2.1/tests/cores/uart16550/uart16550-1.5.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.445414 fusesoc-2.2.1/tests/cores/verilator_tb_utils/
+-rw-r--r--   0 olof      (1000) olof      (1000)      715 2023-02-28 12:28:15.000000 fusesoc-2.2.1/tests/cores/verilator_tb_utils/verilator_tb_utils.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.445414 fusesoc-2.2.1/tests/cores/verilog-arbiter/
+-rw-r--r--   0 olof      (1000) olof      (1000)      761 2023-02-28 12:28:15.000000 fusesoc-2.2.1/tests/cores/verilog-arbiter/verilog-arbiter-r1.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.445414 fusesoc-2.2.1/tests/cores/verilog_utils/
+-rw-r--r--   0 olof      (1000) olof      (1000)      573 2023-02-28 12:28:15.000000 fusesoc-2.2.1/tests/cores/verilog_utils/verilog_utils.core
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/cores/verilog_utils/verilog_utils.vh
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.445414 fusesoc-2.2.1/tests/cores/vga_lcd/
+-rw-r--r--   0 olof      (1000) olof      (1000)     1200 2023-02-28 12:28:15.000000 fusesoc-2.2.1/tests/cores/vga_lcd/vga_lcd.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.445414 fusesoc-2.2.1/tests/cores/vlog_tb_utils/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.446414 fusesoc-2.2.1/tests/cores/vlog_tb_utils/files/
+-rw-r--r--   0 olof      (1000) olof      (1000)      554 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/cores/vlog_tb_utils/files/0001-testpatch.patch
+-rw-r--r--   0 olof      (1000) olof      (1000)     1456 2023-02-28 12:28:15.000000 fusesoc-2.2.1/tests/cores/vlog_tb_utils/vlog_tb_utils-1.1.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.446414 fusesoc-2.2.1/tests/cores/wb_common/
+-rw-r--r--   0 olof      (1000) olof      (1000)      655 2023-02-28 12:28:15.000000 fusesoc-2.2.1/tests/cores/wb_common/wb_common.core
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/cores/wb_common/wb_common.v
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/cores/wb_common/wb_common_params.v
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.446414 fusesoc-2.2.1/tests/cores/wb_intercon/
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/cores/wb_intercon/dummy_icarus.v
+-rw-r--r--   0 olof      (1000) olof      (1000)     1329 2023-02-28 12:28:15.000000 fusesoc-2.2.1/tests/cores/wb_intercon/wb_intercon-1.0.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.446414 fusesoc-2.2.1/tests/test_capi2/
+-rw-r--r--   0 olof      (1000) olof      (1000)       90 2023-02-28 12:28:15.000000 fusesoc-2.2.1/tests/test_capi2/generators.info
+-rw-r--r--   0 olof      (1000) olof      (1000)      207 2023-02-28 12:28:15.000000 fusesoc-2.2.1/tests/test_capi2/targets.info
+-rw-r--r--   0 olof      (1000) olof      (1000)    21205 2023-04-17 12:27:19.000000 fusesoc-2.2.1/tests/test_capi2.py
+-rw-r--r--   0 olof      (1000) olof      (1000)      335 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/test_common.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     2230 2023-02-28 12:28:34.000000 fusesoc-2.2.1/tests/test_config.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     7657 2023-03-23 19:51:07.000000 fusesoc-2.2.1/tests/test_coremanager.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     3988 2023-03-23 19:51:07.000000 fusesoc-2.2.1/tests/test_edalizer.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     1619 2023-03-23 19:51:07.000000 fusesoc-2.2.1/tests/test_exprs.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     1484 2023-02-28 12:28:34.000000 fusesoc-2.2.1/tests/test_ignored_dirs.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     5516 2023-02-28 12:32:13.000000 fusesoc-2.2.1/tests/test_libraries.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.447414 fusesoc-2.2.1/tests/test_provider/
+-rw-r--r--   0 olof      (1000) olof      (1000)      114 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/test_provider/file.tar.gz
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/test_provider/file.v
+-rw-r--r--   0 olof      (1000) olof      (1000)      162 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/test_provider/file.zip
+-rw-r--r--   0 olof      (1000) olof      (1000)     1141 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/test_provider/vlog_functions.v
+-rw-r--r--   0 olof      (1000) olof      (1000)     3000 2023-04-17 12:12:08.000000 fusesoc-2.2.1/tests/test_provider.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     2177 2023-02-28 12:23:16.000000 fusesoc-2.2.1/tests/test_vlnv.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.416413 fusesoc-2.2.1/tests/userguide/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.447414 fusesoc-2.2.1/tests/userguide/blinky/
+-rw-r--r--   0 olof      (1000) olof      (1000)     1743 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/userguide/blinky/blinky.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.447414 fusesoc-2.2.1/tests/userguide/blinky/data/
+-rw-r--r--   0 olof      (1000) olof      (1000)      458 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/userguide/blinky/data/nexys_video.xdc
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.448414 fusesoc-2.2.1/tests/userguide/blinky/rtl/
+-rw-r--r--   0 olof      (1000) olof      (1000)      636 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/userguide/blinky/rtl/blinky.sv
+-rw-r--r--   0 olof      (1000) olof      (1000)      153 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/userguide/blinky/rtl/macros.svh
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.448414 fusesoc-2.2.1/tests/userguide/blinky/tb/
+-rw-r--r--   0 olof      (1000) olof      (1000)     1031 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/userguide/blinky/tb/blinky_tb.sv
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.448414 fusesoc-2.2.1/tests/userguide/dualblinky/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.448414 fusesoc-2.2.1/tests/userguide/dualblinky/data/
+-rw-r--r--   0 olof      (1000) olof      (1000)      574 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/userguide/dualblinky/data/nexys_video.xdc
+-rw-r--r--   0 olof      (1000) olof      (1000)      792 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/userguide/dualblinky/dualblinky.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-24 13:26:51.448414 fusesoc-2.2.1/tests/userguide/dualblinky/rtl/
+-rw-r--r--   0 olof      (1000) olof      (1000)      665 2022-09-29 19:36:09.000000 fusesoc-2.2.1/tests/userguide/dualblinky/rtl/dualblinky.sv
+-rw-r--r--   0 olof      (1000) olof      (1000)     3014 2023-02-28 12:32:13.000000 fusesoc-2.2.1/tox.ini
```

### Comparing `fusesoc-2.2/.github/workflows/ci.yml` & `fusesoc-2.2.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/.pre-commit-config.yaml` & `fusesoc-2.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/LICENSE` & `fusesoc-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/NEWS` & `fusesoc-2.2.1/NEWS`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 2.2 2023-04-18 Olof Kindgren <olof.kindgren@gmail.com>
 ======================================================
-* Use jsonschema to describe anv validate CAPI2 files
+* Use jsonschema to describe and validate CAPI2 files
 * Add switch to allow additional CAPI2 properties
 * Support use expansion everywhere
 * Support setting tags on files
+* + improved error handling, bug fixes and refactoring
 
 Contributors:
 Erik Waling <erik.waling@gmail.com>
 Olof Kindgren <olof.kindgren@gmail.com>
 Patcharapol Sankaew <meen.sankaew@gmail.com>
 
 2.1 2023-03-23 Olof Kindgren <olof.kindgren@gmail.com>
```

### Comparing `fusesoc-2.2/PKG-INFO` & `fusesoc-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusesoc
-Version: 2.2
+Version: 2.2.1
 Summary: FuseSoC is a package manager and a set of build tools for HDL (Hardware Description Language) code.
 Home-page: https://github.com/olofk/fusesoc
 Author: Olof Kindgren
 Author-email: olof.kindgren@gmail.com
 License: BSD-2-Clause
 Keywords: VHDL,verilog,hdl,rtl,synthesis,FPGA,simulation,Xilinx,Altera
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fusesoc-2.2/README.md` & `fusesoc-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/doc/source/conf.py` & `fusesoc-2.2.1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/doc/source/dev/devsetup.rst` & `fusesoc-2.2.1/doc/source/dev/devsetup.rst`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/doc/source/index.rst` & `fusesoc-2.2.1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/doc/source/ref/capi1.rst` & `fusesoc-2.2.1/doc/source/ref/capi1.rst`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/doc/source/ref/glossary.rst` & `fusesoc-2.2.1/doc/source/ref/glossary.rst`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/doc/source/ref/migrations.rst` & `fusesoc-2.2.1/doc/source/ref/migrations.rst`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/doc/source/user/build_system/core_files.rst` & `fusesoc-2.2.1/doc/source/user/build_system/core_files.rst`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/doc/source/user/build_system/dependencies.rst` & `fusesoc-2.2.1/doc/source/user/build_system/dependencies.rst`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/doc/source/user/build_system/eda_flows.rst` & `fusesoc-2.2.1/doc/source/user/build_system/eda_flows.rst`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/doc/source/user/build_system/flags.rst` & `fusesoc-2.2.1/doc/source/user/build_system/flags.rst`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/doc/source/user/build_system/flow_options.rst` & `fusesoc-2.2.1/doc/source/user/build_system/flow_options.rst`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/doc/source/user/build_system/generators.rst` & `fusesoc-2.2.1/doc/source/user/build_system/generators.rst`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/doc/source/user/build_system/index.rst` & `fusesoc-2.2.1/doc/source/user/build_system/index.rst`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/doc/source/user/build_system/tool_options.rst` & `fusesoc-2.2.1/doc/source/user/build_system/tool_options.rst`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/doc/source/user/cli.rst` & `fusesoc-2.2.1/doc/source/user/cli.rst`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/doc/source/user/index.rst` & `fusesoc-2.2.1/doc/source/user/index.rst`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/doc/source/user/installation.rst` & `fusesoc-2.2.1/doc/source/user/installation.rst`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/doc/source/user/introduction.rst` & `fusesoc-2.2.1/doc/source/user/introduction.rst`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/doc/source/user/knowledgebase.rst` & `fusesoc-2.2.1/doc/source/user/knowledgebase.rst`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/doc/source/user/overview.rst` & `fusesoc-2.2.1/doc/source/user/overview.rst`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/doc/source/user/package_manager/index.rst` & `fusesoc-2.2.1/doc/source/user/package_manager/index.rst`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/extras/bash-completion` & `fusesoc-2.2.1/extras/bash-completion`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/fusesoc/capi2/core.py` & `fusesoc-2.2.1/fusesoc/capi2/core.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/fusesoc/capi2/coredata.py` & `fusesoc-2.2.1/fusesoc/capi2/coredata.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             remove = []
             append = {}
             for k, v in data.items():
                 # Only run expand() if a string contains a "?" to avoid
                 # issues with strings containing for instance parentheses
                 if type(v) == str and len(v) > 0 and "?" in v:
                     data[k] = Exprs(v).expand(flags)
-                if type(k) == str:
+                if type(k) == str and "?" in k:
                     expanded_k = Exprs(k).expand(flags)
                     if len(expanded_k) == 0:
                         remove.append(k)
                     elif expanded_k != k:
                         append[expanded_k] = v
                         remove.append(k)
```

### Comparing `fusesoc-2.2/fusesoc/capi2/coreparser.py` & `fusesoc-2.2.1/fusesoc/capi2/coreparser.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/fusesoc/capi2/exprs.py` & `fusesoc-2.2.1/fusesoc/capi2/exprs.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/fusesoc/capi2/generator.py` & `fusesoc-2.2.1/fusesoc/capi2/generator.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/fusesoc/capi2/json_schema.py` & `fusesoc-2.2.1/fusesoc/capi2/json_schema.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/fusesoc/config.py` & `fusesoc-2.2.1/fusesoc/config.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/fusesoc/coremanager.py` & `fusesoc-2.2.1/fusesoc/coremanager.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/fusesoc/edalizer.py` & `fusesoc-2.2.1/fusesoc/edalizer.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/fusesoc/librarymanager.py` & `fusesoc-2.2.1/fusesoc/librarymanager.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/fusesoc/main.py` & `fusesoc-2.2.1/fusesoc/main.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/fusesoc/parser/coreparser.py` & `fusesoc-2.2.1/fusesoc/parser/coreparser.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/fusesoc/provider/git.py` & `fusesoc-2.2.1/fusesoc/provider/git.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/fusesoc/provider/github.py` & `fusesoc-2.2.1/fusesoc/provider/github.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/fusesoc/provider/local.py` & `fusesoc-2.2.1/fusesoc/provider/local.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/fusesoc/provider/opencores.py` & `fusesoc-2.2.1/fusesoc/provider/opencores.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/fusesoc/provider/provider.py` & `fusesoc-2.2.1/fusesoc/provider/provider.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/fusesoc/provider/url.py` & `fusesoc-2.2.1/fusesoc/provider/url.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/fusesoc/utils.py` & `fusesoc-2.2.1/fusesoc/utils.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/fusesoc/vlnv.py` & `fusesoc-2.2.1/fusesoc/vlnv.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/fusesoc.egg-info/PKG-INFO` & `fusesoc-2.2.1/fusesoc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusesoc
-Version: 2.2
+Version: 2.2.1
 Summary: FuseSoC is a package manager and a set of build tools for HDL (Hardware Description Language) code.
 Home-page: https://github.com/olofk/fusesoc
 Author: Olof Kindgren
 Author-email: olof.kindgren@gmail.com
 License: BSD-2-Clause
 Keywords: VHDL,verilog,hdl,rtl,synthesis,FPGA,simulation,Xilinx,Altera
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fusesoc-2.2/fusesoc.egg-info/SOURCES.txt` & `fusesoc-2.2.1/fusesoc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/setup.py` & `fusesoc-2.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/capi2_cores/deptree/generated_child_a.core` & `fusesoc-2.2.1/tests/capi2_cores/deptree/generated_child_a.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/capi2_cores/deptree/root.core` & `fusesoc-2.2.1/tests/capi2_cores/deptree/root.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/capi2_cores/files_out_of_hierarchy/subdir/files_out_of_hierarchy.core` & `fusesoc-2.2.1/tests/capi2_cores/files_out_of_hierarchy/subdir/files_out_of_hierarchy.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/capi2_cores/misc/depends.core` & `fusesoc-2.2.1/tests/capi2_cores/misc/depends.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/capi2_cores/misc/files.core` & `fusesoc-2.2.1/tests/capi2_cores/misc/files.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/capi2_cores/misc/generate/generate.core` & `fusesoc-2.2.1/tests/capi2_cores/misc/generate/generate.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/capi2_cores/misc/generate/testgen.py` & `fusesoc-2.2.1/tests/capi2_cores/misc/generate/testgen.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/capi2_cores/misc/hooks.core` & `fusesoc-2.2.1/tests/capi2_cores/misc/hooks.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/capi2_cores/misc/parameters.core` & `fusesoc-2.2.1/tests/capi2_cores/misc/parameters.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/capi2_cores/misc/typecheck.core` & `fusesoc-2.2.1/tests/capi2_cores/misc/typecheck.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/capi2_cores/misc/vpi.core` & `fusesoc-2.2.1/tests/capi2_cores/misc/vpi.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/cores/adv_debug_sys/adv_debug_sys.core` & `fusesoc-2.2.1/tests/cores/adv_debug_sys/adv_debug_sys.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/cores/atlys/atlys.core` & `fusesoc-2.2.1/tests/cores/atlys/atlys.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/cores/elf-loader/elf-loader.core` & `fusesoc-2.2.1/tests/cores/elf-loader/elf-loader.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/cores/libstorage/libstorage-1.0.core` & `fusesoc-2.2.1/tests/cores/libstorage/libstorage-1.0.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/cores/misc/c3demo.core` & `fusesoc-2.2.1/tests/cores/misc/c3demo.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/cores/misc/filetypes.core` & `fusesoc-2.2.1/tests/cores/misc/filetypes.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/cores/misc/ghdltest.core` & `fusesoc-2.2.1/tests/cores/misc/ghdltest.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/cores/misc/no_exe_script.core` & `fusesoc-2.2.1/tests/cores/misc/no_exe_script.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/cores/misc/paramtest.core` & `fusesoc-2.2.1/tests/cores/misc/paramtest.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/cores/misc/scriptscore.core` & `fusesoc-2.2.1/tests/cores/misc/scriptscore.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/cores/mor1kx/mor1kx-3.1.core` & `fusesoc-2.2.1/tests/cores/mor1kx/mor1kx-3.1.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/cores/mor1kx-arty/mor1kx-arty.core` & `fusesoc-2.2.1/tests/cores/mor1kx-arty/mor1kx-arty.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/cores/mor1kx-generic/mor1kx-generic.core` & `fusesoc-2.2.1/tests/cores/mor1kx-generic/mor1kx-generic.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/cores/sockit/sockit.core` & `fusesoc-2.2.1/tests/cores/sockit/sockit.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/cores/uart16550/uart16550-1.5.core` & `fusesoc-2.2.1/tests/cores/uart16550/uart16550-1.5.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/cores/verilator_tb_utils/verilator_tb_utils.core` & `fusesoc-2.2.1/tests/cores/verilator_tb_utils/verilator_tb_utils.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/cores/verilog-arbiter/verilog-arbiter-r1.core` & `fusesoc-2.2.1/tests/cores/verilog-arbiter/verilog-arbiter-r1.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/cores/verilog_utils/verilog_utils.core` & `fusesoc-2.2.1/tests/cores/verilog_utils/verilog_utils.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/cores/vga_lcd/vga_lcd.core` & `fusesoc-2.2.1/tests/cores/vga_lcd/vga_lcd.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/cores/vlog_tb_utils/files/0001-testpatch.patch` & `fusesoc-2.2.1/tests/cores/vlog_tb_utils/files/0001-testpatch.patch`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/cores/vlog_tb_utils/vlog_tb_utils-1.1.core` & `fusesoc-2.2.1/tests/cores/vlog_tb_utils/vlog_tb_utils-1.1.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/cores/wb_common/wb_common.core` & `fusesoc-2.2.1/tests/cores/wb_common/wb_common.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/cores/wb_intercon/wb_intercon-1.0.core` & `fusesoc-2.2.1/tests/cores/wb_intercon/wb_intercon-1.0.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/test_capi2.py` & `fusesoc-2.2.1/tests/test_capi2.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/test_config.py` & `fusesoc-2.2.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/test_coremanager.py` & `fusesoc-2.2.1/tests/test_coremanager.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/test_edalizer.py` & `fusesoc-2.2.1/tests/test_edalizer.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/test_exprs.py` & `fusesoc-2.2.1/tests/test_exprs.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/test_ignored_dirs.py` & `fusesoc-2.2.1/tests/test_ignored_dirs.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/test_libraries.py` & `fusesoc-2.2.1/tests/test_libraries.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/test_provider/vlog_functions.v` & `fusesoc-2.2.1/tests/test_provider/vlog_functions.v`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/test_provider.py` & `fusesoc-2.2.1/tests/test_provider.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/test_vlnv.py` & `fusesoc-2.2.1/tests/test_vlnv.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/userguide/blinky/blinky.core` & `fusesoc-2.2.1/tests/userguide/blinky/blinky.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/userguide/blinky/rtl/blinky.sv` & `fusesoc-2.2.1/tests/userguide/blinky/rtl/blinky.sv`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/userguide/blinky/tb/blinky_tb.sv` & `fusesoc-2.2.1/tests/userguide/blinky/tb/blinky_tb.sv`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/userguide/dualblinky/data/nexys_video.xdc` & `fusesoc-2.2.1/tests/userguide/dualblinky/data/nexys_video.xdc`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/userguide/dualblinky/dualblinky.core` & `fusesoc-2.2.1/tests/userguide/dualblinky/dualblinky.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tests/userguide/dualblinky/rtl/dualblinky.sv` & `fusesoc-2.2.1/tests/userguide/dualblinky/rtl/dualblinky.sv`

 * *Files identical despite different names*

### Comparing `fusesoc-2.2/tox.ini` & `fusesoc-2.2.1/tox.ini`

 * *Files identical despite different names*

