# Comparing `tmp/tox-4.4.9.tar.gz` & `tmp/tox-4.5.0.tar.gz`

## Comparing `tox-4.4.9.tar` & `tox-4.5.0.tar`

### file list

```diff
@@ -1,222 +1,222 @@
--rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 tox-4.4.9/tox.ini
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/__init__.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/__main__.py
--rw-r--r--   0        0        0     6004 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/provision.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/py.typed
--rw-r--r--   0        0        0    19145 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/pytest.py
--rw-r--r--   0        0        0     8278 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/report.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/run.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/config/__init__.py
--rw-r--r--   0        0        0     6443 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/config/main.py
--rw-r--r--   0        0        0     4187 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/config/of_type.py
--rw-r--r--   0        0        0     4806 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/config/set_env.py
--rw-r--r--   0        0        0     9841 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/config/sets.py
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/config/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/config/cli/__init__.py
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/config/cli/env_var.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/config/cli/ini.py
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/config/cli/parse.py
--rw-r--r--   0        0        0    13671 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/config/cli/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/config/loader/__init__.py
--rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/config/loader/api.py
--rw-r--r--   0        0        0     6411 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/config/loader/convert.py
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/config/loader/memory.py
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/config/loader/section.py
--rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/config/loader/str_convert.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/config/loader/stringify.py
--rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/config/loader/ini/__init__.py
--rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/config/loader/ini/factor.py
--rw-r--r--   0        0        0    13352 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/config/loader/ini/replace.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/config/source/__init__.py
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/config/source/api.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/config/source/discover.py
--rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/config/source/ini.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/config/source/ini_section.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/config/source/legacy_toml.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/config/source/setup_cfg.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/config/source/tox_ini.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/execute/__init__.py
--rw-r--r--   0        0        0     9137 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/execute/api.py
--rw-r--r--   0        0        0     5195 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/execute/pep517_backend.py
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/execute/request.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/execute/stream.py
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/execute/util.py
--rw-r--r--   0        0        0    13863 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/execute/local_sub_process/__init__.py
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/execute/local_sub_process/read_via_thread.py
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/execute/local_sub_process/read_via_thread_unix.py
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/execute/local_sub_process/read_via_thread_windows.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/journal/__init__.py
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/journal/env.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/journal/main.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/plugin/__init__.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/plugin/inline.py
--rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/plugin/manager.py
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/plugin/spec.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/session/__init__.py
--rw-r--r--   0        0        0    18051 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/session/env_select.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/session/state.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/session/cmd/__init__.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/session/cmd/depends.py
--rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/session/cmd/devenv.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/session/cmd/exec_.py
--rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/session/cmd/legacy.py
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/session/cmd/list_env.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/session/cmd/quickstart.py
--rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/session/cmd/show_config.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/session/cmd/version_flag.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/session/cmd/run/__init__.py
--rw-r--r--   0        0        0    16547 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/session/cmd/run/common.py
--rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/session/cmd/run/parallel.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/session/cmd/run/sequential.py
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/session/cmd/run/single.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/tox_env/__init__.py
--rw-r--r--   0        0        0    20134 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/tox_env/api.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/tox_env/errors.py
--rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/tox_env/info.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/tox_env/installer.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/tox_env/package.py
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/tox_env/register.py
--rw-r--r--   0        0        0     7761 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/tox_env/runner.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/tox_env/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/tox_env/python/__init__.py
--rw-r--r--   0        0        0    10900 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/tox_env/python/api.py
--rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/tox_env/python/package.py
--rw-r--r--   0        0        0     4446 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/tox_env/python/runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/tox_env/python/pip/__init__.py
--rw-r--r--   0        0        0    10355 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/tox_env/python/pip/pip_install.py
--rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/tox_env/python/pip/req_file.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/tox_env/python/pip/req/__init__.py
--rw-r--r--   0        0        0     4299 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/tox_env/python/pip/req/args.py
--rw-r--r--   0        0        0    19406 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/tox_env/python/pip/req/file.py
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/tox_env/python/pip/req/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/tox_env/python/virtual_env/__init__.py
--rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/tox_env/python/virtual_env/api.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/tox_env/python/virtual_env/runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/tox_env/python/virtual_env/package/__init__.py
--rw-r--r--   0        0        0     7053 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/tox_env/python/virtual_env/package/cmd_builder.py
--rw-r--r--   0        0        0    17577 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/tox_env/python/virtual_env/package/pyproject.py
--rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/tox_env/python/virtual_env/package/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/util/__init__.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/util/ci.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/util/cpu.py
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/util/file_view.py
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/util/graph.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/util/path.py
--rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 tox-4.4.9/src/tox/util/spinner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.4.9/tests/__init__.py
--rw-r--r--   0        0        0     5330 2020-02-02 00:00:00.000000 tox-4.4.9/tests/conftest.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 tox-4.4.9/tests/test_call_modes.py
--rw-r--r--   0        0        0     9796 2020-02-02 00:00:00.000000 tox-4.4.9/tests/test_provision.py
--rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 tox-4.4.9/tests/test_report.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 tox-4.4.9/tests/test_run.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 tox-4.4.9/tests/test_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.4.9/tests/config/__init__.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 tox-4.4.9/tests/config/conftest.py
--rw-r--r--   0        0        0     3888 2020-02-02 00:00:00.000000 tox-4.4.9/tests/config/test_main.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 tox-4.4.9/tests/config/test_of_types.py
--rw-r--r--   0        0        0     5827 2020-02-02 00:00:00.000000 tox-4.4.9/tests/config/test_set_env.py
--rw-r--r--   0        0        0     7157 2020-02-02 00:00:00.000000 tox-4.4.9/tests/config/test_sets.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 tox-4.4.9/tests/config/test_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.4.9/tests/config/cli/__init__.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 tox-4.4.9/tests/config/cli/conftest.py
--rw-r--r--   0        0        0     5105 2020-02-02 00:00:00.000000 tox-4.4.9/tests/config/cli/test_cli_env_var.py
--rw-r--r--   0        0        0     7197 2020-02-02 00:00:00.000000 tox-4.4.9/tests/config/cli/test_cli_ini.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 tox-4.4.9/tests/config/cli/test_parse.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 tox-4.4.9/tests/config/cli/test_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.4.9/tests/config/loader/__init__.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 tox-4.4.9/tests/config/loader/test_loader.py
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 tox-4.4.9/tests/config/loader/test_memory_loader.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 tox-4.4.9/tests/config/loader/test_section.py
--rw-r--r--   0        0        0     7098 2020-02-02 00:00:00.000000 tox-4.4.9/tests/config/loader/test_str_convert.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.4.9/tests/config/loader/ini/__init__.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 tox-4.4.9/tests/config/loader/ini/conftest.py
--rw-r--r--   0        0        0     6454 2020-02-02 00:00:00.000000 tox-4.4.9/tests/config/loader/ini/test_factor.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 tox-4.4.9/tests/config/loader/ini/test_ini_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.4.9/tests/config/loader/ini/replace/__init__.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tox-4.4.9/tests/config/loader/ini/replace/conftest.py
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 tox-4.4.9/tests/config/loader/ini/replace/test_replace.py
--rw-r--r--   0        0        0     7159 2020-02-02 00:00:00.000000 tox-4.4.9/tests/config/loader/ini/replace/test_replace_env_var.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 tox-4.4.9/tests/config/loader/ini/replace/test_replace_os_pathsep.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 tox-4.4.9/tests/config/loader/ini/replace/test_replace_os_sep.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 tox-4.4.9/tests/config/loader/ini/replace/test_replace_posargs.py
--rw-r--r--   0        0        0     8296 2020-02-02 00:00:00.000000 tox-4.4.9/tests/config/loader/ini/replace/test_replace_tox_env.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 tox-4.4.9/tests/config/loader/ini/replace/test_replace_tty.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.4.9/tests/config/source/__init__.py
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 tox-4.4.9/tests/config/source/test_discover.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 tox-4.4.9/tests/config/source/test_legacy_toml.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 tox-4.4.9/tests/config/source/test_setup_cfg.py
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 tox-4.4.9/tests/config/source/test_source_ini.py
--rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 tox-4.4.9/tests/demo_pkg_inline/build.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 tox-4.4.9/tests/demo_pkg_inline/build.pyi
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 tox-4.4.9/tests/demo_pkg_inline/pyproject.toml
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 tox-4.4.9/tests/demo_pkg_setuptools/pyproject.toml
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 tox-4.4.9/tests/demo_pkg_setuptools/setup.cfg
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 tox-4.4.9/tests/demo_pkg_setuptools/demo_pkg_setuptools/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.4.9/tests/execute/__init__.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 tox-4.4.9/tests/execute/conftest.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 tox-4.4.9/tests/execute/test_request.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 tox-4.4.9/tests/execute/test_stream.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.4.9/tests/execute/local_subprocess/__init__.py
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 tox-4.4.9/tests/execute/local_subprocess/bad_process.py
--rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 tox-4.4.9/tests/execute/local_subprocess/local_subprocess_sigint.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 tox-4.4.9/tests/execute/local_subprocess/test_execute_util.py
--rw-r--r--   0        0        0    14088 2020-02-02 00:00:00.000000 tox-4.4.9/tests/execute/local_subprocess/test_local_subprocess.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 tox-4.4.9/tests/execute/local_subprocess/tty_check.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.4.9/tests/journal/__init__.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 tox-4.4.9/tests/journal/test_main_journal.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 tox-4.4.9/tests/plugin/conftest.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 tox-4.4.9/tests/plugin/test_inline.py
--rw-r--r--   0        0        0     8398 2020-02-02 00:00:00.000000 tox-4.4.9/tests/plugin/test_plugin.py
--rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 tox-4.4.9/tests/plugin/test_plugin_custom_config_set.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.4.9/tests/pytest_/__init__.py
--rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 tox-4.4.9/tests/pytest_/test_init.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.4.9/tests/session/__init__.py
--rw-r--r--   0        0        0     3836 2020-02-02 00:00:00.000000 tox-4.4.9/tests/session/test_env_select.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 tox-4.4.9/tests/session/test_session_common.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.4.9/tests/session/cmd/__init__.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 tox-4.4.9/tests/session/cmd/test_depends.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 tox-4.4.9/tests/session/cmd/test_devenv.py
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 tox-4.4.9/tests/session/cmd/test_exec_.py
--rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 tox-4.4.9/tests/session/cmd/test_legacy.py
--rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 tox-4.4.9/tests/session/cmd/test_list_envs.py
--rw-r--r--   0        0        0     5775 2020-02-02 00:00:00.000000 tox-4.4.9/tests/session/cmd/test_parallel.py
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 tox-4.4.9/tests/session/cmd/test_quickstart.py
--rw-r--r--   0        0        0    18178 2020-02-02 00:00:00.000000 tox-4.4.9/tests/session/cmd/test_sequential.py
--rw-r--r--   0        0        0    11209 2020-02-02 00:00:00.000000 tox-4.4.9/tests/session/cmd/test_show_config.py
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 tox-4.4.9/tests/session/cmd/test_state.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.4.9/tests/session/cmd/run/__init__.py
--rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 tox-4.4.9/tests/session/cmd/run/test_common.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.4.9/tests/tox_env/__init__.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 tox-4.4.9/tests/tox_env/test_api.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 tox-4.4.9/tests/tox_env/test_info.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 tox-4.4.9/tests/tox_env/test_register.py
--rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 tox-4.4.9/tests/tox_env/test_tox_env_api.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 tox-4.4.9/tests/tox_env/test_tox_env_runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.4.9/tests/tox_env/python/__init__.py
--rw-r--r--   0        0        0     8593 2020-02-02 00:00:00.000000 tox-4.4.9/tests/tox_env/python/test_python_api.py
--rw-r--r--   0        0        0     5316 2020-02-02 00:00:00.000000 tox-4.4.9/tests/tox_env/python/test_python_runner.py
--rw-r--r--   0        0        0    17036 2020-02-02 00:00:00.000000 tox-4.4.9/tests/tox_env/python/pip/test_pip_install.py
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 tox-4.4.9/tests/tox_env/python/pip/test_req_file.py
--rw-r--r--   0        0        0    22126 2020-02-02 00:00:00.000000 tox-4.4.9/tests/tox_env/python/pip/req/test_file.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.4.9/tests/tox_env/python/test-pkg/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.4.9/tests/tox_env/python/virtual_env/__init__.py
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 tox-4.4.9/tests/tox_env/python/virtual_env/test_setuptools.py
--rw-r--r--   0        0        0     6537 2020-02-02 00:00:00.000000 tox-4.4.9/tests/tox_env/python/virtual_env/test_virtualenv_api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.4.9/tests/tox_env/python/virtual_env/package/__init__.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 tox-4.4.9/tests/tox_env/python/virtual_env/package/conftest.py
--rw-r--r--   0        0        0     6178 2020-02-02 00:00:00.000000 tox-4.4.9/tests/tox_env/python/virtual_env/package/test_package_cmd_builder.py
--rw-r--r--   0        0        0    10101 2020-02-02 00:00:00.000000 tox-4.4.9/tests/tox_env/python/virtual_env/package/test_package_pyproject.py
--rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 tox-4.4.9/tests/tox_env/python/virtual_env/package/test_python_package_util.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 tox-4.4.9/tests/type_check/add_config_container_factory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.4.9/tests/util/__init__.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 tox-4.4.9/tests/util/test_ci.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 tox-4.4.9/tests/util/test_cpu.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 tox-4.4.9/tests/util/test_graph.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 tox-4.4.9/tests/util/test_path.py
--rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 tox-4.4.9/tests/util/test_spinner.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 tox-4.4.9/.gitignore
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 tox-4.4.9/LICENSE
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 tox-4.4.9/README.md
--rw-r--r--   0        0        0     4525 2020-02-02 00:00:00.000000 tox-4.4.9/pyproject.toml
--rw-r--r--   0        0        0     4964 2020-02-02 00:00:00.000000 tox-4.4.9/PKG-INFO
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 tox-4.5.0/tox.ini
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/__init__.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/__main__.py
+-rw-r--r--   0        0        0     6005 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/provision.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/py.typed
+-rw-r--r--   0        0        0    19145 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/pytest.py
+-rw-r--r--   0        0        0     8278 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/report.py
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/run.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/config/__init__.py
+-rw-r--r--   0        0        0     6443 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/config/main.py
+-rw-r--r--   0        0        0     4187 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/config/of_type.py
+-rw-r--r--   0        0        0     4806 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/config/set_env.py
+-rw-r--r--   0        0        0     9891 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/config/sets.py
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/config/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/config/cli/__init__.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/config/cli/env_var.py
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/config/cli/ini.py
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/config/cli/parse.py
+-rw-r--r--   0        0        0    13671 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/config/cli/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/config/loader/__init__.py
+-rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/config/loader/api.py
+-rw-r--r--   0        0        0     6411 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/config/loader/convert.py
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/config/loader/memory.py
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/config/loader/section.py
+-rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/config/loader/str_convert.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/config/loader/stringify.py
+-rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/config/loader/ini/__init__.py
+-rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/config/loader/ini/factor.py
+-rw-r--r--   0        0        0    13352 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/config/loader/ini/replace.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/config/source/__init__.py
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/config/source/api.py
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/config/source/discover.py
+-rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/config/source/ini.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/config/source/ini_section.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/config/source/legacy_toml.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/config/source/setup_cfg.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/config/source/tox_ini.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/execute/__init__.py
+-rw-r--r--   0        0        0     9137 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/execute/api.py
+-rw-r--r--   0        0        0     5195 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/execute/pep517_backend.py
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/execute/request.py
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/execute/stream.py
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/execute/util.py
+-rw-r--r--   0        0        0    13863 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/execute/local_sub_process/__init__.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/execute/local_sub_process/read_via_thread.py
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/execute/local_sub_process/read_via_thread_unix.py
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/execute/local_sub_process/read_via_thread_windows.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/journal/__init__.py
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/journal/env.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/journal/main.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/plugin/__init__.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/plugin/inline.py
+-rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/plugin/manager.py
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/plugin/spec.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/session/__init__.py
+-rw-r--r--   0        0        0    18051 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/session/env_select.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/session/state.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/session/cmd/__init__.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/session/cmd/depends.py
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/session/cmd/devenv.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/session/cmd/exec_.py
+-rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/session/cmd/legacy.py
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/session/cmd/list_env.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/session/cmd/quickstart.py
+-rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/session/cmd/show_config.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/session/cmd/version_flag.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/session/cmd/run/__init__.py
+-rw-r--r--   0        0        0    16573 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/session/cmd/run/common.py
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/session/cmd/run/parallel.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/session/cmd/run/sequential.py
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/session/cmd/run/single.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/tox_env/__init__.py
+-rw-r--r--   0        0        0    20134 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/tox_env/api.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/tox_env/errors.py
+-rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/tox_env/info.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/tox_env/installer.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/tox_env/package.py
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/tox_env/register.py
+-rw-r--r--   0        0        0     7761 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/tox_env/runner.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/tox_env/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/tox_env/python/__init__.py
+-rw-r--r--   0        0        0    10900 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/tox_env/python/api.py
+-rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/tox_env/python/package.py
+-rw-r--r--   0        0        0     4446 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/tox_env/python/runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/tox_env/python/pip/__init__.py
+-rw-r--r--   0        0        0    10355 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/tox_env/python/pip/pip_install.py
+-rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/tox_env/python/pip/req_file.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/tox_env/python/pip/req/__init__.py
+-rw-r--r--   0        0        0     4299 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/tox_env/python/pip/req/args.py
+-rw-r--r--   0        0        0    19406 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/tox_env/python/pip/req/file.py
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/tox_env/python/pip/req/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/tox_env/python/virtual_env/__init__.py
+-rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/tox_env/python/virtual_env/api.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/tox_env/python/virtual_env/runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/tox_env/python/virtual_env/package/__init__.py
+-rw-r--r--   0        0        0     7053 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/tox_env/python/virtual_env/package/cmd_builder.py
+-rw-r--r--   0        0        0    17577 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/tox_env/python/virtual_env/package/pyproject.py
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/tox_env/python/virtual_env/package/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/util/__init__.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/util/ci.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/util/cpu.py
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/util/file_view.py
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/util/graph.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/util/path.py
+-rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 tox-4.5.0/src/tox/util/spinner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     5439 2020-02-02 00:00:00.000000 tox-4.5.0/tests/conftest.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 tox-4.5.0/tests/test_call_modes.py
+-rw-r--r--   0        0        0     9796 2020-02-02 00:00:00.000000 tox-4.5.0/tests/test_provision.py
+-rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 tox-4.5.0/tests/test_report.py
+-rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 tox-4.5.0/tests/test_run.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 tox-4.5.0/tests/test_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.0/tests/config/__init__.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 tox-4.5.0/tests/config/conftest.py
+-rw-r--r--   0        0        0     3888 2020-02-02 00:00:00.000000 tox-4.5.0/tests/config/test_main.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 tox-4.5.0/tests/config/test_of_types.py
+-rw-r--r--   0        0        0     5827 2020-02-02 00:00:00.000000 tox-4.5.0/tests/config/test_set_env.py
+-rw-r--r--   0        0        0     7157 2020-02-02 00:00:00.000000 tox-4.5.0/tests/config/test_sets.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 tox-4.5.0/tests/config/test_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.0/tests/config/cli/__init__.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 tox-4.5.0/tests/config/cli/conftest.py
+-rw-r--r--   0        0        0     5105 2020-02-02 00:00:00.000000 tox-4.5.0/tests/config/cli/test_cli_env_var.py
+-rw-r--r--   0        0        0     7197 2020-02-02 00:00:00.000000 tox-4.5.0/tests/config/cli/test_cli_ini.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 tox-4.5.0/tests/config/cli/test_parse.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 tox-4.5.0/tests/config/cli/test_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.0/tests/config/loader/__init__.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 tox-4.5.0/tests/config/loader/test_loader.py
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 tox-4.5.0/tests/config/loader/test_memory_loader.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 tox-4.5.0/tests/config/loader/test_section.py
+-rw-r--r--   0        0        0     7098 2020-02-02 00:00:00.000000 tox-4.5.0/tests/config/loader/test_str_convert.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.0/tests/config/loader/ini/__init__.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 tox-4.5.0/tests/config/loader/ini/conftest.py
+-rw-r--r--   0        0        0     6454 2020-02-02 00:00:00.000000 tox-4.5.0/tests/config/loader/ini/test_factor.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 tox-4.5.0/tests/config/loader/ini/test_ini_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.0/tests/config/loader/ini/replace/__init__.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tox-4.5.0/tests/config/loader/ini/replace/conftest.py
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 tox-4.5.0/tests/config/loader/ini/replace/test_replace.py
+-rw-r--r--   0        0        0     7159 2020-02-02 00:00:00.000000 tox-4.5.0/tests/config/loader/ini/replace/test_replace_env_var.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 tox-4.5.0/tests/config/loader/ini/replace/test_replace_os_pathsep.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 tox-4.5.0/tests/config/loader/ini/replace/test_replace_os_sep.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 tox-4.5.0/tests/config/loader/ini/replace/test_replace_posargs.py
+-rw-r--r--   0        0        0     8296 2020-02-02 00:00:00.000000 tox-4.5.0/tests/config/loader/ini/replace/test_replace_tox_env.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 tox-4.5.0/tests/config/loader/ini/replace/test_replace_tty.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.0/tests/config/source/__init__.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 tox-4.5.0/tests/config/source/test_discover.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 tox-4.5.0/tests/config/source/test_legacy_toml.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 tox-4.5.0/tests/config/source/test_setup_cfg.py
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 tox-4.5.0/tests/config/source/test_source_ini.py
+-rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 tox-4.5.0/tests/demo_pkg_inline/build.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 tox-4.5.0/tests/demo_pkg_inline/build.pyi
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 tox-4.5.0/tests/demo_pkg_inline/pyproject.toml
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 tox-4.5.0/tests/demo_pkg_setuptools/pyproject.toml
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 tox-4.5.0/tests/demo_pkg_setuptools/setup.cfg
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 tox-4.5.0/tests/demo_pkg_setuptools/demo_pkg_setuptools/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.0/tests/execute/__init__.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 tox-4.5.0/tests/execute/conftest.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 tox-4.5.0/tests/execute/test_request.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 tox-4.5.0/tests/execute/test_stream.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.0/tests/execute/local_subprocess/__init__.py
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 tox-4.5.0/tests/execute/local_subprocess/bad_process.py
+-rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 tox-4.5.0/tests/execute/local_subprocess/local_subprocess_sigint.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 tox-4.5.0/tests/execute/local_subprocess/test_execute_util.py
+-rw-r--r--   0        0        0    14088 2020-02-02 00:00:00.000000 tox-4.5.0/tests/execute/local_subprocess/test_local_subprocess.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 tox-4.5.0/tests/execute/local_subprocess/tty_check.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.0/tests/journal/__init__.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 tox-4.5.0/tests/journal/test_main_journal.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 tox-4.5.0/tests/plugin/conftest.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 tox-4.5.0/tests/plugin/test_inline.py
+-rw-r--r--   0        0        0     9068 2020-02-02 00:00:00.000000 tox-4.5.0/tests/plugin/test_plugin.py
+-rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 tox-4.5.0/tests/plugin/test_plugin_custom_config_set.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.0/tests/pytest_/__init__.py
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 tox-4.5.0/tests/pytest_/test_init.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.0/tests/session/__init__.py
+-rw-r--r--   0        0        0     3836 2020-02-02 00:00:00.000000 tox-4.5.0/tests/session/test_env_select.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 tox-4.5.0/tests/session/test_session_common.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.0/tests/session/cmd/__init__.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 tox-4.5.0/tests/session/cmd/test_depends.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 tox-4.5.0/tests/session/cmd/test_devenv.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 tox-4.5.0/tests/session/cmd/test_exec_.py
+-rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 tox-4.5.0/tests/session/cmd/test_legacy.py
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 tox-4.5.0/tests/session/cmd/test_list_envs.py
+-rw-r--r--   0        0        0     5775 2020-02-02 00:00:00.000000 tox-4.5.0/tests/session/cmd/test_parallel.py
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 tox-4.5.0/tests/session/cmd/test_quickstart.py
+-rw-r--r--   0        0        0    18713 2020-02-02 00:00:00.000000 tox-4.5.0/tests/session/cmd/test_sequential.py
+-rw-r--r--   0        0        0    11209 2020-02-02 00:00:00.000000 tox-4.5.0/tests/session/cmd/test_show_config.py
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 tox-4.5.0/tests/session/cmd/test_state.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.0/tests/session/cmd/run/__init__.py
+-rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 tox-4.5.0/tests/session/cmd/run/test_common.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.0/tests/tox_env/__init__.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 tox-4.5.0/tests/tox_env/test_api.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 tox-4.5.0/tests/tox_env/test_info.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 tox-4.5.0/tests/tox_env/test_register.py
+-rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 tox-4.5.0/tests/tox_env/test_tox_env_api.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 tox-4.5.0/tests/tox_env/test_tox_env_runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.0/tests/tox_env/python/__init__.py
+-rw-r--r--   0        0        0     8593 2020-02-02 00:00:00.000000 tox-4.5.0/tests/tox_env/python/test_python_api.py
+-rw-r--r--   0        0        0     5428 2020-02-02 00:00:00.000000 tox-4.5.0/tests/tox_env/python/test_python_runner.py
+-rw-r--r--   0        0        0    17036 2020-02-02 00:00:00.000000 tox-4.5.0/tests/tox_env/python/pip/test_pip_install.py
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 tox-4.5.0/tests/tox_env/python/pip/test_req_file.py
+-rw-r--r--   0        0        0    22126 2020-02-02 00:00:00.000000 tox-4.5.0/tests/tox_env/python/pip/req/test_file.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.0/tests/tox_env/python/test-pkg/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.0/tests/tox_env/python/virtual_env/__init__.py
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 tox-4.5.0/tests/tox_env/python/virtual_env/test_setuptools.py
+-rw-r--r--   0        0        0     6537 2020-02-02 00:00:00.000000 tox-4.5.0/tests/tox_env/python/virtual_env/test_virtualenv_api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.0/tests/tox_env/python/virtual_env/package/__init__.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 tox-4.5.0/tests/tox_env/python/virtual_env/package/conftest.py
+-rw-r--r--   0        0        0     6178 2020-02-02 00:00:00.000000 tox-4.5.0/tests/tox_env/python/virtual_env/package/test_package_cmd_builder.py
+-rw-r--r--   0        0        0    10101 2020-02-02 00:00:00.000000 tox-4.5.0/tests/tox_env/python/virtual_env/package/test_package_pyproject.py
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 tox-4.5.0/tests/tox_env/python/virtual_env/package/test_python_package_util.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 tox-4.5.0/tests/type_check/add_config_container_factory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.5.0/tests/util/__init__.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 tox-4.5.0/tests/util/test_ci.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 tox-4.5.0/tests/util/test_cpu.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 tox-4.5.0/tests/util/test_graph.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 tox-4.5.0/tests/util/test_path.py
+-rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 tox-4.5.0/tests/util/test_spinner.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 tox-4.5.0/.gitignore
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 tox-4.5.0/LICENSE
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 tox-4.5.0/README.md
+-rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 tox-4.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 tox-4.5.0/PKG-INFO
```

