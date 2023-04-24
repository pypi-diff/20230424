# Comparing `tmp/snowflake_cli_labs-0.2.7.tar.gz` & `tmp/snowflake_cli_labs-0.2.8.tar.gz`

## Comparing `snowflake_cli_labs-0.2.7.tar` & `snowflake_cli_labs-0.2.8.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/LEGAL.md
--rw-r--r--   0        0        0    11607 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/README.md
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/requirements-dev.txt
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/requirements.txt
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/snowcli.spec
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/tox.ini
--rw-r--r--   0        0        0    13022 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/docs/images/coverage_1.png
--rw-r--r--   0        0        0    24318 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/docs/images/coverage_2.png
--rw-r--r--   0        0        0    12852 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/docs/images/coverage_3.png
--rw-r--r--   0        0        0    24441 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/docs/images/coverage_4.png
--rw-r--r--   0        0        0    14955 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/docs/images/coverage_5.png
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/__init__.py
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/config.py
--rw-r--r--   0        0        0    16558 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/snow_connector.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/snowsql_config.py
--rw-r--r--   0        0        0    21579 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/utils.py
--rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/cli/__init__.py
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/cli/connection.py
--rw-r--r--   0        0        0     6362 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/cli/function.py
--rw-r--r--   0        0        0     5199 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/cli/package.py
--rw-r--r--   0        0        0     7118 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/cli/procedure.py
--rw-r--r--   0        0        0     4537 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/cli/render.py
--rw-r--r--   0        0        0    20029 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/cli/snowpark_shared.py
--rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/cli/sql.py
--rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/cli/stage.py
--rw-r--r--   0        0        0    10105 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/cli/streamlit.py
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/cli/warehouse.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/cli/procedure_coverage/__init__.py
--rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/cli/procedure_coverage/clear.py
--rw-r--r--   0        0        0     5797 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/cli/procedure_coverage/report.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/python_templates/environment.yml.jinja
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/python_templates/snowpark_coverage.py.jinja
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/python_templates/streamlit_app_launcher.py.jinja
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/call_procedure.sql
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/create_function.sql
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/create_procedure.sql
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/create_stage.sql
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/create_streamlit.sql
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/describe_function.sql
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/describe_procedure.sql
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/describe_streamlit.sql
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/drop_function.sql
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/drop_procedure.sql
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/drop_stage.sql
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/drop_streamlit.sql
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/execute_function.sql
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/get_stage.sql
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/get_streamlit_url.sql
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/list_functions.sql
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/list_procedures.sql
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/list_stage.sql
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/list_stages.sql
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/list_streamlits.sql
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/put_stage.sql
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/remove_from_stage.sql
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/set_procedure_comment.sql
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/share_streamlit.sql
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/snowcli/sql/show_warehouses.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/templates/__init__.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/templates/default_function/.gitignore
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/templates/default_function/app.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/templates/default_function/app.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/templates/default_function/requirements.txt
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/templates/default_procedure/.gitignore
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/templates/default_procedure/app.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/templates/default_procedure/app.toml
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/templates/default_procedure/local_connection.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/src/templates/default_procedure/requirements.txt
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/tests/conftest.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/tests/test_main.py
--rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/tests/test_render.py
--rw-r--r--   0        0        0    14849 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/tests/test_snow_connector.py
--rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/tests/test_sql.py
--rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/tests/__snapshots__/test_snow_connector.ambr
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/LICENSE
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/pyproject.toml
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/LEGAL.md
+-rw-r--r--   0        0        0    11607 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/README.md
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/requirements-dev.txt
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/requirements.txt
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/snowcli.spec
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/tox.ini
+-rw-r--r--   0        0        0    13022 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/docs/images/coverage_1.png
+-rw-r--r--   0        0        0    24318 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/docs/images/coverage_2.png
+-rw-r--r--   0        0        0    12852 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/docs/images/coverage_3.png
+-rw-r--r--   0        0        0    24441 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/docs/images/coverage_4.png
+-rw-r--r--   0        0        0    14955 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/docs/images/coverage_5.png
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/__init__.py
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/config.py
+-rw-r--r--   0        0        0    16558 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/snow_connector.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/snowsql_config.py
+-rw-r--r--   0        0        0    21769 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/utils.py
+-rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/cli/__init__.py
+-rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/cli/connection.py
+-rw-r--r--   0        0        0     6362 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/cli/function.py
+-rw-r--r--   0        0        0     5199 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/cli/package.py
+-rw-r--r--   0        0        0     7118 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/cli/procedure.py
+-rw-r--r--   0        0        0     4537 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/cli/render.py
+-rw-r--r--   0        0        0    20029 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/cli/snowpark_shared.py
+-rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/cli/sql.py
+-rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/cli/stage.py
+-rw-r--r--   0        0        0    10105 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/cli/streamlit.py
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/cli/warehouse.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/cli/procedure_coverage/__init__.py
+-rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/cli/procedure_coverage/clear.py
+-rw-r--r--   0        0        0     5797 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/cli/procedure_coverage/report.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/python_templates/environment.yml.jinja
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/python_templates/snowpark_coverage.py.jinja
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/python_templates/streamlit_app_launcher.py.jinja
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/call_procedure.sql
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/create_function.sql
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/create_procedure.sql
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/create_stage.sql
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/create_streamlit.sql
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/describe_function.sql
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/describe_procedure.sql
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/describe_streamlit.sql
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/drop_function.sql
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/drop_procedure.sql
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/drop_stage.sql
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/drop_streamlit.sql
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/execute_function.sql
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/get_stage.sql
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/get_streamlit_url.sql
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/list_functions.sql
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/list_procedures.sql
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/list_stage.sql
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/list_stages.sql
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/list_streamlits.sql
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/put_stage.sql
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/remove_from_stage.sql
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/set_procedure_comment.sql
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/share_streamlit.sql
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/show_warehouses.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/templates/__init__.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/templates/default_function/.gitignore
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/templates/default_function/app.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/templates/default_function/app.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/templates/default_function/requirements.txt
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/templates/default_procedure/.gitignore
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/templates/default_procedure/app.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/templates/default_procedure/app.toml
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/templates/default_procedure/local_connection.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/templates/default_procedure/requirements.txt
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/tests/conftest.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/tests/test_main.py
+-rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/tests/test_render.py
+-rw-r--r--   0        0        0    14849 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/tests/test_snow_connector.py
+-rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/tests/test_sql.py
+-rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/tests/__snapshots__/test_snow_connector.ambr
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/LICENSE
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/PKG-INFO
```

### Comparing `snowflake_cli_labs-0.2.7/.pre-commit-config.yaml` & `snowflake_cli_labs-0.2.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.7/README.md` & `snowflake_cli_labs-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.7/snowcli.spec` & `snowflake_cli_labs-0.2.8/snowcli.spec`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.7/docs/images/coverage_1.png` & `snowflake_cli_labs-0.2.8/docs/images/coverage_1.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.7/docs/images/coverage_2.png` & `snowflake_cli_labs-0.2.8/docs/images/coverage_2.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.7/docs/images/coverage_3.png` & `snowflake_cli_labs-0.2.8/docs/images/coverage_3.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.7/docs/images/coverage_4.png` & `snowflake_cli_labs-0.2.8/docs/images/coverage_4.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.7/docs/images/coverage_5.png` & `snowflake_cli_labs-0.2.8/docs/images/coverage_5.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.7/src/snowcli/config.py` & `snowflake_cli_labs-0.2.8/src/snowcli/config.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.7/src/snowcli/snow_connector.py` & `snowflake_cli_labs-0.2.8/src/snowcli/snow_connector.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.7/src/snowcli/snowsql_config.py` & `snowflake_cli_labs-0.2.8/src/snowcli/snowsql_config.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.7/src/snowcli/utils.py` & `snowflake_cli_labs-0.2.8/src/snowcli/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -419,46 +419,48 @@
         if (
             not str(file).startswith(".")
             and not file.match(f"{pack_dir}/*")
             and not file.match(dest_zip)
         ):
             zipf.write(os.path.relpath(file))
 
-    for dir_path in os.getenv("SNOWCLI_INCLUDE_PATHS", "").split(":"):
-        directory = pathlib.Path(dir_path)
-        if directory.is_dir():
-            for file in pathlib.Path(directory).glob("**/*"):
-                if (
-                    not str(file).startswith(".")
-                    and not file.match("*.pyc")
-                    and not file.match("*__pycache__*")
-                ):
-                    zipf.write(file, arcname=os.path.relpath(file, directory))
+    if os.getenv("SNOWCLI_INCLUDE_PATHS") is not None:
+        for dir_path in os.getenv("SNOWCLI_INCLUDE_PATHS", "").split(":"):
+            directory = pathlib.Path(dir_path)
+            if directory.is_dir():
+                for file in pathlib.Path(directory).glob("**/*"):
+                    if (
+                        not str(file).startswith(".")
+                        and not file.match("*.pyc")
+                        and not file.match("*__pycache__*")
+                    ):
+                        zipf.write(file, arcname=os.path.relpath(file, directory))
 
     # close the zip file object
     zipf.close()
     return True
 
 
 def standardZipDir(dest_zip: str) -> bool:
     zipf = zipfile.ZipFile(dest_zip, "w", zipfile.ZIP_DEFLATED, allowZip64=True)
     for file in pathlib.Path(".").glob("*"):
         if not file.match(".*"):
             zipf.write(os.path.relpath(file))
 
-    for dir_path in os.getenv("SNOWCLI_INCLUDE_PATHS", "").split(":"):
-        directory = pathlib.Path(dir_path)
-        if directory.is_dir():
-            for file in pathlib.Path(directory).glob("**/*"):
-                if (
-                    not str(file).startswith(".")
-                    and not file.match("*.pyc")
-                    and not file.match("*__pycache__*")
-                ):
-                    zipf.write(file, arcname=os.path.relpath(file, directory))
+    if os.getenv("SNOWCLI_INCLUDE_PATHS") is not None:
+        for dir_path in os.getenv("SNOWCLI_INCLUDE_PATHS", "").split(":"):
+            directory = pathlib.Path(dir_path)
+            if directory.is_dir():
+                for file in pathlib.Path(directory).glob("**/*"):
+                    if (
+                        not str(file).startswith(".")
+                        and not file.match("*.pyc")
+                        and not file.match("*__pycache__*")
+                    ):
+                        zipf.write(file, arcname=os.path.relpath(file, directory))
 
     # close the zip file object
     zipf.close()
     return True
 
 
 def getSnowflakePackages() -> list[str]:
```