### Comparing `tox-4.4.9/tox.ini` & `tox-4.5.0/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 [tox]
-envlist =
+requires =
+    tox>=4.2
+env_list =
     fix
     py311
     py310
     py39
     py38
     py37
     cov
     type
     docs
     pkg_meta
-isolated_build = true
 skip_missing_interpreters = true
-minversion = 3.22
 
 [testenv]
 description = run the tests with pytest under {envname}
-passenv =
+package = wheel
+wheel_build_env = .pkg
+extras =
+    testing
+pass_env =
     PYTEST_*
     SSL_CERT_FILE
-setenv =
+set_env =
     COVERAGE_FILE = {env:COVERAGE_FILE:{toxworkdir}{/}.coverage.{envname}}
     COVERAGE_PROCESS_START = {toxinidir}{/}pyproject.toml
-extras =
-    testing
 commands =
     pytest {posargs: \
       --junitxml {toxworkdir}{/}junit.{envname}.xml --cov {envsitepackagesdir}{/}tox --cov {toxinidir}{/}tests \
       --cov-config={toxinidir}{/}pyproject.toml --no-cov-on-fail --cov-report term-missing:skip-covered --cov-context=test \
       --cov-report html:{envtmpdir}{/}htmlcov \
       --cov-report xml:{toxworkdir}{/}coverage.{envname}.xml \
       -n={env:PYTEST_XDIST_AUTO_NUM_WORKERS:auto} \
       tests --durations 5 --run-integration}
     diff-cover --compare-branch {env:DIFF_AGAINST:origin/main} {toxworkdir}{/}coverage.{envname}.xml
-package = wheel
-wheel_build_env = .pkg
 
 [testenv:fix]
 description = format the code base to adhere to our styles, and complain about what we cannot do automatically
-passenv =
-    {[testenv]passenv}
-    PROGRAMDATA
 skip_install = true
 deps =
-    pre-commit>=3.2
+    pre-commit>=3.2.2
+pass_env =
+    {[testenv]passenv}
+    PROGRAMDATA
 commands =
     pre-commit run --all-files --show-diff-on-failure {posargs}
     python -c 'print(r"hint: run {envbindir}{/}pre-commit install to add checks as pre-commit hook")'
 
 [testenv:type]
 description = run type check on code base
 deps =
-    mypy==1.1.1
-    types-cachetools>=5.3.0.4
-    types-chardet>=5.0.4.2
+    mypy==1.2
+    types-cachetools>=5.3.0.5
+    types-chardet>=5.0.4.3
 commands =
     mypy src/tox
     mypy tests
 
 [testenv:docs]
 description = build documentation
 extras =
@@ -79,22 +79,22 @@
     check-wheel-contents --no-config {envtmpdir}
 
 [testenv:release]
 description = do a release, required posarg of the version number
 skip_install = true
 deps =
     gitpython>=3.1.31
-    packaging>=23
+    packaging>=23.1
     towncrier>=22.12
 commands =
     python {toxinidir}/tasks/release.py --version {posargs}
 
 [testenv:dev]
 description = dev environment with all deps at {envdir}