### Comparing `snowflake_cli_labs-0.2.7/src/snowcli/cli/__init__.py` & `snowflake_cli_labs-0.2.8/src/snowcli/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.7/src/snowcli/cli/connection.py` & `snowflake_cli_labs-0.2.8/src/snowcli/cli/connection.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.7/src/snowcli/cli/function.py` & `snowflake_cli_labs-0.2.8/src/snowcli/cli/function.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.7/src/snowcli/cli/package.py` & `snowflake_cli_labs-0.2.8/src/snowcli/cli/package.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.7/src/snowcli/cli/procedure.py` & `snowflake_cli_labs-0.2.8/src/snowcli/cli/procedure.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.7/src/snowcli/cli/render.py` & `snowflake_cli_labs-0.2.8/src/snowcli/cli/render.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.7/src/snowcli/cli/snowpark_shared.py` & `snowflake_cli_labs-0.2.8/src/snowcli/cli/snowpark_shared.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.7/src/snowcli/cli/sql.py` & `snowflake_cli_labs-0.2.8/src/snowcli/cli/sql.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.7/src/snowcli/cli/stage.py` & `snowflake_cli_labs-0.2.8/src/snowcli/cli/stage.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.7/src/snowcli/cli/streamlit.py` & `snowflake_cli_labs-0.2.8/src/snowcli/cli/streamlit.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.7/src/snowcli/cli/warehouse.py` & `snowflake_cli_labs-0.2.8/src/snowcli/cli/warehouse.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.7/src/snowcli/cli/procedure_coverage/clear.py` & `snowflake_cli_labs-0.2.8/src/snowcli/cli/procedure_coverage/clear.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.7/src/snowcli/cli/procedure_coverage/report.py` & `snowflake_cli_labs-0.2.8/src/snowcli/cli/procedure_coverage/report.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.7/src/snowcli/python_templates/snowpark_coverage.py.jinja` & `snowflake_cli_labs-0.2.8/src/snowcli/python_templates/snowpark_coverage.py.jinja`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.7/src/snowcli/python_templates/streamlit_app_launcher.py.jinja` & `snowflake_cli_labs-0.2.8/src/snowcli/python_templates/streamlit_app_launcher.py.jinja`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.7/src/snowcli/sql/create_procedure.sql` & `snowflake_cli_labs-0.2.8/src/snowcli/sql/create_procedure.sql`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.7/src/templates/default_procedure/app.py` & `snowflake_cli_labs-0.2.8/src/templates/default_procedure/app.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.7/src/templates/default_procedure/local_connection.py` & `snowflake_cli_labs-0.2.8/src/templates/default_procedure/local_connection.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.7/tests/test_render.py` & `snowflake_cli_labs-0.2.8/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.7/tests/test_snow_connector.py` & `snowflake_cli_labs-0.2.8/tests/test_snow_connector.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.7/tests/test_sql.py` & `snowflake_cli_labs-0.2.8/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.7/tests/__snapshots__/test_snow_connector.ambr` & `snowflake_cli_labs-0.2.8/tests/__snapshots__/test_snow_connector.ambr`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.7/LICENSE` & `snowflake_cli_labs-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.7/pyproject.toml` & `snowflake_cli_labs-0.2.8/pyproject.toml`

 * *Files identical despite different names*