-usedevelop = true
+package = editable
 deps =
     {[testenv:release]deps}
 extras =
     docs
     testing
 commands =
     python -m pip list --format=columns
```

### Comparing `tox-4.4.9/src/tox/provision.py` & `tox-4.5.0/src/tox/provision.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,14 +80,19 @@
     state.conf.core.add_config(
         keys="requires",
         of_type=List[Requirement],
         default=[],
         desc="Name of the virtual environment used to provision a tox.",
         post_process=add_tox_requires_min_version,
     )
+
+    from tox.plugin.manager import MANAGER
+
+    MANAGER.tox_add_core_config(state.conf.core, state)
+
     requires: list[Requirement] = state.conf.core["requires"]
     missing = _get_missing(requires)
 
     deps = ", ".join(f"{p}{'' if v is None else f' ({v})'}" for p, v in missing)
     loader = MemoryLoader(  # these configuration values are loaded from in-memory always (no file conf)
         base=[],  # disable inheritance for provision environments
         package="skip",  # no packaging for this please
@@ -96,18 +101,14 @@
         pass_env=["*"],  # do not filter environment variables, will be handled by provisioned tox
         recreate=state.conf.options.recreate and not state.conf.options.no_recreate_provision,
     )
     provision_tox_env: str = state.conf.core["provision_tox_env"]
     state.conf.memory_seed_loaders[provision_tox_env].append(loader)
     state.envs._mark_provision(bool(missing), provision_tox_env)
 
-    from tox.plugin.manager import MANAGER
-
-    MANAGER.tox_add_core_config(state.conf.core, state)
-
     if not missing:
         return False
 
     miss_msg = f"is missing [requires (has)]: {deps}"
 
     no_provision: bool | str = state.conf.options.no_provision
     if no_provision:
```

### Comparing `tox-4.4.9/src/tox/pytest.py` & `tox-4.5.0/src/tox/pytest.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/report.py` & `tox-4.5.0/src/tox/report.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/run.py` & `tox-4.5.0/src/tox/run.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/config/main.py` & `tox-4.5.0/src/tox/config/main.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/config/of_type.py` & `tox-4.5.0/src/tox/config/of_type.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/config/set_env.py` & `tox-4.5.0/src/tox/config/set_env.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/config/sets.py` & `tox-4.5.0/src/tox/config/sets.py`

 * *Files 5% similar despite different names*

```diff
@@ -175,40 +175,43 @@
     def __init__(self, conf: Config, section: Section, root: Path, src_path: Path) -> None:
         self._root = root
         self._src_path = src_path
         super().__init__(conf, section=section, env_name=None)
         desc = "define environments to automatically run"
         self.add_config(keys=["env_list", "envlist"], of_type=EnvList, default=EnvList([]), desc=desc)
 
+    def _default_work_dir(self, conf: Config, env_name: str | None) -> Path:  # noqa: U100
+        return cast(Path, self["tox_root"] / ".tox")
+
+    def _default_temp_dir(self, conf: Config, env_name: str | None) -> Path:  # noqa: U100
+        return cast(Path, self["work_dir"] / ".tmp")
+
+    def _work_dir_post_process(self, dir: Path) -> Path:
+        return self._conf.work_dir if self._conf.options.work_dir else dir
+
     def register_config(self) -> None:
         self.add_constant(keys=["config_file_path"], desc="path to the configuration file", value=self._src_path)
         self.add_config(
             keys=["tox_root", "toxinidir"],
             of_type=Path,
             default=self._root,
             desc="the root directory (where the configuration file is found)",
         )
 
-        def work_dir_builder(conf: Config, env_name: str | None) -> Path:  # noqa: U100
-            return (conf.work_dir if conf.work_dir is not None else cast(Path, self["tox_root"])) / ".tox"
-
-        def work_dir_post_process(value: Path) -> Path:
-            return self._conf.work_dir if self._conf.options.work_dir else value
-
         self.add_config(
             keys=["work_dir", "toxworkdir"],
             of_type=Path,
-            default=work_dir_builder,
-            post_process=work_dir_post_process,
+            default=self._default_work_dir,
+            post_process=self._work_dir_post_process,
             desc="working directory",
         )
         self.add_config(
             keys=["temp_dir"],
             of_type=Path,
-            default=lambda conf, _: cast(Path, self["work_dir"]) / ".tmp",  # noqa: U100, U101
+            default=self._default_temp_dir,
             desc="a folder for temporary files (is not cleaned at start)",
         )
         self.add_constant("host_python", "the host python executable path", sys.executable)
 
     def _on_duplicate_conf(self, key: str, definition: ConfigDefinition[V]) -> None:  # noqa: U100
         pass  # core definitions may be defined multiple times as long as all their options match, first defined wins
```

### Comparing `tox-4.4.9/src/tox/config/types.py` & `tox-4.5.0/src/tox/config/types.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/config/cli/env_var.py` & `tox-4.5.0/src/tox/config/cli/env_var.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/config/cli/ini.py` & `tox-4.5.0/src/tox/config/cli/ini.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/config/cli/parse.py` & `tox-4.5.0/src/tox/config/cli/parse.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/config/cli/parser.py` & `tox-4.5.0/src/tox/config/cli/parser.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/config/loader/api.py` & `tox-4.5.0/src/tox/config/loader/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/config/loader/convert.py` & `tox-4.5.0/src/tox/config/loader/convert.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/config/loader/memory.py` & `tox-4.5.0/src/tox/config/loader/memory.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/config/loader/section.py` & `tox-4.5.0/src/tox/config/loader/section.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/config/loader/str_convert.py` & `tox-4.5.0/src/tox/config/loader/str_convert.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/config/loader/stringify.py` & `tox-4.5.0/src/tox/config/loader/stringify.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/config/loader/ini/__init__.py` & `tox-4.5.0/src/tox/config/loader/ini/__init__.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/config/loader/ini/factor.py` & `tox-4.5.0/src/tox/config/loader/ini/factor.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/config/loader/ini/replace.py` & `tox-4.5.0/src/tox/config/loader/ini/replace.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/config/source/api.py` & `tox-4.5.0/src/tox/config/source/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/config/source/discover.py` & `tox-4.5.0/src/tox/config/source/discover.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/config/source/ini.py` & `tox-4.5.0/src/tox/config/source/ini.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/config/source/ini_section.py` & `tox-4.5.0/src/tox/config/source/ini_section.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/config/source/legacy_toml.py` & `tox-4.5.0/src/tox/config/source/legacy_toml.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/execute/api.py` & `tox-4.5.0/src/tox/execute/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/execute/pep517_backend.py` & `tox-4.5.0/src/tox/execute/pep517_backend.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/execute/request.py` & `tox-4.5.0/src/tox/execute/request.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/execute/stream.py` & `tox-4.5.0/src/tox/execute/stream.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/execute/util.py` & `tox-4.5.0/src/tox/execute/util.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/execute/local_sub_process/__init__.py` & `tox-4.5.0/src/tox/execute/local_sub_process/__init__.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/execute/local_sub_process/read_via_thread.py` & `tox-4.5.0/src/tox/execute/local_sub_process/read_via_thread.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/execute/local_sub_process/read_via_thread_unix.py` & `tox-4.5.0/src/tox/execute/local_sub_process/read_via_thread_unix.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/execute/local_sub_process/read_via_thread_windows.py` & `tox-4.5.0/src/tox/execute/local_sub_process/read_via_thread_windows.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/journal/env.py` & `tox-4.5.0/src/tox/journal/env.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/journal/main.py` & `tox-4.5.0/src/tox/journal/main.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/plugin/__init__.py` & `tox-4.5.0/src/tox/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/plugin/inline.py` & `tox-4.5.0/src/tox/plugin/inline.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/plugin/manager.py` & `tox-4.5.0/src/tox/plugin/manager.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/plugin/spec.py` & `tox-4.5.0/src/tox/plugin/spec.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/session/env_select.py` & `tox-4.5.0/src/tox/session/env_select.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/session/state.py` & `tox-4.5.0/src/tox/session/state.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/session/cmd/depends.py` & `tox-4.5.0/src/tox/session/cmd/depends.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/session/cmd/devenv.py` & `tox-4.5.0/src/tox/session/cmd/devenv.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/session/cmd/exec_.py` & `tox-4.5.0/src/tox/session/cmd/exec_.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/session/cmd/legacy.py` & `tox-4.5.0/src/tox/session/cmd/legacy.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/session/cmd/list_env.py` & `tox-4.5.0/src/tox/session/cmd/list_env.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/session/cmd/quickstart.py` & `tox-4.5.0/src/tox/session/cmd/quickstart.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/session/cmd/show_config.py` & `tox-4.5.0/src/tox/session/cmd/show_config.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/session/cmd/version_flag.py` & `tox-4.5.0/src/tox/session/cmd/version_flag.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/session/cmd/run/common.py` & `tox-4.5.0/src/tox/session/cmd/run/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,15 @@
         if verbosity:
             print(f"{color_ if is_colored else ''}{message}{Fore.RESET if is_colored else ''}")
 
     successful, skipped = [], []
     for run in runs:
         successful.append(run.code == Outcome.OK or run.ignore_outcome)
         skipped.append(run.skipped)
-        duration_individual = [o.elapsed for o in run.outcomes]
+        duration_individual = [o.elapsed for o in run.outcomes] if verbosity >= 2 else []
         extra = f"+cmd[{','.join(f'{i:.2f}' for i in duration_individual)}]" if duration_individual else ""
         setup = run.duration - sum(duration_individual)
         msg, color = _get_outcome_message(run)
         out = f"  {run.name}: {msg} ({run.duration:.2f}{f'=setup[{setup:.2f}]{extra}' if extra else ''} seconds)"
         _print(color, out)
 
     duration = time.monotonic() - start
```

### Comparing `tox-4.4.9/src/tox/session/cmd/run/parallel.py` & `tox-4.5.0/src/tox/session/cmd/run/parallel.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/session/cmd/run/sequential.py` & `tox-4.5.0/src/tox/session/cmd/run/sequential.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/session/cmd/run/single.py` & `tox-4.5.0/src/tox/session/cmd/run/single.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/tox_env/api.py` & `tox-4.5.0/src/tox/tox_env/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/tox_env/info.py` & `tox-4.5.0/src/tox/tox_env/info.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/tox_env/installer.py` & `tox-4.5.0/src/tox/tox_env/installer.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/tox_env/package.py` & `tox-4.5.0/src/tox/tox_env/package.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/tox_env/register.py` & `tox-4.5.0/src/tox/tox_env/register.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/tox_env/runner.py` & `tox-4.5.0/src/tox/tox_env/runner.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/tox_env/util.py` & `tox-4.5.0/src/tox/tox_env/util.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/tox_env/python/api.py` & `tox-4.5.0/src/tox/tox_env/python/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/tox_env/python/package.py` & `tox-4.5.0/src/tox/tox_env/python/package.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/tox_env/python/runner.py` & `tox-4.5.0/src/tox/tox_env/python/runner.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/tox_env/python/pip/pip_install.py` & `tox-4.5.0/src/tox/tox_env/python/pip/pip_install.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/tox_env/python/pip/req_file.py` & `tox-4.5.0/src/tox/tox_env/python/pip/req_file.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/tox_env/python/pip/req/args.py` & `tox-4.5.0/src/tox/tox_env/python/pip/req/args.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/tox_env/python/pip/req/file.py` & `tox-4.5.0/src/tox/tox_env/python/pip/req/file.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/tox_env/python/pip/req/util.py` & `tox-4.5.0/src/tox/tox_env/python/pip/req/util.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/tox_env/python/virtual_env/api.py` & `tox-4.5.0/src/tox/tox_env/python/virtual_env/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/tox_env/python/virtual_env/runner.py` & `tox-4.5.0/src/tox/tox_env/python/virtual_env/runner.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/tox_env/python/virtual_env/package/cmd_builder.py` & `tox-4.5.0/src/tox/tox_env/python/virtual_env/package/cmd_builder.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/tox_env/python/virtual_env/package/pyproject.py` & `tox-4.5.0/src/tox/tox_env/python/virtual_env/package/pyproject.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/tox_env/python/virtual_env/package/util.py` & `tox-4.5.0/src/tox/tox_env/python/virtual_env/package/util.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/util/ci.py` & `tox-4.5.0/src/tox/util/ci.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/util/file_view.py` & `tox-4.5.0/src/tox/util/file_view.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/util/graph.py` & `tox-4.5.0/src/tox/util/graph.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/util/path.py` & `tox-4.5.0/src/tox/util/path.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/src/tox/util/spinner.py` & `tox-4.5.0/src/tox/util/spinner.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/conftest.py` & `tox-4.5.0/tests/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from unittest.mock import patch
 from uuid import uuid4
 
 import pytest
 from _pytest.monkeypatch import MonkeyPatch  # cannot import from tox.pytest yet
 from _pytest.tmpdir import TempPathFactory
 from distlib.scripts import ScriptMaker
+from filelock import FileLock
 from pytest_mock import MockerFixture
 from virtualenv import cli_run
 
 from tox.config.cli.parser import Parsed
 from tox.config.loader.api import Override
 from tox.config.main import Config
 from tox.config.source import discover_source
@@ -73,16 +74,18 @@
 
 @pytest.fixture(scope="session")
 def demo_pkg_setuptools() -> Path:
     return HERE / "demo_pkg_setuptools"
 
 
 @pytest.fixture(scope="session")
-def demo_pkg_inline() -> Path:
-    return HERE / "demo_pkg_inline"
+def demo_pkg_inline() -> Iterator[Path]:
+    demo_path = HERE / "demo_pkg_inline"
+    with FileLock(f"{demo_path}.lock"):
+        yield demo_path
 
 
 @pytest.fixture()
 def patch_prev_py(mocker: MockerFixture) -> Callable[[bool], tuple[str, str]]:
     def _func(has_prev: bool) -> tuple[str, str]:
         ver = sys.version_info[0:2]
         prev_ver = "".join(str(i) for i in (ver[0], ver[1] - 1))
```

### Comparing `tox-4.4.9/tests/test_provision.py` & `tox-4.5.0/tests/test_provision.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/test_report.py` & `tox-4.5.0/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/test_version.py` & `tox-4.5.0/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/config/test_main.py` & `tox-4.5.0/tests/config/test_main.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/config/test_of_types.py` & `tox-4.5.0/tests/config/test_of_types.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/config/test_set_env.py` & `tox-4.5.0/tests/config/test_set_env.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/config/test_sets.py` & `tox-4.5.0/tests/config/test_sets.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/config/test_types.py` & `tox-4.5.0/tests/config/test_types.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/config/cli/conftest.py` & `tox-4.5.0/tests/config/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/config/cli/test_cli_env_var.py` & `tox-4.5.0/tests/config/cli/test_cli_env_var.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/config/cli/test_cli_ini.py` & `tox-4.5.0/tests/config/cli/test_cli_ini.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/config/cli/test_parse.py` & `tox-4.5.0/tests/config/cli/test_parse.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/config/cli/test_parser.py` & `tox-4.5.0/tests/config/cli/test_parser.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/config/loader/test_loader.py` & `tox-4.5.0/tests/config/loader/test_loader.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/config/loader/test_memory_loader.py` & `tox-4.5.0/tests/config/loader/test_memory_loader.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/config/loader/test_section.py` & `tox-4.5.0/tests/config/loader/test_section.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/config/loader/test_str_convert.py` & `tox-4.5.0/tests/config/loader/test_str_convert.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/config/loader/ini/conftest.py` & `tox-4.5.0/tests/config/loader/ini/conftest.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/config/loader/ini/test_factor.py` & `tox-4.5.0/tests/config/loader/ini/test_factor.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/config/loader/ini/test_ini_loader.py` & `tox-4.5.0/tests/config/loader/ini/test_ini_loader.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/config/loader/ini/replace/conftest.py` & `tox-4.5.0/tests/config/loader/ini/replace/conftest.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/config/loader/ini/replace/test_replace.py` & `tox-4.5.0/tests/config/loader/ini/replace/test_replace.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/config/loader/ini/replace/test_replace_env_var.py` & `tox-4.5.0/tests/config/loader/ini/replace/test_replace_env_var.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/config/loader/ini/replace/test_replace_os_sep.py` & `tox-4.5.0/tests/config/loader/ini/replace/test_replace_os_sep.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/config/loader/ini/replace/test_replace_posargs.py` & `tox-4.5.0/tests/config/loader/ini/replace/test_replace_posargs.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/config/loader/ini/replace/test_replace_tox_env.py` & `tox-4.5.0/tests/config/loader/ini/replace/test_replace_tox_env.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/config/loader/ini/replace/test_replace_tty.py` & `tox-4.5.0/tests/config/loader/ini/replace/test_replace_tty.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/config/source/test_discover.py` & `tox-4.5.0/tests/config/source/test_discover.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/config/source/test_setup_cfg.py` & `tox-4.5.0/tests/config/source/test_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/config/source/test_source_ini.py` & `tox-4.5.0/tests/config/source/test_source_ini.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/demo_pkg_inline/build.py` & `tox-4.5.0/tests/demo_pkg_inline/build.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/demo_pkg_inline/build.pyi` & `tox-4.5.0/tests/demo_pkg_inline/build.pyi`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/execute/test_request.py` & `tox-4.5.0/tests/execute/test_request.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/execute/local_subprocess/bad_process.py` & `tox-4.5.0/tests/execute/local_subprocess/bad_process.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/execute/local_subprocess/local_subprocess_sigint.py` & `tox-4.5.0/tests/execute/local_subprocess/local_subprocess_sigint.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/execute/local_subprocess/test_execute_util.py` & `tox-4.5.0/tests/execute/local_subprocess/test_execute_util.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/execute/local_subprocess/test_local_subprocess.py` & `tox-4.5.0/tests/execute/local_subprocess/test_local_subprocess.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/journal/test_main_journal.py` & `tox-4.5.0/tests/journal/test_main_journal.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/plugin/test_inline.py` & `tox-4.5.0/tests/plugin/test_inline.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/plugin/test_plugin.py` & `tox-4.5.0/tests/plugin/test_plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import logging
 import os
 import sys
+from pathlib import Path
 from typing import Any
 from unittest.mock import patch
 
 import pytest
 from pytest_mock import MockerFixture
 
 from tox.config.cli.parser import ToxParser
@@ -98,14 +99,41 @@
         mocker.ANY,  # report a
         mocker.ANY,  # report b
         mocker.ANY,  # overall report
     ]
     assert result.out.splitlines() == expected, result.out
 
 
+@pytest.mark.parametrize(
+    "dir_name",
+    [
+        "tox_root",
+        "work_dir",
+        "temp_dir",
+    ],
+)
+def test_plugin_can_set_core_conf(
+    tox_project: ToxProjectCreator,
+    mocker: MockerFixture,
+    dir_name: str,
+    tmp_path: Path,
+) -> None:
+    @impl
+    def tox_add_core_config(core_conf: CoreConfigSet, state: State) -> None:  # noqa: U100
+        core_conf.loaders.insert(0, MemoryLoader(**{dir_name: tmp_path}))
+
+    register_inline_plugin(mocker, tox_add_core_config)
+
+    project = tox_project({})
+    result = project.run("c")
+    result.assert_success()
+
+    assert result.state.conf.core[dir_name] == tmp_path
+
+
 def test_plugin_can_read_env_list(tox_project: ToxProjectCreator, mocker: MockerFixture) -> None:
     @impl
     def tox_add_core_config(core_conf: CoreConfigSet, state: State) -> None:  # noqa: U100
         logging.warning("All envs: %s", ", ".join(state.envs.iter(only_active=False)))
         logging.warning("Default envs: %s", ", ".join(state.envs.iter(only_active=True)))
 
     register_inline_plugin(mocker, tox_add_core_config)
```

### Comparing `tox-4.4.9/tests/plugin/test_plugin_custom_config_set.py` & `tox-4.5.0/tests/plugin/test_plugin_custom_config_set.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/pytest_/test_init.py` & `tox-4.5.0/tests/pytest_/test_init.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/session/test_env_select.py` & `tox-4.5.0/tests/session/test_env_select.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/session/test_session_common.py` & `tox-4.5.0/tests/session/test_session_common.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/session/cmd/test_depends.py` & `tox-4.5.0/tests/session/cmd/test_depends.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/session/cmd/test_devenv.py` & `tox-4.5.0/tests/session/cmd/test_devenv.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/session/cmd/test_exec_.py` & `tox-4.5.0/tests/session/cmd/test_exec_.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/session/cmd/test_legacy.py` & `tox-4.5.0/tests/session/cmd/test_legacy.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/session/cmd/test_list_envs.py` & `tox-4.5.0/tests/session/cmd/test_list_envs.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/session/cmd/test_parallel.py` & `tox-4.5.0/tests/session/cmd/test_parallel.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/session/cmd/test_quickstart.py` & `tox-4.5.0/tests/session/cmd/test_quickstart.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/session/cmd/test_sequential.py` & `tox-4.5.0/tests/session/cmd/test_sequential.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,24 @@
     outcome.assert_failed()
     reports = outcome.out.splitlines()[-3:]
     assert Matches(r"  evaluation failed :\( \(.* seconds\)") == reports[-1]
     assert Matches(r"  b: OK \(.*=setup\[.*\]\+cmd\[.*\] seconds\)") == reports[-2]
     assert Matches(r"  a: FAIL code 1 \(.*=setup\[.*\]\+cmd\[.*\] seconds\)") == reports[-3]
 
 
+def test_run_sequential_quiet(tox_project: ToxProjectCreator) -> None:
+    ini = "[tox]\nenv_list=a\nno_package=true\n[testenv]\ncommands=python -V"
+    project = tox_project({"tox.ini": ini})
+    outcome = project.run("r", "-q", "-e", "a")
+    outcome.assert_success()
+    reports = outcome.out.splitlines()[-3:]
+    assert Matches(r"  congratulations :\) \(.* seconds\)") == reports[-1]
+    assert Matches(r"  a: OK \([\d.]+ seconds\)") == reports[-2]
+
+
 @pytest.mark.integration()
 def test_result_json_sequential(
     tox_project: ToxProjectCreator,
     enable_pip_pypi_access: str | None,  # noqa: U100
 ) -> None:
     cmd = [
         "- python -c 'import sys; print(\"magic fail\", file=sys.stderr); sys.exit(1)'",
@@ -276,15 +286,15 @@
     result_first.assert_success()
     assert result_first.out.startswith("py: skip building and installing the package"), result_first.out
 
 
 def test_skip_develop_mode(tox_project: ToxProjectCreator, demo_pkg_setuptools: Path) -> None:
     proj = tox_project({"tox.ini": "[testenv]\npackage=wheel\n"})
     execute_calls = proj.patch_execute(lambda r: 0 if "install" in r.run_id else None)
-    result = proj.run("--root", str(demo_pkg_setuptools), "--develop")
+    result = proj.run("--root", str(demo_pkg_setuptools), "--develop", "--workdir", str(proj.path / ".tox"))
     result.assert_success()
     calls = [(i[0][0].conf.name, i[0][3].run_id) for i in execute_calls.call_args_list]
     expected = [
         (".pkg", "install_requires"),
         (".pkg", "_optional_hooks"),
         (".pkg", "get_requires_for_build_editable"),
         (".pkg", "install_requires_for_build_editable"),
@@ -426,15 +436,15 @@
 def test_sequential_inserted_env_vars(tox_project: ToxProjectCreator, demo_pkg_inline: Path) -> None:
     ini = """
     [testenv]
     commands=python -c 'import os; [print(f"{k}={v}") for k, v in os.environ.items() if \
                         k.startswith("TOX_") or k == "VIRTUAL_ENV"]'
     """
     project = tox_project({"tox.ini": ini})
-    result = project.run("r", "--root", str(demo_pkg_inline))
+    result = project.run("r", "--root", str(demo_pkg_inline), "--workdir", str(project.path / ".tox"))
     result.assert_success()
 
     assert re.search(f"TOX_PACKAGE={re.escape(str(project.path))}.*.tar.gz{os.linesep}", result.out)
     assert f"TOX_ENV_NAME=py{os.linesep}" in result.out
     work_dir = project.path / ".tox"
     assert f"TOX_WORK_DIR={work_dir}{os.linesep}" in result.out
     env_dir = work_dir / "py"
```

### Comparing `tox-4.4.9/tests/session/cmd/test_show_config.py` & `tox-4.5.0/tests/session/cmd/test_show_config.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/session/cmd/test_state.py` & `tox-4.5.0/tests/session/cmd/test_state.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/session/cmd/run/test_common.py` & `tox-4.5.0/tests/session/cmd/run/test_common.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/tox_env/test_api.py` & `tox-4.5.0/tests/tox_env/test_api.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/tox_env/test_register.py` & `tox-4.5.0/tests/tox_env/test_register.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/tox_env/test_tox_env_api.py` & `tox-4.5.0/tests/tox_env/test_tox_env_api.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/tox_env/test_tox_env_runner.py` & `tox-4.5.0/tests/tox_env/test_tox_env_runner.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/tox_env/python/test_python_api.py` & `tox-4.5.0/tests/tox_env/python/test_python_api.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/tox_env/python/test_python_runner.py` & `tox-4.5.0/tests/tox_env/python/test_python_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,24 @@
             "type": "dir",
         },
     }
 
 
 def test_package_temp_dir_view(tox_project: ToxProjectCreator, demo_pkg_inline: Path) -> None:
     project = tox_project({"tox.ini": "[testenv]\npackage=wheel"})
-    result = project.run("r", "-vv", "-e", "py", "--root", str(demo_pkg_inline))
+    result = project.run(
+        "r",
+        "-vv",
+        "-e",
+        "py",
+        "--root",
+        str(demo_pkg_inline),
+        "--workdir",
+        str(project.path / ".tox"),
+    )
     result.assert_success()
     wheel_name = "demo_pkg_inline-1.0.0-py3-none-any.whl"
     session_path = Path(".tmp") / "package" / "1" / wheel_name
     msg = f" D package {session_path} links to {Path('.pkg') / 'dist'/ wheel_name} ({project.path/ '.tox'}) "
     assert msg in result.out
     assert f" D delete package {project.path / '.tox' / session_path}" in result.out
```

### Comparing `tox-4.4.9/tests/tox_env/python/pip/test_pip_install.py` & `tox-4.5.0/tests/tox_env/python/pip/test_pip_install.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/tox_env/python/pip/test_req_file.py` & `tox-4.5.0/tests/tox_env/python/pip/test_req_file.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/tox_env/python/pip/req/test_file.py` & `tox-4.5.0/tests/tox_env/python/pip/req/test_file.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/tox_env/python/virtual_env/test_setuptools.py` & `tox-4.5.0/tests/tox_env/python/virtual_env/test_setuptools.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/tox_env/python/virtual_env/test_virtualenv_api.py` & `tox-4.5.0/tests/tox_env/python/virtual_env/test_virtualenv_api.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/tox_env/python/virtual_env/package/conftest.py` & `tox-4.5.0/tests/tox_env/python/virtual_env/package/conftest.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/tox_env/python/virtual_env/package/test_package_cmd_builder.py` & `tox-4.5.0/tests/tox_env/python/virtual_env/package/test_package_cmd_builder.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/tox_env/python/virtual_env/package/test_package_pyproject.py` & `tox-4.5.0/tests/tox_env/python/virtual_env/package/test_package_pyproject.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/tox_env/python/virtual_env/package/test_python_package_util.py` & `tox-4.5.0/tests/tox_env/python/virtual_env/package/test_python_package_util.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/util/test_ci.py` & `tox-4.5.0/tests/util/test_ci.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/util/test_graph.py` & `tox-4.5.0/tests/util/test_graph.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/tests/util/test_spinner.py` & `tox-4.5.0/tests/util/test_spinner.py`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/LICENSE` & `tox-4.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/README.md` & `tox-4.5.0/README.md`

 * *Files identical despite different names*

### Comparing `tox-4.4.9/pyproject.toml` & `tox-4.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = [
   "hatch-vcs>=0.3",
-  "hatchling>=1.13",
+  "hatchling>=1.14",
 ]
 
 [project]
 name = "tox"
 description = "tox is a generic virtualenv management and test command line tool"
 readme.content-type = "text/markdown"
 readme.file = "README.md"
@@ -47,45 +47,45 @@
 dynamic = [
   "version",
 ]
 dependencies = [
   "cachetools>=5.3",
   "chardet>=5.1",
   "colorama>=0.4.6",
-  "filelock>=3.10",
-  'importlib-metadata>=6.1; python_version < "3.8"',
-  "packaging>=23",
-  "platformdirs>=3.1.1",
+  "filelock>=3.11",
+  'importlib-metadata>=6.4.1; python_version < "3.8"',
+  "packaging>=23.1",
+  "platformdirs>=3.2",
   "pluggy>=1",
   "pyproject-api>=1.5.1",
   'tomli>=2.0.1; python_version < "3.11"',
   'typing-extensions>=4.5; python_version < "3.8"',
   "virtualenv>=20.21",
 ]
 optional-dependencies.docs = [
-  "furo>=2022.12.7",
+  "furo>=2023.3.27",
   "sphinx>=6.1.3",
   "sphinx-argparse-cli>=1.11",
-  "sphinx-autodoc-typehints!=1.23.4,>=1.22",
-  "sphinx-copybutton>=0.5.1",
+  "sphinx-autodoc-typehints!=1.23.4,>=1.23",
+  "sphinx-copybutton>=0.5.2",
   "sphinx-inline-tabs>=2022.1.2b11",
   "sphinxcontrib-towncrier>=0.2.1a0",
   "towncrier>=22.12",
 ]
 optional-dependencies.testing = [
   "build[virtualenv]>=0.10",
   "covdefaults>=2.3",
   "devpi-process>=0.3",
   "diff-cover>=7.5",
   "distlib>=0.3.6",
   "flaky>=3.7",
   "hatch-vcs>=0.3",
-  "hatchling>=1.13",
+  "hatchling>=1.14",
   "psutil>=5.9.4",
-  "pytest>=7.2.2",
+  "pytest>=7.3.1",
   "pytest-cov>=4",
   "pytest-mock>=3.10",
   "pytest-xdist>=3.2.1",
   "re-assert>=1.1",
   'time-machine>=2.9; implementation_name != "pypy"',
   "wheel>=0.40",
 ]
```

### Comparing `tox-4.4.9/PKG-INFO` & `tox-4.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tox
-Version: 4.4.9
+Version: 4.5.0
 Summary: tox is a generic virtualenv management and test command line tool
 Project-URL: Documentation, https://tox.wiki
 Project-URL: Homepage, http://tox.readthedocs.org
 Project-URL: Release Notes, https://tox.wiki/en/latest/changelog.html
 Project-URL: Source, https://github.com/tox-dev/tox
 Project-URL: Tracker, https://github.com/tox-dev/tox/issues
 Author-email: Bernát Gábor <gaborjbernat@gmail.com>
@@ -29,46 +29,46 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Requires-Dist: cachetools>=5.3
 Requires-Dist: chardet>=5.1
 Requires-Dist: colorama>=0.4.6
-Requires-Dist: filelock>=3.10
-Requires-Dist: importlib-metadata>=6.1; python_version < '3.8'
-Requires-Dist: packaging>=23
-Requires-Dist: platformdirs>=3.1.1
+Requires-Dist: filelock>=3.11
+Requires-Dist: importlib-metadata>=6.4.1; python_version < '3.8'
+Requires-Dist: packaging>=23.1
+Requires-Dist: platformdirs>=3.2
 Requires-Dist: pluggy>=1
 Requires-Dist: pyproject-api>=1.5.1
 Requires-Dist: tomli>=2.0.1; python_version < '3.11'
 Requires-Dist: typing-extensions>=4.5; python_version < '3.8'
 Requires-Dist: virtualenv>=20.21
 Provides-Extra: docs
-Requires-Dist: furo>=2022.12.7; extra == 'docs'
+Requires-Dist: furo>=2023.3.27; extra == 'docs'
 Requires-Dist: sphinx-argparse-cli>=1.11; extra == 'docs'
-Requires-Dist: sphinx-autodoc-typehints!=1.23.4,>=1.22; extra == 'docs'
-Requires-Dist: sphinx-copybutton>=0.5.1; extra == 'docs'
+Requires-Dist: sphinx-autodoc-typehints!=1.23.4,>=1.23; extra == 'docs'
+Requires-Dist: sphinx-copybutton>=0.5.2; extra == 'docs'
 Requires-Dist: sphinx-inline-tabs>=2022.1.2b11; extra == 'docs'
 Requires-Dist: sphinx>=6.1.3; extra == 'docs'
 Requires-Dist: sphinxcontrib-towncrier>=0.2.1a0; extra == 'docs'
 Requires-Dist: towncrier>=22.12; extra == 'docs'
 Provides-Extra: testing
 Requires-Dist: build[virtualenv]>=0.10; extra == 'testing'
 Requires-Dist: covdefaults>=2.3; extra == 'testing'
 Requires-Dist: devpi-process>=0.3; extra == 'testing'
 Requires-Dist: diff-cover>=7.5; extra == 'testing'
 Requires-Dist: distlib>=0.3.6; extra == 'testing'
 Requires-Dist: flaky>=3.7; extra == 'testing'
 Requires-Dist: hatch-vcs>=0.3; extra == 'testing'
-Requires-Dist: hatchling>=1.13; extra == 'testing'
+Requires-Dist: hatchling>=1.14; extra == 'testing'
 Requires-Dist: psutil>=5.9.4; extra == 'testing'
 Requires-Dist: pytest-cov>=4; extra == 'testing'
 Requires-Dist: pytest-mock>=3.10; extra == 'testing'
 Requires-Dist: pytest-xdist>=3.2.1; extra == 'testing'
-Requires-Dist: pytest>=7.2.2; extra == 'testing'
+Requires-Dist: pytest>=7.3.1; extra == 'testing'
 Requires-Dist: re-assert>=1.1; extra == 'testing'
 Requires-Dist: time-machine>=2.9; implementation_name != 'pypy' and extra == 'testing'
 Requires-Dist: wheel>=0.40; extra == 'testing'
 Description-Content-Type: text/markdown
 
 # tox
```

